# Comparing `tmp/gluetool-2.8.tar.gz` & `tmp/gluetool-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gluetool-2.8.tar", max compression
+gzip compressed data, was "gluetool-2.9.tar", max compression
```

## Comparing `gluetool-2.8.tar` & `gluetool-2.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1072 2023-03-14 16:49:21.402618 gluetool-2.8/README.rst
--rw-r--r--   0        0        0     4522 2023-03-14 16:49:21.402618 gluetool-2.8/assets/html-log/prism.css
--rw-r--r--   0        0        0    13651 2023-03-14 16:49:21.402618 gluetool-2.8/assets/html-log/prism.js
--rw-r--r--   0        0        0   628536 2023-03-14 16:49:21.404618 gluetool-2.8/assets/html-log/semantic.min.css
--rw-r--r--   0        0        0   275730 2023-03-14 16:49:21.405618 gluetool-2.8/assets/html-log/semantic.min.js
--rw-r--r--   0        0        0      351 2023-03-14 16:49:21.406618 gluetool-2.8/gluetool/__init__.py
--rw-r--r--   0        0        0    12916 2023-03-14 16:49:21.406618 gluetool-2.8/gluetool/action.py
--rw-r--r--   0        0        0     2167 2023-03-14 16:49:21.406618 gluetool-2.8/gluetool/color.py
--rw-r--r--   0        0        0      765 2023-03-14 16:49:21.406618 gluetool-2.8/gluetool/core.moduleinfo
--rw-r--r--   0        0        0    98880 2023-11-07 13:28:48.661926 gluetool-2.8/gluetool/glue.py
--rw-r--r--   0        0        0    19758 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/help.py
--rw-r--r--   0        0        0    14613 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/html_log.py
--rw-r--r--   0        0        0    47386 2023-10-16 11:31:32.292310 gluetool-2.8/gluetool/log.py
--rw-r--r--   0        0        0     3752 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/proxy.py
--rw-r--r--   0        0        0        0 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/py.typed
--rw-r--r--   0        0        0     4254 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/pylint/__init__.py
--rw-r--r--   0        0        0     5248 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/pylint/option_default.py
--rw-r--r--   0        0        0     4698 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/pylint/shared_defined.py
--rw-r--r--   0        0        0     3221 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/pylint/unknown_option.py
--rw-r--r--   0        0        0     6265 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/result.py
--rw-r--r--   0        0        0    11350 2023-10-16 11:31:32.292310 gluetool-2.8/gluetool/sentry.py
--rw-r--r--   0        0        0     2620 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/tests/__init__.py
--rw-r--r--   0        0        0      311 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/tests/assets/parse_config/configroot/config/data_config_root_a
--rw-r--r--   0        0        0      321 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/tests/assets/parse_config/configroot/config/data_config_root_b
--rw-r--r--   0        0        0       42 2023-03-14 16:49:21.407618 gluetool-2.8/gluetool/tests/assets/parse_config/configroot/config/data_not_unicode
--rw-r--r--   0        0        0      346 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/assets/parse_config/configroota/config/data_config_root_a
--rw-r--r--   0        0        0      321 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/assets/parse_config/configrootb/config/data_config_root_b
--rw-r--r--   0        0        0     1134 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/conftest.py
--rw-r--r--   0        0        0     5550 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_core.py
--rw-r--r--   0        0        0     4395 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_error.py
--rw-r--r--   0        0        0     1024 2023-11-07 13:28:48.662926 gluetool-2.8/gluetool/tests/test_eval_context.py
--rw-r--r--   0        0        0     1280 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_help.py
--rw-r--r--   0        0        0     1996 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_json.py
--rw-r--r--   0        0        0     3564 2023-12-07 15:19:32.688916 gluetool-2.8/gluetool/tests/test_load_yaml.py
--rw-r--r--   0        0        0     2342 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_log_exception.py
--rw-r--r--   0        0        0     1288 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_logging.py
--rw-r--r--   0        0        0     4470 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_module_discovery.py
--rw-r--r--   0        0        0      573 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_new_xml_element.py
--rw-r--r--   0        0        0     3296 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_normalize_option.py
--rw-r--r--   0        0        0     1132 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_option.py
--rw-r--r--   0        0        0     5087 2023-11-07 13:28:48.662926 gluetool-2.8/gluetool/tests/test_parse_config.py
--rw-r--r--   0        0        0     1791 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_pipeline_step.py
--rw-r--r--   0        0        0      734 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_render_template.py
--rw-r--r--   0        0        0      665 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_requests.py
--rw-r--r--   0        0        0     2637 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_result.py
--rw-r--r--   0        0        0     8672 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_run_command.py
--rw-r--r--   0        0        0     8165 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_run_modules.py
--rw-r--r--   0        0        0     4738 2023-11-07 13:28:48.662926 gluetool-2.8/gluetool/tests/test_tool.py
--rw-r--r--   0        0        0      754 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_treat_url.py
--rw-r--r--   0        0        0     2813 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_utils.py
--rw-r--r--   0        0        0     1987 2023-03-14 16:49:21.408618 gluetool-2.8/gluetool/tests/test_wait.py
--rw-r--r--   0        0        0    17600 2023-12-07 15:19:32.688916 gluetool-2.8/gluetool/tool.py
--rw-r--r--   0        0        0    58625 2023-12-07 15:19:32.689916 gluetool-2.8/gluetool/utils.py
--rw-r--r--   0        0        0      165 2023-03-14 16:49:21.409618 gluetool-2.8/gluetool/version.py
--rw-r--r--   0        0        0        0 2023-03-14 16:49:21.409618 gluetool-2.8/gluetool_modules/__init__.py
--rw-r--r--   0        0        0     4062 2023-03-14 16:49:21.409618 gluetool-2.8/gluetool_modules/bash_completion.py
--rw-r--r--   0        0        0    10863 2023-03-14 16:49:21.409618 gluetool-2.8/gluetool_modules/dep_list.py
--rw-r--r--   0        0        0     7490 2023-03-14 16:49:21.409618 gluetool-2.8/gluetool_modules/yaml_pipeline.py
--rw-r--r--   0        0        0     3440 2023-12-07 18:29:01.021873 gluetool-2.8/pyproject.toml
--rw-r--r--   0        0        0     2939 1970-01-01 00:00:00.000000 gluetool-2.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-14 16:49:21.402618 gluetool-2.9/README.rst
+-rw-r--r--   0        0        0     4522 2024-03-20 21:35:08.676248 gluetool-2.9/assets/html-log/prism.css
+-rw-r--r--   0        0        0    13651 2023-03-14 16:49:21.402618 gluetool-2.9/assets/html-log/prism.js
+-rw-r--r--   0        0        0   628536 2024-03-20 21:35:08.678248 gluetool-2.9/assets/html-log/semantic.min.css
+-rw-r--r--   0        0        0   275730 2024-03-20 21:35:08.679248 gluetool-2.9/assets/html-log/semantic.min.js
+-rw-r--r--   0        0        0      351 2024-03-20 21:35:08.679248 gluetool-2.9/gluetool/__init__.py
+-rw-r--r--   0        0        0    12916 2024-03-20 21:35:08.679248 gluetool-2.9/gluetool/action.py
+-rw-r--r--   0        0        0     2167 2024-03-20 21:35:08.679248 gluetool-2.9/gluetool/color.py
+-rw-r--r--   0        0        0      765 2023-03-14 16:49:21.406618 gluetool-2.9/gluetool/core.moduleinfo
+-rw-r--r--   0        0        0    99857 2024-05-09 13:30:21.181937 gluetool-2.9/gluetool/glue.py
+-rw-r--r--   0        0        0    19758 2024-03-20 21:35:08.680248 gluetool-2.9/gluetool/help.py
+-rw-r--r--   0        0        0    14613 2024-03-20 21:35:08.680248 gluetool-2.9/gluetool/html_log.py
+-rw-r--r--   0        0        0    49286 2024-05-06 19:19:25.773823 gluetool-2.9/gluetool/log.py
+-rw-r--r--   0        0        0     3752 2024-03-20 21:35:08.680248 gluetool-2.9/gluetool/proxy.py
+-rw-r--r--   0        0        0        0 2023-03-14 16:49:21.407618 gluetool-2.9/gluetool/py.typed
+-rw-r--r--   0        0        0     4254 2024-03-20 21:35:08.680248 gluetool-2.9/gluetool/pylint/__init__.py
+-rw-r--r--   0        0        0     5248 2024-03-20 21:35:08.680248 gluetool-2.9/gluetool/pylint/option_default.py
+-rw-r--r--   0        0        0     4698 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/pylint/shared_defined.py
+-rw-r--r--   0        0        0     3221 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/pylint/unknown_option.py
+-rw-r--r--   0        0        0     6265 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/result.py
+-rw-r--r--   0        0        0    12079 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/sentry.py
+-rw-r--r--   0        0        0     2620 2024-03-24 15:19:56.144985 gluetool-2.9/gluetool/tests/__init__.py
+-rw-r--r--   0        0        0      311 2023-03-14 16:49:21.407618 gluetool-2.9/gluetool/tests/assets/parse_config/configroot/config/data_config_root_a
+-rw-r--r--   0        0        0      321 2023-03-14 16:49:21.407618 gluetool-2.9/gluetool/tests/assets/parse_config/configroot/config/data_config_root_b
+-rw-r--r--   0        0        0       42 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/tests/assets/parse_config/configroot/config/data_not_unicode
+-rw-r--r--   0        0        0      346 2023-03-14 16:49:21.408618 gluetool-2.9/gluetool/tests/assets/parse_config/configroota/config/data_config_root_a
+-rw-r--r--   0        0        0      321 2023-03-14 16:49:21.408618 gluetool-2.9/gluetool/tests/assets/parse_config/configrootb/config/data_config_root_b
+-rw-r--r--   0        0        0     1134 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/tests/conftest.py
+-rw-r--r--   0        0        0     5550 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/tests/test_core.py
+-rw-r--r--   0        0        0     4959 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/tests/test_error.py
+-rw-r--r--   0        0        0     1024 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/tests/test_eval_context.py
+-rw-r--r--   0        0        0     1280 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/tests/test_help.py
+-rw-r--r--   0        0        0     1996 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/tests/test_json.py
+-rw-r--r--   0        0        0     3564 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/tests/test_load_yaml.py
+-rw-r--r--   0        0        0     2342 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/tests/test_log_exception.py
+-rw-r--r--   0        0        0     3402 2024-05-06 19:19:25.773823 gluetool-2.9/gluetool/tests/test_logging.py
+-rw-r--r--   0        0        0     4470 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/tests/test_module_discovery.py
+-rw-r--r--   0        0        0      573 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/tests/test_new_xml_element.py
+-rw-r--r--   0        0        0     3296 2024-03-20 21:35:08.681248 gluetool-2.9/gluetool/tests/test_normalize_option.py
+-rw-r--r--   0        0        0     1132 2024-03-20 21:35:08.682248 gluetool-2.9/gluetool/tests/test_option.py
+-rw-r--r--   0        0        0     5087 2024-03-20 21:35:08.682248 gluetool-2.9/gluetool/tests/test_parse_config.py
+-rw-r--r--   0        0        0     1791 2024-03-20 21:35:08.682248 gluetool-2.9/gluetool/tests/test_pipeline_step.py
+-rw-r--r--   0        0        0      734 2024-03-20 21:35:08.682248 gluetool-2.9/gluetool/tests/test_render_template.py
+-rw-r--r--   0        0        0      665 2024-03-20 21:35:08.682248 gluetool-2.9/gluetool/tests/test_requests.py
+-rw-r--r--   0        0        0     2637 2024-03-20 21:35:08.682248 gluetool-2.9/gluetool/tests/test_result.py
+-rw-r--r--   0        0        0     8672 2024-03-20 21:35:08.682248 gluetool-2.9/gluetool/tests/test_run_command.py
+-rw-r--r--   0        0        0     8165 2024-03-20 21:35:08.682248 gluetool-2.9/gluetool/tests/test_run_modules.py
+-rw-r--r--   0        0        0     4864 2024-05-09 13:30:21.181937 gluetool-2.9/gluetool/tests/test_tool.py
+-rw-r--r--   0        0        0      754 2024-03-20 21:35:08.682248 gluetool-2.9/gluetool/tests/test_treat_url.py
+-rw-r--r--   0        0        0     2813 2024-03-20 21:35:08.682248 gluetool-2.9/gluetool/tests/test_utils.py
+-rw-r--r--   0        0        0     1987 2024-03-20 21:35:08.682248 gluetool-2.9/gluetool/tests/test_wait.py
+-rw-r--r--   0        0        0    18292 2024-05-09 13:30:21.181937 gluetool-2.9/gluetool/tool.py
+-rw-r--r--   0        0        0    58658 2024-05-06 19:19:25.774823 gluetool-2.9/gluetool/utils.py
+-rw-r--r--   0        0        0      165 2024-03-20 21:35:08.682248 gluetool-2.9/gluetool/version.py
+-rw-r--r--   0        0        0        0 2023-03-14 16:49:21.409618 gluetool-2.9/gluetool_modules/__init__.py
+-rw-r--r--   0        0        0     4062 2024-03-20 21:35:08.683248 gluetool-2.9/gluetool_modules/bash_completion.py
+-rw-r--r--   0        0        0    10863 2024-03-20 21:35:08.683248 gluetool-2.9/gluetool_modules/dep_list.py
+-rw-r--r--   0        0        0     7490 2024-03-20 21:35:08.683248 gluetool-2.9/gluetool_modules/yaml_pipeline.py
+-rw-r--r--   0        0        0     3440 2024-05-09 14:03:11.805930 gluetool-2.9/pyproject.toml
+-rw-r--r--   0        0        0     2939 1970-01-01 00:00:00.000000 gluetool-2.9/PKG-INFO
```

### Comparing `gluetool-2.8/README.rst` & `gluetool-2.9/README.rst`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/assets/html-log/prism.css` & `gluetool-2.9/assets/html-log/prism.css`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/assets/html-log/prism.js` & `gluetool-2.9/assets/html-log/prism.js`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/assets/html-log/semantic.min.css` & `gluetool-2.9/assets/html-log/semantic.min.css`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/assets/html-log/semantic.min.js` & `gluetool-2.9/assets/html-log/semantic.min.js`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/action.py` & `gluetool-2.9/gluetool/action.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/color.py` & `gluetool-2.9/gluetool/color.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/core.moduleinfo` & `gluetool-2.9/gluetool/core.moduleinfo`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/glue.py` & `gluetool-2.9/gluetool/glue.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import jinja2
 import mock
 import pkg_resources
 
 from .action import Action
 from .color import Colors, switch as switch_colors
 from .help import LineWrapRawTextHelpFormatter, option_help, docstring_to_help, trim_docstring, eval_context_help
-from .log import Logging, LoggerMixin, ContextAdapter, ModuleAdapter, log_dict, VERBOSE
+from .log import Logging, LoggerMixin, Topic, ContextAdapter, ModuleAdapter, log_dict, VERBOSE
 
 # Type annotations
 # pylint: disable=unused-import,wrong-import-order
 from typing import TYPE_CHECKING, cast, overload, Any, Callable, Dict, Iterable, List, Optional, NoReturn  # noqa
 from typing import Sequence, Tuple, Type, Union, NamedTuple  # noqa
 from types import TracebackType  # noqa
 from .log import LoggingFunctionType, ExceptionInfoType  # noqa
@@ -1740,15 +1740,24 @@
                 'help': """
                         List of child process names which will have whole process tree terminated.
                         By default only the child process is terminated and  it is left to them to terminate
                         their children. (Default: none)
                         """,
                 'action': 'append',
                 'default': []
-            }
+            },
+            'terminate-process-group-leftovers': {
+                'help': """
+                        Terminate any leftover processes in the process group. This is done after terminating
+                        the process tree. For example, Ansible detaches some processes from the pipeline process
+                        tree, which can cause the pipeline execution to hang until these processes have finished.
+                        """,
+                'action': 'store_true',
+                'default': False
+            },
         }),
         ('Output control', {
             ('c', 'colors'): {
                 'help': 'Colorize logging on the terminal',
                 'action': 'store_true'
             },
             ('d', 'debug'): {
@@ -1789,14 +1798,20 @@
             ('o', 'debug-file', 'output'): {
                 'help': 'Log messages with at least ``DEBUG`` level are sent to this file.'
             },
             'verbose-file': {
                 'help': 'Log messages with ``VERBOSE`` level sent to this file.',
                 'default': None
             },
+            'log-topic': {
+                'help': 'If specified, also emit logs for the given topics.',
+                'default': None,
+                'choices': [topic.value for topic in Topic],
+                'action': 'append'
+            },
             ('p', 'pid'): {
                 'help': 'Log PID of gluetool process',
                 'action': 'store_true'
             },
             ('q', 'quiet'): {
                 'help': 'Silence info messages',
                 'action': 'store_true'
@@ -2477,27 +2492,31 @@
         debug_file = self.option('debug-file')
         verbose_file = self.option('verbose-file')
         json_file = self.option('json-file')
         json_file_pretty = normalize_bool_option(self.option('json-file-pretty'))
         json_output = normalize_bool_option(self.option('json-output'))
         json_output_pretty = normalize_bool_option(self.option('json-output-pretty'))
 
+        from .utils import normalize_multistring_option
+        topics = set(Topic(topic) for topic in normalize_multistring_option(self.option('log-topic')))
+
         if debug_file and not verbose_file:
             verbose_file = '{}.verbose'.format(debug_file)
 
         Logging.setup_logger(
             level=level,
             debug_file=debug_file,
             verbose_file=verbose_file,
             json_file=json_file,
             json_file_pretty=json_file_pretty,
             json_output=json_output,
             json_output_pretty=json_output_pretty,
             sentry=self._sentry,
-            show_traceback=normalize_bool_option(self.option('show-traceback'))
+            show_traceback=normalize_bool_option(self.option('show-traceback')),
+            topics=topics
         )
 
         if level == logging.DEBUG and not verbose_file:
             # pylint: disable=line-too-long
             self.warn('Debug output enabled but no verbose destination set.')
             self.warn('Either use ``-v`` to display verbose messages on screen, or ``--verbose-file`` to store them in a file.')
```

### Comparing `gluetool-2.8/gluetool/help.py` & `gluetool-2.9/gluetool/help.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/html_log.py` & `gluetool-2.9/gluetool/html_log.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/log.py` & `gluetool-2.9/gluetool/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
          super(Foo, self).__init__(logger)
 
          self.debug('foo!')
 """
 
 import atexit
 import contextlib
+import enum
 import hashlib
 import json
 import logging
 import os
 import sys
 import time
 import traceback
@@ -47,15 +48,15 @@
 import tabulate
 from six import PY2, ensure_str, ensure_binary, iteritems, iterkeys
 
 from .color import Colors
 
 # Type annotations
 # pylint: disable=unused-import,wrong-import-order,line-too-long
-from typing import TYPE_CHECKING, Any, AnyStr, Callable, Dict, Iterable, List, MutableMapping, Optional, Tuple, Type, Union, cast  # noqa
+from typing import TYPE_CHECKING, Any, AnyStr, Callable, Dict, Iterable, List, MutableMapping, Optional, Set, Tuple, Type, Union, cast  # noqa
 from types import TracebackType  # noqa
 from mypy_extensions import Arg, DefaultArg, NamedArg, DefaultNamedArg, VarArg, KwArg  # noqa
 import bs4  # noqa
 
 if TYPE_CHECKING:
     # pylint: disable=cyclic-import
     import gluetool  # noqa
@@ -78,15 +79,16 @@
 ]
 
 LoggingFunctionType = Callable[
     [
         Arg(str),
         DefaultNamedArg(ExceptionInfoType, 'exc_info'),  # noqa: F821
         DefaultNamedArg(Dict[str, Any], 'extra'),  # noqa: F821
-        DefaultNamedArg(bool, 'sentry')  # noqa: F821
+        DefaultNamedArg(bool, 'sentry'),  # noqa: F821
+        DefaultNamedArg(Optional['Topic'], 'topic')  # noqa: F821
     ],
     None
 ]
 
 ContextInfoType = Tuple[int, Any]
 
 
@@ -118,14 +120,18 @@
         {{ name }} = {{ frame.f_locals[name] }}
     {%- endfor %}
 {% endfor %}
 ---^---^---^---^---^---^----------^---^---^---^---^---^---
 """
 
 
+class Topic(enum.Enum):
+    EVAL_CONTEXT = 'eval-context'
+
+
 class BlobLogger(object):
     """
     Context manager to help with "real time" logging - some code may produce output continuously,
     e.g. when running a command and streaming its output to our stdout, and yet we still want to
     wrap it with boundaries and add a header.
 
     This code:
@@ -308,15 +314,15 @@
     """
 
     prettyfied: str = element.prettify()
 
     return prettyfied
 
 
-def log_dict(writer: LoggingFunctionType, intro: str, data: Any) -> None:
+def log_dict(writer: LoggingFunctionType, intro: str, data: Any, topic: Optional[Topic] = None) -> None:
 
     """
     Log structured data, e.g. JSON responses or a Python ``list``.
 
     .. note::
 
        For logging unstructured "blobs" of text, use :py:func:`gluetool.log.log_blob`. It does not
@@ -340,77 +346,81 @@
        If you need more formatting, or you wish to fit more information into a single message, using
        logger methods with ``format_dict`` is a way to go, while for logging a single structure ``log_dict``
        is more suitable.
 
     :param callable writer: A function which is used to actually log the text. Usually a one of some logger methods.
     :param str intro: Label to show what is the meaning of the logged structure.
     :param str blob: The actual data to log.
+    :param Topic topic: Log topic to use.
     """
 
     writer('{}:\n{}'.format(intro, format_dict(data)), extra={
         'raw_intro': intro,
         'raw_struct': data
-    })
+    }, topic=topic)
 
 
-def log_blob(writer: LoggingFunctionType, intro: str, blob: AnyStr) -> None:
+def log_blob(writer: LoggingFunctionType, intro: str, blob: AnyStr, topic: Optional[Topic] = None) -> None:
 
     """
     Log "blob" of characters of unknown structure, e.g. output of a command or response
     of a HTTP request. The blob is preceded by a header and followed by a footer to mark
     exactly the blob boundaries.
 
     .. note::
 
        For logging structured data, e.g. JSON or Python structures, use :py:func:`gluetool.log.log_dict`. It will
        make structure of the data more visible, resulting in better readability of the log.
 
     :param callable writer: A function which is used to actually log the text. Usually a one of some logger methods.
     :param str intro: Label to show what is the meaning of the logged blob.
     :param str blob: The actual blob of text.
+    :param Topic topic: Log topic to use.
     """
 
     writer("{}:\n{}".format(intro, format_blob(blob)), extra={
         'raw_intro': intro,
         'raw_blob': blob
-    })
+    }, topic=topic)
 
 
-def log_table(writer: LoggingFunctionType, intro: str, table: Iterable[Iterable[str]], **kwargs: Any) -> None:
+def log_table(
+        writer: LoggingFunctionType, intro: str, table: Iterable[Iterable[str]],
+        topic: Optional[Topic] = None, **kwargs: Any) -> None:
 
     """
     Log a formatted table.
 
     All keyword arguments are passed to :py:meth:`format_table` call which does the actual formatting.
 
     :param callable writer: A function which is used to actually log the text. Usually a one of some logger methods.
     :param str intro: Label to show what is the meaning of the logged table.
     :param list(list()) table: table to format.
     """
 
     writer('{}:\n{}'.format(intro, format_table(table, **kwargs)), extra={
         'raw_intro': intro,
         'raw_table': table
-    })
+    }, topic=topic)
 
 
-def log_xml(writer: LoggingFunctionType, intro: str, element: bs4.BeautifulSoup) -> None:
+def log_xml(writer: LoggingFunctionType, intro: str, element: bs4.BeautifulSoup, topic: Optional[Topic] = None) -> None:
 
     """
     Log an XML element, e.g. Beaker job description.
 
     :param callable writer: A function which is used to actually log the text. Usually a one of some logger methods.
     :param str intro: Label to show what is the meaning of the logged blob.
     :param element: XML element to log.
     """
 
     writer("{}:\n{}".format(intro, format_xml(element)), extra={
         'raw_intro': intro,
         'raw_xml': element
-    })
+    }, topic=topic)
 
 
 # pylint: disable=invalid-name
 def _extract_stack(tb: Any) -> List[Any]:
     """
     Construct a "stack" by merging two sources of data:
 
@@ -581,34 +591,40 @@
         # method. Note that we took care about removing any contexts from adapter's `extra` and from the `extra`
         # parameter.
         extra.update(self.extra)  # type: ignore  # `self.extra` does exist
 
         # Force aggregation store into the `extra` parameter - it may have been missing, see the initialization above.
         extra['contexts'] = contexts
 
+        # Add log topic
+        extra['topic'] = kwargs.get('topic')
+        del kwargs['topic']
+
         # Save updated `extra` value back to `kwargs`. It may have been `None`, but from now on it's a dictionary,
         # with an item dedicated to context aggregation.
         kwargs['extra'] = extra
 
         return msg, kwargs
 
     # pylint: disable=too-many-arguments,arguments-differ
     def log(self,  # type: ignore  #  Signature of "log" incompatible with supertype "LoggerAdapter"
             level: int,
             msg: str,
             exc_info: Optional[ExceptionInfoType] = None,
             extra: Optional[Dict[str, Any]] = None,
-            sentry: bool = False) -> None:
+            sentry: bool = False,
+            topic: Optional[Topic] = None) -> None:
 
         msg, kwargs = self.process(
             msg,
             # yes, process doesn't accept **kwargs...
             {
                 'exc_info': exc_info,
-                'extra': extra
+                'extra': extra,
+                'topic': topic
             }
         )
 
         self._logger.log(level, msg, **kwargs)
 
         if sentry and Logging.sentry:
             Logging.sentry.submit_message(msg, logger=self)
@@ -617,15 +633,16 @@
 
         return self._logger.isEnabledFor(level)
 
     def verbose(self,
                 msg: str,
                 exc_info: Optional[ExceptionInfoType] = None,
                 extra: Optional[Dict[str, Any]] = None,
-                sentry: bool = False) -> None:
+                sentry: bool = False,
+                topic: Optional[Topic] = None) -> None:
 
         if not self.isEnabledFor(VERBOSE):
             return
 
         # When we are expected to emit record of VERBOSE level, make a DEBUG note
         # as well, to "link" debug and verbose outputs. With this, one might read
         # DEBUG log, and use this reference to find corresponding VERBOSE record.
@@ -658,66 +675,71 @@
                 hint = msg[0:new_line_index]
 
             else:
                 hint = '{}...'.format(msg[0:keep_len])
 
         placeholder_message = '{} (See "verbose" log for the actual message)'.format(hint)
 
-        self.log(logging.DEBUG, placeholder_message, exc_info=exc_info, extra=extra, sentry=sentry)
-        self.log(VERBOSE, msg, exc_info=exc_info, extra=extra, sentry=sentry)
+        self.log(logging.DEBUG, placeholder_message, exc_info=exc_info, extra=extra, sentry=sentry, topic=topic)
+        self.log(VERBOSE, msg, exc_info=exc_info, extra=extra, sentry=sentry, topic=topic)
 
     # Disabling type checking of logging methods' signatures - they differ from supertype's signatures
     # but that is on purpose.
 
     # pylint: disable=arguments-differ
     def debug(self,  # type: ignore
               msg: str,
               exc_info: Optional[ExceptionInfoType] = None,
               extra: Optional[Dict[str, Any]] = None,
-              sentry: bool = False) -> None:
+              sentry: bool = False,
+              topic: Optional[Topic] = None) -> None:
 
-        self.log(logging.DEBUG, msg, exc_info=exc_info, extra=extra, sentry=sentry)
+        self.log(logging.DEBUG, msg, exc_info=exc_info, extra=extra, sentry=sentry, topic=topic)
 
     # pylint: disable=arguments-differ
     def info(self,   # type: ignore
              msg: str,
              exc_info: Optional[ExceptionInfoType] = None,
              extra: Optional[Dict[str, Any]] = None,
-             sentry: bool = False) -> None:
+             sentry: bool = False,
+             topic: Optional[Topic] = None) -> None:
 
-        self.log(logging.INFO, msg, exc_info=exc_info, extra=extra, sentry=sentry)
+        self.log(logging.INFO, msg, exc_info=exc_info, extra=extra, sentry=sentry, topic=topic)
 
     # pylint: disable=arguments-differ
     def warning(self,   # type: ignore
                 msg: str,
                 exc_info: Optional[ExceptionInfoType] = None,
                 extra: Optional[Dict[str, Any]] = None,
-                sentry: bool = False) -> None:
+                sentry: bool = False,
+                topic: Optional[Topic] = None) -> None:
 
-        self.log(logging.WARNING, msg, exc_info=exc_info, extra=extra, sentry=sentry)
+        self.log(logging.WARNING, msg, exc_info=exc_info, extra=extra, sentry=sentry, topic=topic)
 
     warn = warning  # type: ignore
 
     # pylint: disable=arguments-differ
     def error(self,   # type: ignore
               msg: str,
               exc_info: Optional[ExceptionInfoType] = None,
               extra: Optional[Dict[str, Any]] = None,
-              sentry: bool = False) -> None:
+              sentry: bool = False,
+              topic: Optional[Topic] = None) -> None:
 
-        self.log(logging.ERROR, msg, exc_info=exc_info, extra=extra, sentry=sentry)
+        self.log(logging.ERROR, msg, exc_info=exc_info, extra=extra, sentry=sentry, topic=topic)
 
     # pylint: disable=arguments-differ
     def exception(self,   # type: ignore
                   msg: str,
                   exc_info: Optional[ExceptionInfoType] = None,
                   extra: Optional[Dict[str, Any]] = None,
-                  sentry: bool = False) -> None:
+                  sentry: bool = False,
+                  topic: Optional[Topic] = None) -> None:
 
-        self.log(logging.ERROR, msg, exc_info=exc_info, extra=extra, sentry=sentry)
+        self.log(logging.ERROR, msg, exc_info=exc_info, extra=extra, sentry=sentry, topic=topic)
 
 
 class ModuleAdapter(ContextAdapter):
     """
     Custom logger adapter, adding module name as a context.
 
     :param logger: parent logger this adapter modifies.
@@ -1051,14 +1073,17 @@
 
     debug_file_handler = None
     verbose_file_handler = None
     json_file_handler = None
 
     sentry: Optional['gluetool.sentry.Sentry'] = None
 
+    #: Logging topics
+    topics: Set[Topic]
+
     @staticmethod
     def get_logger() -> ContextAdapter:
 
         """
         Returns a logger-like object suitable for logging stuff.
 
         :rtype: ContextAdapter
@@ -1141,19 +1166,19 @@
     OUR_LOGGERS = (
         logging.getLogger('gluetool'),
         logging.getLogger('jaeger_tracing'),
         logging.getLogger('urllib3')
     )
 
     @staticmethod
-    def _setup_log_file(filepath: str,
+    def _setup_log_file(filepath: str,  # pylint: disable=too-many-arguments
                         level: int,
                         limit_level: bool = False,
                         formatter_class: Type[Union[LoggingFormatter, JSONLoggingFormatter]] = LoggingFormatter,
-                        prettify: bool = False
+                        prettify: bool = False,
                        ) -> Optional[logging.FileHandler]:  # noqa
 
         if filepath is None:
             return None
 
         if limit_level:
             handler: logging.FileHandler = SingleLogLevelFileHandler(level, filepath, 'w')
@@ -1179,25 +1204,46 @@
 
         atexit.register(_close_log_file)
 
         Logging.get_logger().debug("created output file '{}'".format(filepath))
 
         return handler
 
+    @staticmethod
+    def add_topic_filter() -> None:
+
+        def _topic_filter(record: logging.LogRecord) -> bool:
+            topic = getattr(record, 'topic', None)
+
+            # record has no topic
+            if not topic:
+                return True
+
+            # topic in enabled log topics
+            if topic in Logging.topics:
+                return True
+
+            # log topic of the record not enabled
+            return False
+
+        assert Logging.logger
+        Logging.logger.addFilter(_topic_filter)
+
     # pylint: disable=too-many-arguments,line-too-long
     @staticmethod
     def setup_logger(level: int = DEFAULT_LOG_LEVEL,
                      debug_file: Optional[str] = None,
                      verbose_file: Optional[str] = None,
                      json_file: Optional[str] = None,
                      json_file_pretty: bool = False,
                      json_output: bool = False,
                      json_output_pretty: bool = False,
                      sentry: Optional['gluetool.sentry.Sentry'] = None,
-                     show_traceback: bool = False
+                     show_traceback: bool = False,
+                     topics: Optional[Set[Topic]] = None
                     ) -> ContextAdapter:  # noqa
 
         """
         Create and setup logger.
 
         This method is called at least twice:
 
@@ -1217,20 +1263,23 @@
             JSON structures.
         :param int level: desired log level. One of constants defined in :py:mod:`logging` module,
             e.g. :py:data:`logging.DEBUG` or :py:data:`logging.ERROR`.
         :param bool sentry: if set, logger will be augmented to send every log message to the Sentry
             server.
         :param bool show_traceback: if set, exception tracebacks would be sent to ``stderr`` handler
             as well as to the debug file.
+        :param list(Topic) topics: list of topics to log
         :rtype: ContextAdapter
         :returns: a :py:class:`ContextAdapter` instance, set up for logging.
         """
 
         level = level or logging.INFO
 
+        Logging.topics = topics or set()
+
         # store for later use by configure_logger & co.
         Logging.sentry = sentry
 
         if Logging.logger is None:
             # we're doing the very first setup of logging handlers, therefore create new stderr handler,
             # configure it and attach it to correct places
             Logging.stderr_handler = logging.StreamHandler()
@@ -1270,28 +1319,32 @@
                 formatter_class=JSONLoggingFormatter,
                 prettify=json_file_pretty
             )
 
         # now our main logger should definitely exist and it should be usable
         logger = Logging.get_logger()
 
-        logger.debug('logger setup: level={}, debug file={}, verbose file={}, json file={}, sentry={}, show traceback={}'.format(
+        logger.debug('logger setup: level={}, debug file={}, verbose file={}, json file={}, sentry={}, show traceback={}, topics={}'.format(  # Ignore: PEP8Bear
             level,
             debug_file,
             verbose_file,
             json_file,
             'yes' if sentry else 'no',
-            show_traceback
+            show_traceback,
+            ','.join([topic.value for topic in topics]) if topics else None
         ))
 
         # Enable debug and verbose files
         Logging.enable_debug_file(logger)
         Logging.enable_verbose_file(logger)
         Logging.enable_json_file(logger)
 
+        # Add topics filter
+        Logging.add_topic_filter()
+
         list(map(Logging.enable_debug_file, Logging.OUR_LOGGERS))
         list(map(Logging.enable_verbose_file, Logging.OUR_LOGGERS))
         list(map(Logging.enable_json_file, Logging.OUR_LOGGERS))
 
         return logger
```

### Comparing `gluetool-2.8/gluetool/proxy.py` & `gluetool-2.9/gluetool/proxy.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/pylint/__init__.py` & `gluetool-2.9/gluetool/pylint/__init__.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/pylint/option_default.py` & `gluetool-2.9/gluetool/pylint/option_default.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/pylint/shared_defined.py` & `gluetool-2.9/gluetool/pylint/shared_defined.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/pylint/unknown_option.py` & `gluetool-2.9/gluetool/pylint/unknown_option.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/result.py` & `gluetool-2.9/gluetool/result.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/sentry.py` & `gluetool-2.9/gluetool/sentry.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,22 +67,26 @@
     :param str tags_map_env_var: Name of environment variable setting mapping between environment
         variables and additional tags. Set to ``None`` to disable adding these tags.
     """
 
     def __init__(self,
                  dsn_env_var: Optional[str] = 'SENTRY_DSN',
                  base_url_env_var: Optional[str] = 'SENTRY_BASE_URL',
+                 event_url_template_env_var: Optional[str] = 'SENTRY_EVENT_URL_TEMPLATE',
                  tags_map_env_var: Optional[str] = 'SENTRY_TAG_MAP') -> None:
 
         self._client = None
         self._base_url = None
 
         if base_url_env_var:
             self._base_url = os.environ.get(base_url_env_var, None)
 
+        if event_url_template_env_var:
+            self._event_url_template = os.environ.get(event_url_template_env_var, None)
+
         self._tag_map: Dict[str, str] = {}
 
         if tags_map_env_var and os.environ.get(tags_map_env_var):
             try:
                 for pair in os.environ[tags_map_env_var].split(','):
                     tag, env_var = pair.split('=')
                     self._tag_map[env_var.strip()] = tag.strip()
@@ -149,18 +153,34 @@
         is returned instead.
 
         :param str event_id: ID of the Sentry event, e.g. the one returned by
             :py:meth:`submit_exception` or :py:meth:`submit_warning`.
         :param gluetool.log.ContextAdapter logger: logger to use for logging.
         """
 
-        if not self._base_url:
-            return None
+        if self._event_url_template:
+            try:
+                event_url = gluetool.utils.render_template(
+                    self._event_url_template,
+                    logger=logger,
+                    EVENT_ID=event_id
+                )
+
+            except gluetool.GlueError as exc:
+                if logger:
+                    logger.warning(f"Could not render Sentry event URL template: {exc}")
+
+                return None
+
+            return gluetool.utils.treat_url(event_url, logger=logger)
+
+        if self._base_url:
+            return gluetool.utils.treat_url('{}/?query={}'.format(self._base_url, event_id), logger=logger)
 
-        return gluetool.utils.treat_url('{}/?query={}'.format(self._base_url, event_id), logger=logger)
+        return None
 
     @staticmethod
     def log_issue(failure: Optional[gluetool.glue.Failure],
                   logger: Optional[gluetool.log.ContextAdapter] = None) -> None:
 
         """
         Nicely log issue and possibly its URL.
```

### Comparing `gluetool-2.8/gluetool/tests/__init__.py` & `gluetool-2.9/gluetool/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/conftest.py` & `gluetool-2.9/gluetool/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_core.py` & `gluetool-2.9/gluetool/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_error.py` & `gluetool-2.9/gluetool/tests/test_error.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pytest
 import six
 
 from mock import MagicMock
 from hypothesis import example, given, strategies as st
 
 import gluetool
+import gluetool.sentry
 from gluetool import GlueError
 
 
 @given(message=st.text(string.printable))
 def test_message(message):
     with pytest.raises(GlueError) as excinfo:
         raise GlueError(message)
@@ -89,14 +90,27 @@
     expected = current.copy()
     if explicit:
         expected.update(explicit)
 
     assert GlueError('', sentry_tags=explicit).sentry_tags(current) == expected
 
 
+def test_sentry_event_url_template(monkeypatch):
+    monkeypatch.setenv('SENTRY_BASE_URL', 'https://foo.bar/')
+    monkeypatch.setenv('SENTRY_EVENT_URL_TEMPLATE', 'https://foo.bar/?event_id={{ EVENT_ID }}')
+
+    assert gluetool.sentry.Sentry().event_url('dummy-event-id') == 'https://foo.bar/?event_id=dummy-event-id'
+
+
+def test_sentry_event_url_base_url(monkeypatch):
+    monkeypatch.setenv('SENTRY_BASE_URL', 'https://foo.bar/')
+
+    assert gluetool.sentry.Sentry().event_url('dummy-event-id') == 'https://foo.bar/?query=dummy-event-id'
+
+
 @given(cmd=st.lists(st.text(string.printable)), exit_code=st.integers())
 def test_command_error(cmd, exit_code):
     stringified = [six.ensure_str(s) for s in cmd]
 
     mock_output = MagicMock(exit_code=exit_code)
 
     exc = gluetool.GlueCommandError(stringified, mock_output)
```

### Comparing `gluetool-2.8/gluetool/tests/test_eval_context.py` & `gluetool-2.9/gluetool/tests/test_eval_context.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_help.py` & `gluetool-2.9/gluetool/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_json.py` & `gluetool-2.9/gluetool/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_load_yaml.py` & `gluetool-2.9/gluetool/tests/test_load_yaml.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_log_exception.py` & `gluetool-2.9/gluetool/tests/test_log_exception.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_module_discovery.py` & `gluetool-2.9/gluetool/tests/test_module_discovery.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_new_xml_element.py` & `gluetool-2.9/gluetool/tests/test_new_xml_element.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_normalize_option.py` & `gluetool-2.9/gluetool/tests/test_normalize_option.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_option.py` & `gluetool-2.9/gluetool/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_parse_config.py` & `gluetool-2.9/gluetool/tests/test_parse_config.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_pipeline_step.py` & `gluetool-2.9/gluetool/tests/test_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_render_template.py` & `gluetool-2.9/gluetool/tests/test_render_template.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_requests.py` & `gluetool-2.9/gluetool/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_result.py` & `gluetool-2.9/gluetool/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_run_command.py` & `gluetool-2.9/gluetool/tests/test_run_command.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_run_modules.py` & `gluetool-2.9/gluetool/tests/test_run_modules.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_tool.py` & `gluetool-2.9/gluetool/tests/test_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=blacklisted-name
 
 import logging
 import os
+import re
 import signal
 import subprocess
 
 import pkg_resources
 import pytest
 from mock import MagicMock
 
@@ -131,20 +132,26 @@
     # * we expect that at least one sleep command receives both signals
     # * log.match can match whole strings only, and we have no idea what the PID of sleep processes will be
     assert log.match(levelno=logging.WARNING, message="Sending SIGTERM to child process 'sh' (PID {})".format(process.pid))
 
     sleep_sigterm = any(
             True
             for record in log.records
-            if record.message.startswith("Sending SIGTERM to child process 'sleep'") and record.levelno == logging.WARNING
+            if re.match(
+                r"Sending SIGTERM to (?:grand)?child process 'sleep'.*",
+                record.message
+            ) and record.levelno == logging.WARNING
         )
     sleep_sigkill = any(
             True
             for record in log.records
-            if record.message.startswith("Sending SIGKILL to child process 'sleep'") and record.levelno == logging.WARNING
+            if re.match(
+                r"Sending SIGKILL to (?:grand)?child process 'sleep'.*",
+                record.message
+            ) and record.levelno == logging.WARNING
         )
 
     # sleep should be terminated only if terminate_process_tree set, because it is a child process of `sh`
     if terminate_process_tree:
         assert sleep_sigterm
         assert sleep_sigkill
     else:
```

### Comparing `gluetool-2.8/gluetool/tests/test_treat_url.py` & `gluetool-2.9/gluetool/tests/test_treat_url.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_utils.py` & `gluetool-2.9/gluetool/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tests/test_wait.py` & `gluetool-2.9/gluetool/tests/test_wait.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool/tool.py` & `gluetool-2.9/gluetool/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,33 +293,46 @@
 
         # Python installs SIGINT handler that translates signal to
         # a KeyboardInterrupt exception. It's so good we want to use
         # it for SIGTERM as well, just wrap the handler with some logging.
         orig_sigint_handler = signal.getsignal(signal.SIGINT)
         sigmap = {getattr(signal, name): name for name in [name for name in dir(signal) if name.startswith('SIG')]}
 
-        def _terminate_or_kill(child: psutil.Process) -> None:
-            Glue.warn("Sending SIGTERM to child process '{}' (PID {})".format(child.name(), child.pid))
+        def _terminate_or_kill(child: psutil.Process, description: str) -> None:
+            Glue.warn("Sending SIGTERM to {} process '{}' (PID {})".format(description, child.name(), child.pid))
             child.terminate()
 
             try:
                 child.wait(timeout=DEFAULT_SIGTERM_TIMEOUT)
 
             except psutil.TimeoutExpired:
                 Glue.warn("Sending SIGKILL to child process '{}' (PID {})".format(child.name(), child.pid))
                 child.kill()
 
         def _terminate_children() -> None:
+            process = psutil.Process()
+
             # Terminate child processes. For children marked by `--terminate-process-tree` terminate whole process tree.
             terminate_process_tree = gluetool.utils.normalize_multistring_option(Glue.option('terminate-process-tree'))
-            for child in psutil.Process().children():
+            for child in process.children():
                 if child.name() in terminate_process_tree:
                     for process in sorted(child.children(recursive=True), key=lambda x: x.pid, reverse=True):
-                        _terminate_or_kill(process)
-                _terminate_or_kill(child)
+                        _terminate_or_kill(process, "grandchild")
+                _terminate_or_kill(child, "child")
+
+            # Terminate leftover processes in the same proccess group. For children marked by `--terminate-process-tree`
+            # terminate whole process tree.
+            if Glue.option('terminate-process-group-leftovers'):
+                process_pgid = os.getpgid(process.pid)
+                leftovers = [
+                    proc for proc in psutil.process_iter(attrs=['pid'])
+                    if os.getpgid(proc.pid) == process_pgid and proc.pid != process.pid
+                ]
+                for process in leftovers:
+                    _terminate_or_kill(process, "process group leftover")
 
         def _signal_handler(signum: int,
                             frame: Optional[FrameType],
                             handler: Optional[Callable[[int, FrameType], None]] = None,
                             msg: Optional[str] = None) -> Any:
 
             msg = msg or 'Signal {} received'.format(sigmap[signum])
```

### Comparing `gluetool-2.8/gluetool/utils.py` & `gluetool-2.9/gluetool/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import requests as original_requests
 import ruamel.yaml
 import cattrs
 import cattrs.strategies
 
 from .glue import GlueError, SoftGlueError, GlueCommandError
 from .result import Result
-from .log import Logging, ContextAdapter, PackageAdapter, LoggerMixin, BlobLogger, \
+from .log import Logging, ContextAdapter, PackageAdapter, LoggerMixin, BlobLogger, Topic, \
     log_blob, log_dict, print_wrapper
 
 # Type annotations
 # pylint: disable=unused-import, wrong-import-order
 from typing import IO, cast, overload  # noqa
 from typing import (Any, Callable, Deque, Dict, List, Optional, Pattern, Tuple, TypeVar, Union, Generic, Type,
                     TYPE_CHECKING)  # noqa
@@ -969,15 +969,15 @@
 
     try:
         def _render(template: jinja2.Template, source: str) -> str:
 
             assert logger is not None
 
             log_blob(logger.debug, 'rendering template', source)
-            log_dict(logger.verbose, 'context', kwargs)
+            log_dict(logger.verbose, 'context', kwargs, topic=Topic.EVAL_CONTEXT)
 
             return ensure_str(template.render(**kwargs).strip())
 
         if isinstance(template, six.string_types):
             return _render(jinja2.Template(template), template)
 
         if isinstance(template, jinja2.environment.Template):
```

### Comparing `gluetool-2.8/gluetool_modules/bash_completion.py` & `gluetool-2.9/gluetool_modules/bash_completion.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool_modules/dep_list.py` & `gluetool-2.9/gluetool_modules/dep_list.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/gluetool_modules/yaml_pipeline.py` & `gluetool-2.9/gluetool_modules/yaml_pipeline.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.8/pyproject.toml` & `gluetool-2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gluetool"
-version = "2.8"
+version = "2.9"
 description = "Python framework for constructing command-line pipelines."
 authors = [
   "Milos Prchlik <mprchlik@redhat.com>",
   "Miroslav Vadkerti <mvadkert@redhat.com>",
   "Martin Kluson <mkluson@redhat.com>",
   "Ondrej Ptak <optak@redhat.com>",
   "Evgeny Fedin <efedin@redhat.com>",
```

### Comparing `gluetool-2.8/PKG-INFO` & `gluetool-2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluetool
-Version: 2.8
+Version: 2.9
 Summary: Python framework for constructing command-line pipelines.
 Home-page: https://gluetool.readthedocs.org/
 License: BSD
 Author: Milos Prchlik
 Author-email: mprchlik@redhat.com
 Requires-Python: >=3.8,<3.10
 Classifier: Development Status :: 5 - Production/Stable
```

