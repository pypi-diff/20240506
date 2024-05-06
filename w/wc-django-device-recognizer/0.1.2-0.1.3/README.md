# Comparing `tmp/wc-django-device-recognizer-0.1.2.tar.gz` & `tmp/wc-django-device-recognizer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-device-recognizer-0.1.2.tar", last modified: Thu Apr 25 08:24:19 2024, max compression
+gzip compressed data, was "wc-django-device-recognizer-0.1.3.tar", last modified: Mon May  6 15:15:38 2024, max compression
```

## Comparing `wc-django-device-recognizer-0.1.2.tar` & `wc-django-device-recognizer-0.1.3.tar`

### file list

```diff
@@ -1,377 +1,377 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      335 2024-04-25 08:22:20.000000 wc-django-device-recognizer-0.1.2/CHANGELOG.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1072 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/LICENSE
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      163 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/MANIFEST.in
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1254 2024-04-25 08:24:06.000000 wc-django-device-recognizer-0.1.2/Makefile
--rw-r--r--   0 preusx    (1000) preusx    (1000)     2945 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/PKG-INFO
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1638 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/README.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/setup.cfg
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1628 2024-04-25 08:03:50.000000 wc-django-device-recognizer-0.1.2/setup.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.381945 wc-django-device-recognizer-0.1.2/tests/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     2871 2024-04-25 08:21:10.000000 wc-django-device-recognizer-0.1.2/tests/test_registry.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     2444 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/tests/test_request_resolver.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      562 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/
--rw-r--r--   0 preusx    (1000) preusx    (1000)     2945 2024-04-25 08:24:19.000000 wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/PKG-INFO
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)    10091 2024-04-25 08:24:19.000000 wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/SOURCES.txt
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)        1 2024-04-25 08:24:19.000000 wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/dependency_links.txt
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      171 2024-04-25 08:24:19.000000 wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/requires.txt
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       22 2024-04-25 08:24:19.000000 wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.381945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      131 2024-04-25 08:21:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/__init__.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1527 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/admin.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      352 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/apps.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      259 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/conf.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       82 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/const.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       57 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/discovery.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1138 2024-04-25 07:57:05.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/dtos.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.381945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/af/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/af/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/af/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/af/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ar/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      463 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ar/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3562 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ar/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ast/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ast/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ast/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ast/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/az/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/az/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/az/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/az/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/be/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/be/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/be/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3620 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/be/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bg/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bg/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bg/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/br/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/br/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      671 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/br/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3779 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/br/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bs/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bs/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bs/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3553 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bs/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ca/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ca/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ca/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ca/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cs/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      460 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cs/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3559 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      425 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3524 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/da/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/da/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/da/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/da/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/de/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/de/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/dsb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/dsb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/dsb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3531 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/dsb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/el/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.385945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/el/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/el/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/el/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/en/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/en/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eo/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eo/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eo/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eo/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/es/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/es/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/et/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/et/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/et/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/et/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.369946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eu/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eu/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eu/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eu/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fa/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fa/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fa/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3475 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fa/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3475 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ga/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ga/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      418 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ga/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3517 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ga/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gd/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gd/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      441 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gd/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3540 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gd/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/he/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/he/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/he/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3573 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/he/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      452 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3551 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hsb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.389945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hsb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hsb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3531 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hsb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hu/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hu/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hu/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hu/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hy/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hy/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hy/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hy/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ia/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ia/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ia/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ia/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/id/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/id/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ig/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ig/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ig/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ig/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/io/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/io/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/io/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/io/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/is/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/is/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      402 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/is/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3498 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/is/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/it/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/it/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ja/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ja/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ka/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ka/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ka/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3474 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ka/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kab/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kab/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kab/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kab/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3474 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/km/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/km/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/km/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/km/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3475 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ko/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ky/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.393945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ky/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ky/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ky/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      511 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3613 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.373946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lv/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lv/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lv/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3514 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lv/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      410 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3506 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ml/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ml/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ml/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ml/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ms/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ms/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ms/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ms/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/my/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/my/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/my/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/my/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nb/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nb/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nb/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nb/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ne/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ne/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ne/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ne/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nn/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nn/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nn/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nn/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/os/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/os/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/os/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/os/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pa/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pa/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pa/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pa/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.397945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      526 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3628 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ro/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ro/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      421 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ro/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3520 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ro/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ru/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3620 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      455 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3554 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sl/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sl/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sl/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3531 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sl/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sq/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sq/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sq/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sq/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3553 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sv/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sw/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sw/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sw/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sw/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ta/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ta/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ta/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ta/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/te/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/te/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/te/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/te/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tg/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tg/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tg/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tg/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/th/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/th/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/th/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/th/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tr/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tr/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3475 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tr/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tt/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.401945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tt/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tt/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tt/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/udm/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/udm/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/udm/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/udm/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.377946 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uk/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      602 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3707 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.381945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ur/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ur/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ur/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3476 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ur/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.381945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uz/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uz/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uz/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uz/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.381945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/vi/
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/vi/LC_MESSAGES/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/vi/LC_MESSAGES/django.mo
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3469 2024-04-25 08:24:08.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/vi/LC_MESSAGES/django.po
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/migrations/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     5876 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/migrations/0001_initial.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/migrations/__init__.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     5795 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/models.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-04-25 08:24:19.405945 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/services/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/services/__init__.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     2558 2024-04-25 08:00:59.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/services/registry.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     5000 2024-04-25 07:58:53.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/services/request_resolver.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1478 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.2/wcd_device_recognizer/utils.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.684877 wc-django-device-recognizer-0.1.3/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      335 2024-04-25 08:22:20.000000 wc-django-device-recognizer-0.1.3/CHANGELOG.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1072 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/LICENSE
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      163 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/MANIFEST.in
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1254 2024-04-25 08:24:06.000000 wc-django-device-recognizer-0.1.3/Makefile
+-rw-r--r--   0 preusx    (1000) preusx    (1000)     2945 2024-05-06 15:15:38.684877 wc-django-device-recognizer-0.1.3/PKG-INFO
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1638 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/README.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2024-05-06 15:15:38.684877 wc-django-device-recognizer-0.1.3/setup.cfg
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1628 2024-04-25 08:03:50.000000 wc-django-device-recognizer-0.1.3/setup.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/tests/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     2871 2024-04-25 08:21:10.000000 wc-django-device-recognizer-0.1.3/tests/test_registry.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     2444 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/tests/test_request_resolver.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      562 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wc_django_device_recognizer.egg-info/
+-rw-r--r--   0 preusx    (1000) preusx    (1000)     2945 2024-05-06 15:15:38.000000 wc-django-device-recognizer-0.1.3/wc_django_device_recognizer.egg-info/PKG-INFO
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)    10091 2024-05-06 15:15:38.000000 wc-django-device-recognizer-0.1.3/wc_django_device_recognizer.egg-info/SOURCES.txt
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)        1 2024-05-06 15:15:38.000000 wc-django-device-recognizer-0.1.3/wc_django_device_recognizer.egg-info/dependency_links.txt
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      171 2024-05-06 15:15:38.000000 wc-django-device-recognizer-0.1.3/wc_django_device_recognizer.egg-info/requires.txt
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       22 2024-05-06 15:15:38.000000 wc-django-device-recognizer-0.1.3/wc_django_device_recognizer.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.660877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      131 2024-05-06 15:11:18.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     3114 2024-05-06 15:02:04.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/admin.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      352 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/apps.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      259 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/conf.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       82 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/const.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       57 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/discovery.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1138 2024-04-25 07:57:05.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/dtos.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/af/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.660877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/af/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/af/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/af/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ar/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.660877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      463 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3773 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ast/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.660877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ast/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ast/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ast/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/az/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.660877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/az/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/az/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/az/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/be/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.660877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/be/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/be/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3831 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/be/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.660877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.660877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/br/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.660877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/br/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      671 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/br/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3990 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/br/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.660877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bs/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3764 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ca/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.660877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ca/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ca/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ca/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/cs/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      460 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3770 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/cy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/cy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      425 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/cy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3735 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/cy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.644877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/da/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/da/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/da/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/da/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/de/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/dsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/dsb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/dsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3742 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/dsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/el/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/el/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/el/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/el/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/en/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/eo/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/eo/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/eo/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/eo/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/es/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/et/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/et/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/et/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/et/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/eu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/eu/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/eu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/eu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fa/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3686 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3686 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ga/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.664877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ga/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      418 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ga/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3728 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ga/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/gd/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/gd/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      441 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/gd/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3751 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/gd/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/gl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/gl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/gl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/gl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/he/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/he/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/he/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3784 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/he/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      452 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3762 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hsb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hsb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hsb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3742 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hsb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hu/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hu/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hu/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hy/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hy/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hy/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hy/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ia/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ia/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ia/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ia/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/id/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ig/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ig/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ig/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ig/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/io/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/io/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/io/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/io/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/is/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/is/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      402 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/is/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3709 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/is/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/it/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ja/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ka/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ka/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ka/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3685 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ka/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.648877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kab/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.668877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kab/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kab/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kab/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      378 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3685 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/km/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/km/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/km/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/km/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3686 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ko/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ky/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ky/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ky/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ky/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      511 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3824 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lv/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3725 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      410 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3717 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ml/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ml/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ml/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ml/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ms/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ms/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ms/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ms/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/my/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/my/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/my/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/my/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nb/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nb/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nb/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nb/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ne/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.672877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ne/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ne/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ne/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nn/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nn/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nn/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nn/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/os/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/os/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/os/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/os/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pa/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pa/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pa/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      526 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3839 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ro/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ro/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      421 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ro/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3731 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ro/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ru/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      518 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3831 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      455 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3765 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sl/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sl/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      432 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3742 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sl/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sq/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sq/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sq/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sq/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      454 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3764 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sv/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.652877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sw/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sw/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sw/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sw/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ta/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ta/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ta/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ta/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/te/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.676877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/te/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/te/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/te/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tg/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tg/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tg/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/th/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/th/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/th/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/th/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tr/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      379 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3686 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tr/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tt/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tt/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tt/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/udm/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/udm/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/udm/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/udm/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/uk/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      602 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3918 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ur/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ur/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      380 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ur/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3687 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ur/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/uz/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/uz/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/uz/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:48.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/uz/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.656877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/vi/
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/vi/LC_MESSAGES/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      373 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/vi/LC_MESSAGES/django.mo
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3680 2024-05-06 15:09:49.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/vi/LC_MESSAGES/django.po
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/migrations/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     5876 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/migrations/0001_initial.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/migrations/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     5795 2024-05-06 14:52:56.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/models.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2024-05-06 15:15:38.680877 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/services/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/services/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     2558 2024-04-25 08:00:59.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/services/registry.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     5000 2024-04-25 07:58:53.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/services/request_resolver.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1478 2022-09-20 08:50:23.000000 wc-django-device-recognizer-0.1.3/wcd_device_recognizer/utils.py
```

### Comparing `wc-django-device-recognizer-0.1.2/LICENSE` & `wc-django-device-recognizer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/Makefile` & `wc-django-device-recognizer-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/PKG-INFO` & `wc-django-device-recognizer-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-device-recognizer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django device recognizing utility.
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `wc-django-device-recognizer-0.1.2/README.md` & `wc-django-device-recognizer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/setup.py` & `wc-django-device-recognizer-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/tests/test_registry.py` & `wc-django-device-recognizer-0.1.3/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/tests/test_request_resolver.py` & `wc-django-device-recognizer-0.1.3/tests/test_request_resolver.py`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/tox.ini` & `wc-django-device-recognizer-0.1.3/tox.ini`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/PKG-INFO` & `wc-django-device-recognizer-0.1.3/wc_django_device_recognizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-device-recognizer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django device recognizing utility.
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `wc-django-device-recognizer-0.1.2/wc_django_device_recognizer.egg-info/SOURCES.txt` & `wc-django-device-recognizer-0.1.3/wc_django_device_recognizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/admin.py` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/admin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.contrib import admin
+from django.utils.translation import pgettext_lazy
 
 from .models import InterlocutorNetwork, Interlocutor, App, OS, Device
 
 
 @admin.register(App)
 class AppAdmin(admin.ModelAdmin):
     list_display = 'id', 'family', 'version',
@@ -40,11 +41,45 @@
     list_filter = 'os', 'device', 'app',
     autocomplete_fields = 'os', 'device', 'app'
     date_hierarchy = 'created_at'
     search_fields = (
         'id', 'user_agent', 'client_hints', 'outer_id',
         'device__id', 'os__id', 'app__id', 'network_connections__ip'
     )
-    inlines = InterlocutorNetworkInline,
+    # inlines = InterlocutorNetworkInline,
 
     def get_queryset(self, request):
         return super().get_queryset(request).with_relateds().distinct()
+
+
+@admin.register(InterlocutorNetwork)
+class InterlocutorNetworkAdmin(admin.ModelAdmin):
+    list_display = 'ip', 'get_os', 'get_device', 'get_app', 'get_outer_id', 'created_at',
+    list_filter = 'interlocutor__os', 'interlocutor__device', 'interlocutor__app',
+    autocomplete_fields = 'interlocutor',
+    search_fields = (
+        'ip',
+        'interlocutor__user_agent', 'interlocutor__client_hints', 'interlocutor__outer_id',
+        'interlocutor__device__id', 'interlocutor__os__id',
+        'interlocutor__app__id', 'interlocutor__network_connections__ip'
+    )
+    list_select_related = 'interlocutor', 'interlocutor__os', 'interlocutor__device', 'interlocutor__app',
+
+    def get_os(self, obj):
+        return str(obj.interlocutor.os)
+    get_os.short_description = pgettext_lazy('wcd_device_recognizer', 'OS')
+    get_os.admin_order_field = 'interlocutor__os__id'
+
+    def get_app(self, obj):
+        return str(obj.interlocutor.app)
+    get_app.short_description = pgettext_lazy('wcd_device_recognizer', 'App')
+    get_app.admin_order_field = 'interlocutor__app__id'
+
+    def get_device(self, obj):
+        return str(obj.interlocutor.device)
+    get_device.short_description = pgettext_lazy('wcd_device_recognizer', 'Device')
+    get_device.admin_order_field = 'interlocutor__device__id'
+
+    def get_outer_id(self, obj):
+        return str(obj.interlocutor.outer_id)
+    get_outer_id.short_description = pgettext_lazy('wcd_outer_id_recognizer', 'Outer id')
+    get_outer_id.admin_order_field = 'interlocutor__outer_id'
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/dtos.py` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/dtos.py`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/af/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/af/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ar/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/cy/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
-"&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
+"Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n==2) ? 1 : (n != 8 && n != "
+"11) ? 2 : 3;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ast/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ast/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/az/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/az/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/be/LC_MESSAGES/django.mo` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/be/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/be/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/be/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,49 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -45,44 +69,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bg/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bg/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bn/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bn/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/br/LC_MESSAGES/django.mo` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/br/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/br/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/br/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,51 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=5; plural=((n%10 == 1) && (n%100 != 11) && (n%100 !"
-"=71) && (n%100 !=91) ? 0 :(n%10 == 2) && (n%100 != 12) && (n%100 !=72) && (n"
-"%100 !=92) ? 1 :(n%10 ==3 || n%10==4 || n%10==9) && (n%100 < 10 || n% 100 > "
-"19) && (n%100 < 70 || n%100 > 79) && (n%100 < 90 || n%100 > 99) ? 2 :(n != 0 "
-"&& n % 1000000 == 0) ? 3 : 4);\n"
+"=71) && (n%100 !=91) ? 0 :(n%10 == 2) && (n%100 != 12) && (n%100 !=72) && "
+"(n%100 !=92) ? 1 :(n%10 ==3 || n%10==4 || n%10==9) && (n%100 < 10 || n% 100 "
+"> 19) && (n%100 < 70 || n%100 > 79) && (n%100 < 90 || n%100 > 99) ? 2 :(n != "
+"0 && n % 1000000 == 0) ? 3 : 4);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -47,44 +71,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/bs/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/uk/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,50 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
+"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
+"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
+"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +70,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ca/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ca/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cs/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
-"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"Plural-Forms: nplurals=2; plural=(n % 10 == 1 && n % 100 != 11) ? 0 : 1;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/cy/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lt/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,49 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n==2) ? 1 : (n != 8 && n != "
-"11) ? 2 : 3;\n"
+"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
+"11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
+"1 : n % 1 != 0 ? 2: 3);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +69,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/da/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/da/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/de/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/dsb/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/gd/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
-"n%100==4 ? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n==1 || n==11) ? 0 : (n==2 || n==12) ? 1 : "
+"(n > 2 && n < 20) ? 2 : 3;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/el/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/el/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/en/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/en/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eo/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/eo/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/es/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/es/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/et/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/et/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/eu/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/eu/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fa/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fa/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fi/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fi/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fr/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/fy/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/fy/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ga/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pl/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,49 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=5; plural=(n==1 ? 0 : n==2 ? 1 : n<7 ? 2 : n<11 ? 3 : "
-"4);\n"
+"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
+"(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
+"n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +69,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gd/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,49 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1 || n==11) ? 0 : (n==2 || n==12) ? 1 : "
-"(n > 2 && n < 20) ? 2 : 3;\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
+"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +69,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/gl/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ga/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=5; plural=(n==1 ? 0 : n==2 ? 1 : n<7 ? 2 : n<11 ? 3 : "
+"4);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/he/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/he/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
 "1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hi/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/gl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hr/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hi/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,24 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hsb/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/dsb/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
 "n%100==4 ? 2 : 3);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hu/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hu/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/hy/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hy/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ia/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ia/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/id/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/io/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ig/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/it/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/io/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ka/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n!=1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/is/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kab/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n % 10 != 1 || n % 100 == 11);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/it/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n!=1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ja/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/kn/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ka/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lb/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n!=1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kab/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ml/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kk/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mn/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n!=1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/km/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/mr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/kn/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nb/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ko/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ne/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ky/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lb/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/nn/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lt/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hsb/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,25 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
-"11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
-"1 : n % 1 != 0 ? 2: 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -45,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/lv/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/os/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : "
-"2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mk/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pa/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n % 10 == 1 && n % 100 != 11) ? 0 : 1;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ml/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pt/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mn/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sq/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/mr/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sv/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ms/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sw/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/my/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ta/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nb/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/te/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ne/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tg/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nl/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/nn/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/os/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ur/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pa/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/id/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pl/LC_MESSAGES/django.mo` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pl/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sl/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
-"(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
-"n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -45,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/pt/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ig/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ro/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ro/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
 "2:1));\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ru/LC_MESSAGES/django.mo` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ru/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/is/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
-"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=2; plural=(n % 10 != 1 || n % 100 == 11);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -45,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sk/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ja/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
-">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sl/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sk/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
-"n%100==4 ? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sq/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/km/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sr/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ko/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -44,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sv/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ky/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/sw/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ms/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ta/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/my/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/te/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/th/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tg/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/tt/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/th/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/udm/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tk/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/uz/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tr/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/vi/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +67,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/tt/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/bs/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/udm/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/cs/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uk/LC_MESSAGES/django.mo` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uk/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/ar/LC_MESSAGES/django.po`

 * *Files 17% similar despite different names*

```diff
@@ -4,26 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
-"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
-"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
-"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
+"&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -46,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/ur/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/lv/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : "
+"2);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/uz/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/sr/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/locale/vi/LC_MESSAGES/django.po` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/locale/hr/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,48 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 11:23+0300\n"
+"POT-Creation-Date: 2024-05-06 18:09+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+
+#: wcd_device_recognizer/admin.py:69 wcd_device_recognizer/models.py:80
+#: wcd_device_recognizer/models.py:141
+msgctxt "wcd_device_recognizer"
+msgid "OS"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:74 wcd_device_recognizer/models.py:71
+#: wcd_device_recognizer/models.py:146
+msgctxt "wcd_device_recognizer"
+msgid "App"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:79 wcd_device_recognizer/models.py:94
+#: wcd_device_recognizer/models.py:151
+msgctxt "wcd_device_recognizer"
+msgid "Device"
+msgstr ""
+
+#: wcd_device_recognizer/admin.py:84
+msgctxt "wcd_outer_id_recognizer"
+msgid "Outer id"
+msgstr ""
+
 #: wcd_device_recognizer/apps.py:12
 msgctxt "wcd_device_recognizer"
 msgid "Device recognizer"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:22
 msgctxt "wcd_device_recognizer"
@@ -43,44 +68,29 @@
 msgstr ""
 
 #: wcd_device_recognizer/models.py:64
 msgctxt "wcd_device_recognizer"
 msgid "Family"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:71 wcd_device_recognizer/models.py:146
-msgctxt "wcd_device_recognizer"
-msgid "App"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:72
 msgctxt "wcd_device_recognizer"
 msgid "Apps"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:80 wcd_device_recognizer/models.py:141
-msgctxt "wcd_device_recognizer"
-msgid "OS"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:81
 msgctxt "wcd_device_recognizer"
 msgid "OSs"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:84
 msgctxt "wcd_device_recognizer"
 msgid "Architecture"
 msgstr ""
 
-#: wcd_device_recognizer/models.py:94 wcd_device_recognizer/models.py:151
-msgctxt "wcd_device_recognizer"
-msgid "Device"
-msgstr ""
-
 #: wcd_device_recognizer/models.py:95
 msgctxt "wcd_device_recognizer"
 msgid "Devices"
 msgstr ""
 
 #: wcd_device_recognizer/models.py:98
 msgctxt "wcd_device_recognizer"
```

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/migrations/0001_initial.py` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/models.py` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/models.py`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/services/registry.py` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/services/registry.py`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/services/request_resolver.py` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/services/request_resolver.py`

 * *Files identical despite different names*

### Comparing `wc-django-device-recognizer-0.1.2/wcd_device_recognizer/utils.py` & `wc-django-device-recognizer-0.1.3/wcd_device_recognizer/utils.py`

 * *Files identical despite different names*

