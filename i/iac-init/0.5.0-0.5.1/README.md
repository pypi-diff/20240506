# Comparing `tmp/iac_init-0.5.0.tar.gz` & `tmp/iac_init-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.5.0.tar", max compression
+gzip compressed data, was "iac_init-0.5.1.tar", max compression
```

## Comparing `iac_init-0.5.0.tar` & `iac_init-0.5.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0    16295 2024-05-06 09:05:17.811920 iac_init-0.5.0/LICENSE
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.811920 iac_init-0.5.0/README.md
--rw-r--r--   0        0        0      389 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/__main__.py
--rw-r--r--   0        0        0    13768 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/cli/main.py
--rw-r--r--   0        0        0      206 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/cli/options.py
--rw-r--r--   0        0        0     2064 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     2886 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0     1041 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2595 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     7490 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      453 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0      263 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0     3778 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6823 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1464 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1020 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-06 09:05:17.811920 iac_init-0.5.0/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 09:05:17.815920 iac_init-0.5.0/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/templates/12-config_backup/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4910 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/utils/functional.py
--rw-r--r--   0        0        0    11463 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/validator.py
--rw-r--r--   0        0        0     5093 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5222 2024-05-06 09:05:17.819920 iac_init-0.5.0/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1636 2024-05-06 09:05:17.819920 iac_init-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-06 10:00:00.443603 iac_init-0.5.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.443603 iac_init-0.5.1/README.md
+-rw-r--r--   0        0        0      389 2024-05-06 10:00:00.443603 iac_init-0.5.1/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-06 10:00:00.443603 iac_init-0.5.1/iac_init/__main__.py
+-rw-r--r--   0        0        0    13247 2024-05-06 10:00:00.443603 iac_init-0.5.1/iac_init/cli/main.py
+-rw-r--r--   0        0        0      206 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/cli/options.py
+-rw-r--r--   0        0        0     2064 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     2886 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1041 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2595 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7490 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      453 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0      263 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0     3778 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6823 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1464 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1522 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-06 10:00:00.447603 iac_init-0.5.1/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-06 10:00:00.451603 iac_init-0.5.1/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-06 10:00:00.455603 iac_init-0.5.1/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-05-06 10:00:00.455603 iac_init-0.5.1/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4910 2024-05-06 10:00:00.455603 iac_init-0.5.1/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    11463 2024-05-06 10:00:00.455603 iac_init-0.5.1/iac_init/validator.py
+-rw-r--r--   0        0        0     5093 2024-05-06 10:00:00.455603 iac_init-0.5.1/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5222 2024-05-06 10:00:00.455603 iac_init-0.5.1/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1636 2024-05-06 10:00:00.455603 iac_init-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.5.1/PKG-INFO
```

### Comparing `iac_init-0.5.0/LICENSE` & `iac_init-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/cli/main.py` & `iac_init-0.5.1/iac_init/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -154,19 +154,14 @@
 
             except Exception as e:
                 msg = "Run Step 1 wipe aci fabric ansible-playbook failed detail:\nError: {}".format(e)
                 logger.error(msg)
                 exit()
 
         elif int(option) in [2]:
-            global ansible_run_result
-            ansible_run_result = 1
-            error = validator.validate_ssh_telnet_connection()
-            if error:
-                exit()
             yaml_path = validator.validate_yaml_exist(settings.DEFAULT_DATA_PATH)
             if not yaml_path:
                 exit()
             error = validator.validate_cimc_precheck()
             if error:
                 exit()
             option_yaml_path = validator.validate_yaml_exist(settings.DATA_PATH[int(option) - 1])
@@ -215,31 +210,23 @@
                                  quiet=True, event_handler=callback)
 
                     if runner.status == "successful":
                         logger.info("Successfully finish Step {}: {}".format(option, step_name.upper()))
 
                     else:
                         logger.error("Failed run Step {}: {}".format(option, step_name.upper()))
-                        global ansible_run_result
-                        ansible_run_result = 0
+                        exit()
 
                 ansible_deploy_function("playbook_apic_discovery.yaml", settings.ANSIBLE_STEP[5])
 
             except Exception as e:
                 msg = "Run Step 2 APIC discovery ansible-playbook fail detail:\nError: {}".format(e)
                 logger.error(msg)
                 exit()
 
-            global ansible_run_result
-            if ansible_run_result == 0:
-                logger.error("Exist iac-init tool Step 1 failed pls check log for detail")
-                exit()
-            else:
-                logger.info("Wipe aci fabric Success proceed.")
-
         else:
             error = validator.validate_apic_aaa_connection()
             if error:
                 exit()
             yaml_path = validator.validate_yaml_exist(settings.DEFAULT_DATA_PATH)
             if not yaml_path:
                 exit()
@@ -290,8 +277,8 @@
                 exit()
 
 
 def exit() -> None:
     if error_handler.fired:
         sys.exit(1)
     else:
-        sys.exit(0)
+        sys.exit(0)
```

### Comparing `iac_init-0.5.0/iac_init/conf/__init__.py` & `iac_init-0.5.1/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/conf/global_settings.py` & `iac_init-0.5.1/iac_init/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/scripts/ansible_tool.py` & `iac_init-0.5.1/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.5.1/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.5.1/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.5.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.5.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.5.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.5.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/utils/functional.py` & `iac_init-0.5.1/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/validator.py` & `iac_init-0.5.1/iac_init/validator.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/yaml_conf/yaml.py` & `iac_init-0.5.1/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.5.1/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.0/pyproject.toml` & `iac_init-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.5.0"
+version = "0.5.1"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.5.0/PKG-INFO` & `iac_init-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

