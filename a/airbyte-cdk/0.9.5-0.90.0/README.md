# Comparing `tmp/airbyte-cdk-0.9.5.tar.gz` & `tmp/airbyte_cdk-0.90.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-cdk-0.9.5.tar", last modified: Fri Nov 18 17:17:27 2022, max compression
+gzip compressed data, was "airbyte_cdk-0.90.0.tar", max compression
```

## Comparing `airbyte-cdk-0.9.5.tar` & `airbyte_cdk-0.90.0.tar`

### file list

```diff
@@ -1,296 +1,292 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:27.002035 airbyte-cdk-0.9.5/
--rw-r--r--   0 root         (0) root         (0)     1051 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     4992 2022-11-18 17:17:27.002035 airbyte-cdk-0.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4105 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.966035 airbyte-cdk-0.9.5/airbyte_cdk/
--rw-r--r--   0 root         (0) root         (0)      262 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3548 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/connector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.966035 airbyte-cdk-0.9.5/airbyte_cdk/destinations/
--rw-r--r--   0 root         (0) root         (0)      126 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/destinations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5420 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/destinations/destination.py
--rw-r--r--   0 root         (0) root         (0)     6902 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     1125 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/exception_handler.py
--rw-r--r--   0 root         (0) root         (0)     3985 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.966035 airbyte-cdk-0.9.5/airbyte_cdk/models/
--rw-r--r--   0 root         (0) root         (0)      103 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18012 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/models/airbyte_protocol.py
--rw-r--r--   0 root         (0) root         (0)     2729 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/models/well_known_types.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.970035 airbyte-cdk-0.9.5/airbyte_cdk/sources/
--rw-r--r--   0 root         (0) root         (0)      218 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15181 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/abstract_source.py
--rw-r--r--   0 root         (0) root         (0)      856 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/config.py
--rw-r--r--   0 root         (0) root         (0)    10469 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/connector_state_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.970035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.970035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/auth/
--rw-r--r--   0 root         (0) root         (0)      201 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      745 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/auth/declarative_authenticator.py
--rw-r--r--   0 root         (0) root         (0)     5234 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/auth/oauth.py
--rw-r--r--   0 root         (0) root         (0)     4438 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/auth/token.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.970035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/checks/
--rw-r--r--   0 root         (0) root         (0)      274 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2469 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/checks/check_stream.py
--rw-r--r--   0 root         (0) root         (0)     1368 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/checks/connection_checker.py
--rw-r--r--   0 root         (0) root         (0)     3305 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/create_partial.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.970035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/datetime/
--rw-r--r--   0 root         (0) root         (0)      177 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/datetime/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1737 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/datetime/datetime_parser.py
--rw-r--r--   0 root         (0) root         (0)     4118 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/datetime/min_max_datetime.py
--rw-r--r--   0 root         (0) root         (0)     1452 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/declarative_source.py
--rw-r--r--   0 root         (0) root         (0)     6648 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/declarative_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.970035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/decoders/
--rw-r--r--   0 root         (0) root         (0)      247 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/decoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)      702 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/decoders/decoder.py
--rw-r--r--   0 root         (0) root         (0)      692 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/decoders/json_decoder.py
--rw-r--r--   0 root         (0) root         (0)      299 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.974035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/extractors/
--rw-r--r--   0 root         (0) root         (0)      478 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/extractors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2858 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/extractors/dpath_extractor.py
--rw-r--r--   0 root         (0) root         (0)     1178 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/extractors/http_selector.py
--rw-r--r--   0 root         (0) root         (0)      784 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/extractors/record_extractor.py
--rw-r--r--   0 root         (0) root         (0)     1428 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/extractors/record_filter.py
--rw-r--r--   0 root         (0) root         (0)     1787 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/extractors/record_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.974035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/
--rw-r--r--   0 root         (0) root         (0)      437 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1771 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/filters.py
--rw-r--r--   0 root         (0) root         (0)     1864 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/interpolated_boolean.py
--rw-r--r--   0 root         (0) root         (0)     1825 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/interpolated_mapping.py
--rw-r--r--   0 root         (0) root         (0)     2441 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/interpolated_string.py
--rw-r--r--   0 root         (0) root         (0)      929 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/interpolation.py
--rw-r--r--   0 root         (0) root         (0)     2634 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/jinja.py
--rw-r--r--   0 root         (0) root         (0)     2670 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/macros.py
--rw-r--r--   0 root         (0) root         (0)     9907 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/manifest_declarative_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.974035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/parsers/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/parsers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5073 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/parsers/class_types_registry.py
--rw-r--r--   0 root         (0) root         (0)     3767 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/parsers/default_implementation_registry.py
--rw-r--r--   0 root         (0) root         (0)    14466 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/parsers/factory.py
--rw-r--r--   0 root         (0) root         (0)     6115 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/parsers/manifest_reference_resolver.py
--rw-r--r--   0 root         (0) root         (0)      292 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/parsers/undefined_reference_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.974035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/
--rw-r--r--   0 root         (0) root         (0)      364 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.978035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/
--rw-r--r--   0 root         (0) root         (0)      717 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.978035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/
--rw-r--r--   0 root         (0) root         (0)      875 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1343 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/constant_backoff_strategy.py
--rw-r--r--   0 root         (0) root         (0)     1206 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/exponential_backoff_strategy.py
--rw-r--r--   0 root         (0) root         (0)     1125 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/header_helper.py
--rw-r--r--   0 root         (0) root         (0)     1520 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_time_from_header_backoff_strategy.py
--rw-r--r--   0 root         (0) root         (0)     2615 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_until_time_from_header_backoff_strategy.py
--rw-r--r--   0 root         (0) root         (0)      765 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategy.py
--rw-r--r--   0 root         (0) root         (0)     2349 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/composite_error_handler.py
--rw-r--r--   0 root         (0) root         (0)     5800 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/default_error_handler.py
--rw-r--r--   0 root         (0) root         (0)      989 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/error_handler.py
--rw-r--r--   0 root         (0) root         (0)     4610 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/http_response_filter.py
--rw-r--r--   0 root         (0) root         (0)      405 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/response_action.py
--rw-r--r--   0 root         (0) root         (0)     2595 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/response_status.py
--rw-r--r--   0 root         (0) root         (0)     7363 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/http_requester.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.978035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/
--rw-r--r--   0 root         (0) root         (0)      541 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6945 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/default_paginator.py
--rw-r--r--   0 root         (0) root         (0)     1908 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/no_pagination.py
--rw-r--r--   0 root         (0) root         (0)     1832 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/paginator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.978035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/strategies/
--rw-r--r--   0 root         (0) root         (0)      483 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/strategies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2971 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/strategies/cursor_pagination_strategy.py
--rw-r--r--   0 root         (0) root         (0)     1158 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/strategies/offset_increment.py
--rw-r--r--   0 root         (0) root         (0)     1130 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/strategies/page_increment.py
--rw-r--r--   0 root         (0) root         (0)     1023 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/strategies/pagination_strategy.py
--rw-r--r--   0 root         (0) root         (0)     1501 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/request_option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.978035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/request_options/
--rw-r--r--   0 root         (0) root         (0)      410 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/request_options/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2269 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_input_provider.py
--rw-r--r--   0 root         (0) root         (0)     4521 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_options_provider.py
--rw-r--r--   0 root         (0) root         (0)     2693 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/request_options/request_options_provider.py
--rw-r--r--   0 root         (0) root         (0)     5285 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/requester.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.978035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/retrievers/
--rw-r--r--   0 root         (0) root         (0)      269 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/retrievers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2098 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/retrievers/retriever.py
--rw-r--r--   0 root         (0) root         (0)    18891 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/retrievers/simple_retriever.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.982035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/schema/
--rw-r--r--   0 root         (0) root         (0)      404 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1838 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/schema/default_schema_loader.py
--rw-r--r--   0 root         (0) root         (0)     3949 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/schema/json_file_schema_loader.py
--rw-r--r--   0 root         (0) root         (0)      448 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/schema/schema_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.982035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/spec/
--rw-r--r--   0 root         (0) root         (0)      141 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/spec/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1246 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/spec/spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.982035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/
--rw-r--r--   0 root         (0) root         (0)      780 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4354 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/cartesian_product_stream_slicer.py
--rw-r--r--   0 root         (0) root         (0)    12046 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/datetime_stream_slicer.py
--rw-r--r--   0 root         (0) root         (0)     5046 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/list_stream_slicer.py
--rw-r--r--   0 root         (0) root         (0)     1910 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/single_slice.py
--rw-r--r--   0 root         (0) root         (0)     1597 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/stream_slicer.py
--rw-r--r--   0 root         (0) root         (0)     7125 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/substream_slicer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.982035 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/transformations/
--rw-r--r--   0 root         (0) root         (0)      919 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/transformations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4499 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/transformations/add_fields.py
--rw-r--r--   0 root         (0) root         (0)     2104 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/transformations/remove_fields.py
--rw-r--r--   0 root         (0) root         (0)     1162 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/transformations/transformation.py
--rw-r--r--   0 root         (0) root         (0)      482 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/types.py
--rw-r--r--   0 root         (0) root         (0)     1684 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/yaml_declarative_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.982035 airbyte-cdk-0.9.5/airbyte_cdk/sources/deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3524 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/deprecated/base_source.py
--rw-r--r--   0 root         (0) root         (0)     3560 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/deprecated/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.982035 airbyte-cdk-0.9.5/airbyte_cdk/sources/singer/
--rw-r--r--   0 root         (0) root         (0)      246 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/singer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15649 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/singer/singer_helpers.py
--rw-r--r--   0 root         (0) root         (0)     8526 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/singer/source.py
--rw-r--r--   0 root         (0) root         (0)     4279 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.982035 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/
--rw-r--r--   0 root         (0) root         (0)      176 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10007 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.986035 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/
--rw-r--r--   0 root         (0) root         (0)      261 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.986035 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/auth/
--rw-r--r--   0 root         (0) root         (0)      432 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      819 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/auth/core.py
--rw-r--r--   0 root         (0) root         (0)     3472 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/auth/oauth.py
--rw-r--r--   0 root         (0) root         (0)     1940 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/auth/token.py
--rw-r--r--   0 root         (0) root         (0)     1334 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    20382 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/http.py
--rw-r--r--   0 root         (0) root         (0)     2662 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/rate_limiting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.986035 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/requests_native_auth/
--rw-r--r--   0 root         (0) root         (0)      304 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/requests_native_auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4594 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_oauth.py
--rw-r--r--   0 root         (0) root         (0)      961 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_token.py
--rw-r--r--   0 root         (0) root         (0)     2555 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/requests_native_auth/oauth.py
--rw-r--r--   0 root         (0) root         (0)     2456 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/requests_native_auth/token.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.986035 airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/
--rw-r--r--   0 root         (0) root         (0)      118 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      244 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/casing.py
--rw-r--r--   0 root         (0) root         (0)      714 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/catalog_helpers.py
--rw-r--r--   0 root         (0) root         (0)     1702 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/record_helper.py
--rw-r--r--   0 root         (0) root         (0)     7428 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/schema_helpers.py
--rw-r--r--   0 root         (0) root         (0)     3151 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/schema_models.py
--rw-r--r--   0 root         (0) root         (0)     9488 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/transform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.986035 airbyte-cdk-0.9.5/airbyte_cdk/utils/
--rw-r--r--   0 root         (0) root         (0)      152 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2894 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/utils/airbyte_secrets_utils.py
--rw-r--r--   0 root         (0) root         (0)     2377 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/utils/event_timing.py
--rw-r--r--   0 root         (0) root         (0)     3216 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/airbyte_cdk/utils/traced_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.966035 airbyte-cdk-0.9.5/airbyte_cdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4992 2022-11-18 17:17:26.000000 airbyte-cdk-0.9.5/airbyte_cdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13724 2022-11-18 17:17:26.000000 airbyte-cdk-0.9.5/airbyte_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-18 17:17:26.000000 airbyte-cdk-0.9.5/airbyte_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      320 2022-11-18 17:17:26.000000 airbyte-cdk-0.9.5/airbyte_cdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2022-11-18 17:17:26.000000 airbyte-cdk-0.9.5/airbyte_cdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      145 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-18 17:17:27.002035 airbyte-cdk-0.9.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2208 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.966035 airbyte-cdk-0.9.5/unit_tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.986035 airbyte-cdk-0.9.5/unit_tests/destinations/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/destinations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10269 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/destinations/test_destination.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.990035 airbyte-cdk-0.9.5/unit_tests/singer/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/singer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1762 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/singer/test_singer_helpers.py
--rw-r--r--   0 root         (0) root         (0)     4442 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/singer/test_singer_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.990035 airbyte-cdk-0.9.5/unit_tests/sources/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.990035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.990035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/auth/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3395 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/auth/test_oauth.py
--rw-r--r--   0 root         (0) root         (0)     3666 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/auth/test_token_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.990035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/checks/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1783 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/checks/test_check_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.990035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/decoders/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/decoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)      590 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/decoders/test_json_decoder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.990035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/extractors/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/extractors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1765 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/extractors/test_dpath_extractor.py
--rw-r--r--   0 root         (0) root         (0)     2314 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/extractors/test_record_filter.py
--rw-r--r--   0 root         (0) root         (0)     3254 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/extractors/test_record_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.994035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/interpolation/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/interpolation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1472 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/interpolation/test_filters.py
--rw-r--r--   0 root         (0) root         (0)     1869 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/interpolation/test_interpolated_boolean.py
--rw-r--r--   0 root         (0) root         (0)     1350 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/interpolation/test_interpolated_mapping.py
--rw-r--r--   0 root         (0) root         (0)      884 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/interpolation/test_interpolated_string.py
--rw-r--r--   0 root         (0) root         (0)     2546 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/interpolation/test_jinja.py
--rw-r--r--   0 root         (0) root         (0)     1007 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/interpolation/test_macros.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.994035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/iterators/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/iterators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      380 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/iterators/test_only_once.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.994035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/parsers/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/parsers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4396 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/parsers/test_manifest_reference_resolver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.994035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.994035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.994035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/backoff_strategies/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/backoff_strategies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1505 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/backoff_strategies/test_constant_backoff.py
--rw-r--r--   0 root         (0) root         (0)     1281 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/backoff_strategies/test_exponential_backoff.py
--rw-r--r--   0 root         (0) root         (0)     1763 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/backoff_strategies/test_header_helper.py
--rw-r--r--   0 root         (0) root         (0)     1647 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/backoff_strategies/test_wait_time_from_header.py
--rw-r--r--   0 root         (0) root         (0)     3053 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/backoff_strategies/test_wait_until_time_from_header.py
--rw-r--r--   0 root         (0) root         (0)     3884 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/test_composite_error_handler.py
--rw-r--r--   0 root         (0) root         (0)     7224 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/test_default_error_handler.py
--rw-r--r--   0 root         (0) root         (0)     4408 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/test_http_response_filter.py
--rw-r--r--   0 root         (0) root         (0)     1971 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/error_handlers/test_response_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.998035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/paginators/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/paginators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2886 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/paginators/test_cursor_pagination_strategy.py
--rw-r--r--   0 root         (0) root         (0)     7516 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/paginators/test_default_paginator.py
--rw-r--r--   0 root         (0) root         (0)      332 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/paginators/test_no_paginator.py
--rw-r--r--   0 root         (0) root         (0)     1162 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/paginators/test_offset_increment.py
--rw-r--r--   0 root         (0) root         (0)     1148 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/paginators/test_page_increment.py
--rw-r--r--   0 root         (0) root         (0)     1576 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/paginators/test_request_option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.998035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/request_options/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/request_options/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5595 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/request_options/test_interpolated_request_options_provider.py
--rw-r--r--   0 root         (0) root         (0)     4411 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/test_http_requester.py
--rw-r--r--   0 root         (0) root         (0)     1682 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/requesters/test_interpolated_request_input_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.998035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/retrievers/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/retrievers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17096 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/retrievers/test_simple_retriever.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.998035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/schema/
--rw-r--r--   0 root         (0) root         (0)      134 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/schema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.998035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/schema/source_test/
--rw-r--r--   0 root         (0) root         (0)      118 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/schema/source_test/SourceTest.py
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/schema/source_test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1091 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/schema/test_default_schema_loader.py
--rw-r--r--   0 root         (0) root         (0)     1209 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/schema/test_json_file_schema_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.998035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/states/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/states/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.998035 airbyte-cdk-0.9.5/unit_tests/sources/declarative/stream_slicers/
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/stream_slicers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9277 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/stream_slicers/test_cartesian_product_stream_slicer.py
--rw-r--r--   0 root         (0) root         (0)    27258 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/stream_slicers/test_datetime_stream_slicer.py
--rw-r--r--   0 root         (0) root         (0)     5720 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/stream_slicers/test_list_stream_slicer.py
--rw-r--r--   0 root         (0) root         (0)    10479 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/stream_slicers/test_substream_slicer.py
--rw-r--r--   0 root         (0) root         (0)     2594 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/test_create_partial.py
--rw-r--r--   0 root         (0) root         (0)     2760 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/test_declarative_stream.py
--rw-r--r--   0 root         (0) root         (0)    37220 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/test_factory.py
--rw-r--r--   0 root         (0) root         (0)    35020 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/test_manifest_declarative_source.py
--rw-r--r--   0 root         (0) root         (0)     5100 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/declarative/test_yaml_declarative_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.998035 airbyte-cdk-0.9.5/unit_tests/sources/streams/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/streams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:26.998035 airbyte-cdk-0.9.5/unit_tests/sources/streams/http/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/streams/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:27.002035 airbyte-cdk-0.9.5/unit_tests/sources/streams/http/auth/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/streams/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5672 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/streams/http/auth/test_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:27.002035 airbyte-cdk-0.9.5/unit_tests/sources/streams/http/requests_native_auth/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/streams/http/requests_native_auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6899 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/streams/http/requests_native_auth/test_requests_native_auth.py
--rw-r--r--   0 root         (0) root         (0)    19656 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/streams/http/test_http.py
--rw-r--r--   0 root         (0) root         (0)     5059 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/streams/test_streams_core.py
--rw-r--r--   0 root         (0) root         (0)    37665 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/test_abstract_source.py
--rw-r--r--   0 root         (0) root         (0)     2477 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/test_config.py
--rw-r--r--   0 root         (0) root         (0)    24264 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/test_connector_state_manager.py
--rw-r--r--   0 root         (0) root         (0)    18420 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/sources/test_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 17:17:27.002035 airbyte-cdk-0.9.5/unit_tests/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4886 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/utils/test_secret_utils.py
--rw-r--r--   0 root         (0) root         (0)     4198 2022-11-18 17:15:12.000000 airbyte-cdk-0.9.5/unit_tests/utils/test_traced_exception.py
+-rw-r--r--   0        0        0     1051 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/LICENSE.txt
+-rw-r--r--   0        0        0     9977 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/README.md
+-rw-r--r--   0        0        0      339 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/__init__.py
+-rw-r--r--   0        0        0     3610 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/config_observation.py
+-rw-r--r--   0        0        0     4396 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/connector.py
+-rw-r--r--   0        0        0     1665 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/connector_builder/README.md
+-rw-r--r--   0        0        0       61 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/connector_builder/__init__.py
+-rw-r--r--   0        0        0     3958 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/connector_builder/connector_builder_handler.py
+-rw-r--r--   0        0        0     3365 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/connector_builder/main.py
+-rw-r--r--   0        0        0    17120 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/connector_builder/message_grouper.py
+-rw-r--r--   0        0        0     1420 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/connector_builder/models.py
+-rw-r--r--   0        0        0      126 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/destinations/__init__.py
+-rw-r--r--   0        0        0     5420 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/destinations/destination.py
+-rw-r--r--   0        0        0     2115 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/destinations/vector_db_based/README.md
+-rw-r--r--   0        0        0     1006 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/destinations/vector_db_based/__init__.py
+-rw-r--r--   0        0        0    12324 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/destinations/vector_db_based/config.py
+-rw-r--r--   0        0        0     9081 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/destinations/vector_db_based/document_processor.py
+-rw-r--r--   0        0        0    11443 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/destinations/vector_db_based/embedder.py
+-rw-r--r--   0        0        0     3243 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/destinations/vector_db_based/indexer.py
+-rw-r--r--   0        0        0     1807 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/destinations/vector_db_based/test_utils.py
+-rw-r--r--   0        0        0     1073 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/destinations/vector_db_based/utils.py
+-rw-r--r--   0        0        0     4394 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/destinations/vector_db_based/writer.py
+-rw-r--r--   0        0        0    14978 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/entrypoint.py
+-rw-r--r--   0        0        0     1930 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/exception_handler.py
+-rw-r--r--   0        0        0     3985 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/logger.py
+-rw-r--r--   0        0        0     1708 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/models/__init__.py
+-rw-r--r--   0        0        0      100 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/models/airbyte_protocol.py
+-rw-r--r--   0        0        0      117 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/models/well_known_types.py
+-rw-r--r--   0        0        0        0 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/py.typed
+-rw-r--r--   0        0        0     1141 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/__init__.py
+-rw-r--r--   0        0        0    14428 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/abstract_source.py
+-rw-r--r--   0        0        0       61 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/concurrent_source/__init__.py
+-rw-r--r--   0        0        0    11976 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/concurrent_source/concurrent_read_processor.py
+-rw-r--r--   0        0        0     8750 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/concurrent_source/concurrent_source.py
+-rw-r--r--   0        0        0     3691 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/concurrent_source/concurrent_source_adapter.py
+-rw-r--r--   0        0        0      696 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/concurrent_source/partition_generation_completed_sentinel.py
+-rw-r--r--   0        0        0      764 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/concurrent_source/stream_thread_exception.py
+-rw-r--r--   0        0        0     5076 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/concurrent_source/thread_pool_manager.py
+-rw-r--r--   0        0        0      856 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/config.py
+-rw-r--r--   0        0        0     9903 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/connector_state_manager.py
+-rw-r--r--   0        0        0       61 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/__init__.py
+-rw-r--r--   0        0        0      294 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/auth/__init__.py
+-rw-r--r--   0        0        0     1090 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/auth/declarative_authenticator.py
+-rw-r--r--   0        0        0     8007 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/auth/jwt.py
+-rw-r--r--   0        0        0     8272 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/auth/oauth.py
+-rw-r--r--   0        0        0     1347 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/auth/selective_authenticator.py
+-rw-r--r--   0        0        0    11032 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/auth/token.py
+-rw-r--r--   0        0        0     2887 2024-05-17 05:27:46.738706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/auth/token_provider.py
+-rw-r--r--   0        0        0      274 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/checks/__init__.py
+-rw-r--r--   0        0        0     2154 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/checks/check_stream.py
+-rw-r--r--   0        0        0     1368 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/checks/connection_checker.py
+-rw-r--r--   0        0        0      177 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/datetime/__init__.py
+-rw-r--r--   0        0        0     2369 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/datetime/datetime_parser.py
+-rw-r--r--   0        0        0     5187 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/datetime/min_max_datetime.py
+-rw-r--r--   0        0        0    97462 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/declarative_component_schema.yaml
+-rw-r--r--   0        0        0     1517 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/declarative_source.py
+-rw-r--r--   0        0        0     7495 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/declarative_stream.py
+-rw-r--r--   0        0        0      247 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/decoders/__init__.py
+-rw-r--r--   0        0        0      639 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/decoders/decoder.py
+-rw-r--r--   0        0        0      637 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/decoders/json_decoder.py
+-rw-r--r--   0        0        0      176 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/exceptions.py
+-rw-r--r--   0        0        0      478 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/extractors/__init__.py
+-rw-r--r--   0        0        0     2990 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/extractors/dpath_extractor.py
+-rw-r--r--   0        0        0     1213 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/extractors/http_selector.py
+-rw-r--r--   0        0        0      691 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/extractors/record_extractor.py
+-rw-r--r--   0        0        0     1421 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/extractors/record_filter.py
+-rw-r--r--   0        0        0     4671 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/extractors/record_selector.py
+-rw-r--r--   0        0        0      459 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/incremental/__init__.py
+-rw-r--r--   0        0        0    18380 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/incremental/datetime_based_cursor.py
+-rw-r--r--   0        0        0      536 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/incremental/declarative_cursor.py
+-rw-r--r--   0        0        0    12286 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/incremental/per_partition_cursor.py
+-rw-r--r--   0        0        0      437 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/__init__.py
+-rw-r--r--   0        0        0     3331 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/filters.py
+-rw-r--r--   0        0        0     1844 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/interpolated_boolean.py
+-rw-r--r--   0        0        0     2018 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/interpolated_mapping.py
+-rw-r--r--   0        0        0     1791 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/interpolated_nested_mapping.py
+-rw-r--r--   0        0        0     2443 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/interpolated_string.py
+-rw-r--r--   0        0        0      934 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/interpolation.py
+-rw-r--r--   0        0        0     5367 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/jinja.py
+-rw-r--r--   0        0        0     3556 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/macros.py
+-rw-r--r--   0        0        0    12253 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/manifest_declarative_source.py
+-rw-r--r--   0        0        0        0 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/migrations/__init__.py
+-rw-r--r--   0        0        0     3729 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/migrations/legacy_to_per_partition_state_migration.py
+-rw-r--r--   0        0        0      794 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/migrations/state_migration.py
+-rw-r--r--   0        0        0       93 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/models/__init__.py
+-rw-r--r--   0        0        0    65245 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/models/declarative_component_schema.py
+-rw-r--r--   0        0        0       61 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/parsers/__init__.py
+-rw-r--r--   0        0        0     6204 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/parsers/class_types_registry.py
+-rw-r--r--   0        0        0      553 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/parsers/custom_exceptions.py
+-rw-r--r--   0        0        0     3801 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/parsers/default_implementation_registry.py
+-rw-r--r--   0        0        0     8287 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/parsers/manifest_component_transformer.py
+-rw-r--r--   0        0        0     6728 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/parsers/manifest_reference_resolver.py
+-rw-r--r--   0        0        0    63618 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/parsers/model_to_component_factory.py
+-rw-r--r--   0        0        0      476 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/partition_routers/__init__.py
+-rw-r--r--   0        0        0     4312 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/partition_routers/list_partition_router.py
+-rw-r--r--   0        0        0     1599 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/partition_routers/single_partition_router.py
+-rw-r--r--   0        0        0     7952 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/partition_routers/substream_partition_router.py
+-rw-r--r--   0        0        0      364 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/__init__.py
+-rw-r--r--   0        0        0      717 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/__init__.py
+-rw-r--r--   0        0        0      875 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/__init__.py
+-rw-r--r--   0        0        0     1571 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/constant_backoff_strategy.py
+-rw-r--r--   0        0        0     1366 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/exponential_backoff_strategy.py
+-rw-r--r--   0        0        0     1156 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/header_helper.py
+-rw-r--r--   0        0        0     1816 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_time_from_header_backoff_strategy.py
+-rw-r--r--   0        0        0     2803 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_until_time_from_header_backoff_strategy.py
+-rw-r--r--   0        0        0      697 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategy.py
+-rw-r--r--   0        0        0     2476 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/composite_error_handler.py
+-rw-r--r--   0        0        0     6041 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/default_error_handler.py
+-rw-r--r--   0        0        0     1141 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/error_handler.py
+-rw-r--r--   0        0        0     4979 2024-05-17 05:27:46.742706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/http_response_filter.py
+-rw-r--r--   0        0        0      405 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/response_action.py
+-rw-r--r--   0        0        0     2656 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/response_status.py
+-rw-r--r--   0        0        0    27968 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/http_requester.py
+-rw-r--r--   0        0        0      599 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/__init__.py
+-rw-r--r--   0        0        0    10305 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/default_paginator.py
+-rw-r--r--   0        0        0     1877 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/no_pagination.py
+-rw-r--r--   0        0        0     1927 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/paginator.py
+-rw-r--r--   0        0        0      740 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/__init__.py
+-rw-r--r--   0        0        0     3445 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/cursor_pagination_strategy.py
+-rw-r--r--   0        0        0     2887 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/offset_increment.py
+-rw-r--r--   0        0        0     2152 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/page_increment.py
+-rw-r--r--   0        0        0     1240 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/pagination_strategy.py
+-rw-r--r--   0        0        0     1967 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/stop_condition.py
+-rw-r--r--   0        0        0     1055 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/request_option.py
+-rw-r--r--   0        0        0      410 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/request_options/__init__.py
+-rw-r--r--   0        0        0     2275 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_nested_request_input_provider.py
+-rw-r--r--   0        0        0     2883 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_input_provider.py
+-rw-r--r--   0        0        0     4995 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_options_provider.py
+-rw-r--r--   0        0        0     2590 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/request_options/request_options_provider.py
+-rw-r--r--   0        0        0      299 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/request_path.py
+-rw-r--r--   0        0        0     5539 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/requester.py
+-rw-r--r--   0        0        0      339 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/retrievers/__init__.py
+-rw-r--r--   0        0        0     1741 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/retrievers/retriever.py
+-rw-r--r--   0        0        0    19727 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/retrievers/simple_retriever.py
+-rw-r--r--   0        0        0      517 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/schema/__init__.py
+-rw-r--r--   0        0        0     1790 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/schema/default_schema_loader.py
+-rw-r--r--   0        0        0      464 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/schema/inline_schema_loader.py
+-rw-r--r--   0        0        0     4150 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/schema/json_file_schema_loader.py
+-rw-r--r--   0        0        0      379 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/schema/schema_loader.py
+-rw-r--r--   0        0        0      141 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/spec/__init__.py
+-rw-r--r--   0        0        0     1786 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/spec/spec.py
+-rw-r--r--   0        0        0      328 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/stream_slicers/__init__.py
+-rw-r--r--   0        0        0     4721 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/stream_slicers/cartesian_product_stream_slicer.py
+-rw-r--r--   0        0        0      856 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/stream_slicers/stream_slicer.py
+-rw-r--r--   0        0        0      919 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/transformations/__init__.py
+-rw-r--r--   0        0        0     4884 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/transformations/add_fields.py
+-rw-r--r--   0        0        0     2725 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/transformations/remove_fields.py
+-rw-r--r--   0        0        0     1123 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/transformations/transformation.py
+-rw-r--r--   0        0        0      749 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/types.py
+-rw-r--r--   0        0        0     1879 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/yaml_declarative_source.py
+-rw-r--r--   0        0        0       61 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/embedded/__init__.py
+-rw-r--r--   0        0        0     2264 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/embedded/base_integration.py
+-rw-r--r--   0        0        0     1571 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/embedded/catalog.py
+-rw-r--r--   0        0        0     1390 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/embedded/runner.py
+-rw-r--r--   0        0        0      744 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/embedded/tools.py
+-rw-r--r--   0        0        0    11085 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/__init__.py
+-rw-r--r--   0        0        0      371 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/availability_strategy/__init__.py
+-rw-r--r--   0        0        0     2137 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/availability_strategy/abstract_file_based_availability_strategy.py
+-rw-r--r--   0        0        0     5289 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/availability_strategy/default_file_based_availability_strategy.py
+-rw-r--r--   0        0        0        0 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/config/__init__.py
+-rw-r--r--   0        0        0     4956 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/config/abstract_file_based_spec.py
+-rw-r--r--   0        0        0      712 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/config/avro_format.py
+-rw-r--r--   0        0        0     7804 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/config/csv_format.py
+-rw-r--r--   0        0        0     4229 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/config/file_based_stream_config.py
+-rw-r--r--   0        0        0      374 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/config/jsonl_format.py
+-rw-r--r--   0        0        0      737 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/config/parquet_format.py
+-rw-r--r--   0        0        0     3513 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/config/unstructured_format.py
+-rw-r--r--   0        0        0      283 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/discovery_policy/__init__.py
+-rw-r--r--   0        0        0      621 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/discovery_policy/abstract_discovery_policy.py
+-rw-r--r--   0        0        0      939 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/discovery_policy/default_discovery_policy.py
+-rw-r--r--   0        0        0     5613 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/exceptions.py
+-rw-r--r--   0        0        0    13784 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/file_based_source.py
+-rw-r--r--   0        0        0     3749 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/file_based_stream_reader.py
+-rw-r--r--   0        0        0     1017 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/file_types/__init__.py
+-rw-r--r--   0        0        0     9167 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/file_types/avro_parser.py
+-rw-r--r--   0        0        0    19461 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/file_types/csv_parser.py
+-rw-r--r--   0        0        0     2819 2024-05-17 05:27:46.746706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/file_types/file_type_parser.py
+-rw-r--r--   0        0        0     5666 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/file_types/jsonl_parser.py
+-rw-r--r--   0        0        0     9998 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/file_types/parquet_parser.py
+-rw-r--r--   0        0        0    16736 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/file_types/unstructured_parser.py
+-rw-r--r--   0        0        0      312 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/remote_file.py
+-rw-r--r--   0        0        0     9291 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/schema_helpers.py
+-rw-r--r--   0        0        0      527 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/schema_validation_policies/__init__.py
+-rw-r--r--   0        0        0      604 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/schema_validation_policies/abstract_schema_validation_policy.py
+-rw-r--r--   0        0        0     1643 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/schema_validation_policies/default_schema_validation_policies.py
+-rw-r--r--   0        0        0      265 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/stream/__init__.py
+-rw-r--r--   0        0        0     6557 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/stream/abstract_file_based_stream.py
+-rw-r--r--   0        0        0        0 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/stream/concurrent/__init__.py
+-rw-r--r--   0        0        0    12818 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/stream/concurrent/adapters.py
+-rw-r--r--   0        0        0      329 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/stream/concurrent/cursor/__init__.py
+-rw-r--r--   0        0        0     1961 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/stream/concurrent/cursor/abstract_concurrent_file_based_cursor.py
+-rw-r--r--   0        0        0    14331 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/stream/concurrent/cursor/file_based_concurrent_cursor.py
+-rw-r--r--   0        0        0     3150 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/stream/concurrent/cursor/file_based_final_state_cursor.py
+-rw-r--r--   0        0        0      191 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/stream/cursor/__init__.py
+-rw-r--r--   0        0        0     1920 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/stream/cursor/abstract_file_based_cursor.py
+-rw-r--r--   0        0        0     6815 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/stream/cursor/default_file_based_cursor.py
+-rw-r--r--   0        0        0    13113 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/stream/default_file_based_stream.py
+-rw-r--r--   0        0        0      218 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/file_based/types.py
+-rw-r--r--   0        0        0      730 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/http_config.py
+-rw-r--r--   0        0        0     1437 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/http_logger.py
+-rw-r--r--   0        0        0      372 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/message/__init__.py
+-rw-r--r--   0        0        0     4583 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/message/repository.py
+-rw-r--r--   0        0        0     4412 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/source.py
+-rw-r--r--   0        0        0      256 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/__init__.py
+-rw-r--r--   0        0        0     1007 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/availability_strategy.py
+-rw-r--r--   0        0        0    20555 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/call_rate.py
+-rw-r--r--   0        0        0      408 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/checkpoint/__init__.py
+-rw-r--r--   0        0        0     4893 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/checkpoint/checkpoint_reader.py
+-rw-r--r--   0        0        0     2946 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/checkpoint/cursor.py
+-rw-r--r--   0        0        0     1070 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/README.md
+-rw-r--r--   0        0        0       61 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/__init__.py
+-rw-r--r--   0        0        0     3792 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/abstract_stream.py
+-rw-r--r--   0        0        0     1358 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/abstract_stream_facade.py
+-rw-r--r--   0        0        0    16279 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/adapters.py
+-rw-r--r--   0        0        0     2013 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/availability_strategy.py
+-rw-r--r--   0        0        0    15155 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/cursor.py
+-rw-r--r--   0        0        0     3059 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/default_stream.py
+-rw-r--r--   0        0        0      468 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/exceptions.py
+-rw-r--r--   0        0        0     1290 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/helpers.py
+-rw-r--r--   0        0        0     3315 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/partition_enqueuer.py
+-rw-r--r--   0        0        0     1747 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/partition_reader.py
+-rw-r--r--   0        0        0       61 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/partitions/__init__.py
+-rw-r--r--   0        0        0     1795 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/partitions/partition.py
+-rw-r--r--   0        0        0      441 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/partitions/partition_generator.py
+-rw-r--r--   0        0        0      600 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/partitions/record.py
+-rw-r--r--   0        0        0     1182 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/partitions/types.py
+-rw-r--r--   0        0        0        0 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/state_converters/__init__.py
+-rw-r--r--   0        0        0     5539 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/state_converters/abstract_stream_state_converter.py
+-rw-r--r--   0        0        0     5504 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/concurrent/state_converters/datetime_stream_state_converter.py
+-rw-r--r--   0        0        0    22387 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/core.py
+-rw-r--r--   0        0        0      311 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/__init__.py
+-rw-r--r--   0        0        0      432 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/auth/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/auth/core.py
+-rw-r--r--   0        0        0     4135 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/auth/oauth.py
+-rw-r--r--   0        0        0     1940 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/auth/token.py
+-rw-r--r--   0        0        0     6884 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/availability_strategy.py
+-rw-r--r--   0        0        0      665 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/error_handlers/__init__.py
+-rw-r--r--   0        0        0      826 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/error_handlers/backoff_strategy.py
+-rw-r--r--   0        0        0      991 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/error_handlers/default_backoff_strategy.py
+-rw-r--r--   0        0        0      781 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/error_handlers/error_handler.py
+-rw-r--r--   0        0        0      456 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/error_handlers/error_message_parser.py
+-rw-r--r--   0        0        0     6172 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/error_handlers/http_status_error_handler.py
+-rw-r--r--   0        0        0     1491 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/error_handlers/json_error_message_parser.py
+-rw-r--r--   0        0        0      476 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/error_handlers/response_models.py
+-rw-r--r--   0        0        0     1743 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/exceptions.py
+-rw-r--r--   0        0        0    24534 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/http.py
+-rw-r--r--   0        0        0    11292 2024-05-17 05:27:46.750706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/http_client.py
+-rw-r--r--   0        0        0     5258 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/rate_limiting.py
+-rw-r--r--   0        0        0      413 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/requests_native_auth/__init__.py
+-rw-r--r--   0        0        0    10125 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_oauth.py
+-rw-r--r--   0        0        0      961 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_token.py
+-rw-r--r--   0        0        0    13381 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/requests_native_auth/oauth.py
+-rw-r--r--   0        0        0     2456 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/requests_native_auth/token.py
+-rw-r--r--   0        0        0       61 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/utils/__init__.py
+-rw-r--r--   0        0        0     1645 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/utils/stream_helper.py
+-rw-r--r--   0        0        0     3588 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/types.py
+-rw-r--r--   0        0        0      118 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/__init__.py
+-rw-r--r--   0        0        0      256 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/casing.py
+-rw-r--r--   0        0        0      714 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/catalog_helpers.py
+-rw-r--r--   0        0        0     1711 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/record_helper.py
+-rw-r--r--   0        0        0     8483 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/schema_helpers.py
+-rw-r--r--   0        0        0     3151 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/schema_models.py
+-rw-r--r--   0        0        0     1731 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/slice_logger.py
+-rw-r--r--   0        0        0     9493 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/transform.py
+-rw-r--r--   0        0        0      175 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/types.py
+-rw-r--r--   0        0        0      199 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/test/__init__.py
+-rw-r--r--   0        0        0     2691 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/test/catalog_builder.py
+-rw-r--r--   0        0        0     7399 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/test/entrypoint_wrapper.py
+-rw-r--r--   0        0        0      322 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/test/mock_http/__init__.py
+-rw-r--r--   0        0        0     1240 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/test/mock_http/matcher.py
+-rw-r--r--   0        0        0     6412 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/test/mock_http/mocker.py
+-rw-r--r--   0        0        0     3687 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/test/mock_http/request.py
+-rw-r--r--   0        0        0      588 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/test/mock_http/response.py
+-rw-r--r--   0        0        0     7789 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/test/mock_http/response_builder.py
+-rw-r--r--   0        0        0      609 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/test/state_builder.py
+-rw-r--r--   0        0        0      294 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/__init__.py
+-rw-r--r--   0        0        0     3079 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/airbyte_secrets_utils.py
+-rw-r--r--   0        0        0      598 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/analytics_message.py
+-rw-r--r--   0        0        0      108 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/constants.py
+-rw-r--r--   0        0        0     3954 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/datetime_format_inferrer.py
+-rw-r--r--   0        0        0     2377 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/event_timing.py
+-rw-r--r--   0        0        0      574 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/is_cloud_environment.py
+-rw-r--r--   0        0        0     1729 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/mapping_helpers.py
+-rw-r--r--   0        0        0      953 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/message_utils.py
+-rw-r--r--   0        0        0     1180 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/oneof_option_config.py
+-rw-r--r--   0        0        0     8622 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/schema_inferrer.py
+-rw-r--r--   0        0        0      741 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/spec_schema_transformations.py
+-rw-r--r--   0        0        0      971 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/stream_status_utils.py
+-rw-r--r--   0        0        0     5245 2024-05-17 05:27:46.754706 airbyte_cdk-0.90.0/airbyte_cdk/utils/traced_exception.py
+-rw-r--r--   0        0        0     4085 2024-05-17 05:27:46.758706 airbyte_cdk-0.90.0/pyproject.toml
+-rw-r--r--   0        0        0    12798 1970-01-01 00:00:00.000000 airbyte_cdk-0.90.0/PKG-INFO
```

### Comparing `airbyte-cdk-0.9.5/LICENSE.txt` & `airbyte_cdk-0.90.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/connector.py` & `airbyte_cdk-0.90.0/airbyte_cdk/connector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 import json
 import logging
 import os
 import pkgutil
 from abc import ABC, abstractmethod
-from typing import Any, Generic, Mapping, Optional, Protocol, TypeVar
+from typing import Any, Generic, List, Mapping, Optional, Protocol, TypeVar, Union
 
 import yaml
 from airbyte_cdk.models import AirbyteConnectionStatus, ConnectorSpecification
 
 
 def load_optional_package_file(package: str, filename: str) -> Optional[bytes]:
     """Gets a resource from a package, returning None if it does not exist"""
@@ -43,18 +43,32 @@
     @abstractmethod
     def configure(self, config: Mapping[str, Any], temp_dir: str) -> TConfig:
         """
         Persist config in temporary directory to run the Source job
         """
 
     @staticmethod
-    def read_config(config_path: str) -> TConfig:
-        with open(config_path, "r") as file:
+    def read_config(config_path: str) -> Mapping[str, Any]:
+        config = BaseConnector._read_json_file(config_path)
+        if isinstance(config, Mapping):
+            return config
+        else:
+            raise ValueError(
+                f"The content of {config_path} is not an object and therefore is not a valid config. Please ensure the file represent a config."
+            )
+
+    @staticmethod
+    def _read_json_file(file_path: str) -> Union[None, bool, float, int, str, List[Any], Mapping[str, Any]]:
+        with open(file_path, "r") as file:
             contents = file.read()
-        return json.loads(contents)
+
+        try:
+            return json.loads(contents)
+        except json.JSONDecodeError as error:
+            raise ValueError(f"Could not read json file {file_path}: {error}. Please ensure that it is a valid JSON.")
 
     @staticmethod
     def write_config(config: TConfig, config_path: str):
         with open(config_path, "w") as fh:
             fh.write(json.dumps(config))
 
     def spec(self, logger: logging.Logger) -> ConnectorSpecification:
@@ -70,15 +84,18 @@
 
         if yaml_spec and json_spec:
             raise RuntimeError("Found multiple spec files in the package. Only one of spec.yaml or spec.json should be provided.")
 
         if yaml_spec:
             spec_obj = yaml.load(yaml_spec, Loader=yaml.SafeLoader)
         elif json_spec:
-            spec_obj = json.loads(json_spec)
+            try:
+                spec_obj = json.loads(json_spec)
+            except json.JSONDecodeError as error:
+                raise ValueError(f"Could not read json spec file: {error}. Please ensure that it is a valid JSON.")
         else:
             raise FileNotFoundError("Unable to find spec.yaml or spec.json in the package.")
 
         return ConnectorSpecification.parse_obj(spec_obj)
 
     @abstractmethod
     def check(self, logger: logging.Logger, config: TConfig) -> AirbyteConnectionStatus:
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/destinations/destination.py` & `airbyte_cdk-0.90.0/airbyte_cdk/destinations/destination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import argparse
 import io
 import logging
 import sys
 from abc import ABC, abstractmethod
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/logger.py` & `airbyte_cdk-0.90.0/airbyte_cdk/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import json
 import logging
 import logging.config
 import traceback
 from typing import Tuple
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/config.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from typing import Any, Dict
 
 from airbyte_cdk.sources.utils.schema_helpers import expand_refs, rename_key
 from pydantic import BaseModel
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/connector_state_manager.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/connector_state_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import copy
 from typing import Any, List, Mapping, MutableMapping, Optional, Tuple, Union
 
-from airbyte_cdk.models import AirbyteMessage, AirbyteStateBlob, AirbyteStateMessage, AirbyteStateType, AirbyteStreamState, StreamDescriptor
+from airbyte_cdk.models import (
+    AirbyteMessage,
+    AirbyteStateBlob,
+    AirbyteStateMessage,
+    AirbyteStateType,
+    AirbyteStream,
+    AirbyteStreamState,
+    StreamDescriptor,
+)
 from airbyte_cdk.models import Type as MessageType
 from airbyte_cdk.sources.streams import Stream
 from pydantic import Extra
 
 
 class HashableStreamDescriptor(StreamDescriptor):
     """
@@ -24,82 +32,80 @@
 
 class ConnectorStateManager:
     """
     ConnectorStateManager consolidates the various forms of a stream's incoming state message (STREAM / GLOBAL / LEGACY) under a common
     interface. It also provides methods to extract and update state
     """
 
-    def __init__(self, stream_instance_map: Mapping[str, Stream], state: Union[List[AirbyteStateMessage], MutableMapping[str, Any]] = None):
+    def __init__(
+        self,
+        stream_instance_map: Mapping[str, Union[Stream, AirbyteStream]],
+        state: Optional[Union[List[AirbyteStateMessage], MutableMapping[str, Any]]] = None,
+    ):
         shared_state, per_stream_states = self._extract_from_state_message(state, stream_instance_map)
 
         # We explicitly throw an error if we receive a GLOBAL state message that contains a shared_state because API sources are
         # designed to checkpoint state independently of one another. API sources should never be emitting a state message where
         # shared_state is populated. Rather than define how to handle shared_state without a clear use case, we're opting to throw an
         # error instead and if/when we find one, we will then implement processing of the shared_state value.
         if shared_state:
             raise ValueError(
                 "Received a GLOBAL AirbyteStateMessage that contains a shared_state. This library only ever generates per-STREAM "
                 "STATE messages so this was not generated by this connector. This must be an orchestrator or platform error. GLOBAL "
                 "state messages with shared_state will not be processed correctly. "
             )
         self.per_stream_states = per_stream_states
 
-    def get_stream_state(self, stream_name: str, namespace: Optional[str]) -> Mapping[str, Any]:
+    def get_stream_state(self, stream_name: str, namespace: Optional[str]) -> MutableMapping[str, Any]:
         """
         Retrieves the state of a given stream based on its descriptor (name + namespace).
         :param stream_name: Name of the stream being fetched
         :param namespace: Namespace of the stream being fetched
         :return: The per-stream state for a stream
         """
         stream_state = self.per_stream_states.get(HashableStreamDescriptor(name=stream_name, namespace=namespace))
         if stream_state:
-            return stream_state.dict()
+            return stream_state.dict()  # type: ignore # mypy thinks dict() returns any, but it returns a dict
         return {}
 
-    def update_state_for_stream(self, stream_name: str, namespace: Optional[str], value: Mapping[str, Any]):
+    def update_state_for_stream(self, stream_name: str, namespace: Optional[str], value: Mapping[str, Any]) -> None:
         """
         Overwrites the state blob of a specific stream based on the provided stream name and optional namespace
         :param stream_name: The name of the stream whose state is being updated
         :param namespace: The namespace of the stream if it exists
         :param value: A stream state mapping that is being updated for a stream
         """
         stream_descriptor = HashableStreamDescriptor(name=stream_name, namespace=namespace)
         self.per_stream_states[stream_descriptor] = AirbyteStateBlob.parse_obj(value)
 
-    def create_state_message(self, stream_name: str, namespace: Optional[str], send_per_stream_state: bool) -> AirbyteMessage:
+    def create_state_message(self, stream_name: str, namespace: Optional[str]) -> AirbyteMessage:
         """
         Generates an AirbyteMessage using the current per-stream state of a specified stream in either the per-stream or legacy format
         :param stream_name: The name of the stream for the message that is being created
         :param namespace: The namespace of the stream for the message that is being created
-        :param send_per_stream_state: Decides which state format the message should be generated as
         :return: The Airbyte state message to be emitted by the connector during a sync
         """
-        if send_per_stream_state:
-            hashable_descriptor = HashableStreamDescriptor(name=stream_name, namespace=namespace)
-            stream_state = self.per_stream_states.get(hashable_descriptor) or AirbyteStateBlob()
-
-            # According to the Airbyte protocol, the StreamDescriptor namespace field is not required. However, the platform will throw
-            # a validation error if it receives namespace=null. That is why if namespace is None, the field should be omitted instead.
-            stream_descriptor = (
-                StreamDescriptor(name=stream_name) if namespace is None else StreamDescriptor(name=stream_name, namespace=namespace)
-            )
+        hashable_descriptor = HashableStreamDescriptor(name=stream_name, namespace=namespace)
+        stream_state = self.per_stream_states.get(hashable_descriptor) or AirbyteStateBlob()
 
-            return AirbyteMessage(
-                type=MessageType.STATE,
-                state=AirbyteStateMessage(
-                    type=AirbyteStateType.STREAM,
-                    stream=AirbyteStreamState(stream_descriptor=stream_descriptor, stream_state=stream_state),
-                    data=dict(self._get_legacy_state()),
+        return AirbyteMessage(
+            type=MessageType.STATE,
+            state=AirbyteStateMessage(
+                type=AirbyteStateType.STREAM,
+                stream=AirbyteStreamState(
+                    stream_descriptor=StreamDescriptor(name=stream_name, namespace=namespace), stream_state=stream_state
                 ),
-            )
-        return AirbyteMessage(type=MessageType.STATE, state=AirbyteStateMessage(data=dict(self._get_legacy_state())))
+            ),
+        )
 
     @classmethod
     def _extract_from_state_message(
-        cls, state: Union[List[AirbyteStateMessage], MutableMapping[str, Any]], stream_instance_map: Mapping[str, Stream]
+        cls,
+        state: Optional[Union[List[AirbyteStateMessage], MutableMapping[str, Any]]],
+        stream_instance_map: Mapping[str, Union[Stream, AirbyteStream]],
     ) -> Tuple[Optional[AirbyteStateBlob], MutableMapping[HashableStreamDescriptor, Optional[AirbyteStateBlob]]]:
         """
         Takes an incoming list of state messages or the legacy state format and extracts state attributes according to type
         which can then be assigned to the new state manager being instantiated
         :param state: The incoming state input
         :return: A tuple of shared state and per stream state assembled from the incoming state list
         """
@@ -109,25 +115,25 @@
         is_legacy = cls._is_legacy_dict_state(state)
         is_migrated_legacy = cls._is_migrated_legacy_state(state)
         is_global = cls._is_global_state(state)
         is_per_stream = cls._is_per_stream_state(state)
 
         # Incoming pure legacy object format
         if is_legacy:
-            streams = cls._create_descriptor_to_stream_state_mapping(state, stream_instance_map)
+            streams = cls._create_descriptor_to_stream_state_mapping(state, stream_instance_map)  # type: ignore # We verified state is a dict in _is_legacy_dict_state
             return None, streams
 
         # When processing incoming state in source.read_state(), legacy state gets deserialized into List[AirbyteStateMessage]
         # which can be translated into independent per-stream state values
         if is_migrated_legacy:
-            streams = cls._create_descriptor_to_stream_state_mapping(state[0].data, stream_instance_map)
+            streams = cls._create_descriptor_to_stream_state_mapping(state[0].data, stream_instance_map)  # type: ignore # We verified that state is a list in _is_migrated_legacy_state
             return None, streams
 
         if is_global:
-            global_state = state[0].global_
+            global_state = state[0].global_  # type: ignore # We verified state is a list in _is_global_state
             shared_state = copy.deepcopy(global_state.shared_state, {})
             streams = {
                 HashableStreamDescriptor(
                     name=per_stream_state.stream_descriptor.name, namespace=per_stream_state.stream_descriptor.namespace
                 ): per_stream_state.stream_state
                 for per_stream_state in global_state.stream_states
             }
@@ -135,46 +141,39 @@
 
         if is_per_stream:
             streams = {
                 HashableStreamDescriptor(
                     name=per_stream_state.stream.stream_descriptor.name, namespace=per_stream_state.stream.stream_descriptor.namespace
                 ): per_stream_state.stream.stream_state
                 for per_stream_state in state
-                if per_stream_state.type == AirbyteStateType.STREAM and hasattr(per_stream_state, "stream")
+                if per_stream_state.type == AirbyteStateType.STREAM and hasattr(per_stream_state, "stream")  # type: ignore # state is always a list of AirbyteStateMessage if is_per_stream is True
             }
             return None, streams
         else:
             raise ValueError("Input state should come in the form of list of Airbyte state messages or a mapping of states")
 
     @staticmethod
     def _create_descriptor_to_stream_state_mapping(
-        state: MutableMapping[str, Any], stream_to_instance_map: Mapping[str, Stream]
+        state: MutableMapping[str, Any], stream_to_instance_map: Mapping[str, Union[Stream, AirbyteStream]]
     ) -> MutableMapping[HashableStreamDescriptor, Optional[AirbyteStateBlob]]:
         """
         Takes incoming state received in the legacy format and transforms it into a mapping of StreamDescriptor to AirbyteStreamState
         :param state: A mapping object representing the complete state of all streams in the legacy format
         :param stream_to_instance_map: A mapping of stream name to stream instance used to retrieve a stream's namespace
         :return: The mapping of all of a sync's streams to the corresponding stream state
         """
         streams = {}
         for stream_name, state_value in state.items():
             namespace = stream_to_instance_map[stream_name].namespace if stream_name in stream_to_instance_map else None
             stream_descriptor = HashableStreamDescriptor(name=stream_name, namespace=namespace)
             streams[stream_descriptor] = AirbyteStateBlob.parse_obj(state_value or {})
         return streams
 
-    def _get_legacy_state(self) -> Mapping[str, Any]:
-        """
-        Using the current per-stream state, creates a mapping of all the stream states for the connector being synced
-        :return: A deep copy of the mapping of stream name to stream state value
-        """
-        return {descriptor.name: state.dict() if state else {} for descriptor, state in self.per_stream_states.items()}
-
     @staticmethod
-    def _is_legacy_dict_state(state: Union[List[AirbyteStateMessage], MutableMapping[str, Any]]):
+    def _is_legacy_dict_state(state: Union[List[AirbyteStateMessage], MutableMapping[str, Any]]) -> bool:
         return isinstance(state, dict)
 
     @staticmethod
     def _is_migrated_legacy_state(state: Union[List[AirbyteStateMessage], MutableMapping[str, Any]]) -> bool:
         return (
             isinstance(state, List)
             and len(state) == 1
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/auth/declarative_authenticator.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/auth/declarative_authenticator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
-from typing import Any, Mapping
+from typing import Any, Mapping, Union
 
 from airbyte_cdk.sources.streams.http.requests_native_auth.abstract_token import AbstractHeaderAuthenticator
-from dataclasses_jsonschema import JsonSchemaMixin
 
 
 @dataclass
-class DeclarativeAuthenticator(JsonSchemaMixin):
+class DeclarativeAuthenticator(AbstractHeaderAuthenticator):
     """
     Interface used to associate which authenticators can be used as part of the declarative framework
     """
 
+    def get_request_params(self) -> Mapping[str, Any]:
+        """HTTP request parameter to add to the requests"""
+        return {}
+
+    def get_request_body_data(self) -> Union[Mapping[str, Any], str]:
+        """Form-encoded body data to set on the requests"""
+        return {}
+
+    def get_request_body_json(self) -> Mapping[str, Any]:
+        """JSON-encoded body data to set on the requests"""
+        return {}
+
 
 @dataclass
-class NoAuth(AbstractHeaderAuthenticator, DeclarativeAuthenticator, JsonSchemaMixin):
-    options: InitVar[Mapping[str, Any]]
+class NoAuth(DeclarativeAuthenticator):
+    parameters: InitVar[Mapping[str, Any]]
 
     @property
     def auth_header(self) -> str:
         return ""
 
     @property
     def token(self) -> str:
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/checks/check_stream.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/checks/check_stream.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import logging
+import traceback
 from dataclasses import InitVar, dataclass
 from typing import Any, List, Mapping, Tuple
 
-from airbyte_cdk.models.airbyte_protocol import SyncMode
 from airbyte_cdk.sources.declarative.checks.connection_checker import ConnectionChecker
 from airbyte_cdk.sources.source import Source
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.streams.http.availability_strategy import HttpAvailabilityStrategy
 
 
 @dataclass
-class CheckStream(ConnectionChecker, JsonSchemaMixin):
+class CheckStream(ConnectionChecker):
     """
-    Checks the connections by trying to read records from one or many of the streams selected by the developer
+    Checks the connections by checking availability of one or many streams selected by the developer
 
     Attributes:
-        stream_name (List[str]): name of streams to read records from
+        stream_name (List[str]): names of streams to check
     """
 
     stream_names: List[str]
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
 
-    def __post_init__(self, options: Mapping[str, Any]):
-        self._options = options
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        self._parameters = parameters
 
-    def check_connection(self, source: Source, logger: logging.Logger, config: Mapping[str, Any]) -> Tuple[bool, any]:
-        streams = source.streams(config)
+    def check_connection(self, source: Source, logger: logging.Logger, config: Mapping[str, Any]) -> Tuple[bool, Any]:
+        streams = source.streams(config)  # type: ignore # source is always a DeclarativeSource, but this parameter type adheres to the outer interface
         stream_name_to_stream = {s.name: s for s in streams}
         if len(streams) == 0:
             return False, f"No streams to connect to from source {source}"
         for stream_name in self.stream_names:
-            if stream_name in stream_name_to_stream.keys():
-                stream = stream_name_to_stream[stream_name]
-                try:
-                    # Some streams need a stream slice to read records (eg if they have a SubstreamSlicer)
-                    stream_slice = self._get_stream_slice(stream)
-                    records = stream.read_records(sync_mode=SyncMode.full_refresh, stream_slice=stream_slice)
-                    next(records)
-                except Exception as error:
-                    return False, f"Unable to connect to stream {stream_name} - {error}"
-            else:
-                raise ValueError(f"{stream_name} is not part of the catalog. Expected one of {stream_name_to_stream.keys()}")
-        return True, None
+            if stream_name not in stream_name_to_stream.keys():
+                raise ValueError(f"{stream_name} is not part of the catalog. Expected one of {stream_name_to_stream.keys()}.")
 
-    def _get_stream_slice(self, stream):
-        # We wrap the return output of stream_slices() because some implementations return types that are iterable,
-        # but not iterators such as lists or tuples
-        slices = iter(
-            stream.stream_slices(
-                cursor_field=stream.cursor_field,
-                sync_mode=SyncMode.full_refresh,
-            )
-        )
-        try:
-            return next(slices)
-        except StopIteration:
-            return {}
+            stream = stream_name_to_stream[stream_name]
+            availability_strategy = stream.availability_strategy or HttpAvailabilityStrategy()
+            try:
+                stream_is_available, reason = availability_strategy.check_availability(stream, logger, source)
+                if not stream_is_available:
+                    return False, reason
+            except Exception as error:
+                logger.error(f"Encountered an error trying to connect to stream {stream_name}. Error: \n {traceback.format_exc()}")
+                return False, f"Unable to connect to stream {stream_name} - {error}"
+        return True, None
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/checks/connection_checker.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/checks/connection_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Mapping, Tuple
 
 from airbyte_cdk.sources.source import Source
@@ -11,15 +11,15 @@
 
 class ConnectionChecker(ABC):
     """
     Abstract base class for checking a connection
     """
 
     @abstractmethod
-    def check_connection(self, source: Source, logger: logging.Logger, config: Mapping[str, Any]) -> Tuple[bool, any]:
+    def check_connection(self, source: Source, logger: logging.Logger, config: Mapping[str, Any]) -> Tuple[bool, Any]:
         """
         Tests if the input configuration can be used to successfully connect to the integration e.g: if a provided Stripe API token can be used to connect
         to the Stripe API.
 
         :param source: source
         :param logger: source logger
         :param config: The user-provided configuration as specified by the source's spec.
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/datetime/datetime_parser.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/datetime/datetime_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import datetime
 from typing import Union
 
 
 class DatetimeParser:
@@ -12,27 +12,40 @@
 
     This class mainly acts as a wrapper to properly handling timestamp formatting through the "%s" directive.
 
     %s is part of the list of format codes required by  the 1989 C standard, but it is unreliable because it always return a datetime in the system's timezone.
     Instead of using the directive directly, we can use datetime.fromtimestamp and dt.timestamp()
     """
 
-    def parse(self, date: Union[str, int], format: str, timezone):
+    _UNIX_EPOCH = datetime.datetime(1970, 1, 1, tzinfo=datetime.timezone.utc)
+
+    def parse(self, date: Union[str, int], format: str) -> datetime.datetime:
         # "%s" is a valid (but unreliable) directive for formatting, but not for parsing
         # It is defined as
         # The number of seconds since the Epoch, 1970-01-01 00:00:00+0000 (UTC). https://man7.org/linux/man-pages/man3/strptime.3.html
         #
         # The recommended way to parse a date from its timestamp representation is to use datetime.fromtimestamp
         # See https://stackoverflow.com/a/4974930
         if format == "%s":
-            return datetime.datetime.fromtimestamp(int(date), tz=timezone)
-        else:
-            return datetime.datetime.strptime(str(date), format).replace(tzinfo=timezone)
+            return datetime.datetime.fromtimestamp(int(date), tz=datetime.timezone.utc)
+        elif format == "%ms":
+            return self._UNIX_EPOCH + datetime.timedelta(milliseconds=int(date))
+
+        parsed_datetime = datetime.datetime.strptime(str(date), format)
+        if self._is_naive(parsed_datetime):
+            return parsed_datetime.replace(tzinfo=datetime.timezone.utc)
+        return parsed_datetime
 
     def format(self, dt: datetime.datetime, format: str) -> str:
         # strftime("%s") is unreliable because it ignores the time zone information and assumes the time zone of the system it's running on
         # It's safer to use the timestamp() method than the %s directive
         # See https://stackoverflow.com/a/4974930
         if format == "%s":
             return str(int(dt.timestamp()))
+        if format == "%ms":
+            # timstamp() returns a float representing the number of seconds since the unix epoch
+            return str(int(dt.timestamp() * 1000))
         else:
             return dt.strftime(format)
+
+    def _is_naive(self, dt: datetime.datetime) -> bool:
+        return dt.tzinfo is None or dt.tzinfo.utcoffset(dt) is None
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/datetime/min_max_datetime.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/datetime/min_max_datetime.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import datetime as dt
 from dataclasses import InitVar, dataclass, field
-from typing import Any, Mapping, Union
+from typing import Any, Mapping, Optional, Union
 
 from airbyte_cdk.sources.declarative.datetime.datetime_parser import DatetimeParser
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
-from dataclasses_jsonschema import JsonSchemaMixin
 
 
 @dataclass
-class MinMaxDatetime(JsonSchemaMixin):
+class MinMaxDatetime:
     """
     Compares the provided date against optional minimum or maximum times. If date is earlier than
     min_date, then min_date is returned. If date is greater than max_date, then max_date is returned.
     If neither, the input date is returned.
 
     The timestamp format accepts the same format codes as datetime.strfptime, which are
     all the format codes required by the 1989 C standard.
@@ -26,58 +25,74 @@
         datetime (Union[InterpolatedString, str]): InterpolatedString or string representing the datetime in the format specified by `datetime_format`
         datetime_format (str): Format of the datetime passed as argument
         min_datetime (Union[InterpolatedString, str]): Represents the minimum allowed datetime value.
         max_datetime (Union[InterpolatedString, str]): Represents the maximum allowed datetime value.
     """
 
     datetime: Union[InterpolatedString, str]
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     # datetime_format is a unique case where we inherit it from the parent if it is not specified before using the default value
     # which is why we need dedicated getter/setter methods and private dataclass field
     datetime_format: str = ""
     _datetime_format: str = field(init=False, repr=False, default="")
     min_datetime: Union[InterpolatedString, str] = ""
     max_datetime: Union[InterpolatedString, str] = ""
 
-    def __post_init__(self, options: Mapping[str, Any]):
-        self.datetime = InterpolatedString.create(self.datetime, options=options or {})
-        self.timezone = dt.timezone.utc
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        self.datetime = InterpolatedString.create(self.datetime, parameters=parameters or {})
         self._parser = DatetimeParser()
-        self.min_datetime = InterpolatedString.create(self.min_datetime, options=options) if self.min_datetime else None
-        self.max_datetime = InterpolatedString.create(self.max_datetime, options=options) if self.max_datetime else None
+        self.min_datetime = InterpolatedString.create(self.min_datetime, parameters=parameters) if self.min_datetime else None  # type: ignore
+        self.max_datetime = InterpolatedString.create(self.max_datetime, parameters=parameters) if self.max_datetime else None  # type: ignore
 
-        self._timezone = dt.timezone.utc
-
-    def get_datetime(self, config, **additional_options) -> dt.datetime:
+    def get_datetime(self, config: Mapping[str, Any], **additional_parameters: Mapping[str, Any]) -> dt.datetime:
         """
         Evaluates and returns the datetime
         :param config: The user-provided configuration as specified by the source's spec
-        :param additional_options: Additional arguments to be passed to the strings for interpolation
+        :param additional_parameters: Additional arguments to be passed to the strings for interpolation
         :return: The evaluated datetime
         """
         # We apply a default datetime format here instead of at instantiation, so it can be set by the parent first
         datetime_format = self._datetime_format
         if not datetime_format:
             datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
 
-        time = self._parser.parse(str(self.datetime.eval(config, **additional_options)), datetime_format, self.timezone)
+        time = self._parser.parse(str(self.datetime.eval(config, **additional_parameters)), datetime_format)  # type: ignore # datetime is always cast to an interpolated string
 
         if self.min_datetime:
-            min_time = self._parser.parse(str(self.min_datetime.eval(config, **additional_options)), datetime_format, self.timezone)
-            time = max(time, min_time)
+            min_time = str(self.min_datetime.eval(config, **additional_parameters))  # type: ignore # min_datetime is always cast to an interpolated string
+            if min_time:
+                min_datetime = self._parser.parse(min_time, datetime_format)  # type: ignore # min_datetime is always cast to an interpolated string
+                time = max(time, min_datetime)
         if self.max_datetime:
-            max_time = self._parser.parse(str(self.max_datetime.eval(config, **additional_options)), datetime_format, self.timezone)
-            time = min(time, max_time)
+            max_time = str(self.max_datetime.eval(config, **additional_parameters))  # type: ignore # max_datetime is always cast to an interpolated string
+            if max_time:
+                max_datetime = self._parser.parse(max_time, datetime_format)
+                time = min(time, max_datetime)
         return time
 
-    @property
+    @property  # type: ignore # properties don't play well with dataclasses...
     def datetime_format(self) -> str:
         """The format of the string representing the datetime"""
         return self._datetime_format
 
     @datetime_format.setter
-    def datetime_format(self, value: str):
+    def datetime_format(self, value: str) -> None:
         """Setter for the datetime format"""
         # Covers the case where datetime_format is not provided in the constructor, which causes the property object
         # to be set which we need to avoid doing
         if not isinstance(value, property):
             self._datetime_format = value
+
+    @classmethod
+    def create(
+        cls,
+        interpolated_string_or_min_max_datetime: Union[InterpolatedString, str, "MinMaxDatetime"],
+        parameters: Optional[Mapping[str, Any]] = None,
+    ) -> "MinMaxDatetime":
+        if parameters is None:
+            parameters = {}
+        if isinstance(interpolated_string_or_min_max_datetime, InterpolatedString) or isinstance(
+            interpolated_string_or_min_max_datetime, str
+        ):
+            return MinMaxDatetime(datetime=interpolated_string_or_min_max_datetime, parameters=parameters)
+        else:
+            return interpolated_string_or_min_max_datetime
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/declarative_source.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/declarative_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
+import logging
 from abc import abstractmethod
-from typing import Tuple
+from typing import Any, Mapping, Tuple
 
 from airbyte_cdk.sources.abstract_source import AbstractSource
 from airbyte_cdk.sources.declarative.checks.connection_checker import ConnectionChecker
 
 
 class DeclarativeSource(AbstractSource):
     """
     Base class for declarative Source. Concrete sources need to define the connection_checker to use
     """
 
     @property
     @abstractmethod
     def connection_checker(self) -> ConnectionChecker:
-        """Returns the ConnectioChecker to use for the `check` operation"""
+        """Returns the ConnectionChecker to use for the `check` operation"""
 
-    def check_connection(self, logger, config) -> Tuple[bool, any]:
+    def check_connection(self, logger: logging.Logger, config: Mapping[str, Any]) -> Tuple[bool, Any]:
         """
         :param logger: The source logger
         :param config: The user-provided configuration as specified by the source's spec.
           This usually contains information required to check connection e.g. tokens, secrets and keys etc.
         :return: A tuple of (boolean, error). If boolean is true, then the connection check is successful
           and we can connect to the underlying data source using the provided configuration.
           Otherwise, the input config cannot be used to connect to the underlying data source,
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/declarative_stream.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/declarative_stream.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,146 +1,159 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass, field
 from typing import Any, Iterable, List, Mapping, MutableMapping, Optional, Union
 
 from airbyte_cdk.models import SyncMode
+from airbyte_cdk.sources.declarative.interpolation import InterpolatedString
+from airbyte_cdk.sources.declarative.migrations.state_migration import StateMigration
 from airbyte_cdk.sources.declarative.retrievers.retriever import Retriever
 from airbyte_cdk.sources.declarative.schema import DefaultSchemaLoader
 from airbyte_cdk.sources.declarative.schema.schema_loader import SchemaLoader
-from airbyte_cdk.sources.declarative.transformations import RecordTransformation
-from airbyte_cdk.sources.declarative.types import Config, StreamSlice
 from airbyte_cdk.sources.streams.core import Stream
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config, StreamSlice
 
 
 @dataclass
-class DeclarativeStream(Stream, JsonSchemaMixin):
+class DeclarativeStream(Stream):
     """
     DeclarativeStream is a Stream that delegates most of its logic to its schema_load and retriever
 
     Attributes:
         name (str): stream name
         primary_key (Optional[Union[str, List[str], List[List[str]]]]): the primary key of the stream
         schema_loader (SchemaLoader): The schema loader
         retriever (Retriever): The retriever
         config (Config): The user-provided configuration as specified by the source's spec
-        stream_cursor_field (Optional[List[str]]): The cursor field
-        transformations (List[RecordTransformation]): A list of transformations to be applied to each output record in the
+        stream_cursor_field (Optional[Union[InterpolatedString, str]]): The cursor field
         stream. Transformations are applied in the order in which they are defined.
-        checkpoint_interval (Optional[int]): How often the stream will checkpoint state (i.e: emit a STATE message)
     """
 
     retriever: Retriever
     config: Config
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     name: str
     primary_key: Optional[Union[str, List[str], List[List[str]]]]
+    state_migrations: List[StateMigration] = field(repr=True, default_factory=list)
     schema_loader: Optional[SchemaLoader] = None
     _name: str = field(init=False, repr=False, default="")
     _primary_key: str = field(init=False, repr=False, default="")
-    _schema_loader: SchemaLoader = field(init=False, repr=False, default=None)
-    stream_cursor_field: Optional[Union[List[str], str]] = None
-    transformations: List[RecordTransformation] = None
-    checkpoint_interval: Optional[int] = None
-
-    def __post_init__(self, options: Mapping[str, Any]):
-        self.stream_cursor_field = self.stream_cursor_field or []
-        self.transformations = self.transformations or []
-        self._schema_loader = self.schema_loader if self.schema_loader else DefaultSchemaLoader(config=self.config, options=options)
+    stream_cursor_field: Optional[Union[InterpolatedString, str]] = None
 
-    @property
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        self._stream_cursor_field = (
+            InterpolatedString.create(self.stream_cursor_field, parameters=parameters)
+            if isinstance(self.stream_cursor_field, str)
+            else self.stream_cursor_field
+        )
+        self._schema_loader = self.schema_loader if self.schema_loader else DefaultSchemaLoader(config=self.config, parameters=parameters)
+
+    @property  # type: ignore
     def primary_key(self) -> Optional[Union[str, List[str], List[List[str]]]]:
         return self._primary_key
 
     @primary_key.setter
     def primary_key(self, value: str) -> None:
         if not isinstance(value, property):
             self._primary_key = value
 
-    @property
+    @property  # type: ignore
     def name(self) -> str:
         """
         :return: Stream name. By default this is the implementing class name, but it can be overridden as needed.
         """
         return self._name
 
     @name.setter
     def name(self, value: str) -> None:
         if not isinstance(value, property):
             self._name = value
 
     @property
-    def state_checkpoint_interval(self) -> Optional[int]:
-        """
-        Decides how often to checkpoint state (i.e: emit a STATE message). E.g: if this returns a value of 100, then state is persisted after reading
-        100 records, then 200, 300, etc.. A good default value is 1000 although your mileage may vary depending on the underlying data source.
-
-        Checkpointing a stream avoids re-reading records in the case a sync is failed or cancelled.
-
-        return None if state should not be checkpointed e.g: because records returned from the underlying data source are not returned in
-        ascending order with respect to the cursor field. This can happen if the source does not support reading records in ascending order of
-        created_at date (or whatever the cursor is). In those cases, state must only be saved once the full stream has been read.
-        """
-        return self.checkpoint_interval
-
-    @property
     def state(self) -> MutableMapping[str, Any]:
-        return self.retriever.state
+        return self.retriever.state  # type: ignore
 
     @state.setter
-    def state(self, value: MutableMapping[str, Any]):
+    def state(self, value: MutableMapping[str, Any]) -> None:
         """State setter, accept state serialized by state getter."""
-        self.retriever.state = value
-
-    def get_updated_state(self, current_stream_state: MutableMapping[str, Any], latest_record: Mapping[str, Any]):
+        state: Mapping[str, Any] = value
+        if self.state_migrations:
+            for migration in self.state_migrations:
+                if migration.should_migrate(state):
+                    state = migration.migrate(state)
+        self.retriever.state = state
+
+    def get_updated_state(
+        self, current_stream_state: MutableMapping[str, Any], latest_record: Mapping[str, Any]
+    ) -> MutableMapping[str, Any]:
         return self.state
 
     @property
     def cursor_field(self) -> Union[str, List[str]]:
         """
         Override to return the default cursor field used by this stream e.g: an API entity might always use created_at as the cursor field.
         :return: The name of the field used as a cursor. If the cursor is nested, return an array consisting of the path to the cursor.
         """
-        return self.stream_cursor_field
+        cursor = self._stream_cursor_field.eval(self.config)  # type: ignore # _stream_cursor_field is always cast to interpolated string
+        return cursor if cursor else []
+
+    @property
+    def is_resumable(self) -> bool:
+        # Declarative sources always implement state getter/setter, but whether it supports checkpointing is based on
+        # if the retriever has a cursor defined.
+        return self.retriever.cursor is not None if hasattr(self.retriever, "cursor") else False
 
     def read_records(
         self,
         sync_mode: SyncMode,
-        cursor_field: List[str] = None,
-        stream_slice: Mapping[str, Any] = None,
-        stream_state: Mapping[str, Any] = None,
+        cursor_field: Optional[List[str]] = None,
+        stream_slice: Optional[Mapping[str, Any]] = None,
+        stream_state: Optional[Mapping[str, Any]] = None,
     ) -> Iterable[Mapping[str, Any]]:
-        for record in self.retriever.read_records(sync_mode, cursor_field, stream_slice, stream_state):
-            yield self._apply_transformations(record, self.config, stream_slice)
-
-    def _apply_transformations(self, record: Mapping[str, Any], config: Config, stream_slice: StreamSlice):
-        output_record = record
-        for transformation in self.transformations:
-            output_record = transformation.transform(record, config=config, stream_state=self.state, stream_slice=stream_slice)
-
-        return output_record
+        """
+        :param: stream_state We knowingly avoid using stream_state as we want cursors to manage their own state.
+        """
+        if stream_slice is None or stream_slice == {}:
+            # As the parameter is Optional, many would just call `read_records(sync_mode)` during testing without specifying the field
+            # As part of the declarative model without custom components, this should never happen as the CDK would wire up a
+            # SinglePartitionRouter that would create this StreamSlice properly
+            # As part of the declarative model with custom components, a user that would return a `None` slice would now have the default
+            # empty slice which seems to make sense.
+            stream_slice = StreamSlice(partition={}, cursor_slice={})
+        if not isinstance(stream_slice, StreamSlice):
+            raise ValueError(f"DeclarativeStream does not support stream_slices that are not StreamSlice. Got {stream_slice}")
+        yield from self.retriever.read_records(self.get_json_schema(), stream_slice)
 
-    def get_json_schema(self) -> Mapping[str, Any]:
+    def get_json_schema(self) -> Mapping[str, Any]:  # type: ignore
         """
         :return: A dict of the JSON schema representing this stream.
 
         The default implementation of this method looks for a JSONSchema file with the same name as this stream's "name" property.
         Override as needed.
         """
         return self._schema_loader.get_json_schema()
 
     def stream_slices(
-        self, *, sync_mode: SyncMode, cursor_field: List[str] = None, stream_state: Mapping[str, Any] = None
-    ) -> Iterable[Optional[Mapping[str, Any]]]:
+        self, *, sync_mode: SyncMode, cursor_field: Optional[List[str]] = None, stream_state: Optional[Mapping[str, Any]] = None
+    ) -> Iterable[Optional[StreamSlice]]:
         """
         Override to define the slices for this stream. See the stream slicing section of the docs for more information.
 
         :param sync_mode:
         :param cursor_field:
-        :param stream_state:
+        :param stream_state: we knowingly avoid using stream_state as we want cursors to manage their own state
         :return:
         """
-        # this is not passing the cursor field because it is known at init time
-        return self.retriever.stream_slices(sync_mode=sync_mode, stream_state=stream_state)
+        return self.retriever.stream_slices()
+
+    @property
+    def state_checkpoint_interval(self) -> Optional[int]:
+        """
+        We explicitly disable checkpointing here. There are a couple reasons for that and not all are documented here but:
+        * In the case where records are not ordered, the granularity of what is ordered is the slice. Therefore, we will only update the
+            cursor value once at the end of every slice.
+        * Updating the state once every record would generate issues for data feed stop conditions or semi-incremental syncs where the
+            important state is the one at the beginning of the slice
+        """
+        return None
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/decoders/decoder.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/decoders/decoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from abc import abstractmethod
 from dataclasses import dataclass
 from typing import Any, List, Mapping, Union
 
 import requests
-from dataclasses_jsonschema import JsonSchemaMixin
 
 
 @dataclass
-class Decoder(JsonSchemaMixin):
+class Decoder:
     """
     Decoder strategy to transform a requests.Response into a Mapping[str, Any]
     """
 
     @abstractmethod
-    def decode(self, response: requests.Response) -> Union[Mapping[str, Any], List]:
+    def decode(self, response: requests.Response) -> Union[Mapping[str, Any], List[Any]]:
         """
         Decodes a requests.Response into a Mapping[str, Any] or an array
         :param response: the response to decode
         :return: Mapping or array describing the response
         """
         pass
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/decoders/json_decoder.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/decoders/json_decoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
 from typing import Any, List, Mapping, Union
 
 import requests
 from airbyte_cdk.sources.declarative.decoders.decoder import Decoder
-from dataclasses_jsonschema import JsonSchemaMixin
 
 
 @dataclass
-class JsonDecoder(Decoder, JsonSchemaMixin):
+class JsonDecoder(Decoder):
     """
     Decoder strategy that returns the json-encoded content of a response, if any.
     """
 
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
 
-    def decode(self, response: requests.Response) -> Union[Mapping[str, Any], List]:
+    def decode(self, response: requests.Response) -> Union[Mapping[str, Any], List[Any], Any]:
         try:
             return response.json()
         except requests.exceptions.JSONDecodeError:
             return {}
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/extractors/dpath_extractor.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/extractors/dpath_extractor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,82 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
-from typing import Any, List, Mapping, Union
+from typing import Any, Iterable, List, Mapping, Union
 
 import dpath.util
 import requests
 from airbyte_cdk.sources.declarative.decoders.decoder import Decoder
 from airbyte_cdk.sources.declarative.decoders.json_decoder import JsonDecoder
 from airbyte_cdk.sources.declarative.extractors.record_extractor import RecordExtractor
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
-from airbyte_cdk.sources.declarative.types import Config, Record
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config
 
 
 @dataclass
-class DpathExtractor(RecordExtractor, JsonSchemaMixin):
+class DpathExtractor(RecordExtractor):
     """
     Record extractor that searches a decoded response over a path defined as an array of fields.
 
-    If the field pointer points to an array, that array is returned.
-    If the field pointer points to an object, that object is returned wrapped as an array.
-    If the field pointer points to an empty object, an empty array is returned.
-    If the field pointer points to a non-existing path, an empty array is returned.
+    If the field path points to an array, that array is returned.
+    If the field path points to an object, that object is returned wrapped as an array.
+    If the field path points to an empty object, an empty array is returned.
+    If the field path points to a non-existing path, an empty array is returned.
 
     Examples of instantiating this transform:
     ```
       extractor:
         type: DpathExtractor
-        field_pointer:
+        field_path:
           - "root"
           - "data"
     ```
 
     ```
       extractor:
         type: DpathExtractor
-        field_pointer:
+        field_path:
           - "root"
-          - "{{ options['field'] }}"
+          - "{{ parameters['field'] }}"
     ```
 
     ```
       extractor:
         type: DpathExtractor
-        field_pointer: []
+        field_path: []
     ```
 
     Attributes:
-        transform (Union[InterpolatedString, str]): Pointer to the field that should be extracted
+        field_path (Union[InterpolatedString, str]): Path to the field that should be extracted
         config (Config): The user-provided configuration as specified by the source's spec
         decoder (Decoder): The decoder responsible to transfom the response in a Mapping
     """
 
-    field_pointer: List[Union[InterpolatedString, str]]
+    field_path: List[Union[InterpolatedString, str]]
     config: Config
-    options: InitVar[Mapping[str, Any]]
-    decoder: Decoder = JsonDecoder(options={})
+    parameters: InitVar[Mapping[str, Any]]
+    decoder: Decoder = JsonDecoder(parameters={})
 
-    def __post_init__(self, options: Mapping[str, Any]):
-        for pointer_index in range(len(self.field_pointer)):
-            if isinstance(self.field_pointer[pointer_index], str):
-                self.field_pointer[pointer_index] = InterpolatedString.create(self.field_pointer[pointer_index], options=options)
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        self._field_path = [InterpolatedString.create(path, parameters=parameters) for path in self.field_path]
+        for path_index in range(len(self.field_path)):
+            if isinstance(self.field_path[path_index], str):
+                self._field_path[path_index] = InterpolatedString.create(self.field_path[path_index], parameters=parameters)
 
-    def extract_records(self, response: requests.Response) -> List[Record]:
+    def extract_records(self, response: requests.Response) -> Iterable[Mapping[str, Any]]:
         response_body = self.decoder.decode(response)
-        if len(self.field_pointer) == 0:
+        if len(self._field_path) == 0:
             extracted = response_body
         else:
-            pointer = [pointer.eval(self.config) for pointer in self.field_pointer]
-            extracted = dpath.util.get(response_body, pointer, default=[])
+            path = [path.eval(self.config) for path in self._field_path]
+            if "*" in path:
+                extracted = dpath.util.values(response_body, path)
+            else:
+                extracted = dpath.util.get(response_body, path, default=[])
         if isinstance(extracted, list):
-            return extracted
+            yield from extracted
         elif extracted:
-            return [extracted]
+            yield extracted
         else:
-            return []
+            yield from []
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/extractors/http_selector.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/extractors/http_selector.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import Any, List, Mapping, Optional
+from typing import Any, Iterable, Mapping, Optional
 
 import requests
-from airbyte_cdk.sources.declarative.types import Record, StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Record, StreamSlice, StreamState
 
 
 @dataclass
-class HttpSelector(JsonSchemaMixin):
+class HttpSelector:
     """
     Responsible for translating an HTTP response into a list of records by extracting records from the response and optionally filtering
     records based on a heuristic.
     """
 
     @abstractmethod
     def select_records(
         self,
         response: requests.Response,
         stream_state: StreamState,
+        records_schema: Mapping[str, Any],
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> List[Record]:
+    ) -> Iterable[Record]:
         """
         Selects records from the response
         :param response: The response to select the records from
         :param stream_state: The stream state
+        :param records_schema: json schema of records to return
         :param stream_slice: The stream slice
         :param next_page_token: The paginator token
         :return: List of Records selected from the response
         """
         pass
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/extractors/record_extractor.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/extractors/record_extractor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
-
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import List
+from typing import Any, Iterable, Mapping
 
 import requests
-from airbyte_cdk.sources.declarative.types import Record
-from dataclasses_jsonschema import JsonSchemaMixin
 
 
 @dataclass
-class RecordExtractor(JsonSchemaMixin):
+class RecordExtractor:
     """
     Responsible for translating an HTTP response into a list of records by extracting records from the response.
     """
 
     @abstractmethod
     def extract_records(
         self,
         response: requests.Response,
-    ) -> List[Record]:
+    ) -> Iterable[Mapping[str, Any]]:
         """
         Selects records from the response
         :param response: The response to extract the records from
         :return: List of Records extracted from the response
         """
         pass
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/extractors/record_filter.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/extractors/record_filter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
-from typing import Any, List, Mapping, Optional
+from typing import Any, Iterable, Mapping, Optional
 
 from airbyte_cdk.sources.declarative.interpolation.interpolated_boolean import InterpolatedBoolean
-from airbyte_cdk.sources.declarative.types import Config, Record, StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config, StreamSlice, StreamState
 
 
 @dataclass
-class RecordFilter(JsonSchemaMixin):
+class RecordFilter:
     """
     Filter applied on a list of Records
 
     config (Config): The user-provided configuration as specified by the source's spec
     condition (str): The string representing the predicate to filter a record. Records will be removed if evaluated to False
     """
 
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     config: Config
     condition: str = ""
 
-    def __post_init__(self, options: Mapping[str, Any]):
-        self._filter_interpolator = InterpolatedBoolean(condition=self.condition, options=options)
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        self._filter_interpolator = InterpolatedBoolean(condition=self.condition, parameters=parameters)
 
     def filter_records(
         self,
-        records: List[Record],
+        records: Iterable[Mapping[str, Any]],
         stream_state: StreamState,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> List[Record]:
+    ) -> Iterable[Mapping[str, Any]]:
         kwargs = {"stream_state": stream_state, "stream_slice": stream_slice, "next_page_token": next_page_token}
-        return [record for record in records if self._filter_interpolator.eval(self.config, record=record, **kwargs)]
+        for record in records:
+            if self._filter_interpolator.eval(self.config, record=record, **kwargs):
+                yield record
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/interpolated_boolean.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/interpolated_boolean.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
 from typing import Any, Final, List, Mapping
 
 from airbyte_cdk.sources.declarative.interpolation.jinja import JinjaInterpolation
-from airbyte_cdk.sources.declarative.types import Config
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config
 
-FALSE_VALUES: Final[List[Any]] = ["False", "false", "{}", "[]", "()", "", "0", "0.0", "False", "false", {}, False, [], (), set()]
+FALSE_VALUES: Final[List[Any]] = ["False", "false", "{}", "[]", "()", "", "0", "0.0", {}, False, [], (), set()]
 
 
 @dataclass
-class InterpolatedBoolean(JsonSchemaMixin):
+class InterpolatedBoolean:
     f"""
     Wrapper around a string to be evaluated to a boolean value.
     The string will be evaluated as False if it interpolates to a value in {FALSE_VALUES}
 
     Attributes:
         condition (str): The string representing the condition to evaluate to a boolean
     """
     condition: str
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
 
-    def __post_init__(self, options: Mapping[str, Any]):
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
         self._default = "False"
         self._interpolation = JinjaInterpolation()
-        self._options = options
+        self._parameters = parameters
 
-    def eval(self, config: Config, **additional_options):
+    def eval(self, config: Config, **additional_parameters: Any) -> bool:
         """
         Interpolates the predicate condition string using the config and other optional arguments passed as parameter.
 
         :param config: The user-provided configuration as specified by the source's spec
-        :param additional_options: Optional parameters used for interpolation
+        :param additional_parameters: Optional parameters used for interpolation
         :return: The interpolated string
         """
         if isinstance(self.condition, bool):
             return self.condition
         else:
-            evaluated = self._interpolation.eval(self.condition, config, self._default, options=self._options, **additional_options)
+            evaluated = self._interpolation.eval(
+                self.condition, config, self._default, parameters=self._parameters, **additional_parameters
+            )
             if evaluated in FALSE_VALUES:
                 return False
             # The presence of a value is generally regarded as truthy, so we treat it as such
             return True
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/interpolated_mapping.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/interpolated_mapping.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 from dataclasses import InitVar, dataclass
-from typing import Any, Mapping, Optional
+from typing import Any, Dict, Mapping, Optional
 
 from airbyte_cdk.sources.declarative.interpolation.jinja import JinjaInterpolation
-from airbyte_cdk.sources.declarative.types import Config
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config
 
 
 @dataclass
-class InterpolatedMapping(JsonSchemaMixin):
+class InterpolatedMapping:
     """
     Wrapper around a Mapping[str, str] where both the keys and values are to be interpolated.
 
     Attributes:
         mapping (Mapping[str, str]): to be evaluated
     """
 
     mapping: Mapping[str, str]
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
 
-    def __post_init__(self, options: Optional[Mapping[str, Any]]):
+    def __post_init__(self, parameters: Optional[Mapping[str, Any]]) -> None:
         self._interpolation = JinjaInterpolation()
-        self._options = options
+        self._parameters = parameters
 
-    def eval(self, config: Config, **additional_options):
+    def eval(self, config: Config, **additional_parameters: Any) -> Dict[str, Any]:
         """
         Wrapper around a Mapping[str, str] that allows for both keys and values to be interpolated.
 
         :param config: The user-provided configuration as specified by the source's spec
-        :param additional_options: Optional parameters used for interpolation
-        :return: The interpolated string
+        :param additional_parameters: Optional parameters used for interpolation
+        :return: The interpolated mapping
         """
-        interpolated_values = {
-            self._interpolation.eval(name, config, options=self._options, **additional_options): self._eval(
-                value, config, **additional_options
-            )
+        valid_key_types = additional_parameters.pop("valid_key_types", (str,))
+        valid_value_types = additional_parameters.pop("valid_value_types", None)
+        return {
+            self._interpolation.eval(
+                name, config, valid_types=valid_key_types, parameters=self._parameters, **additional_parameters
+            ): self._eval(value, config, valid_types=valid_value_types, **additional_parameters)
             for name, value in self.mapping.items()
         }
-        return interpolated_values
 
-    def _eval(self, value, config, **kwargs):
+    def _eval(self, value: str, config: Config, **kwargs: Any) -> Any:
         # The values in self._mapping can be of Any type
         # We only want to interpolate them if they are strings
-        if type(value) == str:
-            return self._interpolation.eval(value, config, options=self._options, **kwargs)
+        if isinstance(value, str):
+            return self._interpolation.eval(value, config, parameters=self._parameters, **kwargs)
         else:
             return value
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/interpolated_string.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/interpolated_string.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
 from typing import Any, Mapping, Optional, Union
 
 from airbyte_cdk.sources.declarative.interpolation.jinja import JinjaInterpolation
-from airbyte_cdk.sources.declarative.types import Config
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config
 
 
 @dataclass
-class InterpolatedString(JsonSchemaMixin):
+class InterpolatedString:
     """
     Wrapper around a raw string to be interpolated with the Jinja2 templating engine
 
     Attributes:
         string (str): The string to evalute
         default (Optional[str]): The default value to return if the evaluation returns an empty string
-        options (Mapping[str, Any]): Additional runtime parameters to be used for string interpolation
+        parameters (Mapping[str, Any]): Additional runtime parameters to be used for string interpolation
     """
 
     string: str
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     default: Optional[str] = None
 
-    def __post_init__(self, options: Mapping[str, Any]):
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
         self.default = self.default or self.string
         self._interpolation = JinjaInterpolation()
-        self._options = options
+        self._parameters = parameters
 
-    def eval(self, config: Config, **kwargs):
+    def eval(self, config: Config, **kwargs: Any) -> Any:
         """
         Interpolates the input string using the config and other optional arguments passed as parameter.
 
         :param config: The user-provided configuration as specified by the source's spec
         :param kwargs: Optional parameters used for interpolation
         :return: The interpolated string
         """
-        return self._interpolation.eval(self.string, config, self.default, options=self._options, **kwargs)
+        return self._interpolation.eval(self.string, config, self.default, parameters=self._parameters, **kwargs)
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if not isinstance(other, InterpolatedString):
             return False
         return self.string == other.string and self.default == other.default
 
     @classmethod
     def create(
         cls,
         string_or_interpolated: Union["InterpolatedString", str],
         *,
-        options: Mapping[str, Any],
-    ):
+        parameters: Mapping[str, Any],
+    ) -> "InterpolatedString":
         """
         Helper function to obtain an InterpolatedString from either a raw string or an InterpolatedString.
 
         :param string_or_interpolated: either a raw string or an InterpolatedString.
-        :param options: options parameters propagated from parent component
+        :param parameters: parameters propagated from parent component
         :return: InterpolatedString representing the input string.
         """
         if isinstance(string_or_interpolated, str):
-            return InterpolatedString(string=string_or_interpolated, options=options)
+            return InterpolatedString(string=string_or_interpolated, parameters=parameters)
         else:
             return string_or_interpolated
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/interpolation/interpolation.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/interpolation/interpolation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from abc import ABC, abstractmethod
-from typing import Optional
+from typing import Any, Optional
 
-from airbyte_cdk.sources.declarative.types import Config
+from airbyte_cdk.sources.types import Config
 
 
 class Interpolation(ABC):
     """
     Strategy for evaluating the interpolated value of a string at runtime using Jinja.
     """
 
     @abstractmethod
-    def eval(self, input_str: str, config: Config, default: Optional[str] = None, **additional_options):
+    def eval(self, input_str: str, config: Config, default: Optional[str] = None, **additional_options: Any) -> Any:
         """
         Interpolates the input string using the config, and additional options passed as parameter.
 
         :param input_str: The string to interpolate
         :param config: The user-provided configuration as specified by the source's spec
         :param default: Default value to return if the evaluation returns an empty string
         :param additional_options: Optional parameters used for interpolation
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/manifest_declarative_source.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_oauth.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,207 +1,258 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
-import inspect
-import json
 import logging
-import typing
-from dataclasses import dataclass, fields
-from enum import Enum, EnumMeta
-from typing import Any, Iterator, List, Mapping, MutableMapping, Union
-
-from airbyte_cdk.models import (
-    AirbyteConnectionStatus,
-    AirbyteMessage,
-    AirbyteStateMessage,
-    ConfiguredAirbyteCatalog,
-    ConnectorSpecification,
-)
-from airbyte_cdk.sources.declarative.checks import CheckStream
-from airbyte_cdk.sources.declarative.checks.connection_checker import ConnectionChecker
-from airbyte_cdk.sources.declarative.declarative_source import DeclarativeSource
-from airbyte_cdk.sources.declarative.declarative_stream import DeclarativeStream
-from airbyte_cdk.sources.declarative.exceptions import InvalidConnectorDefinitionException
-from airbyte_cdk.sources.declarative.parsers.factory import DeclarativeComponentFactory
-from airbyte_cdk.sources.declarative.parsers.manifest_reference_resolver import ManifestReferenceResolver
-from airbyte_cdk.sources.declarative.types import ConnectionDefinition
-from airbyte_cdk.sources.streams.core import Stream
-from dataclasses_jsonschema import JsonSchemaMixin
-from jsonschema.validators import validate
-
-
-@dataclass
-class ConcreteDeclarativeSource(JsonSchemaMixin):
-    version: str
-    checker: CheckStream
-    streams: List[DeclarativeStream]
-
-
-class ManifestDeclarativeSource(DeclarativeSource):
-    """Declarative source defined by a manifest of low-code components that define source connector behavior"""
-
-    VALID_TOP_LEVEL_FIELDS = {"check", "definitions", "spec", "streams", "version"}
-
-    def __init__(self, source_config: ConnectionDefinition, debug: bool = False):
-        """
-        :param source_config(Mapping[str, Any]): The manifest of low-code components that describe the source connector
-        :param debug(bool): True if debug mode is enabled
-        """
-        self.logger = logging.getLogger(f"airbyte.{self.name}")
-
-        evaluated_manifest = {}
-        resolved_source_config = ManifestReferenceResolver().preprocess_manifest(source_config, evaluated_manifest, "")
-        self._source_config = resolved_source_config
-        self._debug = debug
-        self._factory = DeclarativeComponentFactory()
-
-        self._validate_source()
-
-        # Stopgap to protect the top-level namespace until it's validated through the schema
-        unknown_fields = [key for key in self._source_config.keys() if key not in self.VALID_TOP_LEVEL_FIELDS]
-        if unknown_fields:
-            raise InvalidConnectorDefinitionException(f"Found unknown top-level fields: {unknown_fields}")
+from abc import abstractmethod
+from json import JSONDecodeError
+from typing import Any, List, Mapping, MutableMapping, Optional, Tuple, Union
+
+import backoff
+import pendulum
+import requests
+from airbyte_cdk.models import FailureType, Level
+from airbyte_cdk.sources.http_logger import format_http_message
+from airbyte_cdk.sources.message import MessageRepository, NoopMessageRepository
+from airbyte_cdk.utils import AirbyteTracedException
+from airbyte_cdk.utils.airbyte_secrets_utils import add_to_secrets
+from requests.auth import AuthBase
+
+from ..exceptions import DefaultBackoffException
+
+logger = logging.getLogger("airbyte")
+_NOOP_MESSAGE_REPOSITORY = NoopMessageRepository()
+
+
+class AbstractOauth2Authenticator(AuthBase):
+    """
+    Abstract class for an OAuth authenticators that implements the OAuth token refresh flow. The authenticator
+    is designed to generically perform the refresh flow without regard to how config fields are get/set by
+    delegating that behavior to the classes implementing the interface.
+    """
 
-    @property
-    def connection_checker(self) -> ConnectionChecker:
-        check = self._source_config["check"]
-        if "class_name" not in check:
-            check["class_name"] = "airbyte_cdk.sources.declarative.checks.check_stream.CheckStream"
-        return self._factory.create_component(check, dict())(source=self)
-
-    def streams(self, config: Mapping[str, Any]) -> List[Stream]:
-        self._emit_manifest_debug_message(extra_args={"source_name": self.name, "parsed_config": json.dumps(self._source_config)})
-
-        source_streams = [self._factory.create_component(stream_config, config, True)() for stream_config in self._stream_configs()]
-        for stream in source_streams:
-            # make sure the log level is always applied to the stream's logger
-            self._apply_log_level_to_stream_logger(self.logger, stream)
-        return source_streams
-
-    def spec(self, logger: logging.Logger) -> ConnectorSpecification:
-        """
-        Returns the connector specification (spec) as defined in the Airbyte Protocol. The spec is an object describing the possible
-        configurations (e.g: username and password) which can be configured when running this connector. For low-code connectors, this
-        will first attempt to load the spec from the manifest's spec block, otherwise it will load it from "spec.yaml" or "spec.json"
-        in the project root.
-        """
-        self._configure_logger_level(logger)
-        self._emit_manifest_debug_message(extra_args={"source_name": self.name, "parsed_config": json.dumps(self._source_config)})
-
-        spec = self._source_config.get("spec")
-        if spec:
-            if "class_name" not in spec:
-                spec["class_name"] = "airbyte_cdk.sources.declarative.spec.Spec"
-            spec_component = self._factory.create_component(spec, dict())()
-            return spec_component.generate_spec()
+    _NO_STREAM_NAME = None
+
+    def __init__(
+        self,
+        refresh_token_error_status_codes: Tuple[int, ...] = (),
+        refresh_token_error_key: str = "",
+        refresh_token_error_values: Tuple[str, ...] = (),
+    ) -> None:
+        """
+        If all of refresh_token_error_status_codes, refresh_token_error_key, and refresh_token_error_values are set,
+        then http errors with such params will be wrapped in AirbyteTracedException.
+        """
+        self._refresh_token_error_status_codes = refresh_token_error_status_codes
+        self._refresh_token_error_key = refresh_token_error_key
+        self._refresh_token_error_values = refresh_token_error_values
+
+    def __call__(self, request: requests.PreparedRequest) -> requests.PreparedRequest:
+        """Attach the HTTP headers required to authenticate on the HTTP request"""
+        request.headers.update(self.get_auth_header())
+        return request
+
+    def get_auth_header(self) -> Mapping[str, Any]:
+        """HTTP header to set on the requests"""
+        return {"Authorization": f"Bearer {self.get_access_token()}"}
+
+    def get_access_token(self) -> str:
+        """Returns the access token"""
+        if self.token_has_expired():
+            token, expires_in = self.refresh_access_token()
+            self.access_token = token
+            self.set_token_expiry_date(expires_in)
+
+        return self.access_token
+
+    def token_has_expired(self) -> bool:
+        """Returns True if the token is expired"""
+        return pendulum.now() > self.get_token_expiry_date()  # type: ignore # this is always a bool despite what mypy thinks
+
+    def build_refresh_request_body(self) -> Mapping[str, Any]:
+        """
+        Returns the request body to set on the refresh request
+
+        Override to define additional parameters
+        """
+        payload: MutableMapping[str, Any] = {
+            "grant_type": self.get_grant_type(),
+            "client_id": self.get_client_id(),
+            "client_secret": self.get_client_secret(),
+            "refresh_token": self.get_refresh_token(),
+        }
+
+        if self.get_scopes():
+            payload["scopes"] = self.get_scopes()
+
+        if self.get_refresh_request_body():
+            for key, val in self.get_refresh_request_body().items():
+                # We defer to existing oauth constructs over custom configured fields
+                if key not in payload:
+                    payload[key] = val
+
+        return payload
+
+    def _wrap_refresh_token_exception(self, exception: requests.exceptions.RequestException) -> bool:
+        try:
+            if exception.response is not None:
+                exception_content = exception.response.json()
+            else:
+                return False
+        except JSONDecodeError:
+            return False
+        return (
+            exception.response.status_code in self._refresh_token_error_status_codes
+            and exception_content.get(self._refresh_token_error_key) in self._refresh_token_error_values
+        )
+
+    @backoff.on_exception(
+        backoff.expo,
+        DefaultBackoffException,
+        on_backoff=lambda details: logger.info(
+            f"Caught retryable error after {details['tries']} tries. Waiting {details['wait']} seconds then retrying..."
+        ),
+        max_time=300,
+    )
+    def _get_refresh_access_token_response(self) -> Any:
+        try:
+            response = requests.request(method="POST", url=self.get_token_refresh_endpoint(), data=self.build_refresh_request_body())
+            if response.ok:
+                response_json = response.json()
+                # Add the access token to the list of secrets so it is replaced before logging the response
+                # An argument could be made to remove the prevous access key from the list of secrets, but unmasking values seems like a security incident waiting to happen...
+                access_key = response_json.get(self.get_access_token_name())
+                if not access_key:
+                    raise Exception("Token refresh API response was missing access token {self.get_access_token_name()}")
+                add_to_secrets(access_key)
+                self._log_response(response)
+                return response_json
+            else:
+                # log the response even if the request failed for troubleshooting purposes
+                self._log_response(response)
+                response.raise_for_status()
+        except requests.exceptions.RequestException as e:
+            if e.response is not None:
+                if e.response.status_code == 429 or e.response.status_code >= 500:
+                    raise DefaultBackoffException(request=e.response.request, response=e.response)
+            if self._wrap_refresh_token_exception(e):
+                message = "Refresh token is invalid or expired. Please re-authenticate from Sources/<your source>/Settings."
+                raise AirbyteTracedException(internal_message=message, message=message, failure_type=FailureType.config_error)
+            raise
+        except Exception as e:
+            raise Exception(f"Error while refreshing access token: {e}") from e
+
+    def refresh_access_token(self) -> Tuple[str, Union[str, int]]:
+        """
+        Returns the refresh token and its expiration datetime
+
+        :return: a tuple of (access_token, token_lifespan)
+        """
+        response_json = self._get_refresh_access_token_response()
+
+        return response_json[self.get_access_token_name()], response_json[self.get_expires_in_name()]
+
+    def _parse_token_expiration_date(self, value: Union[str, int]) -> pendulum.DateTime:
+        """
+        Return the expiration datetime of the refresh token
+
+        :return: expiration datetime
+        """
+
+        if self.token_expiry_is_time_of_expiration:
+            if not self.token_expiry_date_format:
+                raise ValueError(
+                    f"Invalid token expiry date format {self.token_expiry_date_format}; a string representing the format is required."
+                )
+            return pendulum.from_format(str(value), self.token_expiry_date_format)
         else:
-            return super().spec(logger)
+            return pendulum.now().add(seconds=int(float(value)))
 
-    def check(self, logger: logging.Logger, config: Mapping[str, Any]) -> AirbyteConnectionStatus:
-        self._configure_logger_level(logger)
-        return super().check(logger, config)
+    @property
+    def token_expiry_is_time_of_expiration(self) -> bool:
+        """
+        Indicates that the Token Expiry returns the date until which the token will be valid, not the amount of time it will be valid.
+        """
 
-    def read(
-        self,
-        logger: logging.Logger,
-        config: Mapping[str, Any],
-        catalog: ConfiguredAirbyteCatalog,
-        state: Union[List[AirbyteStateMessage], MutableMapping[str, Any]] = None,
-    ) -> Iterator[AirbyteMessage]:
-        self._configure_logger_level(logger)
-        yield from super().read(logger, config, catalog, state)
-
-    def _configure_logger_level(self, logger: logging.Logger):
-        """
-        Set the log level to logging.DEBUG if debug mode is enabled
-        """
-        if self._debug:
-            logger.setLevel(logging.DEBUG)
-
-    def _validate_source(self):
-        full_config = {}
-        if "version" in self._source_config:
-            full_config["version"] = self._source_config["version"]
-        if "check" in self._source_config:
-            full_config["checker"] = self._source_config["check"]
-        streams = [self._factory.create_component(stream_config, {}, False)() for stream_config in self._stream_configs()]
-        if len(streams) > 0:
-            full_config["streams"] = streams
-        declarative_source_schema = ConcreteDeclarativeSource.json_schema()
-        validate(full_config, declarative_source_schema)
-
-    def _stream_configs(self):
-        stream_configs = self._source_config.get("streams", [])
-        for s in stream_configs:
-            if "class_name" not in s:
-                s["class_name"] = "airbyte_cdk.sources.declarative.declarative_stream.DeclarativeStream"
-        return stream_configs
-
-    @staticmethod
-    def generate_schema() -> str:
-        expanded_source_manifest = ManifestDeclarativeSource.expand_schema_interfaces(ConcreteDeclarativeSource, {})
-        expanded_schema = expanded_source_manifest.json_schema()
-        return json.dumps(expanded_schema, cls=SchemaEncoder)
-
-    @staticmethod
-    def expand_schema_interfaces(expand_class: type, visited: dict) -> type:
-        """
-        Recursive function that takes in class type that will have its interface fields unpacked and expended and then recursively
-        attempt the same expansion on all the class' underlying fields that are declarative component. It also performs expansion
-        with respect to interfaces that are contained within generic data types.
-        :param expand_class: The declarative component class that will have its interface fields expanded
-        :param visited: cache used to store a record of already visited declarative classes that have already been seen
-        :return: The expanded declarative component
-        """
-
-        # Recursive base case to stop recursion if we have already expanded an interface in case of cyclical components
-        # like CompositeErrorHandler
-        if expand_class.__name__ in visited:
-            return visited[expand_class.__name__]
-        visited[expand_class.__name__] = expand_class
-
-        next_classes = []
-        class_fields = fields(expand_class)
-        for field in class_fields:
-            unpacked_field_types = DeclarativeComponentFactory.unpack(field.type)
-            expand_class.__annotations__[field.name] = unpacked_field_types
-            next_classes.extend(ManifestDeclarativeSource._get_next_expand_classes(field.type))
-        for next_class in next_classes:
-            ManifestDeclarativeSource.expand_schema_interfaces(next_class, visited)
-        return expand_class
-
-    @staticmethod
-    def _get_next_expand_classes(field_type) -> list[type]:
-        """
-        Parses through a given field type and assembles a list of all underlying declarative components. For a concrete declarative class
-        it will return itself. For a declarative interface it will return its subclasses. For declarative components in a generic type
-        it will return the unpacked classes. Any non-declarative types will be skipped.
-        :param field_type: A field type that
-        :return:
-        """
-        generic_type = typing.get_origin(field_type)
-        if generic_type is None:
-            # We can only continue parsing declarative that inherit from the JsonSchemaMixin class because it is used
-            # to generate the final json schema
-            if inspect.isclass(field_type) and issubclass(field_type, JsonSchemaMixin) and not isinstance(field_type, EnumMeta):
-                subclasses = field_type.__subclasses__()
-                if subclasses:
-                    return subclasses
-                else:
-                    return [field_type]
-        elif generic_type == list or generic_type == Union:
-            next_classes = []
-            for underlying_type in typing.get_args(field_type):
-                next_classes.extend(ManifestDeclarativeSource._get_next_expand_classes(underlying_type))
-            return next_classes
-        return []
-
-    def _emit_manifest_debug_message(self, extra_args: dict):
-        self.logger.debug("declarative source created from manifest", extra=extra_args)
-
-
-class SchemaEncoder(json.JSONEncoder):
-    def default(self, obj):
-        if isinstance(obj, property) or isinstance(obj, Enum):
-            return str(obj)
-        return json.JSONEncoder.default(self, obj)
+        return False
+
+    @property
+    def token_expiry_date_format(self) -> Optional[str]:
+        """
+        Format of the datetime; exists it if expires_in is returned as the expiration datetime instead of seconds until it expires
+        """
+
+        return None
+
+    @abstractmethod
+    def get_token_refresh_endpoint(self) -> str:
+        """Returns the endpoint to refresh the access token"""
+
+    @abstractmethod
+    def get_client_id(self) -> str:
+        """The client id to authenticate"""
+
+    @abstractmethod
+    def get_client_secret(self) -> str:
+        """The client secret to authenticate"""
+
+    @abstractmethod
+    def get_refresh_token(self) -> Optional[str]:
+        """The token used to refresh the access token when it expires"""
+
+    @abstractmethod
+    def get_scopes(self) -> List[str]:
+        """List of requested scopes"""
+
+    @abstractmethod
+    def get_token_expiry_date(self) -> pendulum.DateTime:
+        """Expiration date of the access token"""
+
+    @abstractmethod
+    def set_token_expiry_date(self, value: Union[str, int]) -> None:
+        """Setter for access token expiration date"""
+
+    @abstractmethod
+    def get_access_token_name(self) -> str:
+        """Field to extract access token from in the response"""
+
+    @abstractmethod
+    def get_expires_in_name(self) -> str:
+        """Returns the expires_in field name"""
+
+    @abstractmethod
+    def get_refresh_request_body(self) -> Mapping[str, Any]:
+        """Returns the request body to set on the refresh request"""
+
+    @abstractmethod
+    def get_grant_type(self) -> str:
+        """Returns grant_type specified for requesting access_token"""
+
+    @property
+    @abstractmethod
+    def access_token(self) -> str:
+        """Returns the access token"""
+
+    @access_token.setter
+    @abstractmethod
+    def access_token(self, value: str) -> str:
+        """Setter for the access token"""
+
+    @property
+    def _message_repository(self) -> Optional[MessageRepository]:
+        """
+        The implementation can define a message_repository if it wants debugging logs for HTTP requests
+        """
+        return _NOOP_MESSAGE_REPOSITORY
+
+    def _log_response(self, response: requests.Response) -> None:
+        if self._message_repository:
+            self._message_repository.log_message(
+                Level.DEBUG,
+                lambda: format_http_message(
+                    response,
+                    "Refresh token",
+                    "Obtains access token",
+                    self._NO_STREAM_NAME,
+                    is_auxiliary=True,
+                ),
+            )
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/parsers/class_types_registry.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/parsers/class_types_registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
-from typing import Mapping, Type
+from typing import Mapping
 
 from airbyte_cdk.sources.declarative.auth.declarative_authenticator import NoAuth
+from airbyte_cdk.sources.declarative.auth.jwt import JwtAuthenticator
 from airbyte_cdk.sources.declarative.auth.oauth import DeclarativeOauth2Authenticator
-from airbyte_cdk.sources.declarative.auth.token import ApiKeyAuthenticator, BasicHttpAuthenticator, BearerAuthenticator
+from airbyte_cdk.sources.declarative.auth.token import (
+    ApiKeyAuthenticator,
+    BasicHttpAuthenticator,
+    BearerAuthenticator,
+    LegacySessionTokenAuthenticator,
+)
+from airbyte_cdk.sources.declarative.checks import CheckStream
 from airbyte_cdk.sources.declarative.datetime.min_max_datetime import MinMaxDatetime
 from airbyte_cdk.sources.declarative.declarative_stream import DeclarativeStream
+from airbyte_cdk.sources.declarative.extractors import RecordFilter
 from airbyte_cdk.sources.declarative.extractors.dpath_extractor import DpathExtractor
 from airbyte_cdk.sources.declarative.extractors.record_selector import RecordSelector
+from airbyte_cdk.sources.declarative.incremental.datetime_based_cursor import DatetimeBasedCursor
 from airbyte_cdk.sources.declarative.interpolation.interpolated_boolean import InterpolatedBoolean
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
+from airbyte_cdk.sources.declarative.partition_routers.list_partition_router import ListPartitionRouter
+from airbyte_cdk.sources.declarative.partition_routers.substream_partition_router import ParentStreamConfig, SubstreamPartitionRouter
+from airbyte_cdk.sources.declarative.requesters import RequestOption
+from airbyte_cdk.sources.declarative.requesters.error_handlers import HttpResponseFilter
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategies.constant_backoff_strategy import ConstantBackoffStrategy
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategies.exponential_backoff_strategy import (
     ExponentialBackoffStrategy,
 )
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategies.wait_time_from_header_backoff_strategy import (
     WaitTimeFromHeaderBackoffStrategy,
 )
@@ -27,57 +40,65 @@
 from airbyte_cdk.sources.declarative.requesters.error_handlers.default_error_handler import DefaultErrorHandler
 from airbyte_cdk.sources.declarative.requesters.http_requester import HttpRequester
 from airbyte_cdk.sources.declarative.requesters.paginators.default_paginator import DefaultPaginator
 from airbyte_cdk.sources.declarative.requesters.paginators.no_pagination import NoPagination
 from airbyte_cdk.sources.declarative.requesters.paginators.strategies.cursor_pagination_strategy import CursorPaginationStrategy
 from airbyte_cdk.sources.declarative.requesters.paginators.strategies.offset_increment import OffsetIncrement
 from airbyte_cdk.sources.declarative.requesters.paginators.strategies.page_increment import PageIncrement
+from airbyte_cdk.sources.declarative.requesters.request_options import InterpolatedRequestOptionsProvider
 from airbyte_cdk.sources.declarative.retrievers.simple_retriever import SimpleRetriever
+from airbyte_cdk.sources.declarative.schema.inline_schema_loader import InlineSchemaLoader
 from airbyte_cdk.sources.declarative.schema.json_file_schema_loader import JsonFileSchemaLoader
 from airbyte_cdk.sources.declarative.spec import Spec
 from airbyte_cdk.sources.declarative.stream_slicers.cartesian_product_stream_slicer import CartesianProductStreamSlicer
-from airbyte_cdk.sources.declarative.stream_slicers.datetime_stream_slicer import DatetimeStreamSlicer
-from airbyte_cdk.sources.declarative.stream_slicers.list_stream_slicer import ListStreamSlicer
-from airbyte_cdk.sources.declarative.stream_slicers.single_slice import SingleSlice
-from airbyte_cdk.sources.declarative.stream_slicers.substream_slicer import SubstreamSlicer
 from airbyte_cdk.sources.declarative.transformations import RemoveFields
-from airbyte_cdk.sources.declarative.transformations.add_fields import AddFields
+from airbyte_cdk.sources.declarative.transformations.add_fields import AddedFieldDefinition, AddFields
+from airbyte_cdk.sources.streams.http.requests_native_auth.oauth import SingleUseRefreshTokenOauth2Authenticator
 
 """
 CLASS_TYPES_REGISTRY contains a mapping of developer-friendly string -> class to abstract the specific class referred to
 """
-CLASS_TYPES_REGISTRY: Mapping[str, Type] = {
+CLASS_TYPES_REGISTRY: Mapping[str, type] = {
+    "AddedFieldDefinition": AddedFieldDefinition,
     "AddFields": AddFields,
     "ApiKeyAuthenticator": ApiKeyAuthenticator,
     "BasicHttpAuthenticator": BasicHttpAuthenticator,
     "BearerAuthenticator": BearerAuthenticator,
     "CartesianProductStreamSlicer": CartesianProductStreamSlicer,
+    "CheckStream": CheckStream,
     "CompositeErrorHandler": CompositeErrorHandler,
     "ConstantBackoffStrategy": ConstantBackoffStrategy,
     "CursorPagination": CursorPaginationStrategy,
-    "DatetimeStreamSlicer": DatetimeStreamSlicer,
+    "DatetimeBasedCursor": DatetimeBasedCursor,
     "DeclarativeStream": DeclarativeStream,
     "DefaultErrorHandler": DefaultErrorHandler,
     "DefaultPaginator": DefaultPaginator,
     "DpathExtractor": DpathExtractor,
     "ExponentialBackoffStrategy": ExponentialBackoffStrategy,
     "HttpRequester": HttpRequester,
+    "HttpResponseFilter": HttpResponseFilter,
+    "InlineSchemaLoader": InlineSchemaLoader,
     "InterpolatedBoolean": InterpolatedBoolean,
+    "InterpolatedRequestOptionsProvider": InterpolatedRequestOptionsProvider,
     "InterpolatedString": InterpolatedString,
-    "JsonSchema": JsonFileSchemaLoader,  # todo remove after hacktoberfest and update connectors to use JsonFileSchemaLoader
     "JsonFileSchemaLoader": JsonFileSchemaLoader,
-    "ListStreamSlicer": ListStreamSlicer,
+    "JwtAuthenticator": JwtAuthenticator,
+    "ListPartitionRouter": ListPartitionRouter,
     "MinMaxDatetime": MinMaxDatetime,
     "NoAuth": NoAuth,
     "NoPagination": NoPagination,
     "OAuthAuthenticator": DeclarativeOauth2Authenticator,
+    "SingleUseRefreshTokenOAuthAuthenticator": SingleUseRefreshTokenOauth2Authenticator,
     "OffsetIncrement": OffsetIncrement,
     "PageIncrement": PageIncrement,
+    "ParentStreamConfig": ParentStreamConfig,
+    "RecordFilter": RecordFilter,
     "RecordSelector": RecordSelector,
+    "RequestOption": RequestOption,
     "RemoveFields": RemoveFields,
     "SimpleRetriever": SimpleRetriever,
-    "SingleSlice": SingleSlice,
     "Spec": Spec,
-    "SubstreamSlicer": SubstreamSlicer,
+    "SubstreamPartitionRouter": SubstreamPartitionRouter,
+    "SessionTokenAuthenticator": LegacySessionTokenAuthenticator,
     "WaitUntilTimeFromHeader": WaitUntilTimeFromHeaderBackoffStrategy,
     "WaitTimeFromHeader": WaitTimeFromHeaderBackoffStrategy,
 }
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/parsers/default_implementation_registry.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/parsers/default_implementation_registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from typing import Mapping, Type
 
 from airbyte_cdk.sources.declarative.checks.check_stream import CheckStream
 from airbyte_cdk.sources.declarative.checks.connection_checker import ConnectionChecker
 from airbyte_cdk.sources.declarative.datetime.min_max_datetime import MinMaxDatetime
@@ -12,14 +12,15 @@
 from airbyte_cdk.sources.declarative.decoders.json_decoder import JsonDecoder
 from airbyte_cdk.sources.declarative.extractors.dpath_extractor import DpathExtractor
 from airbyte_cdk.sources.declarative.extractors.http_selector import HttpSelector
 from airbyte_cdk.sources.declarative.extractors.record_extractor import RecordExtractor
 from airbyte_cdk.sources.declarative.extractors.record_selector import RecordSelector
 from airbyte_cdk.sources.declarative.interpolation.interpolated_boolean import InterpolatedBoolean
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
+from airbyte_cdk.sources.declarative.partition_routers.single_partition_router import SinglePartitionRouter
 from airbyte_cdk.sources.declarative.requesters.error_handlers.default_error_handler import DefaultErrorHandler
 from airbyte_cdk.sources.declarative.requesters.error_handlers.error_handler import ErrorHandler
 from airbyte_cdk.sources.declarative.requesters.error_handlers.http_response_filter import HttpResponseFilter
 from airbyte_cdk.sources.declarative.requesters.http_requester import HttpRequester
 from airbyte_cdk.sources.declarative.requesters.paginators.default_paginator import RequestOption
 from airbyte_cdk.sources.declarative.requesters.paginators.no_pagination import NoPagination
 from airbyte_cdk.sources.declarative.requesters.paginators.paginator import Paginator
@@ -28,15 +29,14 @@
 )
 from airbyte_cdk.sources.declarative.requesters.request_options.request_options_provider import RequestOptionsProvider
 from airbyte_cdk.sources.declarative.requesters.requester import Requester
 from airbyte_cdk.sources.declarative.retrievers.retriever import Retriever
 from airbyte_cdk.sources.declarative.retrievers.simple_retriever import SimpleRetriever
 from airbyte_cdk.sources.declarative.schema import DefaultSchemaLoader
 from airbyte_cdk.sources.declarative.schema.schema_loader import SchemaLoader
-from airbyte_cdk.sources.declarative.stream_slicers.single_slice import SingleSlice
 from airbyte_cdk.sources.declarative.stream_slicers.stream_slicer import StreamSlicer
 from airbyte_cdk.sources.declarative.stream_slicers.substream_slicer import ParentStreamConfig
 from airbyte_cdk.sources.streams.core import Stream
 
 """
 DEFAULT_IMPLEMENTATIONS_REGISTRY contains a mapping of interface -> subclass
 enabling the factory to instantiate a reasonable default class when no type or classname is specified
@@ -56,9 +56,9 @@
     RecordExtractor: DpathExtractor,
     RequestOption: RequestOption,
     RequestOptionsProvider: InterpolatedRequestOptionsProvider,
     Requester: HttpRequester,
     Retriever: SimpleRetriever,
     SchemaLoader: DefaultSchemaLoader,
     Stream: DeclarativeStream,
-    StreamSlicer: SingleSlice,
+    StreamSlicer: SinglePartitionRouter,
 }
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/parsers/manifest_reference_resolver.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/parsers/manifest_reference_resolver.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
-from copy import deepcopy
-from typing import Any, Mapping, Tuple, Union
+import re
+from typing import Any, Mapping, Set, Tuple, Union
 
-from airbyte_cdk.sources.declarative.parsers.undefined_reference_exception import UndefinedReferenceException
+from airbyte_cdk.sources.declarative.parsers.custom_exceptions import CircularReferenceException, UndefinedReferenceException
+
+REF_TAG = "$ref"
 
 
 class ManifestReferenceResolver:
     """
     An incoming manifest can contain references to values previously defined.
     This parser will dereference these values to produce a complete ConnectionDefinition.
 
-    References can be defined using a *ref(<arg>) string.
+    References can be defined using a #/<arg> string.
     ```
     key: 1234
-    reference: "*ref(key)"
+    reference: "#/key"
     ```
     will produce the following definition:
     ```
     key: 1234
     reference: 1234
     ```
     This also works with objects:
     ```
     key_value_pairs:
       k1: v1
       k2: v2
-    same_key_value_pairs: "*ref(key_value_pairs)"
+    same_key_value_pairs: "#/key_value_pairs"
     ```
     will produce the following definition:
     ```
     key_value_pairs:
       k1: v1
       k2: v2
     same_key_value_pairs:
@@ -42,15 +44,15 @@
 
     The $ref keyword can be used to refer to an object and enhance it with addition key-value pairs
     ```
     key_value_pairs:
       k1: v1
       k2: v2
     same_key_value_pairs:
-      $ref: "*ref(key_value_pairs)"
+      $ref: "#/key_value_pairs"
       k3: v3
     ```
     will produce the following definition:
     ```
     key_value_pairs:
       k1: v1
       k2: v2
@@ -62,125 +64,143 @@
 
     References can also point to nested values.
     Nested references are ambiguous because one could define a key containing with `.`
     in this example, we want to refer to the limit key in the dict object:
     ```
     dict:
         limit: 50
-    limit_ref: "*ref(dict.limit)"
+    limit_ref: "#/dict/limit"
     ```
     will produce the following definition:
     ```
     dict
         limit: 50
     limit-ref: 50
     ```
 
-    whereas here we want to access the `nested.path` value.
+    whereas here we want to access the `nested/path` value.
     ```
     nested:
         path: "first one"
-    nested.path: "uh oh"
-    value: "ref(nested.path)
+    nested/path: "uh oh"
+    value: "#/nested/path
     ```
     will produce the following definition:
     ```
     nested:
         path: "first one"
-    nested.path: "uh oh"
+    nested/path: "uh oh"
     value: "uh oh"
     ```
 
     to resolve the ambiguity, we try looking for the reference key at the top level, and then traverse the structs downward
     until we find a key with the given path, or until there is nothing to traverse.
     """
 
-    ref_tag = "$ref"
-
-    def preprocess_manifest(self, manifest: Mapping[str, Any], evaluated_mapping: Mapping[str, Any], path: Union[str, Tuple[str]]):
-
+    def preprocess_manifest(self, manifest: Mapping[str, Any]) -> Mapping[str, Any]:
         """
         :param manifest: incoming manifest that could have references to previously defined components
-        :param evaluated_mapping: mapping produced by dereferencing the content of input_mapping
-        :param path: curent path in configuration traversal
         :return:
         """
-        d = {}
-        if self.ref_tag in manifest:
-            partial_ref_string = manifest[self.ref_tag]
-            d = deepcopy(self._preprocess(partial_ref_string, evaluated_mapping, path))
-
-        for key, value in manifest.items():
-            if key == self.ref_tag:
-                continue
-            full_path = self._resolve_value(key, path)
-            if full_path in evaluated_mapping:
-                raise Exception(f"Databag already contains key={key} with path {full_path}")
-            processed_value = self._preprocess(value, evaluated_mapping, full_path)
-            evaluated_mapping[full_path] = processed_value
-            d[key] = processed_value
-
-        return d
-
-    def _get_ref_key(self, s: str) -> str:
-        ref_start = s.find("*ref(")
-        if ref_start == -1:
-            return None
-        return s[ref_start + 5 : s.find(")")]
-
-    def _resolve_value(self, value: str, path):
-        if path:
-            return *path, value
-        else:
-            return (value,)
+        return self._evaluate_node(manifest, manifest, set())  # type: ignore[no-any-return]
 
-    def _preprocess(self, value, evaluated_config: Mapping[str, Any], path):
-        if isinstance(value, str):
-            ref_key = self._get_ref_key(value)
-            if ref_key is None:
-                return value
+    def _evaluate_node(self, node: Any, manifest: Mapping[str, Any], visited: Set[Any]) -> Any:
+        if isinstance(node, dict):
+            evaluated_dict = {k: self._evaluate_node(v, manifest, visited) for k, v in node.items() if not self._is_ref_key(k)}
+            if REF_TAG in node:
+                # The node includes a $ref key, so we splat the referenced value(s) into the evaluated dict
+                evaluated_ref = self._evaluate_node(node[REF_TAG], manifest, visited)
+                if not isinstance(evaluated_ref, dict):
+                    return evaluated_ref
+                else:
+                    # The values defined on the component take precedence over the reference values
+                    return evaluated_ref | evaluated_dict
             else:
-                """
-                references are ambiguous because one could define a key containing with `.`
-                in this example, we want to refer to the limit key in the dict object:
-                    dict:
-                        limit: 50
-                    limit_ref: "*ref(dict.limit)"
-
-                whereas here we want to access the `nested.path` value.
-                  nested:
-                    path: "first one"
-                  nested.path: "uh oh"
-                  value: "ref(nested.path)
-
-                to resolve the ambiguity, we try looking for the reference key at the top level, and then traverse the structs downward
-                until we find a key with the given path, or until there is nothing to traverse.
-                """
-                key = (ref_key,)
-                while key[-1]:
-                    if key in evaluated_config:
-                        return evaluated_config[key]
-                    else:
-                        split = key[-1].split(".")
-                        key = *key[:-1], split[0], ".".join(split[1:])
-                raise UndefinedReferenceException(path, ref_key)
-        elif isinstance(value, dict):
-            return self.preprocess_manifest(value, evaluated_config, path)
-        elif type(value) == list:
-            evaluated_list = [
-                # pass in elem's path instead of the list's path
-                self._preprocess(v, evaluated_config, self._get_path_for_list_item(path, index))
-                for index, v in enumerate(value)
-            ]
-            # Add the list's element to the evaluated config so they can be referenced
-            for index, elem in enumerate(evaluated_list):
-                evaluated_config[self._get_path_for_list_item(path, index)] = elem
-            return evaluated_list
+                return evaluated_dict
+        elif isinstance(node, list):
+            return [self._evaluate_node(v, manifest, visited) for v in node]
+        elif self._is_ref(node):
+            if node in visited:
+                raise CircularReferenceException(node)
+            visited.add(node)
+            ret = self._evaluate_node(self._lookup_ref_value(node, manifest), manifest, visited)
+            visited.remove(node)
+            return ret
         else:
-            return value
+            return node
 
-    def _get_path_for_list_item(self, path, index):
-        # An elem's path is {path_to_list}[{index}]
-        if len(path) > 1:
-            return path[:-1], f"{path[-1]}[{index}]"
-        else:
-            return (f"{path[-1]}[{index}]",)
+    def _lookup_ref_value(self, ref: str, manifest: Mapping[str, Any]) -> Any:
+        ref_match = re.match(r"#/(.*)", ref)
+        if not ref_match:
+            raise ValueError(f"Invalid reference format {ref}")
+        try:
+            path = ref_match.groups()[0]
+            return self._read_ref_value(path, manifest)
+        except (AttributeError, KeyError, IndexError):
+            raise UndefinedReferenceException(path, ref)
+
+    @staticmethod
+    def _is_ref(node: Any) -> bool:
+        return isinstance(node, str) and node.startswith("#/")
+
+    @staticmethod
+    def _is_ref_key(key: str) -> bool:
+        return bool(key == REF_TAG)
+
+    @staticmethod
+    def _read_ref_value(ref: str, manifest_node: Mapping[str, Any]) -> Any:
+        """
+        Read the value at the referenced location of the manifest.
+
+        References are ambiguous because one could define a key containing `/`
+        In this example, we want to refer to the `limit` key in the `dict` object:
+            dict:
+                limit: 50
+            limit_ref: "#/dict/limit"
+
+        Whereas here we want to access the `nested/path` value.
+          nested:
+            path: "first one"
+          nested/path: "uh oh"
+          value: "#/nested/path"
+
+        To resolve the ambiguity, we try looking for the reference key at the top level, and then traverse the structs downward
+        until we find a key with the given path, or until there is nothing to traverse.
+
+        Consider the path foo/bar/baz. To resolve the ambiguity, we first try 'foo/bar/baz' in its entirety as a top-level key. If this
+        fails, we try 'foo' as the top-level key, and if this succeeds, pass 'bar/baz' on as the key to be tried at the next level.
+        """
+        while ref:
+            try:
+                return manifest_node[ref]
+            except (KeyError, TypeError):
+                head, ref = _parse_path(ref)
+                manifest_node = manifest_node[head]  # type: ignore # Couldn't figure out how to fix this since manifest_node can get reassigned into other types like lists
+        return manifest_node
+
+
+def _parse_path(ref: str) -> Tuple[Union[str, int], str]:
+    """
+    Return the next path component, together with the rest of the path.
+
+    A path component may be a string key, or an int index.
+
+    >>> _parse_path("foo/bar")
+    "foo", "bar"
+    >>> _parse_path("foo/7/8/bar")
+    "foo", "7/8/bar"
+    >>> _parse_path("7/8/bar")
+    7, "8/bar"
+    >>> _parse_path("8/bar")
+    8, "bar"
+    >>> _parse_path("8foo/bar")
+    "8foo", "bar"
+    """
+    match = re.match(r"([^/]*)/?(.*)", ref)
+    if match:
+        first, rest = match.groups()
+        try:
+            return int(first), rest
+        except ValueError:
+            return first, rest
+    else:
+        raise ValueError(f"Invalid path {ref} specified")
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/__init__.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategy import BackoffStrategy
 from airbyte_cdk.sources.declarative.requesters.error_handlers.composite_error_handler import CompositeErrorHandler
 from airbyte_cdk.sources.declarative.requesters.error_handlers.default_error_handler import DefaultErrorHandler
 from airbyte_cdk.sources.declarative.requesters.error_handlers.error_handler import ErrorHandler
 from airbyte_cdk.sources.declarative.requesters.error_handlers.http_response_filter import HttpResponseFilter
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/__init__.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategies.constant_backoff_strategy import ConstantBackoffStrategy
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategies.exponential_backoff_strategy import (
     ExponentialBackoffStrategy,
 )
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategies.wait_time_from_header_backoff_strategy import (
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/constant_backoff_strategy.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/exponential_backoff_strategy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
 from typing import Any, Mapping, Optional, Union
 
 import requests
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategy import BackoffStrategy
-from airbyte_cdk.sources.declarative.types import Config
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config
 
 
 @dataclass
-class ConstantBackoffStrategy(BackoffStrategy, JsonSchemaMixin):
+class ExponentialBackoffStrategy(BackoffStrategy):
     """
-    Backoff strategy with a constant backoff interval
+    Backoff strategy with an exponential backoff interval
 
     Attributes:
-        backoff_time_in_seconds (float): time to backoff before retrying a retryable request.
+        factor (float): multiplicative factor
     """
 
-    backoff_time_in_seconds: Union[float, InterpolatedString, str]
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     config: Config
+    factor: Union[float, InterpolatedString, str] = 5
 
-    def __post_init__(self, options: Mapping[str, Any]):
-        if not isinstance(self.backoff_time_in_seconds, InterpolatedString):
-            self.backoff_time_in_seconds = str(self.backoff_time_in_seconds)
-        self.backoff_time_in_seconds = InterpolatedString.create(self.backoff_time_in_seconds, options=options)
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        if not isinstance(self.factor, InterpolatedString):
+            self.factor = str(self.factor)
+        if isinstance(self.factor, float):
+            self.factor = InterpolatedString.create(str(self.factor), parameters=parameters)
+        else:
+            self.factor = InterpolatedString.create(self.factor, parameters=parameters)
 
     def backoff(self, response: requests.Response, attempt_count: int) -> Optional[float]:
-        return self.backoff_time_in_seconds.eval(self.config)
+        return self.factor.eval(self.config) * 2**attempt_count  # type: ignore # factor is always cast to an interpolated string
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/header_helper.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/header_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import numbers
 from re import Pattern
 from typing import Optional
 
 import requests
 
 
-def get_numeric_value_from_header(response: requests.Response, header: str, regex: Optional[Pattern]) -> Optional[float]:
+def get_numeric_value_from_header(response: requests.Response, header: str, regex: Optional[Pattern[str]]) -> Optional[float]:
     """
     Extract a header value from the response as a float
     :param response: response the extract header value from
     :param header: Header to extract
     :param regex: optional regex to apply on the header to obtain the value
     :return: header value as float if it's a number. None otherwise
     """
@@ -23,15 +23,15 @@
     if isinstance(header_value, str):
         if regex:
             match = regex.match(header_value)
             if match:
                 header_value = match.group()
         return _as_float(header_value)
     elif isinstance(header_value, numbers.Number):
-        return float(header_value)
+        return float(header_value)  # type: ignore[arg-type]
     else:
         return None
 
 
 def _as_float(s: str) -> Optional[float]:
     try:
         return float(s)
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_time_from_header_backoff_strategy.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_time_from_header_backoff_strategy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import re
 from dataclasses import InitVar, dataclass
 from typing import Any, Mapping, Optional, Union
 
 import requests
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategies.header_helper import get_numeric_value_from_header
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategy import BackoffStrategy
-from airbyte_cdk.sources.declarative.types import Config
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config
 
 
 @dataclass
-class WaitTimeFromHeaderBackoffStrategy(BackoffStrategy, JsonSchemaMixin):
+class WaitTimeFromHeaderBackoffStrategy(BackoffStrategy):
     """
     Extract wait time from http header
 
     Attributes:
         header (str): header to read wait time from
         regex (Optional[str]): optional regex to apply on the header to extract its value
     """
 
     header: Union[InterpolatedString, str]
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     config: Config
-    regex: Optional[str] = None
+    regex: Optional[Union[InterpolatedString, str]] = None
 
-    def __post_init__(self, options: Mapping[str, Any]):
-        self.regex = re.compile(self.regex) if self.regex else None
-        self.header = InterpolatedString.create(self.header, options=options)
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        self.regex = InterpolatedString.create(self.regex, parameters=parameters) if self.regex else None
+        self.header = InterpolatedString.create(self.header, parameters=parameters)
 
     def backoff(self, response: requests.Response, attempt_count: int) -> Optional[float]:
-        header = self.header.eval(config=self.config)
-        header_value = get_numeric_value_from_header(response, header, self.regex)
+        header = self.header.eval(config=self.config)  # type: ignore  # header is always cast to an interpolated stream
+        if self.regex:
+            evaled_regex = self.regex.eval(self.config)  # type: ignore # header is always cast to an interpolated string
+            regex = re.compile(evaled_regex)
+        else:
+            regex = None
+        header_value = get_numeric_value_from_header(response, header, regex)
         return header_value
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_until_time_from_header_backoff_strategy.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategies/wait_until_time_from_header_backoff_strategy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,62 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import numbers
 import re
 import time
 from dataclasses import InitVar, dataclass
 from typing import Any, Mapping, Optional, Union
 
 import requests
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategies.header_helper import get_numeric_value_from_header
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategy import BackoffStrategy
-from airbyte_cdk.sources.declarative.types import Config
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config
 
 
 @dataclass
-class WaitUntilTimeFromHeaderBackoffStrategy(BackoffStrategy, JsonSchemaMixin):
+class WaitUntilTimeFromHeaderBackoffStrategy(BackoffStrategy):
     """
     Extract time at which we can retry the request from response header
     and wait for the difference between now and that time
 
     Attributes:
         header (str): header to read wait time from
         min_wait (Optional[float]): minimum time to wait for safety
         regex (Optional[str]): optional regex to apply on the header to extract its value
     """
 
     header: Union[InterpolatedString, str]
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     config: Config
     min_wait: Optional[Union[float, InterpolatedString, str]] = None
     regex: Optional[Union[InterpolatedString, str]] = None
 
-    def __post_init__(self, options: Mapping[str, Any]):
-        self.header = InterpolatedString.create(self.header, options=options)
-        self.regex = InterpolatedString.create(self.regex, options=options) if self.regex else None
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        self.header = InterpolatedString.create(self.header, parameters=parameters)
+        self.regex = InterpolatedString.create(self.regex, parameters=parameters) if self.regex else None
         if not isinstance(self.min_wait, InterpolatedString):
-            self.min_wait = InterpolatedString.create(str(self.min_wait), options=options)
+            self.min_wait = InterpolatedString.create(str(self.min_wait), parameters=parameters)
 
     def backoff(self, response: requests.Response, attempt_count: int) -> Optional[float]:
         now = time.time()
-        header = self.header.eval(self.config)
+        header = self.header.eval(self.config)  # type: ignore # header is always cast to an interpolated string
         if self.regex:
-            evaled_regex = self.regex.eval(self.config)
+            evaled_regex = self.regex.eval(self.config)  # type: ignore # header is always cast to an interpolated string
             regex = re.compile(evaled_regex)
         else:
             regex = None
         wait_until = get_numeric_value_from_header(response, header, regex)
-        min_wait = self.min_wait.eval(self.config)
+        min_wait = self.min_wait.eval(self.config)  # type: ignore # header is always cast to an interpolated string
         if wait_until is None or not wait_until:
-            return min_wait
+            return float(min_wait) if min_wait else None
         if (isinstance(wait_until, str) and wait_until.isnumeric()) or isinstance(wait_until, numbers.Number):
             wait_time = float(wait_until) - now
         else:
-            return self.min_wait
+            return float(min_wait)
         if min_wait:
-            return max(wait_time, min_wait)
+            return float(max(wait_time, min_wait))
         elif wait_time < 0:
             return None
         return wait_time
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategy.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/backoff_strategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from abc import abstractmethod
 from dataclasses import dataclass
 from typing import Optional
 
 import requests
-from dataclasses_jsonschema import JsonSchemaMixin
 
 
 @dataclass
-class BackoffStrategy(JsonSchemaMixin):
+class BackoffStrategy:
     """
     Backoff strategy defining how long to wait before retrying a request that resulted in an error.
     """
 
     @abstractmethod
     def backoff(self, response: requests.Response, attempt_count: int) -> Optional[float]:
         """
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/composite_error_handler.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/composite_error_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
 from typing import Any, List, Mapping, Union
 
 import airbyte_cdk.sources.declarative.requesters.error_handlers.response_status as response_status
 import requests
 from airbyte_cdk.sources.declarative.requesters.error_handlers.error_handler import ErrorHandler
 from airbyte_cdk.sources.declarative.requesters.error_handlers.response_action import ResponseAction
 from airbyte_cdk.sources.declarative.requesters.error_handlers.response_status import ResponseStatus
-from dataclasses_jsonschema import JsonSchemaMixin
 
 
 @dataclass
-class CompositeErrorHandler(ErrorHandler, JsonSchemaMixin):
+class CompositeErrorHandler(ErrorHandler):
     """
     Error handler that sequentially iterates over a list of `ErrorHandler`s
 
     Sample config chaining 2 different retriers:
         error_handler:
           type: "CompositeErrorHandler"
           error_handlers:
@@ -35,26 +34,30 @@
                 - type: "ConstantBackoff"
                   backoff_time_in_seconds: 10
     Attributes:
         error_handlers (List[ErrorHandler]): list of error handlers
     """
 
     error_handlers: List[ErrorHandler]
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
 
-    def __post_init__(self, options: Mapping[str, Any]):
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
         if not self.error_handlers:
             raise ValueError("CompositeErrorHandler expects at least 1 underlying error handler")
 
     @property
     def max_retries(self) -> Union[int, None]:
         return self.error_handlers[0].max_retries
 
+    @property
+    def max_time(self) -> Union[int, None]:
+        return max([error_handler.max_time or 0 for error_handler in self.error_handlers])
+
     def interpret_response(self, response: requests.Response) -> ResponseStatus:
-        should_retry = None
+        should_retry = ResponseStatus(ResponseAction.FAIL)
         for retrier in self.error_handlers:
             should_retry = retrier.interpret_response(response)
             if should_retry.action == ResponseAction.SUCCESS:
                 return response_status.SUCCESS
             if should_retry == response_status.IGNORE or should_retry.action == ResponseAction.RETRY:
                 return should_retry
         return should_retry
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/default_error_handler.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/default_error_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass, field
 from typing import Any, List, Mapping, MutableMapping, Optional, Union
 
 import airbyte_cdk.sources.declarative.requesters.error_handlers.response_status as response_status
 import requests
@@ -11,20 +11,19 @@
     ExponentialBackoffStrategy,
 )
 from airbyte_cdk.sources.declarative.requesters.error_handlers.backoff_strategy import BackoffStrategy
 from airbyte_cdk.sources.declarative.requesters.error_handlers.error_handler import ErrorHandler
 from airbyte_cdk.sources.declarative.requesters.error_handlers.http_response_filter import HttpResponseFilter
 from airbyte_cdk.sources.declarative.requesters.error_handlers.response_action import ResponseAction
 from airbyte_cdk.sources.declarative.requesters.error_handlers.response_status import ResponseStatus
-from airbyte_cdk.sources.declarative.types import Config
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config
 
 
 @dataclass
-class DefaultErrorHandler(ErrorHandler, JsonSchemaMixin):
+class DefaultErrorHandler(ErrorHandler):
     """
     Default error handler.
 
     By default, the handler will only retry server errors (HTTP 5XX) and too many requests (HTTP 429) with exponential backoff.
 
     If the response is successful, then return SUCCESS
     Otherwise, iterate over the response_filters.
@@ -88,68 +87,71 @@
         max_retries (Optional[int]): maximum retry attempts
         backoff_strategies (Optional[List[BackoffStrategy]]): list of backoff strategies to use to determine how long
         to wait before retrying
     """
 
     DEFAULT_BACKOFF_STRATEGY = ExponentialBackoffStrategy
 
-    config: Config
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     config: Config
     response_filters: Optional[List[HttpResponseFilter]] = None
     max_retries: Optional[int] = 5
+    max_time: int = 60 * 10
     _max_retries: int = field(init=False, repr=False, default=5)
+    _max_time: int = field(init=False, repr=False, default=60 * 10)
     backoff_strategies: Optional[List[BackoffStrategy]] = None
 
-    def __post_init__(self, options: Mapping[str, Any]):
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
         self.response_filters = self.response_filters or []
 
         if not self.response_filters:
             self.response_filters.append(
                 HttpResponseFilter(
-                    ResponseAction.RETRY, http_codes=HttpResponseFilter.DEFAULT_RETRIABLE_ERRORS, config=self.config, options={}
+                    ResponseAction.RETRY, http_codes=HttpResponseFilter.DEFAULT_RETRIABLE_ERRORS, config=self.config, parameters={}
                 )
             )
-            self.response_filters.append(HttpResponseFilter(ResponseAction.IGNORE, config={}, options={}))
+            self.response_filters.append(HttpResponseFilter(ResponseAction.IGNORE, config={}, parameters={}))
 
         if not self.backoff_strategies:
-            self.backoff_strategies = [DefaultErrorHandler.DEFAULT_BACKOFF_STRATEGY(options=options, config=self.config)]
+            self.backoff_strategies = [DefaultErrorHandler.DEFAULT_BACKOFF_STRATEGY(parameters=parameters, config=self.config)]
 
         self._last_request_to_attempt_count: MutableMapping[requests.PreparedRequest, int] = {}
 
-    @property
+    @property  # type: ignore # overwrite the property to handle the case where max_retries is not provided in the constructor
     def max_retries(self) -> Union[int, None]:
         return self._max_retries
 
     @max_retries.setter
-    def max_retries(self, value: Union[int, None]):
+    def max_retries(self, value: int) -> None:
         # Covers the case where max_retries is not provided in the constructor, which causes the property object
         # to be set which we need to avoid doing
         if not isinstance(value, property):
             self._max_retries = value
 
     def interpret_response(self, response: requests.Response) -> ResponseStatus:
         request = response.request
 
         if request not in self._last_request_to_attempt_count:
             self._last_request_to_attempt_count = {request: 1}
         else:
             self._last_request_to_attempt_count[request] += 1
-        for response_filter in self.response_filters:
-            matched_status = response_filter.matches(
-                response=response, backoff_time=self._backoff_time(response, self._last_request_to_attempt_count[request])
-            )
-            if matched_status is not None:
-                return matched_status
+        if self.response_filters:
+            for response_filter in self.response_filters:
+                matched_status = response_filter.matches(
+                    response=response, backoff_time=self._backoff_time(response, self._last_request_to_attempt_count[request])
+                )
+                if matched_status is not None:
+                    return matched_status
 
         if response.ok:
             return response_status.SUCCESS
         # Fail if the response matches no filters
         return response_status.FAIL
 
     def _backoff_time(self, response: requests.Response, attempt_count: int) -> Optional[float]:
         backoff = None
-        for backoff_strategies in self.backoff_strategies:
-            backoff = backoff_strategies.backoff(response, attempt_count)
-            if backoff:
-                return backoff
+        if self.backoff_strategies:
+            for backoff_strategies in self.backoff_strategies:
+                backoff = backoff_strategies.backoff(response, attempt_count)
+                if backoff:
+                    return backoff
         return backoff
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/error_handler.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/pagination_strategy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import Union
+from typing import Any, Optional
 
 import requests
-from airbyte_cdk.sources.declarative.requesters.error_handlers.response_status import ResponseStatus
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Record
 
 
 @dataclass
-class ErrorHandler(JsonSchemaMixin):
+class PaginationStrategy:
     """
-    Defines whether a request was successful and how to handle a failure.
+    Defines how to get the next page token
     """
 
     @property
     @abstractmethod
-    def max_retries(self) -> Union[int, None]:
+    def initial_token(self) -> Optional[Any]:
         """
-        Specifies maximum amount of retries for backoff policy. Return None for no limit.
+        Return the initial value of the token
+        """
+
+    @abstractmethod
+    def next_page_token(self, response: requests.Response, last_page_size: int, last_record: Optional[Record]) -> Optional[Any]:
+        """
+        :param response: response to process
+        :param last_page_size: the number of records read from the response
+        :param last_record: the last record extracted from the response
+        :return: next page token. Returns None if there are no more pages to fetch
         """
         pass
 
     @abstractmethod
-    def interpret_response(self, response: requests.Response) -> ResponseStatus:
+    def reset(self) -> None:
+        """
+        Reset the pagination's inner state
         """
-        Evaluate response status describing whether a failing request should be retried or ignored.
 
-        :param response: response to evaluate
-        :return: response status
+    @abstractmethod
+    def get_page_size(self) -> Optional[int]:
+        """
+        :return: page size: The number of records to fetch in a page. Returns None if unspecified
         """
-        pass
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/http_response_filter.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/http_response_filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
 from typing import Any, Mapping, Optional, Set, Union
 
 import requests
 from airbyte_cdk.sources.declarative.interpolation import InterpolatedString
 from airbyte_cdk.sources.declarative.interpolation.interpolated_boolean import InterpolatedBoolean
 from airbyte_cdk.sources.declarative.requesters.error_handlers.response_action import ResponseAction
 from airbyte_cdk.sources.declarative.requesters.error_handlers.response_status import ResponseStatus
-from airbyte_cdk.sources.declarative.types import Config
 from airbyte_cdk.sources.streams.http.http import HttpStream
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config
 
 
 @dataclass
-class HttpResponseFilter(JsonSchemaMixin):
+class HttpResponseFilter:
     """
     Filter to select HttpResponses
 
     Attributes:
         action (Union[ResponseAction, str]): action to execute if a request matches
         http_codes (Set[int]): http code of matching requests
         error_message_contains (str): error substring of matching requests
@@ -29,27 +28,27 @@
     """
 
     TOO_MANY_REQUESTS_ERRORS = {429}
     DEFAULT_RETRIABLE_ERRORS = set([x for x in range(500, 600)]).union(TOO_MANY_REQUESTS_ERRORS)
 
     action: Union[ResponseAction, str]
     config: Config
-    options: InitVar[Mapping[str, Any]]
-    http_codes: Set[int] = None
-    error_message_contains: str = None
+    parameters: InitVar[Mapping[str, Any]]
+    http_codes: Optional[Set[int]] = None
+    error_message_contains: Optional[str] = None
     predicate: Union[InterpolatedBoolean, str] = ""
     error_message: Union[InterpolatedString, str] = ""
 
-    def __post_init__(self, options: Mapping[str, Any]):
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
         if isinstance(self.action, str):
             self.action = ResponseAction[self.action]
         self.http_codes = self.http_codes or set()
         if isinstance(self.predicate, str):
-            self.predicate = InterpolatedBoolean(condition=self.predicate, options=options)
-        self.error_message = InterpolatedString.create(string_or_interpolated=self.error_message, options=options)
+            self.predicate = InterpolatedBoolean(condition=self.predicate, parameters=parameters)
+        self.error_message = InterpolatedString.create(string_or_interpolated=self.error_message, parameters=parameters)
 
     def matches(self, response: requests.Response, backoff_time: Optional[float] = None) -> Optional[ResponseStatus]:
         filter_action = self._matches_filter(response)
         if filter_action is not None:
             error_message = self._create_error_message(response)
             if filter_action == ResponseAction.RETRY:
                 return ResponseStatus(
@@ -64,39 +63,39 @@
     def _matches_filter(self, response: requests.Response) -> Optional[ResponseAction]:
         """
         Apply the filter on the response and return the action to execute if it matches
         :param response: The HTTP response to evaluate
         :return: The action to execute. None if the response does not match the filter
         """
         if (
-            response.status_code in self.http_codes
+            response.status_code in self.http_codes  # type: ignore # http_codes set is always initialized to a value in __post_init__
             or (self._response_matches_predicate(response))
             or (self._response_contains_error_message(response))
         ):
-            return self.action
+            return self.action  # type: ignore # action is always cast to a ResponseAction not a str
         else:
             return None
 
     @staticmethod
-    def _safe_response_json(response: requests.Response) -> dict:
+    def _safe_response_json(response: requests.Response) -> dict[str, Any]:
         try:
-            return response.json()
+            return response.json()  # type: ignore # Response.json() returns a dictionary even if the signature does not
         except requests.exceptions.JSONDecodeError:
             return {}
 
     def _create_error_message(self, response: requests.Response) -> str:
         """
         Construct an error message based on the specified message template of the filter.
         :param response: The HTTP response which can be used during interpolation
         :return: The evaluated error message string to be emitted
         """
-        return self.error_message.eval(self.config, response=self._safe_response_json(response), headers=response.headers)
+        return self.error_message.eval(self.config, response=self._safe_response_json(response), headers=response.headers)  # type: ignore # error_message is always cast to an interpolated string
 
     def _response_matches_predicate(self, response: requests.Response) -> bool:
-        return self.predicate and self.predicate.eval(None, response=self._safe_response_json(response), headers=response.headers)
+        return bool(self.predicate and self.predicate.eval(None, response=self._safe_response_json(response), headers=response.headers))  # type: ignore # predicate is always cast to an interpolated string
 
     def _response_contains_error_message(self, response: requests.Response) -> bool:
         if not self.error_message_contains:
             return False
         else:
             error_message = HttpStream.parse_response_error_message(response)
-            return error_message and self.error_message_contains in error_message
+            return bool(error_message and self.error_message_contains in error_message)
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/error_handlers/response_status.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/error_handlers/response_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
-from typing import Final, Optional, Union
+from typing import Any, Final, Optional, Union
 
 from airbyte_cdk.sources.declarative.requesters.error_handlers.response_action import ResponseAction
 
 
 class ResponseStatus:
     """
     ResponseAction amended with backoff time if an action is RETRY
@@ -23,15 +23,15 @@
         if retry_in and response_action != ResponseAction.RETRY:
             raise ValueError(f"Unexpected backoff time ({retry_in} for non-retryable response action {response_action}")
         self._retry_in = retry_in
         self._action = response_action
         self._error_message = error_message
 
     @property
-    def action(self):
+    def action(self) -> Union[ResponseAction, str]:
         """The ResponseAction to execute when a response matches the filter"""
         return self._action
 
     @property
     def retry_in(self) -> Optional[float]:
         """How long to backoff before retrying a response. None if no wait required."""
         return self._retry_in
@@ -47,20 +47,20 @@
         Returns a ResponseStatus defining how long to backoff before retrying
 
         :param retry_in: how long to backoff before retrying. None if no wait required
         :return: A response status defining how long to backoff before retrying
         """
         return ResponseStatus(ResponseAction.RETRY, retry_in)
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if not other:
             return not self
-        return self.action == other.action and self.retry_in == other.retry_in
+        return bool(self.action == other.action and self.retry_in == other.retry_in)
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash([self.action, self.retry_in])
 
 
 """Response is successful. No need to retry"""
 SUCCESS: Final[ResponseStatus] = ResponseStatus(ResponseAction.SUCCESS)
 """Response is unsuccessful. The failure needs to be handled"""
 FAIL: Final[ResponseStatus] = ResponseStatus(ResponseAction.FAIL)
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/default_paginator.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/default_paginator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
-from dataclasses import InitVar, dataclass, field
-from typing import Any, List, Mapping, Optional, Union
+from dataclasses import InitVar, dataclass
+from typing import Any, Mapping, MutableMapping, Optional, Union
 
 import requests
 from airbyte_cdk.sources.declarative.decoders.decoder import Decoder
 from airbyte_cdk.sources.declarative.decoders.json_decoder import JsonDecoder
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
 from airbyte_cdk.sources.declarative.requesters.paginators.paginator import Paginator
 from airbyte_cdk.sources.declarative.requesters.paginators.strategies.pagination_strategy import PaginationStrategy
 from airbyte_cdk.sources.declarative.requesters.request_option import RequestOption, RequestOptionType
-from airbyte_cdk.sources.declarative.types import Config, StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.declarative.requesters.request_path import RequestPath
+from airbyte_cdk.sources.types import Config, Record, StreamSlice, StreamState
 
 
 @dataclass
-class DefaultPaginator(Paginator, JsonSchemaMixin):
+class DefaultPaginator(Paginator):
     """
     Default paginator to request pages of results with a fixed size until the pagination strategy no longer returns a next_page_token
 
     Examples:
         1.
         * fetches up to 10 records at a time by setting the "limit" request param to 10
         * updates the request path with  "{{ response._metadata.next }}"
         ```
           paginator:
             type: "DefaultPaginator"
             page_size_option:
+              type: RequestOption
               inject_into: request_parameter
               field_name: limit
             page_token_option:
-              option_type: path
+              type: RequestPath
+              path: "location"
             pagination_strategy:
               type: "CursorPagination"
               cursor_value: "{{ response._metadata.next }}"
               page_size: 10
         ```
 
         2.
         * fetches up to 5 records at a time by setting the "page_size" header to 5
         * increments a record counter and set the request parameter "offset" to the value of the counter
         ```
           paginator:
             type: "DefaultPaginator"
             page_size_option:
+              type: RequestOption
               inject_into: header
               field_name: page_size
             pagination_strategy:
               type: "OffsetIncrement"
               page_size: 5
             page_token_option:
               option_type: "request_parameter"
@@ -59,70 +62,72 @@
         3.
         * fetches up to 5 records at a time by setting the "page_size" request param to 5
         * increments a page counter and set the request parameter "page" to the value of the counter
         ```
           paginator:
             type: "DefaultPaginator"
             page_size_option:
+              type: RequestOption
               inject_into: request_parameter
               field_name: page_size
             pagination_strategy:
               type: "PageIncrement"
               page_size: 5
             page_token_option:
+              type: RequestOption
               option_type: "request_parameter"
               field_name: "page"
         ```
     Attributes:
         page_size_option (Optional[RequestOption]): the request option to set the page size. Cannot be injected in the path.
-        page_token_option (RequestOption): the request option to set the page token
+        page_token_option (Optional[RequestPath, RequestOption]): the request option to set the page token
         pagination_strategy (PaginationStrategy): Strategy defining how to get the next page token
         config (Config): connection config
         url_base (Union[InterpolatedString, str]): endpoint's base url
         decoder (Decoder): decoder to decode the response
     """
 
     pagination_strategy: PaginationStrategy
     config: Config
     url_base: Union[InterpolatedString, str]
-    options: InitVar[Mapping[str, Any]]
-    decoder: Decoder = JsonDecoder(options={})
-    _token: Optional[Any] = field(init=False, repr=False, default=None)
+    parameters: InitVar[Mapping[str, Any]]
+    decoder: Decoder = JsonDecoder(parameters={})
     page_size_option: Optional[RequestOption] = None
-    page_token_option: Optional[RequestOption] = None
+    page_token_option: Optional[Union[RequestPath, RequestOption]] = None
 
-    def __post_init__(self, options: Mapping[str, Any]):
-        if self.page_size_option and self.page_size_option.inject_into == RequestOptionType.path:
-            raise ValueError("page_size_option cannot be set in as path")
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
         if self.page_size_option and not self.pagination_strategy.get_page_size():
             raise ValueError("page_size_option cannot be set if the pagination strategy does not have a page_size")
         if isinstance(self.url_base, str):
-            self.url_base = InterpolatedString(string=self.url_base, options=options)
+            self.url_base = InterpolatedString(string=self.url_base, parameters=parameters)
+        self._token = self.pagination_strategy.initial_token
 
-    def next_page_token(self, response: requests.Response, last_records: List[Mapping[str, Any]]) -> Optional[Mapping[str, Any]]:
-        self._token = self.pagination_strategy.next_page_token(response, last_records)
+    def next_page_token(
+        self, response: requests.Response, last_page_size: int, last_record: Optional[Record]
+    ) -> Optional[Mapping[str, Any]]:
+        self._token = self.pagination_strategy.next_page_token(response, last_page_size, last_record)
         if self._token:
             return {"next_page_token": self._token}
         else:
             return None
 
-    def path(self):
-        if self._token and self.page_token_option and self.page_token_option.inject_into == RequestOptionType.path:
+    def path(self) -> Optional[str]:
+        if self._token and self.page_token_option and isinstance(self.page_token_option, RequestPath):
             # Replace url base to only return the path
-            return str(self._token).replace(self.url_base.eval(self.config), "")
+            return str(self._token).replace(self.url_base.eval(self.config), "")  # type: ignore # url_base is casted to a InterpolatedString in __post_init__
         else:
             return None
 
     def get_request_params(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Mapping[str, Any]:
+    ) -> MutableMapping[str, Any]:
         return self._get_request_options(RequestOptionType.request_parameter)
 
     def get_request_headers(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
@@ -144,19 +149,92 @@
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
         return self._get_request_options(RequestOptionType.body_json)
 
-    def reset(self):
+    def reset(self) -> None:
         self.pagination_strategy.reset()
+        self._token = self.pagination_strategy.initial_token
 
-    def _get_request_options(self, option_type: RequestOptionType) -> Mapping[str, Any]:
+    def _get_request_options(self, option_type: RequestOptionType) -> MutableMapping[str, Any]:
         options = {}
-        if self.page_token_option and self.page_token_option.inject_into == option_type:
-            if option_type != RequestOptionType.path and self._token:
-                options[self.page_token_option.field_name] = self._token
+
+        if (
+            self.page_token_option
+            and self._token is not None
+            and isinstance(self.page_token_option, RequestOption)
+            and self.page_token_option.inject_into == option_type
+        ):
+            options[self.page_token_option.field_name.eval(config=self.config)] = self._token  # type: ignore # field_name is always cast to an interpolated string
         if self.page_size_option and self.pagination_strategy.get_page_size() and self.page_size_option.inject_into == option_type:
-            if option_type != RequestOptionType.path:
-                options[self.page_size_option.field_name] = self.pagination_strategy.get_page_size()
+            options[self.page_size_option.field_name.eval(config=self.config)] = self.pagination_strategy.get_page_size()  # type: ignore # field_name is always cast to an interpolated string
         return options
+
+
+class PaginatorTestReadDecorator(Paginator):
+    """
+    In some cases, we want to limit the number of requests that are made to the backend source. This class allows for limiting the number of
+    pages that are queried throughout a read command.
+    """
+
+    _PAGE_COUNT_BEFORE_FIRST_NEXT_CALL = 1
+
+    def __init__(self, decorated: Paginator, maximum_number_of_pages: int = 5) -> None:
+        if maximum_number_of_pages and maximum_number_of_pages < 1:
+            raise ValueError(f"The maximum number of pages on a test read needs to be strictly positive. Got {maximum_number_of_pages}")
+        self._maximum_number_of_pages = maximum_number_of_pages
+        self._decorated = decorated
+        self._page_count = self._PAGE_COUNT_BEFORE_FIRST_NEXT_CALL
+
+    def next_page_token(
+        self, response: requests.Response, last_page_size: int, last_record: Optional[Record]
+    ) -> Optional[Mapping[str, Any]]:
+        if self._page_count >= self._maximum_number_of_pages:
+            return None
+
+        self._page_count += 1
+        return self._decorated.next_page_token(response, last_page_size, last_record)
+
+    def path(self) -> Optional[str]:
+        return self._decorated.path()
+
+    def get_request_params(
+        self,
+        *,
+        stream_state: Optional[StreamState] = None,
+        stream_slice: Optional[StreamSlice] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
+    ) -> Mapping[str, Any]:
+        return self._decorated.get_request_params(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
+
+    def get_request_headers(
+        self,
+        *,
+        stream_state: Optional[StreamState] = None,
+        stream_slice: Optional[StreamSlice] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
+    ) -> Mapping[str, str]:
+        return self._decorated.get_request_headers(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
+
+    def get_request_body_data(
+        self,
+        *,
+        stream_state: Optional[StreamState] = None,
+        stream_slice: Optional[StreamSlice] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
+    ) -> Union[Mapping[str, Any], str]:
+        return self._decorated.get_request_body_data(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
+
+    def get_request_body_json(
+        self,
+        *,
+        stream_state: Optional[StreamState] = None,
+        stream_slice: Optional[StreamSlice] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
+    ) -> Mapping[str, Any]:
+        return self._decorated.get_request_body_json(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
+
+    def reset(self) -> None:
+        self._decorated.reset()
+        self._page_count = self._PAGE_COUNT_BEFORE_FIRST_NEXT_CALL
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/no_pagination.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/no_pagination.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
-from typing import Any, List, Mapping, Optional, Union
+from typing import Any, Mapping, MutableMapping, Optional, Union
 
 import requests
 from airbyte_cdk.sources.declarative.requesters.paginators.paginator import Paginator
-from airbyte_cdk.sources.declarative.types import StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Record, StreamSlice, StreamState
 
 
 @dataclass
-class NoPagination(Paginator, JsonSchemaMixin):
+class NoPagination(Paginator):
     """
     Pagination implementation that never returns a next page.
     """
 
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
 
     def path(self) -> Optional[str]:
         return None
 
     def get_request_params(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Mapping[str, Any]:
+    ) -> MutableMapping[str, Any]:
         return {}
 
     def get_request_headers(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
@@ -54,13 +53,13 @@
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
         return {}
 
-    def next_page_token(self, response: requests.Response, last_records: List[Mapping[str, Any]]) -> Mapping[str, Any]:
+    def next_page_token(self, response: requests.Response, last_page_size: int, last_record: Optional[Record]) -> Mapping[str, Any]:
         return {}
 
-    def reset(self):
+    def reset(self) -> None:
         # No state to reset
         pass
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/paginator.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/paginator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Any, List, Mapping, Optional
+from typing import Any, Mapping, Optional
 
 import requests
 from airbyte_cdk.sources.declarative.requesters.request_options.request_options_provider import RequestOptionsProvider
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Record
 
 
 @dataclass
-class Paginator(RequestOptionsProvider, JsonSchemaMixin):
+class Paginator(ABC, RequestOptionsProvider):
     """
     Defines the token to use to fetch the next page of records from the API.
 
     If needed, the Paginator will set request options to be set on the HTTP request to fetch the next page of records.
     If the next_page_token is the path to the next page of records, then it should be accessed through the `path` method
     """
 
     @abstractmethod
-    def reset(self):
+    def reset(self) -> None:
         """
         Reset the pagination's inner state
         """
 
     @abstractmethod
-    def next_page_token(self, response: requests.Response, last_records: List[Mapping[str, Any]]) -> Optional[Mapping[str, Any]]:
+    def next_page_token(
+        self, response: requests.Response, last_page_size: int, last_record: Optional[Record]
+    ) -> Optional[Mapping[str, Any]]:
         """
         Returns the next_page_token to use to fetch the next page of records.
 
         :param response: the response to process
-        :param last_records: the records extracted from the response
+        :param last_page_size: the number of records read from the response
+        :param last_record: the last record extracted from the response
         :return: A mapping {"next_page_token": <token>} for the next page from the input response object. Returning None means there are no more pages to read in this response.
         """
         pass
 
     @abstractmethod
     def path(self) -> Optional[str]:
         """
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/strategies/cursor_pagination_strategy.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/cursor_pagination_strategy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,82 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
-from typing import Any, List, Mapping, Optional, Union
+from typing import Any, Dict, Mapping, Optional, Union
 
 import requests
 from airbyte_cdk.sources.declarative.decoders.decoder import Decoder
 from airbyte_cdk.sources.declarative.decoders.json_decoder import JsonDecoder
 from airbyte_cdk.sources.declarative.interpolation.interpolated_boolean import InterpolatedBoolean
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
 from airbyte_cdk.sources.declarative.requesters.paginators.strategies.pagination_strategy import PaginationStrategy
-from airbyte_cdk.sources.declarative.types import Config
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config, Record
 
 
 @dataclass
-class CursorPaginationStrategy(PaginationStrategy, JsonSchemaMixin):
+class CursorPaginationStrategy(PaginationStrategy):
     """
     Pagination strategy that evaluates an interpolated string to define the next page token
 
     Attributes:
         page_size (Optional[int]): the number of records to request
         cursor_value (Union[InterpolatedString, str]): template string evaluating to the cursor value
         config (Config): connection config
         stop_condition (Optional[InterpolatedBoolean]): template string evaluating when to stop paginating
         decoder (Decoder): decoder to decode the response
     """
 
     cursor_value: Union[InterpolatedString, str]
     config: Config
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     page_size: Optional[int] = None
     stop_condition: Optional[Union[InterpolatedBoolean, str]] = None
-    decoder: Decoder = JsonDecoder(options={})
+    decoder: Decoder = JsonDecoder(parameters={})
 
-    def __post_init__(self, options: Mapping[str, Any]):
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
         if isinstance(self.cursor_value, str):
-            self.cursor_value = InterpolatedString.create(self.cursor_value, options=options)
+            self._cursor_value = InterpolatedString.create(self.cursor_value, parameters=parameters)
+        else:
+            self._cursor_value = self.cursor_value
         if isinstance(self.stop_condition, str):
-            self.stop_condition = InterpolatedBoolean(condition=self.stop_condition, options=options)
+            self._stop_condition: Optional[InterpolatedBoolean] = InterpolatedBoolean(condition=self.stop_condition, parameters=parameters)
+        else:
+            self._stop_condition = self.stop_condition
+
+    @property
+    def initial_token(self) -> Optional[Any]:
+        return None
 
-    def next_page_token(self, response: requests.Response, last_records: List[Mapping[str, Any]]) -> Optional[Any]:
+    def next_page_token(self, response: requests.Response, last_page_size: int, last_record: Optional[Record]) -> Optional[Any]:
         decoded_response = self.decoder.decode(response)
 
         # The default way that link is presented in requests.Response is a string of various links (last, next, etc). This
         # is not indexable or useful for parsing the cursor, so we replace it with the link dictionary from response.links
-        headers = response.headers
+        headers: Dict[str, Any] = dict(response.headers)
         headers["link"] = response.links
-
-        if self.stop_condition:
-            should_stop = self.stop_condition.eval(self.config, response=decoded_response, headers=headers, last_records=last_records)
+        if self._stop_condition:
+            should_stop = self._stop_condition.eval(
+                self.config,
+                response=decoded_response,
+                headers=headers,
+                last_record=last_record,
+                last_page_size=last_page_size,
+            )
             if should_stop:
                 return None
-        token = self.cursor_value.eval(config=self.config, last_records=last_records, response=decoded_response, headers=headers)
+        token = self._cursor_value.eval(
+            config=self.config,
+            response=decoded_response,
+            headers=headers,
+            last_record=last_record,
+            last_page_size=last_page_size,
+        )
         return token if token else None
 
-    def reset(self):
+    def reset(self) -> None:
         # No state to reset
         pass
 
     def get_page_size(self) -> Optional[int]:
         return self.page_size
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/paginators/strategies/offset_increment.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/paginators/strategies/offset_increment.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,79 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
-from typing import Any, List, Mapping, Optional
+from typing import Any, Mapping, Optional, Union
 
 import requests
+from airbyte_cdk.sources.declarative.decoders import Decoder, JsonDecoder
+from airbyte_cdk.sources.declarative.interpolation import InterpolatedString
 from airbyte_cdk.sources.declarative.requesters.paginators.strategies.pagination_strategy import PaginationStrategy
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config, Record
 
 
 @dataclass
-class OffsetIncrement(PaginationStrategy, JsonSchemaMixin):
+class OffsetIncrement(PaginationStrategy):
     """
     Pagination strategy that returns the number of records reads so far and returns it as the next page token
+    Examples:
+        # page_size to be a constant integer value
+        pagination_strategy:
+          type: OffsetIncrement
+          page_size: 2
+
+        # page_size to be a constant string value
+        pagination_strategy:
+          type: OffsetIncrement
+          page_size: "2"
+
+        # page_size to be an interpolated string value
+        pagination_strategy:
+          type: OffsetIncrement
+          page_size: "{{ parameters['items_per_page'] }}"
 
     Attributes:
-        page_size (int): the number of records to request
+        page_size (InterpolatedString): the number of records to request
     """
 
-    page_size: int
-    options: InitVar[Mapping[str, Any]]
+    config: Config
+    page_size: Optional[Union[str, int]]
+    parameters: InitVar[Mapping[str, Any]]
+    decoder: Decoder = JsonDecoder(parameters={})
+    inject_on_first_request: bool = False
 
-    def __post_init__(self, options: Mapping[str, Any]):
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
         self._offset = 0
+        page_size = str(self.page_size) if isinstance(self.page_size, int) else self.page_size
+        if page_size:
+            self._page_size: Optional[InterpolatedString] = InterpolatedString(page_size, parameters=parameters)
+        else:
+            self._page_size = None
+
+    @property
+    def initial_token(self) -> Optional[Any]:
+        if self.inject_on_first_request:
+            return self._offset
+        return None
 
-    def next_page_token(self, response: requests.Response, last_records: List[Mapping[str, Any]]) -> Optional[Any]:
-        if len(last_records) < self.page_size:
+    def next_page_token(self, response: requests.Response, last_page_size: int, last_record: Optional[Record]) -> Optional[Any]:
+        decoded_response = self.decoder.decode(response)
+
+        # Stop paginating when there are fewer records than the page size or the current page has no records
+        if (self._page_size and last_page_size < self._page_size.eval(self.config, response=decoded_response)) or last_page_size == 0:
             return None
         else:
-            self._offset += len(last_records)
+            self._offset += last_page_size
             return self._offset
 
-    def reset(self):
+    def reset(self) -> None:
         self._offset = 0
 
     def get_page_size(self) -> Optional[int]:
-        return self.page_size
+        if self._page_size:
+            page_size = self._page_size.eval(self.config)
+            if not isinstance(page_size, int):
+                raise Exception(f"{page_size} is of type {type(page_size)}. Expected {int}")
+            return page_size
+        else:
+            return None
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_input_provider.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_nested_request_input_provider.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass, field
 from typing import Any, Mapping, Optional, Union
 
-from airbyte_cdk.sources.declarative.interpolation.interpolated_mapping import InterpolatedMapping
+from airbyte_cdk.sources.declarative.interpolation.interpolated_nested_mapping import InterpolatedNestedMapping, NestedMapping
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
-from airbyte_cdk.sources.declarative.types import Config, StreamSlice, StreamState
+from airbyte_cdk.sources.types import Config, StreamSlice, StreamState
 
 
 @dataclass
-class InterpolatedRequestInputProvider:
+class InterpolatedNestedRequestInputProvider:
     """
-    Helper class that generically performs string interpolation on the provided dictionary or string input
+    Helper class that generically performs string interpolation on a provided deeply nested dictionary or string input
     """
 
-    options: InitVar[Mapping[str, Any]]
-    request_inputs: Optional[Union[str, Mapping[str, str]]] = field(default=None)
+    parameters: InitVar[Mapping[str, Any]]
+    request_inputs: Optional[Union[str, NestedMapping]] = field(default=None)
     config: Config = field(default_factory=dict)
-    _interpolator: Union[InterpolatedString, InterpolatedMapping] = field(init=False, repr=False, default=None)
-    _request_inputs: Union[str, Mapping[str, str]] = field(init=False, repr=False, default=None)
+    _interpolator: Optional[Union[InterpolatedString, InterpolatedNestedMapping]] = field(init=False, repr=False, default=None)
+    _request_inputs: Optional[Union[str, NestedMapping]] = field(init=False, repr=False, default=None)
 
-    def __post_init__(self, options: Mapping[str, Any]):
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
 
         self._request_inputs = self.request_inputs or {}
-        if isinstance(self.request_inputs, str):
-            self._interpolator = InterpolatedString(self.request_inputs, default="", options=options)
+        if isinstance(self._request_inputs, str):
+            self._interpolator = InterpolatedString(self._request_inputs, default="", parameters=parameters)
         else:
-            self._interpolator = InterpolatedMapping(self._request_inputs, options=options)
+            self._interpolator = InterpolatedNestedMapping(self._request_inputs, parameters=parameters)
 
     def eval_request_inputs(
-        self, stream_state: StreamState, stream_slice: Optional[StreamSlice] = None, next_page_token: Mapping[str, Any] = None
+        self,
+        stream_state: Optional[StreamState] = None,
+        stream_slice: Optional[StreamSlice] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
         """
         Returns the request inputs to set on an outgoing HTTP request
 
         :param stream_state: The stream state
         :param stream_slice: The stream slice
         :param next_page_token: The pagination token
         :return: The request inputs to set on an outgoing HTTP request
         """
         kwargs = {"stream_state": stream_state, "stream_slice": stream_slice, "next_page_token": next_page_token}
-        interpolated_value = self._interpolator.eval(self.config, **kwargs)
-
-        if isinstance(interpolated_value, dict):
-            non_null_tokens = {k: v for k, v in interpolated_value.items() if v is not None}
-            return non_null_tokens
-        return interpolated_value
+        return self._interpolator.eval(self.config, **kwargs)  # type: ignore  # self._interpolator is always initialized with a value and will not be None
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_options_provider.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/request_options/interpolated_request_options_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,82 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass, field
 from typing import Any, Mapping, MutableMapping, Optional, Union
 
+from airbyte_cdk.sources.declarative.interpolation.interpolated_nested_mapping import NestedMapping
+from airbyte_cdk.sources.declarative.requesters.request_options.interpolated_nested_request_input_provider import (
+    InterpolatedNestedRequestInputProvider,
+)
 from airbyte_cdk.sources.declarative.requesters.request_options.interpolated_request_input_provider import InterpolatedRequestInputProvider
 from airbyte_cdk.sources.declarative.requesters.request_options.request_options_provider import RequestOptionsProvider
-from airbyte_cdk.sources.declarative.types import Config, StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config, StreamSlice, StreamState
 
 RequestInput = Union[str, Mapping[str, str]]
+ValidRequestTypes = (str, list)
 
 
 @dataclass
-class InterpolatedRequestOptionsProvider(RequestOptionsProvider, JsonSchemaMixin):
+class InterpolatedRequestOptionsProvider(RequestOptionsProvider):
     """
     Defines the request options to set on an outgoing HTTP request by evaluating `InterpolatedMapping`s
 
     Attributes:
         config (Config): The user-provided configuration as specified by the source's spec
         request_parameters (Union[str, Mapping[str, str]]): The request parameters to set on an outgoing HTTP request
         request_headers (Union[str, Mapping[str, str]]): The request headers to set on an outgoing HTTP request
         request_body_data (Union[str, Mapping[str, str]]): The body data to set on an outgoing HTTP request
         request_body_json (Union[str, Mapping[str, str]]): The json content to set on an outgoing HTTP request
     """
 
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     config: Config = field(default_factory=dict)
     request_parameters: Optional[RequestInput] = None
     request_headers: Optional[RequestInput] = None
     request_body_data: Optional[RequestInput] = None
-    request_body_json: Optional[RequestInput] = None
+    request_body_json: Optional[NestedMapping] = None
 
-    def __post_init__(self, options: Mapping[str, Any]):
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
         if self.request_parameters is None:
             self.request_parameters = {}
         if self.request_headers is None:
             self.request_headers = {}
         if self.request_body_data is None:
             self.request_body_data = {}
         if self.request_body_json is None:
             self.request_body_json = {}
 
         if self.request_body_json and self.request_body_data:
             raise ValueError("RequestOptionsProvider should only contain either 'request_body_data' or 'request_body_json' not both")
 
         self._parameter_interpolator = InterpolatedRequestInputProvider(
-            config=self.config, request_inputs=self.request_parameters, options=options
+            config=self.config, request_inputs=self.request_parameters, parameters=parameters
         )
         self._headers_interpolator = InterpolatedRequestInputProvider(
-            config=self.config, request_inputs=self.request_headers, options=options
+            config=self.config, request_inputs=self.request_headers, parameters=parameters
         )
         self._body_data_interpolator = InterpolatedRequestInputProvider(
-            config=self.config, request_inputs=self.request_body_data, options=options
+            config=self.config, request_inputs=self.request_body_data, parameters=parameters
         )
-        self._body_json_interpolator = InterpolatedRequestInputProvider(
-            config=self.config, request_inputs=self.request_body_json, options=options
+        self._body_json_interpolator = InterpolatedNestedRequestInputProvider(
+            config=self.config, request_inputs=self.request_body_json, parameters=parameters
         )
 
     def get_request_params(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> MutableMapping[str, Any]:
-        interpolated_value = self._parameter_interpolator.eval_request_inputs(stream_state, stream_slice, next_page_token)
+        interpolated_value = self._parameter_interpolator.eval_request_inputs(
+            stream_state, stream_slice, next_page_token, valid_key_types=(str,), valid_value_types=ValidRequestTypes
+        )
         if isinstance(interpolated_value, dict):
             return interpolated_value
         return {}
 
     def get_request_headers(
         self,
         *,
@@ -82,18 +88,24 @@
 
     def get_request_body_data(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Optional[Union[Mapping, str]]:
-        return self._body_data_interpolator.eval_request_inputs(stream_state, stream_slice, next_page_token)
+    ) -> Union[Mapping[str, Any], str]:
+        return self._body_data_interpolator.eval_request_inputs(
+            stream_state,
+            stream_slice,
+            next_page_token,
+            valid_key_types=(str,),
+            valid_value_types=ValidRequestTypes,
+        )
 
     def get_request_body_json(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Optional[Mapping]:
+    ) -> Mapping[str, Any]:
         return self._body_json_interpolator.eval_request_inputs(stream_state, stream_slice, next_page_token)
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/request_options/request_options_provider.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/request_options/request_options_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import Any, Mapping, MutableMapping, Optional, Union
+from typing import Any, Mapping, Optional, Union
 
-from airbyte_cdk.sources.declarative.types import StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import StreamSlice, StreamState
 
 
 @dataclass
-class RequestOptionsProvider(JsonSchemaMixin):
+class RequestOptionsProvider:
     """
     Defines the request options to set on an outgoing HTTP request
 
     Options can be passed by
     - request parameter
     - request headers
     - body data
@@ -25,15 +24,15 @@
     @abstractmethod
     def get_request_params(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> MutableMapping[str, Any]:
+    ) -> Mapping[str, Any]:
         """
         Specifies the query parameters that should be set on an outgoing HTTP request given the inputs.
 
         E.g: you might want to define query parameters for paging if next_page_token is not None.
         """
         pass
 
@@ -50,15 +49,15 @@
     @abstractmethod
     def get_request_body_data(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Optional[Union[Mapping, str]]:
+    ) -> Union[Mapping[str, Any], str]:
         """
         Specifies how to populate the body of the request with a non-JSON payload.
 
         If returns a ready text that it will be sent as is.
         If returns a dict that it will be converted to a urlencoded form.
         E.g. {"key1": "value1", "key2": "value2"} => "key1=value1&key2=value2"
 
@@ -68,13 +67,13 @@
     @abstractmethod
     def get_request_body_json(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Optional[Mapping]:
+    ) -> Mapping[str, Any]:
         """
         Specifies how to populate the body of the request with a JSON payload.
 
         At the same time only one of the 'request_body_data' and 'request_body_json' functions can be overridden.
         """
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/requesters/requester.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/requester.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from abc import abstractmethod
 from enum import Enum
-from typing import Any, Mapping, MutableMapping, Optional
+from typing import Any, Callable, Mapping, MutableMapping, Optional, Union
 
 import requests
+from airbyte_cdk.sources.declarative.auth.declarative_authenticator import DeclarativeAuthenticator
 from airbyte_cdk.sources.declarative.requesters.error_handlers.response_status import ResponseStatus
 from airbyte_cdk.sources.declarative.requesters.request_options.request_options_provider import RequestOptionsProvider
-from airbyte_cdk.sources.declarative.types import StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
-from requests.auth import AuthBase
+from airbyte_cdk.sources.types import StreamSlice, StreamState
 
 
 class HttpMethod(Enum):
     """
     Http Method to use when submitting an outgoing HTTP request
     """
 
     GET = "GET"
     POST = "POST"
 
 
-class Requester(RequestOptionsProvider, JsonSchemaMixin):
+class Requester(RequestOptionsProvider):
     @abstractmethod
-    def get_authenticator(self) -> AuthBase:
+    def get_authenticator(self) -> DeclarativeAuthenticator:
         """
         Specifies the authenticator to use when submitting requests
         """
         pass
 
     @abstractmethod
     def get_url_base(self) -> str:
@@ -96,15 +95,15 @@
     @abstractmethod
     def get_request_body_data(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Optional[Mapping[str, Any]]:
+    ) -> Union[Mapping[str, Any], str]:
         """
         Specifies how to populate the body of the request with a non-JSON payload.
 
         If returns a ready text that it will be sent as is.
         If returns a dict that it will be converted to a urlencoded form.
         E.g. {"key1": "value1", "key2": "value2"} => "key1=value1&key2=value2"
 
@@ -114,41 +113,34 @@
     @abstractmethod
     def get_request_body_json(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Optional[Mapping[str, Any]]:
+    ) -> Mapping[str, Any]:
         """
         Specifies how to populate the body of the request with a JSON payload.
 
         At the same time only one of the 'request_body_data' and 'request_body_json' functions can be overridden.
         """
 
     @abstractmethod
-    def request_kwargs(
+    def send_request(
         self,
-        *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Mapping[str, Any]:
-        """
-        Returns a mapping of keyword arguments to be used when creating the HTTP request.
-        Any option listed in https://docs.python-requests.org/en/latest/api/#requests.adapters.BaseAdapter.send for can be returned from
-        this method. Note that these options do not conflict with request-level options such as headers, request params, etc..
-        """
+        path: Optional[str] = None,
+        request_headers: Optional[Mapping[str, Any]] = None,
+        request_params: Optional[Mapping[str, Any]] = None,
+        request_body_data: Optional[Union[Mapping[str, Any], str]] = None,
+        request_body_json: Optional[Mapping[str, Any]] = None,
+        log_formatter: Optional[Callable[[requests.Response], Any]] = None,
+    ) -> Optional[requests.Response]:
+        """
+        Sends a request and returns the response. Might return no response if the error handler chooses to ignore the response or throw an exception in case of an error.
+        If path is set, the path configured on the requester itself is ignored.
+        If header, params and body are set, they are merged with the ones configured on the requester itself.
 
-    @property
-    @abstractmethod
-    def cache_filename(self) -> str:
-        """
-        Return the name of cache file
-        """
-
-    @property
-    @abstractmethod
-    def use_cache(self) -> bool:
-        """
-        If True, all records will be cached.
+        If a log formatter is provided, it's used to log the performed request and response. If it's not provided, no logging is performed.
         """
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/retrievers/retriever.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/retrievers/retriever.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import Iterable, List, Optional
+from typing import Any, Iterable, Mapping, Optional
 
-from airbyte_cdk.models import SyncMode
-from airbyte_cdk.sources.declarative.types import StreamSlice, StreamState
+from airbyte_cdk.sources.declarative.incremental.per_partition_cursor import StreamSlice
 from airbyte_cdk.sources.streams.core import StreamData
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import StreamState
 
 
 @dataclass
-class Retriever(JsonSchemaMixin):
+class Retriever:
     """
     Responsible for fetching a stream's records from an HTTP API source.
     """
 
     @abstractmethod
     def read_records(
         self,
-        sync_mode: SyncMode,
-        cursor_field: Optional[List[str]] = None,
+        records_schema: Mapping[str, Any],
         stream_slice: Optional[StreamSlice] = None,
-        stream_state: Optional[StreamState] = None,
     ) -> Iterable[StreamData]:
         """
         Fetch a stream's records from an HTTP API source
 
-        :param sync_mode: Unused but currently necessary for integrating with HttpStream
-        :param cursor_field: Unused but currently necessary for integrating with HttpStream
+        :param records_schema: json schema to describe record
         :param stream_slice: The stream slice to read data for
-        :param stream_state: The initial stream state
         :return: The records read from the API source
         """
 
     @abstractmethod
-    def stream_slices(self, *, sync_mode: SyncMode, stream_state: Optional[StreamState] = None) -> Iterable[Optional[StreamSlice]]:
+    def stream_slices(self) -> Iterable[Optional[StreamSlice]]:
         """Returns the stream slices"""
 
     @property
     @abstractmethod
     def state(self) -> StreamState:
         """State getter, should return state in form that can serialized to a string and send to the output
         as a STATE AirbyteMessage.
@@ -53,9 +48,9 @@
 
          State should try to be as small as possible but at the same time descriptive enough to restore
          syncing process from the point where it stopped.
         """
 
     @state.setter
     @abstractmethod
-    def state(self, value: StreamState):
+    def state(self, value: StreamState) -> None:
         """State setter, accept state serialized by state getter."""
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/retrievers/simple_retriever.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/retrievers/simple_retriever.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
-import json
-import logging
 from dataclasses import InitVar, dataclass, field
-from typing import Any, Iterable, List, Mapping, MutableMapping, Optional, Union
+from functools import partial
+from itertools import islice
+from typing import Any, Callable, Iterable, List, Mapping, Optional, Set, Tuple, Union
 
 import requests
-from airbyte_cdk.models import AirbyteLogMessage, AirbyteMessage, Level, SyncMode
-from airbyte_cdk.models import Type as MessageType
-from airbyte_cdk.sources.declarative.exceptions import ReadException
+from airbyte_cdk.models import AirbyteMessage
 from airbyte_cdk.sources.declarative.extractors.http_selector import HttpSelector
+from airbyte_cdk.sources.declarative.incremental.declarative_cursor import DeclarativeCursor
 from airbyte_cdk.sources.declarative.interpolation import InterpolatedString
-from airbyte_cdk.sources.declarative.requesters.error_handlers.response_action import ResponseAction
+from airbyte_cdk.sources.declarative.partition_routers.single_partition_router import SinglePartitionRouter
 from airbyte_cdk.sources.declarative.requesters.paginators.no_pagination import NoPagination
 from airbyte_cdk.sources.declarative.requesters.paginators.paginator import Paginator
 from airbyte_cdk.sources.declarative.requesters.requester import Requester
 from airbyte_cdk.sources.declarative.retrievers.retriever import Retriever
-from airbyte_cdk.sources.declarative.stream_slicers.single_slice import SingleSlice
 from airbyte_cdk.sources.declarative.stream_slicers.stream_slicer import StreamSlicer
-from airbyte_cdk.sources.declarative.types import Config, Record, StreamSlice, StreamState
+from airbyte_cdk.sources.http_logger import format_http_message
 from airbyte_cdk.sources.streams.core import StreamData
-from airbyte_cdk.sources.streams.http import HttpStream
-from airbyte_cdk.utils.airbyte_secrets_utils import filter_secrets
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config, Record, StreamSlice, StreamState
+from airbyte_cdk.utils.mapping_helpers import combine_mappings
 
 
 @dataclass
-class SimpleRetriever(Retriever, HttpStream, JsonSchemaMixin):
+class SimpleRetriever(Retriever):
     """
     Retrieves records by synchronously sending requests to fetch records.
 
     The retriever acts as an orchestrator between the requester, the record selector, the paginator, and the stream slicer.
 
     For each stream slice, submit requests until there are no more pages of records to fetch.
 
@@ -43,382 +40,411 @@
     Attributes:
         stream_name (str): The stream's name
         stream_primary_key (Optional[Union[str, List[str], List[List[str]]]]): The stream's primary key
         requester (Requester): The HTTP requester
         record_selector (HttpSelector): The record selector
         paginator (Optional[Paginator]): The paginator
         stream_slicer (Optional[StreamSlicer]): The stream slicer
-        options (Mapping[str, Any]): Additional runtime parameters to be used for string interpolation
+        cursor (Optional[cursor]): The cursor
+        parameters (Mapping[str, Any]): Additional runtime parameters to be used for string interpolation
     """
 
     requester: Requester
     record_selector: HttpSelector
     config: Config
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     name: str
     _name: Union[InterpolatedString, str] = field(init=False, repr=False, default="")
     primary_key: Optional[Union[str, List[str], List[List[str]]]]
     _primary_key: str = field(init=False, repr=False, default="")
     paginator: Optional[Paginator] = None
-    stream_slicer: Optional[StreamSlicer] = SingleSlice(options={})
+    stream_slicer: StreamSlicer = SinglePartitionRouter(parameters={})
+    cursor: Optional[DeclarativeCursor] = None
+    ignore_stream_slicer_parameters_on_paginated_requests: bool = False
+
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        self._paginator = self.paginator or NoPagination(parameters=parameters)
+        self._last_response: Optional[requests.Response] = None
+        self._last_page_size: int = 0
+        self._last_record: Optional[Record] = None
+        self._parameters = parameters
+        self._name = InterpolatedString(self._name, parameters=parameters) if isinstance(self._name, str) else self._name
 
-    def __post_init__(self, options: Mapping[str, Any]):
-        self.paginator = self.paginator or NoPagination(options=options)
-        HttpStream.__init__(self, self.requester.get_authenticator())
-        self._last_response = None
-        self._last_records = None
-        self._options = options
-        self.name = InterpolatedString(self._name, options=options)
-
-    @property
+    @property  # type: ignore
     def name(self) -> str:
         """
         :return: Stream name
         """
-        return self._name.eval(self.config)
+        return str(self._name.eval(self.config)) if isinstance(self._name, InterpolatedString) else self._name
 
     @name.setter
     def name(self, value: str) -> None:
         if not isinstance(value, property):
             self._name = value
 
-    @property
-    def url_base(self) -> str:
-        return self.requester.get_url_base()
-
-    @property
-    def http_method(self) -> str:
-        return str(self.requester.get_method().value)
-
-    @property
-    def raise_on_http_errors(self) -> bool:
-        # never raise on http_errors because this overrides the error handler logic...
-        return False
-
-    def should_retry(self, response: requests.Response) -> bool:
-        """
-        Specifies conditions for backoff based on the response from the server.
-
-        By default, back off on the following HTTP response statuses:
-         - 429 (Too Many Requests) indicating rate limiting
-         - 500s to handle transient server errors
-
-        Unexpected but transient exceptions (connection timeout, DNS resolution failed, etc..) are retried by default.
-        """
-        return self.requester.interpret_response_status(response).action == ResponseAction.RETRY
-
-    def backoff_time(self, response: requests.Response) -> Optional[float]:
-        """
-        Specifies backoff time.
-
-         This method is called only if should_backoff() returns True for the input request.
-
-         :param response:
-         :return how long to backoff in seconds. The return value may be a floating point number for subsecond precision. Returning None defers backoff
-         to the default backoff behavior (e.g using an exponential algorithm).
-        """
-        should_retry = self.requester.interpret_response_status(response)
-        if should_retry.action != ResponseAction.RETRY:
-            raise ValueError(f"backoff_time can only be applied on retriable response action. Got {should_retry.action}")
-        assert should_retry.action == ResponseAction.RETRY
-        return should_retry.retry_in
-
-    def error_message(self, response: requests.Response) -> str:
-        """
-        Constructs an error message which can incorporate the HTTP response received from the partner API.
-
-        :param response: The incoming HTTP response from the partner API
-        :return The error message string to be emitted
-        """
-        return self.requester.interpret_response_status(response).error_message
+    def _get_mapping(
+        self, method: Callable[..., Optional[Union[Mapping[str, Any], str]]], **kwargs: Any
+    ) -> Tuple[Union[Mapping[str, Any], str], Set[str]]:
+        """
+        Get mapping from the provided method, and get the keys of the mapping.
+        If the method returns a string, it will return the string and an empty set.
+        If the method returns a dict, it will return the dict and its keys.
+        """
+        mapping = method(**kwargs) or {}
+        keys = set(mapping.keys()) if not isinstance(mapping, str) else set()
+        return mapping, keys
 
     def _get_request_options(
         self,
+        stream_state: Optional[StreamData],
         stream_slice: Optional[StreamSlice],
         next_page_token: Optional[Mapping[str, Any]],
-        requester_method,
-        paginator_method,
-        stream_slicer_method,
-    ):
+        paginator_method: Callable[..., Optional[Union[Mapping[str, Any], str]]],
+        stream_slicer_method: Callable[..., Optional[Union[Mapping[str, Any], str]]],
+    ) -> Union[Mapping[str, Any], str]:
         """
-        Get the request_option from the requester and from the paginator
+        Get the request_option from the paginator and the stream slicer.
         Raise a ValueError if there's a key collision
         Returned merged mapping otherwise
-        :param stream_slice:
-        :param next_page_token:
-        :param requester_method:
-        :param paginator_method:
-        :return:
         """
+        # FIXME we should eventually remove the usage of stream_state as part of the interpolation
+        mappings = [
+            paginator_method(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token),
+        ]
+        if not next_page_token or not self.ignore_stream_slicer_parameters_on_paginated_requests:
+            mappings.append(stream_slicer_method(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token))
+        return combine_mappings(mappings)
 
-        requester_mapping = requester_method(stream_state=self.state, stream_slice=stream_slice, next_page_token=next_page_token)
-        requester_mapping_keys = set(requester_mapping.keys())
-        paginator_mapping = paginator_method(stream_state=self.state, stream_slice=stream_slice, next_page_token=next_page_token)
-        paginator_mapping_keys = set(paginator_mapping.keys())
-        stream_slicer_mapping = stream_slicer_method(stream_slice=stream_slice)
-        stream_slicer_mapping_keys = set(stream_slicer_mapping.keys())
-
-        intersection = (
-            (requester_mapping_keys & paginator_mapping_keys)
-            | (requester_mapping_keys & stream_slicer_mapping_keys)
-            | (paginator_mapping_keys & stream_slicer_mapping_keys)
-        )
-        if intersection:
-            raise ValueError(f"Duplicate keys found: {intersection}")
-        return {**requester_mapping, **paginator_mapping, **stream_slicer_mapping}
-
-    def request_headers(
-        self, stream_state: StreamState, stream_slice: Optional[StreamSlice] = None, next_page_token: Optional[Mapping[str, Any]] = None
+    def _request_headers(
+        self,
+        stream_state: Optional[StreamData] = None,
+        stream_slice: Optional[StreamSlice] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
         """
         Specifies request headers.
         Authentication headers will overwrite any overlapping headers returned from this method.
         """
         headers = self._get_request_options(
+            stream_state,
             stream_slice,
             next_page_token,
-            self.requester.get_request_headers,
-            self.paginator.get_request_headers,
+            self._paginator.get_request_headers,
             self.stream_slicer.get_request_headers,
         )
+        if isinstance(headers, str):
+            raise ValueError("Request headers cannot be a string")
         return {str(k): str(v) for k, v in headers.items()}
 
-    def request_params(
+    def _request_params(
         self,
-        stream_state: StreamSlice,
+        stream_state: Optional[StreamData] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> MutableMapping[str, Any]:
+    ) -> Mapping[str, Any]:
         """
         Specifies the query parameters that should be set on an outgoing HTTP request given the inputs.
 
         E.g: you might want to define query parameters for paging if next_page_token is not None.
         """
-        return self._get_request_options(
+        params = self._get_request_options(
+            stream_state,
             stream_slice,
             next_page_token,
-            self.requester.get_request_params,
-            self.paginator.get_request_params,
+            self._paginator.get_request_params,
             self.stream_slicer.get_request_params,
         )
+        if isinstance(params, str):
+            raise ValueError("Request params cannot be a string")
+        return params
 
-    def request_body_data(
+    def _request_body_data(
         self,
-        stream_state: StreamState,
+        stream_state: Optional[StreamData] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Optional[Union[Mapping, str]]:
+    ) -> Union[Mapping[str, Any], str]:
         """
         Specifies how to populate the body of the request with a non-JSON payload.
 
         If returns a ready text that it will be sent as is.
         If returns a dict that it will be converted to a urlencoded form.
         E.g. {"key1": "value1", "key2": "value2"} => "key1=value1&key2=value2"
 
         At the same time only one of the 'request_body_data' and 'request_body_json' functions can be overridden.
         """
-        # Warning: use self.state instead of the stream_state passed as argument!
-        base_body_data = self.requester.get_request_body_data(
-            stream_state=self.state, stream_slice=stream_slice, next_page_token=next_page_token
-        )
-        if isinstance(base_body_data, str):
-            paginator_body_data = self.paginator.get_request_body_data()
-            if paginator_body_data:
-                raise ValueError(
-                    f"Cannot combine requester's body data= {base_body_data} with paginator's body_data: {paginator_body_data}"
-                )
-            else:
-                return base_body_data
         return self._get_request_options(
+            stream_state,
             stream_slice,
             next_page_token,
-            self.requester.get_request_body_data,
-            self.paginator.get_request_body_data,
+            self._paginator.get_request_body_data,
             self.stream_slicer.get_request_body_data,
         )
 
-    def request_body_json(
+    def _request_body_json(
         self,
-        stream_state: StreamState,
+        stream_state: Optional[StreamData] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Optional[Mapping]:
+    ) -> Optional[Mapping[str, Any]]:
         """
         Specifies how to populate the body of the request with a JSON payload.
 
         At the same time only one of the 'request_body_data' and 'request_body_json' functions can be overridden.
         """
-        # Warning: use self.state instead of the stream_state passed as argument!
-        return self._get_request_options(
+        body_json = self._get_request_options(
+            stream_state,
             stream_slice,
             next_page_token,
-            self.requester.get_request_body_json,
-            self.paginator.get_request_body_json,
+            self._paginator.get_request_body_json,
             self.stream_slicer.get_request_body_json,
         )
+        if isinstance(body_json, str):
+            raise ValueError("Request body json cannot be a string")
+        return body_json
 
-    def request_kwargs(
-        self,
-        stream_state: StreamState,
-        stream_slice: Optional[StreamSlice] = None,
-        next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Mapping[str, Any]:
-        """
-        Specifies how to configure a mapping of keyword arguments to be used when creating the HTTP request.
-        Any option listed in https://docs.python-requests.org/en/latest/api/#requests.adapters.BaseAdapter.send for can be returned from
-        this method. Note that these options do not conflict with request-level options such as headers, request params, etc..
-        """
-        # Warning: use self.state instead of the stream_state passed as argument!
-        return self.requester.request_kwargs(stream_state=self.state, stream_slice=stream_slice, next_page_token=next_page_token)
-
-    def path(
+    def _paginator_path(
         self,
-        *,
-        stream_state: Optional[StreamState] = None,
-        stream_slice: Optional[StreamSlice] = None,
-        next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> str:
+    ) -> Optional[str]:
         """
-        Return the path the submit the next request to.
-        If the paginator points to a path, follow it, else return the requester's path
+        If the paginator points to a path, follow it, else return nothing so the requester is used.
         :param stream_state:
         :param stream_slice:
         :param next_page_token:
         :return:
         """
-        # Warning: use self.state instead of the stream_state passed as argument!
-        paginator_path = self.paginator.path()
-        if paginator_path:
-            return paginator_path
-        else:
-            return self.requester.get_path(stream_state=self.state, stream_slice=stream_slice, next_page_token=next_page_token)
-
-    @property
-    def cache_filename(self) -> str:
-        """
-        Return the name of cache file
-        """
-        return self.requester.cache_filename
+        return self._paginator.path()
 
-    @property
-    def use_cache(self) -> bool:
-        """
-        If True, all records will be cached.
-        """
-        return self.requester.use_cache
-
-    def parse_response(
+    def _parse_response(
         self,
-        response: requests.Response,
-        *,
+        response: Optional[requests.Response],
         stream_state: StreamState,
+        records_schema: Mapping[str, Any],
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Iterable[Record]:
-        # if fail -> raise exception
-        # if ignore -> ignore response and return no records
-        # else -> delegate to record selector
-        response_status = self.requester.interpret_response_status(response)
-        if response_status.action == ResponseAction.FAIL:
-            error_message = response_status.error_message or f"Request {response.request} failed with response {response}"
-            raise ReadException(error_message)
-        elif response_status.action == ResponseAction.IGNORE:
-            self.logger.info(f"Ignoring response for failed request with error message {HttpStream.parse_response_error_message(response)}")
+        if not response:
+            self._last_response = None
             return []
 
-        # Warning: use self.state instead of the stream_state passed as argument!
         self._last_response = response
-        records = self.record_selector.select_records(
-            response=response, stream_state=self.state, stream_slice=stream_slice, next_page_token=next_page_token
+        record_generator = self.record_selector.select_records(
+            response=response,
+            stream_state=stream_state,
+            records_schema=records_schema,
+            stream_slice=stream_slice,
+            next_page_token=next_page_token,
         )
-        self._last_records = records
-        return records
+        self._last_page_size = 0
+        for record in record_generator:
+            self._last_page_size += 1
+            self._last_record = record
+            yield record
 
-    @property
+    @property  # type: ignore
     def primary_key(self) -> Optional[Union[str, List[str], List[List[str]]]]:
         """The stream's primary key"""
         return self._primary_key
 
     @primary_key.setter
     def primary_key(self, value: str) -> None:
         if not isinstance(value, property):
             self._primary_key = value
 
-    def next_page_token(self, response: requests.Response) -> Optional[Mapping[str, Any]]:
+    def _next_page_token(self, response: requests.Response) -> Optional[Mapping[str, Any]]:
         """
         Specifies a pagination strategy.
 
         The value returned from this method is passed to most other methods in this class. Use it to form a request e.g: set headers or query params.
 
         :return: The token for the next page from the input response object. Returning None means there are no more pages to read in this response.
         """
-        return self.paginator.next_page_token(response, self._last_records)
+        return self._paginator.next_page_token(response, self._last_page_size, self._last_record)
+
+    def _fetch_next_page(
+        self, stream_state: Mapping[str, Any], stream_slice: StreamSlice, next_page_token: Optional[Mapping[str, Any]] = None
+    ) -> Optional[requests.Response]:
+        return self.requester.send_request(
+            path=self._paginator_path(),
+            stream_state=stream_state,
+            stream_slice=stream_slice,
+            next_page_token=next_page_token,
+            request_headers=self._request_headers(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token),
+            request_params=self._request_params(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token),
+            request_body_data=self._request_body_data(
+                stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token
+            ),
+            request_body_json=self._request_body_json(
+                stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token
+            ),
+        )
+
+    # This logic is similar to _read_pages in the HttpStream class. When making changes here, consider making changes there as well.
+    def _read_pages(
+        self,
+        records_generator_fn: Callable[[Optional[requests.Response]], Iterable[StreamData]],
+        stream_state: Mapping[str, Any],
+        stream_slice: StreamSlice,
+    ) -> Iterable[StreamData]:
+        pagination_complete = False
+        next_page_token = None
+        while not pagination_complete:
+            response = self._fetch_next_page(stream_state, stream_slice, next_page_token)
+            yield from records_generator_fn(response)
+
+            if not response:
+                pagination_complete = True
+            else:
+                next_page_token = self._next_page_token(response)
+                if not next_page_token:
+                    pagination_complete = True
+
+        # Always return an empty generator just in case no records were ever yielded
+        yield from []
 
     def read_records(
         self,
-        sync_mode: SyncMode,
-        cursor_field: Optional[List[str]] = None,
+        records_schema: Mapping[str, Any],
         stream_slice: Optional[StreamSlice] = None,
-        stream_state: Optional[StreamState] = None,
     ) -> Iterable[StreamData]:
-        # Warning: use self.state instead of the stream_state passed as argument!
-        stream_slice = stream_slice or {}  # None-check
-        self.paginator.reset()
-        records_generator = self._read_pages(
-            self.parse_records_and_emit_request_and_responses,
-            stream_slice,
-            stream_state,
+        """
+        Fetch a stream's records from an HTTP API source
+
+        :param records_schema: json schema to describe record
+        :param stream_slice: The stream slice to read data for
+        :return: The records read from the API source
+        """
+        _slice = stream_slice or StreamSlice(partition={}, cursor_slice={})  # None-check
+        # Fixing paginator types has a long tail of dependencies
+        self._paginator.reset()
+
+        most_recent_record_from_slice = None
+        record_generator = partial(
+            self._parse_records,
+            stream_state=self.state or {},
+            stream_slice=_slice,
+            records_schema=records_schema,
         )
-        for record in records_generator:
-            # Only record messages should be parsed to update the cursor which is indicated by the Mapping type
-            if isinstance(record, Mapping):
-                self.stream_slicer.update_cursor(stream_slice, last_record=record)
-            yield record
+        for stream_data in self._read_pages(record_generator, self.state, _slice):
+            current_record = self._extract_record(stream_data, _slice)
+            if self.cursor and current_record:
+                self.cursor.observe(_slice, current_record)
+
+            # Latest record read, not necessarily within slice boundaries.
+            # TODO Remove once all custom components implement `observe` method.
+            # https://github.com/airbytehq/airbyte-internal-issues/issues/6955
+            most_recent_record_from_slice = self._get_most_recent_record(most_recent_record_from_slice, current_record, _slice)
+            yield stream_data
+
+        if self.cursor:
+            self.cursor.close_slice(_slice, most_recent_record_from_slice)
+        return
+
+    def _get_most_recent_record(
+        self, current_most_recent: Optional[Record], current_record: Optional[Record], stream_slice: StreamSlice
+    ) -> Optional[Record]:
+        if self.cursor and current_record:
+            if not current_most_recent:
+                return current_record
+            else:
+                return current_most_recent if self.cursor.is_greater_than_or_equal(current_most_recent, current_record) else current_record
         else:
-            last_record = self._last_records[-1] if self._last_records else None
-            if last_record and isinstance(last_record, Mapping):
-                self.stream_slicer.update_cursor(stream_slice, last_record=last_record)
-            yield from []
-
-    def stream_slices(
-        self, *, sync_mode: SyncMode, cursor_field: List[str] = None, stream_state: Optional[StreamState] = None
-    ) -> Iterable[Optional[Mapping[str, Any]]]:
+            return None
+
+    @staticmethod
+    def _extract_record(stream_data: StreamData, stream_slice: StreamSlice) -> Optional[Record]:
+        """
+        As we allow the output of _read_pages to be StreamData, it can be multiple things. Therefore, we need to filter out and normalize
+        to data to streamline the rest of the process.
+        """
+        if isinstance(stream_data, Record):
+            # Record is not part of `StreamData` but is the most common implementation of `Mapping[str, Any]` which is part of `StreamData`
+            return stream_data
+        elif isinstance(stream_data, (dict, Mapping)):
+            return Record(dict(stream_data), stream_slice)
+        elif isinstance(stream_data, AirbyteMessage) and stream_data.record:
+            return Record(stream_data.record.data, stream_slice)
+        return None
+
+    # stream_slices is defined with arguments on http stream and fixing this has a long tail of dependencies. Will be resolved by the decoupling of http stream and simple retriever
+    def stream_slices(self) -> Iterable[Optional[StreamSlice]]:  # type: ignore
         """
         Specifies the slices for this stream. See the stream slicing section of the docs for more information.
 
         :param sync_mode:
         :param cursor_field:
         :param stream_state:
         :return:
         """
-        # Warning: use self.state instead of the stream_state passed as argument!
-        return self.stream_slicer.stream_slices(sync_mode, self.state)
+        return self.stream_slicer.stream_slices()
 
     @property
-    def state(self) -> MutableMapping[str, Any]:
-        return self.stream_slicer.get_stream_state()
+    def state(self) -> Mapping[str, Any]:
+        return self.cursor.get_stream_state() if self.cursor else {}
 
     @state.setter
-    def state(self, value: StreamState):
+    def state(self, value: StreamState) -> None:
         """State setter, accept state serialized by state getter."""
-        self.stream_slicer.update_cursor(value)
+        if self.cursor:
+            self.cursor.set_initial_state(value)
 
-    def parse_records_and_emit_request_and_responses(self, request, response, stream_slice, stream_state) -> Iterable[StreamData]:
-        # Only emit requests and responses when running in debug mode
-        if self.logger.isEnabledFor(logging.DEBUG):
-            yield self._create_trace_message_from_request(request)
-            yield self._create_trace_message_from_response(response)
-        # Not great to need to call _read_pages which is a private method
-        # A better approach would be to extract the HTTP client from the HttpStream and call it directly from the HttpRequester
-        yield from self.parse_response(response, stream_slice=stream_slice, stream_state=stream_state)
-
-    def _create_trace_message_from_request(self, request: requests.PreparedRequest):
-        # FIXME: this should return some sort of trace message
-        request_dict = {"url": request.url, "headers": dict(request.headers), "body": request.body}
-        log_message = filter_secrets(f"request:{json.dumps(request_dict)}")
-        return AirbyteMessage(type=MessageType.LOG, log=AirbyteLogMessage(level=Level.INFO, message=log_message))
-
-    def _create_trace_message_from_response(self, response: requests.Response):
-        # FIXME: this should return some sort of trace message
-        response_dict = {"body": response.text, "headers": dict(response.headers), "status_code": response.status_code}
-        log_message = filter_secrets(f"response:{json.dumps(response_dict)}")
-        return AirbyteMessage(type=MessageType.LOG, log=AirbyteLogMessage(level=Level.INFO, message=log_message))
+    def _parse_records(
+        self,
+        response: Optional[requests.Response],
+        stream_state: Mapping[str, Any],
+        records_schema: Mapping[str, Any],
+        stream_slice: Optional[StreamSlice],
+    ) -> Iterable[StreamData]:
+        yield from self._parse_response(
+            response,
+            stream_slice=stream_slice,
+            stream_state=stream_state,
+            records_schema=records_schema,
+        )
+
+    def must_deduplicate_query_params(self) -> bool:
+        return True
+
+
+@dataclass
+class SimpleRetrieverTestReadDecorator(SimpleRetriever):
+    """
+    In some cases, we want to limit the number of requests that are made to the backend source. This class allows for limiting the number of
+    slices that are queried throughout a read command.
+    """
+
+    maximum_number_of_slices: int = 5
+
+    def __post_init__(self, options: Mapping[str, Any]) -> None:
+        super().__post_init__(options)
+        if self.maximum_number_of_slices and self.maximum_number_of_slices < 1:
+            raise ValueError(
+                f"The maximum number of slices on a test read needs to be strictly positive. Got {self.maximum_number_of_slices}"
+            )
+
+    # stream_slices is defined with arguments on http stream and fixing this has a long tail of dependencies. Will be resolved by the decoupling of http stream and simple retriever
+    def stream_slices(self) -> Iterable[Optional[StreamSlice]]:  # type: ignore
+        return islice(super().stream_slices(), self.maximum_number_of_slices)
+
+    def _fetch_next_page(
+        self, stream_state: Mapping[str, Any], stream_slice: StreamSlice, next_page_token: Optional[Mapping[str, Any]] = None
+    ) -> Optional[requests.Response]:
+        return self.requester.send_request(
+            path=self._paginator_path(),
+            stream_state=stream_state,
+            stream_slice=stream_slice,
+            next_page_token=next_page_token,
+            request_headers=self._request_headers(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token),
+            request_params=self._request_params(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token),
+            request_body_data=self._request_body_data(
+                stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token
+            ),
+            request_body_json=self._request_body_json(
+                stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token
+            ),
+            log_formatter=lambda response: format_http_message(
+                response,
+                f"Stream '{self.name}' request",
+                f"Request performed in order to extract records for stream '{self.name}'",
+                self.name,
+            ),
+        )
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/schema/default_schema_loader.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/schema/default_schema_loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import logging
 from dataclasses import InitVar, dataclass
 from typing import Any, Mapping
 
 from airbyte_cdk.sources.declarative.schema.json_file_schema_loader import JsonFileSchemaLoader
 from airbyte_cdk.sources.declarative.schema.schema_loader import SchemaLoader
-from airbyte_cdk.sources.declarative.types import Config
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config
 
 
 @dataclass
-class DefaultSchemaLoader(SchemaLoader, JsonSchemaMixin):
+class DefaultSchemaLoader(SchemaLoader):
     """
     Loads a schema from the default location or returns an empty schema for streams that have not defined their schema file yet.
 
     Attributes:
         config (Config): The user-provided configuration as specified by the source's spec
-        options (Mapping[str, Any]): Additional arguments to pass to the string interpolation if needed
+        parameters (Mapping[str, Any]): Additional arguments to pass to the string interpolation if needed
     """
 
     config: Config
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
 
-    def __post_init__(self, options: Mapping[str, Any]):
-        self._options = options
-        self.default_loader = JsonFileSchemaLoader(options=options, config=self.config)
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        self._parameters = parameters
+        self.default_loader = JsonFileSchemaLoader(parameters=parameters, config=self.config)
 
     def get_json_schema(self) -> Mapping[str, Any]:
         """
         Attempts to retrieve a schema from the default filepath location or returns the empty schema if a schema cannot be found.
 
         :return: The empty schema
         """
 
         try:
             return self.default_loader.get_json_schema()
         except OSError:
             # A slight hack since we don't directly have the stream name. However, when building the default filepath we assume the
             # runtime options stores stream name 'name' so we'll do the same here
-            stream_name = self._options.get("name", "")
+            stream_name = self._parameters.get("name", "")
             logging.info(f"Could not find schema for stream {stream_name}, defaulting to the empty schema")
             return {}
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/schema/json_file_schema_loader.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/schema/json_file_schema_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,80 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import json
 import pkgutil
 import sys
 from dataclasses import InitVar, dataclass, field
-from typing import Any, Mapping, Union
+from typing import Any, Mapping, Tuple, Union
 
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
 from airbyte_cdk.sources.declarative.schema.schema_loader import SchemaLoader
-from airbyte_cdk.sources.declarative.types import Config
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config
+from airbyte_cdk.sources.utils.schema_helpers import ResourceSchemaLoader
 
 
 def _default_file_path() -> str:
     # Schema files are always in "source_<connector_name>/schemas/<stream_name>.json
     # The connector's module name can be inferred by looking at the modules loaded and look for the one starting with source_
     source_modules = [
         k for k, v in sys.modules.items() if "source_" in k
     ]  # example: ['source_exchange_rates', 'source_exchange_rates.source']
     if source_modules:
         module = source_modules[0].split(".")[0]
-        return f"./{module}/schemas/{{{{options['name']}}}}.json"
+        return f"./{module}/schemas/{{{{parameters['name']}}}}.json"
 
     # If we are not in a source_ module, the most likely scenario is we're processing a manifest from the connector builder
     # server which does not require a json schema to be defined.
-    return "./{{options['name']}}.json"
+    return "./{{parameters['name']}}.json"
 
 
 @dataclass
-class JsonFileSchemaLoader(SchemaLoader, JsonSchemaMixin):
+class JsonFileSchemaLoader(ResourceSchemaLoader, SchemaLoader):
     """
     Loads the schema from a json file
 
     Attributes:
         file_path (Union[InterpolatedString, str]): The path to the json file describing the schema
         name (str): The stream's name
         config (Config): The user-provided configuration as specified by the source's spec
-        options (Mapping[str, Any]): Additional arguments to pass to the string interpolation if needed
+        parameters (Mapping[str, Any]): Additional arguments to pass to the string interpolation if needed
     """
 
     config: Config
-    options: InitVar[Mapping[str, Any]]
-    file_path: Union[InterpolatedString, str] = field(default=None)
+    parameters: InitVar[Mapping[str, Any]]
+    file_path: Union[InterpolatedString, str] = field(default="")
 
-    def __post_init__(self, options: Mapping[str, Any]):
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
         if not self.file_path:
             self.file_path = _default_file_path()
-        self.file_path = InterpolatedString.create(self.file_path, options=options)
+        self.file_path = InterpolatedString.create(self.file_path, parameters=parameters)
 
     def get_json_schema(self) -> Mapping[str, Any]:
         # todo: It is worth revisiting if we can replace file_path with just file_name if every schema is in the /schemas directory
         # this would require that we find a creative solution to store or retrieve source_name in here since the files are mounted there
         json_schema_path = self._get_json_filepath()
         resource, schema_path = self.extract_resource_and_schema_path(json_schema_path)
         raw_json_file = pkgutil.get_data(resource, schema_path)
 
         if not raw_json_file:
             raise IOError(f"Cannot find file {json_schema_path}")
         try:
             raw_schema = json.loads(raw_json_file)
         except ValueError as err:
             raise RuntimeError(f"Invalid JSON file format for file {json_schema_path}") from err
-        return raw_schema
+        self.package_name = resource
+        return self._resolve_schema_references(raw_schema)
 
-    def _get_json_filepath(self):
-        return self.file_path.eval(self.config)
+    def _get_json_filepath(self) -> Any:
+        return self.file_path.eval(self.config)  # type: ignore # file_path is always cast to an interpolated string
 
     @staticmethod
-    def extract_resource_and_schema_path(json_schema_path: str) -> (str, str):
+    def extract_resource_and_schema_path(json_schema_path: str) -> Tuple[str, str]:
         """
         When the connector is running on a docker container, package_data is accessible from the resource (source_<name>), so we extract
         the resource from the first part of the schema path and the remaining path is used to find the schema file. This is a slight
         hack to identify the source name while we are in the airbyte_cdk module.
         :param json_schema_path: The path to the schema JSON file
         :return: Tuple of the resource name and the path to the schema file
         """
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/cartesian_product_stream_slicer.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/stream_slicers/cartesian_product_stream_slicer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import itertools
 from collections import ChainMap
 from dataclasses import InitVar, dataclass
 from typing import Any, Iterable, List, Mapping, Optional
 
-from airbyte_cdk.models import SyncMode
 from airbyte_cdk.sources.declarative.stream_slicers.stream_slicer import StreamSlicer
-from airbyte_cdk.sources.declarative.types import StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import StreamSlice, StreamState
 
 
 @dataclass
-class CartesianProductStreamSlicer(StreamSlicer, JsonSchemaMixin):
+class CartesianProductStreamSlicer(StreamSlicer):
     """
     Stream slicers that iterates over the cartesian product of input stream slicers
     Given 2 stream slicers with the following slices:
     A: [{"i": 0}, {"i": 1}, {"i": 2}]
     B: [{"s": "hello"}, {"s": "world"}]
     the resulting stream slices are
     [
@@ -31,30 +29,26 @@
     ]
 
     Attributes:
         stream_slicers (List[StreamSlicer]): Underlying stream slicers. The RequestOptions (e.g: Request headers, parameters, etc..) returned by this slicer are the combination of the RequestOptions of its input slicers. If there are conflicts e.g: two slicers define the same header or request param, the conflict is resolved by taking the value from the first slicer, where ordering is determined by the order in which slicers were input to this composite slicer.
     """
 
     stream_slicers: List[StreamSlicer]
-    options: InitVar[Mapping[str, Any]]
-
-    def update_cursor(self, stream_slice: Mapping[str, Any], last_record: Optional[Mapping[str, Any]] = None):
-        for slicer in self.stream_slicers:
-            slicer.update_cursor(stream_slice, last_record)
+    parameters: InitVar[Mapping[str, Any]]
 
     def get_request_params(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
         return dict(
             ChainMap(
-                *[
+                *[  # type: ignore # ChainMap expects a MutableMapping[Never, Never] for reasons
                     s.get_request_params(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
                     for s in self.stream_slicers
                 ]
             )
         )
 
     def get_request_headers(
@@ -62,15 +56,15 @@
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
         return dict(
             ChainMap(
-                *[
+                *[  # type: ignore # ChainMap expects a MutableMapping[Never, Never] for reasons
                     s.get_request_headers(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
                     for s in self.stream_slicers
                 ]
             )
         )
 
     def get_request_body_data(
@@ -78,36 +72,43 @@
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
         return dict(
             ChainMap(
-                *[
+                *[  # type: ignore # ChainMap expects a MutableMapping[Never, Never] for reasons
                     s.get_request_body_data(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
                     for s in self.stream_slicers
                 ]
             )
         )
 
     def get_request_body_json(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Optional[Mapping]:
+    ) -> Mapping[str, Any]:
         return dict(
             ChainMap(
-                *[
+                *[  # type: ignore # ChainMap expects a MutableMapping[Never, Never] for reasons
                     s.get_request_body_json(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
                     for s in self.stream_slicers
                 ]
             )
         )
 
-    def get_stream_state(self) -> Mapping[str, Any]:
-        return dict(ChainMap(*[slicer.get_stream_state() for slicer in self.stream_slicers]))
-
-    def stream_slices(self, sync_mode: SyncMode, stream_state: Mapping[str, Any]) -> Iterable[Mapping[str, Any]]:
-        sub_slices = (s.stream_slices(sync_mode, stream_state) for s in self.stream_slicers)
-        return (dict(ChainMap(*a)) for a in itertools.product(*sub_slices))
+    def stream_slices(self) -> Iterable[StreamSlice]:
+        sub_slices = (s.stream_slices() for s in self.stream_slicers)
+        product = itertools.product(*sub_slices)
+        for stream_slice_tuple in product:
+            partition = dict(ChainMap(*[s.partition for s in stream_slice_tuple]))  # type: ignore # ChainMap expects a MutableMapping[Never, Never] for reasons
+            cursor_slices = [s.cursor_slice for s in stream_slice_tuple if s.cursor_slice]
+            if len(cursor_slices) > 1:
+                raise ValueError(f"There should only be a single cursor slice. Found {cursor_slices}")
+            if cursor_slices:
+                cursor_slice = cursor_slices[0]
+            else:
+                cursor_slice = {}
+            yield StreamSlice(partition=partition, cursor_slice=cursor_slice)
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/datetime_stream_slicer.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/incremental/datetime_based_cursor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,210 +1,250 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import datetime
-import re
 from dataclasses import InitVar, dataclass, field
-from typing import Any, Iterable, Mapping, Optional, Union
+from typing import Any, Callable, Iterable, List, Mapping, MutableMapping, Optional, Union
 
-from airbyte_cdk.models import SyncMode
+from airbyte_cdk.models import AirbyteLogMessage, AirbyteMessage, Level, Type
 from airbyte_cdk.sources.declarative.datetime.datetime_parser import DatetimeParser
 from airbyte_cdk.sources.declarative.datetime.min_max_datetime import MinMaxDatetime
+from airbyte_cdk.sources.declarative.incremental.declarative_cursor import DeclarativeCursor
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
 from airbyte_cdk.sources.declarative.interpolation.jinja import JinjaInterpolation
 from airbyte_cdk.sources.declarative.requesters.request_option import RequestOption, RequestOptionType
-from airbyte_cdk.sources.declarative.stream_slicers.stream_slicer import StreamSlicer
-from airbyte_cdk.sources.declarative.types import Config, Record, StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
-from dateutil.relativedelta import relativedelta
+from airbyte_cdk.sources.message import MessageRepository
+from airbyte_cdk.sources.types import Config, Record, StreamSlice, StreamState
+from isodate import Duration, parse_duration
 
 
 @dataclass
-class DatetimeStreamSlicer(StreamSlicer, JsonSchemaMixin):
+class DatetimeBasedCursor(DeclarativeCursor):
     """
-    Slices the stream over a datetime range.
+    Slices the stream over a datetime range and create a state with format {<cursor_field>: <datetime> }
 
     Given a start time, end time, a step function, and an optional lookback window,
     the stream slicer will partition the date range from start time - lookback window to end time.
 
-    The step function is defined as a string of the form:
-    `"<number><unit>"`
-
-    where unit can be one of
-    - years, y
-    - months, m
-    - weeks, w
-    - days, d
-
-    For example, "1d" will produce windows of 1 day, and "2w" windows of 2 weeks.
+    The step function is defined as a string of the form ISO8601 duration
 
     The timestamp format accepts the same format codes as datetime.strfptime, which are
     all the format codes required by the 1989 C standard.
     Full list of accepted format codes: https://man7.org/linux/man-pages/man3/strftime.3.html
 
     Attributes:
         start_datetime (Union[MinMaxDatetime, str]): the datetime that determines the earliest record that should be synced
-        end_datetime (Union[MinMaxDatetime, str]): the datetime that determines the last record that should be synced
-        step (str): size of the timewindow
+        end_datetime (Optional[Union[MinMaxDatetime, str]]): the datetime that determines the last record that should be synced
         cursor_field (Union[InterpolatedString, str]): record's cursor field
         datetime_format (str): format of the datetime
+        step (Optional[str]): size of the timewindow (ISO8601 duration)
+        cursor_granularity (Optional[str]): smallest increment the datetime_format has (ISO 8601 duration) that will be used to ensure that the start of a slice does not overlap with the end of the previous one
         config (Config): connection config
         start_time_option (Optional[RequestOption]): request option for start time
         end_time_option (Optional[RequestOption]): request option for end time
-        stream_state_field_start (Optional[str]): stream slice start time field
-        stream_state_field_end (Optional[str]): stream slice end time field
-        lookback_window (Optional[InterpolatedString]): how many days before start_datetime to read data for
+        partition_field_start (Optional[str]): partition start time field
+        partition_field_end (Optional[str]): stream slice end time field
+        lookback_window (Optional[InterpolatedString]): how many days before start_datetime to read data for (ISO8601 duration)
     """
 
     start_datetime: Union[MinMaxDatetime, str]
-    end_datetime: Union[MinMaxDatetime, str]
-    step: str
     cursor_field: Union[InterpolatedString, str]
     datetime_format: str
     config: Config
-    options: InitVar[Mapping[str, Any]]
-    _cursor: dict = field(repr=False, default=None)  # tracks current datetime
-    _cursor_end: dict = field(repr=False, default=None)  # tracks end of current stream slice
+    parameters: InitVar[Mapping[str, Any]]
+    _highest_observed_cursor_field_value: Optional[str] = field(
+        repr=False, default=None
+    )  # tracks the latest observed datetime, which may not be safe to emit in the case of out-of-order records
+    _cursor: Optional[str] = field(
+        repr=False, default=None
+    )  # tracks the latest observed datetime that is appropriate to emit as stream state
+    end_datetime: Optional[Union[MinMaxDatetime, str]] = None
+    step: Optional[Union[InterpolatedString, str]] = None
+    cursor_granularity: Optional[str] = None
     start_time_option: Optional[RequestOption] = None
     end_time_option: Optional[RequestOption] = None
-    stream_state_field_start: Optional[str] = None
-    stream_state_field_end: Optional[str] = None
+    partition_field_start: Optional[str] = None
+    partition_field_end: Optional[str] = None
     lookback_window: Optional[Union[InterpolatedString, str]] = None
+    message_repository: Optional[MessageRepository] = None
+    cursor_datetime_formats: List[str] = field(default_factory=lambda: [])
 
-    timedelta_regex = re.compile(
-        r"((?P<years>[\.\d]+?)y)?" r"((?P<months>[\.\d]+?)m)?" r"((?P<weeks>[\.\d]+?)w)?" r"((?P<days>[\.\d]+?)d)?$"
-    )
-
-    def __post_init__(self, options: Mapping[str, Any]):
-        if not isinstance(self.start_datetime, MinMaxDatetime):
-            self.start_datetime = MinMaxDatetime(self.start_datetime, options)
-        if not isinstance(self.end_datetime, MinMaxDatetime):
-            self.end_datetime = MinMaxDatetime(self.end_datetime, options)
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        if (self.step and not self.cursor_granularity) or (not self.step and self.cursor_granularity):
+            raise ValueError(
+                f"If step is defined, cursor_granularity should be as well and vice-versa. "
+                f"Right now, step is `{self.step}` and cursor_granularity is `{self.cursor_granularity}`"
+            )
+        self._start_datetime = MinMaxDatetime.create(self.start_datetime, parameters)
+        self._end_datetime = None if not self.end_datetime else MinMaxDatetime.create(self.end_datetime, parameters)
 
         self._timezone = datetime.timezone.utc
         self._interpolation = JinjaInterpolation()
 
-        self._step = self._parse_timedelta(self.step)
-        self.cursor_field = InterpolatedString.create(self.cursor_field, options=options)
-        self.stream_slice_field_start = InterpolatedString.create(self.stream_state_field_start or "start_time", options=options)
-        self.stream_slice_field_end = InterpolatedString.create(self.stream_state_field_end or "end_time", options=options)
+        self._step = (
+            self._parse_timedelta(InterpolatedString.create(self.step, parameters=parameters).eval(self.config))
+            if self.step
+            else datetime.timedelta.max
+        )
+        self._cursor_granularity = self._parse_timedelta(self.cursor_granularity)
+        self._cursor_field = InterpolatedString.create(self.cursor_field, parameters=parameters)
+        self._lookback_window = InterpolatedString.create(self.lookback_window, parameters=parameters) if self.lookback_window else None
+        self._partition_field_start = InterpolatedString.create(self.partition_field_start or "start_time", parameters=parameters)
+        self._partition_field_end = InterpolatedString.create(self.partition_field_end or "end_time", parameters=parameters)
         self._parser = DatetimeParser()
 
         # If datetime format is not specified then start/end datetime should inherit it from the stream slicer
-        if not self.start_datetime.datetime_format:
-            self.start_datetime.datetime_format = self.datetime_format
-        if not self.end_datetime.datetime_format:
-            self.end_datetime.datetime_format = self.datetime_format
-
-        if self.start_time_option and self.start_time_option.inject_into == RequestOptionType.path:
-            raise ValueError("Start time cannot be passed by path")
-        if self.end_time_option and self.end_time_option.inject_into == RequestOptionType.path:
-            raise ValueError("End time cannot be passed by path")
+        if not self._start_datetime.datetime_format:
+            self._start_datetime.datetime_format = self.datetime_format
+        if self._end_datetime and not self._end_datetime.datetime_format:
+            self._end_datetime.datetime_format = self.datetime_format
+
+        if not self.cursor_datetime_formats:
+            self.cursor_datetime_formats = [self.datetime_format]
 
     def get_stream_state(self) -> StreamState:
-        return {self.cursor_field.eval(self.config): self._cursor} if self._cursor else {}
+        return {self._cursor_field.eval(self.config): self._cursor} if self._cursor else {}
 
-    def update_cursor(self, stream_slice: StreamSlice, last_record: Optional[Record] = None):
+    def set_initial_state(self, stream_state: StreamState) -> None:
         """
-        Update the cursor value to the max datetime between the last record, the start of the stream_slice, and the current cursor value.
-        Update the cursor_end value with the stream_slice's end time.
+        Cursors are not initialized with their state. As state is needed in order to function properly, this method should be called
+        before calling anything else
 
-        :param stream_slice: current stream slice
-        :param last_record: last record read
-        :return: None
-        """
-        stream_slice_value = stream_slice.get(self.cursor_field.eval(self.config))
-        stream_slice_value_end = stream_slice.get(self.stream_slice_field_end.eval(self.config))
-        last_record_value = last_record.get(self.cursor_field.eval(self.config)) if last_record else None
-        cursor = None
-        if stream_slice_value and last_record_value:
-            cursor = max(stream_slice_value, last_record_value)
-        elif stream_slice_value:
-            cursor = stream_slice_value
-        else:
-            cursor = last_record_value
-        if self._cursor and cursor:
-            self._cursor = max(cursor, self._cursor)
-        elif cursor:
-            self._cursor = cursor
-        if self.stream_slice_field_end:
-            self._cursor_end = stream_slice_value_end
+        :param stream_state: The state of the stream as returned by get_stream_state
+        """
+        self._cursor = stream_state.get(self._cursor_field.eval(self.config)) if stream_state else None
+
+    def observe(self, stream_slice: StreamSlice, record: Record) -> None:
+        """
+        Register a record with the cursor; the cursor instance can then use it to manage the state of the in-progress stream read.
+
+        :param stream_slice: The current slice, which may or may not contain the most recently observed record
+        :param record: the most recently-read record, which the cursor can use to update the stream state. Outwardly-visible changes to the
+          stream state may need to be deferred depending on whether the source reliably orders records by the cursor field.
+        """
+        record_cursor_value = record.get(self._cursor_field.eval(self.config))
+        # if the current record has no cursor value, we cannot meaningfully update the state based on it, so there is nothing more to do
+        if not record_cursor_value:
+            return
+
+        start_field = self._partition_field_start.eval(self.config)
+        end_field = self._partition_field_end.eval(self.config)
+        is_highest_observed_cursor_value = not self._highest_observed_cursor_field_value or self.parse_date(
+            record_cursor_value
+        ) > self.parse_date(self._highest_observed_cursor_field_value)
+        if (
+            self._is_within_daterange_boundaries(record, stream_slice.get(start_field), stream_slice.get(end_field))  # type: ignore # we know that stream_slices for these cursors will use a string representing an unparsed date
+            and is_highest_observed_cursor_value
+        ):
+            self._highest_observed_cursor_field_value = record_cursor_value
+
+    def close_slice(self, stream_slice: StreamSlice, *args: Any) -> None:
+        if stream_slice.partition:
+            raise ValueError(f"Stream slice {stream_slice} should not have a partition. Got {stream_slice.partition}.")
+        cursor_value_str_by_cursor_value_datetime = dict(
+            map(
+                # we need to ensure the cursor value is preserved as is in the state else the CATs might complain of something like
+                # 2023-01-04T17:30:19.000Z' <= '2023-01-04T17:30:19.000000Z'
+                lambda datetime_str: (self.parse_date(datetime_str), datetime_str),  # type: ignore # because of the filter on the next line, this will only be called with a str
+                filter(lambda item: item, [self._cursor, self._highest_observed_cursor_field_value]),
+            )
+        )
+        self._cursor = (
+            cursor_value_str_by_cursor_value_datetime[max(cursor_value_str_by_cursor_value_datetime.keys())]
+            if cursor_value_str_by_cursor_value_datetime
+            else None
+        )
 
-    def stream_slices(self, sync_mode: SyncMode, stream_state: Mapping[str, Any]) -> Iterable[Mapping[str, Any]]:
+    def stream_slices(self) -> Iterable[StreamSlice]:
         """
         Partition the daterange into slices of size = step.
 
-        The start of the window is the minimum datetime between start_datetime - looback_window and the stream_state's datetime
+        The start of the window is the minimum datetime between start_datetime - lookback_window and the stream_state's datetime
         The end of the window is the minimum datetime between the start of the window and end_datetime.
 
-        :param sync_mode:
-        :param stream_state: current stream state. If set, the start_date will be the day following the stream_state.
         :return:
         """
-        stream_state = stream_state or {}
-        kwargs = {"stream_state": stream_state}
-        end_datetime = min(self.end_datetime.get_datetime(self.config, **kwargs), datetime.datetime.now(tz=self._timezone))
-        lookback_delta = self._parse_timedelta(self.lookback_window.eval(self.config, **kwargs) if self.lookback_window else "0d")
-        start_datetime = self.start_datetime.get_datetime(self.config, **kwargs) - lookback_delta
-        start_datetime = min(start_datetime, end_datetime)
-        if self.cursor_field.eval(self.config, stream_state=stream_state) in stream_state:
-            cursor_datetime = self.parse_date(stream_state[self.cursor_field.eval(self.config)])
-        else:
-            cursor_datetime = start_datetime
-
-        start_datetime = max(cursor_datetime, start_datetime)
-
-        state_cursor_value = stream_state.get(self.cursor_field.eval(self.config, stream_state=stream_state))
+        end_datetime = self._select_best_end_datetime()
+        start_datetime = self._calculate_earliest_possible_value(self._select_best_end_datetime())
+        return self._partition_daterange(start_datetime, end_datetime, self._step)
+
+    def _calculate_earliest_possible_value(self, end_datetime: datetime.datetime) -> datetime.datetime:
+        lookback_delta = self._parse_timedelta(self._lookback_window.eval(self.config) if self._lookback_window else "P0D")
+        earliest_possible_start_datetime = min(self._start_datetime.get_datetime(self.config), end_datetime)
+        cursor_datetime = self._calculate_cursor_datetime_from_state(self.get_stream_state())
+        return max(earliest_possible_start_datetime, cursor_datetime) - lookback_delta
+
+    def _select_best_end_datetime(self) -> datetime.datetime:
+        now = datetime.datetime.now(tz=self._timezone)
+        if not self._end_datetime:
+            return now
+        return min(self._end_datetime.get_datetime(self.config), now)
+
+    def _calculate_cursor_datetime_from_state(self, stream_state: Mapping[str, Any]) -> datetime.datetime:
+        if self._cursor_field.eval(self.config, stream_state=stream_state) in stream_state:
+            return self.parse_date(stream_state[self._cursor_field.eval(self.config)])
+        return datetime.datetime.min.replace(tzinfo=datetime.timezone.utc)
 
-        if state_cursor_value:
-            state_date = self.parse_date(state_cursor_value)
-        else:
-            state_date = None
-        if state_date:
-            # If the input_state's date is greater than start_datetime, the start of the time window is the state's next day
-            next_date = state_date + datetime.timedelta(days=1)
-            start_datetime = max(start_datetime, next_date)
-        dates = self._partition_daterange(start_datetime, end_datetime, self._step)
-        return dates
-
-    def _format_datetime(self, dt: datetime.datetime):
+    def _format_datetime(self, dt: datetime.datetime) -> str:
         return self._parser.format(dt, self.datetime_format)
 
-    def _partition_daterange(self, start, end, step: datetime.timedelta):
-        start_field = self.stream_slice_field_start.eval(self.config)
-        end_field = self.stream_slice_field_end.eval(self.config)
+    def _partition_daterange(
+        self, start: datetime.datetime, end: datetime.datetime, step: Union[datetime.timedelta, Duration]
+    ) -> List[StreamSlice]:
+        start_field = self._partition_field_start.eval(self.config)
+        end_field = self._partition_field_end.eval(self.config)
         dates = []
         while start <= end:
-            end_date = self._get_date(start + step - datetime.timedelta(days=1), end, min)
-            dates.append({start_field: self._format_datetime(start), end_field: self._format_datetime(end_date)})
-            start += step
+            next_start = self._evaluate_next_start_date_safely(start, step)
+            end_date = self._get_date(next_start - self._cursor_granularity, end, min)
+            dates.append(
+                StreamSlice(
+                    partition={}, cursor_slice={start_field: self._format_datetime(start), end_field: self._format_datetime(end_date)}
+                )
+            )
+            start = next_start
         return dates
 
-    def _get_date(self, cursor_value, default_date: datetime.datetime, comparator) -> datetime.datetime:
+    def _evaluate_next_start_date_safely(self, start: datetime.datetime, step: datetime.timedelta) -> datetime.datetime:
+        """
+        Given that we set the default step at datetime.timedelta.max, we will generate an OverflowError when evaluating the next start_date
+        This method assumes that users would never enter a step that would generate an overflow. Given that would be the case, the code
+        would have broken anyway.
+        """
+        try:
+            return start + step
+        except OverflowError:
+            return datetime.datetime.max.replace(tzinfo=datetime.timezone.utc)
+
+    def _get_date(
+        self,
+        cursor_value: datetime.datetime,
+        default_date: datetime.datetime,
+        comparator: Callable[[datetime.datetime, datetime.datetime], datetime.datetime],
+    ) -> datetime.datetime:
         cursor_date = cursor_value or default_date
         return comparator(cursor_date, default_date)
 
     def parse_date(self, date: str) -> datetime.datetime:
-        return self._parser.parse(date, self.datetime_format, self._timezone)
+        for datetime_format in self.cursor_datetime_formats + [self.datetime_format]:
+            try:
+                return self._parser.parse(date, datetime_format)
+            except ValueError:
+                pass
+        raise ValueError(f"No format in {self.cursor_datetime_formats} matching {date}")
 
     @classmethod
-    def _parse_timedelta(cls, time_str):
+    def _parse_timedelta(cls, time_str: Optional[str]) -> Union[datetime.timedelta, Duration]:
         """
-        Parse a time string e.g. (2h13m) into a timedelta object.
-        Modified from virhilo's answer at https://stackoverflow.com/a/4628148/851699
-        :param time_str: A string identifying a duration. (eg. 2h13m)
-        :return relativedelta: A relativedelta object
+        :return Parses an ISO 8601 durations into datetime.timedelta or Duration objects.
         """
-        parts = cls.timedelta_regex.match(time_str)
-
-        assert parts is not None
-
-        time_params = {name: float(param) for name, param in parts.groupdict().items() if param}
-        return relativedelta(**time_params)
+        if not time_str:
+            return datetime.timedelta(0)
+        return parse_duration(time_str)
 
     def get_request_params(
         self,
         *,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
@@ -238,14 +278,68 @@
     ) -> Mapping[str, Any]:
         return self._get_request_options(RequestOptionType.body_json, stream_slice)
 
     def request_kwargs(self) -> Mapping[str, Any]:
         # Never update kwargs
         return {}
 
-    def _get_request_options(self, option_type: RequestOptionType, stream_slice: StreamSlice):
-        options = {}
+    def _get_request_options(self, option_type: RequestOptionType, stream_slice: Optional[StreamSlice]) -> Mapping[str, Any]:
+        options: MutableMapping[str, Any] = {}
+        if not stream_slice:
+            return options
         if self.start_time_option and self.start_time_option.inject_into == option_type:
-            options[self.start_time_option.field_name] = stream_slice.get(self.stream_slice_field_start.eval(self.config))
+            options[self.start_time_option.field_name.eval(config=self.config)] = stream_slice.get(  # type: ignore # field_name is always casted to an interpolated string
+                self._partition_field_start.eval(self.config)
+            )
         if self.end_time_option and self.end_time_option.inject_into == option_type:
-            options[self.end_time_option.field_name] = stream_slice.get(self.stream_slice_field_end.eval(self.config))
+            options[self.end_time_option.field_name.eval(config=self.config)] = stream_slice.get(self._partition_field_end.eval(self.config))  # type: ignore # field_name is always casted to an interpolated string
         return options
+
+    def should_be_synced(self, record: Record) -> bool:
+        cursor_field = self._cursor_field.eval(self.config)
+        record_cursor_value = record.get(cursor_field)
+        if not record_cursor_value:
+            self._send_log(
+                Level.WARN,
+                f"Could not find cursor field `{cursor_field}` in record. The incremental sync will assume it needs to be synced",
+            )
+            return True
+        latest_possible_cursor_value = self._select_best_end_datetime()
+        earliest_possible_cursor_value = self._calculate_earliest_possible_value(latest_possible_cursor_value)
+        return self._is_within_daterange_boundaries(record, earliest_possible_cursor_value, latest_possible_cursor_value)
+
+    def _is_within_daterange_boundaries(
+        self, record: Record, start_datetime_boundary: Union[datetime.datetime, str], end_datetime_boundary: Union[datetime.datetime, str]
+    ) -> bool:
+        cursor_field = self._cursor_field.eval(self.config)
+        record_cursor_value = record.get(cursor_field)
+        if not record_cursor_value:
+            self._send_log(
+                Level.WARN,
+                f"Could not find cursor field `{cursor_field}` in record. The record will not be considered when emitting sync state",
+            )
+            return False
+        if isinstance(start_datetime_boundary, str):
+            start_datetime_boundary = self.parse_date(start_datetime_boundary)
+        if isinstance(end_datetime_boundary, str):
+            end_datetime_boundary = self.parse_date(end_datetime_boundary)
+        return start_datetime_boundary <= self.parse_date(record_cursor_value) <= end_datetime_boundary
+
+    def _send_log(self, level: Level, message: str) -> None:
+        if self.message_repository:
+            self.message_repository.emit_message(
+                AirbyteMessage(
+                    type=Type.LOG,
+                    log=AirbyteLogMessage(level=level, message=message),
+                )
+            )
+
+    def is_greater_than_or_equal(self, first: Record, second: Record) -> bool:
+        cursor_field = self._cursor_field.eval(self.config)
+        first_cursor_value = first.get(cursor_field)
+        second_cursor_value = second.get(cursor_field)
+        if first_cursor_value and second_cursor_value:
+            return self.parse_date(first_cursor_value) >= self.parse_date(second_cursor_value)
+        elif first_cursor_value:
+            return True
+        else:
+            return False
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/list_stream_slicer.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/partition_routers/list_partition_router.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,48 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
 from typing import Any, Iterable, List, Mapping, Optional, Union
 
-from airbyte_cdk.models import SyncMode
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
 from airbyte_cdk.sources.declarative.requesters.request_option import RequestOption, RequestOptionType
 from airbyte_cdk.sources.declarative.stream_slicers.stream_slicer import StreamSlicer
-from airbyte_cdk.sources.declarative.types import Config, Record, StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config, StreamSlice, StreamState
 
 
 @dataclass
-class ListStreamSlicer(StreamSlicer, JsonSchemaMixin):
+class ListPartitionRouter(StreamSlicer):
     """
-    Stream slicer that iterates over the values of a list
-    If slice_values is a string, then evaluate it as literal and assert the resulting literal is a list
+    Partition router that iterates over the values of a list
+    If values is a string, then evaluate it as literal and assert the resulting literal is a list
 
     Attributes:
-        slice_values (Union[str, List[str]]): The values to iterate over
+        values (Union[str, List[str]]): The values to iterate over
         cursor_field (Union[InterpolatedString, str]): The name of the cursor field
         config (Config): The user-provided configuration as specified by the source's spec
         request_option (Optional[RequestOption]): The request option to configure the HTTP request
     """
 
-    slice_values: Union[str, List[str]]
+    values: Union[str, List[str]]
     cursor_field: Union[InterpolatedString, str]
     config: Config
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     request_option: Optional[RequestOption] = None
 
-    def __post_init__(self, options: Mapping[str, Any]):
-        if isinstance(self.slice_values, str):
-            self.slice_values = InterpolatedString.create(self.slice_values, options=options).eval(self.config)
-        if isinstance(self.cursor_field, str):
-            self.cursor_field = InterpolatedString(string=self.cursor_field, options=options)
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        if isinstance(self.values, str):
+            self.values = InterpolatedString.create(self.values, parameters=parameters).eval(self.config)
+        self._cursor_field = (
+            InterpolatedString(string=self.cursor_field, parameters=parameters) if isinstance(self.cursor_field, str) else self.cursor_field
+        )
 
-        if self.request_option and self.request_option.inject_into == RequestOptionType.path:
-            raise ValueError("Slice value cannot be injected in the path")
         self._cursor = None
 
-    def update_cursor(self, stream_slice: StreamSlice, last_record: Optional[Record] = None):
-        # This method is called after the records are processed.
-        slice_value = stream_slice.get(self.cursor_field.eval(self.config))
-        if slice_value and slice_value in self.slice_values:
-            self._cursor = slice_value
-        else:
-            raise ValueError(f"Unexpected stream slice: {slice_value}")
-
-    def get_stream_state(self) -> StreamState:
-        return {self.cursor_field.eval(self.config): self._cursor} if self._cursor else {}
-
     def get_request_params(
         self,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
         # Pass the stream_slice from the argument, not the cursor because the cursor is updated after processing the response
@@ -85,19 +71,19 @@
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
         # Pass the stream_slice from the argument, not the cursor because the cursor is updated after processing the response
         return self._get_request_option(RequestOptionType.body_json, stream_slice)
 
-    def stream_slices(self, sync_mode: SyncMode, stream_state: Mapping[str, Any]) -> Iterable[Mapping[str, Any]]:
-        return [{self.cursor_field.eval(self.config): slice_value} for slice_value in self.slice_values]
+    def stream_slices(self) -> Iterable[StreamSlice]:
+        return [StreamSlice(partition={self._cursor_field.eval(self.config): slice_value}, cursor_slice={}) for slice_value in self.values]
 
-    def _get_request_option(self, request_option_type: RequestOptionType, stream_slice: StreamSlice):
+    def _get_request_option(self, request_option_type: RequestOptionType, stream_slice: Optional[StreamSlice]) -> Mapping[str, Any]:
         if self.request_option and self.request_option.inject_into == request_option_type and stream_slice:
-            slice_value = stream_slice.get(self.cursor_field.eval(self.config))
+            slice_value = stream_slice.get(self._cursor_field.eval(self.config))
             if slice_value:
-                return {self.request_option.field_name: slice_value}
+                return {self.request_option.field_name.eval(self.config): slice_value}  # type: ignore # field_name is always casted to InterpolatedString
             else:
                 return {}
         else:
             return {}
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/single_slice.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/partition_routers/single_partition_router.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
 from typing import Any, Iterable, Mapping, Optional
 
-from airbyte_cdk.models import SyncMode
 from airbyte_cdk.sources.declarative.stream_slicers.stream_slicer import StreamSlicer
-from airbyte_cdk.sources.declarative.types import Record, StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import StreamSlice, StreamState
 
 
 @dataclass
-class SingleSlice(StreamSlicer, JsonSchemaMixin):
-    """Stream slicer returning only a single stream slice"""
+class SinglePartitionRouter(StreamSlicer):
+    """Partition router returning only a stream slice"""
 
-    options: InitVar[Mapping[str, Any]]
-
-    def update_cursor(self, stream_slice: StreamSlice, last_record: Optional[Record] = None):
-        pass
-
-    def get_stream_state(self) -> StreamState:
-        return {}
+    parameters: InitVar[Mapping[str, Any]]
 
     def get_request_params(
         self,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
@@ -51,9 +43,9 @@
         self,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
         return {}
 
-    def stream_slices(self, sync_mode: SyncMode, stream_state: Mapping[str, Any]) -> Iterable[StreamSlice]:
-        yield dict()
+    def stream_slices(self) -> Iterable[StreamSlice]:
+        yield StreamSlice(partition={}, cursor_slice={})
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/stream_slicers/substream_slicer.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/partition_routers/substream_partition_router.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
-from typing import Any, Iterable, List, Mapping, Optional
+from typing import TYPE_CHECKING, Any, Iterable, List, Mapping, Optional, Union
 
+import dpath.util
 from airbyte_cdk.models import AirbyteMessage, SyncMode, Type
+from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
 from airbyte_cdk.sources.declarative.requesters.request_option import RequestOption, RequestOptionType
 from airbyte_cdk.sources.declarative.stream_slicers.stream_slicer import StreamSlicer
-from airbyte_cdk.sources.declarative.types import Record, StreamSlice, StreamState
-from airbyte_cdk.sources.streams.core import Stream
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config, Record, StreamSlice, StreamState
+
+if TYPE_CHECKING:
+    from airbyte_cdk.sources.declarative.declarative_stream import DeclarativeStream
 
 
 @dataclass
-class ParentStreamConfig(JsonSchemaMixin):
+class ParentStreamConfig:
     """
     Describes how to create a stream slice from a parent stream
 
     stream: The stream to read records from
     parent_key: The key of the parent stream's records that will be the stream slice key
-    stream_slice_field: The stream slice key
+    partition_field: The partition key
     request_option: How to inject the slice value on an outgoing HTTP request
     """
 
-    stream: Stream
-    parent_key: str
-    stream_slice_field: str
-    options: InitVar[Mapping[str, Any]]
+    stream: "DeclarativeStream"  # Parent streams must be DeclarativeStream because we can't know which part of the stream slice is a partition for regular Stream
+    parent_key: Union[InterpolatedString, str]
+    partition_field: Union[InterpolatedString, str]
+    config: Config
+    parameters: InitVar[Mapping[str, Any]]
     request_option: Optional[RequestOption] = None
 
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        self.parent_key = InterpolatedString.create(self.parent_key, parameters=parameters)
+        self.partition_field = InterpolatedString.create(self.partition_field, parameters=parameters)
+
 
 @dataclass
-class SubstreamSlicer(StreamSlicer, JsonSchemaMixin):
+class SubstreamPartitionRouter(StreamSlicer):
     """
-    Stream slicer that iterates over the parent's stream slices and records and emits slices by interpolating the slice_definition mapping
-    Will populate the state with `parent_stream_slice` and `parent_record` so they can be accessed by other components
+    Partition router that iterates over the parent's stream records and emits slices
+    Will populate the state with `partition_field` and `parent_slice` so they can be accessed by other components
 
     Attributes:
         parent_stream_configs (List[ParentStreamConfig]): parent streams to iterate over and their config
     """
 
     parent_stream_configs: List[ParentStreamConfig]
-    options: InitVar[Mapping[str, Any]]
+    config: Config
+    parameters: InitVar[Mapping[str, Any]]
 
-    def __post_init__(self, options: Mapping[str, Any]):
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
         if not self.parent_stream_configs:
-            raise ValueError("SubstreamSlicer needs at least 1 parent stream")
-        self._cursor = None
-        self._options = options
-
-    def update_cursor(self, stream_slice: StreamSlice, last_record: Optional[Record] = None):
-        # This method is called after the records are processed.
-        cursor = {}
-        for parent_stream_config in self.parent_stream_configs:
-            slice_value = stream_slice.get(parent_stream_config.stream_slice_field)
-            if slice_value:
-                cursor.update({parent_stream_config.stream_slice_field: slice_value})
-        self._cursor = cursor
+            raise ValueError("SubstreamPartitionRouter needs at least 1 parent stream")
+        self._parameters = parameters
 
     def get_request_params(
         self,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
@@ -87,33 +86,30 @@
         return self._get_request_option(RequestOptionType.body_data, stream_slice)
 
     def get_request_body_json(
         self,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
-    ) -> Optional[Mapping]:
+    ) -> Mapping[str, Any]:
         # Pass the stream_slice from the argument, not the cursor because the cursor is updated after processing the response
         return self._get_request_option(RequestOptionType.body_json, stream_slice)
 
-    def _get_request_option(self, option_type: RequestOptionType, stream_slice: StreamSlice):
+    def _get_request_option(self, option_type: RequestOptionType, stream_slice: Optional[StreamSlice]) -> Mapping[str, Any]:
         params = {}
         if stream_slice:
             for parent_config in self.parent_stream_configs:
                 if parent_config.request_option and parent_config.request_option.inject_into == option_type:
-                    key = parent_config.stream_slice_field
+                    key = parent_config.partition_field.eval(self.config)  # type: ignore # partition_field is always casted to an interpolated string
                     value = stream_slice.get(key)
                     if value:
-                        params.update({key: value})
+                        params.update({parent_config.request_option.field_name.eval(config=self.config): value})  # type: ignore # field_name is always casted to an interpolated string
         return params
 
-    def get_stream_state(self) -> StreamState:
-        return self._cursor if self._cursor else {}
-
-    def stream_slices(self, sync_mode: SyncMode, stream_state: StreamState) -> Iterable[StreamSlice]:
+    def stream_slices(self) -> Iterable[StreamSlice]:
         """
         Iterate over each parent stream's record and create a StreamSlice for each record.
 
         For each stream, iterate over its stream_slices.
         For each stream slice, iterate over each record.
         yield a stream slice for each such records.
 
@@ -125,28 +121,38 @@
         - parent_stream_name: string representing the parent stream name
         """
         if not self.parent_stream_configs:
             yield from []
         else:
             for parent_stream_config in self.parent_stream_configs:
                 parent_stream = parent_stream_config.stream
-                parent_field = parent_stream_config.parent_key
-                stream_state_field = parent_stream_config.stream_slice_field
-                for parent_stream_slice in parent_stream.stream_slices(sync_mode=sync_mode, cursor_field=None, stream_state=stream_state):
+                parent_field = parent_stream_config.parent_key.eval(self.config)  # type: ignore # parent_key is always casted to an interpolated string
+                partition_field = parent_stream_config.partition_field.eval(self.config)  # type: ignore # partition_field is always casted to an interpolated string
+                for parent_stream_slice in parent_stream.stream_slices(
+                    sync_mode=SyncMode.full_refresh, cursor_field=None, stream_state=None
+                ):
                     empty_parent_slice = True
-                    parent_slice = parent_stream_slice
+                    parent_partition = parent_stream_slice.partition if parent_stream_slice else {}
 
                     for parent_record in parent_stream.read_records(
                         sync_mode=SyncMode.full_refresh, cursor_field=None, stream_slice=parent_stream_slice, stream_state=None
                     ):
                         # Skip non-records (eg AirbyteLogMessage)
                         if isinstance(parent_record, AirbyteMessage):
                             if parent_record.type == Type.RECORD:
                                 parent_record = parent_record.record.data
                             else:
                                 continue
-                        empty_parent_slice = False
-                        stream_state_value = parent_record.get(parent_field)
-                        yield {stream_state_field: stream_state_value, "parent_slice": parent_slice}
+                        elif isinstance(parent_record, Record):
+                            parent_record = parent_record.data
+                        try:
+                            partition_value = dpath.util.get(parent_record, parent_field)
+                        except KeyError:
+                            pass
+                        else:
+                            empty_parent_slice = False
+                            yield StreamSlice(
+                                partition={partition_field: partition_value, "parent_slice": parent_partition}, cursor_slice={}
+                            )
                     # If the parent slice contains no records,
                     if empty_parent_slice:
                         yield from []
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/transformations/__init__.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/transformations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 # RecordTransformation is depended upon by every class in this module (since it's the abc everything implements). For this reason,
 # the order of imports matters i.e: this file must fully import RecordTransformation before importing anything which depends on RecordTransformation
 # Otherwise there will be a circular dependency (load order will be init.py --> RemoveFields (which tries to import RecordTransformation) -->
 # init.py --> circular dep error, since loading this file causes it to try to import itself down the line.
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/transformations/add_fields.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/transformations/add_fields.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass, field
-from typing import Any, List, Mapping, Optional, Union
+from typing import Any, List, Mapping, Optional, Type, Union
 
 import dpath.util
 from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
 from airbyte_cdk.sources.declarative.transformations import RecordTransformation
-from airbyte_cdk.sources.declarative.types import Config, FieldPointer, Record, StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config, FieldPointer, Record, StreamSlice, StreamState
 
 
 @dataclass(frozen=True)
-class AddedFieldDefinition(JsonSchemaMixin):
+class AddedFieldDefinition:
     """Defines the field to add on a record"""
 
     path: FieldPointer
     value: Union[InterpolatedString, str]
-    options: InitVar[Mapping[str, Any]]
+    value_type: Optional[Type[Any]]
+    parameters: InitVar[Mapping[str, Any]]
 
 
 @dataclass(frozen=True)
-class ParsedAddFieldDefinition(JsonSchemaMixin):
+class ParsedAddFieldDefinition:
     """Defines the field to add on a record"""
 
     path: FieldPointer
     value: InterpolatedString
-    options: InitVar[Mapping[str, Any]]
+    value_type: Optional[Type[Any]]
+    parameters: InitVar[Mapping[str, Any]]
 
 
 @dataclass
-class AddFields(RecordTransformation, JsonSchemaMixin):
+class AddFields(RecordTransformation):
     """
     Transformation which adds field to an output record. The path of the added field can be nested. Adding nested fields will create all
     necessary parent objects (like mkdir -p). Adding fields to an array will extend the array to that index (filling intermediate
     indices with null values). So if you add a field at index 5 to the array ["value"], it will become ["value", null, null, null, null,
     "new_value"].
 
 
@@ -79,43 +80,51 @@
           value: {{ 2 * 2 }}
 
     Attributes:
         fields (List[AddedFieldDefinition]): A list of transformations (path and corresponding value) that will be added to the record
     """
 
     fields: List[AddedFieldDefinition]
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
     _parsed_fields: List[ParsedAddFieldDefinition] = field(init=False, repr=False, default_factory=list)
 
-    def __post_init__(self, options: Mapping[str, Any]):
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
         for add_field in self.fields:
             if len(add_field.path) < 1:
-                raise f"Expected a non-zero-length path for the AddFields transformation {add_field}"
+                raise ValueError(f"Expected a non-zero-length path for the AddFields transformation {add_field}")
 
             if not isinstance(add_field.value, InterpolatedString):
                 if not isinstance(add_field.value, str):
                     raise f"Expected a string value for the AddFields transformation: {add_field}"
                 else:
                     self._parsed_fields.append(
                         ParsedAddFieldDefinition(
-                            add_field.path, InterpolatedString.create(add_field.value, options=options), options=options
+                            add_field.path,
+                            InterpolatedString.create(add_field.value, parameters=parameters),
+                            value_type=add_field.value_type,
+                            parameters=parameters,
                         )
                     )
             else:
-                self._parsed_fields.append(ParsedAddFieldDefinition(add_field.path, add_field.value, options={}))
+                self._parsed_fields.append(
+                    ParsedAddFieldDefinition(add_field.path, add_field.value, value_type=add_field.value_type, parameters={})
+                )
 
     def transform(
         self,
         record: Record,
         config: Optional[Config] = None,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
     ) -> Record:
+        if config is None:
+            config = {}
         kwargs = {"record": record, "stream_state": stream_state, "stream_slice": stream_slice}
         for parsed_field in self._parsed_fields:
-            value = parsed_field.value.eval(config, **kwargs)
+            valid_types = (parsed_field.value_type,) if parsed_field.value_type else None
+            value = parsed_field.value.eval(config, valid_types=valid_types, **kwargs)
             dpath.util.new(record, parsed_field.path, value)
 
         return record
 
-    def __eq__(self, other):
-        return self.__dict__ == other.__dict__
+    def __eq__(self, other: Any) -> bool:
+        return bool(self.__dict__ == other.__dict__)
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/transformations/remove_fields.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/transformations/remove_fields.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from dataclasses import InitVar, dataclass
-from typing import Any, List, Mapping
+from typing import Any, List, Mapping, Optional
 
 import dpath.exceptions
 import dpath.util
+from airbyte_cdk.sources.declarative.interpolation.interpolated_boolean import InterpolatedBoolean
 from airbyte_cdk.sources.declarative.transformations import RecordTransformation
-from airbyte_cdk.sources.declarative.types import FieldPointer, Record
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config, FieldPointer, StreamSlice, StreamState
 
 
 @dataclass
-class RemoveFields(RecordTransformation, JsonSchemaMixin):
+class RemoveFields(RecordTransformation):
     """
     A transformation which removes fields from a record. The fields removed are designated using FieldPointers.
     During transformation, if a field or any of its parents does not exist in the record, no error is thrown.
 
     If an input field pointer references an item in a list (e.g: ["k", 0] in the object {"k": ["a", "b", "c"]}) then
     the object at that index is set to None rather than being not entirely removed from the list. TODO change this behavior.
 
@@ -36,23 +36,37 @@
     ```
 
     Attributes:
         field_pointers (List[FieldPointer]): pointers to the fields that should be removed
     """
 
     field_pointers: List[FieldPointer]
-    options: InitVar[Mapping[str, Any]]
+    parameters: InitVar[Mapping[str, Any]]
+    condition: str = ""
 
-    def transform(self, record: Record, **kwargs) -> Record:
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        self._filter_interpolator = InterpolatedBoolean(condition=self.condition, parameters=parameters)
+
+    def transform(
+        self,
+        record: Mapping[str, Any],
+        config: Optional[Config] = None,
+        stream_state: Optional[StreamState] = None,
+        stream_slice: Optional[StreamSlice] = None,
+    ) -> Mapping[str, Any]:
         """
         :param record: The record to be transformed
         :return: the input record with the requested fields removed
         """
         for pointer in self.field_pointers:
             # the dpath library by default doesn't delete fields from arrays
             try:
-                dpath.util.delete(record, pointer)
+                dpath.util.delete(
+                    record,
+                    pointer,
+                    afilter=(lambda x: self._filter_interpolator.eval(config or {}, property=x)) if self.condition else None,
+                )
             except dpath.exceptions.PathNotFound:
                 # if the (potentially nested) property does not exist, silently skip
                 pass
 
         return record
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/transformations/transformation.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/transformations/transformation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import Optional
+from typing import Any, Mapping, Optional
 
-from airbyte_cdk.sources.declarative.types import Config, Record, StreamSlice, StreamState
-from dataclasses_jsonschema import JsonSchemaMixin
+from airbyte_cdk.sources.types import Config, Record, StreamSlice, StreamState
 
 
 @dataclass
-class RecordTransformation(JsonSchemaMixin):
+class RecordTransformation:
     """
     Implementations of this class define transformations that can be applied to records of a stream.
     """
 
     @abstractmethod
     def transform(
         self,
         record: Record,
         config: Optional[Config] = None,
         stream_state: Optional[StreamState] = None,
         stream_slice: Optional[StreamSlice] = None,
-    ) -> Record:
+    ) -> Mapping[str, Any]:
         """
         Transform a record by adding, deleting, or mutating fields.
 
         :param record: The input record to be transformed
         :param config: The user-provided configuration as specified by the source's spec
         :param stream_state: The stream state
         :param stream_slice: The stream slice
         :return: The transformed record
         """
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         return other.__dict__ == self.__dict__
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/declarative/yaml_declarative_source.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/yaml_declarative_source.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import pkgutil
+from typing import Any
 
 import yaml
 from airbyte_cdk.sources.declarative.manifest_declarative_source import ManifestDeclarativeSource
-from airbyte_cdk.sources.declarative.types import ConnectionDefinition
+from airbyte_cdk.sources.types import ConnectionDefinition
 
 
 class YamlDeclarativeSource(ManifestDeclarativeSource):
     """Declarative source defined by a yaml file"""
 
-    def __init__(self, path_to_yaml, debug: bool = False):
+    def __init__(self, path_to_yaml: str, debug: bool = False) -> None:
         """
         :param path_to_yaml: Path to the yaml file describing the source
         """
         self._path_to_yaml = path_to_yaml
         source_config = self._read_and_parse_yaml_file(path_to_yaml)
         super().__init__(source_config, debug)
 
-    def _read_and_parse_yaml_file(self, path_to_yaml_file) -> ConnectionDefinition:
+    def _read_and_parse_yaml_file(self, path_to_yaml_file: str) -> ConnectionDefinition:
         package = self.__class__.__module__.split(".")[0]
 
         yaml_config = pkgutil.get_data(package, path_to_yaml_file)
-        decoded_yaml = yaml_config.decode()
-        return self._parse(decoded_yaml)
+        if yaml_config:
+            decoded_yaml = yaml_config.decode()
+            return self._parse(decoded_yaml)
+        else:
+            return {}
 
-    def _emit_manifest_debug_message(self, extra_args: dict):
+    def _emit_manifest_debug_message(self, extra_args: dict[str, Any]) -> None:
         extra_args["path_to_yaml"] = self._path_to_yaml
         self.logger.debug("declarative source created from parsed YAML manifest", extra=extra_args)
 
     @staticmethod
     def _parse(connection_definition_str: str) -> ConnectionDefinition:
         """
         Parses a yaml file into a manifest. Component references still exist in the manifest which will be
         resolved during the creating of the DeclarativeSource.
         :param connection_definition_str: yaml string to parse
         :return: The ConnectionDefinition parsed from connection_definition_str
         """
-        return yaml.safe_load(connection_definition_str)
+        return yaml.safe_load(connection_definition_str)  # type: ignore # yaml.safe_load doesn't return a type but know it is a Mapping
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/source.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
-import json
 import logging
 from abc import ABC, abstractmethod
 from collections import defaultdict
-from typing import Any, Generic, Iterable, List, Mapping, MutableMapping, TypeVar, Union
+from typing import Any, Dict, Generic, Iterable, List, Mapping, MutableMapping, Optional, TypeVar, Union
 
 from airbyte_cdk.connector import BaseConnector, DefaultConnectorMixin, TConfig
 from airbyte_cdk.models import AirbyteCatalog, AirbyteMessage, AirbyteStateMessage, AirbyteStateType, ConfiguredAirbyteCatalog
 
 TState = TypeVar("TState")
 TCatalog = TypeVar("TCatalog")
 
@@ -22,15 +21,15 @@
         ...
 
     @abstractmethod
     def read_catalog(self, catalog_path: str) -> TCatalog:
         ...
 
     @abstractmethod
-    def read(self, logger: logging.Logger, config: TConfig, catalog: TCatalog, state: TState = None) -> Iterable[AirbyteMessage]:
+    def read(self, logger: logging.Logger, config: TConfig, catalog: TCatalog, state: Optional[TState] = None) -> Iterable[AirbyteMessage]:
         """
         Returns a generator of the AirbyteMessages generated by reading the source with the given configuration, catalog, and state.
         """
 
     @abstractmethod
     def discover(self, logger: logging.Logger, config: TConfig) -> AirbyteCatalog:
         """
@@ -40,51 +39,53 @@
 
 
 class Source(
     DefaultConnectorMixin,
     BaseSource[Mapping[str, Any], Union[List[AirbyteStateMessage], MutableMapping[str, Any]], ConfiguredAirbyteCatalog],
     ABC,
 ):
-    # can be overridden to change an input state
-    def read_state(self, state_path: str) -> Union[List[AirbyteStateMessage], MutableMapping[str, Any]]:
+    # can be overridden to change an input state.
+    @classmethod
+    def read_state(cls, state_path: str) -> Union[List[AirbyteStateMessage], MutableMapping[str, Any]]:
         """
         Retrieves the input state of a sync by reading from the specified JSON file. Incoming state can be deserialized into either
         a JSON object for legacy state input or as a list of AirbyteStateMessages for the per-stream state format. Regardless of the
         incoming input type, it will always be transformed and output as a list of AirbyteStateMessage(s).
         :param state_path: The filepath to where the stream states are located
         :return: The complete stream state based on the connector's previous sync
         """
         if state_path:
-            state_obj = json.loads(open(state_path, "r").read())
+            state_obj = BaseConnector._read_json_file(state_path)
             if not state_obj:
-                return self._emit_legacy_state_format({})
-            is_per_stream_state = isinstance(state_obj, List)
-            if is_per_stream_state:
+                return cls._emit_legacy_state_format({})
+            if isinstance(state_obj, List):
                 parsed_state_messages = []
-                for state in state_obj:
+                for state in state_obj:  # type: ignore  # `isinstance(state_obj, List)` ensures that this is a list
                     parsed_message = AirbyteStateMessage.parse_obj(state)
                     if not parsed_message.stream and not parsed_message.data and not parsed_message.global_:
                         raise ValueError("AirbyteStateMessage should contain either a stream, global, or state field")
                     parsed_state_messages.append(parsed_message)
                 return parsed_state_messages
             else:
-                return self._emit_legacy_state_format(state_obj)
-        return self._emit_legacy_state_format({})
+                return cls._emit_legacy_state_format(state_obj)  # type: ignore  # assuming it is a dict
+        return cls._emit_legacy_state_format({})
 
-    def _emit_legacy_state_format(self, state_obj) -> Union[List[AirbyteStateMessage], MutableMapping[str, Any]]:
+    @classmethod
+    def _emit_legacy_state_format(cls, state_obj: Dict[str, Any]) -> Union[List[AirbyteStateMessage], MutableMapping[str, Any]]:
         """
         Existing connectors that override read() might not be able to interpret the new state format. We temporarily
         send state in the old format for these connectors, but once all have been upgraded, this method can be removed,
         and we can then emit state in the list format.
         """
         # vars(self.__class__) checks if the current class directly overrides the read() function
-        if "read" in vars(self.__class__):
+        if "read" in vars(cls):
             return defaultdict(dict, state_obj)
         else:
             if state_obj:
                 return [AirbyteStateMessage(type=AirbyteStateType.LEGACY, data=state_obj)]
             else:
                 return []
 
     # can be overridden to change an input catalog
-    def read_catalog(self, catalog_path: str) -> ConfiguredAirbyteCatalog:
-        return ConfiguredAirbyteCatalog.parse_obj(self.read_config(catalog_path))
+    @classmethod
+    def read_catalog(cls, catalog_path: str) -> ConfiguredAirbyteCatalog:
+        return ConfiguredAirbyteCatalog.parse_obj(cls._read_json_file(catalog_path))
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/auth/core.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/auth/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 from abc import ABC, abstractmethod
 from typing import Any, Mapping
 
 from deprecated import deprecated
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/auth/token.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/auth/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 import base64
 from itertools import cycle
 from typing import Any, List, Mapping
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/http.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/declarative/requesters/http_requester.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,331 +1,474 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
-
 import logging
 import os
-from abc import ABC, abstractmethod
-from contextlib import suppress
-from typing import Any, Callable, Iterable, List, Mapping, MutableMapping, Optional, Tuple, Union
+import urllib
+from dataclasses import InitVar, dataclass
+from functools import lru_cache
+from pathlib import Path
+from typing import Any, Callable, Mapping, MutableMapping, Optional, Union
 from urllib.parse import urljoin
 
 import requests
 import requests_cache
-from airbyte_cdk.models import SyncMode
-from airbyte_cdk.sources.streams.core import Stream, StreamData
+from airbyte_cdk.models import Level
+from airbyte_cdk.sources.declarative.auth.declarative_authenticator import DeclarativeAuthenticator, NoAuth
+from airbyte_cdk.sources.declarative.decoders.json_decoder import JsonDecoder
+from airbyte_cdk.sources.declarative.exceptions import ReadException
+from airbyte_cdk.sources.declarative.interpolation.interpolated_string import InterpolatedString
+from airbyte_cdk.sources.declarative.requesters.error_handlers.error_handler import ErrorHandler
+from airbyte_cdk.sources.declarative.requesters.error_handlers.response_action import ResponseAction
+from airbyte_cdk.sources.declarative.requesters.error_handlers.response_status import ResponseStatus
+from airbyte_cdk.sources.declarative.requesters.request_options.interpolated_request_options_provider import (
+    InterpolatedRequestOptionsProvider,
+)
+from airbyte_cdk.sources.declarative.requesters.requester import HttpMethod, Requester
+from airbyte_cdk.sources.http_config import MAX_CONNECTION_POOL_SIZE
+from airbyte_cdk.sources.message import MessageRepository, NoopMessageRepository
+from airbyte_cdk.sources.streams.http.exceptions import DefaultBackoffException, RequestBodyException, UserDefinedBackoffException
+from airbyte_cdk.sources.streams.http.http import BODY_REQUEST_METHODS
+from airbyte_cdk.sources.streams.http.rate_limiting import default_backoff_handler, user_defined_backoff_handler
+from airbyte_cdk.sources.types import Config, StreamSlice, StreamState
+from airbyte_cdk.utils.constants import ENV_REQUEST_CACHE_PATH
+from airbyte_cdk.utils.mapping_helpers import combine_mappings
 from requests.auth import AuthBase
-from requests_cache.session import CachedSession
-
-from .auth.core import HttpAuthenticator, NoAuth
-from .exceptions import DefaultBackoffException, RequestBodyException, UserDefinedBackoffException
-from .rate_limiting import default_backoff_handler, user_defined_backoff_handler
-
-# list of all possible HTTP methods which can be used for sending of request bodies
-BODY_REQUEST_METHODS = ("GET", "POST", "PUT", "PATCH")
 
 
-class HttpStream(Stream, ABC):
-    """
-    Base abstract class for an Airbyte Stream using the HTTP protocol. Basic building block for users building an Airbyte source for a HTTP API.
+@dataclass
+class HttpRequester(Requester):
     """
+    Default implementation of a Requester
 
-    source_defined_cursor = True  # Most HTTP streams use a source defined cursor (i.e: the user can't configure it like on a SQL table)
-    page_size: Optional[int] = None  # Use this variable to define page size for API http requests with pagination support
+    Attributes:
+        name (str): Name of the stream. Only used for request/response caching
+        url_base (Union[InterpolatedString, str]): Base url to send requests to
+        path (Union[InterpolatedString, str]): Path to send requests to
+        http_method (Union[str, HttpMethod]): HTTP method to use when sending requests
+        request_options_provider (Optional[InterpolatedRequestOptionsProvider]): request option provider defining the options to set on outgoing requests
+        authenticator (DeclarativeAuthenticator): Authenticator defining how to authenticate to the source
+        error_handler (Optional[ErrorHandler]): Error handler defining how to detect and handle errors
+        config (Config): The user-provided configuration as specified by the source's spec
+        use_cache (bool): Indicates that data should be cached for this stream
+    """
 
-    # TODO: remove legacy HttpAuthenticator authenticator references
-    def __init__(self, authenticator: Union[AuthBase, HttpAuthenticator] = None):
-        if self.use_cache:
-            self._session = self.request_cache()
+    name: str
+    url_base: Union[InterpolatedString, str]
+    path: Union[InterpolatedString, str]
+    config: Config
+    parameters: InitVar[Mapping[str, Any]]
+    authenticator: Optional[DeclarativeAuthenticator] = None
+    http_method: Union[str, HttpMethod] = HttpMethod.GET
+    request_options_provider: Optional[InterpolatedRequestOptionsProvider] = None
+    error_handler: Optional[ErrorHandler] = None
+    disable_retries: bool = False
+    message_repository: MessageRepository = NoopMessageRepository()
+    use_cache: bool = False
+
+    _DEFAULT_MAX_RETRY = 5
+    _DEFAULT_RETRY_FACTOR = 5
+    _DEFAULT_MAX_TIME = 60 * 10
+
+    def __post_init__(self, parameters: Mapping[str, Any]) -> None:
+        self._url_base = InterpolatedString.create(self.url_base, parameters=parameters)
+        self._path = InterpolatedString.create(self.path, parameters=parameters)
+        if self.request_options_provider is None:
+            self._request_options_provider = InterpolatedRequestOptionsProvider(config=self.config, parameters=parameters)
+        elif isinstance(self.request_options_provider, dict):
+            self._request_options_provider = InterpolatedRequestOptionsProvider(config=self.config, **self.request_options_provider)
         else:
-            self._session = requests.Session()
+            self._request_options_provider = self.request_options_provider
+        self._authenticator = self.authenticator or NoAuth(parameters=parameters)
+        self._http_method = HttpMethod[self.http_method] if isinstance(self.http_method, str) else self.http_method
+        self.error_handler = self.error_handler
+        self._parameters = parameters
+        self.decoder = JsonDecoder(parameters={})
+        self._session = self.request_cache()
+        self._session.mount(
+            "https://", requests.adapters.HTTPAdapter(pool_connections=MAX_CONNECTION_POOL_SIZE, pool_maxsize=MAX_CONNECTION_POOL_SIZE)
+        )
+
+        if isinstance(self._authenticator, AuthBase):
+            self._session.auth = self._authenticator
 
-        self._authenticator: HttpAuthenticator = NoAuth()
-        if isinstance(authenticator, AuthBase):
-            self._session.auth = authenticator
-        elif authenticator:
-            self._authenticator = authenticator
+    # We are using an LRU cache in should_retry() method which requires all incoming arguments (including self) to be hashable.
+    # Dataclasses by default are not hashable, so we need to define __hash__(). Alternatively, we can set @dataclass(frozen=True),
+    # but this has a cascading effect where all dataclass fields must also be set to frozen.
+    def __hash__(self) -> int:
+        return hash(tuple(self.__dict__))
 
     @property
-    def cache_filename(self):
+    def cache_filename(self) -> str:
         """
-        Override if needed. Return the name of cache file
+        Note that if the environment variable REQUEST_CACHE_PATH is not set, the cache will be in-memory only.
         """
         return f"{self.name}.sqlite"
 
-    @property
-    def use_cache(self):
+    def request_cache(self) -> requests.Session:
+        if self.use_cache:
+            cache_dir = os.getenv(ENV_REQUEST_CACHE_PATH)
+            # Use in-memory cache if cache_dir is not set
+            # This is a non-obvious interface, but it ensures we don't write sql files when running unit tests
+            if cache_dir:
+                sqlite_path = str(Path(cache_dir) / self.cache_filename)
+            else:
+                sqlite_path = "file::memory:?cache=shared"
+            return requests_cache.CachedSession(sqlite_path, backend="sqlite")  # type: ignore # there are no typeshed stubs for requests_cache
+        else:
+            return requests.Session()
+
+    def clear_cache(self) -> None:
         """
-        Override if needed. If True, all records will be cached.
+        Clear cached requests for current session, can be called any time
         """
-        return False
+        if isinstance(self._session, requests_cache.CachedSession):
+            self._session.cache.clear()  # type: ignore # cache.clear is not typed
 
-    def request_cache(self) -> CachedSession:
-        self.clear_cache()
-        return requests_cache.CachedSession(self.cache_filename)
+    def get_authenticator(self) -> DeclarativeAuthenticator:
+        return self._authenticator
 
-    def clear_cache(self):
-        """
-        remove cache file only once
-        """
-        STREAM_CACHE_FILES = globals().setdefault("STREAM_CACHE_FILES", set())
-        if self.cache_filename not in STREAM_CACHE_FILES:
-            with suppress(FileNotFoundError):
-                os.remove(self.cache_filename)
-            STREAM_CACHE_FILES.add(self.cache_filename)
+    def get_url_base(self) -> str:
+        return os.path.join(self._url_base.eval(self.config), "")
 
-    @property
-    @abstractmethod
-    def url_base(self) -> str:
-        """
-        :return: URL base for the  API endpoint e.g: if you wanted to hit https://myapi.com/v1/some_entity then this should return "https://myapi.com/v1/"
-        """
+    def get_path(
+        self, *, stream_state: Optional[StreamState], stream_slice: Optional[StreamSlice], next_page_token: Optional[Mapping[str, Any]]
+    ) -> str:
+        kwargs = {"stream_state": stream_state, "stream_slice": stream_slice, "next_page_token": next_page_token}
+        path = str(self._path.eval(self.config, **kwargs))
+        return path.lstrip("/")
 
-    @property
-    def http_method(self) -> str:
-        """
-        Override if needed. See get_request_data/get_request_json if using POST/PUT/PATCH.
-        """
-        return "GET"
+    def get_method(self) -> HttpMethod:
+        return self._http_method
 
-    @property
-    def raise_on_http_errors(self) -> bool:
-        """
-        Override if needed. If set to False, allows opting-out of raising HTTP code exception.
-        """
-        return True
+    def interpret_response_status(self, response: requests.Response) -> ResponseStatus:
+        if self.error_handler is None:
+            raise ValueError("Cannot interpret response status without an error handler")
+
+        # Change CachedRequest to PreparedRequest for response
+        request = response.request
+        if isinstance(request, requests_cache.CachedRequest):
+            response.request = request.prepare()
+
+        return self.error_handler.interpret_response(response)
+
+    def get_request_params(
+        self,
+        *,
+        stream_state: Optional[StreamState] = None,
+        stream_slice: Optional[StreamSlice] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
+    ) -> MutableMapping[str, Any]:
+        return self._request_options_provider.get_request_params(
+            stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token
+        )
+
+    def get_request_headers(
+        self,
+        *,
+        stream_state: Optional[StreamState] = None,
+        stream_slice: Optional[StreamSlice] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
+    ) -> Mapping[str, Any]:
+        return self._request_options_provider.get_request_headers(
+            stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token
+        )
+
+    # fixing request options provider types has a lot of dependencies
+    def get_request_body_data(  # type: ignore
+        self,
+        *,
+        stream_state: Optional[StreamState] = None,
+        stream_slice: Optional[StreamSlice] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
+    ) -> Union[Mapping[str, Any], str]:
+        return (
+            self._request_options_provider.get_request_body_data(
+                stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token
+            )
+            or {}
+        )
+
+    # fixing request options provider types has a lot of dependencies
+    def get_request_body_json(  # type: ignore
+        self,
+        *,
+        stream_state: Optional[StreamState] = None,
+        stream_slice: Optional[StreamSlice] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
+    ) -> Optional[Mapping[str, Any]]:
+        return self._request_options_provider.get_request_body_json(
+            stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token
+        )
 
     @property
     def max_retries(self) -> Union[int, None]:
-        """
-        Override if needed. Specifies maximum amount of retries for backoff policy. Return None for no limit.
-        """
-        return 5
+        if self.disable_retries:
+            return 0
+        if self.error_handler is None:
+            return self._DEFAULT_MAX_RETRY
+        return self.error_handler.max_retries
 
     @property
-    def retry_factor(self) -> float:
+    def max_time(self) -> Union[int, None]:
         """
-        Override if needed. Specifies factor for backoff policy.
+        Override if needed. Specifies maximum total waiting time (in seconds) for backoff policy. Return None for no limit.
         """
-        return 5
+        if self.error_handler is None:
+            return self._DEFAULT_MAX_TIME
+        return self.error_handler.max_time
 
     @property
-    def authenticator(self) -> HttpAuthenticator:
-        return self._authenticator
+    def logger(self) -> logging.Logger:
+        return logging.getLogger(f"airbyte.HttpRequester.{self.name}")
 
-    @abstractmethod
-    def next_page_token(self, response: requests.Response) -> Optional[Mapping[str, Any]]:
+    def _should_retry(self, response: requests.Response) -> bool:
         """
-        Override this method to define a pagination strategy.
+        Specifies conditions for backoff based on the response from the server.
 
-        The value returned from this method is passed to most other methods in this class. Use it to form a request e.g: set headers or query params.
+        By default, back off on the following HTTP response statuses:
+         - 429 (Too Many Requests) indicating rate limiting
+         - 500s to handle transient server errors
 
-        :return: The token for the next page from the input response object. Returning None means there are no more pages to read in this response.
+        Unexpected but transient exceptions (connection timeout, DNS resolution failed, etc..) are retried by default.
         """
+        if self.error_handler is None:
+            return response.status_code == 429 or 500 <= response.status_code < 600
 
-    @abstractmethod
-    def path(
-        self,
-        *,
-        stream_state: Mapping[str, Any] = None,
-        stream_slice: Mapping[str, Any] = None,
-        next_page_token: Mapping[str, Any] = None,
-    ) -> str:
-        """
-        Returns the URL path for the API endpoint e.g: if you wanted to hit https://myapi.com/v1/some_entity then this should return "some_entity"
-        """
+        if self.use_cache:
+            interpret_response_status = self.interpret_response_status
+        else:
+            # Use a tiny cache to limit the memory footprint. It doesn't have to be large because we mostly
+            # only care about the status of the last response received
+            # Cache the result because the HttpStream first checks if we should retry before looking at the backoff time
+            interpret_response_status = lru_cache(maxsize=10)(self.interpret_response_status)
 
-    def request_params(
-        self,
-        stream_state: Mapping[str, Any],
-        stream_slice: Mapping[str, Any] = None,
-        next_page_token: Mapping[str, Any] = None,
-    ) -> MutableMapping[str, Any]:
-        """
-        Override this method to define the query parameters that should be set on an outgoing HTTP request given the inputs.
+        return bool(interpret_response_status(response).action == ResponseAction.RETRY)
 
-        E.g: you might want to define query parameters for paging if next_page_token is not None.
+    def _backoff_time(self, response: requests.Response) -> Optional[float]:
         """
-        return {}
+        Specifies backoff time.
 
-    def request_headers(
-        self, stream_state: Mapping[str, Any], stream_slice: Mapping[str, Any] = None, next_page_token: Mapping[str, Any] = None
-    ) -> Mapping[str, Any]:
-        """
-        Override to return any non-auth headers. Authentication headers will overwrite any overlapping headers returned from this method.
-        """
-        return {}
+         This method is called only if should_backoff() returns True for the input request.
 
-    def request_body_data(
-        self,
-        stream_state: Mapping[str, Any],
-        stream_slice: Mapping[str, Any] = None,
-        next_page_token: Mapping[str, Any] = None,
-    ) -> Optional[Union[Mapping, str]]:
+         :param response:
+         :return how long to backoff in seconds. The return value may be a floating point number for subsecond precision. Returning None defers backoff
+         to the default backoff behavior (e.g using an exponential algorithm).
         """
-        Override when creating POST/PUT/PATCH requests to populate the body of the request with a non-JSON payload.
-
-        If returns a ready text that it will be sent as is.
-        If returns a dict that it will be converted to a urlencoded form.
-        E.g. {"key1": "value1", "key2": "value2"} => "key1=value1&key2=value2"
+        if self.error_handler is None:
+            return None
+        should_retry = self.interpret_response_status(response)
+        if should_retry.action != ResponseAction.RETRY:
+            raise ValueError(f"backoff_time can only be applied on retriable response action. Got {should_retry.action}")
+        assert should_retry.action == ResponseAction.RETRY
+        return should_retry.retry_in
 
-        At the same time only one of the 'request_body_data' and 'request_body_json' functions can be overridden.
+    def _error_message(self, response: requests.Response) -> str:
         """
-        return None
+        Constructs an error message which can incorporate the HTTP response received from the partner API.
 
-    def request_body_json(
-        self,
-        stream_state: Mapping[str, Any],
-        stream_slice: Mapping[str, Any] = None,
-        next_page_token: Mapping[str, Any] = None,
-    ) -> Optional[Mapping]:
+        :param response: The incoming HTTP response from the partner API
+        :return The error message string to be emitted
         """
-        Override when creating POST/PUT/PATCH requests to populate the body of the request with a JSON payload.
+        return self.interpret_response_status(response).error_message
 
-        At the same time only one of the 'request_body_data' and 'request_body_json' functions can be overridden.
-        """
-        return None
+    def _get_request_options(
+        self,
+        stream_state: Optional[StreamState],
+        stream_slice: Optional[StreamSlice],
+        next_page_token: Optional[Mapping[str, Any]],
+        requester_method: Callable[..., Optional[Union[Mapping[str, Any], str]]],
+        auth_options_method: Callable[..., Optional[Union[Mapping[str, Any], str]]],
+        extra_options: Optional[Union[Mapping[str, Any], str]] = None,
+    ) -> Union[Mapping[str, Any], str]:
+        """
+        Get the request_option from the requester, the authenticator and extra_options passed in.
+        Raise a ValueError if there's a key collision
+        Returned merged mapping otherwise
+        """
+        return combine_mappings(
+            [
+                requester_method(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token),
+                auth_options_method(),
+                extra_options,
+            ]
+        )
 
-    def request_kwargs(
+    def _request_headers(
         self,
-        stream_state: Mapping[str, Any],
-        stream_slice: Mapping[str, Any] = None,
-        next_page_token: Mapping[str, Any] = None,
+        stream_state: Optional[StreamState] = None,
+        stream_slice: Optional[StreamSlice] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
+        extra_headers: Optional[Mapping[str, Any]] = None,
     ) -> Mapping[str, Any]:
         """
-        Override to return a mapping of keyword arguments to be used when creating the HTTP request.
-        Any option listed in https://docs.python-requests.org/en/latest/api/#requests.adapters.BaseAdapter.send for can be returned from
-        this method. Note that these options do not conflict with request-level options such as headers, request params, etc..
+        Specifies request headers.
+        Authentication headers will overwrite any overlapping headers returned from this method.
         """
-        return {}
+        headers = self._get_request_options(
+            stream_state,
+            stream_slice,
+            next_page_token,
+            self.get_request_headers,
+            self.get_authenticator().get_auth_header,
+            extra_headers,
+        )
+        if isinstance(headers, str):
+            raise ValueError("Request headers cannot be a string")
+        return {str(k): str(v) for k, v in headers.items()}
 
-    @abstractmethod
-    def parse_response(
+    def _request_params(
         self,
-        response: requests.Response,
-        *,
-        stream_state: Mapping[str, Any],
-        stream_slice: Mapping[str, Any] = None,
-        next_page_token: Mapping[str, Any] = None,
-    ) -> Iterable[Mapping]:
-        """
-        Parses the raw response object into a list of records.
-        By default, this returns an iterable containing the input. Override to parse differently.
-        :param response:
-        :param stream_state:
-        :param stream_slice:
-        :param next_page_token:
-        :return: An iterable containing the parsed response
+        stream_state: Optional[StreamState],
+        stream_slice: Optional[StreamSlice],
+        next_page_token: Optional[Mapping[str, Any]],
+        extra_params: Optional[Mapping[str, Any]] = None,
+    ) -> Mapping[str, Any]:
         """
+        Specifies the query parameters that should be set on an outgoing HTTP request given the inputs.
 
-    # TODO move all the retry logic to a functor/decorator which is input as an init parameter
-    def should_retry(self, response: requests.Response) -> bool:
+        E.g: you might want to define query parameters for paging if next_page_token is not None.
         """
-        Override to set different conditions for backoff based on the response from the server.
+        options = self._get_request_options(
+            stream_state, stream_slice, next_page_token, self.get_request_params, self.get_authenticator().get_request_params, extra_params
+        )
+        if isinstance(options, str):
+            raise ValueError("Request params cannot be a string")
 
-        By default, back off on the following HTTP response statuses:
-         - 429 (Too Many Requests) indicating rate limiting
-         - 500s to handle transient server errors
+        for k, v in options.items():
+            if isinstance(v, (dict,)):
+                raise ValueError(f"Invalid value for `{k}` parameter. The values of request params cannot be an object.")
 
-        Unexpected but transient exceptions (connection timeout, DNS resolution failed, etc..) are retried by default.
-        """
-        return response.status_code == 429 or 500 <= response.status_code < 600
+        return options
 
-    def backoff_time(self, response: requests.Response) -> Optional[float]:
+    def _request_body_data(
+        self,
+        stream_state: Optional[StreamState],
+        stream_slice: Optional[StreamSlice],
+        next_page_token: Optional[Mapping[str, Any]],
+        extra_body_data: Optional[Union[Mapping[str, Any], str]] = None,
+    ) -> Optional[Union[Mapping[str, Any], str]]:
         """
-        Override this method to dynamically determine backoff time e.g: by reading the X-Retry-After header.
+        Specifies how to populate the body of the request with a non-JSON payload.
 
-        This method is called only if should_backoff() returns True for the input request.
+        If returns a ready text that it will be sent as is.
+        If returns a dict that it will be converted to a urlencoded form.
+        E.g. {"key1": "value1", "key2": "value2"} => "key1=value1&key2=value2"
 
-        :param response:
-        :return how long to backoff in seconds. The return value may be a floating point number for subsecond precision. Returning None defers backoff
-        to the default backoff behavior (e.g using an exponential algorithm).
+        At the same time only one of the 'request_body_data' and 'request_body_json' functions can be overridden.
         """
-        return None
+        # Warning: use self.state instead of the stream_state passed as argument!
+        return self._get_request_options(
+            stream_state,
+            stream_slice,
+            next_page_token,
+            self.get_request_body_data,
+            self.get_authenticator().get_request_body_data,
+            extra_body_data,
+        )
 
-    def error_message(self, response: requests.Response) -> str:
+    def _request_body_json(
+        self,
+        stream_state: Optional[StreamState],
+        stream_slice: Optional[StreamSlice],
+        next_page_token: Optional[Mapping[str, Any]],
+        extra_body_json: Optional[Mapping[str, Any]] = None,
+    ) -> Optional[Mapping[str, Any]]:
         """
-        Override this method to specify a custom error message which can incorporate the HTTP response received
+        Specifies how to populate the body of the request with a JSON payload.
 
-        :param response: The incoming HTTP response from the partner API
+        At the same time only one of the 'request_body_data' and 'request_body_json' functions can be overridden.
+        """
+        # Warning: use self.state instead of the stream_state passed as argument!
+        options = self._get_request_options(
+            stream_state,
+            stream_slice,
+            next_page_token,
+            self.get_request_body_json,
+            self.get_authenticator().get_request_body_json,
+            extra_body_json,
+        )
+        if isinstance(options, str):
+            raise ValueError("Request body json cannot be a string")
+        return options
+
+    def deduplicate_query_params(self, url: str, params: Optional[Mapping[str, Any]]) -> Mapping[str, Any]:
+        """
+        Remove query parameters from params mapping if they are already encoded in the URL.
+        :param url: URL with
+        :param params:
         :return:
         """
-        return ""
+        if params is None:
+            params = {}
+        query_string = urllib.parse.urlparse(url).query
+        query_dict = {k: v[0] for k, v in urllib.parse.parse_qs(query_string).items()}
+
+        duplicate_keys_with_same_value = {k for k in query_dict.keys() if str(params.get(k)) == str(query_dict[k])}
+        return {k: v for k, v in params.items() if k not in duplicate_keys_with_same_value}
+
+    @classmethod
+    def _join_url(cls, url_base: str, path: str) -> str:
+        return urljoin(url_base, path)
 
     def _create_prepared_request(
         self,
         path: str,
-        headers: Mapping = None,
-        params: Mapping = None,
+        headers: Optional[Mapping[str, str]] = None,
+        params: Optional[Mapping[str, Any]] = None,
         json: Any = None,
         data: Any = None,
     ) -> requests.PreparedRequest:
-        args = {"method": self.http_method, "url": urljoin(self.url_base, path), "headers": headers, "params": params}
-        if self.http_method.upper() in BODY_REQUEST_METHODS:
+        url = urljoin(self.get_url_base(), path)
+        http_method = str(self._http_method.value)
+        query_params = self.deduplicate_query_params(url, params)
+        args = {"method": http_method, "url": url, "headers": headers, "params": query_params}
+        if http_method.upper() in BODY_REQUEST_METHODS:
             if json and data:
                 raise RequestBodyException(
                     "At the same time only one of the 'request_body_data' and 'request_body_json' functions can return data"
                 )
             elif json:
                 args["json"] = json
             elif data:
                 args["data"] = data
 
         return self._session.prepare_request(requests.Request(**args))
 
-    def _send(self, request: requests.PreparedRequest, request_kwargs: Mapping[str, Any]) -> requests.Response:
-        """
-        Wraps sending the request in rate limit and error handlers.
-        Please note that error handling for HTTP status codes will be ignored if raise_on_http_errors is set to False
-
-        This method handles two types of exceptions:
-            1. Expected transient exceptions e.g: 429 status code.
-            2. Unexpected transient exceptions e.g: timeout.
-
-        To trigger a backoff, we raise an exception that is handled by the backoff decorator. If an exception is not handled by the decorator will
-        fail the sync.
-
-        For expected transient exceptions, backoff time is determined by the type of exception raised:
-            1. CustomBackoffException uses the user-provided backoff value
-            2. DefaultBackoffException falls back on the decorator's default behavior e.g: exponential backoff
-
-        Unexpected transient exceptions use the default backoff parameters.
-        Unexpected persistent exceptions are not handled and will cause the sync to fail.
-        """
-        self.logger.debug(
-            "Making outbound API request", extra={"headers": request.headers, "url": request.url, "request_body": request.body}
+    def send_request(
+        self,
+        stream_state: Optional[StreamState] = None,
+        stream_slice: Optional[StreamSlice] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
+        path: Optional[str] = None,
+        request_headers: Optional[Mapping[str, Any]] = None,
+        request_params: Optional[Mapping[str, Any]] = None,
+        request_body_data: Optional[Union[Mapping[str, Any], str]] = None,
+        request_body_json: Optional[Mapping[str, Any]] = None,
+        log_formatter: Optional[Callable[[requests.Response], Any]] = None,
+    ) -> Optional[requests.Response]:
+        request = self._create_prepared_request(
+            path=path
+            if path is not None
+            else self.get_path(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token),
+            headers=self._request_headers(stream_state, stream_slice, next_page_token, request_headers),
+            params=self._request_params(stream_state, stream_slice, next_page_token, request_params),
+            json=self._request_body_json(stream_state, stream_slice, next_page_token, request_body_json),
+            data=self._request_body_data(stream_state, stream_slice, next_page_token, request_body_data),
         )
-        response: requests.Response = self._session.send(request, **request_kwargs)
 
-        # Evaluation of response.text can be heavy, for example, if streaming a large response
-        # Do it only in debug mode
-        if self.logger.isEnabledFor(logging.DEBUG):
-            self.logger.debug(
-                "Receiving response", extra={"headers": response.headers, "status": response.status_code, "body": response.text}
-            )
-        if self.should_retry(response):
-            custom_backoff_time = self.backoff_time(response)
-            error_message = self.error_message(response)
-            if custom_backoff_time:
-                raise UserDefinedBackoffException(
-                    backoff=custom_backoff_time, request=request, response=response, error_message=error_message
-                )
-            else:
-                raise DefaultBackoffException(request=request, response=response, error_message=error_message)
-        elif self.raise_on_http_errors:
-            # Raise any HTTP exceptions that happened in case there were unexpected ones
-            try:
-                response.raise_for_status()
-            except requests.HTTPError as exc:
-                self.logger.error(response.text)
-                raise exc
-        return response
+        response = self._send_with_retry(request, log_formatter=log_formatter)
+        return self._validate_response(response)
 
-    def _send_request(self, request: requests.PreparedRequest, request_kwargs: Mapping[str, Any]) -> requests.Response:
+    def _send_with_retry(
+        self,
+        request: requests.PreparedRequest,
+        log_formatter: Optional[Callable[[requests.Response], Any]] = None,
+    ) -> requests.Response:
         """
         Creates backoff wrappers which are responsible for retry logic
         """
 
         """
         Backoff package has max_tries parameter that means total number of
         tries before giving up, so if this number is 0 no calls expected to be done.
@@ -342,137 +485,126 @@
         This implies that if max_tries is explicitly set to None there is no
         limit to retry attempts, otherwise it is limited number of tries. But
         this is not true for current version of backoff packages (1.8.0). Setting
         max_tries to 0 or negative number would result in endless retry attempts.
         Add this condition to avoid an endless loop if it hasn't been set
         explicitly (i.e. max_retries is not None).
         """
+        max_time = self.max_time
+        """
+        According to backoff max_time docstring:
+            max_time: The maximum total amount of time to try for before
+                giving up. Once expired, the exception will be allowed to
+                escape. If a callable is passed, it will be
+                evaluated at runtime and its return value used.
+        """
         if max_tries is not None:
             max_tries = max(0, max_tries) + 1
 
-        user_backoff_handler = user_defined_backoff_handler(max_tries=max_tries)(self._send)
-        backoff_handler = default_backoff_handler(max_tries=max_tries, factor=self.retry_factor)
-        return backoff_handler(user_backoff_handler)(request, request_kwargs)
+        user_backoff_handler = user_defined_backoff_handler(max_tries=max_tries, max_time=max_time)(self._send)  # type: ignore # we don't pass in kwargs to the backoff handler
+        backoff_handler = default_backoff_handler(max_tries=max_tries, max_time=max_time, factor=self._DEFAULT_RETRY_FACTOR)
+        # backoff handlers wrap _send, so it will always return a response
+        return backoff_handler(user_backoff_handler)(request, log_formatter=log_formatter)  # type: ignore
+
+    def _send(
+        self,
+        request: requests.PreparedRequest,
+        log_formatter: Optional[Callable[[requests.Response], Any]] = None,
+    ) -> requests.Response:
+        """
+        Wraps sending the request in rate limit and error handlers.
+        Please note that error handling for HTTP status codes will be ignored if raise_on_http_errors is set to False
+
+        This method handles two types of exceptions:
+            1. Expected transient exceptions e.g: 429 status code.
+            2. Unexpected transient exceptions e.g: timeout.
+
+        To trigger a backoff, we raise an exception that is handled by the backoff decorator. If an exception is not handled by the decorator will
+        fail the sync.
+
+        For expected transient exceptions, backoff time is determined by the type of exception raised:
+            1. CustomBackoffException uses the user-provided backoff value
+            2. DefaultBackoffException falls back on the decorator's default behavior e.g: exponential backoff
+
+        Unexpected transient exceptions use the default backoff parameters.
+        Unexpected persistent exceptions are not handled and will cause the sync to fail.
+        """
+        self.logger.debug(
+            "Making outbound API request", extra={"headers": request.headers, "url": request.url, "request_body": request.body}
+        )
+        response: requests.Response = self._session.send(request)
+        self.logger.debug("Receiving response", extra={"headers": response.headers, "status": response.status_code, "body": response.text})
+        if log_formatter:
+            formatter = log_formatter
+            self.message_repository.log_message(
+                Level.DEBUG,
+                lambda: formatter(response),
+            )
+        if self._should_retry(response):
+            custom_backoff_time = self._backoff_time(response)
+            if custom_backoff_time:
+                raise UserDefinedBackoffException(backoff=custom_backoff_time, request=request, response=response)
+            else:
+                raise DefaultBackoffException(request=request, response=response)
+        return response
+
+    def _validate_response(
+        self,
+        response: requests.Response,
+    ) -> Optional[requests.Response]:
+        # if fail -> raise exception
+        # if ignore -> ignore response and return None
+        # else -> delegate to caller
+        if self.error_handler is None:
+            return response
+
+        response_status = self.interpret_response_status(response)
+        if response_status.action == ResponseAction.FAIL:
+            error_message = (
+                response_status.error_message
+                or f"Request to {response.request.url} failed with status code {response.status_code} and error message {HttpRequester.parse_response_error_message(response)}"
+            )
+            raise ReadException(error_message)
+        elif response_status.action == ResponseAction.IGNORE:
+            self.logger.info(
+                f"Ignoring response for failed request with error message {HttpRequester.parse_response_error_message(response)}"
+            )
+
+        return response
 
     @classmethod
     def parse_response_error_message(cls, response: requests.Response) -> Optional[str]:
         """
         Parses the raw response object from a failed request into a user-friendly error message.
         By default, this method tries to grab the error message from JSON responses by following common API patterns. Override to parse differently.
 
         :param response:
         :return: A user-friendly message that indicates the cause of the error
         """
 
         # default logic to grab error from common fields
-        def _try_get_error(value):
+        def _try_get_error(value: Any) -> Any:
             if isinstance(value, str):
                 return value
             elif isinstance(value, list):
-                return ", ".join(_try_get_error(v) for v in value)
+                error_list = [_try_get_error(v) for v in value]
+                return ", ".join(v for v in error_list if v is not None)
             elif isinstance(value, dict):
                 new_value = (
                     value.get("message")
                     or value.get("messages")
                     or value.get("error")
                     or value.get("errors")
                     or value.get("failures")
                     or value.get("failure")
+                    or value.get("details")
+                    or value.get("detail")
                 )
                 return _try_get_error(new_value)
             return None
 
         try:
             body = response.json()
-            return _try_get_error(body)
+            error = _try_get_error(body)
+            return str(error) if error else None
         except requests.exceptions.JSONDecodeError:
             return None
-
-    def get_error_display_message(self, exception: BaseException) -> Optional[str]:
-        """
-        Retrieves the user-friendly display message that corresponds to an exception.
-        This will be called when encountering an exception while reading records from the stream, and used to build the AirbyteTraceMessage.
-
-        The default implementation of this method only handles HTTPErrors by passing the response to self.parse_response_error_message().
-        The method should be overriden as needed to handle any additional exception types.
-
-        :param exception: The exception that was raised
-        :return: A user-friendly message that indicates the cause of the error
-        """
-        if isinstance(exception, requests.HTTPError):
-            return self.parse_response_error_message(exception.response)
-        return None
-
-    def read_records(
-        self,
-        sync_mode: SyncMode,
-        cursor_field: List[str] = None,
-        stream_slice: Mapping[str, Any] = None,
-        stream_state: Mapping[str, Any] = None,
-    ) -> Iterable[StreamData]:
-        yield from self._read_pages(
-            lambda req, res, state, _slice: self.parse_response(res, stream_slice=_slice, stream_state=state), stream_slice, stream_state
-        )
-
-    def _read_pages(
-        self,
-        records_generator_fn: Callable[
-            [requests.PreparedRequest, requests.Response, Mapping[str, Any], Mapping[str, Any]], Iterable[StreamData]
-        ],
-        stream_slice: Mapping[str, Any] = None,
-        stream_state: Mapping[str, Any] = None,
-    ) -> Iterable[StreamData]:
-        stream_state = stream_state or {}
-        pagination_complete = False
-        next_page_token = None
-        while not pagination_complete:
-            request, response = self._fetch_next_page(stream_slice, stream_state, next_page_token)
-            yield from records_generator_fn(request, response, stream_state, stream_slice)
-
-            next_page_token = self.next_page_token(response)
-            if not next_page_token:
-                pagination_complete = True
-
-        # Always return an empty generator just in case no records were ever yielded
-        yield from []
-
-    def _fetch_next_page(
-        self, stream_slice: Mapping[str, Any] = None, stream_state: Mapping[str, Any] = None, next_page_token: Mapping[str, Any] = None
-    ) -> Tuple[requests.PreparedRequest, requests.Response]:
-        request_headers = self.request_headers(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
-        request = self._create_prepared_request(
-            path=self.path(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token),
-            headers=dict(request_headers, **self.authenticator.get_auth_header()),
-            params=self.request_params(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token),
-            json=self.request_body_json(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token),
-            data=self.request_body_data(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token),
-        )
-        request_kwargs = self.request_kwargs(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
-
-        response = self._send_request(request, request_kwargs)
-        return request, response
-
-
-class HttpSubStream(HttpStream, ABC):
-    def __init__(self, parent: HttpStream, **kwargs):
-        """
-        :param parent: should be the instance of HttpStream class
-        """
-        super().__init__(**kwargs)
-        self.parent = parent
-
-    def stream_slices(
-        self, sync_mode: SyncMode, cursor_field: List[str] = None, stream_state: Mapping[str, Any] = None
-    ) -> Iterable[Optional[Mapping[str, Any]]]:
-        parent_stream_slices = self.parent.stream_slices(
-            sync_mode=SyncMode.full_refresh, cursor_field=cursor_field, stream_state=stream_state
-        )
-
-        # iterate over all parent stream_slices
-        for stream_slice in parent_stream_slices:
-            parent_records = self.parent.read_records(
-                sync_mode=SyncMode.full_refresh, cursor_field=cursor_field, stream_slice=stream_slice, stream_state=stream_state
-            )
-
-            # iterate over all parent records with current stream_slice
-            for record in parent_records:
-                yield {"parent": record}
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_token.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/requests_native_auth/abstract_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from abc import abstractmethod
 from typing import Any, Mapping
 
 from requests.auth import AuthBase
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/streams/http/requests_native_auth/oauth.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/streams/http/requests_native_auth/token.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,73 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
-from typing import Any, List, Mapping
+import base64
+from itertools import cycle
+from typing import List
 
-import pendulum
-from airbyte_cdk.sources.streams.http.requests_native_auth.abstract_oauth import AbstractOauth2Authenticator
+from airbyte_cdk.sources.streams.http.requests_native_auth.abstract_token import AbstractHeaderAuthenticator
 
 
-class Oauth2Authenticator(AbstractOauth2Authenticator):
+class MultipleTokenAuthenticator(AbstractHeaderAuthenticator):
     """
-    Generates OAuth2.0 access tokens from an OAuth2.0 refresh token and client credentials.
-    The generated access token is attached to each request via the Authorization header.
+    Builds auth header, based on the list of tokens provided.
+    Auth header is changed per each `get_auth_header` call, using each token in cycle.
+    The token is attached to each request via the `auth_header` header.
     """
 
-    def __init__(
-        self,
-        token_refresh_endpoint: str,
-        client_id: str,
-        client_secret: str,
-        refresh_token: str,
-        scopes: List[str] = None,
-        token_expiry_date: pendulum.DateTime = None,
-        access_token_name: str = "access_token",
-        expires_in_name: str = "expires_in",
-        refresh_request_body: Mapping[str, Any] = None,
-        grant_type: str = "refresh_token",
-    ):
-        self._token_refresh_endpoint = token_refresh_endpoint
-        self._client_secret = client_secret
-        self._client_id = client_id
-        self._refresh_token = refresh_token
-        self._scopes = scopes
-        self._access_token_name = access_token_name
-        self._expires_in_name = expires_in_name
-        self._refresh_request_body = refresh_request_body
-        self._grant_type = grant_type
-
-        self._token_expiry_date = token_expiry_date or pendulum.now().subtract(days=1)
-        self._access_token = None
-
-    def get_token_refresh_endpoint(self) -> str:
-        return self._token_refresh_endpoint
+    @property
+    def auth_header(self) -> str:
+        return self._auth_header
 
-    def get_client_id(self) -> str:
-        return self._client_id
+    @property
+    def token(self) -> str:
+        return f"{self._auth_method} {next(self._tokens_iter)}"
 
-    def get_client_secret(self) -> str:
-        return self._client_secret
+    def __init__(self, tokens: List[str], auth_method: str = "Bearer", auth_header: str = "Authorization"):
+        self._auth_method = auth_method
+        self._auth_header = auth_header
+        self._tokens = tokens
+        self._tokens_iter = cycle(self._tokens)
 
-    def get_refresh_token(self) -> str:
-        return self._refresh_token
 
-    def get_access_token_name(self) -> str:
-        return self._access_token_name
+class TokenAuthenticator(AbstractHeaderAuthenticator):
+    """
+    Builds auth header, based on the token provided.
+    The token is attached to each request via the `auth_header` header.
+    """
 
-    def get_scopes(self) -> [str]:
-        return self._scopes
+    @property
+    def auth_header(self) -> str:
+        return self._auth_header
 
-    def get_expires_in_name(self) -> str:
-        return self._expires_in_name
+    @property
+    def token(self) -> str:
+        return f"{self._auth_method} {self._token}"
 
-    def get_refresh_request_body(self) -> Mapping[str, Any]:
-        return self._refresh_request_body
+    def __init__(self, token: str, auth_method: str = "Bearer", auth_header: str = "Authorization"):
+        self._auth_header = auth_header
+        self._auth_method = auth_method
+        self._token = token
 
-    def get_grant_type(self) -> str:
-        return self._grant_type
 
-    def get_token_expiry_date(self) -> pendulum.DateTime:
-        return self._token_expiry_date
+class BasicHttpAuthenticator(AbstractHeaderAuthenticator):
+    """
+    Builds auth based off the basic authentication scheme as defined by RFC 7617, which transmits credentials as USER ID/password pairs, encoded using bas64
+    https://developer.mozilla.org/en-US/docs/Web/HTTP/Authentication#basic_authentication_scheme
+    """
 
-    def set_token_expiry_date(self, value: pendulum.DateTime):
-        self._token_expiry_date = value
+    @property
+    def auth_header(self) -> str:
+        return self._auth_header
 
     @property
-    def access_token(self) -> str:
-        return self._access_token
+    def token(self) -> str:
+        return f"{self._auth_method} {self._token}"
 
-    @access_token.setter
-    def access_token(self, value: str):
-        self._access_token = value
+    def __init__(self, username: str, password: str = "", auth_method: str = "Basic", auth_header: str = "Authorization"):
+        auth_string = f"{username}:{password}".encode("utf8")
+        b64_encoded = base64.b64encode(auth_string).decode("utf8")
+        self._auth_header = auth_header
+        self._auth_method = auth_method
+        self._token = b64_encoded
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/catalog_helpers.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/catalog_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 from airbyte_cdk.models import AirbyteCatalog, SyncMode
 
 
 class CatalogHelper:
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/record_helper.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/record_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import datetime
 from typing import Any, Mapping
 
 from airbyte_cdk.models import AirbyteLogMessage, AirbyteMessage, AirbyteRecordMessage, AirbyteTraceMessage
 from airbyte_cdk.models import Type as MessageType
@@ -16,16 +16,16 @@
     data_or_message: StreamData,
     transformer: TypeTransformer = TypeTransformer(TransformConfig.NoTransform),
     schema: Mapping[str, Any] = None,
 ) -> AirbyteMessage:
     if schema is None:
         schema = {}
 
-    if isinstance(data_or_message, dict):
-        data = data_or_message
+    if isinstance(data_or_message, Mapping):
+        data = dict(data_or_message)
         now_millis = int(datetime.datetime.now().timestamp() * 1000)
         # Transform object fields according to config. Most likely you will
         # need it to normalize values against json schema. By default no action
         # taken unless configured. See
         # docs/connector-development/cdk-python/schemas.md for details.
         transformer.transform(data, schema)  # type: ignore
         message = AirbyteRecordMessage(stream=stream_name, data=data, emitted_at=now_millis)
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/schema_helpers.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/schema_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 import importlib
 import json
 import os
 import pkgutil
-from typing import Any, ClassVar, Dict, List, Mapping, MutableMapping, Optional, Tuple, Union
+from typing import Any, ClassVar, Dict, List, Mapping, MutableMapping, Optional, Tuple
 
 import jsonref
 from airbyte_cdk.models import ConnectorSpecification, FailureType
 from airbyte_cdk.utils.traced_exception import AirbyteTracedException
 from jsonschema import RefResolver, validate
 from jsonschema.exceptions import ValidationError
 from pydantic import BaseModel, Field
@@ -26,30 +26,38 @@
 
     def __init__(self, uri_base: str, shared: str):
         self.shared = shared
         self.uri_base = uri_base
 
     def __call__(self, uri: str) -> Dict[str, Any]:
         uri = uri.replace(self.uri_base, f"{self.uri_base}/{self.shared}/")
-        return json.load(open(uri))
+        with open(uri) as f:
+            data = json.load(f)
+            if isinstance(data, dict):
+                return data
+            else:
+                raise ValueError(f"Expected to read a dictionary from {uri}. Got: {data}")
 
 
-def resolve_ref_links(obj: Any) -> Union[Dict[str, Any], List[Any]]:
+def resolve_ref_links(obj: Any) -> Any:
     """
     Scan resolved schema and convert jsonref.JsonRef object to JSON serializable dict.
 
     :param obj - jsonschema object with ref field resolved.
     :return JSON serializable object with references without external dependencies.
     """
     if isinstance(obj, jsonref.JsonRef):
         obj = resolve_ref_links(obj.__subject__)
         # Omit existing definitions for external resource since
         # we dont need it anymore.
-        obj.pop("definitions", None)
-        return obj
+        if isinstance(obj, dict):
+            obj.pop("definitions", None)
+            return obj
+        else:
+            raise ValueError(f"Expected obj to be a dict. Got {obj}")
     elif isinstance(obj, dict):
         return {k: resolve_ref_links(v) for k, v in obj.items()}
     elif isinstance(obj, list):
         return [resolve_ref_links(item) for item in obj]
     else:
         return obj
 
@@ -103,15 +111,15 @@
 
 class ResourceSchemaLoader:
     """JSONSchema loader from package resources"""
 
     def __init__(self, package_name: str):
         self.package_name = package_name
 
-    def get_schema(self, name: str) -> dict:
+    def get_schema(self, name: str) -> dict[str, Any]:
         """
         This method retrieves a JSON schema from the schemas/ folder.
 
 
         The expected file structure is to have all top-level schemas (corresponding to streams) in the "schemas/" folder, with any shared $refs
         living inside the "schemas/shared/" folder. For example:
 
@@ -125,32 +133,38 @@
         if not raw_file:
             raise IOError(f"Cannot find file {schema_filename}")
         try:
             raw_schema = json.loads(raw_file)
         except ValueError as err:
             raise RuntimeError(f"Invalid JSON file format for file {schema_filename}") from err
 
-        return self.__resolve_schema_references(raw_schema)
+        return self._resolve_schema_references(raw_schema)
 
-    def __resolve_schema_references(self, raw_schema: dict) -> dict:
+    def _resolve_schema_references(self, raw_schema: dict[str, Any]) -> dict[str, Any]:
         """
         Resolve links to external references and move it to local "definitions" map.
 
         :param raw_schema jsonschema to lookup for external links.
         :return JSON serializable object with references without external dependencies.
         """
 
         package = importlib.import_module(self.package_name)
-        base = os.path.dirname(package.__file__) + "/"
+        if package.__file__:
+            base = os.path.dirname(package.__file__) + "/"
+        else:
+            raise ValueError(f"Package {package} does not have a valid __file__ field")
         resolved = jsonref.JsonRef.replace_refs(raw_schema, loader=JsonFileLoader(base, "schemas/shared"), base_uri=base)
         resolved = resolve_ref_links(resolved)
-        return resolved
+        if isinstance(resolved, dict):
+            return resolved
+        else:
+            raise ValueError(f"Expected resolved to be a dict. Got {resolved}")
 
 
-def check_config_against_spec_or_exit(config: Mapping[str, Any], spec: ConnectorSpecification):
+def check_config_against_spec_or_exit(config: Mapping[str, Any], spec: ConnectorSpecification) -> None:
     """
     Check config object against spec. In case of spec is invalid, throws
     an exception with validation error description.
 
     :param config - config loaded from file specified over command line
     :param spec - spec object generated by connector
     """
@@ -162,35 +176,46 @@
             message="Config validation error: " + validation_error.message,
             internal_message=validation_error.message,
             failure_type=FailureType.config_error,
         ) from None  # required to prevent logging config secrets from the ValidationError's stacktrace
 
 
 class InternalConfig(BaseModel):
-    KEYWORDS: ClassVar[set] = {"_limit", "_page_size"}
+    KEYWORDS: ClassVar[set[str]] = {"_limit", "_page_size"}
     limit: int = Field(None, alias="_limit")
     page_size: int = Field(None, alias="_page_size")
 
-    def dict(self, *args, **kwargs):
+    def dict(self, *args: Any, **kwargs: Any) -> dict[str, Any]:
         kwargs["by_alias"] = True
         kwargs["exclude_unset"] = True
         return super().dict(*args, **kwargs)
 
+    def is_limit_reached(self, records_counter: int) -> bool:
+        """
+        Check if record count reached limit set by internal config.
+        :param records_counter - number of records already red
+        :return True if limit reached, False otherwise
+        """
+        if self.limit:
+            if records_counter >= self.limit:
+                return True
+        return False
+
 
-def split_config(config: Mapping[str, Any]) -> Tuple[dict, InternalConfig]:
+def split_config(config: Mapping[str, Any]) -> Tuple[dict[str, Any], InternalConfig]:
     """
     Break config map object into 2 instances: first is a dict with user defined
     configuration and second is internal config that contains private keys for
     acceptance test configuration.
 
     :param
      config - Dict object that has been loaded from config file.
 
     :return tuple of user defined config dict with filtered out internal
-    parameters and SAT internal config object.
+    parameters and connector acceptance test internal config object.
     """
     main_config = {}
     internal_config = {}
     for k, v in config.items():
         if k in InternalConfig.KEYWORDS:
             internal_config[k] = v
         else:
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/schema_models.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/schema_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from typing import Any, Dict, Optional, Type
 
 from airbyte_cdk.sources.utils.schema_helpers import expand_refs
 from pydantic import BaseModel, Extra
 from pydantic.main import ModelMetaclass
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/sources/utils/transform.py` & `airbyte_cdk-0.90.0/airbyte_cdk/sources/utils/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import logging
 from distutils.util import strtobool
 from enum import Flag, auto
 from typing import Any, Callable, Dict, Mapping, Optional
 
 from jsonschema import Draft7Validator, ValidationError, validators
 
 json_to_python_simple = {"string": str, "number": float, "integer": int, "boolean": bool, "null": type(None)}
-json_to_python = json_to_python_simple | {"object": dict, "array": list}
+json_to_python = {**json_to_python_simple, **{"object": dict, "array": list}}
 python_to_json = {v: k for k, v in json_to_python.items()}
 
 logger = logging.getLogger("airbyte")
 
 
 class TransformConfig(Flag):
     """
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/utils/airbyte_secrets_utils.py` & `airbyte_cdk-0.90.0/airbyte_cdk/utils/airbyte_secrets_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from typing import Any, List, Mapping
 
 import dpath.util
 
 
 def get_secret_paths(spec: Mapping[str, Any]) -> List[List[str]]:
     paths = []
 
-    def traverse_schema(schema_item: Any, path: List[str]):
+    def traverse_schema(schema_item: Any, path: List[str]) -> None:
         """
         schema_item can be any property or value in the originally input jsonschema, depending on how far down the recursion stack we go
         path is the path to that schema item in the original input
         for example if we have the input {'password': {'type': 'string', 'airbyte_secret': True}} then the arguments will evolve
         as follows:
         schema_item=<whole_object>, path=[]
         schema_item={'type': 'string', 'airbyte_secret': True}, path=['password']
@@ -52,20 +52,26 @@
             pass
     return result
 
 
 __SECRETS_FROM_CONFIG: List[str] = []
 
 
-def update_secrets(secrets: List[str]):
+def update_secrets(secrets: List[str]) -> None:
     """Update the list of secrets to be replaced"""
     global __SECRETS_FROM_CONFIG
     __SECRETS_FROM_CONFIG = secrets
 
 
+def add_to_secrets(secret: str) -> None:
+    """Add to the list of secrets to be replaced"""
+    global __SECRETS_FROM_CONFIG
+    __SECRETS_FROM_CONFIG.append(secret)
+
+
 def filter_secrets(string: str) -> str:
     """Filter secrets from a string by replacing them with ****"""
     # TODO this should perform a maximal match for each secret. if "x" and "xk" are both secret values, and this method is called twice on
     #  the input "xk", then depending on call order it might only obfuscate "*k". This is a bug.
     for secret in __SECRETS_FROM_CONFIG:
         if secret:
             string = string.replace(str(secret), "****")
```

### Comparing `airbyte-cdk-0.9.5/airbyte_cdk/utils/event_timing.py` & `airbyte_cdk-0.90.0/airbyte_cdk/utils/event_timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 Airbyte, Inc., all rights reserved.
+# Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import datetime
 import logging
 import time
 from contextlib import contextmanager
 from dataclasses import dataclass, field
```

