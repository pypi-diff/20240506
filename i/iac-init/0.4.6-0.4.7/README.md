# Comparing `tmp/iac_init-0.4.6.tar.gz` & `tmp/iac_init-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.4.6.tar", max compression
+gzip compressed data, was "iac_init-0.4.7.tar", max compression
```

## Comparing `iac_init-0.4.6.tar` & `iac_init-0.4.7.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0    16295 2024-04-18 08:19:45.728918 iac_init-0.4.6/LICENSE
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.728918 iac_init-0.4.6/README.md
--rw-r--r--   0        0        0      389 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/__main__.py
--rw-r--r--   0        0        0     9237 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/cli/main.py
--rw-r--r--   0        0        0      206 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/cli/options.py
--rw-r--r--   0        0        0     2064 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     2886 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0      747 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2595 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     6788 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      453 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0      263 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0     3778 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6823 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1464 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5432 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0       22 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/02-discover_apic/apic_discovery/files/exp_files
--rw-r--r--   0        0        0     1016 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.j2
--rw-r--r--   0        0        0     3585 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.j2
--rw-r--r--   0        0        0     1656 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.j2
--rw-r--r--   0        0        0     1994 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/02-discover_apic/apic_discovery/vars/main.yml
--rw-r--r--   0        0        0      181 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 08:19:45.728918 iac_init-0.4.6/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 08:19:45.732918 iac_init-0.4.6/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/templates/12-config_backup/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4910 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/utils/functional.py
--rw-r--r--   0        0        0    11462 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/validator.py
--rw-r--r--   0        0        0     5093 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5222 2024-04-18 08:19:45.736918 iac_init-0.4.6/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1636 2024-04-18 08:19:45.736918 iac_init-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-05 06:03:49.403116 iac_init-0.4.7/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.403116 iac_init-0.4.7/README.md
+-rw-r--r--   0        0        0      389 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/__main__.py
+-rw-r--r--   0        0        0     9237 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/cli/main.py
+-rw-r--r--   0        0        0      206 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/cli/options.py
+-rw-r--r--   0        0        0     2064 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     2886 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1011 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2595 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7490 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      453 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0      263 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0     3778 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6823 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1464 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-05 06:03:49.403116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1020 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-05 06:03:49.407116 iac_init-0.4.7/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4910 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    11463 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/validator.py
+-rw-r--r--   0        0        0     5093 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5222 2024-05-05 06:03:49.411116 iac_init-0.4.7/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1636 2024-05-05 06:03:49.411116 iac_init-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.4.7/PKG-INFO
```

### Comparing `iac_init-0.4.6/LICENSE` & `iac_init-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/cli/main.py` & `iac_init-0.4.7/iac_init/cli/main.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/conf/__init__.py` & `iac_init-0.4.7/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/conf/global_settings.py` & `iac_init-0.4.7/iac_init/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.4.7/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.4.7/iac_init/scripts/cimc_precheck_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,14 +154,35 @@
         return True
 
     except Exception as e:
         msg = "{}".format(e)
         logger.error(msg)
         return False
 
+def power_down_cimc(CIMC_IP, token):
+    try:
+        cimc_power_down_data = f'''
+        <!-- CIMC Power Off -->
+        <configConfMo cookie="{token}"><inConfig>
+            <computeRackUnit dn="sys/rack-unit-1" adminPower="down" />
+        </inConfig></configConfMo>
+        '''
+        cimc_power_down_response = cimc_api(CIMC_IP, cimc_power_down_data)
+        if cimc_power_down_response:
+            logger.info("CIMC is powered down.")
+        else:
+            return False
+
+        return True
+
+    except Exception as e:
+        msg = "{}".format(e)
+        logger.error(msg)
+        return False
+
 def cimc_precheck(CIMC_IP, CIMC_USERNAME, CIMC_PASSWORD):
     try:
         token = cimc_login(CIMC_IP, CIMC_USERNAME, CIMC_PASSWORD)
         health_check_result = cimc_health_check(CIMC_IP, token)
         if not health_check_result:
             logger.error("CIMC health check failed!!")
             return False
@@ -170,14 +191,17 @@
 
         cimc_mapping_clean_result = cimc_mapping_clean(CIMC_IP, token)
         if not cimc_mapping_clean_result:
             logger.error("CIMC mapping clean failed!!")
             return False
 
         logger.info("CIMC mapping clean successfully!")
+        logger.info("Powering down CIMC...")
+        power_down_cimc(CIMC_IP, token)
         cimc_logout(CIMC_IP, token)
+        
         return True
 
     except Exception as e:
         msg = "{}".format(e)
         logger.error(msg)
         return False
```

### Comparing `iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -34,28 +34,31 @@
 
           <!-- Configure NTP -->
           <configConfMo><inConfig>
             <commNtpProvider dn="sys/svc-ext/ntp-svc" ntpServer1="{{ fabric.global_policies.ntp_server }}"/>
           </inConfig></configConfMo>
 
           <!-- Configure SOL -->
+          <configConfMo><inConfig>
+            <solIf dn="sys/rack-unit-1/sol-if" adminState="enable" speed="115200" comport="com0" sshPort="2400"/>
+          </inConfig></configConfMo>
 
           <!-- Configure CIMC mapping -->
           <configConfMo><inConfig>
             <commVMediaMap volumeName="aci-automation" map="www" remoteShare="{{ fabric.global_policies.aci_image_path }}" remoteFile="{{ fabric.global_policies.apic_image }}" dn="sys/svc-ext/vmedia-svc/vmmap-aci-automation" ></commVMediaMap>
           </inConfig></configConfMo>
 
           <!-- IMC change boot order to CIMC-map -->
           <configConfMo><inConfig>
             <lsbootVMedia dn="sys/rack-unit-1/boot-precision/vm-cimc-map" name="cimc-map" type="VMEDIA" subtype="cimc-mapped-dvd"  order="1" state="Enabled" />
           </inConfig></configConfMo>
 
-          <!-- CIMC hard reset -->
+          <!-- CIMC power up -->
           <configConfMo><inConfig>
-            <computeRackUnit dn="sys/rack-unit-1" adminPower="hard-reset-immediate" />
+            <computeRackUnit dn="sys/rack-unit-1" adminPower="up" />
           </inConfig></configConfMo>
 
       delegate_to: localhost
       loop: "{{ fabric.apic_nodes_connection }}"
 
     - name: Render APIC HTTP speed up script
       template:
```

### Comparing `iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.4.7/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.4.7/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         cmd: echo {{ fabric.global_policies.apic_image }} | awk -F '.' '{print $2}'
       register: apic_version
 
     ## TBD step: Reboot APIC
 
     - name: Render APIC discovery script
       template:
-        src: apic_discovery{{ apic_version.stdout }}.exp.j2
+        src: apic_discovery{{ apic_version.stdout }}.exp.jinja2
         dest: apic_discovery/files/apic_discovery_{{ item.hostname }}.exp
       delegate_to: localhost
       loop: "{{ fabric.apic_nodes_connection }}"
 
     - name: Make APIC discovery script executable
       file:
         path: apic_discovery/files/apic_discovery_{{ item.hostname }}.exp
```

### Comparing `iac_init-0.4.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.j2` & `iac_init-0.4.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.j2` & `iac_init-0.4.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.j2` & `iac_init-0.4.7/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/utils/functional.py` & `iac_init-0.4.7/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/validator.py` & `iac_init-0.4.7/iac_init/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
             image32 = settings.global_policy['fabric']['global_policies']['switch_image32']
             image64 = settings.global_policy['fabric']['global_policies']['switch_image64']
 
             pattern_32 = r"^(.+)\.bin"
             pattern_64 = r'(.+)-cs_64.bin'
 
             if image32 == image64:
-                if not image32.endwith(".bin"):
+                if not image32.endswith(".bin"):
                     msg = "Validate error: Image name must end with .bin."
                     logger.error(msg)
                     return True
             else:
                 if not re.match(pattern_32, image32).group(1) == re.match(pattern_64, image64).group(1):
                     msg = "Validate error: switch_image32 and switch_image64 checking failed."
                     logger.error(msg)
```

### Comparing `iac_init-0.4.6/iac_init/yaml_conf/yaml.py` & `iac_init-0.4.7/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.4.7/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.4.6/pyproject.toml` & `iac_init-0.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.4.6"
+version = "0.4.7"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.4.6/PKG-INFO` & `iac_init-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.4.6
+Version: 0.4.7
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

