# Comparing `tmp/collective.campaignmonitor-1.3.tar.gz` & `tmp/collective_campaignmonitor-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.campaignmonitor-1.3.tar", last modified: Mon Oct 25 14:30:55 2021, max compression
+gzip compressed data, was "collective_campaignmonitor-1.4.tar", last modified: Mon May  6 12:34:27 2024, max compression
```

## Comparing `collective.campaignmonitor-1.3.tar` & `collective_campaignmonitor-1.4.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.574130 collective.campaignmonitor-1.3/
--rw-rw-r--   0 erral     (1000) erral     (1000)     1926 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/.gitlab-ci.yml
--rw-rw-r--   0 erral     (1000) erral     (1000)     1517 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/.travis.yml
--rw-rw-r--   0 erral     (1000) erral     (1000)      942 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/CHANGES.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)       74 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/CONTRIBUTORS.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)      568 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/DEVELOP.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)    18092 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/LICENSE.GPL
--rw-rw-r--   0 erral     (1000) erral     (1000)      673 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/LICENSE.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)      125 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/MANIFEST.in
--rw-rw-r--   0 erral     (1000) erral     (1000)     5050 2021-10-25 14:30:55.574130 collective.campaignmonitor-1.3/PKG-INFO
--rw-rw-r--   0 erral     (1000) erral     (1000)     1962 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/README.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)       27 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/constraints.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)      105 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/constraints_plone51.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)      105 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/constraints_plone52.txt
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.570130 collective.campaignmonitor-1.3/docs/
--rw-rw-r--   0 erral     (1000) erral     (1000)     7937 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/docs/conf.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      101 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/docs/index.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)       50 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/requirements.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)      386 2021-10-25 14:30:55.574130 collective.campaignmonitor-1.3/setup.cfg
--rw-rw-r--   0 erral     (1000) erral     (1000)     2489 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/setup.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.566130 collective.campaignmonitor-1.3/src/
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.570130 collective.campaignmonitor-1.3/src/collective/
--rw-rw-r--   0 erral     (1000) erral     (1000)       80 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/__init__.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.570130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/
--rw-rw-r--   0 erral     (1000) erral     (1000)      143 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/__init__.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.570130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/browser/
--rw-rw-r--   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/browser/__init__.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      810 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/browser/configure.zcml
--rw-rw-r--   0 erral     (1000) erral     (1000)     1924 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/browser/controlpanel.pt
--rw-rw-r--   0 erral     (1000) erral     (1000)     1978 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/browser/controlpanel.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.570130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/browser/static/
--rw-rw-r--   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/browser/static/.gitkeep
--rw-rw-r--   0 erral     (1000) erral     (1000)     2939 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/browser/subscription.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     1716 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/configure.zcml
--rw-rw-r--   0 erral     (1000) erral     (1000)     4338 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/connection.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     2909 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/interfaces.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.570130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/
--rw-rw-r--   0 erral     (1000) erral     (1000)      611 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/README.rst
--rw-rw-r--   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/__init__.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     3089 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/collective.campaignmonitor.pot
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.566130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/en/
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.570130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/en/LC_MESSAGES/
--rw-rw-r--   0 erral     (1000) erral     (1000)      458 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/en/LC_MESSAGES/collective.campaignmonitor.mo
--rw-rw-r--   0 erral     (1000) erral     (1000)     2957 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/en/LC_MESSAGES/collective.campaignmonitor.po
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.566130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/es/
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.570130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/es/LC_MESSAGES/
--rw-rw-r--   0 erral     (1000) erral     (1000)     3224 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.mo
--rw-rw-r--   0 erral     (1000) erral     (1000)     4330 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.po
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.566130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/eu/
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.570130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/
--rw-rw-r--   0 erral     (1000) erral     (1000)     3191 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.mo
--rw-rw-r--   0 erral     (1000) erral     (1000)     4297 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.po
--rw-rw-r--   0 erral     (1000) erral     (1000)     1597 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/update.py
--rwxrwxr-x   0 erral     (1000) erral     (1000)      515 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/update.sh
--rw-rw-r--   0 erral     (1000) erral     (1000)      260 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/permissions.zcml
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.566130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.570130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/default/
--rw-rw-r--   0 erral     (1000) erral     (1000)      204 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/default/browserlayer.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      105 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/default/catalog.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      670 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/default/controlpanel.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      195 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/default/metadata.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      633 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/default/registry.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      118 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/default/rolemap.xml
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.570130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/uninstall/
--rw-rw-r--   0 erral     (1000) erral     (1000)      136 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      318 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/uninstall/controlpanel.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      360 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/uninstall/registry.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      682 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/setuphandlers.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     1610 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/testing.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.574130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/tests/
--rw-rw-r--   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/tests/__init__.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     2630 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/tests/test_setup.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      890 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/tests/test_upgrade_step_1001.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     1202 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_clients_vocabulary.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     1196 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_lists_vocabulary.py
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.574130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/upgrades/
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.574130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/upgrades/1001/
--rw-rw-r--   0 erral     (1000) erral     (1000)      626 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/upgrades/1001/registry.xml
--rw-rw-r--   0 erral     (1000) erral     (1000)      784 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/upgrades/1001.zcml
--rw-rw-r--   0 erral     (1000) erral     (1000)       98 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/upgrades/__init__.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      218 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/upgrades/base.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      180 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/upgrades/configure.zcml
--rw-rw-r--   0 erral     (1000) erral     (1000)      228 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/upgrades/v1001.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      218 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/upgrades.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      395 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/upgrades.zcml
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.574130 collective.campaignmonitor-1.3/src/collective/campaignmonitor/vocabularies/
--rw-rw-r--   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/vocabularies/__init__.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     1155 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/vocabularies/campaign_monitor_clients_vocabulary.py
--rw-rw-r--   0 erral     (1000) erral     (1000)     1047 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/vocabularies/campaign_monitor_lists_vocabulary.py
--rw-rw-r--   0 erral     (1000) erral     (1000)      541 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/src/collective/campaignmonitor/vocabularies/configure.zcml
-drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2021-10-25 14:30:55.570130 collective.campaignmonitor-1.3/src/collective.campaignmonitor.egg-info/
--rw-rw-r--   0 erral     (1000) erral     (1000)     5050 2021-10-25 14:30:55.000000 collective.campaignmonitor-1.3/src/collective.campaignmonitor.egg-info/PKG-INFO
--rw-rw-r--   0 erral     (1000) erral     (1000)     3717 2021-10-25 14:30:55.000000 collective.campaignmonitor-1.3/src/collective.campaignmonitor.egg-info/SOURCES.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)        1 2021-10-25 14:30:55.000000 collective.campaignmonitor-1.3/src/collective.campaignmonitor.egg-info/dependency_links.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)      151 2021-10-25 14:30:55.000000 collective.campaignmonitor-1.3/src/collective.campaignmonitor.egg-info/entry_points.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)       11 2021-10-25 14:30:55.000000 collective.campaignmonitor-1.3/src/collective.campaignmonitor.egg-info/namespace_packages.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)        1 2021-10-25 14:30:55.000000 collective.campaignmonitor-1.3/src/collective.campaignmonitor.egg-info/not-zip-safe
--rw-rw-r--   0 erral     (1000) erral     (1000)      155 2021-10-25 14:30:55.000000 collective.campaignmonitor-1.3/src/collective.campaignmonitor.egg-info/requires.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)       11 2021-10-25 14:30:55.000000 collective.campaignmonitor-1.3/src/collective.campaignmonitor.egg-info/top_level.txt
--rw-rw-r--   0 erral     (1000) erral     (1000)     3905 2021-10-25 14:30:48.000000 collective.campaignmonitor-1.3/tox.ini
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.580118 collective_campaignmonitor-1.4/
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1926 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/.gitlab-ci.yml
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1517 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/.travis.yml
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1034 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/CHANGES.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)       74 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/CONTRIBUTORS.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)      568 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/DEVELOP.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)    18092 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/LICENSE.GPL
+-rw-rw-r--   0 erral     (1000) erral     (1000)      673 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/LICENSE.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)      125 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/MANIFEST.in
+-rw-r--r--   0 erral     (1000) erral     (1000)     4459 2024-05-06 12:34:27.580118 collective_campaignmonitor-1.4/PKG-INFO
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1962 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/README.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)       27 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/constraints.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)      105 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/constraints_plone51.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)      105 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/constraints_plone52.txt
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.572117 collective_campaignmonitor-1.4/docs/
+-rw-rw-r--   0 erral     (1000) erral     (1000)     7937 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/docs/conf.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      101 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/docs/index.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)       50 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/requirements.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)      386 2024-05-06 12:34:27.580118 collective_campaignmonitor-1.4/setup.cfg
+-rw-rw-r--   0 erral     (1000) erral     (1000)     2489 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/setup.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.568117 collective_campaignmonitor-1.4/src/
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.572117 collective_campaignmonitor-1.4/src/collective/
+-rw-rw-r--   0 erral     (1000) erral     (1000)       80 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/__init__.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.572117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      143 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/__init__.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.572117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/
+-rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/__init__.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      810 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/configure.zcml
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1924 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/controlpanel.pt
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1978 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/controlpanel.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.572117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/static/
+-rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/static/.gitkeep
+-rw-rw-r--   0 erral     (1000) erral     (1000)     2939 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/subscription.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1716 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/configure.zcml
+-rw-rw-r--   0 erral     (1000) erral     (1000)     5554 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/connection.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     3337 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/interfaces.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.572117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      611 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/README.rst
+-rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/__init__.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     3089 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/collective.campaignmonitor.pot
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.568117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/en/
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      458 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/en/LC_MESSAGES/collective.campaignmonitor.mo
+-rw-rw-r--   0 erral     (1000) erral     (1000)     2957 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/en/LC_MESSAGES/collective.campaignmonitor.po
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.568117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/es/
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 erral     (1000) erral     (1000)     3224 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.mo
+-rw-rw-r--   0 erral     (1000) erral     (1000)     4330 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.po
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.568117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/eu/
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/
+-rw-rw-r--   0 erral     (1000) erral     (1000)     3191 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.mo
+-rw-rw-r--   0 erral     (1000) erral     (1000)     4297 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.po
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1597 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/update.py
+-rwxrwxr-x   0 erral     (1000) erral     (1000)      515 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/update.sh
+-rw-rw-r--   0 erral     (1000) erral     (1000)      260 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/permissions.zcml
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.568117 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      204 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/browserlayer.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      105 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/catalog.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      670 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/controlpanel.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      195 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/metadata.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      633 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/registry.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      118 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/rolemap.xml
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/uninstall/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      136 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      318 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/uninstall/controlpanel.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      360 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/uninstall/registry.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      682 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/setuphandlers.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1610 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/testing.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/
+-rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/__init__.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     2630 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_setup.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      890 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_upgrade_step_1001.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1202 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_clients_vocabulary.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1196 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_lists_vocabulary.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/1001/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      626 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/1001/registry.xml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      784 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/1001.zcml
+-rw-rw-r--   0 erral     (1000) erral     (1000)       98 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/__init__.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      218 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/base.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      180 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/configure.zcml
+-rw-rw-r--   0 erral     (1000) erral     (1000)      228 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/v1001.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      218 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      395 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades.zcml
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/
+-rw-rw-r--   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/__init__.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1155 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/campaign_monitor_clients_vocabulary.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1047 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/campaign_monitor_lists_vocabulary.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)      541 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/configure.zcml
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2024-05-06 12:34:27.576118 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/
+-rw-r--r--   0 erral     (1000) erral     (1000)     4459 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/PKG-INFO
+-rw-rw-r--   0 erral     (1000) erral     (1000)     3717 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/SOURCES.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)        1 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/dependency_links.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)      131 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/entry_points.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)       11 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/namespace_packages.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)        1 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/not-zip-safe
+-rw-rw-r--   0 erral     (1000) erral     (1000)      155 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/requires.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)       11 2024-05-06 12:34:27.000000 collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/top_level.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)     3905 2024-05-06 12:34:25.000000 collective_campaignmonitor-1.4/tox.ini
```

### Comparing `collective.campaignmonitor-1.3/.gitlab-ci.yml` & `collective_campaignmonitor-1.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/.travis.yml` & `collective_campaignmonitor-1.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/CHANGES.rst` & `collective_campaignmonitor-1.4/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.4 (2024-05-06)
+----------------
+
+- Add additional methods to the utility
+  [libargutxi]
+
+
 1.3 (2021-10-25)
 ----------------
 
 - Fix 'Connection Should not load state' errors, with a new strategy to obtain the settings in the utility.
   [erral]
 
 1.2.1 (2020-07-14)
```

### Comparing `collective.campaignmonitor-1.3/DEVELOP.rst` & `collective_campaignmonitor-1.4/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/LICENSE.GPL` & `collective_campaignmonitor-1.4/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/LICENSE.rst` & `collective_campaignmonitor-1.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/README.rst` & `collective_campaignmonitor-1.4/README.rst`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/docs/conf.py` & `collective_campaignmonitor-1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/setup.py` & `collective_campaignmonitor-1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open('CHANGES.rst').read(),
     ]
 )
 
 
 setup(
     name='collective.campaignmonitor',
-    version='1.3',
+    version='1.4',
     description="CampaingMonitor integration for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/browser/configure.zcml` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/browser/controlpanel.pt` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/browser/controlpanel.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/browser/subscription.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/browser/subscription.py`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/configure.zcml` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/connection.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,23 +98,23 @@
     def lists(self):
         registry, settings = self.initialize()
         cache = registry.get(LISTS_CACHE_KEY, _marker)
         if cache and cache is not _marker:
             return cache
         return self._lists()
 
-    def subscribe(self, email, list_id, name=None, resubscribe=False):
+    def subscribe(self, email, list_id, name=None, custom_fields=[], resubscribe=False):
         self.initialize()
         subscriber = Subscriber({"api_key": self.api_key})
         try:
             subscriber.add(
                 list_id=list_id,
                 email_address=email,
                 name=name or email,
-                custom_fields=[],
+                custom_fields=custom_fields,
                 resubscribe=resubscribe,
                 consent_to_track="yes",
             )
             return True
         except BadRequest as e:
             log.info(str(e))
             return False
@@ -130,7 +130,43 @@
         data["ConfirmedOptIn"] = getattr(details, "ConfirmedOptIn", None)
         data["ListID"] = getattr(details, "ListID", None)
         data["Title"] = getattr(details, "Title", None)
         data["UnsubscribePage"] = getattr(details, "UnsubscribePage", None)
         data["UnsubscribeSetting"] = getattr(details, "UnsubscribeSetting", None)
 
         return data
+
+    def get_subscriber(self, list_id, email_address):
+        self.initialize()
+        subscriber = Subscriber({"api_key": self.api_key})
+        try:
+            return subscriber.get(list_id=list_id, email_address=email_address)
+        except BadRequest as e:
+            log.info(str(e))
+            return False
+
+
+    def list_webhooks(self, list_id):
+        self.initialize()
+        cm_list = List({"api_key": self.api_key}, list_id=list_id)
+        return cm_list.webhooks()
+
+
+    def create_list_webhook(self, list_id, events, url, payload_format="json"):
+        self.initialize()
+        cm_list = List({"api_key": self.api_key}, list_id=list_id)
+        try:
+            webhook = cm_list.create_webhook(events, url, payload_format)
+            return True
+        except BadRequest as e:
+            log.info(str(e))
+            return False
+
+    def delete_list_webhook(self, list_id, webhook_id):
+        self.initialize()
+        cm_list = List({"api_key": self.api_key}, list_id=list_id)
+        try:
+            webhook = cm_list.delete_webhook(webhook_id)
+            return True
+        except BadRequest as e:
+            log.info(str(e))
+            return False
```

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/interfaces.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/interfaces.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
     force_resubscribe = schema.Bool(
         title=_("Force resubscription in default form?"),
         description=_(
             u"When adding a new subscriber from the API, Campaign Monitor checks if the user was previously unsubscribed from the list and if so it prevents from adding it. If this option is enabled, this check is bypassed. Be careful when using this option."
         ),
         default=False,
+        required=False,
     )
 
 
 class ICampaignMonitorConnection(Interface):
     def initialize():
         """ Load connection data from registy and prepare for serving results """
 
@@ -55,17 +56,28 @@
 
     def lists():
         """ Return available lists at the campaign monitor account """
 
     def subscribe(email, list_id):
         """ Subscribe 'email' to 'list_id' Campaign Monitor list """
 
+    def get_subscriber(list_id, email):
+        """ Subscribe 'email' to 'list_id' Campaign Monitor list """
+
     def list_details(list_id):
         """ get details about a given list """
 
+    def list_webhooks(list_id):
+        """ get webhooks of a given list """
+
+    def create_list_webhook(list_id, events, url, payload_format):
+        """ create a webhook in a given list """
+
+    def delete_list_webhook(list_id, webhook_id):
+        """ delete a webhook in a given list """
 
 class NotAnEmailAddress(schema.ValidationError):
     __doc__ = _(u"Invalid email address")
 
 
 check_email = re.compile(r"[a-zA-Z0-9._%-]+@([a-zA-Z0-9-]+.)*[a-zA-Z]{2,4}").match
```

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/README.rst` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/collective.campaignmonitor.pot` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/collective.campaignmonitor.pot`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/en/LC_MESSAGES/collective.campaignmonitor.po` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/en/LC_MESSAGES/collective.campaignmonitor.po`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.mo` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.mo`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.po` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/es/LC_MESSAGES/collective.campaignmonitor.po`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.mo` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.mo`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.po` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/eu/LC_MESSAGES/collective.campaignmonitor.po`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/update.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/locales/update.sh` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/default/controlpanel.xml` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/profiles/default/registry.xml` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/setuphandlers.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/testing.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/testing.py`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/tests/test_setup.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/tests/test_upgrade_step_1001.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_upgrade_step_1001.py`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_clients_vocabulary.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_clients_vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_lists_vocabulary.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/tests/test_vocab_campaign_monitor_lists_vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/upgrades/1001/registry.xml` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/1001/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/upgrades/1001.zcml` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/upgrades/1001.zcml`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/vocabularies/campaign_monitor_clients_vocabulary.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/campaign_monitor_clients_vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/vocabularies/campaign_monitor_lists_vocabulary.py` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/campaign_monitor_lists_vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective/campaignmonitor/vocabularies/configure.zcml` & `collective_campaignmonitor-1.4/src/collective/campaignmonitor/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/src/collective.campaignmonitor.egg-info/SOURCES.txt` & `collective_campaignmonitor-1.4/src/collective.campaignmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.campaignmonitor-1.3/tox.ini` & `collective_campaignmonitor-1.4/tox.ini`

 * *Files identical despite different names*

