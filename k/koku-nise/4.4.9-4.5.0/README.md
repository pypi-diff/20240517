# Comparing `tmp/koku-nise-4.4.9.tar.gz` & `tmp/koku-nise-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koku-nise-4.4.9.tar", last modified: Wed Nov 15 11:12:26 2023, max compression
+gzip compressed data, was "koku-nise-4.5.0.tar", last modified: Fri May 17 17:09:29 2024, max compression
```

## Comparing `koku-nise-4.4.9.tar` & `koku-nise-4.5.0.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.459130 koku-nise-4.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2023-11-15 11:12:08.000000 koku-nise-4.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-15 11:12:08.000000 koku-nise-4.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-11-15 11:12:26.459130 koku-nise-4.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2023-11-15 11:12:08.000000 koku-nise-4.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.451130 koku-nise-4.4.9/koku_nise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.451130 koku-nise-4.4.9/nise/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28577 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/aws-template-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.451130 koku-nise-4.4.9/nise/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.451130 koku-nise-4.4.9/nise/generators/aws/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/aws_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13391 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/aws_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/data_transfer_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/ebs_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/ec2_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/marketplace_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/rds_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/route53_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/s3_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/vpc_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/generators/azure/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16623 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/azure_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/bandwidth_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/ccsp_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/sql_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/virtual_machine_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/virtual_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/cloud_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/compute_engine_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/gcp_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/gcp_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8099 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/gcp_network_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/hcs_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/project_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/generators/oci/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/oci_block_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/oci_compute_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/oci_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/oci_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/oci_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/oci_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40379 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/ocp/ocp_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    55930 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/util/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/yaml_generators/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/yaml_generators/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71376 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/aws/ec2_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9814 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/aws/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/aws/rds_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/aws/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/yaml_generators/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/azure/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.459130 koku-nise-4.4.9/nise/yaml_generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/gcp/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.459130 koku-nise-4.4.9/nise/yaml_generators/oci/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/oci/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/oci/oci_yaml_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.459130 koku-nise-4.4.9/nise/yaml_generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/ocp/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.459130 koku-nise-4.4.9/nise/yaml_generators/ocp_on_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/ocp_on_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/ocp_on_cloud/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.459130 koku-nise-4.4.9/nise/yaml_generators/static/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/aws_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/aws_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/azure_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/azure_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/gcp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/gcp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/oci_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/oci_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      896 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/ocp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/ocp_on_cloud_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/ocp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 11:12:26.459130 koku-nise-4.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2023-11-15 11:12:08.000000 koku-nise-4.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-05-17 17:09:13.000000 koku-nise-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-17 17:09:13.000000 koku-nise-4.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-17 17:09:29.068084 koku-nise-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-05-17 17:09:13.000000 koku-nise-4.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.056084 koku-nise-4.5.0/koku_nise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.060084 koku-nise-4.5.0/nise/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/aws-template-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.060084 koku-nise-4.5.0/nise/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.060084 koku-nise-4.5.0/nise/generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/aws_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/aws_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/data_transfer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/ebs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/ec2_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/marketplace_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/rds_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/route53_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/s3_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/vpc_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16807 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/azure_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/bandwidth_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/ccsp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/data_transfer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/sql_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/virtual_machine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/virtual_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/cloud_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/compute_engine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/gcp_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/gcp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/gcp_network_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/hcs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/project_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/oci_block_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/oci_compute_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/oci_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/oci_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/oci_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/oci_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43084 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/ocp/ocp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56209 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/util/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/yaml_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/yaml_generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71376 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/aws/ec2_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/aws/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/aws/rds_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/aws/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/nise/yaml_generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/azure/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/nise/yaml_generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/gcp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/nise/yaml_generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/oci/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/oci/oci_yaml_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/nise/yaml_generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/ocp/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/nise/yaml_generators/ocp_on_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/ocp_on_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/ocp_on_cloud/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/nise/yaml_generators/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/aws_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/aws_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/azure_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/azure_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/gcp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/gcp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/oci_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/oci_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/ocp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/ocp_on_cloud_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/ocp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 17:09:29.068084 koku-nise-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-17 17:09:13.000000 koku-nise-4.5.0/setup.py
```

### Comparing `koku-nise-4.4.9/LICENSE` & `koku-nise-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/README.md` & `koku-nise-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/koku_nise.egg-info/SOURCES.txt` & `koku-nise-4.5.0/koku_nise.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 nise/generators/aws/route53_generator.py
 nise/generators/aws/s3_generator.py
 nise/generators/aws/vpc_generator.py
 nise/generators/azure/__init__.py
 nise/generators/azure/azure_generator.py
 nise/generators/azure/bandwidth_generator.py
 nise/generators/azure/ccsp_generator.py
+nise/generators/azure/data_transfer_generator.py
 nise/generators/azure/sql_database_generator.py
 nise/generators/azure/storage_generator.py
 nise/generators/azure/virtual_machine_generator.py
 nise/generators/azure/virtual_network_generator.py
 nise/generators/gcp/__init__.py
 nise/generators/gcp/cloud_storage_generator.py
 nise/generators/gcp/compute_engine_generator.py
```

### Comparing `koku-nise-4.4.9/nise/__main__.py` & `koku-nise-4.5.0/nise/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -689,26 +689,33 @@
 
     LOG.info("Loading static data...")
     aws_tags = set()
     start_dates = []
     end_dates = []
     static_report_data = load_yaml(static_file)
     for generator_dict in static_report_data.get("generators"):
-        for _, attributes in generator_dict.items():
+        for attributes in generator_dict.values():
             start_date = get_start_date(attributes, options)
             generated_start_date = calculate_start_date(start_date)
             start_dates.append(generated_start_date)
-            if attributes.get("end_date"):
-                generated_end_date = calculate_end_date(generated_start_date, attributes.get("end_date"))
-            elif options.get("end_date") and options.get("end_date").date() != today().date():
-                generated_end_date = calculate_end_date(generated_start_date, options.get("end_date"))
-            else:
-                generated_end_date = today()
+
+            end_date = attributes.get("end_date", options.get("end_date"))
+            generated_end_date = today()
+            if end_date and (
+                end_date != today().date()
+                or (
+                    isinstance(end_date, datetime.datetime)
+                    and (end_date.date() != today().date() or end_date.hour != 0)
+                )
+            ):
+                generated_end_date = calculate_end_date(generated_start_date, end_date)
+
             if options.get("provider") == "azure":
                 generated_end_date += datetime.timedelta(hours=24)
+
             end_dates.append(generated_end_date)
 
             attributes["start_date"] = str(generated_start_date)
             attributes["end_date"] = str(generated_end_date)
 
             if options.get("provider") == "aws":
                 aws_tags.update(attributes.get("tags", {}).keys())
@@ -737,16 +744,18 @@
 
 def calculate_start_date(start_date):
     """Return a datetime for the start date."""
     if start_date == "last_month":
         generated_start_date = today().replace(day=1, hour=0, minute=0, second=0) + relativedelta(months=-1)
     elif start_date == "today":
         generated_start_date = today().replace(hour=0, minute=0, second=0)
-    elif start_date and isinstance(start_date, datetime.date):
+    elif start_date and isinstance(start_date, datetime.datetime):
         generated_start_date = start_date
+    elif start_date and isinstance(start_date, datetime.date):
+        generated_start_date = datetime.datetime(start_date.year, start_date.month, start_date.day)
     elif start_date:
         generated_start_date = date_parser.parse(start_date)
     else:
         generated_start_date = today().replace(day=1, hour=0, minute=0, second=0)
     if generated_start_date.tzinfo is None:
         generated_start_date = generated_start_date.replace(tzinfo=timezone.utc)
     return generated_start_date
@@ -755,16 +764,18 @@
 def calculate_end_date(start_date, end_date):
     """Return a datetime for the end date."""
     try:
         if end_date == "last_month":
             generated_end_date = today().replace(day=1, hour=0, minute=0, second=0) + relativedelta(months=-1)
         elif end_date == "today":
             generated_end_date = today().replace(hour=0, minute=0, second=0)
-        elif end_date and isinstance(end_date, datetime.date):
+        elif end_date and isinstance(end_date, datetime.datetime):
             generated_end_date = end_date
+        elif end_date and isinstance(end_date, datetime.date):
+            generated_end_date = datetime.datetime(end_date.year, end_date.month, end_date.day)
         else:
             generated_end_date = date_parser.parse(end_date)
     except TypeError:
         offset = end_date
         offset_date = start_date + relativedelta(days=offset)
         if offset_date.month > start_date.month:
             generated_end_date = offset_date
```

### Comparing `koku-nise-4.4.9/nise/aws-template-manifest.json` & `koku-nise-4.5.0/nise/aws-template-manifest.json`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/copy.py` & `koku-nise-4.5.0/nise/copy.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/extract.py` & `koku-nise-4.5.0/nise/extract.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/aws/__init__.py` & `koku-nise-4.5.0/nise/generators/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/aws/aws_constants.py` & `koku-nise-4.5.0/nise/generators/aws/aws_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 """AWS Report Constants"""
 
 REGIONS = (
+    # (location description, region code, sub region code, storage region)
     ("US East (N. Virginia)", "us-east-1", "us-east-1a", "USE1-EBS"),
     ("US East (N. Virginia)", "us-east-1", "us-east-1b", "USE1-EBS"),
     ("US East (N. Virginia)", "us-east-1", "us-east-1c", "USE1-EBS"),
     ("US East (N. Virginia)", "us-east-1", "us-east-1d", "USE1-EBS"),
     ("US East (N. Virginia)", "us-east-1", "us-east-1e", "USE1-EBS"),
     ("US East (N. Virginia)", "us-east-1", "us-east-1f", "USE1-EBS"),
     ("US West (N. California)", "us-west-1", "us-west-1a", "USW1-EBS"),
@@ -49,14 +50,14 @@
     ("Asia Pacific (Seoul)", "ap-northeast-2", "ap-northeast-2a", "APNE2-EBS"),
     ("Asia Pacific (Osaka-Local)", "ap-northeast-3", "ap-northeast-3a", "APNE3-EBS"),
     ("China (Beijing)", "cn-north-1", "cn-north-1a", "CNN1-EBS"),
     ("China (Ningxia)", "cn-northwest-1", "cn-northwest-1a", "CNNW1-EBS"),
     ("SA East (Sao Paulo)", "sa-east-1", "sa-east-1a", "SA1-EBS"),
     ("SA East (Sao Paulo)", "sa-east-1", "sa-east-1b", "SA1-EBS"),
     ("SA East (Sao Paulo)", "sa-east-1", "sa-east-1c", "SA1-EBS"),
-    ("Asia Pacific (Mumbai)	", "ap-south-1", "ap-south-1a", "APS1-EBS"),
-    ("Asia Pacific (Mumbai)	", "ap-south-1", "ap-south-1b", "APS1-EBS"),
+    ("Asia Pacific (Mumbai)", "ap-south-1", "ap-south-1a", "APS1-EBS"),
+    ("Asia Pacific (Mumbai)", "ap-south-1", "ap-south-1b", "APS1-EBS"),
     ("Canada (Central)", "ca-central-1", "ca-central-1a", "CAC1-EBS"),
     ("Africa (Cape Town)", "af-south-1", "af-south-1a", "AFS1-EBS"),
     ("AWS GovCloud (US-East)", "us-gov-east-1", "us-gov-east-1a", "USGE1-EBS"),
     ("AWS GovCloud (US)", "us-gov-west-1", "us-gov-west-1a", "USGW1-EBS"),
 )
```

### Comparing `koku-nise-4.4.9/nise/generators/aws/aws_generator.py` & `koku-nise-4.5.0/nise/generators/aws/aws_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,31 +320,36 @@
                 row[column] = COL_MAP.get(column)
 
         return row
 
     def _get_location(self):
         """Pick instance location."""
         options = None
-        if self.attributes and self.attributes.get("region"):
-            region = self.attributes.get("region")
+        if region := self.attributes.get("region"):
             options = [option for option in REGIONS if region in option]
         if options:
             location = choice(options)
         else:
             location = choice(REGIONS)
         return location
 
+    def _get_legal_entity(self):
+        """Pick legal entity."""
+        if self.attributes and self.attributes.get("legal_entity"):
+            return self.attributes.get("legal_entity")
+        return "Amazon Web Services, Inc."
+
     def _add_common_usage_info(self, row, start, end, **kwargs):
         """Add common usage information."""
         row["lineItem/UsageAccountId"] = choice(self.usage_accounts)
         row["lineItem/LineItemType"] = "Usage"
         row["lineItem/UsageStartDate"] = start
         row["lineItem/UsageEndDate"] = end
         row["lineItem/CurrencyCode"] = self.currency
-        row["lineItem/LegalEntity"] = "Amazon Web Services, Inc."
+        row["lineItem/LegalEntity"] = self._get_legal_entity()
         return row
 
     def _add_tag_data(self, row):
         """Add tag data to the row."""
         if self._tags:
             for tag in self._tags:
                 row[tag] = self._tags[tag]
```

### Comparing `koku-nise-4.4.9/nise/generators/aws/data_transfer_generator.py` & `koku-nise-4.5.0/nise/generators/aws/data_transfer_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,53 +21,54 @@
 from nise.generators.aws.aws_generator import AWSGenerator
 
 
 class DataTransferGenerator(AWSGenerator):
     """Generator for Data Transfer data."""
 
     DATA_TRANSFER = (
-        ("{}-{}-AWS-In-Bytes", "PublicIP-In", "InterRegion Inbound"),
-        ("{}-{}-AWS-Out-Bytes", "PublicIP-Out", "InterRegion Outbound"),
+        # (usage type, operation, transfer type)
+        ("{region1}-{region2}-AWS-{direction}-Bytes", "PublicIP-{direction}", "InterRegion {direction}bound"),
+        ("DataTransfer-{direction}-Bytes", "RunInstances", ""),
+        ("{region1}-DataTransfer-Regional-Bytes", "PublicIP-{direction}", ""),
+        ("{region1}-DataTransfer-Regional-Bytes", "InterZone-{direction}", ""),
     )
+    DATA_TRANSFER_DIRECTIONS = ("in", "out")
 
     def __init__(self, start_date, end_date, currency, payer_account, usage_accounts, attributes=None, tag_cols=None):
         """Initialize the data transfer generator."""
         super().__init__(start_date, end_date, currency, payer_account, usage_accounts, attributes, tag_cols)
-        self._amount = None
-        self._rate = None
-        self._saving = None
-        self._product_sku = None
-        self._resource_id = None
-        self._product_code = "AmazonEC2"
-        self._product_name = "Amazon Elastic Compute Cloud"
-        if attributes:
-            if attributes.get("product_code"):
-                self._product_code = attributes.get("product_code")
-            if attributes.get("product_name"):
-                self._product_name = attributes.get("product_name")
-            if attributes.get("resource_id"):
-                self._resource_id = attributes.get("resource_id")
-            if attributes.get("amount"):
-                self._amount = float(attributes.get("amount"))
-            if attributes.get("rate"):
-                self._rate = float(attributes.get("rate"))
-            if attributes.get("product_sku"):
-                self._product_sku = attributes.get("product_sku")
-            if attributes.get("tags"):
-                self._tags = attributes.get("tags")
-            if attributes.get("saving"):
-                self._saving = float(attributes.get("saving"))
+
+        self._amount = float(self.attributes.get("amount", 0)) or None
+        self._data_direction = self.attributes.get("data_direction")
+        self._product_code = self.attributes.get("product_code", "AmazonEC2")
+        self._product_name = self.attributes.get("product_name", "Amazon Elastic Compute Cloud")
+        self._product_sku = self.attributes.get("product_sku")
+        self._rate = float(self.attributes.get("rate", 0)) or None
+        self._resource_id = self.attributes.get("resource_id")
+        self._saving = float(self.attributes.get("saving", 0)) or None
+        self._tags = self.attributes.get("tags", self._tags)
+
+    @property
+    def data_direction(self):
+        if self._data_direction is not None:
+            return self._data_direction.capitalize()
+
+        # Purposefully not caching this value so a different value is returned on each call
+        return choice(self.DATA_TRANSFER_DIRECTIONS).capitalize()
 
     def _get_data_transfer(self, rate):
         """Get data transfer info."""
         location1, aws_region, _, storage_region1 = self._get_location()
         location2, _, _, storage_region2 = self._get_location()
         trans_desc, operation, trans_type = choice(self.DATA_TRANSFER)
-        trans_desc = trans_desc.format(storage_region1, storage_region2)
+        trans_desc = trans_desc.format(region1=storage_region1, region2=storage_region2, direction=self.data_direction)
+        operation = operation.format(direction=self.data_direction)
+        trans_type = trans_type.format(direction=self.data_direction)
         description = f"${rate} per GB - {location1} data transfer to {location2}"
+
         return trans_desc, operation, description, location1, location2, trans_type, aws_region
 
     def _get_product_sku(self):
         """Generate product sku."""
         if self._product_sku:
             sku = self._product_sku
         else:
```

### Comparing `koku-nise-4.4.9/nise/generators/aws/ebs_generator.py` & `koku-nise-4.5.0/nise/generators/aws/ebs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/aws/ec2_generator.py` & `koku-nise-4.5.0/nise/generators/aws/rds_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,164 +10,151 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
-"""Module for ec2 data generation."""
+"""Module for rds data generation."""
 from random import choice
 
 from nise.generators.aws.aws_generator import AWSGenerator
 
 
-class EC2Generator(AWSGenerator):
-    """Generator for EC2 data."""
+class RDSGenerator(AWSGenerator):
+    """Generator for RDS data."""
 
     INSTANCE_TYPES = (
-        # NOTE: Each tuple represents
-        # (instance type, physical_cores, vCPUs, memory, storage, family, cost, rate, savings, description)
         (
-            "m5.large",
-            "1",
+            "db.t3.medium",
+            "2",
+            "4 GiB",
+            "EBS-Only",
+            "Memory Optimized",
+            "0.072",
+            "0.072",
+            "${} per On Demand Linux {} Instance Hour",
+        ),
+        (
+            "db.t3.large",
             "2",
             "8 GiB",
             "EBS Only",
             "General Purpose",
-            "0.096",
-            "0.096",
-            "0.045",
+            "0.145",
+            "0.145",
             "${} per On Demand Linux {} Instance Hour",
         ),
         (
-            "c5d.2xlarge",
+            "db.m5.xlarge",
             "4",
-            "8",
             "16 GiB",
             "1 x 200 NVMe SSD",
             "Compute Optimized",
-            "0.34",
-            "0.34",
-            "0.17",
+            "0.356",
+            "0.356",
             "${} per On Demand Linux {} Instance Hour",
         ),
         (
-            "c4.xlarge",
-            "2",
-            "4",
-            "7.5 GiB",
+            "db.r5.2xlarge",
+            "8",
+            "64 GiB",
             "EBS-Only",
             "Compute Optimized",
-            "0.199",
-            "0.199",
-            "0.099",
-            "${} per On Demand Linux {} Instance Hour",
-        ),
-        (
-            "r4.large",
-            "1",
-            "2",
-            "15.25 GiB",
-            "EBS-Only",
-            "Memory Optimized",
-            "0.133",
-            "0.133",
-            "0.067",
+            "1.00",
+            "1.00",
             "${} per On Demand Linux {} Instance Hour",
         ),
     )
 
     ARCHS = ("32-bit", "64-bit")
 
     def __init__(self, start_date, end_date, currency, payer_account, usage_accounts, attributes=None, tag_cols=None):
-        """Initialize the EC2 generator."""
+        """Initialize the RDS generator."""
         super().__init__(start_date, end_date, currency, payer_account, usage_accounts, attributes, tag_cols)
         self._processor_arch = choice(self.ARCHS)
-        self._resource_id = "i-{}".format(self.fake.ean8())
         self._product_sku = self.fake.pystr(min_chars=12, max_chars=12).upper()
         self._instance_type = choice(self.INSTANCE_TYPES)
+        self._resource_id = "i-{}".format(self.fake.ean8())
         if self.attributes:
-            if self.attributes.get("processor_arch"):
-                self._processor_arch = self.attributes.get("processor_arch")
-            if self.attributes.get("resource_id"):
-                self._resource_id = "i-{}".format(self.attributes.get("resource_id"))
             if self.attributes.get("product_sku"):
                 self._product_sku = self.attributes.get("product_sku")
+            if self.attributes.get("resource_id"):
+                self._resource_id = "i-{}".format(self.attributes.get("resource_id"))
             if self.attributes.get("tags"):
                 self._tags = self.attributes.get("tags")
             instance_type = self.attributes.get("instance_type")
             if instance_type:
                 self._instance_type = (
                     instance_type.get("inst_type"),
-                    instance_type.get("physical_cores"),
                     instance_type.get("vcpu"),
                     instance_type.get("memory"),
                     instance_type.get("storage"),
                     instance_type.get("family"),
                     instance_type.get("cost"),
                     instance_type.get("rate"),
-                    instance_type.get("saving"),
                     "${} per On Demand Linux {} Instance Hour",
                 )
 
+    def _get_arn(self, avail_zone):
+        """Create an amazon resource name."""
+        return f"arn:aws:rds:{avail_zone}:{self.payer_account}:db:{self._resource_id}"
+
     def _update_data(self, row, start, end, **kwargs):
         """Update data with generator specific data."""
-        inst_type, physical_cores, vcpu, memory, storage, family, cost, rate, saving, description = self._instance_type
+        inst_type, vcpu, memory, storage, family, cost, rate, description = self._instance_type
         inst_description = description.format(cost, inst_type)
         location, aws_region, avail_zone, _ = self._get_location()
         row = self._add_common_usage_info(row, start, end)
-
-        row["lineItem/ProductCode"] = "AmazonEC2"
-        row["lineItem/UsageType"] = f"BoxUsage:{inst_type}"
-        row["lineItem/Operation"] = "RunInstances"
+        # split_region = aws_region.split('-')
+        # region_short_code = aws_region[0:2].upper() + split_region[1][0].upper() + split_region[2]
+        region_short_code = self._generate_region_short_code(aws_region)
+
+        row["lineItem/ProductCode"] = "AmazonRDS"
+        row["lineItem/UsageType"] = f"{region_short_code}-InstanceUsage:{inst_type}"
+        row["lineItem/Operation"] = "CreateDBInstance"
         row["lineItem/AvailabilityZone"] = avail_zone
-        row["lineItem/ResourceId"] = self._resource_id
+        row["lineItem/ResourceId"] = self._get_arn(avail_zone)
         row["lineItem/UsageAmount"] = "1"
         row["lineItem/UnblendedRate"] = rate
         row["lineItem/UnblendedCost"] = cost
         row["lineItem/BlendedRate"] = rate
         row["lineItem/BlendedCost"] = cost
         row["lineItem/LineItemDescription"] = inst_description
-        row["product/ProductName"] = "Amazon Elastic Compute Cloud"
+        row["product/ProductName"] = "Amazon Relational Database Service"
         row["product/clockSpeed"] = "2.8 GHz"
         row["product/currentGeneration"] = "Yes"
         row["product/ecu"] = "14"
         row["product/enhancedNetworkingSupported"] = "Yes"
         row["product/instanceFamily"] = family
         row["product/instanceType"] = inst_type
         row["product/licenseModel"] = "No License required"
         row["product/location"] = location
         row["product/locationType"] = "AWS Region"
         row["product/memory"] = memory
         row["product/networkPerformance"] = "Moderate"
         row["product/operatingSystem"] = "Linux"
         row["product/operation"] = "RunInstances"
-        row["product/physicalCores"] = physical_cores
         row["product/physicalProcessor"] = "Intel Xeon Family"
         row["product/preInstalledSw"] = "NA"
         row["product/processorArchitecture"] = self._processor_arch
         row["product/processorFeatures"] = "Intel AVX Intel Turbo"
-        row["product/productFamily"] = "Compute Instance"
+        row["product/productFamily"] = "Database Instance"
         row["product/region"] = aws_region
-        row["product/servicecode"] = "AmazonEC2"
+        row["product/servicecode"] = "AmazonRDS"
         row["product/sku"] = self._product_sku
         row["product/storage"] = storage
         row["product/tenancy"] = "Shared"
         row["product/usagetype"] = f"BoxUsage:{inst_type}"
         row["product/vcpu"] = vcpu
         row["pricing/publicOnDemandCost"] = cost
         row["pricing/publicOnDemandRate"] = rate
         row["pricing/term"] = "OnDemand"
         row["pricing/unit"] = "Hrs"
-        row["savingsPlan/SavingsPlanEffectiveCost"] = saving
-
-        # Overwrite lineItem/LineItemType for items with applied Savings plan
-        if saving is not None:
-            row["lineItem/LineItemType"] = "SavingsPlanCoveredUsage"
-
         self._add_tag_data(row)
         self._add_category_data(row)
+
         return row
 
     def generate_data(self, report_type=None):
         """Responsibile for generating data."""
         return self._generate_hourly_data()
```

### Comparing `koku-nise-4.4.9/nise/generators/aws/marketplace_generator.py` & `koku-nise-4.5.0/nise/generators/aws/marketplace_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/aws/rds_generator.py` & `koku-nise-4.5.0/nise/generators/aws/ec2_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,151 +10,176 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
-"""Module for rds data generation."""
+"""Module for ec2 data generation."""
 from random import choice
 
 from nise.generators.aws.aws_generator import AWSGenerator
 
 
-class RDSGenerator(AWSGenerator):
-    """Generator for RDS data."""
+class EC2Generator(AWSGenerator):
+    """Generator for EC2 data."""
 
     INSTANCE_TYPES = (
+        # NOTE: Each tuple represents
+        # (instance type, physical_cores, vCPUs, memory, storage, family, cost, rate, savings, description)
         (
-            "db.t3.medium",
-            "2",
-            "4 GiB",
-            "EBS-Only",
-            "Memory Optimized",
-            "0.072",
-            "0.072",
-            "${} per On Demand Linux {} Instance Hour",
-        ),
-        (
-            "db.t3.large",
+            "m5.large",
+            "1",
             "2",
             "8 GiB",
             "EBS Only",
             "General Purpose",
-            "0.145",
-            "0.145",
-            "${} per On Demand Linux {} Instance Hour",
+            "0.096",
+            "0.096",
+            "0.045",
+            "${cost} per On Demand Linux {inst_type} Instance Hour",
         ),
         (
-            "db.m5.xlarge",
+            "c5d.2xlarge",
             "4",
+            "8",
             "16 GiB",
             "1 x 200 NVMe SSD",
             "Compute Optimized",
-            "0.356",
-            "0.356",
-            "${} per On Demand Linux {} Instance Hour",
+            "0.34",
+            "0.34",
+            "0.17",
+            "${cost} per On Demand Linux {inst_type} Instance Hour",
         ),
         (
-            "db.r5.2xlarge",
-            "8",
-            "64 GiB",
+            "c4.xlarge",
+            "2",
+            "4",
+            "7.5 GiB",
             "EBS-Only",
             "Compute Optimized",
-            "1.00",
-            "1.00",
-            "${} per On Demand Linux {} Instance Hour",
+            "0.199",
+            "0.199",
+            "0.099",
+            "${cost} per On Demand Linux {inst_type} Instance Hour",
+        ),
+        (
+            "r4.large",
+            "1",
+            "2",
+            "15.25 GiB",
+            "EBS-Only",
+            "Memory Optimized",
+            "0.133",
+            "0.133",
+            "0.067",
+            "${cost} per On Demand Linux {inst_type} Instance Hour",
         ),
     )
 
     ARCHS = ("32-bit", "64-bit")
 
+    OPERATING_SYSTEMS = (
+        "Amazon Linux",
+        "Ubuntu",
+        "Windows Server",
+        "Red Hat Enterprise Linux",
+        "SUSE Linux Enterprise Server",
+        "openSUSE Leap",
+        "Fedora",
+        "Fedora CoreOS",
+        "Debian",
+        "CentOS",
+        "Gentoo Linux",
+        "Oracle Linux",
+        "FreeBSD",
+    )
+
     def __init__(self, start_date, end_date, currency, payer_account, usage_accounts, attributes=None, tag_cols=None):
-        """Initialize the RDS generator."""
+        """Initialize the EC2 generator."""
         super().__init__(start_date, end_date, currency, payer_account, usage_accounts, attributes, tag_cols)
         self._processor_arch = choice(self.ARCHS)
+        self._resource_id = "i-{}".format(self.fake.ean8())
         self._product_sku = self.fake.pystr(min_chars=12, max_chars=12).upper()
         self._instance_type = choice(self.INSTANCE_TYPES)
-        self._resource_id = "i-{}".format(self.fake.ean8())
-        if self.attributes:
-            if self.attributes.get("product_sku"):
-                self._product_sku = self.attributes.get("product_sku")
-            if self.attributes.get("resource_id"):
-                self._resource_id = "i-{}".format(self.attributes.get("resource_id"))
-            if self.attributes.get("tags"):
-                self._tags = self.attributes.get("tags")
-            instance_type = self.attributes.get("instance_type")
-            if instance_type:
-                self._instance_type = (
-                    instance_type.get("inst_type"),
-                    instance_type.get("vcpu"),
-                    instance_type.get("memory"),
-                    instance_type.get("storage"),
-                    instance_type.get("family"),
-                    instance_type.get("cost"),
-                    instance_type.get("rate"),
-                    "${} per On Demand Linux {} Instance Hour",
-                )
-
-    def _get_arn(self, avail_zone):
-        """Create an amazon resource name."""
-        return f"arn:aws:rds:{avail_zone}:{self.payer_account}:db:{self._resource_id}"
+        self._operating_system = choice(self.OPERATING_SYSTEMS)
+        self._processor_arch = self.attributes.get("processor_arch", choice(self.ARCHS))
+        self._resource_id = f"i-{self.attributes.get('resource_id', self.fake.ean8())}"
+        self._product_sku = self.attributes.get("product_sku", self.fake.pystr(min_chars=12, max_chars=12).upper())
+        self._tags = self.attributes.get("tags", [])
+
+        if instance_type := self.attributes.get("instance_type"):
+            self._instance_type = (
+                instance_type.get("inst_type"),
+                instance_type.get("physical_cores"),
+                instance_type.get("vcpu"),
+                instance_type.get("memory"),
+                instance_type.get("storage"),
+                instance_type.get("family"),
+                instance_type.get("cost"),
+                instance_type.get("rate"),
+                instance_type.get("saving"),
+                "${cost} per On Demand Linux {inst_type} Instance Hour",
+            )
 
     def _update_data(self, row, start, end, **kwargs):
         """Update data with generator specific data."""
-        inst_type, vcpu, memory, storage, family, cost, rate, description = self._instance_type
-        inst_description = description.format(cost, inst_type)
+        inst_type, physical_cores, vcpu, memory, storage, family, cost, rate, saving, description = self._instance_type
+        inst_description = description.format(cost=cost, inst_type=inst_type)
         location, aws_region, avail_zone, _ = self._get_location()
         row = self._add_common_usage_info(row, start, end)
-        # split_region = aws_region.split('-')
-        # region_short_code = aws_region[0:2].upper() + split_region[1][0].upper() + split_region[2]
-        region_short_code = self._generate_region_short_code(aws_region)
-
-        row["lineItem/ProductCode"] = "AmazonRDS"
-        row["lineItem/UsageType"] = f"{region_short_code}-InstanceUsage:{inst_type}"
-        row["lineItem/Operation"] = "CreateDBInstance"
+
+        row["lineItem/ProductCode"] = "AmazonEC2"
+        row["lineItem/UsageType"] = f"BoxUsage:{inst_type}"
+        row["lineItem/Operation"] = "RunInstances"
         row["lineItem/AvailabilityZone"] = avail_zone
-        row["lineItem/ResourceId"] = self._get_arn(avail_zone)
+        row["lineItem/ResourceId"] = self._resource_id
         row["lineItem/UsageAmount"] = "1"
         row["lineItem/UnblendedRate"] = rate
         row["lineItem/UnblendedCost"] = cost
         row["lineItem/BlendedRate"] = rate
         row["lineItem/BlendedCost"] = cost
         row["lineItem/LineItemDescription"] = inst_description
-        row["product/ProductName"] = "Amazon Relational Database Service"
+        row["product/ProductName"] = "Amazon Elastic Compute Cloud"
         row["product/clockSpeed"] = "2.8 GHz"
         row["product/currentGeneration"] = "Yes"
         row["product/ecu"] = "14"
         row["product/enhancedNetworkingSupported"] = "Yes"
         row["product/instanceFamily"] = family
         row["product/instanceType"] = inst_type
         row["product/licenseModel"] = "No License required"
         row["product/location"] = location
         row["product/locationType"] = "AWS Region"
         row["product/memory"] = memory
         row["product/networkPerformance"] = "Moderate"
-        row["product/operatingSystem"] = "Linux"
+        row["product/operatingSystem"] = self._operating_system
         row["product/operation"] = "RunInstances"
+        row["product/physicalCores"] = physical_cores
         row["product/physicalProcessor"] = "Intel Xeon Family"
         row["product/preInstalledSw"] = "NA"
         row["product/processorArchitecture"] = self._processor_arch
         row["product/processorFeatures"] = "Intel AVX Intel Turbo"
-        row["product/productFamily"] = "Database Instance"
+        row["product/productFamily"] = "Compute Instance"
         row["product/region"] = aws_region
-        row["product/servicecode"] = "AmazonRDS"
+        row["product/servicecode"] = "AmazonEC2"
         row["product/sku"] = self._product_sku
         row["product/storage"] = storage
         row["product/tenancy"] = "Shared"
         row["product/usagetype"] = f"BoxUsage:{inst_type}"
         row["product/vcpu"] = vcpu
         row["pricing/publicOnDemandCost"] = cost
         row["pricing/publicOnDemandRate"] = rate
         row["pricing/term"] = "OnDemand"
         row["pricing/unit"] = "Hrs"
+        row["savingsPlan/SavingsPlanEffectiveCost"] = saving
+
+        # Overwrite lineItem/LineItemType for items with applied Savings plan
+        if saving is not None:
+            row["lineItem/LineItemType"] = "SavingsPlanCoveredUsage"
+
         self._add_tag_data(row)
         self._add_category_data(row)
-
         return row
 
     def generate_data(self, report_type=None):
         """Responsibile for generating data."""
         return self._generate_hourly_data()
```

### Comparing `koku-nise-4.4.9/nise/generators/aws/route53_generator.py` & `koku-nise-4.5.0/nise/generators/aws/route53_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/aws/s3_generator.py` & `koku-nise-4.5.0/nise/generators/aws/s3_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/aws/vpc_generator.py` & `koku-nise-4.5.0/nise/generators/aws/vpc_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/azure/__init__.py` & `koku-nise-4.5.0/nise/generators/azure/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,11 +16,12 @@
 #
 """Module for azure data generators."""
 from nise.generators.azure.azure_generator import AZURE_COLUMNS  # noqa: F401
 from nise.generators.azure.azure_generator import AZURE_COLUMNS_V2  # noqa: F401
 from nise.generators.azure.azure_generator import AzureGenerator  # noqa: F401
 from nise.generators.azure.bandwidth_generator import BandwidthGenerator  # noqa: F401
 from nise.generators.azure.ccsp_generator import CCSPGenerator  # noqa: F401
+from nise.generators.azure.data_transfer_generator import DTGenerator  # noqa: F401
 from nise.generators.azure.sql_database_generator import SQLGenerator  # noqa: F401
 from nise.generators.azure.storage_generator import StorageGenerator  # noqa: F401
 from nise.generators.azure.virtual_machine_generator import VMGenerator  # noqa: F401
 from nise.generators.azure.virtual_network_generator import VNGenerator  # noqa: F401
```

### Comparing `koku-nise-4.4.9/nise/generators/azure/azure_generator.py` & `koku-nise-4.5.0/nise/generators/azure/azure_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,20 +107,16 @@
     "invoiceId",
     "previousInvoiceId",
     "resellerName",
     "resellerMpnId",
     "servicePeriodEndDate",
     "servicePeriodStartDate",
     "ProductId",
-    "product",
     "publisherId",
-    "resourceGroupName",
-    "InstanceName",
     "Location",
-    "billingCurrency",
     "pricingCurrency",
     "costInPricingCurrency",
     "costInUsd",
     "paygCostInBillingCurrency",
     "paygCostInUsd",
     "exchangeRatePricingToBilling",
     "exchangeRateDate",
@@ -186,14 +182,16 @@
         self._meter_name = None
         self._resource_location = None
         self._service_tier = None
         self._consumed = None
         self._resource_type = None
         self._meter_cache = {}
         self._billing_currency = currency
+        self._additional_info = None
+        self._data_direction = None
         # Version 2 fields
         self._invoice_section_id = None
         self._invoice_section_name = None
 
         if attributes:
             for key, value in attributes.items():
                 attr_name = "_" + key
@@ -219,20 +217,20 @@
 
     def _get_cached_meter_values(self, meter_id, service_meter):
         """Return meter cached meter data to ensure meter_id and values are consistent."""
         if not self._meter_cache.get(meter_id):
             self._meter_cache[meter_id] = choice(service_meter)
         return self._meter_cache.get(meter_id)
 
-    def _get_resource_info(self, meter_id, service_meter, ex_resource, add_info, service_info):
+    def _get_resource_info(self, meter_id, service_meter, ex_resource, service_info):
         """Return resource information."""
         service_tier, meter_sub, meter_name, units_of_measure = self._get_cached_meter_values(meter_id, service_meter)
         service_info_2 = choice(service_info)
         resource_group, resource_name = choice(ex_resource)
-        additional_info = choice(add_info)
+        additional_info = self._get_additional_info(meter_name)
         if self._instance_id:
             self._consumed, second_part = accts_str = self._get_accts_str(self._service_name)
             self._resource_type = self._consumed + "/" + second_part
             instance_id = self._instance_id
         else:
             self._consumed, second_part = accts_str = self._get_accts_str(self._service_name)
             self._resource_type = self._consumed + "/" + second_part
@@ -291,14 +289,21 @@
         """Pick resource location."""
         if self._resource_location:
             location = choice([option for option in self.RESOURCE_LOCATION if self._resource_location in option])
         else:
             location = choice(self.RESOURCE_LOCATION)
         return location
 
+    def _get_additional_info(self, meter_name=None):
+        """Pick additional info."""
+        if self._additional_info:
+            return self._additional_info
+        else:
+            return choice(self.ADDITIONAL_INFO)
+
     def _add_common_usage_info(self, row, start, end, **kwargs):
         """Add common usage information."""
         if self.azure_columns == AZURE_COLUMNS_V2:
             usage_account = choice(self.usage_accounts)
             row["SubscriptionId"] = self.subscription_guid
             row["SubscriptionName"] = self.account_info.get("subscription_name")
             row["AccountName"] = usage_account[0]
@@ -337,17 +342,15 @@
             instance_id,
             service_tier,
             meter_sub,
             meter_name,
             units_of_measure,
             additional_info,
             service_info_2,
-        ) = self._get_resource_info(
-            meter_id, self.SERVICE_METER, self.EXAMPLE_RESOURCE, self.ADDITIONAL_INFO, self.SERVICE_INFO_2
-        )
+        ) = self._get_resource_info(meter_id, self.SERVICE_METER, self.EXAMPLE_RESOURCE, self.SERVICE_INFO_2)
         if not additional_info:
             additional_info = ""
         if not service_info_2:
             service_info_2 = ""
 
         row["ResourceGroup"] = resource_group
         row["ResourceLocation"] = azure_region
```

### Comparing `koku-nise-4.4.9/nise/generators/azure/bandwidth_generator.py` & `koku-nise-4.5.0/nise/generators/azure/bandwidth_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/azure/ccsp_generator.py` & `koku-nise-4.5.0/nise/generators/azure/ccsp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/azure/sql_database_generator.py` & `koku-nise-4.5.0/nise/generators/azure/sql_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/azure/storage_generator.py` & `koku-nise-4.5.0/nise/generators/azure/storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/azure/virtual_machine_generator.py` & `koku-nise-4.5.0/nise/generators/azure/virtual_machine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/azure/virtual_network_generator.py` & `koku-nise-4.5.0/nise/generators/azure/virtual_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/gcp/__init__.py` & `koku-nise-4.5.0/nise/generators/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/gcp/cloud_storage_generator.py` & `koku-nise-4.5.0/nise/generators/gcp/cloud_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/gcp/compute_engine_generator.py` & `koku-nise-4.5.0/nise/generators/gcp/compute_engine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/gcp/gcp_database_generator.py` & `koku-nise-4.5.0/nise/generators/gcp/gcp_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/gcp/gcp_generator.py` & `koku-nise-4.5.0/nise/generators/gcp/gcp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/gcp/gcp_network_generator.py` & `koku-nise-4.5.0/nise/generators/gcp/gcp_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/gcp/hcs_generator.py` & `koku-nise-4.5.0/nise/generators/gcp/hcs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/gcp/project_generator.py` & `koku-nise-4.5.0/nise/generators/gcp/project_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/generator.py` & `koku-nise-4.5.0/nise/generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/oci/__init__.py` & `koku-nise-4.5.0/nise/generators/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/oci/oci_block_storage_generator.py` & `koku-nise-4.5.0/nise/generators/oci/oci_block_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/oci/oci_compute_generator.py` & `koku-nise-4.5.0/nise/generators/oci/oci_compute_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/oci/oci_constants.py` & `koku-nise-4.5.0/nise/generators/oci/oci_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/oci/oci_database_generator.py` & `koku-nise-4.5.0/nise/generators/oci/oci_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/oci/oci_generator.py` & `koku-nise-4.5.0/nise/generators/oci/oci_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/oci/oci_network_generator.py` & `koku-nise-4.5.0/nise/generators/oci/oci_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/generators/ocp/__init__.py` & `koku-nise-4.5.0/nise/generators/ocp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
-"""Module for aws data generators."""
+"""Module for ocp data generators."""
 from nise.generators.ocp.ocp_generator import OCP_NAMESPACE_LABEL  # noqa: F401
 from nise.generators.ocp.ocp_generator import OCP_NODE_LABEL  # noqa: F401
 from nise.generators.ocp.ocp_generator import OCP_POD_USAGE  # noqa: F401
 from nise.generators.ocp.ocp_generator import OCP_REPORT_TYPE_TO_COLS  # noqa: F401
 from nise.generators.ocp.ocp_generator import OCP_ROS_USAGE  # noqa: F401
 from nise.generators.ocp.ocp_generator import OCP_STORAGE_USAGE  # noqa: F401
 from nise.generators.ocp.ocp_generator import OCPGenerator  # noqa: F401
```

### Comparing `koku-nise-4.4.9/nise/generators/ocp/ocp_generator.py` & `koku-nise-4.5.0/nise/generators/ocp/ocp_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,17 +59,20 @@
 OCP_STORAGE_COLUMNS = (
     "report_period_start",
     "report_period_end",
     "interval_start",
     "interval_end",
     "namespace",
     "pod",
+    "node",
     "persistentvolumeclaim",
     "persistentvolume",
     "storageclass",
+    "csi_driver",
+    "csi_volume_handle",
     "persistentvolumeclaim_capacity_bytes",
     "persistentvolumeclaim_capacity_byte_seconds",
     "volume_request_storage_byte_seconds",
     "persistentvolumeclaim_usage_byte_seconds",
     "persistentvolume_labels",
     "persistentvolumeclaim_labels",
 )
@@ -521,15 +524,22 @@
 
         return pods, namespace2pod, ros_ocp_data_pods
 
     def _gen_volumes(self, namespaces, namespace2pods):  # noqa: R0914,C901
         """Create volumes on specific namespaces and keep relationship."""
         volumes = []
         for namespace, node in namespaces.items():
-            storage_class_default = choice(("gp2", "fast", "slow", "gold"))
+            storage_class_default, csi_default = choice(
+                (
+                    ("gp3-csi", "ebs.csi.aws.com"),
+                    ("fast", "disk.csi.azure.com"),
+                    ("slow", "disk.csi.azure.com"),
+                    ("gold", "pd.csi.storage.gke.io"),
+                )
+            )
             if node.get("namespaces"):
                 specified_volumes = node.get("namespaces").get(namespace).get("volumes", [])
                 for specified_volume in specified_volumes:
                     volume = specified_volume.get("volume_name", self.fake.word())
                     volume_request_gig = specified_volume.get("volume_request_gig")
                     volume_request = volume_request_gig * GIGABYTE
                     specified_vol_claims = specified_volume.get("volume_claims", [])
@@ -556,17 +566,22 @@
                             "pod": pod,
                             "volume_claim_usage_gig": usage_gig,
                         }
                         total_claims += claim_capacity
                     volumes.append(
                         {
                             volume: {
+                                "node": node.get("name"),
                                 "namespace": namespace,
                                 "volume": volume,
                                 "storage_class": specified_volume.get("storage_class", storage_class_default),
+                                "csi_driver": specified_volume.get("csi_driver", csi_default),
+                                "csi_volume_handle": specified_volume.get(
+                                    "csi_volume_handle", f"vol-{self.fake.word()}"
+                                ),
                                 "volume_request": volume_request,
                                 "labels": specified_volume.get("labels", None),
                                 "volume_claims": volume_claims,
                             }
                         }
                     )
             else:
@@ -576,33 +591,44 @@
                     vol_suffix = "".join(choices(ascii_lowercase, k=10))
                     volume = "pvc" + "-" + vol_suffix
                     vol_request_gig = round(uniform(25.0, 80.0), 2)
                     vol_request = vol_request_gig * GIGABYTE
                     volume_claims = {}
                     total_claims = 0
                     for _ in range(num_vol_claims):
-                        if vol_request_gig - total_claims <= GIGABYTE:
+                        if vol_request - total_claims <= GIGABYTE:
                             break
                         vol_claim = self.fake.word()
                         pod = choice(namespace2pods[namespace])
-                        claim_capacity = round(uniform(1.0, vol_request_gig), 2) * GIGABYTE
+                        claim_capacity = round(uniform(1.0, (vol_request_gig - total_claims / GIGABYTE)), 2) * GIGABYTE
                         volume_claims[vol_claim] = {
                             "namespace": namespace,
                             "volume": volume,
                             "labels": self._gen_openshift_labels(),
                             "capacity": claim_capacity,
                             "pod": pod,
                         }
                         total_claims += claim_capacity
+                    storage_class_default, csi_default = choice(
+                        (
+                            ("gp3-csi", "ebs.csi.aws.com"),
+                            ("fast", "disk.csi.azure.com"),
+                            ("slow", "disk.csi.azure.com"),
+                            ("gold", "pd.csi.storage.gke.io"),
+                        )
+                    )
                     volumes.append(
                         {
                             volume: {
                                 "namespace": namespace,
+                                "node": node.get("name"),
                                 "volume": volume,
-                                "storage_class": choice(("gp2", "fast", "slow", "gold")),
+                                "storage_class": storage_class_default,
+                                "csi_driver": csi_default,
+                                "csi_volume_handle": f"vol-{self.fake.word()}",
                                 "volume_request": vol_request,
                                 "labels": self._gen_openshift_labels(),
                                 "volume_claims": volume_claims,
                             }
                         }
                     )
         return volumes
@@ -682,34 +708,40 @@
         row.update(pod)
         return row
 
     def _update_storage_data(self, row, start, end, **kwargs):
         """Update data with generator specific data."""
         volume_claim_usage_gig = self._get_usage_for_date(kwargs.get("volume_claim_usage_gig"), start)
 
-        volume_request = kwargs.get("volume_request")
+        volume_request = kwargs.get("volume_request", 0)
+        # volume_request_storage_byte_seconds is empty for claimless PersistentVolumes
+        volume_request_storage_byte_seconds = volume_request * HOUR if volume_request > 0 else None
         vc_capacity_gig = max(kwargs.get("vc_capacity", 10.0), volume_request) / GIGABYTE
 
         vc_usage_gig = round(uniform(2.0, vc_capacity_gig), 2)
         if volume_claim_usage_gig:
             vc_usage_gig = min(volume_claim_usage_gig, vc_capacity_gig)
-        vc_usage = vc_usage_gig * GIGABYTE
+        # persistentvolumeclaim_usage_byte_seconds is empty for claimless PersistentVolumes
+        vc_usage = vc_usage_gig * GIGABYTE * HOUR if volume_request_storage_byte_seconds else None
 
         data = {
             "namespace": kwargs.get("namespace"),
             "pod": kwargs.get("pod"),
+            "node": kwargs.get("node"),
             "persistentvolumeclaim": kwargs.get("volume_claim"),
             "persistentvolume": kwargs.get("volume_name"),
             "storageclass": kwargs.get("storage_class"),
-            "persistentvolumeclaim_capacity_bytes": kwargs.get("vc_capacity"),
+            "csi_driver": kwargs.get("csi_driver"),
+            "csi_volume_handle": kwargs.get("csi_volume_handle"),
+            "persistentvolumeclaim_capacity_bytes": vc_capacity_gig * GIGABYTE,
             "persistentvolumeclaim_capacity_byte_seconds": vc_capacity_gig * GIGABYTE * HOUR,
-            "volume_request_storage_byte_seconds": volume_request * HOUR,
+            "volume_request_storage_byte_seconds": volume_request_storage_byte_seconds,
+            "persistentvolumeclaim_usage_byte_seconds": vc_usage,
             "persistentvolume_labels": kwargs.get("volume_labels"),
             "persistentvolumeclaim_labels": kwargs.get("volume_claim_labels"),
-            "persistentvolumeclaim_usage_byte_seconds": vc_usage * HOUR,
         }
         row.update(data)
         return row
 
     def _update_node_label_data(self, row, start, end, **kwargs):
         """Update data with generator specific data."""
         data = {"node": kwargs.get("node"), "node_labels": kwargs.get("node_labels")}
@@ -796,42 +828,61 @@
     def _gen_hourly_storage_usage(self, **kwargs):
         """Create hourly data for storage usage."""
         for hour in self.hours:
             start = hour.get("start")
             end = hour.get("end")
             for volume_dict in self.volumes:
                 for volume_name, volume in volume_dict.items():
+                    node = volume.get("node")
                     namespace = volume.get("namespace", None)
                     storage_class = volume.get("storage_class", None)
+                    csi_driver = volume.get("csi_driver", None)
+                    csi_volume_handle = volume.get("csi_volume_handle", None)
                     volume_request = volume.get("volume_request", None)
                     vol_labels = volume.get("labels", None)
                     volume_claims = volume.get("volume_claims", [])
                     for vc_name, volume_claim in volume_claims.items():
                         pod = volume_claim.get("pod")
                         vc_labels = volume_claim.get("labels")
                         capacity = volume_claim.get("capacity")
                         volume_claim_usage_gig = volume_claim.get("volume_claim_usage_gig", None)
                         row = self._init_data_row(start, end, **kwargs)
-                        row = self._update_data(
+                        yield self._update_data(
                             row,
                             start,
                             end,
                             volume_claim=vc_name,
                             pod=pod,
+                            node=node,
                             volume_claim_labels=vc_labels,
                             vc_capacity=capacity,
                             volume_claim_usage_gig=volume_claim_usage_gig,
                             storage_class=storage_class,
+                            csi_driver=csi_driver,
+                            csi_volume_handle=csi_volume_handle,
                             volume_name=volume_name,
                             volume_request=volume_request,
                             volume_labels=vol_labels,
                             namespace=namespace,
                             **kwargs,
                         )
-                        yield row
+                    if not volume_claims:
+                        row = self._init_data_row(start, end, **kwargs)
+                        yield self._update_data(
+                            row,
+                            start,
+                            end,
+                            storage_class=storage_class,
+                            csi_driver=csi_driver,
+                            csi_volume_handle=csi_volume_handle,
+                            volume_name=volume_name,
+                            vc_capacity=volume_request,
+                            volume_labels=vol_labels,
+                            **kwargs,
+                        )
 
     def _gen_hourly_node_label_usage(self, **kwargs):
         """Create hourly data for nodel label report."""
         for hour in self.hours:
             start = hour.get("start")
             end = hour.get("end")
             for node in self.nodes:
```

### Comparing `koku-nise-4.4.9/nise/manifest.py` & `koku-nise-4.5.0/nise/manifest.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/report.py` & `koku-nise-4.5.0/nise/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 from nise.generators.aws import MarketplaceGenerator
 from nise.generators.aws import RDSGenerator
 from nise.generators.aws import Route53Generator
 from nise.generators.aws import S3Generator
 from nise.generators.aws import VPCGenerator
 from nise.generators.azure import BandwidthGenerator
 from nise.generators.azure import CCSPGenerator
+from nise.generators.azure import DTGenerator
 from nise.generators.azure import SQLGenerator
 from nise.generators.azure import StorageGenerator
 from nise.generators.azure import VMGenerator
 from nise.generators.azure import VNGenerator
 from nise.generators.gcp import CloudStorageGenerator
 from nise.generators.gcp import ComputeEngineGenerator
 from nise.generators.gcp import GCP_REPORT_COLUMNS
@@ -497,41 +498,47 @@
 
 
 def _create_generator_dates_from_yaml(attributes, month):
     """Calculate generator start and end dates based on yaml and current month."""
     gen_start_date = None
     gen_end_date = None
 
+    start_date = attributes.get("start_date")
+    end_date = attributes.get("end_date")
+    month_start = month.get("start")
+    month_end = month.get("end")
+
+    # Use a different variable for the end of month comparison. This matters
+    # when the end_date is the same as the month_end, which can happen based
+    # on the specified --end-date parameter or on the first of the month.
+    month_end_compare = month_end
+    if month_end.day != 1:
+        # Create a new datetime object and store it, leaving the original
+        # month_end object unmodified.
+        month_end_compare = month_end_compare.replace(hour=23, minute=59, second=59)
+
     # Generator range is larger then current month on both start and end
-    if attributes.get("start_date") < month.get("start") and attributes.get("end_date") > month.get("end").replace(
-        hour=23, minute=59, second=59
-    ):
-        gen_start_date = month.get("start")
-        gen_end_date = month.get("end")
+    if start_date < month_start and end_date > month_end_compare:
+        gen_start_date = month_start
+        gen_end_date = month_end
 
     # Generator starts before month start and ends within month
-    if attributes.get("start_date") <= month.get("start") and attributes.get("end_date") <= month.get("end").replace(
-        hour=23, minute=59, second=59
-    ):
-        gen_start_date = month.get("start")
-        gen_end_date = attributes.get("end_date")
+    elif start_date < month_start and end_date <= month_end_compare:
+        gen_start_date = month_start
+        gen_end_date = end_date
 
     # Generator is within month
-    if attributes.get("start_date") >= month.get("start") and attributes.get("end_date") <= month.get("end").replace(
-        hour=23, minute=59, second=59
-    ):
-        gen_start_date = attributes.get("start_date")
-        gen_end_date = attributes.get("end_date")
+    elif start_date >= month_start and end_date <= month_end_compare:
+        gen_start_date = start_date
+        gen_end_date = end_date
 
     # Generator starts within month and ends in next month
-    if attributes.get("start_date") >= month.get("start") and attributes.get("end_date") > month.get("end").replace(
-        hour=23, minute=59, second=59
-    ):
-        gen_start_date = attributes.get("start_date")
-        gen_end_date = month.get("end")
+    elif start_date >= month_start and end_date > month_end_compare:
+        gen_start_date = start_date
+        gen_end_date = month_end
 
     return gen_start_date, gen_end_date
 
 
 def write_aws_file(
     file_number, aws_report_name, month_name, year, data, aws_finalize_report, static_report_data, headers
 ):
@@ -589,15 +596,14 @@
         options["accounts_list"] = None
 
         aws_create_report(options)
 
 
 def aws_create_report(options):  # noqa: C901
     """Create a cost usage report file."""
-    data = []
     start_date = options.get("start_date")
     end_date = options.get("end_date")
     aws_finalize_report = options.get("aws_finalize_report")
     static_report_data = options.get("static_report_data")
     manifest_gen = True if options.get("manifest_generation") is None else options.get("manifest_generation")
 
     if static_report_data:
@@ -740,14 +746,15 @@
         generators = [
             {"generator": BandwidthGenerator, "attributes": {}},
             {"generator": CCSPGenerator, "attributes": {}},
             {"generator": SQLGenerator, "attributes": {}},
             {"generator": StorageGenerator, "attributes": {}},
             {"generator": VMGenerator, "attributes": {}},
             {"generator": VNGenerator, "attributes": {}},
+            {"generator": DTGenerator, "attributes": {}},
         ]
         accounts_list = None
 
     months = _create_month_list(start_date, end_date)
 
     account_info = _generate_azure_account_info(accounts_list)
     currency = default_currency(options.get("currency"), account_info["currency_code"])
@@ -1290,15 +1297,15 @@
 
 
 def oci_create_report(options):
     """Create cost and usage report files."""
 
     generate_daily_report = options.get("oci_daily_report", False)
     start_date = options.get("start_date")
-    end_date = start_date if generate_daily_report else options.get("end_date")
+    end_date = start_date.replace(hour=23) if generate_daily_report else options.get("end_date")
     static_report_data = options.get("static_report_data")
 
     if static_report_data:
         generators = _get_generators(static_report_data.get("generators"))
     else:
         generators = [
             {"generator": OCIComputeGenerator},
```

### Comparing `koku-nise-4.4.9/nise/upload.py` & `koku-nise-4.5.0/nise/upload.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/util/__init__.py` & `koku-nise-4.5.0/nise/util/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/util/log.py` & `koku-nise-4.5.0/nise/util/log.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_gen.py` & `koku-nise-4.5.0/nise/yaml_gen.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/aws/ec2_instance_types.py` & `koku-nise-4.5.0/nise/yaml_generators/aws/ec2_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/aws/generator.py` & `koku-nise-4.5.0/nise/yaml_generators/aws/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/aws/rds_instance_types.py` & `koku-nise-4.5.0/nise/yaml_generators/aws/rds_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/aws/regions.py` & `koku-nise-4.5.0/nise/yaml_generators/aws/regions.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/azure/generator.py` & `koku-nise-4.5.0/nise/yaml_generators/azure/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/gcp/generator.py` & `koku-nise-4.5.0/nise/yaml_generators/gcp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/generator.py` & `koku-nise-4.5.0/nise/yaml_generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/oci/generator.py` & `koku-nise-4.5.0/nise/yaml_generators/oci/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/oci/oci_yaml_constants.py` & `koku-nise-4.5.0/nise/yaml_generators/oci/oci_yaml_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/ocp/generator.py` & `koku-nise-4.5.0/nise/yaml_generators/ocp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/ocp_on_cloud/generator.py` & `koku-nise-4.5.0/nise/yaml_generators/ocp_on_cloud/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/static/aws_generator_config.yml` & `koku-nise-4.5.0/nise/yaml_generators/static/aws_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/static/aws_static_data.yml.j2` & `koku-nise-4.5.0/nise/yaml_generators/static/aws_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/static/azure_generator_config.yml` & `koku-nise-4.5.0/nise/yaml_generators/static/azure_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/static/azure_static_data.yml.j2` & `koku-nise-4.5.0/nise/yaml_generators/static/azure_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/static/gcp_static_data.yml.j2` & `koku-nise-4.5.0/nise/yaml_generators/static/gcp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/static/oci_static_data.yml.j2` & `koku-nise-4.5.0/nise/yaml_generators/static/oci_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/static/ocp_generator_config.yml` & `koku-nise-4.5.0/nise/yaml_generators/static/ocp_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/static/ocp_on_cloud_options.yml` & `koku-nise-4.5.0/nise/yaml_generators/static/ocp_on_cloud_options.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/static/ocp_static_data.yml.j2` & `koku-nise-4.5.0/nise/yaml_generators/static/ocp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/nise/yaml_generators/utils.py` & `koku-nise-4.5.0/nise/yaml_generators/utils.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.9/setup.py` & `koku-nise-4.5.0/setup.py`

 * *Files identical despite different names*

