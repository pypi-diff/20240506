# Comparing `tmp/bodosdk-1.5.1.tar.gz` & `tmp/bodosdk-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodosdk-1.5.1.tar", last modified: Tue Jan  2 18:15:08 2024, max compression
+gzip compressed data, was "bodosdk-2.0.0rc1.tar", last modified: Mon May  6 19:03:23 2024, max compression
```

## Comparing `bodosdk-1.5.1.tar` & `bodosdk-2.0.0rc1.tar`

### file list

```diff
@@ -1,58 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 18:15:08.633650 bodosdk-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-02 18:14:57.000000 bodosdk-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-02 18:14:57.000000 bodosdk-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    95334 2024-01-02 18:15:08.633650 bodosdk-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    94639 2024-01-02 18:14:57.000000 bodosdk-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 18:15:08.637650 bodosdk-1.5.1/bodosdk/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-02 18:15:08.637650 bodosdk-1.5.1/bodosdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 18:15:08.629650 bodosdk-1.5.1/bodosdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/request_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 18:15:08.629650 bodosdk-1.5.1/bodosdk/client/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/client/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/client/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/client/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/client/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/client/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/client/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/client/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/client/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/client/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/client/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 18:15:08.633650 bodosdk-1.5.1/bodosdk/error_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/error_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/error_handlers/handle_api_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 18:15:08.633650 bodosdk-1.5.1/bodosdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/models/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/models/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/models/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    17969 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/models/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/models/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-01-02 18:14:57.000000 bodosdk-1.5.1/bodosdk/models/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 18:15:08.625650 bodosdk-1.5.1/bodosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    95334 2024-01-02 18:15:08.000000 bodosdk-1.5.1/bodosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-01-02 18:15:08.000000 bodosdk-1.5.1/bodosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 18:15:08.000000 bodosdk-1.5.1/bodosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-02 18:15:08.000000 bodosdk-1.5.1/bodosdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-02 18:15:08.000000 bodosdk-1.5.1/bodosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-02 18:15:08.637650 bodosdk-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-01-02 18:14:57.000000 bodosdk-1.5.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-01-02 18:14:57.000000 bodosdk-1.5.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    93797 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16330 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/bodosdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/bodosdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.534160 bodosdk-2.0.0rc1/bodosdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/job_tpl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.534160 bodosdk-2.0.0rc1/bodosdk/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/request_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/bodosdk/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/job_tpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/clients/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/bodosdk/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/deprecation_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37725 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/bodosdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45991 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34045 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/bodosdk/models/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/bodosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    93797 2024-05-06 19:03:23.000000 bodosdk-2.0.0rc1/bodosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-06 19:03:23.000000 bodosdk-2.0.0rc1/bodosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:03:23.000000 bodosdk-2.0.0rc1/bodosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 19:03:23.000000 bodosdk-2.0.0rc1/bodosdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 19:03:23.000000 bodosdk-2.0.0rc1/bodosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:03:23.538160 bodosdk-2.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80088 2024-05-06 19:03:01.000000 bodosdk-2.0.0rc1/versioneer.py
```

### Comparing `bodosdk-1.5.1/LICENSE` & `bodosdk-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `bodosdk-1.5.1/bodosdk/api/auth.py` & `bodosdk-2.0.0rc1/bodosdk/api/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 
 import jwt
 
 from bodosdk.api.request_wrapper import RequestWrapper
-from bodosdk.exc import Unauthorized
-from bodosdk.models.base import APIKeys
+from bodosdk.exceptions import Unauthorized
+from bodosdk.base import APIKeys
 
 
 class AuthApi:
     def __init__(
         self,
         auth: APIKeys,
         auth_url="https://auth.bodo.ai",
@@ -17,37 +17,38 @@
         self._requests = requests
         self._auth_url = auth_url
         self._auth = auth
         self._token = None
 
     def _authenticate(self):
         resp = self._requests.post(
-            f"{self._auth_url}/identity/resources/auth/v1/api-token",
+            f"{self._auth_url}/identity/resources/auth/v2/api-token",
             json={
                 "clientId": self._auth.client_id,
                 "secret": self._auth.secret_key,
             },
         )
         if resp.status_code == 200:
-            return resp.json()["accessToken"]
+            return resp.json()["access_token"]
         raise Unauthorized(
             "Authentication failed. Suggestion: check Client ID and Secret Key values."
         )
 
     def switch_workspace(self, auth: APIKeys):
         self._auth = auth
         self._token = self._authenticate()
 
     @property
     def auth_token(self):
         if self._token is not None:
             try:
-                exp = datetime.fromtimestamp(
-                    jwt.decode(self._token, options={"verify_signature": False})["exp"]
-                )
+                exp = datetime.fromtimestamp(self.decode_token(self._token)["exp"])
                 if exp < datetime.now():
                     self._token = self._authenticate()
             except Exception as ex:  # noqa: F841
                 self._token = self._authenticate()
         else:
             self._token = self._authenticate()
         return self._token
+
+    def decode_token(self, token):
+        return jwt.decode(token, options={"verify_signature": False})
```

### Comparing `bodosdk-1.5.1/bodosdk/api/billing.py` & `bodosdk-2.0.0rc1/bodosdk/api/billing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from datetime import date
 from typing import Union
 from uuid import UUID
 
 from pydantic import validate_arguments
 
-from bodosdk.api.base import BackendApi
-from bodosdk.error_handlers.handle_api_error import handle_api_error
-from bodosdk.models.base import PaginationOrder
-from bodosdk.models.cluster import ClusterPriceExportResponse, ClusterPricingResponse
-from bodosdk.models.job import (
+from bodosdk.api.base import BodoApi
+from bodosdk.base import PaginationOrder
+from bodosdk.api.models.cluster import (
+    ClusterPriceExportResponse,
+    ClusterPricingResponse,
+)
+from bodosdk.api.models.job import (
     DEFAULT_PAGE,
     DEFAULT_PAGE_SIZE,
     DEFAULT_ORDER,
 )
-from bodosdk.models.job import JobRunPriceExportResponse, JobRunPricingResponse
+from bodosdk.api.models.job import JobRunPriceExportResponse, JobRunPricingResponse
 
 
-class BillingApi(BackendApi):
+class BillingApi(BodoApi):
     def __init__(self, *args, **kwargs):
         super(BillingApi, self).__init__(*args, **kwargs)
 
     @validate_arguments
     def get_cluster_prices(
         self,
         started_at: Union[str, date],
@@ -36,15 +38,15 @@
         url = f"{self.get_resource_url()}/metering/pricing?startedAt={started_at}"
         f"&finishedAt={finished_at}&page={page}&size={size}&order={order.value}"
 
         if workspace_uuid is not None:
             url = f"{url}&workspaceUUID={workspace_uuid}"
 
         resp = self._requests.get(url, headers=headers)
-        handle_api_error(resp)
+        self.handle_error(resp)
         return ClusterPricingResponse(**resp.json())
 
     @validate_arguments
     def get_job_run_prices(
         self,
         started_at: Union[str, date],
         finished_at: Union[str, date],
@@ -52,22 +54,22 @@
         page: int = DEFAULT_PAGE,
         size: int = DEFAULT_PAGE_SIZE,
         order: PaginationOrder = DEFAULT_ORDER,
     ):
         headers = {"Content-type": "application/json"}
         headers.update(self.get_auth_header())
 
-        url = f"{self.get_resource_url()}/job/runs/pricing?startedAt={started_at}"
+        url = f"{self.get_resource_url()}/v1/jobs/pricing?startedAt={started_at}"
         f"&finishedAt={finished_at}&page={page}&size={size}&order={order.value}"
 
         if workspace_uuid is not None:
             url = f"{url}&workspaceUUID={workspace_uuid}"
 
         resp = self._requests.get(url, headers=headers)
-        handle_api_error(resp)
+        self.handle_error(resp)
         return JobRunPricingResponse(**resp.json())
 
     @validate_arguments
     def get_cluster_price_export(
         self,
         started_at: Union[str, date],
         finished_at: Union[str, date],
@@ -77,28 +79,28 @@
         headers.update(self.get_auth_header())
         url = f"{self.get_resource_url()}/metering/price-export?startedAt={started_at}&finishedAt={finished_at}"
 
         if workspace_uuid is not None:
             url = f"{url}&workspaceUUID={workspace_uuid}"
 
         resp = self._requests.get(url, headers=headers)
-        handle_api_error(resp)
+        self.handle_error(resp)
         return ClusterPriceExportResponse(**resp.json())
 
     @validate_arguments
     def get_job_run_price_export(
         self,
         started_at: Union[str, date],
         finished_at: Union[str, date],
         workspace_uuid: Union[str, UUID] = None,
     ):
         headers = {"Content-type": "application/json"}
         headers.update(self.get_auth_header())
 
-        url = f"{self.get_resource_url()}/job/runs/price-export?startedAt={started_at}&finishedAt={finished_at}"
+        url = f"{self.get_resource_url()}/v1/jobs/price-export?startedAt={started_at}&finishedAt={finished_at}"
 
         if workspace_uuid is not None:
             url = f"{url}&workspaceUUID={workspace_uuid}"
 
         resp = self._requests.get(url, headers=headers)
-        handle_api_error(resp)
+        self.handle_error(resp)
         return JobRunPriceExportResponse(**resp.json())
```

### Comparing `bodosdk-1.5.1/bodosdk/api/cloud_config.py` & `bodosdk-2.0.0rc1/bodosdk/api/cloud_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,75 @@
 from typing import Union
 
-from bodosdk.api.base import BackendApi
-from bodosdk.exc import (
-    ResourceNotFound,
-    ValidationError,
-    ServiceUnavailable,
-    UnknownError,
-)
-from bodosdk.models.cloud_config import (
-    AzureCloudConfig,
-    AwsCloudConfig,
-    CloudConfig,
-    CreateAwsCloudConfig,
-    CreateAzureCloudConfig,
+from bodosdk.api.base import BodoApi
+from bodosdk.api.models.cloud_config import (
+    AzureCloudConfigAPIModel,
+    AwsCloudConfigAPIModel,
+    CloudConfigAPIModel,
+    CreateAwsCloudConfigAPIModel,
+    CreateAzureCloudConfigAPIModel,
 )
+from bodosdk.interfaces import ICloudConfigApi, IAzureCloudConfig, IAwsCloudConfig
 
 
-class CloudConfigApi(BackendApi):
+class CloudConfigApi(BodoApi, ICloudConfigApi):
     def __init__(self, *args, **kwargs):
         super(CloudConfigApi, self).__init__(*args, **kwargs)
         self._resource_url = "cloudConfig"
 
     def create(
-        self, cloud_config: Union[CreateAwsCloudConfig, CreateAzureCloudConfig]
-    ) -> Union[AwsCloudConfig, AzureCloudConfig]:
+        self,
+        cloud_config: Union[IAwsCloudConfig, IAzureCloudConfig],
+    ) -> dict:
         headers = {"Content-type": "application/json"}
         headers.update(self.get_auth_header())
+        if isinstance(cloud_config, IAwsCloudConfig):
+            data = CreateAwsCloudConfigAPIModel(**cloud_config.dict())
+        if isinstance(cloud_config, IAzureCloudConfig):
+            data = CreateAzureCloudConfigAPIModel(**cloud_config.dict())
         resp = self._requests.post(
             self.get_resource_url(),
-            data=cloud_config.json(by_alias=True),
+            data=data.json(by_alias=True),
             headers=headers,
         )
-        if str(resp.status_code).startswith("2"):
-            return CloudConfig.parse_obj(resp.json()).__root__
-        if resp.status_code == 404:
-            raise ResourceNotFound("Probably wrong organization keys")
-        if resp.status_code in (400, 422):
-            raise ValidationError(resp.json())
-        if resp.status_code == 503:
-            raise ServiceUnavailable
-        raise UnknownError(resp)
+        self.handle_error(resp)
+        return resp.json()
 
     def update(
-        self, cloud_config: Union[AwsCloudConfig, AzureCloudConfig]
-    ) -> Union[AwsCloudConfig, AzureCloudConfig]:
+        self,
+        cloud_config: Union[IAwsCloudConfig, IAzureCloudConfig],
+    ) -> dict:
         headers = self.get_auth_header()
+        if isinstance(cloud_config, IAwsCloudConfig):
+            data = AwsCloudConfigAPIModel(**cloud_config.dict())
+        if isinstance(cloud_config, IAzureCloudConfig):
+            data = AzureCloudConfigAPIModel(**cloud_config.dict())
         resp = self._requests.put(
             f"{self.get_resource_url()}/{cloud_config.uuid}",
-            data=cloud_config.json(by_alias=True),
+            data=data.json(by_alias=True),
             headers=headers,
         )
-        if resp.status_code == 200:
-            return CloudConfig.parse_obj(resp.json()).__root__
-        if resp.status_code == 404:
-            raise ResourceNotFound
-        if resp.status_code == 503:
-            raise ServiceUnavailable
-        raise UnknownError(resp.content)
+        self.handle_error(resp)
+        return resp.json()
 
-    def list(self):
+    def list(self, page=None, page_size=None, order=None, provider=None, status=None):
         headers = self.get_auth_header()
-        resp = self._requests.get(f"{self.get_resource_url()}", headers=headers)
-        if resp.status_code == 200:
-            return [CloudConfig.parse_obj(cfg).__root__ for cfg in resp.json()]
-        if resp.status_code == 404:
-            raise ResourceNotFound
-        if resp.status_code == 503:
-            raise ServiceUnavailable
-        raise UnknownError(resp.content)
+        resp = self._requests.get(
+            f"{self.get_resource_url()}",
+            headers=headers,
+            params={"provider": provider, "status": status},
+        )
+        self.handle_error(resp)
+        return [CloudConfigAPIModel.parse_obj(cfg).__root__ for cfg in resp.json()]
 
     def get(self, uuid):
         headers = self.get_auth_header()
         resp = self._requests.get(f"{self.get_resource_url()}/{uuid}", headers=headers)
-        if resp.status_code == 200:
-            return CloudConfig.parse_obj(resp.json()).__root__
-        if resp.status_code == 404:
-            raise ResourceNotFound
-        if resp.status_code == 503:
-            raise ServiceUnavailable
-        raise UnknownError(resp.content)
+        self.handle_error(resp)
+        return CloudConfigAPIModel.parse_obj(resp.json()).__root__
 
     def delete(self, uuid):
         headers = self.get_auth_header()
         resp = self._requests.delete(
             f"{self.get_resource_url()}/{uuid}", headers=headers
         )
-        if str(resp.status_code).startswith("2"):
-            return
-        if resp.status_code == 404:
-            raise ResourceNotFound
-        if resp.status_code == 503:
-            raise ServiceUnavailable
-        raise UnknownError(resp.content)
+        self.handle_error(resp)
```

### Comparing `bodosdk-1.5.1/bodosdk/api/instance_role.py` & `bodosdk-2.0.0rc1/bodosdk/api/catalog.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,80 @@
-from typing import List
+from bodosdk.api.base import BodoApi
+from bodosdk.api.models.catalog import CatalogAPIModel
+from bodosdk.interfaces import ICatalog, ICatalogApi
 
-from bodosdk.api.base import BackendApi
-from bodosdk.exc import (
-    ResourceNotFound,
-    ServiceUnavailable,
-    UnknownError,
-    ValidationError,
-)
-from bodosdk.models import InstanceRoleItem, CreateRoleDefinition, CreateRoleResponse
 
-
-class InstanceRoleApi(BackendApi):
+class CatalogApi(BodoApi, ICatalogApi):
     def __init__(self, *args, **kwargs):
-        super(InstanceRoleApi, self).__init__(*args, **kwargs)
-        self._resource_url = "instance-roles"
+        super(CatalogApi, self).__init__(*args, **kwargs)
+        self._resource_url = "catalogs"
+
+    def create(self, catalog: ICatalog) -> dict:
+        headers = {"Content-type": "application/json"}
+        headers.update(self.get_auth_header())
+        data = CatalogAPIModel(**catalog.dict())
+        resp = self._requests.post(
+            self.get_resource_url("v1"),
+            data=data.json(by_alias=True, exclude_none=True),
+            headers=headers,
+        )
+        self.handle_error(resp)
+        return resp.json()
 
-    def get_role(self, uuid) -> InstanceRoleItem:
+    def get(self, uuid):
         response = self._requests.get(
-            f"{self.get_resource_url()}/{uuid}", headers=self.get_auth_header()
+            f"{self.get_resource_url('v1')}/{uuid}", headers=self.get_auth_header()
         )
-        if str(response.status_code).startswith("2"):
-            return InstanceRoleItem(**response.json())
-        if response.status_code == 404:
-            raise ResourceNotFound
-        if response.status_code == 503:
-            raise ServiceUnavailable
-        raise UnknownError(response.content)
+        self.handle_error(response)
+        return response.json()
 
-    def get_all_roles(self) -> List[InstanceRoleItem]:
+    def get_by_name(self, name):
         response = self._requests.get(
-            f"{self.get_resource_url()}", headers=self.get_auth_header()
+            f"{self.get_resource_url('v1')}",
+            headers=self.get_auth_header(),
+            params={"name": name},
         )
-        all_roles: List[InstanceRoleItem] = []
-        if str(response.status_code).startswith("2"):
-            for entry in response.json():
-                role_info = InstanceRoleItem(**entry)
-                all_roles.append(role_info)
-            return all_roles
-        if response.status_code == 404:
-            raise ResourceNotFound
-        if response.status_code == 503:
-            raise ServiceUnavailable
-        raise UnknownError(response.content)
+        self.handle_error(response)
+        try:
+            return response.json()[0]
+        except IndexError:
+            return []
+
+    def get_all(
+        self,
+        page=None,
+        page_size=None,
+        names=None,
+        uuids=None,
+        order=None,
+    ):
+        response = self._requests.get(
+            f"{self.get_resource_url('v1')}",
+            headers=self.get_auth_header(),
+            params={"name": names, "uuid": uuids},
+        )
+        self.handle_error(response)
+        return response.json()
 
-    def create_role(self, role_definition: CreateRoleDefinition) -> CreateRoleResponse:
+    def update(self, catalog: ICatalog):
         headers = {"Content-type": "application/json"}
         headers.update(self.get_auth_header())
-        resp = self._requests.post(
-            self.get_resource_url(), data=role_definition.json(), headers=headers
+        data = CatalogAPIModel(**catalog.dict())
+        response = self._requests.put(
+            f"{self.get_resource_url('v1')}/{catalog.uuid}",
+            data=data.json(by_alias=True, exclude_none=True),
+            headers=headers,
         )
-        if str(resp.status_code).startswith("2"):
-            return CreateRoleResponse(**resp.json())
-        if resp.status_code == 404:
-            raise ResourceNotFound("Probably wrong workspace keys")
-        if resp.status_code in (400, 422):
-            raise ValidationError(resp.json())
-        if resp.status_code == 503:
-            raise ServiceUnavailable
-        raise UnknownError
+        self.handle_error(response)
+        return response.json()
 
-    def remove_role(self, uuid, mark_as_terminated):
-        params = {"mark_as_terminated": str(mark_as_terminated).lower()}
+    def delete(self, uuid):
         response = self._requests.delete(
-            f"{self.get_resource_url()}/{uuid}",
-            params=params,
-            headers=self.get_auth_header(),
+            f"{self.get_resource_url('v1')}/{uuid}", headers=self.get_auth_header()
+        )
+        self.handle_error(response)
+
+    def delete_all(self):
+        response = self._requests.delete(
+            f"{self.get_resource_url('v1')}", headers=self.get_auth_header()
         )
-        if str(response.status_code).startswith("2"):
-            return
-        if response.status_code == 404:
-            raise ResourceNotFound
-        if response.status_code == 503:
-            raise ServiceUnavailable
-        raise UnknownError(response.content)
+        self.handle_error(response)
```

### Comparing `bodosdk-1.5.1/setup.py` & `bodosdk-2.0.0rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from setuptools import setup, find_packages
 import versioneer
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+with open("INDEX.md", "r") as fh:
+    long_description += "\n\n #INDEX \n\n" + fh.read()
+
 with open("requirements.txt", "r") as fh:
     requirements = fh.read().split("\n")
 
 setup(
     name="bodosdk",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     author="Bodo, Inc.",
     author_email="noreply@bodo.ai",
     packages=find_packages(include=["bodosdk", "bodosdk.*"]),
     scripts=[],
     url="https://github.com/Bodo-inc/bodo-sdk",
-    description="Bodo Platform SDK",
+    description="Bodo Platform SDK " + versioneer.get_version(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=requirements,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `bodosdk-1.5.1/versioneer.py` & `bodosdk-2.0.0rc1/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1756,15 +1756,15 @@
         "error": "unable to compute version",
         "date": None,
     }
 
 
 def get_version():
     """Get the short version string for this project."""
-    return get_versions()["version"]
+    return os.environ.get("VERSION_PREFIX", "") + get_versions()["version"]
 
 
 def get_cmdclass(cmdclass=None):
     """Get the custom setuptools/distutils subclasses used by Versioneer.
 
     If the package uses a different cmdclass (e.g. one from numpy), it
     should be provide as an argument.
```

