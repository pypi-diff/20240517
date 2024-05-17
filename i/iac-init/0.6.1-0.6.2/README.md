# Comparing `tmp/iac_init-0.6.1.tar.gz` & `tmp/iac_init-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.6.1.tar", max compression
+gzip compressed data, was "iac_init-0.6.2.tar", max compression
```

## Comparing `iac_init-0.6.1.tar` & `iac_init-0.6.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0    16295 2024-05-10 08:28:05.368815 iac_init-0.6.1/LICENSE
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.368815 iac_init-0.6.1/README.md
--rw-r--r--   0        0        0      389 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/__main__.py
--rw-r--r--   0        0        0    11616 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/cli/main.py
--rw-r--r--   0        0        0      206 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/cli/options.py
--rw-r--r--   0        0        0     2064 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     2886 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0     1406 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2595 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     7490 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      453 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0      263 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      334 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/scripts/thread_tool.py
--rw-r--r--   0        0        0     3778 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-10 08:28:05.368815 iac_init-0.6.1/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-10 08:28:05.372815 iac_init-0.6.1/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/templates/12-config_backup/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4910 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/utils/functional.py
--rw-r--r--   0        0        0    12028 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/validator.py
--rw-r--r--   0        0        0     5093 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5222 2024-05-10 08:28:05.376815 iac_init-0.6.1/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1636 2024-05-10 08:28:05.376815 iac_init-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-17 09:27:31.653525 iac_init-0.6.2/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.653525 iac_init-0.6.2/README.md
+-rw-r--r--   0        0        0      389 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/__main__.py
+-rw-r--r--   0        0        0    11616 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/cli/main.py
+-rw-r--r--   0        0        0      206 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/cli/options.py
+-rw-r--r--   0        0        0     2064 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     2886 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1397 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2595 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7490 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      453 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0      263 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      334 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/scripts/thread_tool.py
+-rw-r--r--   0        0        0     3778 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-17 09:27:31.653525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:27:31.657525 iac_init-0.6.2/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4910 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    12040 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/validator.py
+-rw-r--r--   0        0        0     5093 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5222 2024-05-17 09:27:31.661525 iac_init-0.6.2/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1636 2024-05-17 09:27:31.665525 iac_init-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.6.2/PKG-INFO
```

### Comparing `iac_init-0.6.1/LICENSE` & `iac_init-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/cli/main.py` & `iac_init-0.6.2/iac_init/cli/main.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/conf/__init__.py` & `iac_init-0.6.2/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/conf/global_settings.py` & `iac_init-0.6.2/iac_init/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/scripts/ansible_tool.py` & `iac_init-0.6.2/iac_init/scripts/ansible_tool.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 import re
 import os
 from ansible_runner import run
 from iac_init.conf import settings
 
 def ansible_deploy_function(playbook_dir, step_name, option, inventory_path=None, quiet=True):
     import logging
-    from logging.handlers import TimedRotatingFileHandler
+    from logging.handlers import RotatingFileHandler
 
     logger = logging.getLogger(playbook_dir)
     logger.setLevel(logging.INFO)
     log_formatter = logging.Formatter('%(message)s')
     log_file = os.path.join(settings.OUTPUT_BASE_DIR, 'iac_init_log',
                             'iac-init-{}-{}.log'.format(option, step_name))
-    file_handler = TimedRotatingFileHandler(log_file, when="M", interval=30, backupCount=0)
+    file_handler = RotatingFileHandler(log_file, maxBytes=30*1024*1024, backupCount=0)
     file_handler.setFormatter(log_formatter)
     logger.addHandler(file_handler)
 
     def callback(res):
         if not quiet and 'stdout' in res:
             print(res['stdout'])
         output = re.compile(r'\x1b\[\[?(?:\d{1,2}(?:;\d{0,2})*)?[m|K]').sub('', res['stdout'])
@@ -31,8 +31,8 @@
 
     if runner.status == "successful":
         logger.info("Successfully finish Step {}: {}".format(option, step_name.upper()))
         return True
 
     else:
         logger.error("Failed run Step {}: {}".format(option, step_name.upper()))
-        return False
+        return False
```

### Comparing `iac_init-0.6.1/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.6.2/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.6.2/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.6.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.6.2/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.6.2/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.6.2/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.6.2/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/utils/functional.py` & `iac_init-0.6.2/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/validator.py` & `iac_init-0.6.2/iac_init/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
 
 import os
 import re
+import time
 import shutil
 import logging
 from ruamel import yaml
 from loguru import logger
 from typing import Any, Dict, List, Optional
 
 from iac_init.conf import settings
```

### Comparing `iac_init-0.6.1/iac_init/yaml_conf/yaml.py` & `iac_init-0.6.2/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.6.2/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.6.1/pyproject.toml` & `iac_init-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.6.1/PKG-INFO` & `iac_init-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

