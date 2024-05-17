# Comparing `tmp/ourskyai_sda_api-1.3.3445.tar.gz` & `tmp/ourskyai_sda_api-1.3.3603.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_sda_api-1.3.3445.tar", max compression
+gzip compressed data, was "ourskyai_sda_api-1.3.3603.tar", max compression
```

## Comparing `ourskyai_sda_api-1.3.3445.tar` & `ourskyai_sda_api-1.3.3603.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     9896 2024-04-25 01:25:01.535316 ourskyai_sda_api-1.3.3445/README.md
--rw-r--r--   0        0        0     5092 2024-04-25 01:25:04.095331 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/__init__.py
--rw-r--r--   0        0        0      104 2024-04-25 01:25:04.127331 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/api/__init__.py
--rw-r--r--   0        0        0   213326 2024-04-25 01:25:04.215332 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/api/default_api.py
--rw-r--r--   0        0        0    30830 2024-04-25 01:25:04.271332 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/api_client.py
--rw-r--r--   0        0        0      852 2024-04-25 01:25:04.323333 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/api_response.py
--rw-r--r--   0        0        0    15175 2024-04-25 01:25:04.375333 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/configuration.py
--rw-r--r--   0        0        0     5923 2024-04-25 01:25:04.419333 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/exceptions.py
--rw-r--r--   0        0        0     4471 2024-04-25 01:25:04.475334 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/__init__.py
--rw-r--r--   0        0        0     3578 2024-04-25 01:25:04.519334 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/astrometric_offsets.py
--rw-r--r--   0        0        0     2394 2024-04-25 01:25:04.575334 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/empty_success.py
--rw-r--r--   0        0        0     1676 2024-04-25 01:25:04.627334 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/filter_type.py
--rw-r--r--   0        0        0     2645 2024-04-25 01:25:04.691335 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/location.py
--rw-r--r--   0        0        0     1237 2024-04-25 01:25:04.751335 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/mount_type.py
--rw-r--r--   0        0        0     2756 2024-04-25 01:25:04.795336 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/observation_bounding_box.py
--rw-r--r--   0        0        0     3713 2024-04-25 01:25:04.855336 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/observation_quality.py
--rw-r--r--   0        0        0     5767 2024-04-25 01:25:04.903336 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/observation_result.py
--rw-r--r--   0        0        0     1320 2024-04-25 01:25:04.955336 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/observation_state.py
--rw-r--r--   0        0        0     1529 2024-04-25 01:25:05.007337 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/orbit_type.py
--rw-r--r--   0        0        0     1361 2024-04-25 01:25:05.059337 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/satellite_target_tracking_status.py
--rw-r--r--   0        0        0     1241 2024-04-25 01:25:05.091337 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/shutter_type.py
--rw-r--r--   0        0        0     2382 2024-04-25 01:25:05.147338 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/successful_create.py
--rw-r--r--   0        0        0     1258 2024-04-25 01:25:05.199338 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/tracking_type.py
--rw-r--r--   0        0        0     2534 2024-04-25 01:25:05.259338 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2605 2024-04-25 01:25:05.315339 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     3169 2024-04-25 01:25:05.375339 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2609 2024-04-25 01:25:05.427339 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_organization_target_request.py
--rw-r--r--   0        0        0     2761 2024-04-25 01:25:05.471340 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_satellite_target_request.py
--rw-r--r--   0        0        0     3373 2024-04-25 01:25:05.511340 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_search_instruction_request.py
--rw-r--r--   0        0        0     3353 2024-04-25 01:25:05.555340 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_survey_instruction_request.py
--rw-r--r--   0        0        0     3017 2024-04-25 01:25:05.607340 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_get_satellite_targets_response.py
--rw-r--r--   0        0        0     4457 2024-04-25 01:25:05.651341 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3922 2024-04-25 01:25:05.695341 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5657 2024-04-25 01:25:05.755341 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     4459 2024-04-25 01:25:05.819342 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_observation_feature.py
--rw-r--r--   0        0        0     3748 2024-04-25 01:25:05.871342 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_observation_sequence_result.py
--rw-r--r--   0        0        0     4306 2024-04-25 01:25:05.923343 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py
--rw-r--r--   0        0        0     4637 2024-04-25 01:25:06.011343 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_observation_status.py
--rw-r--r--   0        0        0     3192 2024-04-25 01:25:06.055343 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_organization_target.py
--rw-r--r--   0        0        0     3226 2024-04-25 01:25:06.115344 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_satellite_potential.py
--rw-r--r--   0        0        0     3528 2024-04-25 01:25:06.167344 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_satellite_target.py
--rw-r--r--   0        0        0     3733 2024-04-25 01:25:06.223344 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_search_instruction.py
--rw-r--r--   0        0        0     3407 2024-04-25 01:25:06.283345 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_search_instruction_step.py
--rw-r--r--   0        0        0     3634 2024-04-25 01:25:06.339345 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_survey_instruction.py
--rw-r--r--   0        0        0     2799 2024-04-25 01:25:06.407345 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_survey_instruction_step.py
--rw-r--r--   0        0        0     2695 2024-04-25 01:25:06.487346 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_target_correlation.py
--rw-r--r--   0        0        0     3185 2024-04-25 01:25:06.535346 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_tdm.py
--rw-r--r--   0        0        0     2575 2024-04-25 01:25:06.639347 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_update_email_configuration_request.py
--rw-r--r--   0        0        0     2913 2024-04-25 01:25:06.731347 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_update_satellite_target_request.py
--rw-r--r--   0        0        0     3146 2024-04-25 01:25:06.823348 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py
--rw-r--r--   0        0        0     2963 2024-04-25 01:25:06.879348 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_webhook_configuration.py
--rw-r--r--   0        0        0     1350 2024-04-25 01:25:06.939349 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/webhook_auth_type.py
--rw-r--r--   0        0        0     1734 2024-04-25 01:25:06.979349 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/webhook_event.py
--rw-r--r--   0        0        0        0 2024-04-25 01:25:07.011349 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/py.typed
--rw-r--r--   0        0        0    13423 2024-04-25 01:25:07.071349 ourskyai_sda_api-1.3.3445/ourskyai_sda_api/rest.py
--rw-r--r--   0        0        0      731 2024-04-25 01:25:07.107350 ourskyai_sda_api-1.3.3445/pyproject.toml
--rw-r--r--   0        0        0    10858 1970-01-01 00:00:00.000000 ourskyai_sda_api-1.3.3445/PKG-INFO
+-rw-r--r--   0        0        0    10115 2024-05-17 19:15:26.271831 ourskyai_sda_api-1.3.3603/README.md
+-rw-r--r--   0        0        0     5163 2024-05-17 19:15:28.983932 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/__init__.py
+-rw-r--r--   0        0        0      104 2024-05-17 19:15:29.019934 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api/__init__.py
+-rw-r--r--   0        0        0   220784 2024-05-17 19:15:29.099937 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api/default_api.py
+-rw-r--r--   0        0        0    30830 2024-05-17 19:15:29.147939 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-17 19:15:29.187940 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api_response.py
+-rw-r--r--   0        0        0    15175 2024-05-17 19:15:29.267943 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/configuration.py
+-rw-r--r--   0        0        0     5923 2024-05-17 19:15:29.359947 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/exceptions.py
+-rw-r--r--   0        0        0     4542 2024-05-17 19:15:29.399948 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/__init__.py
+-rw-r--r--   0        0        0     4311 2024-05-17 19:15:29.435949 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/astrometric_offsets.py
+-rw-r--r--   0        0        0     2394 2024-05-17 19:15:29.479951 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/empty_success.py
+-rw-r--r--   0        0        0     1676 2024-05-17 19:15:29.531953 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/filter_type.py
+-rw-r--r--   0        0        0     2645 2024-05-17 19:15:29.595955 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/location.py
+-rw-r--r--   0        0        0     1237 2024-05-17 19:15:29.643957 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/mount_type.py
+-rw-r--r--   0        0        0     2756 2024-05-17 19:15:29.715960 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_bounding_box.py
+-rw-r--r--   0        0        0     3713 2024-05-17 19:15:29.775962 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_quality.py
+-rw-r--r--   0        0        0     6381 2024-05-17 19:15:29.835965 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_result.py
+-rw-r--r--   0        0        0     1320 2024-05-17 19:15:29.871966 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_state.py
+-rw-r--r--   0        0        0     1529 2024-05-17 19:15:29.923968 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/orbit_type.py
+-rw-r--r--   0        0        0     1361 2024-05-17 19:15:29.999971 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/satellite_target_tracking_status.py
+-rw-r--r--   0        0        0     1241 2024-05-17 19:15:30.079974 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/shutter_type.py
+-rw-r--r--   0        0        0     2382 2024-05-17 19:15:30.135976 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/successful_create.py
+-rw-r--r--   0        0        0     1258 2024-05-17 19:15:30.211979 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2534 2024-05-17 19:15:30.271981 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2605 2024-05-17 19:15:30.343984 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     3169 2024-05-17 19:15:30.407986 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2609 2024-05-17 19:15:30.479989 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_organization_target_request.py
+-rw-r--r--   0        0        0     2761 2024-05-17 19:15:30.535991 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_satellite_target_request.py
+-rw-r--r--   0        0        0     3373 2024-05-17 19:15:30.587993 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_search_instruction_request.py
+-rw-r--r--   0        0        0     3353 2024-05-17 19:15:30.639995 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_survey_instruction_request.py
+-rw-r--r--   0        0        0     3017 2024-05-17 19:15:30.691997 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_get_satellite_targets_response.py
+-rw-r--r--   0        0        0     4457 2024-05-17 19:15:30.723998 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3922 2024-05-17 19:15:30.768000 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5657 2024-05-17 19:15:30.808001 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     4676 2024-05-17 19:15:30.856003 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_feature.py
+-rw-r--r--   0        0        0     3748 2024-05-17 19:15:30.912005 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_sequence_result.py
+-rw-r--r--   0        0        0     4306 2024-05-17 19:15:30.968007 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py
+-rw-r--r--   0        0        0     4637 2024-05-17 19:15:31.016009 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_status.py
+-rw-r--r--   0        0        0     3192 2024-05-17 19:15:31.092012 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_organization_target.py
+-rw-r--r--   0        0        0     3644 2024-05-17 19:15:31.144014 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_satellite_potential.py
+-rw-r--r--   0        0        0     3528 2024-05-17 19:15:31.188015 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_satellite_target.py
+-rw-r--r--   0        0        0     3733 2024-05-17 19:15:31.312020 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_search_instruction.py
+-rw-r--r--   0        0        0     3407 2024-05-17 19:15:31.364022 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_search_instruction_step.py
+-rw-r--r--   0        0        0     3634 2024-05-17 19:15:31.408024 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_survey_instruction.py
+-rw-r--r--   0        0        0     2799 2024-05-17 19:15:31.460026 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_survey_instruction_step.py
+-rw-r--r--   0        0        0     2695 2024-05-17 19:15:31.536028 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_target_correlation.py
+-rw-r--r--   0        0        0     3185 2024-05-17 19:15:31.600031 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_tdm.py
+-rw-r--r--   0        0        0     2575 2024-05-17 19:15:31.656033 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_update_email_configuration_request.py
+-rw-r--r--   0        0        0     2913 2024-05-17 19:15:31.716035 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_update_satellite_target_request.py
+-rw-r--r--   0        0        0     3146 2024-05-17 19:15:31.772037 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py
+-rw-r--r--   0        0        0     2963 2024-05-17 19:15:31.832040 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_webhook_configuration.py
+-rw-r--r--   0        0        0     1386 2024-05-17 19:15:31.884042 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/weather_condition.py
+-rw-r--r--   0        0        0     1350 2024-05-17 19:15:31.920043 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/webhook_auth_type.py
+-rw-r--r--   0        0        0     1734 2024-05-17 19:15:31.956044 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/webhook_event.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:15:31.988046 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/py.typed
+-rw-r--r--   0        0        0    13423 2024-05-17 19:15:32.060048 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/rest.py
+-rw-r--r--   0        0        0      731 2024-05-17 19:15:32.104050 ourskyai_sda_api-1.3.3603/pyproject.toml
+-rw-r--r--   0        0        0    11077 1970-01-01 00:00:00.000000 ourskyai_sda_api-1.3.3603/PKG-INFO
```

### Comparing `ourskyai_sda_api-1.3.3445/README.md` & `ourskyai_sda_api-1.3.3603/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 The basic flow for a new organization is as follows:
 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe.
 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above.
 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3445
-- Package version: 1.3.3445
+- API version: 1.3.3603
+- Package version: 1.3.3603
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -102,14 +102,15 @@
 *DefaultApi* | [**v1_get_image_set_image**](docs/DefaultApi.md#v1_get_image_set_image) | **GET** /v1/image-set-image | 
 *DefaultApi* | [**v1_get_image_set_images**](docs/DefaultApi.md#v1_get_image_set_images) | **GET** /v1/image-set-images | 
 *DefaultApi* | [**v1_get_image_sets**](docs/DefaultApi.md#v1_get_image_sets) | **GET** /v1/image-sets | 
 *DefaultApi* | [**v1_get_node_properties**](docs/DefaultApi.md#v1_get_node_properties) | **GET** /v1/node-properties | 
 *DefaultApi* | [**v1_get_observation_features**](docs/DefaultApi.md#v1_get_observation_features) | **GET** /v1/observation-features | 
 *DefaultApi* | [**v1_get_observation_sequence_results**](docs/DefaultApi.md#v1_get_observation_sequence_results) | **GET** /v1/observation-sequence-results | 
 *DefaultApi* | [**v1_get_observation_statuses**](docs/DefaultApi.md#v1_get_observation_statuses) | **GET** /v1/observation-statuses | 
+*DefaultApi* | [**v1_get_organization_satellite_potentials**](docs/DefaultApi.md#v1_get_organization_satellite_potentials) | **GET** /v1/organization-target-potentials | 
 *DefaultApi* | [**v1_get_organization_targets**](docs/DefaultApi.md#v1_get_organization_targets) | **GET** /v1/organization-targets | 
 *DefaultApi* | [**v1_get_satellite_potentials**](docs/DefaultApi.md#v1_get_satellite_potentials) | **GET** /v1/satellite-target-potentials | 
 *DefaultApi* | [**v1_get_satellite_target**](docs/DefaultApi.md#v1_get_satellite_target) | **GET** /v1/satellite-target | 
 *DefaultApi* | [**v1_get_satellite_targets**](docs/DefaultApi.md#v1_get_satellite_targets) | **GET** /v1/satellite-targets | 
 *DefaultApi* | [**v1_get_search_instructions**](docs/DefaultApi.md#v1_get_search_instructions) | **GET** /v1/search-instructions | 
 *DefaultApi* | [**v1_get_survey_instructions**](docs/DefaultApi.md#v1_get_survey_instructions) | **GET** /v1/survey-instructions | 
 *DefaultApi* | [**v1_get_tdm**](docs/DefaultApi.md#v1_get_tdm) | **GET** /v1/tdm | 
@@ -159,14 +160,15 @@
  - [V1SurveyInstructionStep](docs/V1SurveyInstructionStep.md)
  - [V1TargetCorrelation](docs/V1TargetCorrelation.md)
  - [V1Tdm](docs/V1Tdm.md)
  - [V1UpdateEmailConfigurationRequest](docs/V1UpdateEmailConfigurationRequest.md)
  - [V1UpdateSatelliteTargetRequest](docs/V1UpdateSatelliteTargetRequest.md)
  - [V1UpdateWebhookConfigurationRequest](docs/V1UpdateWebhookConfigurationRequest.md)
  - [V1WebhookConfiguration](docs/V1WebhookConfiguration.md)
+ - [WeatherCondition](docs/WeatherCondition.md)
  - [WebhookAuthType](docs/WebhookAuthType.md)
  - [WebhookEvent](docs/WebhookEvent.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/__init__.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3445"
+__version__ = "1.3.3603"
 
 # import apis into sdk package
 from ourskyai_sda_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_sda_api.api_response import ApiResponse
 from ourskyai_sda_api.api_client import ApiClient
@@ -69,9 +69,10 @@
 from ourskyai_sda_api.models.v1_survey_instruction_step import V1SurveyInstructionStep
 from ourskyai_sda_api.models.v1_target_correlation import V1TargetCorrelation
 from ourskyai_sda_api.models.v1_tdm import V1Tdm
 from ourskyai_sda_api.models.v1_update_email_configuration_request import V1UpdateEmailConfigurationRequest
 from ourskyai_sda_api.models.v1_update_satellite_target_request import V1UpdateSatelliteTargetRequest
 from ourskyai_sda_api.models.v1_update_webhook_configuration_request import V1UpdateWebhookConfigurationRequest
 from ourskyai_sda_api.models.v1_webhook_configuration import V1WebhookConfiguration
+from ourskyai_sda_api.models.weather_condition import WeatherCondition
 from ourskyai_sda_api.models.webhook_auth_type import WebhookAuthType
 from ourskyai_sda_api.models.webhook_event import WebhookEvent
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/api/default_api.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api/default_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
@@ -17,15 +17,15 @@
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 
 from typing_extensions import Annotated
 from datetime import datetime
 
-from pydantic import Field, StrictStr, conlist
+from pydantic import Field, StrictBool, StrictStr, conlist
 
 from typing import List, Optional
 
 from ourskyai_sda_api.models.empty_success import EmptySuccess
 from ourskyai_sda_api.models.orbit_type import OrbitType
 from ourskyai_sda_api.models.successful_create import SuccessfulCreate
 from ourskyai_sda_api.models.v1_create_image_set_image_request import V1CreateImageSetImageRequest
@@ -3090,14 +3090,165 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def v1_get_organization_satellite_potentials(self, until : datetime, include_weather : Optional[StrictBool] = None, **kwargs) -> List[V1SatellitePotential]:  # noqa: E501
+        """v1_get_organization_satellite_potentials  # noqa: E501
+
+        Get potential observation windows for all satellites of your organization across the network from now until the `until` datetime  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_get_organization_satellite_potentials(until, include_weather, async_req=True)
+        >>> result = thread.get()
+
+        :param until: (required)
+        :type until: datetime
+        :param include_weather:
+        :type include_weather: bool
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: List[V1SatellitePotential]
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the v1_get_organization_satellite_potentials_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        return self.v1_get_organization_satellite_potentials_with_http_info(until, include_weather, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def v1_get_organization_satellite_potentials_with_http_info(self, until : datetime, include_weather : Optional[StrictBool] = None, **kwargs) -> ApiResponse:  # noqa: E501
+        """v1_get_organization_satellite_potentials  # noqa: E501
+
+        Get potential observation windows for all satellites of your organization across the network from now until the `until` datetime  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_get_organization_satellite_potentials_with_http_info(until, include_weather, async_req=True)
+        >>> result = thread.get()
+
+        :param until: (required)
+        :type until: datetime
+        :param include_weather:
+        :type include_weather: bool
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(List[V1SatellitePotential], status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'until',
+            'include_weather'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_get_organization_satellite_potentials" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('until') is not None:  # noqa: E501
+            if isinstance(_params['until'], datetime):
+                _query_params.append(('until', _params['until'].strftime(self.api_client.configuration.datetime_format)))
+            else:
+                _query_params.append(('until', _params['until']))
+
+        if _params.get('include_weather') is not None:  # noqa: E501
+            _query_params.append(('includeWeather', _params['include_weather']))
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['Roles', 'BearerToken']  # noqa: E501
+
+        _response_types_map = {
+            '200': "List[V1SatellitePotential]",
+        }
+
+        return self.api_client.call_api(
+            '/v1/organization-target-potentials', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def v1_get_organization_targets(self, **kwargs) -> List[V1OrganizationTarget]:  # noqa: E501
         """v1_get_organization_targets  # noqa: E501
 
         Get organization targets see the [create](#operation/v1CreateOrganizationTarget) endpoint for more details.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
@@ -3222,28 +3373,30 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def v1_get_satellite_potentials(self, satellite_target_id : StrictStr, until : datetime, **kwargs) -> List[V1SatellitePotential]:  # noqa: E501
+    def v1_get_satellite_potentials(self, satellite_target_id : StrictStr, until : datetime, include_weather : Optional[StrictBool] = None, **kwargs) -> List[V1SatellitePotential]:  # noqa: E501
         """v1_get_satellite_potentials  # noqa: E501
 
         Get potential observation windows for a satellite across the network from now until the `until` datetime  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1_get_satellite_potentials(satellite_target_id, until, async_req=True)
+        >>> thread = api.v1_get_satellite_potentials(satellite_target_id, until, include_weather, async_req=True)
         >>> result = thread.get()
 
         :param satellite_target_id: (required)
         :type satellite_target_id: str
         :param until: (required)
         :type until: datetime
+        :param include_weather:
+        :type include_weather: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
@@ -3251,31 +3404,33 @@
                  returns the request thread.
         :rtype: List[V1SatellitePotential]
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the v1_get_satellite_potentials_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return self.v1_get_satellite_potentials_with_http_info(satellite_target_id, until, **kwargs)  # noqa: E501
+        return self.v1_get_satellite_potentials_with_http_info(satellite_target_id, until, include_weather, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def v1_get_satellite_potentials_with_http_info(self, satellite_target_id : StrictStr, until : datetime, **kwargs) -> ApiResponse:  # noqa: E501
+    def v1_get_satellite_potentials_with_http_info(self, satellite_target_id : StrictStr, until : datetime, include_weather : Optional[StrictBool] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """v1_get_satellite_potentials  # noqa: E501
 
         Get potential observation windows for a satellite across the network from now until the `until` datetime  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.v1_get_satellite_potentials_with_http_info(satellite_target_id, until, async_req=True)
+        >>> thread = api.v1_get_satellite_potentials_with_http_info(satellite_target_id, until, include_weather, async_req=True)
         >>> result = thread.get()
 
         :param satellite_target_id: (required)
         :type satellite_target_id: str
         :param until: (required)
         :type until: datetime
+        :param include_weather:
+        :type include_weather: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -3297,15 +3452,16 @@
         :rtype: tuple(List[V1SatellitePotential], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'satellite_target_id',
-            'until'
+            'until',
+            'include_weather'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -3337,14 +3493,17 @@
 
         if _params.get('until') is not None:  # noqa: E501
             if isinstance(_params['until'], datetime):
                 _query_params.append(('until', _params['until'].strftime(self.api_client.configuration.datetime_format)))
             else:
                 _query_params.append(('until', _params['until']))
 
+        if _params.get('include_weather') is not None:  # noqa: E501
+            _query_params.append(('includeWeather', _params['include_weather']))
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/api_client.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.3445/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3603/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/api_response.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/configuration.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,16 +371,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.3445\n"\
-               "SDK Package Version: 1.3.3445".\
+               "Version of the API: 1.3.3603\n"\
+               "SDK Package Version: 1.3.3603".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/exceptions.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/__init__.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
@@ -52,9 +52,10 @@
 from ourskyai_sda_api.models.v1_survey_instruction_step import V1SurveyInstructionStep
 from ourskyai_sda_api.models.v1_target_correlation import V1TargetCorrelation
 from ourskyai_sda_api.models.v1_tdm import V1Tdm
 from ourskyai_sda_api.models.v1_update_email_configuration_request import V1UpdateEmailConfigurationRequest
 from ourskyai_sda_api.models.v1_update_satellite_target_request import V1UpdateSatelliteTargetRequest
 from ourskyai_sda_api.models.v1_update_webhook_configuration_request import V1UpdateWebhookConfigurationRequest
 from ourskyai_sda_api.models.v1_webhook_configuration import V1WebhookConfiguration
+from ourskyai_sda_api.models.weather_condition import WeatherCondition
 from ourskyai_sda_api.models.webhook_auth_type import WebhookAuthType
 from ourskyai_sda_api.models.webhook_event import WebhookEvent
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/astrometric_offsets.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/astrometric_offsets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -21,20 +21,20 @@
 from typing import Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
 class AstrometricOffsets(BaseModel):
     """
     astrometricOffsets  # noqa: E501
     """
-    ra_plate_solve_offset_average: Union[StrictFloat, StrictInt] = Field(..., alias="raPlateSolveOffsetAverage")
-    ra_plate_solve_offset_std_dev: Union[StrictFloat, StrictInt] = Field(..., alias="raPlateSolveOffsetStdDev")
-    dec_plate_solve_offset_average: Union[StrictFloat, StrictInt] = Field(..., alias="decPlateSolveOffsetAverage")
-    dec_plate_solve_offset_std_dev: Union[StrictFloat, StrictInt] = Field(..., alias="decPlateSolveOffsetStdDev")
-    fwhm_std_dev: Union[StrictFloat, StrictInt] = Field(..., alias="fwhmStdDev")
-    fwhm_average: Union[StrictFloat, StrictInt] = Field(..., alias="fwhmAverage")
+    ra_plate_solve_offset_average: Union[StrictFloat, StrictInt] = Field(..., alias="raPlateSolveOffsetAverage", description="the average offset from the star catalog (NOMAD or GAIA DR3) for right ascension in degrees in EME2000 frame")
+    ra_plate_solve_offset_std_dev: Union[StrictFloat, StrictInt] = Field(..., alias="raPlateSolveOffsetStdDev", description="the standard deviation of offset from the star catalog (NOMAD or GAIA DR3) for right ascension in degrees in EME2000 frame")
+    dec_plate_solve_offset_average: Union[StrictFloat, StrictInt] = Field(..., alias="decPlateSolveOffsetAverage", description="the average offset from the star catalog (NOMAD or GAIA DR3) for declination in degrees in EME2000 frame")
+    dec_plate_solve_offset_std_dev: Union[StrictFloat, StrictInt] = Field(..., alias="decPlateSolveOffsetStdDev", description="the standard deviation of offset from the star catalog (NOMAD or GAIA DR3) for declination in degrees in EME2000 frame")
+    fwhm_std_dev: Union[StrictFloat, StrictInt] = Field(..., alias="fwhmStdDev", description="The standard deviation of the full-width-half-max of all stars in the image measured in arcseconds")
+    fwhm_average: Union[StrictFloat, StrictInt] = Field(..., alias="fwhmAverage", description="The average of the full-width-half-max of all stars in the image measured in arcseconds")
     __properties = ["raPlateSolveOffsetAverage", "raPlateSolveOffsetStdDev", "decPlateSolveOffsetAverage", "decPlateSolveOffsetStdDev", "fwhmStdDev", "fwhmAverage"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/empty_success.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/empty_success.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/filter_type.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/filter_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/location.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/mount_type.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/mount_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/observation_bounding_box.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_bounding_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/observation_quality.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/observation_result.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_result.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -28,24 +28,25 @@
     """
     A single observation result. This is a 1:1 mapping with a single image  # noqa: E501
     """
     image_id: StrictStr = Field(..., alias="imageId")
     astrometric_offsets: AstrometricOffsets = Field(..., alias="astrometricOffsets")
     image_url: Optional[StrictStr] = Field(None, alias="imageUrl")
     jpg_url: Optional[StrictStr] = Field(None, alias="jpgUrl")
-    ra: Union[StrictFloat, StrictInt] = Field(...)
-    dec: Union[StrictFloat, StrictInt] = Field(...)
-    corrected_ra: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="correctedRa", description="The measured right ascension calibrated for stellar aberration in degrees")
-    corrected_dec: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="correctedDec", description="The measured declination calibrated for stellar aberration in degrees")
+    ra: Union[StrictFloat, StrictInt] = Field(..., description="The un-corrected apparent right ascension in degrees and EME2000 frame at the ground station")
+    dec: Union[StrictFloat, StrictInt] = Field(..., description="The un-corrected apparent declination in degrees and EME2000 frame at the ground station")
+    corrected_ra: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="correctedRa", description="The measured right ascension calibrated for stellar aberration in degrees and EME2000 frame")
+    corrected_dec: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="correctedDec", description="The measured declination calibrated for stellar aberration in degrees and EME2000 frame")
     bounding_box: Optional[ObservationBoundingBox] = Field(None, alias="boundingBox")
     timestamp: datetime = Field(...)
+    timing_accuracy: Union[StrictFloat, StrictInt] = Field(..., alias="timingAccuracy", description="Timestamps for this image are considered to be accurate to within +/- this value in seconds")
     apparent_magnitude: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="apparentMagnitude", description="BETA: the apparent magnitude of the target at the time of the observation")
-    distance_from_prediction: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="distanceFromPrediction")
+    distance_from_prediction: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="distanceFromPrediction", description="The distance from the predicted location in arcseconds (using SGP4 propagation)")
     features: Optional[conlist(V1ObservationFeature)] = None
-    __properties = ["imageId", "astrometricOffsets", "imageUrl", "jpgUrl", "ra", "dec", "correctedRa", "correctedDec", "boundingBox", "timestamp", "apparentMagnitude", "distanceFromPrediction", "features"]
+    __properties = ["imageId", "astrometricOffsets", "imageUrl", "jpgUrl", "ra", "dec", "correctedRa", "correctedDec", "boundingBox", "timestamp", "timingAccuracy", "apparentMagnitude", "distanceFromPrediction", "features"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -98,14 +99,15 @@
             "jpg_url": obj.get("jpgUrl"),
             "ra": obj.get("ra"),
             "dec": obj.get("dec"),
             "corrected_ra": obj.get("correctedRa"),
             "corrected_dec": obj.get("correctedDec"),
             "bounding_box": ObservationBoundingBox.from_dict(obj.get("boundingBox")) if obj.get("boundingBox") is not None else None,
             "timestamp": obj.get("timestamp"),
+            "timing_accuracy": obj.get("timingAccuracy"),
             "apparent_magnitude": obj.get("apparentMagnitude"),
             "distance_from_prediction": obj.get("distanceFromPrediction"),
             "features": [V1ObservationFeature.from_dict(_item) for _item in obj.get("features")] if obj.get("features") is not None else None
         })
         return _obj
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/observation_state.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/orbit_type.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/orbit_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/satellite_target_tracking_status.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/satellite_target_tracking_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/shutter_type.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/shutter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/successful_create.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/tracking_type.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/tracking_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_image_set_image_request.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_image_set_image_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_image_set_image_response.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_image_set_image_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_image_set_request.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_organization_target_request.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_organization_target_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_satellite_target_request.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_satellite_target_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_search_instruction_request.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_search_instruction_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_create_survey_instruction_request.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_survey_instruction_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_get_satellite_targets_response.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_get_satellite_targets_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_ground_station_participant.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_ground_station_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_image_set.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_image_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_image_set_image.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_observation_feature.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_feature.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -23,20 +23,20 @@
 from ourskyai_sda_api.models.observation_bounding_box import ObservationBoundingBox
 from ourskyai_sda_api.models.v1_target_correlation import V1TargetCorrelation
 
 class V1ObservationFeature(BaseModel):
     """
     Observation Feature  # noqa: E501
     """
-    ra: Union[StrictFloat, StrictInt] = Field(...)
-    dec: Union[StrictFloat, StrictInt] = Field(...)
+    ra: Union[StrictFloat, StrictInt] = Field(..., description="the right ascension in degrees in EME2000 frame")
+    dec: Union[StrictFloat, StrictInt] = Field(..., description="the declination in degrees in EME2000 frame")
     timestamp: datetime = Field(...)
     bounding_box: Optional[ObservationBoundingBox] = Field(None, alias="boundingBox")
     apparent_magnitude: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="apparentMagnitude", description="BETA: the apparent magnitude of the target at the time of the observation")
-    distance_from_prediction: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="distanceFromPrediction")
+    distance_from_prediction: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="distanceFromPrediction", description="The distance from the predicted location in arcseconds (using SGP4 propagation)")
     target_correlations: Optional[conlist(V1TargetCorrelation)] = Field(None, alias="targetCorrelations")
     __properties = ["ra", "dec", "timestamp", "boundingBox", "apparentMagnitude", "distanceFromPrediction", "targetCorrelations"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_observation_sequence_result.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_sequence_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_observation_status.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_organization_target.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_organization_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_satellite_potential.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_satellite_potential.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -17,25 +17,28 @@
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 from ourskyai_sda_api.models.orbit_type import OrbitType
+from ourskyai_sda_api.models.weather_condition import WeatherCondition
 
 class V1SatellitePotential(BaseModel):
     """
     SatellitePotential  # noqa: E501
     """
     first_observable_time: datetime = Field(..., alias="firstObservableTime")
     last_observable_time: datetime = Field(..., alias="lastObservableTime")
     satellite_target_id: Optional[StrictStr] = Field(None, alias="satelliteTargetId")
     norad_id: Optional[StrictStr] = Field(None, alias="noradId")
     orbit_type: Optional[OrbitType] = Field(None, alias="orbitType")
-    __properties = ["firstObservableTime", "lastObservableTime", "satelliteTargetId", "noradId", "orbitType"]
+    weather_condition: Optional[WeatherCondition] = Field(None, alias="weatherCondition")
+    weather_description: Optional[StrictStr] = Field(None, alias="weatherDescription")
+    __properties = ["firstObservableTime", "lastObservableTime", "satelliteTargetId", "noradId", "orbitType", "weatherCondition", "weatherDescription"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -69,12 +72,14 @@
             return V1SatellitePotential.parse_obj(obj)
 
         _obj = V1SatellitePotential.parse_obj({
             "first_observable_time": obj.get("firstObservableTime"),
             "last_observable_time": obj.get("lastObservableTime"),
             "satellite_target_id": obj.get("satelliteTargetId"),
             "norad_id": obj.get("noradId"),
-            "orbit_type": obj.get("orbitType")
+            "orbit_type": obj.get("orbitType"),
+            "weather_condition": obj.get("weatherCondition"),
+            "weather_description": obj.get("weatherDescription")
         })
         return _obj
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_satellite_target.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_satellite_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_search_instruction.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_search_instruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_search_instruction_step.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_search_instruction_step.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_survey_instruction.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_survey_instruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_survey_instruction_step.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_survey_instruction_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_target_correlation.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_target_correlation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_tdm.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_tdm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_update_email_configuration_request.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_update_email_configuration_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_update_satellite_target_request.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_update_satellite_target_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/v1_webhook_configuration.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_webhook_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/webhook_auth_type.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/webhook_auth_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/models/webhook_event.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/webhook_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3445/ourskyai_sda_api/rest.py` & `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_sda_api-1.3.3445/pyproject.toml` & `ourskyai_sda_api-1.3.3603/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_sda_api"
-version = "1.3.3445"
+version = "1.3.3603"
 description = "OurSky SDA"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky SDA"]
 include = ["ourskyai_sda_api/py.typed"]
```

### Comparing `ourskyai_sda_api-1.3.3445/PKG-INFO` & `ourskyai_sda_api-1.3.3603/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_sda_api
-Version: 1.3.3445
+Version: 1.3.3603
 Summary: OurSky SDA
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky SDA
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -27,16 +27,16 @@
 The basic flow for a new organization is as follows:
 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe.
 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above.
 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3445
-- Package version: 1.3.3445
+- API version: 1.3.3603
+- Package version: 1.3.3603
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -127,14 +127,15 @@
 *DefaultApi* | [**v1_get_image_set_image**](docs/DefaultApi.md#v1_get_image_set_image) | **GET** /v1/image-set-image | 
 *DefaultApi* | [**v1_get_image_set_images**](docs/DefaultApi.md#v1_get_image_set_images) | **GET** /v1/image-set-images | 
 *DefaultApi* | [**v1_get_image_sets**](docs/DefaultApi.md#v1_get_image_sets) | **GET** /v1/image-sets | 
 *DefaultApi* | [**v1_get_node_properties**](docs/DefaultApi.md#v1_get_node_properties) | **GET** /v1/node-properties | 
 *DefaultApi* | [**v1_get_observation_features**](docs/DefaultApi.md#v1_get_observation_features) | **GET** /v1/observation-features | 
 *DefaultApi* | [**v1_get_observation_sequence_results**](docs/DefaultApi.md#v1_get_observation_sequence_results) | **GET** /v1/observation-sequence-results | 
 *DefaultApi* | [**v1_get_observation_statuses**](docs/DefaultApi.md#v1_get_observation_statuses) | **GET** /v1/observation-statuses | 
+*DefaultApi* | [**v1_get_organization_satellite_potentials**](docs/DefaultApi.md#v1_get_organization_satellite_potentials) | **GET** /v1/organization-target-potentials | 
 *DefaultApi* | [**v1_get_organization_targets**](docs/DefaultApi.md#v1_get_organization_targets) | **GET** /v1/organization-targets | 
 *DefaultApi* | [**v1_get_satellite_potentials**](docs/DefaultApi.md#v1_get_satellite_potentials) | **GET** /v1/satellite-target-potentials | 
 *DefaultApi* | [**v1_get_satellite_target**](docs/DefaultApi.md#v1_get_satellite_target) | **GET** /v1/satellite-target | 
 *DefaultApi* | [**v1_get_satellite_targets**](docs/DefaultApi.md#v1_get_satellite_targets) | **GET** /v1/satellite-targets | 
 *DefaultApi* | [**v1_get_search_instructions**](docs/DefaultApi.md#v1_get_search_instructions) | **GET** /v1/search-instructions | 
 *DefaultApi* | [**v1_get_survey_instructions**](docs/DefaultApi.md#v1_get_survey_instructions) | **GET** /v1/survey-instructions | 
 *DefaultApi* | [**v1_get_tdm**](docs/DefaultApi.md#v1_get_tdm) | **GET** /v1/tdm | 
@@ -184,14 +185,15 @@
  - [V1SurveyInstructionStep](docs/V1SurveyInstructionStep.md)
  - [V1TargetCorrelation](docs/V1TargetCorrelation.md)
  - [V1Tdm](docs/V1Tdm.md)
  - [V1UpdateEmailConfigurationRequest](docs/V1UpdateEmailConfigurationRequest.md)
  - [V1UpdateSatelliteTargetRequest](docs/V1UpdateSatelliteTargetRequest.md)
  - [V1UpdateWebhookConfigurationRequest](docs/V1UpdateWebhookConfigurationRequest.md)
  - [V1WebhookConfiguration](docs/V1WebhookConfiguration.md)
+ - [WeatherCondition](docs/WeatherCondition.md)
  - [WebhookAuthType](docs/WebhookAuthType.md)
  - [WebhookEvent](docs/WebhookEvent.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
```

