# Comparing `tmp/hexkit-3.0.0.tar.gz` & `tmp/hexkit-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexkit-3.0.0.tar", last modified: Wed Apr 17 13:49:18 2024, max compression
+gzip compressed data, was "hexkit-3.0.1.tar", last modified: Mon May  6 16:04:18 2024, max compression
```

## Comparing `hexkit-3.0.0.tar` & `hexkit-3.0.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.025608 hexkit-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-04-17 13:49:12.000000 hexkit-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 13:49:12.000000 hexkit-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-17 13:49:18.025608 hexkit-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-17 13:49:12.000000 hexkit-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-17 13:49:12.000000 hexkit-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 13:49:18.025608 hexkit-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.013608 hexkit-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.017608 hexkit-3.0.0/src/hexkit/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16935 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/daopub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/daosub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/eventsub.py
--rw-r--r--   0 runner    (1001) docker     (127)    24781 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/protocols/objstorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/providers/akafka/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/providers/akafka/provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/provider/daosub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/provider/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/provider/eventsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/provider/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/testcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/akafka/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/providers/mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/mongodb/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/mongodb/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/providers/mongokafka/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/mongokafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16185 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/mongokafka/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.021608 hexkit-3.0.0/src/hexkit/providers/s3/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33195 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.025608 hexkit-3.0.0/src/hexkit/providers/s3/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/test_files/test_file1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/test_files/test_file2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/test_files/test_file3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/test_files/test_file4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15737 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/s3/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.025608 hexkit-3.0.0/src/hexkit/providers/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/providers/testing/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-17 13:49:12.000000 hexkit-3.0.0/src/hexkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:49:18.025608 hexkit-3.0.0/src/hexkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-17 13:49:18.000000 hexkit-3.0.0/src/hexkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-17 13:49:18.000000 hexkit-3.0.0/src/hexkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:49:18.000000 hexkit-3.0.0/src/hexkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-17 13:49:18.000000 hexkit-3.0.0/src/hexkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 13:49:18.000000 hexkit-3.0.0/src/hexkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.910359 hexkit-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-06 16:04:15.000000 hexkit-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 16:04:15.000000 hexkit-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-06 16:04:18.910359 hexkit-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-06 16:04:15.000000 hexkit-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-06 16:04:15.000000 hexkit-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:04:18.910359 hexkit-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.898359 hexkit-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.898359 hexkit-3.0.1/src/hexkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.902359 hexkit-3.0.1/src/hexkit/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16935 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/daopub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/daosub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/eventsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24781 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/protocols/objstorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.902359 hexkit-3.0.1/src/hexkit/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.902359 hexkit-3.0.1/src/hexkit/providers/akafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.902359 hexkit-3.0.1/src/hexkit/providers/akafka/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/provider/daosub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/provider/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/provider/eventsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/provider/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/testcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/akafka/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.906359 hexkit-3.0.1/src/hexkit/providers/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/mongodb/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/mongodb/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.906359 hexkit-3.0.1/src/hexkit/providers/mongokafka/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/mongokafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16185 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/mongokafka/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.906359 hexkit-3.0.1/src/hexkit/providers/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33195 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.906359 hexkit-3.0.1/src/hexkit/providers/s3/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/test_files/test_file1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/test_files/test_file2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/test_files/test_file3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/test_files/test_file4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15760 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/s3/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.906359 hexkit-3.0.1/src/hexkit/providers/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/providers/testing/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-06 16:04:15.000000 hexkit-3.0.1/src/hexkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:04:18.906359 hexkit-3.0.1/src/hexkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-06 16:04:18.000000 hexkit-3.0.1/src/hexkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-06 16:04:18.000000 hexkit-3.0.1/src/hexkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:04:18.000000 hexkit-3.0.1/src/hexkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-06 16:04:18.000000 hexkit-3.0.1/src/hexkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 16:04:18.000000 hexkit-3.0.1/src/hexkit.egg-info/top_level.txt
```

### Comparing `hexkit-3.0.0/LICENSE` & `hexkit-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/PKG-INFO` & `hexkit-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexkit
-Version: 3.0.0
+Version: 3.0.1
 Summary: A Toolkit for Building Microservices using the Hexagonal Architecture
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/hexkit
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `hexkit-3.0.0/README.md` & `hexkit-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/pyproject.toml` & `hexkit-3.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "hexkit"
-version = "3.0.0"
+version = "3.0.1"
 description = "A Toolkit for Building Microservices using the Hexagonal Architecture"
 dependencies = [
     "pydantic >=2, <3",
     "pydantic_settings >=2, <3",
     "PyYAML >=6.0, <7",
 ]
 
@@ -109,14 +109,15 @@
     "PLR2004",
     "D205",
     "D400",
     "D401",
     "D107",
     "D206",
     "D300",
+    "UP040",
 ]
 select = [
     "C90",
     "F",
     "I",
     "S",
     "B",
@@ -179,8 +180,26 @@
 source = [
     "src",
     "/workspace/src",
     "**/lib/python*/site-packages",
 ]
 
 [tool.tox]
-legacy_tox_ini = "    [tox]\n    env_list = py3{9,12}\n\n    [gh-actions]\n    python =\n        3.9: py39\n        3.10: py310\n        3.11: py311\n        3.12: py312\n\n    [testenv]\n    pass_env =\n        TC_HOST\n        DOCKER_HOST\n    deps =\n        --no-deps -r ./lock/requirements-dev.txt\n    commands = pytest {posargs}\n"
+legacy_tox_ini = """
+    [tox]
+    env_list = py3{9,12}
+
+    [gh-actions]
+    python =
+        3.9: py39
+        3.10: py310
+        3.11: py311
+        3.12: py312
+
+    [testenv]
+    pass_env =
+        TC_HOST
+        DOCKER_HOST
+    deps =
+        --no-deps -r ./lock/requirements-dev.txt
+    commands = pytest {posargs}
+"""
```

### Comparing `hexkit-3.0.0/src/hexkit/__init__.py` & `hexkit-3.0.1/src/hexkit/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/__main__.py` & `hexkit-3.0.1/src/hexkit/__main__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/base.py` & `hexkit-3.0.1/src/hexkit/base.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/config.py` & `hexkit-3.0.1/src/hexkit/config.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/correlation.py` & `hexkit-3.0.1/src/hexkit/correlation.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/custom_types.py` & `hexkit-3.0.1/src/hexkit/custom_types.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/log.py` & `hexkit-3.0.1/src/hexkit/log.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/protocols/__init__.py` & `hexkit-3.0.1/src/hexkit/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/protocols/dao.py` & `hexkit-3.0.1/src/hexkit/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/protocols/daopub.py` & `hexkit-3.0.1/src/hexkit/protocols/daopub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/protocols/daosub.py` & `hexkit-3.0.1/src/hexkit/protocols/daosub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/protocols/eventpub.py` & `hexkit-3.0.1/src/hexkit/protocols/eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/protocols/eventsub.py` & `hexkit-3.0.1/src/hexkit/protocols/eventsub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/protocols/objstorage.py` & `hexkit-3.0.1/src/hexkit/protocols/objstorage.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/__init__.py` & `hexkit-3.0.1/src/hexkit/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/akafka/__init__.py` & `hexkit-3.0.1/src/hexkit/providers/akafka/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/akafka/config.py` & `hexkit-3.0.1/src/hexkit/providers/akafka/config.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/akafka/provider/__init__.py` & `hexkit-3.0.1/src/hexkit/providers/akafka/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/akafka/provider/daosub.py` & `hexkit-3.0.1/src/hexkit/providers/akafka/provider/daosub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/akafka/provider/eventpub.py` & `hexkit-3.0.1/src/hexkit/providers/akafka/provider/eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/akafka/provider/eventsub.py` & `hexkit-3.0.1/src/hexkit/providers/akafka/provider/eventsub.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/akafka/provider/utils.py` & `hexkit-3.0.1/src/hexkit/providers/akafka/provider/utils.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/akafka/testcontainer.py` & `hexkit-3.0.1/src/hexkit/providers/akafka/testcontainer.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/akafka/testutils.py` & `hexkit-3.0.1/src/hexkit/providers/akafka/testutils.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/mongodb/__init__.py` & `hexkit-3.0.1/src/hexkit/providers/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/mongodb/provider.py` & `hexkit-3.0.1/src/hexkit/providers/mongodb/provider.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/mongodb/testutils.py` & `hexkit-3.0.1/src/hexkit/providers/mongodb/testutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 from pymongo import MongoClient
 from pymongo.errors import ExecutionTimeout, OperationFailure
 from testcontainers.mongodb import MongoDbContainer
 
 from hexkit.custom_types import PytestScope
 from hexkit.providers.mongodb.provider import MongoDbConfig, MongoDbDaoFactory
 
+MONGODB_IMAGE = "mongo:6.0.3"
+
 
 @dataclass(frozen=True)
 class MongoDbFixture:
     """Yielded by the `mongodb_fixture` function"""
 
     client: MongoClient
     config: MongoDbConfig
@@ -73,15 +75,15 @@
 
 
 def mongodb_fixture_function() -> Generator[MongoDbFixture, None, None]:
     """Pytest fixture for tests depending on the MongoDbDaoFactory DAO.
 
     **Do not call directly** Instead, use get_mongodb_fixture()
     """
-    with MongoDbContainer(image="mongo:6.0.3") as mongodb:
+    with MongoDbContainer(image=MONGODB_IMAGE) as mongodb:
         config = config_from_mongodb_container(mongodb)
         dao_factory = MongoDbDaoFactory(config=config)
         client = mongodb.get_connection_client()
 
         yield MongoDbFixture(
             client=client,
             config=config,
```

### Comparing `hexkit-3.0.0/src/hexkit/providers/mongokafka/__init__.py` & `hexkit-3.0.1/src/hexkit/providers/s3/test_files/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,12 +8,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#
-
-"""An implementation of the DaoPublisherFactoryProtocol based on MongoDB and Apache Kafka."""
-
-from .provider import MongoKafkaConfig, MongoKafkaDaoPublisherFactory  # noqa: F401
```

### Comparing `hexkit-3.0.0/src/hexkit/providers/mongokafka/provider.py` & `hexkit-3.0.1/src/hexkit/providers/mongokafka/provider.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/s3/__init__.py` & `hexkit-3.0.1/src/hexkit/providers/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/s3/provider.py` & `hexkit-3.0.1/src/hexkit/providers/s3/provider.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit/providers/s3/test_files/__init__.py` & `hexkit-3.0.1/src/hexkit/providers/testing/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,7 +8,16 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
+
+"""
+This sub-package contains providers for testing purposes.
+These providers should be very lightweight and preferably only need dependencies from
+the standard library.
+
+ATTENTION: Do not use these providers in production.
+"""
```

### Comparing `hexkit-3.0.0/src/hexkit/providers/s3/testutils.py` & `hexkit-3.0.1/src/hexkit/providers/s3/testutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 from pydantic import BaseModel, SecretStr, computed_field
 from testcontainers.localstack import LocalStackContainer
 
 from hexkit.custom_types import PytestScope
 from hexkit.protocols.objstorage import ObjectStorageProtocol, PresignedPostURL
 from hexkit.providers.s3.provider import S3Config, S3ObjectStorage
 
+LOCALSTACK_IMAGE = "localstack/localstack:0.14.5"
+
 TEST_FILE_DIR = Path(__file__).parent.resolve() / "test_files"
 
 TEST_FILE_PATHS = [
     TEST_FILE_DIR / filename
     for filename in os.listdir(TEST_FILE_DIR)
     if filename.startswith("test_") and filename.endswith(".yaml")
 ]
@@ -119,17 +121,15 @@
 
 
 def s3_fixture_function() -> Generator[S3Fixture, None, None]:
     """Pytest fixture for tests depending on the S3ObjectStorage DAO.
 
     **Do not call directly** Instead, use get_s3_fixture()
     """
-    with LocalStackContainer(image="localstack/localstack:0.14.5").with_services(
-        "s3"
-    ) as localstack:
+    with LocalStackContainer(image=LOCALSTACK_IMAGE).with_services("s3") as localstack:
         config = config_from_localstack_container(localstack)
 
         storage = S3ObjectStorage(config=config)
         yield S3Fixture(config=config, storage=storage)
 
 
 def get_s3_fixture(scope: PytestScope = "function"):
```

### Comparing `hexkit-3.0.0/src/hexkit/providers/testing/eventpub.py` & `hexkit-3.0.1/src/hexkit/providers/testing/eventpub.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             raise TopicExhaustedError() from error
 
 
 class InMemEventPublisher(EventPublisherProtocol):
     """
     An in-memory EventPublisher for testing purposes.
     Please note, this only works when publisher and consumers are running in the same
-    thread. Not suitable for inter-thread or inter-process comminication.
+    thread. Not suitable for inter-thread or inter-process communication.
     """
 
     def __init__(self, event_store: Optional[InMemEventStore] = None):
         """Initialize with existing event_store or let it create a new one."""
         self.event_store = event_store if event_store else InMemEventStore()
 
     async def _publish_validated(
```

### Comparing `hexkit-3.0.0/src/hexkit/utils.py` & `hexkit-3.0.1/src/hexkit/utils.py`

 * *Files identical despite different names*

### Comparing `hexkit-3.0.0/src/hexkit.egg-info/PKG-INFO` & `hexkit-3.0.1/src/hexkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexkit
-Version: 3.0.0
+Version: 3.0.1
 Summary: A Toolkit for Building Microservices using the Hexagonal Architecture
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/hexkit
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `hexkit-3.0.0/src/hexkit.egg-info/SOURCES.txt` & `hexkit-3.0.1/src/hexkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

