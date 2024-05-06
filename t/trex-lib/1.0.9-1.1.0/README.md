# Comparing `tmp/trex-lib-1.0.9.tar.gz` & `tmp/trex-lib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trex-lib-1.0.9.tar", last modified: Thu Nov  9 07:58:11 2023, max compression
+gzip compressed data, was "trex-lib-1.1.0.tar", last modified: Mon May  6 07:59:53 2024, max compression
```

## Comparing `trex-lib-1.0.9.tar` & `trex-lib-1.1.0.tar`

### file list

```diff
@@ -1,54 +1,61 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/
--rw-r--r--   0 jacklok    (501) staff       (20)     1052 2020-09-03 05:31:42.000000 trex-lib-1.0.9/LICENSE
--rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-1.0.9/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      462 2023-11-09 07:58:11.000000 trex-lib-1.0.9/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-1.0.9/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2021-08-13 04:29:57.000000 trex-lib-1.0.9/pyproject.toml
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-11-09 07:58:11.000000 trex-lib-1.0.9/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)     1202 2023-11-09 07:57:38.000000 trex-lib-1.0.9/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trex_lib.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      462 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trex_lib.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1274 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trex_lib.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trex_lib.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)      292 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trex_lib.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       14 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trex_lib.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-1.0.9/trexlib/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5053 2023-08-16 14:56:05.000000 trex-lib-1.0.9/trexlib/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-1.0.9/trexlib/libs/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/libs/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-02-13 02:03:08.000000 trex-lib-1.0.9/trexlib/libs/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     9782 2023-03-28 03:00:42.000000 trex-lib-1.0.9/trexlib/libs/controllers/task_base_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/libs/firebase/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2022-06-09 04:14:24.000000 trex-lib-1.0.9/trexlib/libs/firebase/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      378 2022-06-09 06:38:00.000000 trex-lib-1.0.9/trexlib/libs/firebase/firebase_helper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/libs/flask_wtf/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-1.0.9/trexlib/libs/flask_wtf/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-1.0.9/trexlib/libs/flask_wtf/crsf_ext.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-1.0.9/trexlib/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/utils/common/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-1.0.9/trexlib/utils/common/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4514 2022-09-26 14:54:31.000000 trex-lib-1.0.9/trexlib/utils/common/common_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      926 2023-08-30 15:08:13.000000 trex-lib-1.0.9/trexlib/utils/common/config_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-1.0.9/trexlib/utils/common/conftest.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-1.0.9/trexlib/utils/common/crm_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1573 2021-04-21 02:37:36.000000 trex-lib-1.0.9/trexlib/utils/common/currency_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3706 2023-11-09 07:11:16.000000 trex-lib-1.0.9/trexlib/utils/common/date_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-1.0.9/trexlib/utils/common/float_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4201 2021-03-04 08:12:18.000000 trex-lib-1.0.9/trexlib/utils/common/format_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1086 2020-09-04 07:48:19.000000 trex-lib-1.0.9/trexlib/utils/common/pagination_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1087 2021-06-24 07:11:43.000000 trex-lib-1.0.9/trexlib/utils/common/phone_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      825 2021-08-13 09:35:21.000000 trex-lib-1.0.9/trexlib/utils/common/user_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      840 2021-07-01 09:54:24.000000 trex-lib-1.0.9/trexlib/utils/crypto_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-09 07:58:11.000000 trex-lib-1.0.9/trexlib/utils/google/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-1.0.9/trexlib/utils/google/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12907 2021-08-20 10:49:32.000000 trex-lib-1.0.9/trexlib/utils/google/bigquery_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4283 2023-10-04 04:35:54.000000 trex-lib-1.0.9/trexlib/utils/google/cloud_tasks_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1364 2023-03-08 04:49:28.000000 trex-lib-1.0.9/trexlib/utils/google/gcloud_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-1.0.9/trexlib/utils/log_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3215 2021-08-13 04:41:06.000000 trex-lib-1.0.9/trexlib/utils/security_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8212 2023-08-16 09:12:40.000000 trex-lib-1.0.9/trexlib/utils/sms_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4946 2023-08-16 03:30:52.000000 trex-lib-1.0.9/trexlib/utils/string_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-1.0.9/trexlib/utils/url_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.188233 trex-lib-1.1.0/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1052 2020-09-03 05:31:42.000000 trex-lib-1.1.0/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-1.1.0/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      622 2024-05-06 07:59:53.187954 trex-lib-1.1.0/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-1.1.0/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2021-08-13 04:29:57.000000 trex-lib-1.1.0/pyproject.toml
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-06 07:59:53.189523 trex-lib-1.1.0/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)     1213 2024-05-06 07:59:30.000000 trex-lib-1.1.0/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.186845 trex-lib-1.1.0/trex_lib.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      622 2024-05-06 07:59:53.000000 trex-lib-1.1.0/trex_lib.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1482 2024-05-06 07:59:53.000000 trex-lib-1.1.0/trex_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-06 07:59:53.000000 trex-lib-1.1.0/trex_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       89 2024-05-06 07:59:53.000000 trex-lib-1.1.0/trex_lib.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       14 2024-05-06 07:59:53.000000 trex-lib-1.1.0/trex_lib.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.149501 trex-lib-1.1.0/trexlib/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-1.1.0/trexlib/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5426 2024-04-05 01:57:54.000000 trex-lib-1.1.0/trexlib/conf_to_remove.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.150637 trex-lib-1.1.0/trexlib/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-1.1.0/trexlib/libs/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.151292 trex-lib-1.1.0/trexlib/libs/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-02-13 02:03:08.000000 trex-lib-1.1.0/trexlib/libs/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9783 2024-04-29 04:45:24.000000 trex-lib-1.1.0/trexlib/libs/controllers/task_base_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.152578 trex-lib-1.1.0/trexlib/libs/facebook/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-04 09:51:48.000000 trex-lib-1.1.0/trexlib/libs/facebook/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.153207 trex-lib-1.1.0/trexlib/libs/facebook/util/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-04 09:52:59.000000 trex-lib-1.1.0/trexlib/libs/facebook/util/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2726 2024-04-08 02:49:39.000000 trex-lib-1.1.0/trexlib/libs/facebook/util/whatsapp_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.154519 trex-lib-1.1.0/trexlib/libs/firebase/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2022-06-09 04:14:24.000000 trex-lib-1.1.0/trexlib/libs/firebase/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      378 2022-06-09 06:38:00.000000 trex-lib-1.1.0/trexlib/libs/firebase/firebase_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.156548 trex-lib-1.1.0/trexlib/libs/flask_wtf/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-1.1.0/trexlib/libs/flask_wtf/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-1.1.0/trexlib/libs/flask_wtf/crsf_ext.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1918 2024-05-01 14:52:30.000000 trex-lib-1.1.0/trexlib/libs/flask_wtf/request_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.165453 trex-lib-1.1.0/trexlib/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-1.1.0/trexlib/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.181199 trex-lib-1.1.0/trexlib/utils/common/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-1.1.0/trexlib/utils/common/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4514 2022-09-26 14:54:31.000000 trex-lib-1.1.0/trexlib/utils/common/common_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      926 2023-08-30 15:08:13.000000 trex-lib-1.1.0/trexlib/utils/common/config_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-1.1.0/trexlib/utils/common/conftest.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-1.1.0/trexlib/utils/common/crm_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1573 2021-04-21 02:37:36.000000 trex-lib-1.1.0/trexlib/utils/common/currency_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3707 2024-04-29 04:45:34.000000 trex-lib-1.1.0/trexlib/utils/common/date_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-1.1.0/trexlib/utils/common/float_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4201 2021-03-04 08:12:18.000000 trex-lib-1.1.0/trexlib/utils/common/format_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1087 2024-04-29 04:45:42.000000 trex-lib-1.1.0/trexlib/utils/common/pagination_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1087 2021-06-24 07:11:43.000000 trex-lib-1.1.0/trexlib/utils/common/phone_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      825 2021-08-13 09:35:21.000000 trex-lib-1.1.0/trexlib/utils/common/user_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      933 2024-01-27 15:50:32.000000 trex-lib-1.1.0/trexlib/utils/crypto_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.185002 trex-lib-1.1.0/trexlib/utils/google/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-1.1.0/trexlib/utils/google/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12870 2024-04-29 04:38:39.000000 trex-lib-1.1.0/trexlib/utils/google/bigquery_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4295 2024-04-29 04:46:45.000000 trex-lib-1.1.0/trexlib/utils/google/cloud_tasks_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1365 2024-04-29 04:44:56.000000 trex-lib-1.1.0/trexlib/utils/google/gcloud_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-1.1.0/trexlib/utils/log_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      766 2024-03-21 04:18:42.000000 trex-lib-1.1.0/trexlib/utils/member_card_generator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3216 2024-04-29 04:46:01.000000 trex-lib-1.1.0/trexlib/utils/security_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8213 2024-04-29 04:46:10.000000 trex-lib-1.1.0/trexlib/utils/sms_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5170 2024-04-22 11:10:51.000000 trex-lib-1.1.0/trexlib/utils/string_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-1.1.0/trexlib/utils/url_util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `trex-lib-1.0.9/LICENSE` & `trex-lib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.9/setup.py` & `trex-lib-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-lib',  
-     version='1.0.9',
+     version='1.1.0',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex Core library package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-lib",
      packages=setuptools.find_packages(),
@@ -21,22 +21,22 @@
           'python-dateutil',
           'cryptography',
           'urllib3',
           'phonenumbers',
           'email_validator',
           'Flask-Script',
           'basicauth',
-          'protobuf==3.17.3',
-          'pyopenssl>=22.0.0',
-          'firebase-admin>=5.3.0',
-          'google-cloud-storage==2.0.0',
-          'google-cloud-tasks==2.8.1',
-          'google-auth==1.35.0',
-          'google-cloud-core==1.7.3',
-          'flask-babel',
-          'flask-restful>=0.3.9',
-          'flask-wtf',
-          'six',
+          #'protobuf==3.17.3',
+          #'pyopenssl>=22.0.0',
+          #'firebase-admin>=5.3.0',
+          #'google-cloud-storage==2.0.0',
+          #'google-cloud-tasks==2.8.1',
+          #'google-auth==1.35.0',
+          #'google-cloud-core==1.7.3',
+          #'flask-babel',
+          #'flask-restful>=0.3.9',
+          #'flask-wtf',
+          #'six',
       ],
      
  )
```

### Comparing `trex-lib-1.0.9/trex_lib.egg-info/SOURCES.txt` & `trex-lib-1.1.0/trex_lib.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -6,25 +6,30 @@
 setup.py
 trex_lib.egg-info/PKG-INFO
 trex_lib.egg-info/SOURCES.txt
 trex_lib.egg-info/dependency_links.txt
 trex_lib.egg-info/requires.txt
 trex_lib.egg-info/top_level.txt
 trexlib/__init__.py
-trexlib/conf.py
+trexlib/conf_to_remove.py
 trexlib/libs/__init__.py
 trexlib/libs/controllers/__init__.py
 trexlib/libs/controllers/task_base_routes.py
+trexlib/libs/facebook/__init__.py
+trexlib/libs/facebook/util/__init__.py
+trexlib/libs/facebook/util/whatsapp_util.py
 trexlib/libs/firebase/__init__.py
 trexlib/libs/firebase/firebase_helper.py
 trexlib/libs/flask_wtf/__init__.py
 trexlib/libs/flask_wtf/crsf_ext.py
+trexlib/libs/flask_wtf/request_wrapper.py
 trexlib/utils/__init__.py
 trexlib/utils/crypto_util.py
 trexlib/utils/log_util.py
+trexlib/utils/member_card_generator.py
 trexlib/utils/security_util.py
 trexlib/utils/sms_util.py
 trexlib/utils/string_util.py
 trexlib/utils/url_util.py
 trexlib/utils/common/__init__.py
 trexlib/utils/common/common_util.py
 trexlib/utils/common/config_util.py
```

### Comparing `trex-lib-1.0.9/trexlib/conf.py` & `trex-lib-1.1.0/trexlib/conf_to_remove.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,20 @@
 SMS_GATEWAY_PATH                                    = os.environ.get('SMS_GATEWAY_PATH')
 SMS_GATEWAY_URL                                     = os.environ.get('SMS_GATEWAY_URL')
 
 SMS_GATEWAY_USERNAME                                = os.environ.get('SMS_GATEWAY_USERNAME')
 SMS_GATEWAY_PASSWORD                                = os.environ.get('SMS_GATEWAY_PASSWORD')
 SMS_GATEWAY_SENDER                                  = os.environ.get('SMS_GATEWAY_SENDER')
 
+WHATSAPP_TOKEN                                      = os.environ.get('WHATSAPP_TOKEN')
+WHATSAPP_PHONE_NUMBER_ID                            = os.environ.get('WHATSAPP_PHONE_NUMBER_ID')
+WHATSAPP_VERIFY_TOKEN                               = os.environ.get('WHATSAPP_VERIFY_TOKEN')
+FACEBOOK_API_VERSION                                = os.environ.get('FACEBOOK_API_VERSION')
+
+
 
 def task_url(path):
     return '{}{}'.format(SYSTEM_BASE_URL, path)
 
 CHECK_CUSTOMER_ENTITLE_REWARD_TASK_URL              = task_url('/rewarding/check-entitle-reward')
 SEND_EMAIL_TASK_URL                                 = task_url('/system/send-email')
```

### Comparing `trex-lib-1.0.9/trexlib/libs/controllers/task_base_routes.py` & `trex-lib-1.1.0/trexlib/libs/controllers/task_base_routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from flask import Blueprint, render_template, request, Response, current_app
 from flask_restful import Resource
 from trexlib.utils.google.cloud_tasks_util import create_task
 import logging
 from trexlib.utils.log_util import get_tracelog
 from trexlib.utils.string_util import random_string
-from trexlib import conf as lib_conf
+from trexconf import conf as lib_conf
 from datetime import datetime
 logger = logging.getLogger('task')
 
 
 # Resource to trigger task
 class TriggerTaskBaseResource(Resource):
```

### Comparing `trex-lib-1.0.9/trexlib/utils/common/common_util.py` & `trex-lib-1.1.0/trexlib/utils/common/common_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.9/trexlib/utils/common/config_util.py` & `trex-lib-1.1.0/trexlib/utils/common/config_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.9/trexlib/utils/common/crm_util.py` & `trex-lib-1.1.0/trexlib/utils/common/crm_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.9/trexlib/utils/common/currency_util.py` & `trex-lib-1.1.0/trexlib/utils/common/currency_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.9/trexlib/utils/common/date_util.py` & `trex-lib-1.1.0/trexlib/utils/common/date_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Created on 19 May 2020
 
 @author: jacklok
 '''
  
 from datetime import datetime, timedelta
 from dateutil.relativedelta import relativedelta
-from trexlib import conf
+from trexconf import conf
 import pytz
 
 
 def parse_date(date_value, date_separator='/', full_year_date_format='%d/%m/%Y', short_year_date_format='%d/%m/%y'):
     if date_value is not None:
         #logging.info('parse_date: date_value=%s', date_value)
         _d_array = date_value.split(date_separator)
```

### Comparing `trex-lib-1.0.9/trexlib/utils/common/format_util.py` & `trex-lib-1.1.0/trexlib/utils/common/format_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.9/trexlib/utils/common/pagination_util.py` & `trex-lib-1.1.0/trexlib/utils/common/pagination_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 3 Sep 2020
 
 @author: jacklok
 '''
-from trexlib import conf
+from trexconf import conf
 import logging 
 from six import string_types
 
 logger = logging.getLogger('pagination_util')
 
 
 def get_offset_by_page_no(page_no, limit=conf.PAGINATION_SIZE):
```

### Comparing `trex-lib-1.0.9/trexlib/utils/common/phone_util.py` & `trex-lib-1.1.0/trexlib/utils/common/phone_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.9/trexlib/utils/common/user_util.py` & `trex-lib-1.1.0/trexlib/utils/common/user_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.9/trexlib/utils/google/bigquery_util.py` & `trex-lib-1.1.0/trexlib/utils/google/bigquery_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 '''
 Created on 11 Jan 2021
 
 @author: jacklok
 '''
-from trexlib import conf as lib_conf
 from google.oauth2 import service_account 
 from google.cloud import bigquery
 from google.cloud.exceptions import NotFound
 import logging
 from datetime import datetime, date, time
 from google.cloud.bigquery.dataset import DatasetReference
 import uuid
```

### Comparing `trex-lib-1.0.9/trexlib/utils/google/cloud_tasks_util.py` & `trex-lib-1.1.0/trexlib/utils/google/cloud_tasks_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 '''
 Created on 13 Jan 2021
 
 @author: jacklok
 '''
 from google.cloud import tasks_v2
-from trexlib import conf as lib_conf
+from trexconf import conf as lib_conf 
 import logging, json
 from datetime import datetime, timedelta
 from google.oauth2 import service_account 
 from google.protobuf import timestamp_pb2
 from trexlib.utils.security_util import create_basic_authentication, verfiy_basic_authentication
 from trexlib.utils.string_util import random_string
-#from trexlib.conf import SYSTEM_TASK_SERVICE_ACCOUNT_KEY, SYSTEM_TASK_GCLOUD_PROJECT_ID, SYSTEM_TASK_GCLOUD_LOCATION, SYSTEM_TASK_SERVICE_ACCOUNT_EMAIL
+#from trexlib.conf_to_remove import SYSTEM_TASK_SERVICE_ACCOUNT_KEY, SYSTEM_TASK_GCLOUD_PROJECT_ID, SYSTEM_TASK_GCLOUD_LOCATION, SYSTEM_TASK_SERVICE_ACCOUNT_EMAIL
 
 logger = logging.getLogger('utils-debug')
 
 def create_task(task_url, queue_name, payload=None, in_seconds=None, http_method='get', headers=None, 
                 credential_path=None, 
                 project_id=None, 
                 location=None,
```

### Comparing `trex-lib-1.0.9/trexlib/utils/google/gcloud_util.py` & `trex-lib-1.1.0/trexlib/utils/google/gcloud_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Created on 24 Dec 2020
 
 @author: jacklok
 '''
 import logging, json
 from google.oauth2 import service_account
 from google.cloud import storage
-from trexlib import conf as lib_conf
+from trexconf import conf as lib_conf
 
 logger = logging.getLogger('debug')
 
 
 def create_cloud_storage_client(info=None, credential_filepath=None):
     if info:
         cred = service_account.Credentials.from_service_account_info(info)
```

### Comparing `trex-lib-1.0.9/trexlib/utils/security_util.py` & `trex-lib-1.1.0/trexlib/utils/security_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import hashlib, hmac, time, uuid, json
-from trexlib import conf
+from trexconf import conf
 import logging
 from basicauth import encode as basic_encode, decode as basic_decode
 
 logger = logging.getLogger('lib')
 
 #-----------------------------------------------------------------
 # Password Hashing & Blending
```

### Comparing `trex-lib-1.0.9/trexlib/utils/sms_util.py` & `trex-lib-1.1.0/trexlib/utils/sms_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @author: jacklok
 '''
 
 import logging, time
 import phonenumbers
 from phonenumbers import carrier
 from phonenumbers.phonenumberutil import number_type
-from trexlib import conf
+from trexconf import conf
 from trexlib.utils.log_util import get_tracelog
 from six.moves import http_client
 from six.moves.urllib.parse import urlencode
 from trexlib.utils.string_util import four_digit_escape, is_ascii, random_string
 from datetime import datetime
 
 logger = logging.getLogger('util')
```

### Comparing `trex-lib-1.0.9/trexlib/utils/string_util.py` & `trex-lib-1.1.0/trexlib/utils/string_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 WHITESPACE_PATTERN  = re.compile(r'\s')
 DASH_PATTERN        = re.compile(r'-')
 
 ALPHANUMERIC_CHARS  = string.ascii_lowercase + string.ascii_uppercase + string.digits
 NUMERIC_CHARS       = string.digits
 
-HUMAN_SAFE_ALPHANUMERIC_CHARS     = 'abcdefghijkmnpqrstuvwxyzABCDEFGHJKLMNPQRSTUVWXYZ123456789'
+HUMAN_SAFE_ALPHANUMERIC_CHARS     = 'abcdefghijkmnopqrstuvwxyzABCDEFGHJKLMNPQRSTUVWXYZ123456789'
 
 
 
 def safe_str_cmp(a: str, b: str) -> bool:
     """This function compares strings in somewhat constant time. This
     requires that the length of at least one string is known in advance.
 
@@ -143,14 +143,21 @@
 def is_not_empty(value):
     return is_empty(value)==False
 
 def truncate_if_max_length(value, max_length):
     if value:
         return value[:max_length]
 
+def truncate_string(original_string, max_length):
+    if len(original_string) <= max_length:
+        return original_string
+    else:
+        truncated_string = original_string[:max_length]
+        return truncated_string
+
 def resolve_unicode_value(unicode_value):
     if unicode_value:
         unicode_value = unicode_value.decode('utf-8')
         return unicode_value
     else:
         return unicode_value
```

### Comparing `trex-lib-1.0.9/trexlib/utils/url_util.py` & `trex-lib-1.1.0/trexlib/utils/url_util.py`

 * *Files identical despite different names*

