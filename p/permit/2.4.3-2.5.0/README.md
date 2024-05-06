# Comparing `tmp/permit-2.4.3.tar.gz` & `tmp/permit-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-2.4.3.tar", last modified: Thu Apr 18 17:29:07 2024, max compression
+gzip compressed data, was "permit-2.5.0.tar", last modified: Mon May  6 14:21:45 2024, max compression
```

## Comparing `permit-2.4.3.tar` & `permit-2.5.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.105849 permit-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 17:27:48.000000 permit-2.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-18 17:27:48.000000 permit-2.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-18 17:29:07.105849 permit-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-18 17:27:48.000000 permit-2.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.097849 permit-2.4.3/permit/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-18 17:27:48.000000 permit-2.4.3/permit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.101849 permit-2.4.3/permit/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/condition_set_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/condition_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9818 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)   160550 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/relationship_tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resource_action_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resource_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resource_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resource_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resource_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resource_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/role_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/sync_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-18 17:27:48.000000 permit-2.4.3/permit/api/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-18 17:27:48.000000 permit-2.4.3/permit/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.101849 permit-2.4.3/permit/enforcement/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:48.000000 permit-2.4.3/permit/enforcement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-04-18 17:27:48.000000 permit-2.4.3/permit/enforcement/enforcer.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-18 17:27:48.000000 permit-2.4.3/permit/enforcement/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-18 17:27:48.000000 permit-2.4.3/permit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-18 17:27:48.000000 permit-2.4.3/permit/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.101849 permit-2.4.3/permit/pdp_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:48.000000 permit-2.4.3/permit/pdp_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-18 17:27:48.000000 permit-2.4.3/permit/pdp_api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-18 17:27:48.000000 permit-2.4.3/permit/pdp_api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-18 17:27:48.000000 permit-2.4.3/permit/pdp_api/pdp_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-18 17:27:48.000000 permit-2.4.3/permit/pdp_api/role_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-18 17:27:48.000000 permit-2.4.3/permit/permit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-18 17:27:48.000000 permit-2.4.3/permit/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.105849 permit-2.4.3/permit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:48.000000 permit-2.4.3/permit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-18 17:27:48.000000 permit-2.4.3/permit/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-18 17:27:48.000000 permit-2.4.3/permit/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-18 17:27:48.000000 permit-2.4.3/permit/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-18 17:27:48.000000 permit-2.4.3/permit/utils/pydantic_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-18 17:27:48.000000 permit-2.4.3/permit/utils/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.097849 permit-2.4.3/permit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-18 17:29:07.000000 permit-2.4.3/permit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-18 17:29:07.000000 permit-2.4.3/permit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:29:07.000000 permit-2.4.3/permit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 17:29:07.000000 permit-2.4.3/permit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 17:29:07.000000 permit-2.4.3/permit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 17:27:48.000000 permit-2.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:29:07.105849 permit-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 17:29:05.000000 permit-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:29:07.105849 permit-2.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:27:48.000000 permit-2.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-18 17:27:48.000000 permit-2.4.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-04-18 17:27:48.000000 permit-2.4.3/tests/test_abac_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-18 17:27:48.000000 permit-2.4.3/tests/test_abac_pdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-04-18 17:27:48.000000 permit-2.4.3/tests/test_rbac_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-04-18 17:27:48.000000 permit-2.4.3/tests/test_rbac_e2e_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    30220 2024-04-18 17:27:48.000000 permit-2.4.3/tests/test_rebac_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-18 17:27:48.000000 permit-2.4.3/tests/utils.py
+drwxr-xr-x   0 odedbd     (501) staff       (20)        0 2024-05-06 14:21:45.802122 permit-2.5.0/
+-rw-r--r--   0 odedbd     (501) staff       (20)    11357 2024-05-02 14:36:11.000000 permit-2.5.0/LICENSE
+-rw-r--r--   0 odedbd     (501) staff       (20)       30 2022-05-23 18:17:23.000000 permit-2.5.0/MANIFEST.in
+-rw-r--r--   0 odedbd     (501) staff       (20)      771 2024-05-06 14:21:45.801936 permit-2.5.0/PKG-INFO
+-rw-r--r--   0 odedbd     (501) staff       (20)      299 2024-05-06 14:10:43.000000 permit-2.5.0/README.md
+drwxr-xr-x   0 odedbd     (501) staff       (20)        0 2024-05-06 14:21:45.789330 permit-2.5.0/permit/
+-rw-r--r--   0 odedbd     (501) staff       (20)      417 2024-05-06 14:10:47.000000 permit-2.5.0/permit/__init__.py
+drwxr-xr-x   0 odedbd     (501) staff       (20)        0 2024-05-06 14:21:45.796267 permit-2.5.0/permit/api/
+-rw-r--r--   0 odedbd     (501) staff       (20)        0 2024-05-02 14:33:02.000000 permit-2.5.0/permit/api/__init__.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     5622 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/api_client.py
+-rw-r--r--   0 odedbd     (501) staff       (20)    12212 2024-05-06 14:10:47.000000 permit-2.5.0/permit/api/base.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     4020 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/condition_set_rules.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     6218 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/condition_sets.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     8347 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/context.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     6493 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/deprecated.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     2102 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/elements.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     9818 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/environments.py
+-rw-r--r--   0 odedbd     (501) staff       (20)   160550 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/models.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     5864 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/projects.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     6510 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/relationship_tuples.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     7176 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/resource_action_groups.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     6842 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/resource_actions.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     7148 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/resource_attributes.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     9617 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/resource_instances.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     5941 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/resource_relations.py
+-rw-r--r--   0 odedbd     (501) staff       (20)    12471 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/resource_roles.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     6814 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/resources.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     6265 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/role_assignments.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     7541 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/roles.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     7125 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/sync_api_client.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     9843 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/tenants.py
+-rw-r--r--   0 odedbd     (501) staff       (20)    12949 2024-05-02 14:36:11.000000 permit-2.5.0/permit/api/users.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     2447 2024-05-06 14:10:47.000000 permit-2.5.0/permit/config.py
+drwxr-xr-x   0 odedbd     (501) staff       (20)        0 2024-05-06 14:21:45.797078 permit-2.5.0/permit/enforcement/
+-rw-r--r--   0 odedbd     (501) staff       (20)        0 2022-05-23 18:17:23.000000 permit-2.5.0/permit/enforcement/__init__.py
+-rw-r--r--   0 odedbd     (501) staff       (20)    18796 2024-05-06 14:10:47.000000 permit-2.5.0/permit/enforcement/enforcer.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     2005 2024-05-06 14:21:13.000000 permit-2.5.0/permit/enforcement/interfaces.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     3928 2024-05-06 14:10:47.000000 permit-2.5.0/permit/exceptions.py
+-rw-r--r--   0 odedbd     (501) staff       (20)      212 2024-05-02 14:36:11.000000 permit-2.5.0/permit/logger.py
+drwxr-xr-x   0 odedbd     (501) staff       (20)        0 2024-05-06 14:21:45.797992 permit-2.5.0/permit/pdp_api/
+-rw-r--r--   0 odedbd     (501) staff       (20)        0 2024-05-06 14:10:43.000000 permit-2.5.0/permit/pdp_api/__init__.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     1631 2024-05-06 14:10:43.000000 permit-2.5.0/permit/pdp_api/base.py
+-rw-r--r--   0 odedbd     (501) staff       (20)      865 2024-05-06 14:10:43.000000 permit-2.5.0/permit/pdp_api/models.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     1121 2024-05-06 14:10:43.000000 permit-2.5.0/permit/pdp_api/pdp_api_client.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     2636 2024-05-06 14:10:43.000000 permit-2.5.0/permit/pdp_api/role_assignments.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     6416 2024-05-06 14:10:47.000000 permit-2.5.0/permit/permit.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     4296 2024-05-06 14:10:43.000000 permit-2.5.0/permit/sync.py
+drwxr-xr-x   0 odedbd     (501) staff       (20)        0 2024-05-06 14:21:45.799192 permit-2.5.0/permit/utils/
+-rw-r--r--   0 odedbd     (501) staff       (20)        0 2022-05-23 18:17:23.000000 permit-2.5.0/permit/utils/__init__.py
+-rw-r--r--   0 odedbd     (501) staff       (20)      836 2024-05-02 14:36:11.000000 permit-2.5.0/permit/utils/context.py
+-rw-r--r--   0 odedbd     (501) staff       (20)      625 2024-05-02 14:36:11.000000 permit-2.5.0/permit/utils/deprecation.py
+-rw-r--r--   0 odedbd     (501) staff       (20)      444 2022-05-23 18:17:23.000000 permit-2.5.0/permit/utils/dicts.py
+-rw-r--r--   0 odedbd     (501) staff       (20)       85 2024-05-02 14:36:11.000000 permit-2.5.0/permit/utils/pydantic_version.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     1351 2024-05-06 14:10:43.000000 permit-2.5.0/permit/utils/sync.py
+drwxr-xr-x   0 odedbd     (501) staff       (20)        0 2024-05-06 14:21:45.790264 permit-2.5.0/permit.egg-info/
+-rw-r--r--   0 odedbd     (501) staff       (20)      771 2024-05-06 14:21:45.000000 permit-2.5.0/permit.egg-info/PKG-INFO
+-rw-r--r--   0 odedbd     (501) staff       (20)     1522 2024-05-06 14:21:45.000000 permit-2.5.0/permit.egg-info/SOURCES.txt
+-rw-r--r--   0 odedbd     (501) staff       (20)        1 2024-05-06 14:21:45.000000 permit-2.5.0/permit.egg-info/dependency_links.txt
+-rw-r--r--   0 odedbd     (501) staff       (20)      104 2024-05-06 14:21:45.000000 permit-2.5.0/permit.egg-info/requires.txt
+-rw-r--r--   0 odedbd     (501) staff       (20)       13 2024-05-06 14:21:45.000000 permit-2.5.0/permit.egg-info/top_level.txt
+-rw-r--r--   0 odedbd     (501) staff       (20)      104 2024-05-02 14:36:11.000000 permit-2.5.0/requirements.txt
+-rw-r--r--   0 odedbd     (501) staff       (20)       38 2024-05-06 14:21:45.802177 permit-2.5.0/setup.cfg
+-rw-r--r--   0 odedbd     (501) staff       (20)     1069 2024-05-06 14:20:57.000000 permit-2.5.0/setup.py
+drwxr-xr-x   0 odedbd     (501) staff       (20)        0 2024-05-06 14:21:45.801618 permit-2.5.0/tests/
+-rw-r--r--   0 odedbd     (501) staff       (20)        0 2022-12-25 11:28:38.000000 permit-2.5.0/tests/__init__.py
+-rw-r--r--   0 odedbd     (501) staff       (20)     1894 2024-05-02 14:36:11.000000 permit-2.5.0/tests/conftest.py
+-rw-r--r--   0 odedbd     (501) staff       (20)    10459 2024-05-02 14:36:11.000000 permit-2.5.0/tests/test_abac_e2e.py
+-rw-r--r--   0 odedbd     (501) staff       (20)      943 2024-05-02 14:36:11.000000 permit-2.5.0/tests/test_abac_pdp.py
+-rw-r--r--   0 odedbd     (501) staff       (20)    13092 2024-05-06 14:10:47.000000 permit-2.5.0/tests/test_rbac_e2e.py
+-rw-r--r--   0 odedbd     (501) staff       (20)    10147 2024-05-06 14:10:43.000000 permit-2.5.0/tests/test_rbac_e2e_sync.py
+-rw-r--r--   0 odedbd     (501) staff       (20)    31476 2024-05-06 14:10:47.000000 permit-2.5.0/tests/test_rebac_e2e.py
+-rw-r--r--   0 odedbd     (501) staff       (20)      358 2024-05-02 14:36:11.000000 permit-2.5.0/tests/utils.py
```

### Comparing `permit-2.4.3/LICENSE` & `permit-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/PKG-INFO` & `permit-2.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permit
-Version: 2.4.3
+Version: 2.5.0
 Summary: Permit.io python sdk
 Author: Asaf Cohen
 Author-email: asaf@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `permit-2.4.3/permit/api/api_client.py` & `permit-2.5.0/permit/api/api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/base.py` & `permit-2.5.0/permit/api/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import functools
 from typing import Callable, Optional, Type, TypeVar, Union
 
 import aiohttp
+from aiohttp import ClientTimeout
 from loguru import logger
 
 from ..utils.pydantic_version import PYDANTIC_VERSION
 
 if PYDANTIC_VERSION < (2, 0):
     from pydantic import BaseModel, Extra, Field, parse_obj_as
 else:
@@ -73,17 +74,21 @@
 
 
 class SimpleHttpClient:
     """
     wraps aiohttp client to reduce boilerplace
     """
 
-    def __init__(self, client_config: dict, base_url: str = ""):
+    def __init__(
+        self, client_config: dict, base_url: str = "", timeout: Optional[int] = None
+    ):
         self._client_config = client_config
         self._base_url = base_url
+        if timeout is not None:
+            self._client_config["timeout"] = ClientTimeout(total=timeout)
 
     def _log_request(self, url: str, method: str) -> None:
         logger.debug("Sending HTTP request: {} {}".format(method, url))
 
     def _log_response(self, url: str, method: str, status: int) -> None:
         logger.debug(
             "Received HTTP response: {} {}, status: {}".format(method, url, status)
@@ -217,14 +222,15 @@
             },
         )
         client_config = client_config.dict()
         client_config.update(kwargs)
         return SimpleHttpClient(
             client_config,
             base_url=endpoint_url,
+            timeout=self.config.api_timeout,
         )
 
     async def _set_context_from_api_key(self) -> None:
         """
         Set the API context and permitted access level based on the API key scope.
         """
         logger.debug("Fetching api key scope")
```

### Comparing `permit-2.4.3/permit/api/condition_set_rules.py` & `permit-2.5.0/permit/api/condition_set_rules.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/condition_sets.py` & `permit-2.5.0/permit/api/condition_sets.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/context.py` & `permit-2.5.0/permit/api/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/deprecated.py` & `permit-2.5.0/permit/api/deprecated.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/elements.py` & `permit-2.5.0/permit/api/elements.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/environments.py` & `permit-2.5.0/permit/api/environments.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/models.py` & `permit-2.5.0/permit/api/models.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/projects.py` & `permit-2.5.0/permit/api/projects.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/relationship_tuples.py` & `permit-2.5.0/permit/api/relationship_tuples.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/resource_action_groups.py` & `permit-2.5.0/permit/api/resource_action_groups.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/resource_actions.py` & `permit-2.5.0/permit/api/resource_actions.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/resource_attributes.py` & `permit-2.5.0/permit/api/resource_attributes.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/resource_instances.py` & `permit-2.5.0/permit/api/resource_instances.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/resource_relations.py` & `permit-2.5.0/permit/api/resource_relations.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/resource_roles.py` & `permit-2.5.0/permit/api/resource_roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/resources.py` & `permit-2.5.0/permit/api/resources.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/role_assignments.py` & `permit-2.5.0/permit/api/role_assignments.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/roles.py` & `permit-2.5.0/permit/api/roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/sync_api_client.py` & `permit-2.5.0/permit/api/sync_api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/tenants.py` & `permit-2.5.0/permit/api/tenants.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/api/users.py` & `permit-2.5.0/permit/api/users.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/config.py` & `permit-2.5.0/permit/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -57,10 +57,18 @@
     multi_tenancy: MultiTenancyConfig = Field(
         MultiTenancyConfig(),
         description="configuration of default tenant assignment for RBAC",
     )
     api_context: ApiContext = Field(
         ApiContext(), description="represents the current API key authorization level."
     )
+    api_timeout: int = Field(
+        None,
+        description="The timeout in seconds for requests to the Permit REST API.",
+    )
+    pdp_timeout: int = Field(
+        None,
+        description="The timeout in seconds for requests to the PDP.",
+    )
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `permit-2.4.3/permit/enforcement/enforcer.py` & `permit-2.5.0/permit/enforcement/enforcer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import json
 from pprint import pformat
 from typing import Union
 
 import aiohttp
+from aiohttp import ClientTimeout
 from loguru import logger
+from pydantic import parse_obj_as
 
 from ..config import PermitConfig
 from ..exceptions import PermitConnectionError
 from ..utils.context import Context, ContextStore
 from ..utils.sync import SyncClass
-from .interfaces import ResourceInput, UserInput
+from .interfaces import AuthorizedUsersResult, ResourceInput, UserInput
 
 
 def set_if_not_none(d: dict, k: str, v):
     if v is not None:
         d[k] = v
 
 
@@ -44,14 +46,123 @@
     def context_store(self):
         """
         we let context store be accessed from the outside so that the
         using app can setup a flexible contextual behavior for authorization queries
         """
         return self._context_store
 
+    @property
+    def _timeout_config(self):
+        timeout_config = {}
+        if self._config.pdp_timeout is not None:
+            timeout_config["timeout"] = ClientTimeout(total=self._config.pdp_timeout)
+        return timeout_config
+
+    async def authorized_users(
+        self,
+        action: Action,
+        resource: Resource,
+        context: Context = {},
+    ) -> AuthorizedUsersResult:
+        """
+        Queries to get all the users that are authorized to perform an action on a resource within the specified context.
+
+        Args:
+            action: The action to be performed on the resource.
+            resource: The resource object representing the resource.
+            context: The context object representing the context in which the action is performed. Defaults to None.
+
+        Returns:
+            AuthorizedUsersResult: Contains all the authorized users and the role assignments that granted the permission.
+
+        Raises:
+            PermitConnectionError: If an error occurs while sending the authorization request to the PDP.
+
+        Examples:
+
+            # all the users that can close any issue?
+            await permit.authorized_users('close', 'issue')
+
+            # all the users that can close an issue who's id is 1234?
+            await permit.authorized_users('close', 'issue:1234')
+
+            # all the users that can close (any) issues belonging to the 't1' tenant?
+            # (in a multi tenant application)
+            await permit.authorized_users('close', {'type': 'issue', 'tenant': 't1'})
+        """
+        normalized_resource: ResourceInput = self._normalize_resource(
+            (
+                self._resource_from_string(resource)
+                if isinstance(resource, str)
+                else ResourceInput(**resource)
+            )
+        )
+        query_context = self._context_store.get_derived_context(context)
+        input = dict(
+            action=action,
+            resource=normalized_resource.dict(exclude_unset=True),
+            context=query_context,
+        )
+
+        async with aiohttp.ClientSession(
+            headers=self._headers, **self._timeout_config
+        ) as session:
+            check_url = f"{self._base_url}/authorized_users"
+            try:
+                async with session.post(
+                    check_url,
+                    data=json.dumps(input),
+                ) as response:
+                    if response.status != 200:
+                        if response.status == 501:
+                            raise PermitConnectionError(
+                                f"Permit SDK got an error: {response.status},\n"
+                                "and cannot connect to the PDP container. Please ensure you are not using ABAC/ReBAC policies,\n"
+                                "as the cloud PDP is not compatible with these kinds of policies.\n"
+                                "Also, please check your configuration and make sure it's running at {self._base_url} and accepting requests.\n"
+                                "Read more about setting up the PDP at "
+                                "https://docs.permit.io/sdk/python/quickstart-python/#2-setup-your-pdp-policy-decision-point-container"
+                            )
+
+                        error_json: dict = await response.json()
+                        logger.error(
+                            "error in permit.authorized_users({}, {}):\n{}\n{}".format(
+                                action,
+                                self._resource_repr(normalized_resource),
+                                f"status code: {response.status}",
+                                repr(error_json),
+                            )
+                        )
+                        raise PermitConnectionError(
+                            f"Permit SDK got unexpected status code: {response.status}, please check your Permit SDK class init and PDP container are configured correctly. \n\
+                            Read more about setting up the PDP at https://docs.permit.io/sdk/python/quickstart-python/#2-setup-your-pdp-policy-decision-point-container"
+                        )
+
+                    content: dict = await response.json()
+                    logger.debug(
+                        f"permit.authorized_users() response:\ninput: {pformat(input, indent=2)}\nresponse status: {response.status}\nresponse data: {pformat(content, indent=2)}"
+                    )
+                    result: AuthorizedUsersResult = parse_obj_as(
+                        AuthorizedUsersResult, content
+                    )
+                    return result
+            except aiohttp.ClientError as err:
+                logger.error(
+                    "error in permit.authorized_users({}, {}):\n{}".format(
+                        action,
+                        self._resource_repr(normalized_resource),
+                        err,
+                    )
+                )
+                raise PermitConnectionError(
+                    f"Permit SDK got error: {err}, \n \
+                    and cannot connect to the PDP container, please check your configuration and make sure it's running at {self._base_url} and accepting requests. \n \
+                    Read more about setting up the PDP at https://docs.permit.io/sdk/python/quickstart-python/#2-setup-your-pdp-policy-decision-point-container"
+                )
+
     async def bulk_check(
         self,
         checks: list[CheckQuery],
         context: Context = {},
     ) -> list[bool]:
         """
         Checks if a user is authorized to perform an action on a resource within the specified context.
@@ -108,15 +219,17 @@
                     user=normalized_user.dict(exclude_unset=True),
                     action=check["action"],
                     resource=normalized_resource.dict(exclude_unset=True),
                     context=query_context,
                 )
             )
 
-        async with aiohttp.ClientSession(headers=self._headers) as session:
+        async with aiohttp.ClientSession(
+            headers=self._headers, **self._timeout_config
+        ) as session:
             check_url = f"{self._base_url}/allowed/bulk"
             try:
                 async with session.post(
                     check_url,
                     data=json.dumps(input),
                 ) as response:
                     if response.status != 200:
@@ -215,16 +328,17 @@
         query_context = self._context_store.get_derived_context(context)
         input = dict(
             user=normalized_user.dict(exclude_unset=True),
             action=action,
             resource=normalized_resource.dict(exclude_unset=True),
             context=query_context,
         )
-
-        async with aiohttp.ClientSession(headers=self._headers) as session:
+        async with aiohttp.ClientSession(
+            headers=self._headers, **self._timeout_config
+        ) as session:
             check_url = f"{self._base_url}/allowed"
             try:
                 async with session.post(
                     check_url,
                     data=json.dumps(input),
                 ) as response:
                     if response.status != 200:
```

### Comparing `permit-2.4.3/permit/exceptions.py` & `permit-2.5.0/permit/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         # handle non-json errors (can be returned by load balancer)
         content_type = response.headers.get("content-type")
         if content_type is not None and content_type.lower() != "application/json":
             error_string = await response.text()
             raise PermitApiError(
                 f"{response.status} API Error",
                 response,
-                json={"status_code": response.status, "error": error_string},
+                {"status_code": response.status, "error": error_string},
             )
 
         # fallback to handle json errors
         json = await response.json()
         raise PermitApiError(f"{response.status} API error", response, json)
```

### Comparing `permit-2.4.3/permit/pdp_api/base.py` & `permit-2.5.0/permit/pdp_api/base.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/pdp_api/models.py` & `permit-2.5.0/permit/pdp_api/models.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/pdp_api/pdp_api_client.py` & `permit-2.5.0/permit/pdp_api/pdp_api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/pdp_api/role_assignments.py` & `permit-2.5.0/permit/pdp_api/role_assignments.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/permit.py` & `permit-2.5.0/permit/sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,71 @@
-import json
 from typing import Optional
 
-from loguru import logger
-
-from .api.api_client import PermitApiClient
-from .api.elements import ElementsApi
+from .api.elements import SyncElementsApi
+from .api.sync_api_client import SyncPermitApiClient
 from .config import PermitConfig
-from .enforcement.enforcer import Action, CheckQuery, Enforcer, Resource, User
-from .logger import configure_logger
-from .pdp_api.pdp_api_client import PermitPdpApiClient
+from .enforcement.enforcer import Action, CheckQuery, Resource, SyncEnforcer, User
+from .pdp_api.pdp_api_client import SyncPDPApi
+from .permit import Permit as AsyncPermit
 from .utils.context import Context
 
 
-class Permit:
+class Permit(AsyncPermit):
     def __init__(self, config: Optional[PermitConfig] = None, **options):
-        self._config: PermitConfig = (
-            config if config is not None else PermitConfig(**options)
-        )
-
-        configure_logger(self._config)
-        self._enforcer = Enforcer(self._config)
-        self._api = PermitApiClient(self._config)
-        self._elements = ElementsApi(self._config)
-        self._pdp_api = PermitPdpApiClient(self._config)
-        logger.debug(
-            "Permit SDK initialized with config:\n${}",
-            json.dumps(self._config.dict(exclude={"api_context"})),
-        )
-
-    @property
-    def config(self):
-        """
-        Access the SDK configuration using this property.
-        Once the SDK is initialized, the configuration is read-only.
-
-        Usage example:
-
-            permit = Permit(config)
-            pdp_url = permit.config.pdp
-        """
-        return self._config.copy()
+        super().__init__(config, **options)
+        self._enforcer = SyncEnforcer(self._config)
+        self._api = SyncPermitApiClient(self._config)
+        self._elements = SyncElementsApi(self._config)
+        self._pdp_api = SyncPDPApi(self._config)
 
     @property
-    def api(self) -> PermitApiClient:
+    def api(self) -> SyncPermitApiClient:
         """
         Access the Permit REST API using this property.
 
         Usage example:
 
             permit = Permit(token="<YOUR_API_KEY>")
-            await permit.api.roles.create(...)
+            permit.api.roles.create(...)
         """
         return self._api
 
     @property
-    def elements(self) -> ElementsApi:
+    def elements(self) -> SyncElementsApi:
         """
         Access the Permit Elements API using this property.
 
         Usage example:
 
             permit = Permit(token="<YOUR_API_KEY>")
-            await permit.elements.loginAs(user, tenant)
+            permit.elements.loginAs(user, tenant)
         """
         return self._elements
 
     @property
-    def pdp_api(self) -> PermitPdpApiClient:
+    def pdp_api(self) -> SyncPDPApi:
         """
         Access the Permit PDP API using this property.
 
         Usage example:
-
-            permit = Permit(token="<YOUR_API_KEY>")
-            await permit.pdp_api.role_assignments.list()
+        permit = Permit(token="<YOUR_API_KEY>")
+        permit.pdp_api.role_assignments(...)
         """
         return self._pdp_api
 
-    async def bulk_check(
+    def bulk_check(
         self,
         checks: list[CheckQuery],
         context: Context = {},
     ) -> list[bool]:
         """
         Checks if a user is authorized to perform an action on a list of resources within the specified context.
 
         Args:
-            checks: A list of check queries, each query contain user, action, and resource.
+            checks: A list of CheckQuery objects representing the authorization checks to be performed.
             context: The context object representing the context in which the action is performed. Defaults to None.
 
         Returns:
             list[bool]: A list of booleans indicating whether the user is authorized for each resource.
 
         Raises:
             PermitConnectionError: If an error occurs while sending the authorization request to the PDP.
@@ -112,17 +87,17 @@
                 {
                     "user": "user_a",
                     "action": "close",
                     "resource": "issue",
                 },
             ])
         """
-        return await self._enforcer.bulk_check(checks, context)
+        return self._enforcer.bulk_check(checks, context)
 
-    async def check(
+    def check(
         self,
         user: User,
         action: Action,
         resource: Resource,
         context: Context = {},
     ) -> bool:
         """
@@ -139,17 +114,17 @@
 
         Raises:
             PermitConnectionError: If an error occurs while sending the authorization request to the PDP.
 
         Examples:
 
             # can the user close any issue?
-            await permit.check(user, 'close', 'issue')
+            permit.check(user, 'close', 'issue')
 
             # can the user close any issue who's id is 1234?
-            await permit.check(user, 'close', 'issue:1234')
+            permit.check(user, 'close', 'issue:1234')
 
             # can the user close (any) issues belonging to the 't1' tenant?
             # (in a multi tenant application)
-            await permit.check(user, 'close', {'type': 'issue', 'tenant': 't1'})
+            permit.check(user, 'close', {'type': 'issue', 'tenant': 't1'})
         """
-        return await self._enforcer.check(user, action, resource, context)
+        return self._enforcer.check(user, action, resource, context)
```

### Comparing `permit-2.4.3/permit/sync.py` & `permit-2.5.0/permit/permit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,137 @@
+import json
 from typing import Optional
 
-from .api.elements import SyncElementsApi
-from .api.sync_api_client import SyncPermitApiClient
+from loguru import logger
+
+from .api.api_client import PermitApiClient
+from .api.elements import ElementsApi
 from .config import PermitConfig
-from .enforcement.enforcer import Action, CheckQuery, Resource, SyncEnforcer, User
-from .pdp_api.pdp_api_client import SyncPDPApi
-from .permit import Permit as AsyncPermit
+from .enforcement.enforcer import (
+    Action,
+    AuthorizedUsersResult,
+    CheckQuery,
+    Enforcer,
+    Resource,
+    User,
+)
+from .logger import configure_logger
+from .pdp_api.pdp_api_client import PermitPdpApiClient
 from .utils.context import Context
 
 
-class Permit(AsyncPermit):
+class Permit:
     def __init__(self, config: Optional[PermitConfig] = None, **options):
-        super().__init__(config, **options)
-        self._enforcer = SyncEnforcer(self._config)
-        self._api = SyncPermitApiClient(self._config)
-        self._elements = SyncElementsApi(self._config)
-        self._pdp_api = SyncPDPApi(self._config)
+        self._config: PermitConfig = (
+            config if config is not None else PermitConfig(**options)
+        )
+
+        configure_logger(self._config)
+        self._enforcer = Enforcer(self._config)
+        self._api = PermitApiClient(self._config)
+        self._elements = ElementsApi(self._config)
+        self._pdp_api = PermitPdpApiClient(self._config)
+        logger.debug(
+            "Permit SDK initialized with config:\n${}",
+            json.dumps(self._config.dict(exclude={"api_context"})),
+        )
 
     @property
-    def api(self) -> SyncPermitApiClient:
+    def config(self):
+        """
+        Access the SDK configuration using this property.
+        Once the SDK is initialized, the configuration is read-only.
+
+        Usage example:
+
+            permit = Permit(config)
+            pdp_url = permit.config.pdp
+        """
+        return self._config.copy()
+
+    @property
+    def api(self) -> PermitApiClient:
         """
         Access the Permit REST API using this property.
 
         Usage example:
 
             permit = Permit(token="<YOUR_API_KEY>")
-            permit.api.roles.create(...)
+            await permit.api.roles.create(...)
         """
         return self._api
 
     @property
-    def elements(self) -> SyncElementsApi:
+    def elements(self) -> ElementsApi:
         """
         Access the Permit Elements API using this property.
 
         Usage example:
 
             permit = Permit(token="<YOUR_API_KEY>")
-            permit.elements.loginAs(user, tenant)
+            await permit.elements.loginAs(user, tenant)
         """
         return self._elements
 
     @property
-    def pdp_api(self) -> SyncPDPApi:
+    def pdp_api(self) -> PermitPdpApiClient:
         """
         Access the Permit PDP API using this property.
 
         Usage example:
-        permit = Permit(token="<YOUR_API_KEY>")
-        permit.pdp_api.role_assignments(...)
+
+            permit = Permit(token="<YOUR_API_KEY>")
+            await permit.pdp_api.role_assignments.list()
         """
         return self._pdp_api
 
-    def bulk_check(
+    async def authorized_users(
+        self,
+        action: Action,
+        resource: Resource,
+        context: Context = {},
+    ) -> AuthorizedUsersResult:
+        """
+        Queries to get all the users that are authorized to perform an action on a resource within the specified context.
+
+        Args:
+            action: The action to be performed on the resource.
+            resource: The resource object representing the resource.
+            context: The context object representing the context in which the action is performed. Defaults to None.
+
+        Returns:
+            AuthorizedUsersResult: Contains all the authorized users and the role assignments that granted the permission.
+
+        Raises:
+            PermitConnectionError: If an error occurs while sending the authorization request to the PDP.
+
+        Examples:
+
+            # all the users that can close any issue?
+            await permit.authorized_users('close', 'issue')
+
+            # all the users that can close an issue who's id is 1234?
+            await permit.authorized_users('close', 'issue:1234')
+
+            # all the users that can close (any) issues belonging to the 't1' tenant?
+            # (in a multi tenant application)
+            await permit.authorized_users('close', {'type': 'issue', 'tenant': 't1'})
+        """
+        return await self._enforcer.authorized_users(action, resource, context)
+
+    async def bulk_check(
         self,
         checks: list[CheckQuery],
         context: Context = {},
     ) -> list[bool]:
         """
         Checks if a user is authorized to perform an action on a list of resources within the specified context.
 
         Args:
-            checks: A list of CheckQuery objects representing the authorization checks to be performed.
+            checks: A list of check queries, each query contain user, action, and resource.
             context: The context object representing the context in which the action is performed. Defaults to None.
 
         Returns:
             list[bool]: A list of booleans indicating whether the user is authorized for each resource.
 
         Raises:
             PermitConnectionError: If an error occurs while sending the authorization request to the PDP.
@@ -87,17 +153,17 @@
                 {
                     "user": "user_a",
                     "action": "close",
                     "resource": "issue",
                 },
             ])
         """
-        return self._enforcer.bulk_check(checks, context)
+        return await self._enforcer.bulk_check(checks, context)
 
-    def check(
+    async def check(
         self,
         user: User,
         action: Action,
         resource: Resource,
         context: Context = {},
     ) -> bool:
         """
@@ -114,17 +180,17 @@
 
         Raises:
             PermitConnectionError: If an error occurs while sending the authorization request to the PDP.
 
         Examples:
 
             # can the user close any issue?
-            permit.check(user, 'close', 'issue')
+            await permit.check(user, 'close', 'issue')
 
             # can the user close any issue who's id is 1234?
-            permit.check(user, 'close', 'issue:1234')
+            await permit.check(user, 'close', 'issue:1234')
 
             # can the user close (any) issues belonging to the 't1' tenant?
             # (in a multi tenant application)
-            permit.check(user, 'close', {'type': 'issue', 'tenant': 't1'})
+            await permit.check(user, 'close', {'type': 'issue', 'tenant': 't1'})
         """
-        return self._enforcer.check(user, action, resource, context)
+        return await self._enforcer.check(user, action, resource, context)
```

### Comparing `permit-2.4.3/permit/utils/context.py` & `permit-2.5.0/permit/utils/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/utils/deprecation.py` & `permit-2.5.0/permit/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit/utils/sync.py` & `permit-2.5.0/permit/utils/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/permit.egg-info/PKG-INFO` & `permit-2.5.0/permit.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permit
-Version: 2.4.3
+Version: 2.5.0
 Summary: Permit.io python sdk
 Author: Asaf Cohen
 Author-email: asaf@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `permit-2.4.3/permit.egg-info/SOURCES.txt` & `permit-2.5.0/permit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/setup.py` & `permit-2.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     this_directory = Path(__file__).parent
     long_description = (this_directory / "README.md").read_text()
     return long_description
 
 
 setup(
     name="permit",
-    version="v2.4.3",
+    version="2.5.0",
     packages=find_packages(),
     author="Asaf Cohen",
     author_email="asaf@permit.io",
     license="Apache 2.0",
     python_requires=">=3.8",
     description="Permit.io python sdk",
     install_requires=get_requirements(),
```

### Comparing `permit-2.4.3/tests/conftest.py` & `permit-2.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/tests/test_abac_e2e.py` & `permit-2.5.0/tests/test_abac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/tests/test_abac_pdp.py` & `permit-2.5.0/tests/test_abac_pdp.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.3/tests/test_rbac_e2e.py` & `permit-2.5.0/tests/test_rbac_e2e_sync.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import time
 from typing import List
 
 import pytest
 from loguru import logger
 
-from permit import Permit, RoleAssignmentRead
+from permit import RoleAssignmentRead
 from permit.exceptions import PermitApiError, PermitConnectionError
 from permit.pdp_api.models import RoleAssignment
+from permit.sync import Permit as SyncPermit
 
 from .utils import handle_api_error
 
 
 def print_break():
     print("\n\n ----------- \n\n")
 
 
-async def test_permission_check_e2e(permit: Permit):
+def test_permission_check_e2e(sync_permit: SyncPermit):
+    permit = sync_permit
     logger.info("initial setup of objects")
     try:
-        document = await permit.api.resources.create(
+        document = permit.api.resources.create(
             {
                 "key": "document",
                 "name": "Document",
                 "urn": "prn:gdrive:document",
                 "description": "google drive document",
                 "actions": {
                     "create": {},
@@ -49,24 +51,24 @@
         assert len(document.actions or {}) == 4
         assert (document.actions or {}).get("create") is not None
         assert (document.actions or {}).get("read") is not None
         assert (document.actions or {}).get("update") is not None
         assert (document.actions or {}).get("delete") is not None
 
         # verify list output
-        resources = await permit.api.resources.list()
+        resources = permit.api.resources.list()
         assert len(resources) == 1
         assert resources[0].id == document.id
         assert resources[0].key == document.key
         assert resources[0].name == document.name
         assert resources[0].description == document.description
         assert resources[0].urn == document.urn
 
         # create admin role
-        admin = await permit.api.roles.create(
+        admin = permit.api.roles.create(
             {
                 "key": "admin",
                 "name": "Admin",
                 "description": "an admin role",
                 "permissions": ["document:create", "document:read"],
             }
         )
@@ -76,15 +78,15 @@
         assert admin.name == "Admin"
         assert admin.description == "an admin role"
         assert admin.permissions is not None
         assert "document:create" in admin.permissions
         assert "document:read" in admin.permissions
 
         # create viewer role
-        viewer = await permit.api.roles.create(
+        viewer = permit.api.roles.create(
             {
                 "key": "viewer",
                 "name": "Viewer",
                 "description": "an viewer role",
             }
         )
 
@@ -92,39 +94,39 @@
         assert viewer.key == "viewer"
         assert viewer.name == "Viewer"
         assert viewer.description == "an viewer role"
         assert viewer.permissions is not None
         assert len(viewer.permissions) == 0
 
         # assign permissions to roles
-        assigned_viewer = await permit.api.roles.assign_permissions(
+        assigned_viewer = permit.api.roles.assign_permissions(
             "viewer", ["document:read"]
         )
 
         assert assigned_viewer.key == "viewer"
         assert len(assigned_viewer.permissions) == 1
         assert "document:read" in assigned_viewer.permissions
         assert "document:create" not in assigned_viewer.permissions
 
         # create a tenant
-        tenant = await permit.api.tenants.create(
+        tenant = permit.api.tenants.create(
             {
                 "key": "tesla",
                 "name": "Tesla Inc",
                 "description": "The car company",
             }
         )
 
         assert tenant.key == "tesla"
         assert tenant.name == "Tesla Inc"
         assert tenant.description == "The car company"
         assert tenant.attributes is None or len(tenant.attributes) == 0
 
         # create a user
-        user = await permit.api.users.sync(
+        user = permit.api.users.sync(
             {
                 "key": "auth0|elon",
                 "email": "elonmusk@tesla.com",
                 "first_name": "Elon",
                 "last_name": "Musk",
                 "attributes": {
                     "age": 50,
@@ -138,15 +140,15 @@
         assert user.first_name == "Elon"
         assert user.last_name == "Musk"
         assert len(user.attributes or {}) == 2
         assert user.attributes["age"] == 50
         assert user.attributes["favoriteColor"] == "red"
 
         # assign role to user in tenant
-        ra = await permit.api.users.assign_role(
+        ra = permit.api.users.assign_role(
             {
                 "user": "auth0|elon",
                 "role": "viewer",
                 "tenant": "tesla",
             }
         )
 
@@ -161,102 +163,97 @@
             "sleeping 2 seconds before permit.check() to make sure all writes propagated from cloud to PDP"
         )
         time.sleep(2)
 
         # positive permission check (will be True because elon is a viewer, and a viewer can read a document)
         logger.info("testing positive permission check")
         resource_attributes = {"secret": True}
-        assert await permit.check(
+        assert permit.check(
             "auth0|elon",
             "read",
             {"type": "document", "tenant": "tesla", "attributes": resource_attributes},
         )
 
         print_break()
 
         logger.info("testing positive permission check with complete user object")
-        assert await permit.check(
+        assert permit.check(
             user.dict(), "read", {"type": document.key, "tenant": tenant.key}
         )
 
         print_break()
 
         # negative permission check (will be False because a viewer cannot create a document)
         logger.info("testing negative permission check")
         assert (
-            await permit.check(
+            permit.check(
                 user.key, "create", {"type": document.key, "tenant": tenant.key}
             )
         ) == False
 
         print_break()
 
-        logger.info("testing bulk permission check")
-        assert (
-            await permit.bulk_check(
-                [
-                    {
-                        "user": "auth0|elon",
-                        "action": "read",
-                        "resource": {
-                            "type": "document",
-                            "tenant": "tesla",
-                            "attributes": resource_attributes,
-                        },
-                    },
-                    {
-                        "user": user.dict(),
-                        "action": "read",
-                        "resource": {"type": document.key, "tenant": tenant.key},
-                    },
-                    {
-                        "user": user.key,
-                        "action": "create",
-                        "resource": {"type": document.key, "tenant": tenant.key},
+        logger.info("testing permissions in bulk")
+        assert permit.bulk_check(
+            [
+                {
+                    "user": "auth0|elon",
+                    "action": "read",
+                    "resource": {
+                        "type": "document",
+                        "tenant": "tesla",
+                        "attributes": resource_attributes,
                     },
-                ],
-                {},
-            )
+                },
+                {
+                    "user": user.dict(),
+                    "action": "read",
+                    "resource": {"type": document.key, "tenant": tenant.key},
+                },
+                {
+                    "user": user.key,
+                    "action": "create",
+                    "resource": {"type": document.key, "tenant": tenant.key},
+                },
+            ]
         ) == [True, True, False]
 
-        print_break()
-
         logger.info("testing list role assignments")
         assignments_returned: List[
             RoleAssignment
-        ] = await permit.pdp_api.role_assignments.list()
+        ] = permit.pdp_api.role_assignments.list()
         assert len(assignments_returned) == 1
         assert assignments_returned[0].user == user.key
         assert assignments_returned[0].role == viewer.key
         assert assignments_returned[0].tenant == tenant.key
         print_break()
 
         logger.info("changing the user roles")
 
         # change the user role - assign admin role
-        await permit.api.users.assign_role(
+        permit.api.users.assign_role(
             {
                 "user": user.key,
                 "role": admin.key,
                 "tenant": tenant.key,
             }
         )
         # change the user role - remove viewer role
-        await permit.api.users.unassign_role(
+        permit.api.users.unassign_role(
             {
                 "user": user.key,
                 "role": viewer.key,
                 "tenant": tenant.key,
             }
         )
 
         # list user roles in all tenants
-        assigned_roles: List[
-            RoleAssignmentRead
-        ] = await permit.api.users.get_assigned_roles(user=user.key)
+        assigned_roles: List[RoleAssignmentRead] = permit.api.users.get_assigned_roles(
+            user=user.key
+        )
 
         assert len(assigned_roles) == 1
         assert assigned_roles[0].user_id == user.id
         assert assigned_roles[0].role_id == admin.id
         assert assigned_roles[0].tenant_id == tenant.id
 
         logger.info(
@@ -264,15 +261,15 @@
         )
         time.sleep(2)
 
         # run the same negative permission check again, this time it's True
         logger.info(
             "testing previously negative permission check, should now be positive"
         )
-        assert await permit.check(
+        assert permit.check(
             user.dict(), "create", {"type": document.key, "tenant": tenant.key}
         )
 
         print_break()
 
     except PermitApiError as error:
         handle_api_error(error, "Got API Error")
@@ -280,23 +277,23 @@
         raise
     except Exception as error:
         logger.error(f"Got error: {error}")
         pytest.fail(f"Got error: {error}")
     finally:
         # cleanup
         try:
-            await permit.api.resources.delete("document")
-            await permit.api.roles.delete("admin")
-            await permit.api.roles.delete("viewer")
-            await permit.api.tenants.delete("tesla")
-            await permit.api.users.delete("auth0|elon")
-            assert len(await permit.api.resources.list()) == 0
-            assert len(await permit.api.roles.list()) == 0
-            assert len(await permit.api.tenants.list()) == 1  # the default tenant
-            assert len((await permit.api.users.list()).data) == 0
+            permit.api.resources.delete("document")
+            permit.api.roles.delete("admin")
+            permit.api.roles.delete("viewer")
+            permit.api.tenants.delete("tesla")
+            permit.api.users.delete("auth0|elon")
+            assert len(permit.api.resources.list()) == 0
+            assert len(permit.api.roles.list()) == 0
+            assert len(permit.api.tenants.list()) == 1  # the default tenant
+            assert len((permit.api.users.list()).data) == 0
         except PermitApiError as error:
             handle_api_error(error, "Got API Error during cleanup")
         except PermitConnectionError as error:
             raise
         except Exception as error:
             logger.error(f"Got error during cleanup: {error}")
             pytest.fail(f"Got error during cleanup: {error}")
```

### Comparing `permit-2.4.3/tests/test_rbac_e2e_sync.py` & `permit-2.5.0/tests/test_rbac_e2e.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,91 @@
+import asyncio
 import time
 from typing import List
 
 import pytest
 from loguru import logger
+from pytest_httpserver import HTTPServer
+from werkzeug import Request, Response
 
-from permit import RoleAssignmentRead
+from permit import Permit, RoleAssignmentRead
 from permit.exceptions import PermitApiError, PermitConnectionError
 from permit.pdp_api.models import RoleAssignment
-from permit.sync import Permit as SyncPermit
 
 from .utils import handle_api_error
 
 
 def print_break():
     print("\n\n ----------- \n\n")
 
 
-def test_permission_check_e2e(sync_permit: SyncPermit):
-    permit = sync_permit
+TEST_TIMEOUT = 1
+MOCKED_URL = "http://localhost"
+MOCKED_PORT = 9999
+
+
+def sleeping(request: Request):
+    time.sleep(TEST_TIMEOUT + 1)
+    return Response("OK", status=200)
+
+
+@pytest.fixture(scope="session")
+def httpserver_listen_address():
+    return "localhost", MOCKED_PORT
+
+
+async def test_api_timeout(httpserver: HTTPServer):
+    permit = Permit(
+        token="mocked",
+        pdp=f"{MOCKED_URL}:{MOCKED_PORT}",
+        api_url=f"{MOCKED_URL}:{MOCKED_PORT}",
+        api_timeout=TEST_TIMEOUT,
+    )
+    current_time = time.time()
+    httpserver.expect_request("/v2/api-key/scope").respond_with_handler(sleeping)
+    with pytest.raises(asyncio.TimeoutError):
+        await permit.api.roles.list()
+    time_passed = time.time() - current_time
+    assert time_passed < 3
+
+
+async def test_pdp_timeout(httpserver: HTTPServer):
+    permit = Permit(
+        token="mocked",
+        pdp=f"{MOCKED_URL}:{MOCKED_PORT}",
+        api_url=f"{MOCKED_URL}:{MOCKED_PORT}",
+        pdp_timeout=TEST_TIMEOUT,
+    )
+    current_time = time.time()
+    httpserver.expect_request("/allowed").respond_with_handler(sleeping)
+    with pytest.raises(asyncio.TimeoutError):
+        await permit.check("user", "action", {"type": "resource", "tenant": "tenant"})
+    time_passed = time.time() - current_time
+    assert time_passed < 3
+
+    current_time = time.time()
+    httpserver.expect_request("/allowed/bulk").respond_with_handler(sleeping)
+    with pytest.raises(asyncio.TimeoutError):
+        await permit.bulk_check(
+            [
+                {
+                    "user": "user",
+                    "action": "action",
+                    "resource": {"type": "resource", "tenant": "tenant"},
+                }
+            ]
+        )
+    time_passed = time.time() - current_time
+    assert time_passed < 3
+
+
+async def test_permission_check_e2e(permit: Permit):
     logger.info("initial setup of objects")
     try:
-        document = permit.api.resources.create(
+        document = await permit.api.resources.create(
             {
                 "key": "document",
                 "name": "Document",
                 "urn": "prn:gdrive:document",
                 "description": "google drive document",
                 "actions": {
                     "create": {},
@@ -51,24 +112,24 @@
         assert len(document.actions or {}) == 4
         assert (document.actions or {}).get("create") is not None
         assert (document.actions or {}).get("read") is not None
         assert (document.actions or {}).get("update") is not None
         assert (document.actions or {}).get("delete") is not None
 
         # verify list output
-        resources = permit.api.resources.list()
+        resources = await permit.api.resources.list()
         assert len(resources) == 1
         assert resources[0].id == document.id
         assert resources[0].key == document.key
         assert resources[0].name == document.name
         assert resources[0].description == document.description
         assert resources[0].urn == document.urn
 
         # create admin role
-        admin = permit.api.roles.create(
+        admin = await permit.api.roles.create(
             {
                 "key": "admin",
                 "name": "Admin",
                 "description": "an admin role",
                 "permissions": ["document:create", "document:read"],
             }
         )
@@ -78,15 +139,15 @@
         assert admin.name == "Admin"
         assert admin.description == "an admin role"
         assert admin.permissions is not None
         assert "document:create" in admin.permissions
         assert "document:read" in admin.permissions
 
         # create viewer role
-        viewer = permit.api.roles.create(
+        viewer = await permit.api.roles.create(
             {
                 "key": "viewer",
                 "name": "Viewer",
                 "description": "an viewer role",
             }
         )
 
@@ -94,39 +155,39 @@
         assert viewer.key == "viewer"
         assert viewer.name == "Viewer"
         assert viewer.description == "an viewer role"
         assert viewer.permissions is not None
         assert len(viewer.permissions) == 0
 
         # assign permissions to roles
-        assigned_viewer = permit.api.roles.assign_permissions(
+        assigned_viewer = await permit.api.roles.assign_permissions(
             "viewer", ["document:read"]
         )
 
         assert assigned_viewer.key == "viewer"
         assert len(assigned_viewer.permissions) == 1
         assert "document:read" in assigned_viewer.permissions
         assert "document:create" not in assigned_viewer.permissions
 
         # create a tenant
-        tenant = permit.api.tenants.create(
+        tenant = await permit.api.tenants.create(
             {
                 "key": "tesla",
                 "name": "Tesla Inc",
                 "description": "The car company",
             }
         )
 
         assert tenant.key == "tesla"
         assert tenant.name == "Tesla Inc"
         assert tenant.description == "The car company"
         assert tenant.attributes is None or len(tenant.attributes) == 0
 
         # create a user
-        user = permit.api.users.sync(
+        user = await permit.api.users.sync(
             {
                 "key": "auth0|elon",
                 "email": "elonmusk@tesla.com",
                 "first_name": "Elon",
                 "last_name": "Musk",
                 "attributes": {
                     "age": 50,
@@ -140,15 +201,15 @@
         assert user.first_name == "Elon"
         assert user.last_name == "Musk"
         assert len(user.attributes or {}) == 2
         assert user.attributes["age"] == 50
         assert user.attributes["favoriteColor"] == "red"
 
         # assign role to user in tenant
-        ra = permit.api.users.assign_role(
+        ra = await permit.api.users.assign_role(
             {
                 "user": "auth0|elon",
                 "role": "viewer",
                 "tenant": "tesla",
             }
         )
 
@@ -163,97 +224,102 @@
             "sleeping 2 seconds before permit.check() to make sure all writes propagated from cloud to PDP"
         )
         time.sleep(2)
 
         # positive permission check (will be True because elon is a viewer, and a viewer can read a document)
         logger.info("testing positive permission check")
         resource_attributes = {"secret": True}
-        assert permit.check(
+        assert await permit.check(
             "auth0|elon",
             "read",
             {"type": "document", "tenant": "tesla", "attributes": resource_attributes},
         )
 
         print_break()
 
         logger.info("testing positive permission check with complete user object")
-        assert permit.check(
+        assert await permit.check(
             user.dict(), "read", {"type": document.key, "tenant": tenant.key}
         )
 
         print_break()
 
         # negative permission check (will be False because a viewer cannot create a document)
         logger.info("testing negative permission check")
         assert (
-            permit.check(
+            await permit.check(
                 user.key, "create", {"type": document.key, "tenant": tenant.key}
             )
         ) == False
 
         print_break()
 
-        logger.info("testing permissions in bulk")
-        assert permit.bulk_check(
-            [
-                {
-                    "user": "auth0|elon",
-                    "action": "read",
-                    "resource": {
-                        "type": "document",
-                        "tenant": "tesla",
-                        "attributes": resource_attributes,
+        logger.info("testing bulk permission check")
+        assert (
+            await permit.bulk_check(
+                [
+                    {
+                        "user": "auth0|elon",
+                        "action": "read",
+                        "resource": {
+                            "type": "document",
+                            "tenant": "tesla",
+                            "attributes": resource_attributes,
+                        },
                     },
-                },
-                {
-                    "user": user.dict(),
-                    "action": "read",
-                    "resource": {"type": document.key, "tenant": tenant.key},
-                },
-                {
-                    "user": user.key,
-                    "action": "create",
-                    "resource": {"type": document.key, "tenant": tenant.key},
-                },
-            ]
+                    {
+                        "user": user.dict(),
+                        "action": "read",
+                        "resource": {"type": document.key, "tenant": tenant.key},
+                    },
+                    {
+                        "user": user.key,
+                        "action": "create",
+                        "resource": {"type": document.key, "tenant": tenant.key},
+                    },
+                ],
+                {},
+            )
         ) == [True, True, False]
 
+        print_break()
+
         logger.info("testing list role assignments")
         assignments_returned: List[
             RoleAssignment
-        ] = permit.pdp_api.role_assignments.list()
+        ] = await permit.pdp_api.role_assignments.list()
         assert len(assignments_returned) == 1
         assert assignments_returned[0].user == user.key
         assert assignments_returned[0].role == viewer.key
         assert assignments_returned[0].tenant == tenant.key
         print_break()
 
         logger.info("changing the user roles")
 
         # change the user role - assign admin role
-        permit.api.users.assign_role(
+        await permit.api.users.assign_role(
             {
                 "user": user.key,
                 "role": admin.key,
                 "tenant": tenant.key,
             }
         )
         # change the user role - remove viewer role
-        permit.api.users.unassign_role(
+        await permit.api.users.unassign_role(
             {
                 "user": user.key,
                 "role": viewer.key,
                 "tenant": tenant.key,
             }
         )
 
         # list user roles in all tenants
-        assigned_roles: List[RoleAssignmentRead] = permit.api.users.get_assigned_roles(
-            user=user.key
-        )
+        assigned_roles: List[
+            RoleAssignmentRead
+        ] = await permit.api.users.get_assigned_roles(user=user.key)
 
         assert len(assigned_roles) == 1
         assert assigned_roles[0].user_id == user.id
         assert assigned_roles[0].role_id == admin.id
         assert assigned_roles[0].tenant_id == tenant.id
 
         logger.info(
@@ -261,39 +327,53 @@
         )
         time.sleep(2)
 
         # run the same negative permission check again, this time it's True
         logger.info(
             "testing previously negative permission check, should now be positive"
         )
-        assert permit.check(
+        assert await permit.check(
             user.dict(), "create", {"type": document.key, "tenant": tenant.key}
         )
 
         print_break()
-
+        logger.info("testing get authorized users")
+        authorized_users = await permit.authorized_users(
+            "create", {"type": document.key, "tenant": tenant.key}
+        )
+        assert authorized_users.tenant == tenant.key
+        assert authorized_users.resource == f"{document.key}:*"
+        assert len(authorized_users.users) == 1
+        assert user.key in authorized_users.users.keys()
+        assignments_authorized = authorized_users.users[user.key]
+        assert len(assignments_authorized) == 1
+        assert assignments_authorized[0].user == user.key
+        assert assignments_authorized[0].role == admin.key
+        assert assignments_authorized[0].tenant == tenant.key
+        assert assignments_authorized[0].resource == f"__tenant:{tenant.key}"
+        print_break()
     except PermitApiError as error:
         handle_api_error(error, "Got API Error")
     except PermitConnectionError as error:
         raise
     except Exception as error:
         logger.error(f"Got error: {error}")
         pytest.fail(f"Got error: {error}")
     finally:
         # cleanup
         try:
-            permit.api.resources.delete("document")
-            permit.api.roles.delete("admin")
-            permit.api.roles.delete("viewer")
-            permit.api.tenants.delete("tesla")
-            permit.api.users.delete("auth0|elon")
-            assert len(permit.api.resources.list()) == 0
-            assert len(permit.api.roles.list()) == 0
-            assert len(permit.api.tenants.list()) == 1  # the default tenant
-            assert len((permit.api.users.list()).data) == 0
+            await permit.api.resources.delete("document")
+            await permit.api.roles.delete("admin")
+            await permit.api.roles.delete("viewer")
+            await permit.api.tenants.delete("tesla")
+            await permit.api.users.delete("auth0|elon")
+            assert len(await permit.api.resources.list()) == 0
+            assert len(await permit.api.roles.list()) == 0
+            assert len(await permit.api.tenants.list()) == 1  # the default tenant
+            assert len((await permit.api.users.list()).data) == 0
         except PermitApiError as error:
             handle_api_error(error, "Got API Error during cleanup")
         except PermitConnectionError as error:
             raise
         except Exception as error:
             logger.error(f"Got error during cleanup: {error}")
             pytest.fail(f"Got error during cleanup: {error}")
```

### Comparing `permit-2.4.3/tests/test_rebac_e2e.py` & `permit-2.5.0/tests/test_rebac_e2e.py`

 * *Files 2% similar despite different names*

```diff
@@ -622,14 +622,39 @@
     logger.info(
         f"asserting: permit.check({q.user}, {q.action}, {str(q.resource)}) === {str(q.expected_decision)}"
     )
     decision = await permit.check(q.user, q.action, q.resource)
     assert q.expected_decision == decision
 
 
+async def assert_permit_authorized_users(
+    permit: Permit, q: CheckAssertion, assignments: list[RoleAssignmentCreate]
+):
+    logger.info(
+        f"asserting: permit.authorized_users({q.action}, {q.resource}) === {q.expected_decision}",
+    )
+    authorized_users = await permit.authorized_users(q.action, q.resource)
+    assert authorized_users.tenant == q.resource["tenant"]
+    assert authorized_users.resource == f"{q.resource['type']}:{q.resource['key']}"
+    if q.expected_decision is True:
+        assert q.user in authorized_users.users.keys()
+        for assignment in authorized_users.users[q.user]:
+            assert any(
+                (
+                    assignment.role.split("#")[1] == created_assignment.role
+                    and assignment.tenant == created_assignment.tenant
+                    and assignment.user == created_assignment.user
+                    and assignment.resource == created_assignment.resource_instance
+                )
+                for created_assignment in assignments
+            )
+    else:
+        assert q.user not in authorized_users.users.keys()
+
+
 async def test_rebac_policy(permit: Permit):
     logger.info("initial setup of objects")
     await cleanup(permit)
     try:
         # schema --------------------------------------------------------------
 
         # create resources
@@ -812,14 +837,17 @@
 
                 for assertion in test_step.assertions:
                     if assertion.pre_assertion_hook is not None:
                         logger.debug("executing pre assertion hook")
                         await assertion.pre_assertion_hook(permit)
                         await asyncio.sleep(1)
                     await assert_permit_check(permit, assertion)
+                    await assert_permit_authorized_users(
+                        permit, assertion, test_step.assignments
+                    )
                     if assertion.post_assertion_hook is not None:
                         logger.debug("executing post assertion hook")
                         await assertion.post_assertion_hook(permit)
                         await asyncio.sleep(1)
             finally:
                 for assignment in test_step.assignments:
                     try:
```

