# Comparing `tmp/adafruit_circuitpython_esp32spi-8.1.0.tar.gz` & `tmp/adafruit_circuitpython_esp32spi-8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_esp32spi-8.1.0.tar", last modified: Fri May  3 02:15:49 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_esp32spi-8.1.1.tar", last modified: Mon May  6 14:31:54 2024, max compression
```

## Comparing `adafruit_circuitpython_esp32spi-8.1.0.tar` & `adafruit_circuitpython_esp32spi-8.1.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.488589 adafruit_circuitpython_esp32spi-8.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.492589 adafruit_circuitpython_esp32spi-8.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.492589 adafruit_circuitpython_esp32spi-8.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.492589 adafruit_circuitpython_esp32spi-8.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-03 02:15:49.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-03 02:15:49.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:15:49.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-03 02:15:49.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 02:15:49.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.496589 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3180 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/PWMOut.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39665 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/adafruit_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/adafruit_esp32spi_socketpool.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13198 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6293 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/digitalio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.496589 adafruit_circuitpython_esp32spi-8.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.496589 adafruit_circuitpython_esp32spi-8.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_cheerlights.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_ipconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_localtime.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_settings.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_simpletest_rp2040.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_tcp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_udp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_wpa2ent_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_wpa2ent_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/examples/gpio/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/gpio/esp32spi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/gpio/gpio.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/examples/server/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/examples/server/esp32spi_wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-03 02:15:46.000000 adafruit_circuitpython_esp32spi-8.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-03 02:15:38.000000 adafruit_circuitpython_esp32spi-8.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:15:49.500589 adafruit_circuitpython_esp32spi-8.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:54.643512 adafruit_circuitpython_esp32spi-8.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:54.631512 adafruit_circuitpython_esp32spi-8.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:54.635512 adafruit_circuitpython_esp32spi-8.1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:54.635512 adafruit_circuitpython_esp32spi-8.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:54.635512 adafruit_circuitpython_esp32spi-8.1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-06 14:31:54.643512 adafruit_circuitpython_esp32spi-8.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:54.639512 adafruit_circuitpython_esp32spi-8.1.1/adafruit_circuitpython_esp32spi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-06 14:31:54.000000 adafruit_circuitpython_esp32spi-8.1.1/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-06 14:31:54.000000 adafruit_circuitpython_esp32spi-8.1.1/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:31:54.000000 adafruit_circuitpython_esp32spi-8.1.1/adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-06 14:31:54.000000 adafruit_circuitpython_esp32spi-8.1.1/adafruit_circuitpython_esp32spi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 14:31:54.000000 adafruit_circuitpython_esp32spi-8.1.1/adafruit_circuitpython_esp32spi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:54.639512 adafruit_circuitpython_esp32spi-8.1.1/adafruit_esp32spi/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3180 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/adafruit_esp32spi/PWMOut.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/adafruit_esp32spi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39665 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/adafruit_esp32spi/adafruit_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/adafruit_esp32spi/adafruit_esp32spi_socketpool.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13198 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6293 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/adafruit_esp32spi/digitalio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:54.639512 adafruit_circuitpython_esp32spi-8.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:54.639512 adafruit_circuitpython_esp32spi-8.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:54.639512 adafruit_circuitpython_esp32spi-8.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_cheerlights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_ipconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_localtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_settings.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_simpletest_rp2040.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_tcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_udp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_wpa2ent_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_wpa2ent_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:54.639512 adafruit_circuitpython_esp32spi-8.1.1/examples/gpio/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/gpio/esp32spi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/gpio/gpio.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:54.639512 adafruit_circuitpython_esp32spi-8.1.1/examples/server/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/examples/server/esp32spi_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-06 14:31:52.000000 adafruit_circuitpython_esp32spi-8.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 14:31:45.000000 adafruit_circuitpython_esp32spi-8.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 14:31:54.643512 adafruit_circuitpython_esp32spi-8.1.1/setup.cfg
```

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_esp32spi-8.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/.gitignore` & `adafruit_circuitpython_esp32spi-8.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/.pre-commit-config.yaml` & `adafruit_circuitpython_esp32spi-8.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/.pylintrc` & `adafruit_circuitpython_esp32spi-8.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_esp32spi-8.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/LICENSE` & `adafruit_circuitpython_esp32spi-8.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_esp32spi-8.1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/LICENSES/MIT.txt` & `adafruit_circuitpython_esp32spi-8.1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_esp32spi-8.1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/PKG-INFO` & `adafruit_circuitpython_esp32spi-8.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32spi
-Version: 8.1.0
+Version: 8.1.1
 Summary: CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
 Keywords: adafruit,blinka,circuitpython,micropython,esp32spi,wifi,esp32
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/README.rst` & `adafruit_circuitpython_esp32spi-8.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO` & `adafruit_circuitpython_esp32spi-8.1.1/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32spi
-Version: 8.1.0
+Version: 8.1.1
 Summary: CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
 Keywords: adafruit,blinka,circuitpython,micropython,esp32spi,wifi,esp32
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt` & `adafruit_circuitpython_esp32spi-8.1.1/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/PWMOut.py` & `adafruit_circuitpython_esp32spi-8.1.1/adafruit_esp32spi/PWMOut.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/adafruit_esp32spi.py` & `adafruit_circuitpython_esp32spi-8.1.1/adafruit_esp32spi/adafruit_esp32spi.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import struct
 import time
 from micropython import const
 from adafruit_bus_device.spi_device import SPIDevice
 from digitalio import Direction
 
-__version__ = "8.1.0"
+__version__ = "8.1.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI.git"
 
 _SET_NET_CMD = const(0x10)
 _SET_PASSPHRASE_CMD = const(0x11)
 _SET_IP_CONFIG = const(0x14)
 _SET_DNS_CONFIG = const(0x15)
 _SET_HOSTNAME = const(0x16)
```

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/adafruit_esp32spi_socketpool.py` & `adafruit_circuitpython_esp32spi-8.1.1/adafruit_esp32spi/adafruit_esp32spi_socketpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,24 +104,28 @@
 
     def connect(self, address, conntype=None):
         """Connect the socket to the 'address' (which can be 32bit packed IP or
         a hostname string). 'conntype' is an extra that may indicate SSL or not,
         depending on the underlying interface"""
         host, port = address
         if conntype is None:
-            conntype = self._interface.TCP_MODE
+            conntype = (
+                self._interface.UDP_MODE
+                if self._type == SocketPool.SOCK_DGRAM
+                else self._interface.TCP_MODE
+            )
         if not self._interface.socket_connect(
             self._socknum, host, port, conn_mode=conntype
         ):
             raise ConnectionError("Failed to connect to host", host)
         self._buffer = b""
 
     def send(self, data):
         """Send some data to the socket."""
-        if self._type is SocketPool.SOCK_DGRAM:
+        if self._type == SocketPool.SOCK_DGRAM:
             conntype = self._interface.UDP_MODE
         else:
             conntype = self._interface.TCP_MODE
         self._interface.socket_write(self._socknum, data, conn_mode=conntype)
         gc.collect()
 
     def recv(self, bufsize: int) -> bytes:
```

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py` & `adafruit_circuitpython_esp32spi-8.1.1/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/adafruit_esp32spi/digitalio.py` & `adafruit_circuitpython_esp32spi-8.1.1/adafruit_esp32spi/digitalio.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/docs/_static/favicon.ico` & `adafruit_circuitpython_esp32spi-8.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/docs/api.rst` & `adafruit_circuitpython_esp32spi-8.1.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/docs/conf.py` & `adafruit_circuitpython_esp32spi-8.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/docs/index.rst` & `adafruit_circuitpython_esp32spi-8.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_aio_post.py` & `adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_cheerlights.py` & `adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_ipconfig.py` & `adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_ipconfig.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_localtime.py` & `adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_localtime.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_settings.toml` & `adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_settings.toml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_simpletest.py` & `adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_simpletest_rp2040.py` & `adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_simpletest_rp2040.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_tcp_client.py` & `adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_tcp_client.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_udp_client.py` & `adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_udp_client.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_wpa2ent_aio_post.py` & `adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_wpa2ent_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/esp32spi_wpa2ent_simpletest.py` & `adafruit_circuitpython_esp32spi-8.1.1/examples/esp32spi_wpa2ent_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/gpio/esp32spi_gpio.py` & `adafruit_circuitpython_esp32spi-8.1.1/examples/gpio/esp32spi_gpio.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/examples/gpio/gpio.md` & `adafruit_circuitpython_esp32spi-8.1.1/examples/gpio/gpio.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.1.0/pyproject.toml` & `adafruit_circuitpython_esp32spi-8.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-esp32spi"
 description = "CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI"
-version = "8.1.0"
+version = "8.1.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI"}
 keywords = [
     "adafruit",
```
