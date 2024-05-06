# Comparing `tmp/collective.volto.gdprcookie-1.0.2.tar.gz` & `tmp/collective.volto.gdprcookie-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.volto.gdprcookie-1.0.2.tar", last modified: Mon Mar 25 11:44:11 2024, max compression
+gzip compressed data, was "collective.volto.gdprcookie-1.0.3.tar", last modified: Mon May  6 10:13:04 2024, max compression
```

## Comparing `collective.volto.gdprcookie-1.0.2.tar` & `collective.volto.gdprcookie-1.0.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.509473 collective.volto.gdprcookie-1.0.2/
--rw-r--r--   0 cekk       (501) staff       (20)      316 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       73 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1338 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      678 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      154 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     4881 2024-03-25 11:44:11.509372 collective.volto.gdprcookie-1.0.2/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3264 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)     5222 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/pyproject.toml
--rw-r--r--   0 cekk       (501) staff       (20)       38 2024-03-25 11:44:11.509506 collective.volto.gdprcookie-1.0.2/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2624 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.502323 collective.volto.gdprcookie-1.0.2/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.504225 collective.volto.gdprcookie-1.0.2/src/collective/
--rw-r--r--   0 cekk       (501) staff       (20)       56 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.505220 collective.volto.gdprcookie-1.0.2/src/collective/volto/
--rw-r--r--   0 cekk       (501) staff       (20)       56 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.506048 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/
--rw-r--r--   0 cekk       (501) staff       (20)      120 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.506374 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      541 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      438 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/browser/controlpanel.py
--rw-r--r--   0 cekk       (501) staff       (20)    24088 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/config.py
--rw-r--r--   0 cekk       (501) staff       (20)     1466 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     2385 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.506909 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2971 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/collective.volto.gdprcookie.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.502699 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.507134 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      458 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/en/LC_MESSAGES/collective.volto.gdprcookie.mo
--rw-r--r--   0 cekk       (501) staff       (20)     2841 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/en/LC_MESSAGES/collective.volto.gdprcookie.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.502807 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.507361 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     2578 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/it/LC_MESSAGES/collective.volto.gdprcookie.mo
--rw-r--r--   0 cekk       (501) staff       (20)     4308 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/it/LC_MESSAGES/collective.volto.gdprcookie.po
--rw-r--r--   0 cekk       (501) staff       (20)     1801 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      518 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      374 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.503045 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.507933 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      199 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      122 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      660 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      195 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/profiles/default/metadata.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.508042 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/profiles/default/registry/
--rw-r--r--   0 cekk       (501) staff       (20)      252 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/profiles/default/registry/main.xml
--rw-r--r--   0 cekk       (501) staff       (20)      289 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.508159 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      130 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.508798 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)     1785 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1301 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      711 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/controlpanel.py
--rw-r--r--   0 cekk       (501) staff       (20)     1825 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/deserializer.py
--rw-r--r--   0 cekk       (501) staff       (20)     2632 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/get.py
--rw-r--r--   0 cekk       (501) staff       (20)     1051 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/serializer.py
--rw-r--r--   0 cekk       (501) staff       (20)      772 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     1246 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.509212 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1923 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/tests/test_controlpanel_api.py
--rw-r--r--   0 cekk       (501) staff       (20)     1903 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/tests/test_expander.py
--rw-r--r--   0 cekk       (501) staff       (20)     3009 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/tests/test_get_gdpr_settings.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-25 11:44:11.505111 collective.volto.gdprcookie-1.0.2/src/collective.volto.gdprcookie.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     4881 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective.volto.gdprcookie.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2726 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective.volto.gdprcookie.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective.volto.gdprcookie.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      132 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective.volto.gdprcookie.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       28 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective.volto.gdprcookie.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective.volto.gdprcookie.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      221 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective.volto.gdprcookie.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2024-03-25 11:44:11.000000 collective.volto.gdprcookie-1.0.2/src/collective.volto.gdprcookie.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.582921 collective.volto.gdprcookie-1.0.3/
+-rw-r--r--   0 cekk       (501) staff       (20)      416 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       73 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     1338 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      678 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      154 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     4981 2024-05-06 10:13:04.582811 collective.volto.gdprcookie-1.0.3/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3264 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     5222 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/pyproject.toml
+-rw-r--r--   0 cekk       (501) staff       (20)       38 2024-05-06 10:13:04.582953 collective.volto.gdprcookie-1.0.3/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2624 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.575268 collective.volto.gdprcookie-1.0.3/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.577449 collective.volto.gdprcookie-1.0.3/src/collective/
+-rw-r--r--   0 cekk       (501) staff       (20)       56 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.578633 collective.volto.gdprcookie-1.0.3/src/collective/volto/
+-rw-r--r--   0 cekk       (501) staff       (20)       56 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.579520 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/
+-rw-r--r--   0 cekk       (501) staff       (20)      120 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.579830 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      541 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      438 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/browser/controlpanel.py
+-rw-r--r--   0 cekk       (501) staff       (20)    24088 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/config.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1466 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2385 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.580350 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2971 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/collective.volto.gdprcookie.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.575664 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.580576 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      458 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/en/LC_MESSAGES/collective.volto.gdprcookie.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     2841 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/en/LC_MESSAGES/collective.volto.gdprcookie.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.575791 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.580801 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     2578 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/it/LC_MESSAGES/collective.volto.gdprcookie.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     4308 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/it/LC_MESSAGES/collective.volto.gdprcookie.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1801 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      518 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      374 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.576068 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.581354 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      199 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      122 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      660 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      195 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/profiles/default/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.581467 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/profiles/default/registry/
+-rw-r--r--   0 cekk       (501) staff       (20)      252 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/profiles/default/registry/main.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      289 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.581574 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      130 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.582224 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)     1785 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1301 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      711 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/controlpanel.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1853 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/deserializer.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2632 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1051 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/serializer.py
+-rw-r--r--   0 cekk       (501) staff       (20)      772 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1246 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.582640 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1923 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/tests/test_controlpanel_api.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1903 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/tests/test_expander.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3009 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/tests/test_get_gdpr_settings.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-06 10:13:04.578501 collective.volto.gdprcookie-1.0.3/src/collective.volto.gdprcookie.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     4981 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective.volto.gdprcookie.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2726 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective.volto.gdprcookie.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective.volto.gdprcookie.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      132 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective.volto.gdprcookie.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       28 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective.volto.gdprcookie.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective.volto.gdprcookie.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      221 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective.volto.gdprcookie.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2024-05-06 10:13:04.000000 collective.volto.gdprcookie-1.0.3/src/collective.volto.gdprcookie.egg-info/top_level.txt
```

### Comparing `collective.volto.gdprcookie-1.0.2/DEVELOP.rst` & `collective.volto.gdprcookie-1.0.3/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/LICENSE.GPL` & `collective.volto.gdprcookie-1.0.3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/LICENSE.rst` & `collective.volto.gdprcookie-1.0.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/PKG-INFO` & `collective.volto.gdprcookie-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.volto.gdprcookie
-Version: 1.0.2
+Version: 1.0.3
 Summary: Add-on for Plone to manage cookie settings for GDPR in Volto
 Home-page: https://github.com/collective/collective.volto.gdprcookie
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.volto.gdprcookie/
 Project-URL: Source, https://github.com/collective/collective.volto.gdprcookie
@@ -131,14 +131,21 @@
 - RedTurtle Technology, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
 
+1.0.3 (2024-05-06)
+------------------
+
+- Fix deserializer and save all data in registry.
+  [cekk]
+
+
 1.0.2 (2024-03-25)
 ------------------
 
 - Fix serializer code.
   [cekk]
```

### Comparing `collective.volto.gdprcookie-1.0.2/README.rst` & `collective.volto.gdprcookie-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/pyproject.toml` & `collective.volto.gdprcookie-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/setup.py` & `collective.volto.gdprcookie-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.volto.gdprcookie",
-    version="1.0.2",
+    version="1.0.3",
     description="Add-on for Plone to manage cookie settings for GDPR in Volto",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/browser/configure.zcml` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/config.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/config.py`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/configure.zcml` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/interfaces.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/README.rst` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/collective.volto.gdprcookie.pot` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/collective.volto.gdprcookie.pot`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/en/LC_MESSAGES/collective.volto.gdprcookie.po` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/en/LC_MESSAGES/collective.volto.gdprcookie.po`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/it/LC_MESSAGES/collective.volto.gdprcookie.mo` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/it/LC_MESSAGES/collective.volto.gdprcookie.mo`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/it/LC_MESSAGES/collective.volto.gdprcookie.po` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/it/LC_MESSAGES/collective.volto.gdprcookie.po`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/update.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/locales/update.sh` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/profiles/default/controlpanel.xml` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/__init__.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/configure.zcml` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/controlpanel.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/deserializer.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/deserializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 @implementer(IDeserializeFromJson)
 @adapter(IGDPRCookieSettingsControlpanel)
 class GDPRCookieSettingsDeserializeFromJson(ControlpanelDeserializeFromJson):
     def __call__(self):
         """
         Convert json data into a string
         """
+        super().__call__()
+
         req = json_body(self.controlpanel.request)
         proxy = self.registry.forInterface(self.schema, prefix=self.schema_prefix)
         errors = []
 
         gdpr_cookie_settings = req.get("gdpr_cookie_settings", {})
         if not gdpr_cookie_settings:
             errors.append(
```

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/get.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/get.py`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/restapi/serializer.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/restapi/serializer.py`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/setuphandlers.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/testing.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/testing.py`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/tests/test_controlpanel_api.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/tests/test_controlpanel_api.py`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/tests/test_expander.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/tests/test_expander.py`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective/volto/gdprcookie/tests/test_get_gdpr_settings.py` & `collective.volto.gdprcookie-1.0.3/src/collective/volto/gdprcookie/tests/test_get_gdpr_settings.py`

 * *Files identical despite different names*

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective.volto.gdprcookie.egg-info/PKG-INFO` & `collective.volto.gdprcookie-1.0.3/src/collective.volto.gdprcookie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.volto.gdprcookie
-Version: 1.0.2
+Version: 1.0.3
 Summary: Add-on for Plone to manage cookie settings for GDPR in Volto
 Home-page: https://github.com/collective/collective.volto.gdprcookie
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.volto.gdprcookie/
 Project-URL: Source, https://github.com/collective/collective.volto.gdprcookie
@@ -131,14 +131,21 @@
 - RedTurtle Technology, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
 
+1.0.3 (2024-05-06)
+------------------
+
+- Fix deserializer and save all data in registry.
+  [cekk]
+
+
 1.0.2 (2024-03-25)
 ------------------
 
 - Fix serializer code.
   [cekk]
```

### Comparing `collective.volto.gdprcookie-1.0.2/src/collective.volto.gdprcookie.egg-info/SOURCES.txt` & `collective.volto.gdprcookie-1.0.3/src/collective.volto.gdprcookie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

