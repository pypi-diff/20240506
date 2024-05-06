# Comparing `tmp/adafruit_circuitpython_avrprog-1.5.0.tar.gz` & `tmp/adafruit_circuitpython_avrprog-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_avrprog-1.5.0.tar", last modified: Sun Apr 21 13:48:04 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_avrprog-1.5.1.tar", last modified: Mon May  6 20:13:16 2024, max compression
```

## Comparing `adafruit_circuitpython_avrprog-1.5.0.tar` & `adafruit_circuitpython_avrprog-1.5.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.037680 adafruit_circuitpython_avrprog-1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.029680 adafruit_circuitpython_avrprog-1.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.033680 adafruit_circuitpython_avrprog-1.5.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.033680 adafruit_circuitpython_avrprog-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.033680 adafruit_circuitpython_avrprog-1.5.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-21 13:48:04.037680 adafruit_circuitpython_avrprog-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)    18395 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/adafruit_avrprog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.037680 adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-21 13:48:04.000000 adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-21 13:48:04.000000 adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:48:04.000000 adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-21 13:48:04.000000 adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 13:48:04.000000 adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.033680 adafruit_circuitpython_avrprog-1.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.037680 adafruit_circuitpython_avrprog-1.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:48:04.037680 adafruit_circuitpython_avrprog-1.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/attiny13a_blink.hex
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/attiny13a_blink.hex.license
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_mega2560.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_tiny13a.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_trinket85.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_uno328.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_read_signature_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/optiboot_atmega328.hex
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/optiboot_atmega328.hex.license
--rw-r--r--   0 runner    (1001) docker     (127)    20548 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/stk500boot_v2_mega2560.hex
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/stk500boot_v2_mega2560.hex.license
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/trinket_boot.hex
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/examples/trinket_boot.hex.license
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-21 13:48:01.000000 adafruit_circuitpython_avrprog-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-21 13:47:55.000000 adafruit_circuitpython_avrprog-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:48:04.037680 adafruit_circuitpython_avrprog-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:13:16.841166 adafruit_circuitpython_avrprog-1.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:13:16.833166 adafruit_circuitpython_avrprog-1.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:13:16.837166 adafruit_circuitpython_avrprog-1.5.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:13:16.837166 adafruit_circuitpython_avrprog-1.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:13:16.837166 adafruit_circuitpython_avrprog-1.5.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-06 20:13:16.841166 adafruit_circuitpython_avrprog-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)    20318 2024-05-06 20:13:14.000000 adafruit_circuitpython_avrprog-1.5.1/adafruit_avrprog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:13:16.841166 adafruit_circuitpython_avrprog-1.5.1/adafruit_circuitpython_avrprog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-06 20:13:16.000000 adafruit_circuitpython_avrprog-1.5.1/adafruit_circuitpython_avrprog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-06 20:13:16.000000 adafruit_circuitpython_avrprog-1.5.1/adafruit_circuitpython_avrprog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:13:16.000000 adafruit_circuitpython_avrprog-1.5.1/adafruit_circuitpython_avrprog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 20:13:16.000000 adafruit_circuitpython_avrprog-1.5.1/adafruit_circuitpython_avrprog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 20:13:16.000000 adafruit_circuitpython_avrprog-1.5.1/adafruit_circuitpython_avrprog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:13:16.837166 adafruit_circuitpython_avrprog-1.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:13:16.837166 adafruit_circuitpython_avrprog-1.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:13:16.841166 adafruit_circuitpython_avrprog-1.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/examples/attiny13a_blink.hex
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/examples/attiny13a_blink.hex.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-06 20:13:14.000000 adafruit_circuitpython_avrprog-1.5.1/examples/avrprog_program_mega2560.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-06 20:13:14.000000 adafruit_circuitpython_avrprog-1.5.1/examples/avrprog_program_tiny13a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-06 20:13:14.000000 adafruit_circuitpython_avrprog-1.5.1/examples/avrprog_program_trinket85.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-06 20:13:14.000000 adafruit_circuitpython_avrprog-1.5.1/examples/avrprog_program_uno328.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-06 20:13:14.000000 adafruit_circuitpython_avrprog-1.5.1/examples/avrprog_read_signature_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/examples/optiboot_atmega328.hex
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/examples/optiboot_atmega328.hex.license
+-rw-r--r--   0 runner    (1001) docker     (127)    20548 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/examples/stk500boot_v2_mega2560.hex
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/examples/stk500boot_v2_mega2560.hex.license
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/examples/trinket_boot.hex
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/examples/trinket_boot.hex.license
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-06 20:13:14.000000 adafruit_circuitpython_avrprog-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 20:13:07.000000 adafruit_circuitpython_avrprog-1.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:13:16.841166 adafruit_circuitpython_avrprog-1.5.1/setup.cfg
```

### Comparing `adafruit_circuitpython_avrprog-1.5.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_avrprog-1.5.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/.gitignore` & `adafruit_circuitpython_avrprog-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/.pre-commit-config.yaml` & `adafruit_circuitpython_avrprog-1.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/.pylintrc` & `adafruit_circuitpython_avrprog-1.5.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_avrprog-1.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/LICENSE` & `adafruit_circuitpython_avrprog-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_avrprog-1.5.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/LICENSES/MIT.txt` & `adafruit_circuitpython_avrprog-1.5.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_avrprog-1.5.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/PKG-INFO` & `adafruit_circuitpython_avrprog-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-avrprog
-Version: 1.5.0
+Version: 1.5.1
 Summary: CircuitPython helper library for programming AVR chips.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AVRprog
 Keywords: adafruit,avr,spi,atmega,attiny,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_avrprog-1.5.0/README.rst` & `adafruit_circuitpython_avrprog-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/adafruit_avrprog.py` & `adafruit_circuitpython_avrprog-1.5.1/adafruit_avrprog.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,21 +25,63 @@
 * Adafruit CircuitPython firmware for the ESP8622 and M0-based boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 # imports
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_AVRprog.git"
 
-from digitalio import Direction, DigitalInOut
+try:
+    from typing import List, Optional, Tuple, Union, TypedDict
+    from typing_extensions import TypeAlias
+    from os import PathLike
+    from busio import SPI
+    from microcontroller import Pin
 
-_SLOW_CLOCK = 100000
-_FAST_CLOCK = 1000000
+    # Technically this type should come from: from _typeshed import FileDescriptorOrPath
+    # Unfortunately _typeshed is only in the standard library in newer releases of Python, e.g. 3.11
+    # Thus have to define a placeholder
+    FileDescriptorOrPath: TypeAlias = Union[
+        int, str, bytes, PathLike[str], PathLike[bytes]
+    ]
+
+    from io import TextIOWrapper
+
+    class ChipDictionary(TypedDict):
+        """
+        Dictionary representing a specific target chip type
+        """
+
+        name: str
+        sig: List[int]
+        flash_size: int
+        page_size: int
+        fuse_mask: Tuple[int, int, int, int]
+
+    class FileState(TypedDict):
+        """
+        Dictionary representing a File State
+        """
+
+        # pylint: disable=invalid-name
+        line: int
+        ext_addr: int
+        eof: bool
+        f: Optional[TextIOWrapper]
+
+except ImportError:
+    pass
+
+
+from digitalio import DigitalInOut, Direction
+
+_SLOW_CLOCK: int = 100000
+_FAST_CLOCK: int = 1000000
 
 
 class AVRprog:
     """
     Helper class used to program AVR chips from CircuitPython.
     """
 
@@ -89,44 +131,50 @@
             "name": "ATmega2560",
             "sig": [0x1E, 0x98, 0x01],
             "flash_size": 262144,
             "page_size": 256,
             "fuse_mask": (0xFF, 0xFF, 0x07, 0x3F),
         }
 
-    _spi = None
-    _rst = None
+    _spi: Optional[SPI] = None
+    _rst: Optional[DigitalInOut] = None
 
-    def init(self, spi_bus, rst_pin):
+    def init(self, spi_bus: SPI, rst_pin: Pin) -> None:
         """
         Initialize the programmer with an SPI port that will be used to
         communicate with the chip. Make sure your SPI supports 'write_readinto'
         Also pass in a reset pin that will be used to get into programming mode
         """
         self._spi = spi_bus
         self._rst = DigitalInOut(rst_pin)
         self._rst.direction = Direction.OUTPUT
         self._rst.value = True
 
-    def verify_sig(self, chip, verbose=False):
+    def verify_sig(self, chip: ChipDictionary, verbose: bool = False) -> bool:
         """
         Verify that the chip is connected properly, responds to commands,
         and has the correct signature. Returns True/False based on success
         """
         self.begin(clock=_SLOW_CLOCK)
         sig = self.read_signature()
         self.end()
         if verbose:
             print("Found signature: %s" % [hex(i) for i in sig])
         if sig != chip["sig"]:
             return False
         return True
 
     # pylint: disable=too-many-branches
-    def program_file(self, chip, file_name, verbose=False, verify=True):
+    def program_file(
+        self,
+        chip: ChipDictionary,
+        file_name: FileDescriptorOrPath,
+        verbose: bool = False,
+        verify: bool = True,
+    ) -> bool:
         """
         Perform a chip erase and program from a file that
         contains Intel HEX data. Returns true on verify-success, False on
         verify-failure. If 'verify' is False, return will always be True
         """
         if not self.verify_sig(chip):
             raise RuntimeError("Signature read failure")
@@ -135,18 +183,16 @@
             print("Erasing chip....")
         self.erase_chip()
 
         clock_speed = chip.get("clock_speed", _FAST_CLOCK)
         self.begin(clock=clock_speed)
 
         # create a file state dictionary
-        file_state = {"line": 0, "ext_addr": 0, "eof": False}
-        with open(file_name, "r") as file_state[  # pylint: disable=unspecified-encoding
-            "f"
-        ]:
+        file_state = {"line": 0, "ext_addr": 0, "eof": False, "f": None}
+        with open(file_name, "r") as file_state["f"]:
             page_size = chip["page_size"]
 
             for page_addr in range(0, chip["flash_size"], page_size):
                 if verbose:
                     print("Programming page $%04X..." % page_addr, end="")
                 page_buffer = bytearray(page_size)
                 for b in range(page_size):
@@ -186,27 +232,30 @@
 
                 if file_state["eof"]:
                     break  # we're done, bail!
 
         self.end()
         return True
 
-    def verify_file(self, chip, file_name, verbose=False):
+    def verify_file(
+        self,
+        chip: ChipDictionary,
+        file_name: FileDescriptorOrPath,
+        verbose: bool = False,
+    ) -> bool:
         """
         Perform a chip full-flash verification from a file that
         contains Intel HEX data. Returns True/False on success/fail.
         """
         if not self.verify_sig(chip):
             raise RuntimeError("Signature read failure")
 
         # create a file state dictionary
-        file_state = {"line": 0, "ext_addr": 0, "eof": False}
-        with open(file_name, "r") as file_name[  # pylint: disable=unspecified-encoding
-            "f"
-        ]:
+        file_state = {"line": 0, "ext_addr": 0, "eof": False, "f": None}
+        with open(file_name, "r") as file_state["f"]:
             page_size = chip["page_size"]
             clock_speed = chip.get("clock_speed", _FAST_CLOCK)
             self.begin(clock=clock_speed)
             for page_addr in range(0x0, chip["flash_size"], page_size):
                 page_buffer = bytearray(page_size)
                 for b in range(page_size):
                     page_buffer[b] = 0xFF  # make an empty page
@@ -233,100 +282,114 @@
 
                 if file_state["eof"]:
                     break  # we're done, bail!
 
         self.end()
         return True
 
-    def read_fuses(self, chip):
+    def read_fuses(self, chip: ChipDictionary) -> Tuple[int, int, int, int]:
         """
-        Read the 4 fuses and return them in a list (low, high, ext, lock)
+        Read the 4 fuses and return them in a tuple (low, high, ext, lock)
         Each fuse is bitwise-&'s with the chip's fuse mask for simplicity
         """
-        mask = chip["fuse_mask"]
+        mask: Tuple[int, int, int, int] = chip["fuse_mask"]
         self.begin(clock=_SLOW_CLOCK)
         low = self._transaction((0x50, 0, 0, 0))[2] & mask[0]
         high = self._transaction((0x58, 0x08, 0, 0))[2] & mask[1]
         ext = self._transaction((0x50, 0x08, 0, 0))[2] & mask[2]
         lock = self._transaction((0x58, 0, 0, 0))[2] & mask[3]
         self.end()
         return (low, high, ext, lock)
 
     # pylint: disable=unused-argument,too-many-arguments
-    def write_fuses(self, chip, low=None, high=None, ext=None, lock=None):
+    def write_fuses(
+        self,
+        chip: ChipDictionary,
+        low: Optional[int] = None,
+        high: Optional[int] = None,
+        ext: Optional[int] = None,
+        lock: Optional[int] = None,
+    ) -> None:
         """
         Write any of the 4 fuses. If the kwarg low/high/ext/lock is not
         passed in or is None, that fuse is skipped
         """
         transaction_comp = (0xE0, 0xA0, 0xA8, 0xA4)
         fuses = (lock, low, high, ext)
         self.begin(clock=_SLOW_CLOCK)
         for fuse, comp in zip(fuses, transaction_comp):
             if fuse:
                 self._transaction((0xAC, comp, 0, fuse))
             self._busy_wait()
         self.end()
 
     # pylint: disable=too-many-arguments
-    def verify_fuses(self, chip, low=None, high=None, ext=None, lock=None):
+    def verify_fuses(
+        self,
+        chip: ChipDictionary,
+        low: Optional[int] = None,
+        high: Optional[int] = None,
+        ext: Optional[int] = None,
+        lock: Optional[int] = None,
+    ) -> bool:
         """
         Verify the 4 fuses. If the kwarg low/high/ext/lock is not
         passed in or is None, that fuse is not checked.
         Each fuse is bitwise-&'s with the chip's fuse mask.
         Returns True on success, False on a fuse verification failure
         """
         fuses = self.read_fuses(chip)
         verify = (low, high, ext, lock)
         for i in range(4):
             # check each fuse if we requested to check it!
             if verify[i] and verify[i] != fuses[i]:
                 return False
         return True
 
-    def erase_chip(self):
+    def erase_chip(self) -> None:
         """
         Fully erases the chip.
         """
         self.begin(clock=_SLOW_CLOCK)
         self._transaction((0xAC, 0x80, 0, 0))
         self._busy_wait()
         self.end()
 
     #################### Mid level
 
-    def begin(self, clock=_FAST_CLOCK):
+    def begin(self, clock: int = _FAST_CLOCK) -> None:
         """
         Begin programming mode: pull reset pin low, initialize SPI, and
         send the initialization command to get the AVR's attention.
         """
         self._rst.value = False
         while self._spi and not self._spi.try_lock():
             pass
         self._spi.configure(baudrate=clock)
         self._transaction((0xAC, 0x53, 0, 0))
 
-    def end(self):
+    def end(self) -> None:
         """
         End programming mode: SPI is released, and reset pin set high.
         """
         self._spi.unlock()
         self._rst.value = True
 
-    def read_signature(self):
+    def read_signature(self) -> List[int]:
         """
         Read and return the signature of the chip as two bytes in an array.
         Requires calling begin() beforehand to put in programming mode.
         """
         # signature is last byte of two transactions:
         sig = []
         for i in range(3):
             sig.append(self._transaction((0x30, 0, i, 0))[2])
         return sig
 
-    def read(self, addr, read_buffer):
+    def read(self, addr: int, read_buffer: bytearray) -> None:
         """
         Read a chunk of memory from address 'addr'. The amount read is the
         same as the size of the bytearray 'read_buffer'. Data read is placed
         directly into 'read_buffer'
         Requires calling begin() beforehand to put in programming mode.
         """
         last_addr = 0
@@ -342,49 +405,53 @@
             # print("%04X: %02X %02X" % (read_addr*2, low, high))
             read_buffer[i * 2] = low
             read_buffer[i * 2 + 1] = high
 
             last_addr = read_addr
 
     #################### Low level
-    def _flash_word(self, addr, low, high):
+    def _flash_word(self, addr: int, low: int, high: int) -> None:
         self._transaction((0x40, addr >> 8, addr, low))
         self._transaction((0x48, addr >> 8, addr, high))
 
-    def _flash_page(self, page_buffer, page_addr, page_size):
+    def _flash_page(
+        self, page_buffer: bytearray, page_addr: int, page_size: int
+    ) -> None:
         page_addr //= 2  # address is by 'words' not bytes!
-        for i in range(page_size / 2):  # page indexed by words, not bytes
+        for i in range(page_size // 2):  # page indexed by words, not bytes
             lo_byte, hi_byte = page_buffer[2 * i : 2 * i + 2]
             self._flash_word(i, lo_byte, hi_byte)
 
         # load extended byte
         self._transaction((0x4D, 0, page_addr >> 16, 0))
 
         commit_reply = self._transaction((0x4C, page_addr >> 8, page_addr, 0))
         if ((commit_reply[1] << 8) + commit_reply[2]) != (page_addr & 0xFFFF):
             raise RuntimeError("Failed to commit page to flash")
         self._busy_wait()
 
-    def _transaction(self, command):
+    def _transaction(self, command: Tuple[int, int, int, int]) -> bytearray:
         reply = bytearray(4)
-        command = bytearray([i & 0xFF for i in command])
+        command_bytes = bytearray([i & 0xFF for i in command])
 
-        self._spi.write_readinto(command, reply)
-        # s = [hex(i) for i in command]
-        # print("Sending %s reply %s" % ([hex(i) for i in command], [hex(i) for i in reply]))
-        if reply[2] != command[1]:
+        self._spi.write_readinto(command_bytes, reply)
+        # s = [hex(i) for i in command_bytes]
+        # print("Sending %s reply %s" % ([hex(i) for i in command_bytes], [hex(i) for i in reply]))
+        if reply[2] != command_bytes[1]:
             raise RuntimeError("SPI transaction failed")
         return reply[1:]  # first byte is ignored
 
-    def _busy_wait(self):
+    def _busy_wait(self) -> None:
         while self._transaction((0xF0, 0, 0, 0))[2] & 0x01:
             pass
 
 
-def read_hex_page(file_state, page_addr, page_size, page_buffer):
+def read_hex_page(
+    file_state: FileState, page_addr: int, page_size: int, page_buffer: bytearray
+) -> bool:
     # pylint: disable=too-many-branches
     """
     Helper function that does the Intel Hex parsing. Takes in a dictionary
     that contains the file 'state'. The dictionary should have file_state['f']
     be the file stream object (returned by open), the file_state['line'] which
     tracks the line number of the file for better debug messages. This function
     will update 'line' as it reads lines. It will set 'eof' when the file has
```

### Comparing `adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/PKG-INFO` & `adafruit_circuitpython_avrprog-1.5.1/adafruit_circuitpython_avrprog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-avrprog
-Version: 1.5.0
+Version: 1.5.1
 Summary: CircuitPython helper library for programming AVR chips.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AVRprog
 Keywords: adafruit,avr,spi,atmega,attiny,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_avrprog-1.5.0/adafruit_circuitpython_avrprog.egg-info/SOURCES.txt` & `adafruit_circuitpython_avrprog-1.5.1/adafruit_circuitpython_avrprog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/docs/_static/favicon.ico` & `adafruit_circuitpython_avrprog-1.5.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/docs/conf.py` & `adafruit_circuitpython_avrprog-1.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/docs/examples.rst` & `adafruit_circuitpython_avrprog-1.5.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/docs/index.rst` & `adafruit_circuitpython_avrprog-1.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_mega2560.py` & `adafruit_circuitpython_avrprog-1.5.1/examples/avrprog_program_mega2560.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_tiny13a.py` & `adafruit_circuitpython_avrprog-1.5.1/examples/avrprog_program_tiny13a.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_trinket85.py` & `adafruit_circuitpython_avrprog-1.5.1/examples/avrprog_program_trinket85.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_program_uno328.py` & `adafruit_circuitpython_avrprog-1.5.1/examples/avrprog_program_uno328.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/examples/avrprog_read_signature_simpletest.py` & `adafruit_circuitpython_avrprog-1.5.1/examples/avrprog_read_signature_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/examples/optiboot_atmega328.hex` & `adafruit_circuitpython_avrprog-1.5.1/examples/optiboot_atmega328.hex`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/examples/stk500boot_v2_mega2560.hex` & `adafruit_circuitpython_avrprog-1.5.1/examples/stk500boot_v2_mega2560.hex`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/examples/trinket_boot.hex` & `adafruit_circuitpython_avrprog-1.5.1/examples/trinket_boot.hex`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_avrprog-1.5.0/pyproject.toml` & `adafruit_circuitpython_avrprog-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-avrprog"
 description = "CircuitPython helper library for programming AVR chips."
-version = "1.5.0"
+version = "1.5.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_AVRprog"}
 keywords = [
     "adafruit",
```

