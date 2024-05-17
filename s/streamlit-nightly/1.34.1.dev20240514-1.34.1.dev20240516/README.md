# Comparing `tmp/streamlit_nightly-1.34.1.dev20240514.tar.gz` & `tmp/streamlit_nightly-1.34.1.dev20240516.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_nightly-1.34.1.dev20240514.tar", last modified: Wed May 15 11:51:50 2024, max compression
+gzip compressed data, was "streamlit_nightly-1.34.1.dev20240516.tar", last modified: Fri May 17 08:49:13 2024, max compression
```

## Comparing `streamlit_nightly-1.34.1.dev20240514.tar` & `streamlit_nightly-1.34.1.dev20240516.tar`

### file list

```diff
@@ -1,576 +1,574 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.319947 streamlit_nightly-1.34.1.dev20240514/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-15 11:51:50.319947 streamlit_nightly-1.34.1.dev20240514/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.195947 streamlit_nightly-1.34.1.dev20240514/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/bin/streamlit.cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:51:50.319947 streamlit_nightly-1.34.1.dev20240514/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.203947 streamlit_nightly-1.34.1.dev20240514/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/case_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/code_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/column_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.203947 streamlit_nightly-1.34.1.dev20240514/streamlit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/commands/execution_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/commands/experimental_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/commands/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/commands/page_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.203947 streamlit_nightly-1.34.1.dev20240514/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.207947 streamlit_nightly-1.34.1.dev20240514/streamlit/components/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/lib/local_component_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.207947 streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/base_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/base_custom_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.207947 streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/custom_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.207947 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/snowflake_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/snowpark_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/sql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/connections/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/delta_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/deprecation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/development.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/echo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.215947 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    23830 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/balloons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/dialog_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.215947 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/built_in_chart_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/column_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/mutable_status_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/pandas_styler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/subtitle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/map.py
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    15344 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    58273 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/vega_charts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.219947 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32860 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/camera_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/data_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/number_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/select_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/selectbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/text_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/time_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/elements/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/error_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.219947 streamlit_nightly-1.34.1.dev20240514/streamlit/external/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.219947 streamlit_nightly-1.34.1.dev20240514/streamlit/external/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/external/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/external/langchain/streamlit_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/folder_black_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/git_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.219947 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/Hello.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.219947 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/0_Animation_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/1_Plotting_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/2_Mapping_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/hello/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/js_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/material_icon_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/net_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.247947 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Alert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AppPage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowNamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Arrow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Audio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AutoRerun_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AutoRerun_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BackMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Balloons_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Block_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Block_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BokehChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Button_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Button_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/CameraInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ChatInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ChatInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Checkbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ClientState_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ColorPicker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Components_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DataFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DateInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DeckGlJsonChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Delta_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DocString_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DownloadButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Element_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Element_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Exception_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Favicon_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/FileUploader_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ForwardMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GitInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GraphVizChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Heading_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Heading_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Html_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Html_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/IFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Json_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Json_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LabelVisibilityMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LinkButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LinkButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Logo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Logo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Markdown_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Metric_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/MultiSelect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NewSession_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NumberInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageConfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageLink_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageLink_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageNotFound_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageProfile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageProfile_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PagesChanged_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ParentMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ParentMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PlotlyChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Progress_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Radio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/RootContainer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Selectbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionEvent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionStatus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Skeleton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Skeleton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Slider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Snow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Spinner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextArea_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Text_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TimeInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Toast_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Toast_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/VegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Video_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Video_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/WidgetStates_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/openmetrics_data_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-15 11:47:59.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/proto/openmetrics_data_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.251947 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36646 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.251947 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cached_message_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.251947 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/forward_msg_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/forward_msg_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.255947 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/media_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/memory_media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/memory_session_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/memory_uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/metrics_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29438 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.255947 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_run_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/session_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.255947 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/query_params_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/safe_session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/session_state_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/websocket_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/source_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.255947 streamlit_nightly-1.34.1.dev20240514/streamlit/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-15 11:48:28.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.195947 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.259947 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/3466.8b8f33d6.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/5441.e3b876c5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/8148.49dfd2ce.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/main.3aaaea00.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.291947 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1074.73973756.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1168.14f7c6ff.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1307.0f0cca93.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1451.3b0a3e31.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1479.6709db03.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/178.7bea8c5d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2178.90362aae.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2187.9469f035.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2469.09ea79bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2634.1249dc7a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2736.4336e2b9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3053.7e70ec3b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/329.464ed8ec.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3301.1d1b10bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3466.05d62820.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3513.7dedbda2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3631.be5c35fa.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4113.99983645.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4132.49bf3f2c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4177.69f9f18d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4319.bf1c86bf.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4477.1bd49702.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4500.b6f348d1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4666.c4b22a63.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/474.87506447.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5106.44f0ff51.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5117.04bfe5d3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5249.f2f4070d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5345.65c91ee7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5379.6571574f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5441.1b94928f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5791.9a42fb4b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6013.4ba2d616.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6405.ac5a6f23.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6718.802da17e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6853.93dd1c4c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   398809 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6950.70fe55c2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7142.83028745.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7175.be4076bc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7323.b74cc85b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7483.64f23be7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7602.e8abc06b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7805.acc6316a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8005.43974a35.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    50192 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8148.a5f74d47.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8477.de889fe5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8492.0d93bd08.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8536.f8de3d9a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8570.6de19120.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8691.9ccf7f89.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9330.2b4c99e0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9336.2d95d840.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/937.a1248039.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9656.8c935274.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9758.6e6d8662.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9865.fd93213d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  4405405 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/main.32c71338.js
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/main.32c71338.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.307947 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
--rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
--rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-15 11:51:47.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/temporary_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/element_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/local_script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    48389 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/ipython/modified_sys_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/pympler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/pympler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/pympler/asizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.311947 streamlit_nightly-1.34.1.dev20240514/streamlit/web/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/cache_storage_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.315947 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/app_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/browser_websocket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/component_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/media_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/stats_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/upload_file_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/websocket_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.315947 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-15 11:51:48.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-05-15 11:51:48.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:51:48.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 11:51:48.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:47:55.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-15 11:51:48.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 11:51:48.000000 streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:51:50.315947 streamlit_nightly-1.34.1.dev20240514/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-15 11:46:17.000000 streamlit_nightly-1.34.1.dev20240514/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.109273 streamlit_nightly-1.34.1.dev20240516/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-17 08:49:13.109273 streamlit_nightly-1.34.1.dev20240516/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:12.993273 streamlit_nightly-1.34.1.dev20240516/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/bin/streamlit.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:49:13.109273 streamlit_nightly-1.34.1.dev20240516/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:12.997273 streamlit_nightly-1.34.1.dev20240516/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/case_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/code_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/column_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.001273 streamlit_nightly-1.34.1.dev20240516/streamlit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/commands/execution_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/commands/experimental_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/commands/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/commands/page_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.001273 streamlit_nightly-1.34.1.dev20240516/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.001273 streamlit_nightly-1.34.1.dev20240516/streamlit/components/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/components/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/components/lib/local_component_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.001273 streamlit_nightly-1.34.1.dev20240516/streamlit/components/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/components/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/components/types/base_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/components/types/base_custom_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.001273 streamlit_nightly-1.34.1.dev20240516/streamlit/components/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/components/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/components/v1/component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/components/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/components/v1/custom_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.001273 streamlit_nightly-1.34.1.dev20240516/streamlit/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/connections/snowflake_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/connections/snowpark_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/connections/sql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/connections/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/delta_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/deprecation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.009273 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23830 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/dialog_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.009273 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/built_in_chart_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/column_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/mutable_status_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/pandas_styler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/subtitle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15344 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58273 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/vega_charts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.013273 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32860 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/camera_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/data_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/number_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/select_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/selectbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/text_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/time_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/elements/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/error_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.013273 streamlit_nightly-1.34.1.dev20240516/streamlit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.013273 streamlit_nightly-1.34.1.dev20240516/streamlit/external/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/external/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/external/langchain/streamlit_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/folder_black_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/git_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.013273 streamlit_nightly-1.34.1.dev20240516/streamlit/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/hello/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/hello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.013273 streamlit_nightly-1.34.1.dev20240516/streamlit/hello/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/hello/pages/0_Animation_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/hello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/js_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/material_icon_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/net_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.037273 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Alert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/AppPage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ArrowNamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Arrow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Audio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/AutoRerun_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/AutoRerun_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/BackMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Balloons_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Block_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/BokehChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Button_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/CameraInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ChatInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ChatInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Checkbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ClientState_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ColorPicker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Components_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DataFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DateInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DeckGlJsonChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Delta_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DocString_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DownloadButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Element_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Exception_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Favicon_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/FileUploader_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ForwardMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/GitInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/GraphVizChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Heading_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Heading_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Html_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Html_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/IFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Json_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/LabelVisibilityMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/LinkButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/LinkButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Logo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Logo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Markdown_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Metric_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/MultiSelect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/NamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/NewSession_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/NumberInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageConfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageLink_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageLink_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageNotFound_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageProfile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageProfile_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PagesChanged_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ParentMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ParentMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PlotlyChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Progress_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Radio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/RootContainer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Selectbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/SessionEvent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/SessionStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/SessionStatus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Skeleton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Skeleton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Slider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Snow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Spinner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/TextArea_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/TextInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Text_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/TimeInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Toast_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Toast_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/VegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Video_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/WidgetStates_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-17 08:45:34.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/proto/openmetrics_data_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.041273 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36646 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.041273 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/cache_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/cache_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/cache_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/cached_message_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.045273 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/forward_msg_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/forward_msg_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.045273 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/legacy_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/legacy_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/legacy_caching/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/legacy_caching/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/media_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/memory_media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/memory_session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/memory_uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/metrics_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29438 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.045273 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/script_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/script_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.045273 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/query_params_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/safe_session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/session_state_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/websocket_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/source_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.049273 streamlit_nightly-1.34.1.dev20240516/streamlit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-17 08:46:02.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:12.989273 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.049273 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/css/3466.8b8f33d6.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/css/5441.e3b876c5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/css/8148.49dfd2ce.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/css/main.3aaaea00.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.081273 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/1074.73973756.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/1168.14f7c6ff.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/1307.0f0cca93.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/1451.3b0a3e31.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/1479.6709db03.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/178.7bea8c5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/2178.90362aae.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/2187.9469f035.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/2469.09ea79bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/2634.1249dc7a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/2736.4336e2b9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/3053.7e70ec3b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/329.464ed8ec.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/3301.1d1b10bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/3466.05d62820.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/3513.7dedbda2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4113.99983645.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4132.49bf3f2c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4177.69f9f18d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4319.bf1c86bf.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4477.1bd49702.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4500.b6f348d1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4666.c4b22a63.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/474.7eb0c6cd.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5106.44f0ff51.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5117.04bfe5d3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5249.f2f4070d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5345.73d26e5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5379.6571574f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5441.1b94928f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5791.9a42fb4b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/6013.4ba2d616.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/6405.ac5a6f23.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/6718.802da17e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/6853.93dd1c4c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   398809 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/6950.70fe55c2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7142.83028745.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7175.be4076bc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7323.b74cc85b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7483.64f23be7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7602.e8abc06b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7805.acc6316a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8005.43974a35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    51109 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8148.f80eec24.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8477.de889fe5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8492.0d93bd08.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8536.f8de3d9a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8570.6de19120.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8691.9ccf7f89.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/9330.2b4c99e0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/9336.2d95d840.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/937.a1248039.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/9656.8c935274.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/9865.fd93213d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4405422 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/main.60ba1bc7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/main.60ba1bc7.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.101273 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-17 08:49:10.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/temporary_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.101273 streamlit_nightly-1.34.1.dev20240516/streamlit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.101273 streamlit_nightly-1.34.1.dev20240516/streamlit/testing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/testing/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/testing/v1/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/testing/v1/element_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/testing/v1/local_script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/testing/v1/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48389 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.101273 streamlit_nightly-1.34.1.dev20240516/streamlit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.101273 streamlit_nightly-1.34.1.dev20240516/streamlit/vendor/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/vendor/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/vendor/ipython/modified_sys_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.101273 streamlit_nightly-1.34.1.dev20240516/streamlit/vendor/pympler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/vendor/pympler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/vendor/pympler/asizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.101273 streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.101273 streamlit_nightly-1.34.1.dev20240516/streamlit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/cache_storage_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.105273 streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/app_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/browser_websocket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/component_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/media_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/stats_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/upload_file_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/websocket_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.105273 streamlit_nightly-1.34.1.dev20240516/streamlit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-17 08:49:11.000000 streamlit_nightly-1.34.1.dev20240516/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23316 2024-05-17 08:49:11.000000 streamlit_nightly-1.34.1.dev20240516/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:49:11.000000 streamlit_nightly-1.34.1.dev20240516/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-17 08:49:11.000000 streamlit_nightly-1.34.1.dev20240516/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:45:31.000000 streamlit_nightly-1.34.1.dev20240516/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 08:49:11.000000 streamlit_nightly-1.34.1.dev20240516/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 08:49:11.000000 streamlit_nightly-1.34.1.dev20240516/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:49:13.105273 streamlit_nightly-1.34.1.dev20240516/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-17 08:44:04.000000 streamlit_nightly-1.34.1.dev20240516/tests/testutil.py
```

### Comparing `streamlit_nightly-1.34.1.dev20240514/PKG-INFO` & `streamlit_nightly-1.34.1.dev20240516/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.34.1.dev20240514
+Version: 1.34.1.dev20240516
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.34.1.dev20240514/bin/streamlit.cmd` & `streamlit_nightly-1.34.1.dev20240516/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/setup.py` & `streamlit_nightly-1.34.1.dev20240516/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.34.1.dev20240514"  # PEP-440
+VERSION = "1.34.1.dev20240516"  # PEP-440
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible:
 # - Include relevant lower bound for any features we use from our dependencies
 # - Always include the lower bound as >= VERSION, to keep testing min versions easy
 # - And include an upper bound that's < NEXT_MAJOR_VERSION
 INSTALL_REQUIRES = [
```

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/__main__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/case_converters.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/cli_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/cli_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/code_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/color_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/color_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/column_config.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/column_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/commands/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/commands/execution_control.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/commands/execution_control.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/commands/experimental_query_params.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/commands/experimental_query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/commands/logo.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/commands/logo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/commands/page_config.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/components/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/components/lib/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/components/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/components/lib/local_component_registry.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/components/lib/local_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/base_component_registry.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/components/types/base_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/components/types/base_custom_component.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/components/types/base_custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/component_arrow.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/component_registry.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/components/v1/component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/components.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/components/v1/custom_component.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/components/v1/custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/config.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/config_option.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/config_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/connections/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/connections/base_connection.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/connections/snowflake_connection.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/connections/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/connections/snowpark_connection.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/connections/snowpark_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/connections/sql_connection.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/connections/sql_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/connections/util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/connections/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/constants.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/constants.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/cursor.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/delta_generator.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/delta_generator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/deprecation_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/development.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/echo.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/alert.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/arrow.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/balloons.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/bokeh_chart.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/code.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/deck_gl_json_chart.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/dialog_decorator.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/dialog_decorator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/doc_string.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/empty.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/empty.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/exception.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/form.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/form.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/graphviz_chart.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/heading.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/heading.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/html.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/html.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/iframe.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/image.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/image.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/json.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/layouts.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/built_in_chart_utils.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/built_in_chart_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/column_config_utils.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/column_config_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import copy
 import json
 from enum import Enum
 from typing import TYPE_CHECKING, Dict, Final, Literal, Mapping, Union
 
 from typing_extensions import TypeAlias
 
 from streamlit.elements.lib.column_types import ColumnConfig, ColumnType
@@ -423,15 +424,17 @@
     transformed_column_config: ColumnConfigMapping = {}
     for column, config in column_config.items():
         if config is None:
             transformed_column_config[column] = ColumnConfig(hidden=True)
         elif isinstance(config, str):
             transformed_column_config[column] = ColumnConfig(label=config)
         elif isinstance(config, dict):
-            transformed_column_config[column] = config
+            # Ensure that the column config objects are cloned
+            # since we will apply in-place changes to it.
+            transformed_column_config[column] = copy.deepcopy(config)
         else:
             raise StreamlitAPIException(
                 f"Invalid column config for column `{column}`. "
                 f"Expected `None`, `str` or `dict`, but got `{type(config)}`."
             )
     return transformed_column_config
```

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/column_types.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/column_types.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/dialog.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/dialog.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/dicttools.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/event_utils.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/event_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/mutable_status_container.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/mutable_status_container.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/pandas_styler_utils.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/pandas_styler_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/streamlit_plotly_theme.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/lib/subtitle_utils.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/lib/subtitle_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/map.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/markdown.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/media.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/media.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/metric.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/plotly_chart.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/progress.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/pyplot.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/snow.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/spinner.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/text.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/toast.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/toast.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/utils.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/vega_charts.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/vega_charts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/button.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/button.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/camera_input.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/camera_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/chat.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/checkbox.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/color_picker.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/color_picker.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/data_editor.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/data_editor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/file_uploader.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/file_uploader.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/multiselect.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/multiselect.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/number_input.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/number_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/radio.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/select_slider.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/select_slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/selectbox.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/selectbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/slider.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/text_widgets.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/text_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/widgets/time_widgets.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/widgets/time_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/elements/write.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/emojis.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/env_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/error_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/errors.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/external/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/external/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/external/langchain/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/external/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/external/langchain/streamlit_callback_handler.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/external/langchain/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/file_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/folder_black_list.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/git_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/Hello.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/0_Animation_Demo.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/1_Plotting_Demo.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/2_Mapping_Demo.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/pages/3_DataFrame_Demo.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/hello/utils.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/js_number.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/logger.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/material_icon_names.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/material_icon_names.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/net_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/platform.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/platform.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Alert_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Alert_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AppPage_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AppPage_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/AppPage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowNamedDataSet_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ArrowNamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ArrowVegaLiteChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ArrowVegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Arrow_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Arrow_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Arrow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Audio_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Audio_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Audio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AutoRerun_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/AutoRerun_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/AutoRerun_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/AutoRerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BackMsg_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BackMsg_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/BackMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Balloons_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Balloons_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Balloons_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Block_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Block_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BokehChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/BokehChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/BokehChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Button_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Button_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Button_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/CameraInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/CameraInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/CameraInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ChatInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ChatInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ChatInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ChatInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Checkbox_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Checkbox_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Checkbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ClientState_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ClientState_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ClientState_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Code_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Code_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ColorPicker_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ColorPicker_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ColorPicker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Common_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Common_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Components_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Components_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Components_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DataFrame_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DataFrame_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DataFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DateInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DateInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DateInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DeckGlJsonChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DeckGlJsonChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Delta_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Delta_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Delta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DocString_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DocString_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DocString_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DownloadButton_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/DownloadButton_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/DownloadButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Element_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Element_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Element_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Empty_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Empty_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Exception_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Exception_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Exception_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Favicon_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Favicon_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Favicon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/FileUploader_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/FileUploader_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/FileUploader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ForwardMsg_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ForwardMsg_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ForwardMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GitInfo_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GitInfo_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/GitInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GraphVizChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/GraphVizChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/GraphVizChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Heading_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Heading_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Heading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Html_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Html_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Html_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Html_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/IFrame_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/IFrame_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/IFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Image_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Image_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Json_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Json_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Json_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LabelVisibilityMessage_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LabelVisibilityMessage_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/LabelVisibilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LinkButton_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/LinkButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/LinkButton_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/LinkButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Logo_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Logo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Logo_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Logo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Markdown_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Markdown_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Markdown_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Metric_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Metric_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/MultiSelect_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/MultiSelect_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/MultiSelect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NamedDataSet_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NamedDataSet_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/NamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NewSession_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NewSession_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/NewSession_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NumberInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/NumberInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/NumberInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageConfig_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageConfig_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageConfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageInfo_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageInfo_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageLink_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageLink_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageLink_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageLink_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageNotFound_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageNotFound_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageNotFound_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageProfile_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PageProfile_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PageProfile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PagesChanged_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PagesChanged_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PagesChanged_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ParentMessage_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ParentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/ParentMessage_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/ParentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PlotlyChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/PlotlyChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/PlotlyChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Progress_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Progress_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Progress_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Radio_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Radio_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Radio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/RootContainer_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/RootContainer_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/RootContainer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Selectbox_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Selectbox_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Selectbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionEvent_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionEvent_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/SessionEvent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionStatus_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/SessionStatus_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/SessionStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Skeleton_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Skeleton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Skeleton_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Skeleton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Slider_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Slider_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Slider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Snow_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Snow_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Snow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Spinner_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Spinner_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Spinner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextArea_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextArea_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/TextArea_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TextInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/TextInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Text_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Text_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TimeInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/TimeInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/TimeInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Toast_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Toast_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Toast_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Toast_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/VegaLiteChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/VegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Video_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/Video_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/Video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/WidgetStates_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/WidgetStates_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/WidgetStates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/proto/openmetrics_data_model_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240516/streamlit/proto/openmetrics_data_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/app_session.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/app_session.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_data_api.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_errors.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_resource_api.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_type.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cache_utils.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/cached_message_replay.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/cached_message_replay.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/hashing.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/connection_factory.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/connection_factory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/credentials.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/forward_msg_cache.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/forward_msg_queue.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/fragment.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/fragment.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/legacy_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/caching.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/legacy_caching/caching.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/legacy_caching/hashing.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/legacy_caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/media_file_manager.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/media_file_storage.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/memory_media_file_storage.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/memory_session_storage.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/memory_uploaded_file_manager.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/memory_uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/metrics_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/metrics_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,10 +465,10 @@
     page_profile.timezone = str(time.tzname)
     page_profile.attributions.extend(attributions)
 
     if uncaught_exception:
         page_profile.uncaught_exception = uncaught_exception
 
     if ctx := get_script_run_ctx():
-        page_profile.is_fragment_run = bool(ctx.current_fragment_id)
+        page_profile.is_fragment_run = bool(ctx.fragment_ids_this_run)
 
     return msg
```

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/runtime.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/runtime_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/runtime_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/script_data.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/magic.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/magic_funcs.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_cache.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/script_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_requests.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_run_context.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/scriptrunner/script_runner.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/secrets.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/session_manager.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/common.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/common.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/query_params.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/query_params_proxy.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/query_params_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/safe_session_state.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/session_state.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/session_state_proxy.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/state/widgets.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/state/widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/stats.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/uploaded_file_manager.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/runtime/websocket_session_manager.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/source_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/asset-manifest.json` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/asset-manifest.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8194444444444444%*

 * *Differences: {"'entrypoints'": "{insert: [(1, 'static/js/main.60ba1bc7.js')], delete: [1]}",*

 * * "'files'": "{'main.js': './static/js/main.60ba1bc7.js', 'static/js/8148.f80eec24.chunk.js': "*

 * *            "'./static/js/8148.f80eec24.chunk.js', 'static/js/5345.73d26e5d.chunk.js': "*

 * *            "'./static/js/5345.73d26e5d.chunk.js', 'static/js/474.7eb0c6cd.chunk.js': "*

 * *            "'./static/js/474.7eb0c6cd.chunk.js', delete: ['static/js/8148.a5f74d47.chunk.js', "*

 * *            "'static/js/5345.65c91ee7.chunk.js', 'static/js/975 […]*

```diff
@@ -1,16 +1,16 @@
 {
     "entrypoints": [
         "static/css/main.3aaaea00.css",
-        "static/js/main.32c71338.js"
+        "static/js/main.60ba1bc7.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.3aaaea00.css",
-        "main.js": "./static/js/main.32c71338.js",
+        "main.js": "./static/js/main.60ba1bc7.js",
         "static/css/3466.8b8f33d6.chunk.css": "./static/css/3466.8b8f33d6.chunk.css",
         "static/css/5441.e3b876c5.chunk.css": "./static/css/5441.e3b876c5.chunk.css",
         "static/css/8148.49dfd2ce.chunk.css": "./static/css/8148.49dfd2ce.chunk.css",
         "static/js/1074.73973756.chunk.js": "./static/js/1074.73973756.chunk.js",
         "static/js/1168.14f7c6ff.chunk.js": "./static/js/1168.14f7c6ff.chunk.js",
         "static/js/1307.0f0cca93.chunk.js": "./static/js/1307.0f0cca93.chunk.js",
         "static/js/1451.3b0a3e31.chunk.js": "./static/js/1451.3b0a3e31.chunk.js",
@@ -23,27 +23,26 @@
         "static/js/2634.1249dc7a.chunk.js": "./static/js/2634.1249dc7a.chunk.js",
         "static/js/2736.4336e2b9.chunk.js": "./static/js/2736.4336e2b9.chunk.js",
         "static/js/3053.7e70ec3b.chunk.js": "./static/js/3053.7e70ec3b.chunk.js",
         "static/js/329.464ed8ec.chunk.js": "./static/js/329.464ed8ec.chunk.js",
         "static/js/3301.1d1b10bb.chunk.js": "./static/js/3301.1d1b10bb.chunk.js",
         "static/js/3466.05d62820.chunk.js": "./static/js/3466.05d62820.chunk.js",
         "static/js/3513.7dedbda2.chunk.js": "./static/js/3513.7dedbda2.chunk.js",
-        "static/js/3631.be5c35fa.chunk.js": "./static/js/3631.be5c35fa.chunk.js",
         "static/js/4113.99983645.chunk.js": "./static/js/4113.99983645.chunk.js",
         "static/js/4132.49bf3f2c.chunk.js": "./static/js/4132.49bf3f2c.chunk.js",
         "static/js/4177.69f9f18d.chunk.js": "./static/js/4177.69f9f18d.chunk.js",
         "static/js/4319.bf1c86bf.chunk.js": "./static/js/4319.bf1c86bf.chunk.js",
         "static/js/4477.1bd49702.chunk.js": "./static/js/4477.1bd49702.chunk.js",
         "static/js/4500.b6f348d1.chunk.js": "./static/js/4500.b6f348d1.chunk.js",
         "static/js/4666.c4b22a63.chunk.js": "./static/js/4666.c4b22a63.chunk.js",
-        "static/js/474.87506447.chunk.js": "./static/js/474.87506447.chunk.js",
+        "static/js/474.7eb0c6cd.chunk.js": "./static/js/474.7eb0c6cd.chunk.js",
         "static/js/5106.44f0ff51.chunk.js": "./static/js/5106.44f0ff51.chunk.js",
         "static/js/5117.04bfe5d3.chunk.js": "./static/js/5117.04bfe5d3.chunk.js",
         "static/js/5249.f2f4070d.chunk.js": "./static/js/5249.f2f4070d.chunk.js",
-        "static/js/5345.65c91ee7.chunk.js": "./static/js/5345.65c91ee7.chunk.js",
+        "static/js/5345.73d26e5d.chunk.js": "./static/js/5345.73d26e5d.chunk.js",
         "static/js/5379.6571574f.chunk.js": "./static/js/5379.6571574f.chunk.js",
         "static/js/5441.1b94928f.chunk.js": "./static/js/5441.1b94928f.chunk.js",
         "static/js/5791.9a42fb4b.chunk.js": "./static/js/5791.9a42fb4b.chunk.js",
         "static/js/6013.4ba2d616.chunk.js": "./static/js/6013.4ba2d616.chunk.js",
         "static/js/6405.ac5a6f23.chunk.js": "./static/js/6405.ac5a6f23.chunk.js",
         "static/js/6718.802da17e.chunk.js": "./static/js/6718.802da17e.chunk.js",
         "static/js/6853.93dd1c4c.chunk.js": "./static/js/6853.93dd1c4c.chunk.js",
@@ -51,26 +50,25 @@
         "static/js/7142.83028745.chunk.js": "./static/js/7142.83028745.chunk.js",
         "static/js/7175.be4076bc.chunk.js": "./static/js/7175.be4076bc.chunk.js",
         "static/js/7323.b74cc85b.chunk.js": "./static/js/7323.b74cc85b.chunk.js",
         "static/js/7483.64f23be7.chunk.js": "./static/js/7483.64f23be7.chunk.js",
         "static/js/7602.e8abc06b.chunk.js": "./static/js/7602.e8abc06b.chunk.js",
         "static/js/7805.acc6316a.chunk.js": "./static/js/7805.acc6316a.chunk.js",
         "static/js/8005.43974a35.chunk.js": "./static/js/8005.43974a35.chunk.js",
-        "static/js/8148.a5f74d47.chunk.js": "./static/js/8148.a5f74d47.chunk.js",
+        "static/js/8148.f80eec24.chunk.js": "./static/js/8148.f80eec24.chunk.js",
         "static/js/8427.bd0a7cf3.chunk.js": "./static/js/8427.bd0a7cf3.chunk.js",
         "static/js/8477.de889fe5.chunk.js": "./static/js/8477.de889fe5.chunk.js",
         "static/js/8492.0d93bd08.chunk.js": "./static/js/8492.0d93bd08.chunk.js",
         "static/js/8536.f8de3d9a.chunk.js": "./static/js/8536.f8de3d9a.chunk.js",
         "static/js/8570.6de19120.chunk.js": "./static/js/8570.6de19120.chunk.js",
         "static/js/8691.9ccf7f89.chunk.js": "./static/js/8691.9ccf7f89.chunk.js",
         "static/js/9330.2b4c99e0.chunk.js": "./static/js/9330.2b4c99e0.chunk.js",
         "static/js/9336.2d95d840.chunk.js": "./static/js/9336.2d95d840.chunk.js",
         "static/js/937.a1248039.chunk.js": "./static/js/937.a1248039.chunk.js",
         "static/js/9656.8c935274.chunk.js": "./static/js/9656.8c935274.chunk.js",
-        "static/js/9758.6e6d8662.chunk.js": "./static/js/9758.6e6d8662.chunk.js",
         "static/js/9865.fd93213d.chunk.js": "./static/js/9865.fd93213d.chunk.js",
         "static/media/KaTeX_AMS-Regular.ttf": "./static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf",
         "static/media/KaTeX_AMS-Regular.woff": "./static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff",
         "static/media/KaTeX_AMS-Regular.woff2": "./static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2",
         "static/media/KaTeX_Caligraphic-Bold.ttf": "./static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf",
         "static/media/KaTeX_Caligraphic-Bold.woff": "./static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff",
         "static/media/KaTeX_Caligraphic-Bold.woff2": "./static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2",
```

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/favicon.png` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/index.html` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.32c71338.js"></script><link href="./static/css/main.3aaaea00.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.60ba1bc7.js"></script><link href="./static/css/main.3aaaea00.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/3466.8b8f33d6.chunk.css` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/css/3466.8b8f33d6.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/5441.e3b876c5.chunk.css` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/css/5441.e3b876c5.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/8148.49dfd2ce.chunk.css` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/css/8148.49dfd2ce.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/css/main.3aaaea00.css` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/css/main.3aaaea00.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1074.73973756.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/1074.73973756.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1168.14f7c6ff.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/1168.14f7c6ff.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1307.0f0cca93.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/1307.0f0cca93.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1451.3b0a3e31.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/1451.3b0a3e31.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1479.6709db03.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/1479.6709db03.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/178.7bea8c5d.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/178.7bea8c5d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/1792.8bd6ce2a.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/1792.8bd6ce2a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2178.90362aae.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/2178.90362aae.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2187.9469f035.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/2187.9469f035.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2469.09ea79bb.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/2469.09ea79bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2634.1249dc7a.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/2634.1249dc7a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/2736.4336e2b9.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/2736.4336e2b9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3053.7e70ec3b.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/3053.7e70ec3b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/329.464ed8ec.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/329.464ed8ec.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3301.1d1b10bb.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/3301.1d1b10bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3466.05d62820.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/3466.05d62820.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/3513.7dedbda2.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/3513.7dedbda2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4113.99983645.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4113.99983645.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4132.49bf3f2c.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4132.49bf3f2c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4177.69f9f18d.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4177.69f9f18d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4319.bf1c86bf.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4319.bf1c86bf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4477.1bd49702.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4477.1bd49702.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4500.b6f348d1.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4500.b6f348d1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/4666.c4b22a63.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/4666.c4b22a63.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5106.44f0ff51.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5106.44f0ff51.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5117.04bfe5d3.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5117.04bfe5d3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5249.f2f4070d.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5249.f2f4070d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5379.6571574f.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5379.6571574f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5441.1b94928f.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5441.1b94928f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/5791.9a42fb4b.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/5791.9a42fb4b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6013.4ba2d616.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/6013.4ba2d616.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6405.ac5a6f23.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/6405.ac5a6f23.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6718.802da17e.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/6718.802da17e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6853.93dd1c4c.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/6853.93dd1c4c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/6950.70fe55c2.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/6950.70fe55c2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7142.83028745.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7142.83028745.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7175.be4076bc.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7175.be4076bc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7323.b74cc85b.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7323.b74cc85b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7483.64f23be7.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7483.64f23be7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7602.e8abc06b.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7602.e8abc06b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/7805.acc6316a.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/7805.acc6316a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8005.43974a35.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8005.43974a35.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8148.a5f74d47.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8148.f80eec24.chunk.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -204,15 +204,15 @@
                     }
                 }
                 return n.displayName = "withFullScreenWrapper(".concat(e.displayName || e.name, ")"), l()(n, e)
             }
         },
         75064: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => Ot
+                default: () => Ft
             });
             var i = n(66845),
                 o = n(67930),
                 l = n(78170),
                 r = n(17330),
                 a = n(20545),
                 s = n(57463),
@@ -227,17 +227,17 @@
                 b = n(34367),
                 v = n(31011),
                 y = n(63730),
                 w = n(68411),
                 x = n(9003),
                 C = n(81354),
                 E = n(46927),
-                M = n(1515),
-                S = n(27466);
-            const T = (0, M.Z)("div", {
+                S = n(1515),
+                M = n(27466);
+            const k = (0, S.Z)("div", {
                     target: "e2wxzia1"
                 })((e => {
                     let {
                         theme: t,
                         locked: n,
                         target: i
                     } = e;
@@ -260,22 +260,22 @@
                                     opacity: 1,
                                     top: "-2.4rem"
                                 }
                             }
                         }
                     }
                 }), ""),
-                k = (0, M.Z)("div", {
+                T = (0, S.Z)("div", {
                     target: "e2wxzia0"
                 })((e => {
                     let {
                         theme: t
                     } = e;
                     return {
-                        color: (0, S.Iy)(t) ? t.colors.fadedText60 : t.colors.bodyText,
+                        color: (0, M.Iy)(t) ? t.colors.fadedText60 : t.colors.bodyText,
                         display: "flex",
                         flexDirection: "row",
                         alignItems: "center",
                         justifyContent: "flex-end",
                         boxShadow: "1px 2px 8px rgba(0, 0, 0, 0.08)",
                         borderRadius: t.radii.lg,
                         backgroundColor: t.colors.lightenedBg05,
@@ -329,89 +329,90 @@
                     onCollapse: n,
                     isFullScreen: i,
                     locked: o,
                     children: l,
                     target: r,
                     disableFullscreenMode: a
                 } = e;
-                return (0, R.jsx)(T, {
+                return (0, R.jsx)(k, {
                     className: "stElementToolbar",
                     "data-testid": "stElementToolbar",
                     locked: o || i,
                     target: r,
-                    children: (0, R.jsxs)(k, {
+                    children: (0, R.jsxs)(T, {
                         children: [l, t && !a && !i && (0, R.jsx)(N, {
                             label: "Fullscreen",
                             icon: b.i,
                             onClick: () => t()
                         }), n && !a && i && (0, R.jsx)(N, {
                             label: "Close fullscreen",
                             icon: v.m,
                             onClick: () => n()
                         })]
                     })
                 })
             };
-            var _ = n(38145),
-                O = n.n(_),
-                D = n(96825),
-                F = n.n(D),
-                A = n(29724),
-                z = n.n(A),
-                V = n(52347),
-                H = n(53608),
-                L = n.n(H),
-                W = (n(87717), n(55842), n(91191));
-            const j = ["true", "t", "yes", "y", "on", "1"],
-                B = ["false", "f", "no", "n", "off", "0"];
+            var _ = n(66694),
+                O = n(38145),
+                D = n.n(O),
+                A = n(96825),
+                F = n.n(A),
+                z = n(29724),
+                V = n.n(z),
+                H = n(52347),
+                L = n(53608),
+                W = n.n(L),
+                j = (n(87717), n(55842), n(91191));
+            const B = ["true", "t", "yes", "y", "on", "1"],
+                P = ["false", "f", "no", "n", "off", "0"];
 
-            function P(e) {
+            function Z(e) {
                 let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "";
                 return e = "\u26a0\ufe0f ".concat(e), {
                     kind: o.p6.Text,
                     readonly: !0,
                     allowOverlay: !0,
                     data: e + (t ? "\n\n".concat(t, "\n") : ""),
                     displayData: e,
                     isError: !0
                 }
             }
 
-            function Z(e) {
+            function Y(e) {
                 return e.hasOwnProperty("isError") && e.isError
             }
 
-            function Y(e) {
+            function U(e) {
                 return e.hasOwnProperty("isMissingValue") && e.isMissingValue
             }
 
-            function U() {
+            function q() {
                 return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? {
                     kind: o.p6.Loading,
                     allowOverlay: !1,
                     isMissingValue: !0
                 } : {
                     kind: o.p6.Loading,
                     allowOverlay: !1
                 }
             }
 
-            function q(e, t) {
+            function J(e, t) {
                 const n = t ? "faded" : "normal";
                 return {
                     kind: o.p6.Text,
                     data: "",
                     displayData: "",
                     allowOverlay: !0,
                     readonly: e,
                     style: n
                 }
             }
 
-            function J(e) {
+            function K(e) {
                 return {
                     id: e.id,
                     title: e.title,
                     hasMenu: !1,
                     themeOverride: e.themeOverride,
                     icon: e.icon,
                     ...e.isStretched && {
@@ -419,126 +420,126 @@
                     },
                     ...e.width && {
                         width: e.width
                     }
                 }
             }
 
-            function K(e, t) {
+            function G(e, t) {
                 return (0, g.le)(e) ? t || {} : (0, g.le)(t) ? e || {} : F()(e, t)
             }
 
-            function G(e) {
+            function X(e) {
                 if ((0, g.le)(e)) return [];
                 if ("number" === typeof e || "boolean" === typeof e) return [e];
                 if ("string" === typeof e) {
                     if ("" === e) return [];
                     if (!e.trim().startsWith("[") || !e.trim().endsWith("]")) return e.split(",");
                     try {
                         return JSON.parse(e)
                     } catch (t) {
                         return [e]
                     }
                 }
                 try {
                     const t = JSON.parse(JSON.stringify(e, ((e, t) => "bigint" === typeof t ? Number(t) : t)));
-                    return Array.isArray(t) ? t.map((e => ["string", "number", "boolean", "null"].includes(typeof e) ? e : X(e))) : [X(t)]
+                    return Array.isArray(t) ? t.map((e => ["string", "number", "boolean", "null"].includes(typeof e) ? e : Q(e))) : [Q(t)]
                 } catch (t) {
-                    return [X(e)]
+                    return [Q(e)]
                 }
             }
 
-            function X(e) {
+            function Q(e) {
                 try {
                     try {
-                        return O()(e)
+                        return D()(e)
                     } catch (t) {
                         return JSON.stringify(e, ((e, t) => "bigint" === typeof t ? Number(t) : t))
                     }
                 } catch (t) {
                     return "[".concat(typeof e, "]")
                 }
             }
 
-            function Q(e) {
+            function $(e) {
                 if ((0, g.le)(e)) return null;
                 if ("boolean" === typeof e) return e;
-                const t = X(e).toLowerCase().trim();
-                return "" === t ? null : !!j.includes(t) || !B.includes(t) && void 0
+                const t = Q(e).toLowerCase().trim();
+                return "" === t ? null : !!B.includes(t) || !P.includes(t) && void 0
             }
 
-            function $(e) {
+            function ee(e) {
                 if ((0, g.le)(e)) return null;
                 if (Array.isArray(e)) return NaN;
                 if ("string" === typeof e) {
                     if (0 === e.trim().length) return null;
                     try {
-                        const t = z().unformat(e.trim());
+                        const t = V().unformat(e.trim());
                         if ((0, g.bb)(t)) return t
                     } catch (t) {}
                 } else if (e instanceof Int32Array) return Number(e[0]);
                 return Number(e)
             }
 
-            function ee(e, t, n) {
-                return Number.isNaN(e) || !Number.isFinite(e) ? "" : (0, g.le)(t) || "" === t ? (0 === n && (e = Math.round(e)), z()(e).format((0, g.bb)(n) ? "0,0.".concat("0".repeat(n)) : "0,0.[0000]")) : "percent" === t ? new Intl.NumberFormat(void 0, {
+            function te(e, t, n) {
+                return Number.isNaN(e) || !Number.isFinite(e) ? "" : (0, g.le)(t) || "" === t ? (0 === n && (e = Math.round(e)), V()(e).format((0, g.bb)(n) ? "0,0.".concat("0".repeat(n)) : "0,0.[0000]")) : "percent" === t ? new Intl.NumberFormat(void 0, {
                     style: "percent",
                     minimumFractionDigits: 2,
                     maximumFractionDigits: 2
                 }).format(e) : ["compact", "scientific", "engineering"].includes(t) ? new Intl.NumberFormat(void 0, {
                     notation: t
-                }).format(e) : "duration[ns]" === t ? L().duration(e / 1e6, "milliseconds").humanize() : t.startsWith("period[") ? W.fu.formatPeriodType(BigInt(e), t) : (0, V.sprintf)(t, e)
+                }).format(e) : "duration[ns]" === t ? W().duration(e / 1e6, "milliseconds").humanize() : t.startsWith("period[") ? j.fu.formatPeriodType(BigInt(e), t) : (0, H.sprintf)(t, e)
             }
 
-            function te(e, t) {
+            function ne(e, t) {
                 return "locale" === t ? new Intl.DateTimeFormat(void 0, {
                     dateStyle: "medium",
                     timeStyle: "medium"
                 }).format(e.toDate()) : "distance" === t ? e.fromNow() : "relative" === t ? e.calendar() : e.format(t)
             }
 
-            function ne(e) {
+            function ie(e) {
                 if ((0, g.le)(e)) return null;
                 if (e instanceof Date) return isNaN(e.getTime()) ? void 0 : e;
                 if ("string" === typeof e && 0 === e.trim().length) return null;
                 try {
                     const t = Number(e);
                     if (!isNaN(t)) {
                         let e = t;
                         t >= 10 ** 18 ? e = t / 1e3 ** 3 : t >= 10 ** 15 ? e = t / 1e6 : t >= 10 ** 12 && (e = t / 1e3);
-                        const n = L().unix(e).utc();
+                        const n = W().unix(e).utc();
                         if (n.isValid()) return n.toDate()
                     }
                     if ("string" === typeof e) {
-                        const t = L().utc(e);
+                        const t = W().utc(e);
                         if (t.isValid()) return t.toDate();
-                        const n = L().utc(e, [L().HTML5_FMT.TIME_MS, L().HTML5_FMT.TIME_SECONDS, L().HTML5_FMT.TIME]);
+                        const n = W().utc(e, [W().HTML5_FMT.TIME_MS, W().HTML5_FMT.TIME_SECONDS, W().HTML5_FMT.TIME]);
                         if (n.isValid()) return n.toDate()
                     }
                 } catch (t) {
                     return
                 }
             }
 
-            function ie(e) {
+            function oe(e) {
                 if (e % 1 === 0) return 0;
                 let t = e.toString();
                 return -1 !== t.indexOf("e") && (t = e.toLocaleString("fullwide", {
                     useGrouping: !1,
                     maximumFractionDigits: 20
                 })), -1 === t.indexOf(".") ? 0 : t.split(".")[1].length
             }
-            const oe = new RegExp(/(\r\n|\n|\r)/gm);
+            const le = new RegExp(/(\r\n|\n|\r)/gm);
 
-            function le(e) {
-                return -1 !== e.indexOf("\n") ? e.replace(oe, " ") : e
+            function re(e) {
+                return -1 !== e.indexOf("\n") ? e.replace(le, " ") : e
             }
-            var re = n(23849);
+            var ae = n(23849);
 
-            function ae(e) {
+            function se(e) {
                 const t = {
                     kind: o.p6.Text,
                     data: "",
                     displayData: "",
                     allowOverlay: !0,
                     contentAlignment: e.contentAlignment,
                     readonly: !0,
@@ -547,33 +548,33 @@
                 return {
                     ...e,
                     kind: "object",
                     sortMode: "default",
                     isEditable: !1,
                     getCell(e) {
                         try {
-                            const n = (0, g.bb)(e) ? X(e) : null,
-                                i = (0, g.bb)(n) ? le(n) : "";
+                            const n = (0, g.bb)(e) ? Q(e) : null,
+                                i = (0, g.bb)(n) ? re(n) : "";
                             return {
                                 ...t,
                                 data: n,
                                 displayData: i,
                                 isMissingValue: (0, g.le)(e)
                             }
                         } catch (n) {
-                            return P(X(e), "The value cannot be interpreted as a string. Error: ".concat(n))
+                            return Z(Q(e), "The value cannot be interpreted as a string. Error: ".concat(n))
                         }
                     },
                     getCellValue: e => void 0 === e.data ? null : e.data
                 }
             }
-            ae.isEditableType = !1;
-            const se = ae;
+            se.isEditableType = !1;
+            const de = se;
 
-            function de(e) {
+            function ce(e) {
                 const t = e.columnTypeOptions || {};
                 let n;
                 if (t.validate) try {
                     n = new RegExp(t.validate, "us")
                 } catch (r) {
                     n = "Invalid validate regex: ".concat(t.validate, ".\nError: ").concat(r)
                 }
@@ -584,65 +585,65 @@
                         allowOverlay: !0,
                         contentAlignment: e.contentAlignment,
                         readonly: !e.isEditable,
                         style: e.isIndex ? "faded" : "normal"
                     },
                     l = i => {
                         if ((0, g.le)(i)) return !e.isRequired;
-                        let o = X(i),
+                        let o = Q(i),
                             l = !1;
                         return t.max_chars && o.length > t.max_chars && (o = o.slice(0, t.max_chars), l = !0), !(n instanceof RegExp && !1 === n.test(o)) && (!l || o)
                     };
                 return {
                     ...e,
                     kind: "text",
                     sortMode: "default",
                     validateInput: l,
                     getCell(e, t) {
-                        if ("string" === typeof n) return P(X(e), n);
+                        if ("string" === typeof n) return Z(Q(e), n);
                         if (t) {
                             const t = l(e);
-                            if (!1 === t) return P(X(e), "Invalid input.");
+                            if (!1 === t) return Z(Q(e), "Invalid input.");
                             "string" === typeof t && (e = t)
                         }
                         try {
-                            const t = (0, g.bb)(e) ? X(e) : null,
-                                n = (0, g.bb)(t) ? le(t) : "";
+                            const t = (0, g.bb)(e) ? Q(e) : null,
+                                n = (0, g.bb)(t) ? re(t) : "";
                             return {
                                 ...i,
                                 isMissingValue: (0, g.le)(t),
                                 data: t,
                                 displayData: n
                             }
                         } catch (r) {
-                            return P("Incompatible value", "The value cannot be interpreted as string. Error: ".concat(r))
+                            return Z("Incompatible value", "The value cannot be interpreted as string. Error: ".concat(r))
                         }
                     },
                     getCellValue: e => void 0 === e.data ? null : e.data
                 }
             }
-            de.isEditableType = !0;
-            const ce = de;
+            ce.isEditableType = !0;
+            const ue = ce;
 
-            function ue(e, t) {
+            function me(e, t) {
                 return e = t.startsWith("+") || t.startsWith("-") ? e.utcOffset(t, !1) : e.tz(t)
             }
 
-            function me(e, t, n, i, l, r, a) {
+            function he(e, t, n, i, l, r, a) {
                 var s;
-                const d = K({
+                const d = G({
                     format: n,
                     step: i,
                     timezone: a
                 }, t.columnTypeOptions);
                 let c, u, m;
                 if ((0, g.bb)(d.timezone)) try {
                     var h;
-                    c = (null === (h = ue(L()(), d.timezone)) || void 0 === h ? void 0 : h.utcOffset()) || void 0
-                } catch (b) {}(0, g.bb)(d.min_value) && (u = ne(d.min_value) || void 0), (0, g.bb)(d.max_value) && (m = ne(d.max_value) || void 0);
+                    c = (null === (h = me(W()(), d.timezone)) || void 0 === h ? void 0 : h.utcOffset()) || void 0
+                } catch (b) {}(0, g.bb)(d.min_value) && (u = ie(d.min_value) || void 0), (0, g.bb)(d.max_value) && (m = ie(d.max_value) || void 0);
                 const p = {
                         kind: o.p6.Custom,
                         allowOverlay: !0,
                         copyData: "",
                         readonly: !t.isEditable,
                         contentAlign: t.contentAlignment,
                         style: t.isIndex ? "faded" : "normal",
@@ -653,50 +654,50 @@
                             step: (null === (s = d.step) || void 0 === s ? void 0 : s.toString()) || "1",
                             format: l,
                             min: u,
                             max: m
                         }
                     },
                     f = e => {
-                        const n = ne(e);
+                        const n = ie(e);
                         return null === n ? !t.isRequired : void 0 !== n && (!((0, g.bb)(u) && r(n) < r(u)) && !((0, g.bb)(m) && r(n) > r(m)))
                     };
                 return {
                     ...t,
                     kind: e,
                     sortMode: "default",
                     validateInput: f,
                     getCell(e, t) {
                         if (!0 === t) {
                             const t = f(e);
-                            if (!1 === t) return P(X(e), "Invalid input.");
+                            if (!1 === t) return Z(Q(e), "Invalid input.");
                             t instanceof Date && (e = t)
                         }
-                        const i = ne(e);
+                        const i = ie(e);
                         let o = "",
                             l = "",
                             r = c;
-                        if (void 0 === i) return P(X(e), "The value cannot be interpreted as a datetime object.");
+                        if (void 0 === i) return Z(Q(e), "The value cannot be interpreted as a datetime object.");
                         if (null !== i) {
-                            let e = L().utc(i);
-                            if (!e.isValid()) return P(X(i), "This should never happen. Please report this bug. \nError: ".concat(e.toString()));
+                            let e = W().utc(i);
+                            if (!e.isValid()) return Z(Q(i), "This should never happen. Please report this bug. \nError: ".concat(e.toString()));
                             if (d.timezone) {
                                 try {
-                                    e = ue(e, d.timezone)
+                                    e = me(e, d.timezone)
                                 } catch (b) {
-                                    return P(e.toISOString(), "Failed to adjust to the provided timezone: ".concat(d.timezone, ". \nError: ").concat(b))
+                                    return Z(e.toISOString(), "Failed to adjust to the provided timezone: ".concat(d.timezone, ". \nError: ").concat(b))
                                 }
                                 r = e.utcOffset()
                             }
                             try {
-                                l = te(e, d.format || n)
+                                l = ne(e, d.format || n)
                             } catch (b) {
-                                return P(e.toISOString(), "Failed to format the date for rendering with: ".concat(d.format, ". \nError: ").concat(b))
+                                return Z(e.toISOString(), "Failed to format the date for rendering with: ".concat(d.format, ". \nError: ").concat(b))
                             }
-                            o = te(e, n)
+                            o = ne(e, n)
                         }
                         return {
                             ...p,
                             copyData: o,
                             isMissingValue: (0, g.le)(i),
                             data: {
                                 ...p.data,
@@ -709,232 +710,232 @@
                     getCellValue(e) {
                         var t;
                         return (0, g.le)(null === e || void 0 === e || null === (t = e.data) || void 0 === t ? void 0 : t.date) ? null : r(e.data.date)
                     }
                 }
             }
 
-            function he(e) {
+            function pe(e) {
                 var t, n, i, o, l;
                 let r = "YYYY-MM-DD HH:mm:ss";
                 (null === (t = e.columnTypeOptions) || void 0 === t ? void 0 : t.step) >= 60 ? r = "YYYY-MM-DD HH:mm" : (null === (n = e.columnTypeOptions) || void 0 === n ? void 0 : n.step) < 1 && (r = "YYYY-MM-DD HH:mm:ss.SSS");
                 const a = null === (i = e.arrowType) || void 0 === i || null === (o = i.meta) || void 0 === o ? void 0 : o.timezone,
                     s = (0, g.bb)(a) || (0, g.bb)(null === e || void 0 === e || null === (l = e.columnTypeOptions) || void 0 === l ? void 0 : l.timezone);
-                return me("datetime", e, s ? r + "Z" : r, 1, "datetime-local", (e => s ? e.toISOString() : e.toISOString().replace("Z", "")), a)
+                return he("datetime", e, s ? r + "Z" : r, 1, "datetime-local", (e => s ? e.toISOString() : e.toISOString().replace("Z", "")), a)
             }
 
-            function pe(e) {
+            function ge(e) {
                 var t, n;
                 let i = "HH:mm:ss";
-                return (null === (t = e.columnTypeOptions) || void 0 === t ? void 0 : t.step) >= 60 ? i = "HH:mm" : (null === (n = e.columnTypeOptions) || void 0 === n ? void 0 : n.step) < 1 && (i = "HH:mm:ss.SSS"), me("time", e, i, 1, "time", (e => e.toISOString().split("T")[1].replace("Z", "")))
+                return (null === (t = e.columnTypeOptions) || void 0 === t ? void 0 : t.step) >= 60 ? i = "HH:mm" : (null === (n = e.columnTypeOptions) || void 0 === n ? void 0 : n.step) < 1 && (i = "HH:mm:ss.SSS"), he("time", e, i, 1, "time", (e => e.toISOString().split("T")[1].replace("Z", "")))
             }
 
-            function ge(e) {
-                return me("date", e, "YYYY-MM-DD", 1, "date", (e => e.toISOString().split("T")[0]))
+            function fe(e) {
+                return he("date", e, "YYYY-MM-DD", 1, "date", (e => e.toISOString().split("T")[0]))
             }
 
-            function fe(e) {
+            function be(e) {
                 const t = {
                     kind: o.p6.Boolean,
                     data: !1,
                     allowOverlay: !1,
                     contentAlign: e.contentAlignment,
                     readonly: !e.isEditable,
                     style: e.isIndex ? "faded" : "normal"
                 };
                 return {
                     ...e,
                     kind: "checkbox",
                     sortMode: "default",
                     getCell(e) {
                         let n = null;
-                        return n = Q(e), void 0 === n ? P(X(e), "The value cannot be interpreted as boolean.") : {
+                        return n = $(e), void 0 === n ? Z(Q(e), "The value cannot be interpreted as boolean.") : {
                             ...t,
                             data: n,
                             isMissingValue: (0, g.le)(n)
                         }
                     },
                     getCellValue: e => void 0 === e.data ? null : e.data
                 }
             }
-            he.isEditableType = !0, pe.isEditableType = !0, ge.isEditableType = !0, fe.isEditableType = !0;
-            const be = fe;
+            pe.isEditableType = !0, ge.isEditableType = !0, fe.isEditableType = !0, be.isEditableType = !0;
+            const ve = be;
 
-            function ve(e) {
+            function ye(e) {
                 return e.startsWith("int") && !e.startsWith("interval") || "range" === e || e.startsWith("uint")
             }
 
-            function ye(e) {
-                const t = W.fu.getTypeName(e.arrowType);
+            function we(e) {
+                const t = j.fu.getTypeName(e.arrowType);
                 let n;
                 "timedelta64[ns]" === t ? n = "duration[ns]" : t.startsWith("period[") && (n = t);
-                const i = K({
-                        step: ve(t) ? 1 : void 0,
+                const i = G({
+                        step: ye(t) ? 1 : void 0,
                         min_value: t.startsWith("uint") ? 0 : void 0,
                         format: n
                     }, e.columnTypeOptions),
                     l = (0, g.le)(i.min_value) || i.min_value < 0,
-                    r = (0, g.bb)(i.step) && !Number.isNaN(i.step) ? ie(i.step) : void 0,
+                    r = (0, g.bb)(i.step) && !Number.isNaN(i.step) ? oe(i.step) : void 0,
                     a = {
                         kind: o.p6.Number,
                         data: void 0,
                         displayData: "",
                         readonly: !e.isEditable,
                         allowOverlay: !0,
                         contentAlign: e.contentAlignment || "right",
                         style: e.isIndex ? "faded" : "normal",
                         allowNegative: l,
                         fixedDecimals: r
                     },
                     s = t => {
-                        let n = $(t);
+                        let n = ee(t);
                         if ((0, g.le)(n)) return !e.isRequired;
                         if (Number.isNaN(n)) return !1;
                         let o = !1;
                         return (0, g.bb)(i.max_value) && n > i.max_value && (n = i.max_value, o = !0), !((0, g.bb)(i.min_value) && n < i.min_value) && (!o || n)
                     };
                 return {
                     ...e,
                     kind: "number",
                     sortMode: "smart",
                     validateInput: s,
                     getCell(e, t) {
                         if (!0 === t) {
                             const t = s(e);
-                            if (!1 === t) return P(X(e), "Invalid input.");
+                            if (!1 === t) return Z(Q(e), "Invalid input.");
                             "number" === typeof t && (e = t)
                         }
-                        let n = $(e),
+                        let n = ee(e),
                             o = "";
                         if ((0, g.bb)(n)) {
-                            if (Number.isNaN(n)) return P(X(e), "The value cannot be interpreted as a number.");
-                            if ((0, g.bb)(r) && (l = n, n = 0 === (d = r) ? Math.trunc(l) : Math.trunc(l * 10 ** d) / 10 ** d), Number.isInteger(n) && !Number.isSafeInteger(n)) return P(X(e), "The value is larger than the maximum supported integer values in number columns (2^53).");
+                            if (Number.isNaN(n)) return Z(Q(e), "The value cannot be interpreted as a number.");
+                            if ((0, g.bb)(r) && (l = n, n = 0 === (d = r) ? Math.trunc(l) : Math.trunc(l * 10 ** d) / 10 ** d), Number.isInteger(n) && !Number.isSafeInteger(n)) return Z(Q(e), "The value is larger than the maximum supported integer values in number columns (2^53).");
                             try {
-                                o = ee(n, i.format, r)
+                                o = te(n, i.format, r)
                             } catch (c) {
-                                return P(X(n), (0, g.bb)(i.format) ? "Failed to format the number based on the provided format configuration: (".concat(i.format, "). Error: ").concat(c) : "Failed to format the number. Error: ".concat(c))
+                                return Z(Q(n), (0, g.bb)(i.format) ? "Failed to format the number based on the provided format configuration: (".concat(i.format, "). Error: ").concat(c) : "Failed to format the number. Error: ".concat(c))
                             }
                         }
                         var l, d;
                         return {
                             ...a,
                             data: n,
                             displayData: o,
                             isMissingValue: (0, g.le)(n)
                         }
                     },
                     getCellValue: e => void 0 === e.data ? null : e.data
                 }
             }
-            ye.isEditableType = !0;
-            const we = ye;
+            we.isEditableType = !0;
+            const xe = we;
 
-            function xe(e) {
+            function Ce(e) {
                 let t = "string";
-                const n = K({
-                        options: "bool" === W.fu.getTypeName(e.arrowType) ? [!0, !1] : []
+                const n = G({
+                        options: "bool" === j.fu.getTypeName(e.arrowType) ? [!0, !1] : []
                     }, e.columnTypeOptions),
                     i = new Set(n.options.map((e => typeof e)));
                 1 === i.size && (i.has("number") || i.has("bigint") ? t = "number" : i.has("boolean") && (t = "boolean"));
                 const l = {
                     kind: o.p6.Custom,
                     allowOverlay: !0,
                     copyData: "",
                     contentAlign: e.contentAlignment,
                     readonly: !e.isEditable,
                     data: {
                         kind: "dropdown-cell",
-                        allowedValues: [...!0 !== e.isRequired ? [null] : [], ...n.options.filter((e => null !== e && "" !== e)).map((e => X(e)))],
+                        allowedValues: [...!0 !== e.isRequired ? [null] : [], ...n.options.filter((e => null !== e && "" !== e)).map((e => Q(e)))],
                         value: "",
                         readonly: !e.isEditable
                     }
                 };
                 return {
                     ...e,
                     kind: "selectbox",
                     sortMode: "default",
                     getCell(e, t) {
                         let n = null;
-                        return (0, g.bb)(e) && "" !== e && (n = X(e)), t && !l.data.allowedValues.includes(n) ? P(X(n), "The value is not part of the allowed options.") : {
+                        return (0, g.bb)(e) && "" !== e && (n = Q(e)), t && !l.data.allowedValues.includes(n) ? Z(Q(n), "The value is not part of the allowed options.") : {
                             ...l,
                             isMissingValue: null === n,
                             copyData: n || "",
                             data: {
                                 ...l.data,
                                 value: n
                             }
                         }
                     },
                     getCellValue(e) {
                         var n, i, o, l, r, a, s;
-                        return (0, g.le)(null === (n = e.data) || void 0 === n ? void 0 : n.value) || "" === (null === (i = e.data) || void 0 === i ? void 0 : i.value) ? null : "number" === t ? null !== (l = $(null === (r = e.data) || void 0 === r ? void 0 : r.value)) && void 0 !== l ? l : null : "boolean" === t ? null !== (a = Q(null === (s = e.data) || void 0 === s ? void 0 : s.value)) && void 0 !== a ? a : null : null === (o = e.data) || void 0 === o ? void 0 : o.value
+                        return (0, g.le)(null === (n = e.data) || void 0 === n ? void 0 : n.value) || "" === (null === (i = e.data) || void 0 === i ? void 0 : i.value) ? null : "number" === t ? null !== (l = ee(null === (r = e.data) || void 0 === r ? void 0 : r.value)) && void 0 !== l ? l : null : "boolean" === t ? null !== (a = $(null === (s = e.data) || void 0 === s ? void 0 : s.value)) && void 0 !== a ? a : null : null === (o = e.data) || void 0 === o ? void 0 : o.value
                     }
                 }
             }
-            xe.isEditableType = !0;
-            const Ce = xe;
+            Ce.isEditableType = !0;
+            const Ee = Ce;
 
-            function Ee(e) {
+            function Se(e) {
                 const t = {
                     kind: o.p6.Bubble,
                     data: [],
                     allowOverlay: !0,
                     contentAlign: e.contentAlignment,
                     style: e.isIndex ? "faded" : "normal"
                 };
                 return {
                     ...e,
                     kind: "list",
                     sortMode: "default",
                     isEditable: !1,
                     getCell(e) {
-                        const n = (0, g.le)(e) ? [] : G(e);
+                        const n = (0, g.le)(e) ? [] : X(e);
                         return {
                             ...t,
                             data: n,
                             isMissingValue: (0, g.le)(e),
-                            copyData: (0, g.le)(e) ? "" : X(n.map((e => "string" === typeof e && e.includes(",") ? e.replace(/,/g, " ") : e)))
+                            copyData: (0, g.le)(e) ? "" : Q(n.map((e => "string" === typeof e && e.includes(",") ? e.replace(/,/g, " ") : e)))
                         }
                     },
-                    getCellValue: e => (0, g.le)(e.data) || Y(e) ? null : e.data
+                    getCellValue: e => (0, g.le)(e.data) || U(e) ? null : e.data
                 }
             }
-            Ee.isEditableType = !1;
-            const Me = Ee;
+            Se.isEditableType = !1;
+            const Me = Se;
 
-            function Se(e, t, n) {
+            function ke(e, t, n) {
                 const i = new RegExp("".concat(e, "[,\\s].*{(?:[^}]*[\\s;]{1})?").concat(t, ":\\s*([^;}]+)[;]?.*}"), "gm");
                 n = n.replace(/{/g, " {");
                 const o = i.exec(n);
                 if (o) return o[1].trim()
             }
 
             function Te(e, t) {
                 const n = e.types.index[t],
                     i = e.indexNames[t];
                 let o = !0;
-                return "range" === W.fu.getTypeName(n) && (o = !1), {
+                return "range" === j.fu.getTypeName(n) && (o = !1), {
                     id: "index-".concat(t),
                     name: i,
                     title: i,
                     isEditable: o,
                     arrowType: n,
                     isIndex: !0,
                     isHidden: !1
                 }
             }
 
-            function ke(e, t) {
+            function Re(e, t) {
                 const n = e.columns[0][t];
                 let i, o = e.types.data[t];
                 if ((0, g.le)(o) && (o = {
                         meta: null,
                         numpy_type: "object",
                         pandas_type: "object"
-                    }), "categorical" === W.fu.getTypeName(o)) {
+                    }), "categorical" === j.fu.getTypeName(o)) {
                     const n = e.getCategoricalOptions(t);
                     (0, g.bb)(n) && (i = {
                         options: n
                     })
                 }
                 return {
                     id: "column-".concat(n, "-").concat(t),
@@ -944,61 +945,61 @@
                     arrowType: o,
                     columnTypeOptions: i,
                     isIndex: !1,
                     isHidden: !1
                 }
             }
 
-            function Re(e, t) {
+            function Ne(e, t) {
                 let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : void 0;
-                const i = e.arrowType ? W.fu.getTypeName(e.arrowType) : null;
+                const i = e.arrowType ? j.fu.getTypeName(e.arrowType) : null;
                 let l;
-                if ("object" === e.kind) l = e.getCell((0, g.bb)(t.content) ? le(W.fu.format(t.content, t.contentType, t.field)) : null);
+                if ("object" === e.kind) l = e.getCell((0, g.bb)(t.content) ? re(j.fu.format(t.content, t.contentType, t.field)) : null);
                 else if (["time", "date", "datetime"].includes(e.kind) && (0, g.bb)(t.content) && ("number" === typeof t.content || "bigint" === typeof t.content)) {
                     var r, a;
                     let n;
                     var s, d, c;
-                    if ("time" === i && (0, g.bb)(null === (r = t.field) || void 0 === r || null === (a = r.type) || void 0 === a ? void 0 : a.unit)) n = L().unix(W.fu.convertToSeconds(t.content, null !== (s = null === (d = t.field) || void 0 === d || null === (c = d.type) || void 0 === c ? void 0 : c.unit) && void 0 !== s ? s : 0)).utc().toDate();
-                    else n = L().utc(Number(t.content)).toDate();
+                    if ("time" === i && (0, g.bb)(null === (r = t.field) || void 0 === r || null === (a = r.type) || void 0 === a ? void 0 : a.unit)) n = W().unix(j.fu.convertToSeconds(t.content, null !== (s = null === (d = t.field) || void 0 === d || null === (c = d.type) || void 0 === c ? void 0 : c.unit) && void 0 !== s ? s : 0)).utc().toDate();
+                    else n = W().utc(Number(t.content)).toDate();
                     l = e.getCell(n)
                 } else if ("decimal" === i) {
-                    const n = (0, g.le)(t.content) ? null : W.fu.format(t.content, t.contentType, t.field);
+                    const n = (0, g.le)(t.content) ? null : j.fu.format(t.content, t.contentType, t.field);
                     l = e.getCell(n)
                 } else l = e.getCell(t.content);
-                if (Z(l)) return l;
+                if (Y(l)) return l;
                 if (!e.isEditable) {
                     if ((0, g.bb)(t.displayContent)) {
                         var u;
-                        const e = le(t.displayContent);
+                        const e = re(t.displayContent);
                         l.kind === o.p6.Text || l.kind === o.p6.Number || l.kind === o.p6.Uri ? l = {
                             ...l,
                             displayData: e
                         } : l.kind === o.p6.Custom && "date-picker-cell" === (null === (u = l.data) || void 0 === u ? void 0 : u.kind) && (l = {
                             ...l,
                             data: {
                                 ...l.data,
                                 displayDate: e
                             }
                         })
                     }
                     n && t.cssId && (l = function(e, t, n) {
                         const i = {},
-                            o = Se(t, "color", n);
+                            o = ke(t, "color", n);
                         o && (i.textDark = o);
-                        const l = Se(t, "background-color", n);
+                        const l = ke(t, "background-color", n);
                         return l && (i.bgCell = l), "yellow" === l && void 0 === o && (i.textDark = "#31333F"), i ? {
                             ...e,
                             themeOverride: i
                         } : e
                     }(l, t.cssId, n))
                 }
                 return l
             }
 
-            function Ne(e) {
+            function Ie(e) {
                 const t = e.columnTypeOptions || {};
                 let n, i;
                 if (t.validate) try {
                     n = new RegExp(t.validate, "us")
                 } catch (a) {
                     n = "Invalid validate regex: ".concat(t.validate, ".\nError: ").concat(a)
                 }
@@ -1016,15 +1017,15 @@
                         hoverEffect: !0,
                         data: "",
                         displayData: "",
                         copyData: ""
                     },
                     r = i => {
                         if ((0, g.le)(i)) return !e.isRequired;
-                        const o = X(i);
+                        const o = Q(i);
                         return !(t.max_chars && o.length > t.max_chars) && !(n instanceof RegExp && !1 === n.test(o))
                     };
                 return {
                     ...e,
                     kind: "link",
                     sortMode: "default",
                     validateInput: r,
@@ -1032,17 +1033,17 @@
                         if ((0, g.le)(e)) return {
                             ...l,
                             data: null,
                             isMissingValue: !0,
                             onClickUri: () => {}
                         };
                         const s = e;
-                        if ("string" === typeof n) return P(X(s), n);
+                        if ("string" === typeof n) return Z(Q(s), n);
                         if (o) {
-                            if (!1 === r(s)) return P(X(s), "Invalid input.")
+                            if (!1 === r(s)) return Z(Q(s), "Invalid input.")
                         }
                         let d = "";
                         return s && (d = void 0 !== i ? function(e, t) {
                             if ((0, g.le)(t)) return "";
                             try {
                                 const n = t.match(e);
                                 return n && void 0 !== n[1] ? decodeURI(n[1]) : t
@@ -1059,18 +1060,18 @@
                             },
                             copyData: s
                         }
                     },
                     getCellValue: e => (0, g.le)(e.data) ? null : e.data
                 }
             }
-            Ne.isEditableType = !0;
-            const Ie = Ne;
+            Ie.isEditableType = !0;
+            const _e = Ie;
 
-            function _e(e) {
+            function Oe(e) {
                 const t = {
                     kind: o.p6.Image,
                     data: [],
                     displayData: [],
                     readonly: !0,
                     allowOverlay: !0,
                     contentAlign: e.contentAlignment || "center",
@@ -1078,43 +1079,43 @@
                 };
                 return {
                     ...e,
                     kind: "image",
                     sortMode: "default",
                     isEditable: !1,
                     getCell(e) {
-                        const n = (0, g.bb)(e) ? [X(e)] : [];
+                        const n = (0, g.bb)(e) ? [Q(e)] : [];
                         return {
                             ...t,
                             data: n,
                             isMissingValue: !(0, g.bb)(e),
                             displayData: n
                         }
                     },
                     getCellValue: e => void 0 === e.data || 0 === e.data.length ? null : e.data[0]
                 }
             }
-            _e.isEditableType = !1;
-            const Oe = _e;
+            Oe.isEditableType = !1;
+            const De = Oe;
 
-            function De(e) {
-                const t = ve(W.fu.getTypeName(e.arrowType)),
-                    n = K({
+            function Ae(e) {
+                const t = ye(j.fu.getTypeName(e.arrowType)),
+                    n = G({
                         min_value: 0,
                         max_value: t ? 100 : 1,
                         step: t ? 1 : .01,
                         format: t ? "%3d%%" : "percent"
                     }, e.columnTypeOptions);
                 let i;
                 try {
-                    i = ee(n.max_value, n.format)
+                    i = te(n.max_value, n.format)
                 } catch (a) {
-                    i = X(n.max_value)
+                    i = Q(n.max_value)
                 }
-                const l = (0, g.le)(n.step) || Number.isNaN(n.step) ? void 0 : ie(n.step),
+                const l = (0, g.le)(n.step) || Number.isNaN(n.step) ? void 0 : oe(n.step),
                     r = {
                         kind: o.p6.Custom,
                         allowOverlay: !1,
                         copyData: "",
                         contentAlign: e.contentAlignment,
                         data: {
                             kind: "range-cell",
@@ -1129,25 +1130,25 @@
                     };
                 return {
                     ...e,
                     kind: "progress",
                     sortMode: "smart",
                     isEditable: !1,
                     getCell(e) {
-                        if ((0, g.le)(e)) return U();
-                        if ((0, g.le)(n.min_value) || (0, g.le)(n.max_value) || Number.isNaN(n.min_value) || Number.isNaN(n.max_value) || n.min_value >= n.max_value) return P("Invalid min/max parameters", "The min_value (".concat(n.min_value, ") and max_value (").concat(n.max_value, ") parameters must be valid numbers."));
-                        if ((0, g.le)(n.step) || Number.isNaN(n.step)) return P("Invalid step parameter", "The step parameter (".concat(n.step, ") must be a valid number."));
-                        const t = $(e);
-                        if (Number.isNaN(t) || (0, g.le)(t)) return P(X(e), "The value cannot be interpreted as a number.");
-                        if (Number.isInteger(t) && !Number.isSafeInteger(t)) return P(X(e), "The value is larger than the maximum supported integer values in number columns (2^53).");
+                        if ((0, g.le)(e)) return q();
+                        if ((0, g.le)(n.min_value) || (0, g.le)(n.max_value) || Number.isNaN(n.min_value) || Number.isNaN(n.max_value) || n.min_value >= n.max_value) return Z("Invalid min/max parameters", "The min_value (".concat(n.min_value, ") and max_value (").concat(n.max_value, ") parameters must be valid numbers."));
+                        if ((0, g.le)(n.step) || Number.isNaN(n.step)) return Z("Invalid step parameter", "The step parameter (".concat(n.step, ") must be a valid number."));
+                        const t = ee(e);
+                        if (Number.isNaN(t) || (0, g.le)(t)) return Z(Q(e), "The value cannot be interpreted as a number.");
+                        if (Number.isInteger(t) && !Number.isSafeInteger(t)) return Z(Q(e), "The value is larger than the maximum supported integer values in number columns (2^53).");
                         let i = "";
                         try {
-                            i = ee(t, n.format, l)
+                            i = te(t, n.format, l)
                         } catch (a) {
-                            return P(X(t), (0, g.bb)(n.format) ? "Failed to format the number based on the provided format configuration: (".concat(n.format, "). Error: ").concat(a) : "Failed to format the number. Error: ".concat(a))
+                            return Z(Q(t), (0, g.bb)(n.format) ? "Failed to format the number based on the provided format configuration: (".concat(n.format, "). Error: ").concat(a) : "Failed to format the number. Error: ".concat(a))
                         }
                         const o = Math.min(n.max_value, Math.max(n.min_value, t));
                         return {
                             ...r,
                             isMissingValue: (0, g.le)(e),
                             copyData: String(t),
                             data: {
@@ -1159,19 +1160,19 @@
                     },
                     getCellValue(e) {
                         var t, n;
                         return e.kind === o.p6.Loading || void 0 === (null === (t = e.data) || void 0 === t ? void 0 : t.value) ? null : null === (n = e.data) || void 0 === n ? void 0 : n.value
                     }
                 }
             }
-            De.isEditableType = !1;
-            const Fe = De;
+            Ae.isEditableType = !1;
+            const Fe = Ae;
 
-            function Ae(e, t, n) {
-                const i = K({
+            function ze(e, t, n) {
+                const i = G({
                         y_min: 0,
                         y_max: 1
                     }, t.columnTypeOptions),
                     l = {
                         kind: o.p6.Custom,
                         allowOverlay: !1,
                         copyData: "",
@@ -1186,122 +1187,122 @@
                     };
                 return {
                     ...t,
                     kind: e,
                     sortMode: "default",
                     isEditable: !1,
                     getCell(e) {
-                        if ((0, g.le)(i.y_min) || (0, g.le)(i.y_max) || Number.isNaN(i.y_min) || Number.isNaN(i.y_max) || i.y_min >= i.y_max) return P("Invalid min/max y-axis configuration", "The y_min (".concat(i.y_min, ") and y_max (").concat(i.y_max, ") configuration options must be valid numbers."));
-                        if ((0, g.le)(e)) return U();
-                        const t = G(e),
+                        if ((0, g.le)(i.y_min) || (0, g.le)(i.y_max) || Number.isNaN(i.y_min) || Number.isNaN(i.y_max) || i.y_min >= i.y_max) return Z("Invalid min/max y-axis configuration", "The y_min (".concat(i.y_min, ") and y_max (").concat(i.y_max, ") configuration options must be valid numbers."));
+                        if ((0, g.le)(e)) return q();
+                        const t = X(e),
                             n = [];
                         let o = [];
-                        if (0 === t.length) return U();
+                        if (0 === t.length) return q();
                         let r = Number.MIN_SAFE_INTEGER,
                             a = Number.MAX_SAFE_INTEGER;
                         for (let i = 0; i < t.length; i++) {
-                            const e = $(t[i]);
-                            if (Number.isNaN(e) || (0, g.le)(e)) return P(X(t), "The value cannot be interpreted as a numeric array. ".concat(X(e), " is not a number."));
+                            const e = ee(t[i]);
+                            if (Number.isNaN(e) || (0, g.le)(e)) return Z(Q(t), "The value cannot be interpreted as a numeric array. ".concat(Q(e), " is not a number."));
                             e > r && (r = e), e < a && (a = e), n.push(e)
                         }
                         return o = n.length > 0 && (r > i.y_max || a < i.y_min) ? n.map((e => r - a === 0 ? r > (i.y_max || 1) ? i.y_max || 1 : i.y_min || 0 : ((i.y_max || 1) - (i.y_min || 0)) * ((e - a) / (r - a)) + (i.y_min || 0))) : n, {
                             ...l,
                             copyData: n.join(","),
                             data: {
                                 ...l.data,
                                 values: o,
-                                displayValues: n.map((e => ee(e)))
+                                displayValues: n.map((e => te(e)))
                             },
                             isMissingValue: (0, g.le)(e)
                         }
                     },
                     getCellValue(e) {
                         var t, n;
                         return e.kind === o.p6.Loading || void 0 === (null === (t = e.data) || void 0 === t ? void 0 : t.values) ? null : null === (n = e.data) || void 0 === n ? void 0 : n.values
                     }
                 }
             }
 
-            function ze(e) {
-                return Ae("line_chart", e, "line")
-            }
-
             function Ve(e) {
-                return Ae("bar_chart", e, "bar")
+                return ze("line_chart", e, "line")
             }
 
             function He(e) {
-                return Ae("area_chart", e, "area")
+                return ze("bar_chart", e, "bar")
+            }
+
+            function Le(e) {
+                return ze("area_chart", e, "area")
             }
-            ze.isEditableType = !1, Ve.isEditableType = !1, He.isEditableType = !1;
-            const Le = new Map(Object.entries({
-                    object: se,
-                    text: ce,
-                    checkbox: be,
-                    selectbox: Ce,
+            Ve.isEditableType = !1, He.isEditableType = !1, Le.isEditableType = !1;
+            const We = new Map(Object.entries({
+                    object: de,
+                    text: ue,
+                    checkbox: ve,
+                    selectbox: Ee,
                     list: Me,
-                    number: we,
-                    link: Ie,
-                    datetime: he,
-                    date: ge,
-                    time: pe,
-                    line_chart: ze,
-                    bar_chart: Ve,
-                    area_chart: He,
-                    image: Oe,
+                    number: xe,
+                    link: _e,
+                    datetime: pe,
+                    date: fe,
+                    time: ge,
+                    line_chart: Ve,
+                    bar_chart: He,
+                    area_chart: Le,
+                    image: De,
                     progress: Fe
                 })),
-                We = [],
-                je = "_index",
-                Be = "_pos:",
-                Pe = {
+                je = [],
+                Be = "_index",
+                Pe = "_pos:",
+                Ze = {
                     small: 75,
                     medium: 200,
                     large: 400
                 };
 
-            function Ze(e) {
-                if (!(0, g.le)(e)) return "number" === typeof e ? e : e in Pe ? Pe[e] : void 0
+            function Ye(e) {
+                if (!(0, g.le)(e)) return "number" === typeof e ? e : e in Ze ? Ze[e] : void 0
             }
 
-            function Ye(e, t) {
+            function Ue(e, t) {
                 if (!t) return e;
                 let n;
-                return t.has(e.name) && e.name !== je ? n = t.get(e.name) : t.has("".concat(Be).concat(e.indexNumber)) ? n = t.get("".concat(Be).concat(e.indexNumber)) : e.isIndex && t.has(je) && (n = t.get(je)), n ? F()({
+                return t.has(e.name) && e.name !== Be ? n = t.get(e.name) : t.has("".concat(Pe).concat(e.indexNumber)) ? n = t.get("".concat(Pe).concat(e.indexNumber)) : e.isIndex && t.has(Be) && (n = t.get(Be)), n ? F()({
                     ...e
                 }, {
                     title: n.label,
-                    width: Ze(n.width),
+                    width: Ye(n.width),
                     isEditable: (0, g.bb)(n.disabled) ? !n.disabled : void 0,
                     isHidden: n.hidden,
                     isRequired: n.required,
                     columnTypeOptions: n.type_config,
                     contentAlignment: n.alignment,
                     defaultValue: n.default,
                     help: n.help
                 }) : e
             }
 
-            function Ue(e) {
+            function qe(e) {
                 var t;
                 const n = null === (t = e.columnTypeOptions) || void 0 === t ? void 0 : t.type;
                 let i;
-                return (0, g.bb)(n) && (Le.has(n) ? i = Le.get(n) : (0, re.KE)("Unknown column type configured in column configuration: ".concat(n))), (0, g.le)(i) && (i = function(e) {
-                    let t = e ? W.fu.getTypeName(e) : null;
-                    return t ? (t = t.toLowerCase().trim(), ["unicode", "empty"].includes(t) ? ce : ["datetime", "datetimetz"].includes(t) ? he : "time" === t ? pe : "date" === t ? ge : ["object", "bytes"].includes(t) ? se : ["bool"].includes(t) ? be : ["int8", "int16", "int32", "int64", "uint8", "uint16", "uint32", "uint64", "float16", "float32", "float64", "float96", "float128", "range", "decimal"].includes(t) ? we : "categorical" === t ? Ce : t.startsWith("list") ? Me : se) : se
+                return (0, g.bb)(n) && (We.has(n) ? i = We.get(n) : (0, ae.KE)("Unknown column type configured in column configuration: ".concat(n))), (0, g.le)(i) && (i = function(e) {
+                    let t = e ? j.fu.getTypeName(e) : null;
+                    return t ? (t = t.toLowerCase().trim(), ["unicode", "empty"].includes(t) ? ue : ["datetime", "datetimetz"].includes(t) ? pe : "time" === t ? ge : "date" === t ? fe : ["object", "bytes"].includes(t) ? de : ["bool"].includes(t) ? ve : ["int8", "int16", "int32", "int64", "uint8", "uint16", "uint32", "uint64", "float16", "float32", "float64", "float96", "float128", "range", "decimal"].includes(t) ? xe : "categorical" === t ? Ee : t.startsWith("list") ? Me : de) : de
                 }(e.arrowType)), i
             }
-            const qe = function(e, t, n) {
+            const Je = function(e, t, n) {
                 const o = (0, f.u)(),
                     l = i.useMemo((() => function(e) {
                         if (!e) return new Map;
                         try {
                             return new Map(Object.entries(JSON.parse(e)))
                         } catch (t) {
-                            return (0, re.H)(t), new Map
+                            return (0, ae.H)(t), new Map
                         }
                     }(e.columns)), [e.columns]),
                     r = e.useContainerWidth || (0, g.bb)(e.width) && e.width > 0;
                 return {
                     columns: i.useMemo((() => {
                         let i = function(e) {
                             const t = [],
@@ -1322,27 +1323,27 @@
                                     ...Te(e, l),
                                     indexNumber: l
                                 };
                                 t.push(n)
                             }
                             for (let l = 0; l < o; l++) {
                                 const n = {
-                                    ...ke(e, l),
+                                    ...Re(e, l),
                                     indexNumber: l + i
                                 };
                                 t.push(n)
                             }
                             return t
                         }(t).map((t => {
                             let i = {
                                 ...t,
-                                ...Ye(t, l),
+                                ...Ue(t, l),
                                 isStretched: r
                             };
-                            const a = Ue(i);
+                            const a = qe(i);
                             return (e.editingMode === p.Eh.EditingMode.READ_ONLY || n || !1 === a.isEditableType) && (i = {
                                 ...i,
                                 isEditable: !1
                             }), e.editingMode !== p.Eh.EditingMode.READ_ONLY && 1 == i.isEditable && (i = {
                                 ...i,
                                 icon: "editable"
                             }, i.isRequired && e.editingMode === p.Eh.EditingMode.DYNAMIC && (i = {
@@ -1355,29 +1356,29 @@
                             i.forEach((e => {
                                 e.isIndex && t.push(e)
                             })), e.columnOrder.forEach((e => {
                                 const n = i.find((t => t.name === e));
                                 n && !n.isIndex && t.push(n)
                             })), i = t
                         }
-                        return i.length > 0 ? i : [se({
+                        return i.length > 0 ? i : [de({
                             id: "empty-index",
                             title: "",
                             indexNumber: 0,
                             isEditable: !1,
                             isIndex: !0
                         })]
                     }), [t, l, r, n, e.editingMode, e.columnOrder, o])
                 }
             };
 
-            function Je(e) {
-                return e.isIndex ? je : (0, g.le)(e.name) ? "" : e.name
+            function Ke(e) {
+                return e.isIndex ? Be : (0, g.le)(e.name) ? "" : e.name
             }
-            const Ke = class {
+            const Ge = class {
                 constructor(e) {
                     this.editedCells = new Map, this.addedRows = [], this.deletedRows = [], this.numRows = 0, this.numRows = e
                 }
                 toJson(e) {
                     const t = new Map;
                     e.forEach((e => {
                         t.set(e.indexNumber, e)
@@ -1387,39 +1388,39 @@
                         added_rows: [],
                         deleted_rows: []
                     };
                     this.editedCells.forEach(((e, i, o) => {
                         const l = {};
                         e.forEach(((e, n, i) => {
                             const o = t.get(n);
-                            o && (l[Je(o)] = o.getCellValue(e))
+                            o && (l[Ke(o)] = o.getCellValue(e))
                         })), n.edited_rows[i] = l
                     })), this.addedRows.forEach((e => {
                         const i = {};
                         let o = !1;
                         e.forEach(((e, n, l) => {
                             const r = t.get(n);
                             if (r) {
                                 const t = r.getCellValue(e);
-                                r.isRequired && r.isEditable && Y(e) && (o = !0), (0, g.bb)(t) && (i[Je(r)] = t)
+                                r.isRequired && r.isEditable && U(e) && (o = !0), (0, g.bb)(t) && (i[Ke(r)] = t)
                             }
                         })), o || n.added_rows.push(i)
                     })), n.deleted_rows = this.deletedRows;
                     return JSON.stringify(n, ((e, t) => void 0 === t ? null : t))
                 }
                 fromJson(e, t) {
                     this.editedCells = new Map, this.addedRows = [], this.deletedRows = [];
                     const n = JSON.parse(e),
                         i = new Map;
                     t.forEach((e => {
                         i.set(e.indexNumber, e)
                     }));
                     const o = new Map;
                     t.forEach((e => {
-                        o.set(Je(e), e)
+                        o.set(Ke(e), e)
                     })), Object.keys(n.edited_rows).forEach((e => {
                         const t = Number(e),
                             i = n.edited_rows[e];
                         Object.keys(i).forEach((e => {
                             const n = i[e],
                                 l = o.get(e);
                             if (l) {
@@ -1475,43 +1476,43 @@
                     for (let n = 0; n < this.deletedRows.length && !(this.deletedRows[n] > t); n++) t += 1;
                     return t
                 }
                 getNumRows() {
                     return this.numRows + this.addedRows.length - this.deletedRows.length
                 }
             };
-            var Ge = n(35704);
-            const Xe = function() {
+            var Xe = n(35704);
+            const Qe = function() {
                 const e = (0, f.u)(),
                     t = i.useMemo((() => ({
                         editable: e => '<svg xmlns="http://www.w3.org/2000/svg" height="40" viewBox="0 96 960 960" width="40" fill="'.concat(e.bgColor, '"><path d="m800.641 679.743-64.384-64.384 29-29q7.156-6.948 17.642-6.948 10.485 0 17.742 6.948l29 29q6.948 7.464 6.948 17.95 0 10.486-6.948 17.434l-29 29Zm-310.64 246.256v-64.383l210.82-210.821 64.384 64.384-210.821 210.82h-64.383Zm-360-204.872v-50.254h289.743v50.254H130.001Zm0-162.564v-50.255h454.615v50.255H130.001Zm0-162.307v-50.255h454.615v50.255H130.001Z"/></svg>')
                     })), []);
                 return {
                     theme: i.useMemo((() => ({
                         accentColor: e.colors.primary,
                         accentFg: e.colors.white,
-                        accentLight: (0, Ge.DZ)(e.colors.primary, .9),
+                        accentLight: (0, Xe.DZ)(e.colors.primary, .9),
                         borderColor: e.colors.fadedText05,
                         horizontalBorderColor: e.colors.fadedText05,
                         fontFamily: e.genericFonts.bodyFont,
-                        bgSearchResult: (0, Ge.DZ)(e.colors.primary, .9),
+                        bgSearchResult: (0, Xe.DZ)(e.colors.primary, .9),
                         resizeIndicatorColor: e.colors.primary,
                         bgIconHeader: e.colors.fadedText60,
                         fgIconHeader: e.colors.white,
                         bgHeader: e.colors.bgMix,
                         bgHeaderHasFocus: e.colors.secondaryBg,
                         bgHeaderHovered: e.colors.secondaryBg,
                         textHeader: e.colors.fadedText60,
                         textHeaderSelected: e.colors.white,
                         textGroupHeader: e.colors.fadedText60,
                         headerFontStyle: "".concat(e.fontSizes.sm),
                         baseFontStyle: e.fontSizes.sm,
                         editorFontSize: e.fontSizes.sm,
                         textDark: e.colors.bodyText,
-                        textMedium: (0, Ge.DZ)(e.colors.bodyText, .2),
+                        textMedium: (0, Xe.DZ)(e.colors.bodyText, .2),
                         textLight: e.colors.fadedText40,
                         textBubble: e.colors.fadedText60,
                         bgCell: e.colors.bgColor,
                         bgCellMedium: e.colors.bgColor,
                         cellHorizontalPadding: 8,
                         cellVerticalPadding: 3,
                         bgBubble: e.colors.secondaryBg,
@@ -1519,44 +1520,44 @@
                         linkColor: e.colors.linkText,
                         drilldownBorder: e.colors.darkenedBgMix25
                     })), [e]),
                     tableBorderRadius: e.radii.lg,
                     headerIcons: t
                 }
             };
-            const Qe = function(e, t, n, o) {
+            const $e = function(e, t, n, o) {
                 return {
                     getCellContent: i.useCallback((i => {
                         let [l, r] = i;
-                        if (l > t.length - 1) return P("Column index out of bounds.", "This should never happen. Please report this bug.");
-                        if (r > n - 1) return P("Row index out of bounds.", "This should never happen. Please report this bug.");
+                        if (l > t.length - 1) return Z("Column index out of bounds.", "This should never happen. Please report this bug.");
+                        if (r > n - 1) return Z("Row index out of bounds.", "This should never happen. Please report this bug.");
                         const a = t[l],
                             s = a.indexNumber,
                             d = o.current.getOriginalRowIndex(r),
                             c = o.current.isAddedRow(d);
                         if (a.isEditable || c) {
                             const e = o.current.getCell(s, d);
                             if ((0, g.bb)(e)) return e;
-                            if (c) return P("Error during cell creation.", "This should never happen. Please report this bug. " + "No cell found for an added row: col=".concat(s, "; row=").concat(d))
+                            if (c) return Z("Error during cell creation.", "This should never happen. Please report this bug. " + "No cell found for an added row: col=".concat(s, "; row=").concat(d))
                         }
                         try {
-                            return Re(a, e.getCell(d + 1, s), e.cssStyles)
+                            return Ne(a, e.getCell(d + 1, s), e.cssStyles)
                         } catch (u) {
-                            return P("Error during cell creation.", "This should never happen. Please report this bug. \nError: ".concat(u))
+                            return Z("Error during cell creation.", "This should never happen. Please report this bug. \nError: ".concat(u))
                         }
                     }), [t, n, e, o])
                 }
             };
-            var $e = n(32700);
-            const et = function(e, t, n) {
+            var et = n(32700);
+            const tt = function(e, t, n) {
                 const [o, l] = i.useState(), {
                     getCellContent: r,
                     getOriginalIndex: a
-                } = (0, $e.fF)({
-                    columns: t.map((e => J(e))),
+                } = (0, et.fF)({
+                    columns: t.map((e => K(e))),
                     getCellContent: n,
                     rows: e,
                     sort: o
                 }), s = i.useMemo((() => function(e, t) {
                     return void 0 === t ? e : e.map((e => e.id === t.column.id ? {
                         ...e,
                         title: "asc" === t.direction ? "\u2191 ".concat(e.title) : "\u2193 ".concat(e.title)
@@ -1565,134 +1566,166 @@
                     let t = "asc";
                     const n = s[e];
                     if (o && o.column.id === n.id) {
                         if ("asc" !== o.direction) return void l(void 0);
                         t = "desc"
                     }
                     l({
-                        column: J(n),
+                        column: K(n),
                         direction: t,
                         mode: n.sortMode
                     })
                 }), [o, s]);
                 return {
                     columns: s,
                     sortColumn: d,
                     getOriginalIndex: a,
                     getCellContent: r
                 }
             };
-            var tt = n(62813),
-                nt = n.n(tt);
-            const it = function(e, t, n, l) {
-                    const [r, a] = i.useState({
+            var nt = n(62813),
+                it = n.n(nt);
+            const ot = function(e, t, n, l, r) {
+                    const [a, s] = i.useState({
                         columns: o.EV.empty(),
                         rows: o.EV.empty(),
                         current: void 0
-                    }), s = !t && !n && (e.selectionMode.includes(p.Eh.SelectionMode.MULTI_ROW) || e.selectionMode.includes(p.Eh.SelectionMode.SINGLE_ROW)), d = s && e.selectionMode.includes(p.Eh.SelectionMode.MULTI_ROW), c = !t && !n && (e.selectionMode.includes(p.Eh.SelectionMode.SINGLE_COLUMN) || e.selectionMode.includes(p.Eh.SelectionMode.MULTI_COLUMN)), u = c && e.selectionMode.includes(p.Eh.SelectionMode.MULTI_COLUMN), m = r.rows.length > 0, h = r.columns.length > 0, g = void 0 !== r.current, f = i.useCallback((e => {
-                        const t = !nt()(e.rows.toArray(), r.rows.toArray()),
-                            n = !nt()(e.columns.toArray(), r.columns.toArray()),
-                            i = !nt()(e.current, r.current);
-                        let o = s && t || c && n,
-                            d = e;
-                        (s || c) && void 0 !== e.current && i && (d = {
-                            ...e,
-                            rows: r.rows,
-                            columns: r.columns
-                        }, o = !1), t && e.rows.length > 0 && n && 0 === e.columns.length && (d = {
-                            ...d,
-                            columns: r.columns
-                        }, o = !0), n && e.columns.length > 0 && t && 0 === e.rows.length && (d = {
-                            ...d,
-                            rows: r.rows
-                        }, o = !0), a(d), o && l(d)
-                    }), [r, s, c, l]), b = i.useCallback((function() {
+                    }), d = !t && !n && (e.selectionMode.includes(p.Eh.SelectionMode.MULTI_ROW) || e.selectionMode.includes(p.Eh.SelectionMode.SINGLE_ROW)), c = d && e.selectionMode.includes(p.Eh.SelectionMode.MULTI_ROW), u = !t && !n && (e.selectionMode.includes(p.Eh.SelectionMode.SINGLE_COLUMN) || e.selectionMode.includes(p.Eh.SelectionMode.MULTI_COLUMN)), m = u && e.selectionMode.includes(p.Eh.SelectionMode.MULTI_COLUMN), h = a.rows.length > 0, g = a.columns.length > 0, f = void 0 !== a.current, b = i.useCallback((e => {
+                        const t = !it()(e.rows.toArray(), a.rows.toArray()),
+                            n = !it()(e.columns.toArray(), a.columns.toArray()),
+                            i = !it()(e.current, a.current);
+                        let o = d && t || u && n,
+                            c = e;
+                        if ((d || u) && void 0 !== e.current && i && (c = {
+                                ...e,
+                                rows: a.rows,
+                                columns: a.columns
+                            }, o = !1), t && e.rows.length > 0 && n && 0 === e.columns.length && (c = {
+                                ...c,
+                                columns: a.columns
+                            }, o = !0), n && e.columns.length > 0 && t && 0 === e.rows.length && (c = {
+                                ...c,
+                                rows: a.rows
+                            }, o = !0), n && c.columns.length >= 0) {
+                            let e = c.columns;
+                            l.forEach(((t, n) => {
+                                t.isIndex && (e = e.remove(n))
+                            })), e.length < c.columns.length && (c = {
+                                ...c,
+                                columns: e
+                            })
+                        }
+                        s(c), o && r(c)
+                    }), [a, d, u, r, l]), v = i.useCallback((function() {
                         let e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0],
                             t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1];
                         const n = {
-                            columns: t ? r.columns : o.EV.empty(),
-                            rows: e ? r.rows : o.EV.empty(),
+                            columns: t ? a.columns : o.EV.empty(),
+                            rows: e ? a.rows : o.EV.empty(),
                             current: void 0
                         };
-                        a(n), (!e && s || !t && c) && l(n)
-                    }), [r, s, c, l]);
+                        s(n), (!e && d || !t && u) && r(n)
+                    }), [a, d, u, r]);
                     return {
-                        gridSelection: r,
-                        isRowSelectionActivated: s,
-                        isMultiRowSelectionActivated: d,
-                        isColumnSelectionActivated: c,
-                        isMultiColumnSelectionActivated: u,
-                        isRowSelected: m,
-                        isColumnSelected: h,
-                        isCellSelected: g,
-                        clearSelection: b,
-                        processSelectionChange: f
+                        gridSelection: a,
+                        isRowSelectionActivated: d,
+                        isMultiRowSelectionActivated: c,
+                        isColumnSelectionActivated: u,
+                        isMultiColumnSelectionActivated: m,
+                        isRowSelected: h,
+                        isColumnSelected: g,
+                        isCellSelected: f,
+                        clearSelection: v,
+                        processSelectionChange: b
                     }
                 },
-                ot = ",",
-                lt = '"',
+                lt = ",",
                 rt = '"',
-                at = "\n",
-                st = new RegExp("[".concat([ot, lt, at].join(""), "]"));
+                at = '"',
+                st = "\n",
+                dt = "\ufeff",
+                ct = new RegExp("[".concat([lt, rt, st].join(""), "]"));
 
-            function dt(e) {
+            function ut(e) {
                 return e.map((e => function(e) {
                     if ((0, g.le)(e)) return "";
-                    const t = X(e);
-                    if (st.test(t)) return "".concat(lt).concat(t.replace(new RegExp(lt, "g"), rt + lt)).concat(lt);
+                    const t = Q(e);
+                    if (ct.test(t)) return "".concat(rt).concat(t.replace(new RegExp(rt, "g"), at + rt)).concat(rt);
                     return t
-                }(e))).join(ot) + at
+                }(e))).join(lt) + st
+            }
+            async function mt(e, t, n, i) {
+                const o = new TextEncoder;
+                await e.write(o.encode(dt));
+                const l = n.map((e => e.name));
+                await e.write(o.encode(ut(l)));
+                for (let r = 0; r < i; r++) {
+                    const i = [];
+                    n.forEach(((e, n, o) => {
+                        i.push(e.getCellValue(t([n, r])))
+                    })), await e.write(o.encode(ut(i)))
+                }
+                await e.close()
             }
-            const ct = function(e, t, o) {
+            const ht = function(e, t, o, l) {
                 return {
                     exportToCsv: i.useCallback((async () => {
+                        const i = (new Date).toISOString().slice(0, 16).replace(":", "-"),
+                            r = "".concat(i, "_export.csv");
                         try {
                             const i = await n.e(5345).then(n.bind(n, 95345)),
-                                l = (new Date).toISOString().slice(0, 16).replace(":", "-"),
-                                r = "".concat(l, "_export.csv"),
-                                a = await i.showSaveFilePicker({
+                                l = await i.showSaveFilePicker({
                                     suggestedName: r,
                                     types: [{
                                         accept: {
                                             "text/csv": [".csv"]
                                         }
                                     }],
                                     excludeAcceptAllOption: !1
                                 }),
-                                s = new TextEncoder,
-                                d = await a.createWritable();
-                            await d.write(s.encode("\ufeff"));
-                            const c = t.map((e => e.name));
-                            await d.write(s.encode(dt(c)));
-                            for (let n = 0; n < o; n++) {
-                                const i = [];
-                                t.forEach(((t, o, l) => {
-                                    i.push(t.getCellValue(e([o, n])))
-                                })), await d.write(s.encode(dt(i)))
-                            }
-                            await d.close()
-                        } catch (i) {
-                            (0, re.KE)("Failed to export data as CSV", i)
+                                a = await l.createWritable();
+                            await mt(a, e, t, o)
+                        } catch (a) {
+                            if (a instanceof Error && "AbortError" === a.name) return;
+                            try {
+                                (0, ae.KE)("Failed to export data as CSV with FileSystem API, trying fallback method", a);
+                                let n = "";
+                                const i = new WritableStream({
+                                    write: async e => {
+                                        n += new TextDecoder("utf-8").decode(e)
+                                    },
+                                    close: async () => {}
+                                });
+                                await mt(i.getWriter(), e, t, o);
+                                const s = new Blob([n], {
+                                        type: "text/csv;charset=utf-8;"
+                                    }),
+                                    d = URL.createObjectURL(s),
+                                    c = document.createElement("a");
+                                l ? c.setAttribute("target", "_blank") : c.setAttribute("target", "_self"), c.style.display = "none", c.href = d, c.download = r, document.body.appendChild(c), c.click(), document.body.removeChild(c), URL.revokeObjectURL(d)
+                            } catch (a) {
+                                (0, ae.H)("Failed to export data as CSV", a)
+                            }
                         }
-                    }), [t, o, e])
+                    }), [t, o, e, l])
                 }
             };
-            const ut = function(e, t, n, o, l, r, a, s, d) {
+            const pt = function(e, t, n, o, l, r, a, s, d) {
                 const c = i.useCallback(((t, i) => {
                         let [r, a] = t;
                         const d = e[r];
                         if (!d.isEditable) return;
                         const c = d.indexNumber,
                             u = n.current.getOriginalRowIndex(l(a)),
                             m = o([r, a]),
                             h = d.getCellValue(m),
                             p = d.getCellValue(i);
-                        if (!Z(m) && p === h) return;
+                        if (!Y(m) && p === h) return;
                         const g = d.getCell(p, !0);
-                        Z(g) ? (0, re.KE)("Not applying the cell edit since it causes this error:\n ".concat(g.data)) : (n.current.setCell(c, u, {
+                        Y(g) ? (0, ae.KE)("Not applying the cell edit since it causes this error:\n ".concat(g.data)) : (n.current.setCell(c, u, {
                             ...g,
                             lastUpdated: performance.now()
                         }), s())
                     }), [e, n, l, o, s]),
                     u = i.useCallback((() => {
                         if (t) return;
                         const i = new Map;
@@ -1736,15 +1769,15 @@
                                 const r = i[t],
                                     a = h + c,
                                     s = t + d;
                                 if (s >= e.length) break;
                                 const u = e[s];
                                 if (u.isEditable) {
                                     const e = u.getCell(r, !0);
-                                    if ((0, g.bb)(e) && !Z(e)) {
+                                    if ((0, g.bb)(e) && !Y(e)) {
                                         const t = u.indexNumber,
                                             i = n.current.getOriginalRowIndex(l(a)),
                                             r = u.getCellValue(o([s, a]));
                                         u.getCellValue(e) !== r && (n.current.setCell(t, i, {
                                             ...e,
                                             lastUpdated: performance.now()
                                         }), m.push({
@@ -1771,26 +1804,26 @@
                     onCellEdited: c,
                     onPaste: p,
                     onRowAppended: m,
                     onDelete: h,
                     validateCell: f
                 }
             };
-            const mt = function(e, t) {
+            const gt = function(e, t) {
                 const [n, o] = i.useState(), l = i.useRef(null), r = i.useCallback((n => {
                     if (clearTimeout(l.current), l.current = 0, o(void 0), ("header" === n.kind || "cell" === n.kind) && n.location) {
                         const i = n.location[0],
                             r = n.location[1];
                         let a;
                         if (i < 0 || i >= e.length) return;
                         const s = e[i];
                         if ("header" === n.kind && (0, g.bb)(s)) a = s.help;
                         else if ("cell" === n.kind) {
                             const e = t([i, r]);
-                            s.isRequired && s.isEditable && Y(e) ? a = "\u26a0\ufe0f Please fill out this cell." : function(e) {
+                            s.isRequired && s.isEditable && U(e) ? a = "\u26a0\ufe0f Please fill out this cell." : function(e) {
                                 return e.hasOwnProperty("tooltip") && "" !== e.tooltip
                             }(e) && (a = e.tooltip)
                         }
                         a && (l.current = setTimeout((() => {
                             a && o({
                                 content: a,
                                 left: n.bounds.x + n.bounds.width / 2,
@@ -1803,37 +1836,37 @@
                     tooltip: n,
                     clearTooltip: i.useCallback((() => {
                         o(void 0)
                     }), [o]),
                     onItemHovered: r
                 }
             };
-            var ht = n(39806),
-                pt = n(97613),
-                gt = n(5527),
-                ft = n(85e3),
-                bt = n(37538);
-            const vt = function(e) {
+            var ft = n(39806),
+                bt = n(97613),
+                vt = n(5527),
+                yt = n(85e3),
+                wt = n(37538);
+            const xt = function(e) {
                 return {
                     drawCell: i.useCallback(((t, n) => {
                         const {
                             cell: i,
                             theme: o,
                             ctx: l,
                             rect: r
                         } = t, a = t.col;
-                        if (Y(i) && a < e.length) {
+                        if (U(i) && a < e.length) {
                             const i = e[a];
                             return ["checkbox", "line_chart", "bar_chart", "progress"].includes(i.kind) ? n() : (e => {
                                 const {
                                     cell: t,
                                     theme: n,
                                     ctx: i
                                 } = e;
-                                (0, ht.L6)({
+                                (0, ft.L6)({
                                     ...e,
                                     theme: {
                                         ...n,
                                         textDark: n.textLight,
                                         headerFontFull: "".concat(n.headerFontStyle, " ").concat(n.fontFamily),
                                         baseFontFull: "".concat(n.baseFontStyle, " ").concat(n.fontFamily),
                                         markerFontFull: "".concat(n.markerFontStyle, " ").concat(n.fontFamily)
@@ -1843,42 +1876,42 @@
                                 }, "None", t.contentAlign), i.fillStyle = n.textDark
                             })(t), void(i.isRequired && i.isEditable && function(e, t, n) {
                                 e.save(), e.beginPath(), e.moveTo(t.x + t.width - 8, t.y + 1), e.lineTo(t.x + t.width, t.y + 1), e.lineTo(t.x + t.width, t.y + 1 + 8), e.fillStyle = n.accentColor, e.fill(), e.restore()
                             }(l, r, o))
                         }
                         n()
                     }), [e]),
-                    customRenderers: i.useMemo((() => [pt.Z, gt.Z, ft.Z, bt.ZP, ...We]), [])
+                    customRenderers: i.useMemo((() => [bt.Z, vt.Z, yt.Z, wt.ZP, ...je]), [])
                 }
             };
-            const yt = function(e) {
+            const Ct = function(e) {
                     const [t, n] = (0, i.useState)((() => new Map)), o = i.useCallback(((e, i, o, l) => {
                         e.id && n(new Map(t).set(e.id, l))
                     }), [t]);
                     return {
                         columns: i.useMemo((() => e.map((e => e.id && t.has(e.id) && void 0 !== t.get(e.id) ? {
                             ...e,
                             width: t.get(e.id),
                             grow: 0
                         } : e))), [e, t]),
                         onColumnResize: o
                     }
                 },
-                wt = 2,
-                xt = 35,
-                Ct = 50 + wt,
-                Et = 2 * xt + wt;
-            const Mt = function(e, t, n, o, l) {
+                Et = 2,
+                St = 35,
+                Mt = 50 + Et,
+                kt = 2 * St + Et;
+            const Tt = function(e, t, n, o, l) {
                     let r, a = function(e) {
-                            return Math.max(e * xt + wt, Et)
+                            return Math.max(e * St + Et, kt)
                         }(t + 1 + (e.editingMode === p.Eh.EditingMode.DYNAMIC ? 1 : 0)),
                         s = Math.min(a, 400);
-                    e.height && (s = Math.max(e.height, Et), a = Math.max(e.height, a)), o && (s = Math.min(s, o), a = Math.min(a, o), e.height || (s = a));
+                    e.height && (s = Math.max(e.height, kt), a = Math.max(e.height, a)), o && (s = Math.min(s, o), a = Math.min(a, o), e.height || (s = a));
                     let d = n;
-                    e.useContainerWidth ? r = n : e.width && (r = Math.min(Math.max(e.width, Ct), n), d = Math.min(Math.max(e.width, d), n));
+                    e.useContainerWidth ? r = n : e.width && (r = Math.min(Math.max(e.width, Mt), n), d = Math.min(Math.max(e.width, d), n));
                     const [c, u] = i.useState({
                         width: r || "100%",
                         height: s
                     });
                     return i.useLayoutEffect((() => {
                         e.useContainerWidth && "100%" === c.width && u({
                             width: n,
@@ -1907,75 +1940,75 @@
                                 height: a
                             })
                         } else u({
                             width: r || "100%",
                             height: s
                         })
                     }), [l]), {
-                        minHeight: Et,
+                        minHeight: kt,
                         maxHeight: a,
-                        minWidth: Ct,
+                        minWidth: Mt,
                         maxWidth: d,
                         resizableSize: c,
                         setResizableSize: u
                     }
                 },
-                St = (0, M.Z)("img", {
+                Rt = (0, S.Z)("img", {
                     target: "e24uaba0"
                 })((() => ({
                     maxWidth: "100%",
                     maxHeight: "600px",
                     objectFit: "scale-down"
                 })), ""),
-                Tt = e => {
+                Nt = e => {
                     let {
                         urls: t
                     } = e;
                     const n = t && t.length > 0 ? t[0] : "";
                     return n.startsWith("http") ? (0, R.jsx)("a", {
                         href: n,
                         target: "_blank",
                         rel: "noreferrer noopener",
-                        children: (0, R.jsx)(St, {
+                        children: (0, R.jsx)(Rt, {
                             src: n
                         })
-                    }) : (0, R.jsx)(St, {
+                    }) : (0, R.jsx)(Rt, {
                         src: n
                     })
                 };
-            var kt = n(31572),
-                Rt = n(13553),
-                Nt = n(80152);
-            const It = function(e) {
+            var It = n(31572),
+                _t = n(13553),
+                Ot = n(80152);
+            const Dt = function(e) {
                     let {
                         top: t,
                         left: n,
                         content: o,
                         clearTooltip: l
                     } = e;
                     const [r, a] = i.useState(!0), s = (0, f.u)(), {
                         colors: d,
                         fontSizes: c,
                         radii: u
                     } = s, m = i.useCallback((() => {
                         a(!1), l()
                     }), [l, a]);
-                    return (0, R.jsx)(kt.Z, {
-                        content: (0, R.jsx)(Nt.Uo, {
+                    return (0, R.jsx)(It.Z, {
+                        content: (0, R.jsx)(Ot.Uo, {
                             className: "stTooltipContent",
                             children: (0, R.jsx)(y.ZP, {
                                 style: {
                                     fontSize: c.sm
                                 },
                                 source: o,
                                 allowHTML: !1
                             })
                         }),
-                        placement: Rt.r4.top,
-                        accessibilityType: Rt.SI.tooltip,
+                        placement: _t.r4.top,
+                        accessibilityType: _t.SI.tooltip,
                         showArrow: !1,
                         popoverMargin: 5,
                         onClickOutside: m,
                         onEsc: m,
                         overrides: {
                             Body: {
                                 style: {
@@ -1988,15 +2021,15 @@
                                     paddingLeft: "0 !important",
                                     paddingRight: "0 !important",
                                     backgroundColor: "transparent"
                                 }
                             },
                             Inner: {
                                 style: {
-                                    backgroundColor: (0, S.Iy)(s) ? d.bgColor : d.secondaryBg,
+                                    backgroundColor: (0, M.Iy)(s) ? d.bgColor : d.secondaryBg,
                                     color: d.bodyText,
                                     fontSize: c.sm,
                                     fontWeight: "normal",
                                     paddingTop: "0 !important",
                                     paddingBottom: "0 !important",
                                     paddingLeft: "0 !important",
                                     paddingRight: "0 !important"
@@ -2011,15 +2044,15 @@
                                 position: "fixed",
                                 top: t,
                                 left: n
                             }
                         })
                     })
                 },
-                _t = (0, M.Z)("div", {
+                At = (0, S.Z)("div", {
                     target: "e1w7nams0"
                 })((e => {
                     let {
                         hasCustomizedScrollbars: t,
                         theme: n
                     } = e;
                     return {
@@ -2036,403 +2069,408 @@
                             },
                             overflowX: "auto !important",
                             overflowY: "auto !important"
                         }
                     }
                 }), "");
             n(2739), n(24665);
-            const Ot = (0, h.Z)((function(e) {
+            const Ft = (0, h.Z)((function(e) {
                 let {
                     element: t,
                     data: n,
                     width: h,
                     height: f,
                     disabled: b,
                     widgetMgr: v,
                     isFullScreen: y,
                     disableFullscreenMode: w,
                     expand: x,
                     collapse: C,
                     fragmentId: E
                 } = e;
-                const M = i.useRef(null),
-                    S = i.useRef(null),
-                    T = i.useRef(null),
+                const S = i.useRef(null),
+                    M = i.useRef(null),
+                    k = i.useRef(null),
+                    {
+                        theme: T,
+                        headerIcons: O,
+                        tableBorderRadius: D
+                    } = Qe(),
                     {
-                        theme: k,
-                        headerIcons: _,
-                        tableBorderRadius: O
-                    } = Xe(),
-                    [D, F] = i.useState(!0),
-                    [A, z] = i.useState(!1),
+                        libConfig: {
+                            enforceDownloadInNewTab: A = !1
+                        }
+                    } = i.useContext(_.E),
+                    [F, z] = i.useState(!0),
                     [V, H] = i.useState(!1),
                     [L, W] = i.useState(!1),
-                    j = i.useMemo((() => window.matchMedia && window.matchMedia("(pointer: coarse)").matches), []),
-                    B = i.useMemo((() => window.navigator.userAgent.includes("Mac OS") && window.navigator.userAgent.includes("Safari") || window.navigator.userAgent.includes("Chrome")), []);
+                    [j, B] = i.useState(!1),
+                    P = i.useMemo((() => window.matchMedia && window.matchMedia("(pointer: coarse)").matches), []),
+                    Z = i.useMemo((() => window.navigator.userAgent.includes("Mac OS") && window.navigator.userAgent.includes("Safari") || window.navigator.userAgent.includes("Chrome")), []);
                 (0, g.le)(t.editingMode) && (t.editingMode = p.Eh.EditingMode.READ_ONLY);
                 const {
-                    READ_ONLY: P,
-                    DYNAMIC: Z
-                } = p.Eh.EditingMode, Y = n.dimensions, U = Math.max(0, Y.rows - 1), K = 0 === U && !(t.editingMode === Z && Y.dataColumns > 0), G = U > 15e4, X = i.useRef(new Ke(U)), [Q, $] = i.useState(X.current.getNumRows());
+                    READ_ONLY: Y,
+                    DYNAMIC: U
+                } = p.Eh.EditingMode, q = n.dimensions, G = Math.max(0, q.rows - 1), X = 0 === G && !(t.editingMode === U && q.dataColumns > 0), Q = G > 15e4, $ = i.useRef(new Ge(G)), [ee, te] = i.useState($.current.getNumRows());
                 i.useEffect((() => {
-                    X.current = new Ke(U), $(X.current.getNumRows())
-                }), [U]);
-                const ee = i.useCallback((() => {
-                        X.current = new Ke(U), $(X.current.getNumRows())
-                    }), [U]),
+                    $.current = new Ge(G), te($.current.getNumRows())
+                }), [G]);
+                const ne = i.useCallback((() => {
+                        $.current = new Ge(G), te($.current.getNumRows())
+                    }), [G]),
                     {
-                        columns: te
-                    } = qe(t, n, b);
+                        columns: ie
+                    } = Je(t, n, b);
                 i.useEffect((() => {
-                    if (t.editingMode === P) return;
+                    if (t.editingMode === Y) return;
                     const e = v.getStringValue({
                         id: t.id,
                         formId: t.formId
                     });
-                    e && (X.current.fromJson(e, te), $(X.current.getNumRows()))
+                    e && ($.current.fromJson(e, ie), te($.current.getNumRows()))
                 }), []);
                 const {
-                    getCellContent: ne
-                } = Qe(n, te, Q, X), {
-                    columns: ie,
-                    sortColumn: oe,
-                    getOriginalIndex: le,
-                    getCellContent: re
-                } = et(U, te, ne), ae = i.useCallback((0, g.Ds)(150, (e => {
+                    getCellContent: oe
+                } = $e(n, ie, ee, $), {
+                    columns: le,
+                    sortColumn: re,
+                    getOriginalIndex: ae,
+                    getCellContent: se
+                } = tt(G, ie, oe), de = i.useCallback((0, g.Ds)(150, (e => {
                     const n = {
                         selection: {
                             rows: [],
                             columns: []
                         }
                     };
-                    n.selection.rows = e.rows.toArray().map((e => le(e))), n.selection.columns = e.columns.toArray().map((e => Je(te[e])));
+                    n.selection.rows = e.rows.toArray().map((e => ae(e))), n.selection.columns = e.columns.toArray().map((e => Ke(le[e])));
                     const i = JSON.stringify(n),
                         o = v.getStringValue({
                             id: t.id,
                             formId: t.formId
                         });
                     void 0 !== o && o === i || v.setStringValue({
                         id: t.id,
                         formId: t.formId
                     }, i, {
                         fromUi: !0
                     }, E)
                 })), [t.id, t.formId, v, E]), {
-                    gridSelection: se,
-                    isRowSelectionActivated: de,
-                    isMultiRowSelectionActivated: ce,
-                    isColumnSelectionActivated: ue,
-                    isMultiColumnSelectionActivated: me,
-                    isRowSelected: he,
-                    isColumnSelected: pe,
-                    isCellSelected: ge,
-                    clearSelection: fe,
-                    processSelectionChange: be
-                } = it(t, K, b, ae);
+                    gridSelection: ce,
+                    isRowSelectionActivated: ue,
+                    isMultiRowSelectionActivated: me,
+                    isColumnSelectionActivated: he,
+                    isMultiColumnSelectionActivated: pe,
+                    isRowSelected: ge,
+                    isColumnSelected: fe,
+                    isCellSelected: be,
+                    clearSelection: ve,
+                    processSelectionChange: ye
+                } = ot(t, X, b, le, de);
                 i.useEffect((() => {
-                    fe(!0, !0)
+                    ve(!0, !0)
                 }), [y]);
-                const ve = i.useCallback((e => {
+                const we = i.useCallback((e => {
                     var t;
-                    null === (t = S.current) || void 0 === t || t.updateCells(e)
+                    null === (t = M.current) || void 0 === t || t.updateCells(e)
                 }), []);
                 i.useEffect((() => {
-                    if (!de && !ue) return;
+                    if (!ue && !he) return;
                     const e = v.getStringValue({
                         id: t.id,
                         formId: t.formId
                     });
                     if (e) {
                         var n, i, l, r;
-                        const t = ie.map((e => Je(e))),
+                        const t = le.map((e => Ke(e))),
                             a = JSON.parse(e);
                         let s = o.EV.empty(),
                             d = o.EV.empty();
                         if (null === (n = a.selection) || void 0 === n || null === (i = n.rows) || void 0 === i || i.forEach((e => {
                                 s = s.add(e)
                             })), null === (l = a.selection) || void 0 === l || null === (r = l.columns) || void 0 === r || r.forEach((e => {
                                 d = d.add(t.indexOf(e))
                             })), s.length > 0 || d.length > 0) {
-                            be({
+                            ye({
                                 rows: s,
                                 columns: d,
                                 current: void 0
                             })
                         }
                     }
                 }), []);
-                const ye = i.useCallback((() => {
-                        Q !== X.current.getNumRows() && $(X.current.getNumRows())
-                    }), [Q]),
-                    we = i.useCallback((0, g.Ds)(150, (() => {
-                        const e = X.current.toJson(ie);
+                const xe = i.useCallback((() => {
+                        ee !== $.current.getNumRows() && te($.current.getNumRows())
+                    }), [ee]),
+                    Ce = i.useCallback((0, g.Ds)(150, (() => {
+                        const e = $.current.toJson(le);
                         let n = v.getStringValue({
                             id: t.id,
                             formId: t.formId
                         });
-                        void 0 === n && (n = new Ke(0).toJson([])), e !== n && v.setStringValue({
+                        void 0 === n && (n = new Ge(0).toJson([])), e !== n && v.setStringValue({
                             id: t.id,
                             formId: t.formId
                         }, e, {
                             fromUi: !0
                         }, E)
-                    })), [t.id, t.formId, v, E, ie, X.current]),
+                    })), [t.id, t.formId, v, E, le, $.current]),
                     {
-                        exportToCsv: xe
-                    } = ct(re, ie, Q),
+                        exportToCsv: Ee
+                    } = ht(se, le, ee, A),
                     {
-                        onCellEdited: Ce,
-                        onPaste: Ee,
-                        onRowAppended: Me,
-                        onDelete: Se,
-                        validateCell: Te
-                    } = ut(ie, t.editingMode !== Z, X, re, le, ve, ye, we, fe),
+                        onCellEdited: Se,
+                        onPaste: Me,
+                        onRowAppended: ke,
+                        onDelete: Te,
+                        validateCell: Re
+                    } = pt(le, t.editingMode !== U, $, se, ae, we, xe, Ce, ve),
                     {
-                        tooltip: ke,
-                        clearTooltip: Re,
-                        onItemHovered: Ne
-                    } = mt(ie, re),
+                        tooltip: Ne,
+                        clearTooltip: Ie,
+                        onItemHovered: _e
+                    } = gt(le, se),
                     {
-                        drawCell: Ie,
-                        customRenderers: _e
-                    } = vt(ie),
-                    Oe = i.useMemo((() => ie.map((e => J(e)))), [ie]),
+                        drawCell: Oe,
+                        customRenderers: De
+                    } = xt(le),
+                    Ae = i.useMemo((() => le.map((e => K(e)))), [le]),
                     {
-                        columns: De,
-                        onColumnResize: Fe
-                    } = yt(Oe),
+                        columns: Fe,
+                        onColumnResize: ze
+                    } = Ct(Ae),
                     {
-                        minHeight: Ae,
-                        maxHeight: ze,
-                        minWidth: Ve,
-                        maxWidth: He,
-                        resizableSize: Le,
-                        setResizableSize: We
-                    } = Mt(t, Q, h, f, y),
-                    je = i.useCallback((e => {
+                        minHeight: Ve,
+                        maxHeight: He,
+                        minWidth: Le,
+                        maxWidth: We,
+                        resizableSize: je,
+                        setResizableSize: Be
+                    } = Tt(t, ee, h, f, y),
+                    Pe = i.useCallback((e => {
                         let [t, n] = e;
                         return {
-                            ...q(!0, !1),
+                            ...J(!0, !1),
                             displayData: "empty",
                             contentAlign: "center",
                             allowOverlay: !1,
                             themeOverride: {
-                                textDark: k.textLight
+                                textDark: T.textLight
                             },
-                            span: [0, Math.max(ie.length - 1, 0)]
+                            span: [0, Math.max(le.length - 1, 0)]
                         }
-                    }), [ie, k.textLight]);
+                    }), [le, T.textLight]);
                 i.useEffect((() => {
                     if (!t.formId) return;
                     const e = new m.K;
                     return e.manageFormClearListener(v, t.formId, (() => {
-                        ee(), fe()
+                        ne(), ve()
                     })), () => {
                         e.disconnect()
                     }
-                }), [t.formId, ee, fe, v]);
-                const Be = !K && t.editingMode === Z && !b,
-                    Pe = K ? 0 : ie.filter((e => e.isIndex)).length;
+                }), [t.formId, ne, ve, v]);
+                const Ze = !X && t.editingMode === U && !b,
+                    Ye = X ? 0 : le.filter((e => e.isIndex)).length;
                 return i.useEffect((() => {
                     setTimeout((() => {
-                        if (T.current && S.current) {
+                        if (k.current && M.current) {
                             var e, t;
-                            const n = null === (e = T.current) || void 0 === e || null === (t = e.querySelector(".dvn-stack")) || void 0 === t ? void 0 : t.getBoundingClientRect();
-                            n && (H(n.height > T.current.clientHeight), W(n.width > T.current.clientWidth))
+                            const n = null === (e = k.current) || void 0 === e || null === (t = e.querySelector(".dvn-stack")) || void 0 === t ? void 0 : t.getBoundingClientRect();
+                            n && (W(n.height > k.current.clientHeight), B(n.width > k.current.clientWidth))
                         }
                     }), 1)
-                }), [Le, Q, De]), (0, R.jsxs)(_t, {
+                }), [je, ee, Fe]), (0, R.jsxs)(At, {
                     "data-testid": "stDataFrame",
                     className: "stDataFrame",
-                    hasCustomizedScrollbars: B,
-                    ref: T,
+                    hasCustomizedScrollbars: Z,
+                    ref: k,
                     onMouseDown: e => {
-                        if (T.current && B) {
-                            const t = T.current.getBoundingClientRect();
-                            L && t.height - 7 < e.clientY - t.top && e.stopPropagation(), V && t.width - 7 < e.clientX - t.left && e.stopPropagation()
+                        if (k.current && Z) {
+                            const t = k.current.getBoundingClientRect();
+                            j && t.height - 7 < e.clientY - t.top && e.stopPropagation(), L && t.width - 7 < e.clientX - t.left && e.stopPropagation()
                         }
                     },
                     onBlur: e => {
-                        D || j || e.currentTarget.contains(e.relatedTarget) || fe(!0, !0)
+                        F || P || e.currentTarget.contains(e.relatedTarget) || ve(!0, !0)
                     },
                     children: [(0, R.jsxs)(I, {
                         isFullScreen: y,
                         disableFullscreenMode: w,
-                        locked: he && !de || ge || j && D,
+                        locked: ge && !ue || be || P && F,
                         onExpand: x,
                         onCollapse: C,
-                        target: _t,
-                        children: [(de && he || ue && pe) && (0, R.jsx)(N, {
+                        target: At,
+                        children: [(ue && ge || he && fe) && (0, R.jsx)(N, {
                             label: "Clear selection",
                             icon: a.x,
                             onClick: () => {
-                                fe(), Re()
+                                ve(), Ie()
                             }
-                        }), Be && he && (0, R.jsx)(N, {
+                        }), Ze && ge && (0, R.jsx)(N, {
                             label: "Delete row(s)",
                             icon: s.H,
                             onClick: () => {
-                                Se && (Se(se), Re())
+                                Te && (Te(ce), Ie())
                             }
-                        }), Be && !he && (0, R.jsx)(N, {
+                        }), Ze && !ge && (0, R.jsx)(N, {
                             label: "Add row",
                             icon: d.m,
                             onClick: () => {
-                                Me && (F(!0), Me(), Re())
+                                ke && (z(!0), ke(), Ie())
                             }
-                        }), !G && !K && (0, R.jsx)(N, {
+                        }), !Q && !X && (0, R.jsx)(N, {
                             label: "Download as CSV",
                             icon: c.k,
-                            onClick: () => xe()
-                        }), !K && (0, R.jsx)(N, {
+                            onClick: () => Ee()
+                        }), !X && (0, R.jsx)(N, {
                             label: "Search",
                             icon: u.o,
                             onClick: () => {
-                                A ? z(!1) : (F(!0), z(!0)), Re()
+                                V ? H(!1) : (z(!0), H(!0)), Ie()
                             }
                         })]
                     }), (0, R.jsx)(r.e, {
                         "data-testid": "stDataFrameResizable",
-                        ref: M,
-                        defaultSize: Le,
+                        ref: S,
+                        defaultSize: je,
                         style: {
-                            border: "1px solid ".concat(k.borderColor),
-                            borderRadius: "".concat(O)
+                            border: "1px solid ".concat(T.borderColor),
+                            borderRadius: "".concat(D)
                         },
-                        minHeight: Ae,
-                        maxHeight: ze,
-                        minWidth: Ve,
-                        maxWidth: He,
-                        size: Le,
+                        minHeight: Ve,
+                        maxHeight: He,
+                        minWidth: Le,
+                        maxWidth: We,
+                        size: je,
                         enable: {
                             top: !1,
                             right: !1,
                             bottom: !1,
                             left: !1,
                             topRight: !1,
                             bottomRight: !0,
                             bottomLeft: !1,
                             topLeft: !1
                         },
-                        grid: [1, xt],
-                        snapGap: xt / 3,
+                        grid: [1, St],
+                        snapGap: St / 3,
                         onResizeStop: (e, t, n, i) => {
-                            M.current && We({
-                                width: M.current.size.width,
-                                height: ze - M.current.size.height === wt ? M.current.size.height + wt : M.current.size.height
+                            S.current && Be({
+                                width: S.current.size.width,
+                                height: He - S.current.size.height === Et ? S.current.size.height + Et : S.current.size.height
                             })
                         },
                         children: (0, R.jsx)(l.F, {
                             className: "glideDataEditor",
-                            ref: S,
-                            columns: De,
-                            rows: K ? 1 : Q,
+                            ref: M,
+                            columns: Fe,
+                            rows: X ? 1 : ee,
                             minColumnWidth: 50,
                             maxColumnWidth: 1e3,
                             maxColumnAutoWidth: 500,
-                            rowHeight: xt,
-                            headerHeight: xt,
-                            getCellContent: K ? je : re,
-                            onColumnResize: j ? void 0 : Fe,
+                            rowHeight: St,
+                            headerHeight: St,
+                            getCellContent: X ? Pe : se,
+                            onColumnResize: P ? void 0 : ze,
                             resizeIndicator: "header",
-                            freezeColumns: Pe,
+                            freezeColumns: Ye,
                             smoothScrollX: !0,
                             smoothScrollY: !0,
                             verticalBorder: !0,
                             getCellsForSelection: !0,
                             rowMarkers: "none",
-                            rangeSelect: j ? "cell" : "rect",
+                            rangeSelect: P ? "cell" : "rect",
                             columnSelect: "none",
                             rowSelect: "none",
-                            onItemHovered: Ne,
+                            onItemHovered: _e,
                             keybindings: {
                                 downFill: !0
                             },
                             onKeyDown: e => {
-                                (e.ctrlKey || e.metaKey) && "f" === e.key && (z((e => !e)), e.stopPropagation(), e.preventDefault())
+                                (e.ctrlKey || e.metaKey) && "f" === e.key && (H((e => !e)), e.stopPropagation(), e.preventDefault())
                             },
-                            showSearch: A,
+                            showSearch: V,
                             onSearchClose: () => {
-                                z(!1), Re()
+                                H(!1), Ie()
                             },
                             onHeaderClicked: (e, t) => {
-                                K || G || ue || (de && he && fe(), oe(e))
+                                X || Q || he || (ue && ge && ve(), re(e))
                             },
-                            gridSelection: se,
+                            gridSelection: ce,
                             onGridSelectionChange: e => {
-                                (D || j) && (be(e), void 0 !== ke && Re())
+                                (F || P) && (ye(e), void 0 !== Ne && Ie())
                             },
-                            theme: k,
+                            theme: T,
                             onMouseMove: e => {
-                                "out-of-bounds" === e.kind && D ? F(!1) : "out-of-bounds" === e.kind || D || F(!0)
+                                "out-of-bounds" === e.kind && F ? z(!1) : "out-of-bounds" === e.kind || F || z(!0)
                             },
                             fixedShadowX: !0,
                             fixedShadowY: !0,
                             experimental: {
                                 scrollbarWidthOverride: 0,
-                                ...B && {
-                                    paddingBottom: L ? -6 : void 0,
-                                    paddingRight: V ? -6 : void 0
+                                ...Z && {
+                                    paddingBottom: j ? -6 : void 0,
+                                    paddingRight: L ? -6 : void 0
                                 }
                             },
-                            drawCell: Ie,
-                            customRenderers: _e,
-                            imageEditorOverride: Tt,
-                            headerIcons: _,
-                            validateCell: Te,
+                            drawCell: Oe,
+                            customRenderers: De,
+                            imageEditorOverride: Nt,
+                            headerIcons: O,
+                            validateCell: Re,
                             onPaste: !1,
-                            ...de && {
+                            ...ue && {
                                 rowMarkers: {
                                     kind: "checkbox",
                                     checkboxStyle: "square",
                                     theme: {
-                                        bgCell: k.bgHeader,
-                                        bgCellMedium: k.bgHeader
+                                        bgCell: T.bgHeader,
+                                        bgCellMedium: T.bgHeader
                                     }
                                 },
-                                rowSelectionMode: ce ? "multi" : "auto",
-                                rowSelect: b ? "none" : ce ? "multi" : "single",
+                                rowSelectionMode: me ? "multi" : "auto",
+                                rowSelect: b ? "none" : me ? "multi" : "single",
                                 rowSelectionBlending: "mixed",
                                 rangeSelectionBlending: "exclusive"
                             },
-                            ...ue && {
-                                columnSelect: b ? "none" : me ? "multi" : "single",
+                            ...he && {
+                                columnSelect: b ? "none" : pe ? "multi" : "single",
                                 columnSelectionBlending: "mixed",
                                 rangeSelectionBlending: "exclusive"
                             },
-                            ...!K && t.editingMode !== P && !b && {
-                                fillHandle: !j,
-                                onCellEdited: Ce,
-                                onPaste: Ee,
-                                onDelete: Se
+                            ...!X && t.editingMode !== Y && !b && {
+                                fillHandle: !P,
+                                onCellEdited: Se,
+                                onPaste: Me,
+                                onDelete: Te
                             },
-                            ...!K && t.editingMode === Z && {
+                            ...!X && t.editingMode === U && {
                                 trailingRowOptions: {
                                     sticky: !1,
                                     tint: !0
                                 },
                                 rowMarkers: {
                                     kind: "checkbox",
                                     checkboxStyle: "square",
                                     theme: {
-                                        bgCell: k.bgHeader,
-                                        bgCellMedium: k.bgHeader
+                                        bgCell: T.bgHeader,
+                                        bgCellMedium: T.bgHeader
                                     }
                                 },
                                 rowSelectionMode: "multi",
                                 rowSelect: b ? "none" : "multi",
-                                onRowAppended: b ? void 0 : Me,
+                                onRowAppended: b ? void 0 : ke,
                                 onHeaderClicked: void 0
                             }
                         })
-                    }), ke && ke.content && (0, R.jsx)(It, {
-                        top: ke.top,
-                        left: ke.left,
-                        content: ke.content,
-                        clearTooltip: Re
+                    }), Ne && Ne.content && (0, R.jsx)(Dt, {
+                        top: Ne.top,
+                        left: Ne.left,
+                        content: Ne.content,
+                        clearTooltip: Ie
                     })]
                 })
             }), !0)
         },
         87814: (e, t, n) => {
             n.d(t, {
                 K: () => o
```

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8427.bd0a7cf3.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8427.bd0a7cf3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8477.de889fe5.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8477.de889fe5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8492.0d93bd08.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8492.0d93bd08.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8536.f8de3d9a.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8536.f8de3d9a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8570.6de19120.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8570.6de19120.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/8691.9ccf7f89.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/8691.9ccf7f89.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9330.2b4c99e0.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/9330.2b4c99e0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9336.2d95d840.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/9336.2d95d840.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/937.a1248039.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/937.a1248039.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9656.8c935274.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/9656.8c935274.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/9865.fd93213d.chunk.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/9865.fd93213d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/main.32c71338.js` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/main.60ba1bc7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.32c71338.js.LICENSE.txt */
+/*! For license information please see main.60ba1bc7.js.LICENSE.txt */
 (() => {
     var __webpack_modules__ = {
             68785: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     B: () => i,
                     Id: () => r,
@@ -116067,15 +116067,15 @@
         for (var n in t) __webpack_require__.o(t, n) && !__webpack_require__.o(e, n) && Object.defineProperty(e, n, {
             enumerable: !0,
             get: t[n]
         })
     }, __webpack_require__.f = {}, __webpack_require__.e = e => Promise.all(Object.keys(__webpack_require__.f).reduce(((t, n) => (__webpack_require__.f[n](e, t), t)), [])), __webpack_require__.u = e => "static/js/" + e + "." + {
         178: "7bea8c5d",
         329: "464ed8ec",
-        474: "87506447",
+        474: "7eb0c6cd",
         937: "a1248039",
         1074: "73973756",
         1168: "14f7c6ff",
         1307: "0f0cca93",
         1451: "3b0a3e31",
         1479: "6709db03",
         1792: "8bd6ce2a",
@@ -116084,26 +116084,25 @@
         2469: "09ea79bb",
         2634: "1249dc7a",
         2736: "4336e2b9",
         3053: "7e70ec3b",
         3301: "1d1b10bb",
         3466: "05d62820",
         3513: "7dedbda2",
-        3631: "be5c35fa",
         4113: "99983645",
         4132: "49bf3f2c",
         4177: "69f9f18d",
         4319: "bf1c86bf",
         4477: "1bd49702",
         4500: "b6f348d1",
         4666: "c4b22a63",
         5106: "44f0ff51",
         5117: "04bfe5d3",
         5249: "f2f4070d",
-        5345: "65c91ee7",
+        5345: "73d26e5d",
         5379: "6571574f",
         5441: "1b94928f",
         5791: "9a42fb4b",
         6013: "4ba2d616",
         6405: "ac5a6f23",
         6718: "802da17e",
         6853: "93dd1c4c",
@@ -116111,25 +116110,24 @@
         7142: "83028745",
         7175: "be4076bc",
         7323: "b74cc85b",
         7483: "64f23be7",
         7602: "e8abc06b",
         7805: "acc6316a",
         8005: "43974a35",
-        8148: "a5f74d47",
+        8148: "f80eec24",
         8427: "bd0a7cf3",
         8477: "de889fe5",
         8492: "0d93bd08",
         8536: "f8de3d9a",
         8570: "6de19120",
         8691: "9ccf7f89",
         9330: "2b4c99e0",
         9336: "2d95d840",
         9656: "8c935274",
-        9758: "6e6d8662",
         9865: "fd93213d"
     } [e] + ".chunk.js", __webpack_require__.miniCssF = e => "static/css/" + e + "." + {
         3466: "8b8f33d6",
         5441: "e3b876c5",
         8148: "49dfd2ce"
     } [e] + ".chunk.css", __webpack_require__.g = function() {
         if ("object" === typeof globalThis) return globalThis;
@@ -127178,16 +127176,18 @@
                         this.hostCommunicationMgr.sendMessageToHost({
                             type: "SET_APP_PAGES",
                             appPages: t
                         })
                     }))
                 }, this.handlePageProfileMsg = e => {
                     var t, n, r;
+                    const o = je.AG.toObject(e);
                     this.metricsMgr.enqueue("pageProfile", {
-                        ...je.AG.toObject(e),
+                        ...o,
+                        isFragmentRun: Boolean(o.isFragmentRun),
                         appId: this.sessionInfo.current.appId,
                         numPages: null === (t = this.state.appPages) || void 0 === t ? void 0 : t.length,
                         sessionId: this.sessionInfo.current.sessionId,
                         pythonVersion: this.sessionInfo.current.pythonVersion,
                         pageScriptHash: this.state.currentPageScriptHash,
                         activeTheme: null === (n = this.props.theme) || void 0 === n || null === (r = n.activeTheme) || void 0 === r ? void 0 : r.name,
                         totalLoadTime: Math.round(1e3 * (performance.now() - this.state.latestRunTime))
```

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/js/main.32c71338.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/js/main.60ba1bc7.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg` & `streamlit_nightly-1.34.1.dev20240516/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/string_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/temporary_directory.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/testing/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/testing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/app_test.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/testing/v1/app_test.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/element_tree.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/testing/v1/element_tree.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/local_script_runner.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/testing/v1/local_script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/testing/v1/util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/testing/v1/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/time_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/time_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/type_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/url_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/user_info.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/ipython/modified_sys_path.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/vendor/pympler/asizeof.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/vendor/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/version.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/event_based_path_watcher.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/local_sources_watcher.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/path_watcher.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/polling_path_watcher.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/watcher/util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/bootstrap.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/bootstrap.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/cache_storage_manager_config.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/cli.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/__init__.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/app_static_file_handler.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/browser_websocket_handler.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/browser_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/component_request_handler.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/media_file_handler.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/routes.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/routes.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/server.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/server.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/server_util.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/stats_request_handler.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/upload_file_request_handler.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit/web/server/websocket_headers.py` & `streamlit_nightly-1.34.1.dev20240516/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/PKG-INFO` & `streamlit_nightly-1.34.1.dev20240516/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.34.1.dev20240514
+Version: 1.34.1.dev20240516
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.34.1.dev20240514/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit_nightly-1.34.1.dev20240516/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -356,28 +356,27 @@
 streamlit/static/static/js/3053.7e70ec3b.chunk.js
 streamlit/static/static/js/329.464ed8ec.chunk.js
 streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
 streamlit/static/static/js/3301.1d1b10bb.chunk.js
 streamlit/static/static/js/3466.05d62820.chunk.js
 streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
 streamlit/static/static/js/3513.7dedbda2.chunk.js
-streamlit/static/static/js/3631.be5c35fa.chunk.js
 streamlit/static/static/js/4113.99983645.chunk.js
 streamlit/static/static/js/4132.49bf3f2c.chunk.js
 streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
 streamlit/static/static/js/4177.69f9f18d.chunk.js
 streamlit/static/static/js/4319.bf1c86bf.chunk.js
 streamlit/static/static/js/4477.1bd49702.chunk.js
 streamlit/static/static/js/4500.b6f348d1.chunk.js
 streamlit/static/static/js/4666.c4b22a63.chunk.js
-streamlit/static/static/js/474.87506447.chunk.js
+streamlit/static/static/js/474.7eb0c6cd.chunk.js
 streamlit/static/static/js/5106.44f0ff51.chunk.js
 streamlit/static/static/js/5117.04bfe5d3.chunk.js
 streamlit/static/static/js/5249.f2f4070d.chunk.js
-streamlit/static/static/js/5345.65c91ee7.chunk.js
+streamlit/static/static/js/5345.73d26e5d.chunk.js
 streamlit/static/static/js/5379.6571574f.chunk.js
 streamlit/static/static/js/5441.1b94928f.chunk.js
 streamlit/static/static/js/5791.9a42fb4b.chunk.js
 streamlit/static/static/js/6013.4ba2d616.chunk.js
 streamlit/static/static/js/6405.ac5a6f23.chunk.js
 streamlit/static/static/js/6718.802da17e.chunk.js
 streamlit/static/static/js/6853.93dd1c4c.chunk.js
@@ -388,30 +387,29 @@
 streamlit/static/static/js/7323.b74cc85b.chunk.js
 streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
 streamlit/static/static/js/7483.64f23be7.chunk.js
 streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
 streamlit/static/static/js/7602.e8abc06b.chunk.js
 streamlit/static/static/js/7805.acc6316a.chunk.js
 streamlit/static/static/js/8005.43974a35.chunk.js
-streamlit/static/static/js/8148.a5f74d47.chunk.js
+streamlit/static/static/js/8148.f80eec24.chunk.js
 streamlit/static/static/js/8427.bd0a7cf3.chunk.js
 streamlit/static/static/js/8477.de889fe5.chunk.js
 streamlit/static/static/js/8492.0d93bd08.chunk.js
 streamlit/static/static/js/8536.f8de3d9a.chunk.js
 streamlit/static/static/js/8570.6de19120.chunk.js
 streamlit/static/static/js/8691.9ccf7f89.chunk.js
 streamlit/static/static/js/9330.2b4c99e0.chunk.js
 streamlit/static/static/js/9336.2d95d840.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
 streamlit/static/static/js/9656.8c935274.chunk.js
-streamlit/static/static/js/9758.6e6d8662.chunk.js
 streamlit/static/static/js/9865.fd93213d.chunk.js
-streamlit/static/static/js/main.32c71338.js
-streamlit/static/static/js/main.32c71338.js.LICENSE.txt
+streamlit/static/static/js/main.60ba1bc7.js
+streamlit/static/static/js/main.60ba1bc7.js.LICENSE.txt
 streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
 streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
 streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
```

### Comparing `streamlit_nightly-1.34.1.dev20240514/tests/testutil.py` & `streamlit_nightly-1.34.1.dev20240516/tests/testutil.py`

 * *Files identical despite different names*

