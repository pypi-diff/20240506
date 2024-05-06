# Comparing `tmp/invenio-records-resources-5.6.0.tar.gz` & `tmp/invenio-records-resources-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-records-resources-5.6.0.tar", last modified: Tue Apr 23 11:25:17 2024, max compression
+gzip compressed data, was "dist/invenio-records-resources-5.7.0.tar", last modified: Mon May  6 18:04:17 2024, max compression
```

## Comparing `invenio-records-resources-5.6.0.tar` & `invenio-records-resources-5.7.0.tar`

### file list

```diff
@@ -1,475 +1,475 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/.github/workflows/tests-feature.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/babel.ini
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/factories/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/factories/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/dumpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/jsonschemas/definitions-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/jsonschemas/definitions-v2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/calculated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/entity_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/files/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/files/field.py
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/files/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/pid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/pid_statuscheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/relations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/references/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/references/entity_resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/references/entity_resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/references/entity_resolvers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/references/entity_resolvers/records.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/references/entity_resolvers/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/references/grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/references/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/files/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/files/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/files/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/files/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/records/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/records/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/resources/records/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/base/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/base/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/base/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/base/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/base/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/base/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/components/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/components/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/components/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/components/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/links.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/processors/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/processors/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/files/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/facets/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/facets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/facets/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/facets/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/facets/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/links.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/querystr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/queryparser/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/queryparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/queryparser/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/queryparser/suggest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/queryparser/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    18663 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/records/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/references/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/references/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/services/uow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 11:25:16.000000 invenio-records-resources-5.6.0/invenio_records_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/requirements-feature.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1277 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/factories/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/factories/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/factories/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/factories/test_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module/jsonschemas/records/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/jsonschemas/records/record-nofiles-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/os-v1/records/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/os-v1/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/os-v2/records/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/os-v2/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/v7/records/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/mappings/v7/records/record-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/jsonschemas/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/jsonschemas/grants/grant-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/os-v1/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/os-v1/grants/grant-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/os-v2/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/os-v2/grants/grant-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/v7/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/v7/grants/grant-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/records/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/records/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/records/test_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13445 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/records/test_systemfield_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/records/test_systemfield_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/records/test_systemfield_modelpid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/records/test_systemfield_pid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/records/test_systemfield_pidstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/resources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    15825 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/resources/test_files_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/resources/test_resource_faceting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/resources/test_resource_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/resources/test_resource_pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/resources/test_resource_preference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/resources/test_resource_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/resources/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/resources/test_resources_etag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/custom_fields/test_base_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/custom_fields/test_boolean_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/custom_fields/test_date_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/custom_fields/test_number_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/custom_fields/test_schema_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/custom_fields/test_text_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/custom_fields/test_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:25:17.000000 invenio-records-resources-5.6.0/tests/services/files/
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/files/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/files/files_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/files/test_file_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    15466 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/files/test_file_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/files/test_files_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/files/test_files_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/files/testimage.png
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/test_results_expand.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/test_service_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/test_service_facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/test_service_pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/test_service_queryparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/test_service_relation_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/test_service_revision_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/test_service_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/services/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/test_invenio_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-23 11:25:11.000000 invenio-records-resources-5.6.0/tests/test_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.github/workflows/tests-feature.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/factories/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/dumpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/jsonschemas/definitions-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/jsonschemas/definitions-v2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/calculated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/entity_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/files/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17053 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/files/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/pid_statuscheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/relations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/files/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/files/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/files/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/links.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/processors/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/links.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/querystr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/suggest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18663 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/references/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/uow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/requirements-feature.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1277 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/factories/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/factories/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/factories/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/records/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/records/record-nofiles-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v1/records/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v1/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v2/records/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v2/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/v7/records/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/v7/records/record-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/jsonschemas/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/jsonschemas/grants/grant-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v1/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v1/grants/grant-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v2/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v2/grants/grant-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/v7/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/v7/grants/grant-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_systemfield_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_systemfield_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_systemfield_modelpid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_systemfield_pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_systemfield_pidstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_files_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resource_faceting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resource_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resource_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resource_preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resource_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resources_etag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_base_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_boolean_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_date_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_number_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_schema_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_text_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/services/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/files_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/test_file_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15803 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/test_file_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/test_files_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/test_files_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/testimage.png
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_results_expand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_queryparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_relation_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_revision_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/test_invenio_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/test_tasks.py
```

### Comparing `invenio-records-resources-5.6.0/.editorconfig` & `invenio-records-resources-5.7.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/.github/workflows/pypi-publish.yml` & `invenio-records-resources-5.7.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/.github/workflows/tests-feature.yml` & `invenio-records-resources-5.7.0/.github/workflows/tests-feature.yml`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/.github/workflows/tests.yml` & `invenio-records-resources-5.7.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/.tx/config` & `invenio-records-resources-5.7.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/CHANGES.rst` & `invenio-records-resources-5.7.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     Invenio-Records-Resources is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 5.7.0 (released 2024-05-06)
+
+- files-schema: hide `uri` from serialization
+- records: added access field to files
+
 Version 5.6.0 (released 2024-04-23)
 
 - services: add support for nested links
 
 Version 5.5.0 (released 2024-04-09)
 
 * records: add calculated system field with indexing; allows calculated system field to cache the value in the index, and
```

### Comparing `invenio-records-resources-5.6.0/CONTRIBUTING.rst` & `invenio-records-resources-5.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/LICENSE` & `invenio-records-resources-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/MANIFEST.in` & `invenio-records-resources-5.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/PKG-INFO` & `invenio-records-resources-5.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-resources
-Version: 5.6.0
+Version: 5.7.0
 Summary: Invenio resources module to create REST APIs.
 Home-page: https://github.com/inveniosoftware/invenio-records-resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -45,14 +45,19 @@
             Invenio-Records-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 5.7.0 (released 2024-05-06)
+        
+        - files-schema: hide `uri` from serialization
+        - records: added access field to files
+        
         Version 5.6.0 (released 2024-04-23)
         
         - services: add support for nested links
         
         Version 5.5.0 (released 2024-04-09)
         
         * records: add calculated system field with indexing; allows calculated system field to cache the value in the index, and
```

### Comparing `invenio-records-resources-5.6.0/README.rst` & `invenio-records-resources-5.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/docs/Makefile` & `invenio-records-resources-5.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/docs/conf.py` & `invenio-records-resources-5.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/docs/index.rst` & `invenio-records-resources-5.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/docs/make.bat` & `invenio-records-resources-5.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/config.py` & `invenio-records-resources-5.7.0/invenio_records_resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/errors.py` & `invenio-records-resources-5.7.0/invenio_records_resources/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/ext.py` & `invenio-records-resources-5.7.0/invenio_records_resources/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/factories/factory.py` & `invenio-records-resources-5.7.0/invenio_records_resources/factories/factory.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/pagination.py` & `invenio-records-resources-5.7.0/invenio_records_resources/pagination.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/proxies.py` & `invenio-records-resources-5.7.0/invenio_records_resources/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/api.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2023 CERN.
+# Copyright (C) 2020-2024 CERN.
 # Copyright (C) 2020 Northwestern University.
 #
 # Invenio-Records-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Records API."""
@@ -13,15 +13,15 @@
 import os
 from contextlib import contextmanager
 
 from invenio_db import db
 from invenio_files_rest.models import FileInstance, ObjectVersion
 from invenio_records.api import Record as RecordBase
 from invenio_records.dumpers import SearchDumper
-from invenio_records.systemfields import DictField, SystemFieldsMixin
+from invenio_records.systemfields import DictField, SystemField, SystemFieldsMixin
 from invenio_records.systemfields.model import ModelField
 
 
 class Record(RecordBase, SystemFieldsMixin):
     """Base class for record APIs.
 
     Subclass this record, and specify as minimum the ``model_cls`` class-level
@@ -46,14 +46,106 @@
     #: Concrete implementations need to implement the index field.
     # index = IndexField(...)
 
     #: Concrete implementations need to implement the files field.
     # files = FilesField(...)
 
 
+# NOTE: Defined here to avoid circular imports
+class FileAccess:
+    """Access management for files."""
+
+    def __init__(self, hidden=None):
+        """Create a new FileAccess object for a file."""
+        self._hidden = hidden or False
+        self.dirty = hidden is not None
+
+    @property
+    def hidden(self):
+        """Get the hidden status."""
+        return self._hidden
+
+    @hidden.setter
+    def hidden(self, value):
+        """Set the hidden status."""
+        if not isinstance(value, bool):
+            raise ValueError("Invalid value for 'hidden', it must be a boolean.")
+        self._hidden = value
+        self.dirty = True
+
+    @classmethod
+    def from_dict(cls, access_dict):
+        """Create a new FileAccess object from the specified 'access' property."""
+        # provide defaults in case there is no 'access' property
+        return cls(
+            hidden=access_dict.get("hidden", False),
+        )
+
+    def dump(self):
+        """Dump the field values as dictionary."""
+        return {
+            "hidden": self.hidden,
+        }
+
+
+class FileAccessField(SystemField):
+    """File access field."""
+
+    def __init__(self, key=None, access_obj_class=FileAccess):
+        """Initialize the access field."""
+        self._access_obj_class = access_obj_class
+        super().__init__(key=key)
+
+    def obj(self, instance):
+        """Get the access object."""
+        obj = self._get_cache(instance)
+        if obj is not None:
+            return obj
+
+        data = self.get_dictkey(instance)
+        if data:
+            obj = self._access_obj_class.from_dict(data)
+        else:
+            obj = self._access_obj_class()
+
+        self._set_cache(instance, obj)
+        return obj
+
+    def set_obj(self, record, obj):
+        """Set the access object."""
+        # We accept both dicts and access class objects.
+        if isinstance(obj, dict):
+            obj = self._access_obj_class.from_dict(obj)
+
+        assert isinstance(obj, self._access_obj_class)
+
+        # We do not dump the object until the pre_commit hook
+        # I.e. record.access != record['access']
+        self._set_cache(record, obj)
+
+    def __get__(self, record, owner=None):
+        """Get the record's access object."""
+        if record is None:
+            # access by class
+            return self
+
+        # access by object
+        return self.obj(record)
+
+    def __set__(self, record, obj):
+        """Set the records access object."""
+        self.set_obj(record, obj)
+
+    def pre_commit(self, record):
+        """Dump the configured values before the record is committed."""
+        obj = self.obj(record)
+        if obj.dirty:
+            record["access"] = obj.dump()
+
+
 class FileRecord(RecordBase, SystemFieldsMixin):
     """Base class for a record describing a file."""
 
     @classmethod
     def get_by_key(cls, record_id, key):
         """Get a record file by record ID and filename/key."""
         with db.session.no_autoflush:
@@ -119,14 +211,17 @@
 
     #: Default dumper (which happens to also be used for indexing).
     dumper = SearchDumper()
 
     #: Metadata system field.
     metadata = DictField(clear_none=True, create_if_missing=True)
 
+    #: Access system field
+    access = FileAccessField()
+
     key = ModelField()
     object_version_id = ModelField()
     object_version = ModelField(dump=False)
     record_id = ModelField()
     _record = ModelField("record", dump=False)
 
     def __repr__(
```

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/dumpers.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/dumpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022-2023 CERN.
+# Copyright (C) 2022-2024 CERN.
 #
 # Invenio-Records-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Records dumpers and extensions."""
 
@@ -49,26 +49,32 @@
         """Dump a partial file record to include into another record."""
         data = {
             "uuid": str(record.id),
             "version_id": record.revision_id + 1,
             "metadata": deepcopy(dict(record.get("metadata", {}))),
             "key": record.key,
         }
+        access = record.get("access")
+        if access:
+            data.update({"access": access})
         if record.file:
             data.update(record.file.dumps())
         return data
 
     def load(self, data, record_cls):
         """Load a record from the source document of a search engine hit."""
         model_data = {
             "id": str(data["uuid"]),
             "version_id": data["version_id"],
             "key": data["key"],
             "record_id": data["record_id"],
             "object_version_id": data["object_version_id"],
         }
-        record_data = {"metadata": data["metadata"]}
+        record_data = {"metadata": data.get("metadata", {})}
+        access = data.get("access")
+        if access:
+            record_data["access"] = access
         model = record_cls.model_cls(**model_data)
         record = record_cls(record_data, model=model)
         f = File.from_dump(data)
         record.object_version = f.object_model
         return record
```

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/jsonschemas/definitions-v1.0.0.json` & `invenio-records-resources-5.7.0/invenio_records_resources/records/jsonschemas/definitions-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/jsonschemas/definitions-v2.0.0.json` & `invenio-records-resources-5.7.0/invenio_records_resources/records/jsonschemas/definitions-v2.0.0.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993686868686869%*

 * *Differences: {"'file'": "{'properties': {'access': OrderedDict([('description', 'Access properties of the "*

 * *           "file.'), ('type', 'object'), ('additionalProperties', False), ('properties', "*

 * *           "OrderedDict([('hidden', OrderedDict([('description', 'Control whether to hide the file "*

 * *           "in the UI.'), ('type', 'boolean')]))]))])}}"}*

```diff
@@ -15,14 +15,25 @@
             "null"
         ]
     },
     "file": {
         "additionalProperties": false,
         "description": "A file object.",
         "properties": {
+            "access": {
+                "additionalProperties": false,
+                "description": "Access properties of the file.",
+                "properties": {
+                    "hidden": {
+                        "description": "Control whether to hide the file in the UI.",
+                        "type": "boolean"
+                    }
+                },
+                "type": "object"
+            },
             "checksum": {
                 "description": "Checksum of the file.",
                 "type": "string"
             },
             "ext": {
                 "description": "Checksum of the file.",
                 "type": "string"
```

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/models.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/providers.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/providers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/resolver.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/calculated.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/calculated.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/entity_reference.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/entity_reference.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/files/field.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/files/field.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/files/manager.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/files/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2023 CERN.
+# Copyright (C) 2020-2024 CERN.
 # Copyright (C) 2020-2021 Northwestern University.
 #
 # Invenio-Records-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Files field.
@@ -167,15 +167,15 @@
             if isinstance(obj, dict):
                 fi = FileInstance.create()
                 fi.set_uri(**obj.pop("file"))
                 obj = ObjectVersion.create(self.bucket, key, fi.id)
             rf.object_version_id = obj.version_id
             rf.object_version = obj
         if data:
-            rf.metadata = data
+            rf.update(data)
         rf.commit()
         self._entries[key] = rf
         return rf
 
     @ensure_enabled
     def create_obj(self, key, stream, data=None, **kwargs):
         """Create an ObjectVersion but do not pop it to the top of the stack."""
@@ -186,24 +186,25 @@
 
         return ObjectVersion.create(self.bucket, key, stream=stream, **kwargs)
 
     @ensure_enabled
     def update(self, key, obj=None, stream=None, data=None, **kwargs):
         """Update a file."""
         assert not (obj and stream)
+        data = data or {}
         rf = self.get(key)
 
         if stream:
             obj = self.create_obj(key, stream=stream, **kwargs)
         if obj:
             rf.object_version_id = obj.version_id
             rf.object_version = obj
         if data:
-            rf.metadata = data
-            rf.commit()
+            rf.update(data)
+        rf.commit()
         return rf
 
     @ensure_enabled
     def commit(self, file_key):
         """Commit a file."""
         file_obj = ObjectVersion.get(self.bucket.id, file_key)
         if not file_obj:
@@ -294,15 +295,15 @@
                     "id": uuid.uuid4(),
                     "created": datetime.utcnow(),
                     "updated": datetime.utcnow(),
                     "key": key,
                     "record_id": record_id,
                     "version_id": 1,
                     "object_version_id": ovs_by_key[key]["version_id"],
-                    "json": rf.metadata or {},
+                    "json": dict(rf),
                 }
                 rf_to_bulk_insert.append(new_rf)
 
             if rf_to_bulk_insert:
                 db.session.execute(insert(self.file_cls.model_cls), rf_to_bulk_insert)
                 # we need to populate entries from DB so we store the record file model
                 # instance
@@ -318,18 +319,17 @@
                 if copy_obj:
                     dst_obj = rf.object_version.copy(bucket=self.bucket)
                 else:
                     dst_obj = rf.object_version
 
                 # Copy file record
                 if rf.metadata is not None:
-                    self[key] = dst_obj, rf.metadata
+                    self[key] = dst_obj, dict(rf)
                 else:
                     self[key] = dst_obj
-
         self.default_preview = src_files.default_preview
         self.order = src_files.order
 
     def sync(self, src_files, delete_extras=True):
         """Sync changes from source files to this manager.
 
         The source files are fully mirrored with the destination files following the
@@ -338,14 +338,15 @@
          * same ObjectVersions are not touched
          * new ObjectVersions are added to destination
          * deleted ObjectVersions are deleted in destination
          * extra ObjectVersions in dest are deleted if `delete_extras` param is
            True
         Logic follows the bucket sync logic
         """
+        # TODO record file data is not synced
         self.default_preview = src_files.default_preview
         self.order = src_files.order
 
         # Sync file additions/removals/changes
         if self.bucket.locked:
             raise BucketLockedError()
```

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/index.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/index.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/pid.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/pid.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/pid_statuscheck.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/pid_statuscheck.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/records/systemfields/relations.py` & `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/relations.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/references/entity_resolvers/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/references/entity_resolvers/base.py` & `invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/references/entity_resolvers/records.py` & `invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/records.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/references/entity_resolvers/results.py` & `invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/references/grants.py` & `invenio-records-resources-5.7.0/invenio_records_resources/references/grants.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/references/registry.py` & `invenio-records-resources-5.7.0/invenio_records_resources/references/registry.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/registry.py` & `invenio-records-resources-5.7.0/invenio_records_resources/registry.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/resources/errors.py` & `invenio-records-resources-5.7.0/invenio_records_resources/resources/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/resources/files/config.py` & `invenio-records-resources-5.7.0/invenio_records_resources/resources/files/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/resources/files/parser.py` & `invenio-records-resources-5.7.0/invenio_records_resources/resources/files/parser.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/resources/files/resource.py` & `invenio-records-resources-5.7.0/invenio_records_resources/resources/files/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/resources/records/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/resources/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/resources/records/args.py` & `invenio-records-resources-5.7.0/invenio_records_resources/resources/records/args.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/resources/records/config.py` & `invenio-records-resources-5.7.0/invenio_records_resources/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/resources/records/headers.py` & `invenio-records-resources-5.7.0/invenio_records_resources/resources/records/headers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/resources/records/resource.py` & `invenio-records-resources-5.7.0/invenio_records_resources/resources/records/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/resources/records/utils.py` & `invenio-records-resources-5.7.0/invenio_records_resources/resources/records/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/base/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/base/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/base/components.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/base/components.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/base/config.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/base/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/base/links.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/base/links.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/base/results.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/base/results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/base/service.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/base/service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/base/utils.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/base/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/base.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/boolean.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/boolean.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/date.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/date.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/errors.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/mappings.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/mappings.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/number.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/number.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/schema.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/text.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/text.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/custom_fields/validate.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/validate.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/errors.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/components/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/components/base.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/components/content.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/content.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/components/metadata.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021-2022 CERN.
+# Copyright (C) 2021-2024 CERN.
 #
 # Invenio-Records-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Files metadata component components."""
 
 from copy import deepcopy
 
 from ...errors import FilesCountExceededException
-from ..schema import InitFileSchema
 from ..transfer import Transfer
 from .base import FileServiceComponent
 
 
 class FileMetadataComponent(FileServiceComponent):
     """File metadata service component."""
 
     def init_files(self, identity, id, record, data):
         """Init files handler."""
-        schema = InitFileSchema(many=True)
+        schema = self.service.file_schema.schema(many=True)
         validated_data = schema.load(data)
 
         # All brand-new drafts don't allow exceeding files limit (while added via rest API).
         # Old records that already had more files than limited can continue adding files.
         # In case files amount goes back to under limit, users lose the privilege of adding more files.
         resulting_files_count = record.files.count + len(validated_data)
         maxFiles = self.service.config.max_files_count
 
         if maxFiles and record.files.count <= maxFiles:
             if resulting_files_count > maxFiles:
                 raise FilesCountExceededException(
                     max_files=maxFiles, resulting_files_count=resulting_files_count
                 )
 
-        for file_metadata in validated_data:
-            temporary_obj = deepcopy(file_metadata)
-            file_type = temporary_obj.pop("storage_class", None)
+        for file_data in validated_data:
+            copy_fdata = deepcopy(file_data)
+            file_type = copy_fdata.pop("storage_class", None)
             transfer = Transfer.get_transfer(
                 file_type, service=self.service, uow=self.uow
             )
-            _ = transfer.init_file(record, temporary_obj)
+            _ = transfer.init_file(record, copy_fdata)
 
     def update_file_metadata(self, identity, id, file_key, record, data):
         """Update file metadata handler."""
         # FIXME: move this call to a transfer call
-        record.files.update(file_key, data=data)
+        schema = self.service.file_schema.schema(many=False)
+
+        # 'key' is required in the schema, but might not be in the data
+        if "key" not in data:
+            data["key"] = file_key
+        validated_data = schema.load(data)
+        record.files.update(file_key, data=validated_data)
 
     # TODO: `commit_file` might vary based on your storage backend (e.g. S3)
     def commit_file(self, identity, id, file_key, record):
         """Commit file handler."""
         Transfer.commit_file(record, file_key)
```

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/components/processor.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/processor.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/config.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/generators.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/links.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/links.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/processors/base.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/processors/base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/processors/image.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/processors/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 #
 # Invenio-Records-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Image metadata extractor."""
 
-import os
-
 import pkg_resources
 from flask import current_app
 
 from .base import FileProcessor
 
 try:
     pkg_resources.get_distribution("wand")
```

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/results.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/schema.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2022 CERN.
+# Copyright (C) 2020-2024 CERN.
 # Copyright (C) 2020 European Union.
 #
 # Invenio-Records-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """File schema."""
@@ -18,16 +18,16 @@
     RAISE,
     Schema,
     ValidationError,
     pre_dump,
     validate,
     validates,
 )
-from marshmallow.fields import UUID, Dict, Integer, Str
-from marshmallow_utils.fields import GenMethod, Links, SanitizedUnicode, TZDateTime
+from marshmallow.fields import UUID, Boolean, Dict, Integer, Nested, Str
+from marshmallow_utils.fields import GenMethod, Links, TZDateTime
 
 from .transfer import TransferType
 
 
 class InitFileSchema(Schema):
     """Service (component) schema for file initialization.
 
@@ -51,15 +51,15 @@
     class Meta:
         """Meta."""
 
         unknown = INCLUDE
 
     key = Str(required=True)
     storage_class = Str()
-    uri = Str()
+    uri = Str(load_only=True)
     checksum = Str()
     size = Integer()
 
     @validates("uri")
     def validate_names(self, value):
         """Validate the domain of the URI is allowed."""
         # checking if storage class and uri are compatible is a
@@ -97,31 +97,44 @@
                 value = getattr(data.file, field, None)
                 if value is not None:
                     data[field] = value
 
         return data
 
 
+class FileAccessSchema(Schema):
+    """Schema for file access."""
+
+    class Meta:
+        """Meta."""
+
+        unknown = RAISE
+
+    hidden = Boolean()
+
+
 class FileSchema(InitFileSchema):
     """Service schema for files."""
 
     class Meta:
         """Meta."""
 
         unknown = RAISE
 
     created = TZDateTime(timezone=timezone.utc, format="iso", dump_only=True)
     updated = TZDateTime(timezone=timezone.utc, format="iso", dump_only=True)
 
     status = GenMethod("dump_status")
-    metadata = Dict(dump_only=True)
     mimetype = Str(dump_only=True, attribute="file.mimetype")
-    version_id = UUID(attribute="file.version_id")
-    file_id = UUID(attribute="file.file_id")
-    bucket_id = UUID(attribute="file.bucket_id")
+    version_id = UUID(attribute="file.version_id", dump_only=True)
+    file_id = UUID(attribute="file.file_id", dump_only=True)
+    bucket_id = UUID(attribute="file.bucket_id", dump_only=True)
+
+    metadata = Dict()
+    access = Nested(FileAccessSchema)
 
     links = Links()
 
     def dump_status(self, obj):
         """Dump file status."""
         # due to time constraints the status check is done here
         # however, ideally this class should not need knowledge of
```

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/service.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/tasks.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 CERN.
+# Copyright (C) 2022-2024 CERN.
 #
 # Invenio-Records-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Files tasks."""
 
@@ -19,15 +19,15 @@
 
 @shared_task(ignore_result=True)
 def fetch_file(service_id, record_id, file_key):
     """Fetch file from external storage."""
     try:
         service = current_service_registry.get(service_id)
         file_record = service.read_file_metadata(system_identity, record_id, file_key)
-        source_url = file_record.data["uri"]
+        source_url = file_record._file.file.uri
         # download file
         # verify=True for self signed certificates by default
         with requests.get(source_url, stream=True, allow_redirects=True) as response:
             # save file
             service.set_file_content(
                 system_identity,
                 record_id,
```

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/files/transfer.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/files/transfer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 CERN.
+# Copyright (C) 2022-2024 CERN.
 #
 # Invenio-Records-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Files transfer."""
 
@@ -59,15 +59,15 @@
     def __init__(self, type, service=None, uow=None):
         """Constructor."""
         self.type = type
         self.service = service
         self.uow = uow
 
     @abstractmethod
-    def init_file(self, record, file_metadata):
+    def init_file(self, record, file_data):
         """Initialize a file."""
         raise NotImplementedError()
 
     def set_file_content(self, record, file, file_key, stream, content_length):
         """Set file content."""
         bucket = record.bucket
 
@@ -99,33 +99,33 @@
             allow_empty_files = current_app.config.get(
                 "RECORDS_RESOURCES_ALLOW_EMPTY_FILES", True
             )
             if not allow_empty_files:
                 raise FileSizeError(description=_("Empty files are not accepted."))
 
     # @abstractmethod
-    # def read_file_content(self, record, file_metadata):
+    # def read_file_content(self, record, data):
     #     """Read a file content."""
     #     pass
 
 
 class LocalTransfer(BaseTransfer):
     """Local transfer."""
 
     def __init__(self, **kwargs):
         """Constructor."""
         super().__init__(TransferType.LOCAL, **kwargs)
 
-    def init_file(self, record, file_metadata):
+    def init_file(self, record, file_data):
         """Initialize a file."""
-        uri = file_metadata.pop("uri", None)
+        uri = file_data.pop("uri", None)
         if uri:
             raise Exception("Cannot set URI for local files.")
 
-        file = record.files.create(key=file_metadata.pop("key"), data=file_metadata)
+        file = record.files.create(key=file_data.pop("key"), data=file_data)
 
         return file
 
     def set_file_content(self, record, file, file_key, stream, content_length):
         """Set file content."""
         if file:
             raise TransferException(f'File with key "{file_key}" is committed.')
@@ -136,33 +136,33 @@
 class FetchTransfer(BaseTransfer):
     """Fetch transfer."""
 
     def __init__(self, **kwargs):
         """Constructor."""
         super().__init__(TransferType.FETCH, **kwargs)
 
-    def init_file(self, record, file_metadata):
+    def init_file(self, record, file_data):
         """Initialize a file."""
-        uri = file_metadata.pop("uri", None)
+        uri = file_data.pop("uri", None)
         if not uri:
             raise Exception("URI is required for fetch files.")
 
         obj_kwargs = {
             "file": {
                 "uri": uri,
                 "storage_class": self.type,
-                "checksum": file_metadata.pop("checksum", None),
-                "size": file_metadata.pop("size", None),
+                "checksum": file_data.pop("checksum", None),
+                "size": file_data.pop("size", None),
             }
         }
 
-        file_key = file_metadata.pop("key")
+        file_key = file_data.pop("key")
         file = record.files.create(
             key=file_key,
-            data=file_metadata,
+            data=file_data,
             obj=obj_kwargs,
         )
 
         self.uow.register(
             TaskOp(
                 fetch_file,
                 service_id=self.service.id,
```

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/base.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/data.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/data.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/files.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/files.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/metadata.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/components/relations.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/relations.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/config.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/facets/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/facets/facets.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/facets/labels.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/labels.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/facets/response.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/response.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/links.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/links.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/base.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/facets.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/filter.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/filter.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/pagination.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/pagination.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/querystr.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/querystr.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/params/sort.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/sort.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/queryparser/__init__.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/queryparser/query.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/query.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/queryparser/suggest.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/suggest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/queryparser/transformer.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/transformer.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/results.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/schema.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/records/service.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/records/service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/references/schema.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/references/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/services/uow.py` & `invenio-records-resources-5.7.0/invenio_records_resources/services/uow.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/tasks.py` & `invenio-records-resources-5.7.0/invenio_records_resources/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources.egg-info/PKG-INFO` & `invenio-records-resources-5.7.0/invenio_records_resources.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-resources
-Version: 5.6.0
+Version: 5.7.0
 Summary: Invenio resources module to create REST APIs.
 Home-page: https://github.com/inveniosoftware/invenio-records-resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -45,14 +45,19 @@
             Invenio-Records-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 5.7.0 (released 2024-05-06)
+        
+        - files-schema: hide `uri` from serialization
+        - records: added access field to files
+        
         Version 5.6.0 (released 2024-04-23)
         
         - services: add support for nested links
         
         Version 5.5.0 (released 2024-04-09)
         
         * records: add calculated system field with indexing; allows calculated system field to cache the value in the index, and
```

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources.egg-info/SOURCES.txt` & `invenio-records-resources-5.7.0/invenio_records_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources.egg-info/entry_points.txt` & `invenio-records-resources-5.7.0/invenio_records_resources.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/invenio_records_resources.egg-info/requires.txt` & `invenio-records-resources-5.7.0/invenio_records_resources.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/run-tests.sh` & `invenio-records-resources-5.7.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/setup.cfg` & `invenio-records-resources-5.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/conftest.py` & `invenio-records-resources-5.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/factories/conftest.py` & `invenio-records-resources-5.7.0/tests/factories/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/factories/test_factory.py` & `invenio-records-resources-5.7.0/tests/factories/test_factory.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/factories/test_service.py` & `invenio-records-resources-5.7.0/tests/factories/test_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module/api.py` & `invenio-records-resources-5.7.0/tests/mock_module/api.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module/config.py` & `invenio-records-resources-5.7.0/tests/mock_module/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module/jsonschemas/records/record-nofiles-v1.0.0.json` & `invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/records/record-nofiles-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json` & `invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module/mappings/os-v1/records/record-v1.0.0.json` & `invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v1/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module/mappings/os-v2/records/record-v1.0.0.json` & `invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v2/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module/mappings/v7/records/record-v1.0.0.json` & `invenio-records-resources-5.7.0/tests/mock_module/mappings/v7/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module/models.py` & `invenio-records-resources-5.7.0/tests/mock_module/models.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module/permissions.py` & `invenio-records-resources-5.7.0/tests/mock_module/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module/resource.py` & `invenio-records-resources-5.7.0/tests/mock_module/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module/schemas.py` & `invenio-records-resources-5.7.0/tests/mock_module/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/os-v1/grants/grant-v1.0.0.json` & `invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v1/grants/grant-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/os-v2/grants/grant-v1.0.0.json` & `invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v2/grants/grant-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/mock_module_factory/mappings/v7/grants/grant-v1.0.0.json` & `invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/v7/grants/grant-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/records/conftest.py` & `invenio-records-resources-5.7.0/tests/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/records/test_api.py` & `invenio-records-resources-5.7.0/tests/records/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/records/test_dumpers.py` & `invenio-records-resources-5.7.0/tests/records/test_dumpers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/records/test_systemfield_files.py` & `invenio-records-resources-5.7.0/tests/records/test_systemfield_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2023 CERN.
+# Copyright (C) 2020-2024 CERN.
 # Copyright (C) 2020 Northwestern University.
 #
 # Invenio-Records-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Files field tests."""
@@ -72,30 +72,30 @@
 
 
 def test_record_files_operations(base_app, db, location):
     """Test record files bucket creation."""
     record = Record.create({})
 
     # Initialize a file
-    record.files["test.pdf"] = {"description": "A test file."}
+    record.files["test.pdf"] = {"metadata": {"description": "A test file."}}
     rf = record.files["test.pdf"]
     assert rf.key == "test.pdf"
     assert rf.object_version is None
     assert rf.object_version_id is None
     assert rf.record_id is not None
     assert rf.record_id == record.id
     assert rf.metadata == {"description": "A test file."}
     assert rf["metadata"] == {"description": "A test file."}
     db.session.commit()
 
     assert models.FileRecordMetadata.query.count() == 1
     assert ObjectVersion.query.count() == 0
 
     # Update the file's metadata
-    record.files["test.pdf"] = {"description": "A new description"}
+    record.files["test.pdf"] = {"metadata": {"description": "A new description"}}
     rf = record.files["test.pdf"]
     assert rf.key == "test.pdf"
     assert rf.object_version is None
     assert rf.object_version_id is None
     assert rf.record_id is not None
     assert rf.record_id == record.id
     assert rf.metadata == {"description": "A new description"}
@@ -132,19 +132,22 @@
 
 
 def test_record_files_clear(base_app, db, location):
     """Test clearing record files (hard deletion)."""
     record = Record.create({})
 
     # Add a file with metadata + bytes
-    record.files["f1.pdf"] = (BytesIO(b"testfile"), {"description": "Test file"})
+    record.files["f1.pdf"] = (
+        BytesIO(b"testfile"),
+        {"metadata": {"description": "Test file"}},
+    )
     # Add a file with only bytes
     record.files["f2.pdf"] = BytesIO(b"testfile")
     # Add a file with only metadata
-    record.files["f3.pdf"] = {"description": "Metadata only"}
+    record.files["f3.pdf"] = {"metadata": {"description": "Metadata only"}}
     record.commit()
     db.session.commit()
 
     assert models.FileRecordMetadata.query.count() == 3
     assert FileInstance.query.count() == 2
     assert ObjectVersion.query.count() == 2
     assert Bucket.query.count() == 1
@@ -167,19 +170,22 @@
 
 
 def test_record_files_teardown_full(base_app, db, location):
     """Test clearing record files (hard deletion)."""
     record = Record.create({})
 
     # Add a file with metadata + bytes
-    record.files["f1.pdf"] = (BytesIO(b"testfile"), {"description": "Test file"})
+    record.files["f1.pdf"] = (
+        BytesIO(b"testfile"),
+        {"metadata": {"description": "Test file"}},
+    )
     # Add a file with only bytes
     record.files["f2.pdf"] = BytesIO(b"testfile")
     # Add a file with only metadata
-    record.files["f3.pdf"] = {"description": "Metadata only"}
+    record.files["f3.pdf"] = {"metadata": {"description": "Metadata only"}}
     record.commit()
     db.session.commit()
 
     assert models.FileRecordMetadata.query.count() == 3
     assert FileInstance.query.count() == 2
     assert ObjectVersion.query.count() == 2
     assert Bucket.query.count() == 1
@@ -202,19 +208,22 @@
 
 
 def test_record_files_teardown_partial(base_app, db, location):
     """Test soft deleting record files."""
     record = Record.create({})
 
     # Add a file with metadata + bytes
-    record.files["f1.pdf"] = (BytesIO(b"testfile"), {"description": "Test file"})
+    record.files["f1.pdf"] = (
+        BytesIO(b"testfile"),
+        {"metadata": {"description": "Test file"}},
+    )
     # Add a file with only bytes
     record.files["f2.pdf"] = BytesIO(b"testfile")
     # Add a file with only metadata
-    record.files["f3.pdf"] = {"description": "Metadata only"}
+    record.files["f3.pdf"] = {"metadata": {"description": "Metadata only"}}
     record.commit()
     db.session.commit()
 
     assert models.FileRecordMetadata.query.count() == 3
     assert FileInstance.query.count() == 2
     assert ObjectVersion.query.count() == 2
     assert Bucket.query.count() == 1
@@ -242,19 +251,22 @@
 
 
 def test_record_files_soft_delete(base_app, db, location):
     """Test soft deleting record files."""
     record = Record.create({})
 
     # Add a file with metadata + bytes
-    record.files["f1.pdf"] = (BytesIO(b"testfile"), {"description": "Test file"})
+    record.files["f1.pdf"] = (
+        BytesIO(b"testfile"),
+        {"metadata": {"description": "Test file"}},
+    )
     # Add a file with only bytes
     record.files["f2.pdf"] = BytesIO(b"testfile")
     # Add a file with only metadata
-    record.files["f3.pdf"] = {"description": "Metadata only"}
+    record.files["f3.pdf"] = {"metadata": {"description": "Metadata only"}}
     record.commit()
     db.session.commit()
 
     assert models.FileRecordMetadata.query.count() == 3
     assert FileInstance.query.count() == 2
     assert ObjectVersion.query.count() == 2
     assert Bucket.query.count() == 1
@@ -282,15 +294,18 @@
 
 
 def test_record_files_store(base_app, db, location):
     """Test JSON stored for files."""
     record = Record.create({})
 
     # Add a file with bytes + metadata
-    record.files["f1.pdf"] = (BytesIO(b"testfile"), {"description": "Test file"})
+    record.files["f1.pdf"] = (
+        BytesIO(b"testfile"),
+        {"metadata": {"description": "Test file"}},
+    )
     # Add a file with only bytes
     record.files["f2.pdf"] = BytesIO(b"testfile")
 
     rf1 = record.files["f1.pdf"]
     rf2 = record.files["f2.pdf"]
     record.commit()
     assert record["files"]["entries"] == {
@@ -310,15 +325,18 @@
     }
 
 
 def test_record_files_copy(base_app, db, location):
     """Test record files bucket creation."""
     # Create source record
     src = Record.create({})
-    src.files["f1.pdf"] = (BytesIO(b"testfile"), {"description": "Test file"})
+    src.files["f1.pdf"] = (
+        BytesIO(b"testfile"),
+        {"metadata": {"description": "Test file"}},
+    )
     src.files.default_preview = "f1.pdf"
     src.files.order = ["f1.pdf"]
     src.commit()
     db.session.commit()
 
     assert ObjectVersion.query.count() == 1
     assert Bucket.query.count() == 1
@@ -365,15 +383,18 @@
     dst.files.copy(src.files)
     assert dst.files.enabled is False
 
 
 def test_record_files_dump(base_app, db, location):
     """Test dumped data for record."""
     record = Record2.create({})
-    record.files["f1.txt"] = (BytesIO(b"testfile"), {"description": "Test file"})
+    record.files["f1.txt"] = (
+        BytesIO(b"testfile"),
+        {"metadata": {"description": "Test file"}},
+    )
     rf = record.files["f1.txt"]
     record.commit()
 
     # Assert files data dumped inside the record
     data = record.dumps()
     assert data["files"] == {
         "enabled": True,
@@ -400,7 +421,40 @@
     # Load data
     new_record = Record2.loads(data)
     new_rf = new_record.files["f1.txt"]
     assert new_rf.dumps(dumper=PartialFileDumper()) == rf.dumps(
         dumper=PartialFileDumper()
     )
     assert new_record == record
+
+
+def test_record_files_access_explicit_set(base_app, db, location):
+    """Test record files access, when explicitely set.
+
+    When the access field is set, it should be dumped.
+    """
+    record = Record.create({})
+    record.files["f1.txt"] = (
+        BytesIO(b"testfile"),
+        {"metadata": {"description": "Test file"}, "access": {"hidden": True}},
+    )
+    rf = record.files["f1.txt"]
+    assert rf.access.hidden is True
+    record.commit()
+    data = record.dumps()
+    assert data["files"]["entries"][0]["access"] == {"hidden": True}
+    assert record.files["f1.txt"].model.json["access"] == {"hidden": True}
+
+
+def test_record_files_access_implicit_not_set(base_app, db, location):
+    """Test record files access, when not implicitely set.
+
+    When the access field is not set, it should not be dumped.
+    """
+    record = Record.create({})
+    record.files["f1.txt"] = BytesIO(b"testfile")
+    rf = record.files["f1.txt"]
+    assert rf.access.hidden is False
+    record.commit()
+    data = record.dumps()
+    assert data["files"]["entries"][0].get("access") is None
+    assert record.files["f1.txt"].model.json.get("access") is None
```

### Comparing `invenio-records-resources-5.6.0/tests/records/test_systemfield_index.py` & `invenio-records-resources-5.7.0/tests/records/test_systemfield_index.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/records/test_systemfield_modelpid.py` & `invenio-records-resources-5.7.0/tests/records/test_systemfield_modelpid.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/records/test_systemfield_pid.py` & `invenio-records-resources-5.7.0/tests/records/test_systemfield_pid.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/records/test_systemfield_pidstatus.py` & `invenio-records-resources-5.7.0/tests/records/test_systemfield_pidstatus.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/resources/conftest.py` & `invenio-records-resources-5.7.0/tests/resources/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/resources/test_files_resource.py` & `invenio-records-resources-5.7.0/tests/resources/test_files_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2021 CERN.
+# Copyright (C) 2020-2024 CERN.
 # Copyright (C) 2021 Northwestern University.
 # Copyright (C) 2021 European Union.
 #
 # Invenio-Records-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
@@ -77,15 +77,15 @@
     assert res.json["links"]["files"].endswith(f"/api/mocks/{id_}/files")
 
     # Initialize files upload
     res = client.post(
         f"/mocks/{id_}/files",
         headers=headers,
         json=[
-            {"key": "test.pdf", "title": "Test file"},
+            {"key": "test.pdf", "metadata": {"title": "Test file"}},
         ],
     )
     assert res.status_code == 201
     res_file = res.json["entries"][0]
     assert res_file["key"] == "test.pdf"
     assert res_file["status"] == "pending"
     assert res_file["metadata"] == {"title": "Test file"}
@@ -133,15 +133,17 @@
     # Read a file's content
     res = client.get(f"/mocks/{id_}/files/test.pdf/content", headers=headers)
     assert res.status_code == 200
     assert res.data == b"testfile"
 
     # Update file metadata
     res = client.put(
-        f"/mocks/{id_}/files/test.pdf", headers=headers, json={"title": "New title"}
+        f"/mocks/{id_}/files/test.pdf",
+        headers=headers,
+        json={"metadata": {"title": "New title"}},
     )
     assert res.status_code == 200
     assert res.json["key"] == "test.pdf"
     assert res.json["status"] == "completed"
     assert res.json["metadata"] == {"title": "New title"}
 
     # Get all files
@@ -171,15 +173,15 @@
     assert res.json["links"]["files"].endswith(f"/api/mocks/{id_}/files")
 
     # Initialize files upload
     res = client.post(
         f"/mocks/{id_}/files",
         headers=headers,
         json=[
-            {"key": "empty", "title": "Zero-length test file"},
+            {"key": "empty", "metadata": {"title": "Zero-length test file"}},
         ],
     )
     assert res.status_code == 201
 
     # Upload the empty file
     res = client.put(
         f"/mocks/{id_}/files/empty/content",
@@ -308,15 +310,15 @@
     res = client.post(f"/mocks/{id_}/files", headers=headers, json={"key": "test.pdf"})
     assert res.status_code == 400
 
     res = client.post(
         f"/mocks/{id_}/files",
         headers=headers,
         json=[
-            {"key": "test.pdf", "title": "Test file"},
+            {"key": "test.pdf", "metadata": {"title": "Test file"}},
         ],
     )
     assert res.status_code == 201
 
     # Upload a file
     res = client.put(
         f"/mocks/{id_}/files/test.pdf/content",
```

### Comparing `invenio-records-resources-5.6.0/tests/resources/test_resource_faceting.py` & `invenio-records-resources-5.7.0/tests/resources/test_resource_faceting.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/resources/test_resource_links.py` & `invenio-records-resources-5.7.0/tests/resources/test_resource_links.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/resources/test_resource_pagination.py` & `invenio-records-resources-5.7.0/tests/resources/test_resource_pagination.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/resources/test_resource_preference.py` & `invenio-records-resources-5.7.0/tests/resources/test_resource_preference.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/resources/test_resource_sorting.py` & `invenio-records-resources-5.7.0/tests/resources/test_resource_sorting.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/resources/test_resources.py` & `invenio-records-resources-5.7.0/tests/resources/test_resources.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/resources/test_resources_etag.py` & `invenio-records-resources-5.7.0/tests/resources/test_resources_etag.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/conftest.py` & `invenio-records-resources-5.7.0/tests/services/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/custom_fields/test_boolean_cf.py` & `invenio-records-resources-5.7.0/tests/services/custom_fields/test_boolean_cf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/custom_fields/test_date_cf.py` & `invenio-records-resources-5.7.0/tests/services/custom_fields/test_date_cf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/custom_fields/test_number_cf.py` & `invenio-records-resources-5.7.0/tests/services/custom_fields/test_number_cf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/custom_fields/test_schema_cf.py` & `invenio-records-resources-5.7.0/tests/services/custom_fields/test_schema_cf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/custom_fields/test_text_cf.py` & `invenio-records-resources-5.7.0/tests/services/custom_fields/test_text_cf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/custom_fields/test_validate.py` & `invenio-records-resources-5.7.0/tests/services/custom_fields/test_validate.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/files/conftest.py` & `invenio-records-resources-5.7.0/tests/services/files/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/files/files_utils.py` & `invenio-records-resources-5.7.0/tests/services/files/files_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/files/test_file_results.py` & `invenio-records-resources-5.7.0/tests/services/files/test_file_results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/files/test_file_service.py` & `invenio-records-resources-5.7.0/tests/services/files/test_file_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2022 CERN.
+# Copyright (C) 2020-2024 CERN.
 #
 # Invenio-Records-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """File service tests."""
 
@@ -51,15 +51,15 @@
 
 
 #
 # Local files
 #
 
 
-def test_file_flow(file_service, location, example_file_record, identity_simple):
+def test_file_flow(file_service, location, example_file_record, identity_simple, db):
     """Test the lifecycle of a file.
 
     - Initialize file saving
     - Save 1 files
     - Commit the files
     - List files of the record
     - Read file metadata
@@ -105,15 +105,14 @@
     assert result.to_dict()["entries"][0]["storage_class"] == "L"
     assert "uri" not in result.to_dict()["entries"][0]
 
     # Read file metadata
     result = file_service.read_file_metadata(identity_simple, recid, "article.txt")
     assert result.to_dict()["key"] == file_to_initialise[0]["key"]
     assert result.to_dict()["storage_class"] == "L"
-    assert "uri" not in result.to_dict()
 
     # Retrieve file
     result = file_service.get_file_content(identity_simple, recid, "article.txt")
     assert result.file_id == "article.txt"
 
     # Delete file
     result = file_service.delete_file(identity_simple, recid, "article.txt")
@@ -126,14 +125,15 @@
 
     # Delete all remaining files
     result = file_service.delete_all_files(identity_simple, recid)
     assert list(result.entries) == []
 
 
 def test_init_files(file_service, location, example_file_record, identity_simple):
+    """Test the initialization of local files, with different metadata and access."""
     recid = example_file_record["id"]
 
     # Pass an object with missing required field
     file_to_initialise = [{}]
 
     with pytest.raises(ValidationError) as e:
         file_service.init_files(identity_simple, recid, file_to_initialise)
@@ -141,25 +141,29 @@
     error = e.value
     assert {
         0: {"key": ["Missing data for required field."]}
     } == error.normalized_messages()
 
     # Pass an object with added field
     file_to_initialise = [
-        {
-            "key": "article.txt",
-            "foo": "bar",
-        }
+        {"key": "article.txt", "metadata": {"foo": "bar"}},
+        {"key": "article.csv", "metadata": {"foo": "baz"}, "access": {"hidden": True}},
     ]
 
     result = file_service.init_files(identity_simple, recid, file_to_initialise)
 
-    entry = result.to_dict()["entries"][0]
-    assert file_to_initialise[0]["key"] == entry["key"]
-    assert file_to_initialise[0]["foo"] == entry["metadata"]["foo"]
+    first_entry = result.to_dict()["entries"][0]
+    assert file_to_initialise[0]["key"] == first_entry["key"]
+    assert file_to_initialise[0]["metadata"] == first_entry["metadata"]
+    assert first_entry["access"]["hidden"] is False  # default value
+
+    second_entry = result.to_dict()["entries"][1]
+    assert file_to_initialise[1]["key"] == second_entry["key"]
+    assert file_to_initialise[1]["metadata"] == second_entry["metadata"]
+    assert second_entry["access"]["hidden"] is True
 
 
 #
 # External files
 #
 
 
@@ -284,15 +288,14 @@
     assert result.to_dict()["entries"][0]["key"] == file_to_initialise[0]["key"]
 
     # Check it is still external
     result = file_service.read_file_metadata(identity_simple, recid, "article.txt")
     result = result.to_dict()
     assert result["key"] == file_to_initialise[0]["key"]
     assert result["storage_class"] == "F"
-    assert "uri" in result
 
     # Set content as user
     content = BytesIO(b"test file content")
     with pytest.raises(PermissionDeniedError):
         file_service.set_file_content(
             identity_simple,
             recid,
@@ -308,15 +311,15 @@
         file_to_initialise[0]["key"],
         content,
         content.getbuffer().nbytes,
     )
     result = result.to_dict()
     assert result["key"] == file_to_initialise[0]["key"]
     assert result["storage_class"] == "F"  # not commited yet
-    assert "uri" in result
+    assert "uri" not in result
 
     # Commit as user
     with pytest.raises(PermissionDeniedError):
         file_service.commit_file(identity_simple, recid, "article.txt")
 
     # Commit as system
     result = file_service.commit_file(system_identity, recid, "article.txt")
@@ -360,15 +363,14 @@
     assert result.to_dict()["entries"][0]["key"] == file_to_initialise[0]["key"]
 
     # Check it is still external
     result = file_service.read_file_metadata(identity_simple, recid, "article.txt")
     result = result.to_dict()
     assert result["key"] == file_to_initialise[0]["key"]
     assert result["storage_class"] == "F"
-    assert "uri" in result
 
     # Delete file
     file_service.delete_file(identity_simple, recid, "article.txt")
     with pytest.raises(FileKeyNotFoundError):
         result = file_service.read_file_metadata(identity_simple, recid, "article.txt")
 
     # Assert deleted
@@ -431,26 +433,24 @@
     assert result.to_dict()["entries"][0]["key"] == file_to_initialise[0]["key"]
 
     # Check it is still external
     result = file_service.read_file_metadata(identity_simple, recid, "article.txt")
     result = result.to_dict()
     assert result["key"] == file_to_initialise[0]["key"]
     assert result["storage_class"] == "F"
-    assert "uri" in result
 
     # List files
     result = file_service.list_files(identity_simple, recid)
     assert result.to_dict()["entries"][0]["key"] == file_to_initialise[0]["key"]
 
     # Read file metadata
     result = file_service.read_file_metadata(identity_simple, recid, "article.txt")
     result = result.to_dict()
     assert result["key"] == file_to_initialise[0]["key"]
     assert result["storage_class"] == "F"  # changed after commit
-    assert "uri" in result
 
     # Retrieve file
     with pytest.raises(PermissionDeniedError):
         file_service.get_file_content(identity_simple, recid, "article.txt")
 
 
 @pytest.mark.parametrize("allow_empty_files", [True, False])
```

### Comparing `invenio-records-resources-5.6.0/tests/services/files/test_files_options.py` & `invenio-records-resources-5.7.0/tests/services/files/test_files_options.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/files/test_files_processing.py` & `invenio-records-resources-5.7.0/tests/services/files/test_files_processing.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/files/testimage.png` & `invenio-records-resources-5.7.0/tests/services/files/testimage.png`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/test_results.py` & `invenio-records-resources-5.7.0/tests/services/test_results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/test_results_expand.py` & `invenio-records-resources-5.7.0/tests/services/test_results_expand.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/test_service.py` & `invenio-records-resources-5.7.0/tests/services/test_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/test_service_create.py` & `invenio-records-resources-5.7.0/tests/services/test_service_create.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/test_service_facets.py` & `invenio-records-resources-5.7.0/tests/services/test_service_facets.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/test_service_pagination.py` & `invenio-records-resources-5.7.0/tests/services/test_service_pagination.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/test_service_queryparser.py` & `invenio-records-resources-5.7.0/tests/services/test_service_queryparser.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/test_service_relation_propagation.py` & `invenio-records-resources-5.7.0/tests/services/test_service_relation_propagation.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/test_service_revision_id.py` & `invenio-records-resources-5.7.0/tests/services/test_service_revision_id.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/test_service_sort.py` & `invenio-records-resources-5.7.0/tests/services/test_service_sort.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/services/test_utils.py` & `invenio-records-resources-5.7.0/tests/services/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/test_invenio_resources.py` & `invenio-records-resources-5.7.0/tests/test_invenio_resources.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.6.0/tests/test_tasks.py` & `invenio-records-resources-5.7.0/tests/test_tasks.py`

 * *Files identical despite different names*

