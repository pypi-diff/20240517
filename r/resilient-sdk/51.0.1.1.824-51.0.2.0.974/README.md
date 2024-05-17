# Comparing `tmp/resilient_sdk-51.0.1.1.824.tar.gz` & `tmp/resilient_sdk-51.0.2.0.974.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_sdk-51.0.1.1.824.tar", last modified: Wed Apr  3 15:17:18 2024, max compression
+gzip compressed data, was "resilient_sdk-51.0.2.0.974.tar", last modified: Fri May 17 18:37:35 2024, max compression
```

## Comparing `resilient_sdk-51.0.1.1.824.tar` & `resilient_sdk-51.0.2.0.974.tar`

### file list

```diff
@@ -1,263 +1,263 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.478412 resilient_sdk-51.0.1.1.824/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13053 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     3212 2024-04-03 15:17:18.478412 resilient_sdk-51.0.1.1.824/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2385 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/assets/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    62353 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/assets/IBM_Security_lockup_pos_RGB.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6685 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/app.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)      551 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8255 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/base_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36395 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/clone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37325 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/codegen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11406 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/dev.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38221 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/docgen.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/ext/
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/ext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8309 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/ext/ext_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7664 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/extract.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13591 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8693 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/run_init.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47981 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/validate.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/
--rw-rw-r--   0 travis    (2000) travis    (2000)      608 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      432 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/MANIFEST.in.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/README.md.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2686 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      534 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/
--rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/LICENSE.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      145 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/__init__.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/components/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/components/__init__.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3131 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/lib/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/lib/__init__.py.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     7935 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/__init__.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_close_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_update_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)    10817 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/__init__.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      962 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5425 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/data/export.res.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/payload_samples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/blank.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_fail.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_success.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/tests/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3132 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      750 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/docgen/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/docgen/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16666 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/docgen/templates/README.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/ext/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/ext/icons/
--rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/ext/icons/app_logo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/ext/icons/company_logo.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/run_init/
--rw-rw-r--   0 travis    (2000) travis    (2000)      146 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/run_init/app.config.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      847 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/run_init/sdk_settings.json.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/validate/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18106 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/validate/.pylintrc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/data/validate/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/data/validate/templates/validate_report.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/resilient_sdk/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9174 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3006 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/jinja2_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54989 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/package_file_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3104 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/resilient_objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      817 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3168 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_genson_overwrites.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73816 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27552 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_validate_configs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86804 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_validate_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3388 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_validate_issue.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.290412 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3212 2024-04-03 15:17:18.000000 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    16016 2024-04-03 15:17:18.000000 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:17:18.000000 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2024-04-03 15:17:18.000000 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-04-03 15:17:18.000000 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2024-04-03 15:17:18.000000 resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1399 2024-04-03 15:17:18.478412 resilient_sdk-51.0.1.1.824/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20369 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3785 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.294412 resilient_sdk-51.0.1.1.824/tests/integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/integration/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1227 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/integration/test_installation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.298412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      806 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/.mock_sdk_settings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    19566 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)        3 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)    24687 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_app.log
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   224427 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    58851 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_export.resz
--rw-rw-r--   0 travis    (2000) travis    (2000)   223680 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_export_corrupt.res
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.298412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/
--rw-rw-r--   0 travis    (2000) travis    (2000)      627 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    57247 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   191223 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/customize_old.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.298412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/
--rw-rw-r--   0 travis    (2000) travis    (2000)    66751 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    41671 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    41951 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     2773 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   539206 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    46693 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_export_w_playbook_w_scripts.res
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.298412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)      394 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile
--rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile.old
--rw-rw-r--   0 travis    (2000) travis    (2000)      214 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5843 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1619 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.330412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5148 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      712 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.330412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/
--rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      566 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.330412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.330412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2254 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3465 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.330412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6889 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.334412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.362412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_close_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_update_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)    10660 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.366412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.366412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    49696 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.366412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/
--rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.286412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.398412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.434412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.438412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.438412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.470412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2325 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2381 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      741 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)    53354 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/setup_callable_data.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/setup_py_lines.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   413882 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_reload_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_xml_test_report.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.474412 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)  3278485 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)   594886 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/export.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/orgs.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/session.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_mock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3008 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/shared_mock_data/sdk_mock_paths.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.474412 resilient_sdk-51.0.1.1.824/tests/unit/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1838 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_app.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.474412 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.474412 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/ext/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/ext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6929 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/ext/test_ext_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2070 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_base_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20811 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_clone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34428 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_codegen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4953 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_dev.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19150 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_docgen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1247 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_extract.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8611 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9712 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_run_init.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23814 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_validate.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:18.478412 resilient_sdk-51.0.1.1.824/tests/unit/test_util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2148 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_jinja_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21936 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_package_file_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_resilient_objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      470 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      947 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34738 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3948 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_validate_configs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47084 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_validate_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_validate_issue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2024-04-03 15:15:23.000000 resilient_sdk-51.0.1.1.824/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.311164 resilient_sdk-51.0.2.0.974/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13601 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/CHANGES
+-rw-r--r--   0 travis    (2000) travis    (2000)     3717 2024-05-17 18:37:35.311164 resilient_sdk-51.0.2.0.974/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2385 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.103164 resilient_sdk-51.0.2.0.974/assets/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    62353 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/assets/IBM_Security_lockup_pos_RGB.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.103164 resilient_sdk-51.0.2.0.974/resilient_sdk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6685 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/app.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.107164 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      551 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8255 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/base_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36395 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/clone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37325 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/codegen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11406 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/dev.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38411 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/docgen.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.107164 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/ext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/ext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8309 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/ext/ext_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7664 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/extract.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13591 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/list.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8693 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/run_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48139 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/validate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.099164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.099164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.099164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.107164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      608 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      432 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/MANIFEST.in.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/README.md.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.107164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2686 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      534 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.099164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/doc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.107164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.107164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/LICENSE.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      172 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/__init__.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.107164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/components/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/components/__init__.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3131 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.107164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/lib/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/lib/__init__.py.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7935 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.107164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/poller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/poller/__init__.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.107164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/poller/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_close_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_update_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10865 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.107164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/util/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/util/__init__.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      962 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5425 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.107164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/util/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/util/data/export.res.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.099164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/payload_samples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.111164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/blank.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_fail.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_success.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.111164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/tests/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3132 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      750 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.099164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/docgen/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.111164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/docgen/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16751 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/docgen/templates/README.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.099164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/ext/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.111164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/ext/icons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/ext/icons/app_logo.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/ext/icons/company_logo.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.111164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/run_init/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      146 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/run_init/app.config.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      847 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/run_init/sdk_settings.json.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.111164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/validate/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18106 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/validate/.pylintrc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.111164 resilient_sdk-51.0.2.0.974/resilient_sdk/data/validate/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/data/validate/templates/validate_report.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.111164 resilient_sdk-51.0.2.0.974/resilient_sdk/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9239 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/util/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2990 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/util/jinja2_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55369 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/util/package_file_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3104 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/util/resilient_objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      817 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3168 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_genson_overwrites.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74468 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29102 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_validate_configs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90761 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_validate_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3388 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_validate_issue.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.311164 resilient_sdk-51.0.2.0.974/resilient_sdk.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     3717 2024-05-17 18:37:34.000000 resilient_sdk-51.0.2.0.974/resilient_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16016 2024-05-17 18:37:35.000000 resilient_sdk-51.0.2.0.974/resilient_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:37:34.000000 resilient_sdk-51.0.2.0.974/resilient_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       57 2024-05-17 18:37:34.000000 resilient_sdk-51.0.2.0.974/resilient_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      239 2024-05-17 18:37:34.000000 resilient_sdk-51.0.2.0.974/resilient_sdk.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2024-05-17 18:37:34.000000 resilient_sdk-51.0.2.0.974/resilient_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-05-17 18:37:35.315164 resilient_sdk-51.0.2.0.974/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.111164 resilient_sdk-51.0.2.0.974/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20886 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3785 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.111164 resilient_sdk-51.0.2.0.974/tests/integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/integration/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1227 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/integration/test_installation.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.115164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      806 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/.mock_sdk_settings.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19566 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)        3 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24687 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_app.log
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   224427 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58851 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_export.resz
+-rw-rw-r--   0 travis    (2000) travis    (2000)   223680 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_export_corrupt.res
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.119164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      627 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    57247 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   191223 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/customize_old.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.119164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_app_zip_files/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    66751 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41671 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41951 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2773 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   539206 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46693 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_export_w_playbook_w_scripts.res
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.099164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.123164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      394 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile.old
+-rw-rw-r--   0 travis    (2000) travis    (2000)      214 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5843 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1619 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.123164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5148 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      712 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.103164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.123164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      566 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.159164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       30 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      271 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.159164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2254 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3465 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.159164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6889 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.163164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.163164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_close_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_update_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10660 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.195164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      591 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.195164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49696 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.199164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.103164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.227164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.231164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.263164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.263164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.295164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2325 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2381 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      741 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53354 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/setup_callable_data.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/setup_py_lines.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   413882 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_reload_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_xml_test_report.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.303164 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/resilient_api_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  3278485 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)   594886 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/resilient_api_data/export.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/resilient_api_data/orgs.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/resilient_api_data/session.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/resilient_api_mock.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3008 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/shared_mock_data/sdk_mock_paths.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.303164 resilient_sdk-51.0.2.0.974/tests/unit/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1809 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_app.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.307164 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.307164 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/ext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/ext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6929 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/ext/test_ext_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2070 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_base_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20811 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_clone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34428 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_codegen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4953 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_dev.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19822 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_docgen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1247 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_extract.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8611 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_list.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9712 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_run_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23814 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_validate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:37:35.311164 resilient_sdk-51.0.2.0.974/tests/unit/test_util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2623 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_jinja_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22754 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_package_file_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_resilient_objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      470 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_sdk_argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      947 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_sdk_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36060 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_sdk_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3948 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_sdk_validate_configs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64542 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_sdk_validate_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_sdk_validate_issue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1082 2024-05-17 18:36:00.000000 resilient_sdk-51.0.2.0.974/tox.ini
```

### Comparing `resilient_sdk-51.0.1.1.824/CHANGES` & `resilient_sdk-51.0.2.0.974/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+**2024-05: version 51.0.2.0**
+
+* Added official support for Python 3.12
+* Improved the ``docgen`` command for export files to eliminate duplicate objects
+* The ``gather-results`` feature of the ``codegen`` command now clears out sensitive host values
+* The ``validate`` command now checks apps for any playbooks which are dependent on SOAR objects
+  that might not have been included in during the ``codegen`` process. Developers should still be
+  sure to test their apps in a staging environments to ensure that all objects are properly packaged
+
 **2024-04: version 51.0.1.1**
 
 * No major changes. Just bumping build number to coincide with other builds
 
 **2024-02: version 51.0.1.0**
 
 * All SOAR Python libraries now officially support Python 3.11
```

### Comparing `resilient_sdk-51.0.1.1.824/PKG-INFO` & `resilient_sdk-51.0.2.0.974/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 Metadata-Version: 2.1
 Name: resilient_sdk
-Version: 51.0.1.1.824
+Version: 51.0.2.0.974
 Summary: Python SDK for developing Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-sdk
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
 Project-URL: Change Log, https://ibm.biz/resilient-sdk-changes
 Keywords: ibm,soar,resilient,resilient-circuits,circuits,resilient-sdk,sdk
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.12,>=2.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7
 Description-Content-Type: text/markdown; charset=UTF-8
+Requires-Dist: resilient>=51.0.2.0
+Requires-Dist: packaging~=24.0; python_version > "3.6"
+Requires-Dist: jinja2~=3.1; python_version > "3.6"
+Requires-Dist: genson~=1.3; python_version > "3.6"
+Requires-Dist: packaging~=21.3; python_version == "3.6"
+Requires-Dist: jinja2~=3.0; python_version == "3.6"
+Requires-Dist: genson==1.2; python_version <= "3.6"
+Requires-Dist: jinja2~=2.0; python_version == "2.7"
+Requires-Dist: packaging~=20.9; python_version == "2.7"
 
 ![IBM Security](https://raw.githubusercontent.com/ibmresilient/resilient-python-api/master/resilient-sdk/assets/IBM_Security_lockup_pos_RGB.png)
 
 # IBM SOAR SDK
 
 
 ## Overview
```

### Comparing `resilient_sdk-51.0.1.1.824/README.md` & `resilient_sdk-51.0.2.0.974/README.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/assets/IBM_Security_lockup_pos_RGB.png` & `resilient_sdk-51.0.2.0.974/assets/IBM_Security_lockup_pos_RGB.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/LICENSE` & `resilient_sdk-51.0.2.0.974/resilient_sdk/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/app.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/app.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/__init__.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/base_cmd.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/base_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/clone.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/clone.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/codegen.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/codegen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/dev.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/dev.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/docgen.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/docgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     def _get_pre_and_post_processing_scripts_from_playbooks(the_function, playbooks, scripts, export):
         """
         Look through all playbooks in the export, searching for any that
         use the function in question. If any do, if the function instance
         uses a pre-processing script, use that as the pre-processing script.
         If any scripts in the playbook reference the output of the function
         in their script (we do a very specific search which looks for Python
-        code (not comments) that reference the specific string 
+        code (not comments) that reference the specific string
         ``playbook.functions.results.<output_name>``), then use that script
         as an example post-processing script. If none are found in local
         scripts, search the global scripts of the export
 
         :param the_function: the function in question for which we want example scripts
         :type the_function: dict
         :param playbooks: list of playbooks in the export
@@ -174,15 +174,15 @@
             # loop through the playbook to find its functions
             for pb_fn in pb_objects.get("functions", []):
                 # the best proxy we have for "post processing" script is
                 # if the output name of the function is used in the script's
                 # code. we check for that there and if so, we've found a
                 # "post processing" script
 
-                # This regex searches for Python code instances of the 
+                # This regex searches for Python code instances of the
                 # output. It is relatively robust and will not match commented code
                 # nor non-exact matches
                 # For examples on this regex, see: https://regex101.com/r/Fv5AQm
                 regex_str = r"^(?!#).*playbook\.functions\.results\.{0}\b.*".format(pb_fn.get("result_name"))
                 regex_compiled = re.compile(regex_str, re.MULTILINE)
 
 
@@ -750,22 +750,22 @@
             "author": requirements_obj.get("setup_py_attributes", {}).get("author"),
             "support_url": requirements_obj.get("setup_py_attributes", {}).get("url"),
             "res_circuits_dependency_str": requirements_obj.get("res_circuits_dep_str"),
             "supported_app": requirements_obj.get("supported_app"),
             "app_configs": requirements_obj.get("jinja_app_configs", [{},{}])[1],
 
             # lists of customizations (make unique)
-            "functions": package_helpers.make_list_of_dicts_unique(jinja_functions),
-            "scripts": package_helpers.make_list_of_dicts_unique(jinja_scripts),
-            "rules": package_helpers.make_list_of_dicts_unique(jinja_rules),
-            "datatables": package_helpers.make_list_of_dicts_unique(jinja_datatables),
-            "custom_fields": package_helpers.make_list_of_dicts_unique(jinja_custom_fields),
-            "custom_artifact_types": package_helpers.make_list_of_dicts_unique(jinja_custom_artifact_types),
-            "playbooks": package_helpers.make_list_of_dicts_unique(jinja_playbooks),
-            "apps": package_helpers.make_list_of_dicts_unique(jinja_apps),
+            "functions": package_helpers.make_list_of_dicts_unique(jinja_functions, lambda x: x["anchor"]),
+            "scripts": package_helpers.make_list_of_dicts_unique(jinja_scripts, lambda x: x["anchor"]),
+            "rules": package_helpers.make_list_of_dicts_unique(jinja_rules, lambda x: x["name"]),
+            "datatables": package_helpers.make_list_of_dicts_unique(jinja_datatables, lambda x: x["anchor"]),
+            "custom_fields": package_helpers.make_list_of_dicts_unique(jinja_custom_fields, lambda x: x["api_name"]),
+            "custom_artifact_types": package_helpers.make_list_of_dicts_unique(jinja_custom_artifact_types, lambda x: x["api_name"]),
+            "playbooks": package_helpers.make_list_of_dicts_unique(jinja_playbooks, lambda x: x["api_name"]),
+            "apps": package_helpers.make_list_of_dicts_unique(jinja_apps, lambda x: x["export_key"]),
 
             # constants
             "placeholder_string": constants.DOCGEN_PLACEHOLDER_STRING,
             "poller_flag": args.poller,
             "poller_templates": requirements_obj.get("poller_templates", {}),
             "sdk_version": sdk_helpers.get_resilient_sdk_version(),
             "docgen_export": requirements_obj.get("docgen_export", False)
```

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/ext/ext_package.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/ext/ext_package.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/extract.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/extract.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/list.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/list.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/run_init.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/run_init.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/cmds/validate.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/cmds/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,18 @@
 
 
 # optional parameters are skipped if they aren't included in the setup.py
 SETUP_OPTIONAL_ATTRS = ("python_requires", "author_email")
 
 
 class CmdValidate(BaseCmd):
-    """TODO Docstring"""
+    """
+    Command to run SDK validate on a package. Provides static validations (file checks)
+    as well as dynamic validations (selftest, unit tests, etc...)
+    """
 
     CMD_NAME = "validate"
     CMD_HELP = "Tests the content of all files associated with the app, including code, before packaging it. Only Python >= 3.6 supported."
     CMD_USAGE = """
     $ resilient-sdk validate -p <name_of_package>
     $ resilient-sdk validate -p <name_of_package> -c '/usr/custom_app.config'
     $ resilient-sdk validate -p <name_of_package> --validate
@@ -171,15 +174,15 @@
         self._log(constants.VALIDATE_LOG_LEVEL_INFO, "\nSee the detailed report at {0}".format(path_report))
 
 
         return path_report
 
     def _run_main_validation(self, args):
         """
-        TODO: docstring, unit tests
+        Run all validations (no flags provided)
         """
         self._log(constants.VALIDATE_LOG_LEVEL_INFO, "{0}Running main validation{0}".format(constants.LOG_DIVIDER))
         self._validate(args)
         self._run_selftest(args)
         self._run_tests(args)
         self._run_pylint_scan(args)
         self._run_bandit_scan(args)
@@ -487,15 +490,15 @@
         # get package name and package version
         parsed_setup = package_helpers.parse_setup_py(os.path.join(path_package, package_helpers.BASE_NAME_SETUP_PY), ["name", "version"])
         package_name = parsed_setup.get("name")
         package_version = parsed_setup.get("version")
 
         attributes = validation_configurations.package_files
 
-        for filename,attr_dict in attributes:
+        for filename, attr_dict in attributes:
 
             # if a specific path is required for this file, it will be specified in the "path" attribute
             if attr_dict.get("path"):
                 path_file = os.path.join(path_package, attr_dict.get("path").format(package_name))
             else:
                 # otherwise the file is in root package directory
                 path_file = os.path.join(path_package, filename)
```

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     # <add additional initialization steps for your endpoint as necessary>
 
     return app_common
 
 def query_entities(app_common, last_poller_time):
     """
-    Method call to query the endpoint solution for newly created or 
+    Method call to query the endpoint solution for newly created or
     modified entities for synchronization with IBM SOAR
 
     :param app_common: class for app API calls
     :type app_common: obj
     :param last_poller_time: timestamp in milliseconds to collect the changed entities (alerts, cases, etc.)
     :type last_poller_time: int
     :return: list of entities to synchronize with SOAR
@@ -192,17 +192,18 @@
         The logic is to determine if a SOAR case needs to be created, updated or closed, and
         apply the correct template file to apply the field changes.
 
         :param query_results: list of endpoint entities to check against SOAR cases
         :type query_results: list
         """
 
-        try:
-            cases_insert = cases_closed = cases_updated = 0
-            for entity in query_results:
+        cases_insert = cases_closed = cases_updated = 0
+        entity_id = None
+        for entity in query_results:
+            try:
                 entity_id = get_entity_id(entity)
 
                 # create linkback url
                 entity["entity_url"] = self.app_common.make_linkback_url(entity_id)
 
                 # determine if this is an existing SOAR case
                 soar_case, _error_msg = self.soar_common.get_soar_case({ SOAR_ENTITY_ID_FIELD: entity_id }, open_cases=False)
@@ -245,12 +246,12 @@
                             entity)
                         _update_soar_case = self.soar_common.update_soar_case(
                             soar_case_id,
                             soar_update_payload)
 
                         cases_updated += 1
                         LOG.info("Updated SOAR case %s from %s %s", soar_case_id, ENTITY_LABEL, entity_id)
+            except Exception as err:
+                LOG.error("%s poller run failed for entity %s: %s", PACKAGE_NAME, entity_id, str(err))
 
-            LOG.info("IBM SOAR cases created: %s, cases closed: %s, cases updated: %s",
-                     cases_insert, cases_closed, cases_updated)
-        except Exception as err:
-            LOG.error("%s poller run failed: %s", PACKAGE_NAME, str(err))
+        LOG.info("IBM SOAR cases created: %s, cases closed: %s, cases updated: %s",
+                    cases_insert, cases_closed, cases_updated)
```

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/docgen/templates/README.md.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/docgen/templates/README.md.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 {% endif %}
 - [Troubleshooting & Support](#troubleshooting--support)
 
 ---
 
 ## Release Notes
 <!--
-  Specify all changes in this release. Do not remove the release 
+  Specify all changes in this release. Do not remove the release
   notes of a previous release
 -->
 | Version | Date | Notes |
 | ------- | ---- | ----- |
 | 1.0.0 | MM/YYYY | Initial Release | <!-- {{ placeholder_string }} -->
 
 ---
@@ -102,62 +102,62 @@
 * Key Feature 2 <!-- {{ placeholder_string }} -->
 * Key Feature 3 <!-- {{ placeholder_string }} -->
 
 ---
 
 ## Requirements
 <!--
-  List any Requirements 
---> 
+  List any Requirements
+-->
 <!-- {{ placeholder_string }} -->
 This app supports the IBM Security QRadar SOAR Platform and the IBM Security QRadar SOAR for IBM Cloud Pak for Security.
 
 ### SOAR platform
 The SOAR platform supports two app deployment mechanisms, Edge Gateway (also known as App Host) and integration server.
 
 If deploying to a SOAR platform with an App Host, the requirements are:
 * SOAR platform >= `{{ server_version }}`.
 * The app is in a container-based format (available from the AppExchange as a `zip` file).
 
 If deploying to a SOAR platform with an integration server, the requirements are:
 * SOAR platform >= `{{ server_version }}`.
 * The app is in the older integration format (available from the AppExchange as a `zip` file which contains a `tar.gz` file).
 * Integration server is running `{{ res_circuits_dependency_str }}`.
-* If using an API key account, make sure the account provides the following minimum permissions: 
+* If using an API key account, make sure the account provides the following minimum permissions:
   | Name | Permissions |
   | ---- | ----------- |
   | Org Data | Read |
   | Function | Read |
   <!-- {{ placeholder_string }} -->
 
-The following SOAR platform guides provide additional information: 
-* _Edge Gateway Deployment Guide_ or _App Host Deployment Guide_: provides installation, configuration, and troubleshooting information, including proxy server settings. 
+The following SOAR platform guides provide additional information:
+* _Edge Gateway Deployment Guide_ or _App Host Deployment Guide_: provides installation, configuration, and troubleshooting information, including proxy server settings.
 * _Integration Server Guide_: provides installation, configuration, and troubleshooting information, including proxy server settings.
-* _System Administrator Guide_: provides the procedure to install, configure and deploy apps. 
+* _System Administrator Guide_: provides the procedure to install, configure and deploy apps.
 
 The above guides are available on the IBM Documentation website at [ibm.biz/soar-docs](https://ibm.biz/soar-docs). On this web page, select your SOAR platform version. On the follow-on page, you can find the _Edge Gateway Deployment Guide_, _App Host Deployment Guide_, or _Integration Server Guide_ by expanding **Apps** in the Table of Contents pane. The System Administrator Guide is available by expanding **System Administrator**.
 
 ### Cloud Pak for Security
 If you are deploying to IBM Cloud Pak for Security, the requirements are:
 * IBM Cloud Pak for Security >= `1.10.15`.
 * Cloud Pak is configured with an Edge Gateway.
 * The app is in a container-based format (available from the AppExchange as a `zip` file).
 
-The following Cloud Pak guides provide additional information: 
+The following Cloud Pak guides provide additional information:
 * _Edge Gateway Deployment Guide_ or _App Host Deployment Guide_: provides installation, configuration, and troubleshooting information, including proxy server settings. From the Table of Contents, select Case Management and Orchestration & Automation > **Orchestration and Automation Apps**.
 * _System Administrator Guide_: provides information to install, configure, and deploy apps. From the IBM Cloud Pak for Security IBM Documentation table of contents, select Case Management and Orchestration & Automation > **System administrator**.
 
 These guides are available on the IBM Documentation website at [ibm.biz/cp4s-docs](https://ibm.biz/cp4s-docs). From this web page, select your IBM Cloud Pak for Security version. From the version-specific IBM Documentation page, select Case Management and Orchestration & Automation.
 
 ### Proxy Server
 The app **does/does not** <!-- {{ placeholder_string }} --> support a proxy server.
 
-{% if all_dependencies %}
 ### Python Environment
-Python 3.6 and Python 3.9 are supported.
+Python 3.9, 3.11, and 3.12 are officially supported. When deployed as an app, the app runs on Python 3.11.
+{% if all_dependencies %}
 Additional package dependencies may exist for each of these packages:
 {% for dep in all_dependencies|sort %}
 * {{dep}}
 {% endfor %}
 {% endif %}
 
 ### <!-- {{ placeholder_string }} --> Development Version
@@ -247,15 +247,15 @@
 
 Minimum SOAR version required for this export: `{{ server_version }}` (NOTE: this may be higher than each app's minimum required version).
 
 {% if apps %}
 ### Apps Included with Export
 | App | Version | Minimum SOAR Version |
 | --- | ------- | -------------------- |
-{% for app in apps %}
+{% for app in apps|sort(attribute="display_name") %}
 | {{ app.display_name }} | {{ app.version }} | {{ app.minimum_resilient_version.version }} |
 {% endfor %}
 {% else %} {# else no apps #}
 
 ### Apps Required
 <!--
 List any apps required to install with the exports
@@ -302,15 +302,15 @@
     # TODO: Generate an example of the Function Output within this code block.
     # To get the output of a Function:
     #   1. Run resilient-circuits in DEBUG mode: $ resilient-circuits run --loglevel=DEBUG
     #   2. Invoke the Function in SOAR
     #   3. Gather the results using: $ resilient-sdk codegen -p {{ name_underscore }} --gather-results
     #   4. Run docgen again: $ resilient-sdk docgen -p {{ name_underscore }}
     # Or simply paste example outputs manually here. Be sure to remove any personal information
-} 
+}
 ```
 {% endif %}
 
 </p>
 </details>
 
 <details><summary>Example Function Input Script:</summary>
@@ -400,15 +400,15 @@
 ---
 {% endfor %}
 
 {% if custom_fields %}
 ## Custom Fields
 | Label | API Access Name | Type | Prefix | Placeholder | Tooltip |
 | ----- | --------------- | ---- | ------ | ----------- | ------- |
-{% for f in custom_fields|sort(attribute="api_name") %}
+{% for f in custom_fields|sort(attribute="label") %}
 | {{ f.label }} | `{{ f.api_name }}` | `{{ f.type }}` | `{{ f.prefix }}` | {{ f.placeholder }} | {{ f.tooltip }} |
 {% endfor %}
 
 ---
 {% endif %}
 
 {% if custom_artifact_types %}
```

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/ext/icons/app_logo.png` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/ext/icons/app_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/ext/icons/company_logo.png` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/ext/icons/company_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/run_init/sdk_settings.json.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/run_init/sdk_settings.json.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/validate/.pylintrc` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/validate/.pylintrc`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/data/validate/templates/validate_report.md.jinja2` & `resilient_sdk-51.0.2.0.974/resilient_sdk/data/validate/templates/validate_report.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/util/constants.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/util/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 LOGGER_NAME = "resilient_sdk_log"
 LOG_DIVIDER = "\n------------------------\n"
 ENV_VAR_DEV = "RES_SDK_DEV"
 ENV_VAR_APP_CONFIG_FILE = "APP_CONFIG_FILE"
 
 # UPDATE BEFORE RELEASING NEW VERSION
-RESILIENT_LIBRARIES_VERSION = "51.0.1.1.0"
-RESILIENT_LIBRARIES_VERSION_DEV = "51.0.1.1.0"
+RESILIENT_LIBRARIES_VERSION = "51.0.2.0.0"
+RESILIENT_LIBRARIES_VERSION_DEV = "51.0.2.0.0"
 
 RESILIENT_VERSION_WITH_PROXY_SUPPORT = (42, 0, 0)
 CURRENT_SOAR_SERVER_VERSION = None
 MIN_SOAR_SERVER_VERSION_PLAYBOOKS = parse_version("44.0")
 # new SOAR versioning schema introduced in v51.0.0.x
 # use "51.0.0" rather than "51.0.0.0" so that sonarqube
 # won't flag as an IP address...
@@ -133,14 +133,15 @@
 CODEGEN_DEFAULT_SETUP_PY_LICENSE = "<<insert here>>"
 CODEGEN_DEFAULT_SETUP_PY_AUTHOR = "<<your name here>>"
 CODEGEN_DEFAULT_SETUP_PY_EMAIL = "you@example.com"
 CODEGEN_DEFAULT_SETUP_PY_URL = "<<your company url>>"
 CODEGEN_DEFAULT_SETUP_PY_LONG_DESC = "<<{}>> Enter a long description, including the key features of the App. \\\\\\nMultiple continuation lines are supported with a backslash. Line breaks are supported too:\\n<br>- This will be rendered like a list\\n<br>- once the App is installed in SOAR".format(DOCGEN_PLACEHOLDER_STRING)
 CODEGEN_DEFAULT_LICENSE_CONTENT = "<<PUT YOUR LICENSE TEXT HERE>>"
 CODEGEN_DEFAULT_COPYRIGHT_CONTENT = "<<PUT YOUR COPYRIGHT TEXT HERE>>"
+CODEGEN_PAYLOAD_SAMPLES_CLEAR_HOST_DEFAULT_VALUE = "my.app.host"
 
 # resilient-sdk init internal defaults
 INIT_INTERNAL_AUTHOR = "IBM SOAR"
 INIT_INTERNAL_AUTHOR_EMAIL = ""
 INIT_INTERNAL_URL = "https://ibm.com/mysupport"
 INIT_INTERNAL_LICENSE = "MIT"
 INIT_INTERNAL_LONG_DESC = "Links: \
```

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/util/jinja2_filters.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/util/jinja2_filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,27 +43,27 @@
     return re.sub(r"([0-9a-z_]+\-*\.py)", r"`\1`", val)
 
 
 def _scrub_ansi(val):
     """
     Return a value with all all ansi color codes removed
     """
-    return re.sub(r"\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])", r"", val) 
+    return re.sub(r"\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])", r"", val)
 
 
 def _convert_to_code(val):
     """
     Convert ' to code(`) or ''' code blocks(```) and convert ' within code blocks to "
       e.g.: 'display_name' converts to `display_name`
       e.g.: '''pip install -U 'resilient-circuits'''' converts to
             ```shell
             $ pip install -U "resilient-circuits"
             ```
     """
-    return re.sub(r"'{3}(.*)'(.*)'(.*)'{3}", r'\n\n```shell\n$ \1"\2"\3\n```\n', val).replace("'", "`").replace("\t\t", "\t")
+    return re.sub(r"'{3}(.*?)'{3}", r'\n\n```shell\n$ \1\n```\n', val).replace("'", "`").replace("\t\t", "\t")
 
 
 def _defaults_to_code(val):
     """
     Make sure that any defaults that are surrounded by << >>  are in code quotes so that they render properly.
       e.g.: <<display_name>> converts to '<<display_name>>'
     """
```

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/util/package_file_helpers.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/util/package_file_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import struct
 import sys
 import tempfile
 import zipfile
 from collections import defaultdict
 
 import pkg_resources
+from packaging.version import parse
 from resilient import ImportDefinition
 from resilient_sdk.util import constants, sdk_helpers
 from resilient_sdk.util.resilient_objects import (DEFAULT_INCIDENT_TYPE_UUID,
                                                   ResilientObjMap)
 from resilient_sdk.util.sdk_exception import SDKException
 
 if sys.version_info.major < 3:
@@ -1024,15 +1025,15 @@
     :param python_requires_str: str representation of the value assosciated with the 'python_requires' attr in setup.py
     :raise SDKException: if format of python_requires is not correct (i.e. in '>=<version>' format)
     :return: return the minimum required python version or None if not found
     :rtype: tuple with (<major>, <minor>) version format
     """
     try:
         version_str = re.match(r"(?:>=)([0-9]+[\.0-9]*)", python_requires_str).groups()[0]
-        version = pkg_resources.parse_version(version_str)
+        version = parse(version_str)
 
         return sdk_helpers.parse_version_object(version)
     except AttributeError as e:
         raise SDKException("'python_requires' version not given in correct format.")
 
 def check_package_installed(package_name):
     """
@@ -1217,26 +1218,31 @@
         "$ pip install -U resilient-sdk"
     ])
 
     w = "{0}\n{1}\n{2}\n\n{3}\n\t{4}\n{0}".format(colored_lines[0], colored_lines[1], colored_lines[2], colored_lines[3], colored_lines[4])
 
     LOG.warning(w)
 
-def make_list_of_dicts_unique(list_of_dicts):
+def make_list_of_dicts_unique(list_of_dicts, uniqueness_key_func = None):
     """
     Creates temporary dictionary of schema str(dict):dict
     for each dict in the list, then captures the values
     of the temporary dictionary (just the dict side) and
     returns that list. The crucial part of this is that the
     temporary dictionary keys are unique -- thus guaranteeing
     that any two dictionaries whose str() cast would be the same,
     won't appear more than once in the temporary object.
 
     :param list_of_dicts: List of dictionaries to make unique
     :type list_of_dicts: list[dict]
+    :param uniqueness_key_func: key func to determine uniqueness of a given dict; defaults to str(x)
+    :type uniqueness_key_func: Callable
     :return: same list as started with with any extra duplicates removed
     :rtype: list[dict]
     """
+    if uniqueness_key_func is None:
+        # set default uniqueness function to: str(x)
+        uniqueness_key_func = str # no need for a lambda here as str(x) will work just fine
 
     # .values() only grabs each x from the unique, temporary dictionary created in-line
-    unique_list = list({str(x): x for x in list_of_dicts}.values())
+    unique_list = list({uniqueness_key_func(x): x for x in list_of_dicts}.values())
     return unique_list
```

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/util/resilient_objects.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/util/resilient_objects.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_argparse.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_argparse.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_exception.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_exception.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_genson_overwrites.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_genson_overwrites.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_helpers.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,4578 +37,4619 @@
 00000240: 7274 2072 6571 7565 7374 730a 696d 706f  rt requests.impo
 00000250: 7274 2072 6571 7565 7374 732e 6578 6365  rt requests.exce
 00000260: 7074 696f 6e73 0a66 726f 6d20 6a69 6e6a  ptions.from jinj
 00000270: 6132 2069 6d70 6f72 7420 456e 7669 726f  a2 import Enviro
 00000280: 6e6d 656e 742c 2050 6163 6b61 6765 4c6f  nment, PackageLo
 00000290: 6164 6572 0a66 726f 6d20 7061 636b 6167  ader.from packag
 000002a0: 696e 672e 7665 7273 696f 6e20 696d 706f  ing.version impo
-000002b0: 7274 2070 6172 7365 2061 7320 7061 7273  rt parse as pars
-000002c0: 655f 7665 7273 696f 6e0a 6672 6f6d 2072  e_version.from r
-000002d0: 6573 696c 6965 6e74 5f73 646b 2e75 7469  esilient_sdk.uti
-000002e0: 6c20 696d 706f 7274 2063 6f6e 7374 616e  l import constan
-000002f0: 7473 0a66 726f 6d20 7265 7369 6c69 656e  ts.from resilien
-00000300: 745f 7364 6b2e 7574 696c 2e6a 696e 6a61  t_sdk.util.jinja
-00000310: 325f 6669 6c74 6572 7320 696d 706f 7274  2_filters import
-00000320: 2061 6464 5f66 696c 7465 7273 5f74 6f5f   add_filters_to_
-00000330: 6a69 6e6a 615f 656e 760a 6672 6f6d 2072  jinja_env.from r
-00000340: 6573 696c 6965 6e74 5f73 646b 2e75 7469  esilient_sdk.uti
-00000350: 6c2e 7265 7369 6c69 656e 745f 6f62 6a65  l.resilient_obje
-00000360: 6374 7320 696d 706f 7274 2028 4445 4641  cts import (DEFA
-00000370: 554c 545f 494e 4349 4445 4e54 5f46 4945  ULT_INCIDENT_FIE
-00000380: 4c44 2c0a 2020 2020 2020 2020 2020 2020  LD,.            
-00000390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003b0: 2020 2020 2020 4445 4641 554c 545f 494e        DEFAULT_IN
-000003c0: 4349 4445 4e54 5f54 5950 452c 0a20 2020  CIDENT_TYPE,.   
+000002b0: 7274 2049 6e76 616c 6964 5665 7273 696f  rt InvalidVersio
+000002c0: 6e0a 6672 6f6d 2070 6163 6b61 6769 6e67  n.from packaging
+000002d0: 2e76 6572 7369 6f6e 2069 6d70 6f72 7420  .version import 
+000002e0: 7061 7273 6520 6173 2070 6172 7365 5f76  parse as parse_v
+000002f0: 6572 7369 6f6e 0a66 726f 6d20 7265 7369  ersion.from resi
+00000300: 6c69 656e 745f 7364 6b2e 7574 696c 2069  lient_sdk.util i
+00000310: 6d70 6f72 7420 636f 6e73 7461 6e74 730a  mport constants.
+00000320: 6672 6f6d 2072 6573 696c 6965 6e74 5f73  from resilient_s
+00000330: 646b 2e75 7469 6c2e 6a69 6e6a 6132 5f66  dk.util.jinja2_f
+00000340: 696c 7465 7273 2069 6d70 6f72 7420 6164  ilters import ad
+00000350: 645f 6669 6c74 6572 735f 746f 5f6a 696e  d_filters_to_jin
+00000360: 6a61 5f65 6e76 0a66 726f 6d20 7265 7369  ja_env.from resi
+00000370: 6c69 656e 745f 7364 6b2e 7574 696c 2e72  lient_sdk.util.r
+00000380: 6573 696c 6965 6e74 5f6f 626a 6563 7473  esilient_objects
+00000390: 2069 6d70 6f72 7420 2844 4546 4155 4c54   import (DEFAULT
+000003a0: 5f49 4e43 4944 454e 545f 4649 454c 442c  _INCIDENT_FIELD,
+000003b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000003c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003f0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-00000400: 4352 4950 545f 5459 5045 5f4d 4150 2c0a  CRIPT_TYPE_MAP,.
+000003e0: 2020 2044 4546 4155 4c54 5f49 4e43 4944     DEFAULT_INCID
+000003f0: 454e 545f 5459 5045 2c0a 2020 2020 2020  ENT_TYPE,.      
+00000400: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000440: 2020 5265 7369 6c69 656e 7446 6965 6c64    ResilientField
-00000450: 5479 7065 732c 0a20 2020 2020 2020 2020  Types,.         
-00000460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000480: 2020 2020 2020 2020 2052 6573 696c 6965           Resilie
-00000490: 6e74 4f62 6a4d 6170 2c0a 2020 2020 2020  ntObjMap,.      
+00000420: 2020 2020 2020 2020 2020 2020 5343 5249              SCRI
+00000430: 5054 5f54 5950 455f 4d41 502c 0a20 2020  PT_TYPE_MAP,.   
+00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000460: 2020 2020 2020 2020 2020 2020 2020 2052                 R
+00000470: 6573 696c 6965 6e74 4669 656c 6454 7970  esilientFieldTyp
+00000480: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00000490: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000004a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004c0: 2020 2020 2020 2020 2020 2020 5265 7369              Resi
-000004d0: 6c69 656e 7454 7970 6549 6473 290a 6672  lientTypeIds).fr
-000004e0: 6f6d 2072 6573 696c 6965 6e74 5f73 646b  om resilient_sdk
-000004f0: 2e75 7469 6c2e 7364 6b5f 6578 6365 7074  .util.sdk_except
-00000500: 696f 6e20 696d 706f 7274 2053 444b 4578  ion import SDKEx
-00000510: 6365 7074 696f 6e0a 0a66 726f 6d20 7265  ception..from re
-00000520: 7369 6c69 656e 7420 696d 706f 7274 2041  silient import A
-00000530: 7267 756d 656e 7450 6172 7365 720a 6672  rgumentParser.fr
-00000540: 6f6d 2072 6573 696c 6965 6e74 2069 6d70  om resilient imp
-00000550: 6f72 7420 636f 6e73 7461 6e74 7320 6173  ort constants as
-00000560: 2072 6573 5f63 6f6e 7374 616e 7473 0a66   res_constants.f
-00000570: 726f 6d20 7265 7369 6c69 656e 7420 696d  rom resilient im
-00000580: 706f 7274 2067 6574 5f63 6c69 656e 742c  port get_client,
-00000590: 2067 6574 5f63 6f6e 6669 675f 6669 6c65   get_config_file
-000005a0: 0a66 726f 6d20 7265 7369 6c69 656e 742e  .from resilient.
-000005b0: 6865 6c70 6572 7320 696d 706f 7274 2072  helpers import r
-000005c0: 656d 6f76 655f 7461 670a 0a69 6620 7379  emove_tag..if sy
-000005d0: 732e 7665 7273 696f 6e5f 696e 666f 2e6d  s.version_info.m
-000005e0: 616a 6f72 203c 2033 3a0a 2020 2020 2320  ajor < 3:.    # 
-000005f0: 4861 6e64 6c65 2050 5920 3220 7370 6563  Handle PY 2 spec
-00000600: 6966 6963 2069 6d70 6f72 7473 0a20 2020  ific imports.   
-00000610: 2023 204a 534f 4e44 6563 6f64 6545 7272   # JSONDecodeErr
-00000620: 6f72 2069 7320 6e6f 7420 6176 6169 6c61  or is not availa
-00000630: 626c 6520 696e 2050 5932 2e37 2073 6f20  ble in PY2.7 so 
-00000640: 7765 2073 6574 2069 7420 746f 204e 6f6e  we set it to Non
-00000650: 650a 2020 2020 4a53 4f4e 4465 636f 6465  e.    JSONDecode
-00000660: 4572 726f 7220 3d20 4e6f 6e65 0a65 6c73  Error = None.els
-00000670: 653a 0a20 2020 2023 2048 616e 646c 6520  e:.    # Handle 
-00000680: 5059 2033 2073 7065 6369 6669 6320 696d  PY 3 specific im
-00000690: 706f 7274 730a 2020 2020 2320 7265 6c6f  ports.    # relo
-000006a0: 6164 2870 6163 6b61 6765 2920 696e 2050  ad(package) in P
-000006b0: 5932 2e37 2c20 696d 706f 7274 6c69 622e  Y2.7, importlib.
-000006c0: 7265 6c6f 6164 2870 6163 6b61 6765 2920  reload(package) 
-000006d0: 696e 2050 5933 2e36 0a20 2020 2072 656c  in PY3.6.    rel
-000006e0: 6f61 6420 3d20 696d 706f 7274 6c69 622e  oad = importlib.
-000006f0: 7265 6c6f 6164 0a20 2020 2066 726f 6d20  reload.    from 
-00000700: 6a73 6f6e 2e64 6563 6f64 6572 2069 6d70  json.decoder imp
-00000710: 6f72 7420 4a53 4f4e 4465 636f 6465 4572  ort JSONDecodeEr
-00000720: 726f 720a 0a23 2054 656d 7020 6669 7820  ror..# Temp fix 
-00000730: 746f 2068 616e 646c 6520 7468 6520 7265  to handle the re
-00000740: 7369 6c69 656e 7420 6d6f 6475 6c65 206c  silient module l
-00000750: 6f67 730a 6c6f 6767 696e 672e 6765 744c  ogs.logging.getL
-00000760: 6f67 6765 7228 2272 6573 696c 6965 6e74  ogger("resilient
-00000770: 2e63 6f33 2229 2e61 6464 4861 6e64 6c65  .co3").addHandle
-00000780: 7228 6c6f 6767 696e 672e 5374 7265 616d  r(logging.Stream
-00000790: 4861 6e64 6c65 7228 2929 0a23 2047 6574  Handler()).# Get
-000007a0: 2074 6865 2073 616d 6520 6c6f 6767 6572   the same logger
-000007b0: 206f 626a 6563 7420 7468 6174 2069 7320   object that is 
-000007c0: 7573 6564 2069 6e20 6170 702e 7079 0a4c  used in app.py.L
-000007d0: 4f47 203d 206c 6f67 6769 6e67 2e67 6574  OG = logging.get
-000007e0: 4c6f 6767 6572 2863 6f6e 7374 616e 7473  Logger(constants
-000007f0: 2e4c 4f47 4745 525f 4e41 4d45 290a 0a0a  .LOGGER_NAME)...
-00000800: 6465 6620 6765 745f 7265 7369 6c69 656e  def get_resilien
-00000810: 745f 636c 6965 6e74 2870 6174 685f 636f  t_client(path_co
-00000820: 6e66 6967 5f66 696c 653d 4e6f 6e65 293a  nfig_file=None):
-00000830: 0a20 2020 2022 2222 0a20 2020 2052 6574  .    """.    Ret
-00000840: 7572 6e20 6120 5369 6d70 6c65 436c 6965  urn a SimpleClie
-00000850: 6e74 2066 6f72 2052 6573 696c 6965 6e74  nt for Resilient
-00000860: 2052 4553 5420 4150 4920 7573 696e 6720   REST API using 
-00000870: 636f 6e66 6967 7572 6174 696f 6e73 0a20  configurations. 
-00000880: 2020 206f 7074 696f 6e73 2066 726f 6d20     options from 
-00000890: 7072 6f76 6964 6564 2070 6174 685f 636f  provided path_co
-000008a0: 6e66 6967 5f66 696c 6520 6f72 2066 726f  nfig_file or fro
-000008b0: 6d20 7e2f 2e72 6573 696c 6965 6e74 2f61  m ~/.resilient/a
-000008c0: 7070 2e63 6f6e 6669 670a 0a20 2020 203a  pp.config..    :
-000008d0: 7061 7261 6d20 7061 7468 5f63 6f6e 6669  param path_confi
-000008e0: 675f 6669 6c65 3a20 5061 7468 2074 6f20  g_file: Path to 
-000008f0: 6170 702e 636f 6e66 6967 2066 696c 6520  app.config file 
-00000900: 746f 2075 7365 0a20 2020 203a 7265 7475  to use.    :retu
-00000910: 726e 3a20 5369 6d70 6c65 436c 6965 6e74  rn: SimpleClient
-00000920: 2066 6f72 2052 6573 696c 6965 6e74 2052   for Resilient R
-00000930: 4553 5420 4150 490a 2020 2020 3a72 7479  EST API.    :rty
-00000940: 7065 3a20 5369 6d70 6c65 436c 6965 6e74  pe: SimpleClient
-00000950: 0a20 2020 2022 2222 0a0a 2020 2020 6966  .    """..    if
-00000960: 206e 6f74 2070 6174 685f 636f 6e66 6967   not path_config
-00000970: 5f66 696c 653a 0a20 2020 2020 2020 2070  _file:.        p
-00000980: 6174 685f 636f 6e66 6967 5f66 696c 6520  ath_config_file 
-00000990: 3d20 6765 745f 636f 6e66 6967 5f66 696c  = get_config_fil
-000009a0: 6528 290a 0a20 2020 204c 4f47 2e64 6562  e()..    LOG.deb
-000009b0: 7567 2822 5573 696e 6720 6170 702e 636f  ug("Using app.co
-000009c0: 6e66 6967 2066 696c 6520 6174 3a20 2573  nfig file at: %s
-000009d0: 222c 2070 6174 685f 636f 6e66 6967 5f66  ", path_config_f
-000009e0: 696c 6529 0a0a 2020 2020 636f 6e66 6967  ile)..    config
-000009f0: 5f70 6172 7365 7220 3d20 4172 6775 6d65  _parser = Argume
-00000a00: 6e74 5061 7273 6572 2863 6f6e 6669 675f  ntParser(config_
-00000a10: 6669 6c65 3d70 6174 685f 636f 6e66 6967  file=path_config
-00000a20: 5f66 696c 6529 0a20 2020 206f 7074 7320  _file).    opts 
-00000a30: 3d20 636f 6e66 6967 5f70 6172 7365 722e  = config_parser.
-00000a40: 7061 7273 655f 6b6e 6f77 6e5f 6172 6773  parse_known_args
-00000a50: 2829 5b30 5d0a 0a20 2020 204c 4f47 2e69  ()[0]..    LOG.i
-00000a60: 6e66 6f28 2243 6f6e 6e65 6374 696e 6720  nfo("Connecting 
-00000a70: 746f 2049 424d 2053 6563 7572 6974 7920  to IBM Security 
-00000a80: 534f 4152 2061 743a 2025 7322 2c20 6f70  SOAR at: %s", op
-00000a90: 7473 2e67 6574 2822 686f 7374 2229 290a  ts.get("host")).
-00000aa0: 0a20 2020 2072 6574 7279 5f61 7267 7320  .    retry_args 
-00000ab0: 3d20 7b0a 2020 2020 2020 2020 7265 735f  = {.        res_
-00000ac0: 636f 6e73 7461 6e74 732e 4150 505f 434f  constants.APP_CO
-00000ad0: 4e46 4947 5f4d 4158 5f43 4f4e 4e45 4354  NFIG_MAX_CONNECT
-00000ae0: 494f 4e5f 5245 5452 4945 533a 206f 7074  ION_RETRIES: opt
-00000af0: 732e 6765 7428 7265 735f 636f 6e73 7461  s.get(res_consta
-00000b00: 6e74 732e 4150 505f 434f 4e46 4947 5f4d  nts.APP_CONFIG_M
-00000b10: 4158 5f43 4f4e 4e45 4354 494f 4e5f 5245  AX_CONNECTION_RE
-00000b20: 5452 4945 5329 2c0a 2020 2020 2020 2020  TRIES),.        
-00000b30: 7265 735f 636f 6e73 7461 6e74 732e 4150  res_constants.AP
-00000b40: 505f 434f 4e46 4947 5f52 4551 5545 5354  P_CONFIG_REQUEST
-00000b50: 5f4d 4158 5f52 4554 5249 4553 3a20 6f70  _MAX_RETRIES: op
-00000b60: 7473 2e67 6574 2872 6573 5f63 6f6e 7374  ts.get(res_const
-00000b70: 616e 7473 2e41 5050 5f43 4f4e 4649 475f  ants.APP_CONFIG_
-00000b80: 5245 5155 4553 545f 4d41 585f 5245 5452  REQUEST_MAX_RETR
-00000b90: 4945 5329 2c0a 2020 2020 2020 2020 7265  IES),.        re
-00000ba0: 735f 636f 6e73 7461 6e74 732e 4150 505f  s_constants.APP_
-00000bb0: 434f 4e46 4947 5f52 4551 5545 5354 5f52  CONFIG_REQUEST_R
-00000bc0: 4554 5259 5f44 454c 4159 3a20 6f70 7473  ETRY_DELAY: opts
-00000bd0: 2e67 6574 2872 6573 5f63 6f6e 7374 616e  .get(res_constan
-00000be0: 7473 2e41 5050 5f43 4f4e 4649 475f 5245  ts.APP_CONFIG_RE
-00000bf0: 5155 4553 545f 5245 5452 595f 4445 4c41  QUEST_RETRY_DELA
-00000c00: 5929 2c0a 2020 2020 2020 2020 7265 735f  Y),.        res_
-00000c10: 636f 6e73 7461 6e74 732e 4150 505f 434f  constants.APP_CO
-00000c20: 4e46 4947 5f52 4551 5545 5354 5f52 4554  NFIG_REQUEST_RET
-00000c30: 5259 5f42 4143 4b4f 4646 3a20 6f70 7473  RY_BACKOFF: opts
-00000c40: 2e67 6574 2872 6573 5f63 6f6e 7374 616e  .get(res_constan
-00000c50: 7473 2e41 5050 5f43 4f4e 4649 475f 5245  ts.APP_CONFIG_RE
-00000c60: 5155 4553 545f 5245 5452 595f 4241 434b  QUEST_RETRY_BACK
-00000c70: 4f46 4629 0a20 2020 207d 0a0a 2020 2020  OFF).    }..    
-00000c80: 7265 7475 726e 2067 6574 5f63 6c69 656e  return get_clien
-00000c90: 7428 6f70 7473 2c20 2a2a 7265 7472 795f  t(opts, **retry_
-00000ca0: 6172 6773 290a 0a0a 6465 6620 7365 7475  args)...def setu
-00000cb0: 705f 6a69 6e6a 615f 656e 7628 7265 6c61  p_jinja_env(rela
-00000cc0: 7469 7665 5f70 6174 685f 746f 5f74 656d  tive_path_to_tem
-00000cd0: 706c 6174 6573 293a 0a20 2020 2022 2222  plates):.    """
-00000ce0: 0a20 2020 2052 6574 7572 6e73 2061 204a  .    Returns a J
-00000cf0: 696e 6a61 3220 456e 7669 726f 6e6d 656e  inja2 Environmen
-00000d00: 7420 7769 7468 204a 696e 6a61 2074 656d  t with Jinja tem
-00000d10: 706c 6174 6573 2066 6f75 6e64 2069 6e20  plates found in 
-00000d20: 7265 7369 6c69 656e 745f 7364 6b2f 3c3c  resilient_sdk/<<
-00000d30: 7265 6c61 7469 7665 5f70 6174 685f 746f  relative_path_to
-00000d40: 5f74 656d 706c 6174 6573 3e3e 0a20 2020  _templates>>.   
-00000d50: 2022 2222 0a20 2020 206a 696e 6a61 5f65   """.    jinja_e
-00000d60: 6e76 203d 2045 6e76 6972 6f6e 6d65 6e74  nv = Environment
-00000d70: 280a 2020 2020 2020 2020 6c6f 6164 6572  (.        loader
-00000d80: 3d50 6163 6b61 6765 4c6f 6164 6572 2822  =PackageLoader("
-00000d90: 7265 7369 6c69 656e 745f 7364 6b22 2c20  resilient_sdk", 
-00000da0: 7265 6c61 7469 7665 5f70 6174 685f 746f  relative_path_to
-00000db0: 5f74 656d 706c 6174 6573 292c 2020 2320  _templates),  # 
-00000dc0: 4c6f 6164 7320 4a69 6e6a 6120 5465 6d70  Loads Jinja Temp
-00000dd0: 6c61 7465 7320 696e 2072 6573 696c 6965  lates in resilie
-00000de0: 6e74 5f73 646b 2f3c 3c72 656c 6174 6976  nt_sdk/<<relativ
-00000df0: 655f 7061 7468 5f74 6f5f 7465 6d70 6c61  e_path_to_templa
-00000e00: 7465 733e 3e0a 2020 2020 2020 2020 7472  tes>>.        tr
-00000e10: 696d 5f62 6c6f 636b 733d 5472 7565 2c20  im_blocks=True, 
-00000e20: 2023 2046 6972 7374 206e 6577 6c69 6e65   # First newline
-00000e30: 2061 6674 6572 2061 2062 6c6f 636b 2069   after a block i
-00000e40: 7320 7265 6d6f 7665 640a 2020 2020 2020  s removed.      
-00000e50: 2020 6c73 7472 6970 5f62 6c6f 636b 733d    lstrip_blocks=
-00000e60: 5472 7565 2c20 2023 204c 6561 6469 6e67  True,  # Leading
-00000e70: 2073 7061 6365 7320 616e 6420 7461 6273   spaces and tabs
-00000e80: 2061 7265 2073 7472 6970 7065 6420 6672   are stripped fr
-00000e90: 6f6d 2074 6865 2073 7461 7274 206f 6620  om the start of 
-00000ea0: 6120 6c69 6e65 2074 6f20 6120 626c 6f63  a line to a bloc
-00000eb0: 6b0a 2020 2020 2020 2020 6b65 6570 5f74  k.        keep_t
-00000ec0: 7261 696c 696e 675f 6e65 776c 696e 653d  railing_newline=
-00000ed0: 5472 7565 2020 2320 5072 6573 6572 7665  True  # Preserve
-00000ee0: 2074 6865 2074 7261 696c 696e 6720 6e65   the trailing ne
-00000ef0: 776c 696e 6520 7768 656e 2072 656e 6465  wline when rende
-00000f00: 7269 6e67 2074 656d 706c 6174 6573 0a20  ring templates. 
-00000f10: 2020 2029 0a0a 2020 2020 2320 4164 6420     )..    # Add 
-00000f20: 6375 7374 6f6d 2066 696c 7465 7273 2074  custom filters t
-00000f30: 6f20 6f75 7220 6a69 6e6a 615f 656e 760a  o our jinja_env.
-00000f40: 2020 2020 6164 645f 6669 6c74 6572 735f      add_filters_
-00000f50: 746f 5f6a 696e 6a61 5f65 6e76 286a 696e  to_jinja_env(jin
-00000f60: 6a61 5f65 6e76 290a 0a20 2020 2072 6574  ja_env)..    ret
-00000f70: 7572 6e20 6a69 6e6a 615f 656e 760a 0a0a  urn jinja_env...
-00000f80: 6465 6620 7365 7475 705f 656e 765f 616e  def setup_env_an
-00000f90: 645f 7265 6e64 6572 5f6a 696e 6a61 5f66  d_render_jinja_f
-00000fa0: 696c 6528 7265 6c61 7469 7665 5f70 6174  ile(relative_pat
-00000fb0: 685f 746f 5f74 656d 706c 6174 652c 2066  h_to_template, f
-00000fc0: 696c 656e 616d 652c 202a 6172 6773 2c20  ilename, *args, 
-00000fd0: 2a2a 6b77 6172 6773 293a 0a20 2020 2022  **kwargs):.    "
-00000fe0: 2222 0a20 2020 2043 7265 6174 6573 2061  "".    Creates a
-00000ff0: 204a 696e 6a61 2065 6e76 2061 6e64 2072   Jinja env and r
-00001000: 6574 7572 6e73 2074 6865 2072 656e 6465  eturns the rende
-00001010: 7265 6420 7374 7269 6e67 2066 726f 6d20  red string from 
-00001020: 6120 6a69 6e6a 6120 7465 6d70 6c61 7465  a jinja template
-00001030: 206f 6620 6120 6769 7665 6e20 6669 6c65   of a given file
-00001040: 6e61 6d65 2e0a 2020 2020 5061 7373 6573  name..    Passes
-00001050: 206f 6e20 6172 6773 2061 6e64 206b 7761   on args and kwa
-00001060: 7267 7320 746f 2074 6865 2072 656e 6465  rgs to the rende
-00001070: 7220 6675 6e63 7469 6f6e 0a20 2020 2022  r function.    "
-00001080: 2222 0a0a 2020 2020 2320 696e 7374 616e  ""..    # instan
-00001090: 7469 6174 6520 4a69 6e6a 6132 2045 6e76  tiate Jinja2 Env
-000010a0: 6972 6f6e 6d65 6e74 2077 6974 6820 7061  ironment with pa
-000010b0: 7468 2074 6f20 4a69 6e6a 6132 2074 656d  th to Jinja2 tem
-000010c0: 706c 6174 6573 0a20 2020 206a 696e 6a61  plates.    jinja
-000010d0: 5f65 6e76 203d 2073 6574 7570 5f6a 696e  _env = setup_jin
-000010e0: 6a61 5f65 6e76 2872 656c 6174 6976 655f  ja_env(relative_
-000010f0: 7061 7468 5f74 6f5f 7465 6d70 6c61 7465  path_to_template
-00001100: 290a 0a20 2020 2023 204c 6f61 6420 7468  )..    # Load th
-00001110: 6520 4a69 6e6a 6132 2054 656d 706c 6174  e Jinja2 Templat
-00001120: 6520 6672 6f6d 2066 696c 656e 616d 6520  e from filename 
-00001130: 2b20 6a69 6e6a 6132 2065 7874 0a20 2020  + jinja2 ext.   
-00001140: 2066 696c 655f 7465 6d70 6c61 7465 203d   file_template =
-00001150: 206a 696e 6a61 5f65 6e76 2e67 6574 5f74   jinja_env.get_t
-00001160: 656d 706c 6174 6528 6669 6c65 6e61 6d65  emplate(filename
-00001170: 202b 2022 2e6a 696e 6a61 3222 290a 0a20   + ".jinja2").. 
-00001180: 2020 2023 2072 656e 6465 7220 7468 6520     # render the 
-00001190: 7465 6d70 6c61 7465 2077 6974 6820 7468  template with th
-000011a0: 6520 7265 7175 6972 6564 2076 6172 6961  e required varia
-000011b0: 626c 6573 2061 6e64 2072 6574 7572 6e20  bles and return 
-000011c0: 7468 6520 7374 7269 6e67 2076 616c 7565  the string value
-000011d0: 0a20 2020 2072 6574 7572 6e20 6669 6c65  .    return file
-000011e0: 5f74 656d 706c 6174 652e 7265 6e64 6572  _template.render
-000011f0: 282a 6172 6773 2c20 2a2a 6b77 6172 6773  (*args, **kwargs
-00001200: 290a 0a0a 6465 6620 7772 6974 655f 6669  )...def write_fi
-00001210: 6c65 2870 6174 682c 2063 6f6e 7465 6e74  le(path, content
-00001220: 7329 3a0a 2020 2020 2222 2257 7269 7465  s):.    """Write
-00001230: 7320 7468 6520 5374 7269 6e67 2063 6f6e  s the String con
-00001240: 7465 6e74 7320 746f 2061 2066 696c 6520  tents to a file 
-00001250: 6174 2070 6174 6822 2222 0a0a 2020 2020  at path"""..    
-00001260: 6966 2073 7973 2e76 6572 7369 6f6e 5f69  if sys.version_i
-00001270: 6e66 6f5b 305d 203c 2033 2061 6e64 2069  nfo[0] < 3 and i
-00001280: 7369 6e73 7461 6e63 6528 636f 6e74 656e  sinstance(conten
-00001290: 7473 2c20 7374 7229 3a0a 2020 2020 2020  ts, str):.      
-000012a0: 2020 636f 6e74 656e 7473 203d 2075 6e69    contents = uni
-000012b0: 636f 6465 2863 6f6e 7465 6e74 732c 2022  code(contents, "
-000012c0: 7574 662d 3822 290a 0a20 2020 2077 6974  utf-8")..    wit
-000012d0: 6820 696f 2e6f 7065 6e28 7061 7468 2c20  h io.open(path, 
-000012e0: 6d6f 6465 3d22 7774 222c 2065 6e63 6f64  mode="wt", encod
-000012f0: 696e 673d 2275 7466 2d38 222c 206e 6577  ing="utf-8", new
-00001300: 6c69 6e65 3d22 5c6e 2229 2061 7320 7468  line="\n") as th
-00001310: 655f 6669 6c65 3a0a 2020 2020 2020 2020  e_file:.        
-00001320: 7468 655f 6669 6c65 2e77 7269 7465 2863  the_file.write(c
-00001330: 6f6e 7465 6e74 7329 0a0a 0a64 6566 2077  ontents)...def w
-00001340: 7269 7465 5f6c 6174 6573 745f 7079 7069  rite_latest_pypi
-00001350: 5f74 6d70 5f66 696c 6528 6c61 7465 7374  _tmp_file(latest
-00001360: 5f76 6572 7369 6f6e 2c20 7061 7468 5f73  _version, path_s
-00001370: 646b 5f74 6d70 5f70 7970 695f 7665 7273  dk_tmp_pypi_vers
-00001380: 696f 6e29 3a0a 2020 2020 2222 220a 2020  ion):.    """.  
-00001390: 2020 5772 6974 6573 2074 6865 2060 606c    Writes the ``l
-000013a0: 6174 6573 745f 7665 7273 696f 6e60 6020  atest_version`` 
-000013b0: 616e 6420 7468 6520 7473 206f 6620 7468  and the ts of th
-000013c0: 6520 6375 7272 656e 7420 7469 6d65 0a20  e current time. 
-000013d0: 2020 2074 6f20 6060 7061 7468 5f73 646b     to ``path_sdk
-000013e0: 5f74 6d70 5f70 7970 695f 7665 7273 696f  _tmp_pypi_versio
-000013f0: 6e60 600a 0a20 2020 2049 6620 6060 6c61  n``..    If ``la
-00001400: 7465 7374 5f76 6572 7369 6f6e 6060 2069  test_version`` i
-00001410: 7320 6120 6060 706b 675f 7265 736f 7572  s a ``pkg_resour
-00001420: 6365 732e 5665 7273 696f 6e60 602c 2067  ces.Version``, g
-00001430: 6574 2069 7473 2060 6062 6173 655f 7665  et its ``base_ve
-00001440: 7273 696f 6e60 602e 0a20 2020 204e 6f74  rsion``..    Not
-00001450: 653a 2074 6869 7320 6973 2061 6374 7561  e: this is actua
-00001460: 6c6c 7920 6120 6469 6666 6572 656e 7420  lly a different 
-00001470: 5665 7273 696f 6e20 7479 7065 202d 2077  Version type - w
-00001480: 6520 776f 756c 6420 6861 7665 2074 6f20  e would have to 
-00001490: 696d 706f 7274 2065 7874 7261 0a20 2020  import extra.   
-000014a0: 2064 6570 656e 6465 6e63 6965 7320 746f   dependencies to
-000014b0: 2063 6f72 7265 6374 6c79 2075 7365 2069   correctly use i
-000014c0: 7369 6e73 7461 6e63 6528 6c61 7465 7374  sinstance(latest
-000014d0: 5f76 6572 7369 6f6e 2c20 5665 7273 696f  _version, Versio
-000014e0: 6e29 202d 2073 6f20 6a75 7374 2063 6865  n) - so just che
-000014f0: 636b 696e 670a 2020 2020 6966 2069 7420  cking.    if it 
-00001500: 6861 7320 7468 6520 6174 7472 6962 7574  has the attribut
-00001510: 650a 2020 2020 2222 220a 2020 2020 2320  e.    """.    # 
-00001520: 5472 7920 6765 7420 7468 6520 2762 6173  Try get the 'bas
-00001530: 655f 7665 7273 696f 6e27 2069 6620 7468  e_version' if th
-00001540: 6973 2069 7320 6120 5665 7273 696f 6e20  is is a Version 
-00001550: 6f62 6a65 6374 0a20 2020 2069 6620 6973  object.    if is
-00001560: 696e 7374 616e 6365 286c 6174 6573 745f  instance(latest_
-00001570: 7665 7273 696f 6e2c 206f 626a 6563 7429  version, object)
-00001580: 3a0a 2020 2020 2020 2020 6c61 7465 7374  :.        latest
-00001590: 5f76 6572 7369 6f6e 203d 2067 6574 6174  _version = getat
-000015a0: 7472 286c 6174 6573 745f 7665 7273 696f  tr(latest_versio
-000015b0: 6e2c 2022 6261 7365 5f76 6572 7369 6f6e  n, "base_version
-000015c0: 222c 206c 6174 6573 745f 7665 7273 696f  ", latest_versio
-000015d0: 6e29 0a0a 2020 2020 7361 7665 645f 7665  n)..    saved_ve
-000015e0: 7273 696f 6e5f 6461 7461 203d 207b 0a20  rsion_data = {. 
-000015f0: 2020 2020 2020 2022 7473 223a 2069 6e74         "ts": int
-00001600: 2874 696d 652e 7469 6d65 2829 292c 0a20  (time.time()),. 
-00001610: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
-00001620: 3a20 6c61 7465 7374 5f76 6572 7369 6f6e  : latest_version
-00001630: 0a20 2020 207d 0a0a 2020 2020 7772 6974  .    }..    writ
-00001640: 655f 6669 6c65 2870 6174 685f 7364 6b5f  e_file(path_sdk_
-00001650: 746d 705f 7079 7069 5f76 6572 7369 6f6e  tmp_pypi_version
-00001660: 2c20 6a73 6f6e 2e64 756d 7073 2873 6176  , json.dumps(sav
-00001670: 6564 5f76 6572 7369 6f6e 5f64 6174 6129  ed_version_data)
-00001680: 290a 0a0a 6465 6620 7265 6164 5f66 696c  )...def read_fil
-00001690: 6528 7061 7468 293a 0a20 2020 2022 2222  e(path):.    """
-000016a0: 5265 7475 726e 7320 616c 6c20 7468 6520  Returns all the 
-000016b0: 6c69 6e65 7320 6f66 2061 2066 696c 6520  lines of a file 
-000016c0: 6174 2070 6174 6820 6173 2061 204c 6973  at path as a Lis
-000016d0: 7422 2222 0a20 2020 2066 696c 655f 6c69  t""".    file_li
-000016e0: 6e65 7320 3d20 5b5d 0a20 2020 2077 6974  nes = [].    wit
-000016f0: 6820 696f 2e6f 7065 6e28 7061 7468 2c20  h io.open(path, 
-00001700: 6d6f 6465 3d22 7274 222c 2065 6e63 6f64  mode="rt", encod
-00001710: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
-00001720: 7468 655f 6669 6c65 3a0a 2020 2020 2020  the_file:.      
-00001730: 2020 6669 6c65 5f6c 696e 6573 203d 2074    file_lines = t
-00001740: 6865 5f66 696c 652e 7265 6164 6c69 6e65  he_file.readline
-00001750: 7328 290a 2020 2020 7265 7475 726e 2066  s().    return f
-00001760: 696c 655f 6c69 6e65 730a 0a0a 6465 6620  ile_lines...def 
-00001770: 7265 6164 5f6a 736f 6e5f 6669 6c65 2870  read_json_file(p
-00001780: 6174 682c 2073 6563 7469 6f6e 3d4e 6f6e  ath, section=Non
-00001790: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-000017a0: 4966 2074 6865 2063 6f6e 7465 6e74 7320  If the contents 
-000017b0: 6f66 2074 6865 2066 696c 6520 6174 2070  of the file at p
-000017c0: 6174 6820 6973 2076 616c 6964 204a 534f  ath is valid JSO
-000017d0: 4e2c 0a20 2020 2072 6574 7572 6e73 2074  N,.    returns t
-000017e0: 6865 2063 6f6e 7465 6e74 7320 6f66 2074  he contents of t
-000017f0: 6865 2066 696c 6520 6173 2061 2064 6963  he file as a dic
-00001800: 7469 6f6e 6172 790a 0a20 2020 203a 7061  tionary..    :pa
-00001810: 7261 6d20 7061 7468 3a20 5061 7468 2074  ram path: Path t
-00001820: 6f20 4a53 4f4e 2066 696c 6520 746f 2072  o JSON file to r
-00001830: 6561 640a 2020 2020 3a74 7970 6520 7061  ead.    :type pa
-00001840: 7468 3a20 7374 720a 2020 2020 3a70 6172  th: str.    :par
-00001850: 616d 2073 6563 7469 6f6e 3a20 5365 6374  am section: Sect
-00001860: 696f 6e20 6e61 6d65 2069 6e20 4a53 4f4e  ion name in JSON
-00001870: 2066 696c 6520 2865 672e 2063 6f6d 6d61   file (eg. comma
-00001880: 6e64 7320 696e 2072 6573 696c 6965 6e74  nds in resilient
-00001890: 2d73 646b 290a 2020 2020 3a74 7970 6520  -sdk).    :type 
-000018a0: 7365 6374 696f 6e3a 2073 7472 0a20 2020  section: str.   
-000018b0: 203a 7265 7475 726e 3a20 4669 6c65 2063   :return: File c
-000018c0: 6f6e 7465 6e74 7320 6173 2061 2064 6963  ontents as a dic
-000018d0: 7469 6f6e 6172 790a 2020 2020 3a72 7479  tionary.    :rty
-000018e0: 7065 3a20 6469 6374 0a20 2020 2022 2222  pe: dict.    """
-000018f0: 0a20 2020 2066 696c 655f 636f 6e74 656e  .    file_conten
-00001900: 7473 203d 204e 6f6e 650a 2020 2020 7769  ts = None.    wi
-00001910: 7468 2069 6f2e 6f70 656e 2870 6174 682c  th io.open(path,
-00001920: 206d 6f64 653d 2272 7422 2c20 656e 636f   mode="rt", enco
-00001930: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
-00001940: 2074 6865 5f66 696c 653a 0a20 2020 2020   the_file:.     
-00001950: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00001960: 2020 2020 6669 6c65 5f63 6f6e 7465 6e74      file_content
-00001970: 7320 3d20 6a73 6f6e 2e6c 6f61 6428 7468  s = json.load(th
-00001980: 655f 6669 6c65 290a 2020 2020 2020 2020  e_file).        
-00001990: 2320 496e 2050 5932 2e37 2069 7420 7261  # In PY2.7 it ra
-000019a0: 6973 6573 2061 2056 616c 7565 4572 726f  ises a ValueErro
-000019b0: 7220 616e 6420 696e 2050 5933 2e36 2069  r and in PY3.6 i
-000019c0: 7420 7261 6973 6573 0a20 2020 2020 2020  t raises.       
-000019d0: 2023 2061 204a 534f 4e44 6563 6f64 6545   # a JSONDecodeE
-000019e0: 7272 6f72 2069 6620 6974 2063 616e 6e6f  rror if it canno
-000019f0: 7420 6c6f 6164 2074 6865 204a 534f 4e20  t load the JSON 
-00001a00: 6672 6f6d 2074 6865 2066 696c 650a 2020  from the file.  
-00001a10: 2020 2020 2020 6578 6365 7074 2028 5661        except (Va
-00001a20: 6c75 6545 7272 6f72 2c20 4a53 4f4e 4465  lueError, JSONDe
-00001a30: 636f 6465 4572 726f 7229 2061 7320 6572  codeError) as er
-00001a40: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
-00001a50: 6169 7365 2053 444b 4578 6365 7074 696f  aise SDKExceptio
-00001a60: 6e28 2243 6f75 6c64 206e 6f74 2072 6561  n("Could not rea
-00001a70: 6420 636f 7272 7570 7420 4a53 4f4e 2066  d corrupt JSON f
-00001a80: 696c 6520 6174 207b 307d 5c6e 7b31 7d22  ile at {0}\n{1}"
-00001a90: 2e66 6f72 6d61 7428 7061 7468 2c20 6572  .format(path, er
-00001aa0: 7229 290a 2020 2020 6966 2073 6563 7469  r)).    if secti
-00001ab0: 6f6e 3a0a 2020 2020 2020 2020 6966 2073  on:.        if s
-00001ac0: 6563 7469 6f6e 2069 6e20 6669 6c65 5f63  ection in file_c
-00001ad0: 6f6e 7465 6e74 733a 0a20 2020 2020 2020  ontents:.       
-00001ae0: 2020 2020 2072 6574 7572 6e20 6669 6c65       return file
-00001af0: 5f63 6f6e 7465 6e74 732e 6765 7428 7365  _contents.get(se
-00001b00: 6374 696f 6e2c 207b 7d29 0a20 2020 2020  ction, {}).     
-00001b10: 2020 2065 6c73 653a 200a 2020 2020 2020     else: .      
-00001b20: 2020 2020 2020 4c4f 472e 6465 6275 6728        LOG.debug(
-00001b30: 2253 6563 7469 6f6e 207b 7d20 6e6f 7420  "Section {} not 
-00001b40: 666f 756e 6420 696e 2070 726f 7669 6465  found in provide
-00001b50: 6420 4a53 4f4e 2e22 2e66 6f72 6d61 7428  d JSON.".format(
-00001b60: 7365 6374 696f 6e29 290a 2020 2020 2020  section)).      
-00001b70: 2020 2020 2020 7265 7475 726e 207b 7d0a        return {}.
-00001b80: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00001b90: 2020 7265 7475 726e 2066 696c 655f 636f    return file_co
-00001ba0: 6e74 656e 7473 0a0a 0a64 6566 2072 6561  ntents...def rea
-00001bb0: 645f 7a69 705f 6669 6c65 2870 6174 682c  d_zip_file(path,
-00001bc0: 2070 6174 7465 726e 293a 0a20 2020 2022   pattern):.    "
-00001bd0: 2222 5265 7475 726e 7320 756e 7a69 7070  ""Returns unzipp
-00001be0: 6564 2063 6f6e 7465 6e74 7320 6f66 2066  ed contents of f
-00001bf0: 696c 6520 7768 6f73 6520 6e61 6d65 206d  ile whose name m
-00001c00: 6174 6368 6573 2061 2070 6174 7465 726e  atches a pattern
-00001c10: 0a20 2020 2069 6e20 7a69 7020 6669 6c65  .    in zip file
-00001c20: 2061 7420 7061 7468 2e0a 0a20 2020 203a   at path...    :
-00001c30: 7061 7261 6d20 7061 7468 3a20 5061 7468  param path: Path
-00001c40: 2074 6f20 7a69 7020 6669 6c65 2e0a 2020   to zip file..  
-00001c50: 2020 3a70 6172 616d 2070 6174 7465 726e    :param pattern
-00001c60: 3a20 4669 6c65 2070 6174 7465 726e 2074  : File pattern t
-00001c70: 6f20 6d61 7463 6820 696e 2074 6865 207a  o match in the z
-00001c80: 6970 2066 696c 652e 0a20 2020 203a 7265  ip file..    :re
-00001c90: 7475 726e 3a20 6669 6c65 5f63 6f6e 7465  turn: file_conte
-00001ca0: 6e74 3a20 5265 7475 726e 2075 6e7a 6970  nt: Return unzip
-00001cb0: 7065 6420 6669 6c65 2063 6f6e 7465 6e74  ped file content
-00001cc0: 2e0a 2020 2020 2222 220a 2020 2020 6669  ..    """.    fi
-00001cd0: 6c65 5f63 6f6e 7465 6e74 203d 204e 6f6e  le_content = Non
-00001ce0: 650a 2020 2020 7472 793a 0a20 2020 2020  e.    try:.     
-00001cf0: 2020 2077 6974 6820 5a69 7046 696c 6528     with ZipFile(
-00001d00: 2870 6174 6829 2c20 2772 2729 2061 7320  (path), 'r') as 
-00001d10: 7a6f 626a 3a0a 2020 2020 2020 2020 2020  zobj:.          
-00001d20: 2020 2320 4765 7420 616c 6c20 6669 6c65    # Get all file
-00001d30: 206e 616d 6573 206d 6174 6368 696e 6720   names matching 
-00001d40: 2770 6174 7465 726e 272e 0a20 2020 2020  'pattern'..     
-00001d50: 2020 2020 2020 2066 696c 655f 6d61 7463         file_matc
-00001d60: 6865 7320 3d20 5b66 2066 6f72 2066 2069  hes = [f for f i
-00001d70: 6e20 7a6f 626a 2e6e 616d 656c 6973 7428  n zobj.namelist(
-00001d80: 2920 6966 2070 6174 7465 726e 2e6c 6f77  ) if pattern.low
-00001d90: 6572 2829 2069 6e20 662e 6c6f 7765 7228  er() in f.lower(
-00001da0: 295d 0a20 2020 2020 2020 2020 2020 2069  )].            i
-00001db0: 6620 6c65 6e28 6669 6c65 5f6d 6174 6368  f len(file_match
-00001dc0: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
-00001dd0: 2020 2020 2069 6620 6c65 6e28 6669 6c65       if len(file
-00001de0: 5f6d 6174 6368 6573 2920 3e20 313a 0a20  _matches) > 1:. 
-00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e00: 2020 2072 6169 7365 2053 444b 4578 6365     raise SDKExce
-00001e10: 7074 696f 6e28 224d 6f72 6520 7468 616e  ption("More than
-00001e20: 206f 6e65 2066 696c 6520 6d61 7463 6869   one file matchi
-00001e30: 6e67 2070 6174 7465 726e 207b 307d 2066  ng pattern {0} f
-00001e40: 6f75 6e64 2069 6e20 7a69 7020 6669 6c65  ound in zip file
-00001e50: 3a20 7b31 7d22 0a20 2020 2020 2020 2020  : {1}".         
-00001e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e70: 2020 2020 2020 2020 2020 2020 2020 2e66                .f
-00001e80: 6f72 6d61 7428 7061 7474 6572 6e2c 2070  ormat(pattern, p
-00001e90: 6174 6829 290a 2020 2020 2020 2020 2020  ath)).          
-00001ea0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ec0: 6669 6c65 5f6e 616d 6520 3d20 6669 6c65  file_name = file
-00001ed0: 5f6d 6174 6368 6573 2e70 6f70 2829 0a20  _matches.pop(). 
-00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ef0: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
-00001f00: 2066 696c 652e 0a20 2020 2020 2020 2020   file..         
-00001f10: 2020 2020 2020 2020 2020 2066 203d 207a             f = z
-00001f20: 6f62 6a2e 6f70 656e 2866 696c 655f 6e61  obj.open(file_na
-00001f30: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-00001f40: 2020 2020 2020 2020 2320 5265 6164 2066          # Read f
-00001f50: 696c 6520 616e 6420 636f 6e76 6572 7420  ile and convert 
-00001f60: 636f 6e74 656e 7420 6672 6f6d 2062 7974  content from byt
-00001f70: 6573 2074 6f20 7374 7269 6e67 2e0a 2020  es to string..  
-00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f90: 2020 6669 6c65 5f63 6f6e 7465 6e74 203d    file_content =
-00001fa0: 2066 2e72 6561 6428 292e 6465 636f 6465   f.read().decode
-00001fb0: 2827 7574 6638 272c 2027 6967 6e6f 7265  ('utf8', 'ignore
-00001fc0: 2729 0a20 2020 2020 2020 2020 2020 2065  ').            e
-00001fd0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00001fe0: 2020 2020 2072 6169 7365 2053 444b 4578       raise SDKEx
-00001ff0: 6365 7074 696f 6e28 2241 2066 696c 6520  ception("A file 
-00002000: 6d61 7463 6869 6e67 2070 6174 7465 726e  matching pattern
-00002010: 207b 307d 2077 6173 206e 6f74 2066 6f75   {0} was not fou
-00002020: 6e64 2069 6e20 7a69 7020 6669 6c65 3a20  nd in zip file: 
-00002030: 7b31 7d22 0a20 2020 2020 2020 2020 2020  {1}".           
-00002040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002050: 2020 2020 2020 2020 2e66 6f72 6d61 7428          .format(
-00002060: 7061 7474 6572 6e2c 2070 6174 6829 290a  pattern, path)).
-00002070: 2020 2020 6578 6365 7074 2042 6164 5a69      except BadZi
-00002080: 7066 696c 653a 0a20 2020 2020 2020 2072  pfile:.        r
-00002090: 6169 7365 2053 444b 4578 6365 7074 696f  aise SDKExceptio
-000020a0: 6e28 2242 6164 207a 6970 2066 696c 6520  n("Bad zip file 
-000020b0: 7b30 7d2e 222e 666f 726d 6174 2870 6174  {0}.".format(pat
-000020c0: 6829 290a 0a20 2020 2065 7863 6570 7420  h))..    except 
-000020d0: 5344 4b45 7863 6570 7469 6f6e 2061 7320  SDKException as 
-000020e0: 6572 723a 0a20 2020 2020 2020 2072 6169  err:.        rai
-000020f0: 7365 2065 7272 0a0a 2020 2020 6578 6365  se err..    exce
-00002100: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00002110: 6572 723a 0a20 2020 2020 2020 2023 2041  err:.        # A
-00002120: 6e20 616e 2075 6e65 7870 6563 7465 6420  n an unexpected 
-00002130: 6572 726f 7220 7472 7969 6e67 2074 6f20  error trying to 
-00002140: 7265 6164 2061 207a 6970 6669 6c65 2e0a  read a zipfile..
-00002150: 2020 2020 2020 2020 7261 6973 6520 5344          raise SD
-00002160: 4b45 7863 6570 7469 6f6e 2822 476f 7420  KException("Got 
-00002170: 616e 2065 7272 6f72 2027 7b30 7d27 2061  an error '{0}' a
-00002180: 7474 656d 7074 696e 6720 746f 2072 6561  ttempting to rea
-00002190: 6420 7a69 7020 6669 6c65 207b 317d 222e  d zip file {1}".
-000021a0: 666f 726d 6174 2865 7272 2c20 7061 7468  format(err, path
-000021b0: 2929 0a0a 2020 2020 7265 7475 726e 2066  ))..    return f
-000021c0: 696c 655f 636f 6e74 656e 740a 0a0a 6465  ile_content...de
-000021d0: 6620 7265 6e61 6d65 5f66 696c 6528 7061  f rename_file(pa
-000021e0: 7468 5f63 7572 7265 6e74 5f66 696c 652c  th_current_file,
-000021f0: 206e 6577 5f6e 616d 6529 3a0a 2020 2020   new_name):.    
-00002200: 2222 2252 656e 616d 6573 2074 6865 2066  """Renames the f
-00002210: 696c 6520 6174 2070 6174 685f 6375 7272  ile at path_curr
-00002220: 656e 745f 6669 6c65 2077 6974 6820 7468  ent_file with th
-00002230: 6520 6e65 775f 6e61 6d65 2222 220a 2020  e new_name""".  
-00002240: 2020 6f73 2e72 656e 616d 6528 7061 7468    os.rename(path
-00002250: 5f63 7572 7265 6e74 5f66 696c 652c 206f  _current_file, o
-00002260: 732e 7061 7468 2e6a 6f69 6e28 6f73 2e70  s.path.join(os.p
-00002270: 6174 682e 6469 726e 616d 6528 7061 7468  ath.dirname(path
-00002280: 5f63 7572 7265 6e74 5f66 696c 6529 2c20  _current_file), 
-00002290: 6e65 775f 6e61 6d65 2929 0a0a 0a64 6566  new_name))...def
-000022a0: 2069 735f 7661 6c69 645f 7061 636b 6167   is_valid_packag
-000022b0: 655f 6e61 6d65 286e 616d 6529 3a0a 2020  e_name(name):.  
-000022c0: 2020 2222 2254 6573 7420 6966 2027 6e61    """Test if 'na
-000022d0: 6d65 2720 6973 2061 2076 616c 6964 2069  me' is a valid i
-000022e0: 6465 6e74 6966 6965 7220 666f 7220 6120  dentifier for a 
-000022f0: 7061 636b 6167 6520 6f72 206d 6f64 756c  package or modul
-00002300: 650a 0a20 2020 2020 2020 3e3e 3e20 6973  e..       >>> is
-00002310: 5f76 616c 6964 5f70 6163 6b61 6765 5f6e  _valid_package_n
-00002320: 616d 6528 2222 290a 2020 2020 2020 2046  ame("").       F
-00002330: 616c 7365 0a20 2020 2020 2020 3e3e 3e20  alse.       >>> 
-00002340: 6973 5f76 616c 6964 5f70 6163 6b61 6765  is_valid_package
-00002350: 5f6e 616d 6528 4e6f 6e65 290a 2020 2020  _name(None).    
-00002360: 2020 2046 616c 7365 0a20 2020 2020 2020     False.       
-00002370: 3e3e 3e20 6973 5f76 616c 6964 5f70 6163  >>> is_valid_pac
-00002380: 6b61 6765 5f6e 616d 6528 2267 6574 2229  kage_name("get")
-00002390: 0a20 2020 2020 2020 4661 6c73 650a 2020  .       False.  
-000023a0: 2020 2020 203e 3e3e 2069 735f 7661 6c69       >>> is_vali
-000023b0: 645f 7061 636b 6167 655f 6e61 6d65 2822  d_package_name("
-000023c0: 6261 6e67 2122 290a 2020 2020 2020 2046  bang!").       F
-000023d0: 616c 7365 0a20 2020 2020 2020 3e3e 3e20  alse.       >>> 
-000023e0: 6973 5f76 616c 6964 5f70 6163 6b61 6765  is_valid_package
-000023f0: 5f6e 616d 6528 225f 736f 6d65 7468 696e  _name("_somethin
-00002400: 6722 290a 2020 2020 2020 2054 7275 650a  g").       True.
-00002410: 2020 2020 2020 203e 3e3e 2069 735f 7661         >>> is_va
-00002420: 6c69 645f 7061 636b 6167 655f 6e61 6d65  lid_package_name
-00002430: 2822 2d73 6f6d 6574 6869 6e67 2229 0a20  ("-something"). 
-00002440: 2020 2020 2020 5472 7565 0a20 2020 2022        True.    "
-00002450: 2222 0a0a 2020 2020 6966 206b 6579 776f  ""..    if keywo
-00002460: 7264 2e69 736b 6579 776f 7264 286e 616d  rd.iskeyword(nam
-00002470: 6529 3a0a 2020 2020 2020 2020 7265 7475  e):.        retu
-00002480: 726e 2046 616c 7365 0a20 2020 2065 6c69  rn False.    eli
-00002490: 6620 6e61 6d65 2069 6e20 6469 7228 5f5f  f name in dir(__
-000024a0: 6275 696c 7469 6e73 5f5f 293a 0a20 2020  builtins__):.   
-000024b0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000024c0: 650a 2020 2020 656c 6966 206e 616d 6520  e.    elif name 
-000024d0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+000004b0: 2020 2020 2020 5265 7369 6c69 656e 744f        ResilientO
+000004c0: 626a 4d61 702c 0a20 2020 2020 2020 2020  bjMap,.         
+000004d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004f0: 2020 2020 2020 2020 2052 6573 696c 6965           Resilie
+00000500: 6e74 5479 7065 4964 7329 0a66 726f 6d20  ntTypeIds).from 
+00000510: 7265 7369 6c69 656e 745f 7364 6b2e 7574  resilient_sdk.ut
+00000520: 696c 2e73 646b 5f65 7863 6570 7469 6f6e  il.sdk_exception
+00000530: 2069 6d70 6f72 7420 5344 4b45 7863 6570   import SDKExcep
+00000540: 7469 6f6e 0a0a 6672 6f6d 2072 6573 696c  tion..from resil
+00000550: 6965 6e74 2069 6d70 6f72 7420 4172 6775  ient import Argu
+00000560: 6d65 6e74 5061 7273 6572 0a66 726f 6d20  mentParser.from 
+00000570: 7265 7369 6c69 656e 7420 696d 706f 7274  resilient import
+00000580: 2063 6f6e 7374 616e 7473 2061 7320 7265   constants as re
+00000590: 735f 636f 6e73 7461 6e74 730a 6672 6f6d  s_constants.from
+000005a0: 2072 6573 696c 6965 6e74 2069 6d70 6f72   resilient impor
+000005b0: 7420 6765 745f 636c 6965 6e74 2c20 6765  t get_client, ge
+000005c0: 745f 636f 6e66 6967 5f66 696c 650a 6672  t_config_file.fr
+000005d0: 6f6d 2072 6573 696c 6965 6e74 2e68 656c  om resilient.hel
+000005e0: 7065 7273 2069 6d70 6f72 7420 7265 6d6f  pers import remo
+000005f0: 7665 5f74 6167 0a0a 6966 2073 7973 2e76  ve_tag..if sys.v
+00000600: 6572 7369 6f6e 5f69 6e66 6f2e 6d61 6a6f  ersion_info.majo
+00000610: 7220 3c20 333a 0a20 2020 2023 2048 616e  r < 3:.    # Han
+00000620: 646c 6520 5059 2032 2073 7065 6369 6669  dle PY 2 specifi
+00000630: 6320 696d 706f 7274 730a 2020 2020 2320  c imports.    # 
+00000640: 4a53 4f4e 4465 636f 6465 4572 726f 7220  JSONDecodeError 
+00000650: 6973 206e 6f74 2061 7661 696c 6162 6c65  is not available
+00000660: 2069 6e20 5059 322e 3720 736f 2077 6520   in PY2.7 so we 
+00000670: 7365 7420 6974 2074 6f20 4e6f 6e65 0a20  set it to None. 
+00000680: 2020 204a 534f 4e44 6563 6f64 6545 7272     JSONDecodeErr
+00000690: 6f72 203d 204e 6f6e 650a 656c 7365 3a0a  or = None.else:.
+000006a0: 2020 2020 2320 4861 6e64 6c65 2050 5920      # Handle PY 
+000006b0: 3320 7370 6563 6966 6963 2069 6d70 6f72  3 specific impor
+000006c0: 7473 0a20 2020 2023 2072 656c 6f61 6428  ts.    # reload(
+000006d0: 7061 636b 6167 6529 2069 6e20 5059 322e  package) in PY2.
+000006e0: 372c 2069 6d70 6f72 746c 6962 2e72 656c  7, importlib.rel
+000006f0: 6f61 6428 7061 636b 6167 6529 2069 6e20  oad(package) in 
+00000700: 5059 332e 360a 2020 2020 7265 6c6f 6164  PY3.6.    reload
+00000710: 203d 2069 6d70 6f72 746c 6962 2e72 656c   = importlib.rel
+00000720: 6f61 640a 2020 2020 6672 6f6d 206a 736f  oad.    from jso
+00000730: 6e2e 6465 636f 6465 7220 696d 706f 7274  n.decoder import
+00000740: 204a 534f 4e44 6563 6f64 6545 7272 6f72   JSONDecodeError
+00000750: 0a0a 2320 5465 6d70 2066 6978 2074 6f20  ..# Temp fix to 
+00000760: 6861 6e64 6c65 2074 6865 2072 6573 696c  handle the resil
+00000770: 6965 6e74 206d 6f64 756c 6520 6c6f 6773  ient module logs
+00000780: 0a6c 6f67 6769 6e67 2e67 6574 4c6f 6767  .logging.getLogg
+00000790: 6572 2822 7265 7369 6c69 656e 742e 636f  er("resilient.co
+000007a0: 3322 292e 6164 6448 616e 646c 6572 286c  3").addHandler(l
+000007b0: 6f67 6769 6e67 2e53 7472 6561 6d48 616e  ogging.StreamHan
+000007c0: 646c 6572 2829 290a 2320 4765 7420 7468  dler()).# Get th
+000007d0: 6520 7361 6d65 206c 6f67 6765 7220 6f62  e same logger ob
+000007e0: 6a65 6374 2074 6861 7420 6973 2075 7365  ject that is use
+000007f0: 6420 696e 2061 7070 2e70 790a 4c4f 4720  d in app.py.LOG 
+00000800: 3d20 6c6f 6767 696e 672e 6765 744c 6f67  = logging.getLog
+00000810: 6765 7228 636f 6e73 7461 6e74 732e 4c4f  ger(constants.LO
+00000820: 4747 4552 5f4e 414d 4529 0a0a 0a64 6566  GGER_NAME)...def
+00000830: 2067 6574 5f72 6573 696c 6965 6e74 5f63   get_resilient_c
+00000840: 6c69 656e 7428 7061 7468 5f63 6f6e 6669  lient(path_confi
+00000850: 675f 6669 6c65 3d4e 6f6e 6529 3a0a 2020  g_file=None):.  
+00000860: 2020 2222 220a 2020 2020 5265 7475 726e    """.    Return
+00000870: 2061 2053 696d 706c 6543 6c69 656e 7420   a SimpleClient 
+00000880: 666f 7220 5265 7369 6c69 656e 7420 5245  for Resilient RE
+00000890: 5354 2041 5049 2075 7369 6e67 2063 6f6e  ST API using con
+000008a0: 6669 6775 7261 7469 6f6e 730a 2020 2020  figurations.    
+000008b0: 6f70 7469 6f6e 7320 6672 6f6d 2070 726f  options from pro
+000008c0: 7669 6465 6420 7061 7468 5f63 6f6e 6669  vided path_confi
+000008d0: 675f 6669 6c65 206f 7220 6672 6f6d 207e  g_file or from ~
+000008e0: 2f2e 7265 7369 6c69 656e 742f 6170 702e  /.resilient/app.
+000008f0: 636f 6e66 6967 0a0a 2020 2020 3a70 6172  config..    :par
+00000900: 616d 2070 6174 685f 636f 6e66 6967 5f66  am path_config_f
+00000910: 696c 653a 2050 6174 6820 746f 2061 7070  ile: Path to app
+00000920: 2e63 6f6e 6669 6720 6669 6c65 2074 6f20  .config file to 
+00000930: 7573 650a 2020 2020 3a72 6574 7572 6e3a  use.    :return:
+00000940: 2053 696d 706c 6543 6c69 656e 7420 666f   SimpleClient fo
+00000950: 7220 5265 7369 6c69 656e 7420 5245 5354  r Resilient REST
+00000960: 2041 5049 0a20 2020 203a 7274 7970 653a   API.    :rtype:
+00000970: 2053 696d 706c 6543 6c69 656e 740a 2020   SimpleClient.  
+00000980: 2020 2222 220a 0a20 2020 2069 6620 6e6f    """..    if no
+00000990: 7420 7061 7468 5f63 6f6e 6669 675f 6669  t path_config_fi
+000009a0: 6c65 3a0a 2020 2020 2020 2020 7061 7468  le:.        path
+000009b0: 5f63 6f6e 6669 675f 6669 6c65 203d 2067  _config_file = g
+000009c0: 6574 5f63 6f6e 6669 675f 6669 6c65 2829  et_config_file()
+000009d0: 0a0a 2020 2020 4c4f 472e 6465 6275 6728  ..    LOG.debug(
+000009e0: 2255 7369 6e67 2061 7070 2e63 6f6e 6669  "Using app.confi
+000009f0: 6720 6669 6c65 2061 743a 2025 7322 2c20  g file at: %s", 
+00000a00: 7061 7468 5f63 6f6e 6669 675f 6669 6c65  path_config_file
+00000a10: 290a 0a20 2020 2063 6f6e 6669 675f 7061  )..    config_pa
+00000a20: 7273 6572 203d 2041 7267 756d 656e 7450  rser = ArgumentP
+00000a30: 6172 7365 7228 636f 6e66 6967 5f66 696c  arser(config_fil
+00000a40: 653d 7061 7468 5f63 6f6e 6669 675f 6669  e=path_config_fi
+00000a50: 6c65 290a 2020 2020 6f70 7473 203d 2063  le).    opts = c
+00000a60: 6f6e 6669 675f 7061 7273 6572 2e70 6172  onfig_parser.par
+00000a70: 7365 5f6b 6e6f 776e 5f61 7267 7328 295b  se_known_args()[
+00000a80: 305d 0a0a 2020 2020 4c4f 472e 696e 666f  0]..    LOG.info
+00000a90: 2822 436f 6e6e 6563 7469 6e67 2074 6f20  ("Connecting to 
+00000aa0: 4942 4d20 5365 6375 7269 7479 2053 4f41  IBM Security SOA
+00000ab0: 5220 6174 3a20 2573 222c 206f 7074 732e  R at: %s", opts.
+00000ac0: 6765 7428 2268 6f73 7422 2929 0a0a 2020  get("host"))..  
+00000ad0: 2020 7265 7472 795f 6172 6773 203d 207b    retry_args = {
+00000ae0: 0a20 2020 2020 2020 2072 6573 5f63 6f6e  .        res_con
+00000af0: 7374 616e 7473 2e41 5050 5f43 4f4e 4649  stants.APP_CONFI
+00000b00: 475f 4d41 585f 434f 4e4e 4543 5449 4f4e  G_MAX_CONNECTION
+00000b10: 5f52 4554 5249 4553 3a20 6f70 7473 2e67  _RETRIES: opts.g
+00000b20: 6574 2872 6573 5f63 6f6e 7374 616e 7473  et(res_constants
+00000b30: 2e41 5050 5f43 4f4e 4649 475f 4d41 585f  .APP_CONFIG_MAX_
+00000b40: 434f 4e4e 4543 5449 4f4e 5f52 4554 5249  CONNECTION_RETRI
+00000b50: 4553 292c 0a20 2020 2020 2020 2072 6573  ES),.        res
+00000b60: 5f63 6f6e 7374 616e 7473 2e41 5050 5f43  _constants.APP_C
+00000b70: 4f4e 4649 475f 5245 5155 4553 545f 4d41  ONFIG_REQUEST_MA
+00000b80: 585f 5245 5452 4945 533a 206f 7074 732e  X_RETRIES: opts.
+00000b90: 6765 7428 7265 735f 636f 6e73 7461 6e74  get(res_constant
+00000ba0: 732e 4150 505f 434f 4e46 4947 5f52 4551  s.APP_CONFIG_REQ
+00000bb0: 5545 5354 5f4d 4158 5f52 4554 5249 4553  UEST_MAX_RETRIES
+00000bc0: 292c 0a20 2020 2020 2020 2072 6573 5f63  ),.        res_c
+00000bd0: 6f6e 7374 616e 7473 2e41 5050 5f43 4f4e  onstants.APP_CON
+00000be0: 4649 475f 5245 5155 4553 545f 5245 5452  FIG_REQUEST_RETR
+00000bf0: 595f 4445 4c41 593a 206f 7074 732e 6765  Y_DELAY: opts.ge
+00000c00: 7428 7265 735f 636f 6e73 7461 6e74 732e  t(res_constants.
+00000c10: 4150 505f 434f 4e46 4947 5f52 4551 5545  APP_CONFIG_REQUE
+00000c20: 5354 5f52 4554 5259 5f44 454c 4159 292c  ST_RETRY_DELAY),
+00000c30: 0a20 2020 2020 2020 2072 6573 5f63 6f6e  .        res_con
+00000c40: 7374 616e 7473 2e41 5050 5f43 4f4e 4649  stants.APP_CONFI
+00000c50: 475f 5245 5155 4553 545f 5245 5452 595f  G_REQUEST_RETRY_
+00000c60: 4241 434b 4f46 463a 206f 7074 732e 6765  BACKOFF: opts.ge
+00000c70: 7428 7265 735f 636f 6e73 7461 6e74 732e  t(res_constants.
+00000c80: 4150 505f 434f 4e46 4947 5f52 4551 5545  APP_CONFIG_REQUE
+00000c90: 5354 5f52 4554 5259 5f42 4143 4b4f 4646  ST_RETRY_BACKOFF
+00000ca0: 290a 2020 2020 7d0a 0a20 2020 2072 6574  ).    }..    ret
+00000cb0: 7572 6e20 6765 745f 636c 6965 6e74 286f  urn get_client(o
+00000cc0: 7074 732c 202a 2a72 6574 7279 5f61 7267  pts, **retry_arg
+00000cd0: 7329 0a0a 0a64 6566 2073 6574 7570 5f6a  s)...def setup_j
+00000ce0: 696e 6a61 5f65 6e76 2872 656c 6174 6976  inja_env(relativ
+00000cf0: 655f 7061 7468 5f74 6f5f 7465 6d70 6c61  e_path_to_templa
+00000d00: 7465 7329 3a0a 2020 2020 2222 220a 2020  tes):.    """.  
+00000d10: 2020 5265 7475 726e 7320 6120 4a69 6e6a    Returns a Jinj
+00000d20: 6132 2045 6e76 6972 6f6e 6d65 6e74 2077  a2 Environment w
+00000d30: 6974 6820 4a69 6e6a 6120 7465 6d70 6c61  ith Jinja templa
+00000d40: 7465 7320 666f 756e 6420 696e 2072 6573  tes found in res
+00000d50: 696c 6965 6e74 5f73 646b 2f3c 3c72 656c  ilient_sdk/<<rel
+00000d60: 6174 6976 655f 7061 7468 5f74 6f5f 7465  ative_path_to_te
+00000d70: 6d70 6c61 7465 733e 3e0a 2020 2020 2222  mplates>>.    ""
+00000d80: 220a 2020 2020 6a69 6e6a 615f 656e 7620  ".    jinja_env 
+00000d90: 3d20 456e 7669 726f 6e6d 656e 7428 0a20  = Environment(. 
+00000da0: 2020 2020 2020 206c 6f61 6465 723d 5061         loader=Pa
+00000db0: 636b 6167 654c 6f61 6465 7228 2272 6573  ckageLoader("res
+00000dc0: 696c 6965 6e74 5f73 646b 222c 2072 656c  ilient_sdk", rel
+00000dd0: 6174 6976 655f 7061 7468 5f74 6f5f 7465  ative_path_to_te
+00000de0: 6d70 6c61 7465 7329 2c20 2023 204c 6f61  mplates),  # Loa
+00000df0: 6473 204a 696e 6a61 2054 656d 706c 6174  ds Jinja Templat
+00000e00: 6573 2069 6e20 7265 7369 6c69 656e 745f  es in resilient_
+00000e10: 7364 6b2f 3c3c 7265 6c61 7469 7665 5f70  sdk/<<relative_p
+00000e20: 6174 685f 746f 5f74 656d 706c 6174 6573  ath_to_templates
+00000e30: 3e3e 0a20 2020 2020 2020 2074 7269 6d5f  >>.        trim_
+00000e40: 626c 6f63 6b73 3d54 7275 652c 2020 2320  blocks=True,  # 
+00000e50: 4669 7273 7420 6e65 776c 696e 6520 6166  First newline af
+00000e60: 7465 7220 6120 626c 6f63 6b20 6973 2072  ter a block is r
+00000e70: 656d 6f76 6564 0a20 2020 2020 2020 206c  emoved.        l
+00000e80: 7374 7269 705f 626c 6f63 6b73 3d54 7275  strip_blocks=Tru
+00000e90: 652c 2020 2320 4c65 6164 696e 6720 7370  e,  # Leading sp
+00000ea0: 6163 6573 2061 6e64 2074 6162 7320 6172  aces and tabs ar
+00000eb0: 6520 7374 7269 7070 6564 2066 726f 6d20  e stripped from 
+00000ec0: 7468 6520 7374 6172 7420 6f66 2061 206c  the start of a l
+00000ed0: 696e 6520 746f 2061 2062 6c6f 636b 0a20  ine to a block. 
+00000ee0: 2020 2020 2020 206b 6565 705f 7472 6169         keep_trai
+00000ef0: 6c69 6e67 5f6e 6577 6c69 6e65 3d54 7275  ling_newline=Tru
+00000f00: 6520 2023 2050 7265 7365 7276 6520 7468  e  # Preserve th
+00000f10: 6520 7472 6169 6c69 6e67 206e 6577 6c69  e trailing newli
+00000f20: 6e65 2077 6865 6e20 7265 6e64 6572 696e  ne when renderin
+00000f30: 6720 7465 6d70 6c61 7465 730a 2020 2020  g templates.    
+00000f40: 290a 0a20 2020 2023 2041 6464 2063 7573  )..    # Add cus
+00000f50: 746f 6d20 6669 6c74 6572 7320 746f 206f  tom filters to o
+00000f60: 7572 206a 696e 6a61 5f65 6e76 0a20 2020  ur jinja_env.   
+00000f70: 2061 6464 5f66 696c 7465 7273 5f74 6f5f   add_filters_to_
+00000f80: 6a69 6e6a 615f 656e 7628 6a69 6e6a 615f  jinja_env(jinja_
+00000f90: 656e 7629 0a0a 2020 2020 7265 7475 726e  env)..    return
+00000fa0: 206a 696e 6a61 5f65 6e76 0a0a 0a64 6566   jinja_env...def
+00000fb0: 2073 6574 7570 5f65 6e76 5f61 6e64 5f72   setup_env_and_r
+00000fc0: 656e 6465 725f 6a69 6e6a 615f 6669 6c65  ender_jinja_file
+00000fd0: 2872 656c 6174 6976 655f 7061 7468 5f74  (relative_path_t
+00000fe0: 6f5f 7465 6d70 6c61 7465 2c20 6669 6c65  o_template, file
+00000ff0: 6e61 6d65 2c20 2a61 7267 732c 202a 2a6b  name, *args, **k
+00001000: 7761 7267 7329 3a0a 2020 2020 2222 220a  wargs):.    """.
+00001010: 2020 2020 4372 6561 7465 7320 6120 4a69      Creates a Ji
+00001020: 6e6a 6120 656e 7620 616e 6420 7265 7475  nja env and retu
+00001030: 726e 7320 7468 6520 7265 6e64 6572 6564  rns the rendered
+00001040: 2073 7472 696e 6720 6672 6f6d 2061 206a   string from a j
+00001050: 696e 6a61 2074 656d 706c 6174 6520 6f66  inja template of
+00001060: 2061 2067 6976 656e 2066 696c 656e 616d   a given filenam
+00001070: 652e 0a20 2020 2050 6173 7365 7320 6f6e  e..    Passes on
+00001080: 2061 7267 7320 616e 6420 6b77 6172 6773   args and kwargs
+00001090: 2074 6f20 7468 6520 7265 6e64 6572 2066   to the render f
+000010a0: 756e 6374 696f 6e0a 2020 2020 2222 220a  unction.    """.
+000010b0: 0a20 2020 2023 2069 6e73 7461 6e74 6961  .    # instantia
+000010c0: 7465 204a 696e 6a61 3220 456e 7669 726f  te Jinja2 Enviro
+000010d0: 6e6d 656e 7420 7769 7468 2070 6174 6820  nment with path 
+000010e0: 746f 204a 696e 6a61 3220 7465 6d70 6c61  to Jinja2 templa
+000010f0: 7465 730a 2020 2020 6a69 6e6a 615f 656e  tes.    jinja_en
+00001100: 7620 3d20 7365 7475 705f 6a69 6e6a 615f  v = setup_jinja_
+00001110: 656e 7628 7265 6c61 7469 7665 5f70 6174  env(relative_pat
+00001120: 685f 746f 5f74 656d 706c 6174 6529 0a0a  h_to_template)..
+00001130: 2020 2020 2320 4c6f 6164 2074 6865 204a      # Load the J
+00001140: 696e 6a61 3220 5465 6d70 6c61 7465 2066  inja2 Template f
+00001150: 726f 6d20 6669 6c65 6e61 6d65 202b 206a  rom filename + j
+00001160: 696e 6a61 3220 6578 740a 2020 2020 6669  inja2 ext.    fi
+00001170: 6c65 5f74 656d 706c 6174 6520 3d20 6a69  le_template = ji
+00001180: 6e6a 615f 656e 762e 6765 745f 7465 6d70  nja_env.get_temp
+00001190: 6c61 7465 2866 696c 656e 616d 6520 2b20  late(filename + 
+000011a0: 222e 6a69 6e6a 6132 2229 0a0a 2020 2020  ".jinja2")..    
+000011b0: 2320 7265 6e64 6572 2074 6865 2074 656d  # render the tem
+000011c0: 706c 6174 6520 7769 7468 2074 6865 2072  plate with the r
+000011d0: 6571 7569 7265 6420 7661 7269 6162 6c65  equired variable
+000011e0: 7320 616e 6420 7265 7475 726e 2074 6865  s and return the
+000011f0: 2073 7472 696e 6720 7661 6c75 650a 2020   string value.  
+00001200: 2020 7265 7475 726e 2066 696c 655f 7465    return file_te
+00001210: 6d70 6c61 7465 2e72 656e 6465 7228 2a61  mplate.render(*a
+00001220: 7267 732c 202a 2a6b 7761 7267 7329 0a0a  rgs, **kwargs)..
+00001230: 0a64 6566 2077 7269 7465 5f66 696c 6528  .def write_file(
+00001240: 7061 7468 2c20 636f 6e74 656e 7473 293a  path, contents):
+00001250: 0a20 2020 2022 2222 5772 6974 6573 2074  .    """Writes t
+00001260: 6865 2053 7472 696e 6720 636f 6e74 656e  he String conten
+00001270: 7473 2074 6f20 6120 6669 6c65 2061 7420  ts to a file at 
+00001280: 7061 7468 2222 220a 0a20 2020 2069 6620  path"""..    if 
+00001290: 7379 732e 7665 7273 696f 6e5f 696e 666f  sys.version_info
+000012a0: 5b30 5d20 3c20 3320 616e 6420 6973 696e  [0] < 3 and isin
+000012b0: 7374 616e 6365 2863 6f6e 7465 6e74 732c  stance(contents,
+000012c0: 2073 7472 293a 0a20 2020 2020 2020 2063   str):.        c
+000012d0: 6f6e 7465 6e74 7320 3d20 756e 6963 6f64  ontents = unicod
+000012e0: 6528 636f 6e74 656e 7473 2c20 2275 7466  e(contents, "utf
+000012f0: 2d38 2229 0a0a 2020 2020 7769 7468 2069  -8")..    with i
+00001300: 6f2e 6f70 656e 2870 6174 682c 206d 6f64  o.open(path, mod
+00001310: 653d 2277 7422 2c20 656e 636f 6469 6e67  e="wt", encoding
+00001320: 3d22 7574 662d 3822 2c20 6e65 776c 696e  ="utf-8", newlin
+00001330: 653d 225c 6e22 2920 6173 2074 6865 5f66  e="\n") as the_f
+00001340: 696c 653a 0a20 2020 2020 2020 2074 6865  ile:.        the
+00001350: 5f66 696c 652e 7772 6974 6528 636f 6e74  _file.write(cont
+00001360: 656e 7473 290a 0a0a 6465 6620 7772 6974  ents)...def writ
+00001370: 655f 6c61 7465 7374 5f70 7970 695f 746d  e_latest_pypi_tm
+00001380: 705f 6669 6c65 286c 6174 6573 745f 7665  p_file(latest_ve
+00001390: 7273 696f 6e2c 2070 6174 685f 7364 6b5f  rsion, path_sdk_
+000013a0: 746d 705f 7079 7069 5f76 6572 7369 6f6e  tmp_pypi_version
+000013b0: 293a 0a20 2020 2022 2222 0a20 2020 2057  ):.    """.    W
+000013c0: 7269 7465 7320 7468 6520 6060 6c61 7465  rites the ``late
+000013d0: 7374 5f76 6572 7369 6f6e 6060 2061 6e64  st_version`` and
+000013e0: 2074 6865 2074 7320 6f66 2074 6865 2063   the ts of the c
+000013f0: 7572 7265 6e74 2074 696d 650a 2020 2020  urrent time.    
+00001400: 746f 2060 6070 6174 685f 7364 6b5f 746d  to ``path_sdk_tm
+00001410: 705f 7079 7069 5f76 6572 7369 6f6e 6060  p_pypi_version``
+00001420: 0a0a 2020 2020 4966 2060 606c 6174 6573  ..    If ``lates
+00001430: 745f 7665 7273 696f 6e60 6020 6973 2061  t_version`` is a
+00001440: 2060 6070 6b67 5f72 6573 6f75 7263 6573   ``pkg_resources
+00001450: 2e56 6572 7369 6f6e 6060 2c20 6765 7420  .Version``, get 
+00001460: 6974 7320 6060 6261 7365 5f76 6572 7369  its ``base_versi
+00001470: 6f6e 6060 2e0a 2020 2020 4e6f 7465 3a20  on``..    Note: 
+00001480: 7468 6973 2069 7320 6163 7475 616c 6c79  this is actually
+00001490: 2061 2064 6966 6665 7265 6e74 2056 6572   a different Ver
+000014a0: 7369 6f6e 2074 7970 6520 2d20 7765 2077  sion type - we w
+000014b0: 6f75 6c64 2068 6176 6520 746f 2069 6d70  ould have to imp
+000014c0: 6f72 7420 6578 7472 610a 2020 2020 6465  ort extra.    de
+000014d0: 7065 6e64 656e 6369 6573 2074 6f20 636f  pendencies to co
+000014e0: 7272 6563 746c 7920 7573 6520 6973 696e  rrectly use isin
+000014f0: 7374 616e 6365 286c 6174 6573 745f 7665  stance(latest_ve
+00001500: 7273 696f 6e2c 2056 6572 7369 6f6e 2920  rsion, Version) 
+00001510: 2d20 736f 206a 7573 7420 6368 6563 6b69  - so just checki
+00001520: 6e67 0a20 2020 2069 6620 6974 2068 6173  ng.    if it has
+00001530: 2074 6865 2061 7474 7269 6275 7465 0a20   the attribute. 
+00001540: 2020 2022 2222 0a20 2020 2023 2054 7279     """.    # Try
+00001550: 2067 6574 2074 6865 2027 6261 7365 5f76   get the 'base_v
+00001560: 6572 7369 6f6e 2720 6966 2074 6869 7320  ersion' if this 
+00001570: 6973 2061 2056 6572 7369 6f6e 206f 626a  is a Version obj
+00001580: 6563 740a 2020 2020 6966 2069 7369 6e73  ect.    if isins
+00001590: 7461 6e63 6528 6c61 7465 7374 5f76 6572  tance(latest_ver
+000015a0: 7369 6f6e 2c20 6f62 6a65 6374 293a 0a20  sion, object):. 
+000015b0: 2020 2020 2020 206c 6174 6573 745f 7665         latest_ve
+000015c0: 7273 696f 6e20 3d20 6765 7461 7474 7228  rsion = getattr(
+000015d0: 6c61 7465 7374 5f76 6572 7369 6f6e 2c20  latest_version, 
+000015e0: 2262 6173 655f 7665 7273 696f 6e22 2c20  "base_version", 
+000015f0: 6c61 7465 7374 5f76 6572 7369 6f6e 290a  latest_version).
+00001600: 0a20 2020 2073 6176 6564 5f76 6572 7369  .    saved_versi
+00001610: 6f6e 5f64 6174 6120 3d20 7b0a 2020 2020  on_data = {.    
+00001620: 2020 2020 2274 7322 3a20 696e 7428 7469      "ts": int(ti
+00001630: 6d65 2e74 696d 6528 2929 2c0a 2020 2020  me.time()),.    
+00001640: 2020 2020 2276 6572 7369 6f6e 223a 206c      "version": l
+00001650: 6174 6573 745f 7665 7273 696f 6e0a 2020  atest_version.  
+00001660: 2020 7d0a 0a20 2020 2077 7269 7465 5f66    }..    write_f
+00001670: 696c 6528 7061 7468 5f73 646b 5f74 6d70  ile(path_sdk_tmp
+00001680: 5f70 7970 695f 7665 7273 696f 6e2c 206a  _pypi_version, j
+00001690: 736f 6e2e 6475 6d70 7328 7361 7665 645f  son.dumps(saved_
+000016a0: 7665 7273 696f 6e5f 6461 7461 2929 0a0a  version_data))..
+000016b0: 0a64 6566 2072 6561 645f 6669 6c65 2870  .def read_file(p
+000016c0: 6174 6829 3a0a 2020 2020 2222 2252 6574  ath):.    """Ret
+000016d0: 7572 6e73 2061 6c6c 2074 6865 206c 696e  urns all the lin
+000016e0: 6573 206f 6620 6120 6669 6c65 2061 7420  es of a file at 
+000016f0: 7061 7468 2061 7320 6120 4c69 7374 2222  path as a List""
+00001700: 220a 2020 2020 6669 6c65 5f6c 696e 6573  ".    file_lines
+00001710: 203d 205b 5d0a 2020 2020 7769 7468 2069   = [].    with i
+00001720: 6f2e 6f70 656e 2870 6174 682c 206d 6f64  o.open(path, mod
+00001730: 653d 2272 7422 2c20 656e 636f 6469 6e67  e="rt", encoding
+00001740: 3d22 7574 662d 3822 2920 6173 2074 6865  ="utf-8") as the
+00001750: 5f66 696c 653a 0a20 2020 2020 2020 2066  _file:.        f
+00001760: 696c 655f 6c69 6e65 7320 3d20 7468 655f  ile_lines = the_
+00001770: 6669 6c65 2e72 6561 646c 696e 6573 2829  file.readlines()
+00001780: 0a20 2020 2072 6574 7572 6e20 6669 6c65  .    return file
+00001790: 5f6c 696e 6573 0a0a 0a64 6566 2072 6561  _lines...def rea
+000017a0: 645f 6a73 6f6e 5f66 696c 6528 7061 7468  d_json_file(path
+000017b0: 2c20 7365 6374 696f 6e3d 4e6f 6e65 293a  , section=None):
+000017c0: 0a20 2020 2022 2222 0a20 2020 2049 6620  .    """.    If 
+000017d0: 7468 6520 636f 6e74 656e 7473 206f 6620  the contents of 
+000017e0: 7468 6520 6669 6c65 2061 7420 7061 7468  the file at path
+000017f0: 2069 7320 7661 6c69 6420 4a53 4f4e 2c0a   is valid JSON,.
+00001800: 2020 2020 7265 7475 726e 7320 7468 6520      returns the 
+00001810: 636f 6e74 656e 7473 206f 6620 7468 6520  contents of the 
+00001820: 6669 6c65 2061 7320 6120 6469 6374 696f  file as a dictio
+00001830: 6e61 7279 0a0a 2020 2020 3a70 6172 616d  nary..    :param
+00001840: 2070 6174 683a 2050 6174 6820 746f 204a   path: Path to J
+00001850: 534f 4e20 6669 6c65 2074 6f20 7265 6164  SON file to read
+00001860: 0a20 2020 203a 7479 7065 2070 6174 683a  .    :type path:
+00001870: 2073 7472 0a20 2020 203a 7061 7261 6d20   str.    :param 
+00001880: 7365 6374 696f 6e3a 2053 6563 7469 6f6e  section: Section
+00001890: 206e 616d 6520 696e 204a 534f 4e20 6669   name in JSON fi
+000018a0: 6c65 2028 6567 2e20 636f 6d6d 616e 6473  le (eg. commands
+000018b0: 2069 6e20 7265 7369 6c69 656e 742d 7364   in resilient-sd
+000018c0: 6b29 0a20 2020 203a 7479 7065 2073 6563  k).    :type sec
+000018d0: 7469 6f6e 3a20 7374 720a 2020 2020 3a72  tion: str.    :r
+000018e0: 6574 7572 6e3a 2046 696c 6520 636f 6e74  eturn: File cont
+000018f0: 656e 7473 2061 7320 6120 6469 6374 696f  ents as a dictio
+00001900: 6e61 7279 0a20 2020 203a 7274 7970 653a  nary.    :rtype:
+00001910: 2064 6963 740a 2020 2020 2222 220a 2020   dict.    """.  
+00001920: 2020 6669 6c65 5f63 6f6e 7465 6e74 7320    file_contents 
+00001930: 3d20 4e6f 6e65 0a20 2020 2077 6974 6820  = None.    with 
+00001940: 696f 2e6f 7065 6e28 7061 7468 2c20 6d6f  io.open(path, mo
+00001950: 6465 3d22 7274 222c 2065 6e63 6f64 696e  de="rt", encodin
+00001960: 673d 2275 7466 2d38 2229 2061 7320 7468  g="utf-8") as th
+00001970: 655f 6669 6c65 3a0a 2020 2020 2020 2020  e_file:.        
+00001980: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00001990: 2066 696c 655f 636f 6e74 656e 7473 203d   file_contents =
+000019a0: 206a 736f 6e2e 6c6f 6164 2874 6865 5f66   json.load(the_f
+000019b0: 696c 6529 0a20 2020 2020 2020 2023 2049  ile).        # I
+000019c0: 6e20 5059 322e 3720 6974 2072 6169 7365  n PY2.7 it raise
+000019d0: 7320 6120 5661 6c75 6545 7272 6f72 2061  s a ValueError a
+000019e0: 6e64 2069 6e20 5059 332e 3620 6974 2072  nd in PY3.6 it r
+000019f0: 6169 7365 730a 2020 2020 2020 2020 2320  aises.        # 
+00001a00: 6120 4a53 4f4e 4465 636f 6465 4572 726f  a JSONDecodeErro
+00001a10: 7220 6966 2069 7420 6361 6e6e 6f74 206c  r if it cannot l
+00001a20: 6f61 6420 7468 6520 4a53 4f4e 2066 726f  oad the JSON fro
+00001a30: 6d20 7468 6520 6669 6c65 0a20 2020 2020  m the file.     
+00001a40: 2020 2065 7863 6570 7420 2856 616c 7565     except (Value
+00001a50: 4572 726f 722c 204a 534f 4e44 6563 6f64  Error, JSONDecod
+00001a60: 6545 7272 6f72 2920 6173 2065 7272 3a0a  eError) as err:.
+00001a70: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00001a80: 6520 5344 4b45 7863 6570 7469 6f6e 2822  e SDKException("
+00001a90: 436f 756c 6420 6e6f 7420 7265 6164 2063  Could not read c
+00001aa0: 6f72 7275 7074 204a 534f 4e20 6669 6c65  orrupt JSON file
+00001ab0: 2061 7420 7b30 7d5c 6e7b 317d 222e 666f   at {0}\n{1}".fo
+00001ac0: 726d 6174 2870 6174 682c 2065 7272 2929  rmat(path, err))
+00001ad0: 0a20 2020 2069 6620 7365 6374 696f 6e3a  .    if section:
+00001ae0: 0a20 2020 2020 2020 2069 6620 7365 6374  .        if sect
+00001af0: 696f 6e20 696e 2066 696c 655f 636f 6e74  ion in file_cont
+00001b00: 656e 7473 3a0a 2020 2020 2020 2020 2020  ents:.          
+00001b10: 2020 7265 7475 726e 2066 696c 655f 636f    return file_co
+00001b20: 6e74 656e 7473 2e67 6574 2873 6563 7469  ntents.get(secti
+00001b30: 6f6e 2c20 7b7d 290a 2020 2020 2020 2020  on, {}).        
+00001b40: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00001b50: 2020 4c4f 472e 6465 6275 6728 2253 6563    LOG.debug("Sec
+00001b60: 7469 6f6e 207b 7d20 6e6f 7420 666f 756e  tion {} not foun
+00001b70: 6420 696e 2070 726f 7669 6465 6420 4a53  d in provided JS
+00001b80: 4f4e 2e22 2e66 6f72 6d61 7428 7365 6374  ON.".format(sect
+00001b90: 696f 6e29 290a 2020 2020 2020 2020 2020  ion)).          
+00001ba0: 2020 7265 7475 726e 207b 7d0a 2020 2020    return {}.    
+00001bb0: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
+00001bc0: 7475 726e 2066 696c 655f 636f 6e74 656e  turn file_conten
+00001bd0: 7473 0a0a 0a64 6566 2072 6561 645f 7a69  ts...def read_zi
+00001be0: 705f 6669 6c65 2870 6174 682c 2070 6174  p_file(path, pat
+00001bf0: 7465 726e 293a 0a20 2020 2022 2222 5265  tern):.    """Re
+00001c00: 7475 726e 7320 756e 7a69 7070 6564 2063  turns unzipped c
+00001c10: 6f6e 7465 6e74 7320 6f66 2066 696c 6520  ontents of file 
+00001c20: 7768 6f73 6520 6e61 6d65 206d 6174 6368  whose name match
+00001c30: 6573 2061 2070 6174 7465 726e 0a20 2020  es a pattern.   
+00001c40: 2069 6e20 7a69 7020 6669 6c65 2061 7420   in zip file at 
+00001c50: 7061 7468 2e0a 0a20 2020 203a 7061 7261  path...    :para
+00001c60: 6d20 7061 7468 3a20 5061 7468 2074 6f20  m path: Path to 
+00001c70: 7a69 7020 6669 6c65 2e0a 2020 2020 3a70  zip file..    :p
+00001c80: 6172 616d 2070 6174 7465 726e 3a20 4669  aram pattern: Fi
+00001c90: 6c65 2070 6174 7465 726e 2074 6f20 6d61  le pattern to ma
+00001ca0: 7463 6820 696e 2074 6865 207a 6970 2066  tch in the zip f
+00001cb0: 696c 652e 0a20 2020 203a 7265 7475 726e  ile..    :return
+00001cc0: 3a20 6669 6c65 5f63 6f6e 7465 6e74 3a20  : file_content: 
+00001cd0: 5265 7475 726e 2075 6e7a 6970 7065 6420  Return unzipped 
+00001ce0: 6669 6c65 2063 6f6e 7465 6e74 2e0a 2020  file content..  
+00001cf0: 2020 2222 220a 2020 2020 6669 6c65 5f63    """.    file_c
+00001d00: 6f6e 7465 6e74 203d 204e 6f6e 650a 2020  ontent = None.  
+00001d10: 2020 7472 793a 0a20 2020 2020 2020 2077    try:.        w
+00001d20: 6974 6820 5a69 7046 696c 6528 2870 6174  ith ZipFile((pat
+00001d30: 6829 2c20 2772 2729 2061 7320 7a6f 626a  h), 'r') as zobj
+00001d40: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00001d50: 4765 7420 616c 6c20 6669 6c65 206e 616d  Get all file nam
+00001d60: 6573 206d 6174 6368 696e 6720 2770 6174  es matching 'pat
+00001d70: 7465 726e 272e 0a20 2020 2020 2020 2020  tern'..         
+00001d80: 2020 2066 696c 655f 6d61 7463 6865 7320     file_matches 
+00001d90: 3d20 5b66 2066 6f72 2066 2069 6e20 7a6f  = [f for f in zo
+00001da0: 626a 2e6e 616d 656c 6973 7428 2920 6966  bj.namelist() if
+00001db0: 2070 6174 7465 726e 2e6c 6f77 6572 2829   pattern.lower()
+00001dc0: 2069 6e20 662e 6c6f 7765 7228 295d 0a20   in f.lower()]. 
+00001dd0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00001de0: 6e28 6669 6c65 5f6d 6174 6368 6573 293a  n(file_matches):
+00001df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001e00: 2069 6620 6c65 6e28 6669 6c65 5f6d 6174   if len(file_mat
+00001e10: 6368 6573 2920 3e20 313a 0a20 2020 2020  ches) > 1:.     
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00001e30: 6169 7365 2053 444b 4578 6365 7074 696f  aise SDKExceptio
+00001e40: 6e28 224d 6f72 6520 7468 616e 206f 6e65  n("More than one
+00001e50: 2066 696c 6520 6d61 7463 6869 6e67 2070   file matching p
+00001e60: 6174 7465 726e 207b 307d 2066 6f75 6e64  attern {0} found
+00001e70: 2069 6e20 7a69 7020 6669 6c65 3a20 7b31   in zip file: {1
+00001e80: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+00001e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ea0: 2020 2020 2020 2020 2020 2e66 6f72 6d61            .forma
+00001eb0: 7428 7061 7474 6572 6e2c 2070 6174 6829  t(pattern, path)
+00001ec0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00001ed0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00001ee0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00001ef0: 5f6e 616d 6520 3d20 6669 6c65 5f6d 6174  _name = file_mat
+00001f00: 6368 6573 2e70 6f70 2829 0a20 2020 2020  ches.pop().     
+00001f10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00001f20: 2045 7874 7261 6374 2074 6865 2066 696c   Extract the fil
+00001f30: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
+00001f40: 2020 2020 2020 2066 203d 207a 6f62 6a2e         f = zobj.
+00001f50: 6f70 656e 2866 696c 655f 6e61 6d65 290a  open(file_name).
+00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f70: 2020 2020 2320 5265 6164 2066 696c 6520      # Read file 
+00001f80: 616e 6420 636f 6e76 6572 7420 636f 6e74  and convert cont
+00001f90: 656e 7420 6672 6f6d 2062 7974 6573 2074  ent from bytes t
+00001fa0: 6f20 7374 7269 6e67 2e0a 2020 2020 2020  o string..      
+00001fb0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00001fc0: 6c65 5f63 6f6e 7465 6e74 203d 2066 2e72  le_content = f.r
+00001fd0: 6561 6428 292e 6465 636f 6465 2827 7574  ead().decode('ut
+00001fe0: 6638 272c 2027 6967 6e6f 7265 2729 0a20  f8', 'ignore'). 
+00001ff0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00002000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002010: 2072 6169 7365 2053 444b 4578 6365 7074   raise SDKExcept
+00002020: 696f 6e28 2241 2066 696c 6520 6d61 7463  ion("A file matc
+00002030: 6869 6e67 2070 6174 7465 726e 207b 307d  hing pattern {0}
+00002040: 2077 6173 206e 6f74 2066 6f75 6e64 2069   was not found i
+00002050: 6e20 7a69 7020 6669 6c65 3a20 7b31 7d22  n zip file: {1}"
+00002060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002080: 2020 2020 2e66 6f72 6d61 7428 7061 7474      .format(patt
+00002090: 6572 6e2c 2070 6174 6829 290a 2020 2020  ern, path)).    
+000020a0: 6578 6365 7074 2042 6164 5a69 7066 696c  except BadZipfil
+000020b0: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
+000020c0: 2053 444b 4578 6365 7074 696f 6e28 2242   SDKException("B
+000020d0: 6164 207a 6970 2066 696c 6520 7b30 7d2e  ad zip file {0}.
+000020e0: 222e 666f 726d 6174 2870 6174 6829 290a  ".format(path)).
+000020f0: 0a20 2020 2065 7863 6570 7420 5344 4b45  .    except SDKE
+00002100: 7863 6570 7469 6f6e 2061 7320 6572 723a  xception as err:
+00002110: 0a20 2020 2020 2020 2072 6169 7365 2065  .        raise e
+00002120: 7272 0a0a 2020 2020 6578 6365 7074 2045  rr..    except E
+00002130: 7863 6570 7469 6f6e 2061 7320 6572 723a  xception as err:
+00002140: 0a20 2020 2020 2020 2023 2041 6e20 616e  .        # An an
+00002150: 2075 6e65 7870 6563 7465 6420 6572 726f   unexpected erro
+00002160: 7220 7472 7969 6e67 2074 6f20 7265 6164  r trying to read
+00002170: 2061 207a 6970 6669 6c65 2e0a 2020 2020   a zipfile..    
+00002180: 2020 2020 7261 6973 6520 5344 4b45 7863      raise SDKExc
+00002190: 6570 7469 6f6e 2822 476f 7420 616e 2065  eption("Got an e
+000021a0: 7272 6f72 2027 7b30 7d27 2061 7474 656d  rror '{0}' attem
+000021b0: 7074 696e 6720 746f 2072 6561 6420 7a69  pting to read zi
+000021c0: 7020 6669 6c65 207b 317d 222e 666f 726d  p file {1}".form
+000021d0: 6174 2865 7272 2c20 7061 7468 2929 0a0a  at(err, path))..
+000021e0: 2020 2020 7265 7475 726e 2066 696c 655f      return file_
+000021f0: 636f 6e74 656e 740a 0a0a 6465 6620 7265  content...def re
+00002200: 6e61 6d65 5f66 696c 6528 7061 7468 5f63  name_file(path_c
+00002210: 7572 7265 6e74 5f66 696c 652c 206e 6577  urrent_file, new
+00002220: 5f6e 616d 6529 3a0a 2020 2020 2222 2252  _name):.    """R
+00002230: 656e 616d 6573 2074 6865 2066 696c 6520  enames the file 
+00002240: 6174 2070 6174 685f 6375 7272 656e 745f  at path_current_
+00002250: 6669 6c65 2077 6974 6820 7468 6520 6e65  file with the ne
+00002260: 775f 6e61 6d65 2222 220a 2020 2020 6f73  w_name""".    os
+00002270: 2e72 656e 616d 6528 7061 7468 5f63 7572  .rename(path_cur
+00002280: 7265 6e74 5f66 696c 652c 206f 732e 7061  rent_file, os.pa
+00002290: 7468 2e6a 6f69 6e28 6f73 2e70 6174 682e  th.join(os.path.
+000022a0: 6469 726e 616d 6528 7061 7468 5f63 7572  dirname(path_cur
+000022b0: 7265 6e74 5f66 696c 6529 2c20 6e65 775f  rent_file), new_
+000022c0: 6e61 6d65 2929 0a0a 0a64 6566 2069 735f  name))...def is_
+000022d0: 7661 6c69 645f 7061 636b 6167 655f 6e61  valid_package_na
+000022e0: 6d65 286e 616d 6529 3a0a 2020 2020 2222  me(name):.    ""
+000022f0: 2254 6573 7420 6966 2027 6e61 6d65 2720  "Test if 'name' 
+00002300: 6973 2061 2076 616c 6964 2069 6465 6e74  is a valid ident
+00002310: 6966 6965 7220 666f 7220 6120 7061 636b  ifier for a pack
+00002320: 6167 6520 6f72 206d 6f64 756c 650a 0a20  age or module.. 
+00002330: 2020 2020 2020 3e3e 3e20 6973 5f76 616c        >>> is_val
+00002340: 6964 5f70 6163 6b61 6765 5f6e 616d 6528  id_package_name(
+00002350: 2222 290a 2020 2020 2020 2046 616c 7365  "").       False
+00002360: 0a20 2020 2020 2020 3e3e 3e20 6973 5f76  .       >>> is_v
+00002370: 616c 6964 5f70 6163 6b61 6765 5f6e 616d  alid_package_nam
+00002380: 6528 4e6f 6e65 290a 2020 2020 2020 2046  e(None).       F
+00002390: 616c 7365 0a20 2020 2020 2020 3e3e 3e20  alse.       >>> 
+000023a0: 6973 5f76 616c 6964 5f70 6163 6b61 6765  is_valid_package
+000023b0: 5f6e 616d 6528 2267 6574 2229 0a20 2020  _name("get").   
+000023c0: 2020 2020 4661 6c73 650a 2020 2020 2020      False.      
+000023d0: 203e 3e3e 2069 735f 7661 6c69 645f 7061   >>> is_valid_pa
+000023e0: 636b 6167 655f 6e61 6d65 2822 6261 6e67  ckage_name("bang
+000023f0: 2122 290a 2020 2020 2020 2046 616c 7365  !").       False
+00002400: 0a20 2020 2020 2020 3e3e 3e20 6973 5f76  .       >>> is_v
+00002410: 616c 6964 5f70 6163 6b61 6765 5f6e 616d  alid_package_nam
+00002420: 6528 225f 736f 6d65 7468 696e 6722 290a  e("_something").
+00002430: 2020 2020 2020 2054 7275 650a 2020 2020         True.    
+00002440: 2020 203e 3e3e 2069 735f 7661 6c69 645f     >>> is_valid_
+00002450: 7061 636b 6167 655f 6e61 6d65 2822 2d73  package_name("-s
+00002460: 6f6d 6574 6869 6e67 2229 0a20 2020 2020  omething").     
+00002470: 2020 5472 7565 0a20 2020 2022 2222 0a0a    True.    """..
+00002480: 2020 2020 6966 206b 6579 776f 7264 2e69      if keyword.i
+00002490: 736b 6579 776f 7264 286e 616d 6529 3a0a  skeyword(name):.
+000024a0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+000024b0: 616c 7365 0a20 2020 2065 6c69 6620 6e61  alse.    elif na
+000024c0: 6d65 2069 6e20 6469 7228 5f5f 6275 696c  me in dir(__buil
+000024d0: 7469 6e73 5f5f 293a 0a20 2020 2020 2020  tins__):.       
 000024e0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-000024f0: 2020 7265 7475 726e 2072 652e 6d61 7463    return re.matc
-00002500: 6828 7222 5b28 5f7c 5c2d 2961 2d7a 5d5b  h(r"[(_|\-)a-z][
-00002510: 285f 7c5c 2d29 612d 7a30 2d39 5d2a 2422  (_|\-)a-z0-9]*$"
-00002520: 2c20 6e61 6d65 2920 6973 206e 6f74 204e  , name) is not N
-00002530: 6f6e 650a 0a0a 6465 6620 6973 5f76 616c  one...def is_val
-00002540: 6964 5f76 6572 7369 6f6e 5f73 796e 7461  id_version_synta
-00002550: 7828 7665 7273 696f 6e29 3a0a 2020 2020  x(version):.    
-00002560: 2222 220a 2020 2020 5265 7475 726e 7320  """.    Returns 
-00002570: 5472 7565 2069 6620 7665 7273 696f 6e20  True if version 
-00002580: 6973 2076 616c 6964 2c20 656c 7365 2046  is valid, else F
-00002590: 616c 7365 2e20 4163 6365 7074 6564 2076  alse. Accepted v
-000025a0: 6572 7369 6f6e 2065 7861 6d70 6c65 7320  ersion examples 
-000025b0: 6172 653a 0a20 2020 2020 2020 2022 312e  are:.        "1.
-000025c0: 302e 3022 2022 312e 312e 3022 2022 3132  0.0" "1.1.0" "12
-000025d0: 332e 302e 3132 3322 0a20 2020 2022 2222  3.0.123".    """
-000025e0: 0a20 2020 2069 6620 6e6f 7420 7665 7273  .    if not vers
-000025f0: 696f 6e3a 0a20 2020 2020 2020 2072 6574  ion:.        ret
-00002600: 7572 6e20 4661 6c73 650a 0a20 2020 2023  urn False..    #
-00002610: 2061 6464 6564 2069 6e20 7635 312e 3020   added in v51.0 
-00002620: 7468 6520 6162 696c 6974 7920 746f 2068  the ability to h
-00002630: 6176 6520 6d6f 7265 2074 6861 6e20 7468  ave more than th
-00002640: 7265 6520 6e75 6d62 6572 7320 696e 2074  ree numbers in t
-00002650: 6865 2076 6572 7369 6f6e 0a20 2020 2023  he version.    #
-00002660: 2028 6d69 6e20 7374 696c 6c20 3329 2073   (min still 3) s
-00002670: 696e 6365 206e 6577 2076 6572 7369 6f6e  ince new version
-00002680: 696e 6720 7363 6865 6d65 2068 6173 2035  ing scheme has 5
-00002690: 2821 2129 206e 756d 6265 7273 0a20 2020  (!!) numbers.   
-000026a0: 2072 6567 6578 203d 2072 652e 636f 6d70   regex = re.comp
-000026b0: 696c 6528 7227 5e5c 642b 5c2e 5c64 2b5c  ile(r'^\d+\.\d+\
-000026c0: 2e5c 642b 283f 3a5c 2e5c 642b 292a 2427  .\d+(?:\.\d+)*$'
-000026d0: 290a 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
-000026e0: 6765 782e 6d61 7463 6828 7665 7273 696f  gex.match(versio
-000026f0: 6e29 2069 7320 6e6f 7420 4e6f 6e65 0a0a  n) is not None..
-00002700: 0a64 6566 2069 735f 7661 6c69 645f 7572  .def is_valid_ur
-00002710: 6c28 7572 6c29 3a0a 2020 2020 2222 220a  l(url):.    """.
-00002720: 2020 2020 5265 7475 726e 7320 5472 7565      Returns True
-00002730: 2069 6620 7572 6c20 6973 2076 616c 6964   if url is valid
-00002740: 2c20 656c 7365 2046 616c 7365 2e20 4163  , else False. Ac
-00002750: 6365 7074 6564 2075 726c 2065 7861 6d70  cepted url examp
-00002760: 6c65 7320 6172 653a 0a20 2020 2020 2020  les are:.       
-00002770: 2022 6874 7470 3a2f 2f77 7777 2e65 7861   "http://www.exa
-00002780: 6d70 6c65 2e63 6f6d 3a38 3030 3022 2c20  mple.com:8000", 
-00002790: 2268 7474 7073 3a2f 2f77 7777 2e65 7861  "https://www.exa
-000027a0: 6d70 6c65 2e63 6f6d 222c 2022 7777 772e  mple.com", "www.
-000027b0: 6578 616d 706c 652e 636f 6d22 2c20 2265  example.com", "e
-000027c0: 7861 6d70 6c65 2e63 6f6d 220a 2020 2020  xample.com".    
-000027d0: 2222 220a 0a20 2020 2069 6620 6e6f 7420  """..    if not 
-000027e0: 7572 6c3a 0a20 2020 2020 2020 2072 6574  url:.        ret
-000027f0: 7572 6e20 4661 6c73 650a 0a20 2020 2072  urn False..    r
-00002800: 6567 6578 203d 2072 652e 636f 6d70 696c  egex = re.compil
-00002810: 6528 0a20 2020 2020 2020 2072 275e 2868  e(.        r'^(h
-00002820: 7474 7073 3f3a 2f2f 293f 2720 2023 206f  ttps?://)?'  # o
-00002830: 7074 696f 6e61 6c20 6874 7470 3a2f 2f20  ptional http:// 
-00002840: 6f72 2068 7474 7073 3a2f 2f0a 2020 2020  or https://.    
-00002850: 2020 2020 7227 283f 3a28 3f3a 5b41 2d5a      r'(?:(?:[A-Z
-00002860: 302d 395d 283f 3a5b 412d 5a30 2d39 2d5d  0-9](?:[A-Z0-9-]
-00002870: 7b30 2c36 317d 5b41 2d5a 302d 395d 293f  {0,61}[A-Z0-9])?
-00002880: 5c2e 292b 5b41 2d5a 5d7b 322c 367d 5c2e  \.)+[A-Z]{2,6}\.
-00002890: 3f29 2720 2023 2064 6f6d 6169 6e2f 686f  ?)'  # domain/ho
-000028a0: 7374 6e61 6d65 0a20 2020 2020 2020 2072  stname.        r
-000028b0: 2728 3f3a 2f3f 7c5b 2f3f 5d5c 532b 2927  '(?:/?|[/?]\S+)'
-000028c0: 2020 2320 2e63 6f6d 2065 7463 2e0a 2020    # .com etc..  
-000028d0: 2020 2020 2020 7227 283f 3a3a 5c64 7b31        r'(?::\d{1
-000028e0: 2c35 7d29 3f24 272c 2020 2320 706f 7274  ,5})?$',  # port
-000028f0: 206e 756d 6265 720a 2020 2020 2020 2020   number.        
-00002900: 7265 2e49 474e 4f52 4543 4153 4529 0a0a  re.IGNORECASE)..
-00002910: 2020 2020 7265 7475 726e 2072 6567 6578      return regex
-00002920: 2e73 6561 7263 6828 7572 6c29 2069 7320  .search(url) is 
-00002930: 6e6f 7420 4e6f 6e65 0a0a 0a64 6566 2069  not None...def i
-00002940: 735f 7661 6c69 645f 6861 7368 2869 6e70  s_valid_hash(inp
-00002950: 7574 5f68 6173 6829 3a0a 2020 2020 2222  ut_hash):.    ""
-00002960: 2252 6574 7572 6e73 2054 7275 6520 6966  "Returns True if
-00002970: 2074 6865 2069 6e70 7574 5f68 6173 6820   the input_hash 
-00002980: 6973 2061 2076 616c 6964 2053 4841 3235  is a valid SHA25
-00002990: 3620 6861 7368 2e0a 2020 2020 5265 7475  6 hash..    Retu
-000029a0: 726e 7320 4661 6c73 6520 6966 3b0a 2020  rns False if;.  
-000029b0: 2020 2020 2020 2d20 2020 696e 7075 745f        -   input_
-000029c0: 6861 7368 2069 7320 6e6f 7420 6120 7374  hash is not a st
-000029d0: 720a 2020 2020 2020 2020 2d20 2020 696e  r.        -   in
-000029e0: 7075 745f 6861 7368 2069 7320 6e6f 7420  put_hash is not 
-000029f0: 6571 7561 6c20 746f 2036 3420 6368 6172  equal to 64 char
-00002a00: 6163 7465 7273 0a20 2020 2020 2020 202d  acters.        -
-00002a10: 2020 2074 6861 7420 616c 6c20 6368 6172     that all char
-00002a20: 6163 7465 7273 2069 6e20 696e 7075 745f  acters in input_
-00002a30: 6861 7368 2061 7265 2062 6173 6520 3136  hash are base 16
-00002a40: 2028 7661 6c69 6420 6865 7861 6465 6369   (valid hexadeci
-00002a50: 6d61 6c29 0a0a 2020 2020 3a70 6172 616d  mal)..    :param
-00002a60: 2069 6e70 7574 5f68 6173 683a 2073 7472   input_hash: str
-00002a70: 2074 6f20 7661 6c69 6461 7465 2069 6620   to validate if 
-00002a80: 6974 7320 6120 5348 4132 3536 2068 6173  its a SHA256 has
-00002a90: 680a 2020 2020 3a74 7970 6520 696e 7075  h.    :type inpu
-00002aa0: 745f 6861 7368 3a20 7374 720a 2020 2020  t_hash: str.    
-00002ab0: 3a72 6574 7572 6e3a 2054 7275 652f 4661  :return: True/Fa
-00002ac0: 6c73 650a 2020 2020 2222 220a 2020 2020  lse.    """.    
-00002ad0: 6966 206e 6f74 2069 6e70 7574 5f68 6173  if not input_has
-00002ae0: 683a 0a20 2020 2020 2020 2072 6574 7572  h:.        retur
-00002af0: 6e20 4661 6c73 650a 0a20 2020 2072 6567  n False..    reg
-00002b00: 6578 203d 2072 652e 636f 6d70 696c 6528  ex = re.compile(
-00002b10: 7227 5e5b 612d 6630 2d39 5d7b 3634 7d28  r'^[a-f0-9]{64}(
-00002b20: 3a2e 2b29 3f24 2729 0a0a 2020 2020 7265  :.+)?$')..    re
-00002b30: 7475 726e 2072 6567 6578 2e6d 6174 6368  turn regex.match
-00002b40: 2869 6e70 7574 5f68 6173 6829 2069 7320  (input_hash) is 
-00002b50: 6e6f 7420 4e6f 6e65 0a0a 0a64 6566 2064  not None...def d
-00002b60: 6f65 735f 7572 6c5f 636f 6e74 6169 6e28  oes_url_contain(
-00002b70: 7572 6c2c 2071 7279 293a 0a20 2020 2022  url, qry):.    "
-00002b80: 2222 0a20 2020 2043 6865 636b 7320 6966  "".    Checks if
-00002b90: 2075 726c 2069 7320 6120 7661 6c69 6420   url is a valid 
-00002ba0: 7572 6c2c 2069 6620 6974 2069 736e 2774  url, if it isn't
-00002bb0: 2072 6574 7572 6e73 2046 616c 7365 2e0a   returns False..
-00002bc0: 2020 2020 4368 6563 6b73 2069 6620 7172      Checks if qr
-00002bd0: 7920 6973 2069 6e20 7572 6c2e 2052 6574  y is in url. Ret
-00002be0: 7572 6e73 2054 7275 6520 6966 2069 7420  urns True if it 
-00002bf0: 6973 0a20 2020 2022 2222 0a20 2020 2069  is.    """.    i
-00002c00: 6620 6e6f 7420 6973 5f76 616c 6964 5f75  f not is_valid_u
-00002c10: 726c 2875 726c 293a 0a20 2020 2020 2020  rl(url):.       
-00002c20: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-00002c30: 2020 2072 6574 7572 6e20 7172 7920 696e     return qry in
-00002c40: 2075 726c 0a0a 0a64 6566 2067 656e 6572   url...def gener
-00002c50: 6174 655f 7575 6964 5f66 726f 6d5f 7374  ate_uuid_from_st
-00002c60: 7269 6e67 2874 6865 5f73 7472 696e 6729  ring(the_string)
-00002c70: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-00002c80: 7475 726e 7320 5374 7269 6e67 2072 6570  turns String rep
-00002c90: 7265 7365 6e74 6174 696f 6e20 6f66 2074  resentation of t
-00002ca0: 6865 2055 5549 4420 6f66 2061 2068 6578  he UUID of a hex
-00002cb0: 206d 6435 2068 6173 6820 6f66 2074 6865   md5 hash of the
-00002cc0: 2067 6976 656e 2073 7472 696e 670a 2020   given string.  
-00002cd0: 2020 2222 220a 0a20 2020 2023 2049 6e73    """..    # Ins
-00002ce0: 7461 6e73 6961 7465 206e 6577 206d 6435  tansiate new md5
-00002cf0: 5f68 6173 680a 2020 2020 6d64 355f 6861  _hash.    md5_ha
-00002d00: 7368 203d 2068 6173 686c 6962 2e6d 6435  sh = hashlib.md5
-00002d10: 2829 0a0a 2020 2020 2320 5061 7373 2074  ()..    # Pass t
-00002d20: 6865 5f73 7472 696e 6720 746f 2074 6865  he_string to the
-00002d30: 206d 6435 5f68 6173 6820 6173 2062 7974   md5_hash as byt
-00002d40: 6573 0a20 2020 206d 6435 5f68 6173 682e  es.    md5_hash.
-00002d50: 7570 6461 7465 2874 6865 5f73 7472 696e  update(the_strin
-00002d60: 672e 656e 636f 6465 2822 7574 662d 3822  g.encode("utf-8"
-00002d70: 2929 0a0a 2020 2020 2320 4765 6e65 7261  ))..    # Genera
-00002d80: 7465 2074 6865 2068 6578 206d 6435 2068  te the hex md5 h
-00002d90: 6173 6820 6f66 2061 6c6c 2074 6865 2072  ash of all the r
-00002da0: 6561 6420 6279 7465 730a 2020 2020 7468  ead bytes.    th
-00002db0: 655f 6d64 355f 6865 785f 7374 7220 3d20  e_md5_hex_str = 
-00002dc0: 6d64 355f 6861 7368 2e68 6578 6469 6765  md5_hash.hexdige
-00002dd0: 7374 2829 0a0a 2020 2020 2320 5265 7475  st()..    # Retu
-00002de0: 726e 2061 2053 7472 696e 6720 7265 7065  rn a String repe
-00002df0: 7273 656e 6174 696f 6e20 6f66 2074 6865  rsenation of the
-00002e00: 2075 7569 6420 6f66 2074 6865 206d 6435   uuid of the md5
-00002e10: 2068 6173 680a 2020 2020 7265 7475 726e   hash.    return
-00002e20: 2073 7472 2875 7569 642e 5555 4944 2874   str(uuid.UUID(t
-00002e30: 6865 5f6d 6435 5f68 6578 5f73 7472 2929  he_md5_hex_str))
-00002e40: 0a0a 0a64 6566 2068 6173 5f70 6572 6d69  ...def has_permi
-00002e50: 7373 696f 6e73 2870 6572 6d69 7373 696f  ssions(permissio
-00002e60: 6e73 2c20 7061 7468 293a 0a20 2020 2022  ns, path):.    "
-00002e70: 2222 0a20 2020 2052 6169 7365 7320 616e  "".    Raises an
-00002e80: 2065 7863 6570 7469 6f6e 2069 6620 7468   exception if th
-00002e90: 6520 7573 6572 2064 6f65 7320 6e6f 7420  e user does not 
-00002ea0: 6861 7665 2074 6865 2067 6976 656e 2070  have the given p
-00002eb0: 6572 6d69 7373 696f 6e73 2074 6f20 7061  ermissions to pa
-00002ec0: 7468 0a20 2020 2022 2222 0a0a 2020 2020  th.    """..    
-00002ed0: 4c4f 472e 6465 6275 6728 2263 6865 636b  LOG.debug("check
-00002ee0: 696e 6720 6966 3a20 2573 2068 6173 2063  ing if: %s has c
-00002ef0: 6f72 7265 6374 2070 6572 6d69 7373 696f  orrect permissio
-00002f00: 6e73 222c 2070 6174 6829 0a0a 2020 2020  ns", path)..    
-00002f10: 6966 206e 6f74 206f 732e 6163 6365 7373  if not os.access
-00002f20: 2870 6174 682c 2070 6572 6d69 7373 696f  (path, permissio
-00002f30: 6e73 293a 0a0a 2020 2020 2020 2020 6966  ns):..        if
-00002f40: 2070 6572 6d69 7373 696f 6e73 2069 7320   permissions is 
-00002f50: 6f73 2e52 5f4f 4b3a 0a20 2020 2020 2020  os.R_OK:.       
-00002f60: 2020 2020 2070 6572 6d69 7373 696f 6e73       permissions
-00002f70: 203d 2022 5245 4144 220a 2020 2020 2020   = "READ".      
-00002f80: 2020 656c 6966 2070 6572 6d69 7373 696f    elif permissio
-00002f90: 6e73 2069 7320 6f73 2e57 5f4f 4b3a 0a20  ns is os.W_OK:. 
-00002fa0: 2020 2020 2020 2020 2020 2070 6572 6d69             permi
-00002fb0: 7373 696f 6e73 203d 2022 5752 4954 4522  ssions = "WRITE"
-00002fc0: 0a0a 2020 2020 2020 2020 7261 6973 6520  ..        raise 
-00002fd0: 5344 4b45 7863 6570 7469 6f6e 2822 5573  SDKException("Us
-00002fe0: 6572 2064 6f65 7320 6e6f 7420 6861 7665  er does not have
-00002ff0: 207b 307d 2070 6572 6d69 7373 696f 6e73   {0} permissions
-00003000: 2066 6f72 3a20 7b31 7d22 2e66 6f72 6d61   for: {1}".forma
-00003010: 7428 7065 726d 6973 7369 6f6e 732c 2070  t(permissions, p
-00003020: 6174 6829 290a 0a0a 6465 6620 7661 6c69  ath))...def vali
-00003030: 6461 7465 5f66 696c 655f 7061 7468 7328  date_file_paths(
-00003040: 7065 726d 6973 7369 6f6e 732c 202a 6172  permissions, *ar
-00003050: 6773 293a 0a20 2020 2022 2222 0a20 2020  gs):.    """.   
-00003060: 2043 6865 636b 2074 6865 2067 6976 656e   Check the given
-00003070: 202a 6172 6773 2070 6174 6873 2065 7869   *args paths exi
-00003080: 7374 2061 6e64 2068 6173 2074 6865 2067  st and has the g
-00003090: 6976 656e 2070 6572 6d69 7373 696f 6e73  iven permissions
-000030a0: 2c20 656c 7365 2072 6169 7365 7320 616e  , else raises an
-000030b0: 2045 7863 6570 7469 6f6e 0a20 2020 2022   Exception.    "
-000030c0: 2222 0a0a 2020 2020 2320 466f 7220 6561  ""..    # For ea
-000030d0: 6368 202a 6172 6773 0a20 2020 2066 6f72  ch *args.    for
-000030e0: 2070 6174 685f 746f 5f66 696c 6520 696e   path_to_file in
-000030f0: 2061 7267 733a 0a20 2020 2020 2020 2023   args:.        #
-00003100: 2043 6865 636b 2074 6865 2066 696c 6520   Check the file 
-00003110: 6578 6973 7473 0a20 2020 2020 2020 2069  exists.        i
-00003120: 6620 6e6f 7420 6f73 2e70 6174 682e 6973  f not os.path.is
-00003130: 6669 6c65 2870 6174 685f 746f 5f66 696c  file(path_to_fil
-00003140: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00003150: 7261 6973 6520 5344 4b45 7863 6570 7469  raise SDKExcepti
-00003160: 6f6e 2875 227b 307d 3a20 7b31 7d22 2e66  on(u"{0}: {1}".f
-00003170: 6f72 6d61 7428 636f 6e73 7461 6e74 732e  ormat(constants.
-00003180: 4552 524f 525f 4e4f 545f 4649 4e44 5f46  ERROR_NOT_FIND_F
-00003190: 494c 452c 2070 6174 685f 746f 5f66 696c  ILE, path_to_fil
-000031a0: 6529 290a 0a20 2020 2020 2020 2069 6620  e))..        if 
-000031b0: 7065 726d 6973 7369 6f6e 733a 0a20 2020  permissions:.   
-000031c0: 2020 2020 2020 2020 2023 2043 6865 636b           # Check
-000031d0: 2077 6520 6861 7665 2074 6865 2063 6f72   we have the cor
-000031e0: 7265 6374 2070 6572 6d69 7373 696f 6e73  rect permissions
-000031f0: 0a20 2020 2020 2020 2020 2020 2068 6173  .            has
-00003200: 5f70 6572 6d69 7373 696f 6e73 2870 6572  _permissions(per
-00003210: 6d69 7373 696f 6e73 2c20 7061 7468 5f74  missions, path_t
-00003220: 6f5f 6669 6c65 290a 0a0a 6465 6620 7661  o_file)...def va
-00003230: 6c69 6461 7465 5f64 6972 5f70 6174 6873  lidate_dir_paths
-00003240: 2870 6572 6d69 7373 696f 6e73 2c20 2a61  (permissions, *a
-00003250: 7267 7329 3a0a 2020 2020 2222 220a 2020  rgs):.    """.  
-00003260: 2020 4368 6563 6b20 7468 6520 6769 7665    Check the give
-00003270: 6e20 2a61 7267 7320 7061 7468 7320 6172  n *args paths ar
-00003280: 6520 4469 7265 6374 6f72 6965 7320 616e  e Directories an
-00003290: 6420 6861 7665 2074 6865 2067 6976 656e  d have the given
-000032a0: 2070 6572 6d69 7373 696f 6e73 2c20 656c   permissions, el
-000032b0: 7365 2072 6169 7365 7320 616e 2045 7863  se raises an Exc
-000032c0: 6570 7469 6f6e 0a20 2020 2022 2222 0a0a  eption.    """..
-000032d0: 2020 2020 2320 466f 7220 6561 6368 202a      # For each *
-000032e0: 6172 6773 0a20 2020 2066 6f72 2070 6174  args.    for pat
-000032f0: 685f 746f 5f64 6972 2069 6e20 6172 6773  h_to_dir in args
-00003300: 3a0a 2020 2020 2020 2020 2320 4368 6563  :.        # Chec
-00003310: 6b20 7468 6520 6469 7220 6578 6973 7473  k the dir exists
-00003320: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00003330: 6f73 2e70 6174 682e 6973 6469 7228 7061  os.path.isdir(pa
-00003340: 7468 5f74 6f5f 6469 7229 3a0a 2020 2020  th_to_dir):.    
-00003350: 2020 2020 2020 2020 7261 6973 6520 5344          raise SD
-00003360: 4b45 7863 6570 7469 6f6e 2875 227b 307d  KException(u"{0}
-00003370: 3a20 7b31 7d22 2e66 6f72 6d61 7428 636f  : {1}".format(co
-00003380: 6e73 7461 6e74 732e 4552 524f 525f 4e4f  nstants.ERROR_NO
-00003390: 545f 4649 4e44 5f44 4952 2c20 7061 7468  T_FIND_DIR, path
-000033a0: 5f74 6f5f 6469 7229 290a 0a20 2020 2020  _to_dir))..     
-000033b0: 2020 2069 6620 7065 726d 6973 7369 6f6e     if permission
-000033c0: 733a 0a20 2020 2020 2020 2020 2020 2023  s:.            #
-000033d0: 2043 6865 636b 2077 6520 6861 7665 2074   Check we have t
-000033e0: 6865 2063 6f72 7265 6374 2070 6572 6d69  he correct permi
-000033f0: 7373 696f 6e73 0a20 2020 2020 2020 2020  ssions.         
-00003400: 2020 2068 6173 5f70 6572 6d69 7373 696f     has_permissio
-00003410: 6e73 2870 6572 6d69 7373 696f 6e73 2c20  ns(permissions, 
-00003420: 7061 7468 5f74 6f5f 6469 7229 0a0a 0a64  path_to_dir)...d
-00003430: 6566 2067 6574 5f72 6573 696c 6965 6e74  ef get_resilient
-00003440: 5f73 6572 7665 725f 696e 666f 2872 6573  _server_info(res
-00003450: 5f63 6c69 656e 742c 206b 6579 735f 746f  _client, keys_to
-00003460: 5f67 6574 3d5b 5d29 3a0a 2020 2020 2222  _get=[]):.    ""
-00003470: 220a 2020 2020 4361 6c6c 7320 7468 6520  ".    Calls the 
-00003480: 636f 6e73 742f 2065 6e64 706f 696e 7420  const/ endpoint 
-00003490: 616e 6420 7265 7475 726e 7320 7468 6520  and returns the 
-000034a0: 696e 666f 2073 7065 6369 6669 6564 2069  info specified i
-000034b0: 6e20 6b65 7973 5f74 6f5f 6765 740a 0a20  n keys_to_get.. 
-000034c0: 2020 202a 2a45 7861 6d70 6c65 3a2a 2a0a     **Example:**.
-000034d0: 0a20 2020 202e 2e20 636f 6465 2d62 6c6f  .    .. code-blo
-000034e0: 636b 3a3a 2070 7974 686f 6e0a 0a20 2020  ck:: python..   
-000034f0: 2020 2020 2073 6572 7665 725f 7665 7273       server_vers
-00003500: 696f 6e20 3d20 6765 745f 7265 7369 6c69  ion = get_resili
-00003510: 656e 745f 7365 7276 6572 5f69 6e66 6f28  ent_server_info(
-00003520: 7265 735f 636c 6965 6e74 2c20 5b22 7365  res_client, ["se
-00003530: 7276 6572 5f76 6572 7369 6f6e 225d 290a  rver_version"]).
-00003540: 0a20 2020 203a 7061 7261 6d20 7265 735f  .    :param res_
-00003550: 636c 6965 6e74 3a20 7265 7175 6972 6564  client: required
-00003560: 2066 6f72 2063 6f6d 6d75 6e69 6361 7469   for communicati
-00003570: 6f6e 2062 6163 6b20 746f 2072 6573 696c  on back to resil
-00003580: 6965 6e74 0a20 2020 203a 7479 7065 2072  ient.    :type r
-00003590: 6573 5f63 6c69 656e 743a 2073 646b 5f68  es_client: sdk_h
-000035a0: 656c 7065 7273 2e67 6574 5f72 6573 696c  elpers.get_resil
-000035b0: 6965 6e74 5f63 6c69 656e 7428 290a 2020  ient_client().  
-000035c0: 2020 3a70 6172 616d 206b 6579 735f 746f    :param keys_to
-000035d0: 5f67 6574 3a20 6c69 7374 206f 6620 7374  _get: list of st
-000035e0: 7269 6e67 7320 6f66 2074 6865 206b 6579  rings of the key
-000035f0: 7320 746f 2072 6574 7572 6e20 6672 6f6d  s to return from
-00003600: 2074 6865 2063 6f6e 7374 2f20 656e 6470   the const/ endp
-00003610: 6f69 6e74 2e20 4966 2060 604e 6f6e 6560  oint. If ``None`
-00003620: 600a 2020 2020 7265 7475 726e 7320 7468  `.    returns th
-00003630: 6520 7768 6f6c 6520 7265 7370 6f6e 7365  e whole response
-00003640: 0a20 2020 203a 7479 7065 206b 6579 735f  .    :type keys_
-00003650: 746f 5f67 6574 3a20 6c69 7374 0a20 2020  to_get: list.   
-00003660: 203a 7265 7475 726e 3a20 7265 7370 6f6e   :return: respon
-00003670: 7365 2066 726f 6d20 636f 6e73 742f 0a20  se from const/. 
-00003680: 2020 203a 7274 7970 653a 2064 6963 740a     :rtype: dict.
-00003690: 2020 2020 2222 220a 2020 2020 4c4f 472e      """.    LOG.
-000036a0: 6465 6275 6728 2247 6574 7469 6e67 2073  debug("Getting s
-000036b0: 6572 7665 7220 696e 666f 2229 0a20 2020  erver info").   
-000036c0: 2073 6572 7665 725f 696e 666f 203d 2072   server_info = r
-000036d0: 6573 5f63 6c69 656e 742e 6765 7428 222f  es_client.get("/
-000036e0: 636f 6e73 742f 222c 2069 735f 7572 695f  const/", is_uri_
-000036f0: 6162 736f 6c75 7465 3d54 7275 6529 0a0a  absolute=True)..
-00003700: 2020 2020 6966 206b 6579 735f 746f 5f67      if keys_to_g
-00003710: 6574 3a0a 2020 2020 2020 2020 7365 7276  et:.        serv
-00003720: 6572 5f69 6e66 6f20 3d20 7b6b 3a20 7365  er_info = {k: se
-00003730: 7276 6572 5f69 6e66 6f2e 6765 7428 6b2c  rver_info.get(k,
-00003740: 207b 7d29 2066 6f72 206b 2069 6e20 6b65   {}) for k in ke
-00003750: 7973 5f74 6f5f 6765 747d 0a0a 2020 2020  ys_to_get}..    
-00003760: 7265 7475 726e 2073 6572 7665 725f 696e  return server_in
-00003770: 666f 0a0a 0a64 6566 2067 6574 5f72 6573  fo...def get_res
-00003780: 696c 6965 6e74 5f73 6572 7665 725f 7665  ilient_server_ve
-00003790: 7273 696f 6e28 7265 735f 636c 6965 6e74  rsion(res_client
-000037a0: 293a 0a20 2020 2022 2222 0a20 2020 2055  ):.    """.    U
-000037b0: 7365 7320 6765 745f 7265 7369 6c69 656e  ses get_resilien
-000037c0: 745f 7365 7276 6572 5f69 6e66 6f20 746f  t_server_info to
-000037d0: 2067 6574 2074 6865 2022 7365 7276 6572   get the "server
-000037e0: 5f76 6572 7369 6f6e 220a 2020 2020 616e  _version".    an
-000037f0: 6420 636f 6e76 6572 7473 2069 7420 696e  d converts it in
-00003800: 746f 2061 2056 6572 7369 6f6e 206f 626a  to a Version obj
-00003810: 6563 7420 616e 6420 7265 7475 726e 7320  ect and returns 
-00003820: 6974 0a0a 2020 2020 3a70 6172 616d 2072  it..    :param r
-00003830: 6573 5f63 6c69 656e 743a 2072 6571 7569  es_client: requi
-00003840: 7265 6420 666f 7220 636f 6d6d 756e 6963  red for communic
-00003850: 6174 696f 6e20 6261 636b 2074 6f20 7265  ation back to re
-00003860: 7369 6c69 656e 740a 2020 2020 3a74 7970  silient.    :typ
-00003870: 6520 7265 735f 636c 6965 6e74 3a20 7364  e res_client: sd
-00003880: 6b5f 6865 6c70 6572 732e 6765 745f 7265  k_helpers.get_re
-00003890: 7369 6c69 656e 745f 636c 6965 6e74 2829  silient_client()
-000038a0: 0a20 2020 203a 7265 7475 726e 3a20 7468  .    :return: th
-000038b0: 6520 7365 7276 6572 5f76 6572 7369 6f6e  e server_version
-000038c0: 2e76 6572 7369 6f6e 2076 616c 7565 0a20  .version value. 
-000038d0: 2020 203a 7274 7970 653a 2056 6572 7369     :rtype: Versi
-000038e0: 6f6e 206f 626a 6563 740a 2020 2020 2222  on object.    ""
-000038f0: 220a 2020 2020 4c4f 472e 6465 6275 6728  ".    LOG.debug(
-00003900: 2247 6574 7469 6e67 2073 6572 7665 7220  "Getting server 
-00003910: 7665 7273 696f 6e22 290a 0a20 2020 2069  version")..    i
-00003920: 6620 636f 6e73 7461 6e74 732e 4355 5252  f constants.CURR
-00003930: 454e 545f 534f 4152 5f53 4552 5645 525f  ENT_SOAR_SERVER_
-00003940: 5645 5253 494f 4e3a 0a20 2020 2020 2020  VERSION:.       
-00003950: 2072 6574 7572 6e20 636f 6e73 7461 6e74   return constant
-00003960: 732e 4355 5252 454e 545f 534f 4152 5f53  s.CURRENT_SOAR_S
-00003970: 4552 5645 525f 5645 5253 494f 4e0a 0a20  ERVER_VERSION.. 
-00003980: 2020 2073 6572 7665 725f 7665 7273 696f     server_versio
-00003990: 6e20 3d20 6765 745f 7265 7369 6c69 656e  n = get_resilien
-000039a0: 745f 7365 7276 6572 5f69 6e66 6f28 7265  t_server_info(re
-000039b0: 735f 636c 6965 6e74 2c20 5b22 7365 7276  s_client, ["serv
-000039c0: 6572 5f76 6572 7369 6f6e 225d 292e 6765  er_version"]).ge
-000039d0: 7428 2273 6572 7665 725f 7665 7273 696f  t("server_versio
-000039e0: 6e22 2c20 7b7d 290a 0a20 2020 2063 6f6e  n", {})..    con
-000039f0: 7374 616e 7473 2e43 5552 5245 4e54 5f53  stants.CURRENT_S
-00003a00: 4f41 525f 5345 5256 4552 5f56 4552 5349  OAR_SERVER_VERSI
-00003a10: 4f4e 203d 2070 6172 7365 5f76 6572 7369  ON = parse_versi
-00003a20: 6f6e 2873 6572 7665 725f 7665 7273 696f  on(server_versio
-00003a30: 6e2e 6765 7428 2276 6572 7369 6f6e 222c  n.get("version",
-00003a40: 2022 302e 302e 302e 3022 2929 0a0a 2020   "0.0.0.0"))..  
-00003a50: 2020 4c4f 472e 696e 666f 2822 4942 4d20    LOG.info("IBM 
-00003a60: 5365 6375 7269 7479 2053 4f41 5220 7665  Security SOAR ve
-00003a70: 7273 696f 6e3a 2076 2573 222c 2063 6f6e  rsion: v%s", con
-00003a80: 7374 616e 7473 2e43 5552 5245 4e54 5f53  stants.CURRENT_S
-00003a90: 4f41 525f 5345 5256 4552 5f56 4552 5349  OAR_SERVER_VERSI
-00003aa0: 4f4e 290a 0a20 2020 2072 6574 7572 6e20  ON)..    return 
-00003ab0: 636f 6e73 7461 6e74 732e 4355 5252 454e  constants.CURREN
-00003ac0: 545f 534f 4152 5f53 4552 5645 525f 5645  T_SOAR_SERVER_VE
-00003ad0: 5253 494f 4e0a 0a0a 6465 6620 6765 745f  RSION...def get_
-00003ae0: 6c61 7465 7374 5f6f 7267 5f65 7870 6f72  latest_org_expor
-00003af0: 7428 7265 735f 636c 6965 6e74 293a 0a20  t(res_client):. 
-00003b00: 2020 2022 2222 0a20 2020 2047 656e 6572     """.    Gener
-00003b10: 6174 6573 2061 206e 6577 2045 7870 6f72  ates a new Expor
-00003b20: 7420 6f6e 2053 4f41 522e 0a20 2020 2052  t on SOAR..    R
-00003b30: 6574 7572 6e73 2074 6865 2050 4f53 5420  eturns the POST 
-00003b40: 7265 7370 6f6e 7365 0a20 2020 2022 2222  response.    """
-00003b50: 0a20 2020 204c 4f47 2e64 6562 7567 2822  .    LOG.debug("
-00003b60: 4765 6e65 7261 7469 6e67 206e 6577 206f  Generating new o
-00003b70: 7267 616e 697a 6174 696f 6e20 6578 706f  rganization expo
-00003b80: 7274 2229 0a20 2020 206c 6174 6573 745f  rt").    latest_
-00003b90: 6578 706f 7274 5f75 7269 203d 2022 2f63  export_uri = "/c
-00003ba0: 6f6e 6669 6775 7261 7469 6f6e 732f 6578  onfigurations/ex
-00003bb0: 706f 7274 732f 220a 0a20 2020 2063 7573  ports/"..    cus
-00003bc0: 746f 6d69 7a61 7469 6f6e 735f 746f 5f67  tomizations_to_g
-00003bd0: 6574 203d 207b 0a20 2020 2020 2020 2022  et = {.        "
-00003be0: 6c61 796f 7574 7322 3a20 5472 7565 2c0a  layouts": True,.
-00003bf0: 2020 2020 2020 2020 2261 6374 696f 6e73          "actions
-00003c00: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
-00003c10: 2022 7068 6173 6573 5f61 6e64 5f74 6173   "phases_and_tas
-00003c20: 6b73 223a 2054 7275 650a 2020 2020 7d0a  ks": True.    }.
-00003c30: 2020 2020 7365 7276 6572 5f76 6572 7369      server_versi
-00003c40: 6f6e 203d 2067 6574 5f72 6573 696c 6965  on = get_resilie
-00003c50: 6e74 5f73 6572 7665 725f 7665 7273 696f  nt_server_versio
-00003c60: 6e28 7265 735f 636c 6965 6e74 290a 0a20  n(res_client).. 
-00003c70: 2020 2069 6620 7365 7276 6572 5f76 6572     if server_ver
-00003c80: 7369 6f6e 203e 3d20 636f 6e73 7461 6e74  sion >= constant
-00003c90: 732e 4d49 4e5f 534f 4152 5f53 4552 5645  s.MIN_SOAR_SERVE
-00003ca0: 525f 5645 5253 494f 4e5f 504c 4159 424f  R_VERSION_PLAYBO
-00003cb0: 4f4b 533a 0a20 2020 2020 2020 2063 7573  OKS:.        cus
-00003cc0: 746f 6d69 7a61 7469 6f6e 735f 746f 5f67  tomizations_to_g
-00003cd0: 6574 2e75 7064 6174 6528 7b22 706c 6179  et.update({"play
-00003ce0: 626f 6f6b 7322 3a20 5472 7565 7d29 0a0a  books": True})..
-00003cf0: 2020 2020 7265 7475 726e 2072 6573 5f63      return res_c
-00003d00: 6c69 656e 742e 706f 7374 286c 6174 6573  lient.post(lates
-00003d10: 745f 6578 706f 7274 5f75 7269 2c20 6375  t_export_uri, cu
-00003d20: 7374 6f6d 697a 6174 696f 6e73 5f74 6f5f  stomizations_to_
-00003d30: 6765 7429 0a0a 0a64 6566 2061 6464 5f63  get)...def add_c
-00003d40: 6f6e 6669 6775 7261 7469 6f6e 5f69 6d70  onfiguration_imp
-00003d50: 6f72 7428 6e65 775f 6578 706f 7274 5f64  ort(new_export_d
-00003d60: 6174 612c 2072 6573 5f63 6c69 656e 7429  ata, res_client)
-00003d70: 3a0a 2020 2020 2222 220a 2020 2020 4d61  :.    """.    Ma
-00003d80: 6b65 7320 6120 5245 5354 2072 6571 7565  kes a REST reque
-00003d90: 7374 2074 6f20 6164 6420 6120 636f 6e66  st to add a conf
-00003da0: 6967 7572 6174 696f 6e20 696d 706f 7274  iguration import
-00003db0: 2e0a 0a20 2020 2041 6674 6572 2074 6865  ...    After the
-00003dc0: 2072 6571 7565 7374 2069 7320 6d61 6465   request is made
-00003dd0: 2c20 7468 6520 636f 6e66 6967 7572 6174  , the configurat
-00003de0: 696f 6e20 696d 706f 7274 2069 7320 7365  ion import is se
-00003df0: 7420 6174 2061 2070 656e 6469 6e67 2073  t at a pending s
-00003e00: 7461 7465 2061 6e64 206e 6565 6473 2074  tate and needs t
-00003e10: 6f20 6265 2063 6f6e 6669 726d 6564 2e0a  o be confirmed..
-00003e20: 2020 2020 4966 2074 6865 2063 6f6e 6669      If the confi
-00003e30: 6775 7261 7469 6f6e 2073 7461 7465 2069  guration state i
-00003e40: 7320 6e6f 7420 7265 706f 7274 6564 2061  s not reported a
-00003e50: 7320 7065 6e64 696e 672c 2072 6169 7365  s pending, raise
-00003e60: 2061 6e20 5344 4b20 4578 6365 7074 696f   an SDK Exceptio
-00003e70: 6e2e 0a0a 0a20 2020 203a 7061 7261 6d20  n....    :param 
-00003e80: 6e65 775f 6578 706f 7274 5f64 6174 613a  new_export_data:
-00003e90: 2041 2064 6963 7420 7265 7072 6573 656e   A dict represen
-00003ea0: 7469 6e67 2061 2063 6f6e 6669 6775 7261  ting a configura
-00003eb0: 7469 6f6e 2069 6d70 6f72 7420 4454 4f0a  tion import DTO.
-00003ec0: 2020 2020 3a74 7970 6520 7265 7375 6c74      :type result
-00003ed0: 3a20 6469 6374 0a20 2020 203a 7061 7261  : dict.    :para
-00003ee0: 6d20 696d 706f 7274 5f69 643a 2054 6865  m import_id: The
-00003ef0: 2049 4420 6f66 2074 6865 2063 6f6e 6669   ID of the confi
-00003f00: 6775 7261 7469 6f6e 2069 6d70 6f72 7420  guration import 
-00003f10: 746f 2063 6f6e 6669 726d 0a20 2020 203a  to confirm.    :
-00003f20: 7479 7065 2069 6d70 6f72 745f 6964 3a20  type import_id: 
-00003f30: 696e 740a 2020 2020 3a70 6172 616d 2072  int.    :param r
-00003f40: 6573 5f63 6c69 656e 743a 2041 6e20 696e  es_client: An in
-00003f50: 7374 616e 7469 6174 6564 2072 6573 5f63  stantiated res_c
-00003f60: 6c69 656e 7420 666f 7220 6d61 6b69 6e67  lient for making
-00003f70: 2052 4553 5420 6361 6c6c 730a 2020 2020   REST calls.    
-00003f80: 3a74 7970 6520 7265 735f 636c 6965 6e74  :type res_client
-00003f90: 3a20 5369 6d70 6c65 436c 6965 6e74 2829  : SimpleClient()
-00003fa0: 0a20 2020 203a 7261 6973 6573 2053 444b  .    :raises SDK
-00003fb0: 4578 6365 7074 696f 6e3a 2049 6620 7468  Exception: If th
-00003fc0: 6520 636f 6e66 6972 6d61 7469 6f6e 2072  e confirmation r
-00003fd0: 6571 7565 7374 2066 6169 6c73 2072 6169  equest fails rai
-00003fe0: 7365 2061 6e20 5344 4b45 7863 6570 7469  se an SDKExcepti
-00003ff0: 6f6e 0a20 2020 2022 2222 0a20 2020 2074  on.    """.    t
-00004000: 7279 3a0a 2020 2020 2020 2020 7265 7375  ry:.        resu
-00004010: 6c74 203d 2072 6573 5f63 6c69 656e 742e  lt = res_client.
-00004020: 706f 7374 2863 6f6e 7374 616e 7473 2e49  post(constants.I
-00004030: 4d50 4f52 545f 5552 4c2c 206e 6577 5f65  MPORT_URL, new_e
-00004040: 7870 6f72 745f 6461 7461 290a 2020 2020  xport_data).    
-00004050: 6578 6365 7074 2072 6571 7565 7374 732e  except requests.
-00004060: 5265 7175 6573 7445 7863 6570 7469 6f6e  RequestException
-00004070: 2061 7320 7570 6c6f 6164 5f65 7863 6570   as upload_excep
-00004080: 7469 6f6e 3a0a 2020 2020 2020 2020 4c4f  tion:.        LO
-00004090: 472e 6465 6275 6728 6e65 775f 6578 706f  G.debug(new_expo
-000040a0: 7274 5f64 6174 6129 0a20 2020 2020 2020  rt_data).       
-000040b0: 2072 6169 7365 2053 444b 4578 6365 7074   raise SDKExcept
-000040c0: 696f 6e28 7570 6c6f 6164 5f65 7863 6570  ion(upload_excep
-000040d0: 7469 6f6e 290a 2020 2020 656c 7365 3a0a  tion).    else:.
-000040e0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-000040f0: 7369 6e73 7461 6e63 6528 7265 7375 6c74  sinstance(result
-00004100: 2c20 6469 6374 290a 2020 2020 6966 2072  , dict).    if r
-00004110: 6573 756c 742e 6765 7428 2273 7461 7475  esult.get("statu
-00004120: 7322 2c20 2727 2920 3d3d 2022 5045 4e44  s", '') == "PEND
-00004130: 494e 4722 3a0a 2020 2020 2020 2020 636f  ING":.        co
-00004140: 6e66 6972 6d5f 636f 6e66 6967 7572 6174  nfirm_configurat
-00004150: 696f 6e5f 696d 706f 7274 2872 6573 756c  ion_import(resul
-00004160: 742c 2072 6573 756c 742e 6765 7428 2269  t, result.get("i
-00004170: 6422 292c 2072 6573 5f63 6c69 656e 7429  d"), res_client)
-00004180: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00004190: 2020 2072 6169 7365 2053 444b 4578 6365     raise SDKExce
-000041a0: 7074 696f 6e28 0a20 2020 2020 2020 2020  ption(.         
-000041b0: 2020 2022 436f 756c 6420 6e6f 7420 696d     "Could not im
-000041c0: 706f 7274 2062 6563 6175 7365 2074 6865  port because the
-000041d0: 2073 6572 7665 7220 6469 6420 6e6f 7420   server did not 
-000041e0: 7265 7475 726e 2061 6e20 696d 706f 7274  return an import
-000041f0: 2049 4422 290a 0a0a 6465 6620 636f 6e66   ID")...def conf
-00004200: 6972 6d5f 636f 6e66 6967 7572 6174 696f  irm_configuratio
-00004210: 6e5f 696d 706f 7274 2872 6573 756c 742c  n_import(result,
-00004220: 2069 6d70 6f72 745f 6964 2c20 7265 735f   import_id, res_
-00004230: 636c 6965 6e74 293a 0a20 2020 2022 2222  client):.    """
-00004240: 0a20 2020 204d 616b 6573 2061 2052 4553  .    Makes a RES
-00004250: 5420 7265 7175 6573 7420 746f 2063 6f6e  T request to con
-00004260: 6669 726d 2061 2070 656e 6469 6e67 2063  firm a pending c
-00004270: 6f6e 6669 6775 7261 7469 6f6e 2069 6d70  onfiguration imp
-00004280: 6f72 7420 6173 2061 6363 6570 7465 642e  ort as accepted.
-00004290: 0a0a 2020 2020 5461 6b65 7320 3320 7061  ..    Takes 3 pa
-000042a0: 7261 6d73 0a20 2020 2054 6865 2072 6573  rams.    The res
-000042b0: 756c 7420 6f66 2061 2063 6f6e 6669 6775  ult of a configu
-000042c0: 7261 7469 6f6e 2069 6d70 6f72 7420 7265  ration import re
-000042d0: 7175 6573 740a 2020 2020 5468 6520 4944  quest.    The ID
-000042e0: 206f 6620 7468 6520 636f 6e66 6967 7572   of the configur
-000042f0: 6174 696f 6e20 696d 706f 7274 2072 6571  ation import req
-00004300: 7565 7374 0a20 2020 2041 2072 6573 5f63  uest.    A res_c
-00004310: 6c69 656e 7420 746f 2070 6572 666f 726d  lient to perform
-00004320: 2074 6865 2072 6571 7565 7374 0a0a 2020   the request..  
-00004330: 2020 3a70 6172 616d 2072 6573 756c 743a    :param result:
-00004340: 2052 6573 756c 7420 6f66 2074 6865 2063   Result of the c
-00004350: 6f6e 6669 6775 7261 7469 6f6e 2069 6d70  onfiguration imp
-00004360: 6f72 7420 7265 7175 6573 740a 2020 2020  ort request.    
-00004370: 3a74 7970 6520 7265 7375 6c74 3a20 6469  :type result: di
-00004380: 6374 0a20 2020 203a 7061 7261 6d20 696d  ct.    :param im
-00004390: 706f 7274 5f69 643a 2054 6865 2049 4420  port_id: The ID 
-000043a0: 6f66 2074 6865 2063 6f6e 6669 6775 7261  of the configura
-000043b0: 7469 6f6e 2069 6d70 6f72 7420 746f 2063  tion import to c
-000043c0: 6f6e 6669 726d 0a20 2020 203a 7479 7065  onfirm.    :type
-000043d0: 2069 6d70 6f72 745f 6964 3a20 696e 740a   import_id: int.
-000043e0: 2020 2020 3a70 6172 616d 2072 6573 5f63      :param res_c
-000043f0: 6c69 656e 743a 2041 6e20 696e 7374 616e  lient: An instan
-00004400: 7469 6174 6564 2072 6573 5f63 6c69 656e  tiated res_clien
-00004410: 7420 666f 7220 6d61 6b69 6e67 2052 4553  t for making RES
-00004420: 5420 6361 6c6c 730a 2020 2020 3a74 7970  T calls.    :typ
-00004430: 6520 7265 735f 636c 6965 6e74 3a20 5369  e res_client: Si
-00004440: 6d70 6c65 436c 6965 6e74 2829 0a20 2020  mpleClient().   
-00004450: 203a 7261 6973 6573 2053 444b 4578 6365   :raises SDKExce
-00004460: 7074 696f 6e3a 2049 6620 7468 6520 636f  ption: If the co
-00004470: 6e66 6972 6d61 7469 6f6e 2072 6571 7565  nfirmation reque
-00004480: 7374 2066 6169 6c73 2072 6169 7365 2061  st fails raise a
-00004490: 6e20 5344 4b45 7863 6570 7469 6f6e 0a20  n SDKException. 
-000044a0: 2020 2022 2222 0a0a 2020 2020 7265 7375     """..    resu
-000044b0: 6c74 5b22 7374 6174 7573 225d 203d 2022  lt["status"] = "
-000044c0: 4143 4345 5054 4544 2220 2020 2020 2023  ACCEPTED"      #
-000044d0: 2048 6176 6520 746f 2063 6f6e 6669 726d   Have to confirm
-000044e0: 2063 6861 6e67 6573 0a20 2020 2075 7269   changes.    uri
-000044f0: 203d 2022 7b7d 2f7b 7d22 2e66 6f72 6d61   = "{}/{}".forma
-00004500: 7428 636f 6e73 7461 6e74 732e 494d 504f  t(constants.IMPO
-00004510: 5254 5f55 524c 2c20 696d 706f 7274 5f69  RT_URL, import_i
-00004520: 6429 0a20 2020 2074 7279 3a0a 2020 2020  d).    try:.    
-00004530: 2020 2020 7265 735f 636c 6965 6e74 2e70      res_client.p
-00004540: 7574 2875 7269 2c20 7265 7375 6c74 290a  ut(uri, result).
-00004550: 2020 2020 2020 2020 4c4f 472e 696e 666f          LOG.info
-00004560: 2822 496d 706f 7274 6564 2063 6f6e 6669  ("Imported confi
-00004570: 6775 7261 7469 6f6e 2063 6861 6e67 6573  guration changes
-00004580: 2073 7563 6365 7373 6675 6c6c 7920 746f   successfully to
-00004590: 2053 4f41 5222 290a 2020 2020 6578 6365   SOAR").    exce
-000045a0: 7074 2072 6571 7565 7374 732e 5265 7175  pt requests.Requ
-000045b0: 6573 7445 7863 6570 7469 6f6e 2061 7320  estException as 
-000045c0: 696d 706f 7274 5f65 7863 6570 7469 6f6e  import_exception
-000045d0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-000045e0: 5344 4b45 7863 6570 7469 6f6e 2872 6570  SDKException(rep
-000045f0: 7228 696d 706f 7274 5f65 7863 6570 7469  r(import_excepti
-00004600: 6f6e 2929 0a0a 6465 6620 7265 6164 5f6c  on))..def read_l
-00004610: 6f63 616c 5f65 7870 6f72 7466 696c 6528  ocal_exportfile(
-00004620: 7061 7468 5f6c 6f63 616c 5f65 7870 6f72  path_local_expor
-00004630: 7466 696c 6529 3a0a 2020 2020 2222 220a  tfile):.    """.
-00004640: 2020 2020 5265 6164 2065 7870 6f72 7420      Read export 
-00004650: 6672 6f6d 2067 6976 656e 2070 6174 680a  from given path.
-00004660: 2020 2020 5265 7475 726e 2072 6573 2065      Return res e
-00004670: 7870 6f72 7420 6173 2064 6963 740a 2020  xport as dict.  
-00004680: 2020 2222 220a 2020 2020 2320 4765 7420    """.    # Get 
-00004690: 6162 736f 6c75 7465 2070 6174 680a 2020  absolute path.  
-000046a0: 2020 7061 7468 5f6c 6f63 616c 5f65 7870    path_local_exp
-000046b0: 6f72 7466 696c 6520 3d20 6f73 2e70 6174  ortfile = os.pat
-000046c0: 682e 6162 7370 6174 6828 7061 7468 5f6c  h.abspath(path_l
-000046d0: 6f63 616c 5f65 7870 6f72 7466 696c 6529  ocal_exportfile)
-000046e0: 0a0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
-000046f0: 2077 6520 6361 6e20 7265 6164 2069 740a   we can read it.
-00004700: 2020 2020 7661 6c69 6461 7465 5f66 696c      validate_fil
-00004710: 655f 7061 7468 7328 6f73 2e52 5f4f 4b2c  e_paths(os.R_OK,
-00004720: 2070 6174 685f 6c6f 6361 6c5f 6578 706f   path_local_expo
-00004730: 7274 6669 6c65 290a 0a20 2020 2023 2052  rtfile)..    # R
-00004740: 6561 6420 7468 6520 6578 706f 7274 2066  ead the export f
-00004750: 696c 6520 636f 6e74 656e 742e 0a20 2020  ile content..   
-00004760: 2069 6620 6973 5f7a 6970 6669 6c65 2870   if is_zipfile(p
-00004770: 6174 685f 6c6f 6361 6c5f 6578 706f 7274  ath_local_export
-00004780: 6669 6c65 293a 0a20 2020 2020 2020 2023  file):.        #
-00004790: 2046 696c 6520 6973 2061 207a 6970 2066   File is a zip f
-000047a0: 696c 6520 6765 7420 756e 7a69 7070 6564  ile get unzipped
-000047b0: 2063 6f6e 7465 6e74 2e0a 2020 2020 2020   content..      
-000047c0: 2020 6578 706f 7274 5f63 6f6e 7465 6e74    export_content
-000047d0: 203d 2072 6561 645f 7a69 705f 6669 6c65   = read_zip_file
-000047e0: 2870 6174 685f 6c6f 6361 6c5f 6578 706f  (path_local_expo
-000047f0: 7274 6669 6c65 2c20 636f 6e73 7461 6e74  rtfile, constant
-00004800: 732e 5245 535f 4558 504f 5254 5f53 5546  s.RES_EXPORT_SUF
-00004810: 4649 5829 0a20 2020 2065 6c73 653a 0a20  FIX).    else:. 
-00004820: 2020 2020 2020 2023 2046 696c 6520 6973         # File is
-00004830: 2061 2061 7373 756d 6564 2074 6f20 6265   a assumed to be
-00004840: 2061 2074 6578 7420 6669 6c65 2072 6561   a text file rea
-00004850: 6420 7468 6520 6578 706f 7274 2066 696c  d the export fil
-00004860: 6520 636f 6e74 656e 742e 0a20 2020 2020  e content..     
-00004870: 2020 2065 7870 6f72 745f 636f 6e74 656e     export_conten
-00004880: 7420 3d20 2727 2e6a 6f69 6e28 7265 6164  t = ''.join(read
-00004890: 5f66 696c 6528 7061 7468 5f6c 6f63 616c  _file(path_local
-000048a0: 5f65 7870 6f72 7466 696c 6529 290a 0a20  _exportfile)).. 
-000048b0: 2020 2069 6620 6e6f 7420 6578 706f 7274     if not export
-000048c0: 5f63 6f6e 7465 6e74 3a0a 2020 2020 2020  _content:.      
-000048d0: 2020 7261 6973 6520 5344 4b45 7863 6570    raise SDKExcep
-000048e0: 7469 6f6e 2822 4661 696c 6564 2074 6f20  tion("Failed to 
-000048f0: 7265 6164 207b 307d 222e 666f 726d 6174  read {0}".format
-00004900: 2870 6174 685f 6c6f 6361 6c5f 6578 706f  (path_local_expo
-00004910: 7274 6669 6c65 2929 0a0a 2020 2020 7265  rtfile))..    re
-00004920: 7475 726e 206a 736f 6e2e 6c6f 6164 7328  turn json.loads(
-00004930: 6578 706f 7274 5f63 6f6e 7465 6e74 290a  export_content).
-00004940: 0a0a 6465 6620 6765 745f 6f62 6a65 6374  ..def get_object
-00004950: 5f61 7069 5f6e 616d 6573 2861 7069 5f6e  _api_names(api_n
-00004960: 616d 652c 206c 6973 745f 6f62 6a73 293a  ame, list_objs):
-00004970: 0a20 2020 2022 2222 0a20 2020 2052 6574  .    """.    Ret
-00004980: 7572 6e20 6120 6c69 7374 206f 6620 6f62  urn a list of ob
-00004990: 6a65 6374 2061 7069 5f6e 616d 6573 2066  ject api_names f
-000049a0: 726f 6d20 6c69 7374 5f6f 626a 730a 2020  rom list_objs.  
-000049b0: 2020 2222 220a 2020 2020 6966 206c 6973    """.    if lis
-000049c0: 745f 6f62 6a73 3a0a 2020 2020 2020 2020  t_objs:.        
-000049d0: 7265 7475 726e 205b 6f2e 6765 7428 6170  return [o.get(ap
-000049e0: 695f 6e61 6d65 2920 666f 7220 6f20 696e  i_name) for o in
-000049f0: 206c 6973 745f 6f62 6a73 5d0a 2020 2020   list_objs].    
-00004a00: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
-00004a10: 7475 726e 205b 5d0a 0a0a 6465 6620 6765  turn []...def ge
-00004a20: 745f 7363 7269 7074 5f69 6e66 6f28 6561  t_script_info(ea
-00004a30: 6368 5f73 6372 6970 745f 696e 5f70 6c61  ch_script_in_pla
-00004a40: 7962 6f6f 6b2c 2073 6372 6970 7473 5f69  ybook, scripts_i
-00004a50: 6e5f 6c6f 6361 7469 6f6e 2c20 7363 7269  n_location, scri
-00004a60: 7074 5f74 7970 6529 3a0a 2020 2020 2727  pt_type):.    ''
-00004a70: 270a 2020 2020 4578 7472 6163 7473 2073  '.    Extracts s
-00004a80: 6372 6970 7420 7265 6c61 7465 6420 696e  cript related in
-00004a90: 666f 726d 6174 696f 6e20 666f 7220 706c  formation for pl
-00004aa0: 6179 626f 6f6b 732e 2053 6372 6970 7473  aybooks. Scripts
-00004ab0: 2063 616e 2062 6520 6f66 2032 2074 7970   can be of 2 typ
-00004ac0: 6573 3a20 6c6f 6361 6c20 6f72 2067 6c6f  es: local or glo
-00004ad0: 6261 6c2e 0a20 2020 204c 6f63 616c 2073  bal..    Local s
-00004ae0: 6372 6970 7473 206c 6976 6520 7769 7468  cripts live with
-00004af0: 696e 2074 6865 2070 6c61 7962 6f6f 6b20  in the playbook 
-00004b00: 6974 7365 6c66 2c20 7768 696c 6520 676c  itself, while gl
-00004b10: 6f62 616c 2073 6372 6970 7473 2061 7265  obal scripts are
-00004b20: 2073 746f 7265 6420 696e 2074 6865 2067   stored in the g
-00004b30: 6c6f 6261 6c5f 6578 706f 7274 2064 6963  lobal_export dic
-00004b40: 742e 0a20 2020 200a 2020 2020 4e6f 7465  t..    .    Note
-00004b50: 3a20 5468 6520 7363 7269 7074 7320 6172  : The scripts ar
-00004b60: 6520 7061 7373 6564 2062 7920 7265 6665  e passed by refe
-00004b70: 7265 6e63 652e 2054 6865 7920 6e65 6564  rence. They need
-00004b80: 206e 6f74 2062 6520 7265 7475 726e 6564   not be returned
-00004b90: 2e20 5468 6579 2061 7265 2064 6972 6563  . They are direc
-00004ba0: 746c 7920 7570 6461 7465 642e 0a20 2020  tly updated..   
-00004bb0: 203a 7061 7261 6d20 6561 6368 5f73 6372   :param each_scr
-00004bc0: 6970 745f 696e 5f70 6c61 7962 6f6f 6b3a  ipt_in_playbook:
-00004bd0: 2049 6e64 6976 6964 7561 6c20 7363 7269   Individual scri
-00004be0: 7074 7320 666f 756e 6420 696e 2074 6865  pts found in the
-00004bf0: 2070 6c61 7962 6f6f 6b0a 2020 2020 3a74   playbook.    :t
-00004c00: 7970 6520 6561 6368 5f73 6372 6970 745f  ype each_script_
-00004c10: 696e 5f70 6c61 7962 6f6f 6b3a 2064 6963  in_playbook: dic
-00004c20: 740a 2020 2020 3a70 6172 616d 2073 6372  t.    :param scr
-00004c30: 6970 7473 5f69 6e5f 6c6f 6361 7469 6f6e  ipts_in_location
-00004c40: 3a20 416c 6c20 7363 7269 7074 7320 696e  : All scripts in
-00004c50: 2074 6865 206c 6f63 6174 696f 6e20 2867   the location (g
-00004c60: 6c6f 6261 6c20 6f72 206c 6f63 616c 292e  lobal or local).
-00004c70: 2047 6c6f 6261 6c20 7363 7269 7074 7320   Global scripts 
-00004c80: 6172 6520 7075 6c6c 6564 2064 6972 6563  are pulled direc
-00004c90: 746c 7920 6672 6f6d 2074 6865 2067 6c6f  tly from the glo
-00004ca0: 6261 6c5f 6578 706f 7274 2064 6963 742e  bal_export dict.
-00004cb0: 204c 6f63 616c 2073 6372 6970 7473 2061   Local scripts a
-00004cc0: 7265 2070 756c 6c65 6420 6672 6f6d 2074  re pulled from t
-00004cd0: 6865 2070 6c61 7962 6f6f 6b0a 2020 2020  he playbook.    
-00004ce0: 3a74 7970 6520 7363 7269 7074 735f 696e  :type scripts_in
-00004cf0: 5f6c 6f63 6174 696f 6e3a 206c 6973 740a  _location: list.
-00004d00: 2020 2020 3a70 6172 616d 2073 6372 6970      :param scrip
-00004d10: 745f 7479 7065 3a20 5468 6520 7479 7065  t_type: The type
-00004d20: 206f 6620 7363 7269 7074 2028 676c 6f62   of script (glob
-00004d30: 616c 206f 7220 6c6f 6361 6c29 0a20 2020  al or local).   
-00004d40: 203a 7479 7065 2073 6372 6970 745f 7479   :type script_ty
-00004d50: 7065 3a20 7374 720a 2020 2020 2727 270a  pe: str.    '''.
-00004d60: 2020 2020 666f 756e 645f 7363 7269 7074      found_script
-00004d70: 203d 2046 616c 7365 0a20 2020 2066 6f72   = False.    for
-00004d80: 2073 6320 696e 2073 6372 6970 7473 5f69   sc in scripts_i
-00004d90: 6e5f 6c6f 6361 7469 6f6e 3a0a 2020 2020  n_location:.    
-00004da0: 2020 2020 6966 2065 6163 685f 7363 7269      if each_scri
-00004db0: 7074 5f69 6e5f 706c 6179 626f 6f6b 2e67  pt_in_playbook.g
-00004dc0: 6574 2822 7575 6964 222c 2022 7575 6964  et("uuid", "uuid
-00004dd0: 5f6e 6f74 5f66 6f75 6e64 5f70 6222 2920  _not_found_pb") 
-00004de0: 3d3d 2073 632e 6765 7428 2275 7569 6422  == sc.get("uuid"
-00004df0: 2c20 2275 7569 645f 6e6f 745f 666f 756e  , "uuid_not_foun
-00004e00: 645f 7363 2229 3a0a 2020 2020 2020 2020  d_sc"):.        
-00004e10: 2020 2020 6561 6368 5f73 6372 6970 745f      each_script_
-00004e20: 696e 5f70 6c61 7962 6f6f 6b5b 226e 616d  in_playbook["nam
-00004e30: 6522 5d20 3d20 7363 2e67 6574 2822 6e61  e"] = sc.get("na
-00004e40: 6d65 2229 0a20 2020 2020 2020 2020 2020  me").           
-00004e50: 2065 6163 685f 7363 7269 7074 5f69 6e5f   each_script_in_
-00004e60: 706c 6179 626f 6f6b 5b22 7363 7269 7074  playbook["script
-00004e70: 5f74 7970 6522 5d20 3d20 7363 7269 7074  _type"] = script
-00004e80: 5f74 7970 650a 2020 2020 2020 2020 2020  _type.          
-00004e90: 2020 6561 6368 5f73 6372 6970 745f 696e    each_script_in
-00004ea0: 5f70 6c61 7962 6f6f 6b5b 2264 6573 6372  _playbook["descr
-00004eb0: 6970 7469 6f6e 225d 203d 2073 632e 6765  iption"] = sc.ge
-00004ec0: 7428 2264 6573 6372 6970 7469 6f6e 2229  t("description")
-00004ed0: 0a20 2020 2020 2020 2020 2020 2065 6163  .            eac
-00004ee0: 685f 7363 7269 7074 5f69 6e5f 706c 6179  h_script_in_play
-00004ef0: 626f 6f6b 5b22 6f62 6a65 6374 5f74 7970  book["object_typ
-00004f00: 6522 5d20 3d20 7363 2e67 6574 2822 6f62  e"] = sc.get("ob
-00004f10: 6a65 6374 5f74 7970 6522 290a 2020 2020  ject_type").    
-00004f20: 2020 2020 2020 2020 6561 6368 5f73 6372          each_scr
-00004f30: 6970 745f 696e 5f70 6c61 7962 6f6f 6b5b  ipt_in_playbook[
-00004f40: 2273 6372 6970 745f 7465 7874 225d 203d  "script_text"] =
-00004f50: 2073 632e 6765 7428 2273 6372 6970 745f   sc.get("script_
-00004f60: 7465 7874 222c 2022 2229 0a20 2020 2020  text", "").     
-00004f70: 2020 2020 2020 2066 6f75 6e64 5f73 6372         found_scr
-00004f80: 6970 7420 3d20 5472 7565 0a20 2020 2020  ipt = True.     
-00004f90: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-00004fa0: 2072 6574 7572 6e20 666f 756e 645f 7363   return found_sc
-00004fb0: 7269 7074 0a0a 0a64 6566 2067 6574 5f6f  ript...def get_o
-00004fc0: 626a 5f66 726f 6d5f 6c69 7374 2869 6465  bj_from_list(ide
-00004fd0: 6e74 6966 6572 2c20 6f62 6a5f 6c69 7374  ntifer, obj_list
-00004fe0: 2c20 636f 6e64 6974 696f 6e3d 6c61 6d62  , condition=lamb
-00004ff0: 6461 206f 3a20 5472 7565 293a 0a20 2020  da o: True):.   
-00005000: 2022 2222 0a20 2020 2052 6574 7572 6e20   """.    Return 
-00005010: 6120 6469 6374 2074 6865 206e 616d 6520  a dict the name 
-00005020: 6f66 2074 6865 206f 626a 6563 7420 6173  of the object as
-00005030: 2069 7473 204b 6579 0a20 2020 2065 2e67   its Key.    e.g
-00005040: 2e20 7b0a 2020 2020 2020 2020 2266 6e5f  . {.        "fn_
-00005050: 6d6f 636b 5f66 756e 6374 696f 6e5f 3122  mock_function_1"
-00005060: 3a20 7b2e 2e2e 7d2c 0a20 2020 2020 2020  : {...},.       
-00005070: 2022 666e 5f6d 6f63 6b5f 6675 6e63 7469   "fn_mock_functi
-00005080: 6f6e 5f32 223a 207b 2e2e 2e7d 0a20 2020  on_2": {...}.   
-00005090: 207d 0a20 2020 203a 7061 7261 6d20 6964   }.    :param id
-000050a0: 656e 7469 6665 723a 2054 6865 2061 7474  entifer: The att
-000050b0: 7269 6275 7465 206f 6620 7468 6520 6f62  ribute of the ob
-000050c0: 6a65 6374 2077 6520 7573 6520 746f 2069  ject we use to i
-000050d0: 6465 6e74 6966 7920 6974 2065 2e67 2e20  dentify it e.g. 
-000050e0: 2270 726f 6772 616d 6d61 7469 635f 6e61  "programmatic_na
-000050f0: 6d65 220a 2020 2020 3a74 7970 6520 6964  me".    :type id
-00005100: 656e 7469 6665 723a 2073 7472 0a20 2020  entifer: str.   
-00005110: 203a 7061 7261 6d20 6f62 6a5f 6c69 7374   :param obj_list
-00005120: 3a20 4c69 7374 206f 6620 5265 7369 6c69  : List of Resili
-00005130: 656e 7420 4f62 6a65 6374 730a 2020 2020  ent Objects.    
-00005140: 3a74 7970 6520 6f62 6a5f 6c69 7374 3a20  :type obj_list: 
-00005150: 4c69 7374 0a20 2020 203a 7061 7261 6d20  List.    :param 
-00005160: 636f 6e64 6974 696f 6e3a 2041 206c 616d  condition: A lam
-00005170: 6264 6120 6675 6e63 7469 6f6e 2074 6f20  bda function to 
-00005180: 6576 616c 7561 7465 2065 6163 6820 6f62  evaluate each ob
-00005190: 6a65 6374 0a20 2020 203a 7479 7065 2063  ject.    :type c
-000051a0: 6f6e 6469 7469 6f6e 3a20 6675 6e63 7469  ondition: functi
-000051b0: 6f6e 0a20 2020 203a 7265 7475 726e 3a20  on.    :return: 
-000051c0: 4469 6374 696f 6e61 7279 206f 6620 6561  Dictionary of ea
-000051d0: 6368 2066 6f75 6e64 206f 626a 6563 7420  ch found object 
-000051e0: 6c69 6b65 2074 6865 2061 626f 7665 2065  like the above e
-000051f0: 7861 6d70 6c65 0a20 2020 203a 7274 7970  xample.    :rtyp
-00005200: 653a 2044 6963 740a 2020 2020 2222 220a  e: Dict.    """.
-00005210: 2020 2020 6966 206f 626a 5f6c 6973 743a      if obj_list:
-00005220: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00005230: 6469 6374 2828 6f5b 6964 656e 7469 6665  dict((o[identife
-00005240: 725d 2e73 7472 6970 2829 2c20 6f29 2066  r].strip(), o) f
-00005250: 6f72 206f 2069 6e20 6f62 6a5f 6c69 7374  or o in obj_list
-00005260: 2069 6620 636f 6e64 6974 696f 6e28 6f29   if condition(o)
-00005270: 290a 2020 2020 7265 7475 726e 207b 7d0a  ).    return {}.
-00005280: 0a0a 6465 6620 6765 745f 7265 735f 6f62  ..def get_res_ob
-00005290: 6a28 6f62 6a5f 6e61 6d65 2c20 6f62 6a5f  j(obj_name, obj_
-000052a0: 6964 656e 7469 6665 722c 206f 626a 5f64  identifer, obj_d
-000052b0: 6973 706c 6179 5f6e 616d 652c 2077 616e  isplay_name, wan
-000052c0: 7465 645f 6c69 7374 2c20 6578 706f 7274  ted_list, export
-000052d0: 2c20 636f 6e64 6974 696f 6e3d 6c61 6d62  , condition=lamb
-000052e0: 6461 206f 3a20 5472 7565 2c20 696e 636c  da o: True, incl
-000052f0: 7564 655f 6170 695f 6e61 6d65 3d54 7275  ude_api_name=Tru
-00005300: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-00005310: 5265 7475 726e 2061 204c 6973 7420 6f66  Return a List of
-00005320: 2052 6573 696c 6965 6e74 204f 626a 6563   Resilient Objec
-00005330: 7473 2074 6861 7420 6172 6520 696e 2074  ts that are in t
-00005340: 6865 2027 7761 6e74 6564 5f6c 6973 7427  he 'wanted_list'
-00005350: 2061 6e64 206d 6565 7420 7468 6520 2763   and meet the 'c
-00005360: 6f6e 6469 7469 6f6e 270a 0a20 2020 203a  ondition'..    :
-00005370: 7061 7261 6d20 6f62 6a5f 6e61 6d65 3a20  param obj_name: 
-00005380: 4e61 6d65 206f 6620 7468 6520 4f62 6a65  Name of the Obje
-00005390: 6374 206c 6973 7420 696e 2074 6865 2045  ct list in the E
-000053a0: 7870 6f72 740a 2020 2020 3a74 7970 6520  xport.    :type 
-000053b0: 6f62 6a5f 6e61 6d65 3a20 7374 720a 2020  obj_name: str.  
-000053c0: 2020 3a70 6172 616d 206f 626a 5f69 6465    :param obj_ide
-000053d0: 6e74 6966 6572 3a20 5468 6520 6174 7472  ntifer: The attr
-000053e0: 6962 7574 6520 6f66 2074 6865 206f 626a  ibute of the obj
-000053f0: 6563 7420 7765 2075 7365 2074 6f20 6964  ect we use to id
-00005400: 656e 7469 6679 2069 7420 652e 672e 2022  entify it e.g. "
-00005410: 7072 6f67 7261 6d6d 6174 6963 5f6e 616d  programmatic_nam
-00005420: 6522 0a20 2020 203a 7479 7065 206f 626a  e".    :type obj
-00005430: 5f69 6465 6e74 6966 6572 3a20 7374 720a  _identifer: str.
-00005440: 2020 2020 3a70 6172 616d 206f 626a 5f64      :param obj_d
-00005450: 6973 706c 6179 5f6e 616d 653a 2054 6865  isplay_name: The
-00005460: 2044 6973 706c 6179 204e 616d 6520 7765   Display Name we
-00005470: 2077 616e 7420 746f 2075 7365 2066 6f72   want to use for
-00005480: 2074 6869 7320 6f62 6a65 6374 2069 6e20   this object in 
-00005490: 6f75 7220 4c6f 6773 0a20 2020 203a 7479  our Logs.    :ty
-000054a0: 7065 206f 626a 5f64 6973 706c 6179 5f6e  pe obj_display_n
-000054b0: 616d 653a 2073 7472 0a20 2020 203a 7061  ame: str.    :pa
-000054c0: 7261 6d20 7761 6e74 6564 5f6c 6973 743a  ram wanted_list:
-000054d0: 204c 6973 7420 6f66 2069 6465 6e74 6966   List of identif
-000054e0: 6572 7320 666f 7220 6f62 6a65 6374 7320  ers for objects 
-000054f0: 7765 2077 616e 7420 746f 2072 6574 7572  we want to retur
-00005500: 6e0a 2020 2020 3a74 7970 6520 7761 6e74  n.    :type want
-00005510: 6564 5f6c 6973 743a 204c 6973 7420 6f66  ed_list: List of
-00005520: 2073 7472 0a20 2020 203a 7061 7261 6d20   str.    :param 
-00005530: 6578 706f 7274 3a20 5468 6520 7265 7375  export: The resu
-00005540: 6c74 206f 6620 6361 6c6c 696e 6720 6765  lt of calling ge
-00005550: 745f 6c61 7465 7374 5f6f 7267 5f65 7870  t_latest_org_exp
-00005560: 6f72 7428 290a 2020 2020 3a74 7970 6520  ort().    :type 
-00005570: 6578 706f 7274 3a20 4469 6374 0a20 2020  export: Dict.   
-00005580: 203a 7061 7261 6d20 636f 6e64 6974 696f   :param conditio
-00005590: 6e3a 2041 206c 616d 6264 6120 6675 6e63  n: A lambda func
-000055a0: 7469 6f6e 2074 6f20 6576 616c 7561 7465  tion to evaluate
-000055b0: 2065 6163 6820 6f62 6a65 6374 0a20 2020   each object.   
-000055c0: 203a 7479 7065 2063 6f6e 6469 7469 6f6e   :type condition
-000055d0: 3a20 6675 6e63 7469 6f6e 0a20 2020 203a  : function.    :
-000055e0: 7061 7261 6d20 696e 636c 7564 655f 6170  param include_ap
-000055f0: 695f 6e61 6d65 3a20 5768 6574 6865 7220  i_name: Whether 
-00005600: 6f72 206e 6f74 2074 6f20 7265 7475 726e  or not to return
-00005610: 2074 6865 206f 626a 6563 7473 2041 5049   the objects API
-00005620: 206e 616d 6520 6173 2061 2066 6965 6c64   name as a field
-00005630: 2e0a 2020 2020 3a74 7970 6520 696e 636c  ..    :type incl
-00005640: 7564 655f 6170 695f 6e61 6d65 3a20 626f  ude_api_name: bo
-00005650: 6f6c 0a20 2020 203a 7265 7475 726e 3a20  ol.    :return: 
-00005660: 4c69 7374 206f 6620 5265 7369 6c69 656e  List of Resilien
-00005670: 7420 4f62 6a65 6374 730a 2020 2020 3a72  t Objects.    :r
-00005680: 7479 7065 3a20 4c69 7374 0a20 2020 2022  type: List.    "
-00005690: 2222 0a20 2020 2072 6574 7572 6e5f 6c69  "".    return_li
-000056a0: 7374 203d 205b 5d0a 0a20 2020 2023 2054  st = []..    # T
-000056b0: 6869 7320 6c6f 6f70 7320 7761 6e74 6564  his loops wanted
-000056c0: 5f6c 6973 740a 2020 2020 2320 4966 2061  _list.    # If a
-000056d0: 6e20 656e 7472 7920 6973 2064 6963 7420  n entry is dict 
-000056e0: 666f 726d 6174 2c20 6974 2077 696c 6c20  format, it will 
-000056f0: 6861 7665 2076 616c 7565 2061 6e64 2069  have value and i
-00005700: 6465 6e74 6966 6965 7220 6174 7472 6962  dentifier attrib
-00005710: 7574 6573 0a20 2020 2023 2057 6520 7573  utes.    # We us
-00005720: 6520 7468 6f73 6520 746f 2067 6574 2074  e those to get t
-00005730: 6865 2027 7072 6f67 7261 6d6d 6174 6963  he 'programmatic
-00005740: 5f6e 616d 6527 206f 7220 2761 7069 5f6e  _name' or 'api_n
-00005750: 616d 6527 0a20 2020 2023 2045 7861 6d70  ame'.    # Examp
-00005760: 6c65 3a20 466f 7220 6d65 7373 6167 655f  le: For message_
-00005770: 6465 7374 696e 6174 696f 6e73 2072 6566  destinations ref
-00005780: 6572 656e 6365 6420 696e 2061 6374 696f  erenced in actio
-00005790: 6e73 2c20 7468 6579 2061 7265 2072 6566  ns, they are ref
-000057a0: 6572 656e 6365 6420 6279 2064 6973 706c  erenced by displ
-000057b0: 6179 206e 616d 650a 2020 2020 2320 5468  ay name.    # Th
-000057c0: 6973 2061 6c6c 6f77 7320 7573 2074 6f20  is allows us to 
-000057d0: 6765 7420 7468 6569 7220 2770 726f 6772  get their 'progr
-000057e0: 616d 6d61 7469 635f 6e61 6d65 270a 2020  ammatic_name'.  
-000057f0: 2020 666f 7220 696e 6465 782c 206f 626a    for index, obj
-00005800: 2069 6e20 656e 756d 6572 6174 6528 7761   in enumerate(wa
-00005810: 6e74 6564 5f6c 6973 7429 3a0a 2020 2020  nted_list):.    
-00005820: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00005830: 6528 6f62 6a2c 2064 6963 7429 3a0a 2020  e(obj, dict):.  
-00005840: 2020 2020 2020 2020 2020 7465 6d70 5f6f            temp_o
-00005850: 626a 5f69 6465 6e74 6966 6965 7220 3d20  bj_identifier = 
-00005860: 6f62 6a2e 6765 7428 2269 6465 6e74 6966  obj.get("identif
-00005870: 6965 7222 2c20 2222 290a 2020 2020 2020  ier", "").      
-00005880: 2020 2020 2020 6f62 6a5f 7661 6c75 6520        obj_value 
-00005890: 3d20 6f62 6a2e 6765 7428 2276 616c 7565  = obj.get("value
-000058a0: 222c 2022 2229 0a20 2020 2020 2020 2020  ", "").         
-000058b0: 2020 2066 756c 6c5f 6f62 6a20 3d20 6765     full_obj = ge
-000058c0: 745f 6f62 6a5f 6672 6f6d 5f6c 6973 7428  t_obj_from_list(
-000058d0: 7465 6d70 5f6f 626a 5f69 6465 6e74 6966  temp_obj_identif
-000058e0: 6965 722c 0a20 2020 2020 2020 2020 2020  ier,.           
-000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005900: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00005910: 706f 7274 2e67 6574 286f 626a 5f6e 616d  port.get(obj_nam
-00005920: 652c 2022 2229 2c0a 2020 2020 2020 2020  e, ""),.        
-00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005950: 206c 616d 6264 6120 7761 6e74 6564 5f6f   lambda wanted_o
-00005960: 626a 2c20 693d 7465 6d70 5f6f 626a 5f69  bj, i=temp_obj_i
-00005970: 6465 6e74 6966 6965 722c 2076 3d6f 626a  dentifier, v=obj
-00005980: 5f76 616c 7565 3a20 5472 7565 2069 6620  _value: True if 
-00005990: 7761 6e74 6564 5f6f 626a 2e67 6574 2869  wanted_obj.get(i
-000059a0: 2920 3d3d 2076 2065 6c73 6520 4661 6c73  ) == v else Fals
-000059b0: 6529 0a0a 2020 2020 2020 2020 2020 2020  e)..            
-000059c0: 7761 6e74 6564 5f6c 6973 745b 696e 6465  wanted_list[inde
-000059d0: 785d 203d 2066 756c 6c5f 6f62 6a2e 6765  x] = full_obj.ge
-000059e0: 7428 6f62 6a5f 7661 6c75 6529 2e67 6574  t(obj_value).get
-000059f0: 286f 626a 5f69 6465 6e74 6966 6572 290a  (obj_identifer).
-00005a00: 0a20 2020 2069 6620 7761 6e74 6564 5f6c  .    if wanted_l
-00005a10: 6973 743a 0a20 2020 2020 2020 2065 785f  ist:.        ex_
-00005a20: 6f62 6a20 3d20 6765 745f 6f62 6a5f 6672  obj = get_obj_fr
-00005a30: 6f6d 5f6c 6973 7428 6f62 6a5f 6964 656e  om_list(obj_iden
-00005a40: 7469 6665 722c 2065 7870 6f72 742e 6765  tifer, export.ge
-00005a50: 7428 6f62 6a5f 6e61 6d65 2c20 2222 292c  t(obj_name, ""),
-00005a60: 2063 6f6e 6469 7469 6f6e 290a 0a20 2020   condition)..   
-00005a70: 2020 2020 2066 6f72 206f 2069 6e20 7365       for o in se
-00005a80: 7428 7761 6e74 6564 5f6c 6973 7429 3a0a  t(wanted_list):.
-00005a90: 2020 2020 2020 2020 2020 2020 7374 7269              stri
-00005aa0: 7070 6564 5f6f 203d 206f 2e73 7472 6970  pped_o = o.strip
-00005ab0: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
-00005ac0: 6620 7374 7269 7070 6564 5f6f 206e 6f74  f stripped_o not
-00005ad0: 2069 6e20 6578 5f6f 626a 3a0a 2020 2020   in ex_obj:.    
-00005ae0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00005af0: 6520 5344 4b45 7863 6570 7469 6f6e 2875  e SDKException(u
-00005b00: 227b 307d 3a20 277b 317d 2720 6e6f 7420  "{0}: '{1}' not 
-00005b10: 666f 756e 6420 696e 2074 6869 7320 6578  found in this ex
-00005b20: 706f 7274 2e5c 6e7b 307d 7320 4176 6169  port.\n{0}s Avai
-00005b30: 6c61 626c 653a 5c6e 5c74 7b32 7d22 2e66  lable:\n\t{2}".f
-00005b40: 6f72 6d61 7428 6f62 6a5f 6469 7370 6c61  ormat(obj_displa
-00005b50: 795f 6e61 6d65 2c20 7374 7269 7070 6564  y_name, stripped
-00005b60: 5f6f 2c20 225c 6e5c 7422 2e6a 6f69 6e28  _o, "\n\t".join(
-00005b70: 6578 5f6f 626a 2e6b 6579 7328 2929 2929  ex_obj.keys())))
-00005b80: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00005b90: 4164 6420 785f 6170 695f 6e61 6d65 2074  Add x_api_name t
-00005ba0: 6f20 6561 6368 206f 626a 6563 742c 2073  o each object, s
-00005bb0: 6f20 7765 2063 616e 2065 6173 696c 7920  o we can easily 
-00005bc0: 7265 6665 7265 6e63 652e 2054 6869 7320  reference. This 
-00005bd0: 6176 6f69 6473 206e 6565 6469 6e67 2074  avoids needing t
-00005be0: 6f20 6b6e 6f77 2069 660a 2020 2020 2020  o know if.      
-00005bf0: 2020 2020 2020 2320 6f62 6a20 6174 7472        # obj attr
-00005c00: 6962 7574 6520 6973 2027 6e61 6d65 2720  ibute is 'name' 
-00005c10: 6f72 2027 7072 6f67 7261 6d6d 6174 6963  or 'programmatic
-00005c20: 5f6e 616d 6527 2065 7463 2e0a 2020 2020  _name' etc..    
-00005c30: 2020 2020 2020 2020 6f62 6a20 3d20 6578          obj = ex
-00005c40: 5f6f 626a 2e67 6574 2873 7472 6970 7065  _obj.get(strippe
-00005c50: 645f 6f29 0a20 2020 2020 2020 2020 2020  d_o).           
-00005c60: 2069 6620 696e 636c 7564 655f 6170 695f   if include_api_
-00005c70: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
-00005c80: 2020 2020 2020 6f62 6a5b 2278 5f61 7069        obj["x_api
-00005c90: 5f6e 616d 6522 5d20 3d20 6f62 6a5b 6f62  _name"] = obj[ob
-00005ca0: 6a5f 6964 656e 7469 6665 725d 0a20 2020  j_identifer].   
-00005cb0: 2020 2020 2020 2020 2072 6574 7572 6e5f           return_
-00005cc0: 6c69 7374 2e61 7070 656e 6428 6f62 6a29  list.append(obj)
-00005cd0: 0a0a 2020 2020 7265 7475 726e 2072 6574  ..    return ret
-00005ce0: 7572 6e5f 6c69 7374 0a0a 0a64 6566 2067  urn_list...def g
-00005cf0: 6574 5f66 726f 6d5f 6578 706f 7274 2865  et_from_export(e
-00005d00: 7870 6f72 742c 0a20 2020 2020 2020 2020  xport,.         
-00005d10: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00005d20: 6765 5f64 6573 7469 6e61 7469 6f6e 733d  ge_destinations=
-00005d30: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
-00005d40: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
-00005d50: 733d 5b5d 2c0a 2020 2020 2020 2020 2020  s=[],.          
-00005d60: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-00005d70: 6f77 733d 5b5d 2c0a 2020 2020 2020 2020  ows=[],.        
-00005d80: 2020 2020 2020 2020 2020 2020 7275 6c65              rule
-00005d90: 733d 5b5d 2c0a 2020 2020 2020 2020 2020  s=[],.          
-00005da0: 2020 2020 2020 2020 2020 6669 656c 6473            fields
-00005db0: 3d5b 5d2c 0a20 2020 2020 2020 2020 2020  =[],.           
-00005dc0: 2020 2020 2020 2020 2061 7274 6966 6163           artifac
-00005dd0: 745f 7479 7065 733d 5b5d 2c0a 2020 2020  t_types=[],.    
+000024f0: 2020 656c 6966 206e 616d 6520 6973 204e    elif name is N
+00002500: 6f6e 653a 0a20 2020 2020 2020 2072 6574  one:.        ret
+00002510: 7572 6e20 4661 6c73 650a 2020 2020 7265  urn False.    re
+00002520: 7475 726e 2072 652e 6d61 7463 6828 7222  turn re.match(r"
+00002530: 5b28 5f7c 5c2d 2961 2d7a 5d5b 285f 7c5c  [(_|\-)a-z][(_|\
+00002540: 2d29 612d 7a30 2d39 5d2a 2422 2c20 6e61  -)a-z0-9]*$", na
+00002550: 6d65 2920 6973 206e 6f74 204e 6f6e 650a  me) is not None.
+00002560: 0a0a 6465 6620 6973 5f76 616c 6964 5f76  ..def is_valid_v
+00002570: 6572 7369 6f6e 5f73 796e 7461 7828 7665  ersion_syntax(ve
+00002580: 7273 696f 6e29 3a0a 2020 2020 2222 220a  rsion):.    """.
+00002590: 2020 2020 5265 7475 726e 7320 5472 7565      Returns True
+000025a0: 2069 6620 7665 7273 696f 6e20 6973 2076   if version is v
+000025b0: 616c 6964 2c20 656c 7365 2046 616c 7365  alid, else False
+000025c0: 2e20 4163 6365 7074 6564 2076 6572 7369  . Accepted versi
+000025d0: 6f6e 2065 7861 6d70 6c65 7320 6172 653a  on examples are:
+000025e0: 0a20 2020 2020 2020 2022 312e 302e 3022  .        "1.0.0"
+000025f0: 2022 312e 312e 3022 2022 3132 332e 302e   "1.1.0" "123.0.
+00002600: 3132 3322 0a20 2020 2022 2222 0a20 2020  123".    """.   
+00002610: 2069 6620 6e6f 7420 7665 7273 696f 6e3a   if not version:
+00002620: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002630: 4661 6c73 650a 0a20 2020 2023 2061 6464  False..    # add
+00002640: 6564 2069 6e20 7635 312e 3020 7468 6520  ed in v51.0 the 
+00002650: 6162 696c 6974 7920 746f 2068 6176 6520  ability to have 
+00002660: 6d6f 7265 2074 6861 6e20 7468 7265 6520  more than three 
+00002670: 6e75 6d62 6572 7320 696e 2074 6865 2076  numbers in the v
+00002680: 6572 7369 6f6e 0a20 2020 2023 2028 6d69  ersion.    # (mi
+00002690: 6e20 7374 696c 6c20 3329 2073 696e 6365  n still 3) since
+000026a0: 206e 6577 2076 6572 7369 6f6e 696e 6720   new versioning 
+000026b0: 7363 6865 6d65 2068 6173 2035 2821 2129  scheme has 5(!!)
+000026c0: 206e 756d 6265 7273 0a20 2020 2072 6567   numbers.    reg
+000026d0: 6578 203d 2072 652e 636f 6d70 696c 6528  ex = re.compile(
+000026e0: 7227 5e5c 642b 5c2e 5c64 2b5c 2e5c 642b  r'^\d+\.\d+\.\d+
+000026f0: 283f 3a5c 2e5c 642b 292a 2427 290a 0a20  (?:\.\d+)*$').. 
+00002700: 2020 2072 6574 7572 6e20 7265 6765 782e     return regex.
+00002710: 6d61 7463 6828 7665 7273 696f 6e29 2069  match(version) i
+00002720: 7320 6e6f 7420 4e6f 6e65 0a0a 0a64 6566  s not None...def
+00002730: 2069 735f 7661 6c69 645f 7572 6c28 7572   is_valid_url(ur
+00002740: 6c29 3a0a 2020 2020 2222 220a 2020 2020  l):.    """.    
+00002750: 5265 7475 726e 7320 5472 7565 2069 6620  Returns True if 
+00002760: 7572 6c20 6973 2076 616c 6964 2c20 656c  url is valid, el
+00002770: 7365 2046 616c 7365 2e20 4163 6365 7074  se False. Accept
+00002780: 6564 2075 726c 2065 7861 6d70 6c65 7320  ed url examples 
+00002790: 6172 653a 0a20 2020 2020 2020 2022 6874  are:.        "ht
+000027a0: 7470 3a2f 2f77 7777 2e65 7861 6d70 6c65  tp://www.example
+000027b0: 2e63 6f6d 3a38 3030 3022 2c20 2268 7474  .com:8000", "htt
+000027c0: 7073 3a2f 2f77 7777 2e65 7861 6d70 6c65  ps://www.example
+000027d0: 2e63 6f6d 222c 2022 7777 772e 6578 616d  .com", "www.exam
+000027e0: 706c 652e 636f 6d22 2c20 2265 7861 6d70  ple.com", "examp
+000027f0: 6c65 2e63 6f6d 220a 2020 2020 2222 220a  le.com".    """.
+00002800: 0a20 2020 2069 6620 6e6f 7420 7572 6c3a  .    if not url:
+00002810: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002820: 4661 6c73 650a 0a20 2020 2072 6567 6578  False..    regex
+00002830: 203d 2072 652e 636f 6d70 696c 6528 0a20   = re.compile(. 
+00002840: 2020 2020 2020 2072 275e 2868 7474 7073         r'^(https
+00002850: 3f3a 2f2f 293f 2720 2023 206f 7074 696f  ?://)?'  # optio
+00002860: 6e61 6c20 6874 7470 3a2f 2f20 6f72 2068  nal http:// or h
+00002870: 7474 7073 3a2f 2f0a 2020 2020 2020 2020  ttps://.        
+00002880: 7227 283f 3a28 3f3a 5b41 2d5a 302d 395d  r'(?:(?:[A-Z0-9]
+00002890: 283f 3a5b 412d 5a30 2d39 2d5d 7b30 2c36  (?:[A-Z0-9-]{0,6
+000028a0: 317d 5b41 2d5a 302d 395d 293f 5c2e 292b  1}[A-Z0-9])?\.)+
+000028b0: 5b41 2d5a 5d7b 322c 367d 5c2e 3f29 2720  [A-Z]{2,6}\.?)' 
+000028c0: 2023 2064 6f6d 6169 6e2f 686f 7374 6e61   # domain/hostna
+000028d0: 6d65 0a20 2020 2020 2020 2072 2728 3f3a  me.        r'(?:
+000028e0: 2f3f 7c5b 2f3f 5d5c 532b 2927 2020 2320  /?|[/?]\S+)'  # 
+000028f0: 2e63 6f6d 2065 7463 2e0a 2020 2020 2020  .com etc..      
+00002900: 2020 7227 283f 3a3a 5c64 7b31 2c35 7d29    r'(?::\d{1,5})
+00002910: 3f24 272c 2020 2320 706f 7274 206e 756d  ?$',  # port num
+00002920: 6265 720a 2020 2020 2020 2020 7265 2e49  ber.        re.I
+00002930: 474e 4f52 4543 4153 4529 0a0a 2020 2020  GNORECASE)..    
+00002940: 7265 7475 726e 2072 6567 6578 2e73 6561  return regex.sea
+00002950: 7263 6828 7572 6c29 2069 7320 6e6f 7420  rch(url) is not 
+00002960: 4e6f 6e65 0a0a 0a64 6566 2069 735f 7661  None...def is_va
+00002970: 6c69 645f 6861 7368 2869 6e70 7574 5f68  lid_hash(input_h
+00002980: 6173 6829 3a0a 2020 2020 2222 2252 6574  ash):.    """Ret
+00002990: 7572 6e73 2054 7275 6520 6966 2074 6865  urns True if the
+000029a0: 2069 6e70 7574 5f68 6173 6820 6973 2061   input_hash is a
+000029b0: 2076 616c 6964 2053 4841 3235 3620 6861   valid SHA256 ha
+000029c0: 7368 2e0a 2020 2020 5265 7475 726e 7320  sh..    Returns 
+000029d0: 4661 6c73 6520 6966 3b0a 2020 2020 2020  False if;.      
+000029e0: 2020 2d20 2020 696e 7075 745f 6861 7368    -   input_hash
+000029f0: 2069 7320 6e6f 7420 6120 7374 720a 2020   is not a str.  
+00002a00: 2020 2020 2020 2d20 2020 696e 7075 745f        -   input_
+00002a10: 6861 7368 2069 7320 6e6f 7420 6571 7561  hash is not equa
+00002a20: 6c20 746f 2036 3420 6368 6172 6163 7465  l to 64 characte
+00002a30: 7273 0a20 2020 2020 2020 202d 2020 2074  rs.        -   t
+00002a40: 6861 7420 616c 6c20 6368 6172 6163 7465  hat all characte
+00002a50: 7273 2069 6e20 696e 7075 745f 6861 7368  rs in input_hash
+00002a60: 2061 7265 2062 6173 6520 3136 2028 7661   are base 16 (va
+00002a70: 6c69 6420 6865 7861 6465 6369 6d61 6c29  lid hexadecimal)
+00002a80: 0a0a 2020 2020 3a70 6172 616d 2069 6e70  ..    :param inp
+00002a90: 7574 5f68 6173 683a 2073 7472 2074 6f20  ut_hash: str to 
+00002aa0: 7661 6c69 6461 7465 2069 6620 6974 7320  validate if its 
+00002ab0: 6120 5348 4132 3536 2068 6173 680a 2020  a SHA256 hash.  
+00002ac0: 2020 3a74 7970 6520 696e 7075 745f 6861    :type input_ha
+00002ad0: 7368 3a20 7374 720a 2020 2020 3a72 6574  sh: str.    :ret
+00002ae0: 7572 6e3a 2054 7275 652f 4661 6c73 650a  urn: True/False.
+00002af0: 2020 2020 2222 220a 2020 2020 6966 206e      """.    if n
+00002b00: 6f74 2069 6e70 7574 5f68 6173 683a 0a20  ot input_hash:. 
+00002b10: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00002b20: 6c73 650a 0a20 2020 2072 6567 6578 203d  lse..    regex =
+00002b30: 2072 652e 636f 6d70 696c 6528 7227 5e5b   re.compile(r'^[
+00002b40: 612d 6630 2d39 5d7b 3634 7d28 3a2e 2b29  a-f0-9]{64}(:.+)
+00002b50: 3f24 2729 0a0a 2020 2020 7265 7475 726e  ?$')..    return
+00002b60: 2072 6567 6578 2e6d 6174 6368 2869 6e70   regex.match(inp
+00002b70: 7574 5f68 6173 6829 2069 7320 6e6f 7420  ut_hash) is not 
+00002b80: 4e6f 6e65 0a0a 0a64 6566 2064 6f65 735f  None...def does_
+00002b90: 7572 6c5f 636f 6e74 6169 6e28 7572 6c2c  url_contain(url,
+00002ba0: 2071 7279 293a 0a20 2020 2022 2222 0a20   qry):.    """. 
+00002bb0: 2020 2043 6865 636b 7320 6966 2075 726c     Checks if url
+00002bc0: 2069 7320 6120 7661 6c69 6420 7572 6c2c   is a valid url,
+00002bd0: 2069 6620 6974 2069 736e 2774 2072 6574   if it isn't ret
+00002be0: 7572 6e73 2046 616c 7365 2e0a 2020 2020  urns False..    
+00002bf0: 4368 6563 6b73 2069 6620 7172 7920 6973  Checks if qry is
+00002c00: 2069 6e20 7572 6c2e 2052 6574 7572 6e73   in url. Returns
+00002c10: 2054 7275 6520 6966 2069 7420 6973 0a20   True if it is. 
+00002c20: 2020 2022 2222 0a20 2020 2069 6620 6e6f     """.    if no
+00002c30: 7420 6973 5f76 616c 6964 5f75 726c 2875  t is_valid_url(u
+00002c40: 726c 293a 0a20 2020 2020 2020 2072 6574  rl):.        ret
+00002c50: 7572 6e20 4661 6c73 650a 0a20 2020 2072  urn False..    r
+00002c60: 6574 7572 6e20 7172 7920 696e 2075 726c  eturn qry in url
+00002c70: 0a0a 0a64 6566 2067 656e 6572 6174 655f  ...def generate_
+00002c80: 7575 6964 5f66 726f 6d5f 7374 7269 6e67  uuid_from_string
+00002c90: 2874 6865 5f73 7472 696e 6729 3a0a 2020  (the_string):.  
+00002ca0: 2020 2222 220a 2020 2020 5265 7475 726e    """.    Return
+00002cb0: 7320 5374 7269 6e67 2072 6570 7265 7365  s String represe
+00002cc0: 6e74 6174 696f 6e20 6f66 2074 6865 2055  ntation of the U
+00002cd0: 5549 4420 6f66 2061 2068 6578 206d 6435  UID of a hex md5
+00002ce0: 2068 6173 6820 6f66 2074 6865 2067 6976   hash of the giv
+00002cf0: 656e 2073 7472 696e 670a 2020 2020 2222  en string.    ""
+00002d00: 220a 0a20 2020 2023 2049 6e73 7461 6e73  "..    # Instans
+00002d10: 6961 7465 206e 6577 206d 6435 5f68 6173  iate new md5_has
+00002d20: 680a 2020 2020 6d64 355f 6861 7368 203d  h.    md5_hash =
+00002d30: 2068 6173 686c 6962 2e6d 6435 2829 0a0a   hashlib.md5()..
+00002d40: 2020 2020 2320 5061 7373 2074 6865 5f73      # Pass the_s
+00002d50: 7472 696e 6720 746f 2074 6865 206d 6435  tring to the md5
+00002d60: 5f68 6173 6820 6173 2062 7974 6573 0a20  _hash as bytes. 
+00002d70: 2020 206d 6435 5f68 6173 682e 7570 6461     md5_hash.upda
+00002d80: 7465 2874 6865 5f73 7472 696e 672e 656e  te(the_string.en
+00002d90: 636f 6465 2822 7574 662d 3822 2929 0a0a  code("utf-8"))..
+00002da0: 2020 2020 2320 4765 6e65 7261 7465 2074      # Generate t
+00002db0: 6865 2068 6578 206d 6435 2068 6173 6820  he hex md5 hash 
+00002dc0: 6f66 2061 6c6c 2074 6865 2072 6561 6420  of all the read 
+00002dd0: 6279 7465 730a 2020 2020 7468 655f 6d64  bytes.    the_md
+00002de0: 355f 6865 785f 7374 7220 3d20 6d64 355f  5_hex_str = md5_
+00002df0: 6861 7368 2e68 6578 6469 6765 7374 2829  hash.hexdigest()
+00002e00: 0a0a 2020 2020 2320 5265 7475 726e 2061  ..    # Return a
+00002e10: 2053 7472 696e 6720 7265 7065 7273 656e   String repersen
+00002e20: 6174 696f 6e20 6f66 2074 6865 2075 7569  ation of the uui
+00002e30: 6420 6f66 2074 6865 206d 6435 2068 6173  d of the md5 has
+00002e40: 680a 2020 2020 7265 7475 726e 2073 7472  h.    return str
+00002e50: 2875 7569 642e 5555 4944 2874 6865 5f6d  (uuid.UUID(the_m
+00002e60: 6435 5f68 6578 5f73 7472 2929 0a0a 0a64  d5_hex_str))...d
+00002e70: 6566 2068 6173 5f70 6572 6d69 7373 696f  ef has_permissio
+00002e80: 6e73 2870 6572 6d69 7373 696f 6e73 2c20  ns(permissions, 
+00002e90: 7061 7468 293a 0a20 2020 2022 2222 0a20  path):.    """. 
+00002ea0: 2020 2052 6169 7365 7320 616e 2065 7863     Raises an exc
+00002eb0: 6570 7469 6f6e 2069 6620 7468 6520 7573  eption if the us
+00002ec0: 6572 2064 6f65 7320 6e6f 7420 6861 7665  er does not have
+00002ed0: 2074 6865 2067 6976 656e 2070 6572 6d69   the given permi
+00002ee0: 7373 696f 6e73 2074 6f20 7061 7468 0a20  ssions to path. 
+00002ef0: 2020 2022 2222 0a0a 2020 2020 4c4f 472e     """..    LOG.
+00002f00: 6465 6275 6728 2263 6865 636b 696e 6720  debug("checking 
+00002f10: 6966 3a20 2573 2068 6173 2063 6f72 7265  if: %s has corre
+00002f20: 6374 2070 6572 6d69 7373 696f 6e73 222c  ct permissions",
+00002f30: 2070 6174 6829 0a0a 2020 2020 6966 206e   path)..    if n
+00002f40: 6f74 206f 732e 6163 6365 7373 2870 6174  ot os.access(pat
+00002f50: 682c 2070 6572 6d69 7373 696f 6e73 293a  h, permissions):
+00002f60: 0a0a 2020 2020 2020 2020 6966 2070 6572  ..        if per
+00002f70: 6d69 7373 696f 6e73 2069 7320 6f73 2e52  missions is os.R
+00002f80: 5f4f 4b3a 0a20 2020 2020 2020 2020 2020  _OK:.           
+00002f90: 2070 6572 6d69 7373 696f 6e73 203d 2022   permissions = "
+00002fa0: 5245 4144 220a 2020 2020 2020 2020 656c  READ".        el
+00002fb0: 6966 2070 6572 6d69 7373 696f 6e73 2069  if permissions i
+00002fc0: 7320 6f73 2e57 5f4f 4b3a 0a20 2020 2020  s os.W_OK:.     
+00002fd0: 2020 2020 2020 2070 6572 6d69 7373 696f         permissio
+00002fe0: 6e73 203d 2022 5752 4954 4522 0a0a 2020  ns = "WRITE"..  
+00002ff0: 2020 2020 2020 7261 6973 6520 5344 4b45        raise SDKE
+00003000: 7863 6570 7469 6f6e 2822 5573 6572 2064  xception("User d
+00003010: 6f65 7320 6e6f 7420 6861 7665 207b 307d  oes not have {0}
+00003020: 2070 6572 6d69 7373 696f 6e73 2066 6f72   permissions for
+00003030: 3a20 7b31 7d22 2e66 6f72 6d61 7428 7065  : {1}".format(pe
+00003040: 726d 6973 7369 6f6e 732c 2070 6174 6829  rmissions, path)
+00003050: 290a 0a0a 6465 6620 7661 6c69 6461 7465  )...def validate
+00003060: 5f66 696c 655f 7061 7468 7328 7065 726d  _file_paths(perm
+00003070: 6973 7369 6f6e 732c 202a 6172 6773 293a  issions, *args):
+00003080: 0a20 2020 2022 2222 0a20 2020 2043 6865  .    """.    Che
+00003090: 636b 2074 6865 2067 6976 656e 202a 6172  ck the given *ar
+000030a0: 6773 2070 6174 6873 2065 7869 7374 2061  gs paths exist a
+000030b0: 6e64 2068 6173 2074 6865 2067 6976 656e  nd has the given
+000030c0: 2070 6572 6d69 7373 696f 6e73 2c20 656c   permissions, el
+000030d0: 7365 2072 6169 7365 7320 616e 2045 7863  se raises an Exc
+000030e0: 6570 7469 6f6e 0a20 2020 2022 2222 0a0a  eption.    """..
+000030f0: 2020 2020 2320 466f 7220 6561 6368 202a      # For each *
+00003100: 6172 6773 0a20 2020 2066 6f72 2070 6174  args.    for pat
+00003110: 685f 746f 5f66 696c 6520 696e 2061 7267  h_to_file in arg
+00003120: 733a 0a20 2020 2020 2020 2023 2043 6865  s:.        # Che
+00003130: 636b 2074 6865 2066 696c 6520 6578 6973  ck the file exis
+00003140: 7473 0a20 2020 2020 2020 2069 6620 6e6f  ts.        if no
+00003150: 7420 6f73 2e70 6174 682e 6973 6669 6c65  t os.path.isfile
+00003160: 2870 6174 685f 746f 5f66 696c 6529 3a0a  (path_to_file):.
+00003170: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00003180: 6520 5344 4b45 7863 6570 7469 6f6e 2875  e SDKException(u
+00003190: 227b 307d 3a20 7b31 7d22 2e66 6f72 6d61  "{0}: {1}".forma
+000031a0: 7428 636f 6e73 7461 6e74 732e 4552 524f  t(constants.ERRO
+000031b0: 525f 4e4f 545f 4649 4e44 5f46 494c 452c  R_NOT_FIND_FILE,
+000031c0: 2070 6174 685f 746f 5f66 696c 6529 290a   path_to_file)).
+000031d0: 0a20 2020 2020 2020 2069 6620 7065 726d  .        if perm
+000031e0: 6973 7369 6f6e 733a 0a20 2020 2020 2020  issions:.       
+000031f0: 2020 2020 2023 2043 6865 636b 2077 6520       # Check we 
+00003200: 6861 7665 2074 6865 2063 6f72 7265 6374  have the correct
+00003210: 2070 6572 6d69 7373 696f 6e73 0a20 2020   permissions.   
+00003220: 2020 2020 2020 2020 2068 6173 5f70 6572           has_per
+00003230: 6d69 7373 696f 6e73 2870 6572 6d69 7373  missions(permiss
+00003240: 696f 6e73 2c20 7061 7468 5f74 6f5f 6669  ions, path_to_fi
+00003250: 6c65 290a 0a0a 6465 6620 7661 6c69 6461  le)...def valida
+00003260: 7465 5f64 6972 5f70 6174 6873 2870 6572  te_dir_paths(per
+00003270: 6d69 7373 696f 6e73 2c20 2a61 7267 7329  missions, *args)
+00003280: 3a0a 2020 2020 2222 220a 2020 2020 4368  :.    """.    Ch
+00003290: 6563 6b20 7468 6520 6769 7665 6e20 2a61  eck the given *a
+000032a0: 7267 7320 7061 7468 7320 6172 6520 4469  rgs paths are Di
+000032b0: 7265 6374 6f72 6965 7320 616e 6420 6861  rectories and ha
+000032c0: 7665 2074 6865 2067 6976 656e 2070 6572  ve the given per
+000032d0: 6d69 7373 696f 6e73 2c20 656c 7365 2072  missions, else r
+000032e0: 6169 7365 7320 616e 2045 7863 6570 7469  aises an Excepti
+000032f0: 6f6e 0a20 2020 2022 2222 0a0a 2020 2020  on.    """..    
+00003300: 2320 466f 7220 6561 6368 202a 6172 6773  # For each *args
+00003310: 0a20 2020 2066 6f72 2070 6174 685f 746f  .    for path_to
+00003320: 5f64 6972 2069 6e20 6172 6773 3a0a 2020  _dir in args:.  
+00003330: 2020 2020 2020 2320 4368 6563 6b20 7468        # Check th
+00003340: 6520 6469 7220 6578 6973 7473 0a20 2020  e dir exists.   
+00003350: 2020 2020 2069 6620 6e6f 7420 6f73 2e70       if not os.p
+00003360: 6174 682e 6973 6469 7228 7061 7468 5f74  ath.isdir(path_t
+00003370: 6f5f 6469 7229 3a0a 2020 2020 2020 2020  o_dir):.        
+00003380: 2020 2020 7261 6973 6520 5344 4b45 7863      raise SDKExc
+00003390: 6570 7469 6f6e 2875 227b 307d 3a20 7b31  eption(u"{0}: {1
+000033a0: 7d22 2e66 6f72 6d61 7428 636f 6e73 7461  }".format(consta
+000033b0: 6e74 732e 4552 524f 525f 4e4f 545f 4649  nts.ERROR_NOT_FI
+000033c0: 4e44 5f44 4952 2c20 7061 7468 5f74 6f5f  ND_DIR, path_to_
+000033d0: 6469 7229 290a 0a20 2020 2020 2020 2069  dir))..        i
+000033e0: 6620 7065 726d 6973 7369 6f6e 733a 0a20  f permissions:. 
+000033f0: 2020 2020 2020 2020 2020 2023 2043 6865             # Che
+00003400: 636b 2077 6520 6861 7665 2074 6865 2063  ck we have the c
+00003410: 6f72 7265 6374 2070 6572 6d69 7373 696f  orrect permissio
+00003420: 6e73 0a20 2020 2020 2020 2020 2020 2068  ns.            h
+00003430: 6173 5f70 6572 6d69 7373 696f 6e73 2870  as_permissions(p
+00003440: 6572 6d69 7373 696f 6e73 2c20 7061 7468  ermissions, path
+00003450: 5f74 6f5f 6469 7229 0a0a 0a64 6566 2067  _to_dir)...def g
+00003460: 6574 5f72 6573 696c 6965 6e74 5f73 6572  et_resilient_ser
+00003470: 7665 725f 696e 666f 2872 6573 5f63 6c69  ver_info(res_cli
+00003480: 656e 742c 206b 6579 735f 746f 5f67 6574  ent, keys_to_get
+00003490: 3d5b 5d29 3a0a 2020 2020 2222 220a 2020  =[]):.    """.  
+000034a0: 2020 4361 6c6c 7320 7468 6520 636f 6e73    Calls the cons
+000034b0: 742f 2065 6e64 706f 696e 7420 616e 6420  t/ endpoint and 
+000034c0: 7265 7475 726e 7320 7468 6520 696e 666f  returns the info
+000034d0: 2073 7065 6369 6669 6564 2069 6e20 6b65   specified in ke
+000034e0: 7973 5f74 6f5f 6765 740a 0a20 2020 202a  ys_to_get..    *
+000034f0: 2a45 7861 6d70 6c65 3a2a 2a0a 0a20 2020  *Example:**..   
+00003500: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+00003510: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+00003520: 2073 6572 7665 725f 7665 7273 696f 6e20   server_version 
+00003530: 3d20 6765 745f 7265 7369 6c69 656e 745f  = get_resilient_
+00003540: 7365 7276 6572 5f69 6e66 6f28 7265 735f  server_info(res_
+00003550: 636c 6965 6e74 2c20 5b22 7365 7276 6572  client, ["server
+00003560: 5f76 6572 7369 6f6e 225d 290a 0a20 2020  _version"])..   
+00003570: 203a 7061 7261 6d20 7265 735f 636c 6965   :param res_clie
+00003580: 6e74 3a20 7265 7175 6972 6564 2066 6f72  nt: required for
+00003590: 2063 6f6d 6d75 6e69 6361 7469 6f6e 2062   communication b
+000035a0: 6163 6b20 746f 2072 6573 696c 6965 6e74  ack to resilient
+000035b0: 0a20 2020 203a 7479 7065 2072 6573 5f63  .    :type res_c
+000035c0: 6c69 656e 743a 2073 646b 5f68 656c 7065  lient: sdk_helpe
+000035d0: 7273 2e67 6574 5f72 6573 696c 6965 6e74  rs.get_resilient
+000035e0: 5f63 6c69 656e 7428 290a 2020 2020 3a70  _client().    :p
+000035f0: 6172 616d 206b 6579 735f 746f 5f67 6574  aram keys_to_get
+00003600: 3a20 6c69 7374 206f 6620 7374 7269 6e67  : list of string
+00003610: 7320 6f66 2074 6865 206b 6579 7320 746f  s of the keys to
+00003620: 2072 6574 7572 6e20 6672 6f6d 2074 6865   return from the
+00003630: 2063 6f6e 7374 2f20 656e 6470 6f69 6e74   const/ endpoint
+00003640: 2e20 4966 2060 604e 6f6e 6560 600a 2020  . If ``None``.  
+00003650: 2020 7265 7475 726e 7320 7468 6520 7768    returns the wh
+00003660: 6f6c 6520 7265 7370 6f6e 7365 0a20 2020  ole response.   
+00003670: 203a 7479 7065 206b 6579 735f 746f 5f67   :type keys_to_g
+00003680: 6574 3a20 6c69 7374 0a20 2020 203a 7265  et: list.    :re
+00003690: 7475 726e 3a20 7265 7370 6f6e 7365 2066  turn: response f
+000036a0: 726f 6d20 636f 6e73 742f 0a20 2020 203a  rom const/.    :
+000036b0: 7274 7970 653a 2064 6963 740a 2020 2020  rtype: dict.    
+000036c0: 2222 220a 2020 2020 4c4f 472e 6465 6275  """.    LOG.debu
+000036d0: 6728 2247 6574 7469 6e67 2073 6572 7665  g("Getting serve
+000036e0: 7220 696e 666f 2229 0a20 2020 2073 6572  r info").    ser
+000036f0: 7665 725f 696e 666f 203d 2072 6573 5f63  ver_info = res_c
+00003700: 6c69 656e 742e 6765 7428 222f 636f 6e73  lient.get("/cons
+00003710: 742f 222c 2069 735f 7572 695f 6162 736f  t/", is_uri_abso
+00003720: 6c75 7465 3d54 7275 6529 0a0a 2020 2020  lute=True)..    
+00003730: 6966 206b 6579 735f 746f 5f67 6574 3a0a  if keys_to_get:.
+00003740: 2020 2020 2020 2020 7365 7276 6572 5f69          server_i
+00003750: 6e66 6f20 3d20 7b6b 3a20 7365 7276 6572  nfo = {k: server
+00003760: 5f69 6e66 6f2e 6765 7428 6b2c 207b 7d29  _info.get(k, {})
+00003770: 2066 6f72 206b 2069 6e20 6b65 7973 5f74   for k in keys_t
+00003780: 6f5f 6765 747d 0a0a 2020 2020 7265 7475  o_get}..    retu
+00003790: 726e 2073 6572 7665 725f 696e 666f 0a0a  rn server_info..
+000037a0: 0a64 6566 2067 6574 5f72 6573 696c 6965  .def get_resilie
+000037b0: 6e74 5f73 6572 7665 725f 7665 7273 696f  nt_server_versio
+000037c0: 6e28 7265 735f 636c 6965 6e74 293a 0a20  n(res_client):. 
+000037d0: 2020 2022 2222 0a20 2020 2055 7365 7320     """.    Uses 
+000037e0: 6765 745f 7265 7369 6c69 656e 745f 7365  get_resilient_se
+000037f0: 7276 6572 5f69 6e66 6f20 746f 2067 6574  rver_info to get
+00003800: 2074 6865 2022 7365 7276 6572 5f76 6572   the "server_ver
+00003810: 7369 6f6e 220a 2020 2020 616e 6420 636f  sion".    and co
+00003820: 6e76 6572 7473 2069 7420 696e 746f 2061  nverts it into a
+00003830: 2056 6572 7369 6f6e 206f 626a 6563 7420   Version object 
+00003840: 616e 6420 7265 7475 726e 7320 6974 0a0a  and returns it..
+00003850: 2020 2020 3a70 6172 616d 2072 6573 5f63      :param res_c
+00003860: 6c69 656e 743a 2072 6571 7569 7265 6420  lient: required 
+00003870: 666f 7220 636f 6d6d 756e 6963 6174 696f  for communicatio
+00003880: 6e20 6261 636b 2074 6f20 7265 7369 6c69  n back to resili
+00003890: 656e 740a 2020 2020 3a74 7970 6520 7265  ent.    :type re
+000038a0: 735f 636c 6965 6e74 3a20 7364 6b5f 6865  s_client: sdk_he
+000038b0: 6c70 6572 732e 6765 745f 7265 7369 6c69  lpers.get_resili
+000038c0: 656e 745f 636c 6965 6e74 2829 0a20 2020  ent_client().   
+000038d0: 203a 7265 7475 726e 3a20 7468 6520 7365   :return: the se
+000038e0: 7276 6572 5f76 6572 7369 6f6e 2e76 6572  rver_version.ver
+000038f0: 7369 6f6e 2076 616c 7565 0a20 2020 203a  sion value.    :
+00003900: 7274 7970 653a 2056 6572 7369 6f6e 206f  rtype: Version o
+00003910: 626a 6563 740a 2020 2020 2222 220a 2020  bject.    """.  
+00003920: 2020 4c4f 472e 6465 6275 6728 2247 6574    LOG.debug("Get
+00003930: 7469 6e67 2073 6572 7665 7220 7665 7273  ting server vers
+00003940: 696f 6e22 290a 0a20 2020 2069 6620 636f  ion")..    if co
+00003950: 6e73 7461 6e74 732e 4355 5252 454e 545f  nstants.CURRENT_
+00003960: 534f 4152 5f53 4552 5645 525f 5645 5253  SOAR_SERVER_VERS
+00003970: 494f 4e3a 0a20 2020 2020 2020 2072 6574  ION:.        ret
+00003980: 7572 6e20 636f 6e73 7461 6e74 732e 4355  urn constants.CU
+00003990: 5252 454e 545f 534f 4152 5f53 4552 5645  RRENT_SOAR_SERVE
+000039a0: 525f 5645 5253 494f 4e0a 0a20 2020 2073  R_VERSION..    s
+000039b0: 6572 7665 725f 7665 7273 696f 6e20 3d20  erver_version = 
+000039c0: 6765 745f 7265 7369 6c69 656e 745f 7365  get_resilient_se
+000039d0: 7276 6572 5f69 6e66 6f28 7265 735f 636c  rver_info(res_cl
+000039e0: 6965 6e74 2c20 5b22 7365 7276 6572 5f76  ient, ["server_v
+000039f0: 6572 7369 6f6e 225d 292e 6765 7428 2273  ersion"]).get("s
+00003a00: 6572 7665 725f 7665 7273 696f 6e22 2c20  erver_version", 
+00003a10: 7b7d 290a 0a20 2020 2063 6f6e 7374 616e  {})..    constan
+00003a20: 7473 2e43 5552 5245 4e54 5f53 4f41 525f  ts.CURRENT_SOAR_
+00003a30: 5345 5256 4552 5f56 4552 5349 4f4e 203d  SERVER_VERSION =
+00003a40: 2070 6172 7365 5f76 6572 7369 6f6e 2873   parse_version(s
+00003a50: 6572 7665 725f 7665 7273 696f 6e2e 6765  erver_version.ge
+00003a60: 7428 2276 6572 7369 6f6e 222c 2022 302e  t("version", "0.
+00003a70: 302e 302e 3022 2929 0a0a 2020 2020 4c4f  0.0.0"))..    LO
+00003a80: 472e 696e 666f 2822 4942 4d20 5365 6375  G.info("IBM Secu
+00003a90: 7269 7479 2053 4f41 5220 7665 7273 696f  rity SOAR versio
+00003aa0: 6e3a 2076 2573 222c 2063 6f6e 7374 616e  n: v%s", constan
+00003ab0: 7473 2e43 5552 5245 4e54 5f53 4f41 525f  ts.CURRENT_SOAR_
+00003ac0: 5345 5256 4552 5f56 4552 5349 4f4e 290a  SERVER_VERSION).
+00003ad0: 0a20 2020 2072 6574 7572 6e20 636f 6e73  .    return cons
+00003ae0: 7461 6e74 732e 4355 5252 454e 545f 534f  tants.CURRENT_SO
+00003af0: 4152 5f53 4552 5645 525f 5645 5253 494f  AR_SERVER_VERSIO
+00003b00: 4e0a 0a0a 6465 6620 6765 745f 6c61 7465  N...def get_late
+00003b10: 7374 5f6f 7267 5f65 7870 6f72 7428 7265  st_org_export(re
+00003b20: 735f 636c 6965 6e74 293a 0a20 2020 2022  s_client):.    "
+00003b30: 2222 0a20 2020 2047 656e 6572 6174 6573  "".    Generates
+00003b40: 2061 206e 6577 2045 7870 6f72 7420 6f6e   a new Export on
+00003b50: 2053 4f41 522e 0a20 2020 2052 6574 7572   SOAR..    Retur
+00003b60: 6e73 2074 6865 2050 4f53 5420 7265 7370  ns the POST resp
+00003b70: 6f6e 7365 0a20 2020 2022 2222 0a20 2020  onse.    """.   
+00003b80: 204c 4f47 2e64 6562 7567 2822 4765 6e65   LOG.debug("Gene
+00003b90: 7261 7469 6e67 206e 6577 206f 7267 616e  rating new organ
+00003ba0: 697a 6174 696f 6e20 6578 706f 7274 2229  ization export")
+00003bb0: 0a20 2020 206c 6174 6573 745f 6578 706f  .    latest_expo
+00003bc0: 7274 5f75 7269 203d 2022 2f63 6f6e 6669  rt_uri = "/confi
+00003bd0: 6775 7261 7469 6f6e 732f 6578 706f 7274  gurations/export
+00003be0: 732f 220a 0a20 2020 2063 7573 746f 6d69  s/"..    customi
+00003bf0: 7a61 7469 6f6e 735f 746f 5f67 6574 203d  zations_to_get =
+00003c00: 207b 0a20 2020 2020 2020 2022 6c61 796f   {.        "layo
+00003c10: 7574 7322 3a20 5472 7565 2c0a 2020 2020  uts": True,.    
+00003c20: 2020 2020 2261 6374 696f 6e73 223a 2054      "actions": T
+00003c30: 7275 652c 0a20 2020 2020 2020 2022 7068  rue,.        "ph
+00003c40: 6173 6573 5f61 6e64 5f74 6173 6b73 223a  ases_and_tasks":
+00003c50: 2054 7275 650a 2020 2020 7d0a 2020 2020   True.    }.    
+00003c60: 7365 7276 6572 5f76 6572 7369 6f6e 203d  server_version =
+00003c70: 2067 6574 5f72 6573 696c 6965 6e74 5f73   get_resilient_s
+00003c80: 6572 7665 725f 7665 7273 696f 6e28 7265  erver_version(re
+00003c90: 735f 636c 6965 6e74 290a 0a20 2020 2069  s_client)..    i
+00003ca0: 6620 7365 7276 6572 5f76 6572 7369 6f6e  f server_version
+00003cb0: 203e 3d20 636f 6e73 7461 6e74 732e 4d49   >= constants.MI
+00003cc0: 4e5f 534f 4152 5f53 4552 5645 525f 5645  N_SOAR_SERVER_VE
+00003cd0: 5253 494f 4e5f 504c 4159 424f 4f4b 533a  RSION_PLAYBOOKS:
+00003ce0: 0a20 2020 2020 2020 2063 7573 746f 6d69  .        customi
+00003cf0: 7a61 7469 6f6e 735f 746f 5f67 6574 2e75  zations_to_get.u
+00003d00: 7064 6174 6528 7b22 706c 6179 626f 6f6b  pdate({"playbook
+00003d10: 7322 3a20 5472 7565 7d29 0a0a 2020 2020  s": True})..    
+00003d20: 7265 7475 726e 2072 6573 5f63 6c69 656e  return res_clien
+00003d30: 742e 706f 7374 286c 6174 6573 745f 6578  t.post(latest_ex
+00003d40: 706f 7274 5f75 7269 2c20 6375 7374 6f6d  port_uri, custom
+00003d50: 697a 6174 696f 6e73 5f74 6f5f 6765 7429  izations_to_get)
+00003d60: 0a0a 0a64 6566 2061 6464 5f63 6f6e 6669  ...def add_confi
+00003d70: 6775 7261 7469 6f6e 5f69 6d70 6f72 7428  guration_import(
+00003d80: 6e65 775f 6578 706f 7274 5f64 6174 612c  new_export_data,
+00003d90: 2072 6573 5f63 6c69 656e 7429 3a0a 2020   res_client):.  
+00003da0: 2020 2222 220a 2020 2020 4d61 6b65 7320    """.    Makes 
+00003db0: 6120 5245 5354 2072 6571 7565 7374 2074  a REST request t
+00003dc0: 6f20 6164 6420 6120 636f 6e66 6967 7572  o add a configur
+00003dd0: 6174 696f 6e20 696d 706f 7274 2e0a 0a20  ation import... 
+00003de0: 2020 2041 6674 6572 2074 6865 2072 6571     After the req
+00003df0: 7565 7374 2069 7320 6d61 6465 2c20 7468  uest is made, th
+00003e00: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+00003e10: 696d 706f 7274 2069 7320 7365 7420 6174  import is set at
+00003e20: 2061 2070 656e 6469 6e67 2073 7461 7465   a pending state
+00003e30: 2061 6e64 206e 6565 6473 2074 6f20 6265   and needs to be
+00003e40: 2063 6f6e 6669 726d 6564 2e0a 2020 2020   confirmed..    
+00003e50: 4966 2074 6865 2063 6f6e 6669 6775 7261  If the configura
+00003e60: 7469 6f6e 2073 7461 7465 2069 7320 6e6f  tion state is no
+00003e70: 7420 7265 706f 7274 6564 2061 7320 7065  t reported as pe
+00003e80: 6e64 696e 672c 2072 6169 7365 2061 6e20  nding, raise an 
+00003e90: 5344 4b20 4578 6365 7074 696f 6e2e 0a0a  SDK Exception...
+00003ea0: 0a20 2020 203a 7061 7261 6d20 6e65 775f  .    :param new_
+00003eb0: 6578 706f 7274 5f64 6174 613a 2041 2064  export_data: A d
+00003ec0: 6963 7420 7265 7072 6573 656e 7469 6e67  ict representing
+00003ed0: 2061 2063 6f6e 6669 6775 7261 7469 6f6e   a configuration
+00003ee0: 2069 6d70 6f72 7420 4454 4f0a 2020 2020   import DTO.    
+00003ef0: 3a74 7970 6520 7265 7375 6c74 3a20 6469  :type result: di
+00003f00: 6374 0a20 2020 203a 7061 7261 6d20 696d  ct.    :param im
+00003f10: 706f 7274 5f69 643a 2054 6865 2049 4420  port_id: The ID 
+00003f20: 6f66 2074 6865 2063 6f6e 6669 6775 7261  of the configura
+00003f30: 7469 6f6e 2069 6d70 6f72 7420 746f 2063  tion import to c
+00003f40: 6f6e 6669 726d 0a20 2020 203a 7479 7065  onfirm.    :type
+00003f50: 2069 6d70 6f72 745f 6964 3a20 696e 740a   import_id: int.
+00003f60: 2020 2020 3a70 6172 616d 2072 6573 5f63      :param res_c
+00003f70: 6c69 656e 743a 2041 6e20 696e 7374 616e  lient: An instan
+00003f80: 7469 6174 6564 2072 6573 5f63 6c69 656e  tiated res_clien
+00003f90: 7420 666f 7220 6d61 6b69 6e67 2052 4553  t for making RES
+00003fa0: 5420 6361 6c6c 730a 2020 2020 3a74 7970  T calls.    :typ
+00003fb0: 6520 7265 735f 636c 6965 6e74 3a20 5369  e res_client: Si
+00003fc0: 6d70 6c65 436c 6965 6e74 2829 0a20 2020  mpleClient().   
+00003fd0: 203a 7261 6973 6573 2053 444b 4578 6365   :raises SDKExce
+00003fe0: 7074 696f 6e3a 2049 6620 7468 6520 636f  ption: If the co
+00003ff0: 6e66 6972 6d61 7469 6f6e 2072 6571 7565  nfirmation reque
+00004000: 7374 2066 6169 6c73 2072 6169 7365 2061  st fails raise a
+00004010: 6e20 5344 4b45 7863 6570 7469 6f6e 0a20  n SDKException. 
+00004020: 2020 2022 2222 0a20 2020 2074 7279 3a0a     """.    try:.
+00004030: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00004040: 2072 6573 5f63 6c69 656e 742e 706f 7374   res_client.post
+00004050: 2863 6f6e 7374 616e 7473 2e49 4d50 4f52  (constants.IMPOR
+00004060: 545f 5552 4c2c 206e 6577 5f65 7870 6f72  T_URL, new_expor
+00004070: 745f 6461 7461 290a 2020 2020 6578 6365  t_data).    exce
+00004080: 7074 2072 6571 7565 7374 732e 5265 7175  pt requests.Requ
+00004090: 6573 7445 7863 6570 7469 6f6e 2061 7320  estException as 
+000040a0: 7570 6c6f 6164 5f65 7863 6570 7469 6f6e  upload_exception
+000040b0: 3a0a 2020 2020 2020 2020 4c4f 472e 6465  :.        LOG.de
+000040c0: 6275 6728 6e65 775f 6578 706f 7274 5f64  bug(new_export_d
+000040d0: 6174 6129 0a20 2020 2020 2020 2072 6169  ata).        rai
+000040e0: 7365 2053 444b 4578 6365 7074 696f 6e28  se SDKException(
+000040f0: 7570 6c6f 6164 5f65 7863 6570 7469 6f6e  upload_exception
+00004100: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00004110: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+00004120: 7461 6e63 6528 7265 7375 6c74 2c20 6469  tance(result, di
+00004130: 6374 290a 2020 2020 6966 2072 6573 756c  ct).    if resul
+00004140: 742e 6765 7428 2273 7461 7475 7322 2c20  t.get("status", 
+00004150: 2727 2920 3d3d 2022 5045 4e44 494e 4722  '') == "PENDING"
+00004160: 3a0a 2020 2020 2020 2020 636f 6e66 6972  :.        confir
+00004170: 6d5f 636f 6e66 6967 7572 6174 696f 6e5f  m_configuration_
+00004180: 696d 706f 7274 2872 6573 756c 742c 2072  import(result, r
+00004190: 6573 756c 742e 6765 7428 2269 6422 292c  esult.get("id"),
+000041a0: 2072 6573 5f63 6c69 656e 7429 0a20 2020   res_client).   
+000041b0: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
+000041c0: 6169 7365 2053 444b 4578 6365 7074 696f  aise SDKExceptio
+000041d0: 6e28 0a20 2020 2020 2020 2020 2020 2022  n(.            "
+000041e0: 436f 756c 6420 6e6f 7420 696d 706f 7274  Could not import
+000041f0: 2062 6563 6175 7365 2074 6865 2073 6572   because the ser
+00004200: 7665 7220 6469 6420 6e6f 7420 7265 7475  ver did not retu
+00004210: 726e 2061 6e20 696d 706f 7274 2049 4422  rn an import ID"
+00004220: 290a 0a0a 6465 6620 636f 6e66 6972 6d5f  )...def confirm_
+00004230: 636f 6e66 6967 7572 6174 696f 6e5f 696d  configuration_im
+00004240: 706f 7274 2872 6573 756c 742c 2069 6d70  port(result, imp
+00004250: 6f72 745f 6964 2c20 7265 735f 636c 6965  ort_id, res_clie
+00004260: 6e74 293a 0a20 2020 2022 2222 0a20 2020  nt):.    """.   
+00004270: 204d 616b 6573 2061 2052 4553 5420 7265   Makes a REST re
+00004280: 7175 6573 7420 746f 2063 6f6e 6669 726d  quest to confirm
+00004290: 2061 2070 656e 6469 6e67 2063 6f6e 6669   a pending confi
+000042a0: 6775 7261 7469 6f6e 2069 6d70 6f72 7420  guration import 
+000042b0: 6173 2061 6363 6570 7465 642e 0a0a 2020  as accepted...  
+000042c0: 2020 5461 6b65 7320 3320 7061 7261 6d73    Takes 3 params
+000042d0: 0a20 2020 2054 6865 2072 6573 756c 7420  .    The result 
+000042e0: 6f66 2061 2063 6f6e 6669 6775 7261 7469  of a configurati
+000042f0: 6f6e 2069 6d70 6f72 7420 7265 7175 6573  on import reques
+00004300: 740a 2020 2020 5468 6520 4944 206f 6620  t.    The ID of 
+00004310: 7468 6520 636f 6e66 6967 7572 6174 696f  the configuratio
+00004320: 6e20 696d 706f 7274 2072 6571 7565 7374  n import request
+00004330: 0a20 2020 2041 2072 6573 5f63 6c69 656e  .    A res_clien
+00004340: 7420 746f 2070 6572 666f 726d 2074 6865  t to perform the
+00004350: 2072 6571 7565 7374 0a0a 2020 2020 3a70   request..    :p
+00004360: 6172 616d 2072 6573 756c 743a 2052 6573  aram result: Res
+00004370: 756c 7420 6f66 2074 6865 2063 6f6e 6669  ult of the confi
+00004380: 6775 7261 7469 6f6e 2069 6d70 6f72 7420  guration import 
+00004390: 7265 7175 6573 740a 2020 2020 3a74 7970  request.    :typ
+000043a0: 6520 7265 7375 6c74 3a20 6469 6374 0a20  e result: dict. 
+000043b0: 2020 203a 7061 7261 6d20 696d 706f 7274     :param import
+000043c0: 5f69 643a 2054 6865 2049 4420 6f66 2074  _id: The ID of t
+000043d0: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
+000043e0: 2069 6d70 6f72 7420 746f 2063 6f6e 6669   import to confi
+000043f0: 726d 0a20 2020 203a 7479 7065 2069 6d70  rm.    :type imp
+00004400: 6f72 745f 6964 3a20 696e 740a 2020 2020  ort_id: int.    
+00004410: 3a70 6172 616d 2072 6573 5f63 6c69 656e  :param res_clien
+00004420: 743a 2041 6e20 696e 7374 616e 7469 6174  t: An instantiat
+00004430: 6564 2072 6573 5f63 6c69 656e 7420 666f  ed res_client fo
+00004440: 7220 6d61 6b69 6e67 2052 4553 5420 6361  r making REST ca
+00004450: 6c6c 730a 2020 2020 3a74 7970 6520 7265  lls.    :type re
+00004460: 735f 636c 6965 6e74 3a20 5369 6d70 6c65  s_client: Simple
+00004470: 436c 6965 6e74 2829 0a20 2020 203a 7261  Client().    :ra
+00004480: 6973 6573 2053 444b 4578 6365 7074 696f  ises SDKExceptio
+00004490: 6e3a 2049 6620 7468 6520 636f 6e66 6972  n: If the confir
+000044a0: 6d61 7469 6f6e 2072 6571 7565 7374 2066  mation request f
+000044b0: 6169 6c73 2072 6169 7365 2061 6e20 5344  ails raise an SD
+000044c0: 4b45 7863 6570 7469 6f6e 0a20 2020 2022  KException.    "
+000044d0: 2222 0a0a 2020 2020 7265 7375 6c74 5b22  ""..    result["
+000044e0: 7374 6174 7573 225d 203d 2022 4143 4345  status"] = "ACCE
+000044f0: 5054 4544 2220 2020 2020 2023 2048 6176  PTED"      # Hav
+00004500: 6520 746f 2063 6f6e 6669 726d 2063 6861  e to confirm cha
+00004510: 6e67 6573 0a20 2020 2075 7269 203d 2022  nges.    uri = "
+00004520: 7b7d 2f7b 7d22 2e66 6f72 6d61 7428 636f  {}/{}".format(co
+00004530: 6e73 7461 6e74 732e 494d 504f 5254 5f55  nstants.IMPORT_U
+00004540: 524c 2c20 696d 706f 7274 5f69 6429 0a20  RL, import_id). 
+00004550: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00004560: 7265 735f 636c 6965 6e74 2e70 7574 2875  res_client.put(u
+00004570: 7269 2c20 7265 7375 6c74 290a 2020 2020  ri, result).    
+00004580: 2020 2020 4c4f 472e 696e 666f 2822 496d      LOG.info("Im
+00004590: 706f 7274 6564 2063 6f6e 6669 6775 7261  ported configura
+000045a0: 7469 6f6e 2063 6861 6e67 6573 2073 7563  tion changes suc
+000045b0: 6365 7373 6675 6c6c 7920 746f 2053 4f41  cessfully to SOA
+000045c0: 5222 290a 2020 2020 6578 6365 7074 2072  R").    except r
+000045d0: 6571 7565 7374 732e 5265 7175 6573 7445  equests.RequestE
+000045e0: 7863 6570 7469 6f6e 2061 7320 696d 706f  xception as impo
+000045f0: 7274 5f65 7863 6570 7469 6f6e 3a0a 2020  rt_exception:.  
+00004600: 2020 2020 2020 7261 6973 6520 5344 4b45        raise SDKE
+00004610: 7863 6570 7469 6f6e 2872 6570 7228 696d  xception(repr(im
+00004620: 706f 7274 5f65 7863 6570 7469 6f6e 2929  port_exception))
+00004630: 0a0a 6465 6620 7265 6164 5f6c 6f63 616c  ..def read_local
+00004640: 5f65 7870 6f72 7466 696c 6528 7061 7468  _exportfile(path
+00004650: 5f6c 6f63 616c 5f65 7870 6f72 7466 696c  _local_exportfil
+00004660: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
+00004670: 5265 6164 2065 7870 6f72 7420 6672 6f6d  Read export from
+00004680: 2067 6976 656e 2070 6174 680a 2020 2020   given path.    
+00004690: 5265 7475 726e 2072 6573 2065 7870 6f72  Return res expor
+000046a0: 7420 6173 2064 6963 740a 2020 2020 2222  t as dict.    ""
+000046b0: 220a 2020 2020 2320 4765 7420 6162 736f  ".    # Get abso
+000046c0: 6c75 7465 2070 6174 680a 2020 2020 7061  lute path.    pa
+000046d0: 7468 5f6c 6f63 616c 5f65 7870 6f72 7466  th_local_exportf
+000046e0: 696c 6520 3d20 6f73 2e70 6174 682e 6162  ile = os.path.ab
+000046f0: 7370 6174 6828 7061 7468 5f6c 6f63 616c  spath(path_local
+00004700: 5f65 7870 6f72 7466 696c 6529 0a0a 2020  _exportfile)..  
+00004710: 2020 2320 5661 6c69 6461 7465 2077 6520    # Validate we 
+00004720: 6361 6e20 7265 6164 2069 740a 2020 2020  can read it.    
+00004730: 7661 6c69 6461 7465 5f66 696c 655f 7061  validate_file_pa
+00004740: 7468 7328 6f73 2e52 5f4f 4b2c 2070 6174  ths(os.R_OK, pat
+00004750: 685f 6c6f 6361 6c5f 6578 706f 7274 6669  h_local_exportfi
+00004760: 6c65 290a 0a20 2020 2023 2052 6561 6420  le)..    # Read 
+00004770: 7468 6520 6578 706f 7274 2066 696c 6520  the export file 
+00004780: 636f 6e74 656e 742e 0a20 2020 2069 6620  content..    if 
+00004790: 6973 5f7a 6970 6669 6c65 2870 6174 685f  is_zipfile(path_
+000047a0: 6c6f 6361 6c5f 6578 706f 7274 6669 6c65  local_exportfile
+000047b0: 293a 0a20 2020 2020 2020 2023 2046 696c  ):.        # Fil
+000047c0: 6520 6973 2061 207a 6970 2066 696c 6520  e is a zip file 
+000047d0: 6765 7420 756e 7a69 7070 6564 2063 6f6e  get unzipped con
+000047e0: 7465 6e74 2e0a 2020 2020 2020 2020 6578  tent..        ex
+000047f0: 706f 7274 5f63 6f6e 7465 6e74 203d 2072  port_content = r
+00004800: 6561 645f 7a69 705f 6669 6c65 2870 6174  ead_zip_file(pat
+00004810: 685f 6c6f 6361 6c5f 6578 706f 7274 6669  h_local_exportfi
+00004820: 6c65 2c20 636f 6e73 7461 6e74 732e 5245  le, constants.RE
+00004830: 535f 4558 504f 5254 5f53 5546 4649 5829  S_EXPORT_SUFFIX)
+00004840: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00004850: 2020 2023 2046 696c 6520 6973 2061 2061     # File is a a
+00004860: 7373 756d 6564 2074 6f20 6265 2061 2074  ssumed to be a t
+00004870: 6578 7420 6669 6c65 2072 6561 6420 7468  ext file read th
+00004880: 6520 6578 706f 7274 2066 696c 6520 636f  e export file co
+00004890: 6e74 656e 742e 0a20 2020 2020 2020 2065  ntent..        e
+000048a0: 7870 6f72 745f 636f 6e74 656e 7420 3d20  xport_content = 
+000048b0: 2727 2e6a 6f69 6e28 7265 6164 5f66 696c  ''.join(read_fil
+000048c0: 6528 7061 7468 5f6c 6f63 616c 5f65 7870  e(path_local_exp
+000048d0: 6f72 7466 696c 6529 290a 0a20 2020 2069  ortfile))..    i
+000048e0: 6620 6e6f 7420 6578 706f 7274 5f63 6f6e  f not export_con
+000048f0: 7465 6e74 3a0a 2020 2020 2020 2020 7261  tent:.        ra
+00004900: 6973 6520 5344 4b45 7863 6570 7469 6f6e  ise SDKException
+00004910: 2822 4661 696c 6564 2074 6f20 7265 6164  ("Failed to read
+00004920: 207b 307d 222e 666f 726d 6174 2870 6174   {0}".format(pat
+00004930: 685f 6c6f 6361 6c5f 6578 706f 7274 6669  h_local_exportfi
+00004940: 6c65 2929 0a0a 2020 2020 7265 7475 726e  le))..    return
+00004950: 206a 736f 6e2e 6c6f 6164 7328 6578 706f   json.loads(expo
+00004960: 7274 5f63 6f6e 7465 6e74 290a 0a0a 6465  rt_content)...de
+00004970: 6620 6765 745f 6f62 6a65 6374 5f61 7069  f get_object_api
+00004980: 5f6e 616d 6573 2861 7069 5f6e 616d 652c  _names(api_name,
+00004990: 206c 6973 745f 6f62 6a73 293a 0a20 2020   list_objs):.   
+000049a0: 2022 2222 0a20 2020 2052 6574 7572 6e20   """.    Return 
+000049b0: 6120 6c69 7374 206f 6620 6f62 6a65 6374  a list of object
+000049c0: 2061 7069 5f6e 616d 6573 2066 726f 6d20   api_names from 
+000049d0: 6c69 7374 5f6f 626a 730a 2020 2020 2222  list_objs.    ""
+000049e0: 220a 2020 2020 6966 206c 6973 745f 6f62  ".    if list_ob
+000049f0: 6a73 3a0a 2020 2020 2020 2020 7265 7475  js:.        retu
+00004a00: 726e 205b 6f2e 6765 7428 6170 695f 6e61  rn [o.get(api_na
+00004a10: 6d65 2920 666f 7220 6f20 696e 206c 6973  me) for o in lis
+00004a20: 745f 6f62 6a73 5d0a 2020 2020 656c 7365  t_objs].    else
+00004a30: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00004a40: 205b 5d0a 0a0a 6465 6620 6765 745f 7363   []...def get_sc
+00004a50: 7269 7074 5f69 6e66 6f28 6561 6368 5f73  ript_info(each_s
+00004a60: 6372 6970 745f 696e 5f70 6c61 7962 6f6f  cript_in_playboo
+00004a70: 6b2c 2073 6372 6970 7473 5f69 6e5f 6c6f  k, scripts_in_lo
+00004a80: 6361 7469 6f6e 2c20 7363 7269 7074 5f74  cation, script_t
+00004a90: 7970 6529 3a0a 2020 2020 2727 270a 2020  ype):.    '''.  
+00004aa0: 2020 4578 7472 6163 7473 2073 6372 6970    Extracts scrip
+00004ab0: 7420 7265 6c61 7465 6420 696e 666f 726d  t related inform
+00004ac0: 6174 696f 6e20 666f 7220 706c 6179 626f  ation for playbo
+00004ad0: 6f6b 732e 2053 6372 6970 7473 2063 616e  oks. Scripts can
+00004ae0: 2062 6520 6f66 2032 2074 7970 6573 3a20   be of 2 types: 
+00004af0: 6c6f 6361 6c20 6f72 2067 6c6f 6261 6c2e  local or global.
+00004b00: 0a20 2020 204c 6f63 616c 2073 6372 6970  .    Local scrip
+00004b10: 7473 206c 6976 6520 7769 7468 696e 2074  ts live within t
+00004b20: 6865 2070 6c61 7962 6f6f 6b20 6974 7365  he playbook itse
+00004b30: 6c66 2c20 7768 696c 6520 676c 6f62 616c  lf, while global
+00004b40: 2073 6372 6970 7473 2061 7265 2073 746f   scripts are sto
+00004b50: 7265 6420 696e 2074 6865 2067 6c6f 6261  red in the globa
+00004b60: 6c5f 6578 706f 7274 2064 6963 742e 0a0a  l_export dict...
+00004b70: 2020 2020 4e6f 7465 3a20 5468 6520 7363      Note: The sc
+00004b80: 7269 7074 7320 6172 6520 7061 7373 6564  ripts are passed
+00004b90: 2062 7920 7265 6665 7265 6e63 652e 2054   by reference. T
+00004ba0: 6865 7920 6e65 6564 206e 6f74 2062 6520  hey need not be 
+00004bb0: 7265 7475 726e 6564 2e20 5468 6579 2061  returned. They a
+00004bc0: 7265 2064 6972 6563 746c 7920 7570 6461  re directly upda
+00004bd0: 7465 642e 0a20 2020 203a 7061 7261 6d20  ted..    :param 
+00004be0: 6561 6368 5f73 6372 6970 745f 696e 5f70  each_script_in_p
+00004bf0: 6c61 7962 6f6f 6b3a 2049 6e64 6976 6964  laybook: Individ
+00004c00: 7561 6c20 7363 7269 7074 7320 666f 756e  ual scripts foun
+00004c10: 6420 696e 2074 6865 2070 6c61 7962 6f6f  d in the playboo
+00004c20: 6b0a 2020 2020 3a74 7970 6520 6561 6368  k.    :type each
+00004c30: 5f73 6372 6970 745f 696e 5f70 6c61 7962  _script_in_playb
+00004c40: 6f6f 6b3a 2064 6963 740a 2020 2020 3a70  ook: dict.    :p
+00004c50: 6172 616d 2073 6372 6970 7473 5f69 6e5f  aram scripts_in_
+00004c60: 6c6f 6361 7469 6f6e 3a20 416c 6c20 7363  location: All sc
+00004c70: 7269 7074 7320 696e 2074 6865 206c 6f63  ripts in the loc
+00004c80: 6174 696f 6e20 2867 6c6f 6261 6c20 6f72  ation (global or
+00004c90: 206c 6f63 616c 292e 2047 6c6f 6261 6c20   local). Global 
+00004ca0: 7363 7269 7074 7320 6172 6520 7075 6c6c  scripts are pull
+00004cb0: 6564 2064 6972 6563 746c 7920 6672 6f6d  ed directly from
+00004cc0: 2074 6865 2067 6c6f 6261 6c5f 6578 706f   the global_expo
+00004cd0: 7274 2064 6963 742e 204c 6f63 616c 2073  rt dict. Local s
+00004ce0: 6372 6970 7473 2061 7265 2070 756c 6c65  cripts are pulle
+00004cf0: 6420 6672 6f6d 2074 6865 2070 6c61 7962  d from the playb
+00004d00: 6f6f 6b0a 2020 2020 3a74 7970 6520 7363  ook.    :type sc
+00004d10: 7269 7074 735f 696e 5f6c 6f63 6174 696f  ripts_in_locatio
+00004d20: 6e3a 206c 6973 740a 2020 2020 3a70 6172  n: list.    :par
+00004d30: 616d 2073 6372 6970 745f 7479 7065 3a20  am script_type: 
+00004d40: 5468 6520 7479 7065 206f 6620 7363 7269  The type of scri
+00004d50: 7074 2028 676c 6f62 616c 206f 7220 6c6f  pt (global or lo
+00004d60: 6361 6c29 0a20 2020 203a 7479 7065 2073  cal).    :type s
+00004d70: 6372 6970 745f 7479 7065 3a20 7374 720a  cript_type: str.
+00004d80: 2020 2020 2727 270a 2020 2020 666f 756e      '''.    foun
+00004d90: 645f 7363 7269 7074 203d 2046 616c 7365  d_script = False
+00004da0: 0a20 2020 2066 6f72 2073 6320 696e 2073  .    for sc in s
+00004db0: 6372 6970 7473 5f69 6e5f 6c6f 6361 7469  cripts_in_locati
+00004dc0: 6f6e 3a0a 2020 2020 2020 2020 6966 2065  on:.        if e
+00004dd0: 6163 685f 7363 7269 7074 5f69 6e5f 706c  ach_script_in_pl
+00004de0: 6179 626f 6f6b 2e67 6574 2822 7575 6964  aybook.get("uuid
+00004df0: 222c 2022 7575 6964 5f6e 6f74 5f66 6f75  ", "uuid_not_fou
+00004e00: 6e64 5f70 6222 2920 3d3d 2073 632e 6765  nd_pb") == sc.ge
+00004e10: 7428 2275 7569 6422 2c20 2275 7569 645f  t("uuid", "uuid_
+00004e20: 6e6f 745f 666f 756e 645f 7363 2229 3a0a  not_found_sc"):.
+00004e30: 2020 2020 2020 2020 2020 2020 6561 6368              each
+00004e40: 5f73 6372 6970 745f 696e 5f70 6c61 7962  _script_in_playb
+00004e50: 6f6f 6b5b 226e 616d 6522 5d20 3d20 7363  ook["name"] = sc
+00004e60: 2e67 6574 2822 6e61 6d65 2229 0a20 2020  .get("name").   
+00004e70: 2020 2020 2020 2020 2065 6163 685f 7363           each_sc
+00004e80: 7269 7074 5f69 6e5f 706c 6179 626f 6f6b  ript_in_playbook
+00004e90: 5b22 7363 7269 7074 5f74 7970 6522 5d20  ["script_type"] 
+00004ea0: 3d20 7363 7269 7074 5f74 7970 650a 2020  = script_type.  
+00004eb0: 2020 2020 2020 2020 2020 6561 6368 5f73            each_s
+00004ec0: 6372 6970 745f 696e 5f70 6c61 7962 6f6f  cript_in_playboo
+00004ed0: 6b5b 2264 6573 6372 6970 7469 6f6e 225d  k["description"]
+00004ee0: 203d 2073 632e 6765 7428 2264 6573 6372   = sc.get("descr
+00004ef0: 6970 7469 6f6e 2229 0a20 2020 2020 2020  iption").       
+00004f00: 2020 2020 2065 6163 685f 7363 7269 7074       each_script
+00004f10: 5f69 6e5f 706c 6179 626f 6f6b 5b22 6f62  _in_playbook["ob
+00004f20: 6a65 6374 5f74 7970 6522 5d20 3d20 7363  ject_type"] = sc
+00004f30: 2e67 6574 2822 6f62 6a65 6374 5f74 7970  .get("object_typ
+00004f40: 6522 290a 2020 2020 2020 2020 2020 2020  e").            
+00004f50: 6561 6368 5f73 6372 6970 745f 696e 5f70  each_script_in_p
+00004f60: 6c61 7962 6f6f 6b5b 2273 6372 6970 745f  laybook["script_
+00004f70: 7465 7874 225d 203d 2073 632e 6765 7428  text"] = sc.get(
+00004f80: 2273 6372 6970 745f 7465 7874 222c 2022  "script_text", "
+00004f90: 2229 0a20 2020 2020 2020 2020 2020 2066  ").            f
+00004fa0: 6f75 6e64 5f73 6372 6970 7420 3d20 5472  ound_script = Tr
+00004fb0: 7565 0a20 2020 2020 2020 2020 2020 2062  ue.            b
+00004fc0: 7265 616b 0a20 2020 2072 6574 7572 6e20  reak.    return 
+00004fd0: 666f 756e 645f 7363 7269 7074 0a0a 0a64  found_script...d
+00004fe0: 6566 2067 6574 5f6f 626a 5f66 726f 6d5f  ef get_obj_from_
+00004ff0: 6c69 7374 2869 6465 6e74 6966 6572 2c20  list(identifer, 
+00005000: 6f62 6a5f 6c69 7374 2c20 636f 6e64 6974  obj_list, condit
+00005010: 696f 6e3d 6c61 6d62 6461 206f 3a20 5472  ion=lambda o: Tr
+00005020: 7565 293a 0a20 2020 2022 2222 0a20 2020  ue):.    """.   
+00005030: 2052 6574 7572 6e20 6120 6469 6374 2074   Return a dict t
+00005040: 6865 206e 616d 6520 6f66 2074 6865 206f  he name of the o
+00005050: 626a 6563 7420 6173 2069 7473 204b 6579  bject as its Key
+00005060: 0a20 2020 2065 2e67 2e20 7b0a 2020 2020  .    e.g. {.    
+00005070: 2020 2020 2266 6e5f 6d6f 636b 5f66 756e      "fn_mock_fun
+00005080: 6374 696f 6e5f 3122 3a20 7b2e 2e2e 7d2c  ction_1": {...},
+00005090: 0a20 2020 2020 2020 2022 666e 5f6d 6f63  .        "fn_moc
+000050a0: 6b5f 6675 6e63 7469 6f6e 5f32 223a 207b  k_function_2": {
+000050b0: 2e2e 2e7d 0a20 2020 207d 0a20 2020 203a  ...}.    }.    :
+000050c0: 7061 7261 6d20 6964 656e 7469 6665 723a  param identifer:
+000050d0: 2054 6865 2061 7474 7269 6275 7465 206f   The attribute o
+000050e0: 6620 7468 6520 6f62 6a65 6374 2077 6520  f the object we 
+000050f0: 7573 6520 746f 2069 6465 6e74 6966 7920  use to identify 
+00005100: 6974 2065 2e67 2e20 2270 726f 6772 616d  it e.g. "program
+00005110: 6d61 7469 635f 6e61 6d65 220a 2020 2020  matic_name".    
+00005120: 3a74 7970 6520 6964 656e 7469 6665 723a  :type identifer:
+00005130: 2073 7472 0a20 2020 203a 7061 7261 6d20   str.    :param 
+00005140: 6f62 6a5f 6c69 7374 3a20 4c69 7374 206f  obj_list: List o
+00005150: 6620 5265 7369 6c69 656e 7420 4f62 6a65  f Resilient Obje
+00005160: 6374 730a 2020 2020 3a74 7970 6520 6f62  cts.    :type ob
+00005170: 6a5f 6c69 7374 3a20 4c69 7374 0a20 2020  j_list: List.   
+00005180: 203a 7061 7261 6d20 636f 6e64 6974 696f   :param conditio
+00005190: 6e3a 2041 206c 616d 6264 6120 6675 6e63  n: A lambda func
+000051a0: 7469 6f6e 2074 6f20 6576 616c 7561 7465  tion to evaluate
+000051b0: 2065 6163 6820 6f62 6a65 6374 0a20 2020   each object.   
+000051c0: 203a 7479 7065 2063 6f6e 6469 7469 6f6e   :type condition
+000051d0: 3a20 6675 6e63 7469 6f6e 0a20 2020 203a  : function.    :
+000051e0: 7265 7475 726e 3a20 4469 6374 696f 6e61  return: Dictiona
+000051f0: 7279 206f 6620 6561 6368 2066 6f75 6e64  ry of each found
+00005200: 206f 626a 6563 7420 6c69 6b65 2074 6865   object like the
+00005210: 2061 626f 7665 2065 7861 6d70 6c65 0a20   above example. 
+00005220: 2020 203a 7274 7970 653a 2044 6963 740a     :rtype: Dict.
+00005230: 2020 2020 2222 220a 2020 2020 6966 206f      """.    if o
+00005240: 626a 5f6c 6973 743a 0a20 2020 2020 2020  bj_list:.       
+00005250: 2072 6574 7572 6e20 6469 6374 2828 6f5b   return dict((o[
+00005260: 6964 656e 7469 6665 725d 2e73 7472 6970  identifer].strip
+00005270: 2829 2c20 6f29 2066 6f72 206f 2069 6e20  (), o) for o in 
+00005280: 6f62 6a5f 6c69 7374 2069 6620 636f 6e64  obj_list if cond
+00005290: 6974 696f 6e28 6f29 290a 2020 2020 7265  ition(o)).    re
+000052a0: 7475 726e 207b 7d0a 0a0a 6465 6620 6765  turn {}...def ge
+000052b0: 745f 7265 735f 6f62 6a28 6f62 6a5f 6e61  t_res_obj(obj_na
+000052c0: 6d65 2c20 6f62 6a5f 6964 656e 7469 6665  me, obj_identife
+000052d0: 722c 206f 626a 5f64 6973 706c 6179 5f6e  r, obj_display_n
+000052e0: 616d 652c 2077 616e 7465 645f 6c69 7374  ame, wanted_list
+000052f0: 2c20 6578 706f 7274 2c20 636f 6e64 6974  , export, condit
+00005300: 696f 6e3d 6c61 6d62 6461 206f 3a20 5472  ion=lambda o: Tr
+00005310: 7565 2c20 696e 636c 7564 655f 6170 695f  ue, include_api_
+00005320: 6e61 6d65 3d54 7275 6529 3a0a 2020 2020  name=True):.    
+00005330: 2222 220a 2020 2020 5265 7475 726e 2061  """.    Return a
+00005340: 204c 6973 7420 6f66 2052 6573 696c 6965   List of Resilie
+00005350: 6e74 204f 626a 6563 7473 2074 6861 7420  nt Objects that 
+00005360: 6172 6520 696e 2074 6865 2027 7761 6e74  are in the 'want
+00005370: 6564 5f6c 6973 7427 2061 6e64 206d 6565  ed_list' and mee
+00005380: 7420 7468 6520 2763 6f6e 6469 7469 6f6e  t the 'condition
+00005390: 270a 0a20 2020 203a 7061 7261 6d20 6f62  '..    :param ob
+000053a0: 6a5f 6e61 6d65 3a20 4e61 6d65 206f 6620  j_name: Name of 
+000053b0: 7468 6520 4f62 6a65 6374 206c 6973 7420  the Object list 
+000053c0: 696e 2074 6865 2045 7870 6f72 740a 2020  in the Export.  
+000053d0: 2020 3a74 7970 6520 6f62 6a5f 6e61 6d65    :type obj_name
+000053e0: 3a20 7374 720a 2020 2020 3a70 6172 616d  : str.    :param
+000053f0: 206f 626a 5f69 6465 6e74 6966 6572 3a20   obj_identifer: 
+00005400: 5468 6520 6174 7472 6962 7574 6520 6f66  The attribute of
+00005410: 2074 6865 206f 626a 6563 7420 7765 2075   the object we u
+00005420: 7365 2074 6f20 6964 656e 7469 6679 2069  se to identify i
+00005430: 7420 652e 672e 2022 7072 6f67 7261 6d6d  t e.g. "programm
+00005440: 6174 6963 5f6e 616d 6522 0a20 2020 203a  atic_name".    :
+00005450: 7479 7065 206f 626a 5f69 6465 6e74 6966  type obj_identif
+00005460: 6572 3a20 7374 720a 2020 2020 3a70 6172  er: str.    :par
+00005470: 616d 206f 626a 5f64 6973 706c 6179 5f6e  am obj_display_n
+00005480: 616d 653a 2054 6865 2044 6973 706c 6179  ame: The Display
+00005490: 204e 616d 6520 7765 2077 616e 7420 746f   Name we want to
+000054a0: 2075 7365 2066 6f72 2074 6869 7320 6f62   use for this ob
+000054b0: 6a65 6374 2069 6e20 6f75 7220 4c6f 6773  ject in our Logs
+000054c0: 0a20 2020 203a 7479 7065 206f 626a 5f64  .    :type obj_d
+000054d0: 6973 706c 6179 5f6e 616d 653a 2073 7472  isplay_name: str
+000054e0: 0a20 2020 203a 7061 7261 6d20 7761 6e74  .    :param want
+000054f0: 6564 5f6c 6973 743a 204c 6973 7420 6f66  ed_list: List of
+00005500: 2069 6465 6e74 6966 6572 7320 666f 7220   identifers for 
+00005510: 6f62 6a65 6374 7320 7765 2077 616e 7420  objects we want 
+00005520: 746f 2072 6574 7572 6e0a 2020 2020 3a74  to return.    :t
+00005530: 7970 6520 7761 6e74 6564 5f6c 6973 743a  ype wanted_list:
+00005540: 204c 6973 7420 6f66 2073 7472 0a20 2020   List of str.   
+00005550: 203a 7061 7261 6d20 6578 706f 7274 3a20   :param export: 
+00005560: 5468 6520 7265 7375 6c74 206f 6620 6361  The result of ca
+00005570: 6c6c 696e 6720 6765 745f 6c61 7465 7374  lling get_latest
+00005580: 5f6f 7267 5f65 7870 6f72 7428 290a 2020  _org_export().  
+00005590: 2020 3a74 7970 6520 6578 706f 7274 3a20    :type export: 
+000055a0: 4469 6374 0a20 2020 203a 7061 7261 6d20  Dict.    :param 
+000055b0: 636f 6e64 6974 696f 6e3a 2041 206c 616d  condition: A lam
+000055c0: 6264 6120 6675 6e63 7469 6f6e 2074 6f20  bda function to 
+000055d0: 6576 616c 7561 7465 2065 6163 6820 6f62  evaluate each ob
+000055e0: 6a65 6374 0a20 2020 203a 7479 7065 2063  ject.    :type c
+000055f0: 6f6e 6469 7469 6f6e 3a20 6675 6e63 7469  ondition: functi
+00005600: 6f6e 0a20 2020 203a 7061 7261 6d20 696e  on.    :param in
+00005610: 636c 7564 655f 6170 695f 6e61 6d65 3a20  clude_api_name: 
+00005620: 5768 6574 6865 7220 6f72 206e 6f74 2074  Whether or not t
+00005630: 6f20 7265 7475 726e 2074 6865 206f 626a  o return the obj
+00005640: 6563 7473 2041 5049 206e 616d 6520 6173  ects API name as
+00005650: 2061 2066 6965 6c64 2e0a 2020 2020 3a74   a field..    :t
+00005660: 7970 6520 696e 636c 7564 655f 6170 695f  ype include_api_
+00005670: 6e61 6d65 3a20 626f 6f6c 0a20 2020 203a  name: bool.    :
+00005680: 7265 7475 726e 3a20 4c69 7374 206f 6620  return: List of 
+00005690: 5265 7369 6c69 656e 7420 4f62 6a65 6374  Resilient Object
+000056a0: 730a 2020 2020 3a72 7479 7065 3a20 4c69  s.    :rtype: Li
+000056b0: 7374 0a20 2020 2022 2222 0a20 2020 2072  st.    """.    r
+000056c0: 6574 7572 6e5f 6c69 7374 203d 205b 5d0a  eturn_list = [].
+000056d0: 0a20 2020 2023 2054 6869 7320 6c6f 6f70  .    # This loop
+000056e0: 7320 7761 6e74 6564 5f6c 6973 740a 2020  s wanted_list.  
+000056f0: 2020 2320 4966 2061 6e20 656e 7472 7920    # If an entry 
+00005700: 6973 2064 6963 7420 666f 726d 6174 2c20  is dict format, 
+00005710: 6974 2077 696c 6c20 6861 7665 2076 616c  it will have val
+00005720: 7565 2061 6e64 2069 6465 6e74 6966 6965  ue and identifie
+00005730: 7220 6174 7472 6962 7574 6573 0a20 2020  r attributes.   
+00005740: 2023 2057 6520 7573 6520 7468 6f73 6520   # We use those 
+00005750: 746f 2067 6574 2074 6865 2027 7072 6f67  to get the 'prog
+00005760: 7261 6d6d 6174 6963 5f6e 616d 6527 206f  rammatic_name' o
+00005770: 7220 2761 7069 5f6e 616d 6527 0a20 2020  r 'api_name'.   
+00005780: 2023 2045 7861 6d70 6c65 3a20 466f 7220   # Example: For 
+00005790: 6d65 7373 6167 655f 6465 7374 696e 6174  message_destinat
+000057a0: 696f 6e73 2072 6566 6572 656e 6365 6420  ions referenced 
+000057b0: 696e 2061 6374 696f 6e73 2c20 7468 6579  in actions, they
+000057c0: 2061 7265 2072 6566 6572 656e 6365 6420   are referenced 
+000057d0: 6279 2064 6973 706c 6179 206e 616d 650a  by display name.
+000057e0: 2020 2020 2320 5468 6973 2061 6c6c 6f77      # This allow
+000057f0: 7320 7573 2074 6f20 6765 7420 7468 6569  s us to get thei
+00005800: 7220 2770 726f 6772 616d 6d61 7469 635f  r 'programmatic_
+00005810: 6e61 6d65 270a 2020 2020 666f 7220 696e  name'.    for in
+00005820: 6465 782c 206f 626a 2069 6e20 656e 756d  dex, obj in enum
+00005830: 6572 6174 6528 7761 6e74 6564 5f6c 6973  erate(wanted_lis
+00005840: 7429 3a0a 2020 2020 2020 2020 6966 2069  t):.        if i
+00005850: 7369 6e73 7461 6e63 6528 6f62 6a2c 2064  sinstance(obj, d
+00005860: 6963 7429 3a0a 2020 2020 2020 2020 2020  ict):.          
+00005870: 2020 7465 6d70 5f6f 626a 5f69 6465 6e74    temp_obj_ident
+00005880: 6966 6965 7220 3d20 6f62 6a2e 6765 7428  ifier = obj.get(
+00005890: 2269 6465 6e74 6966 6965 7222 2c20 2222  "identifier", ""
+000058a0: 290a 2020 2020 2020 2020 2020 2020 6f62  ).            ob
+000058b0: 6a5f 7661 6c75 6520 3d20 6f62 6a2e 6765  j_value = obj.ge
+000058c0: 7428 2276 616c 7565 222c 2022 2229 0a20  t("value", ""). 
+000058d0: 2020 2020 2020 2020 2020 2066 756c 6c5f             full_
+000058e0: 6f62 6a20 3d20 6765 745f 6f62 6a5f 6672  obj = get_obj_fr
+000058f0: 6f6d 5f6c 6973 7428 7465 6d70 5f6f 626a  om_list(temp_obj
+00005900: 5f69 6465 6e74 6966 6965 722c 0a20 2020  _identifier,.   
+00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005930: 2020 2020 2020 6578 706f 7274 2e67 6574        export.get
+00005940: 286f 626a 5f6e 616d 652c 2022 2229 2c0a  (obj_name, ""),.
+00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005970: 2020 2020 2020 2020 206c 616d 6264 6120           lambda 
+00005980: 7761 6e74 6564 5f6f 626a 2c20 693d 7465  wanted_obj, i=te
+00005990: 6d70 5f6f 626a 5f69 6465 6e74 6966 6965  mp_obj_identifie
+000059a0: 722c 2076 3d6f 626a 5f76 616c 7565 3a20  r, v=obj_value: 
+000059b0: 5472 7565 2069 6620 7761 6e74 6564 5f6f  True if wanted_o
+000059c0: 626a 2e67 6574 2869 2920 3d3d 2076 2065  bj.get(i) == v e
+000059d0: 6c73 6520 4661 6c73 6529 0a0a 2020 2020  lse False)..    
+000059e0: 2020 2020 2020 2020 7761 6e74 6564 5f6c          wanted_l
+000059f0: 6973 745b 696e 6465 785d 203d 2066 756c  ist[index] = ful
+00005a00: 6c5f 6f62 6a2e 6765 7428 6f62 6a5f 7661  l_obj.get(obj_va
+00005a10: 6c75 6529 2e67 6574 286f 626a 5f69 6465  lue).get(obj_ide
+00005a20: 6e74 6966 6572 290a 0a20 2020 2069 6620  ntifer)..    if 
+00005a30: 7761 6e74 6564 5f6c 6973 743a 0a20 2020  wanted_list:.   
+00005a40: 2020 2020 2065 785f 6f62 6a20 3d20 6765       ex_obj = ge
+00005a50: 745f 6f62 6a5f 6672 6f6d 5f6c 6973 7428  t_obj_from_list(
+00005a60: 6f62 6a5f 6964 656e 7469 6665 722c 2065  obj_identifer, e
+00005a70: 7870 6f72 742e 6765 7428 6f62 6a5f 6e61  xport.get(obj_na
+00005a80: 6d65 2c20 2222 292c 2063 6f6e 6469 7469  me, ""), conditi
+00005a90: 6f6e 290a 0a20 2020 2020 2020 2066 6f72  on)..        for
+00005aa0: 206f 2069 6e20 7365 7428 7761 6e74 6564   o in set(wanted
+00005ab0: 5f6c 6973 7429 3a0a 2020 2020 2020 2020  _list):.        
+00005ac0: 2020 2020 7374 7269 7070 6564 5f6f 203d      stripped_o =
+00005ad0: 206f 2e73 7472 6970 2829 0a20 2020 2020   o.strip().     
+00005ae0: 2020 2020 2020 2069 6620 7374 7269 7070         if stripp
+00005af0: 6564 5f6f 206e 6f74 2069 6e20 6578 5f6f  ed_o not in ex_o
+00005b00: 626a 3a0a 2020 2020 2020 2020 2020 2020  bj:.            
+00005b10: 2020 2020 7261 6973 6520 5344 4b45 7863      raise SDKExc
+00005b20: 6570 7469 6f6e 2875 227b 307d 3a20 277b  eption(u"{0}: '{
+00005b30: 317d 2720 6e6f 7420 666f 756e 6420 696e  1}' not found in
+00005b40: 2074 6869 7320 6578 706f 7274 2e5c 6e7b   this export.\n{
+00005b50: 307d 7320 4176 6169 6c61 626c 653a 5c6e  0}s Available:\n
+00005b60: 5c74 7b32 7d22 2e66 6f72 6d61 7428 6f62  \t{2}".format(ob
+00005b70: 6a5f 6469 7370 6c61 795f 6e61 6d65 2c20  j_display_name, 
+00005b80: 7374 7269 7070 6564 5f6f 2c20 225c 6e5c  stripped_o, "\n\
+00005b90: 7422 2e6a 6f69 6e28 6578 5f6f 626a 2e6b  t".join(ex_obj.k
+00005ba0: 6579 7328 2929 2929 0a0a 2020 2020 2020  eys())))..      
+00005bb0: 2020 2020 2020 2320 4164 6420 785f 6170        # Add x_ap
+00005bc0: 695f 6e61 6d65 2074 6f20 6561 6368 206f  i_name to each o
+00005bd0: 626a 6563 742c 2073 6f20 7765 2063 616e  bject, so we can
+00005be0: 2065 6173 696c 7920 7265 6665 7265 6e63   easily referenc
+00005bf0: 652e 2054 6869 7320 6176 6f69 6473 206e  e. This avoids n
+00005c00: 6565 6469 6e67 2074 6f20 6b6e 6f77 2069  eeding to know i
+00005c10: 660a 2020 2020 2020 2020 2020 2020 2320  f.            # 
+00005c20: 6f62 6a20 6174 7472 6962 7574 6520 6973  obj attribute is
+00005c30: 2027 6e61 6d65 2720 6f72 2027 7072 6f67   'name' or 'prog
+00005c40: 7261 6d6d 6174 6963 5f6e 616d 6527 2065  rammatic_name' e
+00005c50: 7463 2e0a 2020 2020 2020 2020 2020 2020  tc..            
+00005c60: 6f62 6a20 3d20 6578 5f6f 626a 2e67 6574  obj = ex_obj.get
+00005c70: 2873 7472 6970 7065 645f 6f29 0a20 2020  (stripped_o).   
+00005c80: 2020 2020 2020 2020 2069 6620 696e 636c           if incl
+00005c90: 7564 655f 6170 695f 6e61 6d65 3a0a 2020  ude_api_name:.  
+00005ca0: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
+00005cb0: 6a5b 2278 5f61 7069 5f6e 616d 6522 5d20  j["x_api_name"] 
+00005cc0: 3d20 6f62 6a5b 6f62 6a5f 6964 656e 7469  = obj[obj_identi
+00005cd0: 6665 725d 0a20 2020 2020 2020 2020 2020  fer].           
+00005ce0: 2072 6574 7572 6e5f 6c69 7374 2e61 7070   return_list.app
+00005cf0: 656e 6428 6f62 6a29 0a0a 2020 2020 7265  end(obj)..    re
+00005d00: 7475 726e 2072 6574 7572 6e5f 6c69 7374  turn return_list
+00005d10: 0a0a 0a64 6566 2067 6574 5f66 726f 6d5f  ...def get_from_
+00005d20: 6578 706f 7274 2865 7870 6f72 742c 0a20  export(export,. 
+00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d40: 2020 206d 6573 7361 6765 5f64 6573 7469     message_desti
+00005d50: 6e61 7469 6f6e 733d 5b5d 2c0a 2020 2020  nations=[],.    
+00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d70: 6675 6e63 7469 6f6e 733d 5b5d 2c0a 2020  functions=[],.  
+00005d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d90: 2020 776f 726b 666c 6f77 733d 5b5d 2c0a    workflows=[],.
+00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005db0: 2020 2020 7275 6c65 733d 5b5d 2c0a 2020      rules=[],.  
+00005dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005dd0: 2020 6669 656c 6473 3d5b 5d2c 0a20 2020    fields=[],.   
 00005de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005df0: 696e 6369 6465 6e74 5f74 7970 6573 3d5b  incident_types=[
-00005e00: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00005e10: 2020 2020 2020 2064 6174 6174 6162 6c65         datatable
-00005e20: 733d 5b5d 2c0a 2020 2020 2020 2020 2020  s=[],.          
-00005e30: 2020 2020 2020 2020 2020 7461 736b 733d            tasks=
-00005e40: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
-00005e50: 2020 2020 2020 2020 7363 7269 7074 733d          scripts=
-00005e60: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
-00005e70: 2020 2020 2020 2020 706c 6179 626f 6f6b          playbook
-00005e80: 733d 5b5d 2c0a 2020 2020 2020 2020 2020  s=[],.          
-00005e90: 2020 2020 2020 2020 2020 6170 7073 3d5b            apps=[
-00005ea0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00005eb0: 2020 2020 2020 2067 6574 5f72 656c 6174         get_relat
-00005ec0: 6564 5f6f 626a 6563 7473 3d54 7275 6529  ed_objects=True)
-00005ed0: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-00005ee0: 7475 726e 2061 2044 6963 7469 6f6e 6172  turn a Dictionar
-00005ef0: 7920 6f66 2052 6573 696c 6965 6e74 204f  y of Resilient O
-00005f00: 626a 6563 7473 2074 6861 7420 6172 6520  bjects that are 
-00005f10: 666f 756e 6420 696e 2074 6865 2045 7870  found in the Exp
-00005f20: 6f72 742e 0a20 2020 2054 6865 2070 6172  ort..    The par
-00005f30: 616d 6574 6572 7320 6172 6520 4c69 7374  ameters are List
-00005f40: 7320 6f66 2074 6865 204f 626a 6563 7473  s of the Objects
-00005f50: 2079 6f75 2077 616e 740a 0a20 2020 203a   you want..    :
-00005f60: 7061 7261 6d20 6578 706f 7274 3a20 5468  param export: Th
-00005f70: 6520 7265 7375 6c74 206f 6620 6361 6c6c  e result of call
-00005f80: 696e 6720 6765 745f 6c61 7465 7374 5f6f  ing get_latest_o
-00005f90: 7267 5f65 7870 6f72 7428 290a 2020 2020  rg_export().    
-00005fa0: 3a74 7970 6520 6578 706f 7274 3a20 4469  :type export: Di
-00005fb0: 6374 0a20 2020 203a 7061 7261 6d20 6d65  ct.    :param me
-00005fc0: 7373 6167 655f 6465 7374 696e 6174 696f  ssage_destinatio
-00005fd0: 6e73 3a20 4c69 7374 206f 6620 4d65 7373  ns: List of Mess
-00005fe0: 6167 6520 4465 7374 696e 6174 696f 6e20  age Destination 
-00005ff0: 4150 4920 4e61 6d65 730a 2020 2020 3a70  API Names.    :p
-00006000: 6172 616d 2066 756e 6374 696f 6e73 3a20  aram functions: 
-00006010: 4c69 7374 206f 6620 4675 6e63 7469 6f6e  List of Function
-00006020: 2041 5049 204e 616d 6573 0a20 2020 203a   API Names.    :
-00006030: 7061 7261 6d20 776f 726b 666c 6f77 733a  param workflows:
-00006040: 204c 6973 7420 6f66 2057 6f72 6b66 6c6f   List of Workflo
-00006050: 7720 4150 4920 4e61 6d65 730a 2020 2020  w API Names.    
-00006060: 3a70 6172 616d 2072 756c 6573 3a20 4c69  :param rules: Li
-00006070: 7374 206f 6620 5275 6c65 2044 6973 706c  st of Rule Displ
-00006080: 6179 204e 616d 6573 0a20 2020 203a 7061  ay Names.    :pa
-00006090: 7261 6d20 6669 656c 6473 3a20 4c69 7374  ram fields: List
-000060a0: 206f 6620 4669 656c 6420 4150 4920 4e61   of Field API Na
-000060b0: 6d65 730a 2020 2020 3a70 6172 616d 2061  mes.    :param a
-000060c0: 7274 6966 6163 745f 7479 7065 733a 204c  rtifact_types: L
-000060d0: 6973 7420 6f66 2043 7573 746f 6d20 4172  ist of Custom Ar
-000060e0: 7469 6661 6374 2054 7970 6520 4150 4920  tifact Type API 
-000060f0: 4e61 6d65 730a 2020 2020 3a70 6172 616d  Names.    :param
-00006100: 2069 6e63 6964 656e 745f 7479 7065 733a   incident_types:
-00006110: 204c 6973 7420 6f66 2043 7573 746f 6d20   List of Custom 
-00006120: 496e 6369 6465 6e74 2054 7970 6520 4150  Incident Type AP
-00006130: 4920 4e61 6d65 730a 2020 2020 3a70 6172  I Names.    :par
-00006140: 616d 2064 6174 6174 6162 6c65 733a 204c  am datatables: L
-00006150: 6973 7420 6f66 2044 6174 6120 5461 626c  ist of Data Tabl
-00006160: 6520 4150 4920 4e61 6d65 730a 2020 2020  e API Names.    
-00006170: 3a70 6172 616d 2074 6173 6b73 3a20 4c69  :param tasks: Li
-00006180: 7374 206f 6620 4375 7374 6f6d 2054 6173  st of Custom Tas
-00006190: 6b20 4150 4920 4e61 6d65 730a 2020 2020  k API Names.    
-000061a0: 3a70 6172 616d 2073 6372 6970 7473 3a20  :param scripts: 
-000061b0: 4c69 7374 206f 6620 5363 7269 7074 2044  List of Script D
-000061c0: 6973 706c 6179 204e 616d 6573 0a20 2020  isplay Names.   
-000061d0: 203a 7061 7261 6d20 706c 6179 626f 6f6b   :param playbook
-000061e0: 733a 204c 6973 7420 6f66 2050 6c61 7962  s: List of Playb
-000061f0: 6f6f 6b20 4150 4920 4e61 6d65 730a 2020  ook API Names.  
-00006200: 2020 3a70 6172 616d 2067 6574 5f72 656c    :param get_rel
-00006210: 6174 6564 5f6f 626a 6563 7473 3a20 5768  ated_objects: Wh
-00006220: 6574 6865 7220 6f72 206e 6f74 2074 6f20  ether or not to 
-00006230: 6875 6e74 2066 6f72 2072 656c 6174 6564  hunt for related
-00006240: 2061 6374 696f 6e20 6f62 6a65 6374 732c   action objects,
-00006250: 2064 6566 6175 6c74 7320 746f 2054 7275   defaults to Tru
-00006260: 650a 2020 2020 3a72 6574 7572 6e3a 2052  e.    :return: R
-00006270: 6574 7572 6e20 6120 4469 6374 696f 6e61  eturn a Dictiona
-00006280: 7279 206f 6620 5265 7369 6c69 656e 7420  ry of Resilient 
-00006290: 4f62 6a65 6374 730a 2020 2020 3a72 7479  Objects.    :rty
-000062a0: 7065 3a20 4469 6374 0a20 2020 2022 2222  pe: Dict.    """
-000062b0: 0a0a 2020 2020 2320 4372 6561 7465 2061  ..    # Create a
-000062c0: 2064 6565 7063 6f70 7920 6f66 2074 6865   deepcopy of the
-000062d0: 2065 7870 6f72 742c 2073 6f20 7765 2064   export, so we d
-000062e0: 6f6e 2774 206f 7665 7277 7269 7465 2074  on't overwrite t
-000062f0: 6865 206f 7269 6769 6e61 6c0a 2020 2020  he original.    
-00006300: 6578 706f 7274 203d 2063 6f70 792e 6465  export = copy.de
-00006310: 6570 636f 7079 2865 7870 6f72 7429 0a0a  epcopy(export)..
-00006320: 2020 2020 2320 5365 7420 7061 7261 6d61      # Set parama
-00006330: 7465 7273 2074 6f20 4c69 7374 7320 6966  ters to Lists if
-00006340: 2066 616c 7379 0a20 2020 206d 6573 7361   falsy.    messa
-00006350: 6765 5f64 6573 7469 6e61 7469 6f6e 7320  ge_destinations 
-00006360: 3d20 6d65 7373 6167 655f 6465 7374 696e  = message_destin
-00006370: 6174 696f 6e73 2069 6620 6d65 7373 6167  ations if messag
-00006380: 655f 6465 7374 696e 6174 696f 6e73 2065  e_destinations e
-00006390: 6c73 6520 5b5d 0a20 2020 2066 756e 6374  lse [].    funct
-000063a0: 696f 6e73 203d 2066 756e 6374 696f 6e73  ions = functions
-000063b0: 2069 6620 6675 6e63 7469 6f6e 7320 656c   if functions el
-000063c0: 7365 205b 5d0a 2020 2020 776f 726b 666c  se [].    workfl
-000063d0: 6f77 7320 3d20 776f 726b 666c 6f77 7320  ows = workflows 
-000063e0: 6966 2077 6f72 6b66 6c6f 7773 2065 6c73  if workflows els
-000063f0: 6520 5b5d 0a20 2020 2072 756c 6573 203d  e [].    rules =
-00006400: 2072 756c 6573 2069 6620 7275 6c65 7320   rules if rules 
-00006410: 656c 7365 205b 5d0a 2020 2020 6669 656c  else [].    fiel
-00006420: 6473 203d 2066 6965 6c64 7320 6966 2066  ds = fields if f
-00006430: 6965 6c64 7320 656c 7365 205b 5d0a 2020  ields else [].  
-00006440: 2020 6172 7469 6661 6374 5f74 7970 6573    artifact_types
-00006450: 203d 2061 7274 6966 6163 745f 7479 7065   = artifact_type
-00006460: 7320 6966 2061 7274 6966 6163 745f 7479  s if artifact_ty
-00006470: 7065 7320 656c 7365 205b 5d0a 2020 2020  pes else [].    
-00006480: 696e 6369 6465 6e74 5f74 7970 6573 203d  incident_types =
-00006490: 2069 6e63 6964 656e 745f 7479 7065 7320   incident_types 
-000064a0: 6966 2069 6e63 6964 656e 745f 7479 7065  if incident_type
-000064b0: 7320 656c 7365 205b 5d0a 2020 2020 6461  s else [].    da
-000064c0: 7461 7461 626c 6573 203d 2064 6174 6174  tatables = datat
-000064d0: 6162 6c65 7320 6966 2064 6174 6174 6162  ables if datatab
-000064e0: 6c65 7320 656c 7365 205b 5d0a 2020 2020  les else [].    
-000064f0: 7461 736b 7320 3d20 7461 736b 7320 6966  tasks = tasks if
-00006500: 2074 6173 6b73 2065 6c73 6520 5b5d 0a20   tasks else []. 
-00006510: 2020 2073 6372 6970 7473 203d 2073 6372     scripts = scr
-00006520: 6970 7473 2069 6620 7363 7269 7074 7320  ipts if scripts 
-00006530: 656c 7365 205b 5d0a 2020 2020 706c 6179  else [].    play
-00006540: 626f 6f6b 7320 3d20 706c 6179 626f 6f6b  books = playbook
-00006550: 7320 6966 2070 6c61 7962 6f6f 6b73 2065  s if playbooks e
-00006560: 6c73 6520 5b5d 0a0a 2020 2020 2320 4469  lse []..    # Di
-00006570: 6374 2074 6f20 7265 7475 726e 0a20 2020  ct to return.   
-00006580: 2072 6574 7572 6e5f 6469 6374 203d 207b   return_dict = {
-00006590: 0a20 2020 2020 2020 2022 616c 6c5f 6669  .        "all_fi
-000065a0: 656c 6473 223a 205b 5d0a 2020 2020 7d0a  elds": [].    }.
-000065b0: 0a20 2020 2023 2047 6574 2052 756c 6573  .    # Get Rules
-000065c0: 0a20 2020 2072 6574 7572 6e5f 6469 6374  .    return_dict
-000065d0: 5b22 7275 6c65 7322 5d20 3d20 6765 745f  ["rules"] = get_
-000065e0: 7265 735f 6f62 6a28 2261 6374 696f 6e73  res_obj("actions
-000065f0: 222c 2052 6573 696c 6965 6e74 4f62 6a4d  ", ResilientObjM
-00006600: 6170 2e52 554c 4553 2c20 2252 756c 6522  ap.RULES, "Rule"
-00006610: 2c20 7275 6c65 732c 2065 7870 6f72 7429  , rules, export)
-00006620: 0a0a 2020 2020 6966 2067 6574 5f72 656c  ..    if get_rel
-00006630: 6174 6564 5f6f 626a 6563 7473 3a0a 2020  ated_objects:.  
-00006640: 2020 2020 2020 2320 466f 7220 5275 6c65        # For Rule
-00006650: 7320 7765 2061 7474 656d 7074 2074 6f20  s we attempt to 
-00006660: 6c6f 6361 7465 2072 656c 6174 6564 2077  locate related w
-00006670: 6f72 6b66 6c6f 7773 2061 6e64 206d 6573  orkflows and mes
-00006680: 7361 6765 5f64 6573 7469 6e61 7469 6f6e  sage_destination
-00006690: 730a 2020 2020 2020 2020 666f 7220 7220  s.        for r 
-000066a0: 696e 2072 6574 7572 6e5f 6469 6374 2e67  in return_dict.g
-000066b0: 6574 2822 7275 6c65 7322 293a 0a0a 2020  et("rules"):..  
-000066c0: 2020 2020 2020 2020 2020 2320 4765 7420            # Get 
-000066d0: 4163 7469 7669 7479 2046 6965 6c64 7320  Activity Fields 
-000066e0: 666f 7220 5275 6c65 730a 2020 2020 2020  for Rules.      
-000066f0: 2020 2020 2020 7669 6577 5f69 7465 6d73        view_items
-00006700: 203d 2072 2e67 6574 2822 7669 6577 5f69   = r.get("view_i
-00006710: 7465 6d73 222c 205b 5d29 0a20 2020 2020  tems", []).     
-00006720: 2020 2020 2020 2061 6374 6976 6974 795f         activity_
-00006730: 6669 656c 645f 7575 6964 7320 3d20 5b76  field_uuids = [v
-00006740: 2e67 6574 2822 636f 6e74 656e 7422 2920  .get("content") 
-00006750: 666f 7220 7620 696e 2076 6965 775f 6974  for v in view_it
-00006760: 656d 7320 6966 2022 636f 6e74 656e 7422  ems if "content"
-00006770: 2069 6e20 7620 616e 6420 762e 6765 7428   in v and v.get(
-00006780: 2266 6965 6c64 5f74 7970 6522 2920 3d3d  "field_type") ==
-00006790: 2052 6573 696c 6965 6e74 4669 656c 6454   ResilientFieldT
-000067a0: 7970 6573 2e41 4354 4956 4954 595f 4649  ypes.ACTIVITY_FI
-000067b0: 454c 445d 0a20 2020 2020 2020 2020 2020  ELD].           
-000067c0: 2072 5b22 6163 7469 7669 7479 5f66 6965   r["activity_fie
-000067d0: 6c64 7322 5d20 3d20 6765 745f 7265 735f  lds"] = get_res_
-000067e0: 6f62 6a28 2266 6965 6c64 7322 2c20 2275  obj("fields", "u
-000067f0: 7569 6422 2c20 2241 6374 6976 6974 7920  uid", "Activity 
-00006800: 4669 656c 6422 2c20 6163 7469 7669 7479  Field", activity
-00006810: 5f66 6965 6c64 5f75 7569 6473 2c20 6578  _field_uuids, ex
-00006820: 706f 7274 290a 2020 2020 2020 2020 2020  port).          
-00006830: 2020 7265 7475 726e 5f64 6963 745b 2261    return_dict["a
-00006840: 6c6c 5f66 6965 6c64 7322 5d2e 6578 7465  ll_fields"].exte
-00006850: 6e64 285b 7522 6163 7469 6f6e 696e 766f  nd([u"actioninvo
-00006860: 6361 7469 6f6e 2f7b 307d 222e 666f 726d  cation/{0}".form
-00006870: 6174 2866 6c64 2e67 6574 2822 6e61 6d65  at(fld.get("name
-00006880: 2229 2920 666f 7220 666c 6420 696e 2072  ")) for fld in r
-00006890: 2e67 6574 2822 6163 7469 7669 7479 5f66  .get("activity_f
-000068a0: 6965 6c64 7322 295d 290a 0a20 2020 2020  ields")])..     
-000068b0: 2020 2020 2020 2023 2047 6574 206e 616d         # Get nam
-000068c0: 6573 206f 6620 576f 726b 666c 6f77 7320  es of Workflows 
-000068d0: 7468 6174 2061 7265 2072 656c 6174 6564  that are related
-000068e0: 2074 6f20 5275 6c65 0a20 2020 2020 2020   to Rule.       
-000068f0: 2020 2020 2066 6f72 2077 2069 6e20 722e       for w in r.
-00006900: 6765 7428 2277 6f72 6b66 6c6f 7773 222c  get("workflows",
-00006910: 205b 5d29 3a0a 2020 2020 2020 2020 2020   []):.          
-00006920: 2020 2020 2020 776f 726b 666c 6f77 732e        workflows.
-00006930: 6170 7065 6e64 2877 290a 0a20 2020 2020  append(w)..     
-00006940: 2020 2020 2020 2023 2047 6574 206e 616d         # Get nam
-00006950: 6573 206f 6620 4d65 7373 6167 6520 4465  es of Message De
-00006960: 7374 696e 6174 696f 6e73 2074 6861 7420  stinations that 
-00006970: 6172 6520 7265 6c61 7465 6420 746f 2052  are related to R
-00006980: 756c 650a 2020 2020 2020 2020 2020 2020  ule.            
-00006990: 2320 4d65 7373 6167 6520 4465 7374 696e  # Message Destin
-000069a0: 6174 696f 6e73 2069 6e20 5275 6c65 7320  ations in Rules 
-000069b0: 6172 6520 6964 656e 7469 6669 6564 2062  are identified b
-000069c0: 7920 7468 6569 7220 4469 7370 6c61 7920  y their Display 
-000069d0: 4e61 6d65 0a20 2020 2020 2020 2020 2020  Name.           
-000069e0: 2066 6f72 206d 2069 6e20 722e 6765 7428   for m in r.get(
-000069f0: 226d 6573 7361 6765 5f64 6573 7469 6e61  "message_destina
-00006a00: 7469 6f6e 7322 2c20 5b5d 293a 0a20 2020  tions", []):.   
-00006a10: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-00006a20: 7361 6765 5f64 6573 7469 6e61 7469 6f6e  sage_destination
-00006a30: 732e 6170 7065 6e64 287b 2269 6465 6e74  s.append({"ident
-00006a40: 6966 6965 7222 3a20 226e 616d 6522 2c20  ifier": "name", 
-00006a50: 2276 616c 7565 223a 206d 7d29 0a0a 2020  "value": m})..  
-00006a60: 2020 2020 2020 2020 2020 2320 4765 7420            # Get 
-00006a70: 6e61 6d65 7320 6f66 2054 6173 6b73 2f53  names of Tasks/S
-00006a80: 6372 6970 7473 2f46 6965 6c64 7320 7468  cripts/Fields th
-00006a90: 6174 2061 7265 2072 656c 6174 6564 2074  at are related t
-00006aa0: 6f20 5275 6c65 0a20 2020 2020 2020 2020  o Rule.         
-00006ab0: 2020 2061 7574 6f6d 6174 696f 6e73 203d     automations =
-00006ac0: 2072 2e67 6574 2822 6175 746f 6d61 7469   r.get("automati
-00006ad0: 6f6e 7322 2c20 5b5d 290a 2020 2020 2020  ons", []).      
-00006ae0: 2020 2020 2020 666f 7220 6120 696e 2061        for a in a
-00006af0: 7574 6f6d 6174 696f 6e73 3a0a 2020 2020  utomations:.    
-00006b00: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00006b10: 2e67 6574 2822 7461 736b 735f 746f 5f63  .get("tasks_to_c
-00006b20: 7265 6174 6522 293a 0a20 2020 2020 2020  reate"):.       
-00006b30: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00006b40: 2074 2069 6e20 615b 2274 6173 6b73 5f74   t in a["tasks_t
-00006b50: 6f5f 6372 6561 7465 225d 3a0a 2020 2020  o_create"]:.    
-00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b70: 2020 2020 7461 736b 732e 6170 7065 6e64      tasks.append
-00006b80: 2874 290a 0a20 2020 2020 2020 2020 2020  (t)..           
-00006b90: 2020 2020 2065 6c69 6620 612e 6765 7428       elif a.get(
-00006ba0: 2273 6372 6970 7473 5f74 6f5f 7275 6e22  "scripts_to_run"
-00006bb0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00006bc0: 2020 2020 2020 2073 6372 6970 7473 2e61         scripts.a
-00006bd0: 7070 656e 6428 612e 6765 7428 2273 6372  ppend(a.get("scr
-00006be0: 6970 7473 5f74 6f5f 7275 6e22 2929 0a0a  ipts_to_run"))..
-00006bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c00: 656c 6966 2061 2e67 6574 2822 6669 656c  elif a.get("fiel
-00006c10: 6422 293a 0a20 2020 2020 2020 2020 2020  d"):.           
-00006c20: 2020 2020 2020 2020 2066 6965 6c64 732e           fields.
-00006c30: 6170 7065 6e64 2861 2e67 6574 2822 6669  append(a.get("fi
-00006c40: 656c 6422 2929 0a0a 2020 2020 2320 4765  eld"))..    # Ge
-00006c50: 7420 4675 6e63 7469 6f6e 730a 2020 2020  t Functions.    
-00006c60: 6966 2067 6574 5f72 656c 6174 6564 5f6f  if get_related_o
-00006c70: 626a 6563 7473 3a0a 2020 2020 2020 2020  bjects:.        
-00006c80: 2320 466f 7220 6675 6e63 7469 6f6e 7320  # For functions 
-00006c90: 7765 2061 7474 656d 7074 2074 6f20 6c6f  we attempt to lo
-00006ca0: 6361 7465 2072 656c 6174 6564 206d 6573  cate related mes
-00006cb0: 7361 6765 2064 6573 7469 6e61 7469 6f6e  sage destination
-00006cc0: 730a 2020 2020 2020 2020 2320 4765 7420  s.        # Get 
-00006cd0: 4675 6e63 7469 6f6e 206e 616d 6573 2074  Function names t
-00006ce0: 6861 7420 7573 6520 2777 616e 7465 6427  hat use 'wanted'
-00006cf0: 204d 6573 7361 6765 2044 6573 7469 6e61   Message Destina
-00006d00: 7469 6f6e 730a 2020 2020 2020 2020 666f  tions.        fo
-00006d10: 7220 6620 696e 2065 7870 6f72 742e 6765  r f in export.ge
-00006d20: 7428 2266 756e 6374 696f 6e73 222c 205b  t("functions", [
-00006d30: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-00006d40: 6966 2066 2e67 6574 2822 6465 7374 696e  if f.get("destin
-00006d50: 6174 696f 6e5f 6861 6e64 6c65 2229 2069  ation_handle") i
-00006d60: 6e20 6d65 7373 6167 655f 6465 7374 696e  n message_destin
-00006d70: 6174 696f 6e73 3a0a 2020 2020 2020 2020  ations:.        
-00006d80: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
-00006d90: 732e 6170 7065 6e64 2866 2e67 6574 2852  s.append(f.get(R
-00006da0: 6573 696c 6965 6e74 4f62 6a4d 6170 2e46  esilientObjMap.F
-00006db0: 554e 4354 494f 4e53 2929 0a0a 2020 2020  UNCTIONS))..    
-00006dc0: 7265 7475 726e 5f64 6963 745b 2266 756e  return_dict["fun
-00006dd0: 6374 696f 6e73 225d 203d 2067 6574 5f72  ctions"] = get_r
-00006de0: 6573 5f6f 626a 2822 6675 6e63 7469 6f6e  es_obj("function
-00006df0: 7322 2c20 5265 7369 6c69 656e 744f 626a  s", ResilientObj
-00006e00: 4d61 702e 4655 4e43 5449 4f4e 532c 2022  Map.FUNCTIONS, "
-00006e10: 4675 6e63 7469 6f6e 222c 2066 756e 6374  Function", funct
-00006e20: 696f 6e73 2c20 6578 706f 7274 290a 0a20  ions, export).. 
-00006e30: 2020 2066 6f72 2066 2069 6e20 7265 7475     for f in retu
-00006e40: 726e 5f64 6963 742e 6765 7428 2266 756e  rn_dict.get("fun
-00006e50: 6374 696f 6e73 2229 3a0a 2020 2020 2020  ctions"):.      
-00006e60: 2020 2320 4765 7420 4675 6e63 7469 6f6e    # Get Function
-00006e70: 2049 6e70 7574 730a 2020 2020 2020 2020   Inputs.        
-00006e80: 7669 6577 5f69 7465 6d73 203d 2066 2e67  view_items = f.g
-00006e90: 6574 2822 7669 6577 5f69 7465 6d73 222c  et("view_items",
-00006ea0: 205b 5d29 0a20 2020 2020 2020 2066 756e   []).        fun
-00006eb0: 6374 696f 6e5f 696e 7075 745f 7575 6964  ction_input_uuid
-00006ec0: 7320 3d20 5b76 2e67 6574 2822 636f 6e74  s = [v.get("cont
-00006ed0: 656e 7422 2920 666f 7220 7620 696e 2076  ent") for v in v
-00006ee0: 6965 775f 6974 656d 7320 6966 2022 636f  iew_items if "co
-00006ef0: 6e74 656e 7422 2069 6e20 7620 616e 6420  ntent" in v and 
-00006f00: 762e 6765 7428 2266 6965 6c64 5f74 7970  v.get("field_typ
-00006f10: 6522 2920 3d3d 2052 6573 696c 6965 6e74  e") == Resilient
-00006f20: 4669 656c 6454 7970 6573 2e46 554e 4354  FieldTypes.FUNCT
-00006f30: 494f 4e5f 494e 5055 545d 0a20 2020 2020  ION_INPUT].     
-00006f40: 2020 2066 5b22 696e 7075 7473 225d 203d     f["inputs"] =
-00006f50: 2067 6574 5f72 6573 5f6f 626a 2822 6669   get_res_obj("fi
-00006f60: 656c 6473 222c 2022 7575 6964 222c 2022  elds", "uuid", "
-00006f70: 4675 6e63 7469 6f6e 2049 6e70 7574 222c  Function Input",
-00006f80: 2066 756e 6374 696f 6e5f 696e 7075 745f   function_input_
-00006f90: 7575 6964 732c 2065 7870 6f72 7429 0a0a  uuids, export)..
-00006fa0: 2020 2020 2020 2020 7265 7475 726e 5f64          return_d
-00006fb0: 6963 745b 2261 6c6c 5f66 6965 6c64 7322  ict["all_fields"
-00006fc0: 5d2e 6578 7465 6e64 285b 7522 5f5f 6675  ].extend([u"__fu
-00006fd0: 6e63 7469 6f6e 2f7b 307d 222e 666f 726d  nction/{0}".form
-00006fe0: 6174 2866 6c64 2e67 6574 2822 6e61 6d65  at(fld.get("name
-00006ff0: 2229 2920 666f 7220 666c 6420 696e 2066  ")) for fld in f
-00007000: 2e67 6574 2822 696e 7075 7473 2229 5d29  .get("inputs")])
-00007010: 0a0a 2020 2020 2020 2020 2320 4765 7420  ..        # Get 
-00007020: 4675 6e63 7469 6f6e 2773 204d 6573 7361  Function's Messa
-00007030: 6765 2044 6573 7469 6e61 7469 6f6e 206e  ge Destination n
-00007040: 616d 650a 2020 2020 2020 2020 6d65 7373  ame.        mess
-00007050: 6167 655f 6465 7374 696e 6174 696f 6e73  age_destinations
-00007060: 2e61 7070 656e 6428 662e 6765 7428 2264  .append(f.get("d
-00007070: 6573 7469 6e61 7469 6f6e 5f68 616e 646c  estination_handl
-00007080: 6522 2c20 2222 2929 0a0a 2020 2020 2320  e", ""))..    # 
-00007090: 4765 7420 576f 726b 666c 6f77 730a 2020  Get Workflows.  
-000070a0: 2020 7265 7475 726e 5f64 6963 745b 2277    return_dict["w
-000070b0: 6f72 6b66 6c6f 7773 225d 203d 2067 6574  orkflows"] = get
-000070c0: 5f72 6573 5f6f 626a 2822 776f 726b 666c  _res_obj("workfl
-000070d0: 6f77 7322 2c20 5265 7369 6c69 656e 744f  ows", ResilientO
-000070e0: 626a 4d61 702e 574f 524b 464c 4f57 532c  bjMap.WORKFLOWS,
-000070f0: 2022 576f 726b 666c 6f77 222c 2077 6f72   "Workflow", wor
-00007100: 6b66 6c6f 7773 2c20 6578 706f 7274 290a  kflows, export).
-00007110: 0a20 2020 2069 6620 6765 745f 7265 6c61  .    if get_rela
-00007120: 7465 645f 6f62 6a65 6374 733a 0a20 2020  ted_objects:.   
-00007130: 2020 2020 2023 2046 6f72 2077 6f72 6b66       # For workf
-00007140: 6c6f 7773 2077 6520 6174 7465 6d70 7420  lows we attempt 
-00007150: 746f 206c 6f63 6174 6520 7265 6c61 7465  to locate relate
-00007160: 6420 6675 6e63 7469 6f6e 730a 2020 2020  d functions.    
-00007170: 2020 2020 2320 4765 7420 4675 6e63 7469      # Get Functi
-00007180: 6f6e 7320 696e 2057 6f72 6b66 6c6f 770a  ons in Workflow.
-00007190: 2020 2020 2020 2020 666f 7220 776f 726b          for work
-000071a0: 666c 6f77 2069 6e20 7265 7475 726e 5f64  flow in return_d
-000071b0: 6963 745b 2277 6f72 6b66 6c6f 7773 225d  ict["workflows"]
-000071c0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-000071d0: 5468 6973 2067 6574 7320 616c 6c20 7468  This gets all th
-000071e0: 6520 4675 6e63 7469 6f6e 7320 696e 2074  e Functions in t
-000071f0: 6865 2057 6f72 6b66 6c6f 7727 7320 584d  he Workflow's XM
-00007200: 4c0a 2020 2020 2020 2020 2020 2020 7766  L.            wf
-00007210: 5f66 756e 6374 696f 6e73 203d 2067 6574  _functions = get
-00007220: 5f77 6f72 6b66 6c6f 775f 6675 6e63 7469  _workflow_functi
-00007230: 6f6e 7328 776f 726b 666c 6f77 290a 0a20  ons(workflow).. 
-00007240: 2020 2020 2020 2020 2020 2023 2041 6464             # Add
-00007250: 2074 6865 2044 6973 706c 6179 204e 616d   the Display Nam
-00007260: 6520 616e 6420 4e61 6d65 2074 6f20 6561  e and Name to ea
-00007270: 6368 2077 665f 6675 6e63 7469 6f6e 0a20  ch wf_function. 
-00007280: 2020 2020 2020 2020 2020 2066 6f72 2077             for w
-00007290: 665f 666e 2069 6e20 7766 5f66 756e 6374  f_fn in wf_funct
-000072a0: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
-000072b0: 2020 2020 2020 666f 7220 666e 2069 6e20        for fn in 
-000072c0: 7265 7475 726e 5f64 6963 745b 2266 756e  return_dict["fun
-000072d0: 6374 696f 6e73 225d 3a0a 2020 2020 2020  ctions"]:.      
-000072e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000072f0: 2077 665f 666e 2e67 6574 2822 7575 6964   wf_fn.get("uuid
-00007300: 222c 2022 6122 2920 3d3d 2066 6e2e 6765  ", "a") == fn.ge
-00007310: 7428 2275 7569 6422 2c20 2262 2229 3a0a  t("uuid", "b"):.
-00007320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007330: 2020 2020 2020 2020 7766 5f66 6e5b 226e          wf_fn["n
-00007340: 616d 6522 5d20 3d20 666e 2e67 6574 2822  ame"] = fn.get("
-00007350: 6e61 6d65 2229 0a20 2020 2020 2020 2020  name").         
-00007360: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00007370: 665f 666e 5b22 6469 7370 6c61 795f 6e61  f_fn["display_na
-00007380: 6d65 225d 203d 2066 6e2e 6765 7428 2264  me"] = fn.get("d
-00007390: 6973 706c 6179 5f6e 616d 6522 290a 2020  isplay_name").  
-000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073b0: 2020 2020 2020 7766 5f66 6e5b 226d 6573        wf_fn["mes
-000073c0: 7361 6765 5f64 6573 7469 6e61 7469 6f6e  sage_destination
-000073d0: 225d 203d 2066 6e2e 6765 7428 2264 6573  "] = fn.get("des
-000073e0: 7469 6e61 7469 6f6e 5f68 616e 646c 6522  tination_handle"
-000073f0: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
-00007400: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00007410: 6561 6b0a 0a20 2020 2020 2020 2020 2020  eak..           
-00007420: 2077 6f72 6b66 6c6f 775b 2277 665f 6675   workflow["wf_fu
-00007430: 6e63 7469 6f6e 7322 5d20 3d20 7766 5f66  nctions"] = wf_f
-00007440: 756e 6374 696f 6e73 0a0a 2020 2020 2320  unctions..    # 
-00007450: 4765 7420 4d65 7373 6167 6520 4465 7374  Get Message Dest
-00007460: 696e 6174 696f 6e73 0a20 2020 2072 6574  inations.    ret
-00007470: 7572 6e5f 6469 6374 5b22 6d65 7373 6167  urn_dict["messag
-00007480: 655f 6465 7374 696e 6174 696f 6e73 225d  e_destinations"]
-00007490: 203d 2067 6574 5f72 6573 5f6f 626a 2822   = get_res_obj("
-000074a0: 6d65 7373 6167 655f 6465 7374 696e 6174  message_destinat
-000074b0: 696f 6e73 222c 2052 6573 696c 6965 6e74  ions", Resilient
-000074c0: 4f62 6a4d 6170 2e4d 4553 5341 4745 5f44  ObjMap.MESSAGE_D
-000074d0: 4553 5449 4e41 5449 4f4e 532c 2022 4d65  ESTINATIONS, "Me
-000074e0: 7373 6167 6520 4465 7374 696e 6174 696f  ssage Destinatio
-000074f0: 6e22 2c20 6d65 7373 6167 655f 6465 7374  n", message_dest
-00007500: 696e 6174 696f 6e73 2c20 6578 706f 7274  inations, export
-00007510: 290a 0a20 2020 2023 2047 6574 2049 6e63  )..    # Get Inc
-00007520: 6964 656e 7420 4669 656c 6473 2028 4375  ident Fields (Cu
-00007530: 7374 6f6d 2061 6e64 2049 6e74 6572 6e61  stom and Interna
-00007540: 6c29 0a20 2020 2072 6574 7572 6e5f 6469  l).    return_di
-00007550: 6374 5b22 6669 656c 6473 225d 203d 2067  ct["fields"] = g
-00007560: 6574 5f72 6573 5f6f 626a 2822 6669 656c  et_res_obj("fiel
-00007570: 6473 222c 2052 6573 696c 6965 6e74 4f62  ds", ResilientOb
-00007580: 6a4d 6170 2e46 4945 4c44 532c 2022 4669  jMap.FIELDS, "Fi
-00007590: 656c 6422 2c20 6669 656c 6473 2c20 6578  eld", fields, ex
-000075a0: 706f 7274 2c0a 2020 2020 2020 2020 2020  port,.          
-000075b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075c0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000075d0: 6e64 6974 696f 6e3d 6c61 6d62 6461 206f  ndition=lambda o
-000075e0: 3a20 5472 7565 2069 6620 6f2e 6765 7428  : True if o.get(
-000075f0: 2274 7970 655f 6964 2229 203d 3d20 5265  "type_id") == Re
-00007600: 7369 6c69 656e 7454 7970 6549 6473 2e49  silientTypeIds.I
-00007610: 4e43 4944 454e 5420 656c 7365 2046 616c  NCIDENT else Fal
-00007620: 7365 290a 0a20 2020 2072 6574 7572 6e5f  se)..    return_
-00007630: 6469 6374 5b22 616c 6c5f 6669 656c 6473  dict["all_fields
-00007640: 225d 2e65 7874 656e 6428 5b75 2269 6e63  "].extend([u"inc
-00007650: 6964 656e 742f 7b30 7d22 2e66 6f72 6d61  ident/{0}".forma
-00007660: 7428 666c 642e 6765 7428 226e 616d 6522  t(fld.get("name"
-00007670: 2929 2066 6f72 2066 6c64 2069 6e20 7265  )) for fld in re
-00007680: 7475 726e 5f64 6963 742e 6765 7428 2266  turn_dict.get("f
-00007690: 6965 6c64 7322 295d 290a 0a20 2020 2023  ields")])..    #
-000076a0: 2047 6574 2043 7573 746f 6d20 4172 7469   Get Custom Arti
-000076b0: 6661 6374 2054 7970 6573 0a20 2020 2072  fact Types.    r
-000076c0: 6574 7572 6e5f 6469 6374 5b22 6172 7469  eturn_dict["arti
-000076d0: 6661 6374 5f74 7970 6573 225d 203d 2067  fact_types"] = g
-000076e0: 6574 5f72 6573 5f6f 626a 2822 696e 6369  et_res_obj("inci
-000076f0: 6465 6e74 5f61 7274 6966 6163 745f 7479  dent_artifact_ty
-00007700: 7065 7322 2c20 5265 7369 6c69 656e 744f  pes", ResilientO
-00007710: 626a 4d61 702e 494e 4349 4445 4e54 5f41  bjMap.INCIDENT_A
-00007720: 5254 4946 4143 545f 5459 5045 532c 2022  RTIFACT_TYPES, "
-00007730: 4375 7374 6f6d 2041 7274 6966 6163 7422  Custom Artifact"
-00007740: 2c20 6172 7469 6661 6374 5f74 7970 6573  , artifact_types
-00007750: 2c20 6578 706f 7274 290a 0a20 2020 2023  , export)..    #
-00007760: 2047 6574 2049 6e63 6964 656e 7420 5479   Get Incident Ty
-00007770: 7065 730a 2020 2020 7265 7475 726e 5f64  pes.    return_d
-00007780: 6963 745b 2269 6e63 6964 656e 745f 7479  ict["incident_ty
-00007790: 7065 7322 5d20 3d20 6765 745f 7265 735f  pes"] = get_res_
-000077a0: 6f62 6a28 2269 6e63 6964 656e 745f 7479  obj("incident_ty
-000077b0: 7065 7322 2c20 5265 7369 6c69 656e 744f  pes", ResilientO
-000077c0: 626a 4d61 702e 494e 4349 4445 4e54 5f54  bjMap.INCIDENT_T
-000077d0: 5950 4553 2c20 2243 7573 746f 6d20 496e  YPES, "Custom In
-000077e0: 6369 6465 6e74 2054 7970 6522 2c20 696e  cident Type", in
-000077f0: 6369 6465 6e74 5f74 7970 6573 2c20 6578  cident_types, ex
-00007800: 706f 7274 290a 0a20 2020 2023 2047 6574  port)..    # Get
-00007810: 2044 6174 6120 5461 626c 6573 0a20 2020   Data Tables.   
-00007820: 2072 6574 7572 6e5f 6469 6374 5b22 6461   return_dict["da
-00007830: 7461 7461 626c 6573 225d 203d 2067 6574  tatables"] = get
-00007840: 5f72 6573 5f6f 626a 2822 7479 7065 7322  _res_obj("types"
-00007850: 2c20 5265 7369 6c69 656e 744f 626a 4d61  , ResilientObjMa
-00007860: 702e 4441 5441 5441 424c 4553 2c20 2244  p.DATATABLES, "D
-00007870: 6174 6174 6162 6c65 222c 2064 6174 6174  atatable", datat
-00007880: 6162 6c65 732c 2065 7870 6f72 742c 0a20  ables, export,. 
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078b0: 2020 2020 2020 2020 2020 2063 6f6e 6469             condi
-000078c0: 7469 6f6e 3d6c 616d 6264 6120 6f3a 2054  tion=lambda o: T
-000078d0: 7275 6520 6966 206f 2e67 6574 2822 7479  rue if o.get("ty
-000078e0: 7065 5f69 6422 2920 3d3d 2052 6573 696c  pe_id") == Resil
-000078f0: 6965 6e74 5479 7065 4964 732e 4441 5441  ientTypeIds.DATA
-00007900: 5441 424c 4520 656c 7365 2046 616c 7365  TABLE else False
-00007910: 290a 0a20 2020 2023 2047 6574 2043 7573  )..    # Get Cus
-00007920: 746f 6d20 5461 736b 730a 2020 2020 7265  tom Tasks.    re
-00007930: 7475 726e 5f64 6963 745b 2274 6173 6b73  turn_dict["tasks
-00007940: 225d 203d 2067 6574 5f72 6573 5f6f 626a  "] = get_res_obj
-00007950: 2822 6175 746f 6d61 7469 635f 7461 736b  ("automatic_task
-00007960: 7322 2c20 5265 7369 6c69 656e 744f 626a  s", ResilientObj
-00007970: 4d61 702e 5441 534b 532c 2022 4375 7374  Map.TASKS, "Cust
-00007980: 6f6d 2054 6173 6b22 2c20 7461 736b 732c  om Task", tasks,
-00007990: 2065 7870 6f72 7429 0a0a 2020 2020 2320   export)..    # 
-000079a0: 4765 7420 7265 6c61 7465 6420 5068 6173  Get related Phas
-000079b0: 6573 2066 6f72 2054 6173 6b73 0a20 2020  es for Tasks.   
-000079c0: 2070 6861 7365 5f69 6473 203d 205b 742e   phase_ids = [t.
-000079d0: 6765 7428 2270 6861 7365 5f69 6422 2920  get("phase_id") 
-000079e0: 666f 7220 7420 696e 2072 6574 7572 6e5f  for t in return_
-000079f0: 6469 6374 2e67 6574 2822 7461 736b 7322  dict.get("tasks"
-00007a00: 295d 0a20 2020 2072 6574 7572 6e5f 6469  )].    return_di
-00007a10: 6374 5b22 7068 6173 6573 225d 203d 2067  ct["phases"] = g
-00007a20: 6574 5f72 6573 5f6f 626a 2822 7068 6173  et_res_obj("phas
-00007a30: 6573 222c 2052 6573 696c 6965 6e74 4f62  es", ResilientOb
-00007a40: 6a4d 6170 2e50 4841 5345 532c 2022 5068  jMap.PHASES, "Ph
-00007a50: 6173 6522 2c20 7068 6173 655f 6964 732c  ase", phase_ids,
-00007a60: 2065 7870 6f72 7429 0a0a 2020 2020 2320   export)..    # 
-00007a70: 4765 7420 5363 7269 7074 730a 2020 2020  Get Scripts.    
-00007a80: 7265 7475 726e 5f64 6963 745b 2273 6372  return_dict["scr
-00007a90: 6970 7473 225d 203d 2067 6574 5f72 6573  ipts"] = get_res
-00007aa0: 5f6f 626a 2822 7363 7269 7074 7322 2c20  _obj("scripts", 
-00007ab0: 5265 7369 6c69 656e 744f 626a 4d61 702e  ResilientObjMap.
-00007ac0: 5343 5249 5054 532c 2022 5363 7269 7074  SCRIPTS, "Script
-00007ad0: 222c 2073 6372 6970 7473 2c20 6578 706f  ", scripts, expo
-00007ae0: 7274 290a 0a20 2020 2023 2047 6574 2041  rt)..    # Get A
-00007af0: 7070 730a 2020 2020 7265 7475 726e 5f64  pps.    return_d
-00007b00: 6963 745b 2261 7070 7322 5d20 3d20 6765  ict["apps"] = ge
-00007b10: 745f 7265 735f 6f62 6a28 2261 7070 7322  t_res_obj("apps"
-00007b20: 2c20 5265 7369 6c69 656e 744f 626a 4d61  , ResilientObjMa
-00007b30: 702e 4150 5053 2c20 2241 7070 7322 2c20  p.APPS, "Apps", 
-00007b40: 6170 7073 2c20 6578 706f 7274 290a 0a20  apps, export).. 
-00007b50: 2020 2023 2047 6574 2050 6c61 7962 6f6f     # Get Playboo
-00007b60: 6b73 0a20 2020 2069 6620 706c 6179 626f  ks.    if playbo
-00007b70: 6f6b 7320 616e 6420 636f 6e73 7461 6e74  oks and constant
-00007b80: 732e 4355 5252 454e 545f 534f 4152 5f53  s.CURRENT_SOAR_S
-00007b90: 4552 5645 525f 5645 5253 494f 4e20 616e  ERVER_VERSION an
-00007ba0: 6420 636f 6e73 7461 6e74 732e 4355 5252  d constants.CURR
-00007bb0: 454e 545f 534f 4152 5f53 4552 5645 525f  ENT_SOAR_SERVER_
-00007bc0: 5645 5253 494f 4e20 3c20 636f 6e73 7461  VERSION < consta
-00007bd0: 6e74 732e 4d49 4e5f 534f 4152 5f53 4552  nts.MIN_SOAR_SER
-00007be0: 5645 525f 5645 5253 494f 4e5f 504c 4159  VER_VERSION_PLAY
-00007bf0: 424f 4f4b 533a 0a20 2020 2020 2020 2072  BOOKS:.        r
-00007c00: 6169 7365 2053 444b 4578 6365 7074 696f  aise SDKExceptio
-00007c10: 6e28 636f 6e73 7461 6e74 732e 4552 524f  n(constants.ERRO
-00007c20: 525f 504c 4159 424f 4f4b 5f53 5550 504f  R_PLAYBOOK_SUPPO
-00007c30: 5254 290a 2020 2020 656c 7365 3a0a 2020  RT).    else:.  
-00007c40: 2020 2020 2020 7265 7475 726e 5f64 6963        return_dic
-00007c50: 745b 2270 6c61 7962 6f6f 6b73 225d 203d  t["playbooks"] =
-00007c60: 2067 6574 5f72 6573 5f6f 626a 2822 706c   get_res_obj("pl
-00007c70: 6179 626f 6f6b 7322 2c20 5265 7369 6c69  aybooks", Resili
-00007c80: 656e 744f 626a 4d61 702e 504c 4159 424f  entObjMap.PLAYBO
-00007c90: 4f4b 532c 2022 506c 6179 626f 6f6b 222c  OKS, "Playbook",
-00007ca0: 2070 6c61 7962 6f6f 6b73 2c20 6578 706f   playbooks, expo
-00007cb0: 7274 290a 0a20 2020 2020 2020 2069 6620  rt)..        if 
-00007cc0: 6765 745f 7265 6c61 7465 645f 6f62 6a65  get_related_obje
-00007cd0: 6374 733a 0a20 2020 2020 2020 2020 2020  cts:.           
-00007ce0: 2023 2046 6f72 2050 6c61 7962 6f6f 6b73   # For Playbooks
-00007cf0: 2077 6520 6174 7465 6d70 7420 746f 206c   we attempt to l
-00007d00: 6f63 6174 6520 7265 6c61 7465 6420 6675  ocate related fu
-00007d10: 6e63 7469 6f6e 7320 616e 6420 7363 7269  nctions and scri
-00007d20: 7074 730a 2020 2020 2020 2020 2020 2020  pts.            
-00007d30: 2320 4765 7420 4675 6e63 7469 6f6e 7320  # Get Functions 
-00007d40: 696e 2050 6c61 7962 6f6f 6b73 0a20 2020  in Playbooks.   
-00007d50: 2020 2020 2020 2020 2066 6f72 2070 6c61           for pla
-00007d60: 7962 6f6f 6b20 696e 2072 6574 7572 6e5f  ybook in return_
-00007d70: 6469 6374 2e67 6574 2822 706c 6179 626f  dict.get("playbo
-00007d80: 6f6b 7322 2c20 5b5d 293a 0a20 2020 2020  oks", []):.     
-00007d90: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
-00007da0: 7320 6765 7473 2061 6c6c 2074 6865 2066  s gets all the f
-00007db0: 756e 6374 696f 6e73 2061 6e64 2073 6372  unctions and scr
-00007dc0: 6970 7473 2069 6e20 7468 6520 506c 6179  ipts in the Play
-00007dd0: 626f 6f6b 7327 7320 584d 4c0a 2020 2020  books's XML.    
-00007de0: 2020 2020 2020 2020 2020 2020 7062 5f6f              pb_o
-00007df0: 626a 6563 7473 203d 2067 6574 5f70 6c61  bjects = get_pla
-00007e00: 7962 6f6f 6b5f 6f62 6a65 6374 7328 706c  ybook_objects(pl
-00007e10: 6179 626f 6f6b 290a 0a20 2020 2020 2020  aybook)..       
-00007e20: 2020 2020 2020 2020 2023 2041 6464 2074           # Add t
-00007e30: 6865 2044 6973 706c 6179 204e 616d 6520  he Display Name 
-00007e40: 616e 6420 4e61 6d65 2074 6f20 6561 6368  and Name to each
-00007e50: 2077 665f 6675 6e63 7469 6f6e 0a20 2020   wf_function.   
-00007e60: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00007e70: 2070 625f 666e 2069 6e20 7062 5f6f 626a   pb_fn in pb_obj
-00007e80: 6563 7473 2e67 6574 2822 6675 6e63 7469  ects.get("functi
-00007e90: 6f6e 7322 2c20 5b5d 293a 0a20 2020 2020  ons", []):.     
-00007ea0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00007eb0: 6f72 2066 6e20 696e 2072 6574 7572 6e5f  or fn in return_
-00007ec0: 6469 6374 5b22 6675 6e63 7469 6f6e 7322  dict["functions"
-00007ed0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00007ee0: 2020 2020 2020 2020 2020 2069 6620 7062             if pb
-00007ef0: 5f66 6e2e 6765 7428 2275 7569 6422 2c20  _fn.get("uuid", 
-00007f00: 2275 7569 645f 6e6f 745f 666f 756e 645f  "uuid_not_found_
-00007f10: 7062 2229 203d 3d20 666e 2e67 6574 2822  pb") == fn.get("
-00007f20: 7575 6964 222c 2022 7575 6964 5f6e 6f74  uuid", "uuid_not
-00007f30: 5f66 6f75 6e64 5f66 6e22 293a 0a20 2020  _found_fn"):.   
-00007f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f50: 2020 2020 2020 2020 2070 625f 666e 5b22           pb_fn["
-00007f60: 6e61 6d65 225d 203d 2066 6e2e 6765 7428  name"] = fn.get(
-00007f70: 226e 616d 6522 290a 2020 2020 2020 2020  "name").        
-00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f90: 2020 2020 7062 5f66 6e5b 2264 6973 706c      pb_fn["displ
-00007fa0: 6179 5f6e 616d 6522 5d20 3d20 666e 2e67  ay_name"] = fn.g
-00007fb0: 6574 2822 6469 7370 6c61 795f 6e61 6d65  et("display_name
-00007fc0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00007fd0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00007fe0: 625f 666e 5b22 6d65 7373 6167 655f 6465  b_fn["message_de
-00007ff0: 7374 696e 6174 696f 6e22 5d20 3d20 666e  stination"] = fn
-00008000: 2e67 6574 2822 6465 7374 696e 6174 696f  .get("destinatio
-00008010: 6e5f 6861 6e64 6c65 222c 2022 2229 0a20  n_handle", ""). 
-00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008030: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00008040: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008050: 2020 2320 4966 2061 2070 6c61 7962 6f6f    # If a playboo
-00008060: 6b20 7363 7269 7074 2069 7320 6c6f 6361  k script is loca
-00008070: 6c2c 2069 7473 2069 6e66 6f72 6d61 7469  l, its informati
-00008080: 6f6e 2063 616e 2062 6520 6469 7265 6374  on can be direct
-00008090: 6c79 2065 7874 7261 6374 6564 2066 726f  ly extracted fro
-000080a0: 6d20 7468 6520 706c 6179 626f 6f6b 2c0a  m the playbook,.
-000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080c0: 2320 6966 206e 6f74 2c20 7468 6520 7363  # if not, the sc
-000080d0: 7269 7074 2773 2069 6e66 6f72 6d61 7469  ript's informati
-000080e0: 6f6e 2068 6173 2074 6f20 6265 2065 7874  on has to be ext
-000080f0: 7261 6374 6564 2066 726f 6d20 7468 6520  racted from the 
-00008100: 676c 6f62 616c 2073 6372 6970 7473 0a20  global scripts. 
-00008110: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00008120: 6f72 2070 625f 7363 2069 6e20 7062 5f6f  or pb_sc in pb_o
-00008130: 626a 6563 7473 2e67 6574 2822 7363 7269  bjects.get("scri
-00008140: 7074 7322 2c20 5b5d 293a 0a20 2020 2020  pts", []):.     
-00008150: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00008160: 2049 6620 7468 6520 7363 7269 7074 2069   If the script i
-00008170: 7320 6120 6c6f 6361 6c20 7363 7269 7074  s a local script
-00008180: 2c20 7468 656e 2077 6520 6e65 6564 2074  , then we need t
-00008190: 6f20 6669 6e64 2074 6865 2073 6372 6970  o find the scrip
-000081a0: 7420 696e 2074 6865 2050 6c61 7962 6f6f  t in the Playboo
-000081b0: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
-000081c0: 2020 2020 2020 666f 756e 645f 7363 7269        found_scri
-000081d0: 7074 203d 2067 6574 5f73 6372 6970 745f  pt = get_script_
-000081e0: 696e 666f 2870 625f 7363 2c20 706c 6179  info(pb_sc, play
-000081f0: 626f 6f6b 2e67 6574 2822 6c6f 6361 6c5f  book.get("local_
-00008200: 7363 7269 7074 7322 292c 2053 4352 4950  scripts"), SCRIP
-00008210: 545f 5459 5045 5f4d 4150 2e67 6574 2822  T_TYPE_MAP.get("
-00008220: 6c6f 6361 6c22 2929 0a0a 2020 2020 2020  local"))..      
-00008230: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00008240: 4966 2073 6372 6970 7420 6e6f 7420 666f  If script not fo
-00008250: 756e 6420 696e 2070 6c61 7962 6f6f 6b2c  und in playbook,
-00008260: 2073 6561 7263 6869 6e67 2047 6c6f 6261   searching Globa
-00008270: 6c20 5363 7269 7074 730a 2020 2020 2020  l Scripts.      
-00008280: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00008290: 756e 645f 7363 7269 7074 203d 2067 6574  und_script = get
-000082a0: 5f73 6372 6970 745f 696e 666f 2870 625f  _script_info(pb_
-000082b0: 7363 2c20 7265 7475 726e 5f64 6963 745b  sc, return_dict[
-000082c0: 2273 6372 6970 7473 225d 2c20 5343 5249  "scripts"], SCRI
-000082d0: 5054 5f54 5950 455f 4d41 502e 6765 7428  PT_TYPE_MAP.get(
-000082e0: 2267 6c6f 6261 6c22 2929 2069 6620 6e6f  "global")) if no
-000082f0: 7420 666f 756e 645f 7363 7269 7074 2065  t found_script e
-00008300: 6c73 6520 5472 7565 0a0a 2020 2020 2020  lse True..      
-00008310: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00008320: 4966 2074 6865 2073 6372 6970 7420 6973  If the script is
-00008330: 206e 6f74 2066 6f75 6e64 2069 6e20 7468   not found in th
-00008340: 6520 506c 6179 626f 6f6b 206f 7220 476c  e Playbook or Gl
-00008350: 6f62 616c 2053 6372 6970 7473 2c20 7468  obal Scripts, th
-00008360: 656e 2069 7473 2055 5549 4420 6973 2075  en its UUID is u
-00008370: 7365 6420 746f 2066 696e 6420 7468 6520  sed to find the 
-00008380: 7363 7269 7074 2066 6f72 6d20 7468 6520  script form the 
-00008390: 6f72 6720 6578 706f 7274 0a20 2020 2020  org export.     
-000083a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000083b0: 6620 6e6f 7420 666f 756e 645f 7363 7269  f not found_scri
-000083c0: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-000083d0: 2020 2020 2020 2020 2020 2020 5f75 6e66              _unf
-000083e0: 6f75 6e64 5f73 6372 6970 7473 203d 2067  ound_scripts = g
-000083f0: 6574 5f72 6573 5f6f 626a 2822 7363 7269  et_res_obj("scri
-00008400: 7074 7322 2c20 2275 7569 6422 2c20 2253  pts", "uuid", "S
-00008410: 6372 6970 7422 2c20 5b70 625f 7363 2e67  cript", [pb_sc.g
-00008420: 6574 2822 7575 6964 2229 5d2c 2065 7870  et("uuid")], exp
-00008430: 6f72 7429 0a20 2020 2020 2020 2020 2020  ort).           
-00008440: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00008450: 2073 6372 6970 7420 696e 205f 756e 666f   script in _unfo
-00008460: 756e 645f 7363 7269 7074 733a 0a20 2020  und_scripts:.   
-00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008480: 2020 2020 2020 2020 2023 2052 656e 616d           # Renam
-00008490: 696e 6720 7468 6520 785f 6170 695f 6e61  ing the x_api_na
-000084a0: 6d65 2074 6f20 6e61 6d65 2e20 5369 6e63  me to name. Sinc
-000084b0: 6520 7468 6520 7363 7269 7074 2077 6173  e the script was
-000084c0: 2066 6574 6368 6564 2077 6974 6820 5555   fetched with UU
-000084d0: 4944 2c20 7468 6520 785f 6170 695f 6e61  ID, the x_api_na
-000084e0: 6d65 2069 7320 7468 6520 5555 4944 0a20  me is the UUID. 
-000084f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008500: 2020 2020 2020 2020 2020 2073 6372 6970             scrip
-00008510: 745b 2278 5f61 7069 5f6e 616d 6522 5d20  t["x_api_name"] 
-00008520: 3d20 7363 7269 7074 5b22 6e61 6d65 225d  = script["name"]
-00008530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008540: 2020 2020 2020 2020 2066 6f75 6e64 5f73           found_s
-00008550: 6372 6970 7420 3d20 6765 745f 7363 7269  cript = get_scri
-00008560: 7074 5f69 6e66 6f28 7062 5f73 632c 205f  pt_info(pb_sc, _
-00008570: 756e 666f 756e 645f 7363 7269 7074 732c  unfound_scripts,
-00008580: 2053 4352 4950 545f 5459 5045 5f4d 4150   SCRIPT_TYPE_MAP
-00008590: 2e67 6574 2822 676c 6f62 616c 2229 290a  .get("global")).
-000085a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085b0: 2020 2020 2020 2020 2320 4164 6469 6e67          # Adding
-000085c0: 2073 6372 6970 7420 746f 2072 6574 7572   script to retur
-000085d0: 6e5f 6469 6374 2e20 5468 6973 2069 7320  n_dict. This is 
-000085e0: 746f 206d 616b 6520 7375 7265 2074 6861  to make sure tha
-000085f0: 7420 6974 7320 696e 636c 7564 6564 2069  t its included i
-00008600: 6e20 7468 6520 6578 706f 7274 2e72 6573  n the export.res
-00008610: 2061 6e64 2063 7573 746f 6d69 7a65 2e70   and customize.p
-00008620: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-00008630: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008640: 5f64 6963 745b 2273 6372 6970 7473 225d  _dict["scripts"]
-00008650: 2e65 7874 656e 6428 5f75 6e66 6f75 6e64  .extend(_unfound
-00008660: 5f73 6372 6970 7473 290a 0a20 2020 2020  _scripts)..     
-00008670: 2020 2020 2020 2020 2020 2023 2061 6464             # add
-00008680: 206e 616d 6520 746f 2065 6163 6820 7375   name to each su
-00008690: 6220 706c 6179 626f 6f6b 2069 6e70 7574  b playbook input
-000086a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000086b0: 2066 6f72 2070 625f 7375 625f 7062 2069   for pb_sub_pb i
-000086c0: 6e20 7062 5f6f 626a 6563 7473 2e67 6574  n pb_objects.get
-000086d0: 2822 7375 625f 7062 7322 2c20 5b5d 293a  ("sub_pbs", []):
-000086e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000086f0: 2020 2020 2072 6570 6c61 6365 5f75 7569       replace_uui
-00008700: 6473 5f69 6e5f 7375 6270 6c61 7962 6f6f  ds_in_subplayboo
-00008710: 6b5f 6461 7461 2870 625f 7375 625f 7062  k_data(pb_sub_pb
-00008720: 2c20 6578 706f 7274 290a 0a20 2020 2020  , export)..     
-00008730: 2020 2020 2020 2020 2020 2061 6374 6976             activ
-00008740: 6174 696f 6e5f 7479 7065 203d 2070 6c61  ation_type = pla
-00008750: 7962 6f6f 6b2e 6765 7428 2261 6374 6976  ybook.get("activ
-00008760: 6174 696f 6e5f 7479 7065 222c 2022 2229  ation_type", "")
-00008770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008780: 2069 6620 706c 6179 626f 6f6b 2e67 6574   if playbook.get
-00008790: 2822 7479 7065 2229 203d 3d20 2273 7562  ("type") == "sub
-000087a0: 706c 6179 626f 6f6b 223a 0a20 2020 2020  playbook":.     
-000087b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000087c0: 6c61 7962 6f6f 6b5b 2261 6374 6976 6174  laybook["activat
-000087d0: 696f 6e5f 7479 7065 225d 203d 2022 5375  ion_type"] = "Su
-000087e0: 622d 706c 6179 626f 6f6b 220a 2020 2020  b-playbook".    
-000087f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00008800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008810: 2020 2020 2020 706c 6179 626f 6f6b 5b22        playbook["
-00008820: 6163 7469 7661 7469 6f6e 5f74 7970 6522  activation_type"
-00008830: 5d20 3d20 6163 7469 7661 7469 6f6e 5f74  ] = activation_t
-00008840: 7970 652e 6361 7069 7461 6c69 7a65 2829  ype.capitalize()
-00008850: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008860: 2020 6966 2061 6374 6976 6174 696f 6e5f    if activation_
-00008870: 7479 7065 2e6c 6f77 6572 2829 203d 3d20  type.lower() == 
-00008880: 226d 616e 7561 6c22 3a0a 2020 2020 2020  "manual":.      
-00008890: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-000088a0: 7469 7661 7469 6f6e 5f63 6f6e 6469 7469  tivation_conditi
-000088b0: 6f6e 7320 3d20 706c 6179 626f 6f6b 2e67  ons = playbook.g
-000088c0: 6574 2822 6d61 6e75 616c 5f73 6574 7469  et("manual_setti
-000088d0: 6e67 7322 2c20 7b7d 292e 6765 7428 2261  ngs", {}).get("a
-000088e0: 6374 6976 6174 696f 6e5f 636f 6e64 6974  ctivation_condit
-000088f0: 696f 6e73 222c 207b 7d29 0a20 2020 2020  ions", {}).     
-00008900: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00008910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008920: 2020 2020 2061 6374 6976 6174 696f 6e5f       activation_
-00008930: 636f 6e64 6974 696f 6e73 203d 2070 6c61  conditions = pla
-00008940: 7962 6f6f 6b2e 6765 7428 2261 6374 6976  ybook.get("activ
-00008950: 6174 696f 6e5f 6465 7461 696c 7322 2c20  ation_details", 
-00008960: 7b7d 292e 6765 7428 2261 6374 6976 6174  {}).get("activat
-00008970: 696f 6e5f 636f 6e64 6974 696f 6e73 222c  ion_conditions",
-00008980: 207b 7d29 0a20 2020 2020 2020 2020 2020   {}).           
-00008990: 2020 2020 2070 6c61 7962 6f6f 6b5b 2263       playbook["c
-000089a0: 6f6e 6469 7469 6f6e 7322 5d20 3d20 7374  onditions"] = st
-000089b0: 725f 7265 7072 5f61 6374 6976 6174 696f  r_repr_activatio
-000089c0: 6e5f 636f 6e64 6974 696f 6e73 2861 6374  n_conditions(act
-000089d0: 6976 6174 696f 6e5f 636f 6e64 6974 696f  ivation_conditio
-000089e0: 6e73 2920 6f72 2022 2d22 0a20 2020 2020  ns) or "-".     
-000089f0: 2020 2020 2020 2020 2020 2070 6c61 7962             playb
-00008a00: 6f6f 6b5b 2270 625f 6675 6e63 7469 6f6e  ook["pb_function
-00008a10: 7322 5d20 3d20 7062 5f6f 626a 6563 7473  s"] = pb_objects
-00008a20: 2e67 6574 2822 6675 6e63 7469 6f6e 7322  .get("functions"
-00008a30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008a40: 2020 706c 6179 626f 6f6b 5b22 7062 5f73    playbook["pb_s
-00008a50: 6372 6970 7473 225d 2020 203d 2070 625f  cripts"]   = pb_
-00008a60: 6f62 6a65 6374 732e 6765 7428 2273 6372  objects.get("scr
-00008a70: 6970 7473 2229 0a20 2020 2020 2020 2020  ipts").         
-00008a80: 2020 2020 2020 2070 6c61 7962 6f6f 6b5b         playbook[
-00008a90: 2270 625f 7375 625f 7062 7322 5d20 2020  "pb_sub_pbs"]   
-00008aa0: 3d20 7062 5f6f 626a 6563 7473 2e67 6574  = pb_objects.get
-00008ab0: 2822 7375 625f 7062 7322 290a 0a20 2020  ("sub_pbs")..   
-00008ac0: 2072 6574 7572 6e20 7265 7475 726e 5f64   return return_d
-00008ad0: 6963 740a 0a0a 6465 6620 6d69 6e69 6679  ict...def minify
-00008ae0: 5f65 7870 6f72 7428 6578 706f 7274 2c0a  _export(export,.
-00008af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b00: 2020 6b65 7973 5f74 6f5f 6b65 6570 3d5b    keys_to_keep=[
-00008b10: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00008b20: 2020 2020 206d 6573 7361 6765 5f64 6573       message_des
-00008b30: 7469 6e61 7469 6f6e 733d 5b5d 2c0a 2020  tinations=[],.  
-00008b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b50: 6675 6e63 7469 6f6e 733d 5b5d 2c0a 2020  functions=[],.  
-00008b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b70: 776f 726b 666c 6f77 733d 5b5d 2c0a 2020  workflows=[],.  
-00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b90: 7275 6c65 733d 5b5d 2c0a 2020 2020 2020  rules=[],.      
-00008ba0: 2020 2020 2020 2020 2020 2020 6669 656c              fiel
-00008bb0: 6473 3d5b 5d2c 0a20 2020 2020 2020 2020  ds=[],.         
-00008bc0: 2020 2020 2020 2020 2061 7274 6966 6163           artifac
-00008bd0: 745f 7479 7065 733d 5b5d 2c0a 2020 2020  t_types=[],.    
-00008be0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00008bf0: 7461 7461 626c 6573 3d5b 5d2c 0a20 2020  tatables=[],.   
-00008c00: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00008c10: 6173 6b73 3d5b 5d2c 0a20 2020 2020 2020  asks=[],.       
-00008c20: 2020 2020 2020 2020 2020 2070 6861 7365             phase
-00008c30: 733d 5b5d 2c0a 2020 2020 2020 2020 2020  s=[],.          
-00008c40: 2020 2020 2020 2020 7363 7269 7074 733d          scripts=
-00008c50: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
-00008c60: 2020 2020 2020 696e 6369 6465 6e74 5f74        incident_t
-00008c70: 7970 6573 3d5b 5d2c 0a20 2020 2020 2020  ypes=[],.       
-00008c80: 2020 2020 2020 2020 2020 2070 6c61 7962             playb
-00008c90: 6f6f 6b73 3d5b 5d29 3a0a 2020 2020 2222  ooks=[]):.    ""
-00008ca0: 220a 2020 2020 5265 7475 726e 2061 2027  ".    Return a '
-00008cb0: 6d69 6e69 6669 6564 2720 7665 7273 696f  minified' versio
-00008cc0: 6e20 6f66 2074 6865 2065 7870 6f72 742e  n of the export.
-00008cd0: 0a20 2020 2041 6c6c 2070 6172 616d 6574  .    All paramet
-00008ce0: 6572 7320 6172 6520 6120 6c69 7374 206f  ers are a list o
-00008cf0: 6620 6170 695f 6e61 6d65 7320 6f66 206f  f api_names of o
-00008d00: 626a 6563 7473 2074 6f20 696e 636c 7564  bjects to includ
-00008d10: 6520 696e 2074 6865 2065 7870 6f72 742e  e in the export.
-00008d20: 0a20 2020 2041 6e79 7468 696e 6720 6e6f  .    Anything no
-00008d30: 7420 6d65 6e74 696f 6e65 6420 696e 2070  t mentioned in p
-00008d40: 6173 7365 6420 4c69 7374 7320 6172 6520  assed Lists are 
-00008d50: 7365 7420 746f 2065 6d70 7479 206f 7220  set to empty or 
-00008d60: 4e6f 6e65 2e0a 0a20 2020 203a 7061 7261  None...    :para
-00008d70: 6d20 6578 706f 7274 3a20 5468 6520 7265  m export: The re
-00008d80: 7375 6c74 206f 6620 6361 6c6c 696e 6720  sult of calling 
-00008d90: 6765 745f 6c61 7465 7374 5f6f 7267 5f65  get_latest_org_e
-00008da0: 7870 6f72 7428 290a 2020 2020 3a74 7970  xport().    :typ
-00008db0: 6520 6578 706f 7274 3a20 4469 6374 0a20  e export: Dict. 
-00008dc0: 2020 203a 7061 7261 6d20 6b65 7973 5f74     :param keys_t
-00008dd0: 6f5f 6b65 6570 3a20 4b65 7973 2074 6861  o_keep: Keys tha
-00008de0: 7420 7368 6f75 6c64 2072 656d 6169 6e20  t should remain 
-00008df0: 756e 6368 616e 6765 6420 6672 6f6d 2074  unchanged from t
-00008e00: 6865 206f 7269 6769 6e61 6c20 6578 706f  he original expo
-00008e10: 7274 0a20 2020 203a 7479 7065 206b 6579  rt.    :type key
-00008e20: 735f 746f 5f6b 6565 703a 2044 6963 740a  s_to_keep: Dict.
-00008e30: 2020 2020 3a70 6172 616d 206d 6573 7361      :param messa
-00008e40: 6765 5f64 6573 7469 6e61 7469 6f6e 733a  ge_destinations:
-00008e50: 204c 6973 7420 6f66 204d 6573 7361 6765   List of Message
-00008e60: 2044 6573 7469 6e61 7469 6f6e 2041 5049   Destination API
-00008e70: 204e 616d 6573 0a20 2020 203a 7061 7261   Names.    :para
-00008e80: 6d20 6675 6e63 7469 6f6e 733a 204c 6973  m functions: Lis
-00008e90: 7420 6f66 2046 756e 6374 696f 6e20 4150  t of Function AP
-00008ea0: 4920 4e61 6d65 730a 2020 2020 3a70 6172  I Names.    :par
-00008eb0: 616d 2077 6f72 6b66 6c6f 7773 3a20 4c69  am workflows: Li
-00008ec0: 7374 206f 6620 576f 726b 666c 6f77 2041  st of Workflow A
-00008ed0: 5049 204e 616d 6573 0a20 2020 203a 7061  PI Names.    :pa
-00008ee0: 7261 6d20 7275 6c65 733a 204c 6973 7420  ram rules: List 
-00008ef0: 6f66 2052 756c 6520 4469 7370 6c61 7920  of Rule Display 
-00008f00: 4e61 6d65 730a 2020 2020 3a70 6172 616d  Names.    :param
-00008f10: 2066 6965 6c64 733a 204c 6973 7420 6f66   fields: List of
-00008f20: 2046 6965 6c64 2065 7870 6f72 745f 6b65   Field export_ke
-00008f30: 7973 2065 2e67 2e20 5b27 696e 6369 6465  ys e.g. ['incide
-00008f40: 6e74 2f63 7573 746f 6d5f 6669 656c 6427  nt/custom_field'
-00008f50: 2c20 2761 6374 696f 6e69 6e76 6f63 6174  , 'actioninvocat
-00008f60: 696f 6e2f 6375 7374 6f6d 5f61 6374 6976  ion/custom_activ
-00008f70: 6974 795f 6669 656c 6427 2c20 275f 5f66  ity_field', '__f
-00008f80: 756e 6374 696f 6e2f 6375 7374 6f6d 5f66  unction/custom_f
-00008f90: 6e5f 696e 7075 7427 5d0a 2020 2020 3a70  n_input'].    :p
-00008fa0: 6172 616d 2061 7274 6966 6163 745f 7479  aram artifact_ty
-00008fb0: 7065 733a 204c 6973 7420 6f66 2043 7573  pes: List of Cus
-00008fc0: 746f 6d20 4172 7469 6661 6374 2054 7970  tom Artifact Typ
-00008fd0: 6520 4150 4920 4e61 6d65 730a 2020 2020  e API Names.    
-00008fe0: 3a70 6172 616d 2064 6174 6174 6162 6c65  :param datatable
-00008ff0: 733a 204c 6973 7420 6f66 2044 6174 6120  s: List of Data 
-00009000: 5461 626c 6520 4150 4920 4e61 6d65 730a  Table API Names.
-00009010: 2020 2020 3a70 6172 616d 2074 6173 6b73      :param tasks
-00009020: 3a20 4c69 7374 206f 6620 4375 7374 6f6d  : List of Custom
-00009030: 2054 6173 6b20 4150 4920 4e61 6d65 730a   Task API Names.
-00009040: 2020 2020 3a70 6172 616d 2074 6173 6b73      :param tasks
-00009050: 3a20 4c69 7374 206f 6620 5068 6173 6573  : List of Phases
-00009060: 2041 5049 204e 616d 6573 0a20 2020 203a   API Names.    :
-00009070: 7061 7261 6d20 7363 7269 7074 733a 204c  param scripts: L
-00009080: 6973 7420 6f66 2053 6372 6970 7420 4469  ist of Script Di
-00009090: 7370 6c61 7920 4e61 6d65 730a 2020 2020  splay Names.    
-000090a0: 3a70 6172 616d 2069 6e63 6964 656e 745f  :param incident_
-000090b0: 7479 7065 733a 204c 6973 7420 6f66 2043  types: List of C
-000090c0: 7573 746f 6d20 496e 6369 6465 6e74 2054  ustom Incident T
-000090d0: 7970 6520 4e61 6d65 730a 2020 2020 3a70  ype Names.    :p
-000090e0: 6172 616d 2070 6c61 7962 6f6f 6b73 3a20  aram playbooks: 
-000090f0: 4c69 7374 206f 6620 506c 6179 626f 6f6b  List of Playbook
-00009100: 2041 5049 204e 616d 6573 0a20 2020 203a   API Names.    :
-00009110: 7265 7475 726e 3a20 5265 7475 726e 2061  return: Return a
-00009120: 2044 6963 7469 6f6e 6172 7920 6f66 2052   Dictionary of R
-00009130: 6573 696c 6965 6e74 204f 626a 6563 7473  esilient Objects
-00009140: 0a20 2020 203a 7274 7970 653a 2044 6963  .    :rtype: Dic
-00009150: 740a 2020 2020 2222 220a 2020 2020 2320  t.    """.    # 
-00009160: 4465 6570 2063 6f70 7920 7468 6520 6578  Deep copy the ex
-00009170: 706f 7274 2c20 736f 2077 6520 646f 6e27  port, so we don'
-00009180: 7420 6f76 6572 7772 6974 6520 616e 7974  t overwrite anyt
-00009190: 6869 6e67 0a20 2020 206d 696e 6966 6965  hing.    minifie
-000091a0: 645f 6578 706f 7274 203d 2063 6f70 792e  d_export = copy.
-000091b0: 6465 6570 636f 7079 2865 7870 6f72 7429  deepcopy(export)
-000091c0: 0a0a 2020 2020 2320 4966 206e 6f20 6b65  ..    # If no ke
-000091d0: 7973 5f74 6f5f 6b65 6570 2061 7265 2073  ys_to_keep are s
-000091e0: 7065 6369 6669 6564 2c20 7573 6520 7468  pecified, use th
-000091f0: 6573 6520 6465 6661 756c 7473 0a20 2020  ese defaults.   
-00009200: 2023 206b 6579 735f 746f 5f6b 6565 7020   # keys_to_keep 
-00009210: 6973 2075 7365 6420 746f 206b 6565 7020  is used to keep 
-00009220: 7661 6c75 6573 2066 726f 6d20 7468 6520  values from the 
-00009230: 6f72 6967 696e 616c 2065 7870 6f72 740a  original export.
-00009240: 2020 2020 2320 7769 7468 6f75 7420 6265      # without be
-00009250: 696e 6720 6d69 6e69 6669 6564 0a20 2020  ing minified.   
-00009260: 2069 6620 6e6f 7420 6b65 7973 5f74 6f5f   if not keys_to_
-00009270: 6b65 6570 3a0a 2020 2020 2020 2020 6b65  keep:.        ke
-00009280: 7973 5f74 6f5f 6b65 6570 203d 205b 0a20  ys_to_keep = [. 
-00009290: 2020 2020 2020 2020 2020 2022 6578 706f             "expo
-000092a0: 7274 5f64 6174 6522 2c0a 2020 2020 2020  rt_date",.      
-000092b0: 2020 2020 2020 2265 7870 6f72 745f 666f        "export_fo
-000092c0: 726d 6174 5f76 6572 7369 6f6e 222c 0a20  rmat_version",. 
-000092d0: 2020 2020 2020 2020 2020 2022 6964 222c             "id",
-000092e0: 0a20 2020 2020 2020 2020 2020 2022 7365  .            "se
-000092f0: 7276 6572 5f76 6572 7369 6f6e 220a 2020  rver_version".  
-00009300: 2020 2020 2020 5d0a 0a20 2020 2023 2063        ]..    # c
-00009310: 6572 7461 696e 206b 6579 7320 6e65 6564  ertain keys need
-00009320: 2074 6f20 6265 2063 6c65 6172 6564 2c20   to be cleared, 
-00009330: 7261 7468 6572 2074 6861 6e20 7365 7420  rather than set 
-00009340: 746f 2065 6d70 7479 206f 626a 6563 7473  to empty objects
-00009350: 0a20 2020 2023 2073 6f20 6173 206e 6f74  .    # so as not
-00009360: 2074 6f20 7072 6f63 6573 7320 6120 6465   to process a de
-00009370: 6c65 7465 206f 7220 7570 6461 7465 206f  lete or update o
-00009380: 6e20 7468 6520 706c 6174 666f 726d 2077  n the platform w
-00009390: 6865 6e20 7468 650a 2020 2020 2320 6578  hen the.    # ex
-000093a0: 706f 7274 2069 7320 6d6f 6469 6669 6564  port is modified
-000093b0: 2061 6e64 2050 4f53 5465 6420 6261 636b   and POSTed back
-000093c0: 2074 6f20 534f 4152 0a20 2020 206b 6579   to SOAR.    key
-000093d0: 735f 746f 5f63 6c65 6172 203d 205b 0a20  s_to_clear = [. 
-000093e0: 2020 2020 2020 2022 6f76 6572 7269 6465         "override
-000093f0: 7322 0a20 2020 205d 0a0a 2020 2020 2320  s".    ]..    # 
-00009400: 736f 6d65 2069 6e63 6964 656e 7420 7479  some incident ty
-00009410: 7065 7320 6172 6520 7061 7265 6e74 2f63  pes are parent/c
-00009420: 6869 6c64 2e20 5468 6973 2072 6f75 7469  hild. This routi
-00009430: 6e65 2077 696c 6c20 7265 7475 726e 2061  ne will return a
-00009440: 6c6c 2074 6865 2070 6172 656e 7420 696e  ll the parent in
-00009450: 6369 6465 6e74 2074 7970 6573 0a20 2020  cident types.   
-00009460: 2070 6172 656e 745f 6368 696c 645f 696e   parent_child_in
-00009470: 6369 6465 6e74 5f74 7970 6573 203d 2066  cident_types = f
-00009480: 696e 645f 7061 7265 6e74 5f63 6869 6c64  ind_parent_child
-00009490: 5f74 7970 6573 2865 7870 6f72 742c 2022  _types(export, "
-000094a0: 696e 6369 6465 6e74 5f74 7970 6573 222c  incident_types",
-000094b0: 2022 6e61 6d65 222c 2069 6e63 6964 656e   "name", inciden
-000094c0: 745f 7479 7065 7329 0a0a 2020 2020 2320  t_types)..    # 
-000094d0: 5365 7475 7020 7468 6520 6b65 7973 5f74  Setup the keys_t
-000094e0: 6f5f 6d69 6e69 6679 2064 6963 740a 2020  o_minify dict.  
-000094f0: 2020 6b65 7973 5f74 6f5f 6d69 6e69 6679    keys_to_minify
-00009500: 203d 207b 0a20 2020 2020 2020 2022 6d65   = {.        "me
-00009510: 7373 6167 655f 6465 7374 696e 6174 696f  ssage_destinatio
-00009520: 6e73 223a 207b 5265 7369 6c69 656e 744f  ns": {ResilientO
-00009530: 626a 4d61 702e 4d45 5353 4147 455f 4445  bjMap.MESSAGE_DE
-00009540: 5354 494e 4154 494f 4e53 3a20 6d65 7373  STINATIONS: mess
-00009550: 6167 655f 6465 7374 696e 6174 696f 6e73  age_destinations
-00009560: 7d2c 0a20 2020 2020 2020 2022 6675 6e63  },.        "func
-00009570: 7469 6f6e 7322 3a20 7b52 6573 696c 6965  tions": {Resilie
-00009580: 6e74 4f62 6a4d 6170 2e46 554e 4354 494f  ntObjMap.FUNCTIO
-00009590: 4e53 3a20 6675 6e63 7469 6f6e 737d 2c0a  NS: functions},.
-000095a0: 2020 2020 2020 2020 2277 6f72 6b66 6c6f          "workflo
-000095b0: 7773 223a 207b 5265 7369 6c69 656e 744f  ws": {ResilientO
-000095c0: 626a 4d61 702e 574f 524b 464c 4f57 533a  bjMap.WORKFLOWS:
-000095d0: 2077 6f72 6b66 6c6f 7773 7d2c 0a20 2020   workflows},.   
-000095e0: 2020 2020 2022 6163 7469 6f6e 7322 3a20       "actions": 
-000095f0: 7b52 6573 696c 6965 6e74 4f62 6a4d 6170  {ResilientObjMap
-00009600: 2e52 554c 4553 3a20 7275 6c65 737d 2c0a  .RULES: rules},.
-00009610: 2020 2020 2020 2020 2266 6965 6c64 7322          "fields"
-00009620: 3a20 7b22 6578 706f 7274 5f6b 6579 223a  : {"export_key":
-00009630: 2066 6965 6c64 737d 2c0a 2020 2020 2020   fields},.      
-00009640: 2020 2269 6e63 6964 656e 745f 6172 7469    "incident_arti
-00009650: 6661 6374 5f74 7970 6573 223a 207b 5265  fact_types": {Re
-00009660: 7369 6c69 656e 744f 626a 4d61 702e 494e  silientObjMap.IN
-00009670: 4349 4445 4e54 5f41 5254 4946 4143 545f  CIDENT_ARTIFACT_
-00009680: 5459 5045 533a 2061 7274 6966 6163 745f  TYPES: artifact_
-00009690: 7479 7065 737d 2c0a 2020 2020 2020 2020  types},.        
-000096a0: 2274 7970 6573 223a 207b 5265 7369 6c69  "types": {Resili
-000096b0: 656e 744f 626a 4d61 702e 4441 5441 5441  entObjMap.DATATA
-000096c0: 424c 4553 3a20 6461 7461 7461 626c 6573  BLES: datatables
-000096d0: 7d2c 0a20 2020 2020 2020 2022 6175 746f  },.        "auto
-000096e0: 6d61 7469 635f 7461 736b 7322 3a20 7b52  matic_tasks": {R
-000096f0: 6573 696c 6965 6e74 4f62 6a4d 6170 2e54  esilientObjMap.T
-00009700: 4153 4b53 3a20 7461 736b 737d 2c0a 2020  ASKS: tasks},.  
-00009710: 2020 2020 2020 2270 6861 7365 7322 3a20        "phases": 
-00009720: 7b52 6573 696c 6965 6e74 4f62 6a4d 6170  {ResilientObjMap
-00009730: 2e50 4841 5345 533a 2070 6861 7365 737d  .PHASES: phases}
-00009740: 2c0a 2020 2020 2020 2020 2273 6372 6970  ,.        "scrip
-00009750: 7473 223a 207b 5265 7369 6c69 656e 744f  ts": {ResilientO
-00009760: 626a 4d61 702e 5343 5249 5054 533a 2073  bjMap.SCRIPTS: s
-00009770: 6372 6970 7473 7d2c 0a20 2020 2020 2020  cripts},.       
-00009780: 2022 696e 6369 6465 6e74 5f74 7970 6573   "incident_types
-00009790: 223a 207b 5265 7369 6c69 656e 744f 626a  ": {ResilientObj
-000097a0: 4d61 702e 494e 4349 4445 4e54 5f54 5950  Map.INCIDENT_TYP
-000097b0: 4553 3a20 7061 7265 6e74 5f63 6869 6c64  ES: parent_child
-000097c0: 5f69 6e63 6964 656e 745f 7479 7065 737d  _incident_types}
-000097d0: 2c0a 2020 2020 2020 2020 2270 6c61 7962  ,.        "playb
-000097e0: 6f6f 6b73 223a 207b 5265 7369 6c69 656e  ooks": {Resilien
-000097f0: 744f 626a 4d61 702e 504c 4159 424f 4f4b  tObjMap.PLAYBOOK
-00009800: 533a 2070 6c61 7962 6f6f 6b73 7d0a 2020  S: playbooks}.  
-00009810: 2020 7d0a 0a20 2020 2066 6f72 206b 6579    }..    for key
-00009820: 2069 6e20 6d69 6e69 6669 6564 5f65 7870   in minified_exp
-00009830: 6f72 742e 6b65 7973 2829 3a0a 0a20 2020  ort.keys():..   
-00009840: 2020 2020 2023 2049 6620 7765 206b 6565       # If we kee
-00009850: 7020 7468 6973 206f 6e65 2c20 736b 6970  p this one, skip
-00009860: 0a20 2020 2020 2020 2069 6620 6b65 7920  .        if key 
-00009870: 696e 206b 6579 735f 746f 5f6b 6565 703a  in keys_to_keep:
-00009880: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00009890: 7469 6e75 650a 0a20 2020 2020 2020 2023  tinue..        #
-000098a0: 2049 6620 7765 2061 7265 2074 6f20 6d69   If we are to mi
-000098b0: 6e69 6679 2069 740a 2020 2020 2020 2020  nify it.        
-000098c0: 656c 6966 206b 6579 2069 6e20 6b65 7973  elif key in keys
-000098d0: 5f74 6f5f 6d69 6e69 6679 2e6b 6579 7328  _to_minify.keys(
-000098e0: 293a 0a0a 2020 2020 2020 2020 2020 2020  ):..            
-000098f0: 2320 4765 7420 7468 6520 6174 7472 6962  # Get the attrib
-00009900: 7574 655f 6e61 6d65 2074 6f20 6d61 7463  ute_name to matc
-00009910: 6820 6f6e 2028 6e6f 726d 616c 6c79 2027  h on (normally '
-00009920: 6e61 6d65 272f 2770 726f 6772 616d 6d61  name'/'programma
-00009930: 7469 635f 6e61 6d65 272f 2765 7870 6f72  tic_name'/'expor
-00009940: 745f 6b65 7927 290a 2020 2020 2020 2020  t_key').        
-00009950: 2020 2020 6174 7472 6962 7574 655f 6e61      attribute_na
-00009960: 6d65 203d 206c 6973 7428 6b65 7973 5f74  me = list(keys_t
-00009970: 6f5f 6d69 6e69 6679 5b6b 6579 5d2e 6b65  o_minify[key].ke
-00009980: 7973 2829 295b 305d 0a0a 2020 2020 2020  ys())[0]..      
-00009990: 2020 2020 2020 7661 6c75 6573 203d 206b        values = k
-000099a0: 6579 735f 746f 5f6d 696e 6966 795b 6b65  eys_to_minify[ke
-000099b0: 795d 5b61 7474 7269 6275 7465 5f6e 616d  y][attribute_nam
-000099c0: 655d 0a20 2020 2020 2020 2020 2020 2023  e].            #
-000099d0: 2073 7472 6970 206f 7574 2065 7874 7261   strip out extra
-000099e0: 2073 7061 6365 7320 6672 6f6d 2074 6865   spaces from the
-000099f0: 2061 7474 7269 6275 7465 2028 6965 2044   attribute (ie D
-00009a00: 6973 706c 6179 206e 616d 6520 666f 7220  isplay name for 
-00009a10: 5275 6c65 732c 2053 6372 6970 7473 2c20  Rules, Scripts, 
-00009a20: 6574 632e 290a 2020 2020 2020 2020 2020  etc.).          
-00009a30: 2020 7661 6c75 6573 203d 205b 6e61 6d65    values = [name
-00009a40: 2e73 7472 6970 2829 2066 6f72 206e 616d  .strip() for nam
-00009a50: 6520 696e 2076 616c 7565 735d 0a0a 2020  e in values]..  
-00009a60: 2020 2020 2020 2020 2020 6f62 6a20 3d20            obj = 
-00009a70: 6d69 6e69 6669 6564 5f65 7870 6f72 742e  minified_export.
-00009a80: 6765 7428 6b65 7929 0a0a 2020 2020 2020  get(key)..      
-00009a90: 2020 2020 2020 6966 206f 626a 3a0a 2020        if obj:.  
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00009ab0: 7220 6461 7461 2069 6e20 6c69 7374 286f  r data in list(o
-00009ac0: 626a 293a 0a0a 2020 2020 2020 2020 2020  bj):..          
-00009ad0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00009ae0: 2064 6174 612e 6765 7428 6174 7472 6962   data.get(attrib
-00009af0: 7574 655f 6e61 6d65 293a 0a20 2020 2020  ute_name):.     
-00009b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b10: 2020 204c 4f47 2e77 6172 6e69 6e67 2822     LOG.warning("
-00009b20: 4e6f 2025 7320 696e 2025 7322 2c20 6174  No %s in %s", at
-00009b30: 7472 6962 7574 655f 6e61 6d65 2c20 6b65  tribute_name, ke
-00009b40: 7929 0a0a 2020 2020 2020 2020 2020 2020  y)..            
-00009b50: 2020 2020 2020 2020 2320 7374 7269 7020          # strip 
-00009b60: 6f75 7420 6578 7472 6120 7370 6163 6573  out extra spaces
-00009b70: 2066 726f 6d20 7468 6520 6174 7472 6962   from the attrib
-00009b80: 7574 6520 2869 6520 4469 7370 6c61 7920  ute (ie Display 
-00009b90: 6e61 6d65 2066 6f72 2052 756c 6573 2c20  name for Rules, 
-00009ba0: 5363 7269 7074 732c 2065 7463 2e29 0a20  Scripts, etc.). 
-00009bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bc0: 2020 2023 2049 6620 7468 6973 2052 6573     # If this Res
-00009bd0: 696c 6965 6e74 204f 626a 6563 7420 6973  ilient Object is
-00009be0: 206e 6f74 2069 6e20 6f75 7220 6d69 6e69   not in our mini
-00009bf0: 6679 206c 6973 742c 2072 656d 6f76 6520  fy list, remove 
-00009c00: 6974 0a20 2020 2020 2020 2020 2020 2020  it.             
-00009c10: 2020 2020 2020 2069 6620 6e6f 7420 6461         if not da
-00009c20: 7461 2e67 6574 2861 7474 7269 6275 7465  ta.get(attribute
-00009c30: 5f6e 616d 652c 2022 2229 2e73 7472 6970  _name, "").strip
-00009c40: 2829 2069 6e20 7661 6c75 6573 3a0a 2020  () in values:.  
-00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c60: 2020 2020 2020 6d69 6e69 6669 6564 5f65        minified_e
-00009c70: 7870 6f72 745b 6b65 795d 2e72 656d 6f76  xport[key].remov
-00009c80: 6528 6461 7461 290a 0a20 2020 2020 2020  e(data)..       
-00009c90: 2065 6c69 6620 6b65 7920 696e 206b 6579   elif key in key
-00009ca0: 735f 746f 5f63 6c65 6172 3a0a 2020 2020  s_to_clear:.    
-00009cb0: 2020 2020 2020 2020 6d69 6e69 6669 6564          minified
-00009cc0: 5f65 7870 6f72 745b 6b65 795d 203d 204e  _export[key] = N
-00009cd0: 6f6e 650a 0a20 2020 2020 2020 2065 6c69  one..        eli
-00009ce0: 6620 6973 696e 7374 616e 6365 286d 696e  f isinstance(min
-00009cf0: 6966 6965 645f 6578 706f 7274 5b6b 6579  ified_export[key
-00009d00: 5d2c 206c 6973 7429 3a0a 2020 2020 2020  ], list):.      
-00009d10: 2020 2020 2020 6d69 6e69 6669 6564 5f65        minified_e
-00009d20: 7870 6f72 745b 6b65 795d 203d 205b 5d0a  xport[key] = [].
-00009d30: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
-00009d40: 696e 7374 616e 6365 286d 696e 6966 6965  instance(minifie
-00009d50: 645f 6578 706f 7274 5b6b 6579 5d2c 2064  d_export[key], d
-00009d60: 6963 7429 3a0a 2020 2020 2020 2020 2020  ict):.          
-00009d70: 2020 6d69 6e69 6669 6564 5f65 7870 6f72    minified_expor
-00009d80: 745b 6b65 795d 203d 207b 7d0a 0a20 2020  t[key] = {}..   
-00009d90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00009da0: 2020 2020 2020 206d 696e 6966 6965 645f         minified_
-00009db0: 6578 706f 7274 5b6b 6579 5d20 3d20 4e6f  export[key] = No
-00009dc0: 6e65 0a0a 2020 2020 2320 4164 6420 6465  ne..    # Add de
-00009dd0: 6661 756c 7420 696e 6369 6465 6e74 5f74  fault incident_t
-00009de0: 7970 652e 204e 6565 6465 6420 666f 7220  ype. Needed for 
-00009df0: 6576 6572 7920 496d 706f 7274 0a20 2020  every Import.   
-00009e00: 2069 6620 6d69 6e69 6669 6564 5f65 7870   if minified_exp
-00009e10: 6f72 742e 6765 7428 2269 6e63 6964 656e  ort.get("inciden
-00009e20: 745f 7479 7065 7322 293a 0a20 2020 2020  t_types"):.     
-00009e30: 2020 206d 696e 6966 6965 645f 6578 706f     minified_expo
-00009e40: 7274 5b22 696e 6369 6465 6e74 5f74 7970  rt["incident_typ
-00009e50: 6573 225d 2e61 7070 656e 6428 4445 4641  es"].append(DEFA
-00009e60: 554c 545f 494e 4349 4445 4e54 5f54 5950  ULT_INCIDENT_TYP
-00009e70: 4529 0a20 2020 2065 6c73 653a 0a20 2020  E).    else:.   
-00009e80: 2020 2020 206d 696e 6966 6965 645f 6578       minified_ex
-00009e90: 706f 7274 5b22 696e 6369 6465 6e74 5f74  port["incident_t
-00009ea0: 7970 6573 225d 203d 205b 4445 4641 554c  ypes"] = [DEFAUL
-00009eb0: 545f 494e 4349 4445 4e54 5f54 5950 455d  T_INCIDENT_TYPE]
-00009ec0: 0a0a 2020 2020 2320 4966 206e 6f20 4375  ..    # If no Cu
-00009ed0: 7374 6f6d 2049 6e63 6964 656e 7420 4669  stom Incident Fi
-00009ee0: 656c 6473 2061 7265 2069 6e20 7468 6520  elds are in the 
-00009ef0: 6578 706f 7274 2c20 6164 6420 7468 6973  export, add this
-00009f00: 2064 6566 6175 6c74 2e0a 2020 2020 2320   default..    # 
-00009f10: 416e 2069 6d70 6f72 7420 6e65 6564 7320  An import needs 
-00009f20: 6174 206c 6561 7374 2031 2049 6e63 6964  at least 1 Incid
-00009f30: 656e 7420 4669 656c 640a 2020 2020 6966  ent Field.    if
-00009f40: 2022 696e 6369 6465 6e74 2f22 206e 6f74   "incident/" not
-00009f50: 2069 6e20 6669 656c 6473 3a0a 2020 2020   in fields:.    
-00009f60: 2020 2020 6d69 6e69 6669 6564 5f65 7870      minified_exp
-00009f70: 6f72 745b 2266 6965 6c64 7322 5d2e 6170  ort["fields"].ap
-00009f80: 7065 6e64 2844 4546 4155 4c54 5f49 4e43  pend(DEFAULT_INC
-00009f90: 4944 454e 545f 4649 454c 4429 0a0a 2020  IDENT_FIELD)..  
-00009fa0: 2020 2320 436c 6561 6e20 6f75 7420 616e    # Clean out an
-00009fb0: 7920 7069 6920 7661 6c75 6573 2077 6974  y pii values wit
-00009fc0: 6820 6b65 7973 2069 6e63 6c75 6465 6420  h keys included 
-00009fd0: 696e 2070 6969 5f6b 6579 5f6c 6973 740a  in pii_key_list.
-00009fe0: 2020 2020 7069 695f 6b65 795f 6c69 7374      pii_key_list
-00009ff0: 203d 205b 2263 7265 6174 6f72 222c 2022   = ["creator", "
-0000a000: 6372 6561 746f 725f 6964 225d 0a20 2020  creator_id"].   
-0000a010: 206d 696e 6966 6965 645f 6578 706f 7274   minified_export
-0000a020: 203d 2072 6d5f 7069 6928 7069 695f 6b65   = rm_pii(pii_ke
-0000a030: 795f 6c69 7374 2c20 6d69 6e69 6669 6564  y_list, minified
-0000a040: 5f65 7870 6f72 7429 0a0a 2020 2020 6d69  _export)..    mi
-0000a050: 6e69 6669 6564 5f65 7870 6f72 7420 3d20  nified_export = 
-0000a060: 7265 6d6f 7665 5f74 6167 286d 696e 6966  remove_tag(minif
-0000a070: 6965 645f 6578 706f 7274 290a 0a20 2020  ied_export)..   
-0000a080: 2072 6574 7572 6e20 6d69 6e69 6669 6564   return minified
-0000a090: 5f65 7870 6f72 740a 0a0a 6465 6620 726d  _export...def rm
-0000a0a0: 5f70 6969 2870 6969 5f6b 6579 5f6c 6973  _pii(pii_key_lis
-0000a0b0: 742c 2065 7870 6f72 7429 3a0a 2020 2020  t, export):.    
-0000a0c0: 2222 220a 2020 2020 5265 6d6f 7665 2061  """.    Remove a
-0000a0d0: 6e79 206b 6579 7320 6672 6f6d 2027 6578  ny keys from 'ex
-0000a0e0: 706f 7274 2720 7468 6174 2061 7265 2069  port' that are i
-0000a0f0: 6e20 2770 6969 5f6b 6579 5f6c 6973 7427  n 'pii_key_list'
-0000a100: 2e0a 2020 2020 5265 6375 7273 6976 656c  ..    Recursivel
-0000a110: 7920 7365 6172 6368 6573 2074 6865 2065  y searches the e
-0000a120: 7870 6f72 7420 6f62 6a65 6374 2e0a 2020  xport object..  
-0000a130: 2020 0a20 2020 203a 7061 7261 6d20 7069    .    :param pi
-0000a140: 695f 6b65 795f 6c69 7374 3a20 6c69 7374  i_key_list: list
-0000a150: 206f 6620 7374 7220 6b65 7973 2074 6f20   of str keys to 
-0000a160: 6265 2072 656d 6f76 6564 2066 726f 6d20  be removed from 
-0000a170: 2765 7870 6f72 7427 2e20 6578 3a20 5b22  'export'. ex: ["
-0000a180: 6372 6561 746f 7222 2c20 2263 7265 6174  creator", "creat
-0000a190: 6f72 5f69 6422 5d0a 2020 2020 3a74 7970  or_id"].    :typ
-0000a1a0: 6520 7069 695f 6b65 795f 6c69 7374 3a20  e pii_key_list: 
-0000a1b0: 5b73 7472 5d0a 2020 2020 3a70 6172 616d  [str].    :param
-0000a1c0: 2065 7870 6f72 743a 2074 6865 2072 6573   export: the res
-0000a1d0: 756c 7420 6f66 2063 616c 6c69 6e67 2067  ult of calling g
-0000a1e0: 6574 5f6c 6174 6573 745f 6f72 675f 6578  et_latest_org_ex
-0000a1f0: 706f 7274 2829 206f 7220 6d69 6e69 6669  port() or minifi
-0000a200: 6564 5f65 7870 6f72 7420 6672 6f6d 2063  ed_export from c
-0000a210: 616c 6c69 6e67 206d 696e 6966 795f 6578  alling minify_ex
-0000a220: 706f 7274 2829 0a20 2020 203a 7479 7065  port().    :type
-0000a230: 2065 7870 6f72 743a 2044 6963 740a 2020   export: Dict.  
-0000a240: 2020 3a72 6574 7572 6e3a 206d 6f64 6966    :return: modif
-0000a250: 6965 6420 6578 706f 7274 2077 6974 6820  ied export with 
-0000a260: 616e 7920 7069 6920 6b65 7973 2072 656d  any pii keys rem
-0000a270: 6f76 6564 0a20 2020 203a 7274 7970 653a  oved.    :rtype:
-0000a280: 2044 6963 740a 2020 2020 2222 220a 0a20   Dict.    """.. 
-0000a290: 2020 2069 6620 6578 706f 7274 3a0a 2020     if export:.  
-0000a2a0: 2020 2020 2020 6578 706f 7274 5f63 6f70        export_cop
-0000a2b0: 7920 3d20 6578 706f 7274 2e63 6f70 7928  y = export.copy(
-0000a2c0: 290a 0a20 2020 2020 2020 2066 6f72 206b  )..        for k
-0000a2d0: 6579 2069 6e20 6c69 7374 2865 7870 6f72  ey in list(expor
-0000a2e0: 745f 636f 7079 2e6b 6579 7328 2929 3a0a  t_copy.keys()):.
-0000a2f0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0000a300: 656e 7420 3d20 6578 706f 7274 5f63 6f70  ent = export_cop
-0000a310: 795b 6b65 795d 0a0a 2020 2020 2020 2020  y[key]..        
-0000a320: 2020 2020 2320 6966 206b 6579 2069 7320      # if key is 
-0000a330: 696e 2070 6969 5f6c 6973 7420 746f 2072  in pii_list to r
-0000a340: 656d 6f76 652c 2064 656c 6574 6520 656e  emove, delete en
-0000a350: 7472 7920 696e 2070 6179 6c6f 6164 5f72  try in payload_r
-0000a360: 6573 756c 740a 2020 2020 2020 2020 2020  esult.          
-0000a370: 2020 6966 206b 6579 2069 6e20 7069 695f    if key in pii_
-0000a380: 6b65 795f 6c69 7374 3a0a 2020 2020 2020  key_list:.      
-0000a390: 2020 2020 2020 2020 2020 6465 6c20 6578            del ex
-0000a3a0: 706f 7274 5f63 6f70 795b 6b65 795d 0a20  port_copy[key]. 
-0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000a3c0: 6f6e 7469 6e75 650a 0a20 2020 2020 2020  ontinue..       
-0000a3d0: 2020 2020 2023 2069 6620 6b65 7920 7761       # if key wa
-0000a3e0: 736e 2774 2069 6e20 7069 695f 6c69 7374  sn't in pii_list
-0000a3f0: 2c20 636f 6e74 696e 7565 2073 6561 7263  , continue searc
-0000a400: 6869 6e67 2072 6563 7572 7369 7665 6c79  hing recursively
-0000a410: 2066 6f72 2064 6963 7469 6f6e 6172 6965   for dictionarie
-0000a420: 7320 616e 6420 7363 7275 6262 696e 6720  s and scrubbing 
-0000a430: 7069 690a 2020 2020 2020 2020 2020 2020  pii.            
-0000a440: 6966 2069 7369 6e73 7461 6e63 6528 636f  if isinstance(co
-0000a450: 6e74 656e 742c 2064 6963 7429 3a0a 2020  ntent, dict):.  
-0000a460: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-0000a470: 706f 7274 5f63 6f70 795b 6b65 795d 203d  port_copy[key] =
-0000a480: 2072 6d5f 7069 6928 7069 695f 6b65 795f   rm_pii(pii_key_
-0000a490: 6c69 7374 2c20 636f 6e74 656e 7429 0a20  list, content). 
-0000a4a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000a4b0: 6973 696e 7374 616e 6365 2863 6f6e 7465  isinstance(conte
-0000a4c0: 6e74 2c20 6c69 7374 293a 0a20 2020 2020  nt, list):.     
-0000a4d0: 2020 2020 2020 2020 2020 2023 2072 6563             # rec
-0000a4e0: 7265 6174 6573 2074 6865 206c 6973 7420  reates the list 
-0000a4f0: 7768 6572 6520 616e 7920 6469 6374 2065  where any dict e
-0000a500: 6c65 6d65 6e74 7320 6f66 2074 6865 206c  lements of the l
-0000a510: 6973 7420 6172 6520 7265 6375 7273 6976  ist are recursiv
-0000a520: 656c 7920 7363 7275 6262 6564 0a20 2020  ely scrubbed.   
-0000a530: 2020 2020 2020 2020 2020 2020 2023 2069               # i
-0000a540: 6620 6c69 7374 2069 7465 6d20 6973 206e  f list item is n
-0000a550: 6f74 2061 2064 6963 7469 6f6e 6172 792c  ot a dictionary,
-0000a560: 2064 6f6e 2774 200a 2020 2020 2020 2020   don't .        
-0000a570: 2020 2020 2020 2020 6578 706f 7274 5f63          export_c
-0000a580: 6f70 795b 6b65 795d 203d 205b 726d 5f70  opy[key] = [rm_p
-0000a590: 6969 2870 6969 5f6b 6579 5f6c 6973 742c  ii(pii_key_list,
-0000a5a0: 206c 6973 745f 636f 6e74 656e 7429 2069   list_content) i
-0000a5b0: 6620 6973 696e 7374 616e 6365 286c 6973  f isinstance(lis
-0000a5c0: 745f 636f 6e74 656e 742c 2064 6963 7429  t_content, dict)
-0000a5d0: 2065 6c73 6520 6c69 7374 5f63 6f6e 7465   else list_conte
-0000a5e0: 6e74 2066 6f72 206c 6973 745f 636f 6e74  nt for list_cont
-0000a5f0: 656e 7420 696e 2063 6f6e 7465 6e74 5d0a  ent in content].
-0000a600: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000a610: 6578 706f 7274 5f63 6f70 790a 2020 2020  export_copy.    
-0000a620: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
-0000a630: 7475 726e 2065 7870 6f72 740a 0a0a 6465  turn export...de
-0000a640: 6620 6669 6e64 5f70 6172 656e 745f 6368  f find_parent_ch
-0000a650: 696c 645f 7479 7065 7328 6578 706f 7274  ild_types(export
-0000a660: 2c20 6f62 6a65 6374 5f74 7970 652c 2061  , object_type, a
-0000a670: 7474 7269 6275 7465 5f6e 616d 652c 206e  ttribute_name, n
-0000a680: 616d 655f 6c69 7374 293a 0a20 2020 2022  ame_list):.    "
-0000a690: 2222 5b67 6574 2061 6c6c 2070 6172 656e  ""[get all paren
-0000a6a0: 7420 6f62 6a65 6374 7320 286c 696b 6520  t objects (like 
-0000a6b0: 696e 6369 6465 6e74 5f74 7970 6573 295d  incident_types)]
-0000a6c0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-0000a6d0: 2020 2020 6578 706f 7274 2028 5b64 6963      export ([dic
-0000a6e0: 745d 293a 205b 6578 706f 7274 2066 696c  t]): [export fil
-0000a6f0: 6520 746f 2070 6172 7365 5d0a 2020 2020  e to parse].    
-0000a700: 2020 2020 6f62 6a65 6374 5f74 7970 6520      object_type 
-0000a710: 285b 7374 725d 293a 205b 6865 6972 6172  ([str]): [heirar
-0000a720: 6368 7920 6f66 206f 626a 6563 7473 2074  chy of objects t
-0000a730: 6f20 7061 7273 655d 0a20 2020 2020 2020  o parse].       
-0000a740: 2061 7474 7269 6275 7465 5f6e 616d 6520   attribute_name 
-0000a750: 285b 7374 725d 293a 205b 6e61 6d65 206f  ([str]): [name o
-0000a760: 6620 6669 656c 6420 746f 2063 6865 636b  f field to check
-0000a770: 2066 6f72 5d0a 2020 2020 2020 2020 6e61   for].        na
-0000a780: 6d65 5f6c 6973 7420 285b 6c69 7374 5d29  me_list ([list])
-0000a790: 3a20 5b6c 6973 7420 6f66 206f 626a 6563  : [list of objec
-0000a7a0: 7473 2074 6f20 7361 6d65 5d0a 2020 2020  ts to same].    
-0000a7b0: 2222 220a 0a20 2020 2065 7874 656e 6465  """..    extende
-0000a7c0: 645f 6e61 6d65 5f6c 6973 7420 3d20 6e61  d_name_list = na
-0000a7d0: 6d65 5f6c 6973 745b 3a5d 0a0a 2020 2020  me_list[:]..    
-0000a7e0: 6966 2065 7870 6f72 742e 6765 7428 6f62  if export.get(ob
-0000a7f0: 6a65 6374 5f74 7970 6529 3a0a 2020 2020  ject_type):.    
-0000a800: 2020 2020 7365 6374 696f 6e20 3d20 6578      section = ex
-0000a810: 706f 7274 2e67 6574 286f 626a 6563 745f  port.get(object_
-0000a820: 7479 7065 290a 2020 2020 2020 2020 666f  type).        fo
-0000a830: 7220 6e61 6d65 2069 6e20 6e61 6d65 5f6c  r name in name_l
-0000a840: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
-0000a850: 2066 6f72 2069 7465 6d20 696e 2073 6563   for item in sec
-0000a860: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-0000a870: 2020 2020 6966 2069 7465 6d2e 6765 7428      if item.get(
-0000a880: 6174 7472 6962 7574 655f 6e61 6d65 2920  attribute_name) 
-0000a890: 3d3d 206e 616d 653a 0a20 2020 2020 2020  == name:.       
-0000a8a0: 2020 2020 2020 2020 2020 2069 6620 6974             if it
-0000a8b0: 656d 2e67 6574 2827 7061 7265 6e74 5f69  em.get('parent_i
-0000a8c0: 6427 293a 0a20 2020 2020 2020 2020 2020  d'):.           
-0000a8d0: 2020 2020 2020 2020 2020 2023 2061 6464             # add
-0000a8e0: 2074 6865 2070 6172 656e 7420 6869 6572   the parent hier
-0000a8f0: 6172 6368 790a 2020 2020 2020 2020 2020  archy.          
-0000a900: 2020 2020 2020 2020 2020 2020 7061 7265              pare
-0000a910: 6e74 5f6c 6973 7420 3d20 6669 6e64 5f70  nt_list = find_p
-0000a920: 6172 656e 745f 6368 696c 645f 7479 7065  arent_child_type
-0000a930: 7328 6578 706f 7274 2c20 6f62 6a65 6374  s(export, object
-0000a940: 5f74 7970 652c 2061 7474 7269 6275 7465  _type, attribute
-0000a950: 5f6e 616d 652c 205b 6974 656d 2e67 6574  _name, [item.get
-0000a960: 2827 7061 7265 6e74 5f69 6427 295d 290a  ('parent_id')]).
-0000a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a980: 2020 2020 2020 6578 7465 6e64 6564 5f6e        extended_n
-0000a990: 616d 655f 6c69 7374 2e65 7874 656e 6428  ame_list.extend(
-0000a9a0: 7061 7265 6e74 5f6c 6973 7429 0a0a 2020  parent_list)..  
-0000a9b0: 2020 7265 7475 726e 206c 6973 7428 7365    return list(se
-0000a9c0: 7428 6578 7465 6e64 6564 5f6e 616d 655f  t(extended_name_
-0000a9d0: 6c69 7374 2929 0a0a 0a64 6566 206c 6f61  list))...def loa
-0000a9e0: 645f 7079 5f6d 6f64 756c 6528 7061 7468  d_py_module(path
-0000a9f0: 5f70 7974 686f 6e5f 6669 6c65 2c20 6d6f  _python_file, mo
-0000aa00: 6475 6c65 5f6e 616d 6529 3a0a 2020 2020  dule_name):.    
-0000aa10: 2222 220a 2020 2020 5265 7475 726e 2074  """.    Return t
-0000aa20: 6865 2070 6174 685f 7079 7468 6f6e 5f66  he path_python_f
-0000aa30: 696c 6520 6173 2061 2050 7974 686f 6e20  ile as a Python 
-0000aa40: 4d6f 6475 6c65 2e0a 2020 2020 5765 2063  Module..    We c
-0000aa50: 616e 2074 6865 6e20 6163 6365 7373 2069  an then access i
-0000aa60: 7420 6d65 7468 6f64 7320 6c69 6b65 3a0a  t methods like:.
-0000aa70: 0a20 2020 2020 2020 203e 2072 6573 756c  .        > resul
-0000aa80: 7420 3d20 7079 5f6d 6f64 756c 652e 736f  t = py_module.so
-0000aa90: 6d65 5f6d 6574 686f 645f 696e 5f6d 6f64  me_method_in_mod
-0000aaa0: 756c 6528 290a 0a20 2020 203a 7061 7261  ule()..    :para
-0000aab0: 6d20 7061 7468 5f70 7974 686f 6e5f 6669  m path_python_fi
-0000aac0: 6c65 3a20 5061 7468 2074 6f20 7468 6520  le: Path to the 
-0000aad0: 6669 6c65 2074 6861 7420 636f 6e74 6169  file that contai
-0000aae0: 6e73 2074 6865 206d 6f64 756c 650a 2020  ns the module.  
-0000aaf0: 2020 3a70 6172 616d 206d 6f64 756c 655f    :param module_
-0000ab00: 6e61 6d65 3a20 4973 206e 6f72 6d61 6c6c  name: Is normall
-0000ab10: 7920 7468 6520 6669 6c65 206e 616d 6520  y the file name 
-0000ab20: 7769 7468 6f75 7420 7468 6520 2e70 790a  without the .py.
-0000ab30: 2020 2020 3a72 6574 7572 6e3a 2054 6865      :return: The
-0000ab40: 2050 7974 686f 6e20 4d6f 6475 6c65 2066   Python Module f
-0000ab50: 6f75 6e64 0a20 2020 203a 7274 7970 653a  ound.    :rtype:
-0000ab60: 206d 6f64 756c 650a 2020 2020 2222 220a   module.    """.
-0000ab70: 2020 2020 2320 496e 7365 7274 2074 6865      # Insert the
-0000ab80: 2070 6172 656e 7420 6469 7220 6f66 2070   parent dir of p
-0000ab90: 6174 685f 7079 7468 6f6e 5f66 696c 6520  ath_python_file 
-0000aba0: 746f 2074 6865 2073 7461 7274 206f 6620  to the start of 
-0000abb0: 6f75 7220 5079 7468 6f6e 2050 4154 4820  our Python PATH 
-0000abc0: 6174 2072 756e 7469 6d65 0a20 2020 2070  at runtime.    p
-0000abd0: 6174 685f 7061 7265 6e74 5f64 6972 203d  ath_parent_dir =
-0000abe0: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
-0000abf0: 2870 6174 685f 7079 7468 6f6e 5f66 696c  (path_python_fil
-0000ac00: 6529 0a20 2020 2073 7973 2e70 6174 682e  e).    sys.path.
-0000ac10: 696e 7365 7274 2830 2c20 7061 7468 5f70  insert(0, path_p
-0000ac20: 6172 656e 745f 6469 7229 0a0a 2020 2020  arent_dir)..    
-0000ac30: 2320 496d 706f 7274 2074 6865 206d 6f64  # Import the mod
-0000ac40: 756c 650a 2020 2020 7079 5f6d 6f64 756c  ule.    py_modul
-0000ac50: 6520 3d20 696d 706f 7274 6c69 622e 696d  e = importlib.im
-0000ac60: 706f 7274 5f6d 6f64 756c 6528 6d6f 6475  port_module(modu
-0000ac70: 6c65 5f6e 616d 6529 0a0a 2020 2020 2320  le_name)..    # 
-0000ac80: 5265 6c6f 6164 2074 6865 206d 6f64 756c  Reload the modul
-0000ac90: 6520 736f 2077 6520 6765 7420 7468 6520  e so we get the 
-0000aca0: 6c61 7465 7374 206f 6e65 0a20 2020 2023  latest one.    #
-0000acb0: 2049 6620 7765 2064 6f20 6e6f 7420 7265   If we do not re
-0000acc0: 6c6f 6164 2c20 6361 6e20 6765 7420 7374  load, can get st
-0000acd0: 616c 6520 7265 7375 6c74 7320 6966 0a20  ale results if. 
-0000ace0: 2020 2023 2074 6869 7320 6d65 7468 6f64     # this method
-0000acf0: 2069 7320 6361 6c6c 6564 206d 6f72 6520   is called more 
-0000ad00: 7468 656e 206f 6e63 650a 2020 2020 7265  then once.    re
-0000ad10: 6c6f 6164 2870 795f 6d6f 6475 6c65 290a  load(py_module).
-0000ad20: 0a20 2020 2023 2052 656d 6f76 6520 7468  .    # Remove th
-0000ad30: 6520 7061 7468 2066 726f 6d20 5059 5448  e path from PYTH
-0000ad40: 4f4e 5041 5448 0a20 2020 2073 7973 2e70  ONPATH.    sys.p
-0000ad50: 6174 682e 7265 6d6f 7665 2870 6174 685f  ath.remove(path_
-0000ad60: 7061 7265 6e74 5f64 6972 290a 0a20 2020  parent_dir)..   
-0000ad70: 2072 6574 7572 6e20 7079 5f6d 6f64 756c   return py_modul
-0000ad80: 650a 0a0a 6465 6620 7265 6e61 6d65 5f74  e...def rename_t
-0000ad90: 6f5f 6261 6b5f 6669 6c65 2870 6174 685f  o_bak_file(path_
-0000ada0: 6375 7272 656e 745f 6669 6c65 2c20 7061  current_file, pa
-0000adb0: 7468 5f64 6566 6175 6c74 5f66 696c 653d  th_default_file=
-0000adc0: 4e6f 6e65 293a 0a20 2020 2022 2222 5265  None):.    """Re
-0000add0: 6e61 6d65 7320 7061 7468 5f63 7572 7265  names path_curre
-0000ade0: 6e74 5f66 696c 6520 7769 7468 2061 2070  nt_file with a p
-0000adf0: 6f73 7466 6978 6564 2074 696d 6573 7461  ostfixed timesta
-0000ae00: 6d70 2e0a 2020 2020 4966 2070 6174 685f  mp..    If path_
-0000ae10: 6465 6661 756c 745f 6669 6c65 2069 7320  default_file is 
-0000ae20: 7072 6f76 6964 6564 2c20 7061 7468 5f63  provided, path_c
-0000ae30: 7572 7265 6e74 5f66 696c 6520 6973 206f  urrent_file is o
-0000ae40: 6e6c 790a 2020 2020 7265 6e61 6d65 6420  nly.    renamed 
-0000ae50: 6966 2074 6865 2064 6566 6175 6c74 2061  if the default a
-0000ae60: 6e64 2063 7572 7265 6e74 2066 696c 6520  nd current file 
-0000ae70: 6172 6520 6469 6666 6572 656e 7422 2222  are different"""
-0000ae80: 0a20 2020 2069 6620 6e6f 7420 6f73 2e70  .    if not os.p
-0000ae90: 6174 682e 6973 6669 6c65 2870 6174 685f  ath.isfile(path_
-0000aea0: 6375 7272 656e 745f 6669 6c65 293a 0a20  current_file):. 
-0000aeb0: 2020 2020 2020 204c 4f47 2e77 6172 6e69         LOG.warni
-0000aec0: 6e67 2822 4e6f 2062 6163 6b75 7020 6669  ng("No backup fi
-0000aed0: 6c65 2063 7265 6174 6564 2064 7565 2074  le created due t
-0000aee0: 6f20 6669 6c65 206d 6973 7369 6e67 3a20  o file missing: 
-0000aef0: 2573 222c 2070 6174 685f 6375 7272 656e  %s", path_curren
-0000af00: 745f 6669 6c65 290a 2020 2020 2020 2020  t_file).        
-0000af10: 7265 7475 726e 2070 6174 685f 6375 7272  return path_curr
-0000af20: 656e 745f 6669 6c65 0a0a 2020 2020 6966  ent_file..    if
-0000af30: 2070 6174 685f 6465 6661 756c 745f 6669   path_default_fi
-0000af40: 6c65 2069 7320 6e6f 7420 4e6f 6e65 2061  le is not None a
-0000af50: 6e64 206e 6f74 206f 732e 7061 7468 2e69  nd not os.path.i
-0000af60: 7366 696c 6528 7061 7468 5f64 6566 6175  sfile(path_defau
-0000af70: 6c74 5f66 696c 6529 3a0a 2020 2020 2020  lt_file):.      
-0000af80: 2020 7261 6973 6520 494f 4572 726f 7228    raise IOError(
-0000af90: 2244 6566 6175 6c74 2066 696c 6520 746f  "Default file to
-0000afa0: 2063 6f6d 7061 7265 2074 6f20 646f 6573   compare to does
-0000afb0: 206e 6f74 2065 7869 7374 2061 743a 207b   not exist at: {
-0000afc0: 307d 222e 666f 726d 6174 2870 6174 685f  0}".format(path_
-0000afd0: 6465 6661 756c 745f 6669 6c65 2929 0a0a  default_file))..
-0000afe0: 2020 2020 6e65 775f 6669 6c65 5f6e 616d      new_file_nam
-0000aff0: 6520 3d20 227b 307d 2d7b 317d 2e62 616b  e = "{0}-{1}.bak
-0000b000: 222e 666f 726d 6174 286f 732e 7061 7468  ".format(os.path
-0000b010: 2e62 6173 656e 616d 6528 7061 7468 5f63  .basename(path_c
-0000b020: 7572 7265 6e74 5f66 696c 6529 2c20 6765  urrent_file), ge
-0000b030: 745f 7469 6d65 7374 616d 7028 2929 0a0a  t_timestamp())..
-0000b040: 2020 2020 2320 4966 2064 6566 6175 6c74      # If default
-0000b050: 2066 696c 6520 7072 6f76 6964 6564 2c20   file provided, 
-0000b060: 636f 6d70 6172 6520 746f 2063 7572 7265  compare to curre
-0000b070: 6e74 2066 696c 650a 2020 2020 6966 2070  nt file.    if p
-0000b080: 6174 685f 6465 6661 756c 745f 6669 6c65  ath_default_file
-0000b090: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000b0a0: 2020 2020 2020 2320 5265 6164 2074 6865        # Read the
-0000b0b0: 2064 6566 6175 6c74 2066 696c 6520 2b20   default file + 
-0000b0c0: 7468 6520 6375 7272 656e 7420 6669 6c65  the current file
-0000b0d0: 0a20 2020 2020 2020 2064 6566 6175 6c74  .        default
-0000b0e0: 5f66 696c 655f 636f 6e74 656e 7473 203d  _file_contents =
-0000b0f0: 2072 6561 645f 6669 6c65 2870 6174 685f   read_file(path_
-0000b100: 6465 6661 756c 745f 6669 6c65 290a 2020  default_file).  
-0000b110: 2020 2020 2020 6375 7272 656e 745f 6669        current_fi
-0000b120: 6c65 5f63 6f6e 7465 6e74 7320 3d20 7265  le_contents = re
-0000b130: 6164 5f66 696c 6528 7061 7468 5f63 7572  ad_file(path_cur
-0000b140: 7265 6e74 5f66 696c 6529 0a0a 2020 2020  rent_file)..    
-0000b150: 2020 2020 2320 4966 2064 6966 6665 7265      # If differe
-0000b160: 6e74 2c20 7265 6e61 6d65 0a20 2020 2020  nt, rename.     
-0000b170: 2020 2069 6620 6465 6661 756c 745f 6669     if default_fi
-0000b180: 6c65 5f63 6f6e 7465 6e74 7320 213d 2063  le_contents != c
-0000b190: 7572 7265 6e74 5f66 696c 655f 636f 6e74  urrent_file_cont
-0000b1a0: 656e 7473 3a0a 2020 2020 2020 2020 2020  ents:.          
-0000b1b0: 2020 4c4f 472e 6465 6275 6728 2243 7265    LOG.debug("Cre
-0000b1c0: 6174 696e 6720 6120 6261 636b 7570 206f  ating a backup o
-0000b1d0: 663a 2025 7322 2c20 7061 7468 5f63 7572  f: %s", path_cur
-0000b1e0: 7265 6e74 5f66 696c 6529 0a20 2020 2020  rent_file).     
-0000b1f0: 2020 2020 2020 2072 656e 616d 655f 6669         rename_fi
-0000b200: 6c65 2870 6174 685f 6375 7272 656e 745f  le(path_current_
-0000b210: 6669 6c65 2c20 6e65 775f 6669 6c65 5f6e  file, new_file_n
-0000b220: 616d 6529 0a0a 2020 2020 656c 7365 3a0a  ame)..    else:.
-0000b230: 2020 2020 2020 2020 4c4f 472e 6465 6275          LOG.debu
-0000b240: 6728 2243 7265 6174 696e 6720 6120 6261  g("Creating a ba
-0000b250: 636b 7570 206f 663a 2025 7322 2c20 7061  ckup of: %s", pa
-0000b260: 7468 5f63 7572 7265 6e74 5f66 696c 6529  th_current_file)
-0000b270: 0a20 2020 2020 2020 2072 656e 616d 655f  .        rename_
-0000b280: 6669 6c65 2870 6174 685f 6375 7272 656e  file(path_curren
-0000b290: 745f 6669 6c65 2c20 6e65 775f 6669 6c65  t_file, new_file
-0000b2a0: 5f6e 616d 6529 0a0a 2020 2020 7265 7475  _name)..    retu
-0000b2b0: 726e 206f 732e 7061 7468 2e6a 6f69 6e28  rn os.path.join(
-0000b2c0: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-0000b2d0: 7061 7468 5f63 7572 7265 6e74 5f66 696c  path_current_fil
-0000b2e0: 6529 2c20 6e65 775f 6669 6c65 5f6e 616d  e), new_file_nam
-0000b2f0: 6529 0a0a 0a64 6566 2067 656e 6572 6174  e)...def generat
-0000b300: 655f 616e 6368 6f72 2868 6561 6465 7229  e_anchor(header)
-0000b310: 3a0a 2020 2020 2222 220a 2020 2020 436f  :.    """.    Co
-0000b320: 6e76 6572 7473 2068 6561 6465 7220 746f  nverts header to
-0000b330: 206c 6f77 6572 6361 7365 2c20 7265 6d6f   lowercase, remo
-0000b340: 7665 7320 616c 6c20 6368 6172 6163 7465  ves all characte
-0000b350: 7273 2065 7863 6570 7420 612d 7a2c 2030  rs except a-z, 0
-0000b360: 2d39 2c20 2d2c 0a20 2020 2075 6e69 636f  -9, -,.    unico
-0000b370: 6465 2063 6861 7261 7465 7273 2074 6861  de charaters tha
-0000b380: 7420 6172 6520 7573 6564 2069 6e20 776f  t are used in wo
-0000b390: 7264 7320 616e 6420 7370 6163 6573 2074  rds and spaces t
-0000b3a0: 6865 6e20 7265 706c 6163 6573 0a20 2020  hen replaces.   
-0000b3b0: 2061 6c6c 2073 7061 6365 7320 7769 7468   all spaces with
-0000b3c0: 202d 0a0a 2020 2020 416e 2061 6e63 686f   -..    An ancho
-0000b3d0: 7220 6973 2075 7365 6420 696e 204d 6172  r is used in Mar
-0000b3e0: 6b64 6f77 6e20 5465 6d70 6c61 7465 7320  kdown Templates 
-0000b3f0: 746f 206c 696e 6b20 6365 7274 6169 6e20  to link certain 
-0000b400: 7061 7274 7320 6f66 2074 6865 2064 6f63  parts of the doc
-0000b410: 756d 656e 742e 0a0a 2020 2020 3a70 6172  ument...    :par
-0000b420: 616d 2068 6561 6465 723a 2053 7472 696e  am header: Strin
-0000b430: 6720 746f 2063 7265 6174 6520 616e 6368  g to create anch
-0000b440: 6f72 2066 726f 6d0a 2020 2020 3a74 7970  or from.    :typ
-0000b450: 6520 6865 6164 6572 3a20 7374 720a 2020  e header: str.  
-0000b460: 2020 3a72 6574 7572 6e3a 2068 6561 6465    :return: heade
-0000b470: 7220 666f 726d 6174 7465 6420 6173 2061  r formatted as a
-0000b480: 6e20 616e 6368 6f72 0a20 2020 203a 7274  n anchor.    :rt
-0000b490: 7970 653a 2073 7472 0a20 2020 2022 2222  ype: str.    """
-0000b4a0: 0a20 2020 2061 6e63 686f 7220 3d20 6865  .    anchor = he
-0000b4b0: 6164 6572 2e6c 6f77 6572 2829 0a0a 2020  ader.lower()..  
-0000b4c0: 2020 7265 6765 7820 3d20 7265 2e63 6f6d    regex = re.com
-0000b4d0: 7069 6c65 2872 225b 5e5c 775c 2d5c 735d  pile(r"[^\w\-\s]
-0000b4e0: 222c 2072 652e 5529 0a0a 2020 2020 616e  ", re.U)..    an
-0000b4f0: 6368 6f72 203d 2072 652e 7375 6228 7265  chor = re.sub(re
-0000b500: 6765 782c 2022 222c 2061 6e63 686f 7229  gex, "", anchor)
-0000b510: 0a20 2020 2061 6e63 686f 7220 3d20 7265  .    anchor = re
-0000b520: 2e73 7562 2872 225b 5c73 5d22 2c20 222d  .sub(r"[\s]", "-
-0000b530: 222c 2061 6e63 686f 7229 0a0a 2020 2020  ", anchor)..    
-0000b540: 7265 7475 726e 2061 6e63 686f 720a 0a0a  return anchor...
-0000b550: 6465 6620 7369 6d70 6c69 6679 5f73 7472  def simplify_str
-0000b560: 696e 6728 7468 655f 7374 7269 6e67 293a  ing(the_string):
-0000b570: 0a20 2020 2022 2222 0a20 2020 2053 696d  .    """.    Sim
-0000b580: 706c 6966 6965 7320 7468 655f 7374 7269  plifies the_stri
-0000b590: 6e67 2062 7920 636f 6e76 6572 7469 6e67  ng by converting
-0000b5a0: 2069 7420 746f 206c 6f77 6572 6361 7365   it to lowercase
-0000b5b0: 7320 616e 640a 2020 2020 7265 6d6f 7669  s and.    removi
-0000b5c0: 6e67 2061 6c6c 2063 6861 7261 6374 6572  ng all character
-0000b5d0: 7320 6578 6365 7074 2061 2d7a 2c20 302d  s except a-z, 0-
-0000b5e0: 392c 202d 2061 6e64 2073 7061 6365 7320  9, - and spaces 
-0000b5f0: 7468 656e 0a20 2020 2072 6570 6c61 6365  then.    replace
-0000b600: 7320 616c 6c20 7370 6163 6573 2077 6974  s all spaces wit
-0000b610: 6820 2d0a 0a20 2020 203a 7061 7261 6d20  h -..    :param 
-0000b620: 7468 655f 7374 7269 6e67 3a20 5374 7269  the_string: Stri
-0000b630: 6e67 2074 6f20 7369 6d70 6c69 6679 0a20  ng to simplify. 
-0000b640: 2020 203a 7479 7065 2074 6865 5f73 7472     :type the_str
-0000b650: 696e 673a 2073 7472 0a20 2020 203a 7265  ing: str.    :re
-0000b660: 7475 726e 3a20 7468 655f 7374 7269 6e67  turn: the_string
-0000b670: 2066 6f72 6d61 7474 6564 0a20 2020 203a   formatted.    :
-0000b680: 7274 7970 653a 2073 7472 0a20 2020 2022  rtype: str.    "
-0000b690: 2222 0a20 2020 2074 6865 5f73 7472 696e  "".    the_strin
-0000b6a0: 6720 3d20 7468 655f 7374 7269 6e67 2e6c  g = the_string.l
-0000b6b0: 6f77 6572 2829 0a0a 2020 2020 7265 6765  ower()..    rege
-0000b6c0: 7820 3d20 7265 2e63 6f6d 7069 6c65 2872  x = re.compile(r
-0000b6d0: 225b 5e61 2d7a 302d 395c 2d5c 735f 5d22  "[^a-z0-9\-\s_]"
-0000b6e0: 290a 0a20 2020 2074 6865 5f73 7472 696e  )..    the_strin
-0000b6f0: 6720 3d20 7265 2e73 7562 2872 6567 6578  g = re.sub(regex
-0000b700: 2c20 2222 2c20 7468 655f 7374 7269 6e67  , "", the_string
-0000b710: 290a 2020 2020 7468 655f 7374 7269 6e67  ).    the_string
-0000b720: 203d 2072 652e 7375 6228 225f 222c 2022   = re.sub("_", "
-0000b730: 2d22 2c20 7468 655f 7374 7269 6e67 290a  -", the_string).
-0000b740: 2020 2020 7468 655f 7374 7269 6e67 203d      the_string =
-0000b750: 2072 652e 7375 6228 7222 5b5c 735d 222c   re.sub(r"[\s]",
-0000b760: 2022 2d22 2c20 7468 655f 7374 7269 6e67   "-", the_string
-0000b770: 290a 0a20 2020 2072 6574 7572 6e20 7468  )..    return th
-0000b780: 655f 7374 7269 6e67 0a0a 0a64 6566 2067  e_string...def g
-0000b790: 6574 5f77 6f72 6b66 6c6f 775f 6675 6e63  et_workflow_func
-0000b7a0: 7469 6f6e 7328 776f 726b 666c 6f77 2c20  tions(workflow, 
-0000b7b0: 6675 6e63 7469 6f6e 5f75 7569 643d 4e6f  function_uuid=No
-0000b7c0: 6e65 293a 0a20 2020 2022 2222 5061 7273  ne):.    """Pars
-0000b7d0: 6573 2074 6865 2058 4d4c 206f 6620 7468  es the XML of th
-0000b7e0: 6520 576f 726b 666c 6f77 204f 626a 6563  e Workflow Objec
-0000b7f0: 7420 616e 6420 7265 7475 726e 730a 2020  t and returns.  
-0000b800: 2020 6120 4c69 7374 206f 6620 616c 6c20    a List of all 
-0000b810: 4675 6e63 7469 6f6e 7320 666f 756e 642e  Functions found.
-0000b820: 2049 6620 6675 6e63 7469 6f6e 5f75 7569   If function_uui
-0000b830: 6420 6973 2064 6566 696e 6564 0a20 2020  d is defined.   
-0000b840: 2072 6574 7572 6e73 2061 6c6c 206f 6363   returns all occ
-0000b850: 7572 7265 6e63 6573 206f 6620 7468 6174  urrences of that
-0000b860: 2066 756e 6374 696f 6e2e 0a0a 2020 2020   function...    
-0000b870: 4120 576f 726b 666c 6f77 2046 756e 6374  A Workflow Funct
-0000b880: 696f 6e20 6361 6e20 6861 7665 2074 6865  ion can have the
-0000b890: 2061 7474 7269 6275 7465 733a 0a20 2020   attributes:.   
-0000b8a0: 202d 2075 7569 643a 2053 7472 696e 670a   - uuid: String.
-0000b8b0: 2020 2020 2d20 696e 7075 7473 3a20 4469      - inputs: Di
-0000b8c0: 6374 0a20 2020 202d 2070 6f73 745f 7072  ct.    - post_pr
-0000b8d0: 6f63 6573 7369 6e67 5f73 6372 6970 743a  ocessing_script:
-0000b8e0: 2053 7472 696e 670a 2020 2020 2d20 7072   String.    - pr
-0000b8f0: 655f 7072 6f63 6573 7369 6e67 5f73 6372  e_processing_scr
-0000b900: 6970 743a 2053 7472 696e 670a 2020 2020  ipt: String.    
-0000b910: 2d20 7265 7375 6c74 5f6e 616d 653a 2053  - result_name: S
-0000b920: 7472 696e 6722 2222 0a0a 2020 2020 7265  tring"""..    re
-0000b930: 7475 726e 5f66 756e 6374 696f 6e73 203d  turn_functions =
-0000b940: 205b 5d0a 0a20 2020 2023 2057 6f72 6b66   []..    # Workf
-0000b950: 6c6f 7720 584d 4c20 7465 7874 0a20 2020  low XML text.   
-0000b960: 2077 665f 786d 6c20 3d20 776f 726b 666c   wf_xml = workfl
-0000b970: 6f77 2e67 6574 2822 636f 6e74 656e 7422  ow.get("content"
-0000b980: 2c20 7b7d 292e 6765 7428 2278 6d6c 222c  , {}).get("xml",
-0000b990: 204e 6f6e 6529 0a0a 2020 2020 6966 2077   None)..    if w
-0000b9a0: 665f 786d 6c20 6973 204e 6f6e 653a 0a20  f_xml is None:. 
-0000b9b0: 2020 2020 2020 2072 6169 7365 2053 444b         raise SDK
-0000b9c0: 4578 6365 7074 696f 6e28 2243 6f75 6c64  Exception("Could
-0000b9d0: 206e 6f74 206c 6f61 6420 786d 6c20 636f   not load xml co
-0000b9e0: 6e74 656e 7420 6672 6f6d 2057 6f72 6b66  ntent from Workf
-0000b9f0: 6c6f 773a 207b 307d 222e 666f 726d 6174  low: {0}".format
-0000ba00: 2877 6f72 6b66 6c6f 7729 290a 0a20 2020  (workflow))..   
-0000ba10: 2023 2047 6574 2074 6865 2072 6f6f 7420   # Get the root 
-0000ba20: 656c 656d 656e 7420 2b20 656e 646f 6465  element + endode
-0000ba30: 2069 6e20 7574 6638 2069 6e20 6f72 6465   in utf8 in orde
-0000ba40: 7220 746f 2068 616e 646c 6520 556e 6963  r to handle Unic
-0000ba50: 6f64 650a 2020 2020 726f 6f74 203d 2045  ode.    root = E
-0000ba60: 542e 6672 6f6d 7374 7269 6e67 2877 665f  T.fromstring(wf_
-0000ba70: 786d 6c2e 656e 636f 6465 2822 7574 6638  xml.encode("utf8
-0000ba80: 2229 290a 0a20 2020 2023 2047 6574 2074  "))..    # Get t
-0000ba90: 6865 2070 7265 6669 7820 666f 7220 6561  he prefix for ea
-0000baa0: 6368 2065 6c65 6d65 6e74 2773 2074 6167  ch element's tag
-0000bab0: 0a20 2020 2074 6167 5f70 7265 6669 7820  .    tag_prefix 
-0000bac0: 3d20 726f 6f74 2e74 6167 2e72 6570 6c61  = root.tag.repla
-0000bad0: 6365 2822 6465 6669 6e69 7469 6f6e 7322  ce("definitions"
-0000bae0: 2c20 2222 290a 0a20 2020 2078 6d6c 5f70  , "")..    xml_p
-0000baf0: 6174 6820 3d20 222e 2f7b 307d 7072 6f63  ath = "./{0}proc
-0000bb00: 6573 732f 7b30 7d73 6572 7669 6365 5461  ess/{0}serviceTa
-0000bb10: 736b 2f7b 307d 6578 7465 6e73 696f 6e45  sk/{0}extensionE
-0000bb20: 6c65 6d65 6e74 732f 2a22 2e66 6f72 6d61  lements/*".forma
-0000bb30: 7428 7461 675f 7072 6566 6978 290a 2020  t(tag_prefix).  
-0000bb40: 2020 7468 655f 6675 6e63 7469 6f6e 5f65    the_function_e
-0000bb50: 6c65 6d65 6e74 7320 3d20 5b5d 0a0a 2020  lements = []..  
-0000bb60: 2020 6966 2066 756e 6374 696f 6e5f 7575    if function_uu
-0000bb70: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0000bb80: 2020 2020 2020 2020 786d 6c5f 7061 7468          xml_path
-0000bb90: 203d 2022 7b30 7d5b 4075 7569 643d 277b   = "{0}[@uuid='{
-0000bba0: 317d 275d 222e 666f 726d 6174 2878 6d6c  1}']".format(xml
-0000bbb0: 5f70 6174 682c 2066 756e 6374 696f 6e5f  _path, function_
-0000bbc0: 7575 6964 290a 0a20 2020 2020 2020 2023  uuid)..        #
-0000bbd0: 2047 6574 2061 6c6c 2065 6c65 6d65 6e74   Get all element
-0000bbe0: 7320 6174 2078 6d6c 5f70 6174 6820 7468  s at xml_path th
-0000bbf0: 6174 2068 6176 6520 7468 6520 7575 6964  at have the uuid
-0000bc00: 206f 6620 7468 6520 6675 6e63 7469 6f6e   of the function
-0000bc10: 0a20 2020 2020 2020 2074 6865 5f66 756e  .        the_fun
-0000bc20: 6374 696f 6e5f 656c 656d 656e 7473 203d  ction_elements =
-0000bc30: 2072 6f6f 742e 6669 6e64 616c 6c28 786d   root.findall(xm
-0000bc40: 6c5f 7061 7468 290a 0a20 2020 2065 6c73  l_path)..    els
-0000bc50: 653a 0a20 2020 2020 2020 2074 6865 5f65  e:.        the_e
-0000bc60: 7874 656e 7369 6f6e 5f65 6c65 6d65 6e74  xtension_element
-0000bc70: 7320 3d20 726f 6f74 2e66 696e 6461 6c6c  s = root.findall
-0000bc80: 2878 6d6c 5f70 6174 6829 0a20 2020 2020  (xml_path).     
-0000bc90: 2020 2066 6f72 2065 7874 656e 7369 6f6e     for extension
-0000bca0: 5f65 6c65 6d65 6e74 2069 6e20 7468 655f  _element in the_
-0000bcb0: 6578 7465 6e73 696f 6e5f 656c 656d 656e  extension_elemen
-0000bcc0: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-0000bcd0: 6966 2022 6675 6e63 7469 6f6e 2220 696e  if "function" in
-0000bce0: 2065 7874 656e 7369 6f6e 5f65 6c65 6d65   extension_eleme
-0000bcf0: 6e74 2e74 6167 3a0a 2020 2020 2020 2020  nt.tag:.        
-0000bd00: 2020 2020 2020 2020 7468 655f 6675 6e63          the_func
-0000bd10: 7469 6f6e 5f65 6c65 6d65 6e74 732e 6170  tion_elements.ap
-0000bd20: 7065 6e64 2865 7874 656e 7369 6f6e 5f65  pend(extension_e
-0000bd30: 6c65 6d65 6e74 290a 0a20 2020 2023 2046  lement)..    # F
-0000bd40: 6f72 6561 6368 2065 6c65 6d65 6e74 2066  oreach element f
-0000bd50: 6f75 6e64 2c20 6c6f 6164 2069 7420 6173  ound, load it as
-0000bd60: 2061 2064 6963 7469 6f6e 6172 7920 616e   a dictionary an
-0000bd70: 6420 6170 7065 6e64 2074 6f20 7265 7475  d append to retu
-0000bd80: 726e 206c 6973 740a 2020 2020 666f 7220  rn list.    for 
-0000bd90: 666e 5f65 6c65 6d65 6e74 2069 6e20 7468  fn_element in th
-0000bda0: 655f 6675 6e63 7469 6f6e 5f65 6c65 6d65  e_function_eleme
-0000bdb0: 6e74 733a 0a20 2020 2020 2020 2072 6574  nts:.        ret
-0000bdc0: 7572 6e5f 6675 6e63 7469 6f6e 203d 206a  urn_function = j
-0000bdd0: 736f 6e2e 6c6f 6164 7328 666e 5f65 6c65  son.loads(fn_ele
-0000bde0: 6d65 6e74 2e74 6578 7429 0a20 2020 2020  ment.text).     
-0000bdf0: 2020 2072 6574 7572 6e5f 6675 6e63 7469     return_functi
-0000be00: 6f6e 5b22 7575 6964 225d 203d 2066 6e5f  on["uuid"] = fn_
-0000be10: 656c 656d 656e 742e 6174 7472 6962 2e67  element.attrib.g
-0000be20: 6574 2822 7575 6964 222c 2022 2229 0a20  et("uuid", ""). 
-0000be30: 2020 2020 2020 2072 6574 7572 6e5f 6675         return_fu
-0000be40: 6e63 7469 6f6e 5b22 7265 7375 6c74 5f6e  nction["result_n
-0000be50: 616d 6522 5d20 3d20 7265 7475 726e 5f66  ame"] = return_f
-0000be60: 756e 6374 696f 6e2e 6765 7428 2272 6573  unction.get("res
-0000be70: 756c 745f 6e61 6d65 222c 204e 6f6e 6529  ult_name", None)
-0000be80: 0a20 2020 2020 2020 2072 6574 7572 6e5f  .        return_
-0000be90: 6675 6e63 7469 6f6e 5b22 706f 7374 5f70  function["post_p
-0000bea0: 726f 6365 7373 696e 675f 7363 7269 7074  rocessing_script
-0000beb0: 225d 203d 2072 6574 7572 6e5f 6675 6e63  "] = return_func
-0000bec0: 7469 6f6e 2e67 6574 2822 706f 7374 5f70  tion.get("post_p
-0000bed0: 726f 6365 7373 696e 675f 7363 7269 7074  rocessing_script
-0000bee0: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
-0000bef0: 2072 6574 7572 6e5f 6675 6e63 7469 6f6e   return_function
-0000bf00: 5b22 7072 655f 7072 6f63 6573 7369 6e67  ["pre_processing
-0000bf10: 5f73 6372 6970 7422 5d20 3d20 7265 7475  _script"] = retu
-0000bf20: 726e 5f66 756e 6374 696f 6e2e 6765 7428  rn_function.get(
-0000bf30: 2270 7265 5f70 726f 6365 7373 696e 675f  "pre_processing_
-0000bf40: 7363 7269 7074 222c 204e 6f6e 6529 0a0a  script", None)..
-0000bf50: 2020 2020 2020 2020 7265 7475 726e 5f66          return_f
-0000bf60: 756e 6374 696f 6e73 2e61 7070 656e 6428  unctions.append(
-0000bf70: 7265 7475 726e 5f66 756e 6374 696f 6e29  return_function)
-0000bf80: 0a0a 2020 2020 7265 7475 726e 2072 6574  ..    return ret
-0000bf90: 7572 6e5f 6675 6e63 7469 6f6e 730a 0a0a  urn_functions...
-0000bfa0: 6465 6620 6765 745f 706c 6179 626f 6f6b  def get_playbook
-0000bfb0: 5f6f 626a 6563 7473 2870 6c61 7962 6f6f  _objects(playboo
-0000bfc0: 6b2c 2066 756e 6374 696f 6e5f 7575 6964  k, function_uuid
-0000bfd0: 3d4e 6f6e 6529 3a0a 2020 2020 2222 2250  =None):.    """P
-0000bfe0: 6172 7365 7320 7468 6520 584d 4c20 6f66  arses the XML of
-0000bff0: 2074 6865 2050 6c61 7962 6f6f 6b20 4f62   the Playbook Ob
-0000c000: 6a65 6374 2061 6e64 2072 6574 7572 6e73  ject and returns
-0000c010: 0a20 2020 2061 204c 6973 7420 6f66 2061  .    a List of a
-0000c020: 6c6c 2046 756e 6374 696f 6e73 2061 6e64  ll Functions and
-0000c030: 2053 6372 6970 7473 2066 6f75 6e64 2e20   Scripts found. 
-0000c040: 5468 6520 7363 7269 7074 730a 2020 2020  The scripts.    
-0000c050: 7265 7475 726e 6564 206f 6e6c 7920 6861  returned only ha
-0000c060: 7320 7468 6520 7575 6964 2061 7474 7269  s the uuid attri
-0000c070: 6275 7465 2e20 5468 6973 2063 616e 206c  bute. This can l
-0000c080: 6174 6572 0a20 2020 2062 6520 7573 6564  ater.    be used
-0000c090: 2074 6f20 6578 7472 6163 7420 616c 6c20   to extract all 
-0000c0a0: 7363 7269 7074 2d72 656c 6174 6564 2069  script-related i
-0000c0b0: 6e66 6f72 6d61 7469 6f6e 2065 6974 6865  nformation eithe
-0000c0c0: 720a 2020 2020 666f 726d 2074 6865 2070  r.    form the p
-0000c0d0: 6c61 7962 6f6f 6b20 6578 706f 7274 206f  laybook export o
-0000c0e0: 7220 6672 6f6d 2067 6c6f 6261 6c20 7363  r from global sc
-0000c0f0: 7269 7074 732e 2049 660a 2020 2020 6675  ripts. If.    fu
-0000c100: 6e63 7469 6f6e 5f75 7569 6420 6973 2064  nction_uuid is d
-0000c110: 6566 696e 6564 2072 6574 7572 6e73 2061  efined returns a
-0000c120: 6c6c 206f 6363 7572 7265 6e63 6573 206f  ll occurrences o
-0000c130: 6620 7468 6174 0a20 2020 2066 756e 6374  f that.    funct
-0000c140: 696f 6e20 6f6e 6c79 2e0a 0a20 2020 2046  ion only...    F
-0000c150: 756e 6374 696f 6e20 4174 7472 6962 7574  unction Attribut
-0000c160: 6573 3a0a 2020 2020 2d20 7575 6964 3a20  es:.    - uuid: 
-0000c170: 5374 7269 6e67 0a20 2020 202d 2069 6e70  String.    - inp
-0000c180: 7574 733a 2044 6963 740a 2020 2020 2d20  uts: Dict.    - 
-0000c190: 7072 655f 7072 6f63 6573 7369 6e67 5f73  pre_processing_s
-0000c1a0: 6372 6970 743a 2053 7472 696e 670a 2020  cript: String.  
-0000c1b0: 2020 2d20 7265 7375 6c74 5f6e 616d 653a    - result_name:
-0000c1c0: 2053 7472 696e 670a 0a20 2020 2053 6372   String..    Scr
-0000c1d0: 6970 7420 4174 7472 6962 7574 6573 3a0a  ipt Attributes:.
-0000c1e0: 2020 2020 2d20 7575 6964 3a20 5374 7269      - uuid: Stri
-0000c1f0: 6e67 0a20 2020 2022 2222 0a20 2020 2070  ng.    """.    p
-0000c200: 6c61 7962 6f6f 6b5f 656c 656d 656e 7473  laybook_elements
-0000c210: 203d 207b 2266 756e 6374 696f 6e73 223a   = {"functions":
-0000c220: 205b 5d2c 2022 7363 7269 7074 7322 3a20   [], "scripts": 
-0000c230: 5b5d 2c20 2273 7562 5f70 6273 223a 205b  [], "sub_pbs": [
-0000c240: 5d7d 0a0a 2020 2020 2320 506c 6179 626f  ]}..    # Playbo
-0000c250: 6f6b 2058 4d4c 2074 6578 740a 2020 2020  ok XML text.    
-0000c260: 7062 5f78 6d6c 203d 2070 6c61 7962 6f6f  pb_xml = playboo
-0000c270: 6b2e 6765 7428 2263 6f6e 7465 6e74 222c  k.get("content",
-0000c280: 207b 7d29 2e67 6574 2822 786d 6c22 2c20   {}).get("xml", 
-0000c290: 4e6f 6e65 290a 0a20 2020 2069 6620 7062  None)..    if pb
-0000c2a0: 5f78 6d6c 2069 7320 4e6f 6e65 3a0a 2020  _xml is None:.  
-0000c2b0: 2020 2020 2020 7261 6973 6520 5344 4b45        raise SDKE
-0000c2c0: 7863 6570 7469 6f6e 2822 436f 756c 6420  xception("Could 
-0000c2d0: 6e6f 7420 6c6f 6164 2078 6d6c 2063 6f6e  not load xml con
-0000c2e0: 7465 6e74 2066 726f 6d20 506c 6179 626f  tent from Playbo
-0000c2f0: 6f6b 733a 207b 307d 222e 666f 726d 6174  oks: {0}".format
-0000c300: 2870 6c61 7962 6f6f 6b29 290a 0a20 2020  (playbook))..   
-0000c310: 2023 2047 6574 2074 6865 2072 6f6f 7420   # Get the root 
-0000c320: 656c 656d 656e 7420 2b20 656e 636f 6465  element + encode
-0000c330: 6420 696e 2075 7466 3820 696e 206f 7264  d in utf8 in ord
-0000c340: 6572 2074 6f20 6861 6e64 6c65 2055 6e69  er to handle Uni
-0000c350: 636f 6465 0a20 2020 2072 6f6f 7420 3d20  code.    root = 
-0000c360: 4554 2e66 726f 6d73 7472 696e 6728 7062  ET.fromstring(pb
-0000c370: 5f78 6d6c 2e65 6e63 6f64 6528 2275 7466  _xml.encode("utf
-0000c380: 3822 2929 0a0a 2020 2020 2320 4765 7420  8"))..    # Get 
-0000c390: 7468 6520 7072 6566 6978 2066 6f72 2065  the prefix for e
-0000c3a0: 6163 6820 656c 656d 656e 7427 7320 7461  ach element's ta
-0000c3b0: 670a 2020 2020 7461 675f 7072 6566 6978  g.    tag_prefix
-0000c3c0: 203d 2072 6f6f 742e 7461 672e 7265 706c   = root.tag.repl
-0000c3d0: 6163 6528 2264 6566 696e 6974 696f 6e73  ace("definitions
-0000c3e0: 222c 2022 2229 0a0a 2020 2020 786d 6c5f  ", "")..    xml_
-0000c3f0: 6675 6e63 7469 6f6e 5f70 6174 6820 3d20  function_path = 
-0000c400: 222e 2f7b 307d 7072 6f63 6573 732f 7b30  "./{0}process/{0
-0000c410: 7d73 6572 7669 6365 5461 736b 2f7b 307d  }serviceTask/{0}
-0000c420: 6578 7465 6e73 696f 6e45 6c65 6d65 6e74  extensionElement
-0000c430: 732f 2a22 2e66 6f72 6d61 7428 7461 675f  s/*".format(tag_
-0000c440: 7072 6566 6978 290a 2020 2020 786d 6c5f  prefix).    xml_
-0000c450: 7363 7269 7074 5f70 6174 6820 3d20 222e  script_path = ".
-0000c460: 2f7b 307d 7072 6f63 6573 732f 7b30 7d73  /{0}process/{0}s
-0000c470: 6372 6970 7454 6173 6b2f 7b30 7d65 7874  criptTask/{0}ext
-0000c480: 656e 7369 6f6e 456c 656d 656e 7473 2f2a  ensionElements/*
-0000c490: 222e 666f 726d 6174 2874 6167 5f70 7265  ".format(tag_pre
-0000c4a0: 6669 7829 0a20 2020 2078 6d6c 5f73 7562  fix).    xml_sub
-0000c4b0: 5f70 6c61 7962 6f6f 6b5f 7061 7468 203d  _playbook_path =
-0000c4c0: 2022 2e2f 7b30 7d70 726f 6365 7373 2f7b   "./{0}process/{
-0000c4d0: 307d 6361 6c6c 4163 7469 7669 7479 2f7b  0}callActivity/{
-0000c4e0: 307d 6578 7465 6e73 696f 6e45 6c65 6d65  0}extensionEleme
-0000c4f0: 6e74 732f 2a22 2e66 6f72 6d61 7428 7461  nts/*".format(ta
-0000c500: 675f 7072 6566 6978 290a 0a20 2020 2069  g_prefix)..    i
-0000c510: 6620 6675 6e63 7469 6f6e 5f75 7569 6420  f function_uuid 
-0000c520: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000c530: 2020 2020 2078 6d6c 5f66 756e 6374 696f       xml_functio
-0000c540: 6e5f 7061 7468 203d 2022 7b30 7d5b 4075  n_path = "{0}[@u
-0000c550: 7569 643d 277b 317d 275d 222e 666f 726d  uid='{1}']".form
-0000c560: 6174 2878 6d6c 5f66 756e 6374 696f 6e5f  at(xml_function_
-0000c570: 7061 7468 2c20 6675 6e63 7469 6f6e 5f75  path, function_u
-0000c580: 7569 6429 0a0a 2020 2020 2020 2020 2320  uid)..        # 
-0000c590: 4765 7420 616c 6c20 656c 656d 656e 7473  Get all elements
-0000c5a0: 2061 7420 786d 6c5f 7061 7468 2074 6861   at xml_path tha
-0000c5b0: 7420 6861 7665 2074 6865 2075 7569 6420  t have the uuid 
-0000c5c0: 6f66 2074 6865 2066 756e 6374 696f 6e0a  of the function.
-0000c5d0: 2020 2020 2020 2020 706c 6179 626f 6f6b          playbook
-0000c5e0: 5f65 6c65 6d65 6e74 7320 2b3d 2072 6f6f  _elements += roo
-0000c5f0: 742e 6669 6e64 616c 6c28 786d 6c5f 6675  t.findall(xml_fu
-0000c600: 6e63 7469 6f6e 5f70 6174 6829 0a20 2020  nction_path).   
-0000c610: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
-0000c620: 2050 6174 6873 2074 6f20 6675 6e63 7469   Paths to functi
-0000c630: 6f6e 732c 2073 6372 6970 7473 2c20 616e  ons, scripts, an
-0000c640: 6420 7375 6270 6c61 7962 6f6f 6b73 2069  d subplaybooks i
-0000c650: 6e20 7468 6520 584d 4c0a 2020 2020 2020  n the XML.      
-0000c660: 2020 7468 655f 6578 7465 6e73 696f 6e5f    the_extension_
-0000c670: 656c 656d 656e 7473 2020 3d20 726f 6f74  elements  = root
-0000c680: 2e66 696e 6461 6c6c 2878 6d6c 5f66 756e  .findall(xml_fun
-0000c690: 6374 696f 6e5f 7061 7468 290a 2020 2020  ction_path).    
-0000c6a0: 2020 2020 7468 655f 6578 7465 6e73 696f      the_extensio
-0000c6b0: 6e5f 656c 656d 656e 7473 202b 3d20 726f  n_elements += ro
-0000c6c0: 6f74 2e66 696e 6461 6c6c 2878 6d6c 5f73  ot.findall(xml_s
-0000c6d0: 6372 6970 745f 7061 7468 290a 2020 2020  cript_path).    
-0000c6e0: 2020 2020 7468 655f 6578 7465 6e73 696f      the_extensio
-0000c6f0: 6e5f 656c 656d 656e 7473 202b 3d20 726f  n_elements += ro
-0000c700: 6f74 2e66 696e 6461 6c6c 2878 6d6c 5f73  ot.findall(xml_s
-0000c710: 7562 5f70 6c61 7962 6f6f 6b5f 7061 7468  ub_playbook_path
-0000c720: 290a 0a20 2020 2020 2020 2066 6f72 2065  )..        for e
-0000c730: 7874 656e 7369 6f6e 5f65 6c65 6d65 6e74  xtension_element
-0000c740: 2069 6e20 7468 655f 6578 7465 6e73 696f   in the_extensio
-0000c750: 6e5f 656c 656d 656e 7473 3a0a 2020 2020  n_elements:.    
-0000c760: 2020 2020 2020 2020 7265 7475 726e 5f66          return_f
-0000c770: 756e 6374 696f 6e20 3d20 7b7d 0a20 2020  unction = {}.   
-0000c780: 2020 2020 2020 2020 2023 2045 7874 7261           # Extra
-0000c790: 6374 696e 6720 4675 6e63 7469 6f6e 2072  cting Function r
-0000c7a0: 656c 6174 6564 2064 6174 6120 6672 6f6d  elated data from
-0000c7b0: 2074 6865 2058 4d4c 0a20 2020 2020 2020   the XML.       
-0000c7c0: 2020 2020 2069 6620 2266 756e 6374 696f       if "functio
-0000c7d0: 6e22 2069 6e20 6578 7465 6e73 696f 6e5f  n" in extension_
-0000c7e0: 656c 656d 656e 742e 7461 673a 0a20 2020  element.tag:.   
-0000c7f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000c800: 7572 6e5f 6675 6e63 7469 6f6e 203d 206a  urn_function = j
-0000c810: 736f 6e2e 6c6f 6164 7328 6578 7465 6e73  son.loads(extens
-0000c820: 696f 6e5f 656c 656d 656e 742e 7465 7874  ion_element.text
-0000c830: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000c840: 2020 7265 7475 726e 5f66 756e 6374 696f    return_functio
-0000c850: 6e5b 2275 7569 6422 5d20 3d20 6578 7465  n["uuid"] = exte
-0000c860: 6e73 696f 6e5f 656c 656d 656e 742e 6174  nsion_element.at
-0000c870: 7472 6962 2e67 6574 2822 7575 6964 222c  trib.get("uuid",
-0000c880: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
-0000c890: 2020 2020 2072 6574 7572 6e5f 6675 6e63       return_func
-0000c8a0: 7469 6f6e 5b22 7265 7375 6c74 5f6e 616d  tion["result_nam
-0000c8b0: 6522 5d20 3d20 7265 7475 726e 5f66 756e  e"] = return_fun
-0000c8c0: 6374 696f 6e2e 6765 7428 2272 6573 756c  ction.get("resul
-0000c8d0: 745f 6e61 6d65 222c 204e 6f6e 6529 0a20  t_name", None). 
-0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000c8f0: 6574 7572 6e5f 6675 6e63 7469 6f6e 5b22  eturn_function["
-0000c900: 7072 655f 7072 6f63 6573 7369 6e67 5f73  pre_processing_s
-0000c910: 6372 6970 7422 5d20 3d20 7265 7475 726e  cript"] = return
-0000c920: 5f66 756e 6374 696f 6e2e 6765 7428 2270  _function.get("p
-0000c930: 7265 5f70 726f 6365 7373 696e 675f 7363  re_processing_sc
-0000c940: 7269 7074 222c 204e 6f6e 6529 0a20 2020  ript", None).   
-0000c950: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-0000c960: 7962 6f6f 6b5f 656c 656d 656e 7473 5b22  ybook_elements["
-0000c970: 6675 6e63 7469 6f6e 7322 5d2e 6170 7065  functions"].appe
-0000c980: 6e64 2872 6574 7572 6e5f 6675 6e63 7469  nd(return_functi
-0000c990: 6f6e 290a 0a20 2020 2020 2020 2020 2020  on)..           
-0000c9a0: 2023 2045 7874 7261 6374 696e 6720 5363   # Extracting Sc
-0000c9b0: 7269 7074 2072 656c 6174 6564 2064 6174  ript related dat
-0000c9c0: 6120 6672 6f6d 2074 6865 2058 4d4c 0a20  a from the XML. 
-0000c9d0: 2020 2020 2020 2020 2020 2069 6620 2273             if "s
-0000c9e0: 6372 6970 7422 2069 6e20 6578 7465 6e73  cript" in extens
-0000c9f0: 696f 6e5f 656c 656d 656e 742e 7461 673a  ion_element.tag:
-0000ca00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ca10: 2072 6574 7572 6e5f 6675 6e63 7469 6f6e   return_function
-0000ca20: 5b22 7575 6964 225d 203d 2065 7874 656e  ["uuid"] = exten
-0000ca30: 7369 6f6e 5f65 6c65 6d65 6e74 2e67 6574  sion_element.get
-0000ca40: 2822 7575 6964 222c 2022 2229 0a20 2020  ("uuid", "").   
-0000ca50: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-0000ca60: 7962 6f6f 6b5f 656c 656d 656e 7473 5b22  ybook_elements["
-0000ca70: 7363 7269 7074 7322 5d2e 6170 7065 6e64  scripts"].append
-0000ca80: 2872 6574 7572 6e5f 6675 6e63 7469 6f6e  (return_function
-0000ca90: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-0000caa0: 2045 7874 7261 6374 696e 6720 5375 6270   Extracting Subp
-0000cab0: 6c61 7962 6f6f 6b20 7265 6c61 7465 6420  laybook related 
-0000cac0: 6461 7461 2066 726f 6d20 7468 6520 584d  data from the XM
-0000cad0: 4c0a 2020 2020 2020 2020 2020 2020 6966  L.            if
-0000cae0: 2022 7375 622d 706c 6179 626f 6f6b 2220   "sub-playbook" 
-0000caf0: 696e 2065 7874 656e 7369 6f6e 5f65 6c65  in extension_ele
-0000cb00: 6d65 6e74 2e74 6167 3a0a 2020 2020 2020  ment.tag:.      
-0000cb10: 2020 2020 2020 2020 2020 7375 625f 7062            sub_pb
-0000cb20: 203d 206a 736f 6e2e 6c6f 6164 7328 6578   = json.loads(ex
-0000cb30: 7465 6e73 696f 6e5f 656c 656d 656e 742e  tension_element.
-0000cb40: 7465 7874 290a 2020 2020 2020 2020 2020  text).          
-0000cb50: 2020 2020 2020 7375 625f 7062 5b22 7575        sub_pb["uu
-0000cb60: 6964 225d 203d 2065 7874 656e 7369 6f6e  id"] = extension
-0000cb70: 5f65 6c65 6d65 6e74 2e61 7474 7269 622e  _element.attrib.
-0000cb80: 6765 7428 2275 7569 6422 2c20 2222 290a  get("uuid", "").
-0000cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cba0: 706c 6179 626f 6f6b 5f65 6c65 6d65 6e74  playbook_element
-0000cbb0: 735b 2273 7562 5f70 6273 225d 2e61 7070  s["sub_pbs"].app
-0000cbc0: 656e 6428 7375 625f 7062 290a 0a20 2020  end(sub_pb)..   
-0000cbd0: 2072 6574 7572 6e20 706c 6179 626f 6f6b   return playbook
-0000cbe0: 5f65 6c65 6d65 6e74 730a 0a0a 6465 6620  _elements...def 
-0000cbf0: 7265 706c 6163 655f 7575 6964 735f 696e  replace_uuids_in
-0000cc00: 5f73 7562 706c 6179 626f 6f6b 5f64 6174  _subplaybook_dat
-0000cc10: 6128 706c 6179 626f 6f6b 5f64 6174 612c  a(playbook_data,
-0000cc20: 2065 7870 6f72 7429 3a0a 2020 2020 2222   export):.    ""
-0000cc30: 220a 2020 2020 5768 656e 2070 726f 6365  ".    When proce
-0000cc40: 7373 696e 6720 6120 7375 6270 6c61 7962  ssing a subplayb
-0000cc50: 6f6f 6b20 7769 7468 696e 2061 2070 6c61  ook within a pla
-0000cc60: 7962 6f6f 6b2c 2069 7420 6973 2070 6f73  ybook, it is pos
-0000cc70: 7369 626c 6520 7468 6174 2074 6865 7265  sible that there
-0000cc80: 2061 7265 0a20 2020 2072 6566 6572 656e   are.    referen
-0000cc90: 6365 7320 746f 206f 626a 6563 7473 206f  ces to objects o
-0000cca0: 6e6c 7920 7468 726f 7567 6820 5555 4944  nly through UUID
-0000ccb0: 732e 2054 686f 7365 2061 7265 206e 6f74  s. Those are not
-0000ccc0: 2075 7365 6675 6c20 666f 720a 2020 2020   useful for.    
-0000ccd0: 6765 6e65 7261 7469 6e67 204d 6172 6b64  generating Markd
-0000cce0: 6f77 6e20 6669 6c65 7320 7768 6572 6520  own files where 
-0000ccf0: 6120 7573 6572 2077 616e 7473 2074 6f20  a user wants to 
-0000cd00: 7265 6164 2074 6872 6f75 6768 2069 6e20  read through in 
-0000cd10: 706c 6169 6e20 7465 7874 0a20 2020 2074  plain text.    t
-0000cd20: 6865 2076 616c 7565 7320 6f66 2074 6865  he values of the
-0000cd30: 206f 626a 6563 7473 2072 6566 6572 656e   objects referen
-0000cd40: 6365 642e 2054 6869 7320 6675 6e63 7469  ced. This functi
-0000cd50: 6f6e 2072 6570 6c61 6365 7320 616e 7920  on replaces any 
-0000cd60: 7265 6c65 7661 6e74 0a20 2020 2055 5549  relevant.    UUI
-0000cd70: 4473 2077 6974 6820 7468 6569 7220 7472  Ds with their tr
-0000cd80: 7565 2076 616c 7565 2066 726f 6d20 7468  ue value from th
-0000cd90: 6520 6578 706f 7274 2e20 5468 6520 7265  e export. The re
-0000cda0: 706c 6163 656d 656e 7420 6973 2069 6e20  placement is in 
-0000cdb0: 706c 6163 650a 0a20 2020 203a 7061 7261  place..    :para
-0000cdc0: 6d20 706c 6179 626f 6f6b 5f64 6174 613a  m playbook_data:
-0000cdd0: 2073 7562 2070 6c61 7962 6f6f 6b20 746f   sub playbook to
-0000cde0: 2070 726f 6365 7373 0a20 2020 203a 7479   process.    :ty
-0000cdf0: 7065 2070 6c61 7962 6f6f 6b5f 6461 7461  pe playbook_data
-0000ce00: 3a20 6469 6374 0a20 2020 203a 7061 7261  : dict.    :para
-0000ce10: 6d20 6578 706f 7274 3a20 6675 6c6c 2065  m export: full e
-0000ce20: 7870 6f72 7420 6461 7461 0a20 2020 203a  xport data.    :
-0000ce30: 7479 7065 2065 7870 6f72 743a 2064 6963  type export: dic
-0000ce40: 740a 2020 2020 2222 220a 0a20 2020 2023  t.    """..    #
-0000ce50: 2061 6464 206e 616d 6520 746f 2065 6163   add name to eac
-0000ce60: 6820 7375 6220 706c 6179 626f 6f6b 2069  h sub playbook i
-0000ce70: 6e70 7574 0a20 2020 2066 6f72 2073 7562  nput.    for sub
-0000ce80: 5f70 6220 696e 2065 7870 6f72 742e 6765  _pb in export.ge
-0000ce90: 7428 2270 6c61 7962 6f6f 6b73 222c 205b  t("playbooks", [
-0000cea0: 5d29 3a0a 2020 2020 2020 2020 6966 2070  ]):.        if p
-0000ceb0: 6c61 7962 6f6f 6b5f 6461 7461 2e67 6574  laybook_data.get
-0000cec0: 2822 7575 6964 222c 2022 7575 6964 5f6e  ("uuid", "uuid_n
-0000ced0: 6f74 5f66 6f75 6e64 5f70 6222 2920 3d3d  ot_found_pb") ==
-0000cee0: 2073 7562 5f70 622e 6765 7428 2275 7569   sub_pb.get("uui
-0000cef0: 6422 2c20 2275 7569 645f 6e6f 745f 666f  d", "uuid_not_fo
-0000cf00: 756e 645f 666e 2229 3a0a 2020 2020 2020  und_fn"):.      
-0000cf10: 2020 2020 2020 6669 656c 6473 203d 2073        fields = s
-0000cf20: 7562 5f70 622e 6765 7428 2266 6965 6c64  ub_pb.get("field
-0000cf30: 735f 7479 7065 222c 207b 7d29 2e67 6574  s_type", {}).get
-0000cf40: 2822 6669 656c 6473 222c 207b 7d29 0a0a  ("fields", {})..
-0000cf50: 2020 2020 2020 2020 2020 2020 2320 7570              # up
-0000cf60: 6461 7465 2073 7562 2070 6c61 7962 6f6f  date sub playboo
-0000cf70: 6b27 7320 6e61 6d65 0a20 2020 2020 2020  k's name.       
-0000cf80: 2020 2020 2070 6c61 7962 6f6f 6b5f 6461       playbook_da
-0000cf90: 7461 5b22 6e61 6d65 225d 203d 2073 7562  ta["name"] = sub
-0000cfa0: 5f70 622e 6765 7428 2264 6973 706c 6179  _pb.get("display
-0000cfb0: 5f6e 616d 6522 290a 2020 2020 2020 2020  _name").        
-0000cfc0: 2020 2020 666f 7220 6669 656c 645f 6e61      for field_na
-0000cfd0: 6d65 2c20 6669 656c 6420 696e 2066 6965  me, field in fie
-0000cfe0: 6c64 732e 6974 656d 7328 293a 0a20 2020  lds.items():.   
-0000cff0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000d000: 6669 656c 642e 6765 7428 2275 7569 6422  field.get("uuid"
-0000d010: 2c20 2275 7569 645f 6e6f 745f 666f 756e  , "uuid_not_foun
-0000d020: 6422 2920 696e 2070 6c61 7962 6f6f 6b5f  d") in playbook_
-0000d030: 6461 7461 2e67 6574 2822 696e 7075 7473  data.get("inputs
-0000d040: 222c 207b 7d29 3a0a 2020 2020 2020 2020  ", {}):.        
-0000d050: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-0000d060: 6e76 6572 7420 696e 7075 7420 7575 6964  nvert input uuid
-0000d070: 2074 6f20 696e 7075 745f 6e61 6d65 0a20   to input_name. 
-0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d090: 2020 2070 6c61 7962 6f6f 6b5f 6461 7461     playbook_data
-0000d0a0: 5b22 696e 7075 7473 225d 5b66 6965 6c64  ["inputs"][field
-0000d0b0: 2e67 6574 2822 7575 6964 2229 5d5b 2269  .get("uuid")]["i
-0000d0c0: 6e70 7574 5f6e 616d 6522 5d20 3d20 6669  nput_name"] = fi
-0000d0d0: 656c 642e 6765 7428 2274 6578 7422 290a  eld.get("text").
-0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0f0: 2020 2020 706c 6179 626f 6f6b 5f64 6174      playbook_dat
-0000d100: 615b 2269 6e70 7574 7322 5d5b 6669 656c  a["inputs"][fiel
-0000d110: 642e 6765 7428 2275 7569 6422 295d 5b22  d.get("uuid")]["
-0000d120: 696e 7075 745f 6170 695f 6e61 6d65 225d  input_api_name"]
-0000d130: 203d 2066 6965 6c64 5f6e 616d 650a 2020   = field_name.  
-0000d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d150: 2020 2320 6164 6420 696e 7075 7420 7479    # add input ty
-0000d160: 7065 0a20 2020 2020 2020 2020 2020 2020  pe.             
-0000d170: 2020 2020 2020 2070 6c61 7962 6f6f 6b5f         playbook_
-0000d180: 6461 7461 5b22 696e 7075 7473 225d 5b66  data["inputs"][f
-0000d190: 6965 6c64 2e67 6574 2822 7575 6964 2229  ield.get("uuid")
-0000d1a0: 5d5b 2269 6e70 7574 5f74 7970 655f 6e61  ]["input_type_na
-0000d1b0: 6d65 225d 203d 2066 6965 6c64 2e67 6574  me"] = field.get
-0000d1c0: 2822 696e 7075 745f 7479 7065 2229 0a20  ("input_type"). 
-0000d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1e0: 2020 2023 2073 656c 6563 7473 2061 6e64     # selects and
-0000d1f0: 206d 756c 7469 7365 6c65 6374 7320 7265   multiselects re
-0000d200: 6665 7265 6e63 6520 7468 6569 7220 5555  ference their UU
-0000d210: 4944 2069 6e20 7468 6520 6461 7461 2065  ID in the data e
-0000d220: 7874 7261 6374 6564 2066 726f 6d20 786d  xtracted from xm
-0000d230: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-0000d240: 2020 2020 2020 2023 2073 6f20 7765 206e         # so we n
-0000d250: 6565 6420 746f 2072 6570 6c61 6365 2074  eed to replace t
-0000d260: 6861 7420 7769 7468 2074 6865 2074 7275  hat with the tru
-0000d270: 6520 7661 6c75 6520 666f 756e 6420 696e  e value found in
-0000d280: 2074 6865 2073 7562 5f70 620a 2020 2020   the sub_pb.    
-0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2a0: 6966 2066 6965 6c64 2e67 6574 2822 696e  if field.get("in
-0000d2b0: 7075 745f 7479 7065 2229 203d 3d20 2273  put_type") == "s
-0000d2c0: 656c 6563 7422 3a0a 2020 2020 2020 2020  elect":.        
-0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2e0: 7365 6c65 6374 5f69 6e70 7574 5f75 7569  select_input_uui
-0000d2f0: 6420 3d20 706c 6179 626f 6f6b 5f64 6174  d = playbook_dat
-0000d300: 615b 2269 6e70 7574 7322 5d5b 6669 656c  a["inputs"][fiel
-0000d310: 642e 6765 7428 2275 7569 6422 295d 5b22  d.get("uuid")]["
-0000d320: 7374 6174 6963 5f69 6e70 7574 225d 5b22  static_input"]["
-0000d330: 7365 6c65 6374 5f76 616c 7565 225d 0a20  select_value"]. 
-0000d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d350: 2020 2020 2020 2070 6c61 7962 6f6f 6b5f         playbook_
-0000d360: 6461 7461 5b22 696e 7075 7473 225d 5b66  data["inputs"][f
-0000d370: 6965 6c64 2e67 6574 2822 7575 6964 2229  ield.get("uuid")
-0000d380: 5d5b 2273 7461 7469 635f 696e 7075 7422  ]["static_input"
-0000d390: 5d5b 2273 656c 6563 745f 7661 6c75 6522  ]["select_value"
-0000d3a0: 5d20 3d20 6e65 7874 2876 616c 7565 2e67  ] = next(value.g
-0000d3b0: 6574 2822 6c61 6265 6c22 2920 666f 7220  et("label") for 
-0000d3c0: 7661 6c75 6520 696e 2066 6965 6c64 2e67  value in field.g
-0000d3d0: 6574 2822 7661 6c75 6573 2229 2069 6620  et("values") if 
-0000d3e0: 7661 6c75 652e 6765 7428 2275 7569 6422  value.get("uuid"
-0000d3f0: 2920 3d3d 2073 656c 6563 745f 696e 7075  ) == select_inpu
-0000d400: 745f 7575 6964 290a 2020 2020 2020 2020  t_uuid).        
-0000d410: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0000d420: 2066 6965 6c64 2e67 6574 2822 696e 7075   field.get("inpu
-0000d430: 745f 7479 7065 2229 203d 3d20 226d 756c  t_type") == "mul
-0000d440: 7469 7365 6c65 6374 223a 0a20 2020 2020  tiselect":.     
-0000d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d460: 2020 2073 656c 6563 745f 696e 7075 745f     select_input_
-0000d470: 7575 6964 7320 3d20 706c 6179 626f 6f6b  uuids = playbook
-0000d480: 5f64 6174 615b 2269 6e70 7574 7322 5d5b  _data["inputs"][
-0000d490: 6669 656c 642e 6765 7428 2275 7569 6422  field.get("uuid"
-0000d4a0: 295d 5b22 7374 6174 6963 5f69 6e70 7574  )]["static_input
-0000d4b0: 225d 5b22 6d75 6c74 6973 656c 6563 745f  "]["multiselect_
-0000d4c0: 7661 6c75 6522 5d0a 2020 2020 2020 2020  value"].        
-0000d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4e0: 706c 6179 626f 6f6b 5f64 6174 615b 2269  playbook_data["i
-0000d4f0: 6e70 7574 7322 5d5b 6669 656c 642e 6765  nputs"][field.ge
-0000d500: 7428 2275 7569 6422 295d 5b22 7374 6174  t("uuid")]["stat
-0000d510: 6963 5f69 6e70 7574 225d 5b22 6d75 6c74  ic_input"]["mult
-0000d520: 6973 656c 6563 745f 7661 6c75 6522 5d20  iselect_value"] 
-0000d530: 3d20 222c 2022 2e6a 6f69 6e28 7661 6c75  = ", ".join(valu
-0000d540: 652e 6765 7428 226c 6162 656c 2229 2066  e.get("label") f
-0000d550: 6f72 2076 616c 7565 2069 6e20 6669 656c  or value in fiel
-0000d560: 642e 6765 7428 2276 616c 7565 7322 2920  d.get("values") 
-0000d570: 6966 2076 616c 7565 2e67 6574 2822 7575  if value.get("uu
-0000d580: 6964 2229 2069 6e20 7365 6c65 6374 5f69  id") in select_i
-0000d590: 6e70 7574 5f75 7569 6473 290a 0a20 2020  nput_uuids)..   
-0000d5a0: 2023 206d 616b 6520 696e 7075 7420 6561   # make input ea
-0000d5b0: 7369 6572 2074 6f20 6765 7420 696e 206a  sier to get in j
-0000d5c0: 696e 6a61 320a 2020 2020 666f 7220 5f2c  inja2.    for _,
-0000d5d0: 2069 6e70 7574 2069 6e20 706c 6179 626f   input in playbo
-0000d5e0: 6f6b 5f64 6174 612e 6765 7428 2269 6e70  ok_data.get("inp
-0000d5f0: 7574 7322 2c20 7b7d 292e 6974 656d 7328  uts", {}).items(
-0000d600: 293a 0a20 2020 2020 2020 2069 6e70 7574  ):.        input
-0000d610: 5f73 7472 5f72 6570 7220 3d20 2222 0a20  _str_repr = "". 
-0000d620: 2020 2020 2020 2069 6620 2265 7870 7265         if "expre
-0000d630: 7373 696f 6e5f 696e 7075 7422 2069 6e20  ssion_input" in 
-0000d640: 696e 7075 743a 0a20 2020 2020 2020 2020  input:.         
-0000d650: 2020 2069 6e70 7574 5f73 7472 5f72 6570     input_str_rep
-0000d660: 7220 3d20 696e 7075 742e 6765 7428 2265  r = input.get("e
-0000d670: 7870 7265 7373 696f 6e5f 696e 7075 7422  xpression_input"
-0000d680: 2c20 7b7d 292e 6765 7428 2265 7870 7265  , {}).get("expre
-0000d690: 7373 696f 6e22 2c20 2255 4e4b 4e4f 574e  ssion", "UNKNOWN
-0000d6a0: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
-0000d6b0: 2273 7461 7469 635f 696e 7075 7422 2069  "static_input" i
-0000d6c0: 6e20 696e 7075 743a 0a20 2020 2020 2020  n input:.       
-0000d6d0: 2020 2020 2069 6e5f 636f 6e74 656e 7420       in_content 
-0000d6e0: 3d20 696e 7075 742e 6765 7428 2273 7461  = input.get("sta
-0000d6f0: 7469 635f 696e 7075 7422 290a 2020 2020  tic_input").    
-0000d700: 2020 2020 2020 2020 2320 7468 6572 6527          # there'
-0000d710: 7320 6f6e 6c79 206f 6e65 2069 7465 6d20  s only one item 
-0000d720: 6576 6572 2069 6e20 696e 5f63 6f6e 7465  ever in in_conte
-0000d730: 6e74 2073 6f20 7765 2063 616e 2075 7365  nt so we can use
-0000d740: 2060 606e 6578 7428 2960 600a 2020 2020   ``next()``.    
-0000d750: 2020 2020 2020 2020 2320 6f6e 2074 6865          # on the
-0000d760: 2067 656e 6572 6174 6f72 2062 656c 6f77   generator below
-0000d770: 2074 6f20 6765 7420 7468 6520 6974 656d   to get the item
-0000d780: 2773 2076 616c 7565 0a20 2020 2020 2020  's value.       
-0000d790: 2020 2020 2069 6e70 7574 5f73 7472 5f72       input_str_r
-0000d7a0: 6570 7220 3d20 6e65 7874 2876 616c 7565  epr = next(value
-0000d7b0: 2066 6f72 205f 2c20 7661 6c75 6520 696e   for _, value in
-0000d7c0: 2069 6e5f 636f 6e74 656e 742e 6974 656d   in_content.item
-0000d7d0: 7328 2929 0a20 2020 2020 2020 2069 6e70  s()).        inp
-0000d7e0: 7574 5b22 696e 7075 745f 6173 5f73 7472  ut["input_as_str
-0000d7f0: 225d 203d 2069 6e70 7574 5f73 7472 5f72  "] = input_str_r
-0000d800: 6570 720a 0a64 6566 2067 6574 5f6d 6169  epr..def get_mai
-0000d810: 6e5f 636d 6428 293a 0a20 2020 2022 2222  n_cmd():.    """
-0000d820: 0a20 2020 2052 6574 7572 6e20 7468 6520  .    Return the 
-0000d830: 226d 6169 6e22 2063 6f6d 6d61 6e64 2066  "main" command f
-0000d840: 726f 6d20 7468 6520 636f 6d6d 616e 6420  rom the command 
-0000d850: 6c69 6e65 2e0a 0a20 2020 2045 2e67 2e20  line...    E.g. 
-0000d860: 7769 7468 2063 6f6d 6d61 6e64 206c 696e  with command lin
-0000d870: 653a 2027 2420 7265 7369 6c69 656e 742d  e: '$ resilient-
-0000d880: 7364 6b20 636f 6465 6765 6e20 2d70 2061  sdk codegen -p a
-0000d890: 6263 270a 2020 2020 7468 6973 2066 756e  bc'.    this fun
-0000d8a0: 6374 696f 6e20 7769 6c6c 2072 6574 7572  ction will retur
-0000d8b0: 6e20 2763 6f64 6567 656e 270a 2020 2020  n 'codegen'.    
-0000d8c0: 2222 220a 2020 2020 636d 645f 6c69 6e65  """.    cmd_line
-0000d8d0: 203d 2073 7973 2e61 7267 760a 0a20 2020   = sys.argv..   
-0000d8e0: 2069 6620 6c65 6e28 636d 645f 6c69 6e65   if len(cmd_line
-0000d8f0: 2920 3e20 313a 0a20 2020 2020 2020 2072  ) > 1:.        r
-0000d900: 6574 7572 6e20 636d 645f 6c69 6e65 5b31  eturn cmd_line[1
-0000d910: 5d0a 0a20 2020 2072 6574 7572 6e20 4e6f  ]..    return No
-0000d920: 6e65 0a0a 0a64 6566 2067 6574 5f74 696d  ne...def get_tim
-0000d930: 6573 7461 6d70 2874 696d 6573 7461 6d70  estamp(timestamp
-0000d940: 3d4e 6f6e 6529 3a0a 2020 2020 2222 220a  =None):.    """.
-0000d950: 2020 2020 5265 7475 726e 7320 6120 7374      Returns a st
-0000d960: 7269 6e67 206f 6620 7468 6520 6375 7272  ring of the curr
-0000d970: 656e 7420 7469 6d65 0a20 2020 2069 6e20  ent time.    in 
-0000d980: 7468 6520 666f 726d 6174 2059 5959 592d  the format YYYY-
-0000d990: 4d4d 2d44 442d 6868 3a6d 6d3a 7373 0a0a  MM-DD-hh:mm:ss..
-0000d9a0: 2020 2020 4966 2060 7469 6d65 7374 616d      If `timestam
-0000d9b0: 7060 2069 7320 6465 6669 6e65 642c 2069  p` is defined, i
-0000d9c0: 7420 7769 6c6c 2072 6574 7572 6e20 7468  t will return th
-0000d9d0: 6174 2074 696d 6573 7461 6d70 2069 6e0a  at timestamp in.
-0000d9e0: 2020 2020 7468 6520 666f 726d 6174 2059      the format Y
-0000d9f0: 5959 592d 4d4d 2d44 442d 6868 3a6d 6d3a  YYY-MM-DD-hh:mm:
-0000da00: 7373 0a0a 2020 2020 3a70 6172 616d 2074  ss..    :param t
-0000da10: 696d 6573 7461 6d70 3a20 4469 6374 696f  imestamp: Dictio
-0000da20: 6e61 7279 2077 686f 7365 206b 6579 7320  nary whose keys 
-0000da30: 6172 6520 6669 6c65 206e 616d 6573 0a20  are file names. 
-0000da40: 2020 203a 7479 7065 2074 696d 6573 7461     :type timesta
-0000da50: 6d70 3a20 666c 6f61 740a 0a20 2020 203a  mp: float..    :
-0000da60: 7265 7475 726e 3a20 5469 6d65 7374 616d  return: Timestam
-0000da70: 7020 7374 7269 6e67 0a20 2020 203a 7274  p string.    :rt
-0000da80: 7970 653a 2073 7472 0a20 2020 2022 2222  ype: str.    """
-0000da90: 0a20 2020 2054 494d 455f 464f 524d 4154  .    TIME_FORMAT
-0000daa0: 203d 2022 2559 256d 2564 2548 254d 2553   = "%Y%m%d%H%M%S
-0000dab0: 220a 0a20 2020 2069 6620 7469 6d65 7374  "..    if timest
-0000dac0: 616d 703a 0a20 2020 2020 2020 2072 6574  amp:.        ret
-0000dad0: 7572 6e20 6461 7465 7469 6d65 2e64 6174  urn datetime.dat
-0000dae0: 6574 696d 652e 6672 6f6d 7469 6d65 7374  etime.fromtimest
-0000daf0: 616d 7028 7469 6d65 7374 616d 7029 2e73  amp(timestamp).s
-0000db00: 7472 6674 696d 6528 5449 4d45 5f46 4f52  trftime(TIME_FOR
-0000db10: 4d41 5429 0a0a 2020 2020 7265 7475 726e  MAT)..    return
-0000db20: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
-0000db30: 6d65 2e6e 6f77 2829 2e73 7472 6674 696d  me.now().strftim
-0000db40: 6528 5449 4d45 5f46 4f52 4d41 5429 0a0a  e(TIME_FORMAT)..
-0000db50: 0a64 6566 2073 7472 5f74 6f5f 626f 6f6c  .def str_to_bool
-0000db60: 2876 616c 7565 293a 0a20 2020 2022 2222  (value):.    """
-0000db70: 0a20 2020 2052 6570 7265 7365 6e74 7320  .    Represents 
-0000db80: 7661 6c75 6520 6173 2062 6f6f 6c65 616e  value as boolean
-0000db90: 2e0a 2020 2020 3a70 6172 616d 2076 616c  ..    :param val
-0000dba0: 7565 3a0a 2020 2020 3a72 7479 7065 3a20  ue:.    :rtype: 
-0000dbb0: 626f 6f6c 0a20 2020 2022 2222 0a20 2020  bool.    """.   
-0000dbc0: 2076 616c 7565 203d 2073 7472 2876 616c   value = str(val
-0000dbd0: 7565 292e 6c6f 7765 7228 290a 2020 2020  ue).lower().    
-0000dbe0: 7265 7475 726e 2076 616c 7565 2069 6e20  return value in 
-0000dbf0: 2827 3127 2c20 2774 7275 6527 2c20 2779  ('1', 'true', 'y
-0000dc00: 6573 2729 0a0a 0a64 6566 2069 735f 656e  es')...def is_en
-0000dc10: 765f 7661 725f 7365 7428 656e 765f 7661  v_var_set(env_va
-0000dc20: 7229 3a0a 2020 2020 2222 220a 2020 2020  r):.    """.    
-0000dc30: 3a72 6574 7572 6e3a 2054 7275 652f 4661  :return: True/Fa
-0000dc40: 6c73 6520 6966 2065 6e76 5f76 6172 2069  lse if env_var i
-0000dc50: 7320 7365 7420 696e 2065 6e76 6972 6f6e  s set in environ
-0000dc60: 6d65 6e74 0a20 2020 203a 7274 7970 653a  ment.    :rtype:
-0000dc70: 2062 6f6f 6c0a 2020 2020 2222 220a 2020   bool.    """.  
-0000dc80: 2020 7265 7475 726e 2073 7472 5f74 6f5f    return str_to_
-0000dc90: 626f 6f6c 286f 732e 6765 7465 6e76 2865  bool(os.getenv(e
-0000dca0: 6e76 5f76 6172 2929 0a0a 0a64 6566 2067  nv_var))...def g
-0000dcb0: 6574 5f72 6573 696c 6965 6e74 5f6c 6962  et_resilient_lib
-0000dcc0: 7261 7269 6573 5f76 6572 7369 6f6e 5f74  raries_version_t
-0000dcd0: 6f5f 7573 6528 293a 0a20 2020 2022 2222  o_use():.    """
-0000dce0: 0a20 2020 203a 7265 7475 726e 3a20 5665  .    :return: Ve
-0000dcf0: 7273 696f 6e20 6f66 2072 6573 696c 6965  rsion of resilie
-0000dd00: 6e74 2d63 6972 6375 6974 7320 746f 2075  nt-circuits to u
-0000dd10: 7365 2064 6570 656e 6469 6e67 206f 6e20  se depending on 
-0000dd20: 454e 565f 5641 525f 4445 5620 7365 740a  ENV_VAR_DEV set.
-0000dd30: 2020 2020 3a72 7479 7065 3a20 7374 720a      :rtype: str.
-0000dd40: 2020 2020 2222 220a 2020 2020 6966 2069      """.    if i
-0000dd50: 735f 656e 765f 7661 725f 7365 7428 636f  s_env_var_set(co
-0000dd60: 6e73 7461 6e74 732e 454e 565f 5641 525f  nstants.ENV_VAR_
-0000dd70: 4445 5629 3a0a 2020 2020 2020 2020 7265  DEV):.        re
-0000dd80: 7475 726e 2063 6f6e 7374 616e 7473 2e52  turn constants.R
-0000dd90: 4553 494c 4945 4e54 5f4c 4942 5241 5249  ESILIENT_LIBRARI
-0000dda0: 4553 5f56 4552 5349 4f4e 5f44 4556 0a20  ES_VERSION_DEV. 
-0000ddb0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000ddc0: 2072 6574 7572 6e20 636f 6e73 7461 6e74   return constant
-0000ddd0: 732e 5245 5349 4c49 454e 545f 4c49 4252  s.RESILIENT_LIBR
-0000dde0: 4152 4945 535f 5645 5253 494f 4e0a 0a0a  ARIES_VERSION...
-0000ddf0: 6465 6620 6765 745f 7265 7369 6c69 656e  def get_resilien
-0000de00: 745f 7364 6b5f 7665 7273 696f 6e28 293a  t_sdk_version():
-0000de10: 0a20 2020 2022 2222 0a20 2020 2077 7261  .    """.    wra
-0000de20: 7070 6572 206d 6574 686f 6420 746f 2063  pper method to c
-0000de30: 616c 6c20 6765 745f 7061 636b 6167 655f  all get_package_
-0000de40: 7665 7273 696f 6e20 6f6e 2063 6f6e 7374  version on const
-0000de50: 616e 7420 5344 4b5f 5041 434b 4147 455f  ant SDK_PACKAGE_
-0000de60: 4e41 4d45 0a0a 2020 2020 3a72 6574 7572  NAME..    :retur
-0000de70: 6e3a 2061 2056 6572 7369 6f6e 206f 626a  n: a Version obj
-0000de80: 6563 740a 2020 2020 2222 220a 2020 2020  ect.    """.    
-0000de90: 7265 7475 726e 2067 6574 5f70 6163 6b61  return get_packa
-0000dea0: 6765 5f76 6572 7369 6f6e 2863 6f6e 7374  ge_version(const
-0000deb0: 616e 7473 2e53 444b 5f50 4143 4b41 4745  ants.SDK_PACKAGE
-0000dec0: 5f4e 414d 4529 0a0a 0a64 6566 2067 6574  _NAME)...def get
-0000ded0: 5f70 6163 6b61 6765 5f76 6572 7369 6f6e  _package_version
-0000dee0: 2870 6163 6b61 6765 5f6e 616d 6529 3a0a  (package_name):.
-0000def0: 2020 2020 2222 220a 2020 2020 5573 6573      """.    Uses
-0000df00: 2070 6b67 5f72 6573 6f75 7263 6573 2074   pkg_resources t
-0000df10: 6f20 7061 7273 6520 7468 6520 7665 7273  o parse the vers
-0000df20: 696f 6e20 6f66 2061 2070 6163 6b61 6765  ion of a package
-0000df30: 2069 6620 696e 7374 616c 6c65 6420 696e   if installed in
-0000df40: 2074 6865 2065 6e76 6972 6f6e 6d65 6e74   the environment
-0000df50: 2e0a 2020 2020 4966 206e 6f74 2069 6e73  ..    If not ins
-0000df60: 7461 6c6c 6564 2c20 7265 7475 726e 204e  talled, return N
-0000df70: 6f6e 650a 0a20 2020 203a 7061 7261 6d20  one..    :param 
-0000df80: 7061 636b 6167 655f 6e61 6d65 3a20 6e61  package_name: na
-0000df90: 6d65 206f 6620 7468 6520 7061 636b 6167  me of the packag
-0000dfa0: 6520 746f 2067 6574 2076 6572 7369 6f6e  e to get version
-0000dfb0: 206f 660a 2020 2020 3a74 7970 6520 7061   of.    :type pa
-0000dfc0: 636b 6167 655f 6e61 6d65 3a20 7374 720a  ckage_name: str.
-0000dfd0: 2020 2020 3a72 6574 7572 6e3a 2061 2056      :return: a V
-0000dfe0: 6572 7369 6f6e 206f 626a 6563 7420 7265  ersion object re
-0000dff0: 7072 6573 656e 7469 6e67 2074 6865 2076  presenting the v
-0000e000: 6572 7369 6f6e 206f 6620 7468 6520 6769  ersion of the gi
-0000e010: 7665 6e20 7061 636b 6167 6520 6f72 204e  ven package or N
-0000e020: 6f6e 650a 2020 2020 3a72 7479 7065 3a20  one.    :rtype: 
-0000e030: 5665 7273 696f 6e20 6f72 204e 6f6e 650a  Version or None.
-0000e040: 2020 2020 2222 220a 2020 2020 7472 793a      """.    try:
-0000e050: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000e060: 706b 675f 7265 736f 7572 6365 732e 7061  pkg_resources.pa
-0000e070: 7273 655f 7665 7273 696f 6e28 706b 675f  rse_version(pkg_
-0000e080: 7265 736f 7572 6365 732e 7265 7175 6972  resources.requir
-0000e090: 6528 7061 636b 6167 655f 6e61 6d65 295b  e(package_name)[
-0000e0a0: 305d 2e76 6572 7369 6f6e 290a 2020 2020  0].version).    
-0000e0b0: 6578 6365 7074 2070 6b67 5f72 6573 6f75  except pkg_resou
-0000e0c0: 7263 6573 2e44 6973 7472 6962 7574 696f  rces.Distributio
-0000e0d0: 6e4e 6f74 466f 756e 643a 0a20 2020 2020  nNotFound:.     
-0000e0e0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-0000e0f0: 0a64 6566 2067 6574 5f6c 6174 6573 745f  .def get_latest_
-0000e100: 7665 7273 696f 6e5f 6f6e 5f70 7970 6928  version_on_pypi(
-0000e110: 293a 0a20 2020 2022 2222 0a20 2020 2055  ):.    """.    U
-0000e120: 7365 7320 7265 7175 6573 7473 2074 6f20  ses requests to 
-0000e130: 6361 6c6c 2027 6874 7470 733a 2f2f 7079  call 'https://py
-0000e140: 7069 2e6f 7267 2f70 7970 692f 7265 7369  pi.org/pypi/resi
-0000e150: 6c69 656e 742d 7364 6b2f 6a73 6f6e 270a  lient-sdk/json'.
-0000e160: 2020 2020 746f 2067 6574 2061 204a 534f      to get a JSO
-0000e170: 4e20 6469 6374 206f 6620 616c 6c20 7468  N dict of all th
-0000e180: 6520 6176 6169 6c61 626c 6520 7665 7273  e available vers
-0000e190: 696f 6e73 206f 6e20 5079 5069 2e0a 2020  ions on PyPi..  
-0000e1a0: 2020 536f 7274 7320 7468 6520 6469 6374    Sorts the dict
-0000e1b0: 2069 6e74 6f20 6120 6c69 7374 2c20 7468   into a list, th
-0000e1c0: 656e 2067 6574 7320 7468 6520 6c61 7465  en gets the late
-0000e1d0: 7374 0a0a 2020 2020 3a72 6169 7365 7320  st..    :raises 
-0000e1e0: 4854 5450 4572 726f 723a 2069 6620 6120  HTTPError: if a 
-0000e1f0: 7072 6f62 6c65 6d20 6f63 6375 7273 2072  problem occurs r
-0000e200: 6561 6368 696e 6720 7079 7069 2e6f 7267  eaching pypi.org
-0000e210: 0a20 2020 203a 7265 7475 726e 3a20 7468  .    :return: th
-0000e220: 6520 6c61 7465 7374 2061 7661 696c 6162  e latest availab
-0000e230: 6c65 2076 6572 7369 6f6e 206f 6620 7468  le version of th
-0000e240: 6973 206c 6962 7261 7279 206f 6e20 5079  is library on Py
-0000e250: 5069 0a20 2020 203a 7274 7970 653a 2070  Pi.    :rtype: p
-0000e260: 6b67 5f72 6573 6f75 7263 6573 2e65 7874  kg_resources.ext
-0000e270: 6572 6e2e 7061 636b 6167 696e 672e 7665  ern.packaging.ve
-0000e280: 7273 696f 6e2e 5665 7273 696f 6e0a 2020  rsion.Version.  
-0000e290: 2020 2222 220a 2020 2020 7220 3d20 7265    """.    r = re
-0000e2a0: 7175 6573 7473 2e67 6574 2863 6f6e 7374  quests.get(const
-0000e2b0: 616e 7473 2e55 524c 5f50 5950 495f 5645  ants.URL_PYPI_VE
-0000e2c0: 5253 494f 4e2c 2074 696d 656f 7574 3d35  RSION, timeout=5
-0000e2d0: 290a 2020 2020 722e 7261 6973 655f 666f  ).    r.raise_fo
-0000e2e0: 725f 7374 6174 7573 2829 0a0a 2020 2020  r_status()..    
-0000e2f0: 7265 735f 6a73 6f6e 203d 2072 2e6a 736f  res_json = r.jso
-0000e300: 6e28 290a 0a20 2020 2061 7661 696c 6162  n()..    availab
-0000e310: 6c65 5f76 6572 7369 6f6e 7320 3d20 5b5d  le_versions = []
-0000e320: 0a0a 2020 2020 666f 7220 7468 655f 7665  ..    for the_ve
-0000e330: 7273 696f 6e20 696e 2072 6573 5f6a 736f  rsion in res_jso
-0000e340: 6e2e 6765 7428 2272 656c 6561 7365 7322  n.get("releases"
-0000e350: 2c20 7b7d 293a 0a0a 2020 2020 2020 2020  , {}):..        
-0000e360: 7620 3d20 706b 675f 7265 736f 7572 6365  v = pkg_resource
-0000e370: 732e 7061 7273 655f 7665 7273 696f 6e28  s.parse_version(
-0000e380: 7468 655f 7665 7273 696f 6e29 0a0a 2020  the_version)..  
-0000e390: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-0000e3a0: 6e73 7461 6e63 6528 762c 2070 6b67 5f72  nstance(v, pkg_r
-0000e3b0: 6573 6f75 7263 6573 2e65 7874 6572 6e2e  esources.extern.
-0000e3c0: 7061 636b 6167 696e 672e 7665 7273 696f  packaging.versio
-0000e3d0: 6e2e 4c65 6761 6379 5665 7273 696f 6e29  n.LegacyVersion)
-0000e3e0: 3a0a 2020 2020 2020 2020 2020 2020 6176  :.            av
-0000e3f0: 6169 6c61 626c 655f 7665 7273 696f 6e73  ailable_versions
-0000e400: 2e61 7070 656e 6428 7629 0a0a 2020 2020  .append(v)..    
-0000e410: 6176 6169 6c61 626c 655f 7665 7273 696f  available_versio
-0000e420: 6e73 203d 2073 6f72 7465 6428 6176 6169  ns = sorted(avai
-0000e430: 6c61 626c 655f 7665 7273 696f 6e73 290a  lable_versions).
-0000e440: 0a20 2020 2072 6574 7572 6e20 6176 6169  .    return avai
-0000e450: 6c61 626c 655f 7665 7273 696f 6e73 5b2d  lable_versions[-
-0000e460: 315d 0a0a 0a64 6566 2067 6574 5f6c 6174  1]...def get_lat
-0000e470: 6573 745f 6176 6169 6c61 626c 655f 7665  est_available_ve
-0000e480: 7273 696f 6e28 293a 0a20 2020 2022 2222  rsion():.    """
-0000e490: 0a20 2020 2053 6565 7320 6966 2074 6865  .    Sees if the
-0000e4a0: 206c 6174 6573 7420 7665 7273 696f 6e20   latest version 
-0000e4b0: 6973 2073 746f 7265 6420 696e 2061 2074  is stored in a t
-0000e4c0: 6d70 2066 696c 650a 2020 2020 616e 6420  mp file.    and 
-0000e4d0: 6966 2074 6865 2066 696c 6520 6973 206d  if the file is m
-0000e4e0: 6973 7369 6e67 206f 7220 7468 6520 7469  issing or the ti
-0000e4f0: 6d65 7374 616d 7020 6973 206f 6c64 6572  mestamp is older
-0000e500: 0a20 2020 2074 6861 6e20 3320 6461 7973  .    than 3 days
-0000e510: 2c20 6765 7473 2074 6865 206c 6174 6573  , gets the lates
-0000e520: 7420 7665 7273 696f 6e20 6672 6f6d 2050  t version from P
-0000e530: 7950 690a 0a20 2020 203a 7265 7475 726e  yPi..    :return
-0000e540: 3a20 7468 6520 6c61 7465 7374 2061 7661  : the latest ava
-0000e550: 696c 6162 6c65 2076 6572 7369 6f6e 206f  ilable version o
-0000e560: 6620 7468 6973 206c 6962 7261 7279 206f  f this library o
-0000e570: 6e20 5079 5069 0a20 2020 203a 7274 7970  n PyPi.    :rtyp
-0000e580: 653a 2070 6b67 5f72 6573 6f75 7263 6573  e: pkg_resources
-0000e590: 2e56 6572 7369 6f6e 0a20 2020 2022 2222  .Version.    """
-0000e5a0: 0a20 2020 206c 6174 6573 745f 6176 6169  .    latest_avai
-0000e5b0: 6c61 626c 655f 7665 7273 696f 6e20 3d20  lable_version = 
-0000e5c0: 4e6f 6e65 0a0a 2020 2020 7364 6b5f 746d  None..    sdk_tm
-0000e5d0: 705f 6469 7220 3d20 6765 745f 7364 6b5f  p_dir = get_sdk_
-0000e5e0: 746d 705f 6469 7228 290a 2020 2020 7061  tmp_dir().    pa
-0000e5f0: 7468 5f73 646b 5f74 6d70 5f70 7970 695f  th_sdk_tmp_pypi_
-0000e600: 7665 7273 696f 6e20 3d20 6f73 2e70 6174  version = os.pat
-0000e610: 682e 6a6f 696e 2873 646b 5f74 6d70 5f64  h.join(sdk_tmp_d
-0000e620: 6972 2c20 636f 6e73 7461 6e74 732e 544d  ir, constants.TM
-0000e630: 505f 5059 5049 5f56 4552 5349 4f4e 290a  P_PYPI_VERSION).
-0000e640: 0a20 2020 2069 6620 6f73 2e70 6174 682e  .    if os.path.
-0000e650: 6973 6669 6c65 2870 6174 685f 7364 6b5f  isfile(path_sdk_
-0000e660: 746d 705f 7079 7069 5f76 6572 7369 6f6e  tmp_pypi_version
-0000e670: 293a 0a20 2020 2020 2020 2070 7970 695f  ):.        pypi_
-0000e680: 7665 7273 696f 6e5f 6461 7461 203d 2072  version_data = r
-0000e690: 6561 645f 6a73 6f6e 5f66 696c 6528 7061  ead_json_file(pa
-0000e6a0: 7468 5f73 646b 5f74 6d70 5f70 7970 695f  th_sdk_tmp_pypi_
-0000e6b0: 7665 7273 696f 6e29 0a0a 2020 2020 2020  version)..      
-0000e6c0: 2020 6e6f 7720 3d20 6461 7465 7469 6d65    now = datetime
-0000e6d0: 2e64 6174 6574 696d 652e 6e6f 7728 290a  .datetime.now().
-0000e6e0: 2020 2020 2020 2020 7473 203d 2064 6174          ts = dat
-0000e6f0: 6574 696d 652e 6461 7465 7469 6d65 2e66  etime.datetime.f
-0000e700: 726f 6d74 696d 6573 7461 6d70 2870 7970  romtimestamp(pyp
-0000e710: 695f 7665 7273 696f 6e5f 6461 7461 2e67  i_version_data.g
-0000e720: 6574 2822 7473 222c 2022 2229 290a 2020  et("ts", "")).  
-0000e730: 2020 2020 2020 7265 6672 6573 685f 7079        refresh_py
-0000e740: 7069 5f64 6174 6520 3d20 7473 202b 2064  pi_date = ts + d
-0000e750: 6174 6574 696d 652e 7469 6d65 6465 6c74  atetime.timedelt
-0000e760: 6128 6461 7973 3d33 290a 0a20 2020 2020  a(days=3)..     
-0000e770: 2020 2069 6620 6e6f 7720 3e20 7265 6672     if now > refr
-0000e780: 6573 685f 7079 7069 5f64 6174 653a 0a20  esh_pypi_date:. 
-0000e790: 2020 2020 2020 2020 2020 206c 6174 6573             lates
-0000e7a0: 745f 6176 6169 6c61 626c 655f 7665 7273  t_available_vers
-0000e7b0: 696f 6e20 3d20 6765 745f 6c61 7465 7374  ion = get_latest
-0000e7c0: 5f76 6572 7369 6f6e 5f6f 6e5f 7079 7069  _version_on_pypi
-0000e7d0: 2829 0a20 2020 2020 2020 2020 2020 2077  ().            w
-0000e7e0: 7269 7465 5f6c 6174 6573 745f 7079 7069  rite_latest_pypi
-0000e7f0: 5f74 6d70 5f66 696c 6528 6c61 7465 7374  _tmp_file(latest
-0000e800: 5f61 7661 696c 6162 6c65 5f76 6572 7369  _available_versi
-0000e810: 6f6e 2c20 7061 7468 5f73 646b 5f74 6d70  on, path_sdk_tmp
-0000e820: 5f70 7970 695f 7665 7273 696f 6e29 0a0a  _pypi_version)..
-0000e830: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000e840: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000e850: 2070 6b67 5f72 6573 6f75 7263 6573 2e70   pkg_resources.p
-0000e860: 6172 7365 5f76 6572 7369 6f6e 2870 7970  arse_version(pyp
-0000e870: 695f 7665 7273 696f 6e5f 6461 7461 2e67  i_version_data.g
-0000e880: 6574 2822 7665 7273 696f 6e22 2c20 2222  et("version", ""
-0000e890: 2929 0a0a 2020 2020 656c 7365 3a0a 2020  ))..    else:.  
-0000e8a0: 2020 2020 2020 6c61 7465 7374 5f61 7661        latest_ava
-0000e8b0: 696c 6162 6c65 5f76 6572 7369 6f6e 203d  ilable_version =
-0000e8c0: 2067 6574 5f6c 6174 6573 745f 7665 7273   get_latest_vers
-0000e8d0: 696f 6e5f 6f6e 5f70 7970 6928 290a 2020  ion_on_pypi().  
-0000e8e0: 2020 2020 2020 7772 6974 655f 6c61 7465        write_late
-0000e8f0: 7374 5f70 7970 695f 746d 705f 6669 6c65  st_pypi_tmp_file
-0000e900: 286c 6174 6573 745f 6176 6169 6c61 626c  (latest_availabl
-0000e910: 655f 7665 7273 696f 6e2c 2070 6174 685f  e_version, path_
-0000e920: 7364 6b5f 746d 705f 7079 7069 5f76 6572  sdk_tmp_pypi_ver
-0000e930: 7369 6f6e 290a 0a20 2020 2072 6574 7572  sion)..    retur
-0000e940: 6e20 6c61 7465 7374 5f61 7661 696c 6162  n latest_availab
-0000e950: 6c65 5f76 6572 7369 6f6e 0a0a 0a64 6566  le_version...def
-0000e960: 2063 7265 6174 655f 746d 705f 6469 7228   create_tmp_dir(
-0000e970: 7364 6b5f 746d 705f 6469 725f 6e61 6d65  sdk_tmp_dir_name
-0000e980: 3d63 6f6e 7374 616e 7473 2e53 444b 5f52  =constants.SDK_R
-0000e990: 4553 4f55 5243 455f 4e41 4d45 2c20 746d  ESOURCE_NAME, tm
-0000e9a0: 705f 6469 723d 7465 6d70 6669 6c65 2e67  p_dir=tempfile.g
-0000e9b0: 6574 7465 6d70 6469 7228 2929 3a0a 2020  ettempdir()):.  
-0000e9c0: 2020 2222 220a 2020 2020 4368 6563 6b73    """.    Checks
-0000e9d0: 2069 6620 7573 6572 2068 6173 2063 6f72   if user has cor
-0000e9e0: 7265 6374 2070 6572 6d69 7373 696f 6e73  rect permissions
-0000e9f0: 2074 6865 6e20 6372 6561 7465 730a 2020   then creates.  
-0000ea00: 2020 7468 6520 7364 6b5f 746d 705f 6469    the sdk_tmp_di
-0000ea10: 720a 0a20 2020 203a 7061 7261 6d20 7364  r..    :param sd
-0000ea20: 6b5f 746d 705f 6469 725f 6e61 6d65 3a20  k_tmp_dir_name: 
-0000ea30: 7468 6520 6e61 6d65 2066 6f72 2074 6865  the name for the
-0000ea40: 2064 6972 2074 6f20 6372 6561 7465 2069   dir to create i
-0000ea50: 6e20 7468 6520 7379 7374 656d 2773 202f  n the system's /
-0000ea60: 746d 7020 666f 6c64 6572 0a20 2020 203a  tmp folder.    :
-0000ea70: 7479 7065 2073 646b 5f74 6d70 5f64 6972  type sdk_tmp_dir
-0000ea80: 5f6e 616d 653a 2073 7472 0a20 2020 203a  _name: str.    :
-0000ea90: 7061 7261 6d20 746d 705f 6469 723a 2074  param tmp_dir: t
-0000eaa0: 6865 2070 6174 6820 746f 2074 6865 2074  he path to the t
-0000eab0: 656d 7020 6669 6c65 7320 6c6f 6361 7469  emp files locati
-0000eac0: 6f6e 206f 6e20 7468 6520 7379 7374 656d  on on the system
-0000ead0: 0a20 2020 203a 7479 7065 2074 6d70 5f64  .    :type tmp_d
-0000eae0: 6972 3a20 7374 720a 2020 2020 3a72 6574  ir: str.    :ret
-0000eaf0: 7572 6e3a 2070 6174 6820 746f 2074 6865  urn: path to the
-0000eb00: 2073 646b 5f74 6d70 5f64 6972 0a20 2020   sdk_tmp_dir.   
-0000eb10: 203a 7274 7970 653a 2073 7472 0a20 2020   :rtype: str.   
-0000eb20: 2022 2222 0a20 2020 2076 616c 6964 6174   """.    validat
-0000eb30: 655f 6469 725f 7061 7468 7328 6f73 2e57  e_dir_paths(os.W
-0000eb40: 5f4f 4b2c 2074 6d70 5f64 6972 290a 0a20  _OK, tmp_dir).. 
-0000eb50: 2020 2070 6174 685f 7364 6b5f 746d 705f     path_sdk_tmp_
-0000eb60: 6469 7220 3d20 6f73 2e70 6174 682e 6a6f  dir = os.path.jo
-0000eb70: 696e 2874 6d70 5f64 6972 2c20 7364 6b5f  in(tmp_dir, sdk_
-0000eb80: 746d 705f 6469 725f 6e61 6d65 290a 0a20  tmp_dir_name).. 
-0000eb90: 2020 206f 732e 6d61 6b65 6469 7273 2870     os.makedirs(p
-0000eba0: 6174 685f 7364 6b5f 746d 705f 6469 7229  ath_sdk_tmp_dir)
-0000ebb0: 0a0a 2020 2020 7265 7475 726e 2070 6174  ..    return pat
-0000ebc0: 685f 7364 6b5f 746d 705f 6469 720a 0a0a  h_sdk_tmp_dir...
-0000ebd0: 6465 6620 6765 745f 7364 6b5f 746d 705f  def get_sdk_tmp_
-0000ebe0: 6469 7228 7364 6b5f 746d 705f 6469 725f  dir(sdk_tmp_dir_
-0000ebf0: 6e61 6d65 3d63 6f6e 7374 616e 7473 2e53  name=constants.S
-0000ec00: 444b 5f52 4553 4f55 5243 455f 4e41 4d45  DK_RESOURCE_NAME
-0000ec10: 2c20 746d 705f 6469 723d 7465 6d70 6669  , tmp_dir=tempfi
-0000ec20: 6c65 2e67 6574 7465 6d70 6469 7228 2929  le.gettempdir())
-0000ec30: 3a0a 2020 2020 2222 220a 2020 2020 4765  :.    """.    Ge
-0000ec40: 7473 2074 6865 2070 6174 6820 746f 2074  ts the path to t
-0000ec50: 6865 2073 646b 5f74 6d70 5f64 6972 206f  he sdk_tmp_dir o
-0000ec60: 7220 6372 6561 7465 7320 6974 2069 6620  r creates it if 
-0000ec70: 6974 2064 6f65 730a 2020 2020 6e6f 7420  it does.    not 
-0000ec80: 6578 6973 740a 0a20 2020 203a 7061 7261  exist..    :para
-0000ec90: 6d20 7364 6b5f 746d 705f 6469 725f 6e61  m sdk_tmp_dir_na
-0000eca0: 6d65 3a20 7468 6520 6e61 6d65 2066 6f72  me: the name for
-0000ecb0: 2074 6865 2064 6972 206e 6f72 6d61 6c6c   the dir normall
-0000ecc0: 7920 7468 6520 6e61 6d65 206f 6620 7468  y the name of th
-0000ecd0: 6520 7061 636b 6167 650a 2020 2020 3a74  e package.    :t
-0000ece0: 7970 6520 7364 6b5f 746d 705f 6469 725f  ype sdk_tmp_dir_
-0000ecf0: 6e61 6d65 3a20 7374 720a 2020 2020 3a70  name: str.    :p
-0000ed00: 6172 616d 2074 6d70 5f64 6972 3a20 7468  aram tmp_dir: th
-0000ed10: 6520 7061 7468 2074 6f20 7468 6520 7465  e path to the te
-0000ed20: 6d70 2066 696c 6573 206c 6f63 6174 696f  mp files locatio
-0000ed30: 6e20 6f6e 2074 6865 2073 7973 7465 6d0a  n on the system.
-0000ed40: 2020 2020 3a74 7970 6520 746d 705f 6469      :type tmp_di
-0000ed50: 723a 2073 7472 0a20 2020 203a 7265 7475  r: str.    :retu
-0000ed60: 726e 3a20 7061 7468 2074 6f20 7468 6520  rn: path to the 
-0000ed70: 7364 6b5f 746d 705f 6469 720a 2020 2020  sdk_tmp_dir.    
-0000ed80: 3a72 7479 7065 3a20 7374 720a 2020 2020  :rtype: str.    
-0000ed90: 2222 220a 2020 2020 7061 7468 5f73 646b  """.    path_sdk
-0000eda0: 5f74 6d70 5f64 6972 203d 206f 732e 7061  _tmp_dir = os.pa
-0000edb0: 7468 2e6a 6f69 6e28 746d 705f 6469 722c  th.join(tmp_dir,
-0000edc0: 2073 646b 5f74 6d70 5f64 6972 5f6e 616d   sdk_tmp_dir_nam
-0000edd0: 6529 0a0a 2020 2020 6966 206e 6f74 206f  e)..    if not o
-0000ede0: 732e 7061 7468 2e69 7364 6972 2870 6174  s.path.isdir(pat
-0000edf0: 685f 7364 6b5f 746d 705f 6469 7229 3a0a  h_sdk_tmp_dir):.
-0000ee00: 2020 2020 2020 2020 7061 7468 5f73 646b          path_sdk
-0000ee10: 5f74 6d70 5f64 6972 203d 2063 7265 6174  _tmp_dir = creat
-0000ee20: 655f 746d 705f 6469 7228 7364 6b5f 746d  e_tmp_dir(sdk_tm
-0000ee30: 705f 6469 725f 6e61 6d65 2c20 746d 705f  p_dir_name, tmp_
-0000ee40: 6469 7229 0a0a 2020 2020 7265 7475 726e  dir)..    return
-0000ee50: 2070 6174 685f 7364 6b5f 746d 705f 6469   path_sdk_tmp_di
-0000ee60: 720a 0a0a 6465 6620 6973 5f70 7974 686f  r...def is_pytho
-0000ee70: 6e5f 6d69 6e5f 7375 7070 6f72 7465 645f  n_min_supported_
-0000ee80: 7665 7273 696f 6e28 6375 7374 6f6d 5f77  version(custom_w
-0000ee90: 6172 6e69 6e67 3d4e 6f6e 6529 3a0a 2020  arning=None):.  
-0000eea0: 2020 2222 220a 2020 2020 4c6f 6773 2061    """.    Logs a
-0000eeb0: 2057 4152 4e49 4e47 2069 6620 7468 6520   WARNING if the 
-0000eec0: 6375 7272 656e 7420 7665 7273 696f 6e20  current version 
-0000eed0: 6f66 2050 7974 686f 6e20 6973 206e 6f74  of Python is not
-0000eee0: 203e 3d20 4d49 4e5f 5355 5050 4f52 5445   >= MIN_SUPPORTE
-0000eef0: 445f 5059 5f56 4552 5349 4f4e 0a20 2020  D_PY_VERSION.   
-0000ef00: 203a 7061 7261 6d20 6375 7374 6f6d 5f77   :param custom_w
-0000ef10: 6172 6e69 6e67 3a20 6120 6375 7374 6f6d  arning: a custom
-0000ef20: 206d 6573 7361 6765 2079 6f75 2077 616e   message you wan
-0000ef30: 7420 746f 206c 6f67 206f 7574 0a20 2020  t to log out.   
-0000ef40: 203a 7479 7065 2063 7573 746f 6d5f 7761   :type custom_wa
-0000ef50: 726e 696e 673a 2073 7472 0a20 2020 203a  rning: str.    :
-0000ef60: 7265 7475 726e 3a20 6120 626f 6f6c 6561  return: a boolea
-0000ef70: 6e20 746f 2069 6e64 6963 6174 6520 6966  n to indicate if
-0000ef80: 2063 7572 7265 6e74 2076 6572 7369 6f6e   current version
-0000ef90: 2069 7320 7375 7070 6f72 7465 6420 6f72   is supported or
-0000efa0: 206e 6f74 0a20 2020 203a 7274 7970 653a   not.    :rtype:
-0000efb0: 2062 6f6f 6c0a 2020 2020 2222 220a 2020   bool.    """.  
-0000efc0: 2020 6966 2073 7973 2e76 6572 7369 6f6e    if sys.version
-0000efd0: 5f69 6e66 6f20 3c20 636f 6e73 7461 6e74  _info < constant
-0000efe0: 732e 4d49 4e5f 5355 5050 4f52 5445 445f  s.MIN_SUPPORTED_
-0000eff0: 5059 5f56 4552 5349 4f4e 3a0a 0a20 2020  PY_VERSION:..   
-0000f000: 2020 2020 2069 6620 6375 7374 6f6d 5f77       if custom_w
-0000f010: 6172 6e69 6e67 3a0a 2020 2020 2020 2020  arning:.        
-0000f020: 2020 2020 4c4f 472e 7761 726e 696e 6728      LOG.warning(
-0000f030: 2257 4152 4e49 4e47 3a20 2573 222c 2063  "WARNING: %s", c
-0000f040: 7573 746f 6d5f 7761 726e 696e 6729 0a0a  ustom_warning)..
-0000f050: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000f060: 2020 2020 2020 2020 2020 4c4f 472e 7761            LOG.wa
-0000f070: 726e 696e 6728 2257 4152 4e49 4e47 3a20  rning("WARNING: 
-0000f080: 7468 6973 2070 6163 6b61 6765 2073 686f  this package sho
-0000f090: 756c 6420 6f6e 6c79 2062 6520 696e 7374  uld only be inst
-0000f0a0: 616c 6c65 6420 6f6e 2061 2050 7974 686f  alled on a Pytho
-0000f0b0: 6e20 456e 7669 726f 6e6d 656e 7420 3e3d  n Environment >=
-0000f0c0: 207b 307d 2e7b 317d 2022 0a20 2020 2020   {0}.{1} ".     
+00005df0: 2061 7274 6966 6163 745f 7479 7065 733d   artifact_types=
+00005e00: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+00005e10: 2020 2020 2020 2020 696e 6369 6465 6e74          incident
+00005e20: 5f74 7970 6573 3d5b 5d2c 0a20 2020 2020  _types=[],.     
+00005e30: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00005e40: 6174 6174 6162 6c65 733d 5b5d 2c0a 2020  atatables=[],.  
+00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e60: 2020 7461 736b 733d 5b5d 2c0a 2020 2020    tasks=[],.    
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e80: 7363 7269 7074 733d 5b5d 2c0a 2020 2020  scripts=[],.    
+00005e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ea0: 706c 6179 626f 6f6b 733d 5b5d 2c0a 2020  playbooks=[],.  
+00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ec0: 2020 6170 7073 3d5b 5d2c 0a20 2020 2020    apps=[],.     
+00005ed0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00005ee0: 6574 5f72 656c 6174 6564 5f6f 626a 6563  et_related_objec
+00005ef0: 7473 3d54 7275 6529 3a0a 2020 2020 2222  ts=True):.    ""
+00005f00: 220a 2020 2020 5265 7475 726e 2061 2044  ".    Return a D
+00005f10: 6963 7469 6f6e 6172 7920 6f66 2052 6573  ictionary of Res
+00005f20: 696c 6965 6e74 204f 626a 6563 7473 2074  ilient Objects t
+00005f30: 6861 7420 6172 6520 666f 756e 6420 696e  hat are found in
+00005f40: 2074 6865 2045 7870 6f72 742e 0a20 2020   the Export..   
+00005f50: 2054 6865 2070 6172 616d 6574 6572 7320   The parameters 
+00005f60: 6172 6520 4c69 7374 7320 6f66 2074 6865  are Lists of the
+00005f70: 204f 626a 6563 7473 2079 6f75 2077 616e   Objects you wan
+00005f80: 740a 0a20 2020 203a 7061 7261 6d20 6578  t..    :param ex
+00005f90: 706f 7274 3a20 5468 6520 7265 7375 6c74  port: The result
+00005fa0: 206f 6620 6361 6c6c 696e 6720 6765 745f   of calling get_
+00005fb0: 6c61 7465 7374 5f6f 7267 5f65 7870 6f72  latest_org_expor
+00005fc0: 7428 290a 2020 2020 3a74 7970 6520 6578  t().    :type ex
+00005fd0: 706f 7274 3a20 4469 6374 0a20 2020 203a  port: Dict.    :
+00005fe0: 7061 7261 6d20 6d65 7373 6167 655f 6465  param message_de
+00005ff0: 7374 696e 6174 696f 6e73 3a20 4c69 7374  stinations: List
+00006000: 206f 6620 4d65 7373 6167 6520 4465 7374   of Message Dest
+00006010: 696e 6174 696f 6e20 4150 4920 4e61 6d65  ination API Name
+00006020: 730a 2020 2020 3a70 6172 616d 2066 756e  s.    :param fun
+00006030: 6374 696f 6e73 3a20 4c69 7374 206f 6620  ctions: List of 
+00006040: 4675 6e63 7469 6f6e 2041 5049 204e 616d  Function API Nam
+00006050: 6573 0a20 2020 203a 7061 7261 6d20 776f  es.    :param wo
+00006060: 726b 666c 6f77 733a 204c 6973 7420 6f66  rkflows: List of
+00006070: 2057 6f72 6b66 6c6f 7720 4150 4920 4e61   Workflow API Na
+00006080: 6d65 730a 2020 2020 3a70 6172 616d 2072  mes.    :param r
+00006090: 756c 6573 3a20 4c69 7374 206f 6620 5275  ules: List of Ru
+000060a0: 6c65 2044 6973 706c 6179 204e 616d 6573  le Display Names
+000060b0: 0a20 2020 203a 7061 7261 6d20 6669 656c  .    :param fiel
+000060c0: 6473 3a20 4c69 7374 206f 6620 4669 656c  ds: List of Fiel
+000060d0: 6420 4150 4920 4e61 6d65 730a 2020 2020  d API Names.    
+000060e0: 3a70 6172 616d 2061 7274 6966 6163 745f  :param artifact_
+000060f0: 7479 7065 733a 204c 6973 7420 6f66 2043  types: List of C
+00006100: 7573 746f 6d20 4172 7469 6661 6374 2054  ustom Artifact T
+00006110: 7970 6520 4150 4920 4e61 6d65 730a 2020  ype API Names.  
+00006120: 2020 3a70 6172 616d 2069 6e63 6964 656e    :param inciden
+00006130: 745f 7479 7065 733a 204c 6973 7420 6f66  t_types: List of
+00006140: 2043 7573 746f 6d20 496e 6369 6465 6e74   Custom Incident
+00006150: 2054 7970 6520 4150 4920 4e61 6d65 730a   Type API Names.
+00006160: 2020 2020 3a70 6172 616d 2064 6174 6174      :param datat
+00006170: 6162 6c65 733a 204c 6973 7420 6f66 2044  ables: List of D
+00006180: 6174 6120 5461 626c 6520 4150 4920 4e61  ata Table API Na
+00006190: 6d65 730a 2020 2020 3a70 6172 616d 2074  mes.    :param t
+000061a0: 6173 6b73 3a20 4c69 7374 206f 6620 4375  asks: List of Cu
+000061b0: 7374 6f6d 2054 6173 6b20 4150 4920 4e61  stom Task API Na
+000061c0: 6d65 730a 2020 2020 3a70 6172 616d 2073  mes.    :param s
+000061d0: 6372 6970 7473 3a20 4c69 7374 206f 6620  cripts: List of 
+000061e0: 5363 7269 7074 2044 6973 706c 6179 204e  Script Display N
+000061f0: 616d 6573 0a20 2020 203a 7061 7261 6d20  ames.    :param 
+00006200: 706c 6179 626f 6f6b 733a 204c 6973 7420  playbooks: List 
+00006210: 6f66 2050 6c61 7962 6f6f 6b20 4150 4920  of Playbook API 
+00006220: 4e61 6d65 730a 2020 2020 3a70 6172 616d  Names.    :param
+00006230: 2067 6574 5f72 656c 6174 6564 5f6f 626a   get_related_obj
+00006240: 6563 7473 3a20 5768 6574 6865 7220 6f72  ects: Whether or
+00006250: 206e 6f74 2074 6f20 6875 6e74 2066 6f72   not to hunt for
+00006260: 2072 656c 6174 6564 2061 6374 696f 6e20   related action 
+00006270: 6f62 6a65 6374 732c 2064 6566 6175 6c74  objects, default
+00006280: 7320 746f 2054 7275 650a 2020 2020 3a72  s to True.    :r
+00006290: 6574 7572 6e3a 2052 6574 7572 6e20 6120  eturn: Return a 
+000062a0: 4469 6374 696f 6e61 7279 206f 6620 5265  Dictionary of Re
+000062b0: 7369 6c69 656e 7420 4f62 6a65 6374 730a  silient Objects.
+000062c0: 2020 2020 3a72 7479 7065 3a20 4469 6374      :rtype: Dict
+000062d0: 0a20 2020 2022 2222 0a0a 2020 2020 2320  .    """..    # 
+000062e0: 4372 6561 7465 2061 2064 6565 7063 6f70  Create a deepcop
+000062f0: 7920 6f66 2074 6865 2065 7870 6f72 742c  y of the export,
+00006300: 2073 6f20 7765 2064 6f6e 2774 206f 7665   so we don't ove
+00006310: 7277 7269 7465 2074 6865 206f 7269 6769  rwrite the origi
+00006320: 6e61 6c0a 2020 2020 6578 706f 7274 203d  nal.    export =
+00006330: 2063 6f70 792e 6465 6570 636f 7079 2865   copy.deepcopy(e
+00006340: 7870 6f72 7429 0a0a 2020 2020 2320 5365  xport)..    # Se
+00006350: 7420 7061 7261 6d61 7465 7273 2074 6f20  t paramaters to 
+00006360: 4c69 7374 7320 6966 2066 616c 7379 0a20  Lists if falsy. 
+00006370: 2020 206d 6573 7361 6765 5f64 6573 7469     message_desti
+00006380: 6e61 7469 6f6e 7320 3d20 6d65 7373 6167  nations = messag
+00006390: 655f 6465 7374 696e 6174 696f 6e73 2069  e_destinations i
+000063a0: 6620 6d65 7373 6167 655f 6465 7374 696e  f message_destin
+000063b0: 6174 696f 6e73 2065 6c73 6520 5b5d 0a20  ations else []. 
+000063c0: 2020 2066 756e 6374 696f 6e73 203d 2066     functions = f
+000063d0: 756e 6374 696f 6e73 2069 6620 6675 6e63  unctions if func
+000063e0: 7469 6f6e 7320 656c 7365 205b 5d0a 2020  tions else [].  
+000063f0: 2020 776f 726b 666c 6f77 7320 3d20 776f    workflows = wo
+00006400: 726b 666c 6f77 7320 6966 2077 6f72 6b66  rkflows if workf
+00006410: 6c6f 7773 2065 6c73 6520 5b5d 0a20 2020  lows else [].   
+00006420: 2072 756c 6573 203d 2072 756c 6573 2069   rules = rules i
+00006430: 6620 7275 6c65 7320 656c 7365 205b 5d0a  f rules else [].
+00006440: 2020 2020 6669 656c 6473 203d 2066 6965      fields = fie
+00006450: 6c64 7320 6966 2066 6965 6c64 7320 656c  lds if fields el
+00006460: 7365 205b 5d0a 2020 2020 6172 7469 6661  se [].    artifa
+00006470: 6374 5f74 7970 6573 203d 2061 7274 6966  ct_types = artif
+00006480: 6163 745f 7479 7065 7320 6966 2061 7274  act_types if art
+00006490: 6966 6163 745f 7479 7065 7320 656c 7365  ifact_types else
+000064a0: 205b 5d0a 2020 2020 696e 6369 6465 6e74   [].    incident
+000064b0: 5f74 7970 6573 203d 2069 6e63 6964 656e  _types = inciden
+000064c0: 745f 7479 7065 7320 6966 2069 6e63 6964  t_types if incid
+000064d0: 656e 745f 7479 7065 7320 656c 7365 205b  ent_types else [
+000064e0: 5d0a 2020 2020 6461 7461 7461 626c 6573  ].    datatables
+000064f0: 203d 2064 6174 6174 6162 6c65 7320 6966   = datatables if
+00006500: 2064 6174 6174 6162 6c65 7320 656c 7365   datatables else
+00006510: 205b 5d0a 2020 2020 7461 736b 7320 3d20   [].    tasks = 
+00006520: 7461 736b 7320 6966 2074 6173 6b73 2065  tasks if tasks e
+00006530: 6c73 6520 5b5d 0a20 2020 2073 6372 6970  lse [].    scrip
+00006540: 7473 203d 2073 6372 6970 7473 2069 6620  ts = scripts if 
+00006550: 7363 7269 7074 7320 656c 7365 205b 5d0a  scripts else [].
+00006560: 2020 2020 706c 6179 626f 6f6b 7320 3d20      playbooks = 
+00006570: 706c 6179 626f 6f6b 7320 6966 2070 6c61  playbooks if pla
+00006580: 7962 6f6f 6b73 2065 6c73 6520 5b5d 0a0a  ybooks else []..
+00006590: 2020 2020 2320 4469 6374 2074 6f20 7265      # Dict to re
+000065a0: 7475 726e 0a20 2020 2072 6574 7572 6e5f  turn.    return_
+000065b0: 6469 6374 203d 207b 0a20 2020 2020 2020  dict = {.       
+000065c0: 2022 616c 6c5f 6669 656c 6473 223a 205b   "all_fields": [
+000065d0: 5d0a 2020 2020 7d0a 0a20 2020 2023 2047  ].    }..    # G
+000065e0: 6574 2052 756c 6573 0a20 2020 2072 6574  et Rules.    ret
+000065f0: 7572 6e5f 6469 6374 5b22 7275 6c65 7322  urn_dict["rules"
+00006600: 5d20 3d20 6765 745f 7265 735f 6f62 6a28  ] = get_res_obj(
+00006610: 2261 6374 696f 6e73 222c 2052 6573 696c  "actions", Resil
+00006620: 6965 6e74 4f62 6a4d 6170 2e52 554c 4553  ientObjMap.RULES
+00006630: 2c20 2252 756c 6522 2c20 7275 6c65 732c  , "Rule", rules,
+00006640: 2065 7870 6f72 7429 0a0a 2020 2020 6966   export)..    if
+00006650: 2067 6574 5f72 656c 6174 6564 5f6f 626a   get_related_obj
+00006660: 6563 7473 3a0a 2020 2020 2020 2020 2320  ects:.        # 
+00006670: 466f 7220 5275 6c65 7320 7765 2061 7474  For Rules we att
+00006680: 656d 7074 2074 6f20 6c6f 6361 7465 2072  empt to locate r
+00006690: 656c 6174 6564 2077 6f72 6b66 6c6f 7773  elated workflows
+000066a0: 2061 6e64 206d 6573 7361 6765 5f64 6573   and message_des
+000066b0: 7469 6e61 7469 6f6e 730a 2020 2020 2020  tinations.      
+000066c0: 2020 666f 7220 7220 696e 2072 6574 7572    for r in retur
+000066d0: 6e5f 6469 6374 2e67 6574 2822 7275 6c65  n_dict.get("rule
+000066e0: 7322 293a 0a0a 2020 2020 2020 2020 2020  s"):..          
+000066f0: 2020 2320 4765 7420 4163 7469 7669 7479    # Get Activity
+00006700: 2046 6965 6c64 7320 666f 7220 5275 6c65   Fields for Rule
+00006710: 730a 2020 2020 2020 2020 2020 2020 7669  s.            vi
+00006720: 6577 5f69 7465 6d73 203d 2072 2e67 6574  ew_items = r.get
+00006730: 2822 7669 6577 5f69 7465 6d73 222c 205b  ("view_items", [
+00006740: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
+00006750: 6374 6976 6974 795f 6669 656c 645f 7575  ctivity_field_uu
+00006760: 6964 7320 3d20 5b76 2e67 6574 2822 636f  ids = [v.get("co
+00006770: 6e74 656e 7422 2920 666f 7220 7620 696e  ntent") for v in
+00006780: 2076 6965 775f 6974 656d 7320 6966 2022   view_items if "
+00006790: 636f 6e74 656e 7422 2069 6e20 7620 616e  content" in v an
+000067a0: 6420 762e 6765 7428 2266 6965 6c64 5f74  d v.get("field_t
+000067b0: 7970 6522 2920 3d3d 2052 6573 696c 6965  ype") == Resilie
+000067c0: 6e74 4669 656c 6454 7970 6573 2e41 4354  ntFieldTypes.ACT
+000067d0: 4956 4954 595f 4649 454c 445d 0a20 2020  IVITY_FIELD].   
+000067e0: 2020 2020 2020 2020 2072 5b22 6163 7469           r["acti
+000067f0: 7669 7479 5f66 6965 6c64 7322 5d20 3d20  vity_fields"] = 
+00006800: 6765 745f 7265 735f 6f62 6a28 2266 6965  get_res_obj("fie
+00006810: 6c64 7322 2c20 2275 7569 6422 2c20 2241  lds", "uuid", "A
+00006820: 6374 6976 6974 7920 4669 656c 6422 2c20  ctivity Field", 
+00006830: 6163 7469 7669 7479 5f66 6965 6c64 5f75  activity_field_u
+00006840: 7569 6473 2c20 6578 706f 7274 290a 2020  uids, export).  
+00006850: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00006860: 5f64 6963 745b 2261 6c6c 5f66 6965 6c64  _dict["all_field
+00006870: 7322 5d2e 6578 7465 6e64 285b 7522 6163  s"].extend([u"ac
+00006880: 7469 6f6e 696e 766f 6361 7469 6f6e 2f7b  tioninvocation/{
+00006890: 307d 222e 666f 726d 6174 2866 6c64 2e67  0}".format(fld.g
+000068a0: 6574 2822 6e61 6d65 2229 2920 666f 7220  et("name")) for 
+000068b0: 666c 6420 696e 2072 2e67 6574 2822 6163  fld in r.get("ac
+000068c0: 7469 7669 7479 5f66 6965 6c64 7322 295d  tivity_fields")]
+000068d0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+000068e0: 2047 6574 206e 616d 6573 206f 6620 576f   Get names of Wo
+000068f0: 726b 666c 6f77 7320 7468 6174 2061 7265  rkflows that are
+00006900: 2072 656c 6174 6564 2074 6f20 5275 6c65   related to Rule
+00006910: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00006920: 2077 2069 6e20 722e 6765 7428 2277 6f72   w in r.get("wor
+00006930: 6b66 6c6f 7773 222c 205b 5d29 3a0a 2020  kflows", []):.  
+00006940: 2020 2020 2020 2020 2020 2020 2020 776f                wo
+00006950: 726b 666c 6f77 732e 6170 7065 6e64 2877  rkflows.append(w
+00006960: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00006970: 2047 6574 206e 616d 6573 206f 6620 4d65   Get names of Me
+00006980: 7373 6167 6520 4465 7374 696e 6174 696f  ssage Destinatio
+00006990: 6e73 2074 6861 7420 6172 6520 7265 6c61  ns that are rela
+000069a0: 7465 6420 746f 2052 756c 650a 2020 2020  ted to Rule.    
+000069b0: 2020 2020 2020 2020 2320 4d65 7373 6167          # Messag
+000069c0: 6520 4465 7374 696e 6174 696f 6e73 2069  e Destinations i
+000069d0: 6e20 5275 6c65 7320 6172 6520 6964 656e  n Rules are iden
+000069e0: 7469 6669 6564 2062 7920 7468 6569 7220  tified by their 
+000069f0: 4469 7370 6c61 7920 4e61 6d65 0a20 2020  Display Name.   
+00006a00: 2020 2020 2020 2020 2066 6f72 206d 2069           for m i
+00006a10: 6e20 722e 6765 7428 226d 6573 7361 6765  n r.get("message
+00006a20: 5f64 6573 7469 6e61 7469 6f6e 7322 2c20  _destinations", 
+00006a30: 5b5d 293a 0a20 2020 2020 2020 2020 2020  []):.           
+00006a40: 2020 2020 206d 6573 7361 6765 5f64 6573       message_des
+00006a50: 7469 6e61 7469 6f6e 732e 6170 7065 6e64  tinations.append
+00006a60: 287b 2269 6465 6e74 6966 6965 7222 3a20  ({"identifier": 
+00006a70: 226e 616d 6522 2c20 2276 616c 7565 223a  "name", "value":
+00006a80: 206d 7d29 0a0a 2020 2020 2020 2020 2020   m})..          
+00006a90: 2020 2320 4765 7420 6e61 6d65 7320 6f66    # Get names of
+00006aa0: 2054 6173 6b73 2f53 6372 6970 7473 2f46   Tasks/Scripts/F
+00006ab0: 6965 6c64 7320 7468 6174 2061 7265 2072  ields that are r
+00006ac0: 656c 6174 6564 2074 6f20 5275 6c65 0a20  elated to Rule. 
+00006ad0: 2020 2020 2020 2020 2020 2061 7574 6f6d             autom
+00006ae0: 6174 696f 6e73 203d 2072 2e67 6574 2822  ations = r.get("
+00006af0: 6175 746f 6d61 7469 6f6e 7322 2c20 5b5d  automations", []
+00006b00: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+00006b10: 7220 6120 696e 2061 7574 6f6d 6174 696f  r a in automatio
+00006b20: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00006b30: 2020 2020 6966 2061 2e67 6574 2822 7461      if a.get("ta
+00006b40: 736b 735f 746f 5f63 7265 6174 6522 293a  sks_to_create"):
+00006b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006b60: 2020 2020 2066 6f72 2074 2069 6e20 615b       for t in a[
+00006b70: 2274 6173 6b73 5f74 6f5f 6372 6561 7465  "tasks_to_create
+00006b80: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+00006b90: 2020 2020 2020 2020 2020 2020 7461 736b              task
+00006ba0: 732e 6170 7065 6e64 2874 290a 0a20 2020  s.append(t)..   
+00006bb0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00006bc0: 6620 612e 6765 7428 2273 6372 6970 7473  f a.get("scripts
+00006bd0: 5f74 6f5f 7275 6e22 293a 0a20 2020 2020  _to_run"):.     
+00006be0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006bf0: 6372 6970 7473 2e61 7070 656e 6428 612e  cripts.append(a.
+00006c00: 6765 7428 2273 6372 6970 7473 5f74 6f5f  get("scripts_to_
+00006c10: 7275 6e22 2929 0a0a 2020 2020 2020 2020  run"))..        
+00006c20: 2020 2020 2020 2020 656c 6966 2061 2e67          elif a.g
+00006c30: 6574 2822 6669 656c 6422 293a 0a20 2020  et("field"):.   
+00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c50: 2066 6965 6c64 732e 6170 7065 6e64 2861   fields.append(a
+00006c60: 2e67 6574 2822 6669 656c 6422 2929 0a0a  .get("field"))..
+00006c70: 2020 2020 2320 4765 7420 4675 6e63 7469      # Get Functi
+00006c80: 6f6e 730a 2020 2020 6966 2067 6574 5f72  ons.    if get_r
+00006c90: 656c 6174 6564 5f6f 626a 6563 7473 3a0a  elated_objects:.
+00006ca0: 2020 2020 2020 2020 2320 466f 7220 6675          # For fu
+00006cb0: 6e63 7469 6f6e 7320 7765 2061 7474 656d  nctions we attem
+00006cc0: 7074 2074 6f20 6c6f 6361 7465 2072 656c  pt to locate rel
+00006cd0: 6174 6564 206d 6573 7361 6765 2064 6573  ated message des
+00006ce0: 7469 6e61 7469 6f6e 730a 2020 2020 2020  tinations.      
+00006cf0: 2020 2320 4765 7420 4675 6e63 7469 6f6e    # Get Function
+00006d00: 206e 616d 6573 2074 6861 7420 7573 6520   names that use 
+00006d10: 2777 616e 7465 6427 204d 6573 7361 6765  'wanted' Message
+00006d20: 2044 6573 7469 6e61 7469 6f6e 730a 2020   Destinations.  
+00006d30: 2020 2020 2020 666f 7220 6620 696e 2065        for f in e
+00006d40: 7870 6f72 742e 6765 7428 2266 756e 6374  xport.get("funct
+00006d50: 696f 6e73 222c 205b 5d29 3a0a 2020 2020  ions", []):.    
+00006d60: 2020 2020 2020 2020 6966 2066 2e67 6574          if f.get
+00006d70: 2822 6465 7374 696e 6174 696f 6e5f 6861  ("destination_ha
+00006d80: 6e64 6c65 2229 2069 6e20 6d65 7373 6167  ndle") in messag
+00006d90: 655f 6465 7374 696e 6174 696f 6e73 3a0a  e_destinations:.
+00006da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006db0: 6675 6e63 7469 6f6e 732e 6170 7065 6e64  functions.append
+00006dc0: 2866 2e67 6574 2852 6573 696c 6965 6e74  (f.get(Resilient
+00006dd0: 4f62 6a4d 6170 2e46 554e 4354 494f 4e53  ObjMap.FUNCTIONS
+00006de0: 2929 0a0a 2020 2020 7265 7475 726e 5f64  ))..    return_d
+00006df0: 6963 745b 2266 756e 6374 696f 6e73 225d  ict["functions"]
+00006e00: 203d 2067 6574 5f72 6573 5f6f 626a 2822   = get_res_obj("
+00006e10: 6675 6e63 7469 6f6e 7322 2c20 5265 7369  functions", Resi
+00006e20: 6c69 656e 744f 626a 4d61 702e 4655 4e43  lientObjMap.FUNC
+00006e30: 5449 4f4e 532c 2022 4675 6e63 7469 6f6e  TIONS, "Function
+00006e40: 222c 2066 756e 6374 696f 6e73 2c20 6578  ", functions, ex
+00006e50: 706f 7274 290a 0a20 2020 2066 6f72 2066  port)..    for f
+00006e60: 2069 6e20 7265 7475 726e 5f64 6963 742e   in return_dict.
+00006e70: 6765 7428 2266 756e 6374 696f 6e73 2229  get("functions")
+00006e80: 3a0a 2020 2020 2020 2020 2320 4765 7420  :.        # Get 
+00006e90: 4675 6e63 7469 6f6e 2049 6e70 7574 730a  Function Inputs.
+00006ea0: 2020 2020 2020 2020 7669 6577 5f69 7465          view_ite
+00006eb0: 6d73 203d 2066 2e67 6574 2822 7669 6577  ms = f.get("view
+00006ec0: 5f69 7465 6d73 222c 205b 5d29 0a20 2020  _items", []).   
+00006ed0: 2020 2020 2066 756e 6374 696f 6e5f 696e       function_in
+00006ee0: 7075 745f 7575 6964 7320 3d20 5b76 2e67  put_uuids = [v.g
+00006ef0: 6574 2822 636f 6e74 656e 7422 2920 666f  et("content") fo
+00006f00: 7220 7620 696e 2076 6965 775f 6974 656d  r v in view_item
+00006f10: 7320 6966 2022 636f 6e74 656e 7422 2069  s if "content" i
+00006f20: 6e20 7620 616e 6420 762e 6765 7428 2266  n v and v.get("f
+00006f30: 6965 6c64 5f74 7970 6522 2920 3d3d 2052  ield_type") == R
+00006f40: 6573 696c 6965 6e74 4669 656c 6454 7970  esilientFieldTyp
+00006f50: 6573 2e46 554e 4354 494f 4e5f 494e 5055  es.FUNCTION_INPU
+00006f60: 545d 0a20 2020 2020 2020 2066 5b22 696e  T].        f["in
+00006f70: 7075 7473 225d 203d 2067 6574 5f72 6573  puts"] = get_res
+00006f80: 5f6f 626a 2822 6669 656c 6473 222c 2022  _obj("fields", "
+00006f90: 7575 6964 222c 2022 4675 6e63 7469 6f6e  uuid", "Function
+00006fa0: 2049 6e70 7574 222c 2066 756e 6374 696f   Input", functio
+00006fb0: 6e5f 696e 7075 745f 7575 6964 732c 2065  n_input_uuids, e
+00006fc0: 7870 6f72 7429 0a0a 2020 2020 2020 2020  xport)..        
+00006fd0: 7265 7475 726e 5f64 6963 745b 2261 6c6c  return_dict["all
+00006fe0: 5f66 6965 6c64 7322 5d2e 6578 7465 6e64  _fields"].extend
+00006ff0: 285b 7522 5f5f 6675 6e63 7469 6f6e 2f7b  ([u"__function/{
+00007000: 307d 222e 666f 726d 6174 2866 6c64 2e67  0}".format(fld.g
+00007010: 6574 2822 6e61 6d65 2229 2920 666f 7220  et("name")) for 
+00007020: 666c 6420 696e 2066 2e67 6574 2822 696e  fld in f.get("in
+00007030: 7075 7473 2229 5d29 0a0a 2020 2020 2020  puts")])..      
+00007040: 2020 2320 4765 7420 4675 6e63 7469 6f6e    # Get Function
+00007050: 2773 204d 6573 7361 6765 2044 6573 7469  's Message Desti
+00007060: 6e61 7469 6f6e 206e 616d 650a 2020 2020  nation name.    
+00007070: 2020 2020 6d65 7373 6167 655f 6465 7374      message_dest
+00007080: 696e 6174 696f 6e73 2e61 7070 656e 6428  inations.append(
+00007090: 662e 6765 7428 2264 6573 7469 6e61 7469  f.get("destinati
+000070a0: 6f6e 5f68 616e 646c 6522 2c20 2222 2929  on_handle", ""))
+000070b0: 0a0a 2020 2020 2320 4765 7420 576f 726b  ..    # Get Work
+000070c0: 666c 6f77 730a 2020 2020 7265 7475 726e  flows.    return
+000070d0: 5f64 6963 745b 2277 6f72 6b66 6c6f 7773  _dict["workflows
+000070e0: 225d 203d 2067 6574 5f72 6573 5f6f 626a  "] = get_res_obj
+000070f0: 2822 776f 726b 666c 6f77 7322 2c20 5265  ("workflows", Re
+00007100: 7369 6c69 656e 744f 626a 4d61 702e 574f  silientObjMap.WO
+00007110: 524b 464c 4f57 532c 2022 576f 726b 666c  RKFLOWS, "Workfl
+00007120: 6f77 222c 2077 6f72 6b66 6c6f 7773 2c20  ow", workflows, 
+00007130: 6578 706f 7274 290a 0a20 2020 2069 6620  export)..    if 
+00007140: 6765 745f 7265 6c61 7465 645f 6f62 6a65  get_related_obje
+00007150: 6374 733a 0a20 2020 2020 2020 2023 2046  cts:.        # F
+00007160: 6f72 2077 6f72 6b66 6c6f 7773 2077 6520  or workflows we 
+00007170: 6174 7465 6d70 7420 746f 206c 6f63 6174  attempt to locat
+00007180: 6520 7265 6c61 7465 6420 6675 6e63 7469  e related functi
+00007190: 6f6e 730a 2020 2020 2020 2020 2320 4765  ons.        # Ge
+000071a0: 7420 4675 6e63 7469 6f6e 7320 696e 2057  t Functions in W
+000071b0: 6f72 6b66 6c6f 770a 2020 2020 2020 2020  orkflow.        
+000071c0: 666f 7220 776f 726b 666c 6f77 2069 6e20  for workflow in 
+000071d0: 7265 7475 726e 5f64 6963 745b 2277 6f72  return_dict["wor
+000071e0: 6b66 6c6f 7773 225d 3a0a 2020 2020 2020  kflows"]:.      
+000071f0: 2020 2020 2020 2320 5468 6973 2067 6574        # This get
+00007200: 7320 616c 6c20 7468 6520 4675 6e63 7469  s all the Functi
+00007210: 6f6e 7320 696e 2074 6865 2057 6f72 6b66  ons in the Workf
+00007220: 6c6f 7727 7320 584d 4c0a 2020 2020 2020  low's XML.      
+00007230: 2020 2020 2020 7766 5f66 756e 6374 696f        wf_functio
+00007240: 6e73 203d 2067 6574 5f77 6f72 6b66 6c6f  ns = get_workflo
+00007250: 775f 6675 6e63 7469 6f6e 7328 776f 726b  w_functions(work
+00007260: 666c 6f77 290a 0a20 2020 2020 2020 2020  flow)..         
+00007270: 2020 2023 2041 6464 2074 6865 2044 6973     # Add the Dis
+00007280: 706c 6179 204e 616d 6520 616e 6420 4e61  play Name and Na
+00007290: 6d65 2074 6f20 6561 6368 2077 665f 6675  me to each wf_fu
+000072a0: 6e63 7469 6f6e 0a20 2020 2020 2020 2020  nction.         
+000072b0: 2020 2066 6f72 2077 665f 666e 2069 6e20     for wf_fn in 
+000072c0: 7766 5f66 756e 6374 696f 6e73 3a0a 2020  wf_functions:.  
+000072d0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000072e0: 7220 666e 2069 6e20 7265 7475 726e 5f64  r fn in return_d
+000072f0: 6963 745b 2266 756e 6374 696f 6e73 225d  ict["functions"]
+00007300: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007310: 2020 2020 2020 6966 2077 665f 666e 2e67        if wf_fn.g
+00007320: 6574 2822 7575 6964 222c 2022 6122 2920  et("uuid", "a") 
+00007330: 3d3d 2066 6e2e 6765 7428 2275 7569 6422  == fn.get("uuid"
+00007340: 2c20 2262 2229 3a0a 2020 2020 2020 2020  , "b"):.        
+00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007360: 7766 5f66 6e5b 226e 616d 6522 5d20 3d20  wf_fn["name"] = 
+00007370: 666e 2e67 6574 2822 6e61 6d65 2229 0a20  fn.get("name"). 
+00007380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007390: 2020 2020 2020 2077 665f 666e 5b22 6469         wf_fn["di
+000073a0: 7370 6c61 795f 6e61 6d65 225d 203d 2066  splay_name"] = f
+000073b0: 6e2e 6765 7428 2264 6973 706c 6179 5f6e  n.get("display_n
+000073c0: 616d 6522 290a 2020 2020 2020 2020 2020  ame").          
+000073d0: 2020 2020 2020 2020 2020 2020 2020 7766                wf
+000073e0: 5f66 6e5b 226d 6573 7361 6765 5f64 6573  _fn["message_des
+000073f0: 7469 6e61 7469 6f6e 225d 203d 2066 6e2e  tination"] = fn.
+00007400: 6765 7428 2264 6573 7469 6e61 7469 6f6e  get("destination
+00007410: 5f68 616e 646c 6522 2c20 2222 290a 2020  _handle", "").  
+00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007430: 2020 2020 2020 6272 6561 6b0a 0a20 2020        break..   
+00007440: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
+00007450: 775b 2277 665f 6675 6e63 7469 6f6e 7322  w["wf_functions"
+00007460: 5d20 3d20 7766 5f66 756e 6374 696f 6e73  ] = wf_functions
+00007470: 0a0a 2020 2020 2320 4765 7420 4d65 7373  ..    # Get Mess
+00007480: 6167 6520 4465 7374 696e 6174 696f 6e73  age Destinations
+00007490: 0a20 2020 2072 6574 7572 6e5f 6469 6374  .    return_dict
+000074a0: 5b22 6d65 7373 6167 655f 6465 7374 696e  ["message_destin
+000074b0: 6174 696f 6e73 225d 203d 2067 6574 5f72  ations"] = get_r
+000074c0: 6573 5f6f 626a 2822 6d65 7373 6167 655f  es_obj("message_
+000074d0: 6465 7374 696e 6174 696f 6e73 222c 2052  destinations", R
+000074e0: 6573 696c 6965 6e74 4f62 6a4d 6170 2e4d  esilientObjMap.M
+000074f0: 4553 5341 4745 5f44 4553 5449 4e41 5449  ESSAGE_DESTINATI
+00007500: 4f4e 532c 2022 4d65 7373 6167 6520 4465  ONS, "Message De
+00007510: 7374 696e 6174 696f 6e22 2c20 6d65 7373  stination", mess
+00007520: 6167 655f 6465 7374 696e 6174 696f 6e73  age_destinations
+00007530: 2c20 6578 706f 7274 290a 0a20 2020 2023  , export)..    #
+00007540: 2047 6574 2049 6e63 6964 656e 7420 4669   Get Incident Fi
+00007550: 656c 6473 2028 4375 7374 6f6d 2061 6e64  elds (Custom and
+00007560: 2049 6e74 6572 6e61 6c29 0a20 2020 2072   Internal).    r
+00007570: 6574 7572 6e5f 6469 6374 5b22 6669 656c  eturn_dict["fiel
+00007580: 6473 225d 203d 2067 6574 5f72 6573 5f6f  ds"] = get_res_o
+00007590: 626a 2822 6669 656c 6473 222c 2052 6573  bj("fields", Res
+000075a0: 696c 6965 6e74 4f62 6a4d 6170 2e46 4945  ilientObjMap.FIE
+000075b0: 4c44 532c 2022 4669 656c 6422 2c20 6669  LDS, "Field", fi
+000075c0: 656c 6473 2c20 6578 706f 7274 2c0a 2020  elds, export,.  
+000075d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075f0: 2020 2020 2020 636f 6e64 6974 696f 6e3d        condition=
+00007600: 6c61 6d62 6461 206f 3a20 5472 7565 2069  lambda o: True i
+00007610: 6620 6f2e 6765 7428 2274 7970 655f 6964  f o.get("type_id
+00007620: 2229 203d 3d20 5265 7369 6c69 656e 7454  ") == ResilientT
+00007630: 7970 6549 6473 2e49 4e43 4944 454e 5420  ypeIds.INCIDENT 
+00007640: 656c 7365 2046 616c 7365 290a 0a20 2020  else False)..   
+00007650: 2072 6574 7572 6e5f 6469 6374 5b22 616c   return_dict["al
+00007660: 6c5f 6669 656c 6473 225d 2e65 7874 656e  l_fields"].exten
+00007670: 6428 5b75 2269 6e63 6964 656e 742f 7b30  d([u"incident/{0
+00007680: 7d22 2e66 6f72 6d61 7428 666c 642e 6765  }".format(fld.ge
+00007690: 7428 226e 616d 6522 2929 2066 6f72 2066  t("name")) for f
+000076a0: 6c64 2069 6e20 7265 7475 726e 5f64 6963  ld in return_dic
+000076b0: 742e 6765 7428 2266 6965 6c64 7322 295d  t.get("fields")]
+000076c0: 290a 0a20 2020 2023 2047 6574 2043 7573  )..    # Get Cus
+000076d0: 746f 6d20 4172 7469 6661 6374 2054 7970  tom Artifact Typ
+000076e0: 6573 0a20 2020 2072 6574 7572 6e5f 6469  es.    return_di
+000076f0: 6374 5b22 6172 7469 6661 6374 5f74 7970  ct["artifact_typ
+00007700: 6573 225d 203d 2067 6574 5f72 6573 5f6f  es"] = get_res_o
+00007710: 626a 2822 696e 6369 6465 6e74 5f61 7274  bj("incident_art
+00007720: 6966 6163 745f 7479 7065 7322 2c20 5265  ifact_types", Re
+00007730: 7369 6c69 656e 744f 626a 4d61 702e 494e  silientObjMap.IN
+00007740: 4349 4445 4e54 5f41 5254 4946 4143 545f  CIDENT_ARTIFACT_
+00007750: 5459 5045 532c 2022 4375 7374 6f6d 2041  TYPES, "Custom A
+00007760: 7274 6966 6163 7422 2c20 6172 7469 6661  rtifact", artifa
+00007770: 6374 5f74 7970 6573 2c20 6578 706f 7274  ct_types, export
+00007780: 290a 0a20 2020 2023 2047 6574 2049 6e63  )..    # Get Inc
+00007790: 6964 656e 7420 5479 7065 730a 2020 2020  ident Types.    
+000077a0: 7265 7475 726e 5f64 6963 745b 2269 6e63  return_dict["inc
+000077b0: 6964 656e 745f 7479 7065 7322 5d20 3d20  ident_types"] = 
+000077c0: 6765 745f 7265 735f 6f62 6a28 2269 6e63  get_res_obj("inc
+000077d0: 6964 656e 745f 7479 7065 7322 2c20 5265  ident_types", Re
+000077e0: 7369 6c69 656e 744f 626a 4d61 702e 494e  silientObjMap.IN
+000077f0: 4349 4445 4e54 5f54 5950 4553 2c20 2243  CIDENT_TYPES, "C
+00007800: 7573 746f 6d20 496e 6369 6465 6e74 2054  ustom Incident T
+00007810: 7970 6522 2c20 696e 6369 6465 6e74 5f74  ype", incident_t
+00007820: 7970 6573 2c20 6578 706f 7274 290a 0a20  ypes, export).. 
+00007830: 2020 2023 2047 6574 2044 6174 6120 5461     # Get Data Ta
+00007840: 626c 6573 0a20 2020 2072 6574 7572 6e5f  bles.    return_
+00007850: 6469 6374 5b22 6461 7461 7461 626c 6573  dict["datatables
+00007860: 225d 203d 2067 6574 5f72 6573 5f6f 626a  "] = get_res_obj
+00007870: 2822 7479 7065 7322 2c20 5265 7369 6c69  ("types", Resili
+00007880: 656e 744f 626a 4d61 702e 4441 5441 5441  entObjMap.DATATA
+00007890: 424c 4553 2c20 2244 6174 6174 6162 6c65  BLES, "Datatable
+000078a0: 222c 2064 6174 6174 6162 6c65 732c 2065  ", datatables, e
+000078b0: 7870 6f72 742c 0a20 2020 2020 2020 2020  xport,.         
+000078c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078e0: 2020 2063 6f6e 6469 7469 6f6e 3d6c 616d     condition=lam
+000078f0: 6264 6120 6f3a 2054 7275 6520 6966 206f  bda o: True if o
+00007900: 2e67 6574 2822 7479 7065 5f69 6422 2920  .get("type_id") 
+00007910: 3d3d 2052 6573 696c 6965 6e74 5479 7065  == ResilientType
+00007920: 4964 732e 4441 5441 5441 424c 4520 656c  Ids.DATATABLE el
+00007930: 7365 2046 616c 7365 290a 0a20 2020 2023  se False)..    #
+00007940: 2047 6574 2043 7573 746f 6d20 5461 736b   Get Custom Task
+00007950: 730a 2020 2020 7265 7475 726e 5f64 6963  s.    return_dic
+00007960: 745b 2274 6173 6b73 225d 203d 2067 6574  t["tasks"] = get
+00007970: 5f72 6573 5f6f 626a 2822 6175 746f 6d61  _res_obj("automa
+00007980: 7469 635f 7461 736b 7322 2c20 5265 7369  tic_tasks", Resi
+00007990: 6c69 656e 744f 626a 4d61 702e 5441 534b  lientObjMap.TASK
+000079a0: 532c 2022 4375 7374 6f6d 2054 6173 6b22  S, "Custom Task"
+000079b0: 2c20 7461 736b 732c 2065 7870 6f72 7429  , tasks, export)
+000079c0: 0a0a 2020 2020 2320 4765 7420 7265 6c61  ..    # Get rela
+000079d0: 7465 6420 5068 6173 6573 2066 6f72 2054  ted Phases for T
+000079e0: 6173 6b73 0a20 2020 2070 6861 7365 5f69  asks.    phase_i
+000079f0: 6473 203d 205b 742e 6765 7428 2270 6861  ds = [t.get("pha
+00007a00: 7365 5f69 6422 2920 666f 7220 7420 696e  se_id") for t in
+00007a10: 2072 6574 7572 6e5f 6469 6374 2e67 6574   return_dict.get
+00007a20: 2822 7461 736b 7322 295d 0a20 2020 2072  ("tasks")].    r
+00007a30: 6574 7572 6e5f 6469 6374 5b22 7068 6173  eturn_dict["phas
+00007a40: 6573 225d 203d 2067 6574 5f72 6573 5f6f  es"] = get_res_o
+00007a50: 626a 2822 7068 6173 6573 222c 2052 6573  bj("phases", Res
+00007a60: 696c 6965 6e74 4f62 6a4d 6170 2e50 4841  ilientObjMap.PHA
+00007a70: 5345 532c 2022 5068 6173 6522 2c20 7068  SES, "Phase", ph
+00007a80: 6173 655f 6964 732c 2065 7870 6f72 7429  ase_ids, export)
+00007a90: 0a0a 2020 2020 2320 4765 7420 5363 7269  ..    # Get Scri
+00007aa0: 7074 730a 2020 2020 7265 7475 726e 5f64  pts.    return_d
+00007ab0: 6963 745b 2273 6372 6970 7473 225d 203d  ict["scripts"] =
+00007ac0: 2067 6574 5f72 6573 5f6f 626a 2822 7363   get_res_obj("sc
+00007ad0: 7269 7074 7322 2c20 5265 7369 6c69 656e  ripts", Resilien
+00007ae0: 744f 626a 4d61 702e 5343 5249 5054 532c  tObjMap.SCRIPTS,
+00007af0: 2022 5363 7269 7074 222c 2073 6372 6970   "Script", scrip
+00007b00: 7473 2c20 6578 706f 7274 290a 0a20 2020  ts, export)..   
+00007b10: 2023 2047 6574 2041 7070 730a 2020 2020   # Get Apps.    
+00007b20: 7265 7475 726e 5f64 6963 745b 2261 7070  return_dict["app
+00007b30: 7322 5d20 3d20 6765 745f 7265 735f 6f62  s"] = get_res_ob
+00007b40: 6a28 2261 7070 7322 2c20 5265 7369 6c69  j("apps", Resili
+00007b50: 656e 744f 626a 4d61 702e 4150 5053 2c20  entObjMap.APPS, 
+00007b60: 2241 7070 7322 2c20 6170 7073 2c20 6578  "Apps", apps, ex
+00007b70: 706f 7274 290a 0a20 2020 2023 2047 6574  port)..    # Get
+00007b80: 2050 6c61 7962 6f6f 6b73 0a20 2020 2069   Playbooks.    i
+00007b90: 6620 706c 6179 626f 6f6b 7320 616e 6420  f playbooks and 
+00007ba0: 636f 6e73 7461 6e74 732e 4355 5252 454e  constants.CURREN
+00007bb0: 545f 534f 4152 5f53 4552 5645 525f 5645  T_SOAR_SERVER_VE
+00007bc0: 5253 494f 4e20 616e 6420 636f 6e73 7461  RSION and consta
+00007bd0: 6e74 732e 4355 5252 454e 545f 534f 4152  nts.CURRENT_SOAR
+00007be0: 5f53 4552 5645 525f 5645 5253 494f 4e20  _SERVER_VERSION 
+00007bf0: 3c20 636f 6e73 7461 6e74 732e 4d49 4e5f  < constants.MIN_
+00007c00: 534f 4152 5f53 4552 5645 525f 5645 5253  SOAR_SERVER_VERS
+00007c10: 494f 4e5f 504c 4159 424f 4f4b 533a 0a20  ION_PLAYBOOKS:. 
+00007c20: 2020 2020 2020 2072 6169 7365 2053 444b         raise SDK
+00007c30: 4578 6365 7074 696f 6e28 636f 6e73 7461  Exception(consta
+00007c40: 6e74 732e 4552 524f 525f 504c 4159 424f  nts.ERROR_PLAYBO
+00007c50: 4f4b 5f53 5550 504f 5254 290a 2020 2020  OK_SUPPORT).    
+00007c60: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
+00007c70: 7475 726e 5f64 6963 745b 2270 6c61 7962  turn_dict["playb
+00007c80: 6f6f 6b73 225d 203d 2067 6574 5f72 6573  ooks"] = get_res
+00007c90: 5f6f 626a 2822 706c 6179 626f 6f6b 7322  _obj("playbooks"
+00007ca0: 2c20 5265 7369 6c69 656e 744f 626a 4d61  , ResilientObjMa
+00007cb0: 702e 504c 4159 424f 4f4b 532c 2022 506c  p.PLAYBOOKS, "Pl
+00007cc0: 6179 626f 6f6b 222c 2070 6c61 7962 6f6f  aybook", playboo
+00007cd0: 6b73 2c20 6578 706f 7274 290a 0a20 2020  ks, export)..   
+00007ce0: 2020 2020 2069 6620 6765 745f 7265 6c61       if get_rela
+00007cf0: 7465 645f 6f62 6a65 6374 733a 0a20 2020  ted_objects:.   
+00007d00: 2020 2020 2020 2020 2023 2046 6f72 2050           # For P
+00007d10: 6c61 7962 6f6f 6b73 2077 6520 6174 7465  laybooks we atte
+00007d20: 6d70 7420 746f 206c 6f63 6174 6520 7265  mpt to locate re
+00007d30: 6c61 7465 6420 6675 6e63 7469 6f6e 7320  lated functions 
+00007d40: 616e 6420 7363 7269 7074 730a 2020 2020  and scripts.    
+00007d50: 2020 2020 2020 2020 2320 4765 7420 4675          # Get Fu
+00007d60: 6e63 7469 6f6e 7320 696e 2050 6c61 7962  nctions in Playb
+00007d70: 6f6f 6b73 0a20 2020 2020 2020 2020 2020  ooks.           
+00007d80: 2066 6f72 2070 6c61 7962 6f6f 6b20 696e   for playbook in
+00007d90: 2072 6574 7572 6e5f 6469 6374 2e67 6574   return_dict.get
+00007da0: 2822 706c 6179 626f 6f6b 7322 2920 6f72  ("playbooks") or
+00007db0: 205b 5d3a 0a20 2020 2020 2020 2020 2020   []:.           
+00007dc0: 2020 2020 2023 2054 6869 7320 6765 7473       # This gets
+00007dd0: 2061 6c6c 2074 6865 2066 756e 6374 696f   all the functio
+00007de0: 6e73 2061 6e64 2073 6372 6970 7473 2069  ns and scripts i
+00007df0: 6e20 7468 6520 506c 6179 626f 6f6b 7327  n the Playbooks'
+00007e00: 7320 584d 4c0a 2020 2020 2020 2020 2020  s XML.          
+00007e10: 2020 2020 2020 7062 5f6f 626a 6563 7473        pb_objects
+00007e20: 203d 2067 6574 5f70 6c61 7962 6f6f 6b5f   = get_playbook_
+00007e30: 6f62 6a65 6374 7328 706c 6179 626f 6f6b  objects(playbook
+00007e40: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00007e50: 2020 2023 2041 6464 2074 6865 2044 6973     # Add the Dis
+00007e60: 706c 6179 204e 616d 6520 616e 6420 4e61  play Name and Na
+00007e70: 6d65 2074 6f20 6561 6368 2077 665f 6675  me to each wf_fu
+00007e80: 6e63 7469 6f6e 0a20 2020 2020 2020 2020  nction.         
+00007e90: 2020 2020 2020 2066 6f72 2070 625f 666e         for pb_fn
+00007ea0: 2069 6e20 7062 5f6f 626a 6563 7473 2e67   in pb_objects.g
+00007eb0: 6574 2822 6675 6e63 7469 6f6e 7322 2c20  et("functions", 
+00007ec0: 5b5d 293a 0a20 2020 2020 2020 2020 2020  []):.           
+00007ed0: 2020 2020 2020 2020 2066 6f72 2066 6e20           for fn 
+00007ee0: 696e 2072 6574 7572 6e5f 6469 6374 5b22  in return_dict["
+00007ef0: 6675 6e63 7469 6f6e 7322 5d3a 0a20 2020  functions"]:.   
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f10: 2020 2020 2069 6620 7062 5f66 6e2e 6765       if pb_fn.ge
+00007f20: 7428 2275 7569 6422 2c20 2275 7569 645f  t("uuid", "uuid_
+00007f30: 6e6f 745f 666f 756e 645f 7062 2229 203d  not_found_pb") =
+00007f40: 3d20 666e 2e67 6574 2822 7575 6964 222c  = fn.get("uuid",
+00007f50: 2022 7575 6964 5f6e 6f74 5f66 6f75 6e64   "uuid_not_found
+00007f60: 5f66 6e22 293a 0a20 2020 2020 2020 2020  _fn"):.         
+00007f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f80: 2020 2070 625f 666e 5b22 6e61 6d65 225d     pb_fn["name"]
+00007f90: 203d 2066 6e2e 6765 7428 226e 616d 6522   = fn.get("name"
+00007fa0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007fb0: 2020 2020 2020 2020 2020 2020 2020 7062                pb
+00007fc0: 5f66 6e5b 2264 6973 706c 6179 5f6e 616d  _fn["display_nam
+00007fd0: 6522 5d20 3d20 666e 2e67 6574 2822 6469  e"] = fn.get("di
+00007fe0: 7370 6c61 795f 6e61 6d65 2229 0a20 2020  splay_name").   
+00007ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008000: 2020 2020 2020 2020 2070 625f 666e 5b22           pb_fn["
+00008010: 6d65 7373 6167 655f 6465 7374 696e 6174  message_destinat
+00008020: 696f 6e22 5d20 3d20 666e 2e67 6574 2822  ion"] = fn.get("
+00008030: 6465 7374 696e 6174 696f 6e5f 6861 6e64  destination_hand
+00008040: 6c65 222c 2022 2229 0a20 2020 2020 2020  le", "").       
+00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008060: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
+00008070: 2020 2020 2020 2020 2020 2020 2320 4966              # If
+00008080: 2061 2070 6c61 7962 6f6f 6b20 7363 7269   a playbook scri
+00008090: 7074 2069 7320 6c6f 6361 6c2c 2069 7473  pt is local, its
+000080a0: 2069 6e66 6f72 6d61 7469 6f6e 2063 616e   information can
+000080b0: 2062 6520 6469 7265 6374 6c79 2065 7874   be directly ext
+000080c0: 7261 6374 6564 2066 726f 6d20 7468 6520  racted from the 
+000080d0: 706c 6179 626f 6f6b 2c0a 2020 2020 2020  playbook,.      
+000080e0: 2020 2020 2020 2020 2020 2320 6966 206e            # if n
+000080f0: 6f74 2c20 7468 6520 7363 7269 7074 2773  ot, the script's
+00008100: 2069 6e66 6f72 6d61 7469 6f6e 2068 6173   information has
+00008110: 2074 6f20 6265 2065 7874 7261 6374 6564   to be extracted
+00008120: 2066 726f 6d20 7468 6520 676c 6f62 616c   from the global
+00008130: 2073 6372 6970 7473 0a20 2020 2020 2020   scripts.       
+00008140: 2020 2020 2020 2020 2066 6f72 2070 625f           for pb_
+00008150: 7363 2069 6e20 7062 5f6f 626a 6563 7473  sc in pb_objects
+00008160: 2e67 6574 2822 7363 7269 7074 7322 2c20  .get("scripts", 
+00008170: 5b5d 293a 0a20 2020 2020 2020 2020 2020  []):.           
+00008180: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
+00008190: 6520 7363 7269 7074 2069 7320 6120 6c6f  e script is a lo
+000081a0: 6361 6c20 7363 7269 7074 2c20 7468 656e  cal script, then
+000081b0: 2077 6520 6e65 6564 2074 6f20 6669 6e64   we need to find
+000081c0: 2074 6865 2073 6372 6970 7420 696e 2074   the script in t
+000081d0: 6865 2050 6c61 7962 6f6f 6b0a 2020 2020  he Playbook.    
+000081e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081f0: 666f 756e 645f 7363 7269 7074 203d 2067  found_script = g
+00008200: 6574 5f73 6372 6970 745f 696e 666f 2870  et_script_info(p
+00008210: 625f 7363 2c20 706c 6179 626f 6f6b 2e67  b_sc, playbook.g
+00008220: 6574 2822 6c6f 6361 6c5f 7363 7269 7074  et("local_script
+00008230: 7322 292c 2053 4352 4950 545f 5459 5045  s"), SCRIPT_TYPE
+00008240: 5f4d 4150 2e67 6574 2822 6c6f 6361 6c22  _MAP.get("local"
+00008250: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+00008260: 2020 2020 2020 2020 2320 4966 2073 6372          # If scr
+00008270: 6970 7420 6e6f 7420 666f 756e 6420 696e  ipt not found in
+00008280: 2070 6c61 7962 6f6f 6b2c 2073 6561 7263   playbook, searc
+00008290: 6869 6e67 2047 6c6f 6261 6c20 5363 7269  hing Global Scri
+000082a0: 7074 730a 2020 2020 2020 2020 2020 2020  pts.            
+000082b0: 2020 2020 2020 2020 666f 756e 645f 7363          found_sc
+000082c0: 7269 7074 203d 2067 6574 5f73 6372 6970  ript = get_scrip
+000082d0: 745f 696e 666f 2870 625f 7363 2c20 7265  t_info(pb_sc, re
+000082e0: 7475 726e 5f64 6963 745b 2273 6372 6970  turn_dict["scrip
+000082f0: 7473 225d 2c20 5343 5249 5054 5f54 5950  ts"], SCRIPT_TYP
+00008300: 455f 4d41 502e 6765 7428 2267 6c6f 6261  E_MAP.get("globa
+00008310: 6c22 2929 2069 6620 6e6f 7420 666f 756e  l")) if not foun
+00008320: 645f 7363 7269 7074 2065 6c73 6520 5472  d_script else Tr
+00008330: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
+00008340: 2020 2020 2020 2020 2320 4966 2074 6865          # If the
+00008350: 2073 6372 6970 7420 6973 206e 6f74 2066   script is not f
+00008360: 6f75 6e64 2069 6e20 7468 6520 506c 6179  ound in the Play
+00008370: 626f 6f6b 206f 7220 476c 6f62 616c 2053  book or Global S
+00008380: 6372 6970 7473 2c20 7468 656e 2069 7473  cripts, then its
+00008390: 2055 5549 4420 6973 2075 7365 6420 746f   UUID is used to
+000083a0: 2066 696e 6420 7468 6520 7363 7269 7074   find the script
+000083b0: 2066 6f72 6d20 7468 6520 6f72 6720 6578   form the org ex
+000083c0: 706f 7274 0a20 2020 2020 2020 2020 2020  port.           
+000083d0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000083e0: 666f 756e 645f 7363 7269 7074 3a0a 2020  found_script:.  
+000083f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008400: 2020 2020 2020 5f75 6e66 6f75 6e64 5f73        _unfound_s
+00008410: 6372 6970 7473 203d 2067 6574 5f72 6573  cripts = get_res
+00008420: 5f6f 626a 2822 7363 7269 7074 7322 2c20  _obj("scripts", 
+00008430: 2275 7569 6422 2c20 2253 6372 6970 7422  "uuid", "Script"
+00008440: 2c20 5b70 625f 7363 2e67 6574 2822 7575  , [pb_sc.get("uu
+00008450: 6964 2229 5d2c 2065 7870 6f72 7429 0a20  id")], export). 
+00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008470: 2020 2020 2020 2066 6f72 2073 6372 6970         for scrip
+00008480: 7420 696e 205f 756e 666f 756e 645f 7363  t in _unfound_sc
+00008490: 7269 7074 733a 0a20 2020 2020 2020 2020  ripts:.         
+000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084b0: 2020 2023 2052 656e 616d 696e 6720 7468     # Renaming th
+000084c0: 6520 785f 6170 695f 6e61 6d65 2074 6f20  e x_api_name to 
+000084d0: 6e61 6d65 2e20 5369 6e63 6520 7468 6520  name. Since the 
+000084e0: 7363 7269 7074 2077 6173 2066 6574 6368  script was fetch
+000084f0: 6564 2077 6974 6820 5555 4944 2c20 7468  ed with UUID, th
+00008500: 6520 785f 6170 695f 6e61 6d65 2069 7320  e x_api_name is 
+00008510: 7468 6520 5555 4944 0a20 2020 2020 2020  the UUID.       
+00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008530: 2020 2020 2073 6372 6970 745b 2278 5f61       script["x_a
+00008540: 7069 5f6e 616d 6522 5d20 3d20 7363 7269  pi_name"] = scri
+00008550: 7074 5b22 6e61 6d65 225d 0a20 2020 2020  pt["name"].     
+00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008570: 2020 2066 6f75 6e64 5f73 6372 6970 7420     found_script 
+00008580: 3d20 6765 745f 7363 7269 7074 5f69 6e66  = get_script_inf
+00008590: 6f28 7062 5f73 632c 205f 756e 666f 756e  o(pb_sc, _unfoun
+000085a0: 645f 7363 7269 7074 732c 2053 4352 4950  d_scripts, SCRIP
+000085b0: 545f 5459 5045 5f4d 4150 2e67 6574 2822  T_TYPE_MAP.get("
+000085c0: 676c 6f62 616c 2229 290a 2020 2020 2020  global")).      
+000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085e0: 2020 2320 4164 6469 6e67 2073 6372 6970    # Adding scrip
+000085f0: 7420 746f 2072 6574 7572 6e5f 6469 6374  t to return_dict
+00008600: 2e20 5468 6973 2069 7320 746f 206d 616b  . This is to mak
+00008610: 6520 7375 7265 2074 6861 7420 6974 7320  e sure that its 
+00008620: 696e 636c 7564 6564 2069 6e20 7468 6520  included in the 
+00008630: 6578 706f 7274 2e72 6573 2061 6e64 2063  export.res and c
+00008640: 7573 746f 6d69 7a65 2e70 790a 2020 2020  ustomize.py.    
+00008650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008660: 2020 2020 7265 7475 726e 5f64 6963 745b      return_dict[
+00008670: 2273 6372 6970 7473 225d 2e65 7874 656e  "scripts"].exten
+00008680: 6428 5f75 6e66 6f75 6e64 5f73 6372 6970  d(_unfound_scrip
+00008690: 7473 290a 0a20 2020 2020 2020 2020 2020  ts)..           
+000086a0: 2020 2020 2023 2061 6464 206e 616d 6520       # add name 
+000086b0: 746f 2065 6163 6820 7375 6220 706c 6179  to each sub play
+000086c0: 626f 6f6b 2069 6e70 7574 0a20 2020 2020  book input.     
+000086d0: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
+000086e0: 625f 7375 625f 7062 2069 6e20 7062 5f6f  b_sub_pb in pb_o
+000086f0: 626a 6563 7473 2e67 6574 2822 7375 625f  bjects.get("sub_
+00008700: 7062 7322 2c20 5b5d 293a 0a20 2020 2020  pbs", []):.     
+00008710: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00008720: 6570 6c61 6365 5f75 7569 6473 5f69 6e5f  eplace_uuids_in_
+00008730: 7375 6270 6c61 7962 6f6f 6b5f 6461 7461  subplaybook_data
+00008740: 2870 625f 7375 625f 7062 2c20 6578 706f  (pb_sub_pb, expo
+00008750: 7274 290a 0a20 2020 2020 2020 2020 2020  rt)..           
+00008760: 2020 2020 2061 6374 6976 6174 696f 6e5f       activation_
+00008770: 7479 7065 203d 2070 6c61 7962 6f6f 6b2e  type = playbook.
+00008780: 6765 7428 2261 6374 6976 6174 696f 6e5f  get("activation_
+00008790: 7479 7065 222c 2022 2229 0a20 2020 2020  type", "").     
+000087a0: 2020 2020 2020 2020 2020 2069 6620 706c             if pl
+000087b0: 6179 626f 6f6b 2e67 6574 2822 7479 7065  aybook.get("type
+000087c0: 2229 203d 3d20 2273 7562 706c 6179 626f  ") == "subplaybo
+000087d0: 6f6b 223a 0a20 2020 2020 2020 2020 2020  ok":.           
+000087e0: 2020 2020 2020 2020 2070 6c61 7962 6f6f           playboo
+000087f0: 6b5b 2261 6374 6976 6174 696f 6e5f 7479  k["activation_ty
+00008800: 7065 225d 203d 2022 5375 622d 706c 6179  pe"] = "Sub-play
+00008810: 626f 6f6b 220a 2020 2020 2020 2020 2020  book".          
+00008820: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00008830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008840: 706c 6179 626f 6f6b 5b22 6163 7469 7661  playbook["activa
+00008850: 7469 6f6e 5f74 7970 6522 5d20 3d20 6163  tion_type"] = ac
+00008860: 7469 7661 7469 6f6e 5f74 7970 652e 6361  tivation_type.ca
+00008870: 7069 7461 6c69 7a65 2829 0a0a 2020 2020  pitalize()..    
+00008880: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+00008890: 6374 6976 6174 696f 6e5f 7479 7065 2e6c  ctivation_type.l
+000088a0: 6f77 6572 2829 203d 3d20 226d 616e 7561  ower() == "manua
+000088b0: 6c22 3a0a 2020 2020 2020 2020 2020 2020  l":.            
+000088c0: 2020 2020 2020 2020 6163 7469 7661 7469          activati
+000088d0: 6f6e 5f63 6f6e 6469 7469 6f6e 7320 3d20  on_conditions = 
+000088e0: 706c 6179 626f 6f6b 2e67 6574 2822 6d61  playbook.get("ma
+000088f0: 6e75 616c 5f73 6574 7469 6e67 7322 2c20  nual_settings", 
+00008900: 7b7d 292e 6765 7428 2261 6374 6976 6174  {}).get("activat
+00008910: 696f 6e5f 636f 6e64 6974 696f 6e73 222c  ion_conditions",
+00008920: 207b 7d29 0a20 2020 2020 2020 2020 2020   {}).           
+00008930: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00008940: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00008950: 6374 6976 6174 696f 6e5f 636f 6e64 6974  ctivation_condit
+00008960: 696f 6e73 203d 2070 6c61 7962 6f6f 6b2e  ions = playbook.
+00008970: 6765 7428 2261 6374 6976 6174 696f 6e5f  get("activation_
+00008980: 6465 7461 696c 7322 2c20 7b7d 292e 6765  details", {}).ge
+00008990: 7428 2261 6374 6976 6174 696f 6e5f 636f  t("activation_co
+000089a0: 6e64 6974 696f 6e73 222c 207b 7d29 0a20  nditions", {}). 
+000089b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000089c0: 6c61 7962 6f6f 6b5b 2263 6f6e 6469 7469  laybook["conditi
+000089d0: 6f6e 7322 5d20 3d20 7374 725f 7265 7072  ons"] = str_repr
+000089e0: 5f61 6374 6976 6174 696f 6e5f 636f 6e64  _activation_cond
+000089f0: 6974 696f 6e73 2861 6374 6976 6174 696f  itions(activatio
+00008a00: 6e5f 636f 6e64 6974 696f 6e73 2920 6f72  n_conditions) or
+00008a10: 2022 2d22 0a20 2020 2020 2020 2020 2020   "-".           
+00008a20: 2020 2020 2070 6c61 7962 6f6f 6b5b 2270       playbook["p
+00008a30: 625f 6675 6e63 7469 6f6e 7322 5d20 3d20  b_functions"] = 
+00008a40: 7062 5f6f 626a 6563 7473 2e67 6574 2822  pb_objects.get("
+00008a50: 6675 6e63 7469 6f6e 7322 290a 2020 2020  functions").    
+00008a60: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00008a70: 626f 6f6b 5b22 7062 5f73 6372 6970 7473  book["pb_scripts
+00008a80: 225d 2020 203d 2070 625f 6f62 6a65 6374  "]   = pb_object
+00008a90: 732e 6765 7428 2273 6372 6970 7473 2229  s.get("scripts")
+00008aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008ab0: 2070 6c61 7962 6f6f 6b5b 2270 625f 7375   playbook["pb_su
+00008ac0: 625f 7062 7322 5d20 2020 3d20 7062 5f6f  b_pbs"]   = pb_o
+00008ad0: 626a 6563 7473 2e67 6574 2822 7375 625f  bjects.get("sub_
+00008ae0: 7062 7322 290a 0a20 2020 2072 6574 7572  pbs")..    retur
+00008af0: 6e20 7265 7475 726e 5f64 6963 740a 0a0a  n return_dict...
+00008b00: 6465 6620 6d69 6e69 6679 5f65 7870 6f72  def minify_expor
+00008b10: 7428 6578 706f 7274 2c0a 2020 2020 2020  t(export,.      
+00008b20: 2020 2020 2020 2020 2020 2020 6b65 7973              keys
+00008b30: 5f74 6f5f 6b65 6570 3d5b 5d2c 0a20 2020  _to_keep=[],.   
+00008b40: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00008b50: 6573 7361 6765 5f64 6573 7469 6e61 7469  essage_destinati
+00008b60: 6f6e 733d 5b5d 2c0a 2020 2020 2020 2020  ons=[],.        
+00008b70: 2020 2020 2020 2020 2020 6675 6e63 7469            functi
+00008b80: 6f6e 733d 5b5d 2c0a 2020 2020 2020 2020  ons=[],.        
+00008b90: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
+00008ba0: 6f77 733d 5b5d 2c0a 2020 2020 2020 2020  ows=[],.        
+00008bb0: 2020 2020 2020 2020 2020 7275 6c65 733d            rules=
+00008bc0: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+00008bd0: 2020 2020 2020 6669 656c 6473 3d5b 5d2c        fields=[],
+00008be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008bf0: 2020 2061 7274 6966 6163 745f 7479 7065     artifact_type
+00008c00: 733d 5b5d 2c0a 2020 2020 2020 2020 2020  s=[],.          
+00008c10: 2020 2020 2020 2020 6461 7461 7461 626c          datatabl
+00008c20: 6573 3d5b 5d2c 0a20 2020 2020 2020 2020  es=[],.         
+00008c30: 2020 2020 2020 2020 2074 6173 6b73 3d5b           tasks=[
+00008c40: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00008c50: 2020 2020 2070 6861 7365 733d 5b5d 2c0a       phases=[],.
+00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c70: 2020 7363 7269 7074 733d 5b5d 2c0a 2020    scripts=[],.  
+00008c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c90: 696e 6369 6465 6e74 5f74 7970 6573 3d5b  incident_types=[
+00008ca0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00008cb0: 2020 2020 2070 6c61 7962 6f6f 6b73 3d5b       playbooks=[
+00008cc0: 5d29 3a0a 2020 2020 2222 220a 2020 2020  ]):.    """.    
+00008cd0: 5265 7475 726e 2061 2027 6d69 6e69 6669  Return a 'minifi
+00008ce0: 6564 2720 7665 7273 696f 6e20 6f66 2074  ed' version of t
+00008cf0: 6865 2065 7870 6f72 742e 0a20 2020 2041  he export..    A
+00008d00: 6c6c 2070 6172 616d 6574 6572 7320 6172  ll parameters ar
+00008d10: 6520 6120 6c69 7374 206f 6620 6170 695f  e a list of api_
+00008d20: 6e61 6d65 7320 6f66 206f 626a 6563 7473  names of objects
+00008d30: 2074 6f20 696e 636c 7564 6520 696e 2074   to include in t
+00008d40: 6865 2065 7870 6f72 742e 0a20 2020 2041  he export..    A
+00008d50: 6e79 7468 696e 6720 6e6f 7420 6d65 6e74  nything not ment
+00008d60: 696f 6e65 6420 696e 2070 6173 7365 6420  ioned in passed 
+00008d70: 4c69 7374 7320 6172 6520 7365 7420 746f  Lists are set to
+00008d80: 2065 6d70 7479 206f 7220 4e6f 6e65 2e0a   empty or None..
+00008d90: 0a20 2020 203a 7061 7261 6d20 6578 706f  .    :param expo
+00008da0: 7274 3a20 5468 6520 7265 7375 6c74 206f  rt: The result o
+00008db0: 6620 6361 6c6c 696e 6720 6765 745f 6c61  f calling get_la
+00008dc0: 7465 7374 5f6f 7267 5f65 7870 6f72 7428  test_org_export(
+00008dd0: 290a 2020 2020 3a74 7970 6520 6578 706f  ).    :type expo
+00008de0: 7274 3a20 4469 6374 0a20 2020 203a 7061  rt: Dict.    :pa
+00008df0: 7261 6d20 6b65 7973 5f74 6f5f 6b65 6570  ram keys_to_keep
+00008e00: 3a20 4b65 7973 2074 6861 7420 7368 6f75  : Keys that shou
+00008e10: 6c64 2072 656d 6169 6e20 756e 6368 616e  ld remain unchan
+00008e20: 6765 6420 6672 6f6d 2074 6865 206f 7269  ged from the ori
+00008e30: 6769 6e61 6c20 6578 706f 7274 0a20 2020  ginal export.   
+00008e40: 203a 7479 7065 206b 6579 735f 746f 5f6b   :type keys_to_k
+00008e50: 6565 703a 2044 6963 740a 2020 2020 3a70  eep: Dict.    :p
+00008e60: 6172 616d 206d 6573 7361 6765 5f64 6573  aram message_des
+00008e70: 7469 6e61 7469 6f6e 733a 204c 6973 7420  tinations: List 
+00008e80: 6f66 204d 6573 7361 6765 2044 6573 7469  of Message Desti
+00008e90: 6e61 7469 6f6e 2041 5049 204e 616d 6573  nation API Names
+00008ea0: 0a20 2020 203a 7061 7261 6d20 6675 6e63  .    :param func
+00008eb0: 7469 6f6e 733a 204c 6973 7420 6f66 2046  tions: List of F
+00008ec0: 756e 6374 696f 6e20 4150 4920 4e61 6d65  unction API Name
+00008ed0: 730a 2020 2020 3a70 6172 616d 2077 6f72  s.    :param wor
+00008ee0: 6b66 6c6f 7773 3a20 4c69 7374 206f 6620  kflows: List of 
+00008ef0: 576f 726b 666c 6f77 2041 5049 204e 616d  Workflow API Nam
+00008f00: 6573 0a20 2020 203a 7061 7261 6d20 7275  es.    :param ru
+00008f10: 6c65 733a 204c 6973 7420 6f66 2052 756c  les: List of Rul
+00008f20: 6520 4469 7370 6c61 7920 4e61 6d65 730a  e Display Names.
+00008f30: 2020 2020 3a70 6172 616d 2066 6965 6c64      :param field
+00008f40: 733a 204c 6973 7420 6f66 2046 6965 6c64  s: List of Field
+00008f50: 2065 7870 6f72 745f 6b65 7973 2065 2e67   export_keys e.g
+00008f60: 2e20 5b27 696e 6369 6465 6e74 2f63 7573  . ['incident/cus
+00008f70: 746f 6d5f 6669 656c 6427 2c20 2761 6374  tom_field', 'act
+00008f80: 696f 6e69 6e76 6f63 6174 696f 6e2f 6375  ioninvocation/cu
+00008f90: 7374 6f6d 5f61 6374 6976 6974 795f 6669  stom_activity_fi
+00008fa0: 656c 6427 2c20 275f 5f66 756e 6374 696f  eld', '__functio
+00008fb0: 6e2f 6375 7374 6f6d 5f66 6e5f 696e 7075  n/custom_fn_inpu
+00008fc0: 7427 5d0a 2020 2020 3a70 6172 616d 2061  t'].    :param a
+00008fd0: 7274 6966 6163 745f 7479 7065 733a 204c  rtifact_types: L
+00008fe0: 6973 7420 6f66 2043 7573 746f 6d20 4172  ist of Custom Ar
+00008ff0: 7469 6661 6374 2054 7970 6520 4150 4920  tifact Type API 
+00009000: 4e61 6d65 730a 2020 2020 3a70 6172 616d  Names.    :param
+00009010: 2064 6174 6174 6162 6c65 733a 204c 6973   datatables: Lis
+00009020: 7420 6f66 2044 6174 6120 5461 626c 6520  t of Data Table 
+00009030: 4150 4920 4e61 6d65 730a 2020 2020 3a70  API Names.    :p
+00009040: 6172 616d 2074 6173 6b73 3a20 4c69 7374  aram tasks: List
+00009050: 206f 6620 4375 7374 6f6d 2054 6173 6b20   of Custom Task 
+00009060: 4150 4920 4e61 6d65 730a 2020 2020 3a70  API Names.    :p
+00009070: 6172 616d 2074 6173 6b73 3a20 4c69 7374  aram tasks: List
+00009080: 206f 6620 5068 6173 6573 2041 5049 204e   of Phases API N
+00009090: 616d 6573 0a20 2020 203a 7061 7261 6d20  ames.    :param 
+000090a0: 7363 7269 7074 733a 204c 6973 7420 6f66  scripts: List of
+000090b0: 2053 6372 6970 7420 4469 7370 6c61 7920   Script Display 
+000090c0: 4e61 6d65 730a 2020 2020 3a70 6172 616d  Names.    :param
+000090d0: 2069 6e63 6964 656e 745f 7479 7065 733a   incident_types:
+000090e0: 204c 6973 7420 6f66 2043 7573 746f 6d20   List of Custom 
+000090f0: 496e 6369 6465 6e74 2054 7970 6520 4e61  Incident Type Na
+00009100: 6d65 730a 2020 2020 3a70 6172 616d 2070  mes.    :param p
+00009110: 6c61 7962 6f6f 6b73 3a20 4c69 7374 206f  laybooks: List o
+00009120: 6620 506c 6179 626f 6f6b 2041 5049 204e  f Playbook API N
+00009130: 616d 6573 0a20 2020 203a 7265 7475 726e  ames.    :return
+00009140: 3a20 5265 7475 726e 2061 2044 6963 7469  : Return a Dicti
+00009150: 6f6e 6172 7920 6f66 2052 6573 696c 6965  onary of Resilie
+00009160: 6e74 204f 626a 6563 7473 0a20 2020 203a  nt Objects.    :
+00009170: 7274 7970 653a 2044 6963 740a 2020 2020  rtype: Dict.    
+00009180: 2222 220a 2020 2020 2320 4465 6570 2063  """.    # Deep c
+00009190: 6f70 7920 7468 6520 6578 706f 7274 2c20  opy the export, 
+000091a0: 736f 2077 6520 646f 6e27 7420 6f76 6572  so we don't over
+000091b0: 7772 6974 6520 616e 7974 6869 6e67 0a20  write anything. 
+000091c0: 2020 206d 696e 6966 6965 645f 6578 706f     minified_expo
+000091d0: 7274 203d 2063 6f70 792e 6465 6570 636f  rt = copy.deepco
+000091e0: 7079 2865 7870 6f72 7429 0a0a 2020 2020  py(export)..    
+000091f0: 2320 4966 206e 6f20 6b65 7973 5f74 6f5f  # If no keys_to_
+00009200: 6b65 6570 2061 7265 2073 7065 6369 6669  keep are specifi
+00009210: 6564 2c20 7573 6520 7468 6573 6520 6465  ed, use these de
+00009220: 6661 756c 7473 0a20 2020 2023 206b 6579  faults.    # key
+00009230: 735f 746f 5f6b 6565 7020 6973 2075 7365  s_to_keep is use
+00009240: 6420 746f 206b 6565 7020 7661 6c75 6573  d to keep values
+00009250: 2066 726f 6d20 7468 6520 6f72 6967 696e   from the origin
+00009260: 616c 2065 7870 6f72 740a 2020 2020 2320  al export.    # 
+00009270: 7769 7468 6f75 7420 6265 696e 6720 6d69  without being mi
+00009280: 6e69 6669 6564 0a20 2020 2069 6620 6e6f  nified.    if no
+00009290: 7420 6b65 7973 5f74 6f5f 6b65 6570 3a0a  t keys_to_keep:.
+000092a0: 2020 2020 2020 2020 6b65 7973 5f74 6f5f          keys_to_
+000092b0: 6b65 6570 203d 205b 0a20 2020 2020 2020  keep = [.       
+000092c0: 2020 2020 2022 6578 706f 7274 5f64 6174       "export_dat
+000092d0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+000092e0: 2265 7870 6f72 745f 666f 726d 6174 5f76  "export_format_v
+000092f0: 6572 7369 6f6e 222c 0a20 2020 2020 2020  ersion",.       
+00009300: 2020 2020 2022 6964 222c 0a20 2020 2020       "id",.     
+00009310: 2020 2020 2020 2022 7365 7276 6572 5f76         "server_v
+00009320: 6572 7369 6f6e 220a 2020 2020 2020 2020  ersion".        
+00009330: 5d0a 0a20 2020 2023 2063 6572 7461 696e  ]..    # certain
+00009340: 206b 6579 7320 6e65 6564 2074 6f20 6265   keys need to be
+00009350: 2063 6c65 6172 6564 2c20 7261 7468 6572   cleared, rather
+00009360: 2074 6861 6e20 7365 7420 746f 2065 6d70   than set to emp
+00009370: 7479 206f 626a 6563 7473 0a20 2020 2023  ty objects.    #
+00009380: 2073 6f20 6173 206e 6f74 2074 6f20 7072   so as not to pr
+00009390: 6f63 6573 7320 6120 6465 6c65 7465 206f  ocess a delete o
+000093a0: 7220 7570 6461 7465 206f 6e20 7468 6520  r update on the 
+000093b0: 706c 6174 666f 726d 2077 6865 6e20 7468  platform when th
+000093c0: 650a 2020 2020 2320 6578 706f 7274 2069  e.    # export i
+000093d0: 7320 6d6f 6469 6669 6564 2061 6e64 2050  s modified and P
+000093e0: 4f53 5465 6420 6261 636b 2074 6f20 534f  OSTed back to SO
+000093f0: 4152 0a20 2020 206b 6579 735f 746f 5f63  AR.    keys_to_c
+00009400: 6c65 6172 203d 205b 0a20 2020 2020 2020  lear = [.       
+00009410: 2022 6f76 6572 7269 6465 7322 0a20 2020   "overrides".   
+00009420: 205d 0a0a 2020 2020 2320 736f 6d65 2069   ]..    # some i
+00009430: 6e63 6964 656e 7420 7479 7065 7320 6172  ncident types ar
+00009440: 6520 7061 7265 6e74 2f63 6869 6c64 2e20  e parent/child. 
+00009450: 5468 6973 2072 6f75 7469 6e65 2077 696c  This routine wil
+00009460: 6c20 7265 7475 726e 2061 6c6c 2074 6865  l return all the
+00009470: 2070 6172 656e 7420 696e 6369 6465 6e74   parent incident
+00009480: 2074 7970 6573 0a20 2020 2070 6172 656e   types.    paren
+00009490: 745f 6368 696c 645f 696e 6369 6465 6e74  t_child_incident
+000094a0: 5f74 7970 6573 203d 2066 696e 645f 7061  _types = find_pa
+000094b0: 7265 6e74 5f63 6869 6c64 5f74 7970 6573  rent_child_types
+000094c0: 2865 7870 6f72 742c 2022 696e 6369 6465  (export, "incide
+000094d0: 6e74 5f74 7970 6573 222c 2022 6e61 6d65  nt_types", "name
+000094e0: 222c 2069 6e63 6964 656e 745f 7479 7065  ", incident_type
+000094f0: 7329 0a0a 2020 2020 2320 5365 7475 7020  s)..    # Setup 
+00009500: 7468 6520 6b65 7973 5f74 6f5f 6d69 6e69  the keys_to_mini
+00009510: 6679 2064 6963 740a 2020 2020 6b65 7973  fy dict.    keys
+00009520: 5f74 6f5f 6d69 6e69 6679 203d 207b 0a20  _to_minify = {. 
+00009530: 2020 2020 2020 2022 6d65 7373 6167 655f         "message_
+00009540: 6465 7374 696e 6174 696f 6e73 223a 207b  destinations": {
+00009550: 5265 7369 6c69 656e 744f 626a 4d61 702e  ResilientObjMap.
+00009560: 4d45 5353 4147 455f 4445 5354 494e 4154  MESSAGE_DESTINAT
+00009570: 494f 4e53 3a20 6d65 7373 6167 655f 6465  IONS: message_de
+00009580: 7374 696e 6174 696f 6e73 7d2c 0a20 2020  stinations},.   
+00009590: 2020 2020 2022 6675 6e63 7469 6f6e 7322       "functions"
+000095a0: 3a20 7b52 6573 696c 6965 6e74 4f62 6a4d  : {ResilientObjM
+000095b0: 6170 2e46 554e 4354 494f 4e53 3a20 6675  ap.FUNCTIONS: fu
+000095c0: 6e63 7469 6f6e 737d 2c0a 2020 2020 2020  nctions},.      
+000095d0: 2020 2277 6f72 6b66 6c6f 7773 223a 207b    "workflows": {
+000095e0: 5265 7369 6c69 656e 744f 626a 4d61 702e  ResilientObjMap.
+000095f0: 574f 524b 464c 4f57 533a 2077 6f72 6b66  WORKFLOWS: workf
+00009600: 6c6f 7773 7d2c 0a20 2020 2020 2020 2022  lows},.        "
+00009610: 6163 7469 6f6e 7322 3a20 7b52 6573 696c  actions": {Resil
+00009620: 6965 6e74 4f62 6a4d 6170 2e52 554c 4553  ientObjMap.RULES
+00009630: 3a20 7275 6c65 737d 2c0a 2020 2020 2020  : rules},.      
+00009640: 2020 2266 6965 6c64 7322 3a20 7b22 6578    "fields": {"ex
+00009650: 706f 7274 5f6b 6579 223a 2066 6965 6c64  port_key": field
+00009660: 737d 2c0a 2020 2020 2020 2020 2269 6e63  s},.        "inc
+00009670: 6964 656e 745f 6172 7469 6661 6374 5f74  ident_artifact_t
+00009680: 7970 6573 223a 207b 5265 7369 6c69 656e  ypes": {Resilien
+00009690: 744f 626a 4d61 702e 494e 4349 4445 4e54  tObjMap.INCIDENT
+000096a0: 5f41 5254 4946 4143 545f 5459 5045 533a  _ARTIFACT_TYPES:
+000096b0: 2061 7274 6966 6163 745f 7479 7065 737d   artifact_types}
+000096c0: 2c0a 2020 2020 2020 2020 2274 7970 6573  ,.        "types
+000096d0: 223a 207b 5265 7369 6c69 656e 744f 626a  ": {ResilientObj
+000096e0: 4d61 702e 4441 5441 5441 424c 4553 3a20  Map.DATATABLES: 
+000096f0: 6461 7461 7461 626c 6573 7d2c 0a20 2020  datatables},.   
+00009700: 2020 2020 2022 6175 746f 6d61 7469 635f       "automatic_
+00009710: 7461 736b 7322 3a20 7b52 6573 696c 6965  tasks": {Resilie
+00009720: 6e74 4f62 6a4d 6170 2e54 4153 4b53 3a20  ntObjMap.TASKS: 
+00009730: 7461 736b 737d 2c0a 2020 2020 2020 2020  tasks},.        
+00009740: 2270 6861 7365 7322 3a20 7b52 6573 696c  "phases": {Resil
+00009750: 6965 6e74 4f62 6a4d 6170 2e50 4841 5345  ientObjMap.PHASE
+00009760: 533a 2070 6861 7365 737d 2c0a 2020 2020  S: phases},.    
+00009770: 2020 2020 2273 6372 6970 7473 223a 207b      "scripts": {
+00009780: 5265 7369 6c69 656e 744f 626a 4d61 702e  ResilientObjMap.
+00009790: 5343 5249 5054 533a 2073 6372 6970 7473  SCRIPTS: scripts
+000097a0: 7d2c 0a20 2020 2020 2020 2022 696e 6369  },.        "inci
+000097b0: 6465 6e74 5f74 7970 6573 223a 207b 5265  dent_types": {Re
+000097c0: 7369 6c69 656e 744f 626a 4d61 702e 494e  silientObjMap.IN
+000097d0: 4349 4445 4e54 5f54 5950 4553 3a20 7061  CIDENT_TYPES: pa
+000097e0: 7265 6e74 5f63 6869 6c64 5f69 6e63 6964  rent_child_incid
+000097f0: 656e 745f 7479 7065 737d 2c0a 2020 2020  ent_types},.    
+00009800: 2020 2020 2270 6c61 7962 6f6f 6b73 223a      "playbooks":
+00009810: 207b 5265 7369 6c69 656e 744f 626a 4d61   {ResilientObjMa
+00009820: 702e 504c 4159 424f 4f4b 533a 2070 6c61  p.PLAYBOOKS: pla
+00009830: 7962 6f6f 6b73 7d0a 2020 2020 7d0a 0a20  ybooks}.    }.. 
+00009840: 2020 2066 6f72 206b 6579 2069 6e20 6d69     for key in mi
+00009850: 6e69 6669 6564 5f65 7870 6f72 742e 6b65  nified_export.ke
+00009860: 7973 2829 3a0a 0a20 2020 2020 2020 2023  ys():..        #
+00009870: 2049 6620 7765 206b 6565 7020 7468 6973   If we keep this
+00009880: 206f 6e65 2c20 736b 6970 0a20 2020 2020   one, skip.     
+00009890: 2020 2069 6620 6b65 7920 696e 206b 6579     if key in key
+000098a0: 735f 746f 5f6b 6565 703a 0a20 2020 2020  s_to_keep:.     
+000098b0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+000098c0: 0a20 2020 2020 2020 2023 2049 6620 7765  .        # If we
+000098d0: 2061 7265 2074 6f20 6d69 6e69 6679 2069   are to minify i
+000098e0: 740a 2020 2020 2020 2020 656c 6966 206b  t.        elif k
+000098f0: 6579 2069 6e20 6b65 7973 5f74 6f5f 6d69  ey in keys_to_mi
+00009900: 6e69 6679 2e6b 6579 7328 293a 0a0a 2020  nify.keys():..  
+00009910: 2020 2020 2020 2020 2020 2320 4765 7420            # Get 
+00009920: 7468 6520 6174 7472 6962 7574 655f 6e61  the attribute_na
+00009930: 6d65 2074 6f20 6d61 7463 6820 6f6e 2028  me to match on (
+00009940: 6e6f 726d 616c 6c79 2027 6e61 6d65 272f  normally 'name'/
+00009950: 2770 726f 6772 616d 6d61 7469 635f 6e61  'programmatic_na
+00009960: 6d65 272f 2765 7870 6f72 745f 6b65 7927  me'/'export_key'
+00009970: 290a 2020 2020 2020 2020 2020 2020 6174  ).            at
+00009980: 7472 6962 7574 655f 6e61 6d65 203d 206c  tribute_name = l
+00009990: 6973 7428 6b65 7973 5f74 6f5f 6d69 6e69  ist(keys_to_mini
+000099a0: 6679 5b6b 6579 5d2e 6b65 7973 2829 295b  fy[key].keys())[
+000099b0: 305d 0a0a 2020 2020 2020 2020 2020 2020  0]..            
+000099c0: 7661 6c75 6573 203d 206b 6579 735f 746f  values = keys_to
+000099d0: 5f6d 696e 6966 795b 6b65 795d 5b61 7474  _minify[key][att
+000099e0: 7269 6275 7465 5f6e 616d 655d 0a20 2020  ribute_name].   
+000099f0: 2020 2020 2020 2020 2023 2073 7472 6970           # strip
+00009a00: 206f 7574 2065 7874 7261 2073 7061 6365   out extra space
+00009a10: 7320 6672 6f6d 2074 6865 2061 7474 7269  s from the attri
+00009a20: 6275 7465 2028 6965 2044 6973 706c 6179  bute (ie Display
+00009a30: 206e 616d 6520 666f 7220 5275 6c65 732c   name for Rules,
+00009a40: 2053 6372 6970 7473 2c20 6574 632e 290a   Scripts, etc.).
+00009a50: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00009a60: 6573 203d 205b 6e61 6d65 2e73 7472 6970  es = [name.strip
+00009a70: 2829 2066 6f72 206e 616d 6520 696e 2076  () for name in v
+00009a80: 616c 7565 735d 0a0a 2020 2020 2020 2020  alues]..        
+00009a90: 2020 2020 6f62 6a20 3d20 6d69 6e69 6669      obj = minifi
+00009aa0: 6564 5f65 7870 6f72 742e 6765 7428 6b65  ed_export.get(ke
+00009ab0: 7929 0a0a 2020 2020 2020 2020 2020 2020  y)..            
+00009ac0: 6966 206f 626a 3a0a 2020 2020 2020 2020  if obj:.        
+00009ad0: 2020 2020 2020 2020 666f 7220 6461 7461          for data
+00009ae0: 2069 6e20 6c69 7374 286f 626a 293a 0a0a   in list(obj):..
+00009af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b00: 2020 2020 6966 206e 6f74 2064 6174 612e      if not data.
+00009b10: 6765 7428 6174 7472 6962 7574 655f 6e61  get(attribute_na
+00009b20: 6d65 293a 0a20 2020 2020 2020 2020 2020  me):.           
+00009b30: 2020 2020 2020 2020 2020 2020 204c 4f47               LOG
+00009b40: 2e77 6172 6e69 6e67 2822 4e6f 2025 7320  .warning("No %s 
+00009b50: 696e 2025 7322 2c20 6174 7472 6962 7574  in %s", attribut
+00009b60: 655f 6e61 6d65 2c20 6b65 7929 0a0a 2020  e_name, key)..  
+00009b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b80: 2020 2320 7374 7269 7020 6f75 7420 6578    # strip out ex
+00009b90: 7472 6120 7370 6163 6573 2066 726f 6d20  tra spaces from 
+00009ba0: 7468 6520 6174 7472 6962 7574 6520 2869  the attribute (i
+00009bb0: 6520 4469 7370 6c61 7920 6e61 6d65 2066  e Display name f
+00009bc0: 6f72 2052 756c 6573 2c20 5363 7269 7074  or Rules, Script
+00009bd0: 732c 2065 7463 2e29 0a20 2020 2020 2020  s, etc.).       
+00009be0: 2020 2020 2020 2020 2020 2020 2023 2049               # I
+00009bf0: 6620 7468 6973 2052 6573 696c 6965 6e74  f this Resilient
+00009c00: 204f 626a 6563 7420 6973 206e 6f74 2069   Object is not i
+00009c10: 6e20 6f75 7220 6d69 6e69 6679 206c 6973  n our minify lis
+00009c20: 742c 2072 656d 6f76 6520 6974 0a20 2020  t, remove it.   
+00009c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c40: 2069 6620 6e6f 7420 6461 7461 2e67 6574   if not data.get
+00009c50: 2861 7474 7269 6275 7465 5f6e 616d 652c  (attribute_name,
+00009c60: 2022 2229 2e73 7472 6970 2829 2069 6e20   "").strip() in 
+00009c70: 7661 6c75 6573 3a0a 2020 2020 2020 2020  values:.        
+00009c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c90: 6d69 6e69 6669 6564 5f65 7870 6f72 745b  minified_export[
+00009ca0: 6b65 795d 2e72 656d 6f76 6528 6461 7461  key].remove(data
+00009cb0: 290a 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
+00009cc0: 6b65 7920 696e 206b 6579 735f 746f 5f63  key in keys_to_c
+00009cd0: 6c65 6172 3a0a 2020 2020 2020 2020 2020  lear:.          
+00009ce0: 2020 6d69 6e69 6669 6564 5f65 7870 6f72    minified_expor
+00009cf0: 745b 6b65 795d 203d 204e 6f6e 650a 0a20  t[key] = None.. 
+00009d00: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+00009d10: 7374 616e 6365 286d 696e 6966 6965 645f  stance(minified_
+00009d20: 6578 706f 7274 5b6b 6579 5d2c 206c 6973  export[key], lis
+00009d30: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00009d40: 6d69 6e69 6669 6564 5f65 7870 6f72 745b  minified_export[
+00009d50: 6b65 795d 203d 205b 5d0a 0a20 2020 2020  key] = []..     
+00009d60: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00009d70: 6365 286d 696e 6966 6965 645f 6578 706f  ce(minified_expo
+00009d80: 7274 5b6b 6579 5d2c 2064 6963 7429 3a0a  rt[key], dict):.
+00009d90: 2020 2020 2020 2020 2020 2020 6d69 6e69              mini
+00009da0: 6669 6564 5f65 7870 6f72 745b 6b65 795d  fied_export[key]
+00009db0: 203d 207b 7d0a 0a20 2020 2020 2020 2065   = {}..        e
+00009dc0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00009dd0: 206d 696e 6966 6965 645f 6578 706f 7274   minified_export
+00009de0: 5b6b 6579 5d20 3d20 4e6f 6e65 0a0a 2020  [key] = None..  
+00009df0: 2020 2320 4164 6420 6465 6661 756c 7420    # Add default 
+00009e00: 696e 6369 6465 6e74 5f74 7970 652e 204e  incident_type. N
+00009e10: 6565 6465 6420 666f 7220 6576 6572 7920  eeded for every 
+00009e20: 496d 706f 7274 0a20 2020 2069 6620 6d69  Import.    if mi
+00009e30: 6e69 6669 6564 5f65 7870 6f72 742e 6765  nified_export.ge
+00009e40: 7428 2269 6e63 6964 656e 745f 7479 7065  t("incident_type
+00009e50: 7322 293a 0a20 2020 2020 2020 206d 696e  s"):.        min
+00009e60: 6966 6965 645f 6578 706f 7274 5b22 696e  ified_export["in
+00009e70: 6369 6465 6e74 5f74 7970 6573 225d 2e61  cident_types"].a
+00009e80: 7070 656e 6428 4445 4641 554c 545f 494e  ppend(DEFAULT_IN
+00009e90: 4349 4445 4e54 5f54 5950 4529 0a20 2020  CIDENT_TYPE).   
+00009ea0: 2065 6c73 653a 0a20 2020 2020 2020 206d   else:.        m
+00009eb0: 696e 6966 6965 645f 6578 706f 7274 5b22  inified_export["
+00009ec0: 696e 6369 6465 6e74 5f74 7970 6573 225d  incident_types"]
+00009ed0: 203d 205b 4445 4641 554c 545f 494e 4349   = [DEFAULT_INCI
+00009ee0: 4445 4e54 5f54 5950 455d 0a0a 2020 2020  DENT_TYPE]..    
+00009ef0: 2320 4966 206e 6f20 4375 7374 6f6d 2049  # If no Custom I
+00009f00: 6e63 6964 656e 7420 4669 656c 6473 2061  ncident Fields a
+00009f10: 7265 2069 6e20 7468 6520 6578 706f 7274  re in the export
+00009f20: 2c20 6164 6420 7468 6973 2064 6566 6175  , add this defau
+00009f30: 6c74 2e0a 2020 2020 2320 416e 2069 6d70  lt..    # An imp
+00009f40: 6f72 7420 6e65 6564 7320 6174 206c 6561  ort needs at lea
+00009f50: 7374 2031 2049 6e63 6964 656e 7420 4669  st 1 Incident Fi
+00009f60: 656c 640a 2020 2020 6966 2022 696e 6369  eld.    if "inci
+00009f70: 6465 6e74 2f22 206e 6f74 2069 6e20 6669  dent/" not in fi
+00009f80: 656c 6473 3a0a 2020 2020 2020 2020 6d69  elds:.        mi
+00009f90: 6e69 6669 6564 5f65 7870 6f72 745b 2266  nified_export["f
+00009fa0: 6965 6c64 7322 5d2e 6170 7065 6e64 2844  ields"].append(D
+00009fb0: 4546 4155 4c54 5f49 4e43 4944 454e 545f  EFAULT_INCIDENT_
+00009fc0: 4649 454c 4429 0a0a 2020 2020 2320 436c  FIELD)..    # Cl
+00009fd0: 6561 6e20 6f75 7420 616e 7920 7069 6920  ean out any pii 
+00009fe0: 7661 6c75 6573 2077 6974 6820 6b65 7973  values with keys
+00009ff0: 2069 6e63 6c75 6465 6420 696e 2070 6969   included in pii
+0000a000: 5f6b 6579 5f6c 6973 740a 2020 2020 7069  _key_list.    pi
+0000a010: 695f 6b65 795f 6c69 7374 203d 205b 2263  i_key_list = ["c
+0000a020: 7265 6174 6f72 222c 2022 6372 6561 746f  reator", "creato
+0000a030: 725f 6964 225d 0a20 2020 206d 696e 6966  r_id"].    minif
+0000a040: 6965 645f 6578 706f 7274 203d 2072 6d5f  ied_export = rm_
+0000a050: 7069 6928 7069 695f 6b65 795f 6c69 7374  pii(pii_key_list
+0000a060: 2c20 6d69 6e69 6669 6564 5f65 7870 6f72  , minified_expor
+0000a070: 7429 0a0a 2020 2020 6d69 6e69 6669 6564  t)..    minified
+0000a080: 5f65 7870 6f72 7420 3d20 7265 6d6f 7665  _export = remove
+0000a090: 5f74 6167 286d 696e 6966 6965 645f 6578  _tag(minified_ex
+0000a0a0: 706f 7274 290a 0a20 2020 2072 6574 7572  port)..    retur
+0000a0b0: 6e20 6d69 6e69 6669 6564 5f65 7870 6f72  n minified_expor
+0000a0c0: 740a 0a0a 6465 6620 726d 5f70 6969 2870  t...def rm_pii(p
+0000a0d0: 6969 5f6b 6579 5f6c 6973 742c 2065 7870  ii_key_list, exp
+0000a0e0: 6f72 7429 3a0a 2020 2020 2222 220a 2020  ort):.    """.  
+0000a0f0: 2020 5265 6d6f 7665 2061 6e79 206b 6579    Remove any key
+0000a100: 7320 6672 6f6d 2027 6578 706f 7274 2720  s from 'export' 
+0000a110: 7468 6174 2061 7265 2069 6e20 2770 6969  that are in 'pii
+0000a120: 5f6b 6579 5f6c 6973 7427 2e0a 2020 2020  _key_list'..    
+0000a130: 5265 6375 7273 6976 656c 7920 7365 6172  Recursively sear
+0000a140: 6368 6573 2074 6865 2065 7870 6f72 7420  ches the export 
+0000a150: 6f62 6a65 6374 2e0a 0a20 2020 203a 7061  object...    :pa
+0000a160: 7261 6d20 7069 695f 6b65 795f 6c69 7374  ram pii_key_list
+0000a170: 3a20 6c69 7374 206f 6620 7374 7220 6b65  : list of str ke
+0000a180: 7973 2074 6f20 6265 2072 656d 6f76 6564  ys to be removed
+0000a190: 2066 726f 6d20 2765 7870 6f72 7427 2e20   from 'export'. 
+0000a1a0: 6578 3a20 5b22 6372 6561 746f 7222 2c20  ex: ["creator", 
+0000a1b0: 2263 7265 6174 6f72 5f69 6422 5d0a 2020  "creator_id"].  
+0000a1c0: 2020 3a74 7970 6520 7069 695f 6b65 795f    :type pii_key_
+0000a1d0: 6c69 7374 3a20 5b73 7472 5d0a 2020 2020  list: [str].    
+0000a1e0: 3a70 6172 616d 2065 7870 6f72 743a 2074  :param export: t
+0000a1f0: 6865 2072 6573 756c 7420 6f66 2063 616c  he result of cal
+0000a200: 6c69 6e67 2067 6574 5f6c 6174 6573 745f  ling get_latest_
+0000a210: 6f72 675f 6578 706f 7274 2829 206f 7220  org_export() or 
+0000a220: 6d69 6e69 6669 6564 5f65 7870 6f72 7420  minified_export 
+0000a230: 6672 6f6d 2063 616c 6c69 6e67 206d 696e  from calling min
+0000a240: 6966 795f 6578 706f 7274 2829 0a20 2020  ify_export().   
+0000a250: 203a 7479 7065 2065 7870 6f72 743a 2044   :type export: D
+0000a260: 6963 740a 2020 2020 3a72 6574 7572 6e3a  ict.    :return:
+0000a270: 206d 6f64 6966 6965 6420 6578 706f 7274   modified export
+0000a280: 2077 6974 6820 616e 7920 7069 6920 6b65   with any pii ke
+0000a290: 7973 2072 656d 6f76 6564 0a20 2020 203a  ys removed.    :
+0000a2a0: 7274 7970 653a 2044 6963 740a 2020 2020  rtype: Dict.    
+0000a2b0: 2222 220a 0a20 2020 2069 6620 6578 706f  """..    if expo
+0000a2c0: 7274 3a0a 2020 2020 2020 2020 6578 706f  rt:.        expo
+0000a2d0: 7274 5f63 6f70 7920 3d20 6578 706f 7274  rt_copy = export
+0000a2e0: 2e63 6f70 7928 290a 0a20 2020 2020 2020  .copy()..       
+0000a2f0: 2066 6f72 206b 6579 2069 6e20 6c69 7374   for key in list
+0000a300: 2865 7870 6f72 745f 636f 7079 2e6b 6579  (export_copy.key
+0000a310: 7328 2929 3a0a 2020 2020 2020 2020 2020  s()):.          
+0000a320: 2020 636f 6e74 656e 7420 3d20 6578 706f    content = expo
+0000a330: 7274 5f63 6f70 795b 6b65 795d 0a0a 2020  rt_copy[key]..  
+0000a340: 2020 2020 2020 2020 2020 2320 6966 206b            # if k
+0000a350: 6579 2069 7320 696e 2070 6969 5f6c 6973  ey is in pii_lis
+0000a360: 7420 746f 2072 656d 6f76 652c 2064 656c  t to remove, del
+0000a370: 6574 6520 656e 7472 7920 696e 2070 6179  ete entry in pay
+0000a380: 6c6f 6164 5f72 6573 756c 740a 2020 2020  load_result.    
+0000a390: 2020 2020 2020 2020 6966 206b 6579 2069          if key i
+0000a3a0: 6e20 7069 695f 6b65 795f 6c69 7374 3a0a  n pii_key_list:.
+0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3c0: 6465 6c20 6578 706f 7274 5f63 6f70 795b  del export_copy[
+0000a3d0: 6b65 795d 0a20 2020 2020 2020 2020 2020  key].           
+0000a3e0: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
+0000a3f0: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
+0000a400: 6b65 7920 7761 736e 2774 2069 6e20 7069  key wasn't in pi
+0000a410: 695f 6c69 7374 2c20 636f 6e74 696e 7565  i_list, continue
+0000a420: 2073 6561 7263 6869 6e67 2072 6563 7572   searching recur
+0000a430: 7369 7665 6c79 2066 6f72 2064 6963 7469  sively for dicti
+0000a440: 6f6e 6172 6965 7320 616e 6420 7363 7275  onaries and scru
+0000a450: 6262 696e 6720 7069 690a 2020 2020 2020  bbing pii.      
+0000a460: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000a470: 6e63 6528 636f 6e74 656e 742c 2064 6963  nce(content, dic
+0000a480: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+0000a490: 2020 2020 6578 706f 7274 5f63 6f70 795b      export_copy[
+0000a4a0: 6b65 795d 203d 2072 6d5f 7069 6928 7069  key] = rm_pii(pi
+0000a4b0: 695f 6b65 795f 6c69 7374 2c20 636f 6e74  i_key_list, cont
+0000a4c0: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
+0000a4d0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+0000a4e0: 2863 6f6e 7465 6e74 2c20 6c69 7374 293a  (content, list):
+0000a4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a500: 2023 2072 6563 7265 6174 6573 2074 6865   # recreates the
+0000a510: 206c 6973 7420 7768 6572 6520 616e 7920   list where any 
+0000a520: 6469 6374 2065 6c65 6d65 6e74 7320 6f66  dict elements of
+0000a530: 2074 6865 206c 6973 7420 6172 6520 7265   the list are re
+0000a540: 6375 7273 6976 656c 7920 7363 7275 6262  cursively scrubb
+0000a550: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+0000a560: 2020 2023 2069 6620 6c69 7374 2069 7465     # if list ite
+0000a570: 6d20 6973 206e 6f74 2061 2064 6963 7469  m is not a dicti
+0000a580: 6f6e 6172 792c 2064 6f6e 2774 0a20 2020  onary, don't.   
+0000a590: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+0000a5a0: 6f72 745f 636f 7079 5b6b 6579 5d20 3d20  ort_copy[key] = 
+0000a5b0: 5b72 6d5f 7069 6928 7069 695f 6b65 795f  [rm_pii(pii_key_
+0000a5c0: 6c69 7374 2c20 6c69 7374 5f63 6f6e 7465  list, list_conte
+0000a5d0: 6e74 2920 6966 2069 7369 6e73 7461 6e63  nt) if isinstanc
+0000a5e0: 6528 6c69 7374 5f63 6f6e 7465 6e74 2c20  e(list_content, 
+0000a5f0: 6469 6374 2920 656c 7365 206c 6973 745f  dict) else list_
+0000a600: 636f 6e74 656e 7420 666f 7220 6c69 7374  content for list
+0000a610: 5f63 6f6e 7465 6e74 2069 6e20 636f 6e74  _content in cont
+0000a620: 656e 745d 0a0a 2020 2020 2020 2020 7265  ent]..        re
+0000a630: 7475 726e 2065 7870 6f72 745f 636f 7079  turn export_copy
+0000a640: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+0000a650: 2020 2072 6574 7572 6e20 6578 706f 7274     return export
+0000a660: 0a0a 0a64 6566 2066 696e 645f 7061 7265  ...def find_pare
+0000a670: 6e74 5f63 6869 6c64 5f74 7970 6573 2865  nt_child_types(e
+0000a680: 7870 6f72 742c 206f 626a 6563 745f 7479  xport, object_ty
+0000a690: 7065 2c20 6174 7472 6962 7574 655f 6e61  pe, attribute_na
+0000a6a0: 6d65 2c20 6e61 6d65 5f6c 6973 7429 3a0a  me, name_list):.
+0000a6b0: 2020 2020 2222 225b 6765 7420 616c 6c20      """[get all 
+0000a6c0: 7061 7265 6e74 206f 626a 6563 7473 2028  parent objects (
+0000a6d0: 6c69 6b65 2069 6e63 6964 656e 745f 7479  like incident_ty
+0000a6e0: 7065 7329 5d0a 0a20 2020 2041 7267 733a  pes)]..    Args:
+0000a6f0: 0a20 2020 2020 2020 2065 7870 6f72 7420  .        export 
+0000a700: 285b 6469 6374 5d29 3a20 5b65 7870 6f72  ([dict]): [expor
+0000a710: 7420 6669 6c65 2074 6f20 7061 7273 655d  t file to parse]
+0000a720: 0a20 2020 2020 2020 206f 626a 6563 745f  .        object_
+0000a730: 7479 7065 2028 5b73 7472 5d29 3a20 5b68  type ([str]): [h
+0000a740: 6569 7261 7263 6879 206f 6620 6f62 6a65  eirarchy of obje
+0000a750: 6374 7320 746f 2070 6172 7365 5d0a 2020  cts to parse].  
+0000a760: 2020 2020 2020 6174 7472 6962 7574 655f        attribute_
+0000a770: 6e61 6d65 2028 5b73 7472 5d29 3a20 5b6e  name ([str]): [n
+0000a780: 616d 6520 6f66 2066 6965 6c64 2074 6f20  ame of field to 
+0000a790: 6368 6563 6b20 666f 725d 0a20 2020 2020  check for].     
+0000a7a0: 2020 206e 616d 655f 6c69 7374 2028 5b6c     name_list ([l
+0000a7b0: 6973 745d 293a 205b 6c69 7374 206f 6620  ist]): [list of 
+0000a7c0: 6f62 6a65 6374 7320 746f 2073 616d 655d  objects to same]
+0000a7d0: 0a20 2020 2022 2222 0a0a 2020 2020 6578  .    """..    ex
+0000a7e0: 7465 6e64 6564 5f6e 616d 655f 6c69 7374  tended_name_list
+0000a7f0: 203d 206e 616d 655f 6c69 7374 5b3a 5d0a   = name_list[:].
+0000a800: 0a20 2020 2069 6620 6578 706f 7274 2e67  .    if export.g
+0000a810: 6574 286f 626a 6563 745f 7479 7065 293a  et(object_type):
+0000a820: 0a20 2020 2020 2020 2073 6563 7469 6f6e  .        section
+0000a830: 203d 2065 7870 6f72 742e 6765 7428 6f62   = export.get(ob
+0000a840: 6a65 6374 5f74 7970 6529 0a20 2020 2020  ject_type).     
+0000a850: 2020 2066 6f72 206e 616d 6520 696e 206e     for name in n
+0000a860: 616d 655f 6c69 7374 3a0a 2020 2020 2020  ame_list:.      
+0000a870: 2020 2020 2020 666f 7220 6974 656d 2069        for item i
+0000a880: 6e20 7365 6374 696f 6e3a 0a20 2020 2020  n section:.     
+0000a890: 2020 2020 2020 2020 2069 6620 6974 656d           if item
+0000a8a0: 2e67 6574 2861 7474 7269 6275 7465 5f6e  .get(attribute_n
+0000a8b0: 616d 6529 203d 3d20 6e61 6d65 3a0a 2020  ame) == name:.  
+0000a8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8d0: 6966 2069 7465 6d2e 6765 7428 2770 6172  if item.get('par
+0000a8e0: 656e 745f 6964 2729 3a0a 2020 2020 2020  ent_id'):.      
+0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a900: 2320 6164 6420 7468 6520 7061 7265 6e74  # add the parent
+0000a910: 2068 6965 7261 7263 6879 0a20 2020 2020   hierarchy.     
+0000a920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a930: 2070 6172 656e 745f 6c69 7374 203d 2066   parent_list = f
+0000a940: 696e 645f 7061 7265 6e74 5f63 6869 6c64  ind_parent_child
+0000a950: 5f74 7970 6573 2865 7870 6f72 742c 206f  _types(export, o
+0000a960: 626a 6563 745f 7479 7065 2c20 6174 7472  bject_type, attr
+0000a970: 6962 7574 655f 6e61 6d65 2c20 5b69 7465  ibute_name, [ite
+0000a980: 6d2e 6765 7428 2770 6172 656e 745f 6964  m.get('parent_id
+0000a990: 2729 5d29 0a20 2020 2020 2020 2020 2020  ')]).           
+0000a9a0: 2020 2020 2020 2020 2020 2065 7874 656e             exten
+0000a9b0: 6465 645f 6e61 6d65 5f6c 6973 742e 6578  ded_name_list.ex
+0000a9c0: 7465 6e64 2870 6172 656e 745f 6c69 7374  tend(parent_list
+0000a9d0: 290a 0a20 2020 2072 6574 7572 6e20 6c69  )..    return li
+0000a9e0: 7374 2873 6574 2865 7874 656e 6465 645f  st(set(extended_
+0000a9f0: 6e61 6d65 5f6c 6973 7429 290a 0a0a 6465  name_list))...de
+0000aa00: 6620 6c6f 6164 5f70 795f 6d6f 6475 6c65  f load_py_module
+0000aa10: 2870 6174 685f 7079 7468 6f6e 5f66 696c  (path_python_fil
+0000aa20: 652c 206d 6f64 756c 655f 6e61 6d65 293a  e, module_name):
+0000aa30: 0a20 2020 2022 2222 0a20 2020 2052 6574  .    """.    Ret
+0000aa40: 7572 6e20 7468 6520 7061 7468 5f70 7974  urn the path_pyt
+0000aa50: 686f 6e5f 6669 6c65 2061 7320 6120 5079  hon_file as a Py
+0000aa60: 7468 6f6e 204d 6f64 756c 652e 0a20 2020  thon Module..   
+0000aa70: 2057 6520 6361 6e20 7468 656e 2061 6363   We can then acc
+0000aa80: 6573 7320 6974 206d 6574 686f 6473 206c  ess it methods l
+0000aa90: 696b 653a 0a0a 2020 2020 2020 2020 3e20  ike:..        > 
+0000aaa0: 7265 7375 6c74 203d 2070 795f 6d6f 6475  result = py_modu
+0000aab0: 6c65 2e73 6f6d 655f 6d65 7468 6f64 5f69  le.some_method_i
+0000aac0: 6e5f 6d6f 6475 6c65 2829 0a0a 2020 2020  n_module()..    
+0000aad0: 3a70 6172 616d 2070 6174 685f 7079 7468  :param path_pyth
+0000aae0: 6f6e 5f66 696c 653a 2050 6174 6820 746f  on_file: Path to
+0000aaf0: 2074 6865 2066 696c 6520 7468 6174 2063   the file that c
+0000ab00: 6f6e 7461 696e 7320 7468 6520 6d6f 6475  ontains the modu
+0000ab10: 6c65 0a20 2020 203a 7061 7261 6d20 6d6f  le.    :param mo
+0000ab20: 6475 6c65 5f6e 616d 653a 2049 7320 6e6f  dule_name: Is no
+0000ab30: 726d 616c 6c79 2074 6865 2066 696c 6520  rmally the file 
+0000ab40: 6e61 6d65 2077 6974 686f 7574 2074 6865  name without the
+0000ab50: 202e 7079 0a20 2020 203a 7265 7475 726e   .py.    :return
+0000ab60: 3a20 5468 6520 5079 7468 6f6e 204d 6f64  : The Python Mod
+0000ab70: 756c 6520 666f 756e 640a 2020 2020 3a72  ule found.    :r
+0000ab80: 7479 7065 3a20 6d6f 6475 6c65 0a20 2020  type: module.   
+0000ab90: 2022 2222 0a20 2020 2023 2049 6e73 6572   """.    # Inser
+0000aba0: 7420 7468 6520 7061 7265 6e74 2064 6972  t the parent dir
+0000abb0: 206f 6620 7061 7468 5f70 7974 686f 6e5f   of path_python_
+0000abc0: 6669 6c65 2074 6f20 7468 6520 7374 6172  file to the star
+0000abd0: 7420 6f66 206f 7572 2050 7974 686f 6e20  t of our Python 
+0000abe0: 5041 5448 2061 7420 7275 6e74 696d 650a  PATH at runtime.
+0000abf0: 2020 2020 7061 7468 5f70 6172 656e 745f      path_parent_
+0000ac00: 6469 7220 3d20 6f73 2e70 6174 682e 6469  dir = os.path.di
+0000ac10: 726e 616d 6528 7061 7468 5f70 7974 686f  rname(path_pytho
+0000ac20: 6e5f 6669 6c65 290a 2020 2020 7379 732e  n_file).    sys.
+0000ac30: 7061 7468 2e69 6e73 6572 7428 302c 2070  path.insert(0, p
+0000ac40: 6174 685f 7061 7265 6e74 5f64 6972 290a  ath_parent_dir).
+0000ac50: 0a20 2020 2023 2049 6d70 6f72 7420 7468  .    # Import th
+0000ac60: 6520 6d6f 6475 6c65 0a20 2020 2070 795f  e module.    py_
+0000ac70: 6d6f 6475 6c65 203d 2069 6d70 6f72 746c  module = importl
+0000ac80: 6962 2e69 6d70 6f72 745f 6d6f 6475 6c65  ib.import_module
+0000ac90: 286d 6f64 756c 655f 6e61 6d65 290a 0a20  (module_name).. 
+0000aca0: 2020 2023 2052 656c 6f61 6420 7468 6520     # Reload the 
+0000acb0: 6d6f 6475 6c65 2073 6f20 7765 2067 6574  module so we get
+0000acc0: 2074 6865 206c 6174 6573 7420 6f6e 650a   the latest one.
+0000acd0: 2020 2020 2320 4966 2077 6520 646f 206e      # If we do n
+0000ace0: 6f74 2072 656c 6f61 642c 2063 616e 2067  ot reload, can g
+0000acf0: 6574 2073 7461 6c65 2072 6573 756c 7473  et stale results
+0000ad00: 2069 660a 2020 2020 2320 7468 6973 206d   if.    # this m
+0000ad10: 6574 686f 6420 6973 2063 616c 6c65 6420  ethod is called 
+0000ad20: 6d6f 7265 2074 6865 6e20 6f6e 6365 0a20  more then once. 
+0000ad30: 2020 2072 656c 6f61 6428 7079 5f6d 6f64     reload(py_mod
+0000ad40: 756c 6529 0a0a 2020 2020 2320 5265 6d6f  ule)..    # Remo
+0000ad50: 7665 2074 6865 2070 6174 6820 6672 6f6d  ve the path from
+0000ad60: 2050 5954 484f 4e50 4154 480a 2020 2020   PYTHONPATH.    
+0000ad70: 7379 732e 7061 7468 2e72 656d 6f76 6528  sys.path.remove(
+0000ad80: 7061 7468 5f70 6172 656e 745f 6469 7229  path_parent_dir)
+0000ad90: 0a0a 2020 2020 7265 7475 726e 2070 795f  ..    return py_
+0000ada0: 6d6f 6475 6c65 0a0a 0a64 6566 2072 656e  module...def ren
+0000adb0: 616d 655f 746f 5f62 616b 5f66 696c 6528  ame_to_bak_file(
+0000adc0: 7061 7468 5f63 7572 7265 6e74 5f66 696c  path_current_fil
+0000add0: 652c 2070 6174 685f 6465 6661 756c 745f  e, path_default_
+0000ade0: 6669 6c65 3d4e 6f6e 6529 3a0a 2020 2020  file=None):.    
+0000adf0: 2222 2252 656e 616d 6573 2070 6174 685f  """Renames path_
+0000ae00: 6375 7272 656e 745f 6669 6c65 2077 6974  current_file wit
+0000ae10: 6820 6120 706f 7374 6669 7865 6420 7469  h a postfixed ti
+0000ae20: 6d65 7374 616d 702e 0a20 2020 2049 6620  mestamp..    If 
+0000ae30: 7061 7468 5f64 6566 6175 6c74 5f66 696c  path_default_fil
+0000ae40: 6520 6973 2070 726f 7669 6465 642c 2070  e is provided, p
+0000ae50: 6174 685f 6375 7272 656e 745f 6669 6c65  ath_current_file
+0000ae60: 2069 7320 6f6e 6c79 0a20 2020 2072 656e   is only.    ren
+0000ae70: 616d 6564 2069 6620 7468 6520 6465 6661  amed if the defa
+0000ae80: 756c 7420 616e 6420 6375 7272 656e 7420  ult and current 
+0000ae90: 6669 6c65 2061 7265 2064 6966 6665 7265  file are differe
+0000aea0: 6e74 2222 220a 2020 2020 6966 206e 6f74  nt""".    if not
+0000aeb0: 206f 732e 7061 7468 2e69 7366 696c 6528   os.path.isfile(
+0000aec0: 7061 7468 5f63 7572 7265 6e74 5f66 696c  path_current_fil
+0000aed0: 6529 3a0a 2020 2020 2020 2020 4c4f 472e  e):.        LOG.
+0000aee0: 7761 726e 696e 6728 224e 6f20 6261 636b  warning("No back
+0000aef0: 7570 2066 696c 6520 6372 6561 7465 6420  up file created 
+0000af00: 6475 6520 746f 2066 696c 6520 6d69 7373  due to file miss
+0000af10: 696e 673a 2025 7322 2c20 7061 7468 5f63  ing: %s", path_c
+0000af20: 7572 7265 6e74 5f66 696c 6529 0a20 2020  urrent_file).   
+0000af30: 2020 2020 2072 6574 7572 6e20 7061 7468       return path
+0000af40: 5f63 7572 7265 6e74 5f66 696c 650a 0a20  _current_file.. 
+0000af50: 2020 2069 6620 7061 7468 5f64 6566 6175     if path_defau
+0000af60: 6c74 5f66 696c 6520 6973 206e 6f74 204e  lt_file is not N
+0000af70: 6f6e 6520 616e 6420 6e6f 7420 6f73 2e70  one and not os.p
+0000af80: 6174 682e 6973 6669 6c65 2870 6174 685f  ath.isfile(path_
+0000af90: 6465 6661 756c 745f 6669 6c65 293a 0a20  default_file):. 
+0000afa0: 2020 2020 2020 2072 6169 7365 2049 4f45         raise IOE
+0000afb0: 7272 6f72 2822 4465 6661 756c 7420 6669  rror("Default fi
+0000afc0: 6c65 2074 6f20 636f 6d70 6172 6520 746f  le to compare to
+0000afd0: 2064 6f65 7320 6e6f 7420 6578 6973 7420   does not exist 
+0000afe0: 6174 3a20 7b30 7d22 2e66 6f72 6d61 7428  at: {0}".format(
+0000aff0: 7061 7468 5f64 6566 6175 6c74 5f66 696c  path_default_fil
+0000b000: 6529 290a 0a20 2020 206e 6577 5f66 696c  e))..    new_fil
+0000b010: 655f 6e61 6d65 203d 2022 7b30 7d2d 7b31  e_name = "{0}-{1
+0000b020: 7d2e 6261 6b22 2e66 6f72 6d61 7428 6f73  }.bak".format(os
+0000b030: 2e70 6174 682e 6261 7365 6e61 6d65 2870  .path.basename(p
+0000b040: 6174 685f 6375 7272 656e 745f 6669 6c65  ath_current_file
+0000b050: 292c 2067 6574 5f74 696d 6573 7461 6d70  ), get_timestamp
+0000b060: 2829 290a 0a20 2020 2023 2049 6620 6465  ())..    # If de
+0000b070: 6661 756c 7420 6669 6c65 2070 726f 7669  fault file provi
+0000b080: 6465 642c 2063 6f6d 7061 7265 2074 6f20  ded, compare to 
+0000b090: 6375 7272 656e 7420 6669 6c65 0a20 2020  current file.   
+0000b0a0: 2069 6620 7061 7468 5f64 6566 6175 6c74   if path_default
+0000b0b0: 5f66 696c 6520 6973 206e 6f74 204e 6f6e  _file is not Non
+0000b0c0: 653a 0a20 2020 2020 2020 2023 2052 6561  e:.        # Rea
+0000b0d0: 6420 7468 6520 6465 6661 756c 7420 6669  d the default fi
+0000b0e0: 6c65 202b 2074 6865 2063 7572 7265 6e74  le + the current
+0000b0f0: 2066 696c 650a 2020 2020 2020 2020 6465   file.        de
+0000b100: 6661 756c 745f 6669 6c65 5f63 6f6e 7465  fault_file_conte
+0000b110: 6e74 7320 3d20 7265 6164 5f66 696c 6528  nts = read_file(
+0000b120: 7061 7468 5f64 6566 6175 6c74 5f66 696c  path_default_fil
+0000b130: 6529 0a20 2020 2020 2020 2063 7572 7265  e).        curre
+0000b140: 6e74 5f66 696c 655f 636f 6e74 656e 7473  nt_file_contents
+0000b150: 203d 2072 6561 645f 6669 6c65 2870 6174   = read_file(pat
+0000b160: 685f 6375 7272 656e 745f 6669 6c65 290a  h_current_file).
+0000b170: 0a20 2020 2020 2020 2023 2049 6620 6469  .        # If di
+0000b180: 6666 6572 656e 742c 2072 656e 616d 650a  fferent, rename.
+0000b190: 2020 2020 2020 2020 6966 2064 6566 6175          if defau
+0000b1a0: 6c74 5f66 696c 655f 636f 6e74 656e 7473  lt_file_contents
+0000b1b0: 2021 3d20 6375 7272 656e 745f 6669 6c65   != current_file
+0000b1c0: 5f63 6f6e 7465 6e74 733a 0a20 2020 2020  _contents:.     
+0000b1d0: 2020 2020 2020 204c 4f47 2e64 6562 7567         LOG.debug
+0000b1e0: 2822 4372 6561 7469 6e67 2061 2062 6163  ("Creating a bac
+0000b1f0: 6b75 7020 6f66 3a20 2573 222c 2070 6174  kup of: %s", pat
+0000b200: 685f 6375 7272 656e 745f 6669 6c65 290a  h_current_file).
+0000b210: 2020 2020 2020 2020 2020 2020 7265 6e61              rena
+0000b220: 6d65 5f66 696c 6528 7061 7468 5f63 7572  me_file(path_cur
+0000b230: 7265 6e74 5f66 696c 652c 206e 6577 5f66  rent_file, new_f
+0000b240: 696c 655f 6e61 6d65 290a 0a20 2020 2065  ile_name)..    e
+0000b250: 6c73 653a 0a20 2020 2020 2020 204c 4f47  lse:.        LOG
+0000b260: 2e64 6562 7567 2822 4372 6561 7469 6e67  .debug("Creating
+0000b270: 2061 2062 6163 6b75 7020 6f66 3a20 2573   a backup of: %s
+0000b280: 222c 2070 6174 685f 6375 7272 656e 745f  ", path_current_
+0000b290: 6669 6c65 290a 2020 2020 2020 2020 7265  file).        re
+0000b2a0: 6e61 6d65 5f66 696c 6528 7061 7468 5f63  name_file(path_c
+0000b2b0: 7572 7265 6e74 5f66 696c 652c 206e 6577  urrent_file, new
+0000b2c0: 5f66 696c 655f 6e61 6d65 290a 0a20 2020  _file_name)..   
+0000b2d0: 2072 6574 7572 6e20 6f73 2e70 6174 682e   return os.path.
+0000b2e0: 6a6f 696e 286f 732e 7061 7468 2e64 6972  join(os.path.dir
+0000b2f0: 6e61 6d65 2870 6174 685f 6375 7272 656e  name(path_curren
+0000b300: 745f 6669 6c65 292c 206e 6577 5f66 696c  t_file), new_fil
+0000b310: 655f 6e61 6d65 290a 0a0a 6465 6620 6765  e_name)...def ge
+0000b320: 6e65 7261 7465 5f61 6e63 686f 7228 6865  nerate_anchor(he
+0000b330: 6164 6572 293a 0a20 2020 2022 2222 0a20  ader):.    """. 
+0000b340: 2020 2043 6f6e 7665 7274 7320 6865 6164     Converts head
+0000b350: 6572 2074 6f20 6c6f 7765 7263 6173 652c  er to lowercase,
+0000b360: 2072 656d 6f76 6573 2061 6c6c 2063 6861   removes all cha
+0000b370: 7261 6374 6572 7320 6578 6365 7074 2061  racters except a
+0000b380: 2d7a 2c20 302d 392c 202d 2c0a 2020 2020  -z, 0-9, -,.    
+0000b390: 756e 6963 6f64 6520 6368 6172 6174 6572  unicode charater
+0000b3a0: 7320 7468 6174 2061 7265 2075 7365 6420  s that are used 
+0000b3b0: 696e 2077 6f72 6473 2061 6e64 2073 7061  in words and spa
+0000b3c0: 6365 7320 7468 656e 2072 6570 6c61 6365  ces then replace
+0000b3d0: 730a 2020 2020 616c 6c20 7370 6163 6573  s.    all spaces
+0000b3e0: 2077 6974 6820 2d0a 0a20 2020 2041 6e20   with -..    An 
+0000b3f0: 616e 6368 6f72 2069 7320 7573 6564 2069  anchor is used i
+0000b400: 6e20 4d61 726b 646f 776e 2054 656d 706c  n Markdown Templ
+0000b410: 6174 6573 2074 6f20 6c69 6e6b 2063 6572  ates to link cer
+0000b420: 7461 696e 2070 6172 7473 206f 6620 7468  tain parts of th
+0000b430: 6520 646f 6375 6d65 6e74 2e0a 0a20 2020  e document...   
+0000b440: 203a 7061 7261 6d20 6865 6164 6572 3a20   :param header: 
+0000b450: 5374 7269 6e67 2074 6f20 6372 6561 7465  String to create
+0000b460: 2061 6e63 686f 7220 6672 6f6d 0a20 2020   anchor from.   
+0000b470: 203a 7479 7065 2068 6561 6465 723a 2073   :type header: s
+0000b480: 7472 0a20 2020 203a 7265 7475 726e 3a20  tr.    :return: 
+0000b490: 6865 6164 6572 2066 6f72 6d61 7474 6564  header formatted
+0000b4a0: 2061 7320 616e 2061 6e63 686f 720a 2020   as an anchor.  
+0000b4b0: 2020 3a72 7479 7065 3a20 7374 720a 2020    :rtype: str.  
+0000b4c0: 2020 2222 220a 2020 2020 616e 6368 6f72    """.    anchor
+0000b4d0: 203d 2068 6561 6465 722e 6c6f 7765 7228   = header.lower(
+0000b4e0: 290a 0a20 2020 2072 6567 6578 203d 2072  )..    regex = r
+0000b4f0: 652e 636f 6d70 696c 6528 7222 5b5e 5c77  e.compile(r"[^\w
+0000b500: 5c2d 5c73 5d22 2c20 7265 2e55 290a 0a20  \-\s]", re.U).. 
+0000b510: 2020 2061 6e63 686f 7220 3d20 7265 2e73     anchor = re.s
+0000b520: 7562 2872 6567 6578 2c20 2222 2c20 616e  ub(regex, "", an
+0000b530: 6368 6f72 290a 2020 2020 616e 6368 6f72  chor).    anchor
+0000b540: 203d 2072 652e 7375 6228 7222 5b5c 735d   = re.sub(r"[\s]
+0000b550: 222c 2022 2d22 2c20 616e 6368 6f72 290a  ", "-", anchor).
+0000b560: 0a20 2020 2072 6574 7572 6e20 616e 6368  .    return anch
+0000b570: 6f72 0a0a 0a64 6566 2073 696d 706c 6966  or...def simplif
+0000b580: 795f 7374 7269 6e67 2874 6865 5f73 7472  y_string(the_str
+0000b590: 696e 6729 3a0a 2020 2020 2222 220a 2020  ing):.    """.  
+0000b5a0: 2020 5369 6d70 6c69 6669 6573 2074 6865    Simplifies the
+0000b5b0: 5f73 7472 696e 6720 6279 2063 6f6e 7665  _string by conve
+0000b5c0: 7274 696e 6720 6974 2074 6f20 6c6f 7765  rting it to lowe
+0000b5d0: 7263 6173 6573 2061 6e64 0a20 2020 2072  rcases and.    r
+0000b5e0: 656d 6f76 696e 6720 616c 6c20 6368 6172  emoving all char
+0000b5f0: 6163 7465 7273 2065 7863 6570 7420 612d  acters except a-
+0000b600: 7a2c 2030 2d39 2c20 2d20 616e 6420 7370  z, 0-9, - and sp
+0000b610: 6163 6573 2074 6865 6e0a 2020 2020 7265  aces then.    re
+0000b620: 706c 6163 6573 2061 6c6c 2073 7061 6365  places all space
+0000b630: 7320 7769 7468 202d 0a0a 2020 2020 3a70  s with -..    :p
+0000b640: 6172 616d 2074 6865 5f73 7472 696e 673a  aram the_string:
+0000b650: 2053 7472 696e 6720 746f 2073 696d 706c   String to simpl
+0000b660: 6966 790a 2020 2020 3a74 7970 6520 7468  ify.    :type th
+0000b670: 655f 7374 7269 6e67 3a20 7374 720a 2020  e_string: str.  
+0000b680: 2020 3a72 6574 7572 6e3a 2074 6865 5f73    :return: the_s
+0000b690: 7472 696e 6720 666f 726d 6174 7465 640a  tring formatted.
+0000b6a0: 2020 2020 3a72 7479 7065 3a20 7374 720a      :rtype: str.
+0000b6b0: 2020 2020 2222 220a 2020 2020 7468 655f      """.    the_
+0000b6c0: 7374 7269 6e67 203d 2074 6865 5f73 7472  string = the_str
+0000b6d0: 696e 672e 6c6f 7765 7228 290a 0a20 2020  ing.lower()..   
+0000b6e0: 2072 6567 6578 203d 2072 652e 636f 6d70   regex = re.comp
+0000b6f0: 696c 6528 7222 5b5e 612d 7a30 2d39 5c2d  ile(r"[^a-z0-9\-
+0000b700: 5c73 5f5d 2229 0a0a 2020 2020 7468 655f  \s_]")..    the_
+0000b710: 7374 7269 6e67 203d 2072 652e 7375 6228  string = re.sub(
+0000b720: 7265 6765 782c 2022 222c 2074 6865 5f73  regex, "", the_s
+0000b730: 7472 696e 6729 0a20 2020 2074 6865 5f73  tring).    the_s
+0000b740: 7472 696e 6720 3d20 7265 2e73 7562 2822  tring = re.sub("
+0000b750: 5f22 2c20 222d 222c 2074 6865 5f73 7472  _", "-", the_str
+0000b760: 696e 6729 0a20 2020 2074 6865 5f73 7472  ing).    the_str
+0000b770: 696e 6720 3d20 7265 2e73 7562 2872 225b  ing = re.sub(r"[
+0000b780: 5c73 5d22 2c20 222d 222c 2074 6865 5f73  \s]", "-", the_s
+0000b790: 7472 696e 6729 0a0a 2020 2020 7265 7475  tring)..    retu
+0000b7a0: 726e 2074 6865 5f73 7472 696e 670a 0a0a  rn the_string...
+0000b7b0: 6465 6620 6765 745f 776f 726b 666c 6f77  def get_workflow
+0000b7c0: 5f66 756e 6374 696f 6e73 2877 6f72 6b66  _functions(workf
+0000b7d0: 6c6f 772c 2066 756e 6374 696f 6e5f 7575  low, function_uu
+0000b7e0: 6964 3d4e 6f6e 6529 3a0a 2020 2020 2222  id=None):.    ""
+0000b7f0: 2250 6172 7365 7320 7468 6520 584d 4c20  "Parses the XML 
+0000b800: 6f66 2074 6865 2057 6f72 6b66 6c6f 7720  of the Workflow 
+0000b810: 4f62 6a65 6374 2061 6e64 2072 6574 7572  Object and retur
+0000b820: 6e73 0a20 2020 2061 204c 6973 7420 6f66  ns.    a List of
+0000b830: 2061 6c6c 2046 756e 6374 696f 6e73 2066   all Functions f
+0000b840: 6f75 6e64 2e20 4966 2066 756e 6374 696f  ound. If functio
+0000b850: 6e5f 7575 6964 2069 7320 6465 6669 6e65  n_uuid is define
+0000b860: 640a 2020 2020 7265 7475 726e 7320 616c  d.    returns al
+0000b870: 6c20 6f63 6375 7272 656e 6365 7320 6f66  l occurrences of
+0000b880: 2074 6861 7420 6675 6e63 7469 6f6e 2e0a   that function..
+0000b890: 0a20 2020 2041 2057 6f72 6b66 6c6f 7720  .    A Workflow 
+0000b8a0: 4675 6e63 7469 6f6e 2063 616e 2068 6176  Function can hav
+0000b8b0: 6520 7468 6520 6174 7472 6962 7574 6573  e the attributes
+0000b8c0: 3a0a 2020 2020 2d20 7575 6964 3a20 5374  :.    - uuid: St
+0000b8d0: 7269 6e67 0a20 2020 202d 2069 6e70 7574  ring.    - input
+0000b8e0: 733a 2044 6963 740a 2020 2020 2d20 706f  s: Dict.    - po
+0000b8f0: 7374 5f70 726f 6365 7373 696e 675f 7363  st_processing_sc
+0000b900: 7269 7074 3a20 5374 7269 6e67 0a20 2020  ript: String.   
+0000b910: 202d 2070 7265 5f70 726f 6365 7373 696e   - pre_processin
+0000b920: 675f 7363 7269 7074 3a20 5374 7269 6e67  g_script: String
+0000b930: 0a20 2020 202d 2072 6573 756c 745f 6e61  .    - result_na
+0000b940: 6d65 3a20 5374 7269 6e67 2222 220a 0a20  me: String""".. 
+0000b950: 2020 2072 6574 7572 6e5f 6675 6e63 7469     return_functi
+0000b960: 6f6e 7320 3d20 5b5d 0a0a 2020 2020 2320  ons = []..    # 
+0000b970: 576f 726b 666c 6f77 2058 4d4c 2074 6578  Workflow XML tex
+0000b980: 740a 2020 2020 7766 5f78 6d6c 203d 2077  t.    wf_xml = w
+0000b990: 6f72 6b66 6c6f 772e 6765 7428 2263 6f6e  orkflow.get("con
+0000b9a0: 7465 6e74 222c 207b 7d29 2e67 6574 2822  tent", {}).get("
+0000b9b0: 786d 6c22 2c20 4e6f 6e65 290a 0a20 2020  xml", None)..   
+0000b9c0: 2069 6620 7766 5f78 6d6c 2069 7320 4e6f   if wf_xml is No
+0000b9d0: 6e65 3a0a 2020 2020 2020 2020 7261 6973  ne:.        rais
+0000b9e0: 6520 5344 4b45 7863 6570 7469 6f6e 2822  e SDKException("
+0000b9f0: 436f 756c 6420 6e6f 7420 6c6f 6164 2078  Could not load x
+0000ba00: 6d6c 2063 6f6e 7465 6e74 2066 726f 6d20  ml content from 
+0000ba10: 576f 726b 666c 6f77 3a20 7b30 7d22 2e66  Workflow: {0}".f
+0000ba20: 6f72 6d61 7428 776f 726b 666c 6f77 2929  ormat(workflow))
+0000ba30: 0a0a 2020 2020 2320 4765 7420 7468 6520  ..    # Get the 
+0000ba40: 726f 6f74 2065 6c65 6d65 6e74 202b 2065  root element + e
+0000ba50: 6e64 6f64 6520 696e 2075 7466 3820 696e  ndode in utf8 in
+0000ba60: 206f 7264 6572 2074 6f20 6861 6e64 6c65   order to handle
+0000ba70: 2055 6e69 636f 6465 0a20 2020 2072 6f6f   Unicode.    roo
+0000ba80: 7420 3d20 4554 2e66 726f 6d73 7472 696e  t = ET.fromstrin
+0000ba90: 6728 7766 5f78 6d6c 2e65 6e63 6f64 6528  g(wf_xml.encode(
+0000baa0: 2275 7466 3822 2929 0a0a 2020 2020 2320  "utf8"))..    # 
+0000bab0: 4765 7420 7468 6520 7072 6566 6978 2066  Get the prefix f
+0000bac0: 6f72 2065 6163 6820 656c 656d 656e 7427  or each element'
+0000bad0: 7320 7461 670a 2020 2020 7461 675f 7072  s tag.    tag_pr
+0000bae0: 6566 6978 203d 2072 6f6f 742e 7461 672e  efix = root.tag.
+0000baf0: 7265 706c 6163 6528 2264 6566 696e 6974  replace("definit
+0000bb00: 696f 6e73 222c 2022 2229 0a0a 2020 2020  ions", "")..    
+0000bb10: 786d 6c5f 7061 7468 203d 2022 2e2f 7b30  xml_path = "./{0
+0000bb20: 7d70 726f 6365 7373 2f7b 307d 7365 7276  }process/{0}serv
+0000bb30: 6963 6554 6173 6b2f 7b30 7d65 7874 656e  iceTask/{0}exten
+0000bb40: 7369 6f6e 456c 656d 656e 7473 2f2a 222e  sionElements/*".
+0000bb50: 666f 726d 6174 2874 6167 5f70 7265 6669  format(tag_prefi
+0000bb60: 7829 0a20 2020 2074 6865 5f66 756e 6374  x).    the_funct
+0000bb70: 696f 6e5f 656c 656d 656e 7473 203d 205b  ion_elements = [
+0000bb80: 5d0a 0a20 2020 2069 6620 6675 6e63 7469  ]..    if functi
+0000bb90: 6f6e 5f75 7569 6420 6973 206e 6f74 204e  on_uuid is not N
+0000bba0: 6f6e 653a 0a20 2020 2020 2020 2078 6d6c  one:.        xml
+0000bbb0: 5f70 6174 6820 3d20 227b 307d 5b40 7575  _path = "{0}[@uu
+0000bbc0: 6964 3d27 7b31 7d27 5d22 2e66 6f72 6d61  id='{1}']".forma
+0000bbd0: 7428 786d 6c5f 7061 7468 2c20 6675 6e63  t(xml_path, func
+0000bbe0: 7469 6f6e 5f75 7569 6429 0a0a 2020 2020  tion_uuid)..    
+0000bbf0: 2020 2020 2320 4765 7420 616c 6c20 656c      # Get all el
+0000bc00: 656d 656e 7473 2061 7420 786d 6c5f 7061  ements at xml_pa
+0000bc10: 7468 2074 6861 7420 6861 7665 2074 6865  th that have the
+0000bc20: 2075 7569 6420 6f66 2074 6865 2066 756e   uuid of the fun
+0000bc30: 6374 696f 6e0a 2020 2020 2020 2020 7468  ction.        th
+0000bc40: 655f 6675 6e63 7469 6f6e 5f65 6c65 6d65  e_function_eleme
+0000bc50: 6e74 7320 3d20 726f 6f74 2e66 696e 6461  nts = root.finda
+0000bc60: 6c6c 2878 6d6c 5f70 6174 6829 0a0a 2020  ll(xml_path)..  
+0000bc70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000bc80: 7468 655f 6578 7465 6e73 696f 6e5f 656c  the_extension_el
+0000bc90: 656d 656e 7473 203d 2072 6f6f 742e 6669  ements = root.fi
+0000bca0: 6e64 616c 6c28 786d 6c5f 7061 7468 290a  ndall(xml_path).
+0000bcb0: 2020 2020 2020 2020 666f 7220 6578 7465          for exte
+0000bcc0: 6e73 696f 6e5f 656c 656d 656e 7420 696e  nsion_element in
+0000bcd0: 2074 6865 5f65 7874 656e 7369 6f6e 5f65   the_extension_e
+0000bce0: 6c65 6d65 6e74 733a 0a20 2020 2020 2020  lements:.       
+0000bcf0: 2020 2020 2069 6620 2266 756e 6374 696f       if "functio
+0000bd00: 6e22 2069 6e20 6578 7465 6e73 696f 6e5f  n" in extension_
+0000bd10: 656c 656d 656e 742e 7461 673a 0a20 2020  element.tag:.   
+0000bd20: 2020 2020 2020 2020 2020 2020 2074 6865               the
+0000bd30: 5f66 756e 6374 696f 6e5f 656c 656d 656e  _function_elemen
+0000bd40: 7473 2e61 7070 656e 6428 6578 7465 6e73  ts.append(extens
+0000bd50: 696f 6e5f 656c 656d 656e 7429 0a0a 2020  ion_element)..  
+0000bd60: 2020 2320 466f 7265 6163 6820 656c 656d    # Foreach elem
+0000bd70: 656e 7420 666f 756e 642c 206c 6f61 6420  ent found, load 
+0000bd80: 6974 2061 7320 6120 6469 6374 696f 6e61  it as a dictiona
+0000bd90: 7279 2061 6e64 2061 7070 656e 6420 746f  ry and append to
+0000bda0: 2072 6574 7572 6e20 6c69 7374 0a20 2020   return list.   
+0000bdb0: 2066 6f72 2066 6e5f 656c 656d 656e 7420   for fn_element 
+0000bdc0: 696e 2074 6865 5f66 756e 6374 696f 6e5f  in the_function_
+0000bdd0: 656c 656d 656e 7473 3a0a 2020 2020 2020  elements:.      
+0000bde0: 2020 7265 7475 726e 5f66 756e 6374 696f    return_functio
+0000bdf0: 6e20 3d20 6a73 6f6e 2e6c 6f61 6473 2866  n = json.loads(f
+0000be00: 6e5f 656c 656d 656e 742e 7465 7874 290a  n_element.text).
+0000be10: 2020 2020 2020 2020 7265 7475 726e 5f66          return_f
+0000be20: 756e 6374 696f 6e5b 2275 7569 6422 5d20  unction["uuid"] 
+0000be30: 3d20 666e 5f65 6c65 6d65 6e74 2e61 7474  = fn_element.att
+0000be40: 7269 622e 6765 7428 2275 7569 6422 2c20  rib.get("uuid", 
+0000be50: 2222 290a 2020 2020 2020 2020 7265 7475  "").        retu
+0000be60: 726e 5f66 756e 6374 696f 6e5b 2272 6573  rn_function["res
+0000be70: 756c 745f 6e61 6d65 225d 203d 2072 6574  ult_name"] = ret
+0000be80: 7572 6e5f 6675 6e63 7469 6f6e 2e67 6574  urn_function.get
+0000be90: 2822 7265 7375 6c74 5f6e 616d 6522 2c20  ("result_name", 
+0000bea0: 4e6f 6e65 290a 2020 2020 2020 2020 7265  None).        re
+0000beb0: 7475 726e 5f66 756e 6374 696f 6e5b 2270  turn_function["p
+0000bec0: 6f73 745f 7072 6f63 6573 7369 6e67 5f73  ost_processing_s
+0000bed0: 6372 6970 7422 5d20 3d20 7265 7475 726e  cript"] = return
+0000bee0: 5f66 756e 6374 696f 6e2e 6765 7428 2270  _function.get("p
+0000bef0: 6f73 745f 7072 6f63 6573 7369 6e67 5f73  ost_processing_s
+0000bf00: 6372 6970 7422 2c20 4e6f 6e65 290a 2020  cript", None).  
+0000bf10: 2020 2020 2020 7265 7475 726e 5f66 756e        return_fun
+0000bf20: 6374 696f 6e5b 2270 7265 5f70 726f 6365  ction["pre_proce
+0000bf30: 7373 696e 675f 7363 7269 7074 225d 203d  ssing_script"] =
+0000bf40: 2072 6574 7572 6e5f 6675 6e63 7469 6f6e   return_function
+0000bf50: 2e67 6574 2822 7072 655f 7072 6f63 6573  .get("pre_proces
+0000bf60: 7369 6e67 5f73 6372 6970 7422 2c20 4e6f  sing_script", No
+0000bf70: 6e65 290a 0a20 2020 2020 2020 2072 6574  ne)..        ret
+0000bf80: 7572 6e5f 6675 6e63 7469 6f6e 732e 6170  urn_functions.ap
+0000bf90: 7065 6e64 2872 6574 7572 6e5f 6675 6e63  pend(return_func
+0000bfa0: 7469 6f6e 290a 0a20 2020 2072 6574 7572  tion)..    retur
+0000bfb0: 6e20 7265 7475 726e 5f66 756e 6374 696f  n return_functio
+0000bfc0: 6e73 0a0a 0a64 6566 2067 6574 5f70 6c61  ns...def get_pla
+0000bfd0: 7962 6f6f 6b5f 6f62 6a65 6374 7328 706c  ybook_objects(pl
+0000bfe0: 6179 626f 6f6b 2c20 6675 6e63 7469 6f6e  aybook, function
+0000bff0: 5f75 7569 643d 4e6f 6e65 293a 0a20 2020  _uuid=None):.   
+0000c000: 2022 2222 5061 7273 6573 2074 6865 2058   """Parses the X
+0000c010: 4d4c 206f 6620 7468 6520 506c 6179 626f  ML of the Playbo
+0000c020: 6f6b 204f 626a 6563 7420 616e 6420 7265  ok Object and re
+0000c030: 7475 726e 730a 2020 2020 6120 4c69 7374  turns.    a List
+0000c040: 206f 6620 616c 6c20 4675 6e63 7469 6f6e   of all Function
+0000c050: 7320 616e 6420 5363 7269 7074 7320 666f  s and Scripts fo
+0000c060: 756e 642e 2054 6865 2073 6372 6970 7473  und. The scripts
+0000c070: 0a20 2020 2072 6574 7572 6e65 6420 6f6e  .    returned on
+0000c080: 6c79 2068 6173 2074 6865 2075 7569 6420  ly has the uuid 
+0000c090: 6174 7472 6962 7574 652e 2054 6869 7320  attribute. This 
+0000c0a0: 6361 6e20 6c61 7465 720a 2020 2020 6265  can later.    be
+0000c0b0: 2075 7365 6420 746f 2065 7874 7261 6374   used to extract
+0000c0c0: 2061 6c6c 2073 6372 6970 742d 7265 6c61   all script-rela
+0000c0d0: 7465 6420 696e 666f 726d 6174 696f 6e20  ted information 
+0000c0e0: 6569 7468 6572 0a20 2020 2066 6f72 6d20  either.    form 
+0000c0f0: 7468 6520 706c 6179 626f 6f6b 2065 7870  the playbook exp
+0000c100: 6f72 7420 6f72 2066 726f 6d20 676c 6f62  ort or from glob
+0000c110: 616c 2073 6372 6970 7473 2e20 4966 0a20  al scripts. If. 
+0000c120: 2020 2066 756e 6374 696f 6e5f 7575 6964     function_uuid
+0000c130: 2069 7320 6465 6669 6e65 6420 7265 7475   is defined retu
+0000c140: 726e 7320 616c 6c20 6f63 6375 7272 656e  rns all occurren
+0000c150: 6365 7320 6f66 2074 6861 740a 2020 2020  ces of that.    
+0000c160: 6675 6e63 7469 6f6e 206f 6e6c 792e 0a0a  function only...
+0000c170: 2020 2020 4675 6e63 7469 6f6e 2041 7474      Function Att
+0000c180: 7269 6275 7465 733a 0a20 2020 202d 2075  ributes:.    - u
+0000c190: 7569 643a 2053 7472 696e 670a 2020 2020  uid: String.    
+0000c1a0: 2d20 696e 7075 7473 3a20 4469 6374 0a20  - inputs: Dict. 
+0000c1b0: 2020 202d 2070 7265 5f70 726f 6365 7373     - pre_process
+0000c1c0: 696e 675f 7363 7269 7074 3a20 5374 7269  ing_script: Stri
+0000c1d0: 6e67 0a20 2020 202d 2072 6573 756c 745f  ng.    - result_
+0000c1e0: 6e61 6d65 3a20 5374 7269 6e67 0a0a 2020  name: String..  
+0000c1f0: 2020 5363 7269 7074 2041 7474 7269 6275    Script Attribu
+0000c200: 7465 733a 0a20 2020 202d 2075 7569 643a  tes:.    - uuid:
+0000c210: 2053 7472 696e 670a 2020 2020 2222 220a   String.    """.
+0000c220: 2020 2020 706c 6179 626f 6f6b 5f65 6c65      playbook_ele
+0000c230: 6d65 6e74 7320 3d20 7b22 6675 6e63 7469  ments = {"functi
+0000c240: 6f6e 7322 3a20 5b5d 2c20 2273 6372 6970  ons": [], "scrip
+0000c250: 7473 223a 205b 5d2c 2022 7375 625f 7062  ts": [], "sub_pb
+0000c260: 7322 3a20 5b5d 7d0a 0a20 2020 2023 2050  s": []}..    # P
+0000c270: 6c61 7962 6f6f 6b20 584d 4c20 7465 7874  laybook XML text
+0000c280: 0a20 2020 2070 625f 786d 6c20 3d20 706c  .    pb_xml = pl
+0000c290: 6179 626f 6f6b 2e67 6574 2822 636f 6e74  aybook.get("cont
+0000c2a0: 656e 7422 2c20 7b7d 292e 6765 7428 2278  ent", {}).get("x
+0000c2b0: 6d6c 222c 204e 6f6e 6529 0a0a 2020 2020  ml", None)..    
+0000c2c0: 6966 2070 625f 786d 6c20 6973 204e 6f6e  if pb_xml is Non
+0000c2d0: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
+0000c2e0: 2053 444b 4578 6365 7074 696f 6e28 2243   SDKException("C
+0000c2f0: 6f75 6c64 206e 6f74 206c 6f61 6420 786d  ould not load xm
+0000c300: 6c20 636f 6e74 656e 7420 6672 6f6d 2050  l content from P
+0000c310: 6c61 7962 6f6f 6b73 3a20 7b30 7d22 2e66  laybooks: {0}".f
+0000c320: 6f72 6d61 7428 706c 6179 626f 6f6b 2929  ormat(playbook))
+0000c330: 0a0a 2020 2020 2320 4765 7420 7468 6520  ..    # Get the 
+0000c340: 726f 6f74 2065 6c65 6d65 6e74 202b 2065  root element + e
+0000c350: 6e63 6f64 6564 2069 6e20 7574 6638 2069  ncoded in utf8 i
+0000c360: 6e20 6f72 6465 7220 746f 2068 616e 646c  n order to handl
+0000c370: 6520 556e 6963 6f64 650a 2020 2020 726f  e Unicode.    ro
+0000c380: 6f74 203d 2045 542e 6672 6f6d 7374 7269  ot = ET.fromstri
+0000c390: 6e67 2870 625f 786d 6c2e 656e 636f 6465  ng(pb_xml.encode
+0000c3a0: 2822 7574 6638 2229 290a 0a20 2020 2023  ("utf8"))..    #
+0000c3b0: 2047 6574 2074 6865 2070 7265 6669 7820   Get the prefix 
+0000c3c0: 666f 7220 6561 6368 2065 6c65 6d65 6e74  for each element
+0000c3d0: 2773 2074 6167 0a20 2020 2074 6167 5f70  's tag.    tag_p
+0000c3e0: 7265 6669 7820 3d20 726f 6f74 2e74 6167  refix = root.tag
+0000c3f0: 2e72 6570 6c61 6365 2822 6465 6669 6e69  .replace("defini
+0000c400: 7469 6f6e 7322 2c20 2222 290a 0a20 2020  tions", "")..   
+0000c410: 2078 6d6c 5f66 756e 6374 696f 6e5f 7061   xml_function_pa
+0000c420: 7468 203d 2022 2e2f 7b30 7d70 726f 6365  th = "./{0}proce
+0000c430: 7373 2f7b 307d 7365 7276 6963 6554 6173  ss/{0}serviceTas
+0000c440: 6b2f 7b30 7d65 7874 656e 7369 6f6e 456c  k/{0}extensionEl
+0000c450: 656d 656e 7473 2f2a 222e 666f 726d 6174  ements/*".format
+0000c460: 2874 6167 5f70 7265 6669 7829 0a20 2020  (tag_prefix).   
+0000c470: 2078 6d6c 5f73 6372 6970 745f 7061 7468   xml_script_path
+0000c480: 203d 2022 2e2f 7b30 7d70 726f 6365 7373   = "./{0}process
+0000c490: 2f7b 307d 7363 7269 7074 5461 736b 2f7b  /{0}scriptTask/{
+0000c4a0: 307d 6578 7465 6e73 696f 6e45 6c65 6d65  0}extensionEleme
+0000c4b0: 6e74 732f 2a22 2e66 6f72 6d61 7428 7461  nts/*".format(ta
+0000c4c0: 675f 7072 6566 6978 290a 2020 2020 786d  g_prefix).    xm
+0000c4d0: 6c5f 7375 625f 706c 6179 626f 6f6b 5f70  l_sub_playbook_p
+0000c4e0: 6174 6820 3d20 222e 2f7b 307d 7072 6f63  ath = "./{0}proc
+0000c4f0: 6573 732f 7b30 7d63 616c 6c41 6374 6976  ess/{0}callActiv
+0000c500: 6974 792f 7b30 7d65 7874 656e 7369 6f6e  ity/{0}extension
+0000c510: 456c 656d 656e 7473 2f2a 222e 666f 726d  Elements/*".form
+0000c520: 6174 2874 6167 5f70 7265 6669 7829 0a0a  at(tag_prefix)..
+0000c530: 2020 2020 6966 2066 756e 6374 696f 6e5f      if function_
+0000c540: 7575 6964 2069 7320 6e6f 7420 4e6f 6e65  uuid is not None
+0000c550: 3a0a 2020 2020 2020 2020 786d 6c5f 6675  :.        xml_fu
+0000c560: 6e63 7469 6f6e 5f70 6174 6820 3d20 227b  nction_path = "{
+0000c570: 307d 5b40 7575 6964 3d27 7b31 7d27 5d22  0}[@uuid='{1}']"
+0000c580: 2e66 6f72 6d61 7428 786d 6c5f 6675 6e63  .format(xml_func
+0000c590: 7469 6f6e 5f70 6174 682c 2066 756e 6374  tion_path, funct
+0000c5a0: 696f 6e5f 7575 6964 290a 0a20 2020 2020  ion_uuid)..     
+0000c5b0: 2020 2023 2047 6574 2061 6c6c 2065 6c65     # Get all ele
+0000c5c0: 6d65 6e74 7320 6174 2078 6d6c 5f70 6174  ments at xml_pat
+0000c5d0: 6820 7468 6174 2068 6176 6520 7468 6520  h that have the 
+0000c5e0: 7575 6964 206f 6620 7468 6520 6675 6e63  uuid of the func
+0000c5f0: 7469 6f6e 0a20 2020 2020 2020 2070 6c61  tion.        pla
+0000c600: 7962 6f6f 6b5f 656c 656d 656e 7473 202b  ybook_elements +
+0000c610: 3d20 726f 6f74 2e66 696e 6461 6c6c 2878  = root.findall(x
+0000c620: 6d6c 5f66 756e 6374 696f 6e5f 7061 7468  ml_function_path
+0000c630: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+0000c640: 2020 2020 2320 5061 7468 7320 746f 2066      # Paths to f
+0000c650: 756e 6374 696f 6e73 2c20 7363 7269 7074  unctions, script
+0000c660: 732c 2061 6e64 2073 7562 706c 6179 626f  s, and subplaybo
+0000c670: 6f6b 7320 696e 2074 6865 2058 4d4c 0a20  oks in the XML. 
+0000c680: 2020 2020 2020 2074 6865 5f65 7874 656e         the_exten
+0000c690: 7369 6f6e 5f65 6c65 6d65 6e74 7320 203d  sion_elements  =
+0000c6a0: 2072 6f6f 742e 6669 6e64 616c 6c28 786d   root.findall(xm
+0000c6b0: 6c5f 6675 6e63 7469 6f6e 5f70 6174 6829  l_function_path)
+0000c6c0: 0a20 2020 2020 2020 2074 6865 5f65 7874  .        the_ext
+0000c6d0: 656e 7369 6f6e 5f65 6c65 6d65 6e74 7320  ension_elements 
+0000c6e0: 2b3d 2072 6f6f 742e 6669 6e64 616c 6c28  += root.findall(
+0000c6f0: 786d 6c5f 7363 7269 7074 5f70 6174 6829  xml_script_path)
+0000c700: 0a20 2020 2020 2020 2074 6865 5f65 7874  .        the_ext
+0000c710: 656e 7369 6f6e 5f65 6c65 6d65 6e74 7320  ension_elements 
+0000c720: 2b3d 2072 6f6f 742e 6669 6e64 616c 6c28  += root.findall(
+0000c730: 786d 6c5f 7375 625f 706c 6179 626f 6f6b  xml_sub_playbook
+0000c740: 5f70 6174 6829 0a0a 2020 2020 2020 2020  _path)..        
+0000c750: 666f 7220 6578 7465 6e73 696f 6e5f 656c  for extension_el
+0000c760: 656d 656e 7420 696e 2074 6865 5f65 7874  ement in the_ext
+0000c770: 656e 7369 6f6e 5f65 6c65 6d65 6e74 733a  ension_elements:
+0000c780: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000c790: 7572 6e5f 6675 6e63 7469 6f6e 203d 207b  urn_function = {
+0000c7a0: 7d0a 2020 2020 2020 2020 2020 2020 2320  }.            # 
+0000c7b0: 4578 7472 6163 7469 6e67 2046 756e 6374  Extracting Funct
+0000c7c0: 696f 6e20 7265 6c61 7465 6420 6461 7461  ion related data
+0000c7d0: 2066 726f 6d20 7468 6520 584d 4c0a 2020   from the XML.  
+0000c7e0: 2020 2020 2020 2020 2020 6966 2022 6675            if "fu
+0000c7f0: 6e63 7469 6f6e 2220 696e 2065 7874 656e  nction" in exten
+0000c800: 7369 6f6e 5f65 6c65 6d65 6e74 2e74 6167  sion_element.tag
+0000c810: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c820: 2020 7265 7475 726e 5f66 756e 6374 696f    return_functio
+0000c830: 6e20 3d20 6a73 6f6e 2e6c 6f61 6473 2865  n = json.loads(e
+0000c840: 7874 656e 7369 6f6e 5f65 6c65 6d65 6e74  xtension_element
+0000c850: 2e74 6578 7429 0a20 2020 2020 2020 2020  .text).         
+0000c860: 2020 2020 2020 2072 6574 7572 6e5f 6675         return_fu
+0000c870: 6e63 7469 6f6e 5b22 7575 6964 225d 203d  nction["uuid"] =
+0000c880: 2065 7874 656e 7369 6f6e 5f65 6c65 6d65   extension_eleme
+0000c890: 6e74 2e61 7474 7269 622e 6765 7428 2275  nt.attrib.get("u
+0000c8a0: 7569 6422 2c20 2222 290a 2020 2020 2020  uid", "").      
+0000c8b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000c8c0: 5f66 756e 6374 696f 6e5b 2272 6573 756c  _function["resul
+0000c8d0: 745f 6e61 6d65 225d 203d 2072 6574 7572  t_name"] = retur
+0000c8e0: 6e5f 6675 6e63 7469 6f6e 2e67 6574 2822  n_function.get("
+0000c8f0: 7265 7375 6c74 5f6e 616d 6522 2c20 4e6f  result_name", No
+0000c900: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
+0000c910: 2020 2020 7265 7475 726e 5f66 756e 6374      return_funct
+0000c920: 696f 6e5b 2270 7265 5f70 726f 6365 7373  ion["pre_process
+0000c930: 696e 675f 7363 7269 7074 225d 203d 2072  ing_script"] = r
+0000c940: 6574 7572 6e5f 6675 6e63 7469 6f6e 2e67  eturn_function.g
+0000c950: 6574 2822 7072 655f 7072 6f63 6573 7369  et("pre_processi
+0000c960: 6e67 5f73 6372 6970 7422 2c20 4e6f 6e65  ng_script", None
+0000c970: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c980: 2020 706c 6179 626f 6f6b 5f65 6c65 6d65    playbook_eleme
+0000c990: 6e74 735b 2266 756e 6374 696f 6e73 225d  nts["functions"]
+0000c9a0: 2e61 7070 656e 6428 7265 7475 726e 5f66  .append(return_f
+0000c9b0: 756e 6374 696f 6e29 0a0a 2020 2020 2020  unction)..      
+0000c9c0: 2020 2020 2020 2320 4578 7472 6163 7469        # Extracti
+0000c9d0: 6e67 2053 6372 6970 7420 7265 6c61 7465  ng Script relate
+0000c9e0: 6420 6461 7461 2066 726f 6d20 7468 6520  d data from the 
+0000c9f0: 584d 4c0a 2020 2020 2020 2020 2020 2020  XML.            
+0000ca00: 6966 2022 7363 7269 7074 2220 696e 2065  if "script" in e
+0000ca10: 7874 656e 7369 6f6e 5f65 6c65 6d65 6e74  xtension_element
+0000ca20: 2e74 6167 3a0a 2020 2020 2020 2020 2020  .tag:.          
+0000ca30: 2020 2020 2020 7265 7475 726e 5f66 756e        return_fun
+0000ca40: 6374 696f 6e5b 2275 7569 6422 5d20 3d20  ction["uuid"] = 
+0000ca50: 6578 7465 6e73 696f 6e5f 656c 656d 656e  extension_elemen
+0000ca60: 742e 6765 7428 2275 7569 6422 2c20 2222  t.get("uuid", ""
+0000ca70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ca80: 2020 706c 6179 626f 6f6b 5f65 6c65 6d65    playbook_eleme
+0000ca90: 6e74 735b 2273 6372 6970 7473 225d 2e61  nts["scripts"].a
+0000caa0: 7070 656e 6428 7265 7475 726e 5f66 756e  ppend(return_fun
+0000cab0: 6374 696f 6e29 0a0a 2020 2020 2020 2020  ction)..        
+0000cac0: 2020 2020 2320 4578 7472 6163 7469 6e67      # Extracting
+0000cad0: 2053 7562 706c 6179 626f 6f6b 2072 656c   Subplaybook rel
+0000cae0: 6174 6564 2064 6174 6120 6672 6f6d 2074  ated data from t
+0000caf0: 6865 2058 4d4c 0a20 2020 2020 2020 2020  he XML.         
+0000cb00: 2020 2069 6620 2273 7562 2d70 6c61 7962     if "sub-playb
+0000cb10: 6f6f 6b22 2069 6e20 6578 7465 6e73 696f  ook" in extensio
+0000cb20: 6e5f 656c 656d 656e 742e 7461 673a 0a20  n_element.tag:. 
+0000cb30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000cb40: 7562 5f70 6220 3d20 6a73 6f6e 2e6c 6f61  ub_pb = json.loa
+0000cb50: 6473 2865 7874 656e 7369 6f6e 5f65 6c65  ds(extension_ele
+0000cb60: 6d65 6e74 2e74 6578 7429 0a20 2020 2020  ment.text).     
+0000cb70: 2020 2020 2020 2020 2020 2073 7562 5f70             sub_p
+0000cb80: 625b 2275 7569 6422 5d20 3d20 6578 7465  b["uuid"] = exte
+0000cb90: 6e73 696f 6e5f 656c 656d 656e 742e 6174  nsion_element.at
+0000cba0: 7472 6962 2e67 6574 2822 7575 6964 222c  trib.get("uuid",
+0000cbb0: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
+0000cbc0: 2020 2020 2070 6c61 7962 6f6f 6b5f 656c       playbook_el
+0000cbd0: 656d 656e 7473 5b22 7375 625f 7062 7322  ements["sub_pbs"
+0000cbe0: 5d2e 6170 7065 6e64 2873 7562 5f70 6229  ].append(sub_pb)
+0000cbf0: 0a0a 2020 2020 7265 7475 726e 2070 6c61  ..    return pla
+0000cc00: 7962 6f6f 6b5f 656c 656d 656e 7473 0a0a  ybook_elements..
+0000cc10: 0a64 6566 2072 6570 6c61 6365 5f75 7569  .def replace_uui
+0000cc20: 6473 5f69 6e5f 7375 6270 6c61 7962 6f6f  ds_in_subplayboo
+0000cc30: 6b5f 6461 7461 2870 6c61 7962 6f6f 6b5f  k_data(playbook_
+0000cc40: 6461 7461 2c20 6578 706f 7274 293a 0a20  data, export):. 
+0000cc50: 2020 2022 2222 0a20 2020 2057 6865 6e20     """.    When 
+0000cc60: 7072 6f63 6573 7369 6e67 2061 2073 7562  processing a sub
+0000cc70: 706c 6179 626f 6f6b 2077 6974 6869 6e20  playbook within 
+0000cc80: 6120 706c 6179 626f 6f6b 2c20 6974 2069  a playbook, it i
+0000cc90: 7320 706f 7373 6962 6c65 2074 6861 7420  s possible that 
+0000cca0: 7468 6572 6520 6172 650a 2020 2020 7265  there are.    re
+0000ccb0: 6665 7265 6e63 6573 2074 6f20 6f62 6a65  ferences to obje
+0000ccc0: 6374 7320 6f6e 6c79 2074 6872 6f75 6768  cts only through
+0000ccd0: 2055 5549 4473 2e20 5468 6f73 6520 6172   UUIDs. Those ar
+0000cce0: 6520 6e6f 7420 7573 6566 756c 2066 6f72  e not useful for
+0000ccf0: 0a20 2020 2067 656e 6572 6174 696e 6720  .    generating 
+0000cd00: 4d61 726b 646f 776e 2066 696c 6573 2077  Markdown files w
+0000cd10: 6865 7265 2061 2075 7365 7220 7761 6e74  here a user want
+0000cd20: 7320 746f 2072 6561 6420 7468 726f 7567  s to read throug
+0000cd30: 6820 696e 2070 6c61 696e 2074 6578 740a  h in plain text.
+0000cd40: 2020 2020 7468 6520 7661 6c75 6573 206f      the values o
+0000cd50: 6620 7468 6520 6f62 6a65 6374 7320 7265  f the objects re
+0000cd60: 6665 7265 6e63 6564 2e20 5468 6973 2066  ferenced. This f
+0000cd70: 756e 6374 696f 6e20 7265 706c 6163 6573  unction replaces
+0000cd80: 2061 6e79 2072 656c 6576 616e 740a 2020   any relevant.  
+0000cd90: 2020 5555 4944 7320 7769 7468 2074 6865    UUIDs with the
+0000cda0: 6972 2074 7275 6520 7661 6c75 6520 6672  ir true value fr
+0000cdb0: 6f6d 2074 6865 2065 7870 6f72 742e 2054  om the export. T
+0000cdc0: 6865 2072 6570 6c61 6365 6d65 6e74 2069  he replacement i
+0000cdd0: 7320 696e 2070 6c61 6365 0a0a 2020 2020  s in place..    
+0000cde0: 3a70 6172 616d 2070 6c61 7962 6f6f 6b5f  :param playbook_
+0000cdf0: 6461 7461 3a20 7375 6220 706c 6179 626f  data: sub playbo
+0000ce00: 6f6b 2074 6f20 7072 6f63 6573 730a 2020  ok to process.  
+0000ce10: 2020 3a74 7970 6520 706c 6179 626f 6f6b    :type playbook
+0000ce20: 5f64 6174 613a 2064 6963 740a 2020 2020  _data: dict.    
+0000ce30: 3a70 6172 616d 2065 7870 6f72 743a 2066  :param export: f
+0000ce40: 756c 6c20 6578 706f 7274 2064 6174 610a  ull export data.
+0000ce50: 2020 2020 3a74 7970 6520 6578 706f 7274      :type export
+0000ce60: 3a20 6469 6374 0a20 2020 2022 2222 0a0a  : dict.    """..
+0000ce70: 2020 2020 2320 6164 6420 6e61 6d65 2074      # add name t
+0000ce80: 6f20 6561 6368 2073 7562 2070 6c61 7962  o each sub playb
+0000ce90: 6f6f 6b20 696e 7075 740a 2020 2020 666f  ook input.    fo
+0000cea0: 7220 7375 625f 7062 2069 6e20 6578 706f  r sub_pb in expo
+0000ceb0: 7274 2e67 6574 2822 706c 6179 626f 6f6b  rt.get("playbook
+0000cec0: 7322 2c20 5b5d 293a 0a20 2020 2020 2020  s", []):.       
+0000ced0: 2069 6620 706c 6179 626f 6f6b 5f64 6174   if playbook_dat
+0000cee0: 612e 6765 7428 2275 7569 6422 2c20 2275  a.get("uuid", "u
+0000cef0: 7569 645f 6e6f 745f 666f 756e 645f 7062  uid_not_found_pb
+0000cf00: 2229 203d 3d20 7375 625f 7062 2e67 6574  ") == sub_pb.get
+0000cf10: 2822 7575 6964 222c 2022 7575 6964 5f6e  ("uuid", "uuid_n
+0000cf20: 6f74 5f66 6f75 6e64 5f66 6e22 293a 0a20  ot_found_fn"):. 
+0000cf30: 2020 2020 2020 2020 2020 2066 6965 6c64             field
+0000cf40: 7320 3d20 7375 625f 7062 2e67 6574 2822  s = sub_pb.get("
+0000cf50: 6669 656c 6473 5f74 7970 6522 2c20 7b7d  fields_type", {}
+0000cf60: 292e 6765 7428 2266 6965 6c64 7322 2c20  ).get("fields", 
+0000cf70: 7b7d 290a 0a20 2020 2020 2020 2020 2020  {})..           
+0000cf80: 2023 2075 7064 6174 6520 7375 6220 706c   # update sub pl
+0000cf90: 6179 626f 6f6b 2773 206e 616d 650a 2020  aybook's name.  
+0000cfa0: 2020 2020 2020 2020 2020 706c 6179 626f            playbo
+0000cfb0: 6f6b 5f64 6174 615b 226e 616d 6522 5d20  ok_data["name"] 
+0000cfc0: 3d20 7375 625f 7062 2e67 6574 2822 6469  = sub_pb.get("di
+0000cfd0: 7370 6c61 795f 6e61 6d65 2229 0a20 2020  splay_name").   
+0000cfe0: 2020 2020 2020 2020 2066 6f72 2066 6965           for fie
+0000cff0: 6c64 5f6e 616d 652c 2066 6965 6c64 2069  ld_name, field i
+0000d000: 6e20 6669 656c 6473 2e69 7465 6d73 2829  n fields.items()
+0000d010: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d020: 2020 6966 2066 6965 6c64 2e67 6574 2822    if field.get("
+0000d030: 7575 6964 222c 2022 7575 6964 5f6e 6f74  uuid", "uuid_not
+0000d040: 5f66 6f75 6e64 2229 2069 6e20 706c 6179  _found") in play
+0000d050: 626f 6f6b 5f64 6174 612e 6765 7428 2269  book_data.get("i
+0000d060: 6e70 7574 7322 2c20 7b7d 293a 0a20 2020  nputs", {}):.   
+0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d080: 2023 2063 6f6e 7665 7274 2069 6e70 7574   # convert input
+0000d090: 2075 7569 6420 746f 2069 6e70 7574 5f6e   uuid to input_n
+0000d0a0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+0000d0b0: 2020 2020 2020 2020 706c 6179 626f 6f6b          playbook
+0000d0c0: 5f64 6174 615b 2269 6e70 7574 7322 5d5b  _data["inputs"][
+0000d0d0: 6669 656c 642e 6765 7428 2275 7569 6422  field.get("uuid"
+0000d0e0: 295d 5b22 696e 7075 745f 6e61 6d65 225d  )]["input_name"]
+0000d0f0: 203d 2066 6965 6c64 2e67 6574 2822 7465   = field.get("te
+0000d100: 7874 2229 0a20 2020 2020 2020 2020 2020  xt").           
+0000d110: 2020 2020 2020 2020 2070 6c61 7962 6f6f           playboo
+0000d120: 6b5f 6461 7461 5b22 696e 7075 7473 225d  k_data["inputs"]
+0000d130: 5b66 6965 6c64 2e67 6574 2822 7575 6964  [field.get("uuid
+0000d140: 2229 5d5b 2269 6e70 7574 5f61 7069 5f6e  ")]["input_api_n
+0000d150: 616d 6522 5d20 3d20 6669 656c 645f 6e61  ame"] = field_na
+0000d160: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
+0000d170: 2020 2020 2020 2023 2061 6464 2069 6e70         # add inp
+0000d180: 7574 2074 7970 650a 2020 2020 2020 2020  ut type.        
+0000d190: 2020 2020 2020 2020 2020 2020 706c 6179              play
+0000d1a0: 626f 6f6b 5f64 6174 615b 2269 6e70 7574  book_data["input
+0000d1b0: 7322 5d5b 6669 656c 642e 6765 7428 2275  s"][field.get("u
+0000d1c0: 7569 6422 295d 5b22 696e 7075 745f 7479  uid")]["input_ty
+0000d1d0: 7065 5f6e 616d 6522 5d20 3d20 6669 656c  pe_name"] = fiel
+0000d1e0: 642e 6765 7428 2269 6e70 7574 5f74 7970  d.get("input_typ
+0000d1f0: 6522 290a 2020 2020 2020 2020 2020 2020  e").            
+0000d200: 2020 2020 2020 2020 2320 7365 6c65 6374          # select
+0000d210: 7320 616e 6420 6d75 6c74 6973 656c 6563  s and multiselec
+0000d220: 7473 2072 6566 6572 656e 6365 2074 6865  ts reference the
+0000d230: 6972 2055 5549 4420 696e 2074 6865 2064  ir UUID in the d
+0000d240: 6174 6120 6578 7472 6163 7465 6420 6672  ata extracted fr
+0000d250: 6f6d 2078 6d6c 2c0a 2020 2020 2020 2020  om xml,.        
+0000d260: 2020 2020 2020 2020 2020 2020 2320 736f              # so
+0000d270: 2077 6520 6e65 6564 2074 6f20 7265 706c   we need to repl
+0000d280: 6163 6520 7468 6174 2077 6974 6820 7468  ace that with th
+0000d290: 6520 7472 7565 2076 616c 7565 2066 6f75  e true value fou
+0000d2a0: 6e64 2069 6e20 7468 6520 7375 625f 7062  nd in the sub_pb
+0000d2b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d2c0: 2020 2020 2069 6620 6669 656c 642e 6765       if field.ge
+0000d2d0: 7428 2269 6e70 7574 5f74 7970 6522 2920  t("input_type") 
+0000d2e0: 3d3d 2022 7365 6c65 6374 223a 0a20 2020  == "select":.   
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d300: 2020 2020 2073 656c 6563 745f 696e 7075       select_inpu
+0000d310: 745f 7575 6964 203d 2070 6c61 7962 6f6f  t_uuid = playboo
+0000d320: 6b5f 6461 7461 5b22 696e 7075 7473 225d  k_data["inputs"]
+0000d330: 5b66 6965 6c64 2e67 6574 2822 7575 6964  [field.get("uuid
+0000d340: 2229 5d5b 2273 7461 7469 635f 696e 7075  ")]["static_inpu
+0000d350: 7422 5d5b 2273 656c 6563 745f 7661 6c75  t"]["select_valu
+0000d360: 6522 5d0a 2020 2020 2020 2020 2020 2020  e"].            
+0000d370: 2020 2020 2020 2020 2020 2020 706c 6179              play
+0000d380: 626f 6f6b 5f64 6174 615b 2269 6e70 7574  book_data["input
+0000d390: 7322 5d5b 6669 656c 642e 6765 7428 2275  s"][field.get("u
+0000d3a0: 7569 6422 295d 5b22 7374 6174 6963 5f69  uid")]["static_i
+0000d3b0: 6e70 7574 225d 5b22 7365 6c65 6374 5f76  nput"]["select_v
+0000d3c0: 616c 7565 225d 203d 206e 6578 7428 7661  alue"] = next(va
+0000d3d0: 6c75 652e 6765 7428 226c 6162 656c 2229  lue.get("label")
+0000d3e0: 2066 6f72 2076 616c 7565 2069 6e20 6669   for value in fi
+0000d3f0: 656c 642e 6765 7428 2276 616c 7565 7322  eld.get("values"
+0000d400: 2920 6966 2076 616c 7565 2e67 6574 2822  ) if value.get("
+0000d410: 7575 6964 2229 203d 3d20 7365 6c65 6374  uuid") == select
+0000d420: 5f69 6e70 7574 5f75 7569 6429 0a20 2020  _input_uuid).   
+0000d430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d440: 2065 6c69 6620 6669 656c 642e 6765 7428   elif field.get(
+0000d450: 2269 6e70 7574 5f74 7970 6522 2920 3d3d  "input_type") ==
+0000d460: 2022 6d75 6c74 6973 656c 6563 7422 3a0a   "multiselect":.
+0000d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d480: 2020 2020 2020 2020 7365 6c65 6374 5f69          select_i
+0000d490: 6e70 7574 5f75 7569 6473 203d 2070 6c61  nput_uuids = pla
+0000d4a0: 7962 6f6f 6b5f 6461 7461 5b22 696e 7075  ybook_data["inpu
+0000d4b0: 7473 225d 5b66 6965 6c64 2e67 6574 2822  ts"][field.get("
+0000d4c0: 7575 6964 2229 5d5b 2273 7461 7469 635f  uuid")]["static_
+0000d4d0: 696e 7075 7422 5d5b 226d 756c 7469 7365  input"]["multise
+0000d4e0: 6c65 6374 5f76 616c 7565 225d 0a20 2020  lect_value"].   
+0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d500: 2020 2020 2070 6c61 7962 6f6f 6b5f 6461       playbook_da
+0000d510: 7461 5b22 696e 7075 7473 225d 5b66 6965  ta["inputs"][fie
+0000d520: 6c64 2e67 6574 2822 7575 6964 2229 5d5b  ld.get("uuid")][
+0000d530: 2273 7461 7469 635f 696e 7075 7422 5d5b  "static_input"][
+0000d540: 226d 756c 7469 7365 6c65 6374 5f76 616c  "multiselect_val
+0000d550: 7565 225d 203d 2022 2c20 222e 6a6f 696e  ue"] = ", ".join
+0000d560: 2876 616c 7565 2e67 6574 2822 6c61 6265  (value.get("labe
+0000d570: 6c22 2920 666f 7220 7661 6c75 6520 696e  l") for value in
+0000d580: 2066 6965 6c64 2e67 6574 2822 7661 6c75   field.get("valu
+0000d590: 6573 2229 2069 6620 7661 6c75 652e 6765  es") if value.ge
+0000d5a0: 7428 2275 7569 6422 2920 696e 2073 656c  t("uuid") in sel
+0000d5b0: 6563 745f 696e 7075 745f 7575 6964 7329  ect_input_uuids)
+0000d5c0: 0a0a 2020 2020 2320 6d61 6b65 2069 6e70  ..    # make inp
+0000d5d0: 7574 2065 6173 6965 7220 746f 2067 6574  ut easier to get
+0000d5e0: 2069 6e20 6a69 6e6a 6132 0a20 2020 2066   in jinja2.    f
+0000d5f0: 6f72 205f 2c20 696e 7075 7420 696e 2070  or _, input in p
+0000d600: 6c61 7962 6f6f 6b5f 6461 7461 2e67 6574  laybook_data.get
+0000d610: 2822 696e 7075 7473 222c 207b 7d29 2e69  ("inputs", {}).i
+0000d620: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+0000d630: 696e 7075 745f 7374 725f 7265 7072 203d  input_str_repr =
+0000d640: 2022 220a 2020 2020 2020 2020 6966 2022   "".        if "
+0000d650: 6578 7072 6573 7369 6f6e 5f69 6e70 7574  expression_input
+0000d660: 2220 696e 2069 6e70 7574 3a0a 2020 2020  " in input:.    
+0000d670: 2020 2020 2020 2020 696e 7075 745f 7374          input_st
+0000d680: 725f 7265 7072 203d 2069 6e70 7574 2e67  r_repr = input.g
+0000d690: 6574 2822 6578 7072 6573 7369 6f6e 5f69  et("expression_i
+0000d6a0: 6e70 7574 222c 207b 7d29 2e67 6574 2822  nput", {}).get("
+0000d6b0: 6578 7072 6573 7369 6f6e 222c 2022 554e  expression", "UN
+0000d6c0: 4b4e 4f57 4e22 290a 2020 2020 2020 2020  KNOWN").        
+0000d6d0: 656c 6966 2022 7374 6174 6963 5f69 6e70  elif "static_inp
+0000d6e0: 7574 2220 696e 2069 6e70 7574 3a0a 2020  ut" in input:.  
+0000d6f0: 2020 2020 2020 2020 2020 696e 5f63 6f6e            in_con
+0000d700: 7465 6e74 203d 2069 6e70 7574 2e67 6574  tent = input.get
+0000d710: 2822 7374 6174 6963 5f69 6e70 7574 2229  ("static_input")
+0000d720: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
+0000d730: 6865 7265 2773 206f 6e6c 7920 6f6e 6520  here's only one 
+0000d740: 6974 656d 2065 7665 7220 696e 2069 6e5f  item ever in in_
+0000d750: 636f 6e74 656e 7420 736f 2077 6520 6361  content so we ca
+0000d760: 6e20 7573 6520 6060 6e65 7874 2829 6060  n use ``next()``
+0000d770: 0a20 2020 2020 2020 2020 2020 2023 206f  .            # o
+0000d780: 6e20 7468 6520 6765 6e65 7261 746f 7220  n the generator 
+0000d790: 6265 6c6f 7720 746f 2067 6574 2074 6865  below to get the
+0000d7a0: 2069 7465 6d27 7320 7661 6c75 650a 2020   item's value.  
+0000d7b0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
+0000d7c0: 7374 725f 7265 7072 203d 206e 6578 7428  str_repr = next(
+0000d7d0: 7661 6c75 6520 666f 7220 5f2c 2076 616c  value for _, val
+0000d7e0: 7565 2069 6e20 696e 5f63 6f6e 7465 6e74  ue in in_content
+0000d7f0: 2e69 7465 6d73 2829 290a 2020 2020 2020  .items()).      
+0000d800: 2020 696e 7075 745b 2269 6e70 7574 5f61    input["input_a
+0000d810: 735f 7374 7222 5d20 3d20 696e 7075 745f  s_str"] = input_
+0000d820: 7374 725f 7265 7072 0a0a 6465 6620 6765  str_repr..def ge
+0000d830: 745f 6d61 696e 5f63 6d64 2829 3a0a 2020  t_main_cmd():.  
+0000d840: 2020 2222 220a 2020 2020 5265 7475 726e    """.    Return
+0000d850: 2074 6865 2022 6d61 696e 2220 636f 6d6d   the "main" comm
+0000d860: 616e 6420 6672 6f6d 2074 6865 2063 6f6d  and from the com
+0000d870: 6d61 6e64 206c 696e 652e 0a0a 2020 2020  mand line...    
+0000d880: 452e 672e 2077 6974 6820 636f 6d6d 616e  E.g. with comman
+0000d890: 6420 6c69 6e65 3a20 2724 2072 6573 696c  d line: '$ resil
+0000d8a0: 6965 6e74 2d73 646b 2063 6f64 6567 656e  ient-sdk codegen
+0000d8b0: 202d 7020 6162 6327 0a20 2020 2074 6869   -p abc'.    thi
+0000d8c0: 7320 6675 6e63 7469 6f6e 2077 696c 6c20  s function will 
+0000d8d0: 7265 7475 726e 2027 636f 6465 6765 6e27  return 'codegen'
+0000d8e0: 0a20 2020 2022 2222 0a20 2020 2063 6d64  .    """.    cmd
+0000d8f0: 5f6c 696e 6520 3d20 7379 732e 6172 6776  _line = sys.argv
+0000d900: 0a0a 2020 2020 6966 206c 656e 2863 6d64  ..    if len(cmd
+0000d910: 5f6c 696e 6529 203e 2031 3a0a 2020 2020  _line) > 1:.    
+0000d920: 2020 2020 7265 7475 726e 2063 6d64 5f6c      return cmd_l
+0000d930: 696e 655b 315d 0a0a 2020 2020 7265 7475  ine[1]..    retu
+0000d940: 726e 204e 6f6e 650a 0a0a 6465 6620 6765  rn None...def ge
+0000d950: 745f 7469 6d65 7374 616d 7028 7469 6d65  t_timestamp(time
+0000d960: 7374 616d 703d 4e6f 6e65 293a 0a20 2020  stamp=None):.   
+0000d970: 2022 2222 0a20 2020 2052 6574 7572 6e73   """.    Returns
+0000d980: 2061 2073 7472 696e 6720 6f66 2074 6865   a string of the
+0000d990: 2063 7572 7265 6e74 2074 696d 650a 2020   current time.  
+0000d9a0: 2020 696e 2074 6865 2066 6f72 6d61 7420    in the format 
+0000d9b0: 5959 5959 2d4d 4d2d 4444 2d68 683a 6d6d  YYYY-MM-DD-hh:mm
+0000d9c0: 3a73 730a 0a20 2020 2049 6620 6074 696d  :ss..    If `tim
+0000d9d0: 6573 7461 6d70 6020 6973 2064 6566 696e  estamp` is defin
+0000d9e0: 6564 2c20 6974 2077 696c 6c20 7265 7475  ed, it will retu
+0000d9f0: 726e 2074 6861 7420 7469 6d65 7374 616d  rn that timestam
+0000da00: 7020 696e 0a20 2020 2074 6865 2066 6f72  p in.    the for
+0000da10: 6d61 7420 5959 5959 2d4d 4d2d 4444 2d68  mat YYYY-MM-DD-h
+0000da20: 683a 6d6d 3a73 730a 0a20 2020 203a 7061  h:mm:ss..    :pa
+0000da30: 7261 6d20 7469 6d65 7374 616d 703a 2044  ram timestamp: D
+0000da40: 6963 7469 6f6e 6172 7920 7768 6f73 6520  ictionary whose 
+0000da50: 6b65 7973 2061 7265 2066 696c 6520 6e61  keys are file na
+0000da60: 6d65 730a 2020 2020 3a74 7970 6520 7469  mes.    :type ti
+0000da70: 6d65 7374 616d 703a 2066 6c6f 6174 0a0a  mestamp: float..
+0000da80: 2020 2020 3a72 6574 7572 6e3a 2054 696d      :return: Tim
+0000da90: 6573 7461 6d70 2073 7472 696e 670a 2020  estamp string.  
+0000daa0: 2020 3a72 7479 7065 3a20 7374 720a 2020    :rtype: str.  
+0000dab0: 2020 2222 220a 2020 2020 5449 4d45 5f46    """.    TIME_F
+0000dac0: 4f52 4d41 5420 3d20 2225 5925 6d25 6425  ORMAT = "%Y%m%d%
+0000dad0: 4825 4d25 5322 0a0a 2020 2020 6966 2074  H%M%S"..    if t
+0000dae0: 696d 6573 7461 6d70 3a0a 2020 2020 2020  imestamp:.      
+0000daf0: 2020 7265 7475 726e 2064 6174 6574 696d    return datetim
+0000db00: 652e 6461 7465 7469 6d65 2e66 726f 6d74  e.datetime.fromt
+0000db10: 696d 6573 7461 6d70 2874 696d 6573 7461  imestamp(timesta
+0000db20: 6d70 292e 7374 7266 7469 6d65 2854 494d  mp).strftime(TIM
+0000db30: 455f 464f 524d 4154 290a 0a20 2020 2072  E_FORMAT)..    r
+0000db40: 6574 7572 6e20 6461 7465 7469 6d65 2e64  eturn datetime.d
+0000db50: 6174 6574 696d 652e 6e6f 7728 292e 7374  atetime.now().st
+0000db60: 7266 7469 6d65 2854 494d 455f 464f 524d  rftime(TIME_FORM
+0000db70: 4154 290a 0a0a 6465 6620 7374 725f 746f  AT)...def str_to
+0000db80: 5f62 6f6f 6c28 7661 6c75 6529 3a0a 2020  _bool(value):.  
+0000db90: 2020 2222 220a 2020 2020 5265 7072 6573    """.    Repres
+0000dba0: 656e 7473 2076 616c 7565 2061 7320 626f  ents value as bo
+0000dbb0: 6f6c 6561 6e2e 0a20 2020 203a 7061 7261  olean..    :para
+0000dbc0: 6d20 7661 6c75 653a 0a20 2020 203a 7274  m value:.    :rt
+0000dbd0: 7970 653a 2062 6f6f 6c0a 2020 2020 2222  ype: bool.    ""
+0000dbe0: 220a 2020 2020 7661 6c75 6520 3d20 7374  ".    value = st
+0000dbf0: 7228 7661 6c75 6529 2e6c 6f77 6572 2829  r(value).lower()
+0000dc00: 0a20 2020 2072 6574 7572 6e20 7661 6c75  .    return valu
+0000dc10: 6520 696e 2028 2731 272c 2027 7472 7565  e in ('1', 'true
+0000dc20: 272c 2027 7965 7327 290a 0a0a 6465 6620  ', 'yes')...def 
+0000dc30: 6973 5f65 6e76 5f76 6172 5f73 6574 2865  is_env_var_set(e
+0000dc40: 6e76 5f76 6172 293a 0a20 2020 2022 2222  nv_var):.    """
+0000dc50: 0a20 2020 203a 7265 7475 726e 3a20 5472  .    :return: Tr
+0000dc60: 7565 2f46 616c 7365 2069 6620 656e 765f  ue/False if env_
+0000dc70: 7661 7220 6973 2073 6574 2069 6e20 656e  var is set in en
+0000dc80: 7669 726f 6e6d 656e 740a 2020 2020 3a72  vironment.    :r
+0000dc90: 7479 7065 3a20 626f 6f6c 0a20 2020 2022  type: bool.    "
+0000dca0: 2222 0a20 2020 2072 6574 7572 6e20 7374  "".    return st
+0000dcb0: 725f 746f 5f62 6f6f 6c28 6f73 2e67 6574  r_to_bool(os.get
+0000dcc0: 656e 7628 656e 765f 7661 7229 290a 0a0a  env(env_var))...
+0000dcd0: 6465 6620 6765 745f 7265 7369 6c69 656e  def get_resilien
+0000dce0: 745f 6c69 6272 6172 6965 735f 7665 7273  t_libraries_vers
+0000dcf0: 696f 6e5f 746f 5f75 7365 2829 3a0a 2020  ion_to_use():.  
+0000dd00: 2020 2222 220a 2020 2020 3a72 6574 7572    """.    :retur
+0000dd10: 6e3a 2056 6572 7369 6f6e 206f 6620 7265  n: Version of re
+0000dd20: 7369 6c69 656e 742d 6369 7263 7569 7473  silient-circuits
+0000dd30: 2074 6f20 7573 6520 6465 7065 6e64 696e   to use dependin
+0000dd40: 6720 6f6e 2045 4e56 5f56 4152 5f44 4556  g on ENV_VAR_DEV
+0000dd50: 2073 6574 0a20 2020 203a 7274 7970 653a   set.    :rtype:
+0000dd60: 2073 7472 0a20 2020 2022 2222 0a20 2020   str.    """.   
+0000dd70: 2069 6620 6973 5f65 6e76 5f76 6172 5f73   if is_env_var_s
+0000dd80: 6574 2863 6f6e 7374 616e 7473 2e45 4e56  et(constants.ENV
+0000dd90: 5f56 4152 5f44 4556 293a 0a20 2020 2020  _VAR_DEV):.     
+0000dda0: 2020 2072 6574 7572 6e20 636f 6e73 7461     return consta
+0000ddb0: 6e74 732e 5245 5349 4c49 454e 545f 4c49  nts.RESILIENT_LI
+0000ddc0: 4252 4152 4945 535f 5645 5253 494f 4e5f  BRARIES_VERSION_
+0000ddd0: 4445 560a 2020 2020 656c 7365 3a0a 2020  DEV.    else:.  
+0000dde0: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
+0000ddf0: 7374 616e 7473 2e52 4553 494c 4945 4e54  stants.RESILIENT
+0000de00: 5f4c 4942 5241 5249 4553 5f56 4552 5349  _LIBRARIES_VERSI
+0000de10: 4f4e 0a0a 0a64 6566 2067 6574 5f72 6573  ON...def get_res
+0000de20: 696c 6965 6e74 5f73 646b 5f76 6572 7369  ilient_sdk_versi
+0000de30: 6f6e 2829 3a0a 2020 2020 2222 220a 2020  on():.    """.  
+0000de40: 2020 7772 6170 7065 7220 6d65 7468 6f64    wrapper method
+0000de50: 2074 6f20 6361 6c6c 2067 6574 5f70 6163   to call get_pac
+0000de60: 6b61 6765 5f76 6572 7369 6f6e 206f 6e20  kage_version on 
+0000de70: 636f 6e73 7461 6e74 2053 444b 5f50 4143  constant SDK_PAC
+0000de80: 4b41 4745 5f4e 414d 450a 0a20 2020 203a  KAGE_NAME..    :
+0000de90: 7265 7475 726e 3a20 6120 5665 7273 696f  return: a Versio
+0000dea0: 6e20 6f62 6a65 6374 0a20 2020 2022 2222  n object.    """
+0000deb0: 0a20 2020 2072 6574 7572 6e20 6765 745f  .    return get_
+0000dec0: 7061 636b 6167 655f 7665 7273 696f 6e28  package_version(
+0000ded0: 636f 6e73 7461 6e74 732e 5344 4b5f 5041  constants.SDK_PA
+0000dee0: 434b 4147 455f 4e41 4d45 290a 0a0a 6465  CKAGE_NAME)...de
+0000def0: 6620 6765 745f 7061 636b 6167 655f 7665  f get_package_ve
+0000df00: 7273 696f 6e28 7061 636b 6167 655f 6e61  rsion(package_na
+0000df10: 6d65 293a 0a20 2020 2022 2222 0a20 2020  me):.    """.   
+0000df20: 2055 7365 7320 706b 675f 7265 736f 7572   Uses pkg_resour
+0000df30: 6365 7320 746f 2070 6172 7365 2074 6865  ces to parse the
+0000df40: 2076 6572 7369 6f6e 206f 6620 6120 7061   version of a pa
+0000df50: 636b 6167 6520 6966 2069 6e73 7461 6c6c  ckage if install
+0000df60: 6564 2069 6e20 7468 6520 656e 7669 726f  ed in the enviro
+0000df70: 6e6d 656e 742e 0a20 2020 2049 6620 6e6f  nment..    If no
+0000df80: 7420 696e 7374 616c 6c65 642c 2072 6574  t installed, ret
+0000df90: 7572 6e20 4e6f 6e65 0a0a 2020 2020 3a70  urn None..    :p
+0000dfa0: 6172 616d 2070 6163 6b61 6765 5f6e 616d  aram package_nam
+0000dfb0: 653a 206e 616d 6520 6f66 2074 6865 2070  e: name of the p
+0000dfc0: 6163 6b61 6765 2074 6f20 6765 7420 7665  ackage to get ve
+0000dfd0: 7273 696f 6e20 6f66 0a20 2020 203a 7479  rsion of.    :ty
+0000dfe0: 7065 2070 6163 6b61 6765 5f6e 616d 653a  pe package_name:
+0000dff0: 2073 7472 0a20 2020 203a 7265 7475 726e   str.    :return
+0000e000: 3a20 6120 5665 7273 696f 6e20 6f62 6a65  : a Version obje
+0000e010: 6374 2072 6570 7265 7365 6e74 696e 6720  ct representing 
+0000e020: 7468 6520 7665 7273 696f 6e20 6f66 2074  the version of t
+0000e030: 6865 2067 6976 656e 2070 6163 6b61 6765  he given package
+0000e040: 206f 7220 4e6f 6e65 0a20 2020 203a 7274   or None.    :rt
+0000e050: 7970 653a 2056 6572 7369 6f6e 206f 7220  ype: Version or 
+0000e060: 4e6f 6e65 0a20 2020 2022 2222 0a20 2020  None.    """.   
+0000e070: 2074 7279 3a0a 2020 2020 2020 2020 7265   try:.        re
+0000e080: 7475 726e 2070 6172 7365 5f76 6572 7369  turn parse_versi
+0000e090: 6f6e 2870 6b67 5f72 6573 6f75 7263 6573  on(pkg_resources
+0000e0a0: 2e72 6571 7569 7265 2870 6163 6b61 6765  .require(package
+0000e0b0: 5f6e 616d 6529 5b30 5d2e 7665 7273 696f  _name)[0].versio
+0000e0c0: 6e29 0a20 2020 2065 7863 6570 7420 706b  n).    except pk
+0000e0d0: 675f 7265 736f 7572 6365 732e 4469 7374  g_resources.Dist
+0000e0e0: 7269 6275 7469 6f6e 4e6f 7446 6f75 6e64  ributionNotFound
+0000e0f0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0000e100: 204e 6f6e 650a 0a0a 6465 6620 6765 745f   None...def get_
+0000e110: 6c61 7465 7374 5f76 6572 7369 6f6e 5f6f  latest_version_o
+0000e120: 6e5f 7079 7069 2829 3a0a 2020 2020 2222  n_pypi():.    ""
+0000e130: 220a 2020 2020 5573 6573 2072 6571 7565  ".    Uses reque
+0000e140: 7374 7320 746f 2063 616c 6c20 2768 7474  sts to call 'htt
+0000e150: 7073 3a2f 2f70 7970 692e 6f72 672f 7079  ps://pypi.org/py
+0000e160: 7069 2f72 6573 696c 6965 6e74 2d73 646b  pi/resilient-sdk
+0000e170: 2f6a 736f 6e27 0a20 2020 2074 6f20 6765  /json'.    to ge
+0000e180: 7420 6120 4a53 4f4e 2064 6963 7420 6f66  t a JSON dict of
+0000e190: 2061 6c6c 2074 6865 2061 7661 696c 6162   all the availab
+0000e1a0: 6c65 2076 6572 7369 6f6e 7320 6f6e 2050  le versions on P
+0000e1b0: 7950 692e 0a20 2020 2053 6f72 7473 2074  yPi..    Sorts t
+0000e1c0: 6865 2064 6963 7420 696e 746f 2061 206c  he dict into a l
+0000e1d0: 6973 742c 2074 6865 6e20 6765 7473 2074  ist, then gets t
+0000e1e0: 6865 206c 6174 6573 740a 0a20 2020 203a  he latest..    :
+0000e1f0: 7261 6973 6573 2048 5454 5045 7272 6f72  raises HTTPError
+0000e200: 3a20 6966 2061 2070 726f 626c 656d 206f  : if a problem o
+0000e210: 6363 7572 7320 7265 6163 6869 6e67 2070  ccurs reaching p
+0000e220: 7970 692e 6f72 670a 2020 2020 3a72 6574  ypi.org.    :ret
+0000e230: 7572 6e3a 2074 6865 206c 6174 6573 7420  urn: the latest 
+0000e240: 6176 6169 6c61 626c 6520 7665 7273 696f  available versio
+0000e250: 6e20 6f66 2074 6869 7320 6c69 6272 6172  n of this librar
+0000e260: 7920 6f6e 2050 7950 690a 2020 2020 3a72  y on PyPi.    :r
+0000e270: 7479 7065 3a20 706b 675f 7265 736f 7572  type: pkg_resour
+0000e280: 6365 732e 6578 7465 726e 2e70 6163 6b61  ces.extern.packa
+0000e290: 6769 6e67 2e76 6572 7369 6f6e 2e56 6572  ging.version.Ver
+0000e2a0: 7369 6f6e 0a20 2020 2022 2222 0a20 2020  sion.    """.   
+0000e2b0: 2072 203d 2072 6571 7565 7374 732e 6765   r = requests.ge
+0000e2c0: 7428 636f 6e73 7461 6e74 732e 5552 4c5f  t(constants.URL_
+0000e2d0: 5059 5049 5f56 4552 5349 4f4e 2c20 7469  PYPI_VERSION, ti
+0000e2e0: 6d65 6f75 743d 3529 0a20 2020 2072 2e72  meout=5).    r.r
+0000e2f0: 6169 7365 5f66 6f72 5f73 7461 7475 7328  aise_for_status(
+0000e300: 290a 0a20 2020 2072 6573 5f6a 736f 6e20  )..    res_json 
+0000e310: 3d20 722e 6a73 6f6e 2829 0a0a 2020 2020  = r.json()..    
+0000e320: 6176 6169 6c61 626c 655f 7665 7273 696f  available_versio
+0000e330: 6e73 203d 205b 5d0a 0a20 2020 2066 6f72  ns = []..    for
+0000e340: 2074 6865 5f76 6572 7369 6f6e 2069 6e20   the_version in 
+0000e350: 7265 735f 6a73 6f6e 2e67 6574 2822 7265  res_json.get("re
+0000e360: 6c65 6173 6573 222c 207b 7d29 3a0a 0a20  leases", {}):.. 
+0000e370: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0000e380: 2020 2020 2020 2020 7620 3d20 7061 7273          v = pars
+0000e390: 655f 7665 7273 696f 6e28 7468 655f 7665  e_version(the_ve
+0000e3a0: 7273 696f 6e29 0a20 2020 2020 2020 2020  rsion).         
+0000e3b0: 2020 2061 7661 696c 6162 6c65 5f76 6572     available_ver
+0000e3c0: 7369 6f6e 732e 6170 7065 6e64 2876 290a  sions.append(v).
+0000e3d0: 2020 2020 2020 2020 6578 6365 7074 2049          except I
+0000e3e0: 6e76 616c 6964 5665 7273 696f 6e3a 0a20  nvalidVersion:. 
+0000e3f0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0000e400: 6e75 6520 2320 736b 6970 2069 6620 6361  nue # skip if ca
+0000e410: 6e27 7420 7061 7273 650a 0a20 2020 2061  n't parse..    a
+0000e420: 7661 696c 6162 6c65 5f76 6572 7369 6f6e  vailable_version
+0000e430: 7320 3d20 736f 7274 6564 2861 7661 696c  s = sorted(avail
+0000e440: 6162 6c65 5f76 6572 7369 6f6e 7329 0a0a  able_versions)..
+0000e450: 2020 2020 7265 7475 726e 2061 7661 696c      return avail
+0000e460: 6162 6c65 5f76 6572 7369 6f6e 735b 2d31  able_versions[-1
+0000e470: 5d0a 0a0a 6465 6620 6765 745f 6c61 7465  ]...def get_late
+0000e480: 7374 5f61 7661 696c 6162 6c65 5f76 6572  st_available_ver
+0000e490: 7369 6f6e 2829 3a0a 2020 2020 2222 220a  sion():.    """.
+0000e4a0: 2020 2020 5365 6573 2069 6620 7468 6520      Sees if the 
+0000e4b0: 6c61 7465 7374 2076 6572 7369 6f6e 2069  latest version i
+0000e4c0: 7320 7374 6f72 6564 2069 6e20 6120 746d  s stored in a tm
+0000e4d0: 7020 6669 6c65 0a20 2020 2061 6e64 2069  p file.    and i
+0000e4e0: 6620 7468 6520 6669 6c65 2069 7320 6d69  f the file is mi
+0000e4f0: 7373 696e 6720 6f72 2074 6865 2074 696d  ssing or the tim
+0000e500: 6573 7461 6d70 2069 7320 6f6c 6465 720a  estamp is older.
+0000e510: 2020 2020 7468 616e 2033 2064 6179 732c      than 3 days,
+0000e520: 2067 6574 7320 7468 6520 6c61 7465 7374   gets the latest
+0000e530: 2076 6572 7369 6f6e 2066 726f 6d20 5079   version from Py
+0000e540: 5069 0a0a 2020 2020 3a72 6574 7572 6e3a  Pi..    :return:
+0000e550: 2074 6865 206c 6174 6573 7420 6176 6169   the latest avai
+0000e560: 6c61 626c 6520 7665 7273 696f 6e20 6f66  lable version of
+0000e570: 2074 6869 7320 6c69 6272 6172 7920 6f6e   this library on
+0000e580: 2050 7950 690a 2020 2020 3a72 7479 7065   PyPi.    :rtype
+0000e590: 3a20 706b 675f 7265 736f 7572 6365 732e  : pkg_resources.
+0000e5a0: 5665 7273 696f 6e0a 2020 2020 2222 220a  Version.    """.
+0000e5b0: 2020 2020 6c61 7465 7374 5f61 7661 696c      latest_avail
+0000e5c0: 6162 6c65 5f76 6572 7369 6f6e 203d 204e  able_version = N
+0000e5d0: 6f6e 650a 0a20 2020 2073 646b 5f74 6d70  one..    sdk_tmp
+0000e5e0: 5f64 6972 203d 2067 6574 5f73 646b 5f74  _dir = get_sdk_t
+0000e5f0: 6d70 5f64 6972 2829 0a20 2020 2070 6174  mp_dir().    pat
+0000e600: 685f 7364 6b5f 746d 705f 7079 7069 5f76  h_sdk_tmp_pypi_v
+0000e610: 6572 7369 6f6e 203d 206f 732e 7061 7468  ersion = os.path
+0000e620: 2e6a 6f69 6e28 7364 6b5f 746d 705f 6469  .join(sdk_tmp_di
+0000e630: 722c 2063 6f6e 7374 616e 7473 2e54 4d50  r, constants.TMP
+0000e640: 5f50 5950 495f 5645 5253 494f 4e29 0a0a  _PYPI_VERSION)..
+0000e650: 2020 2020 6966 206f 732e 7061 7468 2e69      if os.path.i
+0000e660: 7366 696c 6528 7061 7468 5f73 646b 5f74  sfile(path_sdk_t
+0000e670: 6d70 5f70 7970 695f 7665 7273 696f 6e29  mp_pypi_version)
+0000e680: 3a0a 2020 2020 2020 2020 7079 7069 5f76  :.        pypi_v
+0000e690: 6572 7369 6f6e 5f64 6174 6120 3d20 7265  ersion_data = re
+0000e6a0: 6164 5f6a 736f 6e5f 6669 6c65 2870 6174  ad_json_file(pat
+0000e6b0: 685f 7364 6b5f 746d 705f 7079 7069 5f76  h_sdk_tmp_pypi_v
+0000e6c0: 6572 7369 6f6e 290a 0a20 2020 2020 2020  ersion)..       
+0000e6d0: 206e 6f77 203d 2064 6174 6574 696d 652e   now = datetime.
+0000e6e0: 6461 7465 7469 6d65 2e6e 6f77 2829 0a20  datetime.now(). 
+0000e6f0: 2020 2020 2020 2074 7320 3d20 6461 7465         ts = date
+0000e700: 7469 6d65 2e64 6174 6574 696d 652e 6672  time.datetime.fr
+0000e710: 6f6d 7469 6d65 7374 616d 7028 7079 7069  omtimestamp(pypi
+0000e720: 5f76 6572 7369 6f6e 5f64 6174 612e 6765  _version_data.ge
+0000e730: 7428 2274 7322 2c20 2222 2929 0a20 2020  t("ts", "")).   
+0000e740: 2020 2020 2072 6566 7265 7368 5f70 7970       refresh_pyp
+0000e750: 695f 6461 7465 203d 2074 7320 2b20 6461  i_date = ts + da
+0000e760: 7465 7469 6d65 2e74 696d 6564 656c 7461  tetime.timedelta
+0000e770: 2864 6179 733d 3329 0a0a 2020 2020 2020  (days=3)..      
+0000e780: 2020 6966 206e 6f77 203e 2072 6566 7265    if now > refre
+0000e790: 7368 5f70 7970 695f 6461 7465 3a0a 2020  sh_pypi_date:.  
+0000e7a0: 2020 2020 2020 2020 2020 6c61 7465 7374            latest
+0000e7b0: 5f61 7661 696c 6162 6c65 5f76 6572 7369  _available_versi
+0000e7c0: 6f6e 203d 2067 6574 5f6c 6174 6573 745f  on = get_latest_
+0000e7d0: 7665 7273 696f 6e5f 6f6e 5f70 7970 6928  version_on_pypi(
+0000e7e0: 290a 2020 2020 2020 2020 2020 2020 7772  ).            wr
+0000e7f0: 6974 655f 6c61 7465 7374 5f70 7970 695f  ite_latest_pypi_
+0000e800: 746d 705f 6669 6c65 286c 6174 6573 745f  tmp_file(latest_
+0000e810: 6176 6169 6c61 626c 655f 7665 7273 696f  available_versio
+0000e820: 6e2c 2070 6174 685f 7364 6b5f 746d 705f  n, path_sdk_tmp_
+0000e830: 7079 7069 5f76 6572 7369 6f6e 290a 0a20  pypi_version).. 
+0000e840: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000e850: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000e860: 7061 7273 655f 7665 7273 696f 6e28 7079  parse_version(py
+0000e870: 7069 5f76 6572 7369 6f6e 5f64 6174 612e  pi_version_data.
+0000e880: 6765 7428 2276 6572 7369 6f6e 222c 2022  get("version", "
+0000e890: 2229 290a 0a20 2020 2065 6c73 653a 0a20  "))..    else:. 
+0000e8a0: 2020 2020 2020 206c 6174 6573 745f 6176         latest_av
+0000e8b0: 6169 6c61 626c 655f 7665 7273 696f 6e20  ailable_version 
+0000e8c0: 3d20 6765 745f 6c61 7465 7374 5f76 6572  = get_latest_ver
+0000e8d0: 7369 6f6e 5f6f 6e5f 7079 7069 2829 0a20  sion_on_pypi(). 
+0000e8e0: 2020 2020 2020 2077 7269 7465 5f6c 6174         write_lat
+0000e8f0: 6573 745f 7079 7069 5f74 6d70 5f66 696c  est_pypi_tmp_fil
+0000e900: 6528 6c61 7465 7374 5f61 7661 696c 6162  e(latest_availab
+0000e910: 6c65 5f76 6572 7369 6f6e 2c20 7061 7468  le_version, path
+0000e920: 5f73 646b 5f74 6d70 5f70 7970 695f 7665  _sdk_tmp_pypi_ve
+0000e930: 7273 696f 6e29 0a0a 2020 2020 7265 7475  rsion)..    retu
+0000e940: 726e 206c 6174 6573 745f 6176 6169 6c61  rn latest_availa
+0000e950: 626c 655f 7665 7273 696f 6e0a 0a0a 6465  ble_version...de
+0000e960: 6620 6372 6561 7465 5f74 6d70 5f64 6972  f create_tmp_dir
+0000e970: 2873 646b 5f74 6d70 5f64 6972 5f6e 616d  (sdk_tmp_dir_nam
+0000e980: 653d 636f 6e73 7461 6e74 732e 5344 4b5f  e=constants.SDK_
+0000e990: 5245 534f 5552 4345 5f4e 414d 452c 2074  RESOURCE_NAME, t
+0000e9a0: 6d70 5f64 6972 3d74 656d 7066 696c 652e  mp_dir=tempfile.
+0000e9b0: 6765 7474 656d 7064 6972 2829 293a 0a20  gettempdir()):. 
+0000e9c0: 2020 2022 2222 0a20 2020 2043 6865 636b     """.    Check
+0000e9d0: 7320 6966 2075 7365 7220 6861 7320 636f  s if user has co
+0000e9e0: 7272 6563 7420 7065 726d 6973 7369 6f6e  rrect permission
+0000e9f0: 7320 7468 656e 2063 7265 6174 6573 0a20  s then creates. 
+0000ea00: 2020 2074 6865 2073 646b 5f74 6d70 5f64     the sdk_tmp_d
+0000ea10: 6972 0a0a 2020 2020 3a70 6172 616d 2073  ir..    :param s
+0000ea20: 646b 5f74 6d70 5f64 6972 5f6e 616d 653a  dk_tmp_dir_name:
+0000ea30: 2074 6865 206e 616d 6520 666f 7220 7468   the name for th
+0000ea40: 6520 6469 7220 746f 2063 7265 6174 6520  e dir to create 
+0000ea50: 696e 2074 6865 2073 7973 7465 6d27 7320  in the system's 
+0000ea60: 2f74 6d70 2066 6f6c 6465 720a 2020 2020  /tmp folder.    
+0000ea70: 3a74 7970 6520 7364 6b5f 746d 705f 6469  :type sdk_tmp_di
+0000ea80: 725f 6e61 6d65 3a20 7374 720a 2020 2020  r_name: str.    
+0000ea90: 3a70 6172 616d 2074 6d70 5f64 6972 3a20  :param tmp_dir: 
+0000eaa0: 7468 6520 7061 7468 2074 6f20 7468 6520  the path to the 
+0000eab0: 7465 6d70 2066 696c 6573 206c 6f63 6174  temp files locat
+0000eac0: 696f 6e20 6f6e 2074 6865 2073 7973 7465  ion on the syste
+0000ead0: 6d0a 2020 2020 3a74 7970 6520 746d 705f  m.    :type tmp_
+0000eae0: 6469 723a 2073 7472 0a20 2020 203a 7265  dir: str.    :re
+0000eaf0: 7475 726e 3a20 7061 7468 2074 6f20 7468  turn: path to th
+0000eb00: 6520 7364 6b5f 746d 705f 6469 720a 2020  e sdk_tmp_dir.  
+0000eb10: 2020 3a72 7479 7065 3a20 7374 720a 2020    :rtype: str.  
+0000eb20: 2020 2222 220a 2020 2020 7661 6c69 6461    """.    valida
+0000eb30: 7465 5f64 6972 5f70 6174 6873 286f 732e  te_dir_paths(os.
+0000eb40: 575f 4f4b 2c20 746d 705f 6469 7229 0a0a  W_OK, tmp_dir)..
+0000eb50: 2020 2020 7061 7468 5f73 646b 5f74 6d70      path_sdk_tmp
+0000eb60: 5f64 6972 203d 206f 732e 7061 7468 2e6a  _dir = os.path.j
+0000eb70: 6f69 6e28 746d 705f 6469 722c 2073 646b  oin(tmp_dir, sdk
+0000eb80: 5f74 6d70 5f64 6972 5f6e 616d 6529 0a0a  _tmp_dir_name)..
+0000eb90: 2020 2020 6f73 2e6d 616b 6564 6972 7328      os.makedirs(
+0000eba0: 7061 7468 5f73 646b 5f74 6d70 5f64 6972  path_sdk_tmp_dir
+0000ebb0: 290a 0a20 2020 2072 6574 7572 6e20 7061  )..    return pa
+0000ebc0: 7468 5f73 646b 5f74 6d70 5f64 6972 0a0a  th_sdk_tmp_dir..
+0000ebd0: 0a64 6566 2067 6574 5f73 646b 5f74 6d70  .def get_sdk_tmp
+0000ebe0: 5f64 6972 2873 646b 5f74 6d70 5f64 6972  _dir(sdk_tmp_dir
+0000ebf0: 5f6e 616d 653d 636f 6e73 7461 6e74 732e  _name=constants.
+0000ec00: 5344 4b5f 5245 534f 5552 4345 5f4e 414d  SDK_RESOURCE_NAM
+0000ec10: 452c 2074 6d70 5f64 6972 3d74 656d 7066  E, tmp_dir=tempf
+0000ec20: 696c 652e 6765 7474 656d 7064 6972 2829  ile.gettempdir()
+0000ec30: 293a 0a20 2020 2022 2222 0a20 2020 2047  ):.    """.    G
+0000ec40: 6574 7320 7468 6520 7061 7468 2074 6f20  ets the path to 
+0000ec50: 7468 6520 7364 6b5f 746d 705f 6469 7220  the sdk_tmp_dir 
+0000ec60: 6f72 2063 7265 6174 6573 2069 7420 6966  or creates it if
+0000ec70: 2069 7420 646f 6573 0a20 2020 206e 6f74   it does.    not
+0000ec80: 2065 7869 7374 0a0a 2020 2020 3a70 6172   exist..    :par
+0000ec90: 616d 2073 646b 5f74 6d70 5f64 6972 5f6e  am sdk_tmp_dir_n
+0000eca0: 616d 653a 2074 6865 206e 616d 6520 666f  ame: the name fo
+0000ecb0: 7220 7468 6520 6469 7220 6e6f 726d 616c  r the dir normal
+0000ecc0: 6c79 2074 6865 206e 616d 6520 6f66 2074  ly the name of t
+0000ecd0: 6865 2070 6163 6b61 6765 0a20 2020 203a  he package.    :
+0000ece0: 7479 7065 2073 646b 5f74 6d70 5f64 6972  type sdk_tmp_dir
+0000ecf0: 5f6e 616d 653a 2073 7472 0a20 2020 203a  _name: str.    :
+0000ed00: 7061 7261 6d20 746d 705f 6469 723a 2074  param tmp_dir: t
+0000ed10: 6865 2070 6174 6820 746f 2074 6865 2074  he path to the t
+0000ed20: 656d 7020 6669 6c65 7320 6c6f 6361 7469  emp files locati
+0000ed30: 6f6e 206f 6e20 7468 6520 7379 7374 656d  on on the system
+0000ed40: 0a20 2020 203a 7479 7065 2074 6d70 5f64  .    :type tmp_d
+0000ed50: 6972 3a20 7374 720a 2020 2020 3a72 6574  ir: str.    :ret
+0000ed60: 7572 6e3a 2070 6174 6820 746f 2074 6865  urn: path to the
+0000ed70: 2073 646b 5f74 6d70 5f64 6972 0a20 2020   sdk_tmp_dir.   
+0000ed80: 203a 7274 7970 653a 2073 7472 0a20 2020   :rtype: str.   
+0000ed90: 2022 2222 0a20 2020 2070 6174 685f 7364   """.    path_sd
+0000eda0: 6b5f 746d 705f 6469 7220 3d20 6f73 2e70  k_tmp_dir = os.p
+0000edb0: 6174 682e 6a6f 696e 2874 6d70 5f64 6972  ath.join(tmp_dir
+0000edc0: 2c20 7364 6b5f 746d 705f 6469 725f 6e61  , sdk_tmp_dir_na
+0000edd0: 6d65 290a 0a20 2020 2069 6620 6e6f 7420  me)..    if not 
+0000ede0: 6f73 2e70 6174 682e 6973 6469 7228 7061  os.path.isdir(pa
+0000edf0: 7468 5f73 646b 5f74 6d70 5f64 6972 293a  th_sdk_tmp_dir):
+0000ee00: 0a20 2020 2020 2020 2070 6174 685f 7364  .        path_sd
+0000ee10: 6b5f 746d 705f 6469 7220 3d20 6372 6561  k_tmp_dir = crea
+0000ee20: 7465 5f74 6d70 5f64 6972 2873 646b 5f74  te_tmp_dir(sdk_t
+0000ee30: 6d70 5f64 6972 5f6e 616d 652c 2074 6d70  mp_dir_name, tmp
+0000ee40: 5f64 6972 290a 0a20 2020 2072 6574 7572  _dir)..    retur
+0000ee50: 6e20 7061 7468 5f73 646b 5f74 6d70 5f64  n path_sdk_tmp_d
+0000ee60: 6972 0a0a 0a64 6566 2069 735f 7079 7468  ir...def is_pyth
+0000ee70: 6f6e 5f6d 696e 5f73 7570 706f 7274 6564  on_min_supported
+0000ee80: 5f76 6572 7369 6f6e 2863 7573 746f 6d5f  _version(custom_
+0000ee90: 7761 726e 696e 673d 4e6f 6e65 293a 0a20  warning=None):. 
+0000eea0: 2020 2022 2222 0a20 2020 204c 6f67 7320     """.    Logs 
+0000eeb0: 6120 5741 524e 494e 4720 6966 2074 6865  a WARNING if the
+0000eec0: 2063 7572 7265 6e74 2076 6572 7369 6f6e   current version
+0000eed0: 206f 6620 5079 7468 6f6e 2069 7320 6e6f   of Python is no
+0000eee0: 7420 3e3d 204d 494e 5f53 5550 504f 5254  t >= MIN_SUPPORT
+0000eef0: 4544 5f50 595f 5645 5253 494f 4e0a 2020  ED_PY_VERSION.  
+0000ef00: 2020 3a70 6172 616d 2063 7573 746f 6d5f    :param custom_
+0000ef10: 7761 726e 696e 673a 2061 2063 7573 746f  warning: a custo
+0000ef20: 6d20 6d65 7373 6167 6520 796f 7520 7761  m message you wa
+0000ef30: 6e74 2074 6f20 6c6f 6720 6f75 740a 2020  nt to log out.  
+0000ef40: 2020 3a74 7970 6520 6375 7374 6f6d 5f77    :type custom_w
+0000ef50: 6172 6e69 6e67 3a20 7374 720a 2020 2020  arning: str.    
+0000ef60: 3a72 6574 7572 6e3a 2061 2062 6f6f 6c65  :return: a boole
+0000ef70: 616e 2074 6f20 696e 6469 6361 7465 2069  an to indicate i
+0000ef80: 6620 6375 7272 656e 7420 7665 7273 696f  f current versio
+0000ef90: 6e20 6973 2073 7570 706f 7274 6564 206f  n is supported o
+0000efa0: 7220 6e6f 740a 2020 2020 3a72 7479 7065  r not.    :rtype
+0000efb0: 3a20 626f 6f6c 0a20 2020 2022 2222 0a20  : bool.    """. 
+0000efc0: 2020 2069 6620 7379 732e 7665 7273 696f     if sys.versio
+0000efd0: 6e5f 696e 666f 203c 2063 6f6e 7374 616e  n_info < constan
+0000efe0: 7473 2e4d 494e 5f53 5550 504f 5254 4544  ts.MIN_SUPPORTED
+0000eff0: 5f50 595f 5645 5253 494f 4e3a 0a0a 2020  _PY_VERSION:..  
+0000f000: 2020 2020 2020 6966 2063 7573 746f 6d5f        if custom_
+0000f010: 7761 726e 696e 673a 0a20 2020 2020 2020  warning:.       
+0000f020: 2020 2020 204c 4f47 2e77 6172 6e69 6e67       LOG.warning
+0000f030: 2822 5741 524e 494e 473a 2025 7322 2c20  ("WARNING: %s", 
+0000f040: 6375 7374 6f6d 5f77 6172 6e69 6e67 290a  custom_warning).
+0000f050: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000f060: 2020 2020 2020 2020 2020 204c 4f47 2e77             LOG.w
+0000f070: 6172 6e69 6e67 2822 5741 524e 494e 473a  arning("WARNING:
+0000f080: 2074 6869 7320 7061 636b 6167 6520 7368   this package sh
+0000f090: 6f75 6c64 206f 6e6c 7920 6265 2069 6e73  ould only be ins
+0000f0a0: 7461 6c6c 6564 206f 6e20 6120 5079 7468  talled on a Pyth
+0000f0b0: 6f6e 2045 6e76 6972 6f6e 6d65 6e74 203e  on Environment >
+0000f0c0: 3d20 7b30 7d2e 7b31 7d20 220a 2020 2020  = {0}.{1} ".    
 0000f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0e0: 2020 2022 616e 6420 796f 7572 2063 7572     "and your cur
-0000f0f0: 7265 6e74 2076 6572 7369 6f6e 206f 6620  rent version of 
-0000f100: 5079 7468 6f6e 2069 7320 7b32 7d2e 7b33  Python is {2}.{3
-0000f110: 7d22 2e66 6f72 6d61 7428 636f 6e73 7461  }".format(consta
-0000f120: 6e74 732e 4d49 4e5f 5355 5050 4f52 5445  nts.MIN_SUPPORTE
-0000f130: 445f 5059 5f56 4552 5349 4f4e 5b30 5d2c  D_PY_VERSION[0],
-0000f140: 2063 6f6e 7374 616e 7473 2e4d 494e 5f53   constants.MIN_S
-0000f150: 5550 504f 5254 4544 5f50 595f 5645 5253  UPPORTED_PY_VERS
-0000f160: 494f 4e5b 315d 2c20 7379 732e 7665 7273  ION[1], sys.vers
-0000f170: 696f 6e5f 696e 666f 5b30 5d2c 2073 7973  ion_info[0], sys
-0000f180: 2e76 6572 7369 6f6e 5f69 6e66 6f5b 315d  .version_info[1]
-0000f190: 2929 0a0a 2020 2020 2020 2020 7265 7475  ))..        retu
-0000f1a0: 726e 2046 616c 7365 0a0a 2020 2020 7265  rn False..    re
-0000f1b0: 7475 726e 2054 7275 650a 0a0a 6465 6620  turn True...def 
-0000f1c0: 7061 7273 655f 7665 7273 696f 6e5f 6f62  parse_version_ob
-0000f1d0: 6a65 6374 2876 6572 7369 6f6e 5f6f 626a  ject(version_obj
-0000f1e0: 293a 0a20 2020 2022 2222 0a20 2020 2050  ):.    """.    P
-0000f1f0: 6172 7365 7320 6120 5665 7273 696f 6e20  arses a Version 
-0000f200: 6f62 6a65 6374 2069 6e74 6f20 6120 7475  object into a tu
-0000f210: 706c 6520 6f66 2028 6d61 6a6f 722c 206d  ple of (major, m
-0000f220: 696e 6f72 2c20 6d69 6372 6f29 0a20 2020  inor, micro).   
-0000f230: 2073 6f20 7468 6174 2069 7420 6361 6e20   so that it can 
-0000f240: 6265 2063 6f6d 7061 7265 6420 746f 206f  be compared to o
-0000f250: 7468 6572 2074 7570 6c65 7320 6f66 2076  ther tuples of v
-0000f260: 6572 7369 6f6e 730a 0a20 2020 204d 6f73  ersions..    Mos
-0000f270: 746c 7920 7573 6564 2062 6563 6175 7365  tly used because
-0000f280: 202e 6d61 6a6f 722f 2e6d 696e 6f72 2f2e   .major/.minor/.
-0000f290: 6d69 6372 6f20 6174 7472 6962 7574 6573  micro attributes
-0000f2a0: 2061 7265 6e27 7420 6176 6169 6c61 626c   aren't availabl
-0000f2b0: 6520 696e 2070 7932 370a 0a20 2020 203a  e in py27..    :
-0000f2c0: 7061 7261 6d20 7665 7273 696f 6e5f 6f62  param version_ob
-0000f2d0: 6a3a 2061 2056 6572 7369 6f6e 206f 626a  j: a Version obj
-0000f2e0: 6563 7420 746f 2062 6520 7061 7273 6564  ect to be parsed
-0000f2f0: 0a20 2020 203a 7479 7065 2076 6572 7369  .    :type versi
-0000f300: 6f6e 5f6f 626a 3a20 5665 7273 696f 6e0a  on_obj: Version.
-0000f310: 2020 2020 3a72 6574 7572 6e3a 2028 762e      :return: (v.
-0000f320: 6d61 6a6f 722c 2076 2e6d 696e 6f72 2c20  major, v.minor, 
-0000f330: 762e 6d69 6372 6f29 2074 7570 6c65 0a20  v.micro) tuple. 
-0000f340: 2020 203a 7279 7074 653a 2028 696e 742c     :rypte: (int,
-0000f350: 2069 6e74 2c20 696e 7429 0a20 2020 2022   int, int).    "
-0000f360: 2222 0a0a 2020 2020 6966 2073 7973 2e76  ""..    if sys.v
-0000f370: 6572 7369 6f6e 5f69 6e66 6f5b 305d 203e  ersion_info[0] >
-0000f380: 3d20 333a 2023 2070 7974 686f 6e20 3320  = 3: # python 3 
+0000f0e0: 2020 2020 2261 6e64 2079 6f75 7220 6375      "and your cu
+0000f0f0: 7272 656e 7420 7665 7273 696f 6e20 6f66  rrent version of
+0000f100: 2050 7974 686f 6e20 6973 207b 327d 2e7b   Python is {2}.{
+0000f110: 337d 222e 666f 726d 6174 2863 6f6e 7374  3}".format(const
+0000f120: 616e 7473 2e4d 494e 5f53 5550 504f 5254  ants.MIN_SUPPORT
+0000f130: 4544 5f50 595f 5645 5253 494f 4e5b 305d  ED_PY_VERSION[0]
+0000f140: 2c20 636f 6e73 7461 6e74 732e 4d49 4e5f  , constants.MIN_
+0000f150: 5355 5050 4f52 5445 445f 5059 5f56 4552  SUPPORTED_PY_VER
+0000f160: 5349 4f4e 5b31 5d2c 2073 7973 2e76 6572  SION[1], sys.ver
+0000f170: 7369 6f6e 5f69 6e66 6f5b 305d 2c20 7379  sion_info[0], sy
+0000f180: 732e 7665 7273 696f 6e5f 696e 666f 5b31  s.version_info[1
+0000f190: 5d29 290a 0a20 2020 2020 2020 2072 6574  ]))..        ret
+0000f1a0: 7572 6e20 4661 6c73 650a 0a20 2020 2072  urn False..    r
+0000f1b0: 6574 7572 6e20 5472 7565 0a0a 0a64 6566  eturn True...def
+0000f1c0: 2070 6172 7365 5f76 6572 7369 6f6e 5f6f   parse_version_o
+0000f1d0: 626a 6563 7428 7665 7273 696f 6e5f 6f62  bject(version_ob
+0000f1e0: 6a29 3a0a 2020 2020 2222 220a 2020 2020  j):.    """.    
+0000f1f0: 5061 7273 6573 2061 2056 6572 7369 6f6e  Parses a Version
+0000f200: 206f 626a 6563 7420 696e 746f 2061 2074   object into a t
+0000f210: 7570 6c65 206f 6620 286d 616a 6f72 2c20  uple of (major, 
+0000f220: 6d69 6e6f 722c 206d 6963 726f 290a 2020  minor, micro).  
+0000f230: 2020 736f 2074 6861 7420 6974 2063 616e    so that it can
+0000f240: 2062 6520 636f 6d70 6172 6564 2074 6f20   be compared to 
+0000f250: 6f74 6865 7220 7475 706c 6573 206f 6620  other tuples of 
+0000f260: 7665 7273 696f 6e73 0a0a 2020 2020 4d6f  versions..    Mo
+0000f270: 7374 6c79 2075 7365 6420 6265 6361 7573  stly used becaus
+0000f280: 6520 2e6d 616a 6f72 2f2e 6d69 6e6f 722f  e .major/.minor/
+0000f290: 2e6d 6963 726f 2061 7474 7269 6275 7465  .micro attribute
+0000f2a0: 7320 6172 656e 2774 2061 7661 696c 6162  s aren't availab
+0000f2b0: 6c65 2069 6e20 7079 3237 0a0a 2020 2020  le in py27..    
+0000f2c0: 3a70 6172 616d 2076 6572 7369 6f6e 5f6f  :param version_o
+0000f2d0: 626a 3a20 6120 5665 7273 696f 6e20 6f62  bj: a Version ob
+0000f2e0: 6a65 6374 2074 6f20 6265 2070 6172 7365  ject to be parse
+0000f2f0: 640a 2020 2020 3a74 7970 6520 7665 7273  d.    :type vers
+0000f300: 696f 6e5f 6f62 6a3a 2056 6572 7369 6f6e  ion_obj: Version
+0000f310: 0a20 2020 203a 7265 7475 726e 3a20 2876  .    :return: (v
+0000f320: 2e6d 616a 6f72 2c20 762e 6d69 6e6f 722c  .major, v.minor,
+0000f330: 2076 2e6d 6963 726f 2920 7475 706c 650a   v.micro) tuple.
+0000f340: 2020 2020 3a72 7970 7465 3a20 2869 6e74      :rypte: (int
+0000f350: 2c20 696e 742c 2069 6e74 290a 2020 2020  , int, int).    
+0000f360: 2222 220a 0a20 2020 2069 6620 7379 732e  """..    if sys.
+0000f370: 7665 7273 696f 6e5f 696e 666f 5b30 5d20  version_info[0] 
+0000f380: 3e3d 2033 3a20 2320 7079 7468 6f6e 2033  >= 3: # python 3
 0000f390: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
 0000f3a0: 2876 6572 7369 6f6e 5f6f 626a 2e6d 616a  (version_obj.maj
 0000f3b0: 6f72 2c20 7665 7273 696f 6e5f 6f62 6a2e  or, version_obj.
 0000f3c0: 6d69 6e6f 722c 2076 6572 7369 6f6e 5f6f  minor, version_o
 0000f3d0: 626a 2e6d 6963 726f 290a 2020 2020 656c  bj.micro).    el
 0000f3e0: 7365 3a20 2320 7079 7468 6f6e 2032 2e37  se: # python 2.7
 0000f3f0: 0a20 2020 2020 2020 206d 616a 6f72 5f6d  .        major_m
 0000f400: 696e 6f72 5f6d 6963 726f 203d 2074 7570  inor_micro = tup
 0000f410: 6c65 2869 6e74 2869 2920 666f 7220 6920  le(int(i) for i 
 0000f420: 696e 2073 7472 2876 6572 7369 6f6e 5f6f  in str(version_o
 0000f430: 626a 292e 7370 6c69 7428 222e 2229 290a  bj).split(".")).
-0000f440: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0000f450: 2023 2069 6620 7665 7273 696f 6e20 6973   # if version is
-0000f460: 206f 6e6c 7920 6f6e 6520 6e75 6d62 6572   only one number
-0000f470: 2028 692e 652e 2027 3327 292c 2074 6865   (i.e. '3'), the
-0000f480: 6e20 6164 6420 6120 3020 746f 2074 6865  n add a 0 to the
-0000f490: 2065 6e64 0a20 2020 2020 2020 2069 6620   end.        if 
-0000f4a0: 6c65 6e28 6d61 6a6f 725f 6d69 6e6f 725f  len(major_minor_
-0000f4b0: 6d69 6372 6f29 203d 3d20 313a 0a20 2020  micro) == 1:.   
-0000f4c0: 2020 2020 2020 2020 206d 616a 6f72 5f6d           major_m
-0000f4d0: 696e 6f72 5f6d 6963 726f 203d 2028 6d61  inor_micro = (ma
-0000f4e0: 6a6f 725f 6d69 6e6f 725f 6d69 6372 6f5b  jor_minor_micro[
-0000f4f0: 305d 2c20 302c 2030 290a 2020 2020 2020  0], 0, 0).      
-0000f500: 2020 656c 6966 206c 656e 286d 616a 6f72    elif len(major
-0000f510: 5f6d 696e 6f72 5f6d 6963 726f 2920 3d3d  _minor_micro) ==
-0000f520: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-0000f530: 6d61 6a6f 725f 6d69 6e6f 725f 6d69 6372  major_minor_micr
-0000f540: 6f20 3d20 286d 616a 6f72 5f6d 696e 6f72  o = (major_minor
-0000f550: 5f6d 6963 726f 5b30 5d2c 206d 616a 6f72  _micro[0], major
-0000f560: 5f6d 696e 6f72 5f6d 6963 726f 5b31 5d2c  _minor_micro[1],
-0000f570: 2030 290a 2020 2020 2020 2020 7265 7475   0).        retu
-0000f580: 726e 206d 616a 6f72 5f6d 696e 6f72 5f6d  rn major_minor_m
-0000f590: 6963 726f 0a0a 6465 6620 7061 7273 655f  icro..def parse_
-0000f5a0: 6f70 7469 6f6e 616c 7328 6f70 7469 6f6e  optionals(option
-0000f5b0: 616c 7329 3a0a 2020 2020 2222 220a 2020  als):.    """.  
-0000f5c0: 2020 5265 7475 726e 7320 616c 6c20 6f70    Returns all op
-0000f5d0: 7469 6f6e 616c 7320 6173 2061 2066 6f72  tionals as a for
-0000f5e0: 6d61 7474 6564 2073 7472 696e 670a 2020  matted string.  
-0000f5f0: 2020 7769 7468 2074 6865 206e 756d 6265    with the numbe
-0000f600: 7220 6f66 2074 6162 7320 7573 6564 2064  r of tabs used d
-0000f610: 6570 656e 6469 6e67 0a20 2020 206f 6e20  epending.    on 
-0000f620: 7468 6520 6c65 6e67 7468 0a0a 2020 2020  the length..    
-0000f630: 4d61 696e 6c79 2075 7365 6420 746f 2068  Mainly used to h
-0000f640: 656c 7020 6275 696c 6420 6f75 7220 646f  elp build our do
-0000f650: 6373 0a0a 2020 2020 3a70 6172 616d 206f  cs..    :param o
-0000f660: 7074 696f 6e61 6c73 3a20 4c69 7374 206f  ptionals: List o
-0000f670: 6620 4172 6775 6d65 6e74 5061 7273 6572  f ArgumentParser
-0000f680: 206f 7074 696f 6e61 6c73 0a20 2020 203a   optionals.    :
-0000f690: 7479 7065 206f 7074 696f 6e61 6c73 3a20  type optionals: 
-0000f6a0: 6c69 7374 0a20 2020 203a 7265 7475 726e  list.    :return
-0000f6b0: 3a20 466f 726d 6174 7465 6420 7374 7269  : Formatted stri
-0000f6c0: 6e67 0a20 2020 203a 7274 7970 653a 2073  ng.    :rtype: s
-0000f6d0: 7472 0a20 2020 2022 2222 0a20 2020 2070  tr.    """.    p
-0000f6e0: 6172 7365 645f 6f70 7469 6f6e 616c 7320  arsed_optionals 
-0000f6f0: 3d20 5b5d 0a0a 2020 2020 666f 7220 6f70  = []..    for op
-0000f700: 7469 6f6e 2069 6e20 6f70 7469 6f6e 616c  tion in optional
-0000f710: 733a 0a0a 2020 2020 2020 2020 2320 736b  s:..        # sk
-0000f720: 6970 7065 6420 616e 7920 7375 7070 7265  ipped any suppre
-0000f730: 7373 6564 206f 7074 696f 6e73 0a20 2020  ssed options.   
-0000f740: 2020 2020 2069 6620 6f70 7469 6f6e 2e68       if option.h
-0000f750: 656c 7020 3d3d 2053 5550 5052 4553 533a  elp == SUPPRESS:
-0000f760: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-0000f770: 7469 6e75 650a 0a20 2020 2020 2020 206f  tinue..        o
-0000f780: 7074 696f 6e5f 7374 7269 6e67 7320 3d20  ption_strings = 
-0000f790: 222c 2022 2e6a 6f69 6e28 6f70 7469 6f6e  ", ".join(option
-0000f7a0: 2e6f 7074 696f 6e5f 7374 7269 6e67 7329  .option_strings)
-0000f7b0: 0a0a 2020 2020 2020 2020 7461 6273 203d  ..        tabs =
-0000f7c0: 2022 5c74 5c74 5c74 220a 0a20 2020 2020   "\t\t\t"..     
-0000f7d0: 2020 2069 6620 6c65 6e28 6f70 7469 6f6e     if len(option
-0000f7e0: 5f73 7472 696e 6773 2920 3e3d 2031 363a  _strings) >= 16:
-0000f7f0: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-0000f800: 7320 3d20 225c 745c 7422 0a0a 2020 2020  s = "\t\t"..    
-0000f810: 2020 2020 6966 206c 656e 286f 7074 696f      if len(optio
-0000f820: 6e5f 7374 7269 6e67 7329 203e 3d20 3232  n_strings) >= 22
-0000f830: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
-0000f840: 6273 203d 2022 5c74 220a 0a20 2020 2020  bs = "\t"..     
-0000f850: 2020 2069 6620 6c65 6e28 6f70 7469 6f6e     if len(option
-0000f860: 5f73 7472 696e 6773 2920 3c20 3130 3a0a  _strings) < 10:.
-0000f870: 2020 2020 2020 2020 2020 2020 7461 6273              tabs
-0000f880: 203d 2022 5c74 5c74 5c74 5c74 220a 0a20   = "\t\t\t\t".. 
-0000f890: 2020 2020 2020 2069 6620 6c65 6e28 6f70         if len(op
-0000f8a0: 7469 6f6e 5f73 7472 696e 6773 2920 696e  tion_strings) in
-0000f8b0: 2028 382c 2039 293a 0a20 2020 2020 2020   (8, 9):.       
-0000f8c0: 2020 2020 2074 6162 7320 3d20 225c 745c       tabs = "\t\
-0000f8d0: 745c 7422 0a0a 2020 2020 2020 2020 7061  t\t"..        pa
-0000f8e0: 7273 6564 5f6f 7074 696f 6e61 6c73 2e61  rsed_optionals.a
-0000f8f0: 7070 656e 6428 227b 307d 7b31 7d7b 327d  ppend("{0}{1}{2}
-0000f900: 222e 666f 726d 6174 286f 7074 696f 6e5f  ".format(option_
-0000f910: 7374 7269 6e67 732c 2074 6162 732c 206f  strings, tabs, o
-0000f920: 7074 696f 6e2e 6865 6c70 2929 0a0a 2020  ption.help))..  
-0000f930: 2020 7061 7273 6564 5f6f 7074 696f 6e61    parsed_optiona
-0000f940: 6c73 203d 2022 205c 6e20 222e 6a6f 696e  ls = " \n ".join
-0000f950: 2870 6172 7365 645f 6f70 7469 6f6e 616c  (parsed_optional
-0000f960: 7329 0a20 2020 2070 6172 7365 645f 6f70  s).    parsed_op
-0000f970: 7469 6f6e 616c 7320 3d20 277b 307d 205c  tionals = '{0} \
-0000f980: 6e27 2e66 6f72 6d61 7428 7061 7273 6564  n'.format(parsed
-0000f990: 5f6f 7074 696f 6e61 6c73 290a 0a20 2020  _optionals)..   
-0000f9a0: 2072 6574 7572 6e20 7061 7273 6564 5f6f   return parsed_o
-0000f9b0: 7074 696f 6e61 6c73 0a0a 0a64 6566 2072  ptionals...def r
-0000f9c0: 756e 5f73 7562 7072 6f63 6573 7328 6172  un_subprocess(ar
-0000f9d0: 6773 2c20 6368 616e 6765 5f64 6972 3d4e  gs, change_dir=N
-0000f9e0: 6f6e 652c 2063 6d64 5f6e 616d 653d 2222  one, cmd_name=""
-0000f9f0: 2c20 6c6f 675f 6c65 7665 6c5f 7468 7265  , log_level_thre
-0000fa00: 7368 6f6c 643d 6c6f 6767 696e 672e 4445  shold=logging.DE
-0000fa10: 4255 4729 3a0a 2020 2020 2222 220a 2020  BUG):.    """.  
-0000fa20: 2020 5275 6e20 6120 6769 7665 6e20 636f    Run a given co
-0000fa30: 6d6d 616e 6420 6173 2061 2073 7562 7072  mmand as a subpr
-0000fa40: 6f63 6573 732e 204f 7074 696f 6e61 6c6c  ocess. Optionall
-0000fa50: 7920 6368 616e 6765 2064 6972 6563 746f  y change directo
-0000fa60: 7279 2062 6566 6f72 6520 7275 6e6e 696e  ry before runnin
-0000fa70: 6720 7468 6520 636f 6d6d 616e 6420 2875  g the command (u
-0000fa80: 7365 2063 6861 6e67 655f 6469 7220 7061  se change_dir pa
-0000fa90: 7261 6d65 7465 7229 0a0a 2020 2020 3a70  rameter)..    :p
-0000faa0: 6172 616d 2061 7267 733a 2028 7265 7175  aram args: (requ
-0000fab0: 6972 6564 2920 6172 6773 2073 686f 756c  ired) args shoul
-0000fac0: 6420 6265 2061 2073 6571 7565 6e63 6520  d be a sequence 
-0000fad0: 6f66 2070 726f 6772 616d 2061 7267 756d  of program argum
-0000fae0: 656e 7473 206f 7220 656c 7365 2061 2073  ents or else a s
-0000faf0: 696e 676c 6520 7374 7269 6e67 2028 7365  ingle string (se
-0000fb00: 6520 7375 6270 726f 6365 7373 2e50 6f70  e subprocess.Pop
-0000fb10: 656e 2066 6f72 206d 6f72 6520 6465 7461  en for more deta
-0000fb20: 696c 7329 0a20 2020 203a 7479 7065 2061  ils).    :type a
-0000fb30: 7267 733a 2073 7472 207c 206c 6973 745b  rgs: str | list[
-0000fb40: 7374 725d 0a20 2020 203a 7061 7261 6d20  str].    :param 
-0000fb50: 6368 616e 6765 5f64 6972 3a20 286f 7074  change_dir: (opt
-0000fb60: 696f 6e61 6c29 2070 6174 6820 6f66 2064  ional) path of d
-0000fb70: 6972 6563 746f 7279 2074 6f20 6368 616e  irectory to chan
-0000fb80: 6765 2074 6f20 6265 666f 7265 2072 756e  ge to before run
-0000fb90: 6e69 6e67 2063 6f6d 6d61 6e64 0a20 2020  ning command.   
-0000fba0: 203a 7479 7065 2063 6861 6e67 655f 6469   :type change_di
-0000fbb0: 723a 2073 7472 0a20 2020 203a 7061 7261  r: str.    :para
-0000fbc0: 6d20 636d 645f 6e61 6d65 3a20 286f 7074  m cmd_name: (opt
-0000fbd0: 696f 6e61 6c29 2074 6865 206e 616d 6520  ional) the name 
-0000fbe0: 6f66 2074 6865 2063 6f6d 6d61 6e64 2074  of the command t
-0000fbf0: 6f20 7275 6e20 6173 2061 2073 7562 7072  o run as a subpr
-0000fc00: 6f63 6573 732e 2077 696c 6c20 6265 2075  ocess. will be u
-0000fc10: 7365 6420 746f 206c 6f67 2069 6e20 7468  sed to log in th
-0000fc20: 6520 666f 726d 6174 2022 5275 6e6e 696e  e format "Runnin
-0000fc30: 6720 3c63 6d64 5f6e 616d 653e 202e 2e2e  g <cmd_name> ...
-0000fc40: 220a 2020 2020 3a74 7970 6520 636d 645f  ".    :type cmd_
-0000fc50: 6e61 6d65 3a20 7374 720a 2020 2020 3a70  name: str.    :p
-0000fc60: 6172 616d 206c 6f67 5f6c 6576 656c 5f74  aram log_level_t
-0000fc70: 6872 6573 686f 6c64 3a20 286f 7074 696f  hreshold: (optio
-0000fc80: 6e61 6c29 2074 6865 206c 6f67 6769 6e67  nal) the logging
-0000fc90: 206c 6576 656c 2061 7420 7768 6963 6820   level at which 
-0000fca0: 746f 206f 7574 7075 7420 7468 6520 7374  to output the st
-0000fcb0: 646f 7574 2f73 7464 6572 7220 666f 7220  dout/stderr for 
-0000fcc0: 7468 6520 7375 6270 726f 6365 7373 3b20  the subprocess; 
-0000fcd0: 6465 6661 756c 7420 6973 2044 4542 5547  default is DEBUG
-0000fce0: 0a20 2020 203a 7479 7065 206c 6f67 5f6c  .    :type log_l
-0000fcf0: 6576 656c 5f74 6872 6573 686f 6c64 3a20  evel_threshold: 
-0000fd00: 696e 740a 2020 2020 3a72 6574 7572 6e3a  int.    :return:
-0000fd10: 2074 6865 2065 7869 7420 636f 6465 2061   the exit code a
-0000fd20: 6e64 2073 7472 696e 6720 6465 7461 696c  nd string detail
-0000fd30: 7320 6f66 2074 6865 2072 756e 0a20 2020  s of the run.   
-0000fd40: 203a 7274 7970 653a 2028 696e 742c 2073   :rtype: (int, s
-0000fd50: 7472 290a 2020 2020 2222 220a 0a20 2020  tr).    """..   
-0000fd60: 204c 4f47 2e64 6562 7567 2822 5275 6e6e   LOG.debug("Runn
-0000fd70: 696e 6720 7b30 7d20 6173 2061 2073 7562  ing {0} as a sub
-0000fd80: 7072 6f63 6573 7322 2e66 6f72 6d61 7428  process".format(
-0000fd90: 6172 6773 2929 0a0a 2020 2020 2320 7361  args))..    # sa
-0000fda0: 7665 2073 7461 7274 696e 6720 6469 7265  ve starting dire
-0000fdb0: 6374 6f72 790a 2020 2020 6375 7272 656e  ctory.    curren
-0000fdc0: 745f 6469 7220 3d20 6f73 2e67 6574 6377  t_dir = os.getcw
-0000fdd0: 6428 290a 0a20 2020 2023 2069 6620 6368  d()..    # if ch
-0000fde0: 616e 6765 5f64 6972 2069 7320 7365 742c  ange_dir is set,
-0000fdf0: 2063 6861 6e67 6520 746f 2074 6861 7420   change to that 
-0000fe00: 6469 720a 2020 2020 6966 2063 6861 6e67  dir.    if chang
-0000fe10: 655f 6469 723a 0a20 2020 2020 2020 204c  e_dir:.        L
-0000fe20: 4f47 2e64 6562 7567 2822 4368 616e 6769  OG.debug("Changi
-0000fe30: 6e67 2064 6972 6563 746f 7279 2074 6f20  ng directory to 
-0000fe40: 7b30 7d22 2e66 6f72 6d61 7428 6368 616e  {0}".format(chan
-0000fe50: 6765 5f64 6972 2929 0a20 2020 2020 2020  ge_dir)).       
-0000fe60: 206f 732e 6368 6469 7228 6368 616e 6765   os.chdir(change
-0000fe70: 5f64 6972 290a 0a20 2020 2069 6620 6973  _dir)..    if is
-0000fe80: 696e 7374 616e 6365 2861 7267 732c 2073  instance(args, s
-0000fe90: 7472 293a 0a20 2020 2020 2020 2061 7267  tr):.        arg
-0000fea0: 7320 3d20 7368 6c65 782e 7370 6c69 7428  s = shlex.split(
-0000feb0: 6172 6773 290a 0a20 2020 2023 2072 756e  args)..    # run
-0000fec0: 2067 6976 656e 2063 6f6d 6d61 6e64 2061   given command a
-0000fed0: 7320 6120 7375 6270 726f 6365 7373 0a20  s a subprocess. 
-0000fee0: 2020 2070 726f 6320 3d20 7375 6270 726f     proc = subpro
-0000fef0: 6365 7373 2e50 6f70 656e 2861 7267 732c  cess.Popen(args,
-0000ff00: 2073 7464 6572 723d 7375 6270 726f 6365   stderr=subproce
-0000ff10: 7373 2e53 5444 4f55 542c 2073 7464 6f75  ss.STDOUT, stdou
-0000ff20: 743d 7375 6270 726f 6365 7373 2e50 4950  t=subprocess.PIP
-0000ff30: 452c 2062 7566 7369 7a65 3d30 290a 0a20  E, bufsize=0).. 
-0000ff40: 2020 2073 7973 2e73 7464 6f75 742e 7772     sys.stdout.wr
-0000ff50: 6974 6528 2252 756e 6e69 6e67 207b 307d  ite("Running {0}
-0000ff60: 2028 7468 6973 206d 6179 2074 616b 6520   (this may take 
-0000ff70: 6120 7768 696c 6529 202e 2e2e 222e 666f  a while) ...".fo
-0000ff80: 726d 6174 2863 6d64 5f6e 616d 6529 290a  rmat(cmd_name)).
-0000ff90: 2020 2020 7379 732e 7374 646f 7574 2e66      sys.stdout.f
-0000ffa0: 6c75 7368 2829 0a0a 2020 2020 2320 6966  lush()..    # if
-0000ffb0: 2064 6562 7567 6769 6e67 2065 6e61 626c   debugging enabl
-0000ffc0: 6564 2c20 6361 7074 7572 6520 6f75 7470  ed, capture outp
-0000ffd0: 7574 2064 6972 6563 746c 7920 616e 6420  ut directly and 
-0000ffe0: 7265 6469 7265 6374 2062 6163 6b20 746f  redirect back to
-0000fff0: 2073 7973 2e73 7464 6f75 740a 2020 2020   sys.stdout.    
-00010000: 2320 7573 696e 6720 4c4f 472e 6c6f 6728  # using LOG.log(
-00010010: 6c6f 675f 6c65 7665 6c2e 2e2e 290a 2020  log_level...).  
-00010020: 2020 6966 204c 4f47 2e69 7345 6e61 626c    if LOG.isEnabl
-00010030: 6564 466f 7228 6c6f 675f 6c65 7665 6c5f  edFor(log_level_
-00010040: 7468 7265 7368 6f6c 6429 3a0a 2020 2020  threshold):.    
-00010050: 2020 2020 4c4f 472e 6465 6275 6728 2222      LOG.debug(""
-00010060: 290a 2020 2020 2020 2020 6465 7461 696c  ).        detail
-00010070: 7320 3d20 2222 0a20 2020 2020 2020 2077  s = "".        w
-00010080: 6869 6c65 2070 726f 632e 7374 646f 7574  hile proc.stdout
-00010090: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
-000100a0: 6e65 203d 2070 726f 632e 7374 646f 7574  ne = proc.stdout
-000100b0: 2e72 6561 646c 696e 6528 290a 2020 2020  .readline().    
-000100c0: 2020 2020 2020 2020 6966 206e 6f74 206c          if not l
-000100d0: 696e 653a 0a20 2020 2020 2020 2020 2020  ine:.           
-000100e0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-000100f0: 2020 2020 2020 204c 4f47 2e6c 6f67 286c         LOG.log(l
-00010100: 6f67 5f6c 6576 656c 5f74 6872 6573 686f  og_level_thresho
-00010110: 6c64 2c20 6c69 6e65 2e64 6563 6f64 6528  ld, line.decode(
-00010120: 2275 7466 2d38 2229 2e73 7472 6970 2822  "utf-8").strip("
-00010130: 5c6e 2229 290a 2020 2020 2020 2020 2020  \n")).          
-00010140: 2020 6465 7461 696c 7320 2b3d 206c 696e    details += lin
-00010150: 652e 6465 636f 6465 2822 7574 662d 3822  e.decode("utf-8"
-00010160: 290a 0a20 2020 2020 2020 2070 726f 632e  )..        proc.
-00010170: 7761 6974 2829 2023 2061 6464 6974 696f  wait() # additio
-00010180: 6e61 6c20 7761 6974 2074 6f20 6d61 6b65  nal wait to make
-00010190: 2073 7572 6520 7072 6f63 6573 7320 6973   sure process is
-000101a0: 2063 6f6d 706c 6574 650a 2020 2020 656c   complete.    el
-000101b0: 7365 3a0a 2020 2020 2020 2020 2320 6966  se:.        # if
-000101c0: 2064 6562 7567 6769 6e67 206e 6f74 2065   debugging not e
-000101d0: 6e61 626c 6564 2c20 7573 6520 636f 6d6d  nabled, use comm
-000101e0: 756e 6963 6174 6520 6173 2074 6861 7420  unicate as that 
-000101f0: 6861 7320 7468 650a 2020 2020 2020 2020  has the.        
-00010200: 2320 6772 6561 7465 7374 2061 6269 6c69  # greatest abili
-00010210: 7479 2074 6f20 6465 616c 2077 6974 6820  ty to deal with 
-00010220: 6c61 7267 6520 6275 6666 6572 7320 6f66  large buffers of
-00010230: 206f 7574 7075 7420 0a20 2020 2020 2020   output .       
-00010240: 2023 2062 6569 6e67 2073 746f 7265 6420   # being stored 
-00010250: 696e 2073 7562 7072 6f63 6573 732e 5049  in subprocess.PI
-00010260: 5045 0a20 2020 2020 2020 2073 7464 6f75  PE.        stdou
-00010270: 742c 205f 203d 2070 726f 632e 636f 6d6d  t, _ = proc.comm
-00010280: 756e 6963 6174 6528 290a 2020 2020 2020  unicate().      
-00010290: 2020 7379 732e 7374 646f 7574 2e77 7269    sys.stdout.wri
-000102a0: 7465 2822 207b 307d 2063 6f6d 706c 6574  te(" {0} complet
-000102b0: 655c 6e5c 6e22 2e66 6f72 6d61 7428 636d  e\n\n".format(cm
-000102c0: 645f 6e61 6d65 2929 0a20 2020 2020 2020  d_name)).       
-000102d0: 2073 7973 2e73 7464 6f75 742e 666c 7573   sys.stdout.flus
-000102e0: 6828 290a 2020 2020 2020 2020 7469 6d65  h().        time
-000102f0: 2e73 6c65 6570 2830 2e37 3529 0a20 2020  .sleep(0.75).   
-00010300: 2020 2020 2064 6574 6169 6c73 203d 2073       details = s
-00010310: 7464 6f75 742e 6465 636f 6465 2822 7574  tdout.decode("ut
-00010320: 662d 3822 290a 0a0a 2020 2020 2320 6d6f  f-8")...    # mo
-00010330: 7665 2062 6163 6b20 746f 206f 7269 6769  ve back to origi
-00010340: 6e61 6c20 6469 7265 6374 6f72 790a 2020  nal directory.  
-00010350: 2020 2320 6e6f 7465 2074 6861 7420 7468    # note that th
-00010360: 6973 206a 7573 7420 6368 616e 6765 7320  is just changes 
-00010370: 7468 6520 776f 726b 696e 6720 6469 7265  the working dire
-00010380: 6374 6f72 7920 666f 7220 7468 6520 7079  ctory for the py
-00010390: 7468 6f6e 2070 726f 6365 7373 2c0a 2020  thon process,.  
-000103a0: 2020 2320 e280 9420 7468 7573 2069 6620    # ... thus if 
-000103b0: 7468 6520 7375 6270 726f 6365 7373 2077  the subprocess w
-000103c0: 6173 2069 6e74 6572 7275 7074 6564 2061  as interrupted a
-000103d0: 6e64 2074 6865 2070 726f 6772 616d 2071  nd the program q
-000103e0: 7569 7473 2c0a 2020 2020 2320 7468 6520  uits,.    # the 
-000103f0: 6469 7265 6374 6f72 7920 6f66 2074 6865  directory of the
-00010400: 2075 7365 7227 7320 7465 726d 696e 616c   user's terminal
-00010410: 2077 6f6e 2774 2062 6520 6166 6665 6374   won't be affect
-00010420: 6564 0a20 2020 206f 732e 6368 6469 7228  ed.    os.chdir(
-00010430: 6375 7272 656e 745f 6469 7229 0a0a 2020  current_dir)..  
-00010440: 2020 7265 7475 726e 2070 726f 632e 7265    return proc.re
-00010450: 7475 726e 636f 6465 2c20 6465 7461 696c  turncode, detail
-00010460: 730a 0a0a 6465 6620 7363 7261 7065 5f72  s...def scrape_r
-00010470: 6573 756c 7473 5f66 726f 6d5f 6c6f 675f  esults_from_log_
-00010480: 6669 6c65 2870 6174 685f 6c6f 675f 6669  file(path_log_fi
-00010490: 6c65 293a 0a20 2020 2022 2222 0a20 2020  le):.    """.   
-000104a0: 2056 616c 6964 6174 6520 7468 6174 2070   Validate that p
-000104b0: 6174 685f 6c6f 675f 6669 6c65 2065 7869  ath_log_file exi
-000104c0: 7374 732c 2072 6576 6572 7365 2069 7420  sts, reverse it 
-000104d0: 616e 6420 6c6f 6f6b 2066 6f72 206c 696e  and look for lin
-000104e0: 6573 0a20 2020 2063 6f6e 7461 696e 696e  es.    containin
-000104f0: 6720 6060 5b3c 666e 5f6e 616d 653e 5d20  g ``[<fn_name>] 
-00010500: 5265 7375 6c74 3a20 7b27 7665 7273 696f  Result: {'versio
-00010510: 6e27 3a20 322e 302c 2027 7375 6363 6573  n': 2.0, 'succes
-00010520: 7327 3a20 5472 7565 2e2e 2e60 600a 0a20  s': True...``.. 
-00010530: 2020 204f 6e6c 7920 6765 7473 2074 6865     Only gets the
-00010540: 206c 6174 6573 7420 7265 7375 6c74 2066   latest result f
-00010550: 6f72 2065 6163 6820 3c66 6e5f 6e61 6d65  or each <fn_name
-00010560: 3e20 696e 2074 6865 206c 6f67 2066 696c  > in the log fil
-00010570: 650a 0a20 2020 2054 6865 206c 6f67 2066  e..    The log f
-00010580: 696c 6520 6d75 7374 2062 6520 696e 2074  ile must be in t
-00010590: 6865 2066 6f72 6d61 7420 6f66 2074 6865  he format of the
-000105a0: 2061 7070 2e6c 6f67 0a0a 2020 2020 3a70   app.log..    :p
-000105b0: 6172 616d 2070 6174 685f 6c6f 675f 6669  aram path_log_fi
-000105c0: 6c65 3a20 2872 6571 7569 7265 6429 2061  le: (required) a
-000105d0: 6273 6f6c 7574 6520 7061 7468 2074 6f20  bsolute path to 
-000105e0: 6120 6170 702e 6c6f 6720 6669 6c65 0a20  a app.log file. 
-000105f0: 2020 203a 7479 7065 2061 7267 733a 2073     :type args: s
-00010600: 7472 0a20 2020 203a 7265 7475 726e 3a20  tr.    :return: 
-00010610: 6120 6469 6374 696f 6e61 7279 2069 6e20  a dictionary in 
-00010620: 7468 6520 666f 726d 6174 207b 3c66 6e5f  the format {<fn_
-00010630: 6e61 6d65 3e3a 203c 666e 5f72 6573 756c  name>: <fn_resul
-00010640: 7473 3e7d 0a20 2020 203a 7274 7970 653a  ts>}.    :rtype:
-00010650: 2064 6963 740a 2020 2020 2222 220a 2020   dict.    """.  
-00010660: 2020 7265 7375 6c74 735f 7363 7261 7065    results_scrape
-00010670: 6420 3d20 7b7d 0a0a 2020 2020 7661 6c69  d = {}..    vali
-00010680: 6461 7465 5f66 696c 655f 7061 7468 7328  date_file_paths(
-00010690: 6f73 2e52 5f4f 4b2c 2070 6174 685f 6c6f  os.R_OK, path_lo
-000106a0: 675f 6669 6c65 290a 0a20 2020 206c 6f67  g_file)..    log
-000106b0: 5f66 696c 655f 636f 6e74 656e 7473 203d  _file_contents =
-000106c0: 2072 6561 645f 6669 6c65 2870 6174 685f   read_file(path_
-000106d0: 6c6f 675f 6669 6c65 290a 0a20 2020 2072  log_file)..    r
-000106e0: 6567 6578 5f6c 696e 6520 3d20 7265 2e63  egex_line = re.c
-000106f0: 6f6d 7069 6c65 2872 275c 5b5b 5c77 5d2b  ompile(r'\[[\w]+
-00010700: 5c5d 2052 6573 756c 745c 3a27 2920 2020  \] Result\:')   
-00010710: 2020 2020 2320 4c6f 6f6b 696e 6720 666f      # Looking fo
-00010720: 7220 6c69 6e65 2074 6861 7420 636f 6e74  r line that cont
-00010730: 6169 6e73 205b 3c66 6e5f 6e61 6d65 3e5d  ains [<fn_name>]
-00010740: 2052 6573 756c 743a 207b 2776 6572 7369   Result: {'versi
-00010750: 6f6e 273a 2032 2e30 2c20 2773 7563 6365  on': 2.0, 'succe
-00010760: 7373 273a 2054 7275 652e 2e2e 0a20 2020  ss': True....   
-00010770: 2072 6567 6578 5f66 6e5f 6e61 6d65 203d   regex_fn_name =
-00010780: 2072 652e 636f 6d70 696c 6528 7227 5c5b   re.compile(r'\[
-00010790: 285b 5c77 5d2b 295c 5d20 5265 7375 6c74  ([\w]+)\] Result
-000107a0: 5c3a 2729 2020 2320 4765 7474 696e 6720  \:')  # Getting 
-000107b0: 3c66 6e5f 6e61 6d65 3e20 6672 6f6d 205b  <fn_name> from [
-000107c0: 3c66 6e5f 6e61 6d65 3e5d 2052 6573 756c  <fn_name>] Resul
-000107d0: 743a 207b 2776 6572 7369 6f6e 273a 2032  t: {'version': 2
-000107e0: 2e30 2c20 2773 7563 6365 7373 273a 2054  .0, 'success': T
-000107f0: 7275 652e 2e2e 0a0a 2020 2020 666f 7220  rue.....    for 
-00010800: 6c20 696e 2072 6576 6572 7365 6428 6c6f  l in reversed(lo
-00010810: 675f 6669 6c65 5f63 6f6e 7465 6e74 7329  g_file_contents)
-00010820: 3a0a 2020 2020 2020 2020 6d61 7463 6820  :.        match 
-00010830: 3d20 7265 6765 785f 6c69 6e65 2e73 6561  = regex_line.sea
-00010840: 7263 6828 6c29 0a0a 2020 2020 2020 2020  rch(l)..        
-00010850: 6966 206d 6174 6368 3a0a 2020 2020 2020  if match:.      
-00010860: 2020 2020 2020 666e 5f6e 616d 655f 6772        fn_name_gr
-00010870: 6f75 705f 696e 6465 7820 3d20 300a 0a20  oup_index = 0.. 
-00010880: 2020 2020 2020 2020 2020 2066 6e5f 6e61             fn_na
-00010890: 6d65 5f6d 6174 6368 203d 206d 6174 6368  me_match = match
-000108a0: 2e67 726f 7570 2866 6e5f 6e61 6d65 5f67  .group(fn_name_g
-000108b0: 726f 7570 5f69 6e64 6578 290a 2020 2020  roup_index).    
-000108c0: 2020 2020 2020 2020 666e 5f6e 616d 655f          fn_name_
-000108d0: 6d61 7463 685f 656e 6470 6f73 203d 206d  match_endpos = m
-000108e0: 6174 6368 2e65 6e64 2866 6e5f 6e61 6d65  atch.end(fn_name
-000108f0: 5f67 726f 7570 5f69 6e64 6578 290a 0a20  _group_index).. 
-00010900: 2020 2020 2020 2020 2020 2066 6e5f 6e61             fn_na
-00010910: 6d65 203d 2072 6567 6578 5f66 6e5f 6e61  me = regex_fn_na
-00010920: 6d65 2e6d 6174 6368 2866 6e5f 6e61 6d65  me.match(fn_name
-00010930: 5f6d 6174 6368 292e 6772 6f75 7028 3129  _match).group(1)
-00010940: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00010950: 7375 6c74 735f 6672 6f6d 5f6c 203d 206c  sults_from_l = l
-00010960: 5b66 6e5f 6e61 6d65 5f6d 6174 6368 5f65  [fn_name_match_e
-00010970: 6e64 706f 733a 5d2e 7374 7269 7028 225c  ndpos:].strip("\
-00010980: 5c6e 2022 290a 0a20 2020 2020 2020 2020  \n ")..         
-00010990: 2020 2023 2043 6865 636b 2069 6620 7468     # Check if th
-000109a0: 6973 2066 6e5f 6e61 6d65 2069 7320 616c  is fn_name is al
-000109b0: 7265 6164 7920 696e 2072 6573 756c 7473  ready in results
-000109c0: 5f73 6372 6170 6564 0a20 2020 2020 2020  _scraped.       
-000109d0: 2020 2020 2069 6620 666e 5f6e 616d 6520       if fn_name 
-000109e0: 6e6f 7420 696e 2072 6573 756c 7473 5f73  not in results_s
-000109f0: 6372 6170 6564 2e6b 6579 7328 293a 0a20  craped.keys():. 
-00010a00: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00010a10: 2043 6f6e 7665 7274 2073 7472 2069 6e74   Convert str int
-00010a20: 6f20 6469 6374 0a20 2020 2020 2020 2020  o dict.         
-00010a30: 2020 2020 2020 2072 6573 756c 7473 203d         results =
-00010a40: 2061 7374 2e6c 6974 6572 616c 5f65 7661   ast.literal_eva
-00010a50: 6c28 7265 7375 6c74 735f 6672 6f6d 5f6c  l(results_from_l
-00010a60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010a70: 2020 7265 7375 6c74 735f 7363 7261 7065    results_scrape
-00010a80: 645b 666e 5f6e 616d 655d 203d 2072 6573  d[fn_name] = res
-00010a90: 756c 7473 0a0a 2020 2020 7265 7475 726e  ults..    return
-00010aa0: 2072 6573 756c 7473 5f73 6372 6170 6564   results_scraped
-00010ab0: 0a0a 0a64 6566 2068 616e 646c 655f 6669  ...def handle_fi
-00010ac0: 6c65 5f6e 6f74 5f66 6f75 6e64 5f65 7272  le_not_found_err
-00010ad0: 6f72 2865 2c20 6d73 6729 3a0a 2020 2020  or(e, msg):.    
-00010ae0: 2222 220a 2020 2020 4c6f 6f6b 7320 6174  """.    Looks at
-00010af0: 2065 2773 206d 6573 7361 6765 2061 7474   e's message att
-00010b00: 7269 6275 7465 2061 6e64 2069 660a 2020  ribute and if.  
-00010b10: 2020 6974 2063 6f6e 7461 696e 7320 4552    it contains ER
-00010b20: 524f 525f 4e4f 545f 4649 4e44 5f44 4952  ROR_NOT_FIND_DIR
-00010b30: 206f 7220 4552 524f 525f 4e4f 545f 4649   or ERROR_NOT_FI
-00010b40: 4e44 5f46 494c 450a 2020 2020 7072 696e  ND_FILE.    prin
-00010b50: 7473 2061 204c 4f47 2e77 6172 6e69 6e67  ts a LOG.warning
-00010b60: 206d 6573 7361 6765 2065 6c73 6520 6a75   message else ju
-00010b70: 7374 2072 6169 7365 7320 7468 6520 6578  st raises the ex
-00010b80: 6365 7074 696f 6e0a 0a20 2020 203a 7061  ception..    :pa
-00010b90: 7261 6d20 653a 2028 7265 7175 6972 6564  ram e: (required
-00010ba0: 2920 616e 2045 7863 6570 7469 6f6e 0a20  ) an Exception. 
-00010bb0: 2020 203a 7479 7065 2065 3a20 4578 6365     :type e: Exce
-00010bc0: 7074 696f 6e0a 2020 2020 3a70 6172 616d  ption.    :param
-00010bd0: 206d 7367 3a20 2872 6571 7569 7265 6429   msg: (required)
-00010be0: 2074 6865 2063 7573 746f 6d20 6572 726f   the custom erro
-00010bf0: 7220 6d65 7373 6167 6520 746f 2070 7269  r message to pri
-00010c00: 6e74 2061 7320 6120 5741 524e 494e 4720  nt as a WARNING 
-00010c10: 696e 2074 6865 206c 6f67 730a 2020 2020  in the logs.    
-00010c20: 3a74 7970 6520 6d73 673a 2073 7472 0a20  :type msg: str. 
-00010c30: 2020 203a 7261 6973 6573 3a20 5468 6520     :raises: The 
-00010c40: 6578 6365 7074 696f 6e20 7468 6174 2069  exception that i
-00010c50: 7320 7061 7373 6564 2075 6e6c 6573 7320  s passed unless 
-00010c60: 6974 2063 6f6e 7461 696e 7320 0a20 2020  it contains .   
-00010c70: 2045 5252 4f52 5f4e 4f54 5f46 494e 445f   ERROR_NOT_FIND_
-00010c80: 4449 5220 6f72 2045 5252 4f52 5f4e 4f54  DIR or ERROR_NOT
-00010c90: 5f46 494e 445f 4649 4c45 2069 6e20 6974  _FIND_FILE in it
-00010ca0: 7320 652e 6d65 7373 6167 650a 2020 2020  s e.message.    
-00010cb0: 2222 220a 2020 2020 6966 2063 6f6e 7374  """.    if const
-00010cc0: 616e 7473 2e45 5252 4f52 5f4e 4f54 5f46  ants.ERROR_NOT_F
-00010cd0: 494e 445f 4449 5220 6f72 2063 6f6e 7374  IND_DIR or const
-00010ce0: 616e 7473 2e45 5252 4f52 5f4e 4f54 5f46  ants.ERROR_NOT_F
-00010cf0: 494e 445f 4649 4c45 2069 6e20 652e 6d65  IND_FILE in e.me
-00010d00: 7373 6167 653a 0a20 2020 2020 2020 204c  ssage:.        L
-00010d10: 4f47 2e77 6172 6e69 6e67 2822 5741 524e  OG.warning("WARN
-00010d20: 494e 473a 2025 7322 2c20 6d73 6729 0a20  ING: %s", msg). 
-00010d30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00010d40: 2072 6169 7365 2065 0a0a 6465 6620 7374   raise e..def st
-00010d50: 725f 7265 7072 5f61 6374 6976 6174 696f  r_repr_activatio
-00010d60: 6e5f 636f 6e64 6974 696f 6e73 2861 6374  n_conditions(act
-00010d70: 6976 6174 696f 6e5f 636f 6e64 6974 696f  ivation_conditio
-00010d80: 6e73 293a 0a20 2020 2022 2222 0a20 2020  ns):.    """.   
-00010d90: 2052 6570 7265 7365 6e74 2022 6163 7469   Represent "acti
-00010da0: 7661 7469 6f6e 2063 6f6e 6469 7469 6f6e  vation condition
-00010db0: 7322 2061 7320 6120 7374 7269 6e67 2e0a  s" as a string..
-00010dc0: 0a20 2020 2045 7861 6d70 6c65 3a0a 2020  .    Example:.  
-00010dd0: 2020 2020 2020 6163 7469 7661 7469 6f6e        activation
-00010de0: 5f63 6f6e 6469 7469 6f6e 7320 3d20 7b0a  _conditions = {.
-00010df0: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-00010e00: 6469 7469 6f6e 7322 3a20 5b0a 2020 2020  ditions": [.    
-00010e10: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00010e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e30: 2020 2265 7661 6c75 6174 696f 6e5f 6964    "evaluation_id
-00010e40: 223a 204e 6f6e 652c 0a20 2020 2020 2020  ": None,.       
-00010e50: 2020 2020 2020 2020 2020 2020 2022 6669               "fi
-00010e60: 656c 645f 6e61 6d65 223a 2022 696e 6369  eld_name": "inci
-00010e70: 6465 6e74 2e69 6422 2c0a 2020 2020 2020  dent.id",.      
-00010e80: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-00010e90: 6574 686f 6422 3a20 226e 6f74 5f65 7175  ethod": "not_equ
-00010ea0: 616c 7322 2c0a 2020 2020 2020 2020 2020  als",.          
-00010eb0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00010ec0: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
-00010ed0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
-00010ee0: 7565 223a 2031 3233 3435 360a 2020 2020  ue": 123456.    
-00010ef0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00010f00: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-00010f10: 2020 2020 2020 2020 2022 6c6f 6769 635f           "logic_
-00010f20: 7479 7065 223a 2022 616c 6c22 0a20 2020  type": "all".   
-00010f30: 2020 2020 207d 0a20 2020 200a 0a20 2020       }.    ..   
-00010f40: 203a 7061 7261 6d20 6163 7469 7661 7469   :param activati
-00010f50: 6f6e 5f63 6f6e 6469 7469 6f6e 733a 205f  on_conditions: _
-00010f60: 6465 7363 7269 7074 696f 6e5f 0a20 2020  description_.   
-00010f70: 203a 7479 7065 2061 6374 6976 6174 696f   :type activatio
-00010f80: 6e5f 636f 6e64 6974 696f 6e73 3a20 5f74  n_conditions: _t
-00010f90: 7970 655f 0a20 2020 2022 2222 0a20 2020  ype_.    """.   
-00010fa0: 2063 6f6e 6469 7469 6f6e 7320 3d20 4f72   conditions = Or
-00010fb0: 6465 7265 6444 6963 7428 290a 2020 2020  deredDict().    
-00010fc0: 666f 7220 692c 2063 6f6e 6469 7469 6f6e  for i, condition
-00010fd0: 2069 6e20 656e 756d 6572 6174 6528 6163   in enumerate(ac
-00010fe0: 7469 7661 7469 6f6e 5f63 6f6e 6469 7469  tivation_conditi
-00010ff0: 6f6e 732e 6765 7428 2263 6f6e 6469 7469  ons.get("conditi
-00011000: 6f6e 7322 2c20 5b5d 292c 2073 7461 7274  ons", []), start
-00011010: 3d31 293a 0a20 2020 2020 2020 2066 6965  =1):.        fie
-00011020: 6c64 5f6e 616d 6520 3d20 636f 6e64 6974  ld_name = condit
-00011030: 696f 6e2e 6765 7428 2266 6965 6c64 5f6e  ion.get("field_n
-00011040: 616d 6522 2920 6f72 2022 220a 2020 2020  ame") or "".    
-00011050: 2020 2020 6d65 7468 6f64 203d 2063 6f6e      method = con
-00011060: 6469 7469 6f6e 2e67 6574 2822 6d65 7468  dition.get("meth
-00011070: 6f64 2229 206f 7220 2222 0a20 2020 2020  od") or "".     
-00011080: 2020 2076 616c 7565 203d 2063 6f6e 6469     value = condi
-00011090: 7469 6f6e 2e67 6574 2822 7661 6c75 6522  tion.get("value"
-000110a0: 2920 6f72 2022 220a 0a20 2020 2020 2020  ) or ""..       
-000110b0: 2023 2069 6e64 6578 2069 6e74 6f20 7468   # index into th
-000110c0: 6520 6469 6374 696f 6e61 7279 2062 7920  e dictionary by 
-000110d0: 7468 6520 6576 616c 7561 7469 6f6e 2049  the evaluation I
-000110e0: 4420 7768 6963 6820 6973 206f 6e6c 7920  D which is only 
-000110f0: 7072 6573 656e 740a 2020 2020 2020 2020  present.        
-00011100: 2320 6966 2074 6865 206c 6f67 6963 5f74  # if the logic_t
-00011110: 7970 6520 6973 2022 6164 7661 6e63 6564  ype is "advanced
-00011120: 222e 2049 6620 6e6f 7420 7072 6573 656e  ". If not presen
-00011130: 7420 2869 2e65 2e20 6c6f 6769 635f 7479  t (i.e. logic_ty
-00011140: 7065 3d3d 616e 7920 6f72 2061 6c6c 292c  pe==any or all),
-00011150: 0a20 2020 2020 2020 2023 2074 6865 6e20  .        # then 
-00011160: 7765 206a 7573 7420 6b65 6570 2074 7261  we just keep tra
-00011170: 636b 2077 6974 6820 7468 6520 696e 6465  ck with the inde
-00011180: 7820 696e 2077 6869 6368 2069 7420 7761  x in which it wa
-00011190: 7320 666f 756e 6420 696e 2074 6865 206c  s found in the l
-000111a0: 6973 740a 2020 2020 2020 2020 2320 4e4f  ist.        # NO
-000111b0: 5445 3a20 7573 6520 6060 6669 6c74 6572  TE: use ``filter
-000111c0: 284e 6f6e 652c 205b 2e2e 2e69 7465 6d73  (None, [...items
-000111d0: 2e2e 2e5d 2960 6020 6865 7265 2074 6f20  ...])`` here to 
-000111e0: 6472 6f70 2061 6e79 2065 6c65 6d65 6e74  drop any element
-000111f0: 7320 7468 6174 206d 6967 6874 0a20 2020  s that might.   
-00011200: 2020 2020 2023 2062 6520 4e6f 6e65 2e20       # be None. 
-00011210: 5468 6973 2077 6f75 6c64 206f 6363 7572  This would occur
-00011220: 2069 6e20 7468 6520 6361 7365 2074 6861   in the case tha
-00011230: 7420 6120 636f 6e64 6974 696f 6e20 646f  t a condition do
-00011240: 6573 6e27 7420 6861 7665 0a20 2020 2020  esn't have.     
-00011250: 2020 2023 2061 6c6c 2074 6872 6565 2065     # all three e
-00011260: 6c65 6d65 6e74 732e 2045 7861 6d70 6c65  lements. Example
-00011270: 3a20 2269 6e63 6964 656e 745f 6372 6561  : "incident_crea
-00011280: 7465 6422 2064 6f65 736e 2774 2068 6176  ted" doesn't hav
-00011290: 6520 616e 7920 6d65 7468 6f64 206f 7220  e any method or 
-000112a0: 7661 6c75 650a 2020 2020 2020 2020 636f  value.        co
-000112b0: 6e64 6974 696f 6e73 5b63 6f6e 6469 7469  nditions[conditi
-000112c0: 6f6e 2e67 6574 2822 6576 616c 7561 7469  on.get("evaluati
-000112d0: 6f6e 5f69 6422 2920 6f72 2069 5d20 3d20  on_id") or i] = 
-000112e0: 7522 2022 2e6a 6f69 6e28 6669 6c74 6572  u" ".join(filter
-000112f0: 284e 6f6e 652c 205b 7374 7228 6669 656c  (None, [str(fiel
-00011300: 645f 6e61 6d65 292c 2073 7472 286d 6574  d_name), str(met
-00011310: 686f 6429 2c20 7374 7228 7661 6c75 6529  hod), str(value)
-00011320: 5d29 290a 0a20 2020 2069 6620 7374 7228  ]))..    if str(
-00011330: 6163 7469 7661 7469 6f6e 5f63 6f6e 6469  activation_condi
-00011340: 7469 6f6e 732e 6765 7428 226c 6f67 6963  tions.get("logic
-00011350: 5f74 7970 6522 2c20 2222 2929 2e6c 6f77  _type", "")).low
-00011360: 6572 2829 203d 3d20 2261 6c6c 223a 0a20  er() == "all":. 
-00011370: 2020 2020 2020 2072 6574 7572 6e20 7522         return u"
-00011380: 2041 4e44 2022 2e6a 6f69 6e28 636f 6e64   AND ".join(cond
-00011390: 6974 696f 6e73 2e76 616c 7565 7328 2929  itions.values())
-000113a0: 0a20 2020 2065 6c69 6620 7374 7228 6163  .    elif str(ac
-000113b0: 7469 7661 7469 6f6e 5f63 6f6e 6469 7469  tivation_conditi
-000113c0: 6f6e 732e 6765 7428 226c 6f67 6963 5f74  ons.get("logic_t
-000113d0: 7970 6522 2c20 2222 2929 2e6c 6f77 6572  ype", "")).lower
-000113e0: 2829 203d 3d20 2261 6e79 223a 0a20 2020  () == "any":.   
-000113f0: 2020 2020 2072 6574 7572 6e20 7522 204f       return u" O
-00011400: 5220 222e 6a6f 696e 2863 6f6e 6469 7469  R ".join(conditi
-00011410: 6f6e 732e 7661 6c75 6573 2829 290a 2020  ons.values()).  
-00011420: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00011430: 636f 6e64 6974 696f 6e5f 7374 7220 3d20  condition_str = 
-00011440: 6163 7469 7661 7469 6f6e 5f63 6f6e 6469  activation_condi
-00011450: 7469 6f6e 732e 6765 7428 2263 7573 746f  tions.get("custo
-00011460: 6d5f 636f 6e64 6974 696f 6e22 290a 2020  m_condition").  
-00011470: 2020 2020 2020 2320 6865 7265 2077 6520        # here we 
-00011480: 646f 2074 776f 2070 6173 7365 7320 746f  do two passes to
-00011490: 2070 6572 666f 726d 2061 206b 696e 6420   perform a kind 
-000114a0: 6f66 2022 7361 6c74 696e 6722 0a20 2020  of "salting".   
-000114b0: 2020 2020 2023 2074 6869 7320 6973 206e       # this is n
-000114c0: 6563 6573 7361 7279 2074 6f20 6176 6f69  ecessary to avoi
-000114d0: 6420 7468 6520 636f 6e64 6974 696f 6e20  d the condition 
-000114e0: 7768 6572 6520 696e 206f 6e65 2069 7465  where in one ite
-000114f0: 7261 7469 6f6e 0a20 2020 2020 2020 2023  ration.        #
-00011500: 2077 6520 7265 706c 6163 6520 2231 2220   we replace "1" 
-00011510: 7769 7468 2022 3132 3334 2220 616e 6420  with "1234" and 
-00011520: 6f6e 2074 6865 206e 6578 7420 6974 6572  on the next iter
-00011530: 6174 696f 6e20 7765 2072 6570 6c61 6365  ation we replace
-00011540: 0a20 2020 2020 2020 2023 2022 3222 2077  .        # "2" w
-00011550: 6974 6820 736f 6d65 7468 696e 6720 656c  ith something el
-00011560: 7365 3b20 696e 2074 6869 7320 6b69 6e64  se; in this kind
-00011570: 206f 6620 7363 656e 6172 696f 2c20 7765   of scenario, we
-00011580: 2764 2062 650a 2020 2020 2020 2020 2320  'd be.        # 
-00011590: 7265 706c 6163 696e 6720 6120 2232 2220  replacing a "2" 
-000115a0: 7768 6963 6820 7765 2064 6964 6e27 7420  which we didn't 
-000115b0: 7761 6e74 2074 6f0a 2020 2020 2020 2020  want to.        
-000115c0: 2320 536f 2069 6e73 7465 6164 2c20 7765  # So instead, we
-000115d0: 2067 656e 6572 6174 6520 6120 756e 6971   generate a uniq
-000115e0: 7565 2073 616c 7420 616e 6420 0a20 2020  ue salt and .   
-000115f0: 2020 2020 2023 2077 6520 7265 706c 6163       # we replac
-00011600: 6520 7468 6520 6f72 6967 696e 616c 206e  e the original n
-00011610: 756d 6265 7220 7769 7468 2074 6861 742e  umber with that.
-00011620: 2074 6865 6e20 6f6e 2074 6865 2073 6563   then on the sec
-00011630: 6f6e 6420 7061 7373 2c0a 2020 2020 2020  ond pass,.      
-00011640: 2020 2320 7765 2072 6570 6c61 6365 2074    # we replace t
-00011650: 6865 2073 616c 7420 7769 7468 2074 6865  he salt with the
-00011660: 2069 6e74 656e 6465 6420 7661 6c75 650a   intended value.
-00011670: 2020 2020 2020 2020 2320 4974 2069 7320          # It is 
-00011680: 616c 736f 2043 5255 4349 414c 2074 6861  also CRUCIAL tha
-00011690: 7420 7468 6520 6b65 7973 2061 7265 2070  t the keys are p
-000116a0: 726f 6365 7373 6564 2069 6e20 7265 7665  rocessed in reve
-000116b0: 7273 6520 6f72 6465 720a 2020 2020 2020  rse order.      
-000116c0: 2020 2320 746f 2070 726f 7065 726c 7920    # to properly 
-000116d0: 6861 6e64 6c65 2064 6f75 626c 6520 6469  handle double di
-000116e0: 6769 7420 6576 616c 7561 7469 6f6e 2049  git evaluation I
-000116f0: 4473 0a20 2020 2020 2020 2073 616c 7473  Ds.        salts
-00011700: 203d 207b 7d0a 2020 2020 2020 2020 666f   = {}.        fo
-00011710: 7220 6576 616c 7561 7469 6f6e 5f69 6420  r evaluation_id 
-00011720: 696e 2073 6f72 7465 6428 636f 6e64 6974  in sorted(condit
-00011730: 696f 6e73 2e6b 6579 7328 292c 2072 6576  ions.keys(), rev
-00011740: 6572 7365 3d54 7275 6529 3a0a 2020 2020  erse=True):.    
-00011750: 2020 2020 2020 2020 2320 6e75 6d62 6572          # number
-00011760: 7320 6865 7265 2061 7265 2074 6865 2065  s here are the e
-00011770: 6e65 6d79 202d 2d20 736f 2066 6972 7374  nemy -- so first
-00011780: 2077 6520 6e65 6564 2074 6f20 6d61 7020   we need to map 
-00011790: 6561 6368 2069 6e64 6976 6964 7561 6c20  each individual 
-000117a0: 6469 6769 7420 746f 0a20 2020 2020 2020  digit to.       
-000117b0: 2020 2020 2023 2061 2073 7065 6369 616c       # a special
-000117c0: 2073 7472 696e 6720 7661 6c75 6520 2849   string value (I
-000117d0: 2064 6563 6964 6564 2074 6f20 7573 6520   decided to use 
-000117e0: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
-000117f0: 6720 7661 6c75 6573 206f 6e20 7468 6520  g values on the 
-00011800: 6b65 7962 6f61 7264 290a 2020 2020 2020  keyboard).      
-00011810: 2020 2020 2020 6861 7368 6564 5f65 7661        hashed_eva
-00011820: 6c5f 6964 203d 2022 222e 6a6f 696e 2863  l_id = "".join(c
-00011830: 6f6e 7374 616e 7473 2e53 414c 545f 4841  onstants.SALT_HA
-00011840: 5348 5f4d 4150 5b69 645d 2066 6f72 2069  SH_MAP[id] for i
-00011850: 6420 696e 2073 7472 2865 7661 6c75 6174  d in str(evaluat
-00011860: 696f 6e5f 6964 2929 0a20 2020 2020 2020  ion_id)).       
-00011870: 2020 2020 2023 2074 6865 6e20 6164 6420       # then add 
-00011880: 6f75 7220 756e 6971 7565 2022 646f 6367  our unique "docg
-00011890: 656e 5f7b 7d5f 7361 6c74 2220 7072 6566  en_{}_salt" pref
-000118a0: 6978 2074 6f20 6164 6420 6578 7472 6120  ix to add extra 
-000118b0: 756e 6971 7565 6e65 7373 0a20 2020 2020  uniqueness.     
-000118c0: 2020 2020 2020 2023 204e 4f54 453a 2075         # NOTE: u
-000118d0: 6e69 7175 656e 6573 7320 6973 206e 6f74  niqueness is not
-000118e0: 2067 7561 7261 6e74 6565 6420 6865 7265   guaranteed here
-000118f0: 2066 726f 6d20 6f74 6865 7220 706f 7373   from other poss
-00011900: 6962 6c65 2076 616c 7565 730a 2020 2020  ible values.    
-00011910: 2020 2020 2020 2020 2320 7768 6963 6820          # which 
-00011920: 7765 276c 6c20 6265 2073 7562 7374 6974  we'll be substit
-00011930: 7574 696e 6720 696e 2c20 6275 7420 6974  uting in, but it
-00011940: 2069 7320 756e 6c69 6b65 6c79 2074 6861   is unlikely tha
-00011950: 7420 616e 796f 6e65 2068 6173 0a20 2020  t anyone has.   
-00011960: 2020 2020 2020 2020 2023 2022 646f 6367           # "docg
-00011970: 656e 5f21 4023 245f 7361 6c74 2220 696e  en_!@#$_salt" in
-00011980: 2074 6865 6972 2073 7973 7465 6d2e 2e2e   their system...
-00011990: 2073 6f20 756e 6971 7565 6e65 7373 2069   so uniqueness i
-000119a0: 7320 7072 6163 7469 6361 6c6c 7920 6775  s practically gu
-000119b0: 6172 616e 7465 6564 0a20 2020 2020 2020  aranteed.       
-000119c0: 2020 2020 2073 616c 7473 5b65 7661 6c75       salts[evalu
-000119d0: 6174 696f 6e5f 6964 5d20 3d20 636f 6e73  ation_id] = cons
-000119e0: 7461 6e74 732e 444f 4347 454e 5f53 414c  tants.DOCGEN_SAL
-000119f0: 545f 5052 4546 4958 2e66 6f72 6d61 7428  T_PREFIX.format(
-00011a00: 6861 7368 6564 5f65 7661 6c5f 6964 290a  hashed_eval_id).
-00011a10: 2020 2020 2020 2020 2020 2020 636f 6e64              cond
-00011a20: 6974 696f 6e5f 7374 7220 3d20 636f 6e64  ition_str = cond
-00011a30: 6974 696f 6e5f 7374 722e 7265 706c 6163  ition_str.replac
-00011a40: 6528 7374 7228 6576 616c 7561 7469 6f6e  e(str(evaluation
-00011a50: 5f69 6429 2c20 7361 6c74 732e 6765 7428  _id), salts.get(
-00011a60: 6576 616c 7561 7469 6f6e 5f69 6429 290a  evaluation_id)).
-00011a70: 2020 2020 2020 2020 666f 7220 6576 616c          for eval
-00011a80: 7561 7469 6f6e 5f69 6420 696e 2063 6f6e  uation_id in con
-00011a90: 6469 7469 6f6e 733a 0a20 2020 2020 2020  ditions:.       
-00011aa0: 2020 2020 2063 6f6e 6469 7469 6f6e 5f73       condition_s
-00011ab0: 7472 203d 2063 6f6e 6469 7469 6f6e 5f73  tr = condition_s
-00011ac0: 7472 2e72 6570 6c61 6365 2873 616c 7473  tr.replace(salts
-00011ad0: 2e67 6574 2865 7661 6c75 6174 696f 6e5f  .get(evaluation_
-00011ae0: 6964 292c 2063 6f6e 6469 7469 6f6e 732e  id), conditions.
-00011af0: 6765 7428 6576 616c 7561 7469 6f6e 5f69  get(evaluation_i
-00011b00: 6429 290a 2020 2020 2020 2020 7265 7475  d)).        retu
-00011b10: 726e 2063 6f6e 6469 7469 6f6e 5f73 7472  rn condition_str
-00011b20: 0a0a 636c 6173 7320 436f 6e74 6578 744d  ..class ContextM
-00011b30: 616e 6765 7246 6f72 5465 6d70 6f72 6172  angerForTemporar
-00011b40: 7944 6972 6563 746f 7279 2829 3a0a 2020  yDirectory():.  
-00011b50: 2020 2222 220a 2020 2020 5468 6973 2069    """.    This i
-00011b60: 7320 6120 736d 616c 6c20 636c 6173 7320  s a small class 
-00011b70: 666f 7220 7361 6665 2075 7365 206f 6620  for safe use of 
-00011b80: 6060 7465 6d70 6669 6c65 2e6d 6b64 7465  ``tempfile.mkdte
-00011b90: 6d70 2829 6060 2077 6869 6368 2072 6571  mp()`` which req
-00011ba0: 7569 7265 7320 636c 6561 6e75 7020 6166  uires cleanup af
-00011bb0: 7465 720a 2020 2020 7573 652e 2054 6865  ter.    use. The
-00011bc0: 2063 6c61 7373 2065 6666 6563 7469 7665   class effective
-00011bd0: 6c79 2069 7320 7468 6520 7361 6d65 2061  ly is the same a
-00011be0: 7320 6060 7465 6d70 6669 6c65 2e54 656d  s ``tempfile.Tem
-00011bf0: 706f 7261 7279 4469 7265 6374 6f72 7960  poraryDirectory`
-00011c00: 602c 2068 6f77 6576 6572 2c20 0a20 2020  `, however, .   
-00011c10: 2074 6861 7420 636c 6173 7320 6973 6e27   that class isn'
-00011c20: 7420 6176 6169 6c61 626c 6520 6265 666f  t available befo
-00011c30: 7265 2070 7974 686f 6e20 3320 7468 7573  re python 3 thus
-00011c40: 2074 6865 2069 6d70 6c65 6d65 6e74 6174   the implementat
-00011c50: 696f 6e20 6865 7265 2e0a 2020 2020 4f6e  ion here..    On
-00011c60: 2065 6e74 6572 2c20 6060 7465 6d70 6669   enter, ``tempfi
-00011c70: 6c65 2e6d 6b64 7465 6d70 282a 6172 6773  le.mkdtemp(*args
-00011c80: 2c20 2a2a 6b77 6172 6773 2960 6020 6973  , **kwargs)`` is
-00011c90: 2063 616c 6c65 6420 616e 6420 6f6e 2065   called and on e
-00011ca0: 7869 7420 6060 7368 7574 696c 2e72 6d74  xit ``shutil.rmt
-00011cb0: 7265 6528 7061 7468 5f74 6f5f 6469 7229  ree(path_to_dir)
-00011cc0: 6060 2069 7320 6361 6c6c 6564 2e0a 0a20  `` is called... 
-00011cd0: 2020 2045 7861 6d70 6c65 3a0a 0a20 2020     Example:..   
-00011ce0: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
-00011cf0: 2070 7974 686f 6e0a 2020 2020 2020 2020   python.        
-00011d00: 2320 6372 6561 7465 2074 6865 2063 6f6e  # create the con
-00011d10: 7465 7874 206d 616e 6167 6572 2075 7369  text manager usi
-00011d20: 6e67 2074 6865 2027 7769 7468 202e 2e2e  ng the 'with ...
-00011d30: 2061 733a 2720 7374 6174 656d 656e 740a   as:' statement.
-00011d40: 2020 2020 2020 2020 2320 6f6e 2063 7265          # on cre
-00011d50: 6174 696f 6e20 6f66 2074 6865 2027 7061  ation of the 'pa
-00011d60: 7468 5f74 6f5f 746d 705f 6469 7227 206f  th_to_tmp_dir' o
-00011d70: 626a 6563 742c 2074 6865 2060 605f 5f65  bject, the ``__e
-00011d80: 6e74 6572 5f5f 6060 206d 6574 686f 6420  nter__`` method 
-00011d90: 6973 2063 616c 6c65 640a 0a20 2020 2020  is called..     
-00011da0: 2020 2077 6974 6820 7364 6b5f 6865 6c70     with sdk_help
-00011db0: 6572 732e 436f 6e74 6578 744d 616e 6765  ers.ContextMange
-00011dc0: 7246 6f72 5465 6d70 6f72 6172 7944 6972  rForTemporaryDir
-00011dd0: 6563 746f 7279 2829 2061 7320 7061 7468  ectory() as path
-00011de0: 5f74 6f5f 746d 705f 6469 723a 0a20 2020  _to_tmp_dir:.   
-00011df0: 2020 2020 2020 2020 2023 202e 2e2e 0a20           # .... 
-00011e00: 2020 2020 2020 2020 2020 2023 2064 6f20             # do 
-00011e10: 736f 6d65 7468 696e 6720 7769 7468 2070  something with p
-00011e20: 6174 685f 746f 5f74 6d70 5f64 6972 0a20  ath_to_tmp_dir. 
-00011e30: 2020 2020 2020 2020 2020 2023 202e 2e2e             # ...
-00011e40: 0a0a 2020 2020 2020 2020 2320 6f6e 2065  ..        # on e
-00011e50: 7869 7420 6f66 2063 6f6e 7465 7874 206d  xit of context m
-00011e60: 616e 6167 6572 2c20 7061 7468 5f74 6f5f  anager, path_to_
-00011e70: 746d 705f 6469 7220 7769 6c6c 2062 6520  tmp_dir will be 
-00011e80: 636c 6561 6e65 6420 7570 2062 7920 696d  cleaned up by im
-00011e90: 706c 6963 6974 2063 616c 6c20 6f66 2074  plicit call of t
-00011ea0: 6865 2060 605f 5f65 7869 745f 5f60 6020  he ``__exit__`` 
-00011eb0: 6d65 7468 6f64 0a0a 2020 2020 3a70 6172  method..    :par
-00011ec0: 616d 2061 7267 733a 2061 6e79 206f 7264  am args: any ord
-00011ed0: 6572 6564 2061 7267 7320 7468 6174 2061  ered args that a
-00011ee0: 7265 2072 656c 6576 616e 7420 746f 2063  re relevant to c
-00011ef0: 616c 6c69 6e67 2060 6074 656d 7066 696c  alling ``tempfil
-00011f00: 652e 6d6b 6474 656d 7028 2960 600a 2020  e.mkdtemp()``.  
-00011f10: 2020 3a70 6172 616d 206b 7761 7267 733a    :param kwargs:
-00011f20: 2061 6e79 206b 6579 776f 7264 2061 7267   any keyword arg
-00011f30: 756d 656e 7473 2072 656c 6576 616e 7420  uments relevant 
-00011f40: 746f 2063 616c 6c69 6e67 2060 6074 656d  to calling ``tem
-00011f50: 7066 696c 652e 6d6b 6474 656d 7028 2960  pfile.mkdtemp()`
-00011f60: 600a 2020 2020 2222 220a 0a20 2020 2064  `.    """..    d
-00011f70: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00011f80: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
-00011f90: 7329 3a0a 2020 2020 2020 2020 7365 6c66  s):.        self
-00011fa0: 2e64 6972 203d 2074 656d 7066 696c 652e  .dir = tempfile.
-00011fb0: 6d6b 6474 656d 7028 2a61 7267 732c 202a  mkdtemp(*args, *
-00011fc0: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
-00011fd0: 6620 5f5f 656e 7465 725f 5f28 7365 6c66  f __enter__(self
-00011fe0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00011ff0: 6e20 7365 6c66 2e64 6972 0a0a 2020 2020  n self.dir..    
-00012000: 6465 6620 5f5f 6578 6974 5f5f 2873 656c  def __exit__(sel
-00012010: 662c 2065 7863 5f74 7970 652c 2065 7863  f, exc_type, exc
-00012020: 5f76 616c 7565 2c20 6578 635f 7472 6163  _value, exc_trac
-00012030: 6562 6163 6b29 3a0a 2020 2020 2020 2020  eback):.        
-00012040: 7368 7574 696c 2e72 6d74 7265 6528 7365  shutil.rmtree(se
-00012050: 6c66 2e64 6972 290a                      lf.dir).
+0000f440: 0a20 2020 2020 2020 2023 2069 6620 7665  .        # if ve
+0000f450: 7273 696f 6e20 6973 206f 6e6c 7920 6f6e  rsion is only on
+0000f460: 6520 6e75 6d62 6572 2028 692e 652e 2027  e number (i.e. '
+0000f470: 3327 292c 2074 6865 6e20 6164 6420 6120  3'), then add a 
+0000f480: 3020 746f 2074 6865 2065 6e64 0a20 2020  0 to the end.   
+0000f490: 2020 2020 2069 6620 6c65 6e28 6d61 6a6f       if len(majo
+0000f4a0: 725f 6d69 6e6f 725f 6d69 6372 6f29 203d  r_minor_micro) =
+0000f4b0: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+0000f4c0: 206d 616a 6f72 5f6d 696e 6f72 5f6d 6963   major_minor_mic
+0000f4d0: 726f 203d 2028 6d61 6a6f 725f 6d69 6e6f  ro = (major_mino
+0000f4e0: 725f 6d69 6372 6f5b 305d 2c20 302c 2030  r_micro[0], 0, 0
+0000f4f0: 290a 2020 2020 2020 2020 656c 6966 206c  ).        elif l
+0000f500: 656e 286d 616a 6f72 5f6d 696e 6f72 5f6d  en(major_minor_m
+0000f510: 6963 726f 2920 3d3d 2032 3a0a 2020 2020  icro) == 2:.    
+0000f520: 2020 2020 2020 2020 6d61 6a6f 725f 6d69          major_mi
+0000f530: 6e6f 725f 6d69 6372 6f20 3d20 286d 616a  nor_micro = (maj
+0000f540: 6f72 5f6d 696e 6f72 5f6d 6963 726f 5b30  or_minor_micro[0
+0000f550: 5d2c 206d 616a 6f72 5f6d 696e 6f72 5f6d  ], major_minor_m
+0000f560: 6963 726f 5b31 5d2c 2030 290a 2020 2020  icro[1], 0).    
+0000f570: 2020 2020 7265 7475 726e 206d 616a 6f72      return major
+0000f580: 5f6d 696e 6f72 5f6d 6963 726f 0a0a 6465  _minor_micro..de
+0000f590: 6620 7061 7273 655f 6f70 7469 6f6e 616c  f parse_optional
+0000f5a0: 7328 6f70 7469 6f6e 616c 7329 3a0a 2020  s(optionals):.  
+0000f5b0: 2020 2222 220a 2020 2020 5265 7475 726e    """.    Return
+0000f5c0: 7320 616c 6c20 6f70 7469 6f6e 616c 7320  s all optionals 
+0000f5d0: 6173 2061 2066 6f72 6d61 7474 6564 2073  as a formatted s
+0000f5e0: 7472 696e 670a 2020 2020 7769 7468 2074  tring.    with t
+0000f5f0: 6865 206e 756d 6265 7220 6f66 2074 6162  he number of tab
+0000f600: 7320 7573 6564 2064 6570 656e 6469 6e67  s used depending
+0000f610: 0a20 2020 206f 6e20 7468 6520 6c65 6e67  .    on the leng
+0000f620: 7468 0a0a 2020 2020 4d61 696e 6c79 2075  th..    Mainly u
+0000f630: 7365 6420 746f 2068 656c 7020 6275 696c  sed to help buil
+0000f640: 6420 6f75 7220 646f 6373 0a0a 2020 2020  d our docs..    
+0000f650: 3a70 6172 616d 206f 7074 696f 6e61 6c73  :param optionals
+0000f660: 3a20 4c69 7374 206f 6620 4172 6775 6d65  : List of Argume
+0000f670: 6e74 5061 7273 6572 206f 7074 696f 6e61  ntParser optiona
+0000f680: 6c73 0a20 2020 203a 7479 7065 206f 7074  ls.    :type opt
+0000f690: 696f 6e61 6c73 3a20 6c69 7374 0a20 2020  ionals: list.   
+0000f6a0: 203a 7265 7475 726e 3a20 466f 726d 6174   :return: Format
+0000f6b0: 7465 6420 7374 7269 6e67 0a20 2020 203a  ted string.    :
+0000f6c0: 7274 7970 653a 2073 7472 0a20 2020 2022  rtype: str.    "
+0000f6d0: 2222 0a20 2020 2070 6172 7365 645f 6f70  "".    parsed_op
+0000f6e0: 7469 6f6e 616c 7320 3d20 5b5d 0a0a 2020  tionals = []..  
+0000f6f0: 2020 666f 7220 6f70 7469 6f6e 2069 6e20    for option in 
+0000f700: 6f70 7469 6f6e 616c 733a 0a0a 2020 2020  optionals:..    
+0000f710: 2020 2020 2320 736b 6970 7065 6420 616e      # skipped an
+0000f720: 7920 7375 7070 7265 7373 6564 206f 7074  y suppressed opt
+0000f730: 696f 6e73 0a20 2020 2020 2020 2069 6620  ions.        if 
+0000f740: 6f70 7469 6f6e 2e68 656c 7020 3d3d 2053  option.help == S
+0000f750: 5550 5052 4553 533a 0a20 2020 2020 2020  UPPRESS:.       
+0000f760: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
+0000f770: 2020 2020 2020 206f 7074 696f 6e5f 7374         option_st
+0000f780: 7269 6e67 7320 3d20 222c 2022 2e6a 6f69  rings = ", ".joi
+0000f790: 6e28 6f70 7469 6f6e 2e6f 7074 696f 6e5f  n(option.option_
+0000f7a0: 7374 7269 6e67 7329 0a0a 2020 2020 2020  strings)..      
+0000f7b0: 2020 7461 6273 203d 2022 5c74 5c74 5c74    tabs = "\t\t\t
+0000f7c0: 220a 0a20 2020 2020 2020 2069 6620 6c65  "..        if le
+0000f7d0: 6e28 6f70 7469 6f6e 5f73 7472 696e 6773  n(option_strings
+0000f7e0: 2920 3e3d 2031 363a 0a20 2020 2020 2020  ) >= 16:.       
+0000f7f0: 2020 2020 2074 6162 7320 3d20 225c 745c       tabs = "\t\
+0000f800: 7422 0a0a 2020 2020 2020 2020 6966 206c  t"..        if l
+0000f810: 656e 286f 7074 696f 6e5f 7374 7269 6e67  en(option_string
+0000f820: 7329 203e 3d20 3232 3a0a 2020 2020 2020  s) >= 22:.      
+0000f830: 2020 2020 2020 7461 6273 203d 2022 5c74        tabs = "\t
+0000f840: 220a 0a20 2020 2020 2020 2069 6620 6c65  "..        if le
+0000f850: 6e28 6f70 7469 6f6e 5f73 7472 696e 6773  n(option_strings
+0000f860: 2920 3c20 3130 3a0a 2020 2020 2020 2020  ) < 10:.        
+0000f870: 2020 2020 7461 6273 203d 2022 5c74 5c74      tabs = "\t\t
+0000f880: 5c74 5c74 220a 0a20 2020 2020 2020 2069  \t\t"..        i
+0000f890: 6620 6c65 6e28 6f70 7469 6f6e 5f73 7472  f len(option_str
+0000f8a0: 696e 6773 2920 696e 2028 382c 2039 293a  ings) in (8, 9):
+0000f8b0: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+0000f8c0: 7320 3d20 225c 745c 745c 7422 0a0a 2020  s = "\t\t\t"..  
+0000f8d0: 2020 2020 2020 7061 7273 6564 5f6f 7074        parsed_opt
+0000f8e0: 696f 6e61 6c73 2e61 7070 656e 6428 227b  ionals.append("{
+0000f8f0: 307d 7b31 7d7b 327d 222e 666f 726d 6174  0}{1}{2}".format
+0000f900: 286f 7074 696f 6e5f 7374 7269 6e67 732c  (option_strings,
+0000f910: 2074 6162 732c 206f 7074 696f 6e2e 6865   tabs, option.he
+0000f920: 6c70 2929 0a0a 2020 2020 7061 7273 6564  lp))..    parsed
+0000f930: 5f6f 7074 696f 6e61 6c73 203d 2022 205c  _optionals = " \
+0000f940: 6e20 222e 6a6f 696e 2870 6172 7365 645f  n ".join(parsed_
+0000f950: 6f70 7469 6f6e 616c 7329 0a20 2020 2070  optionals).    p
+0000f960: 6172 7365 645f 6f70 7469 6f6e 616c 7320  arsed_optionals 
+0000f970: 3d20 277b 307d 205c 6e27 2e66 6f72 6d61  = '{0} \n'.forma
+0000f980: 7428 7061 7273 6564 5f6f 7074 696f 6e61  t(parsed_optiona
+0000f990: 6c73 290a 0a20 2020 2072 6574 7572 6e20  ls)..    return 
+0000f9a0: 7061 7273 6564 5f6f 7074 696f 6e61 6c73  parsed_optionals
+0000f9b0: 0a0a 0a64 6566 2072 756e 5f73 7562 7072  ...def run_subpr
+0000f9c0: 6f63 6573 7328 6172 6773 2c20 6368 616e  ocess(args, chan
+0000f9d0: 6765 5f64 6972 3d4e 6f6e 652c 2063 6d64  ge_dir=None, cmd
+0000f9e0: 5f6e 616d 653d 2222 2c20 6c6f 675f 6c65  _name="", log_le
+0000f9f0: 7665 6c5f 7468 7265 7368 6f6c 643d 6c6f  vel_threshold=lo
+0000fa00: 6767 696e 672e 4445 4255 4729 3a0a 2020  gging.DEBUG):.  
+0000fa10: 2020 2222 220a 2020 2020 5275 6e20 6120    """.    Run a 
+0000fa20: 6769 7665 6e20 636f 6d6d 616e 6420 6173  given command as
+0000fa30: 2061 2073 7562 7072 6f63 6573 732e 204f   a subprocess. O
+0000fa40: 7074 696f 6e61 6c6c 7920 6368 616e 6765  ptionally change
+0000fa50: 2064 6972 6563 746f 7279 2062 6566 6f72   directory befor
+0000fa60: 6520 7275 6e6e 696e 6720 7468 6520 636f  e running the co
+0000fa70: 6d6d 616e 6420 2875 7365 2063 6861 6e67  mmand (use chang
+0000fa80: 655f 6469 7220 7061 7261 6d65 7465 7229  e_dir parameter)
+0000fa90: 0a0a 2020 2020 3a70 6172 616d 2061 7267  ..    :param arg
+0000faa0: 733a 2028 7265 7175 6972 6564 2920 6172  s: (required) ar
+0000fab0: 6773 2073 686f 756c 6420 6265 2061 2073  gs should be a s
+0000fac0: 6571 7565 6e63 6520 6f66 2070 726f 6772  equence of progr
+0000fad0: 616d 2061 7267 756d 656e 7473 206f 7220  am arguments or 
+0000fae0: 656c 7365 2061 2073 696e 676c 6520 7374  else a single st
+0000faf0: 7269 6e67 2028 7365 6520 7375 6270 726f  ring (see subpro
+0000fb00: 6365 7373 2e50 6f70 656e 2066 6f72 206d  cess.Popen for m
+0000fb10: 6f72 6520 6465 7461 696c 7329 0a20 2020  ore details).   
+0000fb20: 203a 7479 7065 2061 7267 733a 2073 7472   :type args: str
+0000fb30: 207c 206c 6973 745b 7374 725d 0a20 2020   | list[str].   
+0000fb40: 203a 7061 7261 6d20 6368 616e 6765 5f64   :param change_d
+0000fb50: 6972 3a20 286f 7074 696f 6e61 6c29 2070  ir: (optional) p
+0000fb60: 6174 6820 6f66 2064 6972 6563 746f 7279  ath of directory
+0000fb70: 2074 6f20 6368 616e 6765 2074 6f20 6265   to change to be
+0000fb80: 666f 7265 2072 756e 6e69 6e67 2063 6f6d  fore running com
+0000fb90: 6d61 6e64 0a20 2020 203a 7479 7065 2063  mand.    :type c
+0000fba0: 6861 6e67 655f 6469 723a 2073 7472 0a20  hange_dir: str. 
+0000fbb0: 2020 203a 7061 7261 6d20 636d 645f 6e61     :param cmd_na
+0000fbc0: 6d65 3a20 286f 7074 696f 6e61 6c29 2074  me: (optional) t
+0000fbd0: 6865 206e 616d 6520 6f66 2074 6865 2063  he name of the c
+0000fbe0: 6f6d 6d61 6e64 2074 6f20 7275 6e20 6173  ommand to run as
+0000fbf0: 2061 2073 7562 7072 6f63 6573 732e 2077   a subprocess. w
+0000fc00: 696c 6c20 6265 2075 7365 6420 746f 206c  ill be used to l
+0000fc10: 6f67 2069 6e20 7468 6520 666f 726d 6174  og in the format
+0000fc20: 2022 5275 6e6e 696e 6720 3c63 6d64 5f6e   "Running <cmd_n
+0000fc30: 616d 653e 202e 2e2e 220a 2020 2020 3a74  ame> ...".    :t
+0000fc40: 7970 6520 636d 645f 6e61 6d65 3a20 7374  ype cmd_name: st
+0000fc50: 720a 2020 2020 3a70 6172 616d 206c 6f67  r.    :param log
+0000fc60: 5f6c 6576 656c 5f74 6872 6573 686f 6c64  _level_threshold
+0000fc70: 3a20 286f 7074 696f 6e61 6c29 2074 6865  : (optional) the
+0000fc80: 206c 6f67 6769 6e67 206c 6576 656c 2061   logging level a
+0000fc90: 7420 7768 6963 6820 746f 206f 7574 7075  t which to outpu
+0000fca0: 7420 7468 6520 7374 646f 7574 2f73 7464  t the stdout/std
+0000fcb0: 6572 7220 666f 7220 7468 6520 7375 6270  err for the subp
+0000fcc0: 726f 6365 7373 3b20 6465 6661 756c 7420  rocess; default 
+0000fcd0: 6973 2044 4542 5547 0a20 2020 203a 7479  is DEBUG.    :ty
+0000fce0: 7065 206c 6f67 5f6c 6576 656c 5f74 6872  pe log_level_thr
+0000fcf0: 6573 686f 6c64 3a20 696e 740a 2020 2020  eshold: int.    
+0000fd00: 3a72 6574 7572 6e3a 2074 6865 2065 7869  :return: the exi
+0000fd10: 7420 636f 6465 2061 6e64 2073 7472 696e  t code and strin
+0000fd20: 6720 6465 7461 696c 7320 6f66 2074 6865  g details of the
+0000fd30: 2072 756e 0a20 2020 203a 7274 7970 653a   run.    :rtype:
+0000fd40: 2028 696e 742c 2073 7472 290a 2020 2020   (int, str).    
+0000fd50: 2222 220a 0a20 2020 204c 4f47 2e64 6562  """..    LOG.deb
+0000fd60: 7567 2822 5275 6e6e 696e 6720 7b30 7d20  ug("Running {0} 
+0000fd70: 6173 2061 2073 7562 7072 6f63 6573 7322  as a subprocess"
+0000fd80: 2e66 6f72 6d61 7428 6172 6773 2929 0a0a  .format(args))..
+0000fd90: 2020 2020 2320 7361 7665 2073 7461 7274      # save start
+0000fda0: 696e 6720 6469 7265 6374 6f72 790a 2020  ing directory.  
+0000fdb0: 2020 6375 7272 656e 745f 6469 7220 3d20    current_dir = 
+0000fdc0: 6f73 2e67 6574 6377 6428 290a 0a20 2020  os.getcwd()..   
+0000fdd0: 2023 2069 6620 6368 616e 6765 5f64 6972   # if change_dir
+0000fde0: 2069 7320 7365 742c 2063 6861 6e67 6520   is set, change 
+0000fdf0: 746f 2074 6861 7420 6469 720a 2020 2020  to that dir.    
+0000fe00: 6966 2063 6861 6e67 655f 6469 723a 0a20  if change_dir:. 
+0000fe10: 2020 2020 2020 204c 4f47 2e64 6562 7567         LOG.debug
+0000fe20: 2822 4368 616e 6769 6e67 2064 6972 6563  ("Changing direc
+0000fe30: 746f 7279 2074 6f20 7b30 7d22 2e66 6f72  tory to {0}".for
+0000fe40: 6d61 7428 6368 616e 6765 5f64 6972 2929  mat(change_dir))
+0000fe50: 0a20 2020 2020 2020 206f 732e 6368 6469  .        os.chdi
+0000fe60: 7228 6368 616e 6765 5f64 6972 290a 0a20  r(change_dir).. 
+0000fe70: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000fe80: 2861 7267 732c 2073 7472 293a 0a20 2020  (args, str):.   
+0000fe90: 2020 2020 2061 7267 7320 3d20 7368 6c65       args = shle
+0000fea0: 782e 7370 6c69 7428 6172 6773 290a 0a20  x.split(args).. 
+0000feb0: 2020 2023 2072 756e 2067 6976 656e 2063     # run given c
+0000fec0: 6f6d 6d61 6e64 2061 7320 6120 7375 6270  ommand as a subp
+0000fed0: 726f 6365 7373 0a20 2020 2070 726f 6320  rocess.    proc 
+0000fee0: 3d20 7375 6270 726f 6365 7373 2e50 6f70  = subprocess.Pop
+0000fef0: 656e 2861 7267 732c 2073 7464 6572 723d  en(args, stderr=
+0000ff00: 7375 6270 726f 6365 7373 2e53 5444 4f55  subprocess.STDOU
+0000ff10: 542c 2073 7464 6f75 743d 7375 6270 726f  T, stdout=subpro
+0000ff20: 6365 7373 2e50 4950 452c 2062 7566 7369  cess.PIPE, bufsi
+0000ff30: 7a65 3d30 290a 0a20 2020 2073 7973 2e73  ze=0)..    sys.s
+0000ff40: 7464 6f75 742e 7772 6974 6528 2252 756e  tdout.write("Run
+0000ff50: 6e69 6e67 207b 307d 2028 7468 6973 206d  ning {0} (this m
+0000ff60: 6179 2074 616b 6520 6120 7768 696c 6529  ay take a while)
+0000ff70: 202e 2e2e 222e 666f 726d 6174 2863 6d64   ...".format(cmd
+0000ff80: 5f6e 616d 6529 290a 2020 2020 7379 732e  _name)).    sys.
+0000ff90: 7374 646f 7574 2e66 6c75 7368 2829 0a0a  stdout.flush()..
+0000ffa0: 2020 2020 2320 6966 2064 6562 7567 6769      # if debuggi
+0000ffb0: 6e67 2065 6e61 626c 6564 2c20 6361 7074  ng enabled, capt
+0000ffc0: 7572 6520 6f75 7470 7574 2064 6972 6563  ure output direc
+0000ffd0: 746c 7920 616e 6420 7265 6469 7265 6374  tly and redirect
+0000ffe0: 2062 6163 6b20 746f 2073 7973 2e73 7464   back to sys.std
+0000fff0: 6f75 740a 2020 2020 2320 7573 696e 6720  out.    # using 
+00010000: 4c4f 472e 6c6f 6728 6c6f 675f 6c65 7665  LOG.log(log_leve
+00010010: 6c2e 2e2e 290a 2020 2020 6966 204c 4f47  l...).    if LOG
+00010020: 2e69 7345 6e61 626c 6564 466f 7228 6c6f  .isEnabledFor(lo
+00010030: 675f 6c65 7665 6c5f 7468 7265 7368 6f6c  g_level_threshol
+00010040: 6429 3a0a 2020 2020 2020 2020 4c4f 472e  d):.        LOG.
+00010050: 6465 6275 6728 2222 290a 2020 2020 2020  debug("").      
+00010060: 2020 6465 7461 696c 7320 3d20 2222 0a20    details = "". 
+00010070: 2020 2020 2020 2077 6869 6c65 2070 726f         while pro
+00010080: 632e 7374 646f 7574 3a0a 2020 2020 2020  c.stdout:.      
+00010090: 2020 2020 2020 6c69 6e65 203d 2070 726f        line = pro
+000100a0: 632e 7374 646f 7574 2e72 6561 646c 696e  c.stdout.readlin
+000100b0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+000100c0: 6966 206e 6f74 206c 696e 653a 0a20 2020  if not line:.   
+000100d0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+000100e0: 616b 0a20 2020 2020 2020 2020 2020 204c  ak.            L
+000100f0: 4f47 2e6c 6f67 286c 6f67 5f6c 6576 656c  OG.log(log_level
+00010100: 5f74 6872 6573 686f 6c64 2c20 6c69 6e65  _threshold, line
+00010110: 2e64 6563 6f64 6528 2275 7466 2d38 2229  .decode("utf-8")
+00010120: 2e73 7472 6970 2822 5c6e 2229 290a 2020  .strip("\n")).  
+00010130: 2020 2020 2020 2020 2020 6465 7461 696c            detail
+00010140: 7320 2b3d 206c 696e 652e 6465 636f 6465  s += line.decode
+00010150: 2822 7574 662d 3822 290a 0a20 2020 2020  ("utf-8")..     
+00010160: 2020 2070 726f 632e 7761 6974 2829 2023     proc.wait() #
+00010170: 2061 6464 6974 696f 6e61 6c20 7761 6974   additional wait
+00010180: 2074 6f20 6d61 6b65 2073 7572 6520 7072   to make sure pr
+00010190: 6f63 6573 7320 6973 2063 6f6d 706c 6574  ocess is complet
+000101a0: 650a 2020 2020 656c 7365 3a0a 2020 2020  e.    else:.    
+000101b0: 2020 2020 2320 6966 2064 6562 7567 6769      # if debuggi
+000101c0: 6e67 206e 6f74 2065 6e61 626c 6564 2c20  ng not enabled, 
+000101d0: 7573 6520 636f 6d6d 756e 6963 6174 6520  use communicate 
+000101e0: 6173 2074 6861 7420 6861 7320 7468 650a  as that has the.
+000101f0: 2020 2020 2020 2020 2320 6772 6561 7465          # greate
+00010200: 7374 2061 6269 6c69 7479 2074 6f20 6465  st ability to de
+00010210: 616c 2077 6974 6820 6c61 7267 6520 6275  al with large bu
+00010220: 6666 6572 7320 6f66 206f 7574 7075 740a  ffers of output.
+00010230: 2020 2020 2020 2020 2320 6265 696e 6720          # being 
+00010240: 7374 6f72 6564 2069 6e20 7375 6270 726f  stored in subpro
+00010250: 6365 7373 2e50 4950 450a 2020 2020 2020  cess.PIPE.      
+00010260: 2020 7374 646f 7574 2c20 5f20 3d20 7072    stdout, _ = pr
+00010270: 6f63 2e63 6f6d 6d75 6e69 6361 7465 2829  oc.communicate()
+00010280: 0a20 2020 2020 2020 2073 7973 2e73 7464  .        sys.std
+00010290: 6f75 742e 7772 6974 6528 2220 7b30 7d20  out.write(" {0} 
+000102a0: 636f 6d70 6c65 7465 5c6e 5c6e 222e 666f  complete\n\n".fo
+000102b0: 726d 6174 2863 6d64 5f6e 616d 6529 290a  rmat(cmd_name)).
+000102c0: 2020 2020 2020 2020 7379 732e 7374 646f          sys.stdo
+000102d0: 7574 2e66 6c75 7368 2829 0a20 2020 2020  ut.flush().     
+000102e0: 2020 2074 696d 652e 736c 6565 7028 302e     time.sleep(0.
+000102f0: 3735 290a 2020 2020 2020 2020 6465 7461  75).        deta
+00010300: 696c 7320 3d20 7374 646f 7574 2e64 6563  ils = stdout.dec
+00010310: 6f64 6528 2275 7466 2d38 2229 0a0a 0a20  ode("utf-8")... 
+00010320: 2020 2023 206d 6f76 6520 6261 636b 2074     # move back t
+00010330: 6f20 6f72 6967 696e 616c 2064 6972 6563  o original direc
+00010340: 746f 7279 0a20 2020 2023 206e 6f74 6520  tory.    # note 
+00010350: 7468 6174 2074 6869 7320 6a75 7374 2063  that this just c
+00010360: 6861 6e67 6573 2074 6865 2077 6f72 6b69  hanges the worki
+00010370: 6e67 2064 6972 6563 746f 7279 2066 6f72  ng directory for
+00010380: 2074 6865 2070 7974 686f 6e20 7072 6f63   the python proc
+00010390: 6573 732c 0a20 2020 2023 20e2 8094 2074  ess,.    # ... t
+000103a0: 6875 7320 6966 2074 6865 2073 7562 7072  hus if the subpr
+000103b0: 6f63 6573 7320 7761 7320 696e 7465 7272  ocess was interr
+000103c0: 7570 7465 6420 616e 6420 7468 6520 7072  upted and the pr
+000103d0: 6f67 7261 6d20 7175 6974 732c 0a20 2020  ogram quits,.   
+000103e0: 2023 2074 6865 2064 6972 6563 746f 7279   # the directory
+000103f0: 206f 6620 7468 6520 7573 6572 2773 2074   of the user's t
+00010400: 6572 6d69 6e61 6c20 776f 6e27 7420 6265  erminal won't be
+00010410: 2061 6666 6563 7465 640a 2020 2020 6f73   affected.    os
+00010420: 2e63 6864 6972 2863 7572 7265 6e74 5f64  .chdir(current_d
+00010430: 6972 290a 0a20 2020 2072 6574 7572 6e20  ir)..    return 
+00010440: 7072 6f63 2e72 6574 7572 6e63 6f64 652c  proc.returncode,
+00010450: 2064 6574 6169 6c73 0a0a 0a64 6566 2073   details...def s
+00010460: 6372 6170 655f 7265 7375 6c74 735f 6672  crape_results_fr
+00010470: 6f6d 5f6c 6f67 5f66 696c 6528 7061 7468  om_log_file(path
+00010480: 5f6c 6f67 5f66 696c 6529 3a0a 2020 2020  _log_file):.    
+00010490: 2222 220a 2020 2020 5661 6c69 6461 7465  """.    Validate
+000104a0: 2074 6861 7420 7061 7468 5f6c 6f67 5f66   that path_log_f
+000104b0: 696c 6520 6578 6973 7473 2c20 7265 7665  ile exists, reve
+000104c0: 7273 6520 6974 2061 6e64 206c 6f6f 6b20  rse it and look 
+000104d0: 666f 7220 6c69 6e65 730a 2020 2020 636f  for lines.    co
+000104e0: 6e74 6169 6e69 6e67 2060 605b 3c66 6e5f  ntaining ``[<fn_
+000104f0: 6e61 6d65 3e5d 2052 6573 756c 743a 207b  name>] Result: {
+00010500: 2776 6572 7369 6f6e 273a 2032 2e30 2c20  'version': 2.0, 
+00010510: 2773 7563 6365 7373 273a 2054 7275 652e  'success': True.
+00010520: 2e2e 6060 0a0a 2020 2020 4f6e 6c79 2067  ..``..    Only g
+00010530: 6574 7320 7468 6520 6c61 7465 7374 2072  ets the latest r
+00010540: 6573 756c 7420 666f 7220 6561 6368 203c  esult for each <
+00010550: 666e 5f6e 616d 653e 2069 6e20 7468 6520  fn_name> in the 
+00010560: 6c6f 6720 6669 6c65 0a0a 2020 2020 5468  log file..    Th
+00010570: 6520 6c6f 6720 6669 6c65 206d 7573 7420  e log file must 
+00010580: 6265 2069 6e20 7468 6520 666f 726d 6174  be in the format
+00010590: 206f 6620 7468 6520 6170 702e 6c6f 670a   of the app.log.
+000105a0: 0a20 2020 203a 7061 7261 6d20 7061 7468  .    :param path
+000105b0: 5f6c 6f67 5f66 696c 653a 2028 7265 7175  _log_file: (requ
+000105c0: 6972 6564 2920 6162 736f 6c75 7465 2070  ired) absolute p
+000105d0: 6174 6820 746f 2061 2061 7070 2e6c 6f67  ath to a app.log
+000105e0: 2066 696c 650a 2020 2020 3a74 7970 6520   file.    :type 
+000105f0: 6172 6773 3a20 7374 720a 2020 2020 3a72  args: str.    :r
+00010600: 6574 7572 6e3a 2061 2064 6963 7469 6f6e  eturn: a diction
+00010610: 6172 7920 696e 2074 6865 2066 6f72 6d61  ary in the forma
+00010620: 7420 7b3c 666e 5f6e 616d 653e 3a20 3c66  t {<fn_name>: <f
+00010630: 6e5f 7265 7375 6c74 733e 7d0a 2020 2020  n_results>}.    
+00010640: 3a72 7479 7065 3a20 6469 6374 0a20 2020  :rtype: dict.   
+00010650: 2022 2222 0a20 2020 2072 6573 756c 7473   """.    results
+00010660: 5f73 6372 6170 6564 203d 207b 7d0a 0a20  _scraped = {}.. 
+00010670: 2020 2076 616c 6964 6174 655f 6669 6c65     validate_file
+00010680: 5f70 6174 6873 286f 732e 525f 4f4b 2c20  _paths(os.R_OK, 
+00010690: 7061 7468 5f6c 6f67 5f66 696c 6529 0a0a  path_log_file)..
+000106a0: 2020 2020 6c6f 675f 6669 6c65 5f63 6f6e      log_file_con
+000106b0: 7465 6e74 7320 3d20 7265 6164 5f66 696c  tents = read_fil
+000106c0: 6528 7061 7468 5f6c 6f67 5f66 696c 6529  e(path_log_file)
+000106d0: 0a0a 2020 2020 7265 6765 785f 6c69 6e65  ..    regex_line
+000106e0: 203d 2072 652e 636f 6d70 696c 6528 7227   = re.compile(r'
+000106f0: 5c5b 5b5c 775d 2b5c 5d20 5265 7375 6c74  \[[\w]+\] Result
+00010700: 5c3a 2729 2020 2020 2020 2023 204c 6f6f  \:')       # Loo
+00010710: 6b69 6e67 2066 6f72 206c 696e 6520 7468  king for line th
+00010720: 6174 2063 6f6e 7461 696e 7320 5b3c 666e  at contains [<fn
+00010730: 5f6e 616d 653e 5d20 5265 7375 6c74 3a20  _name>] Result: 
+00010740: 7b27 7665 7273 696f 6e27 3a20 322e 302c  {'version': 2.0,
+00010750: 2027 7375 6363 6573 7327 3a20 5472 7565   'success': True
+00010760: 2e2e 2e0a 2020 2020 7265 6765 785f 666e  ....    regex_fn
+00010770: 5f6e 616d 6520 3d20 7265 2e63 6f6d 7069  _name = re.compi
+00010780: 6c65 2872 275c 5b28 5b5c 775d 2b29 5c5d  le(r'\[([\w]+)\]
+00010790: 2052 6573 756c 745c 3a27 2920 2023 2047   Result\:')  # G
+000107a0: 6574 7469 6e67 203c 666e 5f6e 616d 653e  etting <fn_name>
+000107b0: 2066 726f 6d20 5b3c 666e 5f6e 616d 653e   from [<fn_name>
+000107c0: 5d20 5265 7375 6c74 3a20 7b27 7665 7273  ] Result: {'vers
+000107d0: 696f 6e27 3a20 322e 302c 2027 7375 6363  ion': 2.0, 'succ
+000107e0: 6573 7327 3a20 5472 7565 2e2e 2e0a 0a20  ess': True..... 
+000107f0: 2020 2066 6f72 206c 2069 6e20 7265 7665     for l in reve
+00010800: 7273 6564 286c 6f67 5f66 696c 655f 636f  rsed(log_file_co
+00010810: 6e74 656e 7473 293a 0a20 2020 2020 2020  ntents):.       
+00010820: 206d 6174 6368 203d 2072 6567 6578 5f6c   match = regex_l
+00010830: 696e 652e 7365 6172 6368 286c 290a 0a20  ine.search(l).. 
+00010840: 2020 2020 2020 2069 6620 6d61 7463 683a         if match:
+00010850: 0a20 2020 2020 2020 2020 2020 2066 6e5f  .            fn_
+00010860: 6e61 6d65 5f67 726f 7570 5f69 6e64 6578  name_group_index
+00010870: 203d 2030 0a0a 2020 2020 2020 2020 2020   = 0..          
+00010880: 2020 666e 5f6e 616d 655f 6d61 7463 6820    fn_name_match 
+00010890: 3d20 6d61 7463 682e 6772 6f75 7028 666e  = match.group(fn
+000108a0: 5f6e 616d 655f 6772 6f75 705f 696e 6465  _name_group_inde
+000108b0: 7829 0a20 2020 2020 2020 2020 2020 2066  x).            f
+000108c0: 6e5f 6e61 6d65 5f6d 6174 6368 5f65 6e64  n_name_match_end
+000108d0: 706f 7320 3d20 6d61 7463 682e 656e 6428  pos = match.end(
+000108e0: 666e 5f6e 616d 655f 6772 6f75 705f 696e  fn_name_group_in
+000108f0: 6465 7829 0a0a 2020 2020 2020 2020 2020  dex)..          
+00010900: 2020 666e 5f6e 616d 6520 3d20 7265 6765    fn_name = rege
+00010910: 785f 666e 5f6e 616d 652e 6d61 7463 6828  x_fn_name.match(
+00010920: 666e 5f6e 616d 655f 6d61 7463 6829 2e67  fn_name_match).g
+00010930: 726f 7570 2831 290a 0a20 2020 2020 2020  roup(1)..       
+00010940: 2020 2020 2072 6573 756c 7473 5f66 726f       results_fro
+00010950: 6d5f 6c20 3d20 6c5b 666e 5f6e 616d 655f  m_l = l[fn_name_
+00010960: 6d61 7463 685f 656e 6470 6f73 3a5d 2e73  match_endpos:].s
+00010970: 7472 6970 2822 5c5c 6e20 2229 0a0a 2020  trip("\\n ")..  
+00010980: 2020 2020 2020 2020 2020 2320 4368 6563            # Chec
+00010990: 6b20 6966 2074 6869 7320 666e 5f6e 616d  k if this fn_nam
+000109a0: 6520 6973 2061 6c72 6561 6479 2069 6e20  e is already in 
+000109b0: 7265 7375 6c74 735f 7363 7261 7065 640a  results_scraped.
+000109c0: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+000109d0: 6e5f 6e61 6d65 206e 6f74 2069 6e20 7265  n_name not in re
+000109e0: 7375 6c74 735f 7363 7261 7065 642e 6b65  sults_scraped.ke
+000109f0: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
+00010a00: 2020 2020 2020 2320 436f 6e76 6572 7420        # Convert 
+00010a10: 7374 7220 696e 746f 2064 6963 740a 2020  str into dict.  
+00010a20: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00010a30: 7375 6c74 7320 3d20 6173 742e 6c69 7465  sults = ast.lite
+00010a40: 7261 6c5f 6576 616c 2872 6573 756c 7473  ral_eval(results
+00010a50: 5f66 726f 6d5f 6c29 0a20 2020 2020 2020  _from_l).       
+00010a60: 2020 2020 2020 2020 2072 6573 756c 7473           results
+00010a70: 203d 205f 7265 6d6f 7665 5f70 6969 5f66   = _remove_pii_f
+00010a80: 726f 6d5f 7061 796c 6f61 645f 7361 6d70  rom_payload_samp
+00010a90: 6c65 7328 7265 7375 6c74 7329 0a20 2020  les(results).   
+00010aa0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00010ab0: 756c 7473 5f73 6372 6170 6564 5b66 6e5f  ults_scraped[fn_
+00010ac0: 6e61 6d65 5d20 3d20 7265 7375 6c74 730a  name] = results.
+00010ad0: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
+00010ae0: 6c74 735f 7363 7261 7065 640a 0a64 6566  lts_scraped..def
+00010af0: 205f 7265 6d6f 7665 5f70 6969 5f66 726f   _remove_pii_fro
+00010b00: 6d5f 7061 796c 6f61 645f 7361 6d70 6c65  m_payload_sample
+00010b10: 7328 7265 7375 6c74 7329 3a0a 2020 2020  s(results):.    
+00010b20: 2222 220a 2020 2020 4865 6c70 6572 206d  """.    Helper m
+00010b30: 6574 686f 6420 746f 2072 656d 6f76 6520  ethod to remove 
+00010b40: 7065 7273 6f6e 616c 2069 6e66 6f72 6d61  personal informa
+00010b50: 7469 6f6e 2069 6e20 7061 796c 6f61 6420  tion in payload 
+00010b60: 7361 6d70 6c65 732e 0a0a 2020 2020 4173  samples...    As
+00010b70: 206f 6620 7468 6973 2063 6f6d 6d69 742c   of this commit,
+00010b80: 2074 6869 7320 6f6e 6c79 2072 656d 6f76   this only remov
+00010b90: 6573 2074 6865 2068 6f73 7420 7661 6c75  es the host valu
+00010ba0: 6520 696e 2074 6865 206d 6574 7269 6373  e in the metrics
+00010bb0: 2073 6563 7469 6f6e 2e0a 2020 2020 4275   section..    Bu
+00010bc0: 7420 696e 2074 6865 2066 7574 7572 6520  t in the future 
+00010bd0: 7468 6973 2063 6f75 6c64 2073 7570 706f  this could suppo
+00010be0: 7274 206d 6f72 6520 5049 4920 7265 6d6f  rt more PII remo
+00010bf0: 7661 6c0a 0a20 2020 203a 7061 7261 6d20  val..    :param 
+00010c00: 7265 7375 6c74 733a 2070 6179 6c6f 6164  results: payload
+00010c10: 2072 6573 756c 7473 0a20 2020 203a 7479   results.    :ty
+00010c20: 7065 2072 6573 756c 7473 3a20 6469 6374  pe results: dict
+00010c30: 0a20 2020 203a 7265 7475 726e 3a20 7361  .    :return: sa
+00010c40: 6d65 2072 6573 756c 7473 2067 6976 656e  me results given
+00010c50: 2065 7863 6570 7420 7769 7468 2061 6e79   except with any
+00010c60: 2069 6465 6e74 6966 6961 626c 6520 7069   identifiable pi
+00010c70: 6920 7265 6d6f 7665 640a 2020 2020 3a72  i removed.    :r
+00010c80: 7479 7065 3a20 6469 6374 0a20 2020 2022  type: dict.    "
+00010c90: 2222 0a20 2020 2069 6620 226d 6574 7269  "".    if "metri
+00010ca0: 6373 2220 696e 2072 6573 756c 7473 2061  cs" in results a
+00010cb0: 6e64 2022 686f 7374 2220 696e 2072 6573  nd "host" in res
+00010cc0: 756c 7473 5b22 6d65 7472 6963 7322 5d3a  ults["metrics"]:
+00010cd0: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
+00010ce0: 5b22 6d65 7472 6963 7322 5d5b 2268 6f73  ["metrics"]["hos
+00010cf0: 7422 5d20 3d20 636f 6e73 7461 6e74 732e  t"] = constants.
+00010d00: 434f 4445 4745 4e5f 5041 594c 4f41 445f  CODEGEN_PAYLOAD_
+00010d10: 5341 4d50 4c45 535f 434c 4541 525f 484f  SAMPLES_CLEAR_HO
+00010d20: 5354 5f44 4546 4155 4c54 5f56 414c 5545  ST_DEFAULT_VALUE
+00010d30: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
+00010d40: 756c 7473 0a0a 6465 6620 6861 6e64 6c65  ults..def handle
+00010d50: 5f66 696c 655f 6e6f 745f 666f 756e 645f  _file_not_found_
+00010d60: 6572 726f 7228 652c 206d 7367 293a 0a20  error(e, msg):. 
+00010d70: 2020 2022 2222 0a20 2020 204c 6f6f 6b73     """.    Looks
+00010d80: 2061 7420 6527 7320 6d65 7373 6167 6520   at e's message 
+00010d90: 6174 7472 6962 7574 6520 616e 6420 6966  attribute and if
+00010da0: 0a20 2020 2069 7420 636f 6e74 6169 6e73  .    it contains
+00010db0: 2045 5252 4f52 5f4e 4f54 5f46 494e 445f   ERROR_NOT_FIND_
+00010dc0: 4449 5220 6f72 2045 5252 4f52 5f4e 4f54  DIR or ERROR_NOT
+00010dd0: 5f46 494e 445f 4649 4c45 0a20 2020 2070  _FIND_FILE.    p
+00010de0: 7269 6e74 7320 6120 4c4f 472e 7761 726e  rints a LOG.warn
+00010df0: 696e 6720 6d65 7373 6167 6520 656c 7365  ing message else
+00010e00: 206a 7573 7420 7261 6973 6573 2074 6865   just raises the
+00010e10: 2065 7863 6570 7469 6f6e 0a0a 2020 2020   exception..    
+00010e20: 3a70 6172 616d 2065 3a20 2872 6571 7569  :param e: (requi
+00010e30: 7265 6429 2061 6e20 4578 6365 7074 696f  red) an Exceptio
+00010e40: 6e0a 2020 2020 3a74 7970 6520 653a 2045  n.    :type e: E
+00010e50: 7863 6570 7469 6f6e 0a20 2020 203a 7061  xception.    :pa
+00010e60: 7261 6d20 6d73 673a 2028 7265 7175 6972  ram msg: (requir
+00010e70: 6564 2920 7468 6520 6375 7374 6f6d 2065  ed) the custom e
+00010e80: 7272 6f72 206d 6573 7361 6765 2074 6f20  rror message to 
+00010e90: 7072 696e 7420 6173 2061 2057 4152 4e49  print as a WARNI
+00010ea0: 4e47 2069 6e20 7468 6520 6c6f 6773 0a20  NG in the logs. 
+00010eb0: 2020 203a 7479 7065 206d 7367 3a20 7374     :type msg: st
+00010ec0: 720a 2020 2020 3a72 6169 7365 733a 2054  r.    :raises: T
+00010ed0: 6865 2065 7863 6570 7469 6f6e 2074 6861  he exception tha
+00010ee0: 7420 6973 2070 6173 7365 6420 756e 6c65  t is passed unle
+00010ef0: 7373 2069 7420 636f 6e74 6169 6e73 0a20  ss it contains. 
+00010f00: 2020 2045 5252 4f52 5f4e 4f54 5f46 494e     ERROR_NOT_FIN
+00010f10: 445f 4449 5220 6f72 2045 5252 4f52 5f4e  D_DIR or ERROR_N
+00010f20: 4f54 5f46 494e 445f 4649 4c45 2069 6e20  OT_FIND_FILE in 
+00010f30: 6974 7320 652e 6d65 7373 6167 650a 2020  its e.message.  
+00010f40: 2020 2222 220a 2020 2020 6966 2063 6f6e    """.    if con
+00010f50: 7374 616e 7473 2e45 5252 4f52 5f4e 4f54  stants.ERROR_NOT
+00010f60: 5f46 494e 445f 4449 5220 6f72 2063 6f6e  _FIND_DIR or con
+00010f70: 7374 616e 7473 2e45 5252 4f52 5f4e 4f54  stants.ERROR_NOT
+00010f80: 5f46 494e 445f 4649 4c45 2069 6e20 652e  _FIND_FILE in e.
+00010f90: 6d65 7373 6167 653a 0a20 2020 2020 2020  message:.       
+00010fa0: 204c 4f47 2e77 6172 6e69 6e67 2822 5741   LOG.warning("WA
+00010fb0: 524e 494e 473a 2025 7322 2c20 6d73 6729  RNING: %s", msg)
+00010fc0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00010fd0: 2020 2072 6169 7365 2065 0a0a 6465 6620     raise e..def 
+00010fe0: 7374 725f 7265 7072 5f61 6374 6976 6174  str_repr_activat
+00010ff0: 696f 6e5f 636f 6e64 6974 696f 6e73 2861  ion_conditions(a
+00011000: 6374 6976 6174 696f 6e5f 636f 6e64 6974  ctivation_condit
+00011010: 696f 6e73 293a 0a20 2020 2022 2222 0a20  ions):.    """. 
+00011020: 2020 2052 6570 7265 7365 6e74 2022 6163     Represent "ac
+00011030: 7469 7661 7469 6f6e 2063 6f6e 6469 7469  tivation conditi
+00011040: 6f6e 7322 2061 7320 6120 7374 7269 6e67  ons" as a string
+00011050: 2e0a 0a20 2020 2045 7861 6d70 6c65 3a0a  ...    Example:.
+00011060: 2020 2020 2020 2020 6163 7469 7661 7469          activati
+00011070: 6f6e 5f63 6f6e 6469 7469 6f6e 7320 3d20  on_conditions = 
+00011080: 7b0a 2020 2020 2020 2020 2020 2020 2263  {.            "c
+00011090: 6f6e 6469 7469 6f6e 7322 3a20 5b0a 2020  onditions": [.  
+000110a0: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+000110b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110c0: 2020 2020 2265 7661 6c75 6174 696f 6e5f      "evaluation_
+000110d0: 6964 223a 204e 6f6e 652c 0a20 2020 2020  id": None,.     
+000110e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000110f0: 6669 656c 645f 6e61 6d65 223a 2022 696e  field_name": "in
+00011100: 6369 6465 6e74 2e69 6422 2c0a 2020 2020  cident.id",.    
+00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011120: 226d 6574 686f 6422 3a20 226e 6f74 5f65  "method": "not_e
+00011130: 7175 616c 7322 2c0a 2020 2020 2020 2020  quals",.        
+00011140: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00011150: 6522 3a20 4e6f 6e65 2c0a 2020 2020 2020  e": None,.      
+00011160: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+00011170: 616c 7565 223a 2031 3233 3435 360a 2020  alue": 123456.  
+00011180: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00011190: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
+000111a0: 2020 2020 2020 2020 2020 2022 6c6f 6769             "logi
+000111b0: 635f 7479 7065 223a 2022 616c 6c22 0a20  c_type": "all". 
+000111c0: 2020 2020 2020 207d 0a0a 0a20 2020 203a         }...    :
+000111d0: 7061 7261 6d20 6163 7469 7661 7469 6f6e  param activation
+000111e0: 5f63 6f6e 6469 7469 6f6e 733a 205f 6465  _conditions: _de
+000111f0: 7363 7269 7074 696f 6e5f 0a20 2020 203a  scription_.    :
+00011200: 7479 7065 2061 6374 6976 6174 696f 6e5f  type activation_
+00011210: 636f 6e64 6974 696f 6e73 3a20 5f74 7970  conditions: _typ
+00011220: 655f 0a20 2020 2022 2222 0a20 2020 2063  e_.    """.    c
+00011230: 6f6e 6469 7469 6f6e 7320 3d20 4f72 6465  onditions = Orde
+00011240: 7265 6444 6963 7428 290a 2020 2020 666f  redDict().    fo
+00011250: 7220 692c 2063 6f6e 6469 7469 6f6e 2069  r i, condition i
+00011260: 6e20 656e 756d 6572 6174 6528 6163 7469  n enumerate(acti
+00011270: 7661 7469 6f6e 5f63 6f6e 6469 7469 6f6e  vation_condition
+00011280: 732e 6765 7428 2263 6f6e 6469 7469 6f6e  s.get("condition
+00011290: 7322 2c20 5b5d 292c 2073 7461 7274 3d31  s", []), start=1
+000112a0: 293a 0a20 2020 2020 2020 2066 6965 6c64  ):.        field
+000112b0: 5f6e 616d 6520 3d20 636f 6e64 6974 696f  _name = conditio
+000112c0: 6e2e 6765 7428 2266 6965 6c64 5f6e 616d  n.get("field_nam
+000112d0: 6522 2920 6f72 2022 220a 2020 2020 2020  e") or "".      
+000112e0: 2020 6d65 7468 6f64 203d 2063 6f6e 6469    method = condi
+000112f0: 7469 6f6e 2e67 6574 2822 6d65 7468 6f64  tion.get("method
+00011300: 2229 206f 7220 2222 0a20 2020 2020 2020  ") or "".       
+00011310: 2076 616c 7565 203d 2063 6f6e 6469 7469   value = conditi
+00011320: 6f6e 2e67 6574 2822 7661 6c75 6522 2920  on.get("value") 
+00011330: 6f72 2022 220a 0a20 2020 2020 2020 2023  or ""..        #
+00011340: 2069 6e64 6578 2069 6e74 6f20 7468 6520   index into the 
+00011350: 6469 6374 696f 6e61 7279 2062 7920 7468  dictionary by th
+00011360: 6520 6576 616c 7561 7469 6f6e 2049 4420  e evaluation ID 
+00011370: 7768 6963 6820 6973 206f 6e6c 7920 7072  which is only pr
+00011380: 6573 656e 740a 2020 2020 2020 2020 2320  esent.        # 
+00011390: 6966 2074 6865 206c 6f67 6963 5f74 7970  if the logic_typ
+000113a0: 6520 6973 2022 6164 7661 6e63 6564 222e  e is "advanced".
+000113b0: 2049 6620 6e6f 7420 7072 6573 656e 7420   If not present 
+000113c0: 2869 2e65 2e20 6c6f 6769 635f 7479 7065  (i.e. logic_type
+000113d0: 3d3d 616e 7920 6f72 2061 6c6c 292c 0a20  ==any or all),. 
+000113e0: 2020 2020 2020 2023 2074 6865 6e20 7765         # then we
+000113f0: 206a 7573 7420 6b65 6570 2074 7261 636b   just keep track
+00011400: 2077 6974 6820 7468 6520 696e 6465 7820   with the index 
+00011410: 696e 2077 6869 6368 2069 7420 7761 7320  in which it was 
+00011420: 666f 756e 6420 696e 2074 6865 206c 6973  found in the lis
+00011430: 740a 2020 2020 2020 2020 2320 4e4f 5445  t.        # NOTE
+00011440: 3a20 7573 6520 6060 6669 6c74 6572 284e  : use ``filter(N
+00011450: 6f6e 652c 205b 2e2e 2e69 7465 6d73 2e2e  one, [...items..
+00011460: 2e5d 2960 6020 6865 7265 2074 6f20 6472  .])`` here to dr
+00011470: 6f70 2061 6e79 2065 6c65 6d65 6e74 7320  op any elements 
+00011480: 7468 6174 206d 6967 6874 0a20 2020 2020  that might.     
+00011490: 2020 2023 2062 6520 4e6f 6e65 2e20 5468     # be None. Th
+000114a0: 6973 2077 6f75 6c64 206f 6363 7572 2069  is would occur i
+000114b0: 6e20 7468 6520 6361 7365 2074 6861 7420  n the case that 
+000114c0: 6120 636f 6e64 6974 696f 6e20 646f 6573  a condition does
+000114d0: 6e27 7420 6861 7665 0a20 2020 2020 2020  n't have.       
+000114e0: 2023 2061 6c6c 2074 6872 6565 2065 6c65   # all three ele
+000114f0: 6d65 6e74 732e 2045 7861 6d70 6c65 3a20  ments. Example: 
+00011500: 2269 6e63 6964 656e 745f 6372 6561 7465  "incident_create
+00011510: 6422 2064 6f65 736e 2774 2068 6176 6520  d" doesn't have 
+00011520: 616e 7920 6d65 7468 6f64 206f 7220 7661  any method or va
+00011530: 6c75 650a 2020 2020 2020 2020 636f 6e64  lue.        cond
+00011540: 6974 696f 6e73 5b63 6f6e 6469 7469 6f6e  itions[condition
+00011550: 2e67 6574 2822 6576 616c 7561 7469 6f6e  .get("evaluation
+00011560: 5f69 6422 2920 6f72 2069 5d20 3d20 7522  _id") or i] = u"
+00011570: 2022 2e6a 6f69 6e28 6669 6c74 6572 284e   ".join(filter(N
+00011580: 6f6e 652c 205b 7374 7228 6669 656c 645f  one, [str(field_
+00011590: 6e61 6d65 292c 2073 7472 286d 6574 686f  name), str(metho
+000115a0: 6429 2c20 7374 7228 7661 6c75 6529 5d29  d), str(value)])
+000115b0: 290a 0a20 2020 2069 6620 7374 7228 6163  )..    if str(ac
+000115c0: 7469 7661 7469 6f6e 5f63 6f6e 6469 7469  tivation_conditi
+000115d0: 6f6e 732e 6765 7428 226c 6f67 6963 5f74  ons.get("logic_t
+000115e0: 7970 6522 2c20 2222 2929 2e6c 6f77 6572  ype", "")).lower
+000115f0: 2829 203d 3d20 2261 6c6c 223a 0a20 2020  () == "all":.   
+00011600: 2020 2020 2072 6574 7572 6e20 7522 2041       return u" A
+00011610: 4e44 2022 2e6a 6f69 6e28 636f 6e64 6974  ND ".join(condit
+00011620: 696f 6e73 2e76 616c 7565 7328 2929 0a20  ions.values()). 
+00011630: 2020 2065 6c69 6620 7374 7228 6163 7469     elif str(acti
+00011640: 7661 7469 6f6e 5f63 6f6e 6469 7469 6f6e  vation_condition
+00011650: 732e 6765 7428 226c 6f67 6963 5f74 7970  s.get("logic_typ
+00011660: 6522 2c20 2222 2929 2e6c 6f77 6572 2829  e", "")).lower()
+00011670: 203d 3d20 2261 6e79 223a 0a20 2020 2020   == "any":.     
+00011680: 2020 2072 6574 7572 6e20 7522 204f 5220     return u" OR 
+00011690: 222e 6a6f 696e 2863 6f6e 6469 7469 6f6e  ".join(condition
+000116a0: 732e 7661 6c75 6573 2829 290a 2020 2020  s.values()).    
+000116b0: 656c 7365 3a0a 2020 2020 2020 2020 636f  else:.        co
+000116c0: 6e64 6974 696f 6e5f 7374 7220 3d20 6163  ndition_str = ac
+000116d0: 7469 7661 7469 6f6e 5f63 6f6e 6469 7469  tivation_conditi
+000116e0: 6f6e 732e 6765 7428 2263 7573 746f 6d5f  ons.get("custom_
+000116f0: 636f 6e64 6974 696f 6e22 290a 2020 2020  condition").    
+00011700: 2020 2020 2320 6865 7265 2077 6520 646f      # here we do
+00011710: 2074 776f 2070 6173 7365 7320 746f 2070   two passes to p
+00011720: 6572 666f 726d 2061 206b 696e 6420 6f66  erform a kind of
+00011730: 2022 7361 6c74 696e 6722 0a20 2020 2020   "salting".     
+00011740: 2020 2023 2074 6869 7320 6973 206e 6563     # this is nec
+00011750: 6573 7361 7279 2074 6f20 6176 6f69 6420  essary to avoid 
+00011760: 7468 6520 636f 6e64 6974 696f 6e20 7768  the condition wh
+00011770: 6572 6520 696e 206f 6e65 2069 7465 7261  ere in one itera
+00011780: 7469 6f6e 0a20 2020 2020 2020 2023 2077  tion.        # w
+00011790: 6520 7265 706c 6163 6520 2231 2220 7769  e replace "1" wi
+000117a0: 7468 2022 3132 3334 2220 616e 6420 6f6e  th "1234" and on
+000117b0: 2074 6865 206e 6578 7420 6974 6572 6174   the next iterat
+000117c0: 696f 6e20 7765 2072 6570 6c61 6365 0a20  ion we replace. 
+000117d0: 2020 2020 2020 2023 2022 3222 2077 6974         # "2" wit
+000117e0: 6820 736f 6d65 7468 696e 6720 656c 7365  h something else
+000117f0: 3b20 696e 2074 6869 7320 6b69 6e64 206f  ; in this kind o
+00011800: 6620 7363 656e 6172 696f 2c20 7765 2764  f scenario, we'd
+00011810: 2062 650a 2020 2020 2020 2020 2320 7265   be.        # re
+00011820: 706c 6163 696e 6720 6120 2232 2220 7768  placing a "2" wh
+00011830: 6963 6820 7765 2064 6964 6e27 7420 7761  ich we didn't wa
+00011840: 6e74 2074 6f0a 2020 2020 2020 2020 2320  nt to.        # 
+00011850: 536f 2069 6e73 7465 6164 2c20 7765 2067  So instead, we g
+00011860: 656e 6572 6174 6520 6120 756e 6971 7565  enerate a unique
+00011870: 2073 616c 7420 616e 640a 2020 2020 2020   salt and.      
+00011880: 2020 2320 7765 2072 6570 6c61 6365 2074    # we replace t
+00011890: 6865 206f 7269 6769 6e61 6c20 6e75 6d62  he original numb
+000118a0: 6572 2077 6974 6820 7468 6174 2e20 7468  er with that. th
+000118b0: 656e 206f 6e20 7468 6520 7365 636f 6e64  en on the second
+000118c0: 2070 6173 732c 0a20 2020 2020 2020 2023   pass,.        #
+000118d0: 2077 6520 7265 706c 6163 6520 7468 6520   we replace the 
+000118e0: 7361 6c74 2077 6974 6820 7468 6520 696e  salt with the in
+000118f0: 7465 6e64 6564 2076 616c 7565 0a20 2020  tended value.   
+00011900: 2020 2020 2023 2049 7420 6973 2061 6c73       # It is als
+00011910: 6f20 4352 5543 4941 4c20 7468 6174 2074  o CRUCIAL that t
+00011920: 6865 206b 6579 7320 6172 6520 7072 6f63  he keys are proc
+00011930: 6573 7365 6420 696e 2072 6576 6572 7365  essed in reverse
+00011940: 206f 7264 6572 0a20 2020 2020 2020 2023   order.        #
+00011950: 2074 6f20 7072 6f70 6572 6c79 2068 616e   to properly han
+00011960: 646c 6520 646f 7562 6c65 2064 6967 6974  dle double digit
+00011970: 2065 7661 6c75 6174 696f 6e20 4944 730a   evaluation IDs.
+00011980: 2020 2020 2020 2020 7361 6c74 7320 3d20          salts = 
+00011990: 7b7d 0a20 2020 2020 2020 2066 6f72 2065  {}.        for e
+000119a0: 7661 6c75 6174 696f 6e5f 6964 2069 6e20  valuation_id in 
+000119b0: 736f 7274 6564 2863 6f6e 6469 7469 6f6e  sorted(condition
+000119c0: 732e 6b65 7973 2829 2c20 7265 7665 7273  s.keys(), revers
+000119d0: 653d 5472 7565 293a 0a20 2020 2020 2020  e=True):.       
+000119e0: 2020 2020 2023 206e 756d 6265 7273 2068       # numbers h
+000119f0: 6572 6520 6172 6520 7468 6520 656e 656d  ere are the enem
+00011a00: 7920 2d2d 2073 6f20 6669 7273 7420 7765  y -- so first we
+00011a10: 206e 6565 6420 746f 206d 6170 2065 6163   need to map eac
+00011a20: 6820 696e 6469 7669 6475 616c 2064 6967  h individual dig
+00011a30: 6974 2074 6f0a 2020 2020 2020 2020 2020  it to.          
+00011a40: 2020 2320 6120 7370 6563 6961 6c20 7374    # a special st
+00011a50: 7269 6e67 2076 616c 7565 2028 4920 6465  ring value (I de
+00011a60: 6369 6465 6420 746f 2075 7365 2074 6865  cided to use the
+00011a70: 2063 6f72 7265 7370 6f6e 6469 6e67 2076   corresponding v
+00011a80: 616c 7565 7320 6f6e 2074 6865 206b 6579  alues on the key
+00011a90: 626f 6172 6429 0a20 2020 2020 2020 2020  board).         
+00011aa0: 2020 2068 6173 6865 645f 6576 616c 5f69     hashed_eval_i
+00011ab0: 6420 3d20 2222 2e6a 6f69 6e28 636f 6e73  d = "".join(cons
+00011ac0: 7461 6e74 732e 5341 4c54 5f48 4153 485f  tants.SALT_HASH_
+00011ad0: 4d41 505b 6964 5d20 666f 7220 6964 2069  MAP[id] for id i
+00011ae0: 6e20 7374 7228 6576 616c 7561 7469 6f6e  n str(evaluation
+00011af0: 5f69 6429 290a 2020 2020 2020 2020 2020  _id)).          
+00011b00: 2020 2320 7468 656e 2061 6464 206f 7572    # then add our
+00011b10: 2075 6e69 7175 6520 2264 6f63 6765 6e5f   unique "docgen_
+00011b20: 7b7d 5f73 616c 7422 2070 7265 6669 7820  {}_salt" prefix 
+00011b30: 746f 2061 6464 2065 7874 7261 2075 6e69  to add extra uni
+00011b40: 7175 656e 6573 730a 2020 2020 2020 2020  queness.        
+00011b50: 2020 2020 2320 4e4f 5445 3a20 756e 6971      # NOTE: uniq
+00011b60: 7565 6e65 7373 2069 7320 6e6f 7420 6775  ueness is not gu
+00011b70: 6172 616e 7465 6564 2068 6572 6520 6672  aranteed here fr
+00011b80: 6f6d 206f 7468 6572 2070 6f73 7369 626c  om other possibl
+00011b90: 6520 7661 6c75 6573 0a20 2020 2020 2020  e values.       
+00011ba0: 2020 2020 2023 2077 6869 6368 2077 6527       # which we'
+00011bb0: 6c6c 2062 6520 7375 6273 7469 7475 7469  ll be substituti
+00011bc0: 6e67 2069 6e2c 2062 7574 2069 7420 6973  ng in, but it is
+00011bd0: 2075 6e6c 696b 656c 7920 7468 6174 2061   unlikely that a
+00011be0: 6e79 6f6e 6520 6861 730a 2020 2020 2020  nyone has.      
+00011bf0: 2020 2020 2020 2320 2264 6f63 6765 6e5f        # "docgen_
+00011c00: 2140 2324 5f73 616c 7422 2069 6e20 7468  !@#$_salt" in th
+00011c10: 6569 7220 7379 7374 656d 2e2e 2e20 736f  eir system... so
+00011c20: 2075 6e69 7175 656e 6573 7320 6973 2070   uniqueness is p
+00011c30: 7261 6374 6963 616c 6c79 2067 7561 7261  ractically guara
+00011c40: 6e74 6565 640a 2020 2020 2020 2020 2020  nteed.          
+00011c50: 2020 7361 6c74 735b 6576 616c 7561 7469    salts[evaluati
+00011c60: 6f6e 5f69 645d 203d 2063 6f6e 7374 616e  on_id] = constan
+00011c70: 7473 2e44 4f43 4745 4e5f 5341 4c54 5f50  ts.DOCGEN_SALT_P
+00011c80: 5245 4649 582e 666f 726d 6174 2868 6173  REFIX.format(has
+00011c90: 6865 645f 6576 616c 5f69 6429 0a20 2020  hed_eval_id).   
+00011ca0: 2020 2020 2020 2020 2063 6f6e 6469 7469           conditi
+00011cb0: 6f6e 5f73 7472 203d 2063 6f6e 6469 7469  on_str = conditi
+00011cc0: 6f6e 5f73 7472 2e72 6570 6c61 6365 2873  on_str.replace(s
+00011cd0: 7472 2865 7661 6c75 6174 696f 6e5f 6964  tr(evaluation_id
+00011ce0: 292c 2073 616c 7473 2e67 6574 2865 7661  ), salts.get(eva
+00011cf0: 6c75 6174 696f 6e5f 6964 2929 0a20 2020  luation_id)).   
+00011d00: 2020 2020 2066 6f72 2065 7661 6c75 6174       for evaluat
+00011d10: 696f 6e5f 6964 2069 6e20 636f 6e64 6974  ion_id in condit
+00011d20: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
+00011d30: 2020 636f 6e64 6974 696f 6e5f 7374 7220    condition_str 
+00011d40: 3d20 636f 6e64 6974 696f 6e5f 7374 722e  = condition_str.
+00011d50: 7265 706c 6163 6528 7361 6c74 732e 6765  replace(salts.ge
+00011d60: 7428 6576 616c 7561 7469 6f6e 5f69 6429  t(evaluation_id)
+00011d70: 2c20 636f 6e64 6974 696f 6e73 2e67 6574  , conditions.get
+00011d80: 2865 7661 6c75 6174 696f 6e5f 6964 2929  (evaluation_id))
+00011d90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011da0: 636f 6e64 6974 696f 6e5f 7374 720a 0a63  condition_str..c
+00011db0: 6c61 7373 2043 6f6e 7465 7874 4d61 6e67  lass ContextMang
+00011dc0: 6572 466f 7254 656d 706f 7261 7279 4469  erForTemporaryDi
+00011dd0: 7265 6374 6f72 7928 293a 0a20 2020 2022  rectory():.    "
+00011de0: 2222 0a20 2020 2054 6869 7320 6973 2061  "".    This is a
+00011df0: 2073 6d61 6c6c 2063 6c61 7373 2066 6f72   small class for
+00011e00: 2073 6166 6520 7573 6520 6f66 2060 6074   safe use of ``t
+00011e10: 656d 7066 696c 652e 6d6b 6474 656d 7028  empfile.mkdtemp(
+00011e20: 2960 6020 7768 6963 6820 7265 7175 6972  )`` which requir
+00011e30: 6573 2063 6c65 616e 7570 2061 6674 6572  es cleanup after
+00011e40: 0a20 2020 2075 7365 2e20 5468 6520 636c  .    use. The cl
+00011e50: 6173 7320 6566 6665 6374 6976 656c 7920  ass effectively 
+00011e60: 6973 2074 6865 2073 616d 6520 6173 2060  is the same as `
+00011e70: 6074 656d 7066 696c 652e 5465 6d70 6f72  `tempfile.Tempor
+00011e80: 6172 7944 6972 6563 746f 7279 6060 2c20  aryDirectory``, 
+00011e90: 686f 7765 7665 722c 0a20 2020 2074 6861  however,.    tha
+00011ea0: 7420 636c 6173 7320 6973 6e27 7420 6176  t class isn't av
+00011eb0: 6169 6c61 626c 6520 6265 666f 7265 2070  ailable before p
+00011ec0: 7974 686f 6e20 3320 7468 7573 2074 6865  ython 3 thus the
+00011ed0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
+00011ee0: 6865 7265 2e0a 2020 2020 4f6e 2065 6e74  here..    On ent
+00011ef0: 6572 2c20 6060 7465 6d70 6669 6c65 2e6d  er, ``tempfile.m
+00011f00: 6b64 7465 6d70 282a 6172 6773 2c20 2a2a  kdtemp(*args, **
+00011f10: 6b77 6172 6773 2960 6020 6973 2063 616c  kwargs)`` is cal
+00011f20: 6c65 6420 616e 6420 6f6e 2065 7869 7420  led and on exit 
+00011f30: 6060 7368 7574 696c 2e72 6d74 7265 6528  ``shutil.rmtree(
+00011f40: 7061 7468 5f74 6f5f 6469 7229 6060 2069  path_to_dir)`` i
+00011f50: 7320 6361 6c6c 6564 2e0a 0a20 2020 2045  s called...    E
+00011f60: 7861 6d70 6c65 3a0a 0a20 2020 202e 2e20  xample:..    .. 
+00011f70: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
+00011f80: 686f 6e0a 2020 2020 2020 2020 2320 6372  hon.        # cr
+00011f90: 6561 7465 2074 6865 2063 6f6e 7465 7874  eate the context
+00011fa0: 206d 616e 6167 6572 2075 7369 6e67 2074   manager using t
+00011fb0: 6865 2027 7769 7468 202e 2e2e 2061 733a  he 'with ... as:
+00011fc0: 2720 7374 6174 656d 656e 740a 2020 2020  ' statement.    
+00011fd0: 2020 2020 2320 6f6e 2063 7265 6174 696f      # on creatio
+00011fe0: 6e20 6f66 2074 6865 2027 7061 7468 5f74  n of the 'path_t
+00011ff0: 6f5f 746d 705f 6469 7227 206f 626a 6563  o_tmp_dir' objec
+00012000: 742c 2074 6865 2060 605f 5f65 6e74 6572  t, the ``__enter
+00012010: 5f5f 6060 206d 6574 686f 6420 6973 2063  __`` method is c
+00012020: 616c 6c65 640a 0a20 2020 2020 2020 2077  alled..        w
+00012030: 6974 6820 7364 6b5f 6865 6c70 6572 732e  ith sdk_helpers.
+00012040: 436f 6e74 6578 744d 616e 6765 7246 6f72  ContextMangerFor
+00012050: 5465 6d70 6f72 6172 7944 6972 6563 746f  TemporaryDirecto
+00012060: 7279 2829 2061 7320 7061 7468 5f74 6f5f  ry() as path_to_
+00012070: 746d 705f 6469 723a 0a20 2020 2020 2020  tmp_dir:.       
+00012080: 2020 2020 2023 202e 2e2e 0a20 2020 2020       # ....     
+00012090: 2020 2020 2020 2023 2064 6f20 736f 6d65         # do some
+000120a0: 7468 696e 6720 7769 7468 2070 6174 685f  thing with path_
+000120b0: 746f 5f74 6d70 5f64 6972 0a20 2020 2020  to_tmp_dir.     
+000120c0: 2020 2020 2020 2023 202e 2e2e 0a0a 2020         # .....  
+000120d0: 2020 2020 2020 2320 6f6e 2065 7869 7420        # on exit 
+000120e0: 6f66 2063 6f6e 7465 7874 206d 616e 6167  of context manag
+000120f0: 6572 2c20 7061 7468 5f74 6f5f 746d 705f  er, path_to_tmp_
+00012100: 6469 7220 7769 6c6c 2062 6520 636c 6561  dir will be clea
+00012110: 6e65 6420 7570 2062 7920 696d 706c 6963  ned up by implic
+00012120: 6974 2063 616c 6c20 6f66 2074 6865 2060  it call of the `
+00012130: 605f 5f65 7869 745f 5f60 6020 6d65 7468  `__exit__`` meth
+00012140: 6f64 0a0a 2020 2020 3a70 6172 616d 2061  od..    :param a
+00012150: 7267 733a 2061 6e79 206f 7264 6572 6564  rgs: any ordered
+00012160: 2061 7267 7320 7468 6174 2061 7265 2072   args that are r
+00012170: 656c 6576 616e 7420 746f 2063 616c 6c69  elevant to calli
+00012180: 6e67 2060 6074 656d 7066 696c 652e 6d6b  ng ``tempfile.mk
+00012190: 6474 656d 7028 2960 600a 2020 2020 3a70  dtemp()``.    :p
+000121a0: 6172 616d 206b 7761 7267 733a 2061 6e79  aram kwargs: any
+000121b0: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
+000121c0: 7473 2072 656c 6576 616e 7420 746f 2063  ts relevant to c
+000121d0: 616c 6c69 6e67 2060 6074 656d 7066 696c  alling ``tempfil
+000121e0: 652e 6d6b 6474 656d 7028 2960 600a 2020  e.mkdtemp()``.  
+000121f0: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
+00012200: 5f69 6e69 745f 5f28 7365 6c66 2c20 2a61  _init__(self, *a
+00012210: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
+00012220: 2020 2020 2020 2020 7365 6c66 2e64 6972          self.dir
+00012230: 203d 2074 656d 7066 696c 652e 6d6b 6474   = tempfile.mkdt
+00012240: 656d 7028 2a61 7267 732c 202a 2a6b 7761  emp(*args, **kwa
+00012250: 7267 7329 0a0a 2020 2020 6465 6620 5f5f  rgs)..    def __
+00012260: 656e 7465 725f 5f28 7365 6c66 293a 0a20  enter__(self):. 
+00012270: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00012280: 6c66 2e64 6972 0a0a 2020 2020 6465 6620  lf.dir..    def 
+00012290: 5f5f 6578 6974 5f5f 2873 656c 662c 2065  __exit__(self, e
+000122a0: 7863 5f74 7970 652c 2065 7863 5f76 616c  xc_type, exc_val
+000122b0: 7565 2c20 6578 635f 7472 6163 6562 6163  ue, exc_tracebac
+000122c0: 6b29 3a0a 2020 2020 2020 2020 7368 7574  k):.        shut
+000122d0: 696c 2e72 6d74 7265 6528 7365 6c66 2e64  il.rmtree(self.d
+000122e0: 6972 290a                                ir).
```

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_validate_configs.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_validate_configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,18 +130,18 @@
 # NOTE: selftest_attributes needs to be a list as the order of these checks MATTERS
 selftest_attributes = [
     { # check 1: verify that resilient-circuits is installed in python env
         "func": sdk_validate_helpers.selftest_validate_resilient_circuits_installed,
         "name": "resilient-circuits selftest",
 
         "fail_msg": "'{0}=={1}' is not supported".format(constants.CIRCUITS_PACKAGE_NAME, "{0}"),
-        "fail_solution": "Upgrade '{0}' by running '''pip install -U '{0}>={1}''''".format(constants.CIRCUITS_PACKAGE_NAME, constants.RESILIENT_LIBRARIES_VERSION),
+        "fail_solution": "Upgrade '{0}' by running '''pip install -U {0}'''".format(constants.CIRCUITS_PACKAGE_NAME),
 
         "missing_msg": "'{0}' is not installed in your Python environment".format(constants.CIRCUITS_PACKAGE_NAME),
-        "missing_solution": "Install '{0}' by running '''pip install -U '{0}''''".format(constants.CIRCUITS_PACKAGE_NAME),
+        "missing_solution": "Install '{0}' by running '''pip install -U {0}'''".format(constants.CIRCUITS_PACKAGE_NAME),
 
         "severity": SDKValidateIssue.SEVERITY_LEVEL_CRITICAL,
 
         "pass_msg": "'{0}' was found in the Python environment with the minimum version installed".format(constants.CIRCUITS_PACKAGE_NAME)
     },
     { # check 2: check that the given package is acutally installed in the env
         "func": sdk_validate_helpers.selftest_validate_package_installed,
@@ -293,22 +293,43 @@
         "fail_msg_sub_playbooks_input": u"Input script for a subplaybook in playbook '{0}' packaged with this app is written in Python 2",
         "fail_msg_sub_playbooks_output": u"Output script for subplaybook '{0}' packaged with this app is written in Python 2",
         "fail_msg_pre_processing": u"Pre-processing script for workflow '{0}' packaged with this app is written in Python 2",
         "fail_msg_post_processing": u"Post-processing script for workflow '{0}' packaged with this app is written in Python 2",
         "fail_severity": SDKValidateIssue.SEVERITY_LEVEL_CRITICAL,
         "fail_solution": "Python 2 will soon no longer be supported in SOAR. Update the language of the script to Python 3, being careful to make sure that it is still fully functional",
 
-        "missing_msg": "'customize.py' not found in package at path '{0}'",
+        "missing_msg": "'customize.py' or 'export.res' not found in package at path '{0}'",
         "missing_severity": SDKValidateIssue.SEVERITY_LEVEL_CRITICAL,
         "missing_solution": "Reload code using '''resilient-sdk codegen -p {0} --reload'''",
 
         "pass_msg": "Scripts in app use valid versions of Python",
         "pass_solution": "All scripts are written in Python 3. Be careful to make any new scripts in Python 3 only"
     }),
 
+    ("export.res", {
+        "func": sdk_validate_helpers.package_files_validate_no_playbook_dependencies_missing,
+        "path": "{0}/util/customize.py",
+        "name": "'Playbooks dependencies'",
+
+        "fail_msg": u"App includes playbook '{0}' which references field(s) '{1}' that are not included in the package",
+        "fail_msg_functions": u"App includes playbook '{0}' which references function UUID(s) '{1}' that are not included in the package",
+        "fail_msg_scripts": u"App includes playbook '{0}' which references scripts UUIDs '{1}' that are not included in the package",
+        "fail_severity": SDKValidateIssue.SEVERITY_LEVEL_CRITICAL,
+        "fail_solution": u"Reload your app to include the missing fields: '''resilient-sdk codegen -p {0} --reload --field {1}'''",
+        "fail_solution_functions": u"Reload your app to include the missing functions: '''resilient-sdk codegen -p {0} --reload'''",
+        "fail_solution_scripts": u"Reload your app to include the missing scripts: '''resilient-sdk codegen -p {0} --reload'''",
+
+        "missing_msg": u"'customize.py' or 'export.res' not found in package at path '{0}'",
+        "missing_severity": SDKValidateIssue.SEVERITY_LEVEL_CRITICAL,
+        "missing_solution": u"Reload code using '''resilient-sdk codegen -p {0} --reload'''",
+
+        "pass_msg": "App has no missing dependencies in its packaged playbooks",
+        "pass_solution": "All fields referenced in playbooks are included in the app. Be careful to include any new fields in the app when adding them to parts of the playbook"
+    }),
+
     ("README.md", {
         "func": sdk_validate_helpers.package_files_validate_readme,
         "name": "'README.md'",
 
         "fail_codegen_msg": "'README.md' is still the 'codegen' template",
         "fail_codegen_severity": SDKValidateIssue.SEVERITY_LEVEL_CRITICAL,
         "fail_codegen_solution": "Be sure that you run '''resilient-sdk docgen -p {0}''' when you are done developing",
```

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_validate_helpers.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_validate_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # in py2 StringIO is base module for StringIO
 # in py3 io is the base module for StringIO
 if sys.version_info.major < 3:
     from StringIO import StringIO
 else:
     from io import StringIO
 
-import pkg_resources
+from packaging.version import parse
 from resilient_sdk.util import constants
 from resilient_sdk.util import package_file_helpers as package_helpers
 from resilient_sdk.util import sdk_helpers
 from resilient_sdk.util.sdk_exception import SDKException
 from resilient_sdk.util.sdk_validate_issue import SDKValidateIssue
 
 LOG = logging.getLogger(constants.LOGGER_NAME)
@@ -94,23 +94,23 @@
     :rtype: (bool, SDKValidateIssue)
     """
     LOG.debug("validating that 'resilient-circuits' is installed in the env...\n")
 
 
     res_circuits_version = sdk_helpers.get_package_version(constants.CIRCUITS_PACKAGE_NAME)
 
-    if res_circuits_version and res_circuits_version >= pkg_resources.parse_version(constants.RESILIENT_LIBRARIES_VERSION):
+    if res_circuits_version and res_circuits_version >= parse(constants.RESILIENT_LIBRARIES_VERSION):
         # installed and correct version
         return True, SDKValidateIssue(
             name=attr_dict.get("name"),
             description=attr_dict.get("pass_msg"),
             severity=SDKValidateIssue.SEVERITY_LEVEL_DEBUG,
             solution=""
         )
-    elif res_circuits_version and res_circuits_version < pkg_resources.parse_version(constants.RESILIENT_LIBRARIES_VERSION):
+    elif res_circuits_version and res_circuits_version < parse(constants.RESILIENT_LIBRARIES_VERSION):
         # resilient-circuits installed but version not supported
         return False, SDKValidateIssue(
             name=attr_dict.get("name"),
             description=attr_dict.get("fail_msg").format(res_circuits_version),
             severity=attr_dict.get("severity"),
             solution=attr_dict.get("fail_solution")
         )
@@ -708,14 +708,97 @@
             description=attr_dict.get("pass_msg"),
             severity=SDKValidateIssue.SEVERITY_LEVEL_DEBUG,
             solution=attr_dict.get("pass_solution")
         )]
     else:
         return issues
 
+def package_files_validate_no_playbook_dependencies_missing(path_file, path_package, attr_dict, **_):
+    try:
+        # parse import definition information from customize.py file
+        # this will raise an SDKException if something goes wrong
+        export_res = package_helpers.get_import_definition_from_customize_py(path_file)
+    except SDKException:
+        # something went wrong in reading the import definition.
+        # since this is already checked in another function elsewhere,
+        # ignore and return an empty list
+        return []
+
+    issues = _validate_playbook_conditions_all_fields_included(export_res, attr_dict, path_package)
+    issues.extend(_validate_playbook_conditions_all_functions_included(export_res, attr_dict, path_package))
+
+    if not issues:
+        return [SDKValidateIssue(
+            name=attr_dict.get("name"),
+            description=attr_dict.get("pass_msg"),
+            severity=SDKValidateIssue.SEVERITY_LEVEL_DEBUG,
+            solution=attr_dict.get("pass_solution")
+        )]
+    else:
+        return issues
+
+def _validate_playbook_conditions_all_fields_included(export_res, attr_dict, path_package):
+    issues = []
+    packaged_field_names = [o.get("export_key").split("/")[-1] for o in export_res.get("fields", [])]
+
+    # validate GLOBAL scripts are all python3 only.
+    # for each non-python3 script we find, create an issue
+    for playbook in export_res.get("playbooks") or []:
+        missing_fields_for_pb = []
+
+        # run through the fields in the activation conditions
+        activation_details = playbook.get("activation_details", {}).get("activation_conditions", {}).get("conditions", []) or []
+        cancellation_details = playbook.get("auto_cancelation_details", {}).get("cancelation_conditions", {}).get("conditions", []) or []
+        details = [activation_details, cancellation_details]
+        for pb_conditions in details:
+            for condition in pb_conditions:
+                field_name = condition.get("field_name") or ""
+                field_name_split = field_name.split(".", 2)
+                if len(field_name_split) > 1 and field_name_split[1] == "properties" and field_name_split[-1] not in packaged_field_names:
+                    missing_fields_for_pb.append(field_name_split[-1])
+
+        # if any missing fields, create validate issue for them
+        if missing_fields_for_pb:
+            issues.append(SDKValidateIssue(
+                name=attr_dict.get("name"),
+                description=attr_dict.get("fail_msg").format(playbook.get("display_name", "UNKNOWN PLAYBOOK NAME"), ", ".join(missing_fields_for_pb)),
+                severity=attr_dict.get("fail_severity"),
+                solution=attr_dict.get("fail_solution").format(path_package, " ".join(missing_fields_for_pb))
+            ))
+
+    return issues
+
+def _validate_playbook_conditions_all_functions_included(export_res, attr_dict, path_package):
+    issues = []
+
+
+    for playbook in export_res.get("playbooks") or []:
+
+        # This gets all the functions and scripts in the Playbooks's XML
+        pb_objects = sdk_helpers.get_playbook_objects(playbook)
+
+        # find any missing functions
+        missing_fn_uuids = []
+        for pb_fn in pb_objects.get("functions", []):
+            pb_fn_not_found = len([fn for fn in export_res["functions"] if pb_fn.get("uuid", "uuid_not_found_pb") == fn.get("uuid", "uuid_not_found_fn")]) == 0
+
+            if pb_fn_not_found:
+                missing_fn_uuids.append(pb_fn.get("uuid"))
+
+
+        if missing_fn_uuids:
+            issues.append(SDKValidateIssue(
+                name=attr_dict.get("name"),
+                description=attr_dict.get("fail_msg_functions").format(playbook.get("display_name", "UNKNOWN PLAYBOOK NAME"), ", ".join(missing_fn_uuids)),
+                severity=attr_dict.get("fail_severity"),
+                solution=attr_dict.get("fail_solution_functions").format(path_package)
+            ))
+
+    return issues
+
 def package_files_validate_icon(path_file, attr_dict, filename, **__):
     """
     Helper method for package files to validate an icon
     This works by using the get_icon helper method from package_file_helpers.
     That method loads in a given icon, checks the contents for the correct size,
     and returns the contents if the file is valid.
 
@@ -1001,14 +1084,15 @@
             )]
 
         else: # if only one FROM command is found but it is correct
             issues = [SDKValidateIssue(
                 attr_dict.get("name"),
                 attr_dict.get("pass_msg"),
                 severity=SDKValidateIssue.SEVERITY_LEVEL_DEBUG,
+                solution=""
             )]
 
     elif len(command_dict[from_command]) > 1: # if more than one FROM command found
 
         issues = [SDKValidateIssue(
             attr_dict.get("name"),
             attr_dict.get("fail_msg").format("More than one FROM command found"),
```

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk/util/sdk_validate_issue.py` & `resilient_sdk-51.0.2.0.974/resilient_sdk/util/sdk_validate_issue.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/PKG-INFO` & `resilient_sdk-51.0.2.0.974/resilient_sdk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 Metadata-Version: 2.1
-Name: resilient-sdk
-Version: 51.0.1.1.824
+Name: resilient_sdk
+Version: 51.0.2.0.974
 Summary: Python SDK for developing Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-sdk
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
 Project-URL: Change Log, https://ibm.biz/resilient-sdk-changes
 Keywords: ibm,soar,resilient,resilient-circuits,circuits,resilient-sdk,sdk
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.12,>=2.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7
 Description-Content-Type: text/markdown; charset=UTF-8
+Requires-Dist: resilient>=51.0.2.0
+Requires-Dist: packaging~=24.0; python_version > "3.6"
+Requires-Dist: jinja2~=3.1; python_version > "3.6"
+Requires-Dist: genson~=1.3; python_version > "3.6"
+Requires-Dist: packaging~=21.3; python_version == "3.6"
+Requires-Dist: jinja2~=3.0; python_version == "3.6"
+Requires-Dist: genson==1.2; python_version <= "3.6"
+Requires-Dist: jinja2~=2.0; python_version == "2.7"
+Requires-Dist: packaging~=20.9; python_version == "2.7"
 
 ![IBM Security](https://raw.githubusercontent.com/ibmresilient/resilient-python-api/master/resilient-sdk/assets/IBM_Security_lockup_pos_RGB.png)
 
 # IBM SOAR SDK
 
 
 ## Overview
```

### Comparing `resilient_sdk-51.0.1.1.824/resilient_sdk.egg-info/SOURCES.txt` & `resilient_sdk-51.0.2.0.974/resilient_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/setup.cfg` & `resilient_sdk-51.0.2.0.974/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -11,32 +11,33 @@
 	IBM Community = https://ibm.biz/soarcommunity
 	Change Log = https://ibm.biz/resilient-sdk-changes
 classifiers = 
 	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 keywords = ibm, soar, resilient, resilient-circuits, circuits, resilient-sdk, sdk
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.12
+python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient >= 51.0.1.1
+	resilient >= 51.0.2.0
 	
-	genson    ~= 1.2
-	
-	packaging ~= 23.2; python_version > "3.6"
+	packaging ~= 24.0; python_version > "3.6"
 	jinja2    ~= 3.1;  python_version > "3.6"
+	genson    ~= 1.3;  python_version > "3.6"
 	
 	packaging ~= 21.3; python_version == "3.6"
 	jinja2    ~= 3.0;  python_version == "3.6"
+	genson    == 1.2;  python_version <= "3.6"
 	
 	jinja2    ~= 2.0;  python_version == "2.7"
 	packaging ~= 20.9; python_version == "2.7"
 
 [options.entry_points]
 console_scripts = 
 	resilient-sdk = resilient_sdk.app:main
```

### Comparing `resilient_sdk-51.0.1.1.824/tests/conftest.py` & `resilient_sdk-51.0.2.0.974/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,17 +482,17 @@
     """
     Before: Change the app.config file path to point to the test temp directory
     After: Change the app.config file path back to the original value
     """
     _mk_temp_dir()
     old_config_file_path = constants.PATH_RES_DEFAULT_APP_CONFIG
     constants.PATH_RES_DEFAULT_APP_CONFIG = os.path.join(mock_paths.TEST_TEMP_DIR, "app.config")
-    
+
     yield
-    
+
     _rm_temp_dir()
     constants.PATH_RES_DEFAULT_APP_CONFIG = old_config_file_path
 
 @pytest.fixture
 def fx_mock_settings_file_path():
     """
     Before: Change the settings file path to point to the test temp directory
@@ -551,14 +551,33 @@
     ]
 
     args = _add_to_cmd_line_args(args_to_add)
 
     yield args
 
     sys.argv = original_cmd_line
+
+@pytest.fixture
+def fx_cmd_line_args_docgen_two_export_files():
+    """
+    Before: adds args_to_add to cmd line so can be accessed by ArgParsers
+    After: Set the cmd line args back to its original value
+    """
+    original_cmd_line = copy.deepcopy(sys.argv)
+
+    args_to_add = [
+        "docgen",
+        "-e", mock_paths.MOCK_EXPORT_RES, mock_paths.MOCK_EXPORT_RES_W_PLAYBOOK, mock_paths.MOCK_PYTEST_XML_REPORT_PATH
+    ]
+
+    args = _add_to_cmd_line_args(args_to_add)
+
+    yield args
+
+    sys.argv = original_cmd_line
 
 @pytest.fixture
 def fx_cmd_line_args_clone_typechange():
     """
     Before: adds args_to_add to cmd line so can be accessed by ArgParsers
 
     Sets 2 args for clone, a workflow to clone and a new type for the workflow
```

### Comparing `resilient_sdk-51.0.1.1.824/tests/helpers.py` & `resilient_sdk-51.0.2.0.974/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/integration/test_installation.py` & `resilient_sdk-51.0.2.0.974/tests/integration/test_installation.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/.mock_sdk_settings.json` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/.mock_sdk_settings.json`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/README.md` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/README.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_app.log` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_app.log`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_export.res` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_export.resz` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_export.resz`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_export_corrupt.res` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_export_corrupt.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/config.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/config.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/customize.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/customize.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/customize_old.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/customize_old.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_export_w_playbook_w_scripts.res` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_export_w_playbook_w_scripts.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile.old` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile.old`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/setup.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/setup.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/setup_callable_data.txt` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/setup_callable_data.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_package_files/setup_py_lines.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_package_files/setup_py_lines.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_reload_export.res` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_reload_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/mock_xml_test_report.xml` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/mock_xml_test_report.xml`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/export.JSON` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/resilient_api_data/export.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/orgs.JSON` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/resilient_api_data/orgs.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_data/session.JSON` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/resilient_api_data/session.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/resilient_api_mock.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/resilient_api_mock.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/shared_mock_data/sdk_mock_paths.py` & `resilient_sdk-51.0.2.0.974/tests/shared_mock_data/sdk_mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_app.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_app.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # (c) Copyright IBM Corp. 2010, 2022. All Rights Reserved.
 
 
 import argparse
 import sys
 
-import pkg_resources
+from packaging.version import parse
 import pytest
 import resilient_sdk.app as app
 from mock import MagicMock, patch
 from resilient_sdk.util import constants
 
 
 def test_get_main_app_parser():
@@ -36,16 +36,16 @@
     assert sub_parser.dest == "cmd"
     assert sub_parser.container.description == "one of these subcommands must be provided"
     assert sub_parser.container.title == "subcommands"
 
 
 @pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY_VERSION, reason="requires python3.6 or higher")
 @patch.multiple("resilient_sdk.app.sdk_helpers",
-                get_resilient_sdk_version=MagicMock(return_value=pkg_resources.parse_version("40.0.0")),
-                get_latest_available_version=MagicMock(return_value=pkg_resources.parse_version("41.0.0")))
+                get_resilient_sdk_version=MagicMock(return_value=parse("40.0.0")),
+                get_latest_available_version=MagicMock(return_value=parse("41.0.0")))
 def test_main_print_version_warning(caplog):
 
     with pytest.raises(SystemExit):
         app.main()
 
     msg = "WARNING:\n'40.0.0' is not the latest version of the resilient-sdk. \
 'v41.0.0' is available on https://pypi.org/project/resilient-sdk/\n\n\
```

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/ext/test_ext_package.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/ext/test_ext_package.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_base_cmd.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_base_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_clone.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_clone.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_codegen.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_codegen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_dev.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_dev.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_docgen.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_docgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,7 +367,18 @@
     fx_cmd_line_args_docgen_export_file.extend(["-o", os.path.join(fx_mk_os_tmp_dir, "README.md")])
 
     cmd_docgen.execute_command(cmd_docgen.parser.parse_known_args()[0])
 
     assert "Rendering README for" in caplog.text
     assert "mock_xml_test_report.xml' was skipped for 'docgen --export' because it was not in the proper" in caplog.text
     assert "Writing README to" in caplog.text
+
+def test_execute_command_for_two_exports(fx_get_sub_parser, fx_cmd_line_args_docgen_two_export_files, fx_mk_os_tmp_dir, caplog):
+    cmd_docgen = CmdDocgen(fx_get_sub_parser)
+    # create tmp directory so that we don't overwrite repo's default README when we run this locally
+    fx_cmd_line_args_docgen_two_export_files.extend(["-o", os.path.join(fx_mk_os_tmp_dir, "README.md")])
+
+    cmd_docgen.execute_command(cmd_docgen.parser.parse_known_args()[0])
+
+    assert "Rendering README for" in caplog.text
+    assert "mock_xml_test_report.xml' was skipped for 'docgen --export' because it was not in the proper" in caplog.text
+    assert "Writing README to" in caplog.text
```

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_extract.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_extract.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_list.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_list.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_run_init.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_run_init.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_cmds/test_validate.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_cmds/test_validate.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_jinja_filters.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_jinja_filters.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,19 +39,27 @@
 
     filtered_text = jinja2_filters._scrub_ansi(mock_text)
 
     assert filtered_text == u"some green text"
 
 
 def test_convert_to_code():
-    mock_text = "'''pip install -U 'resilient-circuits''''"
+    mock_text = "'''pip install -U resilient-circuits'''"
 
     filtered_text = jinja2_filters._convert_to_code(mock_text)
 
-    assert "```shell\n$ pip install -U \"resilient-circuits\"\n```" in filtered_text
+    assert filtered_text == "\n\n```shell\n$ pip install -U resilient-circuits\n```\n"
+
+
+def test_convert_to_code_long_block():
+    mock_text = "Resilient-circuits is out of date. You can upgrade it by running: '''pip install -U resilient-circuits''' and making sure that it is the latest version"
+
+    filtered_text = jinja2_filters._convert_to_code(mock_text)
+
+    assert filtered_text == "Resilient-circuits is out of date. You can upgrade it by running: \n\n```shell\n$ pip install -U resilient-circuits\n```\n and making sure that it is the latest version"
 
 
 def test_defaults_to_code():
     mock_text = "<<example url>>"
 
     filtered_text = jinja2_filters._defaults_to_code(mock_text)
```

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_package_file_helpers.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_package_file_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 # -*- coding: utf-8 -*-
 # (c) Copyright IBM Corp. 2010, 2024. All Rights Reserved.
 
 import io
 import json
 import os
 import shutil
+import sys
 
 import pytest
+import tests.shared_mock_data.sdk_mock_paths as mock_paths
 from mock import patch
 from resilient_sdk.util import constants
 from resilient_sdk.util import package_file_helpers as package_helpers
 from resilient_sdk.util import sdk_helpers
 from resilient_sdk.util.sdk_exception import SDKException
 from setuptools import sandbox as use_setuptools
-import tests.shared_mock_data.sdk_mock_paths as mock_paths
 
 
 def test_get_setup_callable():
     # Test callable section returned correctly.
     # Read the mock setup.py content.
     setup_content = sdk_helpers.read_file(mock_paths.MOCK_SETUP_PY)
     setup_callable = package_helpers.get_setup_callable(setup_content)
@@ -459,7 +460,29 @@
     assert export_content
     assert len(export_content["workflows"]) == 2 # just a simple check
 
 def test_get_export_from_zip_not_found():
     with pytest.raises(SDKException):
         package_helpers.get_export_from_zip(mock_paths.MOCK_EXPORT_RES) # not a zip file
 
+
+@pytest.mark.skipif(sys.version_info < constants.MIN_SUPPORTED_PY_VERSION, reason="requires python3.6 or higher to do list of dictionary == check")
+@pytest.mark.parametrize("list_dicts, has_duplicates, optional_lambda",
+    [([
+        {"x": 1, "y": 2, "z": 3},
+        {"a": 4, "b": 5, "c": 6},
+        {"x": 1, "y": 2, "z": 3}
+    ], True, None),
+    ([
+        {"x": 1, "y": 2, "z": 3},
+        {"a": 4, "b": 5, "c": 6}
+    ], False, None),
+    ([
+        {"x": 1, "y": 2, "z": 3},
+        {"x": 4, "b": 5, "c": 6},
+        {"x": 10, "y": 2, "z": 3}
+    ], False, lambda x: x["x"])
+])
+def test_make_list_of_dicts_unique(list_dicts, has_duplicates, optional_lambda):
+
+    result = package_helpers.make_list_of_dicts_unique(list_dicts, optional_lambda)
+    assert (result != list_dicts) == has_duplicates
```

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_resilient_objects.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_resilient_objects.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_exception.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_helpers.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_sdk_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import re
 import shutil
 import stat
 import sys
 import tempfile
 
 import jinja2
-import pkg_resources
 import pytest
 import requests_mock
 from mock import patch
 from packaging.version import parse as parse_version
 from resilient_sdk.cmds import CmdCodegen, CmdValidate
 from resilient_sdk.util import constants, sdk_helpers
 from resilient_sdk.util.resilient_objects import ResilientObjMap
@@ -59,15 +58,15 @@
 
     file_lines = sdk_helpers.read_file(temp_file)
     assert mock_data.mock_file_contents in file_lines
 
 
 def test_write_latest_pypi_tmp_file(fx_mk_temp_dir):
     mock_file_path = os.path.join(mock_paths.TEST_TEMP_DIR, "mock_path_sdk_tmp_pypi_version.json")
-    mock_version = pkg_resources.parse_version("45.0.0")
+    mock_version = parse_version("45.0.0")
     sdk_helpers.write_latest_pypi_tmp_file(mock_version, mock_file_path)
 
     file_contents = sdk_helpers.read_json_file(mock_file_path)
 
     assert file_contents.get("ts")
     assert file_contents.get("version") == "45.0.0"
 
@@ -574,20 +573,20 @@
 
 def test_get_resilient_libraries_version_to_use_dev(fx_add_dev_env_var):
     assert sdk_helpers.get_resilient_libraries_version_to_use() == constants.RESILIENT_LIBRARIES_VERSION_DEV
 
 def test_get_resilient_sdk_version():
     parsed_version = sdk_helpers.get_resilient_sdk_version()
     assert parsed_version is not None
-    assert parsed_version >= pkg_resources.parse_version(constants.RESILIENT_LIBRARIES_VERSION)
+    assert parsed_version >= parse_version(constants.RESILIENT_LIBRARIES_VERSION)
 
 def test_get_package_version_found_in_env():
     parsed_version = sdk_helpers.get_package_version("resilient-sdk")
     assert parsed_version is not None
-    assert parsed_version >= pkg_resources.parse_version(constants.RESILIENT_LIBRARIES_VERSION)
+    assert parsed_version >= parse_version(constants.RESILIENT_LIBRARIES_VERSION)
 
 def test_get_package_version_not_found():
     not_found = sdk_helpers.get_package_version("this-package-doesnt-exist")
     assert not_found is None
 
 
 def test_get_latest_version_on_pypi():
@@ -596,29 +595,29 @@
     assert current_version >= latest_version
 
 
 def test_get_latest_version_on_pypi_legacy_version():
     mock_releases = {"releases": ["41.0.0", "#$%^&*mock_legacy_version"]}
     with requests_mock.Mocker() as m:
         m.get(constants.URL_PYPI_VERSION, json=mock_releases)
-        assert pkg_resources.parse_version("41.0.0") == sdk_helpers.get_latest_version_on_pypi()
+        assert parse_version("41.0.0") == sdk_helpers.get_latest_version_on_pypi()
 
 
 def test_get_latest_available_version_pypi(fx_mk_os_tmp_dir):
     current_version = sdk_helpers.get_resilient_sdk_version()
     latest_version = sdk_helpers.get_latest_available_version()
 
     assert current_version >= latest_version
     assert os.path.isdir(fx_mk_os_tmp_dir)
 
 
 def test_get_latest_available_version_tmp_file(fx_mk_os_tmp_dir):
 
     path_sdk_tmp_pypi_version = os.path.join(fx_mk_os_tmp_dir, constants.TMP_PYPI_VERSION)
-    mock_version = pkg_resources.parse_version("45.0.0")
+    mock_version = parse_version("45.0.0")
 
     sdk_helpers.write_latest_pypi_tmp_file(mock_version, path_sdk_tmp_pypi_version)
     latest_version = sdk_helpers.get_latest_available_version()
 
     assert latest_version.base_version == "45.0.0"
 
 
@@ -722,28 +721,60 @@
     results_scraped = sdk_helpers.scrape_results_from_log_file(mock_paths.MOCK_APP_LOG_PATH)
     mock_function_one_results = results_scraped.get("mock_function_one")
 
     assert isinstance(mock_function_one_results, dict)
 
     # There are two Results for mock_function_one
     # in the mock_app.log file, so this ensures we get the latest
-    assert mock_function_one_results.get("version") == 2.1
-    assert mock_function_one_results.get("reason") == None
+    assert mock_function_one_results == {
+        "version": 2.1,
+        "success": True,
+        "reason": None,
+        "content": {"mock_key": "Mock Value!"},
+        "raw": None,
+        "inputs": {
+            "mock_input_text_with_value_string": "data value one  ล ฦ ว ศ ษ ส ห ฬ อ",
+            "mock_input_text": "abc  à¸¥ à¸¦ à¸§ à¸¨ à¸© à¸ª à¸« à¸¬ à¸\xad abc",
+            "mock_input_boolean": True,
+            "mock_input_multiselect": ["value one", "value two"],
+            "mock_input_select": "select two",
+            "mock_input_number": 1630407352685
+        },
+        "metrics": {
+            "version": "1.0",
+            "package": "fn-main-mock-integration",
+            "package_version": "1.0.3",
+            "host": constants.CODEGEN_PAYLOAD_SAMPLES_CLEAR_HOST_DEFAULT_VALUE,
+            "execution_time_ms": 3233,
+            "timestamp": "2021-12-02 14:48:45"
+        }
+    }
 
 def test_scrape_results_really_long_function_name():
 
     results_scraped = sdk_helpers.scrape_results_from_log_file(mock_paths.MOCK_APP_LOG_PATH)
     mock_function_one_results = results_scraped.get("mock_function_one_but_really_really_really_really_really_really_really_really_long")
 
     assert isinstance(mock_function_one_results, dict)
 
     # There are two Results for mock_function_one
     # in the mock_app.log file, so this ensures we get the latest
     assert mock_function_one_results.get("version") == 2.1
     assert mock_function_one_results.get("reason") == None
+    assert mock_function_one_results.get("metrics", {}).get("host") == constants.CODEGEN_PAYLOAD_SAMPLES_CLEAR_HOST_DEFAULT_VALUE
+
+def test_scrape_results_clears_metrics_host_value():
+
+    results_scraped = sdk_helpers.scrape_results_from_log_file(mock_paths.MOCK_APP_LOG_PATH)
+    mock_function_one_results = results_scraped.get("mock_function_one")
+
+    assert isinstance(mock_function_one_results, dict)
+
+    # specifically test that the host was cleared out
+    assert mock_function_one_results["metrics"]["host"] == constants.CODEGEN_PAYLOAD_SAMPLES_CLEAR_HOST_DEFAULT_VALUE
 
 
 def test_scrape_results_from_log_file_not_found():
     with pytest.raises(SDKException, match=constants.ERROR_NOT_FIND_FILE):
         sdk_helpers.scrape_results_from_log_file("mock_path_non_existent")
```

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_validate_configs.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_sdk_validate_configs.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tests/unit/test_util/test_sdk_validate_issue.py` & `resilient_sdk-51.0.2.0.974/tests/unit/test_util/test_sdk_validate_issue.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-51.0.1.1.824/tox.ini` & `resilient_sdk-51.0.2.0.974/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py27, py36, py39, py311
+envlist = py27, py36, py39, py311, py312
 skip_install=true
 skipsdist=true
 
 
 [testenv:UNIT]
 deps =
     pytest
```

