# Comparing `tmp/types-docker-7.0.0.20240503.tar.gz` & `tmp/types-docker-7.0.0.20240506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-docker-7.0.0.20240503.tar", last modified: Fri May  3 02:20:42 2024, max compression
+gzip compressed data, was "types-docker-7.0.0.20240506.tar", last modified: Mon May  6 02:22:14 2024, max compression
```

## Comparing `types-docker-7.0.0.20240503.tar` & `types-docker-7.0.0.20240506.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.558845 types-docker-7.0.0.20240503/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-03 02:20:40.000000 types-docker-7.0.0.20240503/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 02:20:40.000000 types-docker-7.0.0.20240503/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-03 02:20:42.558845 types-docker-7.0.0.20240503/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.546844 types-docker-7.0.0.20240503/docker-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 02:20:40.000000 types-docker-7.0.0.20240503/docker-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.550844 types-docker-7.0.0.20240503/docker-stubs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/container.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/exec_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/image.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/network.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/secret.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/api/volume.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.550844 types-docker-7.0.0.20240503/docker-stubs/context/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/context/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/context/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/context/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/context/context.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.550844 types-docker-7.0.0.20240503/docker-stubs/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/credentials/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/credentials/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/credentials/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/credentials/store.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/credentials/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/errors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.554844 types-docker-7.0.0.20240503/docker-stubs/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/configs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/images.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/secrets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/models/volumes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:40.000000 types-docker-7.0.0.20240503/docker-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/tls.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.554844 types-docker-7.0.0.20240503/docker-stubs/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/transport/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/transport/basehttpadapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/transport/npipeconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/transport/npipesocket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/transport/sshconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/transport/unixconn.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.554844 types-docker-7.0.0.20240503/docker-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/healthcheck.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/types/swarm.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.558845 types-docker-7.0.0.20240503/docker-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/fnmatch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/json_stream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/ports.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/socket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/utils/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 02:20:30.000000 types-docker-7.0.0.20240503/docker-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:20:42.558845 types-docker-7.0.0.20240503/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-03 02:20:40.000000 types-docker-7.0.0.20240503/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:20:42.558845 types-docker-7.0.0.20240503/types_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-03 02:20:42.000000 types-docker-7.0.0.20240503/types_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-03 02:20:42.000000 types-docker-7.0.0.20240503/types_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:20:42.000000 types-docker-7.0.0.20240503/types_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 02:20:42.000000 types-docker-7.0.0.20240503/types_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 02:20:42.000000 types-docker-7.0.0.20240503/types_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:14.568745 types-docker-7.0.0.20240506/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-06 02:22:14.000000 types-docker-7.0.0.20240506/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 02:22:14.000000 types-docker-7.0.0.20240506/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-06 02:22:14.568745 types-docker-7.0.0.20240506/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:14.560745 types-docker-7.0.0.20240506/docker-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-06 02:22:14.000000 types-docker-7.0.0.20240506/docker-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:14.560745 types-docker-7.0.0.20240506/docker-stubs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/container.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/exec_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/network.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/secret.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/api/volume.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:14.564745 types-docker-7.0.0.20240506/docker-stubs/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/context/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/context/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/context/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/context/context.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:14.564745 types-docker-7.0.0.20240506/docker-stubs/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/credentials/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/credentials/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/credentials/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/credentials/store.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/credentials/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/errors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:14.564745 types-docker-7.0.0.20240506/docker-stubs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/models/configs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/models/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/models/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/models/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/models/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/models/plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/models/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/models/secrets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/models/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/models/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/models/volumes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:14.000000 types-docker-7.0.0.20240506/docker-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/tls.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:14.564745 types-docker-7.0.0.20240506/docker-stubs/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/transport/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/transport/basehttpadapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/transport/npipeconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/transport/npipesocket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/transport/sshconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/transport/unixconn.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:14.568745 types-docker-7.0.0.20240506/docker-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/types/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/types/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/types/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/types/healthcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/types/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/types/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/types/swarm.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:14.568745 types-docker-7.0.0.20240506/docker-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/utils/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/utils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/utils/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/utils/fnmatch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/utils/json_stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/utils/ports.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/utils/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/utils/socket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/utils/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 02:21:48.000000 types-docker-7.0.0.20240506/docker-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 02:22:14.568745 types-docker-7.0.0.20240506/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-06 02:22:14.000000 types-docker-7.0.0.20240506/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:14.568745 types-docker-7.0.0.20240506/types_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-06 02:22:14.000000 types-docker-7.0.0.20240506/types_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-06 02:22:14.000000 types-docker-7.0.0.20240506/types_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 02:22:14.000000 types-docker-7.0.0.20240506/types_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 02:22:14.000000 types-docker-7.0.0.20240506/types_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 02:22:14.000000 types-docker-7.0.0.20240506/types_docker.egg-info/top_level.txt
```

### Comparing `types-docker-7.0.0.20240503/PKG-INFO` & `types-docker-7.0.0.20240506/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240503
+Version: 7.0.0.20240506
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8c0fc298c53b7e74fe3aad431aa4cfe3772170b3` and was tested
+This package was generated from typeshed commit `8ff50fbea2f607380c23d9b120fccfb1926284e5` and was tested
 with mypy 1.10.0, pyright 1.1.361, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240503/docker-stubs/api/build.pyi` & `types-docker-7.0.0.20240506/docker-stubs/api/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/api/client.pyi` & `types-docker-7.0.0.20240506/docker-stubs/api/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/api/container.pyi` & `types-docker-7.0.0.20240506/docker-stubs/api/container.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/api/daemon.pyi` & `types-docker-7.0.0.20240506/docker-stubs/api/daemon.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/api/exec_api.pyi` & `types-docker-7.0.0.20240506/docker-stubs/api/exec_api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/api/image.pyi` & `types-docker-7.0.0.20240506/docker-stubs/api/image.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/api/network.pyi` & `types-docker-7.0.0.20240506/docker-stubs/api/network.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/api/plugin.pyi` & `types-docker-7.0.0.20240506/docker-stubs/api/plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/api/service.pyi` & `types-docker-7.0.0.20240506/docker-stubs/api/service.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/api/swarm.pyi` & `types-docker-7.0.0.20240506/docker-stubs/api/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/api/volume.pyi` & `types-docker-7.0.0.20240506/docker-stubs/api/volume.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/auth.pyi` & `types-docker-7.0.0.20240506/docker-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/client.pyi` & `types-docker-7.0.0.20240506/docker-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/constants.pyi` & `types-docker-7.0.0.20240506/docker-stubs/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/context/api.pyi` & `types-docker-7.0.0.20240506/docker-stubs/context/api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/context/context.pyi` & `types-docker-7.0.0.20240506/docker-stubs/context/context.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/errors.pyi` & `types-docker-7.0.0.20240506/docker-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/models/containers.pyi` & `types-docker-7.0.0.20240506/docker-stubs/models/containers.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def stats(self, **kwargs): ...
     def stop(self, **kwargs): ...
     def top(self, **kwargs): ...
     def unpause(self): ...
     def update(self, **kwargs): ...
     def wait(self, **kwargs): ...
 
-class ContainerCollection(Collection):
+class ContainerCollection(Collection[Container]):
     model: type[Container]
     def run(
         self, image, command: Incomplete | None = None, stdout: bool = True, stderr: bool = False, remove: bool = False, **kwargs
     ): ...
     def create(self, image, command: Incomplete | None = None, **kwargs): ...  # type:ignore[override]
     def get(self, container_id): ...
     def list(
```

### Comparing `types-docker-7.0.0.20240503/docker-stubs/models/images.pyi` & `types-docker-7.0.0.20240506/docker-stubs/transport/sshconn.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,49 @@
+import socket
 from _typeshed import Incomplete
-from collections.abc import Generator
-from typing import Any
 
-from .resource import Collection, Model
+import urllib3
+import urllib3.connection
+from docker.transport.basehttpadapter import BaseHTTPAdapter
 
-class Image(Model):
-    @property
-    def labels(self): ...
-    @property
-    def short_id(self): ...
-    @property
-    def tags(self): ...
-    def history(self): ...
-    def remove(self, force: bool = False, noprune: bool = False): ...
-    def save(self, chunk_size=2097152, named: bool = False): ...
-    def tag(self, repository, tag: str | None = None, **kwargs): ...
-
-class RegistryData(Model):
-    image_name: Incomplete
-    def __init__(self, image_name, *args, **kwargs) -> None: ...
-    @property
-    def id(self): ...
-    @property
-    def short_id(self): ...
-    def pull(self, platform: Incomplete | None = None): ...
-    def has_platform(self, platform): ...
-    attrs: Incomplete
-    def reload(self) -> None: ...
-
-class ImageCollection(Collection):
-    model: type[Image]
-    def build(self, **kwargs) -> tuple[Image, Generator[Any, None, None]]: ...
-    def get(self, name): ...
-    def get_registry_data(self, name, auth_config: Incomplete | None = None): ...
-    def list(self, name: Incomplete | None = None, all: bool = False, filters: Incomplete | None = None): ...
-    def load(self, data): ...
-    def pull(self, repository, tag: str | None = None, all_tags: bool = False, **kwargs): ...
-    def push(self, repository, tag: str | None = None, **kwargs): ...
-    def remove(self, *args, **kwargs) -> None: ...
-    def search(self, *args, **kwargs): ...
-    def prune(self, filters: Incomplete | None = None): ...
-    def prune_builds(self, *args, **kwargs): ...
+RecentlyUsedContainer: Incomplete
 
-def normalize_platform(platform, engine_info): ...
+class SSHSocket(socket.socket):
+    host: Incomplete
+    port: Incomplete
+    user: Incomplete
+    proc: Incomplete
+    def __init__(self, host) -> None: ...
+    def connect(self, **kwargs) -> None: ...  # type:ignore[override]
+    def sendall(self, data) -> None: ...  # type:ignore[override]
+    def send(self, data): ...
+    def recv(self, n): ...
+    def makefile(self, mode): ...
+    def close(self) -> None: ...
+
+class SSHConnection(urllib3.connection.HTTPConnection):
+    ssh_transport: Incomplete
+    timeout: Incomplete
+    ssh_host: Incomplete
+    def __init__(self, ssh_transport: Incomplete | None = None, timeout: int = 60, host: Incomplete | None = None) -> None: ...
+    sock: Incomplete
+    def connect(self) -> None: ...
+
+class SSHConnectionPool(urllib3.connectionpool.HTTPConnectionPool):
+    scheme: str
+    ssh_transport: Incomplete
+    timeout: Incomplete
+    ssh_host: Incomplete
+    def __init__(
+        self, ssh_client: Incomplete | None = None, timeout: int = 60, maxsize: int = 10, host: Incomplete | None = None
+    ) -> None: ...
+
+class SSHHTTPAdapter(BaseHTTPAdapter):
+    __attrs__: Incomplete
+    ssh_client: Incomplete
+    ssh_host: Incomplete
+    timeout: Incomplete
+    max_pool_size: Incomplete
+    pools: Incomplete
+    def __init__(self, base_url, timeout: int = 60, pool_connections=..., max_pool_size=..., shell_out: bool = False) -> None: ...
+    def get_connection(self, url, proxies: Incomplete | None = None): ...
+    def close(self) -> None: ...
```

### Comparing `types-docker-7.0.0.20240503/docker-stubs/models/plugins.pyi` & `types-docker-7.0.0.20240506/docker-stubs/models/plugins.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -13,13 +13,13 @@
     def configure(self, options) -> None: ...
     def disable(self, force: bool = False) -> None: ...
     def enable(self, timeout: int = 0) -> None: ...
     def push(self): ...
     def remove(self, force: bool = False): ...
     def upgrade(self, remote: Incomplete | None = None) -> Generator[Incomplete, Incomplete, None]: ...
 
-class PluginCollection(Collection):
+class PluginCollection(Collection[Plugin]):
     model: type[Plugin]
     def create(self, name, plugin_data_dir, gzip: bool = False): ...  # type:ignore[override]
     def get(self, name): ...
     def install(self, remote_name, local_name: Incomplete | None = None): ...
     def list(self): ...
```

### Comparing `types-docker-7.0.0.20240503/docker-stubs/models/services.pyi` & `types-docker-7.0.0.20240506/docker-stubs/models/services.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def remove(self): ...
     def tasks(self, filters: Incomplete | None = None): ...
     def update(self, **kwargs): ...
     def logs(self, **kwargs): ...
     def scale(self, replicas): ...
     def force_update(self): ...
 
-class ServiceCollection(Collection):
+class ServiceCollection(Collection[Service]):
     model: type[Service]
     def create(self, image, command: Incomplete | None = None, **kwargs): ...  # type:ignore[override]
     def get(self, service_id, insert_defaults: Incomplete | None = None): ...
     def list(self, **kwargs): ...
 
 CONTAINER_SPEC_KWARGS: Incomplete
 TASK_TEMPLATE_KWARGS: Incomplete
```

### Comparing `types-docker-7.0.0.20240503/docker-stubs/models/swarm.pyi` & `types-docker-7.0.0.20240506/docker-stubs/types/networks.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from _typeshed import Incomplete
 
-from .resource import Model
-
-class Swarm(Model):
-    id_attribute: str
-    def __init__(self, *args, **kwargs) -> None: ...
-    @property
-    def version(self): ...
-    def get_unlock_key(self): ...
-    def init(
+class EndpointConfig(dict[str, Incomplete]):
+    def __init__(
         self,
-        advertise_addr: Incomplete | None = None,
-        listen_addr: str = "0.0.0.0:2377",
-        force_new_cluster: bool = False,
-        default_addr_pool: Incomplete | None = None,
-        subnet_size: Incomplete | None = None,
-        data_path_addr: Incomplete | None = None,
-        data_path_port: Incomplete | None = None,
-        **kwargs,
-    ): ...
-    def join(self, *args, **kwargs): ...
-    def leave(self, *args, **kwargs): ...
-    attrs: Incomplete
-    def reload(self) -> None: ...
-    def unlock(self, key): ...
-    def update(
+        version,
+        aliases: Incomplete | None = None,
+        links: Incomplete | None = None,
+        ipv4_address: Incomplete | None = None,
+        ipv6_address: Incomplete | None = None,
+        link_local_ips: Incomplete | None = None,
+        driver_opt: Incomplete | None = None,
+        mac_address: Incomplete | None = None,
+    ) -> None: ...
+
+class NetworkingConfig(dict[str, Incomplete]):
+    def __init__(self, endpoints_config: Incomplete | None = None) -> None: ...
+
+class IPAMConfig(dict[str, Incomplete]):
+    def __init__(
+        self, driver: str = "default", pool_configs: Incomplete | None = None, options: Incomplete | None = None
+    ) -> None: ...
+
+class IPAMPool(dict[str, Incomplete]):
+    def __init__(
         self,
-        rotate_worker_token: bool = False,
-        rotate_manager_token: bool = False,
-        rotate_manager_unlock_key: bool = False,
-        **kwargs,
-    ): ...
+        subnet: Incomplete | None = None,
+        iprange: Incomplete | None = None,
+        gateway: Incomplete | None = None,
+        aux_addresses: Incomplete | None = None,
+    ) -> None: ...
```

### Comparing `types-docker-7.0.0.20240503/docker-stubs/transport/npipeconn.pyi` & `types-docker-7.0.0.20240506/docker-stubs/transport/npipeconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/transport/npipesocket.pyi` & `types-docker-7.0.0.20240506/docker-stubs/transport/npipesocket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/transport/unixconn.pyi` & `types-docker-7.0.0.20240506/docker-stubs/transport/unixconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/types/__init__.pyi` & `types-docker-7.0.0.20240506/docker-stubs/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/types/containers.pyi` & `types-docker-7.0.0.20240506/docker-stubs/types/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/types/healthcheck.pyi` & `types-docker-7.0.0.20240506/docker-stubs/types/healthcheck.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/types/services.pyi` & `types-docker-7.0.0.20240506/docker-stubs/types/services.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/types/swarm.pyi` & `types-docker-7.0.0.20240506/docker-stubs/types/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/utils/__init__.pyi` & `types-docker-7.0.0.20240506/docker-stubs/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/utils/build.pyi` & `types-docker-7.0.0.20240506/docker-stubs/utils/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/utils/proxy.pyi` & `types-docker-7.0.0.20240506/docker-stubs/utils/proxy.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/utils/socket.pyi` & `types-docker-7.0.0.20240506/docker-stubs/utils/socket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/docker-stubs/utils/utils.pyi` & `types-docker-7.0.0.20240506/docker-stubs/utils/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240503/setup.py` & `types-docker-7.0.0.20240506/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8c0fc298c53b7e74fe3aad431aa4cfe3772170b3` and was tested
+This package was generated from typeshed commit `8ff50fbea2f607380c23d9b120fccfb1926284e5` and was tested
 with mypy 1.10.0, pyright 1.1.361, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="7.0.0.20240503",
+      version="7.0.0.20240506",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md",
```

### Comparing `types-docker-7.0.0.20240503/types_docker.egg-info/PKG-INFO` & `types-docker-7.0.0.20240506/types_docker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240503
+Version: 7.0.0.20240506
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8c0fc298c53b7e74fe3aad431aa4cfe3772170b3` and was tested
+This package was generated from typeshed commit `8ff50fbea2f607380c23d9b120fccfb1926284e5` and was tested
 with mypy 1.10.0, pyright 1.1.361, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240503/types_docker.egg-info/SOURCES.txt` & `types-docker-7.0.0.20240506/types_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

