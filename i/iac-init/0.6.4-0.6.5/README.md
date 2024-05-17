# Comparing `tmp/iac_init-0.6.4.tar.gz` & `tmp/iac_init-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.6.4.tar", max compression
+gzip compressed data, was "iac_init-0.6.5.tar", max compression
```

## Comparing `iac_init-0.6.4.tar` & `iac_init-0.6.5.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0    16295 2024-05-17 09:41:21.915139 iac_init-0.6.4/LICENSE
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.915139 iac_init-0.6.4/README.md
--rw-r--r--   0        0        0      389 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/__main__.py
--rw-r--r--   0        0        0    11616 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/cli/main.py
--rw-r--r--   0        0        0      206 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/cli/options.py
--rw-r--r--   0        0        0     2064 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     2886 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0     1397 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2595 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     7490 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      453 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0      263 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      334 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/scripts/thread_tool.py
--rw-r--r--   0        0        0     3778 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-17 09:41:21.915139 iac_init-0.6.4/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.919139 iac_init-0.6.4/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/templates/12-config_backup/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4922 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/utils/functional.py
--rw-r--r--   0        0        0    11816 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/validator.py
--rw-r--r--   0        0        0     5093 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5222 2024-05-17 09:41:21.923138 iac_init-0.6.4/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1636 2024-05-17 09:41:21.923138 iac_init-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-17 09:43:59.002954 iac_init-0.6.5/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.002954 iac_init-0.6.5/README.md
+-rw-r--r--   0        0        0      389 2024-05-17 09:43:59.002954 iac_init-0.6.5/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-17 09:43:59.002954 iac_init-0.6.5/iac_init/__main__.py
+-rwxr-xr-x   0        0        0   723912 2024-05-17 09:44:14.931306 iac_init-0.6.5/iac_init/cli/main.so
+-rwxr-xr-x   0        0        0    69808 2024-05-17 09:44:15.155310 iac_init-0.6.5/iac_init/cli/options.so
+-rw-r--r--   0        0        0     2064 2024-05-17 09:43:59.002954 iac_init-0.6.5/iac_init/conf/__init__.py
+-rwxr-xr-x   0        0        0   176224 2024-05-17 09:44:15.731323 iac_init-0.6.5/iac_init/conf/global_settings.so
+-rwxr-xr-x   0        0        0   246152 2024-05-17 09:44:19.511408 iac_init-0.6.5/iac_init/scripts/ansible_tool.so
+-rwxr-xr-x   0        0        0   293576 2024-05-17 09:44:20.935440 iac_init-0.6.5/iac_init/scripts/apic_connecton_tool.so
+-rwxr-xr-x   0        0        0   675960 2024-05-17 09:44:18.231379 iac_init-0.6.5/iac_init/scripts/cimc_precheck_tool.so
+-rwxr-xr-x   0        0        0   169016 2024-05-17 09:44:21.479452 iac_init-0.6.5/iac_init/scripts/ssh_tool.so
+-rwxr-xr-x   0        0        0   137000 2024-05-17 09:44:19.935418 iac_init-0.6.5/iac_init/scripts/telnet_tool.so
+-rwxr-xr-x   0        0        0   156336 2024-05-17 09:44:18.711390 iac_init-0.6.5/iac_init/scripts/thread_tool.so
+-rw-r--r--   0        0        0     3778 2024-05-17 09:43:59.002954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-17 09:43:59.002954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-17 09:43:59.002954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-05-17 09:43:59.002954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-05-17 09:43:59.002954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.002954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.002954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:43:59.006954 iac_init-0.6.5/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:43:59.010954 iac_init-0.6.5/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rwxr-xr-x   0        0        0    62360 2024-05-17 09:44:06.271113 iac_init-0.6.5/iac_init/utils/exceptions.so
+-rwxr-xr-x   0        0        0   333200 2024-05-17 09:44:06.083109 iac_init-0.6.5/iac_init/utils/functional.so
+-rwxr-xr-x   0        0        0   859344 2024-05-17 09:44:05.003084 iac_init-0.6.5/iac_init/validator.so
+-rwxr-xr-x   0        0        0   503296 2024-05-17 09:44:08.063153 iac_init-0.6.5/iac_init/yaml_conf/yaml.so
+-rwxr-xr-x   0        0        0   601184 2024-05-17 09:44:10.539208 iac_init-0.6.5/iac_init/yaml_conf/yaml_writer.so
+-rw-r--r--   0        0        0     1636 2024-05-17 09:43:59.014954 iac_init-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.6.5/PKG-INFO
```

### Comparing `iac_init-0.6.4/LICENSE` & `iac_init-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/conf/__init__.py` & `iac_init-0.6.5/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.6.5/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.6.5/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.6.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.6.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.6.5/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.4/pyproject.toml` & `iac_init-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.6.4"
+version = "0.6.5"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.6.4/PKG-INFO` & `iac_init-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.6.4
+Version: 0.6.5
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

