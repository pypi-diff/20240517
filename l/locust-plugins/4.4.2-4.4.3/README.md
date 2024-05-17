# Comparing `tmp/locust-plugins-4.4.2.tar.gz` & `tmp/locust_plugins-4.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locust-plugins-4.4.2.tar", last modified: Thu Feb 22 18:08:42 2024, max compression
+gzip compressed data, was "locust_plugins-4.4.3.tar", last modified: Fri May 17 13:51:50 2024, max compression
```

## Comparing `locust-plugins-4.4.2.tar` & `locust_plugins-4.4.3.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.160384 locust-plugins-4.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.136384 locust-plugins-4.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.144384 locust-plugins-4.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.144384 locust-plugins-4.4.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-02-22 18:08:42.160384 locust-plugins-4.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.144384 locust-plugins-4.4.2/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/bin/locust-compose
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.148384 locust-plugins-4.4.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/appinsights_listener_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/cloudwatch_listener_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/cmd_line_examples.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/connection_pool_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/constant_total_ips_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/csvreader_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/distributor_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/embedded_resource_manager_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/jmeter_listener_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/kafka_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/mongoreader_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/mqtt_custom_client_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/mqtt_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/playwright-recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/playwright_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/products.csv
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/reschedule_on_fail_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/rest_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/socketio_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/ssn.csv
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/ssn.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/transaction_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/transaction_example_as_library_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/transaction_example_as_library_master.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/transaction_example_as_library_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/tsvreader_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/examples/webdriver_ex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.148384 locust-plugins-4.4.2/locust_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-22 18:08:42.000000 locust-plugins-4.4.2/locust_plugins/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12621 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/connection_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/csvreader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.152384 locust-plugins-4.4.2/locust_plugins/dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.152384 locust-plugins-4.4.2/locust_plugins/dashboards/locust-grafana/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/locust-grafana/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/locust-grafana/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)      563 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/locust-grafana/create_datasource.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      566 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/locust-grafana/grafana_setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      551 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/locust-grafana/import_dashboards.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.152384 locust-plugins-4.4.2/locust_plugins/dashboards/locust-timescale/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/locust-timescale/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/locust-timescale/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/locust-timescale/timescale_schema.sql
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/locust-timescale/zz_hypertable.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.156384 locust-plugins-4.4.2/locust_plugins/dashboards/screenshots/
--rw-r--r--   0 runner    (1001) docker     (127)   392198 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/screenshots/main_dashboard.png
--rw-r--r--   0 runner    (1001) docker     (127)   425926 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/screenshots/main_dashboard_by_request_graphs.png
--rw-r--r--   0 runner    (1001) docker     (127)   267958 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/screenshots/requests_table.png
--rw-r--r--   0 runner    (1001) docker     (127)   187305 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/screenshots/scatter_plot.png
--rw-r--r--   0 runner    (1001) docker     (127)   372353 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/dashboards/screenshots/testruns.png
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/distributor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.156384 locust-plugins-4.4.2/locust_plugins/listeners/
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/listeners/appinsights.py
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/listeners/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/listeners/jmeter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15227 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/listeners/timescale.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/mongoreader.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/transaction_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.160384 locust-plugins-4.4.2/locust_plugins/users/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/users/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/users/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)    15992 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/users/playwright.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/users/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/users/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/users/socketio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/users/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/locust_plugins/wait_time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.160384 locust-plugins-4.4.2/locust_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-02-22 18:08:42.000000 locust-plugins-4.4.2/locust_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-02-22 18:08:42.000000 locust-plugins-4.4.2/locust_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 18:08:42.000000 locust-plugins-4.4.2/locust_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 18:08:42.000000 locust-plugins-4.4.2/locust_plugins.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-22 18:08:42.000000 locust-plugins-4.4.2/locust_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-22 18:08:42.000000 locust-plugins-4.4.2/locust_plugins.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 18:08:42.160384 locust-plugins-4.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:08:42.160384 locust-plugins-4.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/test/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/test/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/test/test_cloudwatch_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/test/test_missing_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-02-22 18:08:36.000000 locust-plugins-4.4.2/tusk.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.452203 locust_plugins-4.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.432203 locust_plugins-4.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.436203 locust_plugins-4.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.436203 locust_plugins-4.4.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-17 13:51:50.452203 locust_plugins-4.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.436203 locust_plugins-4.4.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/bin/locust-compose
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.440203 locust_plugins-4.4.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/appinsights_listener_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/cloudwatch_listener_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/cmd_line_examples.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/connection_pool_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/constant_total_ips_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/csvreader_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/distributor_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/embedded_resource_manager_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/jmeter_listener_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/kafka_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/mongoreader_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/mqtt_custom_client_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/mqtt_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/playwright-recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/playwright_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/products.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/reschedule_on_fail_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/rest_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/socketio_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/ssn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/ssn.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/transaction_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/transaction_example_as_library_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/transaction_example_as_library_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/transaction_example_as_library_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/tsvreader_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/examples/webdriver_ex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.444203 locust_plugins-4.4.3/locust_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 13:51:50.000000 locust_plugins-4.4.3/locust_plugins/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12621 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/connection_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/csvreader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.444203 locust_plugins-4.4.3/locust_plugins/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.444203 locust_plugins-4.4.3/locust_plugins/dashboards/locust-grafana/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/locust-grafana/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/locust-grafana/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      563 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/locust-grafana/create_datasource.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      566 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/locust-grafana/grafana_setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      551 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/locust-grafana/import_dashboards.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.444203 locust_plugins-4.4.3/locust_plugins/dashboards/locust-timescale/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/locust-timescale/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/locust-timescale/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/locust-timescale/timescale_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/locust-timescale/zz_hypertable.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.448203 locust_plugins-4.4.3/locust_plugins/dashboards/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (127)   392198 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/screenshots/main_dashboard.png
+-rw-r--r--   0 runner    (1001) docker     (127)   425926 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/screenshots/main_dashboard_by_request_graphs.png
+-rw-r--r--   0 runner    (1001) docker     (127)   267958 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/screenshots/requests_table.png
+-rw-r--r--   0 runner    (1001) docker     (127)   187305 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/screenshots/scatter_plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   372353 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/dashboards/screenshots/testruns.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/distributor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.448203 locust_plugins-4.4.3/locust_plugins/listeners/
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/listeners/appinsights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/listeners/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/listeners/jmeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15358 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/listeners/timescale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/mongoreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/transaction_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.452203 locust_plugins-4.4.3/locust_plugins/users/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/users/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/users/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15992 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/users/playwright.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/users/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/users/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/users/socketio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/users/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/locust_plugins/wait_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.452203 locust_plugins-4.4.3/locust_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-17 13:51:50.000000 locust_plugins-4.4.3/locust_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-17 13:51:50.000000 locust_plugins-4.4.3/locust_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:51:50.000000 locust_plugins-4.4.3/locust_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:51:50.000000 locust_plugins-4.4.3/locust_plugins.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-17 13:51:50.000000 locust_plugins-4.4.3/locust_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 13:51:50.000000 locust_plugins-4.4.3/locust_plugins.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 13:51:50.452203 locust_plugins-4.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:51:50.452203 locust_plugins-4.4.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/test/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/test/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/test/test_cloudwatch_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/test/test_missing_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-17 13:51:46.000000 locust_plugins-4.4.3/tusk.yaml
```

### Comparing `locust-plugins-4.4.2/.github/workflows/stale.yml` & `locust_plugins-4.4.3/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/.github/workflows/tests.yml` & `locust_plugins-4.4.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/.pylintrc` & `locust_plugins-4.4.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/.vscode/launch.json` & `locust_plugins-4.4.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/.vscode/settings.json` & `locust_plugins-4.4.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/CONTRIBUTING.md` & `locust_plugins-4.4.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/LICENSE` & `locust_plugins-4.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/PKG-INFO` & `locust_plugins-4.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-plugins
-Version: 4.4.2
+Version: 4.4.3
 Summary: Useful plugins/extensions for Locust
 Home-page: https://github.com/SvenskaSpel/locust-plugins
 Author: Lars Holmberg
 License: Apache-2.0
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `locust-plugins-4.4.2/README.md` & `locust_plugins-4.4.3/README.md`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/cmd_line_examples.sh` & `locust_plugins-4.4.3/examples/cmd_line_examples.sh`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/connection_pool_ex.py` & `locust_plugins-4.4.3/examples/connection_pool_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/constant_total_ips_ex.py` & `locust_plugins-4.4.3/examples/constant_total_ips_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/distributor_ex.py` & `locust_plugins-4.4.3/examples/distributor_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/embedded_resource_manager_ex.py` & `locust_plugins-4.4.3/examples/embedded_resource_manager_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/kafka_ex.py` & `locust_plugins-4.4.3/examples/kafka_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/mongoreader_ex.py` & `locust_plugins-4.4.3/examples/mongoreader_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/mqtt_custom_client_ex.py` & `locust_plugins-4.4.3/examples/mqtt_custom_client_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/mqtt_ex.py` & `locust_plugins-4.4.3/examples/mqtt_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/playwright-recording.py` & `locust_plugins-4.4.3/examples/playwright-recording.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/playwright_ex.py` & `locust_plugins-4.4.3/examples/playwright_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/reschedule_on_fail_ex.py` & `locust_plugins-4.4.3/examples/reschedule_on_fail_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/rest_ex.py` & `locust_plugins-4.4.3/examples/rest_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/socketio_ex.py` & `locust_plugins-4.4.3/examples/socketio_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/transaction_example.py` & `locust_plugins-4.4.3/examples/transaction_example.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/transaction_example_as_library_local.py` & `locust_plugins-4.4.3/examples/transaction_example_as_library_local.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/transaction_example_as_library_master.py` & `locust_plugins-4.4.3/examples/transaction_example_as_library_master.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/transaction_example_as_library_worker.py` & `locust_plugins-4.4.3/examples/transaction_example_as_library_worker.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/examples/webdriver_ex.py` & `locust_plugins-4.4.3/examples/webdriver_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/__init__.py` & `locust_plugins-4.4.3/locust_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/connection_pools.py` & `locust_plugins-4.4.3/locust_plugins/connection_pools.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/csvreader.py` & `locust_plugins-4.4.3/locust_plugins/csvreader.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/dashboards/README.md` & `locust_plugins-4.4.3/locust_plugins/dashboards/README.md`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/dashboards/docker-compose.yml` & `locust_plugins-4.4.3/locust_plugins/dashboards/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/dashboards/locust-grafana/create_datasource.sh` & `locust_plugins-4.4.3/locust_plugins/dashboards/locust-grafana/create_datasource.sh`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/dashboards/locust-grafana/grafana_setup.sh` & `locust_plugins-4.4.3/locust_plugins/dashboards/locust-grafana/grafana_setup.sh`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/dashboards/locust-grafana/import_dashboards.sh` & `locust_plugins-4.4.3/locust_plugins/dashboards/locust-grafana/import_dashboards.sh`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/dashboards/locust-timescale/timescale_schema.sql` & `locust_plugins-4.4.3/locust_plugins/dashboards/locust-timescale/timescale_schema.sql`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/dashboards/screenshots/main_dashboard.png` & `locust_plugins-4.4.3/locust_plugins/dashboards/screenshots/main_dashboard.png`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/dashboards/screenshots/main_dashboard_by_request_graphs.png` & `locust_plugins-4.4.3/locust_plugins/dashboards/screenshots/main_dashboard_by_request_graphs.png`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/dashboards/screenshots/requests_table.png` & `locust_plugins-4.4.3/locust_plugins/dashboards/screenshots/requests_table.png`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/dashboards/screenshots/scatter_plot.png` & `locust_plugins-4.4.3/locust_plugins/dashboards/screenshots/scatter_plot.png`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/dashboards/screenshots/testruns.png` & `locust_plugins-4.4.3/locust_plugins/dashboards/screenshots/testruns.png`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/distributor.py` & `locust_plugins-4.4.3/locust_plugins/distributor.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/listeners/__init__.py` & `locust_plugins-4.4.3/locust_plugins/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/listeners/appinsights.py` & `locust_plugins-4.4.3/locust_plugins/listeners/appinsights.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/listeners/cloudwatch.py` & `locust_plugins-4.4.3/locust_plugins/listeners/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/listeners/jmeter.py` & `locust_plugins-4.4.3/locust_plugins/listeners/jmeter.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/listeners/timescale.py` & `locust_plugins-4.4.3/locust_plugins/listeners/timescale.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# See timescale_listener_ex.py for documentation
 from contextlib import contextmanager
 from locust.exception import CatchResponseError  # need to do this first to make sure monkey patching is done
 import json
 import locust.env
 import gevent
 from gevent.lock import Semaphore
 import logging
@@ -139,14 +138,17 @@
             if environment.runner is not None:
                 logging.debug(f"about to send run_id to workers: {msg}")
                 environment.runner.send_message("run_id", msg)
             self.log_start_testrun()
             self._user_count_logger = gevent.spawn(self._log_user_count)
 
     def _dbconn(self) -> psycopg2.extensions.connection:
+        logging.debug(
+            f"Connecting to Postgres ({self.env.parsed_options.pguser}@{self.env.parsed_options.pghost}:{self.env.parsed_options.pgport or 5432})"
+        )
         try:
             conn = psycopg2.connect(
                 host=self.env.parsed_options.pghost,
                 user=self.env.parsed_options.pguser,
                 password=self.env.parsed_options.pgpassword,
                 database=self.env.parsed_options.pgdatabase,
                 port=self.env.parsed_options.pgport,
```

### Comparing `locust-plugins-4.4.2/locust_plugins/mongoreader.py` & `locust_plugins-4.4.3/locust_plugins/mongoreader.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/transaction_manager.py` & `locust_plugins-4.4.3/locust_plugins/transaction_manager.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/users/kafka.py` & `locust_plugins-4.4.3/locust_plugins/users/kafka.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/users/mqtt.py` & `locust_plugins-4.4.3/locust_plugins/users/mqtt.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/users/playwright.py` & `locust_plugins-4.4.3/locust_plugins/users/playwright.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/users/resource.py` & `locust_plugins-4.4.3/locust_plugins/users/resource.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/users/rest.py` & `locust_plugins-4.4.3/locust_plugins/users/rest.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/users/socketio.py` & `locust_plugins-4.4.3/locust_plugins/users/socketio.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/users/webdriver.py` & `locust_plugins-4.4.3/locust_plugins/users/webdriver.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins/wait_time.py` & `locust_plugins-4.4.3/locust_plugins/wait_time.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/locust_plugins.egg-info/PKG-INFO` & `locust_plugins-4.4.3/locust_plugins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-plugins
-Version: 4.4.2
+Version: 4.4.3
 Summary: Useful plugins/extensions for Locust
 Home-page: https://github.com/SvenskaSpel/locust-plugins
 Author: Lars Holmberg
 License: Apache-2.0
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `locust-plugins-4.4.2/locust_plugins.egg-info/SOURCES.txt` & `locust_plugins-4.4.3/locust_plugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/setup.py` & `locust_plugins-4.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/test/test_all.py` & `locust_plugins-4.4.3/test/test_all.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/test/test_cloudwatch_plugin.py` & `locust_plugins-4.4.3/test/test_cloudwatch_plugin.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/test/test_missing_extras.py` & `locust_plugins-4.4.3/test/test_missing_extras.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/tox.ini` & `locust_plugins-4.4.3/tox.ini`

 * *Files identical despite different names*

### Comparing `locust-plugins-4.4.2/tusk.yaml` & `locust_plugins-4.4.3/tusk.yaml`

 * *Files identical despite different names*

