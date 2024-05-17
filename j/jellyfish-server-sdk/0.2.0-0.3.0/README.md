# Comparing `tmp/jellyfish_server_sdk-0.2.0.tar.gz` & `tmp/jellyfish_server_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jellyfish_server_sdk-0.2.0.tar", max compression
+gzip compressed data, was "jellyfish_server_sdk-0.3.0.tar", max compression
```

## Comparing `jellyfish_server_sdk-0.2.0.tar` & `jellyfish_server_sdk-0.3.0.tar`

### file list

```diff
@@ -1,67 +1,85 @@
--rw-r--r--   0        0        0     4160 2024-01-09 15:27:10.456345 jellyfish_server_sdk-0.2.0/README.md
--rw-r--r--   0        0        0     1420 2023-12-29 10:39:38.195924 jellyfish_server_sdk-0.2.0/jellyfish/__init__.py
--rw-r--r--   0        0        0      166 2023-12-28 13:15:33.045860 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/__init__.py
--rw-r--r--   0        0        0       47 2023-12-28 13:15:33.046000 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-12-28 13:15:33.046076 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/hls/__init__.py
--rw-r--r--   0        0        0     7598 2023-12-28 13:15:33.046241 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/hls/get_hls_content.py
--rw-r--r--   0        0        0     4773 2023-12-28 13:15:33.046345 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/hls/subscribe_hls_to.py
--rw-r--r--   0        0        0        0 2023-12-28 13:15:33.046415 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/recording/__init__.py
--rw-r--r--   0        0        0     4025 2023-12-28 13:15:33.046560 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/recording/delete_recording.py
--rw-r--r--   0        0        0     4414 2023-12-28 13:15:33.046682 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/recording/get_recording_content.py
--rw-r--r--   0        0        0     3688 2023-12-28 13:15:33.046782 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/recording/get_recordings.py
--rw-r--r--   0        0        0        0 2023-12-28 13:15:33.046868 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/__init__.py
--rw-r--r--   0        0        0     5098 2023-12-28 13:15:33.046987 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/add_component.py
--rw-r--r--   0        0        0     4985 2023-12-28 13:15:33.047084 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/add_peer.py
--rw-r--r--   0        0        0     4461 2023-12-28 13:15:33.047183 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/create_room.py
--rw-r--r--   0        0        0     4208 2023-12-28 13:15:33.047283 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/delete_component.py
--rw-r--r--   0        0        0     4111 2023-12-28 13:15:33.047387 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/delete_peer.py
--rw-r--r--   0        0        0     3897 2023-12-28 13:15:33.047454 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/delete_room.py
--rw-r--r--   0        0        0     3681 2023-12-28 13:15:33.047522 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/get_all_rooms.py
--rw-r--r--   0        0        0     4204 2023-12-28 13:15:33.047619 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/get_room.py
--rw-r--r--   0        0        0    12209 2023-12-28 13:15:33.047768 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/client.py
--rw-r--r--   0        0        0      470 2023-12-28 13:15:33.047839 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/errors.py
--rw-r--r--   0        0        0     2469 2023-12-29 10:39:38.196089 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/__init__.py
--rw-r--r--   0        0        0     4127 2023-12-28 13:15:33.048052 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/add_component_json_body.py
--rw-r--r--   0        0        0     1930 2023-12-28 13:15:33.048132 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/add_peer_json_body.py
--rw-r--r--   0        0        0     3322 2023-12-28 13:15:33.048210 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_details_response.py
--rw-r--r--   0        0        0     2558 2023-12-29 10:39:38.196247 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_file.py
--rw-r--r--   0        0        0     2136 2023-12-28 13:15:33.048367 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_hls.py
--rw-r--r--   0        0        0     1675 2023-12-28 13:15:33.048443 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_options_file.py
--rw-r--r--   0        0        0     4192 2023-12-28 13:15:33.048548 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_options_hls.py
--rw-r--r--   0        0        0      268 2023-12-28 13:15:33.048619 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_options_hls_subscribe_mode.py
--rw-r--r--   0        0        0     3151 2023-12-28 13:15:33.048693 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_options_rtsp.py
--rw-r--r--   0        0        0     1693 2023-12-29 10:39:38.196343 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_properties_file.py
--rw-r--r--   0        0        0     2951 2023-12-28 13:15:33.048779 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_properties_hls.py
--rw-r--r--   0        0        0      270 2023-12-28 13:15:33.048842 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_properties_hls_subscribe_mode.py
--rw-r--r--   0        0        0     3170 2023-12-29 10:39:38.196453 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_properties_rtsp.py
--rw-r--r--   0        0        0     2149 2023-12-28 13:15:33.049006 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_rtsp.py
--rw-r--r--   0        0        0     1486 2023-12-28 13:15:33.049076 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/error.py
--rw-r--r--   0        0        0     1849 2023-12-28 13:15:33.049150 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/peer.py
--rw-r--r--   0        0        0     1825 2023-12-28 13:15:33.049226 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/peer_details_response.py
--rw-r--r--   0        0        0     1887 2023-12-28 13:15:33.049301 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/peer_details_response_data.py
--rw-r--r--   0        0        0     1770 2023-12-28 13:15:33.049384 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/peer_options_web_rtc.py
--rw-r--r--   0        0        0      218 2023-12-28 13:15:33.049471 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/peer_status.py
--rw-r--r--   0        0        0     1602 2023-12-28 13:15:33.049541 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/recording_list_response.py
--rw-r--r--   0        0        0     4744 2023-12-28 13:15:33.049633 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/room.py
--rw-r--r--   0        0        0     3172 2023-12-28 13:15:33.049705 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/room_config.py
--rw-r--r--   0        0        0      217 2023-12-28 13:15:33.049774 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/room_config_video_codec.py
--rw-r--r--   0        0        0     1905 2023-12-28 13:15:33.049837 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/room_create_details_response.py
--rw-r--r--   0        0        0     2172 2023-12-28 13:15:33.049910 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/room_create_details_response_data.py
--rw-r--r--   0        0        0     1718 2023-12-28 13:15:33.049975 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/room_details_response.py
--rw-r--r--   0        0        0     1949 2023-12-28 13:15:33.050043 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/rooms_listing_response.py
--rw-r--r--   0        0        0     2448 2023-12-28 13:15:33.050128 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/s3_credentials.py
--rw-r--r--   0        0        0     1842 2023-12-28 13:15:33.050205 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/subscription_config.py
--rw-r--r--   0        0        0       25 2023-12-28 13:15:33.050267 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/py.typed
--rw-r--r--   0        0        0     1001 2023-12-28 13:15:33.050337 jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/types.py
--rw-r--r--   0        0        0      640 2023-12-28 13:15:33.050424 jellyfish_server_sdk-0.2.0/jellyfish/_webhook_notifier.py
--rw-r--r--   0        0        0     5020 2023-12-28 13:15:33.050661 jellyfish_server_sdk-0.2.0/jellyfish/_ws_notifier.py
--rw-r--r--   0        0        0        0 2023-12-28 13:15:33.050786 jellyfish_server_sdk-0.2.0/jellyfish/api/__init__.py
--rw-r--r--   0        0        0      816 2023-12-28 13:15:33.050888 jellyfish_server_sdk-0.2.0/jellyfish/api/_base_api.py
--rw-r--r--   0        0        0     1058 2023-12-28 13:15:33.050990 jellyfish_server_sdk-0.2.0/jellyfish/api/_recording_api.py
--rw-r--r--   0        0        0     5778 2023-12-29 10:39:38.196618 jellyfish_server_sdk-0.2.0/jellyfish/api/_room_api.py
--rw-r--r--   0        0        0     1178 2023-12-28 13:15:33.051159 jellyfish_server_sdk-0.2.0/jellyfish/errors.py
--rw-r--r--   0        0        0      716 2023-12-28 13:15:33.051267 jellyfish_server_sdk-0.2.0/jellyfish/events/__init__.py
--rw-r--r--   0        0        0        0 2023-12-28 13:15:33.051335 jellyfish_server_sdk-0.2.0/jellyfish/events/_protos/__init__.py
--rw-r--r--   0        0        0     4435 2023-12-28 13:15:33.051518 jellyfish_server_sdk-0.2.0/jellyfish/events/_protos/jellyfish/__init__.py
--rw-r--r--   0        0        0     1657 2024-01-09 15:27:10.458158 jellyfish_server_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5189 1970-01-01 00:00:00.000000 jellyfish_server_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5184 2024-02-29 10:19:40.819186 jellyfish_server_sdk-0.3.0/README.md
+-rw-r--r--   0        0        0     1721 2024-02-29 10:19:40.819866 jellyfish_server_sdk-0.3.0/jellyfish/__init__.py
+-rw-r--r--   0        0        0      166 2024-02-07 16:06:54.525370 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-02-07 16:06:54.402541 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 10:19:40.819947 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/health/__init__.py
+-rw-r--r--   0        0        0     3673 2024-02-29 10:19:40.820685 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/health/healthcheck.py
+-rw-r--r--   0        0        0        0 2024-02-07 16:06:54.423129 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/hls/__init__.py
+-rw-r--r--   0        0        0     7598 2024-02-07 16:06:54.523265 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/hls/get_hls_content.py
+-rw-r--r--   0        0        0     4914 2024-02-29 10:19:40.820968 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/hls/subscribe_hls_to.py
+-rw-r--r--   0        0        0        0 2024-02-07 16:06:54.424688 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/recording/__init__.py
+-rw-r--r--   0        0        0     4166 2024-02-29 10:19:40.821217 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/recording/delete_recording.py
+-rw-r--r--   0        0        0     4414 2024-02-07 16:06:54.523510 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/recording/get_recording_content.py
+-rw-r--r--   0        0        0     3829 2024-02-29 10:19:40.821438 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/recording/get_recordings.py
+-rw-r--r--   0        0        0        0 2024-02-07 16:06:54.426112 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/__init__.py
+-rw-r--r--   0        0        0     5098 2024-02-07 16:06:54.524988 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/add_component.py
+-rw-r--r--   0        0        0     4985 2024-02-07 16:06:54.524354 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/add_peer.py
+-rw-r--r--   0        0        0     4461 2024-02-07 16:06:54.524605 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/create_room.py
+-rw-r--r--   0        0        0     4208 2024-02-07 16:06:54.523091 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/delete_component.py
+-rw-r--r--   0        0        0     4111 2024-02-07 16:06:54.523611 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/delete_peer.py
+-rw-r--r--   0        0        0     3897 2024-02-07 16:06:54.522308 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/delete_room.py
+-rw-r--r--   0        0        0     3681 2024-02-07 16:06:54.523923 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/get_all_rooms.py
+-rw-r--r--   0        0        0     4204 2024-02-07 16:06:54.524721 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/get_room.py
+-rw-r--r--   0        0        0        0 2024-02-29 10:19:40.821628 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/sip/__init__.py
+-rw-r--r--   0        0        0     5210 2024-02-29 10:19:40.821855 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/sip/dial.py
+-rw-r--r--   0        0        0     4535 2024-02-29 10:19:40.822017 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/sip/end_call.py
+-rw-r--r--   0        0        0    12209 2024-02-07 16:06:54.525791 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/client.py
+-rw-r--r--   0        0        0      470 2024-02-07 16:06:54.522343 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/errors.py
+-rw-r--r--   0        0        0     3496 2024-02-29 10:19:40.822194 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/__init__.py
+-rw-r--r--   0        0        0     4934 2024-02-29 10:19:40.822558 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/add_component_json_body.py
+-rw-r--r--   0        0        0     1930 2024-02-07 16:06:54.523234 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/add_peer_json_body.py
+-rw-r--r--   0        0        0     3909 2024-02-29 10:19:40.822894 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_details_response.py
+-rw-r--r--   0        0        0     3119 2024-02-12 18:30:22.528060 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_file.py
+-rw-r--r--   0        0        0     2697 2024-02-12 18:30:22.528396 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_hls.py
+-rw-r--r--   0        0        0     2034 2024-02-07 16:06:54.524704 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_options_file.py
+-rw-r--r--   0        0        0     4192 2024-02-07 16:06:54.525445 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_options_hls.py
+-rw-r--r--   0        0        0      268 2024-02-07 16:06:54.522563 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_options_hls_subscribe_mode.py
+-rw-r--r--   0        0        0     3151 2024-02-07 16:06:54.525519 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_options_rtsp.py
+-rw-r--r--   0        0        0     2142 2024-02-29 10:19:40.823013 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_options_sip.py
+-rw-r--r--   0        0        0     2262 2024-02-29 10:19:40.823128 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_options_sipsip_credentials.py
+-rw-r--r--   0        0        0     1962 2024-02-12 18:30:22.528932 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_properties_file.py
+-rw-r--r--   0        0        0     2951 2024-02-07 16:06:54.523684 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_properties_hls.py
+-rw-r--r--   0        0        0      270 2024-02-07 16:06:54.522241 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_properties_hls_subscribe_mode.py
+-rw-r--r--   0        0        0     2825 2024-02-07 16:06:54.523351 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_properties_rtsp.py
+-rw-r--r--   0        0        0     2178 2024-02-29 10:19:40.823227 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_properties_sip.py
+-rw-r--r--   0        0        0     2277 2024-02-29 10:19:40.823347 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_properties_sipsip_credentials.py
+-rw-r--r--   0        0        0     2710 2024-02-12 18:30:22.529076 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_rtsp.py
+-rw-r--r--   0        0        0     2697 2024-02-29 10:19:40.823460 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_sip.py
+-rw-r--r--   0        0        0     1677 2024-02-29 10:19:40.823671 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/dial_config.py
+-rw-r--r--   0        0        0     1486 2024-02-07 16:06:54.524531 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/error.py
+-rw-r--r--   0        0        0     2397 2024-02-12 18:30:22.529305 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/health_report.py
+-rw-r--r--   0        0        0     2451 2024-02-12 18:30:22.529473 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/health_report_distribution.py
+-rw-r--r--   0        0        0      226 2024-02-12 18:30:22.529628 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/health_report_status.py
+-rw-r--r--   0        0        0     1784 2024-02-12 18:30:22.529772 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/healthcheck_response.py
+-rw-r--r--   0        0        0     2641 2024-02-12 18:30:22.529960 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/peer.py
+-rw-r--r--   0        0        0     1825 2024-02-07 16:06:54.522592 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/peer_details_response.py
+-rw-r--r--   0        0        0     1887 2024-02-07 16:06:54.522201 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/peer_details_response_data.py
+-rw-r--r--   0        0        0     1770 2024-02-07 16:06:54.524989 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/peer_options_web_rtc.py
+-rw-r--r--   0        0        0      218 2024-02-07 16:06:54.522758 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/peer_status.py
+-rw-r--r--   0        0        0     1602 2024-02-07 16:06:54.523716 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/recording_list_response.py
+-rw-r--r--   0        0        0     5444 2024-02-29 10:19:40.824043 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/room.py
+-rw-r--r--   0        0        0     3682 2024-02-29 10:19:40.824216 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/room_config.py
+-rw-r--r--   0        0        0      217 2024-02-07 16:06:54.524034 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/room_config_video_codec.py
+-rw-r--r--   0        0        0     1905 2024-02-07 16:06:54.522275 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/room_create_details_response.py
+-rw-r--r--   0        0        0     2172 2024-02-07 16:06:54.523827 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/room_create_details_response_data.py
+-rw-r--r--   0        0        0     1718 2024-02-07 16:06:54.523098 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/room_details_response.py
+-rw-r--r--   0        0        0     1949 2024-02-07 16:06:54.523878 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/rooms_listing_response.py
+-rw-r--r--   0        0        0     2448 2024-02-07 16:06:54.523904 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/s3_credentials.py
+-rw-r--r--   0        0        0     2161 2024-02-29 10:19:40.824326 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/sip_credentials.py
+-rw-r--r--   0        0        0     1842 2024-02-07 16:06:54.524270 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/subscription_config.py
+-rw-r--r--   0        0        0     2285 2024-02-12 18:30:22.530118 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/track.py
+-rw-r--r--   0        0        0      170 2024-02-12 18:30:22.530189 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/track_type.py
+-rw-r--r--   0        0        0       25 2024-02-07 16:06:54.353147 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/py.typed
+-rw-r--r--   0        0        0     1001 2024-02-07 16:06:54.525142 jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/types.py
+-rw-r--r--   0        0        0      566 2024-02-12 18:30:22.530377 jellyfish_server_sdk-0.3.0/jellyfish/_webhook_notifier.py
+-rw-r--r--   0        0        0     5020 2024-02-06 14:13:09.601706 jellyfish_server_sdk-0.3.0/jellyfish/_ws_notifier.py
+-rw-r--r--   0        0        0        0 2024-02-06 14:13:09.601768 jellyfish_server_sdk-0.3.0/jellyfish/api/__init__.py
+-rw-r--r--   0        0        0      816 2024-02-06 14:13:09.601845 jellyfish_server_sdk-0.3.0/jellyfish/api/_base_api.py
+-rw-r--r--   0        0        0     1058 2024-02-06 14:13:09.601929 jellyfish_server_sdk-0.3.0/jellyfish/api/_recording_api.py
+-rw-r--r--   0        0        0     7466 2024-02-29 10:19:40.824509 jellyfish_server_sdk-0.3.0/jellyfish/api/_room_api.py
+-rw-r--r--   0        0        0     1178 2024-02-06 14:13:09.602111 jellyfish_server_sdk-0.3.0/jellyfish/errors.py
+-rw-r--r--   0        0        0     1041 2024-02-12 18:30:22.530668 jellyfish_server_sdk-0.3.0/jellyfish/events/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 14:58:51.964790 jellyfish_server_sdk-0.3.0/jellyfish/events/_protos/__init__.py
+-rw-r--r--   0        0        0     8003 2024-02-12 18:30:22.531109 jellyfish_server_sdk-0.3.0/jellyfish/events/_protos/jellyfish/__init__.py
+-rw-r--r--   0        0        0     1698 2024-02-29 10:19:40.825657 jellyfish_server_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6213 1970-01-01 00:00:00.000000 jellyfish_server_sdk-0.3.0/PKG-INFO
```

### Comparing `jellyfish_server_sdk-0.2.0/README.md` & `jellyfish_server_sdk-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -91,14 +91,37 @@
 
 asyncio.run(test_notifier())
 
 # Received a notification: ServerMessageRoomCreated(room_id='69a3fd1a-6a4d-47bc-ae54-0c72b0d05e29')
 # Received WebRTC metrics: ServerMessageMetricsReport(metrics='{}')
 ```
 
+#### Cluster of Jellyfishes
+
+The cluster of jellyfishes has got embedded load balancer, which means that a new room will be created on jellyfish with the least usage. At the moment to modify this specific room you must communicate with the jellyfish on which this room was created.
+
+```python
+room_api = RoomApi(server_address='localhost:5002')
+
+# Create a room to trigger a server notification with h264 as a codec,
+# that allow to use HLS.
+address, room = room_api.create_room(video_codec="h264")
+
+# Create new room api with returned jellyfish address as a room could be
+# created on a different jellyfish instance
+# (if you communicate with a cluster of jellyfishes)
+new_room_api = RoomApi(server_address=address)
+
+# Add HLS component with manual subscribe mode, we use here `new_room_api` as we are sure that this API refers to the jellyfish on which this room was created.
+_hls_component = new_room_api.add_component(
+    room.id,
+    ComponentOptionsHLS(subscribe_mode=ComponentOptionsHLSSubscribeMode.MANUAL),
+)
+```
+
 ## Testing
 
 You can test the SDK by running
 ```console
 poetry run ci_test
 ```
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/__init__.py` & `jellyfish_server_sdk-0.3.0/jellyfish/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,52 +11,63 @@
 from jellyfish._openapi_client.models import (
     ComponentFile,
     ComponentHLS,
     ComponentOptionsFile,
     ComponentOptionsHLS,
     ComponentOptionsHLSSubscribeMode,
     ComponentOptionsRTSP,
+    ComponentOptionsSIP,
     ComponentPropertiesFile,
     ComponentPropertiesHLS,
     ComponentPropertiesHLSSubscribeMode,
     ComponentPropertiesRTSP,
+    ComponentPropertiesSIP,
+    ComponentPropertiesSIPSIPCredentials,
     ComponentRTSP,
+    ComponentSIP,
     Peer,
     PeerOptionsWebRTC,
     PeerStatus,
     Room,
     RoomConfig,
     RoomConfigVideoCodec,
+    SIPCredentials,
 )
 
 # API
-from jellyfish._webhook_notifier import receive_json
+from jellyfish._webhook_notifier import receive_binary
 from jellyfish._ws_notifier import Notifier
 from jellyfish.api._recording_api import RecordingApi
 from jellyfish.api._room_api import RoomApi
 
 __all__ = [
     "RoomApi",
     "RecordingApi",
     "Notifier",
-    "receive_json",
+    "receive_binary",
     "Room",
     "RoomConfig",
     "RoomConfigVideoCodec",
     "Peer",
     "PeerOptionsWebRTC",
     "PeerStatus",
     "ComponentHLS",
     "ComponentOptionsHLS",
     "ComponentOptionsHLSSubscribeMode",
     "ComponentPropertiesHLS",
     "ComponentPropertiesHLSSubscribeMode",
+    "ComponentSIP",
+    "ComponentOptionsSIP",
+    "ComponentPropertiesSIP",
+    "ComponentPropertiesSIPSIPCredentials",
+    "ComponentFile",
     "ComponentRTSP",
     "ComponentOptionsRTSP",
     "ComponentPropertiesRTSP",
     "ComponentFile",
     "ComponentOptionsFile",
     "ComponentPropertiesFile",
     "events",
     "errors",
+    "SIPCredentials",
 ]
 __docformat__ = "restructuredtext"
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/hls/get_hls_content.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/hls/get_hls_content.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/hls/subscribe_hls_to.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/hls/subscribe_hls_to.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,18 @@
     if response.status_code == HTTPStatus.CREATED:
         response_201 = cast(Any, None)
         return response_201
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = Error.from_dict(response.json())
 
         return response_400
+    if response.status_code == HTTPStatus.UNAUTHORIZED:
+        response_401 = Error.from_dict(response.json())
+
+        return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
         response_404 = Error.from_dict(response.json())
 
         return response_404
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/recording/delete_recording.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/recording/delete_recording.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     if response.status_code == HTTPStatus.NO_CONTENT:
         response_204 = cast(Any, None)
         return response_204
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = Error.from_dict(response.json())
 
         return response_400
+    if response.status_code == HTTPStatus.UNAUTHORIZED:
+        response_401 = Error.from_dict(response.json())
+
+        return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
         response_404 = Error.from_dict(response.json())
 
         return response_404
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/recording/get_recording_content.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/recording/get_recording_content.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/recording/get_recordings.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/recording/get_recordings.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
 ) -> Optional[Union[Error, RecordingListResponse]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = RecordingListResponse.from_dict(response.json())
 
         return response_200
+    if response.status_code == HTTPStatus.UNAUTHORIZED:
+        response_401 = Error.from_dict(response.json())
+
+        return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
         response_404 = Error.from_dict(response.json())
 
         return response_404
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/add_component.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/add_component.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/add_peer.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/add_peer.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/create_room.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/create_room.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/delete_component.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/delete_component.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/delete_peer.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/delete_peer.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/delete_room.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/delete_room.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/get_all_rooms.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/get_all_rooms.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/api/room/get_room.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/api/room/get_room.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/client.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/client.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/__init__.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,61 +5,89 @@
 from .component_details_response import ComponentDetailsResponse
 from .component_file import ComponentFile
 from .component_hls import ComponentHLS
 from .component_options_file import ComponentOptionsFile
 from .component_options_hls import ComponentOptionsHLS
 from .component_options_hls_subscribe_mode import ComponentOptionsHLSSubscribeMode
 from .component_options_rtsp import ComponentOptionsRTSP
+from .component_options_sip import ComponentOptionsSIP
+from .component_options_sipsip_credentials import ComponentOptionsSIPSIPCredentials
 from .component_properties_file import ComponentPropertiesFile
 from .component_properties_hls import ComponentPropertiesHLS
 from .component_properties_hls_subscribe_mode import ComponentPropertiesHLSSubscribeMode
 from .component_properties_rtsp import ComponentPropertiesRTSP
+from .component_properties_sip import ComponentPropertiesSIP
+from .component_properties_sipsip_credentials import (
+    ComponentPropertiesSIPSIPCredentials,
+)
 from .component_rtsp import ComponentRTSP
+from .component_sip import ComponentSIP
+from .dial_config import DialConfig
 from .error import Error
+from .health_report import HealthReport
+from .health_report_distribution import HealthReportDistribution
+from .health_report_status import HealthReportStatus
+from .healthcheck_response import HealthcheckResponse
 from .peer import Peer
 from .peer_details_response import PeerDetailsResponse
 from .peer_details_response_data import PeerDetailsResponseData
 from .peer_options_web_rtc import PeerOptionsWebRTC
 from .peer_status import PeerStatus
 from .recording_list_response import RecordingListResponse
 from .room import Room
 from .room_config import RoomConfig
 from .room_config_video_codec import RoomConfigVideoCodec
 from .room_create_details_response import RoomCreateDetailsResponse
 from .room_create_details_response_data import RoomCreateDetailsResponseData
 from .room_details_response import RoomDetailsResponse
 from .rooms_listing_response import RoomsListingResponse
 from .s3_credentials import S3Credentials
+from .sip_credentials import SIPCredentials
 from .subscription_config import SubscriptionConfig
+from .track import Track
+from .track_type import TrackType
 
 __all__ = (
     "AddComponentJsonBody",
     "AddPeerJsonBody",
     "ComponentDetailsResponse",
     "ComponentFile",
     "ComponentHLS",
     "ComponentOptionsFile",
     "ComponentOptionsHLS",
     "ComponentOptionsHLSSubscribeMode",
     "ComponentOptionsRTSP",
+    "ComponentOptionsSIP",
+    "ComponentOptionsSIPSIPCredentials",
     "ComponentPropertiesFile",
     "ComponentPropertiesHLS",
     "ComponentPropertiesHLSSubscribeMode",
     "ComponentPropertiesRTSP",
+    "ComponentPropertiesSIP",
+    "ComponentPropertiesSIPSIPCredentials",
     "ComponentRTSP",
+    "ComponentSIP",
+    "DialConfig",
     "Error",
+    "HealthcheckResponse",
+    "HealthReport",
+    "HealthReportDistribution",
+    "HealthReportStatus",
     "Peer",
     "PeerDetailsResponse",
     "PeerDetailsResponseData",
     "PeerOptionsWebRTC",
     "PeerStatus",
     "RecordingListResponse",
     "Room",
     "RoomConfig",
     "RoomConfigVideoCodec",
     "RoomCreateDetailsResponse",
     "RoomCreateDetailsResponseData",
     "RoomDetailsResponse",
     "RoomsListingResponse",
     "S3Credentials",
+    "SIPCredentials",
     "SubscriptionConfig",
+    "Track",
+    "TrackType",
 )
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/add_component_json_body.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_details_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,121 +1,112 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..types import UNSET, Unset
-
 if TYPE_CHECKING:
-    from ..models.component_options_file import ComponentOptionsFile
-    from ..models.component_options_hls import ComponentOptionsHLS
-    from ..models.component_options_rtsp import ComponentOptionsRTSP
+    from ..models.component_file import ComponentFile
+    from ..models.component_hls import ComponentHLS
+    from ..models.component_rtsp import ComponentRTSP
+    from ..models.component_sip import ComponentSIP
 
 
-T = TypeVar("T", bound="AddComponentJsonBody")
+T = TypeVar("T", bound="ComponentDetailsResponse")
 
 
 @_attrs_define
-class AddComponentJsonBody:
-    """ """
+class ComponentDetailsResponse:
+    """Response containing component details"""
 
-    type: str
-    """Component type"""
-    options: Union[
-        "ComponentOptionsFile", "ComponentOptionsHLS", "ComponentOptionsRTSP", Unset
-    ] = UNSET
-    """Component-specific options"""
+    data: Union["ComponentFile", "ComponentHLS", "ComponentRTSP", "ComponentSIP"]
+    """Describes component"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
-        from ..models.component_options_hls import ComponentOptionsHLS
-        from ..models.component_options_rtsp import ComponentOptionsRTSP
+        from ..models.component_file import ComponentFile
+        from ..models.component_hls import ComponentHLS
+        from ..models.component_rtsp import ComponentRTSP
+
+        data: Dict[str, Any]
 
-        type = self.type
-        options: Union[Dict[str, Any], Unset]
-        if isinstance(self.options, Unset):
-            options = UNSET
+        if isinstance(self.data, ComponentHLS):
+            data = self.data.to_dict()
 
-        elif isinstance(self.options, ComponentOptionsHLS):
-            options = self.options.to_dict()
+        elif isinstance(self.data, ComponentRTSP):
+            data = self.data.to_dict()
 
-        elif isinstance(self.options, ComponentOptionsRTSP):
-            options = self.options.to_dict()
+        elif isinstance(self.data, ComponentFile):
+            data = self.data.to_dict()
 
         else:
-            options = self.options.to_dict()
+            data = self.data.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "type": type,
+                "data": data,
             }
         )
-        if options is not UNSET:
-            field_dict["options"] = options
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
-        from ..models.component_options_file import ComponentOptionsFile
-        from ..models.component_options_hls import ComponentOptionsHLS
-        from ..models.component_options_rtsp import ComponentOptionsRTSP
+        from ..models.component_file import ComponentFile
+        from ..models.component_hls import ComponentHLS
+        from ..models.component_rtsp import ComponentRTSP
+        from ..models.component_sip import ComponentSIP
 
         d = src_dict.copy()
-        type = d.pop("type")
 
-        def _parse_options(
+        def _parse_data(
             data: object,
-        ) -> Union[
-            "ComponentOptionsFile", "ComponentOptionsHLS", "ComponentOptionsRTSP", Unset
-        ]:
-            if isinstance(data, Unset):
-                return data
+        ) -> Union["ComponentFile", "ComponentHLS", "ComponentRTSP", "ComponentSIP"]:
+            try:
+                if not isinstance(data, dict):
+                    raise TypeError()
+                componentsschemas_component_type_0 = ComponentHLS.from_dict(data)
+
+                return componentsschemas_component_type_0
+            except:  # noqa: E722
+                pass
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
-                componentsschemas_component_options_type_0 = (
-                    ComponentOptionsHLS.from_dict(data)
-                )
+                componentsschemas_component_type_1 = ComponentRTSP.from_dict(data)
 
-                return componentsschemas_component_options_type_0
+                return componentsschemas_component_type_1
             except:  # noqa: E722
                 pass
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
-                componentsschemas_component_options_type_1 = (
-                    ComponentOptionsRTSP.from_dict(data)
-                )
+                componentsschemas_component_type_2 = ComponentFile.from_dict(data)
 
-                return componentsschemas_component_options_type_1
+                return componentsschemas_component_type_2
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
-            componentsschemas_component_options_type_2 = ComponentOptionsFile.from_dict(
-                data
-            )
+            componentsschemas_component_type_3 = ComponentSIP.from_dict(data)
 
-            return componentsschemas_component_options_type_2
+            return componentsschemas_component_type_3
 
-        options = _parse_options(d.pop("options", UNSET))
+        data = _parse_data(d.pop("data"))
 
-        add_component_json_body = cls(
-            type=type,
-            options=options,
+        component_details_response = cls(
+            data=data,
         )
 
-        add_component_json_body.additional_properties = d
-        return add_component_json_body
+        component_details_response.additional_properties = d
+        return component_details_response
 
     @property
     def additional_keys(self) -> List[str]:
         """@private"""
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/add_peer_json_body.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/add_peer_json_body.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_file.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,72 +3,91 @@
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.component_properties_file import ComponentPropertiesFile
+    from ..models.track import Track
 
 
 T = TypeVar("T", bound="ComponentFile")
 
 
 @_attrs_define
 class ComponentFile:
     """Describes the File component"""
 
     id: str
     """Assigned component ID"""
+    tracks: List["Track"]
+    """List of all component's tracks"""
     type: str
     """Component type"""
     properties: Union[Unset, "ComponentPropertiesFile"] = UNSET
     """Properties specific to the File component"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
         id = self.id
+        tracks = []
+        for tracks_item_data in self.tracks:
+            tracks_item = tracks_item_data.to_dict()
+
+            tracks.append(tracks_item)
+
         type = self.type
         properties: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.properties, Unset):
             properties = self.properties.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "id": id,
+                "tracks": tracks,
                 "type": type,
             }
         )
         if properties is not UNSET:
             field_dict["properties"] = properties
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
         from ..models.component_properties_file import ComponentPropertiesFile
+        from ..models.track import Track
 
         d = src_dict.copy()
         id = d.pop("id")
 
+        tracks = []
+        _tracks = d.pop("tracks")
+        for tracks_item_data in _tracks:
+            tracks_item = Track.from_dict(tracks_item_data)
+
+            tracks.append(tracks_item)
+
         type = d.pop("type")
 
         _properties = d.pop("properties", UNSET)
         properties: Union[Unset, ComponentPropertiesFile]
         if isinstance(_properties, Unset):
             properties = UNSET
         else:
             properties = ComponentPropertiesFile.from_dict(_properties)
 
         component_file = cls(
             id=id,
+            tracks=tracks,
             type=type,
             properties=properties,
         )
 
         component_file.additional_properties = d
         return component_file
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_hls.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_sip.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,90 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 if TYPE_CHECKING:
-    from ..models.component_properties_hls import ComponentPropertiesHLS
+    from ..models.component_properties_sip import ComponentPropertiesSIP
+    from ..models.track import Track
 
 
-T = TypeVar("T", bound="ComponentHLS")
+T = TypeVar("T", bound="ComponentSIP")
 
 
 @_attrs_define
-class ComponentHLS:
-    """Describes the HLS component"""
+class ComponentSIP:
+    """Describes the SIP component"""
 
     id: str
     """Assigned component ID"""
-    properties: "ComponentPropertiesHLS"
-    """Properties specific to the HLS component"""
+    properties: "ComponentPropertiesSIP"
+    """Properties specific to the SIP component"""
+    tracks: List["Track"]
+    """List of all component's tracks"""
     type: str
     """Component type"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
         id = self.id
         properties = self.properties.to_dict()
 
+        tracks = []
+        for tracks_item_data in self.tracks:
+            tracks_item = tracks_item_data.to_dict()
+
+            tracks.append(tracks_item)
+
         type = self.type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "id": id,
                 "properties": properties,
+                "tracks": tracks,
                 "type": type,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
-        from ..models.component_properties_hls import ComponentPropertiesHLS
+        from ..models.component_properties_sip import ComponentPropertiesSIP
+        from ..models.track import Track
 
         d = src_dict.copy()
         id = d.pop("id")
 
-        properties = ComponentPropertiesHLS.from_dict(d.pop("properties"))
+        properties = ComponentPropertiesSIP.from_dict(d.pop("properties"))
+
+        tracks = []
+        _tracks = d.pop("tracks")
+        for tracks_item_data in _tracks:
+            tracks_item = Track.from_dict(tracks_item_data)
+
+            tracks.append(tracks_item)
 
         type = d.pop("type")
 
-        component_hls = cls(
+        component_sip = cls(
             id=id,
             properties=properties,
+            tracks=tracks,
             type=type,
         )
 
-        component_hls.additional_properties = d
-        return component_hls
+        component_sip.additional_properties = d
+        return component_sip
 
     @property
     def additional_keys(self) -> List[str]:
         """@private"""
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_options_file.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_options_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,56 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
+from ..types import UNSET, Unset
+
 T = TypeVar("T", bound="ComponentOptionsFile")
 
 
 @_attrs_define
 class ComponentOptionsFile:
     """Options specific to the File component"""
 
     file_path: str
     """Path to track file. Must be either OPUS encapsulated in Ogg or raw h264"""
+    framerate: Union[Unset, None, int] = UNSET
+    """Framerate of video in a file. It is only valid for video track"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
         file_path = self.file_path
+        framerate = self.framerate
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "filePath": file_path,
             }
         )
+        if framerate is not UNSET:
+            field_dict["framerate"] = framerate
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
         d = src_dict.copy()
         file_path = d.pop("filePath")
 
+        framerate = d.pop("framerate", UNSET)
+
         component_options_file = cls(
             file_path=file_path,
+            framerate=framerate,
         )
 
         component_options_file.additional_properties = d
         return component_options_file
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_options_hls.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_options_hls.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_options_rtsp.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_options_rtsp.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_properties_file.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/error.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-T = TypeVar("T", bound="ComponentPropertiesFile")
+T = TypeVar("T", bound="Error")
 
 
 @_attrs_define
-class ComponentPropertiesFile:
-    """Properties specific to the File component"""
+class Error:
+    """Error message"""
 
-    file_path: str
-    """Path to track file. Must be either OPUS encapsulated in Ogg or raw h264"""
+    errors: str
+    """Error details"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
-        file_path = self.file_path
+        errors = self.errors
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "filePath": file_path,
+                "errors": errors,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
         d = src_dict.copy()
-        file_path = d.pop("filePath")
+        errors = d.pop("errors")
 
-        component_properties_file = cls(
-            file_path=file_path,
+        error = cls(
+            errors=errors,
         )
 
-        component_properties_file.additional_properties = d
-        return component_properties_file
+        error.additional_properties = d
+        return error
 
     @property
     def additional_keys(self) -> List[str]:
         """@private"""
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_properties_hls.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_properties_hls.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_properties_rtsp.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_properties_file.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,57 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="ComponentPropertiesRTSP")
+T = TypeVar("T", bound="ComponentPropertiesFile")
 
 
 @_attrs_define
-class ComponentPropertiesRTSP:
-    """Properties specific to the RTSP component"""
+class ComponentPropertiesFile:
+    """Properties specific to the File component"""
 
-    source_uri: str
-    """URI of RTSP source stream"""
-    keep_alive_interval: Union[Unset, int] = UNSET
-    """Interval (in ms) in which keep-alive RTSP messages will be sent to the remote stream source"""
-    pierce_nat: Union[Unset, bool] = UNSET
-    """Whether to attempt to create client-side NAT binding by sending an empty datagram from client to source, after the completion of RTSP setup"""
-    reconnect_delay: Union[Unset, int] = UNSET
-    """Delay (in ms) between successive reconnect attempts"""
-    rtp_port: Union[Unset, int] = UNSET
-    """Local port RTP stream will be received at"""
+    file_path: str
+    """Relative path to track file. Must be either OPUS encapsulated in Ogg or raw h264"""
+    framerate: Optional[int]
+    """Framerate of video in a file. It is only valid for video track"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
-        source_uri = self.source_uri
-        keep_alive_interval = self.keep_alive_interval
-        pierce_nat = self.pierce_nat
-        reconnect_delay = self.reconnect_delay
-        rtp_port = self.rtp_port
+        file_path = self.file_path
+        framerate = self.framerate
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "sourceUri": source_uri,
+                "filePath": file_path,
+                "framerate": framerate,
             }
         )
-        if keep_alive_interval is not UNSET:
-            field_dict["keepAliveInterval"] = keep_alive_interval
-        if pierce_nat is not UNSET:
-            field_dict["pierceNat"] = pierce_nat
-        if reconnect_delay is not UNSET:
-            field_dict["reconnectDelay"] = reconnect_delay
-        if rtp_port is not UNSET:
-            field_dict["rtpPort"] = rtp_port
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
         d = src_dict.copy()
-        source_uri = d.pop("sourceUri")
-
-        keep_alive_interval = d.pop("keepAliveInterval", UNSET)
-
-        pierce_nat = d.pop("pierceNat", UNSET)
-
-        reconnect_delay = d.pop("reconnectDelay", UNSET)
+        file_path = d.pop("filePath")
 
-        rtp_port = d.pop("rtpPort", UNSET)
+        framerate = d.pop("framerate")
 
-        component_properties_rtsp = cls(
-            source_uri=source_uri,
-            keep_alive_interval=keep_alive_interval,
-            pierce_nat=pierce_nat,
-            reconnect_delay=reconnect_delay,
-            rtp_port=rtp_port,
+        component_properties_file = cls(
+            file_path=file_path,
+            framerate=framerate,
         )
 
-        component_properties_rtsp.additional_properties = d
-        return component_properties_rtsp
+        component_properties_file.additional_properties = d
+        return component_properties_file
 
     @property
     def additional_keys(self) -> List[str]:
         """@private"""
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/component_rtsp.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_hls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,90 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 if TYPE_CHECKING:
-    from ..models.component_properties_rtsp import ComponentPropertiesRTSP
+    from ..models.component_properties_hls import ComponentPropertiesHLS
+    from ..models.track import Track
 
 
-T = TypeVar("T", bound="ComponentRTSP")
+T = TypeVar("T", bound="ComponentHLS")
 
 
 @_attrs_define
-class ComponentRTSP:
-    """Describes the RTSP component"""
+class ComponentHLS:
+    """Describes the HLS component"""
 
     id: str
     """Assigned component ID"""
-    properties: "ComponentPropertiesRTSP"
-    """Properties specific to the RTSP component"""
+    properties: "ComponentPropertiesHLS"
+    """Properties specific to the HLS component"""
+    tracks: List["Track"]
+    """List of all component's tracks"""
     type: str
     """Component type"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
         id = self.id
         properties = self.properties.to_dict()
 
+        tracks = []
+        for tracks_item_data in self.tracks:
+            tracks_item = tracks_item_data.to_dict()
+
+            tracks.append(tracks_item)
+
         type = self.type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "id": id,
                 "properties": properties,
+                "tracks": tracks,
                 "type": type,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
-        from ..models.component_properties_rtsp import ComponentPropertiesRTSP
+        from ..models.component_properties_hls import ComponentPropertiesHLS
+        from ..models.track import Track
 
         d = src_dict.copy()
         id = d.pop("id")
 
-        properties = ComponentPropertiesRTSP.from_dict(d.pop("properties"))
+        properties = ComponentPropertiesHLS.from_dict(d.pop("properties"))
+
+        tracks = []
+        _tracks = d.pop("tracks")
+        for tracks_item_data in _tracks:
+            tracks_item = Track.from_dict(tracks_item_data)
+
+            tracks.append(tracks_item)
 
         type = d.pop("type")
 
-        component_rtsp = cls(
+        component_hls = cls(
             id=id,
             properties=properties,
+            tracks=tracks,
             type=type,
         )
 
-        component_rtsp.additional_properties = d
-        return component_rtsp
+        component_hls.additional_properties = d
+        return component_hls
 
     @property
     def additional_keys(self) -> List[str]:
         """@private"""
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/error.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/component_properties_sip.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,62 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-T = TypeVar("T", bound="Error")
+if TYPE_CHECKING:
+    from ..models.component_properties_sipsip_credentials import (
+        ComponentPropertiesSIPSIPCredentials,
+    )
+
+
+T = TypeVar("T", bound="ComponentPropertiesSIP")
 
 
 @_attrs_define
-class Error:
-    """Error message"""
+class ComponentPropertiesSIP:
+    """Properties specific to the SIP component"""
 
-    errors: str
-    """Error details"""
+    registrar_credentials: "ComponentPropertiesSIPSIPCredentials"
+    """Credentials used to authorize in SIP Provider service"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
-        errors = self.errors
+        registrar_credentials = self.registrar_credentials.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "errors": errors,
+                "registrarCredentials": registrar_credentials,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
+        from ..models.component_properties_sipsip_credentials import (
+            ComponentPropertiesSIPSIPCredentials,
+        )
+
         d = src_dict.copy()
-        errors = d.pop("errors")
+        registrar_credentials = ComponentPropertiesSIPSIPCredentials.from_dict(
+            d.pop("registrarCredentials")
+        )
 
-        error = cls(
-            errors=errors,
+        component_properties_sip = cls(
+            registrar_credentials=registrar_credentials,
         )
 
-        error.additional_properties = d
-        return error
+        component_properties_sip.additional_properties = d
+        return component_properties_sip
 
     @property
     def additional_keys(self) -> List[str]:
         """@private"""
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/peer.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/recording_list_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,50 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..models.peer_status import PeerStatus
-
-T = TypeVar("T", bound="Peer")
+T = TypeVar("T", bound="RecordingListResponse")
 
 
 @_attrs_define
-class Peer:
-    """Describes peer status"""
+class RecordingListResponse:
+    """Response containing list of all recording"""
 
-    id: str
-    """Assigned peer id"""
-    status: PeerStatus
-    """Informs about the peer status"""
-    type: str
-    """Peer type"""
+    data: List[str]
+    """None"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
-        id = self.id
-        status = self.status.value
-
-        type = self.type
+        data = self.data
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "id": id,
-                "status": status,
-                "type": type,
+                "data": data,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
         d = src_dict.copy()
-        id = d.pop("id")
-
-        status = PeerStatus(d.pop("status"))
-
-        type = d.pop("type")
+        data = cast(List[str], d.pop("data"))
 
-        peer = cls(
-            id=id,
-            status=status,
-            type=type,
+        recording_list_response = cls(
+            data=data,
         )
 
-        peer.additional_properties = d
-        return peer
+        recording_list_response.additional_properties = d
+        return recording_list_response
 
     @property
     def additional_keys(self) -> List[str]:
         """@private"""
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/peer_details_response.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/peer_details_response.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/peer_details_response_data.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/peer_details_response_data.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/peer_options_web_rtc.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/peer_options_web_rtc.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/recording_list_response.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/room_create_details_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,58 @@
-from typing import Any, Dict, List, Type, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-T = TypeVar("T", bound="RecordingListResponse")
+if TYPE_CHECKING:
+    from ..models.room_create_details_response_data import RoomCreateDetailsResponseData
+
+
+T = TypeVar("T", bound="RoomCreateDetailsResponse")
 
 
 @_attrs_define
-class RecordingListResponse:
-    """Response containing list of all recording"""
+class RoomCreateDetailsResponse:
+    """Response containing room details"""
 
-    data: List[str]
-    """None"""
+    data: "RoomCreateDetailsResponseData"
+    """"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
-        data = self.data
+        data = self.data.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "data": data,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
+        from ..models.room_create_details_response_data import (
+            RoomCreateDetailsResponseData,
+        )
+
         d = src_dict.copy()
-        data = cast(List[str], d.pop("data"))
+        data = RoomCreateDetailsResponseData.from_dict(d.pop("data"))
 
-        recording_list_response = cls(
+        room_create_details_response = cls(
             data=data,
         )
 
-        recording_list_response.additional_properties = d
-        return recording_list_response
+        room_create_details_response.additional_properties = d
+        return room_create_details_response
 
     @property
     def additional_keys(self) -> List[str]:
         """@private"""
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/room.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/room.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,51 +3,58 @@
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 if TYPE_CHECKING:
     from ..models.component_file import ComponentFile
     from ..models.component_hls import ComponentHLS
     from ..models.component_rtsp import ComponentRTSP
+    from ..models.component_sip import ComponentSIP
     from ..models.peer import Peer
     from ..models.room_config import RoomConfig
 
 
 T = TypeVar("T", bound="Room")
 
 
 @_attrs_define
 class Room:
     """Description of the room state"""
 
-    components: List[Union["ComponentFile", "ComponentHLS", "ComponentRTSP"]]
+    components: List[
+        Union["ComponentFile", "ComponentHLS", "ComponentRTSP", "ComponentSIP"]
+    ]
     """List of all components"""
     config: "RoomConfig"
     """Room configuration"""
     id: str
     """Room ID"""
     peers: List["Peer"]
     """List of all peers"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
+        from ..models.component_file import ComponentFile
         from ..models.component_hls import ComponentHLS
         from ..models.component_rtsp import ComponentRTSP
 
         components = []
         for components_item_data in self.components:
             components_item: Dict[str, Any]
 
             if isinstance(components_item_data, ComponentHLS):
                 components_item = components_item_data.to_dict()
 
             elif isinstance(components_item_data, ComponentRTSP):
                 components_item = components_item_data.to_dict()
 
+            elif isinstance(components_item_data, ComponentFile):
+                components_item = components_item_data.to_dict()
+
             else:
                 components_item = components_item_data.to_dict()
 
             components.append(components_item)
 
         config = self.config.to_dict()
 
@@ -73,25 +80,28 @@
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
         from ..models.component_file import ComponentFile
         from ..models.component_hls import ComponentHLS
         from ..models.component_rtsp import ComponentRTSP
+        from ..models.component_sip import ComponentSIP
         from ..models.peer import Peer
         from ..models.room_config import RoomConfig
 
         d = src_dict.copy()
         components = []
         _components = d.pop("components")
         for components_item_data in _components:
 
             def _parse_components_item(
                 data: object,
-            ) -> Union["ComponentFile", "ComponentHLS", "ComponentRTSP"]:
+            ) -> Union[
+                "ComponentFile", "ComponentHLS", "ComponentRTSP", "ComponentSIP"
+            ]:
                 try:
                     if not isinstance(data, dict):
                         raise TypeError()
                     componentsschemas_component_type_0 = ComponentHLS.from_dict(data)
 
                     return componentsschemas_component_type_0
                 except:  # noqa: E722
@@ -100,19 +110,27 @@
                     if not isinstance(data, dict):
                         raise TypeError()
                     componentsschemas_component_type_1 = ComponentRTSP.from_dict(data)
 
                     return componentsschemas_component_type_1
                 except:  # noqa: E722
                     pass
+                try:
+                    if not isinstance(data, dict):
+                        raise TypeError()
+                    componentsschemas_component_type_2 = ComponentFile.from_dict(data)
+
+                    return componentsschemas_component_type_2
+                except:  # noqa: E722
+                    pass
                 if not isinstance(data, dict):
                     raise TypeError()
-                componentsschemas_component_type_2 = ComponentFile.from_dict(data)
+                componentsschemas_component_type_3 = ComponentSIP.from_dict(data)
 
-                return componentsschemas_component_type_2
+                return componentsschemas_component_type_3
 
             components_item = _parse_components_item(components_item_data)
 
             components.append(components_item)
 
         config = RoomConfig.from_dict(d.pop("config"))
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/room_config.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/room_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,38 +11,43 @@
 
 @_attrs_define
 class RoomConfig:
     """Room configuration"""
 
     max_peers: Union[Unset, None, int] = UNSET
     """Maximum amount of peers allowed into the room"""
+    peerless_purge_timeout: Union[Unset, None, int] = UNSET
+    """Duration (in seconds) after which the room will be removed if no peers are connected. If not provided, this feature is disabled."""
     room_id: Union[Unset, None, str] = UNSET
     """Custom id used for identifying room within Jellyfish. Must be unique across all rooms. If not provided, random UUID is generated."""
     video_codec: Union[Unset, None, RoomConfigVideoCodec] = UNSET
     """Enforces video codec for each peer in the room"""
     webhook_url: Union[Unset, None, str] = UNSET
     """URL where Jellyfish notifications will be sent"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
         max_peers = self.max_peers
+        peerless_purge_timeout = self.peerless_purge_timeout
         room_id = self.room_id
         video_codec: Union[Unset, None, str] = UNSET
         if not isinstance(self.video_codec, Unset):
             video_codec = self.video_codec.value if self.video_codec else None
 
         webhook_url = self.webhook_url
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if max_peers is not UNSET:
             field_dict["maxPeers"] = max_peers
+        if peerless_purge_timeout is not UNSET:
+            field_dict["peerlessPurgeTimeout"] = peerless_purge_timeout
         if room_id is not UNSET:
             field_dict["roomId"] = room_id
         if video_codec is not UNSET:
             field_dict["videoCodec"] = video_codec
         if webhook_url is not UNSET:
             field_dict["webhookUrl"] = webhook_url
 
@@ -50,14 +55,16 @@
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
         d = src_dict.copy()
         max_peers = d.pop("maxPeers", UNSET)
 
+        peerless_purge_timeout = d.pop("peerlessPurgeTimeout", UNSET)
+
         room_id = d.pop("roomId", UNSET)
 
         _video_codec = d.pop("videoCodec", UNSET)
         video_codec: Union[Unset, None, RoomConfigVideoCodec]
         if _video_codec is None:
             video_codec = None
         elif isinstance(_video_codec, Unset):
@@ -65,14 +72,15 @@
         else:
             video_codec = RoomConfigVideoCodec(_video_codec)
 
         webhook_url = d.pop("webhookUrl", UNSET)
 
         room_config = cls(
             max_peers=max_peers,
+            peerless_purge_timeout=peerless_purge_timeout,
             room_id=room_id,
             video_codec=video_codec,
             webhook_url=webhook_url,
         )
 
         room_config.additional_properties = d
         return room_config
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/room_create_details_response.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/healthcheck_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 if TYPE_CHECKING:
-    from ..models.room_create_details_response_data import RoomCreateDetailsResponseData
+    from ..models.health_report import HealthReport
 
 
-T = TypeVar("T", bound="RoomCreateDetailsResponse")
+T = TypeVar("T", bound="HealthcheckResponse")
 
 
 @_attrs_define
-class RoomCreateDetailsResponse:
-    """Response containing room details"""
+class HealthcheckResponse:
+    """Response containing health report of Jellyfish"""
 
-    data: "RoomCreateDetailsResponseData"
-    """"""
+    data: "HealthReport"
+    """Describes overall Jellyfish health"""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
     """@private"""
 
     def to_dict(self) -> Dict[str, Any]:
         """@private"""
         data = self.data.to_dict()
 
@@ -32,27 +32,25 @@
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """@private"""
-        from ..models.room_create_details_response_data import (
-            RoomCreateDetailsResponseData,
-        )
+        from ..models.health_report import HealthReport
 
         d = src_dict.copy()
-        data = RoomCreateDetailsResponseData.from_dict(d.pop("data"))
+        data = HealthReport.from_dict(d.pop("data"))
 
-        room_create_details_response = cls(
+        healthcheck_response = cls(
             data=data,
         )
 
-        room_create_details_response.additional_properties = d
-        return room_create_details_response
+        healthcheck_response.additional_properties = d
+        return healthcheck_response
 
     @property
     def additional_keys(self) -> List[str]:
         """@private"""
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/room_create_details_response_data.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/room_create_details_response_data.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/room_details_response.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/room_details_response.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/rooms_listing_response.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/rooms_listing_response.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/s3_credentials.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/s3_credentials.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/models/subscription_config.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/models/subscription_config.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_openapi_client/types.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_openapi_client/types.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/_ws_notifier.py` & `jellyfish_server_sdk-0.3.0/jellyfish/_ws_notifier.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/api/_base_api.py` & `jellyfish_server_sdk-0.3.0/jellyfish/api/_base_api.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/api/_recording_api.py` & `jellyfish_server_sdk-0.3.0/jellyfish/api/_recording_api.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/api/_room_api.py` & `jellyfish_server_sdk-0.3.0/jellyfish/api/_room_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 """
 RoomApi used to manage rooms
 """
 
-from typing import Literal, Union
+from typing import List, Literal, Tuple, Union
 
 from jellyfish._openapi_client.api.hls import subscribe_hls_to as hls_subscribe_hls_to
 from jellyfish._openapi_client.api.room import add_component as room_add_component
 from jellyfish._openapi_client.api.room import add_peer as room_add_peer
 from jellyfish._openapi_client.api.room import create_room as room_create_room
 from jellyfish._openapi_client.api.room import delete_component as room_delete_component
 from jellyfish._openapi_client.api.room import delete_peer as room_delete_peer
 from jellyfish._openapi_client.api.room import delete_room as room_delete_room
 from jellyfish._openapi_client.api.room import get_all_rooms as room_get_all_rooms
 from jellyfish._openapi_client.api.room import get_room as room_get_room
+from jellyfish._openapi_client.api.sip import dial as sip_dial
+from jellyfish._openapi_client.api.sip import end_call as sip_end_call
 from jellyfish._openapi_client.models import (
     AddComponentJsonBody,
     AddPeerJsonBody,
     ComponentFile,
     ComponentHLS,
     ComponentOptionsFile,
     ComponentOptionsHLS,
     ComponentOptionsRTSP,
+    ComponentOptionsSIP,
     ComponentRTSP,
+    ComponentSIP,
+    DialConfig,
     Peer,
     PeerOptionsWebRTC,
     Room,
     RoomConfig,
     RoomConfigVideoCodec,
     SubscriptionConfig,
 )
@@ -53,15 +58,15 @@
 
     def create_room(
         self,
         room_id: str = None,
         max_peers: int = None,
         video_codec: Literal["h264", "vp8"] = None,
         webhook_url: str = None,
-    ) -> (str, Room):
+    ) -> Tuple[str, Room]:
         """
         Creates a new room
 
         Returns a tuple (`jellyfish_address`, `Room`) - the address of the Jellyfish
         in which the room has been created and the created `Room`
 
         The returned address may be different from the current `RoomApi` instance.
@@ -95,22 +100,24 @@
         return self._request(room_get_all_rooms).data
 
     def get_room(self, room_id: str) -> Room:
         """Returns room with the given id"""
 
         return self._request(room_get_room, room_id=room_id).data
 
-    def add_peer(self, room_id: str, options: PeerOptionsWebRTC) -> (str, Peer):
+    def add_peer(self, room_id: str, options: PeerOptionsWebRTC) -> Tuple[str, Peer]:
         """
         Creates peer in the room
 
         Currently only `webrtc` peer is supported
 
         Returns a tuple (`peer_token`, `Peer`) - the token needed by Peer
-        to authenticate to Jellyfish and the new `Peer`
+        to authenticate to Jellyfish and the new `Peer`.
+
+        The possible options to pass for peer are `PeerOptionsWebRTC`.
         """
 
         peer_type = "webrtc"
         json_body = AddPeerJsonBody(type=peer_type, options=options)
 
         resp = self._request(room_add_peer, room_id=room_id, json_body=json_body)
         return (resp.data.token, resp.data.peer)
@@ -119,42 +126,56 @@
         """Deletes peer"""
 
         return self._request(room_delete_peer, id=peer_id, room_id=room_id)
 
     def add_component(
         self,
         room_id: str,
-        options: Union[ComponentOptionsFile, ComponentOptionsHLS, ComponentOptionsRTSP],
-    ) -> Union[ComponentFile, ComponentHLS, ComponentRTSP]:
-        """Creates component in the room"""
+        options: Union[
+            ComponentOptionsFile,
+            ComponentOptionsHLS,
+            ComponentOptionsRTSP,
+            ComponentOptionsSIP,
+        ],
+    ) -> Union[ComponentFile, ComponentHLS, ComponentRTSP, ComponentSIP]:
+        """
+        Creates component in the room.
+        Currently there are 4 different components:
+        * File Component for which the options are `ComponentOptionsFile`
+        * HLS Component which options are `ComponentOptionsHLS`
+        * RTSP Component which options are `ComponentOptionsRTSP`
+        * SIP Component which options are `ComponentOptionsSIP`
+        """
 
         if isinstance(options, ComponentOptionsFile):
             component_type = "file"
         elif isinstance(options, ComponentOptionsHLS):
             component_type = "hls"
         elif isinstance(options, ComponentOptionsRTSP):
             component_type = "rtsp"
+        elif isinstance(options, ComponentOptionsSIP):
+            component_type = "sip"
         else:
             raise ValueError(
-                "options must be ComponentFile, ComponentOptionsHLS"
-                "or ComponentOptionsRTSP"
+                "options must be ComponentOptionsFile, ComponentOptionsHLS,"
+                "ComponentOptionsRTSP or ComponentOptionsSIP"
             )
 
         json_body = AddComponentJsonBody(type=component_type, options=options)
 
         return self._request(
             room_add_component, room_id=room_id, json_body=json_body
         ).data
 
     def delete_component(self, room_id: str, component_id: str) -> None:
         """Deletes component"""
 
         return self._request(room_delete_component, id=component_id, room_id=room_id)
 
-    def hls_subscribe(self, room_id: str, origins: [str]):
+    def hls_subscribe(self, room_id: str, origins: List[str]):
         """
         In order to subscribe to HLS peers/components,
         the HLS component should be initialized with the subscribe_mode set to manual.
         This mode proves beneficial when you do not wish to record or stream
         all the available streams within a room via HLS.
         It allows for selective addition instead –
         you can manually select specific streams.
@@ -162,7 +183,36 @@
         """
 
         return self._request(
             hls_subscribe_hls_to,
             room_id=room_id,
             json_body=SubscriptionConfig(origins=origins),
         )
+
+    def sip_dial(self, room_id: str, component_id: str, phone_number: str):
+        """
+        Starts a phone call from a specified component to a provided phone number.
+
+        This is asynchronous operation.
+        In case of providing incorrect phone number you will receive
+        notification `ComponentCrashed`.
+        """
+
+        return self._request(
+            sip_dial,
+            room_id=room_id,
+            component_id=component_id,
+            json_body=DialConfig(phone_number=phone_number),
+        )
+
+    def sip_end_call(self, room_id: str, component_id: str):
+        """
+        End a phone call on a specified SIP component.
+
+        This is asynchronous operation.
+        """
+
+        return self._request(
+            sip_end_call,
+            room_id=room_id,
+            component_id=component_id,
+        )
```

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/errors.py` & `jellyfish_server_sdk-0.3.0/jellyfish/errors.py`

 * *Files identical despite different names*

### Comparing `jellyfish_server_sdk-0.2.0/jellyfish/events/__init__.py` & `jellyfish_server_sdk-0.3.0/jellyfish/events/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 """
-Server events being sent Jellyfish
+.. include:: ../../docs/server_notifications.md
 """
 
 # Exported messages
 from jellyfish.events._protos.jellyfish import (
     ServerMessageComponentCrashed,
     ServerMessageHlsPlayable,
     ServerMessageMetricsReport,
     ServerMessagePeerConnected,
     ServerMessagePeerCrashed,
     ServerMessagePeerDisconnected,
     ServerMessageRoomCrashed,
     ServerMessageRoomCreated,
     ServerMessageRoomDeleted,
+    ServerMessageTrack,
+    ServerMessageTrackAdded,
+    ServerMessageTrackMetadataUpdated,
+    ServerMessageTrackRemoved,
+    ServerMessageTrackType,
 )
 
 __all__ = [
+    "ServerMessageRoomCreated",
+    "ServerMessageRoomDeleted",
+    "ServerMessageRoomCrashed",
+    "ServerMessagePeerConnected",
+    "ServerMessagePeerDisconnected",
+    "ServerMessagePeerCrashed",
     "ServerMessageComponentCrashed",
+    "ServerMessageTrack",
+    "ServerMessageTrackType",
+    "ServerMessageTrackAdded",
+    "ServerMessageTrackMetadataUpdated",
+    "ServerMessageTrackRemoved",
     "ServerMessageHlsPlayable",
     "ServerMessageMetricsReport",
-    "ServerMessagePeerCrashed",
-    "ServerMessagePeerConnected",
-    "ServerMessagePeerDisconnected",
-    "ServerMessageRoomCrashed",
-    "ServerMessageRoomDeleted",
-    "ServerMessageRoomCreated",
 ]
```

### Comparing `jellyfish_server_sdk-0.2.0/pyproject.toml` & `jellyfish_server_sdk-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jellyfish-server-sdk"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python server SDK for the Jellyfish media server"
 authors = ["Jellyfish Team"]
 homepage = "https://github.com/jellyfish-dev/python-server-sdk"
 documentation = "https://jellyfish-dev.github.io/python-server-sdk/jellyfish"
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "jellyfish" }]
@@ -42,14 +42,15 @@
 local_test = "poetry_scripts:run_local_test"
 format = "poetry_scripts:run_formatter"
 format_check = "poetry_scripts:run_format_check"
 lint = "poetry_scripts:run_linter"
 fix_lint = "poetry_scripts:run_linter_fix"
 generate_docs = "poetry_scripts:generate_docs"
 update_client = "poetry_scripts:update_client"
+examples = "poetry_scripts:run_examples"
 
 [tool.ruff]
 select = ["F", "I"]
 
 [tool.ruff.lint]
 select = ["F", "I", "E"]
 ignore = []
```

### Comparing `jellyfish_server_sdk-0.2.0/PKG-INFO` & `jellyfish_server_sdk-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jellyfish-server-sdk
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python server SDK for the Jellyfish media server
 Home-page: https://github.com/jellyfish-dev/python-server-sdk
 License: Apache-2.0
 Author: Jellyfish Team
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -116,14 +116,37 @@
 
 asyncio.run(test_notifier())
 
 # Received a notification: ServerMessageRoomCreated(room_id='69a3fd1a-6a4d-47bc-ae54-0c72b0d05e29')
 # Received WebRTC metrics: ServerMessageMetricsReport(metrics='{}')
 ```
 
+#### Cluster of Jellyfishes
+
+The cluster of jellyfishes has got embedded load balancer, which means that a new room will be created on jellyfish with the least usage. At the moment to modify this specific room you must communicate with the jellyfish on which this room was created.
+
+```python
+room_api = RoomApi(server_address='localhost:5002')
+
+# Create a room to trigger a server notification with h264 as a codec,
+# that allow to use HLS.
+address, room = room_api.create_room(video_codec="h264")
+
+# Create new room api with returned jellyfish address as a room could be
+# created on a different jellyfish instance
+# (if you communicate with a cluster of jellyfishes)
+new_room_api = RoomApi(server_address=address)
+
+# Add HLS component with manual subscribe mode, we use here `new_room_api` as we are sure that this API refers to the jellyfish on which this room was created.
+_hls_component = new_room_api.add_component(
+    room.id,
+    ComponentOptionsHLS(subscribe_mode=ComponentOptionsHLSSubscribeMode.MANUAL),
+)
+```
+
 ## Testing
 
 You can test the SDK by running
 ```console
 poetry run ci_test
 ```
```

