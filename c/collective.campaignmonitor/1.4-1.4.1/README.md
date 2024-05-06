# Comparing `tmp/collective_campaignmonitor-1.4.tar.gz` & `tmp/collective_campaignmonitor-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective_campaignmonitor-1.4.tar", last modified: Mon May  6 12:34:27 2024, max compression
+gzip compressed data, was "collective_campaignmonitor-1.4.1.tar", last modified: Mon May  6 12:41:22 2024, max compression
```

## Comparing `collective_campaignmonitor-1.4.tar` & `collective_campaignmonitor-1.4.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.580118 collective_campaignmonitor-1.4/
--rw-rw-r--   0 erral     (1000) erral     (1000)     1926 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/.gitlab-ci.yml
--rw-rw-r--   0 erral     (1000) erral     (1000)     1517 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/.travis.yml
--rw-rw-r--   0 erral     (1000) erral     (1000)     1034 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/CHANGES.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)       74 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/CONTRIBUTORS.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)      568 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/DEVELOP.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)    18092 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/LICENSE.GPL
--rw-rw-r--   0 erral     (1000) erral     (1000)      673 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/LICENSE.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)      125 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/MANIFEST.in
--rw-r--r--   0 erral     (1000) erral     (1000)     4459 2024-05-06 12:34:27.580118 collective_campaignmonitor-1.4/PKG-INFO
--rw-rw-r--   0 erral     (1000) erral     (1000)     1962 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/README.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)       27 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/constraints.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)      105 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/constraints_plone51.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)      105 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/constraints_plone52.txt
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.572117 collective_campaignmonitor-1.4/docs/
--rw-rw-r--   0 erral     (1000) erral     (1000)     7937 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/docs/conf.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      101 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/docs/index.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)       50 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/requirements.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)      386 2024-05-06 12:34:27.580118 collective_campaignmonitor-1.4/setup.cfg
--rw-rw-r--   0 erral     (1000) erral     (1000)     2489 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/setup.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.568117 collective_campaignmonitor-1.4/src/
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.572117 collective_campaignmonitor-1.4/src/collective/
--rw-rw-r--   0 erral     (1000) erral     (1000)       80 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/__init__.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.572117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/
--rw-rw-r--   0 erral     (1000) erral     (1000)      143 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/__init__.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.572117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/
--rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/__init__.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      810 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/configure.zcml
--rw-rw-r--   0 erral     (1000) erral     (1000)     1924 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/controlpanel.pt
--rw-rw-r--   0 erral     (1000) erral     (1000)     1978 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/controlpanel.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.572117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/static/
--rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/static/.gitkeep
--rw-rw-r--   0 erral     (1000) erral     (1000)     2939 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/subscription.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     1716 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/configure.zcml
--rw-rw-r--   0 erral     (1000) erral     (1000)     5554 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/connection.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     3337 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/interfaces.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.572117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/
--rw-rw-r--   0 erral     (1000) erral     (1000)      611 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/README.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/__init__.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     3089 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/collective.campaignmonitor.pot
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.568117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/en/
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/en/LC_MESSAGES/
--rw-rw-r--   0 erral     (1000) erral     (1000)      458 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/en/LC_MESSAGES/collective.campaignmonitor.mo
--rw-rw-r--   0 erral     (1000) erral     (1000)     2957 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/en/LC_MESSAGES/collective.campaignmonitor.po
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.568117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/es/
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/es/LC_MESSAGES/
--rw-rw-r--   0 erral     (1000) erral     (1000)     3224 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.mo
--rw-rw-r--   0 erral     (1000) erral     (1000)     4330 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.po
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.568117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/eu/
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/
--rw-rw-r--   0 erral     (1000) erral     (1000)     3191 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.mo
--rw-rw-r--   0 erral     (1000) erral     (1000)     4297 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.po
--rw-rw-r--   0 erral     (1000) erral     (1000)     1597 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/update.py
--rwxrwxr-x   0 erral     (1000) erral     (1000)      515 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/update.sh
--rw-rw-r--   0 erral     (1000) erral     (1000)      260 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/permissions.zcml
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.568117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/
--rw-rw-r--   0 erral     (1000) erral     (1000)      204 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/browserlayer.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      105 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/catalog.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      670 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/controlpanel.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      195 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/metadata.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      633 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/registry.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      118 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/rolemap.xml
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/uninstall/
--rw-rw-r--   0 erral     (1000) erral     (1000)      136 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      318 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/uninstall/controlpanel.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      360 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/uninstall/registry.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      682 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/setuphandlers.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     1610 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/testing.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/
--rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/__init__.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     2630 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_setup.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      890 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_upgrade_step_1001.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     1202 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_clients_vocabulary.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     1196 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_lists_vocabulary.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/1001/
--rw-rw-r--   0 erral     (1000) erral     (1000)      626 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/1001/registry.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      784 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/1001.zcml
--rw-rw-r--   0 erral     (1000) erral     (1000)       98 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/__init__.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      218 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/base.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      180 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/configure.zcml
--rw-rw-r--   0 erral     (1000) erral     (1000)      228 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/v1001.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      218 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      395 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades.zcml
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/
--rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/__init__.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     1155 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/campaign_monitor_clients_vocabulary.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     1047 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/campaign_monitor_lists_vocabulary.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      541 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/configure.zcml
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/
--rw-r--r--   0 erral     (1000) erral     (1000)     4459 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/PKG-INFO
--rw-rw-r--   0 erral     (1000) erral     (1000)     3717 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/SOURCES.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)        1 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/dependency_links.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)      131 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/entry_points.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)       11 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/namespace_packages.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)        1 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/not-zip-safe
--rw-rw-r--   0 erral     (1000) erral     (1000)      155 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/requires.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)       11 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/top_level.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)     3905 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/tox.ini
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.524765 collective_campaignmonitor-1.4.1/
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1926 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/.gitlab-ci.yml
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1517 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/.travis.yml
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1282 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/CHANGES.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)       74 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/CONTRIBUTORS.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)      568 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/DEVELOP.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)    18092 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/LICENSE.GPL
+-rw-rw-r--   0 erral     (1000) erral     (1000)      673 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/LICENSE.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)      125 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/MANIFEST.in
+-rw-r--r--   0 erral     (1000) erral     (1000)     4911 2024-05-06 12:41:22.524765 collective_campaignmonitor-1.4.1/PKG-INFO
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1962 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/README.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)       27 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/constraints.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)      105 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/constraints_plone51.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)      105 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/constraints_plone52.txt
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.516765 collective_campaignmonitor-1.4.1/docs/
+-rw-rw-r--   0 erral     (1000) erral     (1000)     7937 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/docs/conf.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      101 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/docs/index.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)       50 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/requirements.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)      386 2024-05-06 12:41:22.524765 collective_campaignmonitor-1.4.1/setup.cfg
+-rw-rw-r--   0 erral     (1000) erral     (1000)     2689 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/setup.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.512765 collective_campaignmonitor-1.4.1/src/
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.516765 collective_campaignmonitor-1.4.1/src/collective/
+-rw-rw-r--   0 erral     (1000) erral     (1000)       80 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/__init__.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.520765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      143 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/__init__.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.520765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/browser/
+-rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/browser/__init__.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      810 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/browser/configure.zcml
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1924 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/browser/controlpanel.pt
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1978 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/browser/controlpanel.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.520765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/browser/static/
+-rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/browser/static/.gitkeep
+-rw-rw-r--   0 erral     (1000) erral     (1000)     2939 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/browser/subscription.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1716 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/configure.zcml
+-rw-rw-r--   0 erral     (1000) erral     (1000)     5554 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/connection.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     3337 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/interfaces.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.520765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      611 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/README.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/__init__.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     3089 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/collective.campaignmonitor.pot
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.512765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/en/
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.520765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      458 2024-05-06 12:41:22.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/en/LC_MESSAGES/collective.campaignmonitor.mo
+-rw-rw-r--   0 erral     (1000) erral     (1000)     2957 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/en/LC_MESSAGES/collective.campaignmonitor.po
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.512765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/es/
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.520765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 erral     (1000) erral     (1000)     3224 2024-05-06 12:41:22.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.mo
+-rw-rw-r--   0 erral     (1000) erral     (1000)     4330 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.po
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.512765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/eu/
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.520765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/
+-rw-rw-r--   0 erral     (1000) erral     (1000)     3191 2024-05-06 12:41:22.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.mo
+-rw-rw-r--   0 erral     (1000) erral     (1000)     4297 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.po
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1597 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/update.py
+-rwxrwxr-x   0 erral     (1000) erral     (1000)      515 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/update.sh
+-rw-rw-r--   0 erral     (1000) erral     (1000)      260 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/permissions.zcml
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.512765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.520765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/default/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      204 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/default/browserlayer.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      105 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/default/catalog.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      670 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/default/controlpanel.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      195 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/default/metadata.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      633 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/default/registry.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      118 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/default/rolemap.xml
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.520765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/uninstall/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      136 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      318 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/uninstall/controlpanel.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      360 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/uninstall/registry.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      682 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/setuphandlers.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1610 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/testing.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.520765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/tests/
+-rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/tests/__init__.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     2630 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/tests/test_setup.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      890 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/tests/test_upgrade_step_1001.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1202 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_clients_vocabulary.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1196 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_lists_vocabulary.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.524765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/upgrades/
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.524765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/upgrades/1001/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      626 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/upgrades/1001/registry.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      784 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/upgrades/1001.zcml
+-rw-rw-r--   0 erral     (1000) erral     (1000)       98 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/upgrades/__init__.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      218 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/upgrades/base.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      180 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/upgrades/configure.zcml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      228 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/upgrades/v1001.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      218 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/upgrades.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      395 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/upgrades.zcml
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.524765 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/vocabularies/
+-rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/vocabularies/__init__.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1155 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/vocabularies/campaign_monitor_clients_vocabulary.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1047 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/vocabularies/campaign_monitor_lists_vocabulary.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      541 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/vocabularies/configure.zcml
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:41:22.524765 collective_campaignmonitor-1.4.1/src/collective.campaignmonitor.egg-info/
+-rw-r--r--   0 erral     (1000) erral     (1000)     4911 2024-05-06 12:41:22.000000 collective_campaignmonitor-1.4.1/src/collective.campaignmonitor.egg-info/PKG-INFO
+-rw-rw-r--   0 erral     (1000) erral     (1000)     3717 2024-05-06 12:41:22.000000 collective_campaignmonitor-1.4.1/src/collective.campaignmonitor.egg-info/SOURCES.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)        1 2024-05-06 12:41:22.000000 collective_campaignmonitor-1.4.1/src/collective.campaignmonitor.egg-info/dependency_links.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)      131 2024-05-06 12:41:22.000000 collective_campaignmonitor-1.4.1/src/collective.campaignmonitor.egg-info/entry_points.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)       11 2024-05-06 12:41:22.000000 collective_campaignmonitor-1.4.1/src/collective.campaignmonitor.egg-info/namespace_packages.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)        1 2024-05-06 12:41:22.000000 collective_campaignmonitor-1.4.1/src/collective.campaignmonitor.egg-info/not-zip-safe
+-rw-rw-r--   0 erral     (1000) erral     (1000)      155 2024-05-06 12:41:22.000000 collective_campaignmonitor-1.4.1/src/collective.campaignmonitor.egg-info/requires.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)       11 2024-05-06 12:41:22.000000 collective_campaignmonitor-1.4.1/src/collective.campaignmonitor.egg-info/top_level.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)     3905 2024-05-06 12:41:20.000000 collective_campaignmonitor-1.4.1/tox.ini
```

### Comparing `collective_campaignmonitor-1.4/.gitlab-ci.yml` & `collective_campaignmonitor-1.4.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/.travis.yml` & `collective_campaignmonitor-1.4.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/DEVELOP.rst` & `collective_campaignmonitor-1.4.1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/LICENSE.GPL` & `collective_campaignmonitor-1.4.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/LICENSE.rst` & `collective_campaignmonitor-1.4.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/PKG-INFO` & `collective_campaignmonitor-1.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.campaignmonitor
-Version: 1.4
+Version: 1.4.1
 Summary: CampaingMonitor integration for Plone
 Home-page: https://github.com/collective/collective.campaignmonitor
 Author: Mikel Larreategi
 Author-email: mlarreategi@codesyntax.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.campaignmonitor
 Project-URL: Source, https://github.com/collective/collective.campaignmonitor
@@ -14,14 +14,18 @@
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 Requires-Dist: setuptools
 Requires-Dist: plone.api>=1.8.4
 Requires-Dist: createsend<7.0.0,>=6.0.0
@@ -102,14 +106,25 @@
 - Mikel Larreategi, mlarreategi@codesyntax.com
 
 
 Changelog
 =========
 
 
+1.4.1 (2024-05-06)
+------------------
+
+- add new supported python versions [Mikel Larreategi <mlarreategi@codesyntax.com>]
+
+-  [Mikel Larreategi <mlarreategi@codesyntax.com>]
+
+- [ci skip] [Mikel Larreategi <mlarreategi@codesyntax.com>]
+
+  [erral]
+
 1.4 (2024-05-06)
 ----------------
 
 - Add additional methods to the utility
   [libargutxi]
```

### Comparing `collective_campaignmonitor-1.4/README.rst` & `collective_campaignmonitor-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/docs/conf.py` & `collective_campaignmonitor-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/setup.py` & `collective_campaignmonitor-1.4.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,62 +11,66 @@
         open('CONTRIBUTORS.rst').read(),
         open('CHANGES.rst').read(),
     ]
 )
 
 
 setup(
-    name='collective.campaignmonitor',
-    version='1.4',
+    name="collective.campaignmonitor",
+    version="1.4.1",
     description="CampaingMonitor integration for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 5.1",
         "Framework :: Plone :: 5.2",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
-    keywords='Python Plone',
-    author='Mikel Larreategi',
-    author_email='mlarreategi@codesyntax.com',
-    url='https://github.com/collective/collective.campaignmonitor',
+    keywords="Python Plone",
+    author="Mikel Larreategi",
+    author_email="mlarreategi@codesyntax.com",
+    url="https://github.com/collective/collective.campaignmonitor",
     project_urls={
-        'PyPI': 'https://pypi.python.org/pypi/collective.campaignmonitor',
-        'Source': 'https://github.com/collective/collective.campaignmonitor',
-        'Tracker': 'https://github.com/collective/collective.campaignmonitor/issues',
+        "PyPI": "https://pypi.python.org/pypi/collective.campaignmonitor",
+        "Source": "https://github.com/collective/collective.campaignmonitor",
+        "Tracker": "https://github.com/collective/collective.campaignmonitor/issues",
         # 'Documentation': 'https://collective.campaignmonitor.readthedocs.io/en/latest/',
     },
-    license='GPL version 2',
-    packages=find_packages('src', exclude=['ez_setup']),
-    namespace_packages=['collective'],
-    package_dir={'': 'src'},
+    license="GPL version 2",
+    packages=find_packages("src", exclude=["ez_setup"]),
+    namespace_packages=["collective"],
+    package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        'setuptools',
+        "setuptools",
         # -*- Extra requirements: -*-
-        'plone.api>=1.8.4',
-        'createsend>=6.0.0,<7.0.0',
+        "plone.api>=1.8.4",
+        "createsend>=6.0.0,<7.0.0",
     ],
     extras_require={
-        'test': [
-            'plone.app.testing',
+        "test": [
+            "plone.app.testing",
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
             # plone_coredev tests as of 2016-04-01.
-            'plone.testing>=5.0.0',
-            'plone.app.contenttypes',
-            'plone.app.robotframework[debug]',
+            "plone.testing>=5.0.0",
+            "plone.app.contenttypes",
+            "plone.app.robotframework[debug]",
         ]
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     [console_scripts]
     update_locale = collective.campaignmonitor.locales.update:update_locale
```

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/configure.zcml` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/controlpanel.pt` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/browser/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/controlpanel.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/subscription.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/browser/subscription.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/configure.zcml` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/connection.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/connection.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/interfaces.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/README.rst` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/collective.campaignmonitor.pot` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/collective.campaignmonitor.pot`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/en/LC_MESSAGES/collective.campaignmonitor.po` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/en/LC_MESSAGES/collective.campaignmonitor.po`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.mo` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.mo`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.po` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.po`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.mo` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.mo`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.po` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.po`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/update.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/update.sh` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/controlpanel.xml` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/registry.xml` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/setuphandlers.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/testing.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/testing.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_setup.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_upgrade_step_1001.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/tests/test_upgrade_step_1001.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_clients_vocabulary.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_clients_vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_lists_vocabulary.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_lists_vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/1001/registry.xml` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/upgrades/1001/registry.xml`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/1001.zcml` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/upgrades/1001.zcml`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/campaign_monitor_clients_vocabulary.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/vocabularies/campaign_monitor_clients_vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/campaign_monitor_lists_vocabulary.py` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/vocabularies/campaign_monitor_lists_vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/configure.zcml` & `collective_campaignmonitor-1.4.1/src/collective/campaignmonitor/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/PKG-INFO` & `collective_campaignmonitor-1.4.1/src/collective.campaignmonitor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.campaignmonitor
-Version: 1.4
+Version: 1.4.1
 Summary: CampaingMonitor integration for Plone
 Home-page: https://github.com/collective/collective.campaignmonitor
 Author: Mikel Larreategi
 Author-email: mlarreategi@codesyntax.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.campaignmonitor
 Project-URL: Source, https://github.com/collective/collective.campaignmonitor
@@ -14,14 +14,18 @@
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 Requires-Dist: setuptools
 Requires-Dist: plone.api>=1.8.4
 Requires-Dist: createsend<7.0.0,>=6.0.0
@@ -102,14 +106,25 @@
 - Mikel Larreategi, mlarreategi@codesyntax.com
 
 
 Changelog
 =========
 
 
+1.4.1 (2024-05-06)
+------------------
+
+- add new supported python versions [Mikel Larreategi <mlarreategi@codesyntax.com>]
+
+-  [Mikel Larreategi <mlarreategi@codesyntax.com>]
+
+- [ci skip] [Mikel Larreategi <mlarreategi@codesyntax.com>]
+
+  [erral]
+
 1.4 (2024-05-06)
 ----------------
 
 - Add additional methods to the utility
   [libargutxi]
```

### Comparing `collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/SOURCES.txt` & `collective_campaignmonitor-1.4.1/src/collective.campaignmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective_campaignmonitor-1.4/tox.ini` & `collective_campaignmonitor-1.4.1/tox.ini`

 * *Files identical despite different names*

