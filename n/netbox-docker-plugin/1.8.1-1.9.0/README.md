# Comparing `tmp/netbox_docker_plugin-1.8.1.tar.gz` & `tmp/netbox_docker_plugin-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_docker_plugin-1.8.1.tar", last modified: Wed May  8 15:43:42 2024, max compression
+gzip compressed data, was "netbox_docker_plugin-1.9.0.tar", last modified: Wed May 15 13:27:04 2024, max compression
```

## Comparing `netbox_docker_plugin-1.8.1.tar` & `netbox_docker_plugin-1.9.0.tar`

### file list

```diff
@@ -1,136 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.949496 netbox_docker_plugin-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-08 15:43:42.945496 netbox_docker_plugin-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.933496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.933496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15446 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.933496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/network_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.937496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0002_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0003_image_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0004_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0005_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0011_host_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0012_host_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0013_host_netbox_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0014_container_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0016_alter_env_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0017_network_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0020_container_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0021_registry_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0023_delete_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0025_alter_image_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0026_image_digest.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0027_container_restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0029_alter_container_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.941496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.929496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.941496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/container.html
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/host.html
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/image.html
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/network.html
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.941496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/templatetags/host.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.941496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.941496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/container/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/container/test_container_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/container/test_container_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/container/test_container_operation_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/container/test_container_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/container/test_container_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.941496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/host/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/host/test_host_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/host/test_host_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/host/test_replace_password.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.945496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/image/test_image_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/image/test_image_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.945496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/network/test_network_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/network/test_network_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.945496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/registry/test_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/registry/test_registry_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.945496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/volume/test_volume_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/volume/test_volume_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.945496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.945496 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/label.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/network_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:42.945496 netbox_docker_plugin-1.8.1/netbox_docker_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-08 15:43:42.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-08 15:43:42.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:43:42.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 15:43:42.000000 netbox_docker_plugin-1.8.1/netbox_docker_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-08 15:43:39.000000 netbox_docker_plugin-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:43:42.949496 netbox_docker_plugin-1.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.132426 netbox_docker_plugin-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-15 13:27:04.132426 netbox_docker_plugin-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.112426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.116426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15446 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.116426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/network_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.124426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0002_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0003_image_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0004_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0005_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0011_host_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0012_host_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0014_container_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0016_alter_env_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0017_network_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0020_container_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0021_registry_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0023_delete_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0025_alter_image_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0026_image_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0027_container_restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0029_alter_container_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.124426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.112426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.124426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/container-layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/container-logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.124426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templatetags/host.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.124426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_operation_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/test_host_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/test_host_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/test_replace_password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/image/test_image_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/image/test_image_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/network/test_network_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/network/test_network_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/registry/test_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/registry/test_registry_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/volume/test_volume_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/volume/test_volume_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.132426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/network_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.132426 netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-15 13:27:04.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-15 13:27:04.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:27:04.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 13:27:04.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:27:04.132426 netbox_docker_plugin-1.9.0/setup.cfg
```

### Comparing `netbox_docker_plugin-1.8.1/LICENSE` & `netbox_docker_plugin-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/PKG-INFO` & `netbox_docker_plugin-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-docker-plugin
-Version: 1.8.1
+Version: 1.9.0
 Summary: Manage Docker with Netbox & style.
 Author-email: Vincent Simonin <vincent@saashup.com>, David Delassus <david.jose.delassus@gmail.com>
 Project-URL: Homepage, https://github.com/SaaShup/netbox-docker-plugin
 Project-URL: Bug Tracker, https://github.com/SaaShup/netbox-docker-plugin/issues
 Keywords: netbox,netbox-plugin,docker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -162,29 +162,31 @@
 python3 netbox/manage.py runserver 0.0.0.0:8000 --insecure
 ```
 
 Visit http://localhost:8000/
 
 ### Run tests
 
-After installing you development environment, you can run the tests plugin (you don't need to start the Netbox instance):
+After installing your development environment, you can run the tests plugin
+(you don't need to start the Netbox instance):
 
 ```bash
 cd $PROJECT/netbox
+python3 -m pip install requests_mock
 python3 netbox/manage.py test netbox_docker_plugin.tests --keepdb -v 2
 ```
 
 With code coverage, install [coverage.py](https://coverage.readthedocs.io/en/7.3.2/) and use it:
 
 ```bash
 cd $PROJECT/netbox
 python3 -m pip install coverage
 ```
 
-The run the test with coverage.py and print the report:
+Then run the test with coverage.py and print the report:
 
 ```bash
 cd $PROJECT/netbox
 coverage run --include='*/netbox_docker_plugin/*' netbox/manage.py test netbox_docker_plugin.tests --keepdb -v 2
 coverage report -m
 ```
```

### Comparing `netbox_docker_plugin-1.8.1/README.md` & `netbox_docker_plugin-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -149,29 +149,31 @@
 python3 netbox/manage.py runserver 0.0.0.0:8000 --insecure
 ```
 
 Visit http://localhost:8000/
 
 ### Run tests
 
-After installing you development environment, you can run the tests plugin (you don't need to start the Netbox instance):
+After installing your development environment, you can run the tests plugin
+(you don't need to start the Netbox instance):
 
 ```bash
 cd $PROJECT/netbox
+python3 -m pip install requests_mock
 python3 netbox/manage.py test netbox_docker_plugin.tests --keepdb -v 2
 ```
 
 With code coverage, install [coverage.py](https://coverage.readthedocs.io/en/7.3.2/) and use it:
 
 ```bash
 cd $PROJECT/netbox
 python3 -m pip install coverage
 ```
 
-The run the test with coverage.py and print the report:
+Then run the test with coverage.py and print the report:
 
 ```bash
 cd $PROJECT/netbox
 coverage run --include='*/netbox_docker_plugin/*' netbox/manage.py test netbox_docker_plugin.tests --keepdb -v 2
 coverage report -m
 ```
```

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/__init__.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class NetBoxDockerConfig(PluginConfig):
     """Plugin Config Class"""
 
     name = "netbox_docker_plugin"
     verbose_name = " NetBox Docker Plugin"
     description = "Manage Docker"
-    version = "1.8.1"
+    version = "1.9.0"
     base_url = "docker"
     author= "Vincent Simonin <vincent@saashup.com>, David Delassus <david.jose.delassus@gmail.com>"
     author_email= "vincent@saashup.com, david.jose.delassus@gmail.com"
 
     def ready(self):
         from . import signals # pylint: disable=unused-import, import-outside-toplevel
```

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/api/serializers.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/filtersets.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/bind.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/container.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/container.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/env.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/env.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/host.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/host.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/image.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/label.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/label.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/mount.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/mount.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/network.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/network_setting.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/network_setting.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/port.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/port.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/registry.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/forms/volume.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0001_initial.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0002_image.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0002_image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0003_image_size.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0003_image_size.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0004_volume.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0004_volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0005_network.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0005_network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0011_host_token.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0011_host_token.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0012_host_state.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0012_host_state.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0013_host_netbox_url.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0016_alter_env_value.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0016_alter_env_value.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0020_container_hostname.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0020_container_hostname.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0021_registry_and_more.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0021_registry_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0023_delete_hosts.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0023_delete_hosts.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0025_alter_image_version.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0025_alter_image_version.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0026_image_digest.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0026_image_digest.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/migrations/__init__.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/container.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/container.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/host.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/host.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/image.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/network.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/registry.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/models/volume.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/navigation.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/signals.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/signals.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tables.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/container.html` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,11 @@
-{% extends 'generic/object.html' %}
+{% extends "netbox_docker_plugin/container-layout.html" %}
 
 {% load plugins %}
 
-{% block extra_controls %}
-<form action="{% url 'plugins:netbox_docker_plugin:container_operation' pk=object.id operation='start' %}" method="post">
-  {% csrf_token %}
-  <input type="hidden" name="operation" value="start">
-  <button
-    type="submit"
-    class="btn btn-sm btn-success"
-    {% if not object.can_start %}
-    disabled
-    {% endif %}
-  >
-    <i class="mdi mdi-play"></i> Start
-  </button>
-</form>
-
-<form action="{% url 'plugins:netbox_docker_plugin:container_operation' pk=object.id operation='stop' %}" method="post">
-  {% csrf_token %}
-  <input type="hidden" name="operation" value="stop">
-  <button
-    type="submit"
-    class="btn btn-sm btn-danger"
-    {% if not object.can_stop %}
-    disabled
-    {% endif %}
-  >
-    <i class="mdi mdi-stop"></i> Stop
-  </button>
-</form>
-
-<form action="{% url 'plugins:netbox_docker_plugin:container_operation' pk=object.id operation='restart' %}" method="post">
-  {% csrf_token %}
-  <input type="hidden" name="operation" value="restart">
-  <button
-    type="submit"
-    class="btn btn-sm btn-light"
-    {% if not object.can_restart %}
-    disabled
-    {% endif %}
-  >
-    <i class="mdi mdi-restart"></i> Restart
-  </button>
-</form>
-
-<form action="{% url 'plugins:netbox_docker_plugin:container_operation' pk=object.id operation='recreate' %}" method="post">
-  {% csrf_token %}
-  <input type="hidden" name="operation" value="recreate">
-  <button
-    type="submit"
-    class="btn btn-sm btn-dark"
-    {% if not object.can_recreate %}
-    disabled
-    {% endif %}
-  >
-    <i class="mdi mdi-autorenew"></i> Recreate
-  </button>
-</form>
-{% endblock %}
-
 {% block content %}
 <div class="row mb-3">
   <div class="col col-md-6">
     <div class="card">
       <h5 class="card-header">CONTAINER</h5>
       <div class="card-body">
         <table class="table table-hover attr-table">
```

#### html2text {}

```diff
@@ -1,18 +1,9 @@
-{% extends 'generic/object.html' %} {% load plugins %} {% block extra_controls
-%}
-{% csrf_token %}
-% if not object.can_start %} disabled {% endif %} > Start
-{% csrf_token %}
-% if not object.can_stop %} disabled {% endif %} > Stop
-{% csrf_token %}
-% if not object.can_restart %} disabled {% endif %} > Restart
-{% csrf_token %}
-% if not object.can_recreate %} disabled {% endif %} > Recreate
-{% endblock %} {% block content %}
+{% extends "netbox_docker_plugin/container-layout.html" %} {% load plugins %}
+{% block content %}
 **** CCOONNTTAAIINNEERR ****
 HHoosstt           _{_{_ _o_b_j_e_c_t_._h_o_s_t_ _}_}
 IImmaaggee          _{_{_ _o_b_j_e_c_t_._i_m_a_g_e_ _}_}
 NNaammee           {{ object.name }}
 CCoonnttaaiinneerrIIDD    {{ object.ContainerID|placeholder }}
 HHoossttnnaammee       {{ object.hostname|placeholder }}
 SSttaattee          {{ object.get_state_display }}
```

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/host.html` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/image.html` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/network.html` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/base.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/container/test_container_actions.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_actions.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/container/test_container_api.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from netbox_docker_plugin.models.host import Host
 from netbox_docker_plugin.models.network import Network
 from netbox_docker_plugin.models.image import Image
 from netbox_docker_plugin.models.volume import Volume
 from netbox_docker_plugin.models.registry import Registry
 from netbox_docker_plugin.tests.base import BaseAPITestCase
 
+import requests_mock
+
 
 class ContainerApiTestCase(
     BaseAPITestCase,
     APIViewTestCases.GetObjectViewTestCase,
     APIViewTestCases.ListObjectsViewTestCase,
     APIViewTestCases.CreateObjectViewTestCase,
     APIViewTestCases.UpdateObjectViewTestCase,
@@ -71,14 +73,15 @@
 
         Container.objects.create(
             host=host1,
             image=image1,
             name="container1",
             operation="none",
             state="created",
+            ContainerID="1234",
         )
         Container.objects.create(
             host=host1,
             image=image1,
             name="container2",
             operation="none",
             state="created",
@@ -233,7 +236,41 @@
             **self.header,
         )
 
         self.assertHttpStatus(response, status.HTTP_200_OK)
 
         self.assertEqual(Bind.objects.filter(container=container11).count(), 0)
         self.assertEqual(Env.objects.filter(container=container11).count(), 1)
+
+
+    def test_logs_endpoint(self):
+        """ Test logs endpoint """
+
+        container = Container.objects.get(name="container1")
+        container_id = container.ContainerID
+
+        endpoint = reverse(
+            viewname=f"plugins-api:{self._get_view_namespace()}:container-logs",
+            kwargs={"pk": container.pk},
+        )
+
+        # Add object-level permission
+        obj_perm = ObjectPermission(
+            name='Test permission',
+            constraints={"pk": container.pk},
+            actions=["view"],
+        )
+        obj_perm.save()
+        # pylint: disable=E1101
+        obj_perm.users.add(self.user)
+        # pylint: disable=E1101
+        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+
+        with requests_mock.Mocker() as m:
+            m.get(
+                f"http://localhost:8080/api/engine/containers/{container_id}/logs",
+                text="Hello World",
+            )
+
+            response = self.client.get(endpoint, **self.header)
+            self.assertHttpStatus(response, status.HTTP_200_OK)
+            self.assertEqual(response.data, "Hello World")
```

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/container/test_container_operation_view.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_operation_view.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/container/test_container_validation.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_validation.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/container/test_container_views.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/host/test_host_api.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/test_host_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/host/test_host_views.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/test_host_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/host/test_replace_password.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/test_replace_password.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/image/test_image_api.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/image/test_image_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/image/test_image_views.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/image/test_image_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/network/test_network_api.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/network/test_network_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/network/test_network_views.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/network/test_network_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/registry/test_registry_api.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/registry/test_registry_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/registry/test_registry_views.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/registry/test_registry_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/test_init.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/volume/test_volume_api.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/volume/test_volume_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/tests/volume/test_volume_views.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/volume/test_volume_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/urls.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,19 @@
     ),
     path(
         "containers/<int:pk>/",
         container_views.ContainerView.as_view(),
         name="container",
     ),
     path(
+        "containers/<int:pk>/logs",
+        container_views.ContainerLogsView.as_view(),
+        name="container_logs",
+    ),
+    path(
         "containers/<int:pk>/edit/",
         container_views.ContainerEditView.as_view(),
         name="container_edit",
     ),
     path(
         "containers/<int:pk>/delete/",
         container_views.ContainerDeleteView.as_view(),
```

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/utilities/__init__.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/bind.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/container.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Container views definitions"""
 
 from utilities.utils import count_related
+from utilities.views import ViewTab, register_model_view
 from netbox.views import generic
 from .. import tables, filtersets
 from ..forms import container
 from ..models.container import (
     Container,
     Mount,
     Bind,
     Port,
     NetworkSetting,
     Env,
     Label,
 )
 
 
+@register_model_view(Container)
 class ContainerView(generic.ObjectView):
     """Container view definition"""
 
     queryset = Container.objects.prefetch_related(
         "host",
         "image",
         "env",
@@ -26,14 +28,23 @@
         "mounts",
         "binds",
         "ports",
         "network_settings",
     )
 
 
+@register_model_view(Container, name="logs", path="logs")
+class ContainerLogsView(generic.ObjectView):
+    """ Logs tab in Container view """
+
+    queryset = Container.objects.all()
+    tab = ViewTab(label="Logs")
+    template_name = "netbox_docker_plugin/container-logs.html"
+
+
 class ContainerEditView(generic.ObjectEditView):
     """Container edition view definition"""
 
     queryset = Container.objects.all()
     form = container.ContainerForm
```

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/env.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/env.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/host.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/host.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/image.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/label.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/label.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/mount.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/mount.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/network.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/network_setting.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/network_setting.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/port.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/port.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/registry.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin/views/volume.py` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin.egg-info/PKG-INFO` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-docker-plugin
-Version: 1.8.1
+Version: 1.9.0
 Summary: Manage Docker with Netbox & style.
 Author-email: Vincent Simonin <vincent@saashup.com>, David Delassus <david.jose.delassus@gmail.com>
 Project-URL: Homepage, https://github.com/SaaShup/netbox-docker-plugin
 Project-URL: Bug Tracker, https://github.com/SaaShup/netbox-docker-plugin/issues
 Keywords: netbox,netbox-plugin,docker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -162,29 +162,31 @@
 python3 netbox/manage.py runserver 0.0.0.0:8000 --insecure
 ```
 
 Visit http://localhost:8000/
 
 ### Run tests
 
-After installing you development environment, you can run the tests plugin (you don't need to start the Netbox instance):
+After installing your development environment, you can run the tests plugin
+(you don't need to start the Netbox instance):
 
 ```bash
 cd $PROJECT/netbox
+python3 -m pip install requests_mock
 python3 netbox/manage.py test netbox_docker_plugin.tests --keepdb -v 2
 ```
 
 With code coverage, install [coverage.py](https://coverage.readthedocs.io/en/7.3.2/) and use it:
 
 ```bash
 cd $PROJECT/netbox
 python3 -m pip install coverage
 ```
 
-The run the test with coverage.py and print the report:
+Then run the test with coverage.py and print the report:
 
 ```bash
 cd $PROJECT/netbox
 coverage run --include='*/netbox_docker_plugin/*' netbox/manage.py test netbox_docker_plugin.tests --keepdb -v 2
 coverage report -m
 ```
```

### Comparing `netbox_docker_plugin-1.8.1/netbox_docker_plugin.egg-info/SOURCES.txt` & `netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 netbox_docker_plugin/tables.py
 netbox_docker_plugin/urls.py
 netbox_docker_plugin.egg-info/PKG-INFO
 netbox_docker_plugin.egg-info/SOURCES.txt
 netbox_docker_plugin.egg-info/dependency_links.txt
 netbox_docker_plugin.egg-info/top_level.txt
 netbox_docker_plugin/api/__init__.py
+netbox_docker_plugin/api/renderers.py
 netbox_docker_plugin/api/serializers.py
 netbox_docker_plugin/api/urls.py
 netbox_docker_plugin/api/views.py
 netbox_docker_plugin/forms/__init__.py
 netbox_docker_plugin/forms/bind.py
 netbox_docker_plugin/forms/container.py
 netbox_docker_plugin/forms/env.py
@@ -62,14 +63,16 @@
 netbox_docker_plugin/models/__init__.py
 netbox_docker_plugin/models/container.py
 netbox_docker_plugin/models/host.py
 netbox_docker_plugin/models/image.py
 netbox_docker_plugin/models/network.py
 netbox_docker_plugin/models/registry.py
 netbox_docker_plugin/models/volume.py
+netbox_docker_plugin/templates/netbox_docker_plugin/container-layout.html
+netbox_docker_plugin/templates/netbox_docker_plugin/container-logs.html
 netbox_docker_plugin/templates/netbox_docker_plugin/container.html
 netbox_docker_plugin/templates/netbox_docker_plugin/host.html
 netbox_docker_plugin/templates/netbox_docker_plugin/image.html
 netbox_docker_plugin/templates/netbox_docker_plugin/network.html
 netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
 netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
 netbox_docker_plugin/templatetags/__init__.py
```

### Comparing `netbox_docker_plugin-1.8.1/pyproject.toml` & `netbox_docker_plugin-1.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-docker-plugin"
-version = "1.8.1"
+version = "1.9.0"
 authors = [
   { name="Vincent Simonin", email="vincent@saashup.com" },
   { name="David Delassus", email="david.jose.delassus@gmail.com" }
 ]
 description = "Manage Docker with Netbox & style."
 readme = "README.md"
 requires-python = ">=3.8"
```

