# Comparing `tmp/microcosm-flask-4.1.6.tar.gz` & `tmp/microcosm-flask-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microcosm-flask-4.1.6.tar", last modified: Fri Mar 15 15:48:15 2024, max compression
+gzip compressed data, was "dist/microcosm-flask-5.0.0.tar", last modified: Fri May 17 16:50:09 2024, max compression
```

## Comparing `microcosm-flask-4.1.6.tar` & `microcosm-flask-5.0.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1918 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1400 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11299 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/audit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2074 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/basic_auth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2483 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/cloning.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      961 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/context.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1856 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/alias.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5077 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1833 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/build_info.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1053 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/catchall.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2177 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16549 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/crud.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2504 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/crud_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2607 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/discovery.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5785 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/encoding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4673 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/health.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3573 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/landing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3173 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/logging_level.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4048 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10346 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/relation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2419 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/saved_search.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2926 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/swagger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4384 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/conventions/upload.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/converters.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask/decorators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/decorators/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/decorators/logging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4000 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/decorators/schemas.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask/encryption/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/encryption/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask/encryption/conventions/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/encryption/conventions/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1330 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/encryption/conventions/crud_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1660 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/enums.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4697 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1039 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/factories.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask/fields/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      556 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/fields/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      460 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/fields/cleaned_field.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1734 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/fields/enum_field.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      841 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/fields/language_field.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2270 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/fields/order_by_field.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1044 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/fields/query_string_list.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1569 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/fields/timestamp_field.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1963 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/fields/uri_field.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask/formatting/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      302 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/formatting/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1936 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/formatting/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2782 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/formatting/csv_formatter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/formatting/encoding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      280 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/formatting/html_formatter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      331 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/formatting/json_formatter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      281 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/formatting/text_formatter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2098 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/forwarding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3216 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/linking.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2180 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/matchers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2094 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/memory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1422 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/metrics.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      995 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/metrics_classifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5834 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/namespaces.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1492 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/naming.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3011 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/operations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10104 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/paging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      781 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/paths.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1370 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/profiling.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2965 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/routing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      903 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/runserver.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2213 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/sentry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1046 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/session.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1100 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      545 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/decorators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13065 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/definitions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      869 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/naming.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1830 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2889 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      909 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/constant.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      855 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/decorated.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/default.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2272 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/enum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/list.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/nested.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      557 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/numeric.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      708 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/timestamp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3084 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/swagger/schemas.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/templates/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3703 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/templates/landing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1830 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/microcosm_flask/templates/swagger_ui.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1918 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3389 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1910 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/microcosm_flask.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      632 2024-03-15 15:48:15.000000 microcosm-flask-4.1.6/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4150 2024-03-15 15:45:07.000000 microcosm-flask-4.1.6/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1918 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1400 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11299 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/audit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2074 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/basic_auth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2483 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/cloning.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      961 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/context.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1856 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/alias.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5077 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1833 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/build_info.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1053 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/catchall.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2177 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16549 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/crud.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2504 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/crud_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2607 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/discovery.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5785 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/encoding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4673 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/health.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3573 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/landing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3173 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/logging_level.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4048 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/registry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10346 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/relation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2419 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/saved_search.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2926 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/swagger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4384 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/conventions/upload.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/converters.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask/decorators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/decorators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/decorators/logging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4000 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/decorators/schemas.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask/encryption/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/encryption/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask/encryption/conventions/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/encryption/conventions/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1330 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/encryption/conventions/crud_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1660 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/enums.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4697 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1039 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/factories.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask/fields/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      556 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/fields/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      460 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/fields/cleaned_field.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1734 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/fields/enum_field.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      841 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/fields/language_field.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2270 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/fields/order_by_field.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1044 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/fields/query_string_list.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1569 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/fields/timestamp_field.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1963 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/fields/uri_field.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask/formatting/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      302 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/formatting/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1988 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/formatting/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2782 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/formatting/csv_formatter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/formatting/encoding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      280 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/formatting/html_formatter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      331 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/formatting/json_formatter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      281 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/formatting/text_formatter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1891 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/forwarding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3216 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/linking.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2180 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/matchers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2094 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/memory.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1422 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/metrics.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      995 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/metrics_classifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5834 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/namespaces.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1492 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/naming.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3011 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/operations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10104 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/paging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      781 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/paths.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1370 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/profiling.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2965 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/routing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      903 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/runserver.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2269 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/sentry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1046 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/session.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1100 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      545 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/decorators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12795 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/definitions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      869 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/naming.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1830 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2889 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      909 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/constant.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      855 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/decorated.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/default.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2272 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/enum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      654 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/list.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/nested.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      557 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/numeric.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      708 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/timestamp.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3084 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/swagger/schemas.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/templates/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3703 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/templates/landing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1830 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/microcosm_flask/templates/swagger_ui.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1918 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3389 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1910 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      565 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/microcosm_flask.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      632 2024-05-17 16:50:09.000000 microcosm-flask-5.0.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4091 2024-05-17 16:47:44.000000 microcosm-flask-5.0.0/setup.py
```

### Comparing `microcosm-flask-4.1.6/LICENSE` & `microcosm-flask-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/PKG-INFO` & `microcosm-flask-5.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcosm-flask
-Version: 4.1.6
+Version: 5.0.0
 Summary: Opinionated persistence with FlaskQL
 Home-page: https://github.com/globality-corp/microcosm-flask
 Author: Globality Engineering
 Author-email: engineering@globality.com
 License: UNKNOWN
 Keywords: microcosm
 Platform: UNKNOWN
```

### Comparing `microcosm-flask-4.1.6/README.md` & `microcosm-flask-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/audit.py` & `microcosm-flask-5.0.0/microcosm_flask/audit.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/basic_auth.py` & `microcosm-flask-5.0.0/microcosm_flask/basic_auth.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/cloning.py` & `microcosm-flask-5.0.0/microcosm_flask/cloning.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/context.py` & `microcosm-flask-5.0.0/microcosm_flask/context.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/alias.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/alias.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/base.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/base.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/build_info.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/build_info.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/catchall.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/catchall.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/config.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/config.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/crud.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/crud.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/crud_adapter.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/crud_adapter.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/discovery.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/discovery.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/encoding.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/encoding.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/health.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/health.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/landing.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/landing.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/logging_level.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/logging_level.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/registry.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/registry.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/relation.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/relation.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/saved_search.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/saved_search.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/swagger.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/swagger.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/conventions/upload.py` & `microcosm-flask-5.0.0/microcosm_flask/conventions/upload.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/decorators/logging.py` & `microcosm-flask-5.0.0/microcosm_flask/decorators/logging.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/decorators/schemas.py` & `microcosm-flask-5.0.0/microcosm_flask/decorators/schemas.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/encryption/conventions/crud_adapter.py` & `microcosm-flask-5.0.0/microcosm_flask/encryption/conventions/crud_adapter.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/enums.py` & `microcosm-flask-5.0.0/microcosm_flask/enums.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/errors.py` & `microcosm-flask-5.0.0/microcosm_flask/errors.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/factories.py` & `microcosm-flask-5.0.0/microcosm_flask/factories.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/fields/__init__.py` & `microcosm-flask-5.0.0/microcosm_flask/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/fields/enum_field.py` & `microcosm-flask-5.0.0/microcosm_flask/fields/enum_field.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/fields/language_field.py` & `microcosm-flask-5.0.0/microcosm_flask/fields/language_field.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/fields/order_by_field.py` & `microcosm-flask-5.0.0/microcosm_flask/fields/order_by_field.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/fields/query_string_list.py` & `microcosm-flask-5.0.0/microcosm_flask/fields/query_string_list.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/fields/timestamp_field.py` & `microcosm-flask-5.0.0/microcosm_flask/fields/timestamp_field.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/fields/uri_field.py` & `microcosm-flask-5.0.0/microcosm_flask/fields/uri_field.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/formatting/base.py` & `microcosm-flask-5.0.0/microcosm_flask/formatting/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from abc import ABCMeta, abstractmethod
 from binascii import hexlify
 
 from flask import Response
 from werkzeug.http import quote_etag
 from werkzeug.utils import get_content_type
 
+from microcosm_flask.formatting.encoding import UTF_8
+
 
 try:
     import spooky
 except ImportError:
     spooky = None
 
 
@@ -36,15 +38,15 @@
 
     def format(self, response_data):
         return response_data
 
     def build_response(self, response_data):
         return Response(
             self.format(response_data),
-            content_type=get_content_type(self.content_type, "utf-8"),
+            content_type=get_content_type(self.content_type, UTF_8)
         )
 
     def build_headers(self, headers, **kwargs):
         return headers
 
     def build_etag(self, response, include_etag=True, **kwargs):
         """
```

### Comparing `microcosm-flask-4.1.6/microcosm_flask/formatting/csv_formatter.py` & `microcosm-flask-5.0.0/microcosm_flask/formatting/csv_formatter.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/linking.py` & `microcosm-flask-5.0.0/microcosm_flask/linking.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/matchers.py` & `microcosm-flask-5.0.0/microcosm_flask/matchers.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/memory.py` & `microcosm-flask-5.0.0/microcosm_flask/memory.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/metrics.py` & `microcosm-flask-5.0.0/microcosm_flask/metrics.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/metrics_classifier.py` & `microcosm-flask-5.0.0/microcosm_flask/metrics_classifier.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/namespaces.py` & `microcosm-flask-5.0.0/microcosm_flask/namespaces.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/naming.py` & `microcosm-flask-5.0.0/microcosm_flask/naming.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/operations.py` & `microcosm-flask-5.0.0/microcosm_flask/operations.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/paging.py` & `microcosm-flask-5.0.0/microcosm_flask/paging.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/paths.py` & `microcosm-flask-5.0.0/microcosm_flask/paths.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/profiling.py` & `microcosm-flask-5.0.0/microcosm_flask/profiling.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/routing.py` & `microcosm-flask-5.0.0/microcosm_flask/routing.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/runserver.py` & `microcosm-flask-5.0.0/microcosm_flask/runserver.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/sentry.py` & `microcosm-flask-5.0.0/microcosm_flask/sentry.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from microcosm_logging.decorators import logger
 
 
 try:
     import sentry_sdk
     from sentry_sdk.utils import BadDsn
 except ImportError:
-    sentry_sdk = None
+    sentry_sdk = None  # type: ignore[assignment]
 
 
 @dataclass
 class SentryConfig:
     dsn: str | None = None
     enabled: bool = False
     client: Any | None = None
@@ -50,15 +50,15 @@
     if graph.config.sentry_logging.enabled and graph.config.sentry_logging.dsn:
         enabled = graph.config.sentry_logging.enabled
         dsn = graph.config.sentry_logging.dsn
         if graph.metadata.testing:
             sentry = MagicMock()
         elif sentry_sdk:
             try:
-                sentry = sentry_sdk.init(
+                sentry = sentry_sdk.init(  # type: ignore[assignment]
                     graph.config.sentry_logging.dsn,
                     server_name=f"{graph.metadata.name}_api",
                     release=graph.config.build_info_convention.sha1,
                     environment=environ.get("MICROCOSM_ENVIRONMENT") or "undefined",
                     before_send=before_send,
                 )
             except BadDsn:
```

### Comparing `microcosm-flask-4.1.6/microcosm_flask/session.py` & `microcosm-flask-5.0.0/microcosm_flask/session.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/api.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/api.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/decorators.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/decorators.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/definitions.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/definitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 """
 from enum import Enum, unique
 from inspect import getdoc
 from logging import getLogger
 from urllib.parse import unquote
 
-import flask
+from flask.globals import request_ctx
 from openapi import model as swagger
 from werkzeug.routing import BuildError, Rule
 
 from microcosm_flask.conventions.registry import (
     get_qs_schema,
     get_request_schema,
     get_response_schema,
@@ -95,21 +95,15 @@
 
 def _construct_schema_request_arguments():
     """
     Create a mapping between a given endpoint/method and its possible arguments.
     Used in aid of generating paths during swagger generation
 
     """
-    if hasattr(flask, "globals") and hasattr(flask.globals, "request_ctx"):
-        # update session for Flask >= 2.2
-        reqctx = flask.globals.request_ctx._get_current_object()
-    else:  # pragma: no cover
-        # update session for Flask < 2.2
-        reqctx = flask._request_ctx_stack.top
-    url_adapter = reqctx.url_adapter
+    url_adapter = request_ctx.url_adapter
     rules: list[Rule] = url_adapter.map._rules
 
     return {
         (rule.endpoint, method): rule.arguments
         for rule in rules
         for method in rule.methods
     }
```

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/naming.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/naming.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/__init__.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/base.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/base.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/constant.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/constant.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/decorated.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/decorated.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/default.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/default.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/enum.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/enum.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/list.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/list.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/nested.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/nested.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/numeric.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/numeric.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/parameters/timestamp.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/parameters/timestamp.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/swagger/schemas.py` & `microcosm-flask-5.0.0/microcosm_flask/swagger/schemas.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/templates/landing.py` & `microcosm-flask-5.0.0/microcosm_flask/templates/landing.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask/templates/swagger_ui.py` & `microcosm-flask-5.0.0/microcosm_flask/templates/swagger_ui.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask.egg-info/PKG-INFO` & `microcosm-flask-5.0.0/microcosm_flask.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcosm-flask
-Version: 4.1.6
+Version: 5.0.0
 Summary: Opinionated persistence with FlaskQL
 Home-page: https://github.com/globality-corp/microcosm-flask
 Author: Globality Engineering
 Author-email: engineering@globality.com
 License: UNKNOWN
 Keywords: microcosm
 Platform: UNKNOWN
```

### Comparing `microcosm-flask-4.1.6/microcosm_flask.egg-info/SOURCES.txt` & `microcosm-flask-5.0.0/microcosm_flask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/microcosm_flask.egg-info/entry_points.txt` & `microcosm-flask-5.0.0/microcosm_flask.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/setup.cfg` & `microcosm-flask-5.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.6/setup.py` & `microcosm-flask-5.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 
 
 project = "microcosm-flask"
-version = "4.1.6"
+version = "5.0.0"
 
 
 setup(
     name=project,
     version=version,
     description="Opinionated persistence with FlaskQL",
     long_description=open("README.md").read(),
@@ -17,15 +17,15 @@
     url="https://github.com/globality-corp/microcosm-flask",
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.10",
     keywords="microcosm",
     install_requires=[
-        "Flask>=2",
+        "Flask>=3",
         "Flask-BasicAuth>=0.2.0",
         "Flask-Cors>=3.0.7",
         "Flask-UUID>=0.2",
         "jsonschema>=3.2.0",
         "marshmallow>=3.0.0",
         "microcosm>=3.1.0",
         "microcosm-logging>=1.5.0",
@@ -43,26 +43,26 @@
         "spooky": "spooky>=2.0.0",
         "test": [
             "sentry-sdk>=0.14.4",
             "PyHamcrest",
             "coverage",
             "parameterized",
             "pytest-cov",
+            "microcosm-metrics",
         ],
         "lint": [
+            "mypy",
             "flake8",
             "flake8-print",
             "flake8-logging-format",
             "flake8-isort",
+            "types-python-dateutil",
+            "types-setuptools",
         ],
     },
-    setup_requires=[
-        "nose>=1.3.7",
-    ],
-    dependency_links=[],
     entry_points={
         "microcosm_flask.swagger.parameters": [
             "constant = microcosm_flask.swagger.parameters.constant:ConstantParameterBuilder",
             "decorated = microcosm_flask.swagger.parameters.decorated:DecoratedParameterBuilder",
             "enum = microcosm_flask.swagger.parameters.enum:EnumParameterBuilder",
             "list = microcosm_flask.swagger.parameters.list:ListParameterBuilder",
             "nested = microcosm_flask.swagger.parameters.nested:NestedParameterBuilder",
@@ -88,13 +88,8 @@
             "route_metrics = microcosm_flask.metrics:RouteMetrics",
             "sentry_logging = microcosm_flask.sentry:configure_sentry",
             "swagger_convention = microcosm_flask.conventions.swagger:configure_swagger",
             "uuid = microcosm_flask.converters:configure_uuid",
             "memory_profiler = microcosm_flask.memory:MemoryProfiler",
         ],
     },
-    tests_require=[
-        "coverage>=3.7.1",
-        "PyHamcrest>=1.9.0",
-        "pytest-cov",
-    ],
 )
```

