# Comparing `tmp/pulumi_fastly-8.8.0a1715756624.tar.gz` & `tmp/pulumi_fastly-8.8.0a1715970151.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-8.8.0a1715756624.tar", last modified: Wed May 15 07:06:10 2024, max compression
+gzip compressed data, was "pulumi_fastly-8.8.0a1715970151.tar", last modified: Fri May 17 18:26:47 2024, max compression
```

## Comparing `pulumi_fastly-8.8.0a1715756624.tar` & `pulumi_fastly-8.8.0a1715970151.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:06:10.327399 pulumi_fastly-8.8.0a1715756624/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-15 07:06:10.327399 pulumi_fastly-8.8.0a1715756624/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:06:10.323398 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   522888 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24377 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:06:10.327399 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/configstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/configstore_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_configstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_kvstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_package_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_secretstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_vcl_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    15807 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (127)   473470 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/secretstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    92401 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (127)   121205 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    91888 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)    22949 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    20467 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_mutual_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    25864 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:06:10.327399 pulumi_fastly-8.8.0a1715756624/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-15 07:06:10.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-15 07:06:10.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:06:10.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 07:06:10.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 07:06:10.000000 pulumi_fastly-8.8.0a1715756624/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-15 07:06:03.000000 pulumi_fastly-8.8.0a1715756624/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:06:10.327399 pulumi_fastly-8.8.0a1715756624/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:26:47.098633 pulumi_fastly-8.8.0a1715970151/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-17 18:26:47.098633 pulumi_fastly-8.8.0a1715970151/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:26:47.098633 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   538592 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24377 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:26:47.098633 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/configstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/configstore_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_configstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_kvstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_package_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_secretstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_vcl_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15807 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   488284 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/secretstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95305 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123901 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91888 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22949 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20467 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_mutual_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25864 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:26:47.098633 pulumi_fastly-8.8.0a1715970151/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-17 18:26:47.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-17 18:26:47.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 18:26:47.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 18:26:47.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 18:26:47.000000 pulumi_fastly-8.8.0a1715970151/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-17 18:26:40.000000 pulumi_fastly-8.8.0a1715970151/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 18:26:47.098633 pulumi_fastly-8.8.0a1715970151/setup.cfg
```

### Comparing `pulumi_fastly-8.8.0a1715756624/PKG-INFO` & `pulumi_fastly-8.8.0a1715970151/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.8.0a1715756624
+Version: 8.8.0a1715970151
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.8.0a1715756624/README.md` & `pulumi_fastly-8.8.0a1715970151/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/__init__.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/_inputs.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 __all__ = [
     'AlertDimensionsArgs',
     'AlertEvaluationStrategyArgs',
     'ServiceACLEntriesEntryArgs',
     'ServiceComputeBackendArgs',
     'ServiceComputeDictionaryArgs',
     'ServiceComputeDomainArgs',
+    'ServiceComputeImageOptimizerDefaultSettingsArgs',
     'ServiceComputeLoggingBigqueryArgs',
     'ServiceComputeLoggingBlobstorageArgs',
     'ServiceComputeLoggingCloudfileArgs',
     'ServiceComputeLoggingDatadogArgs',
     'ServiceComputeLoggingDigitaloceanArgs',
     'ServiceComputeLoggingElasticsearchArgs',
     'ServiceComputeLoggingFtpArgs',
@@ -52,14 +53,15 @@
     'ServiceVclDictionaryArgs',
     'ServiceVclDirectorArgs',
     'ServiceVclDomainArgs',
     'ServiceVclDynamicsnippetArgs',
     'ServiceVclGzipArgs',
     'ServiceVclHeaderArgs',
     'ServiceVclHealthcheckArgs',
+    'ServiceVclImageOptimizerDefaultSettingsArgs',
     'ServiceVclLoggingBigqueryArgs',
     'ServiceVclLoggingBlobstorageArgs',
     'ServiceVclLoggingCloudfileArgs',
     'ServiceVclLoggingDatadogArgs',
     'ServiceVclLoggingDigitaloceanArgs',
     'ServiceVclLoggingElasticsearchArgs',
     'ServiceVclLoggingFtpArgs',
@@ -780,14 +782,165 @@
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
 
 @pulumi.input_type
+class ServiceComputeImageOptimizerDefaultSettingsArgs:
+    def __init__(__self__, *,
+                 allow_video: Optional[pulumi.Input[bool]] = None,
+                 jpeg_quality: Optional[pulumi.Input[int]] = None,
+                 jpeg_type: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 resize_filter: Optional[pulumi.Input[str]] = None,
+                 upscale: Optional[pulumi.Input[bool]] = None,
+                 webp: Optional[pulumi.Input[bool]] = None,
+                 webp_quality: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[bool] allow_video: Enables GIF to MP4 transformations on this service.
+        :param pulumi.Input[int] jpeg_quality: The default quality to use with JPEG output. This can be overridden with the "quality" parameter on specific image optimizer requests.
+        :param pulumi.Input[str] jpeg_type: The default type of JPEG output to use. This can be overridden with "format=bjpeg" and "format=pjpeg" on specific image optimizer requests. Valid values are `auto`, `baseline` and `progressive`.
+               	- auto: Match the input JPEG type, or baseline if transforming from a non-JPEG input.
+               	- baseline: Output baseline JPEG images
+               	- progressive: Output progressive JPEG images
+        :param pulumi.Input[str] name: Used by the provider to identify modified settings. Changing this value will force the entire block to be deleted, then recreated.
+        :param pulumi.Input[str] resize_filter: The type of filter to use while resizing an image. Valid values are `lanczos3`, `lanczos2`, `bicubic`, `bilinear` and `nearest`.
+               	- lanczos3: A Lanczos filter with a kernel size of 3. Lanczos filters can detect edges and linear features within an image, providing the best possible reconstruction.
+               	- lanczos2: A Lanczos filter with a kernel size of 2.
+               	- bicubic: A filter using an average of a 4x4 environment of pixels, weighing the innermost pixels higher.
+               	- bilinear: A filter using an average of a 2x2 environment of pixels.
+               	- nearest: A filter using the value of nearby translated pixel values. Preserves hard edges.
+        :param pulumi.Input[bool] upscale: Whether or not we should allow output images to render at sizes larger than input.
+        :param pulumi.Input[bool] webp: Controls whether or not to default to WebP output when the client supports it. This is equivalent to adding "auto=webp" to all image optimizer requests.
+        :param pulumi.Input[int] webp_quality: The default quality to use with WebP output. This can be overridden with the second option in the "quality" URL parameter on specific image optimizer requests.
+        """
+        if allow_video is not None:
+            pulumi.set(__self__, "allow_video", allow_video)
+        if jpeg_quality is not None:
+            pulumi.set(__self__, "jpeg_quality", jpeg_quality)
+        if jpeg_type is not None:
+            pulumi.set(__self__, "jpeg_type", jpeg_type)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if resize_filter is not None:
+            pulumi.set(__self__, "resize_filter", resize_filter)
+        if upscale is not None:
+            pulumi.set(__self__, "upscale", upscale)
+        if webp is not None:
+            pulumi.set(__self__, "webp", webp)
+        if webp_quality is not None:
+            pulumi.set(__self__, "webp_quality", webp_quality)
+
+    @property
+    @pulumi.getter(name="allowVideo")
+    def allow_video(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Enables GIF to MP4 transformations on this service.
+        """
+        return pulumi.get(self, "allow_video")
+
+    @allow_video.setter
+    def allow_video(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "allow_video", value)
+
+    @property
+    @pulumi.getter(name="jpegQuality")
+    def jpeg_quality(self) -> Optional[pulumi.Input[int]]:
+        """
+        The default quality to use with JPEG output. This can be overridden with the "quality" parameter on specific image optimizer requests.
+        """
+        return pulumi.get(self, "jpeg_quality")
+
+    @jpeg_quality.setter
+    def jpeg_quality(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "jpeg_quality", value)
+
+    @property
+    @pulumi.getter(name="jpegType")
+    def jpeg_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        The default type of JPEG output to use. This can be overridden with "format=bjpeg" and "format=pjpeg" on specific image optimizer requests. Valid values are `auto`, `baseline` and `progressive`.
+        	- auto: Match the input JPEG type, or baseline if transforming from a non-JPEG input.
+        	- baseline: Output baseline JPEG images
+        	- progressive: Output progressive JPEG images
+        """
+        return pulumi.get(self, "jpeg_type")
+
+    @jpeg_type.setter
+    def jpeg_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "jpeg_type", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Used by the provider to identify modified settings. Changing this value will force the entire block to be deleted, then recreated.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="resizeFilter")
+    def resize_filter(self) -> Optional[pulumi.Input[str]]:
+        """
+        The type of filter to use while resizing an image. Valid values are `lanczos3`, `lanczos2`, `bicubic`, `bilinear` and `nearest`.
+        	- lanczos3: A Lanczos filter with a kernel size of 3. Lanczos filters can detect edges and linear features within an image, providing the best possible reconstruction.
+        	- lanczos2: A Lanczos filter with a kernel size of 2.
+        	- bicubic: A filter using an average of a 4x4 environment of pixels, weighing the innermost pixels higher.
+        	- bilinear: A filter using an average of a 2x2 environment of pixels.
+        	- nearest: A filter using the value of nearby translated pixel values. Preserves hard edges.
+        """
+        return pulumi.get(self, "resize_filter")
+
+    @resize_filter.setter
+    def resize_filter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "resize_filter", value)
+
+    @property
+    @pulumi.getter
+    def upscale(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether or not we should allow output images to render at sizes larger than input.
+        """
+        return pulumi.get(self, "upscale")
+
+    @upscale.setter
+    def upscale(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "upscale", value)
+
+    @property
+    @pulumi.getter
+    def webp(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Controls whether or not to default to WebP output when the client supports it. This is equivalent to adding "auto=webp" to all image optimizer requests.
+        """
+        return pulumi.get(self, "webp")
+
+    @webp.setter
+    def webp(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "webp", value)
+
+    @property
+    @pulumi.getter(name="webpQuality")
+    def webp_quality(self) -> Optional[pulumi.Input[int]]:
+        """
+        The default quality to use with WebP output. This can be overridden with the second option in the "quality" URL parameter on specific image optimizer requests.
+        """
+        return pulumi.get(self, "webp_quality")
+
+    @webp_quality.setter
+    def webp_quality(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "webp_quality", value)
+
+
+@pulumi.input_type
 class ServiceComputeLoggingBigqueryArgs:
     def __init__(__self__, *,
                  dataset: pulumi.Input[str],
                  email: pulumi.Input[str],
                  name: pulumi.Input[str],
                  project_id: pulumi.Input[str],
                  secret_key: pulumi.Input[str],
@@ -928,15 +1081,15 @@
                  public_key: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] account_name: The unique Azure Blob Storage namespace in which your data objects are stored
         :param pulumi.Input[str] container: The name of the Azure Blob Storage container in which to store logs
         :param pulumi.Input[str] name: A unique name to identify the Azure Blob Storage endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] sas_token: The Azure shared access signature providing write access to the blob service objects. Be sure to update your token before it expires or the logging functionality will not work
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: The path to upload logs to. Must end with a trailing slash. If this field is left empty, the files will be saved in the container's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred in seconds. Default `3600`
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
@@ -1010,15 +1163,15 @@
     def sas_token(self, value: pulumi.Input[str]):
         pulumi.set(self, "sas_token", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -1123,15 +1276,15 @@
                  region: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] access_key: Your Cloud File account access key
         :param pulumi.Input[str] bucket_name: The name of your Cloud Files container
         :param pulumi.Input[str] name: The unique name of the Rackspace Cloud Files logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] user: The username for your Cloud Files account
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: The path to upload logs to
         :param pulumi.Input[int] period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param pulumi.Input[str] public_key: The PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] region: The region to stream logs to. One of: DFW (Dallas), ORD (Chicago), IAD (Northern Virginia), LON (London), SYD (Sydney), HKG (Hong Kong)
         :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
@@ -1205,15 +1358,15 @@
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -1371,15 +1524,15 @@
                  public_key: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] access_key: Your DigitalOcean Spaces account access key
         :param pulumi.Input[str] bucket_name: The name of the DigitalOcean Space
         :param pulumi.Input[str] name: The unique name of the DigitalOcean Spaces logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] secret_key: Your DigitalOcean Spaces account secret key
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] domain: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: The path to upload logs to
         :param pulumi.Input[int] period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
@@ -1453,15 +1606,15 @@
     def secret_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "secret_key", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -1763,15 +1916,15 @@
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] address: The FTP address to stream logs to
         :param pulumi.Input[str] name: The unique name of the FTP logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] password: The password for the server (for anonymous use an email address)
         :param pulumi.Input[str] path: The path to upload log files to. If the path ends in `/` then it is treated as a directory
         :param pulumi.Input[str] user: The username for the server (can be `anonymous`)
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds (Default `3600`)
         :param pulumi.Input[int] port: The port number. Default: `21`
         :param pulumi.Input[str] public_key: The PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
@@ -1855,15 +2008,15 @@
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -1955,15 +2108,15 @@
                  secret_key: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] bucket_name: The name of the bucket in which to store the logs
         :param pulumi.Input[str] name: A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] account_name: The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds (Default 3600)
         :param pulumi.Input[str] project_id: The ID of your Google Cloud Platform project
         :param pulumi.Input[str] secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
         :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
@@ -2028,15 +2181,15 @@
     def account_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account_name", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -3141,15 +3294,15 @@
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] access_key: Your OpenStack account access key
         :param pulumi.Input[str] bucket_name: The name of your OpenStack container
         :param pulumi.Input[str] name: The unique name of the OpenStack logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] url: Your OpenStack auth url
         :param pulumi.Input[str] user: The username for your OpenStack account
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
@@ -3233,15 +3386,15 @@
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -3391,28 +3544,28 @@
                  server_side_encryption: Optional[pulumi.Input[str]] = None,
                  server_side_encryption_kms_key_id: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] bucket_name: The name of the bucket in which to store the logs
         :param pulumi.Input[str] name: The unique name of the S3 logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] acl: The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] domain: If you created the S3 bucket outside of `us-east-1`, then specify the corresponding bucket endpoint. Example: `s3-us-west-2.amazonaws.com`
         :param pulumi.Input[int] file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] redundancy: The S3 storage class (redundancy level). Should be one of: `standard`, `intelligent_tiering`, `standard_ia`, `onezone_ia`, `glacier`, `glacier_ir`, `deep_archive`, or `reduced_redundancy`
         :param pulumi.Input[str] s3_access_key: AWS Access Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This key will be not be encrypted. Not required if `iam_role` is provided. You can provide this key via an environment variable, `FASTLY_S3_ACCESS_KEY`
         :param pulumi.Input[str] s3_iam_role: The Amazon Resource Name (ARN) for the IAM role granting Fastly access to S3. Not required if `access_key` and `secret_key` are provided. You can provide this value via an environment variable, `FASTLY_S3_IAM_ROLE`
         :param pulumi.Input[str] s3_secret_key: AWS Secret Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This secret will be not be encrypted. Not required if `iam_role` is provided. You can provide this secret via an environment variable, `FASTLY_S3_SECRET_KEY`
         :param pulumi.Input[str] server_side_encryption: Specify what type of server side encryption should be used. Can be either `AES256` or `aws:kms`
-        :param pulumi.Input[str] server_side_encryption_kms_key_id: Optional server-side KMS Key Id. Must be set if server*side*encryption is set to `aws:kms`
+        :param pulumi.Input[str] server_side_encryption_kms_key_id: Optional server-side KMS Key Id. Must be set if server_side_encryption is set to `aws:kms`
         :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if compression_codec is not None:
@@ -3482,15 +3635,15 @@
     def acl(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "acl", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -3638,15 +3791,15 @@
     def server_side_encryption(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server_side_encryption", value)
 
     @property
     @pulumi.getter(name="serverSideEncryptionKmsKeyId")
     def server_side_encryption_kms_key_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Optional server-side KMS Key Id. Must be set if server*side*encryption is set to `aws:kms`
+        Optional server-side KMS Key Id. Must be set if server_side_encryption is set to `aws:kms`
         """
         return pulumi.get(self, "server_side_encryption_kms_key_id")
 
     @server_side_encryption_kms_key_id.setter
     def server_side_encryption_kms_key_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server_side_encryption_kms_key_id", value)
 
@@ -3751,15 +3904,15 @@
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] address: The SFTP address to stream logs to
         :param pulumi.Input[str] name: The unique name of the SFTP logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] path: The path to upload log files to. If the path ends in `/` then it is treated as a directory
         :param pulumi.Input[str] ssh_known_hosts: A list of host keys for all hosts we can connect to over SFTP
         :param pulumi.Input[str] user: The username for the server
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] password: The password for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
         :param pulumi.Input[int] period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param pulumi.Input[int] port: The port the SFTP service listens on. (Default: `22`)
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] secret_key: The SSH private key for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
@@ -3849,15 +4002,15 @@
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -4313,15 +4466,15 @@
     def __init__(__self__, *,
                  content: Optional[pulumi.Input[str]] = None,
                  filename: Optional[pulumi.Input[str]] = None,
                  source_code_hash: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] content: The contents of the Wasm deployment package as a base64 encoded string (e.g. could be provided using an input variable or via external data source output variable). Conflicts with `filename`. Exactly one of these two arguments must be specified
         :param pulumi.Input[str] filename: The path to the Wasm deployment package within your local filesystem. Conflicts with `content`. Exactly one of these two arguments must be specified
-        :param pulumi.Input[str] source_code_hash: Used to trigger updates. Must be set to a SHA512 hash of all files (in sorted order) within the package. The usual way to set this is using the fastly*package*hash data source.
+        :param pulumi.Input[str] source_code_hash: Used to trigger updates. Must be set to a SHA512 hash of all files (in sorted order) within the package. The usual way to set this is using the get_package_hash data source.
         """
         if content is not None:
             pulumi.set(__self__, "content", content)
         if filename is not None:
             pulumi.set(__self__, "filename", filename)
         if source_code_hash is not None:
             pulumi.set(__self__, "source_code_hash", source_code_hash)
@@ -4350,15 +4503,15 @@
     def filename(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "filename", value)
 
     @property
     @pulumi.getter(name="sourceCodeHash")
     def source_code_hash(self) -> Optional[pulumi.Input[str]]:
         """
-        Used to trigger updates. Must be set to a SHA512 hash of all files (in sorted order) within the package. The usual way to set this is using the fastly*package*hash data source.
+        Used to trigger updates. Must be set to a SHA512 hash of all files (in sorted order) within the package. The usual way to set this is using the get_package_hash data source.
         """
         return pulumi.get(self, "source_code_hash")
 
     @source_code_hash.setter
     def source_code_hash(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "source_code_hash", value)
 
@@ -5864,14 +6017,165 @@
 
     @window.setter
     def window(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "window", value)
 
 
 @pulumi.input_type
+class ServiceVclImageOptimizerDefaultSettingsArgs:
+    def __init__(__self__, *,
+                 allow_video: Optional[pulumi.Input[bool]] = None,
+                 jpeg_quality: Optional[pulumi.Input[int]] = None,
+                 jpeg_type: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 resize_filter: Optional[pulumi.Input[str]] = None,
+                 upscale: Optional[pulumi.Input[bool]] = None,
+                 webp: Optional[pulumi.Input[bool]] = None,
+                 webp_quality: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[bool] allow_video: Enables GIF to MP4 transformations on this service.
+        :param pulumi.Input[int] jpeg_quality: The default quality to use with JPEG output. This can be overridden with the "quality" parameter on specific image optimizer requests.
+        :param pulumi.Input[str] jpeg_type: The default type of JPEG output to use. This can be overridden with "format=bjpeg" and "format=pjpeg" on specific image optimizer requests. Valid values are `auto`, `baseline` and `progressive`.
+               	- auto: Match the input JPEG type, or baseline if transforming from a non-JPEG input.
+               	- baseline: Output baseline JPEG images
+               	- progressive: Output progressive JPEG images
+        :param pulumi.Input[str] name: Used by the provider to identify modified settings. Changing this value will force the entire block to be deleted, then recreated.
+        :param pulumi.Input[str] resize_filter: The type of filter to use while resizing an image. Valid values are `lanczos3`, `lanczos2`, `bicubic`, `bilinear` and `nearest`.
+               	- lanczos3: A Lanczos filter with a kernel size of 3. Lanczos filters can detect edges and linear features within an image, providing the best possible reconstruction.
+               	- lanczos2: A Lanczos filter with a kernel size of 2.
+               	- bicubic: A filter using an average of a 4x4 environment of pixels, weighing the innermost pixels higher.
+               	- bilinear: A filter using an average of a 2x2 environment of pixels.
+               	- nearest: A filter using the value of nearby translated pixel values. Preserves hard edges.
+        :param pulumi.Input[bool] upscale: Whether or not we should allow output images to render at sizes larger than input.
+        :param pulumi.Input[bool] webp: Controls whether or not to default to WebP output when the client supports it. This is equivalent to adding "auto=webp" to all image optimizer requests.
+        :param pulumi.Input[int] webp_quality: The default quality to use with WebP output. This can be overridden with the second option in the "quality" URL parameter on specific image optimizer requests.
+        """
+        if allow_video is not None:
+            pulumi.set(__self__, "allow_video", allow_video)
+        if jpeg_quality is not None:
+            pulumi.set(__self__, "jpeg_quality", jpeg_quality)
+        if jpeg_type is not None:
+            pulumi.set(__self__, "jpeg_type", jpeg_type)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if resize_filter is not None:
+            pulumi.set(__self__, "resize_filter", resize_filter)
+        if upscale is not None:
+            pulumi.set(__self__, "upscale", upscale)
+        if webp is not None:
+            pulumi.set(__self__, "webp", webp)
+        if webp_quality is not None:
+            pulumi.set(__self__, "webp_quality", webp_quality)
+
+    @property
+    @pulumi.getter(name="allowVideo")
+    def allow_video(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Enables GIF to MP4 transformations on this service.
+        """
+        return pulumi.get(self, "allow_video")
+
+    @allow_video.setter
+    def allow_video(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "allow_video", value)
+
+    @property
+    @pulumi.getter(name="jpegQuality")
+    def jpeg_quality(self) -> Optional[pulumi.Input[int]]:
+        """
+        The default quality to use with JPEG output. This can be overridden with the "quality" parameter on specific image optimizer requests.
+        """
+        return pulumi.get(self, "jpeg_quality")
+
+    @jpeg_quality.setter
+    def jpeg_quality(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "jpeg_quality", value)
+
+    @property
+    @pulumi.getter(name="jpegType")
+    def jpeg_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        The default type of JPEG output to use. This can be overridden with "format=bjpeg" and "format=pjpeg" on specific image optimizer requests. Valid values are `auto`, `baseline` and `progressive`.
+        	- auto: Match the input JPEG type, or baseline if transforming from a non-JPEG input.
+        	- baseline: Output baseline JPEG images
+        	- progressive: Output progressive JPEG images
+        """
+        return pulumi.get(self, "jpeg_type")
+
+    @jpeg_type.setter
+    def jpeg_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "jpeg_type", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Used by the provider to identify modified settings. Changing this value will force the entire block to be deleted, then recreated.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="resizeFilter")
+    def resize_filter(self) -> Optional[pulumi.Input[str]]:
+        """
+        The type of filter to use while resizing an image. Valid values are `lanczos3`, `lanczos2`, `bicubic`, `bilinear` and `nearest`.
+        	- lanczos3: A Lanczos filter with a kernel size of 3. Lanczos filters can detect edges and linear features within an image, providing the best possible reconstruction.
+        	- lanczos2: A Lanczos filter with a kernel size of 2.
+        	- bicubic: A filter using an average of a 4x4 environment of pixels, weighing the innermost pixels higher.
+        	- bilinear: A filter using an average of a 2x2 environment of pixels.
+        	- nearest: A filter using the value of nearby translated pixel values. Preserves hard edges.
+        """
+        return pulumi.get(self, "resize_filter")
+
+    @resize_filter.setter
+    def resize_filter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "resize_filter", value)
+
+    @property
+    @pulumi.getter
+    def upscale(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether or not we should allow output images to render at sizes larger than input.
+        """
+        return pulumi.get(self, "upscale")
+
+    @upscale.setter
+    def upscale(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "upscale", value)
+
+    @property
+    @pulumi.getter
+    def webp(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Controls whether or not to default to WebP output when the client supports it. This is equivalent to adding "auto=webp" to all image optimizer requests.
+        """
+        return pulumi.get(self, "webp")
+
+    @webp.setter
+    def webp(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "webp", value)
+
+    @property
+    @pulumi.getter(name="webpQuality")
+    def webp_quality(self) -> Optional[pulumi.Input[int]]:
+        """
+        The default quality to use with WebP output. This can be overridden with the second option in the "quality" URL parameter on specific image optimizer requests.
+        """
+        return pulumi.get(self, "webp_quality")
+
+    @webp_quality.setter
+    def webp_quality(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "webp_quality", value)
+
+
+@pulumi.input_type
 class ServiceVclLoggingBigqueryArgs:
     def __init__(__self__, *,
                  dataset: pulumi.Input[str],
                  email: pulumi.Input[str],
                  name: pulumi.Input[str],
                  project_id: pulumi.Input[str],
                  secret_key: pulumi.Input[str],
@@ -6064,15 +6368,15 @@
                  response_condition: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] account_name: The unique Azure Blob Storage namespace in which your data objects are stored
         :param pulumi.Input[str] container: The name of the Azure Blob Storage container in which to store logs
         :param pulumi.Input[str] name: A unique name to identify the Azure Blob Storage endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] sas_token: The Azure shared access signature providing write access to the blob service objects. Be sure to update your token before it expires or the logging functionality will not work
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param pulumi.Input[str] format: Apache-style string or VCL variables to use for log formatting (default: `%h %l %u %t "%r" %>s %b`)
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (default: 2)
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: The path to upload logs to. Must end with a trailing slash. If this field is left empty, the files will be saved in the container's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred in seconds. Default `3600`
@@ -6158,15 +6462,15 @@
     def sas_token(self, value: pulumi.Input[str]):
         pulumi.set(self, "sas_token", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -6323,15 +6627,15 @@
                  response_condition: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] access_key: Your Cloud File account access key
         :param pulumi.Input[str] bucket_name: The name of your Cloud Files container
         :param pulumi.Input[str] name: The unique name of the Rackspace Cloud Files logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] user: The username for your Cloud Files account
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] format: Apache style log formatting.
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either `1` or `2`. (default: `2`).
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: The path to upload logs to
         :param pulumi.Input[int] period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed. Can be `none` or `waf_debug`.
@@ -6417,15 +6721,15 @@
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -6699,15 +7003,15 @@
                  response_condition: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] access_key: Your DigitalOcean Spaces account access key
         :param pulumi.Input[str] bucket_name: The name of the DigitalOcean Space
         :param pulumi.Input[str] name: The unique name of the DigitalOcean Spaces logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] secret_key: Your DigitalOcean Spaces account secret key
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] domain: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
         :param pulumi.Input[str] format: Apache style log formatting.
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either `1` or `2`. (default: `2`).
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: The path to upload logs to
         :param pulumi.Input[int] period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
@@ -6793,15 +7097,15 @@
     def secret_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "secret_key", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -7219,15 +7523,15 @@
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] address: The FTP address to stream logs to
         :param pulumi.Input[str] name: The unique name of the FTP logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] password: The password for the server (for anonymous use an email address)
         :param pulumi.Input[str] path: The path to upload log files to. If the path ends in `/` then it is treated as a directory
         :param pulumi.Input[str] user: The username for the server (can be `anonymous`)
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] format: Apache-style string or VCL variables to use for log formatting.
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (default: 2).
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds (Default `3600`)
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed.
         :param pulumi.Input[int] port: The port number. Default: `21`
@@ -7323,15 +7627,15 @@
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -7475,15 +7779,15 @@
                  secret_key: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] bucket_name: The name of the bucket in which to store the logs
         :param pulumi.Input[str] name: A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] account_name: The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] format: Apache-style string or VCL variables to use for log formatting
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (Default: 2)
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds (Default 3600)
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed.
@@ -7560,15 +7864,15 @@
     def account_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account_name", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -9498,15 +9802,15 @@
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] access_key: Your OpenStack account access key
         :param pulumi.Input[str] bucket_name: The name of your OpenStack container
         :param pulumi.Input[str] name: The unique name of the OpenStack logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] url: Your OpenStack auth url
         :param pulumi.Input[str] user: The username for your OpenStack account
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] format: Apache style log formatting.
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either `1` or `2`. (default: `2`).
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed. Can be `none` or `waf_debug`.
@@ -9602,15 +9906,15 @@
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -9876,15 +10180,15 @@
                  server_side_encryption: Optional[pulumi.Input[str]] = None,
                  server_side_encryption_kms_key_id: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] bucket_name: The name of the bucket in which to store the logs
         :param pulumi.Input[str] name: The unique name of the S3 logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] acl: The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] domain: If you created the S3 bucket outside of `us-east-1`, then specify the corresponding bucket endpoint. Example: `s3-us-west-2.amazonaws.com`
         :param pulumi.Input[int] file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param pulumi.Input[str] format: Apache-style string or VCL variables to use for log formatting.
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (Default: 2).
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
@@ -9893,15 +10197,15 @@
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] redundancy: The S3 storage class (redundancy level). Should be one of: `standard`, `intelligent_tiering`, `standard_ia`, `onezone_ia`, `glacier`, `glacier_ir`, `deep_archive`, or `reduced_redundancy`
         :param pulumi.Input[str] response_condition: Name of blockAttributes condition to apply this logging.
         :param pulumi.Input[str] s3_access_key: AWS Access Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This key will be not be encrypted. Not required if `iam_role` is provided. You can provide this key via an environment variable, `FASTLY_S3_ACCESS_KEY`
         :param pulumi.Input[str] s3_iam_role: The Amazon Resource Name (ARN) for the IAM role granting Fastly access to S3. Not required if `access_key` and `secret_key` are provided. You can provide this value via an environment variable, `FASTLY_S3_IAM_ROLE`
         :param pulumi.Input[str] s3_secret_key: AWS Secret Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This secret will be not be encrypted. Not required if `iam_role` is provided. You can provide this secret via an environment variable, `FASTLY_S3_SECRET_KEY`
         :param pulumi.Input[str] server_side_encryption: Specify what type of server side encryption should be used. Can be either `AES256` or `aws:kms`
-        :param pulumi.Input[str] server_side_encryption_kms_key_id: Optional server-side KMS Key Id. Must be set if server*side*encryption is set to `aws:kms`
+        :param pulumi.Input[str] server_side_encryption_kms_key_id: Optional server-side KMS Key Id. Must be set if server_side_encryption is set to `aws:kms`
         :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if compression_codec is not None:
@@ -9979,15 +10283,15 @@
     def acl(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "acl", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -10183,15 +10487,15 @@
     def server_side_encryption(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server_side_encryption", value)
 
     @property
     @pulumi.getter(name="serverSideEncryptionKmsKeyId")
     def server_side_encryption_kms_key_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Optional server-side KMS Key Id. Must be set if server*side*encryption is set to `aws:kms`
+        Optional server-side KMS Key Id. Must be set if server_side_encryption is set to `aws:kms`
         """
         return pulumi.get(self, "server_side_encryption_kms_key_id")
 
     @server_side_encryption_kms_key_id.setter
     def server_side_encryption_kms_key_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server_side_encryption_kms_key_id", value)
 
@@ -10364,15 +10668,15 @@
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] address: The SFTP address to stream logs to
         :param pulumi.Input[str] name: The unique name of the SFTP logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] path: The path to upload log files to. If the path ends in `/` then it is treated as a directory
         :param pulumi.Input[str] ssh_known_hosts: A list of host keys for all hosts we can connect to over SFTP
         :param pulumi.Input[str] user: The username for the server
-        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] format: Apache-style string or VCL variables to use for log formatting.
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (default: 2).
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] password: The password for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
         :param pulumi.Input[int] period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed.
@@ -10474,15 +10778,15 @@
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[pulumi.Input[str]]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @compression_codec.setter
     def compression_codec(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compression_codec", value)
 
@@ -11289,15 +11593,15 @@
                  feature_revision: Optional[pulumi.Input[int]] = None,
                  logger_type: Optional[pulumi.Input[str]] = None,
                  ratelimiter_id: Optional[pulumi.Input[str]] = None,
                  response: Optional[pulumi.Input['ServiceVclRateLimiterResponseArgs']] = None,
                  response_object_name: Optional[pulumi.Input[str]] = None,
                  uri_dictionary_name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] action: The action to take when a rate limiter violation is detected (one of: log*only, response, response*object)
+        :param pulumi.Input[str] action: The action to take when a rate limiter violation is detected (one of: log_only, response, response_object)
         :param pulumi.Input[str] client_key: Comma-separated list of VCL variables used to generate a counter key to identify a client
         :param pulumi.Input[str] http_methods: Comma-separated list of HTTP methods to apply rate limiting to
         :param pulumi.Input[str] name: A unique human readable name for the rate limiting rule
         :param pulumi.Input[int] penalty_box_duration: Length of time in minutes that the rate limiter is in effect after the initial violation is detected
         :param pulumi.Input[int] rps_limit: Upper limit of requests per second allowed by the rate limiter
         :param pulumi.Input[int] window_size: Number of seconds during which the RPS limit must be exceeded in order to trigger a violation (one of: 1, 10, 60)
         :param pulumi.Input[int] feature_revision: Revision number of the rate limiting feature implementation
@@ -11327,15 +11631,15 @@
         if uri_dictionary_name is not None:
             pulumi.set(__self__, "uri_dictionary_name", uri_dictionary_name)
 
     @property
     @pulumi.getter
     def action(self) -> pulumi.Input[str]:
         """
-        The action to take when a rate limiter violation is detected (one of: log*only, response, response*object)
+        The action to take when a rate limiter violation is detected (one of: log_only, response, response_object)
         """
         return pulumi.get(self, "action")
 
     @action.setter
     def action(self, value: pulumi.Input[str]):
         pulumi.set(self, "action", value)
```

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/_utilities.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/alert.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/config/__init__.pyi` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/config/vars.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/configstore.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/configstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/configstore_entries.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/configstore_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_configstores.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_configstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_kvstores.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_kvstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_package_hash.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_package_hash.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_secretstores.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_secretstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_services.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_activation_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_vcl_snippets.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_vcl_snippets.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/integration.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/kvstore.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/kvstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/outputs.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 __all__ = [
     'AlertDimensions',
     'AlertEvaluationStrategy',
     'ServiceACLEntriesEntry',
     'ServiceComputeBackend',
     'ServiceComputeDictionary',
     'ServiceComputeDomain',
+    'ServiceComputeImageOptimizerDefaultSettings',
     'ServiceComputeLoggingBigquery',
     'ServiceComputeLoggingBlobstorage',
     'ServiceComputeLoggingCloudfile',
     'ServiceComputeLoggingDatadog',
     'ServiceComputeLoggingDigitalocean',
     'ServiceComputeLoggingElasticsearch',
     'ServiceComputeLoggingFtp',
@@ -53,14 +54,15 @@
     'ServiceVclDictionary',
     'ServiceVclDirector',
     'ServiceVclDomain',
     'ServiceVclDynamicsnippet',
     'ServiceVclGzip',
     'ServiceVclHeader',
     'ServiceVclHealthcheck',
+    'ServiceVclImageOptimizerDefaultSettings',
     'ServiceVclLoggingBigquery',
     'ServiceVclLoggingBlobstorage',
     'ServiceVclLoggingCloudfile',
     'ServiceVclLoggingDatadog',
     'ServiceVclLoggingDigitalocean',
     'ServiceVclLoggingElasticsearch',
     'ServiceVclLoggingFtp',
@@ -715,14 +717,158 @@
         """
         An optional comment about the Domain.
         """
         return pulumi.get(self, "comment")
 
 
 @pulumi.output_type
+class ServiceComputeImageOptimizerDefaultSettings(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "allowVideo":
+            suggest = "allow_video"
+        elif key == "jpegQuality":
+            suggest = "jpeg_quality"
+        elif key == "jpegType":
+            suggest = "jpeg_type"
+        elif key == "resizeFilter":
+            suggest = "resize_filter"
+        elif key == "webpQuality":
+            suggest = "webp_quality"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ServiceComputeImageOptimizerDefaultSettings. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ServiceComputeImageOptimizerDefaultSettings.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ServiceComputeImageOptimizerDefaultSettings.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 allow_video: Optional[bool] = None,
+                 jpeg_quality: Optional[int] = None,
+                 jpeg_type: Optional[str] = None,
+                 name: Optional[str] = None,
+                 resize_filter: Optional[str] = None,
+                 upscale: Optional[bool] = None,
+                 webp: Optional[bool] = None,
+                 webp_quality: Optional[int] = None):
+        """
+        :param bool allow_video: Enables GIF to MP4 transformations on this service.
+        :param int jpeg_quality: The default quality to use with JPEG output. This can be overridden with the "quality" parameter on specific image optimizer requests.
+        :param str jpeg_type: The default type of JPEG output to use. This can be overridden with "format=bjpeg" and "format=pjpeg" on specific image optimizer requests. Valid values are `auto`, `baseline` and `progressive`.
+               	- auto: Match the input JPEG type, or baseline if transforming from a non-JPEG input.
+               	- baseline: Output baseline JPEG images
+               	- progressive: Output progressive JPEG images
+        :param str name: Used by the provider to identify modified settings. Changing this value will force the entire block to be deleted, then recreated.
+        :param str resize_filter: The type of filter to use while resizing an image. Valid values are `lanczos3`, `lanczos2`, `bicubic`, `bilinear` and `nearest`.
+               	- lanczos3: A Lanczos filter with a kernel size of 3. Lanczos filters can detect edges and linear features within an image, providing the best possible reconstruction.
+               	- lanczos2: A Lanczos filter with a kernel size of 2.
+               	- bicubic: A filter using an average of a 4x4 environment of pixels, weighing the innermost pixels higher.
+               	- bilinear: A filter using an average of a 2x2 environment of pixels.
+               	- nearest: A filter using the value of nearby translated pixel values. Preserves hard edges.
+        :param bool upscale: Whether or not we should allow output images to render at sizes larger than input.
+        :param bool webp: Controls whether or not to default to WebP output when the client supports it. This is equivalent to adding "auto=webp" to all image optimizer requests.
+        :param int webp_quality: The default quality to use with WebP output. This can be overridden with the second option in the "quality" URL parameter on specific image optimizer requests.
+        """
+        if allow_video is not None:
+            pulumi.set(__self__, "allow_video", allow_video)
+        if jpeg_quality is not None:
+            pulumi.set(__self__, "jpeg_quality", jpeg_quality)
+        if jpeg_type is not None:
+            pulumi.set(__self__, "jpeg_type", jpeg_type)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if resize_filter is not None:
+            pulumi.set(__self__, "resize_filter", resize_filter)
+        if upscale is not None:
+            pulumi.set(__self__, "upscale", upscale)
+        if webp is not None:
+            pulumi.set(__self__, "webp", webp)
+        if webp_quality is not None:
+            pulumi.set(__self__, "webp_quality", webp_quality)
+
+    @property
+    @pulumi.getter(name="allowVideo")
+    def allow_video(self) -> Optional[bool]:
+        """
+        Enables GIF to MP4 transformations on this service.
+        """
+        return pulumi.get(self, "allow_video")
+
+    @property
+    @pulumi.getter(name="jpegQuality")
+    def jpeg_quality(self) -> Optional[int]:
+        """
+        The default quality to use with JPEG output. This can be overridden with the "quality" parameter on specific image optimizer requests.
+        """
+        return pulumi.get(self, "jpeg_quality")
+
+    @property
+    @pulumi.getter(name="jpegType")
+    def jpeg_type(self) -> Optional[str]:
+        """
+        The default type of JPEG output to use. This can be overridden with "format=bjpeg" and "format=pjpeg" on specific image optimizer requests. Valid values are `auto`, `baseline` and `progressive`.
+        	- auto: Match the input JPEG type, or baseline if transforming from a non-JPEG input.
+        	- baseline: Output baseline JPEG images
+        	- progressive: Output progressive JPEG images
+        """
+        return pulumi.get(self, "jpeg_type")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Used by the provider to identify modified settings. Changing this value will force the entire block to be deleted, then recreated.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="resizeFilter")
+    def resize_filter(self) -> Optional[str]:
+        """
+        The type of filter to use while resizing an image. Valid values are `lanczos3`, `lanczos2`, `bicubic`, `bilinear` and `nearest`.
+        	- lanczos3: A Lanczos filter with a kernel size of 3. Lanczos filters can detect edges and linear features within an image, providing the best possible reconstruction.
+        	- lanczos2: A Lanczos filter with a kernel size of 2.
+        	- bicubic: A filter using an average of a 4x4 environment of pixels, weighing the innermost pixels higher.
+        	- bilinear: A filter using an average of a 2x2 environment of pixels.
+        	- nearest: A filter using the value of nearby translated pixel values. Preserves hard edges.
+        """
+        return pulumi.get(self, "resize_filter")
+
+    @property
+    @pulumi.getter
+    def upscale(self) -> Optional[bool]:
+        """
+        Whether or not we should allow output images to render at sizes larger than input.
+        """
+        return pulumi.get(self, "upscale")
+
+    @property
+    @pulumi.getter
+    def webp(self) -> Optional[bool]:
+        """
+        Controls whether or not to default to WebP output when the client supports it. This is equivalent to adding "auto=webp" to all image optimizer requests.
+        """
+        return pulumi.get(self, "webp")
+
+    @property
+    @pulumi.getter(name="webpQuality")
+    def webp_quality(self) -> Optional[int]:
+        """
+        The default quality to use with WebP output. This can be overridden with the second option in the "quality" URL parameter on specific image optimizer requests.
+        """
+        return pulumi.get(self, "webp_quality")
+
+
+@pulumi.output_type
 class ServiceComputeLoggingBigquery(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "projectId":
             suggest = "project_id"
         elif key == "secretKey":
@@ -883,15 +1029,15 @@
                  public_key: Optional[str] = None,
                  timestamp_format: Optional[str] = None):
         """
         :param str account_name: The unique Azure Blob Storage namespace in which your data objects are stored
         :param str container: The name of the Azure Blob Storage container in which to store logs
         :param str name: A unique name to identify the Azure Blob Storage endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str sas_token: The Azure shared access signature providing write access to the blob service objects. Be sure to update your token before it expires or the logging functionality will not work
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param int file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: The path to upload logs to. Must end with a trailing slash. If this field is left empty, the files will be saved in the container's root path
         :param int period: How frequently the logs should be transferred in seconds. Default `3600`
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
@@ -949,15 +1095,15 @@
         """
         return pulumi.get(self, "sas_token")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter(name="fileMaxBytes")
     def file_max_bytes(self) -> Optional[int]:
         """
@@ -1059,15 +1205,15 @@
                  region: Optional[str] = None,
                  timestamp_format: Optional[str] = None):
         """
         :param str access_key: Your Cloud File account access key
         :param str bucket_name: The name of your Cloud Files container
         :param str name: The unique name of the Rackspace Cloud Files logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str user: The username for your Cloud Files account
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: The path to upload logs to
         :param int period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param str public_key: The PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str region: The region to stream logs to. One of: DFW (Dallas), ORD (Chicago), IAD (Northern Virginia), LON (London), SYD (Sydney), HKG (Hong Kong)
         :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
@@ -1125,15 +1271,15 @@
         """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter(name="gzipLevel")
     def gzip_level(self) -> Optional[int]:
         """
@@ -1278,15 +1424,15 @@
                  public_key: Optional[str] = None,
                  timestamp_format: Optional[str] = None):
         """
         :param str access_key: Your DigitalOcean Spaces account access key
         :param str bucket_name: The name of the DigitalOcean Space
         :param str name: The unique name of the DigitalOcean Spaces logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str secret_key: Your DigitalOcean Spaces account secret key
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param str domain: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: The path to upload logs to
         :param int period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
@@ -1344,15 +1490,15 @@
         """
         return pulumi.get(self, "secret_key")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[str]:
         """
@@ -1626,15 +1772,15 @@
                  timestamp_format: Optional[str] = None):
         """
         :param str address: The FTP address to stream logs to
         :param str name: The unique name of the FTP logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str password: The password for the server (for anonymous use an email address)
         :param str path: The path to upload log files to. If the path ends in `/` then it is treated as a directory
         :param str user: The username for the server (can be `anonymous`)
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param int period: How frequently the logs should be transferred, in seconds (Default `3600`)
         :param int port: The port number. Default: `21`
         :param str public_key: The PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
@@ -1698,15 +1844,15 @@
         """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter(name="gzipLevel")
     def gzip_level(self) -> Optional[int]:
         """
@@ -1801,15 +1947,15 @@
                  secret_key: Optional[str] = None,
                  timestamp_format: Optional[str] = None,
                  user: Optional[str] = None):
         """
         :param str bucket_name: The name of the bucket in which to store the logs
         :param str name: A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str account_name: The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds (Default 3600)
         :param str project_id: The ID of your Google Cloud Platform project
         :param str secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
         :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
@@ -1862,15 +2008,15 @@
         """
         return pulumi.get(self, "account_name")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter(name="gzipLevel")
     def gzip_level(self) -> Optional[int]:
         """
@@ -2863,15 +3009,15 @@
                  timestamp_format: Optional[str] = None):
         """
         :param str access_key: Your OpenStack account access key
         :param str bucket_name: The name of your OpenStack container
         :param str name: The unique name of the OpenStack logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str url: Your OpenStack auth url
         :param str user: The username for your OpenStack account
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
@@ -2935,15 +3081,15 @@
         """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter(name="gzipLevel")
     def gzip_level(self) -> Optional[int]:
         """
@@ -3092,28 +3238,28 @@
                  server_side_encryption: Optional[str] = None,
                  server_side_encryption_kms_key_id: Optional[str] = None,
                  timestamp_format: Optional[str] = None):
         """
         :param str bucket_name: The name of the bucket in which to store the logs
         :param str name: The unique name of the S3 logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str acl: The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param str domain: If you created the S3 bucket outside of `us-east-1`, then specify the corresponding bucket endpoint. Example: `s3-us-west-2.amazonaws.com`
         :param int file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str redundancy: The S3 storage class (redundancy level). Should be one of: `standard`, `intelligent_tiering`, `standard_ia`, `onezone_ia`, `glacier`, `glacier_ir`, `deep_archive`, or `reduced_redundancy`
         :param str s3_access_key: AWS Access Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This key will be not be encrypted. Not required if `iam_role` is provided. You can provide this key via an environment variable, `FASTLY_S3_ACCESS_KEY`
         :param str s3_iam_role: The Amazon Resource Name (ARN) for the IAM role granting Fastly access to S3. Not required if `access_key` and `secret_key` are provided. You can provide this value via an environment variable, `FASTLY_S3_IAM_ROLE`
         :param str s3_secret_key: AWS Secret Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This secret will be not be encrypted. Not required if `iam_role` is provided. You can provide this secret via an environment variable, `FASTLY_S3_SECRET_KEY`
         :param str server_side_encryption: Specify what type of server side encryption should be used. Can be either `AES256` or `aws:kms`
-        :param str server_side_encryption_kms_key_id: Optional server-side KMS Key Id. Must be set if server*side*encryption is set to `aws:kms`
+        :param str server_side_encryption_kms_key_id: Optional server-side KMS Key Id. Must be set if server_side_encryption is set to `aws:kms`
         :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if compression_codec is not None:
@@ -3171,15 +3317,15 @@
         """
         return pulumi.get(self, "acl")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[str]:
         """
@@ -3275,15 +3421,15 @@
         """
         return pulumi.get(self, "server_side_encryption")
 
     @property
     @pulumi.getter(name="serverSideEncryptionKmsKeyId")
     def server_side_encryption_kms_key_id(self) -> Optional[str]:
         """
-        Optional server-side KMS Key Id. Must be set if server*side*encryption is set to `aws:kms`
+        Optional server-side KMS Key Id. Must be set if server_side_encryption is set to `aws:kms`
         """
         return pulumi.get(self, "server_side_encryption_kms_key_id")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
@@ -3410,15 +3556,15 @@
                  timestamp_format: Optional[str] = None):
         """
         :param str address: The SFTP address to stream logs to
         :param str name: The unique name of the SFTP logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str path: The path to upload log files to. If the path ends in `/` then it is treated as a directory
         :param str ssh_known_hosts: A list of host keys for all hosts we can connect to over SFTP
         :param str user: The username for the server
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str password: The password for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
         :param int period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param int port: The port the SFTP service listens on. (Default: `22`)
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str secret_key: The SSH private key for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
@@ -3488,15 +3634,15 @@
         """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter(name="gzipLevel")
     def gzip_level(self) -> Optional[int]:
         """
@@ -3918,15 +4064,15 @@
     def __init__(__self__, *,
                  content: Optional[str] = None,
                  filename: Optional[str] = None,
                  source_code_hash: Optional[str] = None):
         """
         :param str content: The contents of the Wasm deployment package as a base64 encoded string (e.g. could be provided using an input variable or via external data source output variable). Conflicts with `filename`. Exactly one of these two arguments must be specified
         :param str filename: The path to the Wasm deployment package within your local filesystem. Conflicts with `content`. Exactly one of these two arguments must be specified
-        :param str source_code_hash: Used to trigger updates. Must be set to a SHA512 hash of all files (in sorted order) within the package. The usual way to set this is using the fastly*package*hash data source.
+        :param str source_code_hash: Used to trigger updates. Must be set to a SHA512 hash of all files (in sorted order) within the package. The usual way to set this is using the get_package_hash data source.
         """
         if content is not None:
             pulumi.set(__self__, "content", content)
         if filename is not None:
             pulumi.set(__self__, "filename", filename)
         if source_code_hash is not None:
             pulumi.set(__self__, "source_code_hash", source_code_hash)
@@ -3947,15 +4093,15 @@
         """
         return pulumi.get(self, "filename")
 
     @property
     @pulumi.getter(name="sourceCodeHash")
     def source_code_hash(self) -> Optional[str]:
         """
-        Used to trigger updates. Must be set to a SHA512 hash of all files (in sorted order) within the package. The usual way to set this is using the fastly*package*hash data source.
+        Used to trigger updates. Must be set to a SHA512 hash of all files (in sorted order) within the package. The usual way to set this is using the get_package_hash data source.
         """
         return pulumi.get(self, "source_code_hash")
 
 
 @pulumi.output_type
 class ServiceComputeProductEnablement(dict):
     def __init__(__self__, *,
@@ -5310,14 +5456,158 @@
         """
         The number of most recent Healthcheck queries to keep for this Healthcheck. Default `5`
         """
         return pulumi.get(self, "window")
 
 
 @pulumi.output_type
+class ServiceVclImageOptimizerDefaultSettings(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "allowVideo":
+            suggest = "allow_video"
+        elif key == "jpegQuality":
+            suggest = "jpeg_quality"
+        elif key == "jpegType":
+            suggest = "jpeg_type"
+        elif key == "resizeFilter":
+            suggest = "resize_filter"
+        elif key == "webpQuality":
+            suggest = "webp_quality"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ServiceVclImageOptimizerDefaultSettings. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ServiceVclImageOptimizerDefaultSettings.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ServiceVclImageOptimizerDefaultSettings.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 allow_video: Optional[bool] = None,
+                 jpeg_quality: Optional[int] = None,
+                 jpeg_type: Optional[str] = None,
+                 name: Optional[str] = None,
+                 resize_filter: Optional[str] = None,
+                 upscale: Optional[bool] = None,
+                 webp: Optional[bool] = None,
+                 webp_quality: Optional[int] = None):
+        """
+        :param bool allow_video: Enables GIF to MP4 transformations on this service.
+        :param int jpeg_quality: The default quality to use with JPEG output. This can be overridden with the "quality" parameter on specific image optimizer requests.
+        :param str jpeg_type: The default type of JPEG output to use. This can be overridden with "format=bjpeg" and "format=pjpeg" on specific image optimizer requests. Valid values are `auto`, `baseline` and `progressive`.
+               	- auto: Match the input JPEG type, or baseline if transforming from a non-JPEG input.
+               	- baseline: Output baseline JPEG images
+               	- progressive: Output progressive JPEG images
+        :param str name: Used by the provider to identify modified settings. Changing this value will force the entire block to be deleted, then recreated.
+        :param str resize_filter: The type of filter to use while resizing an image. Valid values are `lanczos3`, `lanczos2`, `bicubic`, `bilinear` and `nearest`.
+               	- lanczos3: A Lanczos filter with a kernel size of 3. Lanczos filters can detect edges and linear features within an image, providing the best possible reconstruction.
+               	- lanczos2: A Lanczos filter with a kernel size of 2.
+               	- bicubic: A filter using an average of a 4x4 environment of pixels, weighing the innermost pixels higher.
+               	- bilinear: A filter using an average of a 2x2 environment of pixels.
+               	- nearest: A filter using the value of nearby translated pixel values. Preserves hard edges.
+        :param bool upscale: Whether or not we should allow output images to render at sizes larger than input.
+        :param bool webp: Controls whether or not to default to WebP output when the client supports it. This is equivalent to adding "auto=webp" to all image optimizer requests.
+        :param int webp_quality: The default quality to use with WebP output. This can be overridden with the second option in the "quality" URL parameter on specific image optimizer requests.
+        """
+        if allow_video is not None:
+            pulumi.set(__self__, "allow_video", allow_video)
+        if jpeg_quality is not None:
+            pulumi.set(__self__, "jpeg_quality", jpeg_quality)
+        if jpeg_type is not None:
+            pulumi.set(__self__, "jpeg_type", jpeg_type)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if resize_filter is not None:
+            pulumi.set(__self__, "resize_filter", resize_filter)
+        if upscale is not None:
+            pulumi.set(__self__, "upscale", upscale)
+        if webp is not None:
+            pulumi.set(__self__, "webp", webp)
+        if webp_quality is not None:
+            pulumi.set(__self__, "webp_quality", webp_quality)
+
+    @property
+    @pulumi.getter(name="allowVideo")
+    def allow_video(self) -> Optional[bool]:
+        """
+        Enables GIF to MP4 transformations on this service.
+        """
+        return pulumi.get(self, "allow_video")
+
+    @property
+    @pulumi.getter(name="jpegQuality")
+    def jpeg_quality(self) -> Optional[int]:
+        """
+        The default quality to use with JPEG output. This can be overridden with the "quality" parameter on specific image optimizer requests.
+        """
+        return pulumi.get(self, "jpeg_quality")
+
+    @property
+    @pulumi.getter(name="jpegType")
+    def jpeg_type(self) -> Optional[str]:
+        """
+        The default type of JPEG output to use. This can be overridden with "format=bjpeg" and "format=pjpeg" on specific image optimizer requests. Valid values are `auto`, `baseline` and `progressive`.
+        	- auto: Match the input JPEG type, or baseline if transforming from a non-JPEG input.
+        	- baseline: Output baseline JPEG images
+        	- progressive: Output progressive JPEG images
+        """
+        return pulumi.get(self, "jpeg_type")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Used by the provider to identify modified settings. Changing this value will force the entire block to be deleted, then recreated.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="resizeFilter")
+    def resize_filter(self) -> Optional[str]:
+        """
+        The type of filter to use while resizing an image. Valid values are `lanczos3`, `lanczos2`, `bicubic`, `bilinear` and `nearest`.
+        	- lanczos3: A Lanczos filter with a kernel size of 3. Lanczos filters can detect edges and linear features within an image, providing the best possible reconstruction.
+        	- lanczos2: A Lanczos filter with a kernel size of 2.
+        	- bicubic: A filter using an average of a 4x4 environment of pixels, weighing the innermost pixels higher.
+        	- bilinear: A filter using an average of a 2x2 environment of pixels.
+        	- nearest: A filter using the value of nearby translated pixel values. Preserves hard edges.
+        """
+        return pulumi.get(self, "resize_filter")
+
+    @property
+    @pulumi.getter
+    def upscale(self) -> Optional[bool]:
+        """
+        Whether or not we should allow output images to render at sizes larger than input.
+        """
+        return pulumi.get(self, "upscale")
+
+    @property
+    @pulumi.getter
+    def webp(self) -> Optional[bool]:
+        """
+        Controls whether or not to default to WebP output when the client supports it. This is equivalent to adding "auto=webp" to all image optimizer requests.
+        """
+        return pulumi.get(self, "webp")
+
+    @property
+    @pulumi.getter(name="webpQuality")
+    def webp_quality(self) -> Optional[int]:
+        """
+        The default quality to use with WebP output. This can be overridden with the second option in the "quality" URL parameter on specific image optimizer requests.
+        """
+        return pulumi.get(self, "webp_quality")
+
+
+@pulumi.output_type
 class ServiceVclLoggingBigquery(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "projectId":
             suggest = "project_id"
         elif key == "secretKey":
@@ -5524,15 +5814,15 @@
                  response_condition: Optional[str] = None,
                  timestamp_format: Optional[str] = None):
         """
         :param str account_name: The unique Azure Blob Storage namespace in which your data objects are stored
         :param str container: The name of the Azure Blob Storage container in which to store logs
         :param str name: A unique name to identify the Azure Blob Storage endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str sas_token: The Azure shared access signature providing write access to the blob service objects. Be sure to update your token before it expires or the logging functionality will not work
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param int file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param str format: Apache-style string or VCL variables to use for log formatting (default: `%h %l %u %t "%r" %>s %b`)
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (default: 2)
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: The path to upload logs to. Must end with a trailing slash. If this field is left empty, the files will be saved in the container's root path
         :param int period: How frequently the logs should be transferred in seconds. Default `3600`
@@ -5602,15 +5892,15 @@
         """
         return pulumi.get(self, "sas_token")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter(name="fileMaxBytes")
     def file_max_bytes(self) -> Optional[int]:
         """
@@ -5752,15 +6042,15 @@
                  response_condition: Optional[str] = None,
                  timestamp_format: Optional[str] = None):
         """
         :param str access_key: Your Cloud File account access key
         :param str bucket_name: The name of your Cloud Files container
         :param str name: The unique name of the Rackspace Cloud Files logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str user: The username for your Cloud Files account
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param str format: Apache style log formatting.
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either `1` or `2`. (default: `2`).
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: The path to upload logs to
         :param int period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param str placement: Where in the generated VCL the logging call should be placed. Can be `none` or `waf_debug`.
@@ -5830,15 +6120,15 @@
         """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter
     def format(self) -> Optional[str]:
         """
@@ -6090,15 +6380,15 @@
                  response_condition: Optional[str] = None,
                  timestamp_format: Optional[str] = None):
         """
         :param str access_key: Your DigitalOcean Spaces account access key
         :param str bucket_name: The name of the DigitalOcean Space
         :param str name: The unique name of the DigitalOcean Spaces logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str secret_key: Your DigitalOcean Spaces account secret key
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param str domain: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
         :param str format: Apache style log formatting.
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either `1` or `2`. (default: `2`).
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: The path to upload logs to
         :param int period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
@@ -6168,15 +6458,15 @@
         """
         return pulumi.get(self, "secret_key")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[str]:
         """
@@ -6542,15 +6832,15 @@
                  timestamp_format: Optional[str] = None):
         """
         :param str address: The FTP address to stream logs to
         :param str name: The unique name of the FTP logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str password: The password for the server (for anonymous use an email address)
         :param str path: The path to upload log files to. If the path ends in `/` then it is treated as a directory
         :param str user: The username for the server (can be `anonymous`)
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param str format: Apache-style string or VCL variables to use for log formatting.
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (default: 2).
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param int period: How frequently the logs should be transferred, in seconds (Default `3600`)
         :param str placement: Where in the generated VCL the logging call should be placed.
         :param int port: The port number. Default: `21`
@@ -6626,15 +6916,15 @@
         """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter
     def format(self) -> Optional[str]:
         """
@@ -6769,15 +7059,15 @@
                  secret_key: Optional[str] = None,
                  timestamp_format: Optional[str] = None,
                  user: Optional[str] = None):
         """
         :param str bucket_name: The name of the bucket in which to store the logs
         :param str name: A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str account_name: The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param str format: Apache-style string or VCL variables to use for log formatting
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (Default: 2)
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds (Default 3600)
         :param str placement: Where in the generated VCL the logging call should be placed.
@@ -6842,15 +7132,15 @@
         """
         return pulumi.get(self, "account_name")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter
     def format(self) -> Optional[str]:
         """
@@ -8598,15 +8888,15 @@
                  timestamp_format: Optional[str] = None):
         """
         :param str access_key: Your OpenStack account access key
         :param str bucket_name: The name of your OpenStack container
         :param str name: The unique name of the OpenStack logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str url: Your OpenStack auth url
         :param str user: The username for your OpenStack account
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param str format: Apache style log formatting.
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either `1` or `2`. (default: `2`).
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param str placement: Where in the generated VCL the logging call should be placed. Can be `none` or `waf_debug`.
@@ -8682,15 +8972,15 @@
         """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter
     def format(self) -> Optional[str]:
         """
@@ -8946,15 +9236,15 @@
                  server_side_encryption: Optional[str] = None,
                  server_side_encryption_kms_key_id: Optional[str] = None,
                  timestamp_format: Optional[str] = None):
         """
         :param str bucket_name: The name of the bucket in which to store the logs
         :param str name: The unique name of the S3 logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str acl: The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param str domain: If you created the S3 bucket outside of `us-east-1`, then specify the corresponding bucket endpoint. Example: `s3-us-west-2.amazonaws.com`
         :param int file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param str format: Apache-style string or VCL variables to use for log formatting.
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (Default: 2).
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
@@ -8963,15 +9253,15 @@
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str redundancy: The S3 storage class (redundancy level). Should be one of: `standard`, `intelligent_tiering`, `standard_ia`, `onezone_ia`, `glacier`, `glacier_ir`, `deep_archive`, or `reduced_redundancy`
         :param str response_condition: Name of blockAttributes condition to apply this logging.
         :param str s3_access_key: AWS Access Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This key will be not be encrypted. Not required if `iam_role` is provided. You can provide this key via an environment variable, `FASTLY_S3_ACCESS_KEY`
         :param str s3_iam_role: The Amazon Resource Name (ARN) for the IAM role granting Fastly access to S3. Not required if `access_key` and `secret_key` are provided. You can provide this value via an environment variable, `FASTLY_S3_IAM_ROLE`
         :param str s3_secret_key: AWS Secret Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This secret will be not be encrypted. Not required if `iam_role` is provided. You can provide this secret via an environment variable, `FASTLY_S3_SECRET_KEY`
         :param str server_side_encryption: Specify what type of server side encryption should be used. Can be either `AES256` or `aws:kms`
-        :param str server_side_encryption_kms_key_id: Optional server-side KMS Key Id. Must be set if server*side*encryption is set to `aws:kms`
+        :param str server_side_encryption_kms_key_id: Optional server-side KMS Key Id. Must be set if server_side_encryption is set to `aws:kms`
         :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if compression_codec is not None:
@@ -9037,15 +9327,15 @@
         """
         return pulumi.get(self, "acl")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[str]:
         """
@@ -9173,15 +9463,15 @@
         """
         return pulumi.get(self, "server_side_encryption")
 
     @property
     @pulumi.getter(name="serverSideEncryptionKmsKeyId")
     def server_side_encryption_kms_key_id(self) -> Optional[str]:
         """
-        Optional server-side KMS Key Id. Must be set if server*side*encryption is set to `aws:kms`
+        Optional server-side KMS Key Id. Must be set if server_side_encryption is set to `aws:kms`
         """
         return pulumi.get(self, "server_side_encryption_kms_key_id")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
@@ -9368,15 +9658,15 @@
                  timestamp_format: Optional[str] = None):
         """
         :param str address: The SFTP address to stream logs to
         :param str name: The unique name of the SFTP logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str path: The path to upload log files to. If the path ends in `/` then it is treated as a directory
         :param str ssh_known_hosts: A list of host keys for all hosts we can connect to over SFTP
         :param str user: The username for the server
-        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         :param str format: Apache-style string or VCL variables to use for log formatting.
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (default: 2).
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str password: The password for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
         :param int period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param str placement: Where in the generated VCL the logging call should be placed.
@@ -9458,15 +9748,15 @@
         """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter(name="compressionCodec")
     def compression_codec(self) -> Optional[str]:
         """
-        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
+        The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip_level will default to 3. To specify a different level, leave compression_codec blank and explicitly set the level using gzip_level. Specifying both compression_codec and gzip_level in the same API request will result in an error.
         """
         return pulumi.get(self, "compression_codec")
 
     @property
     @pulumi.getter
     def format(self) -> Optional[str]:
         """
@@ -10204,15 +10494,15 @@
                  feature_revision: Optional[int] = None,
                  logger_type: Optional[str] = None,
                  ratelimiter_id: Optional[str] = None,
                  response: Optional['outputs.ServiceVclRateLimiterResponse'] = None,
                  response_object_name: Optional[str] = None,
                  uri_dictionary_name: Optional[str] = None):
         """
-        :param str action: The action to take when a rate limiter violation is detected (one of: log*only, response, response*object)
+        :param str action: The action to take when a rate limiter violation is detected (one of: log_only, response, response_object)
         :param str client_key: Comma-separated list of VCL variables used to generate a counter key to identify a client
         :param str http_methods: Comma-separated list of HTTP methods to apply rate limiting to
         :param str name: A unique human readable name for the rate limiting rule
         :param int penalty_box_duration: Length of time in minutes that the rate limiter is in effect after the initial violation is detected
         :param int rps_limit: Upper limit of requests per second allowed by the rate limiter
         :param int window_size: Number of seconds during which the RPS limit must be exceeded in order to trigger a violation (one of: 1, 10, 60)
         :param int feature_revision: Revision number of the rate limiting feature implementation
@@ -10242,15 +10532,15 @@
         if uri_dictionary_name is not None:
             pulumi.set(__self__, "uri_dictionary_name", uri_dictionary_name)
 
     @property
     @pulumi.getter
     def action(self) -> str:
         """
-        The action to take when a rate limiter violation is detected (one of: log*only, response, response*object)
+        The action to take when a rate limiter violation is detected (one of: log_only, response, response_object)
         """
         return pulumi.get(self, "action")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> str:
         """
```

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/provider.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/secretstore.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/secretstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_authorization.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_compute.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_compute.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     def __init__(__self__, *,
                  domains: pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]],
                  activate: Optional[pulumi.Input[bool]] = None,
                  backends: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeBackendArgs']]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  dictionaries: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeDictionaryArgs']]]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None,
+                 image_optimizer_default_settings: Optional[pulumi.Input['ServiceComputeImageOptimizerDefaultSettingsArgs']] = None,
                  logging_bigqueries: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingBigqueryArgs']]]] = None,
                  logging_blobstorages: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingBlobstorageArgs']]]] = None,
                  logging_cloudfiles: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingCloudfileArgs']]]] = None,
                  logging_datadogs: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingDatadogArgs']]]] = None,
                  logging_digitaloceans: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingDigitaloceanArgs']]]] = None,
                  logging_elasticsearches: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingElasticsearchArgs']]]] = None,
                  logging_ftps: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingFtpArgs']]]] = None,
@@ -53,32 +54,38 @@
                  product_enablement: Optional[pulumi.Input['ServiceComputeProductEnablementArgs']] = None,
                  resource_links: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ServiceCompute resource.
         :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
-        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
-        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+               will not activate it if this is set to `false`. Default `true`
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+               `false`
         :param pulumi.Input[str] name: The unique name for the Service to create
-        :param pulumi.Input['ServiceComputePackageArgs'] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
+        :param pulumi.Input['ServiceComputePackageArgs'] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted,
+               ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on
+               [Compute](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         pulumi.set(__self__, "domains", domains)
         if activate is not None:
             pulumi.set(__self__, "activate", activate)
         if backends is not None:
             pulumi.set(__self__, "backends", backends)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if dictionaries is not None:
             pulumi.set(__self__, "dictionaries", dictionaries)
         if force_destroy is not None:
             pulumi.set(__self__, "force_destroy", force_destroy)
+        if image_optimizer_default_settings is not None:
+            pulumi.set(__self__, "image_optimizer_default_settings", image_optimizer_default_settings)
         if logging_bigqueries is not None:
             pulumi.set(__self__, "logging_bigqueries", logging_bigqueries)
         if logging_blobstorages is not None:
             pulumi.set(__self__, "logging_blobstorages", logging_blobstorages)
         if logging_cloudfiles is not None:
             pulumi.set(__self__, "logging_cloudfiles", logging_cloudfiles)
         if logging_datadogs is not None:
@@ -152,15 +159,16 @@
     def domains(self, value: pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]]):
         pulumi.set(self, "domains", value)
 
     @property
     @pulumi.getter
     def activate(self) -> Optional[pulumi.Input[bool]]:
         """
-        Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+        will not activate it if this is set to `false`. Default `true`
         """
         return pulumi.get(self, "activate")
 
     @activate.setter
     def activate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "activate", value)
 
@@ -191,23 +199,33 @@
     def dictionaries(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeDictionaryArgs']]]]):
         pulumi.set(self, "dictionaries", value)
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
-        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+        `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @force_destroy.setter
     def force_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_destroy", value)
 
     @property
+    @pulumi.getter(name="imageOptimizerDefaultSettings")
+    def image_optimizer_default_settings(self) -> Optional[pulumi.Input['ServiceComputeImageOptimizerDefaultSettingsArgs']]:
+        return pulumi.get(self, "image_optimizer_default_settings")
+
+    @image_optimizer_default_settings.setter
+    def image_optimizer_default_settings(self, value: Optional[pulumi.Input['ServiceComputeImageOptimizerDefaultSettingsArgs']]):
+        pulumi.set(self, "image_optimizer_default_settings", value)
+
+    @property
     @pulumi.getter(name="loggingBigqueries")
     def logging_bigqueries(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingBigqueryArgs']]]]:
         return pulumi.get(self, "logging_bigqueries")
 
     @logging_bigqueries.setter
     def logging_bigqueries(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingBigqueryArgs']]]]):
         pulumi.set(self, "logging_bigqueries", value)
@@ -449,15 +467,17 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def package(self) -> Optional[pulumi.Input['ServiceComputePackageArgs']]:
         """
-        The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
+        The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted,
+        ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on
+        [Compute](https://developer.fastly.com/learning/compute/)
         """
         return pulumi.get(self, "package")
 
     @package.setter
     def package(self, value: Optional[pulumi.Input['ServiceComputePackageArgs']]):
         pulumi.set(self, "package", value)
 
@@ -512,14 +532,15 @@
                  backends: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeBackendArgs']]]] = None,
                  cloned_version: Optional[pulumi.Input[int]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  dictionaries: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeDictionaryArgs']]]] = None,
                  domains: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None,
                  force_refresh: Optional[pulumi.Input[bool]] = None,
+                 image_optimizer_default_settings: Optional[pulumi.Input['ServiceComputeImageOptimizerDefaultSettingsArgs']] = None,
                  imported: Optional[pulumi.Input[bool]] = None,
                  logging_bigqueries: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingBigqueryArgs']]]] = None,
                  logging_blobstorages: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingBlobstorageArgs']]]] = None,
                  logging_cloudfiles: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingCloudfileArgs']]]] = None,
                  logging_datadogs: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingDatadogArgs']]]] = None,
                  logging_digitaloceans: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingDigitaloceanArgs']]]] = None,
                  logging_elasticsearches: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingElasticsearchArgs']]]] = None,
@@ -547,22 +568,27 @@
                  package: Optional[pulumi.Input['ServiceComputePackageArgs']] = None,
                  product_enablement: Optional[pulumi.Input['ServiceComputeProductEnablementArgs']] = None,
                  resource_links: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ServiceCompute resources.
-        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+               will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
         :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
-        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
-        :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+               `false`
+        :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the
+               import is finished
         :param pulumi.Input[str] name: The unique name for the Service to create
-        :param pulumi.Input['ServiceComputePackageArgs'] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
+        :param pulumi.Input['ServiceComputePackageArgs'] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted,
+               ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on
+               [Compute](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         if activate is not None:
             pulumi.set(__self__, "activate", activate)
         if active_version is not None:
             pulumi.set(__self__, "active_version", active_version)
@@ -576,14 +602,16 @@
             pulumi.set(__self__, "dictionaries", dictionaries)
         if domains is not None:
             pulumi.set(__self__, "domains", domains)
         if force_destroy is not None:
             pulumi.set(__self__, "force_destroy", force_destroy)
         if force_refresh is not None:
             pulumi.set(__self__, "force_refresh", force_refresh)
+        if image_optimizer_default_settings is not None:
+            pulumi.set(__self__, "image_optimizer_default_settings", image_optimizer_default_settings)
         if imported is not None:
             pulumi.set(__self__, "imported", imported)
         if logging_bigqueries is not None:
             pulumi.set(__self__, "logging_bigqueries", logging_bigqueries)
         if logging_blobstorages is not None:
             pulumi.set(__self__, "logging_blobstorages", logging_blobstorages)
         if logging_cloudfiles is not None:
@@ -647,15 +675,16 @@
         if version_comment is not None:
             pulumi.set(__self__, "version_comment", version_comment)
 
     @property
     @pulumi.getter
     def activate(self) -> Optional[pulumi.Input[bool]]:
         """
-        Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+        will not activate it if this is set to `false`. Default `true`
         """
         return pulumi.get(self, "activate")
 
     @activate.setter
     def activate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "activate", value)
 
@@ -722,15 +751,16 @@
     def domains(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]]]):
         pulumi.set(self, "domains", value)
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
-        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+        `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @force_destroy.setter
     def force_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_destroy", value)
 
@@ -740,18 +770,28 @@
         return pulumi.get(self, "force_refresh")
 
     @force_refresh.setter
     def force_refresh(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_refresh", value)
 
     @property
+    @pulumi.getter(name="imageOptimizerDefaultSettings")
+    def image_optimizer_default_settings(self) -> Optional[pulumi.Input['ServiceComputeImageOptimizerDefaultSettingsArgs']]:
+        return pulumi.get(self, "image_optimizer_default_settings")
+
+    @image_optimizer_default_settings.setter
+    def image_optimizer_default_settings(self, value: Optional[pulumi.Input['ServiceComputeImageOptimizerDefaultSettingsArgs']]):
+        pulumi.set(self, "image_optimizer_default_settings", value)
+
+    @property
     @pulumi.getter
     def imported(self) -> Optional[pulumi.Input[bool]]:
         """
-        Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
+        Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the
+        import is finished
         """
         return pulumi.get(self, "imported")
 
     @imported.setter
     def imported(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "imported", value)
 
@@ -1001,15 +1041,17 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def package(self) -> Optional[pulumi.Input['ServiceComputePackageArgs']]:
         """
-        The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
+        The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted,
+        ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on
+        [Compute](https://developer.fastly.com/learning/compute/)
         """
         return pulumi.get(self, "package")
 
     @package.setter
     def package(self, value: Optional[pulumi.Input['ServiceComputePackageArgs']]):
         pulumi.set(self, "package", value)
 
@@ -1063,14 +1105,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  activate: Optional[pulumi.Input[bool]] = None,
                  backends: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeBackendArgs']]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  dictionaries: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDictionaryArgs']]]]] = None,
                  domains: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDomainArgs']]]]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None,
+                 image_optimizer_default_settings: Optional[pulumi.Input[pulumi.InputType['ServiceComputeImageOptimizerDefaultSettingsArgs']]] = None,
                  logging_bigqueries: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingBigqueryArgs']]]]] = None,
                  logging_blobstorages: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingBlobstorageArgs']]]]] = None,
                  logging_cloudfiles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingCloudfileArgs']]]]] = None,
                  logging_datadogs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingDatadogArgs']]]]] = None,
                  logging_digitaloceans: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingDigitaloceanArgs']]]]] = None,
                  logging_elasticsearches: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingElasticsearchArgs']]]]] = None,
                  logging_ftps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingFtpArgs']]]]] = None,
@@ -1115,19 +1158,23 @@
 
         ```sh
         $ pulumi import fastly:index/serviceCompute:ServiceCompute demo xxxxxxxxxxxxxxxxxxxx@2
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+               will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
-        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+               `false`
         :param pulumi.Input[str] name: The unique name for the Service to create
-        :param pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
+        :param pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted,
+               ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on
+               [Compute](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeResourceLinkArgs']]]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -1167,14 +1214,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  activate: Optional[pulumi.Input[bool]] = None,
                  backends: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeBackendArgs']]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  dictionaries: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDictionaryArgs']]]]] = None,
                  domains: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDomainArgs']]]]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None,
+                 image_optimizer_default_settings: Optional[pulumi.Input[pulumi.InputType['ServiceComputeImageOptimizerDefaultSettingsArgs']]] = None,
                  logging_bigqueries: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingBigqueryArgs']]]]] = None,
                  logging_blobstorages: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingBlobstorageArgs']]]]] = None,
                  logging_cloudfiles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingCloudfileArgs']]]]] = None,
                  logging_datadogs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingDatadogArgs']]]]] = None,
                  logging_digitaloceans: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingDigitaloceanArgs']]]]] = None,
                  logging_elasticsearches: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingElasticsearchArgs']]]]] = None,
                  logging_ftps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingFtpArgs']]]]] = None,
@@ -1216,14 +1264,15 @@
             __props__.__dict__["backends"] = backends
             __props__.__dict__["comment"] = comment
             __props__.__dict__["dictionaries"] = dictionaries
             if domains is None and not opts.urn:
                 raise TypeError("Missing required property 'domains'")
             __props__.__dict__["domains"] = domains
             __props__.__dict__["force_destroy"] = force_destroy
+            __props__.__dict__["image_optimizer_default_settings"] = image_optimizer_default_settings
             __props__.__dict__["logging_bigqueries"] = logging_bigqueries
             __props__.__dict__["logging_blobstorages"] = logging_blobstorages
             __props__.__dict__["logging_cloudfiles"] = logging_cloudfiles
             __props__.__dict__["logging_datadogs"] = logging_datadogs
             __props__.__dict__["logging_digitaloceans"] = logging_digitaloceans
             __props__.__dict__["logging_elasticsearches"] = logging_elasticsearches
             __props__.__dict__["logging_ftps"] = logging_ftps
@@ -1271,14 +1320,15 @@
             backends: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeBackendArgs']]]]] = None,
             cloned_version: Optional[pulumi.Input[int]] = None,
             comment: Optional[pulumi.Input[str]] = None,
             dictionaries: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDictionaryArgs']]]]] = None,
             domains: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDomainArgs']]]]] = None,
             force_destroy: Optional[pulumi.Input[bool]] = None,
             force_refresh: Optional[pulumi.Input[bool]] = None,
+            image_optimizer_default_settings: Optional[pulumi.Input[pulumi.InputType['ServiceComputeImageOptimizerDefaultSettingsArgs']]] = None,
             imported: Optional[pulumi.Input[bool]] = None,
             logging_bigqueries: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingBigqueryArgs']]]]] = None,
             logging_blobstorages: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingBlobstorageArgs']]]]] = None,
             logging_cloudfiles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingCloudfileArgs']]]]] = None,
             logging_datadogs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingDatadogArgs']]]]] = None,
             logging_digitaloceans: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingDigitaloceanArgs']]]]] = None,
             logging_elasticsearches: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingElasticsearchArgs']]]]] = None,
@@ -1311,22 +1361,27 @@
         """
         Get an existing ServiceCompute resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+               will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
-        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
-        :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+               `false`
+        :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the
+               import is finished
         :param pulumi.Input[str] name: The unique name for the Service to create
-        :param pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
+        :param pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted,
+               ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on
+               [Compute](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeResourceLinkArgs']]]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ServiceComputeState.__new__(_ServiceComputeState)
 
@@ -1335,14 +1390,15 @@
         __props__.__dict__["backends"] = backends
         __props__.__dict__["cloned_version"] = cloned_version
         __props__.__dict__["comment"] = comment
         __props__.__dict__["dictionaries"] = dictionaries
         __props__.__dict__["domains"] = domains
         __props__.__dict__["force_destroy"] = force_destroy
         __props__.__dict__["force_refresh"] = force_refresh
+        __props__.__dict__["image_optimizer_default_settings"] = image_optimizer_default_settings
         __props__.__dict__["imported"] = imported
         __props__.__dict__["logging_bigqueries"] = logging_bigqueries
         __props__.__dict__["logging_blobstorages"] = logging_blobstorages
         __props__.__dict__["logging_cloudfiles"] = logging_cloudfiles
         __props__.__dict__["logging_datadogs"] = logging_datadogs
         __props__.__dict__["logging_digitaloceans"] = logging_digitaloceans
         __props__.__dict__["logging_elasticsearches"] = logging_elasticsearches
@@ -1374,15 +1430,16 @@
         __props__.__dict__["version_comment"] = version_comment
         return ServiceCompute(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def activate(self) -> pulumi.Output[Optional[bool]]:
         """
-        Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+        will not activate it if this is set to `false`. Default `true`
         """
         return pulumi.get(self, "activate")
 
     @property
     @pulumi.getter(name="activeVersion")
     def active_version(self) -> pulumi.Output[int]:
         """
@@ -1421,28 +1478,35 @@
         """
         return pulumi.get(self, "domains")
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> pulumi.Output[Optional[bool]]:
         """
-        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+        `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @property
     @pulumi.getter(name="forceRefresh")
     def force_refresh(self) -> pulumi.Output[bool]:
         return pulumi.get(self, "force_refresh")
 
     @property
+    @pulumi.getter(name="imageOptimizerDefaultSettings")
+    def image_optimizer_default_settings(self) -> pulumi.Output[Optional['outputs.ServiceComputeImageOptimizerDefaultSettings']]:
+        return pulumi.get(self, "image_optimizer_default_settings")
+
+    @property
     @pulumi.getter
     def imported(self) -> pulumi.Output[bool]:
         """
-        Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
+        Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the
+        import is finished
         """
         return pulumi.get(self, "imported")
 
     @property
     @pulumi.getter(name="loggingBigqueries")
     def logging_bigqueries(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceComputeLoggingBigquery']]]:
         return pulumi.get(self, "logging_bigqueries")
@@ -1580,15 +1644,17 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def package(self) -> pulumi.Output[Optional['outputs.ServiceComputePackage']]:
         """
-        The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
+        The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted,
+        ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on
+        [Compute](https://developer.fastly.com/learning/compute/)
         """
         return pulumi.get(self, "package")
 
     @property
     @pulumi.getter(name="productEnablement")
     def product_enablement(self) -> pulumi.Output[Optional['outputs.ServiceComputeProductEnablement']]:
         return pulumi.get(self, "product_enablement")
```

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_vcl.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_vcl.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
                  directors: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclDirectorArgs']]]] = None,
                  dynamicsnippets: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclDynamicsnippetArgs']]]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None,
                  gzips: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclGzipArgs']]]] = None,
                  headers: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclHeaderArgs']]]] = None,
                  healthchecks: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclHealthcheckArgs']]]] = None,
                  http3: Optional[pulumi.Input[bool]] = None,
+                 image_optimizer_default_settings: Optional[pulumi.Input['ServiceVclImageOptimizerDefaultSettingsArgs']] = None,
                  logging_bigqueries: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingBigqueryArgs']]]] = None,
                  logging_blobstorages: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingBlobstorageArgs']]]] = None,
                  logging_cloudfiles: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingCloudfileArgs']]]] = None,
                  logging_datadogs: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingDatadogArgs']]]] = None,
                  logging_digitaloceans: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingDigitaloceanArgs']]]] = None,
                  logging_elasticsearches: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingElasticsearchArgs']]]] = None,
                  logging_ftps: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingFtpArgs']]]] = None,
@@ -71,18 +72,20 @@
                  stale_if_error_ttl: Optional[pulumi.Input[int]] = None,
                  vcls: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclVclArgs']]]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None,
                  waf: Optional[pulumi.Input['ServiceVclWafArgs']] = None):
         """
         The set of arguments for constructing a ServiceVcl resource.
         :param pulumi.Input[Sequence[pulumi.Input['ServiceVclDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
-        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+               will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[str] default_host: The default hostname
         :param pulumi.Input[int] default_ttl: The default Time-to-live (TTL) for requests
-        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+               `false`
         :param pulumi.Input[bool] http3: Enables support for the HTTP/3 (QUIC) protocol
         :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[bool] stale_if_error: Enables serving a stale object if there is an error
         :param pulumi.Input[int] stale_if_error_ttl: The default time-to-live (TTL) for serving the stale object for the version
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         pulumi.set(__self__, "domains", domains)
@@ -114,14 +117,16 @@
             pulumi.set(__self__, "gzips", gzips)
         if headers is not None:
             pulumi.set(__self__, "headers", headers)
         if healthchecks is not None:
             pulumi.set(__self__, "healthchecks", healthchecks)
         if http3 is not None:
             pulumi.set(__self__, "http3", http3)
+        if image_optimizer_default_settings is not None:
+            pulumi.set(__self__, "image_optimizer_default_settings", image_optimizer_default_settings)
         if logging_bigqueries is not None:
             pulumi.set(__self__, "logging_bigqueries", logging_bigqueries)
         if logging_blobstorages is not None:
             pulumi.set(__self__, "logging_blobstorages", logging_blobstorages)
         if logging_cloudfiles is not None:
             pulumi.set(__self__, "logging_cloudfiles", logging_cloudfiles)
         if logging_datadogs is not None:
@@ -218,15 +223,16 @@
     def acls(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclAclArgs']]]]):
         pulumi.set(self, "acls", value)
 
     @property
     @pulumi.getter
     def activate(self) -> Optional[pulumi.Input[bool]]:
         """
-        Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+        will not activate it if this is set to `false`. Default `true`
         """
         return pulumi.get(self, "activate")
 
     @activate.setter
     def activate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "activate", value)
 
@@ -317,15 +323,16 @@
     def dynamicsnippets(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclDynamicsnippetArgs']]]]):
         pulumi.set(self, "dynamicsnippets", value)
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
-        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+        `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @force_destroy.setter
     def force_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_destroy", value)
 
@@ -365,14 +372,23 @@
         return pulumi.get(self, "http3")
 
     @http3.setter
     def http3(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "http3", value)
 
     @property
+    @pulumi.getter(name="imageOptimizerDefaultSettings")
+    def image_optimizer_default_settings(self) -> Optional[pulumi.Input['ServiceVclImageOptimizerDefaultSettingsArgs']]:
+        return pulumi.get(self, "image_optimizer_default_settings")
+
+    @image_optimizer_default_settings.setter
+    def image_optimizer_default_settings(self, value: Optional[pulumi.Input['ServiceVclImageOptimizerDefaultSettingsArgs']]):
+        pulumi.set(self, "image_optimizer_default_settings", value)
+
+    @property
     @pulumi.getter(name="loggingBigqueries")
     def logging_bigqueries(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingBigqueryArgs']]]]:
         return pulumi.get(self, "logging_bigqueries")
 
     @logging_bigqueries.setter
     def logging_bigqueries(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingBigqueryArgs']]]]):
         pulumi.set(self, "logging_bigqueries", value)
@@ -751,14 +767,15 @@
                  dynamicsnippets: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclDynamicsnippetArgs']]]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None,
                  force_refresh: Optional[pulumi.Input[bool]] = None,
                  gzips: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclGzipArgs']]]] = None,
                  headers: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclHeaderArgs']]]] = None,
                  healthchecks: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclHealthcheckArgs']]]] = None,
                  http3: Optional[pulumi.Input[bool]] = None,
+                 image_optimizer_default_settings: Optional[pulumi.Input['ServiceVclImageOptimizerDefaultSettingsArgs']] = None,
                  imported: Optional[pulumi.Input[bool]] = None,
                  logging_bigqueries: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingBigqueryArgs']]]] = None,
                  logging_blobstorages: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingBlobstorageArgs']]]] = None,
                  logging_cloudfiles: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingCloudfileArgs']]]] = None,
                  logging_datadogs: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingDatadogArgs']]]] = None,
                  logging_digitaloceans: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingDigitaloceanArgs']]]] = None,
                  logging_elasticsearches: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingElasticsearchArgs']]]] = None,
@@ -793,23 +810,26 @@
                  stale_if_error: Optional[pulumi.Input[bool]] = None,
                  stale_if_error_ttl: Optional[pulumi.Input[int]] = None,
                  vcls: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclVclArgs']]]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None,
                  waf: Optional[pulumi.Input['ServiceVclWafArgs']] = None):
         """
         Input properties used for looking up and filtering ServiceVcl resources.
-        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+               will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
         :param pulumi.Input[str] default_host: The default hostname
         :param pulumi.Input[int] default_ttl: The default Time-to-live (TTL) for requests
         :param pulumi.Input[Sequence[pulumi.Input['ServiceVclDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
-        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+               `false`
         :param pulumi.Input[bool] http3: Enables support for the HTTP/3 (QUIC) protocol
-        :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
+        :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the
+               import is finished
         :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[bool] stale_if_error: Enables serving a stale object if there is an error
         :param pulumi.Input[int] stale_if_error_ttl: The default time-to-live (TTL) for serving the stale object for the version
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         if acls is not None:
             pulumi.set(__self__, "acls", acls)
@@ -847,14 +867,16 @@
             pulumi.set(__self__, "gzips", gzips)
         if headers is not None:
             pulumi.set(__self__, "headers", headers)
         if healthchecks is not None:
             pulumi.set(__self__, "healthchecks", healthchecks)
         if http3 is not None:
             pulumi.set(__self__, "http3", http3)
+        if image_optimizer_default_settings is not None:
+            pulumi.set(__self__, "image_optimizer_default_settings", image_optimizer_default_settings)
         if imported is not None:
             pulumi.set(__self__, "imported", imported)
         if logging_bigqueries is not None:
             pulumi.set(__self__, "logging_bigqueries", logging_bigqueries)
         if logging_blobstorages is not None:
             pulumi.set(__self__, "logging_blobstorages", logging_blobstorages)
         if logging_cloudfiles is not None:
@@ -941,15 +963,16 @@
     def acls(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclAclArgs']]]]):
         pulumi.set(self, "acls", value)
 
     @property
     @pulumi.getter
     def activate(self) -> Optional[pulumi.Input[bool]]:
         """
-        Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+        will not activate it if this is set to `false`. Default `true`
         """
         return pulumi.get(self, "activate")
 
     @activate.setter
     def activate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "activate", value)
 
@@ -1076,15 +1099,16 @@
     def dynamicsnippets(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclDynamicsnippetArgs']]]]):
         pulumi.set(self, "dynamicsnippets", value)
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
-        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+        `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @force_destroy.setter
     def force_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_destroy", value)
 
@@ -1133,18 +1157,28 @@
         return pulumi.get(self, "http3")
 
     @http3.setter
     def http3(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "http3", value)
 
     @property
+    @pulumi.getter(name="imageOptimizerDefaultSettings")
+    def image_optimizer_default_settings(self) -> Optional[pulumi.Input['ServiceVclImageOptimizerDefaultSettingsArgs']]:
+        return pulumi.get(self, "image_optimizer_default_settings")
+
+    @image_optimizer_default_settings.setter
+    def image_optimizer_default_settings(self, value: Optional[pulumi.Input['ServiceVclImageOptimizerDefaultSettingsArgs']]):
+        pulumi.set(self, "image_optimizer_default_settings", value)
+
+    @property
     @pulumi.getter
     def imported(self) -> Optional[pulumi.Input[bool]]:
         """
-        Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
+        Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the
+        import is finished
         """
         return pulumi.get(self, "imported")
 
     @imported.setter
     def imported(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "imported", value)
 
@@ -1530,14 +1564,15 @@
                  domains: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDomainArgs']]]]] = None,
                  dynamicsnippets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDynamicsnippetArgs']]]]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None,
                  gzips: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclGzipArgs']]]]] = None,
                  headers: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclHeaderArgs']]]]] = None,
                  healthchecks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclHealthcheckArgs']]]]] = None,
                  http3: Optional[pulumi.Input[bool]] = None,
+                 image_optimizer_default_settings: Optional[pulumi.Input[pulumi.InputType['ServiceVclImageOptimizerDefaultSettingsArgs']]] = None,
                  logging_bigqueries: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingBigqueryArgs']]]]] = None,
                  logging_blobstorages: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingBlobstorageArgs']]]]] = None,
                  logging_cloudfiles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingCloudfileArgs']]]]] = None,
                  logging_datadogs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingDatadogArgs']]]]] = None,
                  logging_digitaloceans: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingDigitaloceanArgs']]]]] = None,
                  logging_elasticsearches: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingElasticsearchArgs']]]]] = None,
                  logging_ftps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingFtpArgs']]]]] = None,
@@ -1589,19 +1624,21 @@
 
         ```sh
         $ pulumi import fastly:index/serviceVcl:ServiceVcl demo xxxxxxxxxxxxxxxxxxxx@2
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+               will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[str] default_host: The default hostname
         :param pulumi.Input[int] default_ttl: The default Time-to-live (TTL) for requests
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
-        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+               `false`
         :param pulumi.Input[bool] http3: Enables support for the HTTP/3 (QUIC) protocol
         :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[bool] stale_if_error: Enables serving a stale object if there is an error
         :param pulumi.Input[int] stale_if_error_ttl: The default time-to-live (TTL) for serving the stale object for the version
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         ...
@@ -1655,14 +1692,15 @@
                  domains: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDomainArgs']]]]] = None,
                  dynamicsnippets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDynamicsnippetArgs']]]]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None,
                  gzips: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclGzipArgs']]]]] = None,
                  headers: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclHeaderArgs']]]]] = None,
                  healthchecks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclHealthcheckArgs']]]]] = None,
                  http3: Optional[pulumi.Input[bool]] = None,
+                 image_optimizer_default_settings: Optional[pulumi.Input[pulumi.InputType['ServiceVclImageOptimizerDefaultSettingsArgs']]] = None,
                  logging_bigqueries: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingBigqueryArgs']]]]] = None,
                  logging_blobstorages: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingBlobstorageArgs']]]]] = None,
                  logging_cloudfiles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingCloudfileArgs']]]]] = None,
                  logging_datadogs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingDatadogArgs']]]]] = None,
                  logging_digitaloceans: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingDigitaloceanArgs']]]]] = None,
                  logging_elasticsearches: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingElasticsearchArgs']]]]] = None,
                  logging_ftps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingFtpArgs']]]]] = None,
@@ -1722,14 +1760,15 @@
             __props__.__dict__["domains"] = domains
             __props__.__dict__["dynamicsnippets"] = dynamicsnippets
             __props__.__dict__["force_destroy"] = force_destroy
             __props__.__dict__["gzips"] = gzips
             __props__.__dict__["headers"] = headers
             __props__.__dict__["healthchecks"] = healthchecks
             __props__.__dict__["http3"] = http3
+            __props__.__dict__["image_optimizer_default_settings"] = image_optimizer_default_settings
             __props__.__dict__["logging_bigqueries"] = logging_bigqueries
             __props__.__dict__["logging_blobstorages"] = logging_blobstorages
             __props__.__dict__["logging_cloudfiles"] = logging_cloudfiles
             __props__.__dict__["logging_datadogs"] = logging_datadogs
             __props__.__dict__["logging_digitaloceans"] = logging_digitaloceans
             __props__.__dict__["logging_elasticsearches"] = logging_elasticsearches
             __props__.__dict__["logging_ftps"] = logging_ftps
@@ -1795,14 +1834,15 @@
             dynamicsnippets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDynamicsnippetArgs']]]]] = None,
             force_destroy: Optional[pulumi.Input[bool]] = None,
             force_refresh: Optional[pulumi.Input[bool]] = None,
             gzips: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclGzipArgs']]]]] = None,
             headers: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclHeaderArgs']]]]] = None,
             healthchecks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclHealthcheckArgs']]]]] = None,
             http3: Optional[pulumi.Input[bool]] = None,
+            image_optimizer_default_settings: Optional[pulumi.Input[pulumi.InputType['ServiceVclImageOptimizerDefaultSettingsArgs']]] = None,
             imported: Optional[pulumi.Input[bool]] = None,
             logging_bigqueries: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingBigqueryArgs']]]]] = None,
             logging_blobstorages: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingBlobstorageArgs']]]]] = None,
             logging_cloudfiles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingCloudfileArgs']]]]] = None,
             logging_datadogs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingDatadogArgs']]]]] = None,
             logging_digitaloceans: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingDigitaloceanArgs']]]]] = None,
             logging_elasticsearches: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingElasticsearchArgs']]]]] = None,
@@ -1842,23 +1882,26 @@
         """
         Get an existing ServiceVcl resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+               will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
         :param pulumi.Input[str] default_host: The default hostname
         :param pulumi.Input[int] default_ttl: The default Time-to-live (TTL) for requests
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
-        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+               `false`
         :param pulumi.Input[bool] http3: Enables support for the HTTP/3 (QUIC) protocol
-        :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
+        :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the
+               import is finished
         :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[bool] stale_if_error: Enables serving a stale object if there is an error
         :param pulumi.Input[int] stale_if_error_ttl: The default time-to-live (TTL) for serving the stale object for the version
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -1880,14 +1923,15 @@
         __props__.__dict__["dynamicsnippets"] = dynamicsnippets
         __props__.__dict__["force_destroy"] = force_destroy
         __props__.__dict__["force_refresh"] = force_refresh
         __props__.__dict__["gzips"] = gzips
         __props__.__dict__["headers"] = headers
         __props__.__dict__["healthchecks"] = healthchecks
         __props__.__dict__["http3"] = http3
+        __props__.__dict__["image_optimizer_default_settings"] = image_optimizer_default_settings
         __props__.__dict__["imported"] = imported
         __props__.__dict__["logging_bigqueries"] = logging_bigqueries
         __props__.__dict__["logging_blobstorages"] = logging_blobstorages
         __props__.__dict__["logging_cloudfiles"] = logging_cloudfiles
         __props__.__dict__["logging_datadogs"] = logging_datadogs
         __props__.__dict__["logging_digitaloceans"] = logging_digitaloceans
         __props__.__dict__["logging_elasticsearches"] = logging_elasticsearches
@@ -1931,15 +1975,16 @@
     def acls(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclAcl']]]:
         return pulumi.get(self, "acls")
 
     @property
     @pulumi.getter
     def activate(self) -> pulumi.Output[Optional[bool]]:
         """
-        Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
+        Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but
+        will not activate it if this is set to `false`. Default `true`
         """
         return pulumi.get(self, "activate")
 
     @property
     @pulumi.getter(name="activeVersion")
     def active_version(self) -> pulumi.Output[int]:
         """
@@ -2014,15 +2059,16 @@
     def dynamicsnippets(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclDynamicsnippet']]]:
         return pulumi.get(self, "dynamicsnippets")
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> pulumi.Output[Optional[bool]]:
         """
-        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default
+        `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @property
     @pulumi.getter(name="forceRefresh")
     def force_refresh(self) -> pulumi.Output[bool]:
         return pulumi.get(self, "force_refresh")
@@ -2047,18 +2093,24 @@
     def http3(self) -> pulumi.Output[Optional[bool]]:
         """
         Enables support for the HTTP/3 (QUIC) protocol
         """
         return pulumi.get(self, "http3")
 
     @property
+    @pulumi.getter(name="imageOptimizerDefaultSettings")
+    def image_optimizer_default_settings(self) -> pulumi.Output[Optional['outputs.ServiceVclImageOptimizerDefaultSettings']]:
+        return pulumi.get(self, "image_optimizer_default_settings")
+
+    @property
     @pulumi.getter
     def imported(self) -> pulumi.Output[bool]:
         """
-        Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
+        Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the
+        import is finished
         """
         return pulumi.get(self, "imported")
 
     @property
     @pulumi.getter(name="loggingBigqueries")
     def logging_bigqueries(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclLoggingBigquery']]]:
         return pulumi.get(self, "logging_bigqueries")
```

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_activation.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_mutual_authentication.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly/user.py` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.8.0a1715756624
+Version: 8.8.0a1715970151
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.8.0a1715756624/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-8.8.0a1715970151/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.8.0a1715756624/pyproject.toml` & `pulumi_fastly-8.8.0a1715970151/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_fastly"
   description = "A Pulumi package for creating and managing fastly cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "fastly"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "8.8.0a1715756624"
+  version = "8.8.0a1715970151"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-fastly"
 
 [build-system]
```

