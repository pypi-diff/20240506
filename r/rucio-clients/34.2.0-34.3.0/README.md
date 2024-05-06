# Comparing `tmp/rucio_clients-34.2.0.tar.gz` & `tmp/rucio_clients-34.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio_clients-34.2.0.tar", last modified: Tue Apr 16 10:35:08 2024, max compression
+gzip compressed data, was "rucio_clients-34.3.0.tar", last modified: Mon May  6 12:44:10 2024, max compression
```

## Comparing `rucio_clients-34.2.0.tar` & `rucio_clients-34.3.0.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.421055 rucio_clients-34.2.0/
--rwxr-xr-x   0 root         (0) root         (0)     4487 2024-03-19 15:04:29.000000 rucio_clients-34.2.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio_clients-34.2.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio_clients-34.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-16 10:35:04.000000 rucio_clients-34.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2024-04-16 10:35:08.421055 rucio_clients-34.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2024-04-16 07:53:27.000000 rucio_clients-34.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.385055 rucio_clients-34.2.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)   127117 2024-04-09 08:44:02.000000 rucio_clients-34.2.0/bin/rucio
--rwxr-xr-x   0 root         (0) root         (0)   133531 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/bin/rucio-admin
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.386055 rucio_clients-34.2.0/etc/
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio_clients-34.2.0/etc/rse-accounts.cfg.template
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio_clients-34.2.0/etc/rucio.cfg.atlas.client.template
--rw-r--r--   0 root         (0) root         (0)     8534 2024-03-13 10:19:28.000000 rucio_clients-34.2.0/etc/rucio.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.383055 rucio_clients-34.2.0/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.387055 rucio_clients-34.2.0/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/alembicrevision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.391055 rucio_clients-34.2.0/lib/rucio/client/
--rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16353 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/accountclient.py
--rw-r--r--   0 root         (0) root         (0)     5961 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/accountlimitclient.py
--rw-r--r--   0 root         (0) root         (0)    47980 2024-04-08 15:35:56.000000 rucio_clients-34.2.0/lib/rucio/client/baseclient.py
--rw-r--r--   0 root         (0) root         (0)     3079 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/client.py
--rw-r--r--   0 root         (0) root         (0)     4401 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/configclient.py
--rw-r--r--   0 root         (0) root         (0)     1989 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/credentialclient.py
--rw-r--r--   0 root         (0) root         (0)    28378 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/didclient.py
--rw-r--r--   0 root         (0) root         (0)     2114 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/diracclient.py
--rw-r--r--   0 root         (0) root         (0)    86092 2024-04-08 15:35:57.000000 rucio_clients-34.2.0/lib/rucio/client/downloadclient.py
--rw-r--r--   0 root         (0) root         (0)     1575 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/exportclient.py
--rw-r--r--   0 root         (0) root         (0)     1610 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/fileclient.py
--rw-r--r--   0 root         (0) root         (0)     1469 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/importclient.py
--rw-r--r--   0 root         (0) root         (0)     2822 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/lifetimeclient.py
--rw-r--r--   0 root         (0) root         (0)     3914 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/lockclient.py
--rw-r--r--   0 root         (0) root         (0)     5195 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/metaconventionsclient.py
--rw-r--r--   0 root         (0) root         (0)     1390 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/pingclient.py
--rw-r--r--   0 root         (0) root         (0)    19284 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/replicaclient.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/requestclient.py
--rw-r--r--   0 root         (0) root         (0)    27124 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/rseclient.py
--rw-r--r--   0 root         (0) root         (0)    12682 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/ruleclient.py
--rw-r--r--   0 root         (0) root         (0)     3147 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/scopeclient.py
--rw-r--r--   0 root         (0) root         (0)     7971 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/subscriptionclient.py
--rw-r--r--   0 root         (0) root         (0)     2642 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/touchclient.py
--rw-r--r--   0 root         (0) root         (0)    46563 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/client/uploadclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.394055 rucio_clients-34.2.0/lib/rucio/common/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2234 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/lib/rucio/common/cache.py
--rw-r--r--   0 root         (0) root         (0)    24284 2024-04-08 15:14:19.000000 rucio_clients-34.2.0/lib/rucio/common/config.py
--rw-r--r--   0 root         (0) root         (0)     3300 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/constants.py
--rw-r--r--   0 root         (0) root         (0)      726 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/constraints.py
--rwxr-xr-x   0 root         (0) root         (0)     6291 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/didtype.py
--rw-r--r--   0 root         (0) root         (0)    32345 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/exception.py
--rw-r--r--   0 root         (0) root         (0)     1398 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/extra.py
--rw-r--r--   0 root         (0) root         (0)    15046 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/logging.py
--rw-r--r--   0 root         (0) root         (0)    45297 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/lib/rucio/common/pcache.py
--rw-r--r--   0 root         (0) root         (0)     6056 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/lib/rucio/common/plugins.py
--rw-r--r--   0 root         (0) root         (0)     3013 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.396055 rucio_clients-34.2.0/lib/rucio/common/schema/
--rw-r--r--   0 root         (0) root         (0)     5152 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15589 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/atlas.py
--rw-r--r--   0 root         (0) root         (0)    15406 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/belleii.py
--rw-r--r--   0 root         (0) root         (0)    18523 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/cms.py
--rw-r--r--   0 root         (0) root         (0)    14987 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/domatpc.py
--rw-r--r--   0 root         (0) root         (0)    15926 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/escape.py
--rw-r--r--   0 root         (0) root         (0)    16241 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/generic.py
--rw-r--r--   0 root         (0) root         (0)    15468 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)    15277 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/icecube.py
--rw-r--r--   0 root         (0) root         (0)    15885 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/schema/lsst.py
--rw-r--r--   0 root         (0) root         (0)     5414 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/stomp_utils.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     4935 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)     5069 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/common/types.py
--rw-r--r--   0 root         (0) root         (0)    79128 2024-04-08 15:14:19.000000 rucio_clients-34.2.0/lib/rucio/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.396055 rucio_clients-34.2.0/lib/rucio/rse/
--rw-r--r--   0 root         (0) root         (0)     3303 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.400055 rucio_clients-34.2.0/lib/rucio/rse/protocols/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7198 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/bittorrent.py
--rw-r--r--   0 root         (0) root         (0)     4603 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/cache.py
--rw-r--r--   0 root         (0) root         (0)     4225 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/dummy.py
--rw-r--r--   0 root         (0) root         (0)    29093 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/gfal.py
--rw-r--r--   0 root         (0) root         (0)     9680 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/globus.py
--rw-r--r--   0 root         (0) root         (0)     3409 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/gsiftp.py
--rw-r--r--   0 root         (0) root         (0)     2975 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/http_cache.py
--rw-r--r--   0 root         (0) root         (0)     4495 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/mock.py
--rw-r--r--   0 root         (0) root         (0)     7224 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/ngarc.py
--rw-r--r--   0 root         (0) root         (0)    10394 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/posix.py
--rw-r--r--   0 root         (0) root         (0)    22650 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/protocol.py
--rw-r--r--   0 root         (0) root         (0)    15256 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/rclone.py
--rw-r--r--   0 root         (0) root         (0)     5499 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/rfio.py
--rw-r--r--   0 root         (0) root         (0)    14651 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/srm.py
--rw-r--r--   0 root         (0) root         (0)    17467 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/ssh.py
--rw-r--r--   0 root         (0) root         (0)     8127 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/storm.py
--rw-r--r--   0 root         (0) root         (0)    22166 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/webdav.py
--rw-r--r--   0 root         (0) root         (0)    12567 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/protocols/xrootd.py
--rw-r--r--   0 root         (0) root         (0)    37238 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/lib/rucio/rse/rsemanager.py
--rw-r--r--   0 root         (0) root         (0)      244 2024-04-16 07:53:37.000000 rucio_clients-34.2.0/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1577 2024-04-08 15:22:52.000000 rucio_clients-34.2.0/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.419055 rucio_clients-34.2.0/lib/rucio_clients.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5205 2024-04-16 10:35:08.000000 rucio_clients-34.2.0/lib/rucio_clients.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2024-03-13 10:19:28.000000 rucio_clients-34.2.0/pylintrc
--rw-r--r--   0 root         (0) root         (0)     1235 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5048 2024-04-16 07:53:27.000000 rucio_clients-34.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2024-04-16 10:35:08.423055 rucio_clients-34.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3050 2024-04-16 10:35:04.000000 rucio_clients-34.2.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     4778 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.419055 rucio_clients-34.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10677 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3229 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15920 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20523 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13352 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4074 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2181 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4201 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    15058 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3464 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23264 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12425 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107413 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2065 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     8398 2024-04-08 15:14:19.000000 rucio_clients-34.2.0/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1865 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6942 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    96558 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    23797 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7679 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7337 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2618 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28187 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2736 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    58823 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29517 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4185 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7118 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16419 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10867 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3082 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38301 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7953 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10106 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5819 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18584 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57223 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5258 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22277 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20428 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12180 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6299 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2034 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54264 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2759 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11582 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   108356 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7583 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2741 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2023 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27487 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6440 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62385 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    38873 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22741 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    17184 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    12978 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75019 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13184 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8941 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4277 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3267 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3690 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4799 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     3979 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3780 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7746 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    91864 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)    13848 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_schema_cms.py
--rw-r--r--   0 root         (0) root         (0)     7486 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48328 2024-04-02 11:36:32.000000 rucio_clients-34.2.0/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)    55587 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3181 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    25254 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8923 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_transfer_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8412 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15526 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     7427 2024-03-21 13:32:52.000000 rucio_clients-34.2.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:08.419055 rucio_clients-34.2.0/tools/
--rw-r--r--   0 root         (0) root         (0)     6163 2024-03-21 13:32:51.000000 rucio_clients-34.2.0/tools/merge_rucio_configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.743766 rucio_clients-34.3.0/
+-rwxr-xr-x   0 root         (0) root         (0)     4487 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio_clients-34.3.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio_clients-34.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      598 2024-05-06 12:44:07.000000 rucio_clients-34.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-05-06 12:44:10.743766 rucio_clients-34.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.709766 rucio_clients-34.3.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)   127119 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/bin/rucio
+-rwxr-xr-x   0 root         (0) root         (0)   133582 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/bin/rucio-admin
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.710766 rucio_clients-34.3.0/etc/
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio_clients-34.3.0/etc/rse-accounts.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio_clients-34.3.0/etc/rucio.cfg.atlas.client.template
+-rw-r--r--   0 root         (0) root         (0)     8534 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/etc/rucio.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.707766 rucio_clients-34.3.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.711766 rucio_clients-34.3.0/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/alembicrevision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.715766 rucio_clients-34.3.0/lib/rucio/client/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16352 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/accountclient.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/accountlimitclient.py
+-rw-r--r--   0 root         (0) root         (0)    48007 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/baseclient.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     4401 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/configclient.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/credentialclient.py
+-rw-r--r--   0 root         (0) root         (0)    28378 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/didclient.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/diracclient.py
+-rw-r--r--   0 root         (0) root         (0)    86094 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/downloadclient.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/exportclient.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/fileclient.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/importclient.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/lifetimeclient.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/lockclient.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/metaconventionsclient.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/pingclient.py
+-rw-r--r--   0 root         (0) root         (0)    19284 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/replicaclient.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/requestclient.py
+-rw-r--r--   0 root         (0) root         (0)    27121 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/rseclient.py
+-rw-r--r--   0 root         (0) root         (0)    12734 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/ruleclient.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/scopeclient.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/subscriptionclient.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/touchclient.py
+-rw-r--r--   0 root         (0) root         (0)    46627 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/uploadclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.718766 rucio_clients-34.3.0/lib/rucio/common/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/cache.py
+-rw-r--r--   0 root         (0) root         (0)    24636 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/constants.py
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/constraints.py
+-rwxr-xr-x   0 root         (0) root         (0)     6545 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/didtype.py
+-rw-r--r--   0 root         (0) root         (0)    32345 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/exception.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/extra.py
+-rw-r--r--   0 root         (0) root         (0)    15046 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/logging.py
+-rw-r--r--   0 root         (0) root         (0)    45296 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/pcache.py
+-rw-r--r--   0 root         (0) root         (0)     6071 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.720766 rucio_clients-34.3.0/lib/rucio/common/schema/
+-rw-r--r--   0 root         (0) root         (0)     5384 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15589 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    18523 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/cms.py
+-rw-r--r--   0 root         (0) root         (0)    14987 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/domatpc.py
+-rw-r--r--   0 root         (0) root         (0)    15926 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/escape.py
+-rw-r--r--   0 root         (0) root         (0)    16241 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/generic.py
+-rw-r--r--   0 root         (0) root         (0)    15468 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)    15277 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/icecube.py
+-rw-r--r--   0 root         (0) root         (0)    15885 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/lsst.py
+-rw-r--r--   0 root         (0) root         (0)     5414 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/stomp_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)     5427 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/types.py
+-rw-r--r--   0 root         (0) root         (0)    79121 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/lib/rucio/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.720766 rucio_clients-34.3.0/lib/rucio/rse/
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.723766 rucio_clients-34.3.0/lib/rucio/rse/protocols/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7199 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/bittorrent.py
+-rw-r--r--   0 root         (0) root         (0)     4603 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/dummy.py
+-rw-r--r--   0 root         (0) root         (0)    29100 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/gfal.py
+-rw-r--r--   0 root         (0) root         (0)     9730 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/globus.py
+-rw-r--r--   0 root         (0) root         (0)     3411 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/gsiftp.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/http_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/ngarc.py
+-rw-r--r--   0 root         (0) root         (0)    10400 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/posix.py
+-rw-r--r--   0 root         (0) root         (0)    22703 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    15260 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/rclone.py
+-rw-r--r--   0 root         (0) root         (0)     5501 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/rfio.py
+-rw-r--r--   0 root         (0) root         (0)    14655 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/srm.py
+-rw-r--r--   0 root         (0) root         (0)    17473 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     8127 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/storm.py
+-rw-r--r--   0 root         (0) root         (0)    22168 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/webdav.py
+-rw-r--r--   0 root         (0) root         (0)    12571 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/xrootd.py
+-rw-r--r--   0 root         (0) root         (0)    37238 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/rsemanager.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-05-06 11:04:02.000000 rucio_clients-34.3.0/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.741766 rucio_clients-34.3.0/lib/rucio_clients.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5205 2024-05-06 12:44:10.000000 rucio_clients-34.3.0/lib/rucio_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/pylintrc
+-rw-r--r--   0 root         (0) root         (0)     4349 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5235 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-06 12:44:10.745766 rucio_clients-34.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-05-06 12:44:07.000000 rucio_clients-34.3.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.741766 rucio_clients-34.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10677 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15923 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    14964 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23265 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12425 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107450 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6942 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    96724 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    23870 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7728 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28183 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    58823 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29517 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16419 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10869 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38301 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10106 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57290 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5258 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22277 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20429 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54332 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   108359 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7662 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27487 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62453 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    38868 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22796 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    17257 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    13033 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75080 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13184 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8940 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4799 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     3979 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7746 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    91949 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)    13848 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_schema_cms.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48389 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    55587 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    25254 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8924 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_transfer_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    15575 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.741766 rucio_clients-34.3.0/tools/
+-rw-r--r--   0 root         (0) root         (0)     6163 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tools/merge_rucio_configs.py
```

### Comparing `rucio_clients-34.2.0/AUTHORS.rst` & `rucio_clients-34.3.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/LICENSE` & `rucio_clients-34.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/MANIFEST.in` & `rucio_clients-34.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/PKG-INFO` & `rucio_clients-34.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio-clients
-Version: 34.2.0
+Version: 34.3.0
 Summary: Rucio Client Lite Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rucio_clients-34.2.0/README.rst` & `rucio_clients-34.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/bin/rucio` & `rucio_clients-34.3.0/bin/rucio`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         except KeyError as error:
             if 'x-rucio-auth-token' in str(error):
                 used_account = None
                 try:  # get the configured account from the configuration file
                     used_account = '%s (from rucio.cfg)' % config_get('client', 'account')
                 except:
                     pass
-                try:  # are we overriden by the environment?
+                try:  # are we overridden by the environment?
                     used_account = '%s (from RUCIO_ACCOUNT)' % os.environ['RUCIO_ACCOUNT']
                 except:
                     pass
                 logger.error('Specified account %s does not have an associated identity.' % used_account)
             else:
                 logger.debug(traceback.format_exc())
                 contact = config_get('policy', 'support', raise_exception=False)
@@ -1546,15 +1546,15 @@
     %(prog)s list-rse-attributes [options] <field1=value1 field2=value2 ...>
 
     List rses.
 
     """
     client = get_client(args)
     attributes = client.list_rse_attributes(rse=args.rse)
-    table = [(k + ':', str(v)) for (k, v) in sorted(attributes.items())]  # columns hav mixed datatypes
+    table = [(k + ':', str(v)) for (k, v) in sorted(attributes.items())]  # columns have mixed datatypes
     print(tabulate(table, tablefmt='plain', disable_numparse=True))  # disabling number parsing
     return SUCCESS
 
 
 @exception_handler
 def list_rse_usage(args):
     """
```

### Comparing `rucio_clients-34.2.0/bin/rucio-admin` & `rucio_clients-34.3.0/bin/rucio-admin`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from textwrap import dedent
 
 from tabulate import tabulate
 
 from rucio import version
 from rucio.client import Client
 from rucio.common.config import config_get
+from rucio.common.constants import RseAttr
 from rucio.common.exception import (
     AccessDenied,
     AccountNotFound,
     CannotAuthenticate,
     ConfigNotFound,
     DataIdentifierAlreadyExists,
     DataIdentifierNotFound,
@@ -381,15 +382,15 @@
         byte_limit = -1
     else:
         byte_limit = get_bytes_value_from_string(limit_input)
         if not byte_limit:
             try:
                 byte_limit = int(limit_input)
             except ValueError:
-                logger.error('The limit could not be set. Either you misspelled infinity or your input could not be converted to integer or you used a wrong pattern. Please use a format like 10GB with B,KB,MB,GB,TB,PB as units (not case sensistive)')
+                logger.error('The limit could not be set. Either you misspelled infinity or your input could not be converted to integer or you used a wrong pattern. Please use a format like 10GB with B,KB,MB,GB,TB,PB as units (not case sensitive)')
                 return FAILURE
 
     client.set_account_limit(account=args.account, rse=args.rse, bytes_=byte_limit, locality=locality)
     print('Set account limit for account %s on RSE %s: %s' % (args.account, args.rse, sizefmt(byte_limit, True)))
     return SUCCESS
 
 
@@ -1240,15 +1241,15 @@
                 result = list(pfn.values())[0]
             except ReplicaNotFound as error:
                 result = error
             if isinstance(result, (RSEOperationNotSupported, ReplicaNotFound)):
                 if not rse_info['deterministic']:
                     logger.warning('This is a non-deterministic site, so the real PFN might be different from the on suggested')
                     rse_attr = client.list_rse_attributes(rse)
-                    naming_convention = rse_attr.get('naming_convention', None)
+                    naming_convention = rse_attr.get(RseAttr.NAMING_CONVENTION, None)
                     parents = [did for did in client.list_parent_dids(scope, name)]
                     if len(parents) > 1:
                         logger.warning('The file has multiple parents')
                     for did in parents:
                         if did['type'] == 'DATASET':
                             path = construct_surl(did['name'], scope, name, naming_convention=naming_convention)
                             pfn = ''.join([proto.attributes['scheme'],
@@ -1379,15 +1380,15 @@
     oparser.add_argument('--oidc-auto', dest='oidc_auto', default=False, action='store_true', help='If not specified, username and password credentials are not required and users will be given a URL '
                          + 'to use in their browser. If specified, the users explicitly trust Rucio with their IdP credentials.')  # NOQA: W503
     oparser.add_argument('--oidc-polling', dest='oidc_polling', default=False, action='store_true', help='If not specified, user will be asked to enter a code returned by the browser to the command line. '
                          + 'If --polling is set, Rucio Client should get the token without any further interaction of the user. This option is active only if --auto is *not* specified.')  # NOQA: W503
     oparser.add_argument('--oidc-refresh-lifetime', dest='oidc_refresh_lifetime', default=None, help='Max lifetime in hours for this an access token will be refreshed by asynchronous Rucio daemon. '
                          + 'If not specified, refresh will be stopped after 4 days. This option is effective only if --oidc-scope includes offline_access scope for a refresh token to be granted to Rucio.')  # NOQA: W503
     oparser.add_argument('--oidc-issuer', dest='oidc_issuer', default=None,
-                         help='Defines which Identity Provider is goign to be used. The issuer string must correspond '
+                         help='Defines which Identity Provider is going to be used. The issuer string must correspond '
                          + 'to the keys configured in the /etc/idpsecrets.json auth server configuration file.')  # NOQA: W503
 
     # Options for the x509  auth_strategy
     oparser.add_argument('--certificate', dest='certificate', default=None, help='Client certificate file')
     oparser.add_argument('--ca-certificate', dest='ca_certificate', default=None, help='CA certificate to verify peer against (SSL)')
 
     # The import export subparser
@@ -1428,15 +1429,15 @@
     list_account_parser = account_subparser.add_parser('list',
                                                        help='List Rucio accounts.',
                                                        formatter_class=argparse.RawDescriptionHelpFormatter,
                                                        epilog='Usage example\n'
                                                               '"""""""""""""\n'
                                                               '::\n'
                                                               '\n'
-                                                              '    $ rucio-admin account list --type \'user\'\n'
+                                                              '    $ rucio-admin account list --type USER\n'
                                                               '\n')
     list_account_parser.add_argument('--type', dest='account_type', action='store', help='Account Type (USER, GROUP, SERVICE)')
     list_account_parser.add_argument('--id', dest='identity', action='store', help='Identity (e.g. DN)')
     list_account_parser.add_argument('--filters', dest='filters', action='store', help='Filter arguments in form `key=value,another_key=next_value`')
     list_account_parser.set_defaults(which='list_accounts')
 
     # The list_account_attributes command
@@ -1704,15 +1705,15 @@
                                                            epilog='Usage example\n'
                                                                   '"""""""""""""\n'
                                                                   '::\n'
                                                                   '\n'
                                                                   '    $ rucio-admin identity delete --account jdoe --type X509 --id \'CN=Joe Doe,CN=707658,CN=jdoe,OU=Users,OU=Organic Units,DC=cern,DC=ch\'\n'
                                                                   '    Deleted identity: CN=Joe Doe,CN=707658,CN=jdoe,OU=Users,OU=Organic Units,DC=cern,DC=ch\n'
                                                                   '\n'
-                                                                  'Note: if the identity was accidentaly deleted, use add option.\n'
+                                                                  'Note: if the identity was accidentally deleted, use add option.\n'
                                                                   '\n')
     identity_delete_parser.set_defaults(which='identity_delete')
     identity_delete_parser.add_argument('--account', dest='account', action='store', help='Account name', required=True)
     identity_delete_parser.add_argument('--type', dest='authtype', action='store', choices=['X509', 'GSS', 'USERPASS', 'SSH', 'SAML', 'OIDC'], help='Authentication type [X509|GSS|USERPASS|SSH|SAML|OIDC]', required=True)
     identity_delete_parser.add_argument('--id', dest='identity', action='store', help='Identity', required=True)
 
     # The RSE subparser
@@ -1952,15 +1953,15 @@
                                                        epilog='Usage example\n'
                                                               '"""""""""""""\n'
                                                               '::\n'
                                                               '\n'
                                                               '    $ rucio-admin rse add-protocol --hostname jdoes.test.org --scheme gsiftp --prefix \'/atlasdatadisk/rucio/\' --port 8443 JDOE_DATADISK\n'
                                                               '\n'
                                                               'Note: no printed stdout.\n'
-                                                              'Note: examples of optional parametres::\n'
+                                                              'Note: examples of optional parameters::\n'
                                                               '\n'
                                                               '    --space-token DATADISK\n'
                                                               '    --web-service-path \'/srm/managerv2?SFN=\'\n'
                                                               '    --port 8443\n'
                                                               '    --impl \'rucio.rse.protocols.gfal.Default\'\n'
                                                               '      (for other protocol implementation, replace gfal2 with impl. name, e.g. srm)\n'
                                                               '    --domain-json\n'
@@ -2106,15 +2107,15 @@
                                                           'Note: alternatively: rucio list-scopes.\n'
                                                           '\n')
     list_scope_parser.set_defaults(which='list_scopes')
     list_scope_parser.add_argument('--account', dest='account', action='store', help='Account name')
 
     # The config subparser
     config_parser = subparsers.add_parser('config',
-                                          help='Configuration methods. The global configuration of data mangement system can by modified.',
+                                          help='Configuration methods. The global configuration of data management system can by modified.',
                                           formatter_class=argparse.RawDescriptionHelpFormatter,
                                           epilog='''e.g. quotas, daemons, rses''')
     config_subparser = config_parser.add_subparsers(dest='config_subcommand', **required_arg)
 
     # The get_config command
     get_config_parser = config_subparser.add_parser('get',
                                                     help='Get matching configuration.',
@@ -2307,17 +2308,17 @@
                                                                        '\n')
     declare_bad_file_replicas_parser.set_defaults(which='declare_bad_file_replicas')
     declare_bad_file_replicas_parser.add_argument(dest='listbadfiles', action='store', nargs='*', help='List of bad items. Each can be a PFN (for one replica) or an LFN (for all replicas of the LFN) or a collection DID (for all file replicas in the DID)')
     declare_bad_file_replicas_parser.add_argument('--reason', dest='reason', required=True, action='store', help='Reason')
     declare_bad_file_replicas_parser.add_argument('--inputfile', dest='inputfile', nargs='?', action='store', help='File containing list of bad items')
     declare_bad_file_replicas_parser.add_argument('--allow-collection', dest='allow_collection', action='store_true', help='Allow passing a collection DID as bad item')
 
-    declare_bad_file_replicas_parser.add_argument('--lfns', dest='lfns', nargs='?', action='store', help='File cotaining list of LFNs for bad replicas. Requires --rse and --scope')
-    declare_bad_file_replicas_parser.add_argument('--scope', dest='scope', nargs='?', action='store', help='Common scope for bad replicas secified with LFN list, ignored wthout --lfns')
-    declare_bad_file_replicas_parser.add_argument('--rse', dest='rse', nargs='?', action='store', help='Common RSE for bad replicas secified with LFN list, ignored wthout --lfns')
+    declare_bad_file_replicas_parser.add_argument('--lfns', dest='lfns', nargs='?', action='store', help='File containing list of LFNs for bad replicas. Requires --rse and --scope')
+    declare_bad_file_replicas_parser.add_argument('--scope', dest='scope', nargs='?', action='store', help='Common scope for bad replicas specified with LFN list, ignored without --lfns')
+    declare_bad_file_replicas_parser.add_argument('--rse', dest='rse', nargs='?', action='store', help='Common RSE for bad replicas specified with LFN list, ignored without --lfns')
 
     # The declare-temporary-unavailable command
     declare_temporary_unavailable_replicas_parser = rep_subparser.add_parser('declare-temporary-unavailable',
                                                                              help='Declare temporary unavailable replicas',
                                                                              formatter_class=argparse.RawDescriptionHelpFormatter,
                                                                              epilog='Usage example\n'
                                                                                     '"""""""""""""\n'
```

### Comparing `rucio_clients-34.2.0/etc/rse-accounts.cfg.template` & `rucio_clients-34.3.0/etc/rse-accounts.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/etc/rucio.cfg.atlas.client.template` & `rucio_clients-34.3.0/etc/rucio.cfg.atlas.client.template`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/etc/rucio.cfg.template` & `rucio_clients-34.3.0/etc/rucio.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/__init__.py` & `rucio_clients-34.3.0/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/alembicrevision.py` & `rucio_clients-34.3.0/lib/rucio/alembicrevision.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/__init__.py` & `rucio_clients-34.3.0/lib/rucio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/accountclient.py` & `rucio_clients-34.3.0/lib/rucio/client/accountclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     def list_accounts(self, account_type=None, identity=None, filters=None):
         """
         Sends the request to list all rucio accounts.
 
         :param type: The account type
         :param identity: The identity key name. For example x509 DN, or a username.
-        :param filters: A dictionnary key:account attribute to use for the filtering
+        :param filters: A dictionary key:account attribute to use for the filtering
 
         :return: a list containing account info dictionary for all rucio accounts.
         :raises AccountNotFound: if account doesn't exist.
         """
         path = '/'.join([self.ACCOUNTS_BASEURL])
         url = build_url(choice(self.list_hosts), path=path)
         params = {}
```

### Comparing `rucio_clients-34.2.0/lib/rucio/client/accountlimitclient.py` & `rucio_clients-34.3.0/lib/rucio/client/accountlimitclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/baseclient.py` & `rucio_clients-34.3.0/lib/rucio/client/baseclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 
 import errno
 import getpass
 import os
 import secrets
 import sys
 import time
+from collections.abc import Generator
 from configparser import NoOptionError, NoSectionError
 from logging import Logger
 from os import environ, fdopen, geteuid, makedirs, path
 from shutil import move
 from tempfile import mkstemp
-from typing import Any, Generator, Optional
+from typing import Any, Optional
 from urllib.parse import urlparse
 
 import requests
 from dogpile.cache import make_region
 from requests import Response, Session
 from requests.exceptions import ConnectionError
 from requests.status_codes import codes
@@ -231,15 +232,15 @@
                     raise MissingClientParameter('Option \'%s\' cannot be found in config file' % error.args[0])
         return auth_type
 
     def _get_creds(self, creds: Optional[dict[str, Any]]) -> dict[str, Any]:
         if self.auth_type == 'oidc':
             if not creds:
                 creds = {}
-            # if there are defautl values, check if rucio.cfg does not specify them, otherwise put default
+            # if there are default values, check if rucio.cfg does not specify them, otherwise put default
             if 'oidc_refresh_lifetime' not in creds or creds['oidc_refresh_lifetime'] is None:
                 creds['oidc_refresh_lifetime'] = config_get('client', 'oidc_refresh_lifetime', False, None)
             if 'oidc_issuer' not in creds or creds['oidc_issuer'] is None:
                 creds['oidc_issuer'] = config_get('client', 'oidc_issuer', False, None)
             if 'oidc_audience' not in creds or creds['oidc_audience'] is None:
                 creds['oidc_audience'] = config_get('client', 'oidc_audience', False, None)
             if 'oidc_auto' not in creds or creds['oidc_auto'] is False:
@@ -611,15 +612,15 @@
                     else:
                         print("The Rucio Auth Server did not respond as expected. Please, "
                               + "try again and make sure you typed the correct code.")  # NOQA: W503
                         count += 1
 
         else:
             print("\nAccording to the OAuth2/OIDC standard you should NOT be sharing \n"
-                  + "your password with any 3rd party appplication, therefore, \n"  # NOQA: W503
+                  + "your password with any 3rd party application, therefore, \n"  # NOQA: W503
                   + "we strongly discourage you from following this --oidc-auto approach.")  # NOQA: W503
             print("-------------------------------------------------------------------------")
             auth_res = self._send_request(auth_url, get_token=True)
             # getting the login URL and logging in the user
             login_url = auth_res.url
             start = time.time()
             result = self._send_request(login_url, type_='POST', data=userpass)
@@ -654,15 +655,15 @@
             exc_cls, exc_msg = self._get_exception(headers=result.headers,
                                                    status_code=result.status_code,
                                                    data=result.content)
             raise exc_cls(exc_msg)
 
         self.auth_token = result.headers['x-rucio-auth-token']
         if self.auth_oidc_refresh_active:
-            self.logger.debug("Reseting the token expiration epoch file content.")
+            self.logger.debug("Resetting the token expiration epoch file content.")
             # reset the token expiration epoch file content
             # at new CLI OIDC authentication
             self.token_exp_epoch = None
             file_d, file_n = mkstemp(dir=self.token_path)
             with fdopen(file_d, "w") as f_exp_epoch:
                 f_exp_epoch.write(str(self.token_exp_epoch))
             move(file_n, self.token_exp_epoch_file)
```

### Comparing `rucio_clients-34.2.0/lib/rucio/client/client.py` & `rucio_clients-34.3.0/lib/rucio/client/client.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/configclient.py` & `rucio_clients-34.3.0/lib/rucio/client/configclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/credentialclient.py` & `rucio_clients-34.3.0/lib/rucio/client/credentialclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/didclient.py` & `rucio_clients-34.3.0/lib/rucio/client/didclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         :param did_type: The type of the did: 'all'(container, dataset or file)|'collection'(dataset or container)|'dataset'|'container'|'file'
         :param long: Long format option to display more information for each DID.
         :param recursive: Recursively list DIDs content.
         """
         path = '/'.join([self.DIDS_BASEURL, quote_plus(scope), 'dids', 'search'])
 
         # stringify dates.
-        if isinstance(filters, dict):   # backwards compatability for filters as single {}
+        if isinstance(filters, dict):   # backwards compatibility for filters as single {}
             filters = [filters]
         for or_group in filters:
             for key, value in or_group.items():
                 if isinstance(value, datetime):
                     or_group[key] = date_to_str(value)
 
         payload = {
```

### Comparing `rucio_clients-34.2.0/lib/rucio/client/diracclient.py` & `rucio_clients-34.3.0/lib/rucio/client/diracclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/downloadclient.py` & `rucio_clients-34.3.0/lib/rucio/client/downloadclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
             rse                            - Optional: rse name (e.g. 'CERN-PROD_DATADISK') or rse expression from where to download
             impl                           - Optional: name of the protocol implementation to be used to download this item.
             no_resolve_archives            - Optional: bool indicating whether archives should not be considered for download (Default: False)
             resolve_archives               - Deprecated: Use no_resolve_archives instead
             force_scheme                   - Optional: force a specific scheme to download this item. (Default: None)
             base_dir                       - Optional: base directory where the downloaded files will be stored. (Default: '.')
             no_subdir                      - Optional: If true, files are written directly into base_dir. (Default: False)
-            nrandom                        - Optional: if the DID addresses a dataset, nrandom files will be randomly choosen for download from the dataset
+            nrandom                        - Optional: if the DID addresses a dataset, nrandom files will be randomly chosen for download from the dataset
             ignore_checksum                - Optional: If true, skips the checksum validation between the downloaded file and the rucio catalouge. (Default: False)
             transfer_timeout               - Optional: Timeout time for the download protocols. (Default: None)
             transfer_speed_timeout         - Optional: Minimum allowed transfer speed (in KBps). Ignored if transfer_timeout set. Otherwise, used to compute default timeout (Default: 500)
             check_local_with_filesize_only - Optional: If true, already downloaded files will not be validated by checksum.
         :param num_threads: Suggestion of number of threads to use for the download. It will be lowered if it's too high.
         :param trace_custom_fields: Custom key value pairs to send with the traces.
         :param traces_copy_out: reference to an external list, where the traces should be uploaded
@@ -667,18 +667,18 @@
         dest_file_path_iter = iter(dest_file_paths)
         first_dest_file_path = next(dest_file_path_iter)
         logger(logging.DEBUG, "renaming '%s' to '%s'" % (temp_file_path, first_dest_file_path))
         os.rename(temp_file_path, first_dest_file_path)
 
         # if the file was downloaded with success, it can be linked to pcache
         if pcache:
-            logger(logging.INFO, 'File %s is going to be registerred into pcache.' % dest_file_path)
+            logger(logging.INFO, 'File %s is going to be registered into pcache.' % dest_file_path)
             try:
                 pcache_state, hardlink_state = pcache.check_and_link(src=pfn, storage_root=storage_prefix, local_src=first_dest_file_path)
-                logger(logging.INFO, 'File %s is now registerred into pcache.' % first_dest_file_path)
+                logger(logging.INFO, 'File %s is now registered into pcache.' % first_dest_file_path)
             except Exception as e:
                 logger(logging.WARNING, 'Failed to load file to pcache: %s' % str(e))
 
         for cur_dest_file_path in dest_file_path_iter:
             logger(logging.DEBUG, "copying '%s' to '%s'" % (first_dest_file_path, cur_dest_file_path))
             shutil.copy2(first_dest_file_path, cur_dest_file_path)
 
@@ -737,15 +737,15 @@
         Aria2c needs to be installed and X509_USER_PROXY needs to be set!
 
         :param items: List of dictionaries. Each dictionary describing an item to download. Keys:
             did                            - DID string of this file (e.g. 'scope:file.name'). Wildcards are not allowed
             rse                            - Optional: rse name (e.g. 'CERN-PROD_DATADISK') or rse expression from where to download
             base_dir                       - Optional: base directory where the downloaded files will be stored. (Default: '.')
             no_subdir                      - Optional: If true, files are written directly into base_dir. (Default: False)
-            nrandom                        - Optional: if the DID addresses a dataset, nrandom files will be randomly choosen for download from the dataset
+            nrandom                        - Optional: if the DID addresses a dataset, nrandom files will be randomly chosen for download from the dataset
             ignore_checksum                - Optional: If true, skips the checksum validation between the downloaded file and the rucio catalouge. (Default: False)
             check_local_with_filesize_only - Optional: If true, already downloaded files will not be validated by checksum.
 
         :param trace_custom_fields: Custom key value pairs to send with the traces
         :param filters: dictionary containing filter options
         :param deactivate_file_download_exceptions: Boolean, if file download exceptions shouldn't be raised
         :param sort: Select best replica by replica sorting algorithm. Available algorithms:
@@ -794,15 +794,15 @@
         """
         Starts aria2c in RPC mode as a subprocess. Also creates
         the RPC proxy instance.
         (This function is meant to be used as class internal only)
 
         :param rpc_secret: the secret for the RPC proxy
 
-        :returns: a tupel with the process and the rpc proxy objects
+        :returns: a tuple with the process and the rpc proxy objects
 
         :raises RucioException: if the process or the proxy could not be created
         """
         logger = self.logger
         from xmlrpc.client import ServerProxy as RPCServerProxy
 
         cmd = 'aria2c '\
@@ -954,15 +954,15 @@
                 file_scope = item['scope']
                 file_name = item['name']
                 file_did_str = '%s:%s' % (file_scope, file_name)
                 temp_file_path = item['temp_file_path']
                 # workaround: only consider first dest file path for aria2c download
                 dest_file_path = next(iter(item['dest_file_paths']))
 
-                # ensure we didnt miss the active state (e.g. a very fast download)
+                # ensure we didn't miss the active state (e.g. a very fast download)
                 start_time = item.setdefault('transferStart', time.time())
                 end_time = item.setdefault('transferEnd', time.time())
 
                 # get used pfn for traces
                 trace = item['trace']
                 for uri in dlinfo['files'][0]['uris']:
                     if uri['status'].lower() == 'used':
@@ -1089,15 +1089,15 @@
                     logger(logging.DEBUG, item)
                     raise InputValidationError('Item without did and filter/scope')
         if resolve_archives:
             # perhaps we'll need an extraction tool so check what is installed
             self.extraction_tools = [tool for tool in self.extraction_tools if tool.is_useable()]
             if len(self.extraction_tools) < 1:
                 logger(logging.WARNING, 'Archive resolution is enabled but no extraction tool is available. '
-                                        'Sources whose protocol doesnt support extraction wont be considered for download.')
+                                        'Sources whose protocol does not support extraction will not be considered for download.')
 
         # if excluding tapes, we need to list them first
         tape_rses = []
         if self.is_tape_excluded:
             try:
                 tape_rses = [endp['rse'] for endp in self.client.list_rses(rse_expression='istape=true')]
             except:
@@ -1106,15 +1106,15 @@
         # Matches each dereferenced DID back to a list of input items
         did_to_input_items = {}
 
         # Resolve DIDs
         for item in input_items:
             resolved_dids = list(self._resolve_one_item_dids(item))
             if not resolved_dids:
-                logger(logging.WARNING, 'An item didnt have any DIDs after resolving the input: %s.' % item.get('did', item))
+                logger(logging.WARNING, 'An item did not have any DIDs after resolving the input: %s.' % item.get('did', item))
             item['dids'] = resolved_dids
             for did in resolved_dids:
                 did_to_input_items.setdefault(DID(did), []).append(item)
 
                 if 'CONTAINER' in did.get('did_type', '').upper() or ('length' in did and not did['length']):
                     did_with_size = self.client.get_did(scope=did['scope'], name=did['name'], dynamic_depth='FILE')
                     did['length'] = did_with_size['length']
@@ -1338,15 +1338,15 @@
             if not options:
                 continue
             resolve_archives = options.get('resolve_archives')
             file_item['merged_options'] = options
             file_item['dest_file_paths'] = list(dest_file_paths)
             file_item['temp_file_path'] = '%s.part' % file_item['dest_file_paths'][0]
 
-            # the file did str ist not an unique key for this dict because multiple calls of list_replicas
+            # the file did str is not an unique key for this dict because multiple calls of list_replicas
             # could result in the same DID multiple times. So we're using the id of the dictionary objects
             fiid = id(file_item)
             fiid_to_file_item[fiid] = file_item
 
             if resolve_archives:
                 min_cea_priority = None
                 num_non_cea_sources = 0
@@ -1496,15 +1496,15 @@
         return download_packs
 
     def _split_did_str(self, did_str):
         """
         Splits a given DID string (e.g. 'scope1:name.file') into its scope and name part
         (This function is meant to be used as class internal only)
 
-        :param did_str: the DID string that will be splitted
+        :param did_str: the DID string that will be split
 
         :returns: the scope- and name part of the given DID
 
         :raises InputValidationError: if the given DID string is not valid
         """
         did = did_str.split(':')
         if len(did) == 2:
@@ -1534,15 +1534,15 @@
         destination directory if it's not existent.
         (This function is meant to be used as class internal only)
 
         :param base_dir: base directory part
         :param dest_dir_name: name of the destination directory
         :param no_subdir: if no subdirectory should be created
 
-        :returns: the absolut path of the destination directory
+        :returns: the absolute path of the destination directory
         """
         # append dest_dir_name, if subdir should be used
         if dest_dir_name.startswith('/'):
             dest_dir_name = dest_dir_name[1:]
         dest_dir_path = os.path.join(os.path.abspath(base_dir), '' if no_subdir else dest_dir_name)
 
         if not os.path.isdir(dest_dir_path):
```

### Comparing `rucio_clients-34.2.0/lib/rucio/client/exportclient.py` & `rucio_clients-34.3.0/lib/rucio/client/exportclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/fileclient.py` & `rucio_clients-34.3.0/lib/rucio/client/fileclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/importclient.py` & `rucio_clients-34.3.0/lib/rucio/client/importclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/lifetimeclient.py` & `rucio_clients-34.3.0/lib/rucio/client/lifetimeclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/lockclient.py` & `rucio_clients-34.3.0/lib/rucio/client/lockclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/metaconventionsclient.py` & `rucio_clients-34.3.0/lib/rucio/client/metaconventionsclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/pingclient.py` & `rucio_clients-34.3.0/lib/rucio/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/replicaclient.py` & `rucio_clients-34.3.0/lib/rucio/client/replicaclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/requestclient.py` & `rucio_clients-34.3.0/lib/rucio/client/requestclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/rseclient.py` & `rucio_clients-34.3.0/lib/rucio/client/rseclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         raise exc_cls(exc_msg)
 
     def update_rse(self, rse, parameters):
         """
         Update RSE properties like availability or name.
 
         :param rse: the name of the new rse.
-        :param  parameters: A dictionnary with property (name, read, write, delete as keys).
+        :param  parameters: A dictionary with property (name, read, write, delete as keys).
         """
         path = 'rses/' + rse
         url = build_url(choice(self.list_hosts), path=path)
         r = self._send_request(url, type_='PUT', data=dumps(parameters))
         if r.status_code == codes.created:
             return True
         exc_cls, exc_msg = self._get_exception(headers=r.headers, status_code=r.status_code, data=r.content)
@@ -337,15 +337,15 @@
     def update_protocols(self, rse, scheme, data, hostname=None, port=None):
         """
         Updates matching protocols from RSE. Protocol using the same identifier can be
         distinguished by hostname and port.
 
         :param rse: the RSE name.
         :param scheme: identifier of the protocol.
-        :param data: A dict providing the new values of the protocol attibutes.
+        :param data: A dict providing the new values of the protocol attributes.
                      Keys must match column names in database.
         :param hostname: hostname of the protocol.
         :param port: port of the protocol.
 
         :returns: True if success.
 
         :raises RSEProtocolNotSupported: if no matching protocol entry could be found.
@@ -508,15 +508,15 @@
     def list_rse_usage_history(self, rse, filters=None):
         """
         List RSE usage history information.
 
         :param rse: The RSE name.
         :param filters: dictionary of attributes by which the results should be filtered.
 
-        :returns:  list of dictionnaries.
+        :returns:  list of dictionaries.
         """
         path = [self.RSE_BASEURL, rse, 'usage', 'history']
         path = '/'.join(path)
         url = build_url(choice(self.list_hosts), path=path)
         r = self._send_request(url, type_='GET', params=filters)
         if r.status_code == codes.ok:
             return self._load_json_data(r)
@@ -589,15 +589,15 @@
 
     def add_distance(self, source, destination, parameters):
         """
         Add a src-dest distance.
 
         :param source: The source.
         :param destination: The destination.
-        :param parameters: A dictionnary with property.
+        :param parameters: A dictionary with property.
         """
         path = [self.RSE_BASEURL, source, 'distances', destination]
         path = '/'.join(path)
         url = build_url(choice(self.list_hosts), path=path)
         r = self._send_request(url, type_='POST', data=dumps(parameters))
         if r.status_code == codes.created:
             return True
@@ -608,15 +608,15 @@
 
     def update_distance(self, source, destination, parameters):
         """
         Update distances with the given RSE ids.
 
         :param source: The source.
         :param destination: The destination.
-        :param parameters: A dictionnary with property.
+        :param parameters: A dictionary with property.
         """
         path = [self.RSE_BASEURL, source, 'distances', destination]
         path = '/'.join(path)
         url = build_url(choice(self.list_hosts), path=path)
         r = self._send_request(url, type_='PUT', data=dumps(parameters))
         if r.status_code == codes.ok:
             return True
```

### Comparing `rucio_clients-34.2.0/lib/rucio/client/ruleclient.py` & `rucio_clients-34.3.0/lib/rucio/client/ruleclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from collections.abc import Sequence
 from json import dumps, loads
 from typing import Any, Optional, Union
 from urllib.parse import quote_plus
 
 from requests.status_codes import codes
 
 from rucio.client.baseclient import BaseClient, choice
@@ -26,15 +27,15 @@
 
     """RuleClient class for working with replication rules"""
 
     RULE_BASEURL = 'rules'
 
     def add_replication_rule(
         self,
-        dids: list[str],
+        dids: Sequence[dict[str, str]],
         copies: int,
         rse_expression: str,
         priority: int = 3,
         lifetime: Optional[int] = None,
         grouping: str = 'DATASET',
         notify: str = 'N',
         source_replica_expression: Optional[str] = None,
```

### Comparing `rucio_clients-34.2.0/lib/rucio/client/scopeclient.py` & `rucio_clients-34.3.0/lib/rucio/client/scopeclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/subscriptionclient.py` & `rucio_clients-34.3.0/lib/rucio/client/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/touchclient.py` & `rucio_clients-34.3.0/lib/rucio/client/touchclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/client/uploadclient.py` & `rucio_clients-34.3.0/lib/rucio/client/uploadclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import random
 import socket
 import time
 
 from rucio import version
 from rucio.client.client import Client
 from rucio.common.config import config_get, config_get_bool, config_get_int
+from rucio.common.constants import RseAttr
 from rucio.common.exception import (
     DataIdentifierAlreadyExists,
     DataIdentifierNotFound,
     FileReplicaAlreadyExists,
     InputValidationError,
     NoFilesUploaded,
     NotAllFilesUploaded,
@@ -191,16 +192,16 @@
             # resolving local area networks
             domain = 'wan'
             rse_attributes = {}
             try:
                 rse_attributes = self.client.list_rse_attributes(rse)
             except:
                 logger(logging.WARNING, 'Attributes of the RSE: %s not available.' % rse)
-            if (self.client_location and 'lan' in rse_settings['domain'] and 'site' in rse_attributes):
-                if self.client_location['site'] == rse_attributes['site']:
+            if (self.client_location and 'lan' in rse_settings['domain'] and RseAttr.SITE in rse_attributes):
+                if self.client_location['site'] == rse_attributes[RseAttr.SITE]:
                     domain = 'lan'
             logger(logging.DEBUG, '{} domain is used for the upload'.format(domain))
 
             # FIXME:
             # Rewrite preferred_impl selection - also check test_upload.py/test_download.py and fix impl order (see FIXME there)
             #
             # if not impl and not force_scheme:
@@ -454,15 +455,15 @@
             if status != 0:
                 msg = 'Trying to upload ROOT files but pool_extractFileIdentifier tool can not be found.\n'
                 msg += 'Setup your ATHENA environment and try again.'
                 raise RucioException(msg)
             try:
                 guid = output.splitlines()[-1].split()[0].replace('-', '').lower()
             except Exception:
-                raise RucioException('Error extracting GUID from ouput of pool_extractFileIdentifier')
+                raise RucioException('Error extracting GUID from output of pool_extractFileIdentifier')
         elif guid:
             guid = guid.replace('-', '')
         else:
             guid = generate_uuid()
         return guid
 
     def _collect_file_info(self, filepath, item):
@@ -670,15 +671,15 @@
         try:
             retry(protocol_write.put, base_name, pfn_tmp, source_dir, transfer_timeout=transfer_timeout)(mtries=2, logger=logger)
             logger(logging.INFO, 'Successful upload of temporary file. {}'.format(pfn_tmp))
         except Exception as error:
             raise RSEOperationNotSupported(str(error))
 
         # Is stat after that upload allowed?
-        skip_upload_stat = rse_attributes.get('skip_upload_stat', False)
+        skip_upload_stat = rse_attributes.get(RseAttr.SKIP_UPLOAD_STAT, False)
         self.logger(logging.DEBUG, 'skip_upload_stat=%s', skip_upload_stat)
 
         # Checksum verification, obsolete, see Gabriele changes.
         if not skip_upload_stat:
             try:
                 stats = self._retry_protocol_stat(protocol_write, pfn_tmp)
                 if not isinstance(stats, dict):
@@ -736,15 +737,15 @@
                     raise error
                 self.logger(logging.DEBUG, 'stat: unknown edge case, retrying in %ss' % 2**attempt)
                 time.sleep(2**attempt)
         return protocol.stat(pfn)
 
     def _create_protocol(self, rse_settings, operation, impl=None, force_scheme=None, domain='wan'):
         """
-        Protol construction.
+        Protocol construction.
         :param rse_settings:        rse_settings
         :param operation:           activity, e.g. read, write, delete etc.
         :param force_scheme:        custom scheme
         :param auth_token: Optionally passing JSON Web Token (OIDC) string for authentication
         """
         try:
             protocol = rsemgr.create_protocol(rse_settings, operation, scheme=force_scheme, domain=domain, impl=impl, auth_token=self.auth_token, logger=self.logger)
```

### Comparing `rucio_clients-34.2.0/lib/rucio/common/__init__.py` & `rucio_clients-34.3.0/lib/rucio/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/cache.py` & `rucio_clients-34.3.0/lib/rucio/common/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from rucio.common.config import config_get
 from rucio.common.utils import is_client
 
 if TYPE_CHECKING:
     from collections.abc import Callable
     from typing import Optional
 
+    from dogpile.cache.region import CacheRegion
+
 CACHE_URL = config_get('cache', 'url', False, '127.0.0.1:11211', check_config_table=False)
 
 ENABLE_CACHING = True
 _mc_client = None
 try:
     if is_client():
         ENABLE_CACHING = False
@@ -43,15 +45,15 @@
         _mc_client.close()
 
 
 def make_region_memcached(
         expiration_time: int,
         function_key_generator: "Optional[Callable]" = None,
         memcached_expire_time: "Optional[int]" = None
-):
+) -> "CacheRegion":
     """
     Make and configure a dogpile.cache.pymemcache region
     """
     if function_key_generator:
         region = make_region(function_key_generator=function_key_generator)
     else:
         region = make_region()
```

### Comparing `rucio_clients-34.2.0/lib/rucio/common/config.py` & `rucio_clients-34.3.0/lib/rucio/common/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 
 """Provides functions to access the local configuration. The configuration locations are provided by get_config_dirs."""
 
 import configparser
 import json
 import os
 from collections.abc import Callable
-from typing import TYPE_CHECKING, Optional, TypeVar, Union, overload
+from typing import TYPE_CHECKING, Any, Optional, TypeVar, Union, overload
 
 from rucio.common import exception
 from rucio.common.exception import ConfigNotFound, DatabaseException
 
 _T = TypeVar('_T')
 _U = TypeVar('_U')
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
 
-def convert_to_any_type(value) -> Union[bool, int, float, str]:
+def convert_to_any_type(value: str) -> Union[bool, int, float, str]:
     if value.lower() in ['true', 'yes', 'on']:
         return True
     elif value.lower() in ['false', 'no', 'off']:
         return False
 
     for conv in (int, float):
         try:
             return conv(value)
         except:
             pass
 
     return value
 
 
-def _convert_to_boolean(value):
+def _convert_to_boolean(value: Union[str, bool]) -> bool:
     if isinstance(value, bool):
         return value
     if value.lower() in ['true', 'yes', 'on', '1']:
         return True
     elif value.lower() in ['false', 'no', 'off', '0']:
         return False
     raise ValueError('Not a boolean: %s' % value)
@@ -293,34 +293,34 @@
     ...
 
 
 @overload
 def config_get_int(
         section: str,
         option: str,
-        raise_exception,
+        raise_exception: bool,
         default: _T = ...,
         *,
         check_config_table: bool = ...,
         session: "Optional[Session]" = ...,
         use_cache: bool = ...,
         expiration_time: int = ...,
 ) -> Union[int, _T]:
     ...
 
 
 def config_get_int(
-        section,
-        option,
-        raise_exception=True,
+        section: str,
+        option: str,
+        raise_exception: bool = True,
         default=None,
-        check_config_table=True,
-        session=None,
-        use_cache=True,
-        expiration_time=900,
+        check_config_table: bool = True,
+        session: "Optional[Session]" = None,
+        use_cache: bool = True,
+        expiration_time: int = 900,
 ):
     """
     Return the integer value for a given option in a section
 
     :param section: the named section.
     :param option: the named option.
     :param raise_exception: Boolean to raise or not NoOptionError, NoSectionError or RuntimeError.
@@ -391,22 +391,22 @@
         use_cache: bool = ...,
         expiration_time: int = ...,
 ) -> Union[float, _T]:
     ...
 
 
 def config_get_float(
-        section,
-        option,
-        raise_exception=True,
+        section: str,
+        option: str,
+        raise_exception: bool = True,
         default=None,
-        check_config_table=True,
-        session=None,
-        use_cache=True,
-        expiration_time=900,
+        check_config_table: bool = True,
+        session: "Optional[Session]" = None,
+        use_cache: bool = True,
+        expiration_time: int = 900,
 ):
     """
     Return the floating point value for a given option in a section
 
     :param section: the named section.
     :param option: the named option.
     :param raise_exception: Boolean to raise or not NoOptionError, NoSectionError or RuntimeError.
@@ -478,22 +478,22 @@
         use_cache: bool = ...,
         expiration_time: int = ...,
 ) -> Union[bool, _T]:
     ...
 
 
 def config_get_bool(
-        section,
-        option,
-        raise_exception=True,
+        section: str,
+        option: str,
+        raise_exception: bool = True,
         default=None,
-        check_config_table=True,
-        session=None,
-        use_cache=True,
-        expiration_time=900,
+        check_config_table: bool = True,
+        session: "Optional[Session]" = None,
+        use_cache: bool = True,
+        expiration_time: int = 900,
 ):
     """
     Return the boolean value for a given option in a section
 
     :param section: the named section.
     :param option: the named option.
     :param raise_exception: Boolean to raise or not NoOptionError, NoSectionError or RuntimeError.
@@ -565,22 +565,22 @@
         use_cache: bool = ...,
         expiration_time: int = ...,
 ) -> Union[list[str], _T]:
     ...
 
 
 def config_get_list(
-        section,
-        option,
-        raise_exception=True,
+        section: str,
+        option: str,
+        raise_exception: bool = True,
         default=None,
-        check_config_table=True,
-        session=None,
-        use_cache=True,
-        expiration_time=900,
+        check_config_table: bool = True,
+        session: "Optional[Session]" = None,
+        use_cache: bool = True,
+        expiration_time: int = 900,
 ):
     """
     Return a list for a given option in a section
 
     :param section: the named section.
     :param option: the named option.
     :param raise_exception: Boolean to raise or not NoOptionError, NoSectionError or RuntimeError.
@@ -687,28 +687,28 @@
     :returns: True if the option existed in the configuration, False otherwise.
 
     :raises NoSectionError: If the section does not exist.
     """
     return get_config().remove_option(section, option)
 
 
-def config_set(section: str, option: str, value: str):
+def config_set(section: str, option: str, value: str) -> None:
     """
     Set a configuration option in a given section.
 
     :param section: Name of section in the Rucio config.
     :param option: Name of option to set in the Rucio configuration.
     :param value: New value for the option.
 
     :raises NoSectionError: If the section does not exist.
     """
     return get_config().set(section, option, value)
 
 
-def get_config_dirs():
+def get_config_dirs() -> list[str]:
     """
     Returns all available configuration directories in order:
     - $RUCIO_HOME/etc/
     - $VIRTUAL_ENV/etc/
     - /opt/rucio/
     """
     configdirs = []
@@ -720,25 +720,25 @@
         configdirs.append('%s/etc/' % os.environ['VIRTUAL_ENV'])
 
     configdirs.append('/opt/rucio/etc/')
 
     return configdirs
 
 
-def get_lfn2pfn_algorithm_default():
+def get_lfn2pfn_algorithm_default() -> str:
     """Returns the default algorithm name for LFN2PFN translation for this server."""
     default_lfn2pfn = "hash"
     try:
         default_lfn2pfn = config_get('policy', 'lfn2pfn_algorithm_default')
     except (configparser.NoOptionError, configparser.NoSectionError, ConfigNotFound, RuntimeError):
         pass
     return default_lfn2pfn
 
 
-def get_rse_credentials(path_to_credentials_file: Optional[Union[str, os.PathLike]] = None):
+def get_rse_credentials(path_to_credentials_file: Optional[Union[str, os.PathLike]] = None) -> dict[str, Any]:
     """ Returns credentials for RSEs. """
 
     path = ''
     if path_to_credentials_file:  # Use specific file for this connect
         path = path_to_credentials_file
     else:  # Use file defined in th RSEMgr
         for confdir in get_config_dirs():
@@ -761,15 +761,15 @@
     """Factory function for the configuration class. Returns the ConfigParser instance."""
     global __CONFIG
     if __CONFIG is None:
         __CONFIG = Config()
     return __CONFIG.parser
 
 
-def clean_cached_config():
+def clean_cached_config() -> None:
     """Deletes the cached config singleton instance."""
     global __CONFIG
     __CONFIG = None
 
 
 class Config:
     """
```

### Comparing `rucio_clients-34.2.0/lib/rucio/common/constraints.py` & `rucio_clients-34.3.0/lib/rucio/common/constraints.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/didtype.py` & `rucio_clients-34.3.0/lib/rucio/common/didtype.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 DID type to represent a did and to simplify operations on it
 """
 
+from typing import Union
+
 from rucio.common.exception import DIDError
 
 
 class DID:
 
     """
     Class used to store a DID
@@ -49,37 +51,38 @@
             DID(scope='kw.scope', name='kw.name')
             DID(did={'scope': 'kw.did.scope', 'name': 'kw.did.name'})
             DID(did=['kw.list.scope', 'kw.list.name'])
             DID(did=('kw.tuple.scope', 'kw.tuple.name'))
             DID('arg.scope', name='kwarg.name')
             DID('arg.name', scope='kwarg.scope')
         """
-        self.scope = self.name = ''
+        self.scope: str = ''
+        self.name: str = ''
 
         num_args = len(args)
         num_kwargs = len(kwargs)
         if (num_args + num_kwargs) > 2:
             raise DIDError('Constructor takes at most 2 arguments. Given number: {}'.format(num_args + num_kwargs))
 
-        did = ''
+        did: Union["DID", str, tuple[str, str], list[str], dict[str, str]] = ''
         if num_args == 1:
             did = args[0]
 
             if num_kwargs == 1:
-                if not isinstance(did, str):
+                if isinstance(did, str):
+                    k, v = next(iter(kwargs.items()))
+                    if k == 'scope':
+                        did = (v, did)
+                    elif k == 'name':
+                        did = (did, v)
+                    else:
+                        raise DIDError('Constructor got unexpected keyword argument: {}'.format(k))
+                else:
                     raise DIDError('First argument of constructor is expected to be string type'
                                    'when keyword argument is given. Given type: {}'.format(type(did)))
-
-                k, v = next(iter(kwargs.items()))
-                if k == 'scope':
-                    did = (v, did)
-                elif k == 'name':
-                    did = (did, v)
-                else:
-                    raise DIDError('Constructor got unexpected keyword argument: {}'.format(k))
         elif num_args == 0:
             did = kwargs.get('did', kwargs)
         else:
             did = args
 
         if isinstance(did, dict):
             self.scope = did.get('scope', '')
@@ -109,78 +112,78 @@
 
         if self.name.endswith('/'):
             self.name = self.name[:-1]
 
         if not self.is_valid_format():
             raise DIDError('Object has invalid format after construction: {}'.format(str(self)))
 
-    def update_implicit_scope(self):
+    def update_implicit_scope(self) -> None:
         """
-        This method sets the scope  if it is implicitly given in self.name
+        This method sets the scope if it is implicitly given in self.name
         """
         did_parts = self.name.split(DID.IMPLICIT_SCOPE_SEPARATOR)
         num_scope_parts = DID.IMPLICIT_SCOPE_TO_LEN.get(did_parts[0], 0)
         if num_scope_parts > 0:
             self.scope = '.'.join(did_parts[0:num_scope_parts])
 
-    def is_valid_format(self):
+    def is_valid_format(self) -> bool:
         """
         Method to check if the stored DID has a valid format
         :return: bool
         """
         if self.scope.count(DID.SCOPE_SEPARATOR) or self.name.count(DID.SCOPE_SEPARATOR):
             return False
         return True
 
-    def has_scope(self):
+    def has_scope(self) -> bool:
         """
         Method to check if the scope part was set
         :return: bool
         """
         return len(self.scope) > 0
 
-    def has_name(self):
+    def has_name(self) -> bool:
         """
         Method to check if the name part was set
         :return: bool
         """
         return len(self.name) > 0
 
-    def __str__(self):
+    def __str__(self) -> str:
         """
         Creates the string representation of self
         :return: string
         """
         if self.has_scope() and self.has_name():
             return '{}{}{}'.format(self.scope, DID.SCOPE_SEPARATOR, self.name)
         elif self.has_scope():
             return self.scope
         return self.name
 
-    def __eq__(self, other):
+    def __eq__(self, other: Union[str, "DID"]) -> bool:
         """
         Equality comparison with another object
         :return: bool
         """
         if isinstance(other, str):
             return str(self) == other
         elif not isinstance(other, DID):
             try:
                 other = DID(other)
             except DIDError:
                 return False
 
         return self.scope == other.scope and self.name == other.name
 
-    def __ne__(self, other):
+    def __ne__(self, other: Union[str, "DID"]) -> bool:
         """
         Inequality comparison with another object
         :return: bool
         """
         return not self.__eq__(other)
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         """
         Uses the string representation of self to create a hash
         :return: int
         """
         return hash(str(self))
```

### Comparing `rucio_clients-34.2.0/lib/rucio/common/exception.py` & `rucio_clients-34.3.0/lib/rucio/common/exception.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/extra.py` & `rucio_clients-34.3.0/lib/rucio/common/extra.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/logging.py` & `rucio_clients-34.3.0/lib/rucio/common/logging.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/pcache.py` & `rucio_clients-34.3.0/lib/rucio/common/pcache.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     # Wait for the command to complete
     try:
 
         # Collect the output when the command completes
         stdout = p.communicate()[0][:-1]
 
-        # Commmand completed in time, cancel the alarm
+        # Command completed in time, cancel the alarm
         if (timeout > 0):
             signal.alarm(0)
 
     # Command timed out
     except Alarm:
 
         # The pid of our spawn
@@ -93,15 +93,15 @@
         return (-1, None)
 
     return (p.returncode, stdout)
 
 
 def get_process_children(pid):
 
-    # Get a list of all pids assocaited with a given pid
+    # Get a list of all pids associated with a given pid
     p = subprocess.Popen(args='ps --no-headers -o pid --ppid %d' % pid,
                          shell=True,
                          stdout=subprocess.PIPE,
                          stderr=subprocess.PIPE)
 
     # Wait and fetch the stdout
     stdout, stderr = p.communicate()
```

### Comparing `rucio_clients-34.2.0/lib/rucio/common/plugins.py` & `rucio_clients-34.3.0/lib/rucio/common/plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,75 +10,76 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import importlib
 import os
+from collections.abc import Callable
 from configparser import NoOptionError, NoSectionError
-from typing import Any, Callable, Dict, Type, TypeVar
+from typing import Any, TypeVar
 
 from rucio.common import config
 from rucio.common.exception import InvalidAlgorithmName
 
 PolicyPackageAlgorithmsT = TypeVar('PolicyPackageAlgorithmsT', bound='PolicyPackageAlgorithms')
 
 
 class PolicyPackageAlgorithms:
     """
     Base class for Rucio Policy Package Algorithms
 
     ALGORITHMS is of type Dict[str, Dict[str. Callable[..., Any]]]
     where the key is the algorithm type and the value is a dictionary of algorithm names and their callables
     """
-    _ALGORITHMS: Dict[str, Dict[str, Callable[..., Any]]] = {}
+    _ALGORITHMS: dict[str, dict[str, Callable[..., Any]]] = {}
     _loaded_policy_modules = False
 
     def __init__(self) -> None:
         if not self._loaded_policy_modules:
             self._register_all_policy_package_algorithms()
             self._loaded_policy_modules = True
 
     @classmethod
-    def _get_one_algorithm(cls: Type[PolicyPackageAlgorithmsT], algorithm_type: str, name: str) -> Callable[..., Any]:
+    def _get_one_algorithm(cls: type[PolicyPackageAlgorithmsT], algorithm_type: str, name: str) -> Callable[..., Any]:
         """
         Get the algorithm from the dictionary of algorithms
         """
         return cls._ALGORITHMS[algorithm_type][name]
 
     @classmethod
-    def _get_algorithms(cls: Type[PolicyPackageAlgorithmsT], algorithm_type: str) -> Dict[str, Callable[..., Any]]:
+    def _get_algorithms(cls: type[PolicyPackageAlgorithmsT], algorithm_type: str) -> dict[str, Callable[..., Any]]:
         """
         Get the dictionary of algorithms for a given type
         """
         return cls._ALGORITHMS[algorithm_type]
 
     @classmethod
     def _register(
-            cls: Type[PolicyPackageAlgorithmsT],
-            algorithm_type: str, algorithm_dict: Dict[str, Callable[..., Any]]) -> None:
+            cls: type[PolicyPackageAlgorithmsT],
+            algorithm_type: str, algorithm_dict: dict[str, Callable[..., Any]]) -> None:
         """
         Provided a dictionary of callable function,
         and the associated algorithm type,
         register it as one of the valid algorithms.
         """
         if algorithm_type in cls._ALGORITHMS:
             cls._ALGORITHMS[algorithm_type].update(algorithm_dict)
         else:
             cls._ALGORITHMS[algorithm_type] = algorithm_dict
 
     @classmethod
-    def _supports(cls: Type[PolicyPackageAlgorithmsT], algorithm_type: str, name: str) -> bool:
+    def _supports(cls: type[PolicyPackageAlgorithmsT], algorithm_type: str, name: str) -> bool:
         """
         Check if a algorithm is supported by the plugin
         """
         return name in cls._ALGORITHMS.get(algorithm_type, {})
 
     @classmethod
-    def _register_all_policy_package_algorithms(cls: Type[PolicyPackageAlgorithmsT]) -> None:
+    def _register_all_policy_package_algorithms(cls: type[PolicyPackageAlgorithmsT]) -> None:
         '''
         Loads all the algorithms of a given type from the policy package(s) and registers them
         :param algorithm_type: the type of algorithm to register (e.g. 'surl', 'lfn2pfn')
         :param dictionary: the dictionary to register them in
         :param vo: the name of the relevant VO (None for single VO)
         '''
         try:
@@ -113,15 +114,15 @@
                 from rucio.core.vo import list_vos
                 # policy package per VO
                 vos = list_vos()
                 for vo in vos:
                     cls._try_importing_policy(vo['vo'])
 
     @classmethod
-    def _try_importing_policy(cls: Type[PolicyPackageAlgorithmsT], vo: str = "") -> None:
+    def _try_importing_policy(cls: type[PolicyPackageAlgorithmsT], vo: str = "") -> None:
         try:
             # import from utils here to avoid circular import
             from rucio.common.utils import check_policy_package_version
 
             env_name = 'RUCIO_POLICY_PACKAGE' + ('' if not vo else '_' + vo.upper())
             package = getattr(os.environ, env_name, "")
             if not package:
```

### Comparing `rucio_clients-34.2.0/lib/rucio/common/policy.py` & `rucio_clients-34.3.0/lib/rucio/common/policy.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,49 +12,50 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
 from configparser import NoOptionError, NoSectionError
 from functools import wraps
+from typing import Any
 
 from dogpile.cache import make_region
 from dogpile.cache.api import NoValue
 
 from rucio.common.config import config_get
 from rucio.common.exception import UndefinedPolicy
 
 REGION = make_region().configure('dogpile.cache.memory',
                                  expiration_time=900)
 
 
-def get_policy():
+def get_policy() -> str:
     policy = REGION.get('policy')
     if isinstance(policy, NoValue):
         try:
             policy = config_get('policy', 'permission')
         except (NoOptionError, NoSectionError):
             policy = 'atlas'
         REGION.set('policy', policy)
     return policy
 
 
-def get_scratchdisk_lifetime():
+def get_scratchdisk_lifetime() -> int:
     scratchdisk_lifetime = REGION.get('scratchdisk_lifetime')
     if isinstance(scratchdisk_lifetime, NoValue):
         try:
             scratchdisk_lifetime = config_get('policy', 'scratchdisk_lifetime')
             scratchdisk_lifetime = int(scratchdisk_lifetime)
         except (NoOptionError, NoSectionError, ValueError):
             scratchdisk_lifetime = 14
         REGION.set('scratchdisk_lifetime', scratchdisk_lifetime)
     return scratchdisk_lifetime
 
 
-def get_lifetime_policy():
+def get_lifetime_policy() -> dict[str, list[dict[str, Any]]]:
     lifetime_dict = REGION.get('lifetime_dict')
     if isinstance(lifetime_dict, NoValue):
         lifetime_dict = {'data': [], 'mc': [], 'valid': [], 'other': []}
         lifetime_dir = '/opt/rucio/etc/policies'
         try:
             lifetime_dir = config_get('lifetime', 'directory')
         except (NoSectionError, NoOptionError):
```

### Comparing `rucio_clients-34.2.0/lib/rucio/common/schema/__init__.py` & `rucio_clients-34.3.0/lib/rucio/common/schema/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import importlib
 from configparser import NoOptionError, NoSectionError
 from os import environ
+from typing import TYPE_CHECKING, Any
 
 from rucio.common import config, exception
 from rucio.common.utils import check_policy_package_version
 
+if TYPE_CHECKING:
+    from types import ModuleType
+
 # dictionary of schema modules for each VO
-schema_modules = {}
+schema_modules: dict[str, "ModuleType"] = {}
 
 # list of unique SCOPE_NAME_REGEXP values from all schemas
-scope_name_regexps = []
+scope_name_regexps: list[str] = []
 
 try:
     multivo = config.config_get_bool('common', 'multi_vo', check_config_table=False)
 except (NoOptionError, NoSectionError):
     multivo = False
 
 # multi-VO version loads schema per-VO on demand
@@ -59,15 +63,15 @@
     except ImportError:
         raise exception.PolicyPackageNotFound('Module ' + POLICY + ' not found')
 
     schema_modules["def"] = module
     scope_name_regexps.append(module.SCOPE_NAME_REGEXP)
 
 
-def load_schema_for_vo(vo):
+def load_schema_for_vo(vo: str) -> None:
     GENERIC_FALLBACK = 'generic_multi_vo'
     if config.config_has_section('policy'):
         try:
             env_name = 'RUCIO_POLICY_PACKAGE_' + vo.upper()
             if env_name in environ:
                 POLICY = environ[env_name]
             else:
@@ -88,27 +92,27 @@
         module = importlib.import_module(POLICY)
     except ImportError:
         raise exception.PolicyPackageNotFound('Module ' + POLICY + ' not found')
 
     schema_modules[vo] = module
 
 
-def validate_schema(name, obj, vo='def'):
+def validate_schema(name: str, obj: Any, vo: str = 'def') -> None:
     if vo not in schema_modules:
         load_schema_for_vo(vo)
     schema_modules[vo].validate_schema(name, obj)
 
 
-def get_schema_value(key, vo='def'):
+def get_schema_value(key: str, vo: str = 'def') -> Any:
     if vo not in schema_modules:
         load_schema_for_vo(vo)
     return getattr(schema_modules[vo], key)
 
 
-def get_scope_name_regexps():
+def get_scope_name_regexps() -> list[str]:
     """ returns a list of all unique SCOPE_NAME_REGEXPs from all schemas """
 
     if len(scope_name_regexps) == 0:
         # load schemas for all VOs here and add unique scope_name_regexps to list
         from rucio.core.vo import list_vos
         vos = list_vos()
         for vo in vos:
@@ -116,15 +120,15 @@
                 load_schema_for_vo(vo['vo'])
             scope_name_regexp = schema_modules[vo['vo']].SCOPE_NAME_REGEXP
             if scope_name_regexp not in scope_name_regexps:
                 scope_name_regexps.append(scope_name_regexp)
     return scope_name_regexps
 
 
-def insert_scope_name(urls):
+def insert_scope_name(urls: tuple[str, ...]) -> tuple[str, str]:
     """
     given a tuple of URLs for webpy with '%s' as a placeholder for
     SCOPE_NAME_REGEXP, return a finalised tuple of URLs that will work for all
     SCOPE_NAME_REGEXPs in all schemas
     """
 
     regexps = get_scope_name_regexps()
```

### Comparing `rucio_clients-34.2.0/lib/rucio/common/schema/atlas.py` & `rucio_clients-34.3.0/lib/rucio/common/schema/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/schema/belleii.py` & `rucio_clients-34.3.0/lib/rucio/common/schema/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/schema/cms.py` & `rucio_clients-34.3.0/lib/rucio/common/schema/cms.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/schema/domatpc.py` & `rucio_clients-34.3.0/lib/rucio/common/schema/domatpc.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/schema/escape.py` & `rucio_clients-34.3.0/lib/rucio/common/schema/escape.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/schema/generic.py` & `rucio_clients-34.3.0/lib/rucio/common/schema/generic.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/schema/generic_multi_vo.py` & `rucio_clients-34.3.0/lib/rucio/common/schema/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/schema/icecube.py` & `rucio_clients-34.3.0/lib/rucio/common/schema/icecube.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/schema/lsst.py` & `rucio_clients-34.3.0/lib/rucio/common/schema/lsst.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/stomp_utils.py` & `rucio_clients-34.3.0/lib/rucio/common/stomp_utils.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/stopwatch.py` & `rucio_clients-34.3.0/lib/rucio/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/test_rucio_server.py` & `rucio_clients-34.3.0/lib/rucio/common/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/common/types.py` & `rucio_clients-34.3.0/lib/rucio/common/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Any, Callable, Literal, Optional, TypedDict, Union
+from collections.abc import Callable
+from typing import TYPE_CHECKING, Any, Literal, Optional, TypedDict, Union
+
+if TYPE_CHECKING:
+    from rucio.common.constants import SUPPORTED_PROTOCOLS_LITERAL
 
 
 class InternalType:
     '''
     Base for Internal representations of string types
     '''
     def __init__(self, value, vo='def', fromExternal=True):
@@ -174,7 +178,16 @@
     notify: Optional[Literal['Y', 'N', 'C', 'P']]
     purge_replicas: bool
 
 
 class DIDDict(TypedDict):
     name: str
     scope: InternalScope
+
+
+class HopDict(TypedDict):
+    source_rse_id: str
+    source_scheme: "SUPPORTED_PROTOCOLS_LITERAL"
+    source_scheme_priority: int
+    dest_rse_id: str
+    dest_scheme: "SUPPORTED_PROTOCOLS_LITERAL"
+    dest_scheme_priority: int
```

### Comparing `rucio_clients-34.2.0/lib/rucio/common/utils.py` & `rucio_clients-34.3.0/lib/rucio/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 import zlib
 from collections import OrderedDict
 from collections.abc import Callable, Sequence
 from enum import Enum
 from functools import partial, wraps
 from io import StringIO
 from itertools import zip_longest
-from typing import TYPE_CHECKING, Optional, Type, TypeVar
+from typing import TYPE_CHECKING, Optional, TypeVar
 from urllib.parse import parse_qsl, quote, urlencode, urlparse, urlunparse
 from uuid import uuid4 as uuid
 from xml.etree import ElementTree
 
 import requests
 
 from rucio.common.config import config_get, config_has_section
@@ -219,27 +219,27 @@
 CHECKSUM_ALGO_DICT = {}
 PREFERRED_CHECKSUM = GLOBALLY_SUPPORTED_CHECKSUMS[0]
 CHECKSUM_KEY = 'supported_checksums'
 
 
 def is_checksum_valid(checksum_name):
     """
-    A simple function to check wether a checksum algorithm is supported.
+    A simple function to check whether a checksum algorithm is supported.
     Relies on GLOBALLY_SUPPORTED_CHECKSUMS to allow for expandability.
 
     :param checksum_name: The name of the checksum to be verified.
     :returns: True if checksum_name is in GLOBALLY_SUPPORTED_CHECKSUMS list, False otherwise.
     """
 
     return checksum_name in GLOBALLY_SUPPORTED_CHECKSUMS
 
 
 def set_preferred_checksum(checksum_name):
     """
-    A simple function to check wether a checksum algorithm is supported.
+    A simple function to check whether a checksum algorithm is supported.
     Relies on GLOBALLY_SUPPORTED_CHECKSUMS to allow for expandability.
 
     :param checksum_name: The name of the checksum to be verified.
     :returns: True if checksum_name is in GLOBALLY_SUPPORTED_CHECKSUMS list, False otherwise.
     """
     if is_checksum_valid(checksum_name):
         global PREFERRED_CHECKSUM
@@ -669,15 +669,15 @@
 
 def rse_supported_protocol_operations():
     """ Returns a list with operations supported by all RSE protocols."""
     return ['read', 'write', 'delete', 'third_party_copy_read', 'third_party_copy_write']
 
 
 def rse_supported_protocol_domains():
-    """ Returns a list with all supoorted RSE protocol domains."""
+    """ Returns a list with all supported RSE protocol domains."""
     return ['lan', 'wan']
 
 
 def grouper(iterable, n, fillvalue=None):
     """ Collect data into fixed-length chunks or blocks """
     # grouper('ABCDEFG', 3, 'x') --> ABC DEF Gxx
     args = [iter(iterable)] * n
@@ -740,38 +740,38 @@
     def construct_surl(self, dsn: str, scope: str, filename: str, naming_convention: str) -> str:
         """
         Calls the correct algorithm to generate a SURL
         """
         return self.get_algorithm(naming_convention)(dsn, scope, filename)
 
     @classmethod
-    def supports(cls: Type[SurlAlgorithmsT], naming_convention: str) -> bool:
+    def supports(cls: type[SurlAlgorithmsT], naming_convention: str) -> bool:
         """
         Checks whether a SURL algorithm is supported
         """
         return super()._supports(cls._algorithm_type, naming_convention)
 
     @classmethod
-    def _module_init_(cls: Type[SurlAlgorithmsT]) -> None:
+    def _module_init_(cls: type[SurlAlgorithmsT]) -> None:
         """
         Registers the included SURL algorithms
         """
         cls.register('T0', cls.construct_surl_T0)
         cls.register('DQ2', cls.construct_surl_DQ2)
         cls.register('BelleII', cls.construct_surl_BelleII)
 
     @classmethod
-    def get_algorithm(cls: Type[SurlAlgorithmsT], naming_convention: str) -> Callable[[str, str, str], str]:
+    def get_algorithm(cls: type[SurlAlgorithmsT], naming_convention: str) -> Callable[[str, str, str], str]:
         """
         Looks up a SURL algorithm by name
         """
         return super()._get_one_algorithm(cls._algorithm_type, naming_convention)
 
     @classmethod
-    def register(cls: Type[SurlAlgorithmsT], name: str, fn_construct_surl: Callable[[str, str, str], str]) -> None:
+    def register(cls: type[SurlAlgorithmsT], name: str, fn_construct_surl: Callable[[str, str, str], str]) -> None:
         """
         Register a new SURL algorithm
         """
         algorithm_dict = {name: fn_construct_surl}
         super()._register(cls._algorithm_type, algorithm_dict)
 
     @staticmethod
@@ -940,38 +940,38 @@
     def extract_scope(self, did: str, scopes: Optional[Sequence[str]], extract_scope_convention: str) -> Sequence[str]:
         """
         Calls the correct algorithm for scope extraction
         """
         return self.get_algorithm(extract_scope_convention)(did, scopes)
 
     @classmethod
-    def supports(cls: Type[ScopeExtractionAlgorithmsT], extract_scope_convention: str) -> bool:
+    def supports(cls: type[ScopeExtractionAlgorithmsT], extract_scope_convention: str) -> bool:
         """
         Checks whether the specified scope extraction algorithm is supported
         """
         return super()._supports(cls._algorithm_type, extract_scope_convention)
 
     @classmethod
-    def _module_init_(cls: Type[ScopeExtractionAlgorithmsT]) -> None:
+    def _module_init_(cls: type[ScopeExtractionAlgorithmsT]) -> None:
         """
         Registers the included scope extraction algorithms
         """
         cls.register('atlas', cls.extract_scope_atlas)
         cls.register('belleii', cls.extract_scope_belleii)
         cls.register('dirac', cls.extract_scope_dirac)
 
     @classmethod
-    def get_algorithm(cls: Type[ScopeExtractionAlgorithmsT], extract_scope_convention: str) -> Callable[[str, Optional[Sequence[str]]], Sequence[str]]:
+    def get_algorithm(cls: type[ScopeExtractionAlgorithmsT], extract_scope_convention: str) -> Callable[[str, Optional[Sequence[str]]], Sequence[str]]:
         """
         Looks up a scope extraction algorithm by name
         """
         return super()._get_one_algorithm(cls._algorithm_type, extract_scope_convention)
 
     @classmethod
-    def register(cls: Type[ScopeExtractionAlgorithmsT], name: str, fn_extract_scope: Callable[[str, Optional[Sequence[str]]], Sequence[str]]) -> None:
+    def register(cls: type[ScopeExtractionAlgorithmsT], name: str, fn_extract_scope: Callable[[str, Optional[Sequence[str]]], Sequence[str]]) -> None:
         """
         Registers a new scope extraction algorithm
         """
         algorithm_dict = {name: fn_extract_scope}
         super()._register(cls._algorithm_type, algorithm_dict)
 
     @staticmethod
@@ -1267,30 +1267,29 @@
     return {'ip': ip,
             'fqdn': socket.getfqdn(),
             'site': site,
             'latitude': latitude,
             'longitude': longitude}
 
 
-def ssh_sign(private_key, message):
+def ssh_sign(private_key: str, message: str) -> str:
     """
     Sign a string message using the private key.
 
     :param private_key: The SSH RSA private key as a string.
     :param message: The message to sign as a string.
     :return: Base64 encoded signature as a string.
     """
-    if isinstance(message, str):
-        message = message.encode()
+    encoded_message = message.encode()
     if not EXTRA_MODULES['paramiko']:
         raise MissingModuleException('The paramiko module is not installed or faulty.')
     sio_private_key = StringIO(private_key)
     priv_k = RSAKey.from_private_key(sio_private_key)
     sio_private_key.close()
-    signature_stream = priv_k.sign_ssh_data(message)
+    signature_stream = priv_k.sign_ssh_data(encoded_message)
     signature_stream.rewind()
     base64_encoded = base64.b64encode(signature_stream.get_remainder())
     base64_encoded = base64_encoded.decode()
     return base64_encoded
 
 
 def make_valid_did(lfn_dict):
@@ -1646,15 +1645,15 @@
     return files
 
 
 def get_thread_with_periodic_running_function(interval, action, graceful_stop):
     """
     Get a thread where a function runs periodically.
 
-    :param interval: Interval in seconds when the action fucntion should run.
+    :param interval: Interval in seconds when the action function should run.
     :param action: Function, that should run periodically.
     :param graceful_stop: Threading event used to check for graceful stop.
     """
     def start():
         while not graceful_stop.is_set():
             starttime = time.time()
             action()
@@ -1858,15 +1857,15 @@
 
 class retry:
     """Retry callable object with configuragle number of attempts"""
 
     def __init__(self, func, *args, **kwargs):
         '''
         :param func: a method that should be executed with retries
-        :param args: parametres of the func
+        :param args: parameters of the func
         :param kwargs: key word arguments of the func
         '''
         self.func, self.args, self.kwargs = func, args, kwargs
 
     def __call__(self, mtries=3, logger=logging.log):
         '''
         :param mtries: maximum number of attempts to execute the function
@@ -2082,15 +2081,15 @@
     if current_version not in supported_version:
         raise PolicyPackageVersionError(package)
 
 
 class Availability:
     """
     This util class acts as a translator between the availability stored as
-    integer and as boolen values.
+    integer and as boolean values.
 
     `None` represents a missing value. This lets a user update a specific value
     without altering the other ones. If it needs to be evaluated, it will
     correspond to `True`.
     """
 
     read = None
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/__init__.py` & `rucio_clients-34.3.0/lib/rucio/rse/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/__init__.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/bittorrent.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/bittorrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             if self.attributes['port'] != port:
                 raise exception.RSEFileNameNotSupported('Invalid port: provided \'%s\', expected \'%s\'' % (port, self.attributes['port']))
 
             if not path.startswith(self.attributes['prefix']):
                 raise exception.RSEFileNameNotSupported('Invalid prefix: provided \'%s\', expected \'%s\'' % ('/'.join(path.split('/')[0:len(self.attributes['prefix'].split('/')) - 1]),
                                                                                                               self.attributes['prefix']))  # len(...)-1 due to the leading '/
 
-            # Spliting parsed.path into prefix, path, filename
+            # Splitting parsed.path into prefix, path, filename
             prefix = self.attributes['prefix']
             path = path.partition(self.attributes['prefix'])[2]
             path = '/'.join(path.split('/')[:-1])
             if not path.startswith('/'):
                 path = '/' + path
             if path != '/' and not path.endswith('/'):
                 path = path + '/'
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/cache.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
             :returns: RSE specific URI of the physical file
         """
         return '%s/%s' % (scope, name)
 
     def path2pfn(self, path):
         """
-            Retruns a fully qualified PFN for the file referred by path.
+            Returns a fully qualified PFN for the file referred by path.
 
             :param path: The path to the file.
 
             :returns: Fully qualified PFN.
 
         """
         return ''.join([self.rse['scheme'], '://%s' % self.rse['hostname'], path])
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/dummy.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         super(Default, self).__init__(protocol_attr, rse_settings, logger=logger)
         self.attributes.pop('determinism_type', None)
         self.files = []
 
     def path2pfn(self, path):
         """
-            Retruns a fully qualified PFN for the file referred by path.
+            Returns a fully qualified PFN for the file referred by path.
 
             :param path: The path to the file.
 
             :returns: Fully qualified PFN.
 
         """
         return ''.join([self.rse['scheme'], '://%s' % self.rse['hostname'], path])
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/gfal.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/gfal.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                 raise exception.RSEFileNameNotSupported('Invalid port: provided \'%s\', expected \'%s\'' % (port, self.attributes['port']))
             elif port == '':
                 port = self.attributes['port']
 
             if not path.startswith(self.attributes['prefix']):
                 raise exception.RSEFileNameNotSupported('Invalid prefix: provided \'%s\', expected \'%s\'' % ('/'.join(path.split('/')[0:len(self.attributes['prefix'].split('/')) - 1]),
                                                                                                               self.attributes['prefix']))  # len(...)-1 due to the leading '/
-            # Spliting path into prefix, path, filename
+            # Splitting path into prefix, path, filename
             prefix = self.attributes['prefix']
             path = path.partition(self.attributes['prefix'])[2]
             name = path.split('/')[-1]
             path = '/'.join(path.split('/')[:-1])
             if not path.startswith('/'):
                 path = '/' + path
             if path != '/' and not path.endswith('/'):
@@ -226,15 +226,15 @@
         Provides access to files stored inside connected the RSE.
 
         :param path: Physical file name of requested file
         :param dest: Name and path of the files when stored at the client
         :param transfer_timeout: Transfer timeout (in seconds)
 
         :raises DestinationNotAccessible: if the destination storage was not accessible.
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
         :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'downloading file from {} to {}'.format(path, dest))
 
         dest = os.path.abspath(dest)
         if ':' not in dest:
             dest = "file://" + dest
@@ -256,15 +256,15 @@
 
         :param source: path to the source file on the client file system
         :param target: path to the destination file on the storage
         :param source_dir: Path where the to be transferred files are stored in the local file system
         :param transfer_timeout: Transfer timeout (in seconds)
 
         :raises DestinationNotAccessible: if the destination storage was not accessible.
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
         :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'uploading file from {} to {}'.format(source, target))
 
         source_url = '%s/%s' % (source_dir, source) if source_dir else source
         source_url = os.path.abspath(source_url)
         if not os.path.exists(source_url):
@@ -289,15 +289,15 @@
 
     def delete(self, path):
         """
         Deletes a file from the connected RSE.
 
         :param path: path to the to be deleted file
 
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
         :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'deleting file {}'.format(path))
 
         pfns = [path] if isinstance(path, STRING_TYPES) else path
 
         try:
@@ -313,15 +313,15 @@
         """
         Allows to rename a file stored inside the connected RSE.
 
         :param path: path to the current file on the storage
         :param new_path: path to the new file on the storage
 
         :raises DestinationNotAccessible: if the destination storage was not accessible.
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
         :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'renaming file from {} to {}'.format(path, new_path))
 
         try:
             status = self.__gfal2_rename(path, new_path)
             if status:
@@ -365,15 +365,15 @@
 
     def stat(self, path):
         """
             Returns the stats of a file.
 
             :param path: path to file
 
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
 
             :returns: a dict with two keys, filesize and an element of GLOBALLY_SUPPORTED_CHECKSUMS.
         """
         self.logger(logging.DEBUG, 'getting stats of file {}'.format(path))
 
         ret = {}
         ctx = self.__ctx
@@ -549,15 +549,15 @@
 
     def get_space_usage(self):
         """
         Get RSE space usage information.
 
         :returns: a list with dict containing 'totalsize' and 'unusedsize'
 
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
         """
         endpoint_basepath = self.path2pfn(self.attributes['prefix'])
         self.logger(logging.DEBUG, 'getting space usage from {}'.format(endpoint_basepath))
 
         space_token = None
         if self.attributes['extended_attributes'] is not None and 'space_token' in list(self.attributes['extended_attributes'].keys()):
             space_token = self.attributes['extended_attributes']['space_token']
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/globus.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/globus.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from urllib.parse import urlparse
 
 from rucio.common import exception
+from rucio.common.constants import RseAttr
 from rucio.common.extra import import_extras
 from rucio.core.rse import get_rse_attribute
 from rucio.rse.protocols.protocol import RSEProtocol
 from rucio.transfertool.globus_library import get_transfer_client, send_bulk_delete_task, send_delete_task
 
 EXTRA_MODULES = import_extras(['globus_sdk'])
 
@@ -32,20 +33,20 @@
 
     def __init__(self, protocol_attr, rse_settings, logger=logging.log):
         """ Initializes the object with information about the referred RSE.
 
             :param props: Properties of the requested protocol
         """
         super(GlobusRSEProtocol, self).__init__(protocol_attr, rse_settings, logger=logger)
-        self.globus_endpoint_id = get_rse_attribute(self.rse.get('id'), 'globus_endpoint_id')
+        self.globus_endpoint_id = get_rse_attribute(self.rse.get('id'), RseAttr.GLOBUS_ENDPOINT_ID)
         self.logger = logger
 
     def lfns2pfns(self, lfns):
         """
-            Retruns a fully qualified PFN for the file referred by path.
+            Returns a fully qualified PFN for the file referred by path.
 
             :param path: The path to the file.
 
             :returns: Fully qualified PFN.
         """
         pfns = {}
         prefix = self.attributes['prefix']
@@ -75,15 +76,15 @@
 
             :returns: RSE specific URI of the physical file
         """
         return self.translator.path(scope, name)
 
     def parse_pfns(self, pfns):
         """
-            Splits the given PFN into the parts known by the protocol. It is also checked if the provided protocol supportes the given PFNs.
+            Splits the given PFN into the parts known by the protocol. It is also checked if the provided protocol supports the given PFNs.
 
             :param pfns: a list of a fully qualified PFNs
 
             :returns: dic with PFN as key and a dict with path and name as value
 
             :raises RSEFileNameNotSupported: if the provided PFN doesn't match with the protocol settings
         """
@@ -112,15 +113,15 @@
             if self.attributes['port'] != port:
                 raise exception.RSEFileNameNotSupported('Invalid port: provided \'%s\', expected \'%s\'' % (port, self.attributes['port']))
 
             if not path.startswith(self.attributes['prefix']):
                 raise exception.RSEFileNameNotSupported('Invalid prefix: provided \'%s\', expected \'%s\'' % ('/'.join(path.split('/')[0:len(self.attributes['prefix'].split('/')) - 1]),
                                                                                                               self.attributes['prefix']))  # len(...)-1 due to the leading '/
 
-            # Spliting parsed.path into prefix, path, filename
+            # Splitting parsed.path into prefix, path, filename
             prefix = self.attributes['prefix']
             path = path.partition(self.attributes['prefix'])[2]
             name = path.split('/')[-1]
             path = '/'.join(path.split('/')[:-1])
             if not path.startswith('/'):
                 path = '/' + path
             if path != '/' and not path.endswith('/'):
@@ -185,15 +186,15 @@
 
     def delete(self, path):
         """
             Deletes a file from the connected RSE.
 
             :param path: path to the to be deleted file
 
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         if self.globus_endpoint_id:
             try:
                 delete_response = send_delete_task(endpoint_id=self.globus_endpoint_id, path=path, logger=self.logger)
             except TransferAPIError as err:
                 self.logger(logging.WARNING, str(err))
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/gsiftp.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/gsiftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,20 +48,20 @@
 
     def get_space_usage(self):
         """
         Get RSE space usage information.
 
         :returns: a list with dict containing 'totalsize' and 'unusedsize'
 
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
         """
         rse_name = self.rse['rse']
         dest = '/tmp/rucio-gsiftp-site-size_' + rse_name
         space_usage_url = ''
-        # url of space usage json, woud be nicer to have it in rse_settings
+        # url of space usage json, would be nicer to have it in rse_settings
         agis = requests.get('http://atlas-agis-api.cern.ch/request/ddmendpoint/query/list/?json').json()
         agis_token = ''
         for res in agis:
             if rse_name == res['name']:
                 agis_token = res['token']
                 space_usage_url = res['space_usage_url']
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/http_cache.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/http_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
             :returns: RSE specific URI of the physical file
         """
         return '%s/%s' % (scope, name)
 
     def path2pfn(self, path):
         """
-            Retruns a fully qualified PFN for the file referred by path.
+            Returns a fully qualified PFN for the file referred by path.
 
             :param path: The path to the file.
 
             :returns: Fully qualified PFN.
 
         """
         return ''.join([self.attributes['scheme'], '://%s' % self.attributes['hostname'], path])
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/mock.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         """
         super(Default, self).__init__(protocol_attr, rse_settings, logger=logger)
         self.attributes.pop('determinism_type', None)
         self.files = []
 
     def path2pfn(self, path):
         """
-            Retruns a fully qualified PFN for the file referred by path.
+            Returns a fully qualified PFN for the file referred by path.
 
             :param path: The path to the file.
 
             :returns: Fully qualified PFN.
 
         """
         return ''.join([self.rse['scheme'], '://%s' % self.rse['hostname'], path])
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/ngarc.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/ngarc.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         try:
             self.cfg.ProxyPath(os.environ['X509_USER_PROXY'])
         except:
             pass
 
     def path2pfn(self, path):
         """
-            Retruns a fully qualified PFN for the file referred by path.
+            Returns a fully qualified PFN for the file referred by path.
 
             :param path: The path to the file.
 
             :returns: Fully qualified PFN.
 
         """
         return ''.join([self.rse['scheme'], '://%s' % self.rse['hostname'], path])
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/posix.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/posix.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             raise exception.ServiceUnavailable(e)
         return status
 
     def connect(self):
         """
             Establishes the actual connection to the referred RSE.
 
-            :param credentials: needed to establish a connection with the stroage.
+            :param credentials: needed to establish a connection with the storage.
 
             :raises RSEAccessDenied: if no connection could be established.
         """
         pass
 
     def close(self):
         """ Closes the connection to RSE."""
@@ -61,21 +61,21 @@
         """ Provides access to files stored inside connected the RSE.
 
             :param pfn: Physical file name of requested file
             :param dest: Name and path of the files when stored at the client
             :param transfer_timeout Transfer timeout (in seconds) - dummy
 
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
          """
         try:
             shutil.copy(self.pfn2path(pfn), dest)
         except OSError as e:
-            try:  # To check if the error happend local or remote
+            try:  # To check if the error happened local or remote
                 with open(dest, 'wb'):
                     pass
                 call(['rm', '-rf', dest])
             except OSError as e:
                 if e.errno == 2:
                     raise exception.DestinationNotAccessible(e)
                 else:
@@ -91,15 +91,15 @@
 
             :param source: path to the source file on the client file system
             :param target: path to the destination file on the storage
             :param source_dir: Path where the to be transferred files are stored in the local file system
             :param transfer_timeout Transfer timeout (in seconds) - dummy
 
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         target = self.pfn2path(target)
 
         if source_dir:
             sf = source_dir + '/' + source
         else:
@@ -122,15 +122,15 @@
                 raise exception.DestinationNotAccessible(e)
 
     def delete(self, pfn):
         """ Deletes a file from the connected RSE.
 
             :param pfn: pfn to the to be deleted file
 
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         try:
             os.remove(self.pfn2path(pfn))
         except OSError as e:
             if e.errno == 2:
                 raise exception.SourceNotFound(e)
@@ -138,15 +138,15 @@
     def rename(self, pfn, new_pfn):
         """ Allows to rename a file stored inside the connected RSE.
 
             :param path: path to the current file on the storage
             :param new_path: path to the new file on the storage
 
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         path = self.pfn2path(pfn)
         new_path = self.pfn2path(new_pfn)
         try:
             if not os.path.exists(os.path.dirname(new_path)):
                 os.makedirs(os.path.dirname(new_path))
@@ -219,15 +219,15 @@
         """ Provides access to files stored inside connected the RSE.
             A download/get will create a symlink on the local file system pointing to the
             underlying file. Other operations act directly on the remote file.
             :param pfn: Physical file name of requested file
             :param dest: Name and path of the files when stored at the client
             :param transfer_timeout Transfer timeout (in seconds) - dummy
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
          """
         path = self.pfn2path(pfn)
         os.symlink(path, dest)
         self.logger(logging.DEBUG,
                     'Symlink {} created for {} from {}'
                     .format(dest, path, pfn))
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/protocol.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import hashlib
 import logging
 from configparser import NoOptionError, NoSectionError
 from typing import TypeVar
 from urllib.parse import urlparse
 
 from rucio.common import config, exception
+from rucio.common.constants import RseAttr
 from rucio.common.plugins import PolicyPackageAlgorithms
 from rucio.rse import rsemanager
 
 if getattr(rsemanager, 'CLIENT_MODE', None):
     from rucio.client.rseclient import RSEClient
 
 if getattr(rsemanager, 'SERVER_MODE', None):
@@ -247,15 +248,15 @@
         """ Transforms the logical file name into a PFN's path.
 
             :param lfn: filename
             :param scope: scope
 
             :returns: RSE specific URI of the physical file
         """
-        algorithm = self.rse_attributes.get('lfn2pfn_algorithm', 'default')
+        algorithm = self.rse_attributes.get(RseAttr.LFN2PFN_ALGORITHM, 'default')
         if algorithm == 'default':
             algorithm = RSEDeterministicTranslation._DEFAULT_LFN2PFN
         algorithm_callable = super()._get_one_algorithm(RSEDeterministicTranslation._algorithm_type, algorithm)
         return algorithm_callable(scope, name, self.rse, self.rse_attributes, self.protocol_attributes)
 
 
 RSEDeterministicTranslation._module_init_()  # pylint: disable=protected-access
@@ -289,15 +290,15 @@
             if getattr(rsemanager, 'CLIENT_MODE', None):
                 setattr(self, 'lfns2pfns', self.__lfns2pfns_client)
             if getattr(rsemanager, 'SERVER_MODE', None):
                 setattr(self, '_get_path', self._get_path_nondeterministic_server)
 
     def lfns2pfns(self, lfns):
         """
-            Retruns a fully qualified PFN for the file referred by path.
+            Returns a fully qualified PFN for the file referred by path.
 
             :param path: The path to the file.
 
             :returns: Fully qualified PFN.
         """
         pfns = {}
         prefix = self.attributes['prefix']
@@ -330,15 +331,15 @@
                                                              self._get_path(scope=scope, name=name)
                                                              ])
                 except exception.ReplicaNotFound as e:
                     self.logger(logging.WARNING, str(e))
         return pfns
 
     def __lfns2pfns_client(self, lfns):
-        """ Provides the path of a replica for non-deterministic sites. Will be assigned to get path by the __init__ method if neccessary.
+        """ Provides the path of a replica for non-deterministic sites. Will be assigned to get path by the __init__ method if necessary.
 
             :param scope: list of DIDs
 
             :returns: dict with scope:name as keys and PFN as value (in case of errors the Rucio exception si assigned to the key)
         """
         client = RSEClient()  # pylint: disable=E0601
 
@@ -355,15 +356,15 @@
             :param name: filename
 
             :returns: RSE specific URI of the physical file
         """
         return self.translator.path(scope, name)
 
     def _get_path_nondeterministic_server(self, scope, name):  # pylint: disable=invalid-name
-        """ Provides the path of a replica for non-deterministic sites. Will be assigned to get path by the __init__ method if neccessary. """
+        """ Provides the path of a replica for non-deterministic sites. Will be assigned to get path by the __init__ method if necessary. """
         vo = get_rse_vo(self.rse['id'])  # pylint: disable=E0601
         scope = InternalScope(scope, vo=vo)  # pylint: disable=E0601
         rep = replica.get_replica(scope=scope, name=name, rse_id=self.rse['id'])  # pylint: disable=E0601
         if 'path' in rep and rep['path'] is not None:
             path = rep['path']
         elif 'state' in rep and (rep['state'] is None or rep['state'] == 'UNAVAILABLE'):
             raise exception.ReplicaUnAvailable('Missing path information and state is UNAVAILABLE for replica %s:%s on non-deterministic storage named %s' % (scope, name, self.rse['rse']))
@@ -373,15 +374,15 @@
             path = path[1:]
         if path.endswith('/'):
             path = path[:-1]
         return path
 
     def parse_pfns(self, pfns):
         """
-            Splits the given PFN into the parts known by the protocol. It is also checked if the provided protocol supportes the given PFNs.
+            Splits the given PFN into the parts known by the protocol. It is also checked if the provided protocol supports the given PFNs.
 
             :param pfns: a list of a fully qualified PFNs
 
             :returns: dic with PFN as key and a dict with path and name as value
 
             :raises RSEFileNameNotSupported: if the provided PFN doesn't match with the protocol settings
         """
@@ -413,15 +414,15 @@
             if self.attributes['port'] != port:
                 raise exception.RSEFileNameNotSupported('Invalid port: provided \'%s\', expected \'%s\'' % (port, self.attributes['port']))
 
             if not path.startswith(prefix):
                 raise exception.RSEFileNameNotSupported('Invalid prefix: provided \'%s\', expected \'%s\'' % ('/'.join(path.split('/')[0:len(prefix.split('/')) - 1]),
                                                                                                               prefix))  # len(...)-1 due to the leading '/
 
-            # Spliting parsed.path into prefix, path, filename
+            # Splitting parsed.path into prefix, path, filename
             path = path.partition(prefix)[2]
             name = path.split('/')[-1]
             path = '/'.join(path.split('/')[:-1])
             if not path.startswith('/'):
                 path = '/' + path
             if path != '/' and not path.endswith('/'):
                 path = path + '/'
@@ -458,72 +459,72 @@
             Provides access to files stored inside connected the RSE.
 
             :param path: Physical file name of requested file
             :param dest: Name and path of the files when stored at the client
             :param transfer_timeout: Transfer timeout (in seconds)
 
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
          """
         raise NotImplementedError
 
     def put(self, source, target, source_dir, transfer_timeout=None):
         """
             Allows to store files inside the referred RSE.
 
             :param source: path to the source file on the client file system
             :param target: path to the destination file on the storage
             :param source_dir: Path where the to be transferred files are stored in the local file system
             :param transfer_timeout: Transfer timeout (in seconds)
 
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         raise NotImplementedError
 
     def delete(self, path):
         """
             Deletes a file from the connected RSE.
 
             :param path: path to the to be deleted file
 
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         raise NotImplementedError
 
     def rename(self, path, new_path):
         """ Allows to rename a file stored inside the connected RSE.
 
             :param path: path to the current file on the storage
             :param new_path: path to the new file on the storage
 
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         raise NotImplementedError
 
     def get_space_usage(self):
         """
             Get RSE space usage information.
 
             :returns: a list with dict containing 'totalsize' and 'unusedsize'
 
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
         """
         raise NotImplementedError
 
     def stat(self, path):
         """
             Returns the stats of a file.
 
             :param path: path to file
 
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
 
             :returns: a dict with two keys, filesize and adler32 of the file provided in path.
         """
         raise NotImplementedError
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/rclone.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/rclone.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
     def stat(self, path):
         """
         Returns the stats of a file.
 
         :param path: path to file
 
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
 
         :returns: a dict with two keys, filesize and an element of GLOBALLY_SUPPORTED_CHECKSUMS.
         """
         self.logger(logging.DEBUG, 'rclone.stat: path: {}'.format(path))
         ret = {}
         chsum = None
         if path.startswith('rclone://'):
@@ -294,15 +294,15 @@
 
             :param source: path to the source file on the client file system
             :param target: path to the destination file on the storage
             :param source_dir: Path where the to be transferred files are stored in the local file system
             :param transfer_timeout: Transfer timeout (in seconds) - dummy
 
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'rclone.put: filename: {} target: {}'.format(filename, target))
         source_dir = source_dir or '.'
         source_url = '%s/%s' % (source_dir, filename)
         self.logger(logging.DEBUG, 'rclone.put: source url: {}'.format(source_url))
 
@@ -320,15 +320,15 @@
 
     def delete(self, pfn):
         """
             Deletes a file from the connected RSE.
 
             :param pfn: Physical file name
 
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'rclone.delete: pfn: {}'.format(pfn))
         if not self.exists(pfn):
             raise exception.SourceNotFound()
         try:
             path = self.pfn2path(pfn)
@@ -342,15 +342,15 @@
 
     def rename(self, pfn, new_pfn):
         """ Allows to rename a file stored inside the connected RSE.
 
             :param pfn:      Current physical file name
             :param new_pfn  New physical file name
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'rclone.rename: pfn: {}'.format(pfn))
         if not self.exists(pfn):
             raise exception.SourceNotFound()
         try:
             path = self.pfn2path(pfn)
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/rfio.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/rfio.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 class Default(protocol.RSEProtocol):
     """ Implementing access to RSEs using the RFIO protocol. """
 
     def connect(self, credentials):
         """
             Establishes the actual connection to the referred RSE.
 
-            :param credentials: needed to establish a connection with the stroage.
+            :param credentials: needed to establish a connection with the storage.
 
             :raises RSEAccessDenied: if no connection could be established.
         """
         extended_attributes = self.rse['protocol']['extended_attributes']
         if 'STAGE_SVCCLASS' in extended_attributes:
             os.environ['STAGE_SVCCLASS'] = extended_attributes['STAGE_SVCCLASS']
 
     def path2pfn(self, path):
         """
-            Retruns a fully qualified PFN for the file referred by path.
+            Returns a fully qualified PFN for the file referred by path.
 
             :param path: The path to the file.
 
             :returns: Fully qualified PFN.
 
         """
         return ''.join([self.rse['scheme'], '://', path])
@@ -76,15 +76,15 @@
 
             :param source: path to the source file on the client file system
             :param target: path to the destination file on the storage
             :param source_dir: Path where the to be transferred files are stored in the local file system
             :param transfer_timeout: Transfer timeout (in seconds) - dummy
 
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         if not self.exists(dirname(target)):
             self.mkdir(dirname(target))
 
         cmd = f'rfcp {source} {target}'
         status, out, err = execute(cmd)
@@ -123,14 +123,14 @@
 
         if self.rse['hostname'] != ret['hostname']:
             raise exception.RSEFileNameNotSupported('Invalid hostname: provided \'%s\', expected \'%s\'' % (ret['hostname'], self.rse['hostname']))
 
         if not ret['path'].startswith(self.rse['prefix']):
             raise exception.RSEFileNameNotSupported('Invalid prefix: provided \'%s\', expected \'%s\'' % ('/'.join(ret['path'].split('/')[0:len(self.rse['prefix'].split('/')) - 1]),
                                                                                                           self.rse['prefix']))  # len(...)-1 due to the leading '/
-        # Spliting parsed.path into prefix, path, filename
+        # Splitting parsed.path into prefix, path, filename
         ret['prefix'] = self.rse['prefix']
         ret['path'] = ret['path'].partition(self.rse['prefix'])[2]
         ret['name'] = ret['path'].split('/')[-1]
         ret['path'] = ret['path'].partition(ret['name'])[0]
 
         return ret
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/srm.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/srm.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             elif port == '':
                 port = self.attributes['port']
 
             if not path.startswith(self.attributes['prefix']):
                 raise exception.RSEFileNameNotSupported('Invalid prefix: provided \'%s\', expected \'%s\'' % ('/'.join(path.split('/')[0:len(self.attributes['prefix'].split('/')) - 1]),
                                                                                                               self.attributes['prefix']))  # len(...)-1 due to the leading '/
 
-            # Spliting path into prefix, path, filename
+            # Splitting path into prefix, path, filename
             prefix = self.attributes['prefix']
             path = path.partition(self.attributes['prefix'])[2]
             name = path.split('/')[-1]
             path = '/' + '/'.join(path.split('/')[:-1]) if not self.rse['staging_area'] else None
 
             if path != '/' and path[:-1] != '/':
                 path += '/'
@@ -163,15 +163,15 @@
                 return ''.join([self.attributes['scheme'], '://', hostname, web_service_path, path])
         else:
             return path
 
     def connect(self):
         """
         Establishes the actual connection to the referred RSE.
-        As a quick and dirty impelementation we just use this method to check if the lcg tools are available.
+        As a quick and dirty implementation we just use this method to check if the lcg tools are available.
         If we decide to use gfal, init should be done here.
 
         :raises RSEAccessDenied: Cannot connect.
         """
 
         status, lcglscommand = getstatusoutput('which lcg-ls')
         if status:
@@ -189,15 +189,15 @@
         Provides access to files stored inside connected the RSE.
 
         :param path: Physical file name of requested file
         :param dest: Name and path of the files when stored at the client
         :param transfer_timeout: Transfer timeout (in seconds)
 
         :raises DestinationNotAccessible: if the destination storage was not accessible.
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
         :raises SourceNotFound: if the source file was not found on the referred storage.
         """
 
         timeout_option = ''
         if transfer_timeout:
             timeout_option = '--sendreceive-timeout %s' % transfer_timeout
 
@@ -219,15 +219,15 @@
 
         :param source: path to the source file on the client file system
         :param target: path to the destination file on the storage
         :param source_dir: Path where the to be transferred files are stored in the local file system
         :param transfer_timeout: Transfer timeout (in seconds)
 
         :raises DestinationNotAccessible: if the destination storage was not accessible.
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
         :raises SourceNotFound: if the source file was not found on the referred storage.
         """
 
         source_url = '%s/%s' % (source_dir, source) if source_dir else source
 
         if not os.path.exists(source_url):
             raise exception.SourceNotFound()
@@ -249,15 +249,15 @@
             raise exception.ServiceUnavailable(error)
 
     def delete(self, path):
         """
         Deletes a file from the connected RSE.
 
         :param path: path to the to be deleted file
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
         :raises SourceNotFound: if the source file was not found on the referred storage.
         """
 
         pfns = [path] if isinstance(path, str) else path
 
         try:
             pfn_chunks = [pfns[i:i + 20] for i in range(0, len(pfns), 20)]
@@ -278,15 +278,15 @@
     def rename(self, path, new_path):
         """
         Allows to rename a file stored inside the connected RSE.
 
         :param path: path to the current file on the storage
         :param new_path: path to the new file on the storage
         :raises DestinationNotAccessible: if the destination storage was not accessible.
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
         :raises SourceNotFound: if the source file was not found on the referred storage.
         """
 
         space_token = ''
         if self.attributes['extended_attributes'] is not None and 'space_token' in list(self.attributes['extended_attributes'].keys()):
             space_token = '--dst %s' % self.attributes['extended_attributes']['space_token']
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/ssh.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/ssh.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     def stat(self, path):
         """
         Returns the stats of a file.
 
         :param path: path to file
 
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
 
         :returns: a dict with two keys, filesize and an element of GLOBALLY_SUPPORTED_CHECKSUMS.
         """
         self.logger(logging.DEBUG, 'ssh.stat: path: {}'.format(path))
         ret = {}
         chsum = None
         path = self.pfn2path(path)
@@ -214,15 +214,15 @@
 
             :param source: path to the source file on the client file system
             :param target: path to the destination file on the storage
             :param source_dir: Path where the to be transferred files are stored in the local file system
             :param transfer_timeout: Transfer timeout (in seconds) - dummy
 
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'ssh.put: filename: {} target: {}'.format(filename, target))
         source_dir = source_dir or '.'
         source_url = '%s/%s' % (source_dir, filename)
         self.logger(logging.DEBUG, 'ssh.put: source url: {}'.format(source_url))
 
@@ -241,15 +241,15 @@
 
     def delete(self, pfn):
         """
             Deletes a file from the connected RSE.
 
             :param pfn: Physical file name
 
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'ssh.delete: pfn: {}'.format(pfn))
         if not self.exists(pfn):
             raise exception.SourceNotFound()
         try:
             path = self.pfn2path(pfn)
@@ -263,15 +263,15 @@
 
     def rename(self, pfn, new_pfn):
         """ Allows to rename a file stored inside the connected RSE.
 
             :param pfn:      Current physical file name
             :param new_pfn  New physical file name
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'ssh.rename: pfn: {}'.format(pfn))
         if not self.exists(pfn):
             raise exception.SourceNotFound()
         try:
             path = self.pfn2path(pfn)
@@ -294,15 +294,15 @@
 
     def stat(self, path):
         """
         Returns the stats of a file.
 
         :param path: path to file
 
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
 
         :returns: a dict with two keys, filesize and an element of GLOBALLY_SUPPORTED_CHECKSUMS.
         """
         self.logger(logging.DEBUG, 'rsync.stat: path: {}'.format(path))
         ret = {}
         chsum = None
         path = self.pfn2path(path)
@@ -386,15 +386,15 @@
 
             :param source: path to the source file on the client file system
             :param target: path to the destination file on the storage
             :param source_dir: Path where the to be transferred files are stored in the local file system
             :param transfer_timeout: Transfer timeout (in seconds) - dummy
 
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'rsync.put: filename: {} target: {}'.format(filename, target))
         source_dir = source_dir or '.'
         source_url = '%s/%s' % (source_dir, filename)
         self.logger(logging.DEBUG, 'rsync.put: source url: {}'.format(source_url))
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/storm.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/storm.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                                                                                     name=lfn['name'])
             pfns['%s:%s' % (lfn['scope'], lfn['name'])] = ''.join(['storm://', hostname, ':', str(self.attributes['port']), prefix, path])
 
         return pfns
 
     def path2pfn(self, path):
         """
-            Retruns a fully qualified PFN for the file referred by path.
+            Returns a fully qualified PFN for the file referred by path.
 
             :param path: The path to the file.
 
             :returns: Fully qualified PFN.
 
         """
         return ''.join([self.rse['scheme'], '://%s' % self.rse['hostname'], path])
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/webdav.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/webdav.py`

 * *Files 1% similar despite different names*

```diff
@@ -474,15 +474,15 @@
 
     def stat(self, path):
         """
             Returns the stats of a file.
 
             :param path: path to file
 
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
             :raises RSEAccessDenied: in case of permission issue.
 
             :returns: a dict with filesize of the file provided in path as a key.
         """
         headers = {'Depth': '1'}
         dict_ = {}
@@ -523,15 +523,15 @@
 
     def get_space_usage(self):
         """
         Get RSE space usage information.
 
         :returns: a list with dict containing 'totalsize' and 'unusedsize'
 
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
         """
         endpoint_basepath = self.path2pfn('')
         headers = {'Depth': '0'}
 
         try:
             root = ET.fromstring(self.session.request('PROPFIND', endpoint_basepath, verify=False, headers=headers, cert=self.session.cert).text)
             usedsize = root[0][1][0].find('{DAV:}quota-used-bytes').text
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/protocols/xrootd.py` & `rucio_clients-34.3.0/lib/rucio/rse/protocols/xrootd.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
     def stat(self, path):
         """
         Returns the stats of a file.
 
         :param path: path to file
 
-        :raises ServiceUnavailable: if some generic error occured in the library.
+        :raises ServiceUnavailable: if some generic error occurred in the library.
 
         :returns: a dict with two keys, filesize and an element of GLOBALLY_SUPPORTED_CHECKSUMS.
         """
         self.logger(logging.DEBUG, f'xrootd.stat: path: {path}')
         ret = {}
         chsum = None
         if path.startswith('root:'):
@@ -228,15 +228,15 @@
 
             :param source: path to the source file on the client file system
             :param target: path to the destination file on the storage
             :param source_dir: Path where the to be transferred files are stored in the local file system
             :param transfer_timeout: Transfer timeout (in seconds) - dummy
 
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'xrootd.put: filename: {} target: {}'.format(filename, target))
         source_dir = source_dir or '.'
         source_url = '%s/%s' % (source_dir, filename)
         self.logger(logging.DEBUG, 'xrootd put: source url: {}'.format(source_url))
         path = self.path2pfn(target)
@@ -253,15 +253,15 @@
 
     def delete(self, pfn):
         """
             Deletes a file from the connected RSE.
 
             :param pfn: Physical file name
 
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'xrootd.delete: pfn: {}'.format(pfn))
         if not self.exists(pfn):
             raise exception.SourceNotFound()
         try:
             path = self.pfn2path(pfn)
@@ -275,15 +275,15 @@
 
     def rename(self, pfn, new_pfn):
         """ Allows to rename a file stored inside the connected RSE.
 
             :param pfn:      Current physical file name
             :param new_pfn  New physical file name
             :raises DestinationNotAccessible: if the destination storage was not accessible.
-            :raises ServiceUnavailable: if some generic error occured in the library.
+            :raises ServiceUnavailable: if some generic error occurred in the library.
             :raises SourceNotFound: if the source file was not found on the referred storage.
         """
         self.logger(logging.DEBUG, 'xrootd.rename: pfn: {}'.format(pfn))
         if not self.exists(pfn):
             raise exception.SourceNotFound()
         try:
             path = self.pfn2path(pfn)
```

### Comparing `rucio_clients-34.2.0/lib/rucio/rse/rsemanager.py` & `rucio_clients-34.3.0/lib/rucio/rse/rsemanager.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio/version.py` & `rucio_clients-34.3.0/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/lib/rucio_clients.egg-info/SOURCES.txt` & `rucio_clients-34.3.0/lib/rucio_clients.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/pylintrc` & `rucio_clients-34.3.0/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/requirements.txt` & `rucio_clients-34.3.0/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -45,13 +45,14 @@
 pytest-xdist~=3.5.0                                         # Used for parallel testing
 pyflakes==3.1.0                                             # Passive checker of Python programs
 flake8==6.1.0                                               # Wrapper around PyFlakes&pep8; python_version < '3.9'
 pycodestyle==2.11.0                                         # New package replacing pep8; python_version < '3.9'
 pylint==3.0.2
 astroid==3.0.1
 virtualenv==20.24.7                                         # Virtual Python Environment builder
+xmlsec==1.3.13,!=1.3.14                                     # Required to install pyproject.toml-based projects; 1.3.14 excluded due to https://github.com/xmlsec/python-xmlsec/issues/314
 xmltodict==0.13.0                                           # Makes working with XML feel like you are working with JSON
 pytz==2023.3.post1                                          # World timezone definitions, modern and historical
 pydoc-markdown~=4.8.2                                       # Used for generating Markdown documentation for docusaurus
 sh~=2.0.6                                                   # Convenience library for running subprocesses in Python
 apispec==6.3.0                                              # Generate OpenApi definition out of pydoc comments
 apispec-webframeworks                                       # Integration of apispec in Flask
```

### Comparing `rucio_clients-34.2.0/setup.py` & `rucio_clients-34.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/setuputil.py` & `rucio_clients-34.3.0/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_abacus_account.py` & `rucio_clients-34.3.0/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_abacus_collection_replica.py` & `rucio_clients-34.3.0/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_abacus_rse.py` & `rucio_clients-34.3.0/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_account.py` & `rucio_clients-34.3.0/tests/test_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         invalid_usr = account_name_generator()
         add_account(usr, 'USER', 'rucio@email.com', 'root', vo=vo)
         assert account_exists(usr, vo=vo)
         assert not account_exists(invalid_usr, vo=vo)
         del_account(usr, 'root', vo=vo)
 
     def test_update_account(self, vo):
-        """ ACCOUNT (CORE): Test changing and quering account parameters """
+        """ ACCOUNT (CORE): Test changing and querying account parameters """
         usr = account_name_generator()
         add_account(usr, 'USER', 'rucio@email.com', 'root', vo=vo)
         assert get_account_info(usr, vo=vo)['status'] == AccountStatus.ACTIVE  # Should be active by default
         update_account(account=usr, key='status', value=AccountStatus.SUSPENDED, vo=vo)
         assert get_account_info(usr, vo=vo)['status'] == AccountStatus.SUSPENDED
         update_account(account=usr, key='status', value=AccountStatus.ACTIVE, vo=vo)
         assert get_account_info(usr, vo=vo)['status'] == AccountStatus.ACTIVE
@@ -124,16 +124,16 @@
     assert response.status_code == 200
     body = loads(response.get_data(as_text=True))
     assert body['account'] == acntusr
 
 
 def test_get_user_failure(rest_client, auth_token):
     """ ACCOUNT (REST): send a GET with a wrong user test the error """
-    reponse = rest_client.get('/accounts/wronguser', headers=headers(auth(auth_token)))
-    assert reponse.status_code == 404
+    response = rest_client.get('/accounts/wronguser', headers=headers(auth(auth_token)))
+    assert response.status_code == 404
 
 
 def test_del_user_success(rest_client, auth_token):
     """ ACCOUNT (REST): send a DELETE to disable the new user """
     acntusr = account_name_generator()
     data = {'type': 'USER', 'email': 'rucio@email.com'}
     response = rest_client.post('/accounts/' + acntusr, headers=headers(auth(auth_token)), json=data)
```

### Comparing `rucio_clients-34.2.0/tests/test_account_limits.py` & `rucio_clients-34.3.0/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_api_external_representation.py` & `rucio_clients-34.3.0/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_archive.py` & `rucio_clients-34.3.0/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_auditor.py` & `rucio_clients-34.3.0/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_auditor_hdfs.py` & `rucio_clients-34.3.0/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_auditor_srmdumps.py` & `rucio_clients-34.3.0/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_authentication.py` & `rucio_clients-34.3.0/tests/test_authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import base64
 import datetime
 import time
 
 import pytest
 from requests import session
 
 from rucio.api.authentication import get_auth_token_saml, get_auth_token_ssh, get_auth_token_user_pass, get_ssh_challenge_token
@@ -121,15 +120,15 @@
         try:
             add_account_identity(PUBLIC_KEY, IdentityType.SSH, root_account, email='ph-adp-ddm-lab@cern.ch')
         except Duplicate:
             pass  # might already exist, can skip
 
         challenge_token = get_ssh_challenge_token(account='root', appid='test', ip='127.0.0.1', vo=vo).get('token')
 
-        signature = base64.b64decode(ssh_sign(PRIVATE_KEY, challenge_token))
+        signature = ssh_sign(PRIVATE_KEY, challenge_token)
 
         result = get_auth_token_ssh(account='root', signature=signature, appid='test', ip='127.0.0.1', vo=vo)
 
         assert result is not None
 
         del_account_identity(PUBLIC_KEY, IdentityType.SSH, root_account)
 
@@ -155,16 +154,15 @@
         try:
             add_account_identity(INVALID_PADDED_PUBLIC_KEY, IdentityType.SSH, root_account, email='ph-adp-ddm-lab@cern.ch')
         except Duplicate:
             pass  # might already exist, can skip
 
         challenge_token = get_ssh_challenge_token(account='root', appid='test', ip='127.0.0.1', vo=vo).get('token')
 
-        ssh_sign_string = ssh_sign(PRIVATE_KEY, challenge_token)
-        signature = base64.b64decode(ssh_sign_string)
+        signature = ssh_sign(PRIVATE_KEY, challenge_token)
         result = get_auth_token_ssh(account='root', signature=signature, appid='test', ip='127.0.0.1', vo=vo)
         assert result is not None
 
         del_account_identity(INVALID_PADDED_PUBLIC_KEY, IdentityType.SSH, root_account)
 
     def test_get_auth_token_saml_success(self, vo, root_account):
         """AUTHENTICATION (CORE): SAML NameID (correct credentials)."""
@@ -276,15 +274,15 @@
         response = rest_client.get('/auth/saml', headers=headers(hdrdict(headers_dict)))
 
     assert response.status_code == 401
 
 
 @pytest.mark.noparallel(reason='adds many tokens')
 def test_many_tokens(vo, root_account, db_session):
-    """AUTHENTIFICATION (REST): Error when deleting too many tokens."""
+    """AUTHENTICATION (REST): Error when deleting too many tokens."""
     for i in range(2000):
         models.Token(account=root_account, token="dummytoken" + str(i), ip='127.0.0.1', expired_at=datetime.datetime.utcnow()).save(session=db_session)
     db_session.commit()
 
     # Ensures that the tokens are expired
     time.sleep(1)
     print(get_auth_token_user_pass(account='root', username='ddmlab', password='secret', appid='test', ip='127.0.0.1', vo=vo))
```

### Comparing `rucio_clients-34.2.0/tests/test_automatix.py` & `rucio_clients-34.3.0/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_bad_replica.py` & `rucio_clients-34.3.0/tests/test_bad_replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
             if badrep['rse_id'] == rse3_id:
                 if badrep['scope'].external == rep['scope'] and badrep['name'] == rep['name']:
                     nbbadrep += 1
     assert len(replicas) == nbbadrep
 
     list_rep.extend(['srm://%s.cern.ch/test_%s/%s/%s' % (rse2_id, rse2_id, tmp_scope, generate_uuid()), ])
     with pytest.raises(InvalidType):
-        # this should fail becase the replica list will now contain a mix of PFNs and dictionaries
+        # this should fail because the replica list will now contain a mix of PFNs and dictionaries
         replica_client.declare_bad_file_replicas(list_rep, 'This is a good reason')
 
 
 def test_client_add_suspicious_replicas(rse_factory, replica_client):
     """ REPLICA (CLIENT): Add suspicious replicas"""
     tmp_scope = 'mock'
     nbfiles = 5
```

### Comparing `rucio_clients-34.2.0/tests/test_bb8.py` & `rucio_clients-34.3.0/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_belleii.py` & `rucio_clients-34.3.0/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_bin_rucio.py` & `rucio_clients-34.3.0/tests/test_bin_rucio.py`

 * *Files 1% similar despite different names*

```diff
@@ -613,15 +613,15 @@
         print(out, err)
         # create dataset
         cmd = 'rucio add-dataset ' + tmp_dataset
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add files to dataset
-        cmd = 'rucio attach {0} {3}:{1} {3}:{2}'.format(tmp_dataset, tmp_file1[5:], tmp_file2[5:], self.user)  # triming '/tmp/' from filename
+        cmd = 'rucio attach {0} {3}:{1} {3}:{2}'.format(tmp_dataset, tmp_file1[5:], tmp_file2[5:], self.user)  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # find the added files
         cmd = 'rucio list-files ' + tmp_dataset
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
@@ -633,15 +633,15 @@
         tmp_file1 = file_generator()
         # add files
         cmd = 'rucio upload --rse {0} --scope {1} {2}'.format(self.def_rse, self.user, tmp_file1)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # download files
-        cmd = 'rucio -v download --dir /tmp {0}:{1}'.format(self.user, tmp_file1[5:])  # triming '/tmp/' from filename
+        cmd = 'rucio -v download --dir /tmp {0}:{1}'.format(self.user, tmp_file1[5:])  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # search for the files with ls
         cmd = 'ls /tmp/'    # search in /tmp/
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
@@ -651,15 +651,15 @@
         tmp_file1 = file_generator()
         # add files
         cmd = 'rucio upload --rse {0} --scope {1} {2}'.format(self.def_rse, self.user, tmp_file1)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # download files
-        cmd = 'rucio -v download --dir /tmp {0}:{1}'.format(self.user, tmp_file1[5:-2] + '*')  # triming '/tmp/' from filename
+        cmd = 'rucio -v download --dir /tmp {0}:{1}'.format(self.user, tmp_file1[5:-2] + '*')  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # search for the files with ls
         cmd = 'ls /tmp/'    # search in /tmp/
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
@@ -707,15 +707,15 @@
         impl = 'posix'
         # add files
         cmd = 'rucio upload --rse {0} --scope {1} --impl {2} {3}'.format(self.def_rse, self.user, impl, tmp_file1)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # download files
-        cmd = 'rucio -v download --dir /tmp {0}:{1} --impl {2}'.format(self.user, tmp_file1[5:], impl)  # triming '/tmp/' from filename
+        cmd = 'rucio -v download --dir /tmp {0}:{1} --impl {2}'.format(self.user, tmp_file1[5:], impl)  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # search for the files with ls
         cmd = 'ls /tmp/'    # search in /tmp/
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
@@ -725,15 +725,15 @@
         tmp_file1 = file_generator()
         # add files
         cmd = 'rucio upload --rse {0} --scope {1} --impl {2} {3}'.format(self.def_rse, self.user, impl, tmp_file1)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # download files
-        cmd = 'rucio -v download --dir /tmp {0}:{1} --impl {2}'.format(self.user, tmp_file1[5:-2] + '*', impl)  # triming '/tmp/' from filename
+        cmd = 'rucio -v download --dir /tmp {0}:{1} --impl {2}'.format(self.user, tmp_file1[5:-2] + '*', impl)  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # search for the files with ls
         cmd = 'ls /tmp/'    # search in /tmp/
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
@@ -754,27 +754,27 @@
         # add files
         cmd = 'rucio upload --rse {0} --scope {1} {2}'.format(self.def_rse, self.user, tmp_file)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         assert exitcode == 0
         # download files with --no-subdir
-        cmd = 'rucio -v download --no-subdir --dir /tmp {0}:{1}'.format(self.user, tmp_file[5:])  # triming '/tmp/' from filename
+        cmd = 'rucio -v download --no-subdir --dir /tmp {0}:{1}'.format(self.user, tmp_file[5:])  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         assert exitcode == 0
         # search for the files with ls
         cmd = 'ls /tmp/'    # search in /tmp/
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         assert tmp_file[5:] in out
         # download again with --no-subdir
-        cmd = 'rucio -v download --no-subdir --dir /tmp {0}:{1}'.format(self.user, tmp_file[5:])  # triming '/tmp/' from filename
+        cmd = 'rucio -v download --no-subdir --dir /tmp {0}:{1}'.format(self.user, tmp_file[5:])  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         assert exitcode == 0
         assert re.search(r'Downloaded files:\s+0', out) is not None
         assert re.search(r'Files already found locally:\s+1', out) is not None
 
@@ -898,15 +898,15 @@
         tmp_file1 = file_generator()
         # add files
         cmd = 'rucio upload --rse {0} --scope {1} {2}'.format(self.def_rse, self.user, tmp_file1)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # download files
-        cmd = 'rucio download --dir /tmp --transfer-timeout 3 --transfer-speed-timeout 1000 {0}:{1}'.format(self.user, tmp_file1[5:])  # triming '/tmp/' from filename
+        cmd = 'rucio download --dir /tmp --transfer-timeout 3 --transfer-speed-timeout 1000 {0}:{1}'.format(self.user, tmp_file1[5:])  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         assert 'successfully downloaded' in err
         # search for the files with ls
         cmd = 'ls /tmp/'    # search in /tmp/
         print(self.marker + cmd)
@@ -1042,50 +1042,50 @@
         print(out, err)
         # create dataset
         cmd = 'rucio add-dataset ' + tmp_dataset
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add files to dataset
-        cmd = 'rucio attach {0} {1}:{2}'.format(tmp_dataset, self.user, tmp_file1[5:])  # triming '/tmp/' from filename
+        cmd = 'rucio attach {0} {1}:{2}'.format(tmp_dataset, self.user, tmp_file1[5:])  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
 
         os.remove(tmp_file1)
 
         # download dataset
-        cmd = 'rucio -v download --dir /tmp {0}'.format(tmp_dataset)  # triming '/tmp/' from filename
+        cmd = 'rucio -v download --dir /tmp {0}'.format(tmp_dataset)  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
-        search = '{0} successfully downloaded'.format(tmp_file1[5:])  # triming '/tmp/' from filename
+        search = '{0} successfully downloaded'.format(tmp_file1[5:])  # trimming '/tmp/' from filename
         assert re.search(search, err) is not None
 
     def test_download_file_check_by_size(self):
         """CLIENT(USER): Rucio download files"""
         tmp_file1 = file_generator()
         # add files
         cmd = 'rucio upload --rse {0} --scope {1} {2}'.format(self.def_rse, self.user, tmp_file1)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # download files
-        cmd = 'rucio -v download --dir /tmp {0}:{1}'.format(self.user, tmp_file1[5:])  # triming '/tmp/' from filename
+        cmd = 'rucio -v download --dir /tmp {0}:{1}'.format(self.user, tmp_file1[5:])  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # Alter downloaded file
-        cmd = 'echo "dummy" >> /tmp/{}/{}'.format(self.user, tmp_file1[5:])  # triming '/tmp/' from filename
+        cmd = 'echo "dummy" >> /tmp/{}/{}'.format(self.user, tmp_file1[5:])  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         assert exitcode == 0
         # Download file again and check for mismatch
-        cmd = 'rucio -v download --check-local-with-filesize-only --dir /tmp {0}:{1}'.format(self.user, tmp_file1[5:])  # triming '/tmp/' from filename
+        cmd = 'rucio -v download --check-local-with-filesize-only --dir /tmp {0}:{1}'.format(self.user, tmp_file1[5:])  # trimming '/tmp/' from filename
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         assert exitcode == 0
         assert "File with same name exists locally, but filesize mismatches" in err
 
     def test_list_blocklisted_replicas(self):
@@ -1100,15 +1100,15 @@
               '--domain-json \'{"wan": {"read": 1, "write": 1, "delete": 1, "third_party_copy_read": 1, "third_party_copy_write": 1}}\' %s' % tmp_rse
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
 
         # add files
         tmp_file1 = file_generator()
-        file_name = tmp_file1[5:]  # triming '/tmp/' from filename
+        file_name = tmp_file1[5:]  # trimming '/tmp/' from filename
         cmd = 'rucio upload --rse {0} --scope {1} {2}'.format(tmp_rse, self.user, tmp_file1)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
 
         # create dataset
         tmp_dataset = self.user + ':DSet' + rse_name_generator()
@@ -1155,52 +1155,52 @@
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         # add quota
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value ATLASSCRATCHDISK'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add rse
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add quota
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value ATLASSCRATCHDISK'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add rse
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add quota
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value ATLASSCRATCHDISK'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add rules
         cmd = "rucio add-rule {0}:{1} 3 'spacetoken=ATLASSCRATCHDISK'".format(self.user, tmp_file1[5:])
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         assert not err
-        rule = out[:-1]  # triming new line character
+        rule = out[:-1]  # trimming new line character
         assert re.match(r'^\w+$', rule)
         # check if rule exist for the file
         cmd = "rucio list-rules {0}:{1}".format(self.user, tmp_file1[5:])
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         assert re.search(rule, out) is not None
@@ -1217,15 +1217,15 @@
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add quota
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value ATLASRULEDELAYED'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # try adding rule with an incorrect delay-injection. Must fail
         cmd = "rucio add-rule --delay-injection asdsaf {0}:{1} 1 'spacetoken=ATLASRULEDELAYED'".format(self.user, tmp_file1[5:])
         print(self.marker + cmd)
@@ -1233,15 +1233,15 @@
         assert err
         # Add a correct rule
         cmd = "rucio add-rule --delay-injection 3600 {0}:{1} 1 'spacetoken=ATLASRULEDELAYED'".format(self.user, tmp_file1[5:])
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         assert not err
-        rule = out[:-1]  # triming new line character
+        rule = out[:-1]  # trimming new line character
         cmd = "rucio rule-info {0}".format(rule)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         out_lines = out.splitlines()
         assert any(re.match(r'State:.* INJECT', line) for line in out_lines)
         assert any(re.match(r'Locks OK/REPLICATING/STUCK:.* 0/0/0', line) for line in out_lines)
@@ -1264,15 +1264,15 @@
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
 
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value ATLASDELETERULE'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add rules
         cmd = "rucio add-rule {0}:{1} 1 'spacetoken=ATLASDELETERULE'".format(self.user, tmp_file1[5:])
         print(self.marker + cmd)
@@ -1313,62 +1313,62 @@
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         # add quota
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value ATLASSCRATCHDISK'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add rse
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add quota
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value ATLASSCRATCHDISK'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add rse
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add quota
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value ATLASSCRATCHDISK'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add rules
         cmd = "rucio add-rule {0}:{1} 3 'spacetoken=ATLASSCRATCHDISK'".format(self.user, tmp_file1[5:])
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         assert not err
-        rule = out[:-1]  # triming new line character
+        rule = out[:-1]  # trimming new line character
         assert re.match(r'^\w+$', rule)
 
         # move rule
         new_rule_expr = "'spacetoken=ATLASSCRATCHDISK|spacetoken=ATLASSD'"
         cmd = "rucio move-rule {} {}".format(rule, new_rule_expr)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         assert not err
-        new_rule = out[:-1]  # triming new line character
+        new_rule = out[:-1]  # trimming new line character
 
         # check if rule exist for the file
         cmd = "rucio list-rules {0}:{1}".format(self.user, tmp_file1[5:])
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         assert re.search(new_rule, out) is not None
@@ -1385,63 +1385,63 @@
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         # add quota
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value ATLASSCRATCHDISK'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add rse
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add quota
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value ATLASSCRATCHDISK'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add rse
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add quota
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value ATLASSCRATCHDISK'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add rules
         cmd = "rucio add-rule {0}:{1} 3 'spacetoken=ATLASSCRATCHDISK'".format(self.user, tmp_file1[5:])
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         assert not err
-        rule = out[:-1]  # triming new line character
+        rule = out[:-1]  # trimming new line character
         assert re.match(r'^\w+$', rule)
         # move rule
         new_rule_expr = "spacetoken=ATLASSCRATCHDISK|spacetoken=ATLASSD"
         new_rule_activity = "No User Subscription"
         new_rule_source_replica_expression = "spacetoken=ATLASSCRATCHDISK|spacetoken=ATLASSD"
         cmd = "rucio move-rule --activity '{}' --source-replica-expression '{}' {} '{}'".format(new_rule_activity, new_rule_source_replica_expression, rule, new_rule_expr)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         assert not err
-        new_rule_id = out[:-1]  # triming new line character
+        new_rule_id = out[:-1]  # trimming new line character
 
         # check if rule exist for the file
         cmd = "rucio list-rules {0}:{1}".format(self.user, tmp_file1[5:])
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         assert re.search(new_rule_id, out) is not None
@@ -1480,15 +1480,15 @@
         print(out, err)
         rule = out
         # delete the file from the catalog
         cmd = "rucio delete-rule {0}".format(rule)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
-        # delete the fisical file
+        # delete the physical file
         cmd = "find /tmp/rucio_rse/ -name {0} |xargs rm".format(tmp_file1[5:])
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # modify the file to avoid same checksum
         cmd = "echo 'delta' >> {0}".format(tmp_file1)
         print(self.marker + cmd)
@@ -1520,15 +1520,15 @@
         exitcode, out, err = execute(cmd)
         print(out)
         print(err)
         remove(tmp_file1)
         remove(tmp_file2)
         remove(tmp_file3)
         # attach the files to the dataset
-        cmd = 'rucio attach {0} {1}:{2} {1}:{3}'.format(tmp_dsn, self.user, tmp_file2[5:], tmp_file3[5:])  # triming '/tmp/' from filenames
+        cmd = 'rucio attach {0} {1}:{2} {1}:{3}'.format(tmp_dsn, self.user, tmp_file2[5:], tmp_file3[5:])  # trimming '/tmp/' from filenames
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         print(err)
         # searching for the file in the new dataset
         cmd = 'rucio list-files {0}'.format(tmp_dsn)
         print(self.marker + cmd)
@@ -1553,15 +1553,15 @@
         exitcode, out, err = execute(cmd)
         print(out)
         print(err)
         remove(tmp_file1)
         remove(tmp_file2)
         remove(tmp_file3)
         # detach the files to the dataset
-        cmd = 'rucio detach {0} {1}:{2} {1}:{3}'.format(tmp_dsn, self.user, tmp_file2[5:], tmp_file3[5:])  # triming '/tmp/' from filenames
+        cmd = 'rucio detach {0} {1}:{2} {1}:{3}'.format(tmp_dsn, self.user, tmp_file2[5:], tmp_file3[5:])  # trimming '/tmp/' from filenames
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         print(err)
         # searching for the file in the new dataset
         cmd = 'rucio list-files {0}'.format(tmp_dsn)
         print(self.marker + cmd)
@@ -1582,15 +1582,15 @@
         cmd = 'rucio upload --rse {0} --scope {1} {2} {3}'.format(self.def_rse, self.user, tmp_file1, tmp_dsn)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         print(err)
         remove(tmp_file1)
         # attach the files to the dataset
-        cmd = 'rucio attach {0} {1}:{2}'.format(tmp_dsn, self.user, tmp_file1[5:])  # triming '/tmp/' from filenames
+        cmd = 'rucio attach {0} {1}:{2}'.format(tmp_dsn, self.user, tmp_file1[5:])  # trimming '/tmp/' from filenames
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         print(err)
         assert re.search("The file already exists", err) is not None
 
     def test_attach_dataset_twice(self):
@@ -1620,15 +1620,15 @@
         cmd = 'rucio upload --rse {0} --scope {1} {2} {3}'.format(self.def_rse, self.user, tmp_file1, tmp_dsn)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         print(err)
         remove(tmp_file1)
         # attach the files to the dataset
-        cmd = 'rucio detach {0} {1}:{2}'.format(tmp_dsn, self.user, 'file_ghost')  # triming '/tmp/' from filenames
+        cmd = 'rucio detach {0} {1}:{2}'.format(tmp_dsn, self.user, 'file_ghost')  # trimming '/tmp/' from filenames
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         print(err)
         assert re.search("Data identifier not found.", err) is not None
 
     @pytest.mark.dirty
@@ -1678,15 +1678,15 @@
         cmd = 'rucio attach {0}'.format(tmp_dsn_did)
         for tmp_file in files:
             cmd += ' {0}:{1}'.format(tmp_file['scope'], tmp_file['name'])
         exitcode, out, err = execute(cmd)
         print(out)
         print(err)
 
-        # Checking if the execution was successfull and if the DIDs belong together
+        # Checking if the execution was successful and if the DIDs belong together
         assert re.search('DIDs successfully attached', out) is not None
         cmd = 'rucio list-content {0}'.format(tmp_dsn_did)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         # first dataset must be in the container
         assert re.search("{0}:{1}".format(self.user, files[0]['name']), out) is not None
         # last dataset must be in the container
@@ -1707,15 +1707,15 @@
         cmd = 'rucio attach {0} -f {1}'.format(tmp_dsn_did, did_file_path)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         print(err)
         remove(did_file_path)
 
-        # Checking if the execution was successfull and if the DIDs belong together
+        # Checking if the execution was successful and if the DIDs belong together
         assert re.search('DIDs successfully attached', out) is not None
         cmd = 'rucio list-content {0}'.format(tmp_dsn_did)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         # first file must be in the dataset
         assert re.search("{0}:{1}".format(self.user, files[0]['name']), out) is not None
         # last file must be in the dataset
@@ -2179,15 +2179,15 @@
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
 
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value ATLASDELETERULE'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add rules
         cmd = "rucio add-rule {0}:{1} 1 'spacetoken=ATLASDELETERULE'".format(self.user, tmp_file1[5:])
         print(self.marker + cmd)
@@ -2226,15 +2226,15 @@
         tmp_rse = rse_name_generator()
         cmd = 'rucio-admin rse add {0}'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out)
         self.account_client.set_local_account_limit('root', tmp_rse, -1)
 
-        # add rse atributes
+        # add rse attributes
         cmd = 'rucio-admin rse set-attribute --rse {0} --key spacetoken --value MARIOSPACEODYSSEY'.format(tmp_rse)
         print(self.marker + cmd)
         exitcode, out, err = execute(cmd)
         print(out, err)
         # add rules
         cmd = "rucio add-rule {0}:{1} 1 'spacetoken=MARIOSPACEODYSSEY'".format(self.user, tmp_file1[5:])
         print(self.marker + cmd)
```

### Comparing `rucio_clients-34.2.0/tests/test_boolean.py` & `rucio_clients-34.3.0/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_clients.py` & `rucio_clients-34.3.0/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_common_types.py` & `rucio_clients-34.3.0/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_config.py` & `rucio_clients-34.3.0/tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 from rucio.common import exception
 from rucio.common.utils import generate_uuid
 
 
 class TestConfigCore:
 
     def test_get_config_sections(self):
-        """ CONFIG (CORE): Retreive configuration section only """
+        """ CONFIG (CORE): Retrieve configuration section only """
         expected_sections = [str(generate_uuid()), str(generate_uuid())]
         for section in expected_sections:
             core_config.set(section, str(generate_uuid()), str(generate_uuid()))
         sections = core_config.sections(use_cache=False)
         for section in expected_sections:
             assert section in sections
 
     def test_get_and_set_section_option(self):
-        """ CONFIG (CORE): Retreive configuration option only """
+        """ CONFIG (CORE): Retrieve configuration option only """
         # get and set
         section = str(generate_uuid())
         option = str(generate_uuid())
         expected_value = str(generate_uuid())
         core_config.set(section=section, option=option, value=expected_value)
         value = core_config.get(section, option, use_cache=False, convert_type_fnc=lambda x: x)
         assert value == expected_value
```

### Comparing `rucio_clients-34.2.0/tests/test_conveyor.py` & `rucio_clients-34.3.0/tests/test_conveyor.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from unittest.mock import patch
 from urllib.parse import parse_qsl, urlencode, urlparse, urlunparse
 
 import pytest
 from sqlalchemy import update
 
 import rucio.daemons.reaper.reaper
+from rucio.common.constants import RseAttr
 from rucio.common.exception import ReplicaNotFound, RequestNotFound
 from rucio.common.types import InternalAccount
 from rucio.common.utils import adler32, generate_uuid
 from rucio.core import config as core_config
 from rucio.core import did as did_core
 from rucio.core import distance as distance_core
 from rucio.core import lock as lock_core
@@ -220,15 +221,15 @@
         replica = replica_core.get_replica(rse_id=jump_rse_id, **did)
         assert replica['state'] == ReplicaState.COPYING
 
         # Wait for the intermediate replica to become ready
         replica = __wait_for_replica_transfer(dst_rse_id=jump_rse_id, **did)
         assert replica['state'] == ReplicaState.AVAILABLE
 
-        # ensure tha the ranking was correct for all sources and intermediate rses
+        # ensure that the ranking was correct for all sources and intermediate rses
         assert __get_source(request_id=request['id'], src_rse_id=src_rse1_id, **did).ranking == 0
         assert __get_source(request_id=request['id'], src_rse_id=jump_rse_id, **did).ranking == 0
         assert __get_source(request_id=request['id'], src_rse_id=src_rse2_id, **did).ranking == 0
         # Only group_bulk=1 part of the path was submitted.
         # run submitter again to copy from jump rse to destination rse
         __update_request(request_core.get_request_by_did(rse_id=dst_rse_id, **did)['id'], last_processed_by=None)
         submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], partition_wait_time=0, transfertype='single', filter_transfertool=None)
@@ -297,15 +298,15 @@
     # Finisher will handle transfers of the same multihop one hop at a time
     finisher(once=True, partition_wait_time=0)
     finisher(once=True, partition_wait_time=0)
     # The intermediate request must not be re-scheduled by finisher
     with pytest.raises(RequestNotFound):
         request_core.get_request_by_did(rse_id=jump_rse_id, **did)
     request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
-    # ensure tha the ranking was correctly decreased for the whole path
+    # ensure that the ranking was correctly decreased for the whole path
     assert __get_source(request_id=request['id'], src_rse_id=jump_rse_id, **did).ranking == -1
     assert __get_source(request_id=request['id'], src_rse_id=src_rse_id, **did).ranking == -1
     assert request['state'] == RequestState.QUEUED
 
 
 @skip_rse_tests_with_accounts
 @pytest.mark.dirty(reason="leaves files in XRD containers")
@@ -537,15 +538,15 @@
         # Finisher will handle transfers of the same multihop one hop at a time
         finisher(once=True, partition_wait_time=0)
         finisher(once=True, partition_wait_time=0)
         # The intermediate request must not be re-scheduled by finisher
         with pytest.raises(RequestNotFound):
             request_core.get_request_by_did(rse_id=jump_rse_id, **did)
         request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
-        # ensure tha the ranking was correctly decreased for the whole path
+        # ensure that the ranking was correctly decreased for the whole path
         assert __get_source(request_id=request['id'], src_rse_id=jump_rse_id, **did).ranking == -1
         assert __get_source(request_id=request['id'], src_rse_id=src_rse_id, **did).ranking == -1
         assert request['state'] == RequestState.QUEUED
     finally:
         receiver_graceful_stop.set()
         receiver_thread.join(timeout=5)
         receiver_graceful_stop.clear()
@@ -627,15 +628,15 @@
 
     with patch('rucio.daemons.conveyor.receiver.Receiver', ReceiverWrapper):
         receiver_thread = threading.Thread(target=receiver, kwargs={'id_': 0, 'all_vos': True, 'total_threads': 1})
         receiver_thread.start()
         # Fake that destination RSE is a tape
         rse_core.update_rse(rse_id=dst_rse_id, parameters={'rse_type': RSEType.TAPE})
         try:
-            rse_core.add_rse_attribute(dst_rse_id, 'archive_timeout', 60)
+            rse_core.add_rse_attribute(dst_rse_id, RseAttr.ARCHIVE_TIMEOUT, 60)
 
             did = did_factory.upload_test_file(src_rse)
             rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None, activity='test')
             submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=2, partition_wait_time=0, transfertype='single', filter_transfertool=None)
 
             # Wait for the reception of the FTS Completion message for the submitted request
             request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
@@ -653,15 +654,15 @@
             assert request['state'] == RequestState.SUBMITTED
             # Poller should also correctly handle "ARCHIVING" transfers and not mark them as DONE
             poller(once=True, older_than=0, partition_wait_time=0)
             request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
             assert request['state'] == RequestState.SUBMITTED
         finally:
             rse_core.update_rse(rse_id=dst_rse_id, parameters={'rse_type': RSEType.DISK})
-            rse_core.del_rse_attribute(dst_rse_id, 'archive_timeout')
+            rse_core.del_rse_attribute(dst_rse_id, RseAttr.ARCHIVE_TIMEOUT)
 
             receiver_graceful_stop.set()
             receiver_thread.join(timeout=5)
             receiver_graceful_stop.clear()
 
 
 @skip_rse_tests_with_accounts
@@ -675,15 +676,15 @@
     """
     src_rse, src_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     dst_rse1, dst_rse_id1 = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     dst_rse2, dst_rse_id2 = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     all_rses = [src_rse_id, dst_rse_id1, dst_rse_id2]
 
     for rse_id in all_rses:
-        rse_core.add_rse_attribute(rse_id, 'fts', TEST_FTS_HOST)
+        rse_core.add_rse_attribute(rse_id, RseAttr.FTS, TEST_FTS_HOST)
     distance_core.add_distance(src_rse_id, dst_rse_id1, distance=10)
     distance_core.add_distance(src_rse_id, dst_rse_id2, distance=10)
     # Set limits only for one of the RSEs
     request_core.set_transfer_limit(dst_rse1, max_transfers=1, activity='all_activities', strategy='fifo')
 
     did1 = did_factory.upload_test_file(src_rse)
     did2 = did_factory.upload_test_file(src_rse)
@@ -838,17 +839,17 @@
     https://gitlab.cern.ch/dmc/gfal2/-/blob/master/src/plugins/mock/README_PLUGIN_MOCK
     """
     src_rse, src_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', rse_type=RSEType.TAPE)
     dst_rse, dst_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     all_rses = [src_rse_id, dst_rse_id]
 
     distance_core.add_distance(src_rse_id, dst_rse_id, distance=10)
-    rse_core.add_rse_attribute(src_rse_id, 'staging_buffer', dst_rse)
+    rse_core.add_rse_attribute(src_rse_id, RseAttr.STAGING_BUFFER, dst_rse)
     for rse_id in all_rses:
-        rse_core.add_rse_attribute(rse_id, 'fts', TEST_FTS_HOST)
+        rse_core.add_rse_attribute(rse_id, RseAttr.FTS, TEST_FTS_HOST)
 
     did = did_factory.upload_test_file(src_rse)
     replica = replica_core.get_replica(rse_id=src_rse_id, **did)
 
     replica_client.add_replicas(rse=dst_rse, files=[{'scope': did['scope'].external, 'name': did['name'], 'state': 'C',
                                                      'bytes': replica['bytes'], 'adler32': replica['adler32'], 'md5': replica['md5']}])
     request_core.queue_requests(requests=[{'dest_rse_id': dst_rse_id,
@@ -882,16 +883,16 @@
     src_rse, src_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', rse_type=RSEType.TAPE)
     dst_rse, dst_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', rse_type=RSEType.DISK)
     all_rses = [src_rse_id, dst_rse_id]
 
     maximum_pin_lifetime = 86400
 
     distance_core.add_distance(src_rse_id, dst_rse_id, distance=10)
-    rse_core.add_rse_attribute(dst_rse_id, 'staging_required', True)
-    rse_core.add_rse_attribute(dst_rse_id, 'maximum_pin_lifetime', maximum_pin_lifetime)
+    rse_core.add_rse_attribute(dst_rse_id, RseAttr.STAGING_REQUIRED, True)
+    rse_core.add_rse_attribute(dst_rse_id, RseAttr.MAXIMUM_PIN_LIFETIME, maximum_pin_lifetime)
 
     did = did_factory.upload_test_file(rse_name=src_rse)
 
     rule1_id = rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)[0]
     request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
 
     assert request['request_type'] == RequestType.TRANSFER
@@ -943,16 +944,16 @@
     """
     src_rse, src_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', rse_type=RSEType.TAPE)
     dst_rse, dst_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', rse_type=RSEType.DISK)
 
     maximum_pin_lifetime = 86400
 
     distance_core.add_distance(src_rse_id, dst_rse_id, distance=10)
-    rse_core.add_rse_attribute(dst_rse_id, 'staging_required', True)
-    rse_core.add_rse_attribute(dst_rse_id, 'maximum_pin_lifetime', maximum_pin_lifetime)
+    rse_core.add_rse_attribute(dst_rse_id, RseAttr.STAGING_REQUIRED, True)
+    rse_core.add_rse_attribute(dst_rse_id, RseAttr.MAXIMUM_PIN_LIFETIME, maximum_pin_lifetime)
 
     did = did_factory.upload_test_file(rse_name=src_rse)
 
     rule1_id = rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)[0]
     request = request_core.get_request_by_did(rse_id=dst_rse_id, **did)
 
     assert request['request_type'] == RequestType.TRANSFER
@@ -1005,15 +1006,15 @@
     """
     src_rse, src_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     dst_rse, dst_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     all_rses = [src_rse_id, dst_rse_id]
 
     distance_core.add_distance(src_rse_id, dst_rse_id, distance=10)
     for rse_id in all_rses:
-        rse_core.add_rse_attribute(rse_id, 'fts', TEST_FTS_HOST)
+        rse_core.add_rse_attribute(rse_id, RseAttr.FTS, TEST_FTS_HOST)
 
     did = did_factory.upload_test_file(src_rse)
 
     rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
 
     # Fake that the transfer is submitted and lost
     submitter(once=True, rses=[{'id': rse_id} for rse_id in all_rses], group_bulk=2, partition_wait_time=0, transfertype='single', filter_transfertool=None)
@@ -1044,15 +1045,15 @@
     """
     src_rse, src_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     dst_rse, dst_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     all_rses = [src_rse_id, dst_rse_id]
 
     distance_core.add_distance(src_rse_id, dst_rse_id, distance=10)
     for rse_id in all_rses:
-        rse_core.add_rse_attribute(rse_id, 'fts', TEST_FTS_HOST)
+        rse_core.add_rse_attribute(rse_id, RseAttr.FTS, TEST_FTS_HOST)
 
     did = did_factory.upload_test_file(src_rse)
 
     [rule_id] = rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
 
     class _FTSWrapper(FTSWrapper):
         @staticmethod
@@ -1151,19 +1152,19 @@
         rule_core.add_rule(dids=[did1, did2], account=root_account, copies=1, rse_expression=rse3, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
 
         return rse1_id, rse2_id, rse3_id, did1, did2
 
     # Fake that destination RSE is a tape
     rse_core.update_rse(rse_id=rse3_id, parameters={'rse_type': RSEType.TAPE})
     try:
-        rse_core.add_rse_attribute(rse3_id, 'archive_timeout', 60)
+        rse_core.add_rse_attribute(rse3_id, RseAttr.ARCHIVE_TIMEOUT, 60)
         yield __create_dids
     finally:
         rse_core.update_rse(rse_id=rse3_id, parameters={'rse_type': RSEType.DISK})
-        rse_core.del_rse_attribute(rse3_id, 'archive_timeout')
+        rse_core.del_rse_attribute(rse3_id, RseAttr.ARCHIVE_TIMEOUT)
 
 
 @skip_rse_tests_with_accounts
 @pytest.mark.dirty(reason="leaves files in XRD containers")
 @pytest.mark.noparallel(groups=[NoParallelGroups.SUBMITTER, NoParallelGroups.POLLER])
 @pytest.mark.parametrize("caches_mock", [{"caches_to_mock": [
     'rucio.core.rse.REGION',
@@ -1284,15 +1285,15 @@
     'rucio.core.rse_expression_parser.REGION',  # The list of multihop RSEs is retrieved by an expression
     'rucio.core.config.REGION',
     'rucio.rse.rsemanager.RSE_REGION',  # for RSE info
 ]}], indirect=True)
 def test_overwrite_corrupted_files(overwrite_on_tape_topology, core_config_mock, caches_mock):
     """
     If a transfer fails because the destination exists, and the size+checksums of the destination file are wrong,
-    the next submission must be performed according to the overwrite_corrupted_files config paramenter.
+    the next submission must be performed according to the overwrite_corrupted_files config parameter.
     """
     rse1_id, rse2_id, rse3_id, did1, did2 = overwrite_on_tape_topology(did1_corrupted=True, did2_corrupted=True)
     all_rses = [rse1_id, rse2_id, rse3_id]
 
     class _FTSWrapper(FTSWrapper):
         @staticmethod
         def on_receive(job_params):
@@ -1359,15 +1360,15 @@
 
     def __init_test_for_vo(vo, scope):
         src_rse, src_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', vo=vo)
         dst_rse, dst_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', vo=vo)
         all_rses = [src_rse_id, dst_rse_id]
 
         for rse_id in all_rses:
-            rse_core.add_rse_attribute(rse_id, 'fts', TEST_FTS_HOST)
+            rse_core.add_rse_attribute(rse_id, RseAttr.FTS, TEST_FTS_HOST)
         distance_core.add_distance(src_rse_id, dst_rse_id, distance=10)
         account = InternalAccount('root', vo=vo)
         did = did_factory.random_file_did(scope=scope)
         replica_core.add_replica(rse_id=src_rse_id, scope=scope, name=did['name'], bytes_=1, account=account, adler32=None, md5=None)
         rule_core.add_rule(dids=[did], account=account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None,
                            lifetime=None, locked=False, subscription_id=None, ignore_account_limit=True)
         return all_rses
@@ -1437,15 +1438,15 @@
     rse3, rse3_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     rse4, rse4_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     rse5, rse5_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     rse6, rse6_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     rse7, rse7_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     all_rses = [rse1_id, rse2_id, rse3_id, rse4_id, rse5_id, rse6_id, rse7_id]
     for rse_id in all_rses:
-        rse_core.add_rse_attribute(rse_id, 'fts', TEST_FTS_HOST)
+        rse_core.add_rse_attribute(rse_id, RseAttr.FTS, TEST_FTS_HOST)
         rse_core.set_rse_limits(rse_id=rse_id, name='MinFreeSpace', value=1)
         rse_core.set_rse_usage(rse_id=rse_id, source='storage', used=1, free=0)
     distance_core.add_distance(rse1_id, rse2_id, distance=10)
     distance_core.add_distance(rse2_id, rse3_id, distance=10)
     distance_core.add_distance(rse3_id, rse4_id, distance=10)
     distance_core.add_distance(rse4_id, rse5_id, distance=10)
     distance_core.add_distance(rse3_id, rse6_id, distance=10)
@@ -1541,18 +1542,18 @@
     dst_rse2, dst_rse2_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     dst_rse3, dst_rse3_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default')
     all_rses = [src_rse_id, dst_rse1_id, dst_rse2_id, dst_rse3_id]
 
     for rse_id in [dst_rse1_id, dst_rse2_id, dst_rse3_id]:
         distance_core.add_distance(src_rse_id, rse_id, distance=10)
     for rse_id in all_rses:
-        rse_core.add_rse_attribute(rse_id, 'fts', TEST_FTS_HOST)
+        rse_core.add_rse_attribute(rse_id, RseAttr.FTS, TEST_FTS_HOST)
 
     rse_core.add_rse_attribute(src_rse_id, 'supported_checksums', 'adler32')
-    rse_core.add_rse_attribute(dst_rse1_id, 'verify_checksum', False)
+    rse_core.add_rse_attribute(dst_rse1_id, RseAttr.VERIFY_CHECKSUM, False)
     rse_core.add_rse_attribute(dst_rse2_id, 'supported_checksums', 'md5')
     rse_core.add_rse_attribute(dst_rse3_id, 'supported_checksums', 'md5,adler32')
 
     did = did_factory.upload_test_file(src_rse)
     replica = replica_core.get_replica(rse_id=src_rse_id, **did)
 
     rule_core.add_rule(dids=[did], account=root_account, copies=3, rse_expression=f'{dst_rse1}|{dst_rse2}|{dst_rse3}', grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
@@ -1640,15 +1641,15 @@
 
     def __setup_test():
         src_rse, src_rse_id = rse_factory.make_posix_rse()
         dst_rse, dst_rse_id = rse_factory.make_posix_rse()
 
         distance_core.add_distance(src_rse_id, dst_rse_id, distance=10)
         for rse_id in [src_rse_id, dst_rse_id]:
-            rse_core.add_rse_attribute(rse_id, 'fts', TEST_FTS_HOST)
+            rse_core.add_rse_attribute(rse_id, RseAttr.FTS, TEST_FTS_HOST)
         did = did_factory.upload_test_file(src_rse)
         rule_core.add_rule(dids=[did], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
 
         rse_core.update_rse(src_rse_id, {'availability_read': False})
 
         return src_rse_id, dst_rse_id, did
 
@@ -1679,18 +1680,18 @@
         Add existing plugin to fts3 transfertool, verify submission goes through.
     """
     def __setup_test():
         src_rse, src_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', rse_type=RSEType.TAPE)
         dst_rse, dst_rse_id = rse_factory.make_rse(scheme='mock', protocol_impl='rucio.rse.protocols.posix.Default', rse_type=RSEType.TAPE)
 
         distance_core.add_distance(src_rse_id, dst_rse_id, distance=10)
-        rse_core.add_rse_attribute(dst_rse_id, 'verify_checksum', False)
+        rse_core.add_rse_attribute(dst_rse_id, RseAttr.VERIFY_CHECKSUM, False)
 
         for rse_id in [src_rse_id, dst_rse_id]:
-            rse_core.add_rse_attribute(rse_id, 'fts', TEST_FTS_HOST)
+            rse_core.add_rse_attribute(rse_id, RseAttr.FTS, TEST_FTS_HOST)
 
         did_fast = did_factory.upload_test_file(src_rse)
         did_slow = did_factory.upload_test_file(src_rse)
 
         activity_dict = {did_fast['name']: "fast", did_slow['name']: "slow"}
 
         rule_core.add_rule(dids=[did_fast, did_slow], account=root_account, copies=1, rse_expression=dst_rse, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
@@ -1713,15 +1714,15 @@
     with patch("rucio.transfertool.fts3.FTS3Transfertool", _Fts3PluginTestWrapper):
         submitter(once=True, rses=[{'id': rse_id} for rse_id in (src_rse_id, dst_rse_id)], group_bulk=1, partition_wait_time=0, transfertools=['fts3'], transfertype='single')
 
     # Verify that both the submission works
     request_fast = request_core.get_request_by_did(rse_id=dst_rse_id, **did_fast)
     request_slow = request_core.get_request_by_did(rse_id=dst_rse_id, **did_slow)
 
-    # Does not impact the actual prority of the transfer - is read by placement algorithm not fts3.
+    # Does not impact the actual priority of the transfer - is read by placement algorithm not fts3.
     assert request_fast['state'] != RequestState.SUBMISSION_FAILED
     assert request_slow['state'] != RequestState.SUBMISSION_FAILED
     assert request_fast['state'] != RequestState.FAILED
     assert request_slow['state'] != RequestState.FAILED
 
 
 @skip_rse_tests_with_accounts
```

### Comparing `rucio_clients-34.2.0/tests/test_conveyor_submitter.py` & `rucio_clients-34.3.0/tests/test_conveyor_submitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from datetime import datetime, timedelta
 from random import randint
 from unittest.mock import patch
 
 import pytest
 from sqlalchemy import delete
 
+from rucio.common.constants import RseAttr
 from rucio.common.exception import RequestNotFound
 from rucio.core import config as core_config
 from rucio.core import distance as distance_core
 from rucio.core import replica as replica_core
 from rucio.core import request as request_core
 from rucio.core import rse as rse_core
 from rucio.core import rule as rule_core
@@ -141,23 +142,23 @@
     all_rses = jump_rses + [src_rse_id, dst_rse_id]
 
     rse_tombstone_delay = 3600
     rse_multihop_tombstone_delay = 12 * 3600
     default_multihop_tombstone_delay = 24 * 3600
 
     # if both attributes are set, the multihop one will take precedence
-    rse_core.add_rse_attribute(jump_rse1_id, 'tombstone_delay', rse_tombstone_delay)
-    rse_core.add_rse_attribute(jump_rse1_id, 'multihop_tombstone_delay', rse_multihop_tombstone_delay)
+    rse_core.add_rse_attribute(jump_rse1_id, RseAttr.TOMBSTONE_DELAY, rse_tombstone_delay)
+    rse_core.add_rse_attribute(jump_rse1_id, RseAttr.MULTIHOP_TOMBSTONE_DELAY, rse_multihop_tombstone_delay)
 
     # if multihop delay not set, it's the default multihop takes precedence. Not normal tombstone delay.
-    rse_core.add_rse_attribute(jump_rse2_id, 'tombstone_delay', rse_tombstone_delay)
+    rse_core.add_rse_attribute(jump_rse2_id, RseAttr.TOMBSTONE_DELAY, rse_tombstone_delay)
     core_config.set(section='transfers', option='multihop_tombstone_delay', value=default_multihop_tombstone_delay)
 
     # if multihop delay is set to 0, the replica will have no tombstone
-    rse_core.add_rse_attribute(jump_rse3_id, 'multihop_tombstone_delay', 0)
+    rse_core.add_rse_attribute(jump_rse3_id, RseAttr.MULTIHOP_TOMBSTONE_DELAY, 0)
 
     distance_core.add_distance(src_rse_id, jump_rse1_id, distance=10)
     distance_core.add_distance(jump_rse1_id, jump_rse2_id, distance=10)
     distance_core.add_distance(jump_rse2_id, jump_rse3_id, distance=10)
     distance_core.add_distance(jump_rse3_id, dst_rse_id, distance=10)
 
     did = did_factory.upload_test_file(src_rse_name)
@@ -350,15 +351,15 @@
     rse3, rse3_id = rse_factory.make_posix_rse()
     rse4, rse4_id = rse_factory.make_posix_rse()
     all_rses = [rse1_id, rse2_id, rse3_id, rse4_id]
 
     distance_core.add_distance(rse1_id, rse2_id, distance=10)
     distance_core.add_distance(rse3_id, rse4_id, distance=10)
     for rse_id in all_rses:
-        rse_core.add_rse_attribute(rse_id, 'globus_endpoint_id', rse_id)
+        rse_core.add_rse_attribute(rse_id, RseAttr.GLOBUS_ENDPOINT_ID, rse_id)
 
     # Single submission
     did1 = did_factory.upload_test_file(rse1)
     rule_core.add_rule(dids=[did1], account=root_account, copies=1, rse_expression=rse2, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
     did2 = did_factory.upload_test_file(rse3)
     rule_core.add_rule(dids=[did2], account=root_account, copies=1, rse_expression=rse4, grouping='ALL', weight=None, lifetime=None, locked=False, subscription_id=None)
     with patch('rucio.transfertool.globus.bulk_submit_xfer') as mock_bulk_submit:
```

### Comparing `rucio_clients-34.2.0/tests/test_counter.py` & `rucio_clients-34.3.0/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_credential.py` & `rucio_clients-34.3.0/tests/test_credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 import pytest
 
+from rucio.common.constants import RseAttr
 from rucio.common.exception import UnsupportedOperation
 from rucio.core.credential import get_signed_url
 from rucio.core.replica import add_replicas
 from rucio.core.rse import add_protocol, add_rse_attribute
 
 
 class TestCredential:
@@ -103,15 +104,15 @@
                      account=root_account,
                      ignore_availability=True)
         add_replicas(rse_id=self.rse2_id,
                      files=files,
                      account=root_account,
                      ignore_availability=True)
 
-        add_rse_attribute(rse_id=self.rse1_id, key='sign_url', value='gcs')
+        add_rse_attribute(rse_id=self.rse1_id, key=RseAttr.SIGN_URL, value='gcs')
         replicas = [r for r in replica_client.list_replicas(dids=[{'scope': 'mock',
                                                                    'name': f['name'],
                                                                    'type': 'FILE'} for f in files],
                                                             rse_expression=self.rse1)]
         found_pfns = [list(replica['pfns'].keys())[0] for replica in replicas]
         for pfn in found_pfns:
             assert '&Signature=' in pfn
```

### Comparing `rucio_clients-34.2.0/tests/test_curl.py` & `rucio_clients-34.3.0/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_daemons.py` & `rucio_clients-34.3.0/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_dataset_replicas.py` & `rucio_clients-34.3.0/tests/test_dataset_replicas.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.exc import NoResultFound
 
 from rucio.client.didclient import DIDClient
 from rucio.client.replicaclient import ReplicaClient
 from rucio.client.ruleclient import RuleClient
 from rucio.common.exception import InvalidObject
 from rucio.common.schema import get_schema_value
 from rucio.core.did import add_dids, attach_dids
```

### Comparing `rucio_clients-34.2.0/tests/test_db.py` & `rucio_clients-34.3.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_did.py` & `rucio_clients-34.3.0/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_did_meta_plugins.py` & `rucio_clients-34.3.0/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_didtype.py` & `rucio_clients-34.3.0/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_download.py` & `rucio_clients-34.3.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_dumper.py` & `rucio_clients-34.3.0/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_dumper_consistency.py` & `rucio_clients-34.3.0/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_dumper_data_model.py` & `rucio_clients-34.3.0/tests/test_dumper_data_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         assert self.data_concrete[0] == 'aa'
 
     def test_csv_header(self):
         """ test csv header """
         assert self._DataConcrete.csv_header() == 'a,b,c,d,e,f,g,h'
 
     def test_formated_fields(self):
-        """ test formated fields """
+        """ test formatted fields """
         assert self.data_concrete.formated_fields(print_fields=('a', 'e')) == ['aa', '42']
 
     def test_csv(self):
         """ test csv """
         assert self.data_concrete.csv(fields=('a', 'e')) == 'aa,42'
 
     def test_csv_default_formatting(self):
@@ -215,15 +215,15 @@
             )
 
 
 class TestCompleteDataset:
 
     @staticmethod
     def test_creation_with_7_parameters():
-        """ test ceation with 7 parameters """
+        """ test creation with 7 parameters """
         complete_dataset = data_models.CompleteDataset(
             'RSE',
             'scope',
             'name',
             'owner',
             '42',
             '2015-01-01 23:00:00',
```

### Comparing `rucio_clients-34.2.0/tests/test_dumper_path_parsing.py` & `rucio_clients-34.3.0/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_filter_engine.py` & `rucio_clients-34.3.0/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_heartbeat.py` & `rucio_clients-34.3.0/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_hermes.py` & `rucio_clients-34.3.0/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_identity.py` & `rucio_clients-34.3.0/tests/test_identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     # normal addition
     headers_dict = {'X-Rucio-Username': username, 'X-Rucio-Password': 'secret', 'X-Rucio-Email': 'email'}
     response = rest_client.put('/identities/root/userpass', headers=headers(auth(auth_token), hdrdict(headers_dict)))
     assert response.status_code == 201
 
 
 def test_verify_userpass_identity():
-    """ Test if an idenity exists in the db, mapping to at least one account. """
+    """ Test if an identity exists in the db, mapping to at least one account. """
     if config_get_bool('common', 'multi_vo', raise_exception=False, default=False):
         vo = {'vo': get_vo()}
     else:
         vo = {}
     account_name = account_name_generator()
     account = InternalAccount(account_name, **vo)
     username = ''.join(random.choice(string.ascii_letters) for i in range(10))
@@ -103,15 +103,15 @@
 
     del_account_identity(username, IdentityType.USERPASS, account)
     del_identity(username, IdentityType.USERPASS)
     del_account(account)
 
 
 def test_verify_x509_identity():
-    """ Test if an x509 idenity exists in the db, mapped to at least one account. """
+    """ Test if an x509 identity exists in the db, mapped to at least one account. """
     if config_get_bool('common', 'multi_vo', raise_exception=False, default=False):
         vo = {'vo': get_vo()}
     else:
         vo = {}
     account_name = account_name_generator()
     account = InternalAccount(account_name, **vo)
     dn = rfc2253_dn_generator()
```

### Comparing `rucio_clients-34.2.0/tests/test_impl_upload_download.py` & `rucio_clients-34.3.0/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_import_export.py` & `rucio_clients-34.3.0/tests/test_import_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from copy import deepcopy
 
 import pytest
 
 from rucio.client.exportclient import ExportClient
 from rucio.client.importclient import ImportClient
 from rucio.common.config import config_add_section, config_has_section, config_set
+from rucio.common.constants import RseAttr
 from rucio.common.exception import RSENotFound
 from rucio.common.types import InternalAccount
 from rucio.common.utils import parse_response, render_json
 from rucio.core.account import add_account, get_account
 from rucio.core.distance import add_distance, get_distances
 from rucio.core.exporter import export_data, export_rses
 from rucio.core.identity import add_account_identity, add_identity, list_accounts_for_identity, list_identities
@@ -52,16 +53,16 @@
     assert rse['availability_write'] == test_data[rse_name]['availability_write']
     assert rse['availability_delete'] == test_data[rse_name]['availability_delete']
 
 
 def check_protocols(rse, test_data, vo='def'):
     rse_id = get_rse_id(rse=rse, vo=vo)
     protocols = get_rse_protocols(rse_id)
-    assert test_data[rse]['lfn2pfn_algorithm'] == get_rse_attribute(rse_id, 'lfn2pfn_algorithm', use_cache=False)
-    assert test_data[rse]['verify_checksum'] == get_rse_attribute(rse_id, 'verify_checksum', use_cache=False)
+    assert test_data[rse]['lfn2pfn_algorithm'] == get_rse_attribute(rse_id, RseAttr.LFN2PFN_ALGORITHM, use_cache=False)
+    assert test_data[rse]['verify_checksum'] == get_rse_attribute(rse_id, RseAttr.VERIFY_CHECKSUM, use_cache=False)
     assert test_data[rse]['availability_write'] == protocols['availability_write']
     assert test_data[rse]['availability_read'] == protocols['availability_read']
     assert test_data[rse]['availability_delete'] == protocols['availability_delete']
     protocols = [{'hostname': protocol['hostname'], 'scheme': protocol['scheme'], 'port': protocol['port'], 'impl': protocol['impl'], 'prefix': protocol['prefix']} for protocol in protocols['protocols']]
     for protocol in test_data[rse]['protocols']:
         assert {'hostname': protocol['hostname'], 'scheme': protocol['scheme'], 'port': protocol['port'], 'impl': protocol.get('impl', ''), 'prefix': protocol.get('prefix', '')} in protocols
 
@@ -145,16 +146,16 @@
     example_data.old_rse_id_1 = add_rse(example_data.old_rse_1, availability_read=False, availability_write=False, region_code='DE', country_name='DE',
                                         deterministic=True, volatile=True, staging_area=True, time_zone='Europe', latitude='1', longitude='2', vo=vo)
     add_protocol(example_data.old_rse_id_1, {'scheme': 'scheme1', 'hostname': 'hostname1', 'port': 1000, 'impl': 'TODO'})
     add_protocol(example_data.old_rse_id_1, {'scheme': 'scheme3', 'hostname': 'hostname3', 'port': 1000, 'impl': 'TODO'})
 
     set_rse_limits(rse_id=example_data.old_rse_id_1, name='MinFreeSpace', value='10')
     add_rse_attribute(rse_id=example_data.old_rse_id_1, key='attr1', value='test10')
-    add_rse_attribute(rse_id=example_data.old_rse_id_1, key='lfn2pfn_algorithm', value='test10')
-    add_rse_attribute(rse_id=example_data.old_rse_id_1, key='verify_checksum', value=True)
+    add_rse_attribute(rse_id=example_data.old_rse_id_1, key=RseAttr.LFN2PFN_ALGORITHM, value='test10')
+    add_rse_attribute(rse_id=example_data.old_rse_id_1, key=RseAttr.VERIFY_CHECKSUM, value=True)
 
     # RSE 2 that already exists
     example_data.old_rse_2 = rse_name_generator()
     example_data.old_rse_id_2 = add_rse(example_data.old_rse_2, vo=vo)
 
     # RSE 3 that already exists
     example_data.old_rse_3 = rse_name_generator()
@@ -176,15 +177,15 @@
     add_account(example_data.old_account_2, AccountType.USER, email='test')
 
     # Identity that should be removed
     example_data.identity_to_be_removed = rse_name_generator()
     add_identity(example_data.identity_to_be_removed, IdentityType.X509, email='email')
     add_account_identity(example_data.identity_to_be_removed, IdentityType.X509, example_data.old_account_2, 'email')
 
-    # Identity that already exsits but should be added to the account
+    # Identity that already exists but should be added to the account
     example_data.identity_to_be_added_to_account = rse_name_generator()
     add_identity(example_data.identity_to_be_added_to_account, IdentityType.X509, email='email')
 
     example_data.data1 = {
         'rses': {
             example_data.new_rse: {
                 'rse_type': RSEType.TAPE,
```

### Comparing `rucio_clients-34.2.0/tests/test_judge_cleaner.py` & `rucio_clients-34.3.0/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_judge_evaluator.py` & `rucio_clients-34.3.0/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_judge_injector.py` & `rucio_clients-34.3.0/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_judge_repairer.py` & `rucio_clients-34.3.0/tests/test_judge_repairer.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         transfs = cancel_request_did(scope=scope, name=files[3]['name'], dest_rse_id=get_replica_locks(scope=files[3]['scope'], name=files[2]['name'])[0].rse_id)
         cancel_transfers(transfs)
 
         assert (rule_id == get_rule(rule_id)['id'].replace('-', '').lower())
         assert (RuleState.STUCK == get_rule(rule_id)['state'])
         rule_repairer(once=True)
 
-        # Stil assert STUCK because of delays:
+        # Still assert STUCK because of delays:
         assert (RuleState.STUCK == get_rule(rule_id)['state'])
         assert (get_replica_locks(scope=files[2]['scope'], name=files[2]['name'])[0].rse_id == get_replica_locks(scope=files[3]['scope'], name=files[3]['name'])[0].rse_id)
         # assert (RuleState.REPLICATING == get_rule(rule_id)['state'])
         # assert (get_replica_locks(scope=files[2]['scope'], name=files[2]['name'])[0].rse_id == get_replica_locks(scope=files[3]['scope'], name=files[3]['name'])[0].rse_id)
 
     def test_to_repair_a_rule_with_NONE_grouping_whose_transfer_failed_and_flipping_to_other_rse(self):
         """ JUDGE REPAIRER: Test to repair a rule with 1 failed transfer and flip to other rse(lock)"""
```

### Comparing `rucio_clients-34.2.0/tests/test_lifetime.py` & `rucio_clients-34.3.0/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_message.py` & `rucio_clients-34.3.0/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_meta_conventions.py` & `rucio_clients-34.3.0/tests/test_meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_meta_did.py` & `rucio_clients-34.3.0/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_module_import.py` & `rucio_clients-34.3.0/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_monitor.py` & `rucio_clients-34.3.0/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_multi_vo.py` & `rucio_clients-34.3.0/tests/test_multi_vo.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from rucio.api.subscription import add_subscription, list_subscriptions
 from rucio.client.accountlimitclient import AccountLimitClient
 from rucio.client.client import Client
 from rucio.client.replicaclient import ReplicaClient
 from rucio.client.subscriptionclient import SubscriptionClient
 from rucio.client.uploadclient import UploadClient
 from rucio.common.config import config_add_section, config_has_section, config_remove_option, config_set
+from rucio.common.constants import RseAttr
 from rucio.common.exception import AccessDenied, Duplicate, InvalidRSEExpression, RucioException, UnsupportedAccountName, UnsupportedOperation
 from rucio.common.types import InternalAccount
 from rucio.common.utils import generate_uuid, get_tmp_dir, parse_response, ssh_sign
 from rucio.core import config as core_config
 from rucio.core.account_counter import add_counter
 from rucio.core.replica import add_replica
 from rucio.core.rse import get_rse_id, get_rse_vo, get_rses_with_attribute_value
@@ -628,15 +629,15 @@
         # We get all the account names with the long VO name and short VO name and check they are equal
         accounts_long = get_vo_accounts(long_vo)
         accounts_short = get_vo_accounts(vo)
         assert len(accounts_short) > 0
         assert accounts_short == accounts_long
 
     def test_rest_vomap_bad(self, rest_client):
-        """ MULTI VO (REST): Test that we get a bad paramter (400) error with an invalid (out of spec) VO name. """
+        """ MULTI VO (REST): Test that we get a bad parameter (400) error with an invalid (out of spec) VO name. """
         # VO names cannot include an exclaimation mark
         response = rest_client.get('/auth/userpass', headers=headers(loginhdr('root', 'ddmlab', 'secret'), vohdr("BadVO!")))
         assert response.status_code == 400
 
 
 class TestMultiVoClients:
 
@@ -1003,20 +1004,20 @@
                              'lan': {'read': 1,
                                      'write': 1,
                                      'delete': 1},
                              'wan': {'read': 1,
                                      'write': 1,
                                      'delete': 1}}}
         rse_client.add_rse(shr_rse)
-        rse_client.add_rse_attribute(rse=shr_rse, key='verify_checksum', value=False)
-        rse_client.add_rse_attribute(rse=shr_rse, key='skip_upload_stat', value=True)
+        rse_client.add_rse_attribute(rse=shr_rse, key=RseAttr.VERIFY_CHECKSUM, value=False)
+        rse_client.add_rse_attribute(rse=shr_rse, key=RseAttr.SKIP_UPLOAD_STAT, value=True)
         rse_client.add_protocol(shr_rse, mock_protocol)
         add_rse(shr_rse, 'root', vo=second_vo)
-        add_rse_attribute(rse=shr_rse, key='verify_checksum', value=False, issuer='root', vo=second_vo)
-        add_rse_attribute(rse=shr_rse, key='skip_upload_stat', value=True, issuer='root', vo=second_vo)
+        add_rse_attribute(rse=shr_rse, key=RseAttr.VERIFY_CHECKSUM, value=False, issuer='root', vo=second_vo)
+        add_rse_attribute(rse=shr_rse, key=RseAttr.SKIP_UPLOAD_STAT, value=True, issuer='root', vo=second_vo)
         add_protocol(rse=shr_rse, data=mock_protocol, issuer='root', vo=second_vo)
 
         if not config_has_section("automatix"):
             config_add_section("automatix")
         config_set("automatix", "rses", shr_rse)
         config_set("automatix", "scope", shr_scope)
```

### Comparing `rucio_clients-34.2.0/tests/test_naming_convention.py` & `rucio_clients-34.3.0/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_oauthmanager.py` & `rucio_clients-34.3.0/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_oidc.py` & `rucio_clients-34.3.0/tests/test_oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 
     @classmethod
     def do_any(cls, request=None, request_args=None, response=None):
         oidc_tokens = EXCHANGED_TOKEN_DICT.copy()
         oidc_tokens['scope'] = request_args['scope']
         oidc_tokens['audience'] = request_args['audience']
         oidc_tokens['id_token'] = {'sub': request_args['client_id'], 'iss': 'https://test_issuer/'}
-        # we need to passs the full dict in the access_token key again in order to have  a chance to bypas the token validation method
+        # we need to pass the full dict in the access_token key again in order to have  a chance to bypass the token validation method
         access_token = encode_access_token([oidc_tokens['access_token'], oidc_tokens['scope'],
                                            oidc_tokens['audience'], request_args['client_id'], 'https://test_issuer/'])
         oidc_tokens['access_token'] = access_token
         return oidc_tokens
 
     @classmethod
     def construct_AuthorizationRequest(cls, request_args=None):
@@ -219,15 +219,15 @@
         oidc_tokens = EXCHANGED_TOKEN_DICT.copy()
         oidc_token_dict = dencode_access_token(request_args['subject_token'])
         user_sub = oidc_token_dict['identity'].split(',')[0].split('=')[1]
         user_issuer = oidc_token_dict['identity'].split(',')[1].split('=')[1]
         oidc_tokens['scope'] = request_args['scope']
         oidc_tokens['audience'] = request_args['audience']
         oidc_tokens['id_token'] = {'sub': user_sub, 'iss': user_issuer}
-        # we need to passs the full dict in the access_token key again in order to have  a chance to bypas the token validation method
+        # we need to pass the full dict in the access_token key again in order to have  a chance to bypass the token validation method
         access_token = encode_access_token([oidc_tokens['access_token'], oidc_tokens['scope'],
                                            oidc_tokens['audience'], user_sub, user_issuer])
         oidc_tokens['access_token'] = access_token
         return MockResponse(oidc_tokens)
 
 
 class MockADMINClientOtherISSOIDC(MagicMock):
@@ -236,15 +236,15 @@
 
     @classmethod
     def do_any(cls, request=None, request_args=None, response=None):
         oidc_tokens = EXCHANGED_TOKEN_DICT.copy()
         oidc_tokens['scope'] = request_args['scope']
         oidc_tokens['audience'] = request_args['audience']
         oidc_tokens['id_token'] = {'sub': request_args['client_id'], 'iss': 'https://test_other_issuer/'}
-        # we need to passs the full dict in the access_token key again in order to have  a chance to bypas the token validation method
+        # we need to pass the full dict in the access_token key again in order to have  a chance to bypass the token validation method
         access_token = encode_access_token([oidc_tokens['access_token'], oidc_tokens['scope'],
                                            oidc_tokens['audience'], request_args['client_id'], 'https://test_other_issuer/'])
         oidc_tokens['access_token'] = access_token
         return oidc_tokens
 
     @classmethod
     def construct_AuthorizationRequest(cls, request_args=None):
@@ -274,15 +274,15 @@
             self.vo = {}
 
         self.db_session = get_session()
         self.accountstring = 'test_' + rndstr()
         self.accountstring = self.accountstring.lower()
         self.account = InternalAccount(self.accountstring, **self.vo)
         self.adminaccountstring = 'admin_' + rndstr()[:-1]  # Too long to use full string
-        print("ADMIN ACOUNT STRING: ", self.adminaccountstring)
+        print("ADMIN ACCOUNT STRING: ", self.adminaccountstring)
         self.adminaccountstring = self.adminaccountstring.lower()
         self.adminaccount = InternalAccount(self.adminaccountstring, **self.vo)
         self.adminaccSUB = str('adminSUB' + rndstr()).lower()
         self.adminaccSUB_otherISS = str('adminSUB_otherISS' + rndstr()).lower()
         self.adminClientSUB = str('adminclientSUB' + rndstr()).lower()
         self.adminClientSUB_otherISS = str('adminclientSUB_otherISS' + rndstr()).lower()
         try:
@@ -327,15 +327,15 @@
             'refresh_lifetime': 96,
             'ip': None,
             'webhome': 'https://rucio-test.cern.ch/ui',
         }
         auth_url = get_auth_oidc(account, session=session, **kwargs)
         print("[get_auth_init_and_mock_response] got auth_url:", auth_url)
         # get the state from the auth_url and add an arbitrary code value to the query string
-        # to mimick a return of IdP with authz_code
+        # to mimic a return of IdP with authz_code
         urlparsed = urlparse(auth_url)
         if ('_polling' in auth_url) or (not polling and not auto):
             auth_url = redirect_auth_oidc(urlparsed.query, session=session)
             print("[get_auth_init_and_mock_response] got redirect auth_url:", auth_url)
             urlparsed = urlparse(auth_url)
         urlparams = parse_qs(urlparsed.query)
         assert 'state' in urlparams
@@ -399,15 +399,15 @@
             print(traceback.format_exc())
 
     def test_get_token_oidc_unknown_state(self):
         """ OIDC Token request with unknown state from IdP
 
             Runs the Test:
 
-            - requesting token with parameters without coresponding
+            - requesting token with parameters without corresponding
               DB entry (in oauth_Requests table)
 
             End:
 
             - checking the relevant exception to be thrown
         """
         try:
@@ -562,15 +562,15 @@
               and with it the corresponding entry in the oauth_requests table
             - filling the right identity into the token (mocking the IdP response)
             - calling the get_token_oidc core function
 
             End:
 
             - checking if the right token is saved in the DB and if it is present
-              in the return dict of the get_token_oidc fucntion
+              in the return dict of the get_token_oidc function
         """
         mock_oidc_client.side_effect = get_mock_oidc_client
         auth_init_response = self.get_auth_init_and_mock_response(code_response=rndstr(), account=InternalAccount('webui', **self.vo), session=self.db_session)
         oauth_session_row = get_oauth_session_row(InternalAccount('webui', **self.vo), state=auth_init_response['state'], session=self.db_session)
         assert oauth_session_row
         # mocking the token response
         access_token = rndstr()
@@ -1699,15 +1699,15 @@
         req_audience = 'transfer_audience_' + rndstr() + ' some_other_audience' + rndstr()
         req_account = self.account
         final_token_account = self.account
         final_token_issuer = 'https://test_issuer/'
         user_sub = 'knownsub'
         req_admin = False
         # ---------------------------
-        # giving a USER a subject token - ned to bypass the usual auth grant flow
+        # giving a USER a subject token - need to bypass the usual auth grant flow
         # as that is not the purpose of this test
         preexisting_user_access_token_strpart = rndstr()
         request_args = {'scope': EXPECTED_OIDC_SCOPE,
                         'audience': EXPECTED_OIDC_AUDIENCE,
                         'client_id': user_sub,
                         'issuer': final_token_issuer,
                         'account': final_token_account,
@@ -1786,15 +1786,15 @@
         req_audience = 'transfer_audience_' + rndstr() + ' some_other_audience' + rndstr()
         req_account = self.account
         final_token_account = self.account
         final_token_issuer = 'https://test_issuer/'
         user_sub = 'knownsub'
         req_admin = False
         # ---------------------------
-        # giving a USER a subject token - ned to bypass the usual auth grant flow
+        # giving a USER a subject token - need to bypass the usual auth grant flow
         # as that is not the purpose of this test
         preexisting_user_access_token_strpart = rndstr()
         request_args = {'scope': EXPECTED_OIDC_SCOPE,
                         'audience': EXPECTED_OIDC_AUDIENCE,
                         'client_id': user_sub,
                         'issuer': final_token_issuer,
                         'account': final_token_account,
```

### Comparing `rucio_clients-34.2.0/tests/test_permission.py` & `rucio_clients-34.3.0/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_pfns.py` & `rucio_clients-34.3.0/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_ping.py` & `rucio_clients-34.3.0/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_preparer.py` & `rucio_clients-34.3.0/tests/test_preparer.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import pytest
 
+from rucio.common.constants import RseAttr
 from rucio.core.distance import add_distance, get_distances
 from rucio.core.replica import add_replicas
 from rucio.core.request import get_request, list_and_mark_transfer_requests_and_source_replicas, list_transfer_limits, set_transfer_limit
 from rucio.core.rse import RseCollection, RseData, add_rse_attribute
 from rucio.core.transfer import get_supported_transfertools
 from rucio.daemons.conveyor.preparer import preparer
 from rucio.db.sqla import models
@@ -146,16 +147,16 @@
 
 
 @pytest.mark.noparallel(reason='uses preparer')
 @pytest.mark.parametrize("caches_mock", [{"caches_to_mock": [
     'rucio.core.rse.REGION'
 ]}], indirect=True)
 def test_preparer_without_and_with_mat(source_rse, dest_rse, mock_request, caches_mock):
-    add_rse_attribute(source_rse['id'], 'fts', 'a')
-    add_rse_attribute(dest_rse['id'], 'globus_endpoint_id', 'b')
+    add_rse_attribute(source_rse['id'], RseAttr.FTS, 'a')
+    add_rse_attribute(dest_rse['id'], RseAttr.GLOBUS_ENDPOINT_ID, 'b')
 
     [cache_region] = caches_mock
     cache_region.invalidate()
 
     preparer(once=True, transfertools=['fts3', 'globus'], partition_wait_time=0)
 
     updated_mock_request = get_request(mock_request['id'])
@@ -196,17 +197,17 @@
     assert not transfertools
 
 
 def test_get_supported_transfertools_fts_globus(vo, rse_factory):
     source_rse, source_rse_id = rse_factory.make_mock_rse()
     dest_rse, dest_rse_id = rse_factory.make_mock_rse()
 
-    add_rse_attribute(source_rse_id, 'fts', 'a')
-    add_rse_attribute(dest_rse_id, 'fts', 'b')
-    add_rse_attribute(source_rse_id, 'globus_endpoint_id', 'a')
-    add_rse_attribute(dest_rse_id, 'globus_endpoint_id', 'b')
+    add_rse_attribute(source_rse_id, RseAttr.FTS, 'a')
+    add_rse_attribute(dest_rse_id, RseAttr.FTS, 'b')
+    add_rse_attribute(source_rse_id, RseAttr.GLOBUS_ENDPOINT_ID, 'a')
+    add_rse_attribute(dest_rse_id, RseAttr.GLOBUS_ENDPOINT_ID, 'b')
 
     transfertools = get_supported_transfertools(source_rse=RseData(source_rse_id), dest_rse=RseData(dest_rse_id), transfertools=['fts3', 'globus'])
 
     assert len(transfertools) == 2
     assert 'fts3' in transfertools
     assert 'globus' in transfertools
```

### Comparing `rucio_clients-34.2.0/tests/test_qos.py` & `rucio_clients-34.3.0/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_quarantined_replica.py` & `rucio_clients-34.3.0/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_reaper.py` & `rucio_clients-34.3.0/tests/test_reaper.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
     assert len(deleted_dids) == len(dids)
 
 
 @pytest.mark.parametrize("caches_mock", [{"caches_to_mock": [
     'rucio.daemons.reaper.reaper.REGION'
 ]}], indirect=True)
 def test_run_on_non_existing_scheme(vo, caches_mock):
-    """ REAPER (DAEMON): Mock test the reaper daemon with a speficied scheme."""
+    """ REAPER (DAEMON): Mock test the reaper daemon with a specified scheme."""
     [cache_region] = caches_mock
     scope = InternalScope('data13_hip', vo=vo)
 
     nb_files = 250
     file_size = 200  # 2G
     rse_name, rse_id, dids = __add_test_rse_and_replicas(vo=vo, scope=scope, rse_name=rse_name_generator(),
                                                          names=['lfn' + generate_uuid() for _ in range(nb_files)], file_size=file_size)
```

### Comparing `rucio_clients-34.2.0/tests/test_redirect.py` & `rucio_clients-34.3.0/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_replica.py` & `rucio_clients-34.3.0/tests/test_replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from xml.etree import ElementTree
 
 import pytest
 import xmltodict
 from werkzeug.datastructures import Headers, MultiDict
 
 from rucio.client.ruleclient import RuleClient
+from rucio.common.constants import RseAttr
 from rucio.common.exception import AccessDenied, DatabaseException, DataIdentifierNotFound, InputValidationError, ReplicaIsLocked, ReplicaNotFound, RucioException, ScopeNotFound
 from rucio.common.schema import get_schema_value
 from rucio.common.utils import clean_surls, generate_uuid, parse_response
 from rucio.core.config import set as cconfig_set
 from rucio.core.did import add_did, attach_dids, get_did, get_did_atime, list_files, set_status
 from rucio.core.replica import add_bad_dids, add_replica, add_replicas, delete_replicas, get_bad_pfns, get_replica, get_replica_atime, get_replicas_state, get_RSEcoverage_of_dataset, list_replicas, set_tombstone, touch_replica, update_replica_state
 from rucio.core.rse import add_protocol, add_rse_attribute, del_rse_attribute
@@ -213,15 +214,15 @@
         # bear in mind that if a bad value is entered as rse_attribute, the default value is 1
         simulate_multirange, nconns, expectedconns = params
 
         _, rse_id = rse_factory.make_mock_rse()
 
         if simulate_multirange:
             add_rse_attribute(
-                rse_id=rse_id, key='simulate_multirange', value=str(nconns)
+                rse_id=rse_id, key=RseAttr.SIMULATE_MULTIRANGE, value=str(nconns)
             )
 
         # add files
         file_name = did_name_generator('testfiles')
         add_replica(rse_id, mock_scope, file_name, 2, root_account)
 
         dids = [{'scope': mock_scope, 'name': file_name, 'type': DIDType.FILE}]
@@ -452,26 +453,26 @@
                               'port': 1409,
                               'prefix': '//test/chamber/',
                               'impl': 'rucio.rse.protocols.xrootd.Default',
                               'domains': {
                                   'lan': {'read': 1, 'write': 1, 'delete': 1},
                                   'wan': {'read': 1, 'write': 1, 'delete': 1}}})
 
-        add_rse_attribute(rse_id=rse_id, key='site', value='APERTURE')
+        add_rse_attribute(rse_id=rse_id, key=RseAttr.SITE, value='APERTURE')
 
         files = [{'scope': mock_scope, 'name': 'element_%s' % generate_uuid(),
                   'bytes': 1234, 'adler32': 'deadbeef'}]
         add_replicas(rse_id=rse_id, files=files, account=root_account)
 
         replicas = [r for r in replica_client.list_replicas(dids=[{'scope': 'mock', 'name': f['name']} for f in files])]
         assert 'root://' in list(replicas[0]['pfns'].keys())[0]
         replicas = [r for r in replica_client.list_replicas(dids=[{'scope': 'mock', 'name': f['name']} for f in files],
                                                             client_location={'site': 'SOMEWHERE'})]
         assert 'root://' in list(replicas[0]['pfns'].keys())[0]
-        del_rse_attribute(rse_id=rse_id, key='site')
+        del_rse_attribute(rse_id=rse_id, key=RseAttr.SITE)
 
         replicas = [r for r in replica_client.list_replicas(dids=[{'scope': 'mock', 'name': f['name']} for f in files])]
         assert 'root://' in list(replicas[0]['pfns'].keys())[0]
         replicas = [r for r in replica_client.list_replicas(dids=[{'scope': 'mock', 'name': f['name']} for f in files],
                                                             client_location={'site': 'SOMEWHERE'})]
         assert 'root://' in list(replicas[0]['pfns'].keys())[0]
 
@@ -539,15 +540,15 @@
         """ REPLICA (CORE): Per-RSE default tombstone is correctly taken into consideration"""
 
         # One RSE has an attribute set, the other uses the default value of "None" for tombstone
         rse1, rse1_id = rse_factory.make_mock_rse()
         rse2, rse2_id = rse_factory.make_mock_rse()
         activity = get_schema_value('ACTIVITY')['enum'][0]
         tombstone_delay = 3600
-        add_rse_attribute(rse_id=rse2_id, key='tombstone_delay', value=tombstone_delay)
+        add_rse_attribute(rse_id=rse2_id, key=RseAttr.TOMBSTONE_DELAY, value=tombstone_delay)
 
         # Will use the default tombstone delay
         did1 = did_factory.random_file_did()
         add_replica(rse1_id, bytes_=4, account=root_account, **did1)
         assert get_replica(rse1_id, **did1)['tombstone'] is None
 
         # Will use the configured value on the RSE
@@ -936,15 +937,15 @@
 
     rep = []
     for did in files:
         print(did)
         did['state'] = ReplicaState.TEMPORARY_UNAVAILABLE
         rep.append(did)
 
-    time.sleep(10)  # Test broken if minos_tu_expiration excuted immediately. Threading effect ?
+    time.sleep(10)  # Test broken if minos_tu_expiration executed immediately. Threading effect ?
     # Run the minos expiration
     minos_tu_expiration(once=True)
     # Check the state in the replica table
     for did in files:
         rep = get_replicas_state(scope=mock_scope, name=did['name'])
         print(rep)
         assert list(rep.keys())[0] == ReplicaState.AVAILABLE
```

### Comparing `rucio_clients-34.2.0/tests/test_replica_recoverer.py` & `rucio_clients-34.3.0/tests/test_replica_recoverer.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,16 @@
             # Upload files with scope "scope_nopolicy"
             cmd = 'rucio -v upload --rse {0} --scope {1} {2}'.format(rse, self.scope_ignore.external, self.tmp_file10)
             exitcode, out, err = execute(cmd)
             print("scope_ignore:", exitcode, out, err)
             # checking if Rucio upload went OK
             assert exitcode == 0
 
-        # Explaination of the fictional data types:
-        # testtypedeclarebad: Files are speficied to be declared bad
+        # Explanation of the fictional data types:
+        # testtypedeclarebad: Files are specified to be declared bad
         # testtypeignore: Files are specified to be ignored
         # testtypenopolicy: Files either have no policy or no recognised policy and are ignored by default
 
         # Set fictional datatypes
         set_metadata(mock_scope, self.tmp_file3.name, 'datatype', 'RAW')
         set_metadata(mock_scope, self.tmp_file4.name, 'datatype', 'testtypedeclarebad')
         set_metadata(mock_scope, self.tmp_file5.name, 'datatype', 'testtypenopolicy')
@@ -387,24 +387,24 @@
         # tmp_file9    unavailable                              suspicious (available)                    scope_declarebad            testtypeignore
         # tmp_file10   unavailable                              suspicious (available)                    scope_ignore                testtypedeclarebad
         # tmp_file11   unavailable                              suspicious (available)                    scope_declarebad            <none>
         # tmp_file12   unavailable                              suspicious (available)                    mock_scope                  <none>
         # tmp_file13   unavailable                              suspicious (available)                    scope_declarebad            testtypedryrun
         # ----------------------------------------------------------------------------------------------------------------------------------------------------
 
-            - Explaination: Suspicious replicas that are the last remaining copy (unavailable on rse4recovery) are handeled differently depending
+            - Explanation: Suspicious replicas that are the last remaining copy (unavailable on rse4recovery) are handled differently depending
                             by their metadata "datatype".
                             - Files that are the last remaining copy, but do not have a data type, are automatically ignored. For this reason, testing
                               just the scope policies (tmp_file7 and tmp_file8) still requires a data type.
                             - RAW files have the poilcy to be ignored.
                             - testtypedeclarebad files are of a fictional type that has the policy of being declared bad.
                             - testtypenopolicy files are of a fictional type that doesn't have a specified policy, meaning they should be ignored by default.
                             - scope_declarebad files belong to a fictional scope that has the policy of being declared bad.
                             - scope_nopolicy files belong to a fictional scope that doesn't have a specified policy, meaning they should be ignored by default.
-                            If a policiy is set for the file type and the scope, then the policiy for the file type takes priority (meaning tmp_file9 should be
+                            If a policy is set for the file type and the scope, then the policy for the file type takes priority (meaning tmp_file9 should be
                             ignored).
 
             Runs the Test:
 
             - running suspicious_replica_recoverer
 
             Concluding:
```

### Comparing `rucio_clients-34.2.0/tests/test_replica_sorting.py` & `rucio_clients-34.3.0/tests/test_replica_sorting.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from unittest import mock
 from urllib.parse import urlparse
 
 import geoip2.database
 import pytest
 
 from rucio.common.config import config_get
+from rucio.common.constants import RseAttr
 from rucio.common.utils import parse_replicas_from_string
 from rucio.core import replica_sorter, rse_expression_parser
 from rucio.core.replica import add_replicas, delete_replicas
 from rucio.core.rse import add_protocol, add_rse, add_rse_attribute, del_rse, del_rse_attribute
 from rucio.tests.common import Mime, accept, auth, headers, rse_name_generator, vohdr
 
 from .inputs import GEOIP_LITE2_CITY_TEST_DB
@@ -104,15 +105,15 @@
     rse_info = copy.deepcopy(base_rse_info)
 
     files = [{'scope': mock_scope, 'name': 'element_0', 'bytes': 1234, 'adler32': 'deadbeef'}]
 
     for idx in range(len(rse_info)):
         rse_info[idx]['name'] = '%s_%s' % (rse_info[idx]['site'], rse_name_generator())
         rse_info[idx]['id'] = add_rse(rse_info[idx]['name'], vo=vo)
-        add_rse_attribute(rse_id=rse_info[idx]['id'], key='site', value=base_rse_info[idx]['site'])
+        add_rse_attribute(rse_id=rse_info[idx]['id'], key=RseAttr.SITE, value=base_rse_info[idx]['site'])
         add_replicas(rse_id=rse_info[idx]['id'], files=files, account=root_account)
 
     # invalidate cache for parse_expression('site=…')
     rse_expression_parser.REGION.invalidate()
 
     # check sites
     for idx in range(len(rse_info)):
@@ -170,15 +171,15 @@
                                          'lan': {'read': 1, 'write': 1, 'delete': 1},
                                          'wan': {'read': 3, 'write': 3, 'delete': 3}}})
 
     yield {'files': files, 'rse_info': rse_info}
 
     for info in rse_info:
         delete_replicas(rse_id=info['id'], files=files)
-        del_rse_attribute(rse_id=info['id'], key='site')
+        del_rse_attribute(rse_id=info['id'], key=RseAttr.SITE)
         del_rse(info['id'])
 
 
 @pytest.mark.noparallel(reason='fails when run in parallel, lists replicas and checks for length of returned list')
 @pytest.mark.parametrize("content_type", [Mime.METALINK, Mime.JSON_STREAM])
 @pytest.mark.parametrize("file_config_mock", [
     # Run test twice: with root proxy and without
```

### Comparing `rucio_clients-34.2.0/tests/test_request.py` & `rucio_clients-34.3.0/tests/test_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import json
 from datetime import datetime
 from typing import Union
 
 import pytest
 
 from rucio.common.config import config_get_bool
+from rucio.common.constants import RseAttr
 from rucio.common.utils import generate_uuid, parse_response
 from rucio.core.distance import add_distance
 from rucio.core.replica import add_replica
 from rucio.core.request import TransferStatsManager, get_request_by_did, list_requests, list_requests_history, queue_requests, set_transfer_limit
 from rucio.core.rse import add_rse_attribute
 from rucio.db.sqla import constants, models
 from rucio.db.sqla.constants import RequestState, RequestType
@@ -174,19 +175,19 @@
     source_rse3, source_rse_id3 = rse_factory.make_mock_rse(session=db_session)
     dest_rse, dest_rse_id = rse_factory.make_mock_rse(session=db_session)
     dest_rse2, dest_rse_id2 = rse_factory.make_mock_rse(session=db_session)
     source_site = tag_factory.new_tag()
     source_site2 = tag_factory.new_tag()
     dst_site = tag_factory.new_tag()
     dst_site2 = tag_factory.new_tag()
-    add_rse_attribute(source_rse_id, 'site', source_site, session=db_session)
-    add_rse_attribute(source_rse_id2, 'site', source_site2, session=db_session)
-    add_rse_attribute(source_rse_id3, 'site', source_site, session=db_session)
-    add_rse_attribute(dest_rse_id, 'site', dst_site, session=db_session)
-    add_rse_attribute(dest_rse_id2, 'site', dst_site2, session=db_session)
+    add_rse_attribute(source_rse_id, RseAttr.SITE, source_site, session=db_session)
+    add_rse_attribute(source_rse_id2, RseAttr.SITE, source_site2, session=db_session)
+    add_rse_attribute(source_rse_id3, RseAttr.SITE, source_site, session=db_session)
+    add_rse_attribute(dest_rse_id, RseAttr.SITE, dst_site, session=db_session)
+    add_rse_attribute(dest_rse_id2, RseAttr.SITE, dst_site2, session=db_session)
 
     name1 = generate_uuid()
     name2 = generate_uuid()
     name3 = generate_uuid()
     model(state=constants.RequestState.WAITING, source_rse_id=source_rse_id, dest_rse_id=dest_rse_id, name=name3).save(session=db_session)
     model(state=constants.RequestState.SUBMITTED, source_rse_id=source_rse_id2, dest_rse_id=dest_rse_id, name=name1).save(session=db_session)
     model(state=constants.RequestState.SUBMITTED, source_rse_id=source_rse_id, dest_rse_id=dest_rse_id2, name=name1).save(session=db_session)
```

### Comparing `rucio_clients-34.2.0/tests/test_root_proxy.py` & `rucio_clients-34.3.0/tests/test_root_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from urllib.parse import urlencode
 
 import pytest
 
+from rucio.common.constants import RseAttr
 from rucio.core.config import set as config_set
 from rucio.core.replica import add_replicas, delete_replicas
 from rucio.core.rse import add_protocol, add_rse, add_rse_attribute, del_rse
 from rucio.tests.common import headers, rse_name_generator, vohdr
 
 client_location_without_proxy = {'ip': '192.168.0.1',
                                  'fqdn': 'anomalous-materials.blackmesa.com',
@@ -31,21 +32,21 @@
 
 
 @pytest.fixture(scope='module', autouse=True)
 def root_proxy_example_data(vo, root_account, mock_scope):
     rse_without_proxy = rse_name_generator()
     rse_without_proxy_id = add_rse(rse_without_proxy, vo=vo)
     add_rse_attribute(rse_id=rse_without_proxy_id,
-                      key='site',
+                      key=RseAttr.SITE,
                       value='BLACKMESA1')
 
     rse_with_proxy = rse_name_generator()
     rse_with_proxy_id = add_rse(rse_with_proxy, vo=vo)
     add_rse_attribute(rse_id=rse_with_proxy_id,
-                      key='site',
+                      key=RseAttr.SITE,
                       value='APERTURE1')
 
     # APERTURE1 site has an internal proxy
     config_set('root-proxy-internal', 'APERTURE1', 'proxy.aperture.com:1094')
 
     files = [{'scope': mock_scope,
               'name': 'half-life_%s' % i,
```

### Comparing `rucio_clients-34.2.0/tests/test_rse.py` & `rucio_clients-34.3.0/tests/test_rse.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
 
 from rucio.client.replicaclient import ReplicaClient
 from rucio.common import exception
+from rucio.common.constants import RseAttr
 from rucio.common.exception import Duplicate, InputValidationError, InvalidObject, ResourceTemporaryUnavailable, RSEAttributeNotFound, RSENotFound, RSEOperationNotSupported, RSEProtocolNotSupported
 from rucio.common.schema import get_schema_value
 from rucio.common.utils import CHECKSUM_KEY, GLOBALLY_SUPPORTED_CHECKSUMS
 from rucio.core.account_limit import get_rse_account_usage, set_local_account_limit
 from rucio.core.did import add_did, attach_dids
 from rucio.core.request import delete_transfer_limit, set_transfer_limit
 from rucio.core.rse import (
@@ -107,15 +108,15 @@
         """ RSE (CORE): Test the listing of all RSEs """
         rse = rse_name_generator()
         rse_id = add_rse(rse, vo=vo)
         assert rse_exists(rse=rse, vo=vo)
         add_rse_attribute(rse_id=rse_id, key='tier', value='1')
         rses = list_rses(filters={'tier': '1'})
         assert (rse_id, rse) in [(r['id'], r['rse']) for r in rses]
-        add_rse_attribute(rse_id=rse_id, key='country', value='us')
+        add_rse_attribute(rse_id=rse_id, key=RseAttr.COUNTRY, value='us')
 
         rses = list_rses(filters={'tier': '1', 'country': 'us'})
         assert (rse_id, rse) in [(r['id'], r['rse']) for r in rses]
 
         del_rse(rse_id)
 
     @pytest.mark.dirty
@@ -1477,25 +1478,25 @@
             print(distance)
             assert distance['distance'] == 0
 
     def test_get_rse_protocols_includes_verify_checksum(self, vo):
         """ RSE (CORE): Test validate_checksum in RSEs info"""
         rse = rse_name_generator()
         rse_id = add_rse(rse, vo=vo)
-        add_rse_attribute(rse_id=rse_id, key='verify_checksum', value=False)
+        add_rse_attribute(rse_id=rse_id, key=RseAttr.VERIFY_CHECKSUM, value=False)
         info = get_rse_protocols(rse_id)
 
         assert 'verify_checksum' in info
         assert info['verify_checksum'] is False
 
         del_rse(rse_id)
 
         rse = rse_name_generator()
         rse_id = add_rse(rse, vo=vo)
-        add_rse_attribute(rse_id=rse_id, key='verify_checksum', value=True)
+        add_rse_attribute(rse_id=rse_id, key=RseAttr.VERIFY_CHECKSUM, value=True)
         info = get_rse_protocols(rse_id)
 
         assert 'verify_checksum' in info
         assert info['verify_checksum'] is True
         del_rse(rse_id)
 
     @pytest.mark.dirty
```

### Comparing `rucio_clients-34.2.0/tests/test_rse_expression_parser.py` & `rucio_clients-34.3.0/tests/test_rse_expression_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     def test_unconnected_operator(self):
         """ RSE_EXPRESSION_PARSER (CORE) Test invalid rse expression: unconnected operator"""
         with pytest.raises(InvalidRSEExpression):
             rse_expression_parser.parse_expression("TEST_RSE1|", **self.filter)
 
     def test_wrong_parantheses(self):
-        """ RSE_EXPRESSION_PARSER (CORE) Test invalid rse expression: wrong parantheses """
+        """ RSE_EXPRESSION_PARSER (CORE) Test invalid rse expression: wrong parentheses """
         with pytest.raises(InvalidRSEExpression):
             rse_expression_parser.parse_expression("TEST_RSE1)", **self.filter)
 
     def test_unknown_rse(self):
         """ RSE_EXPRESSION_PARSER (CORE) Test unknown RSE """
         with pytest.raises(InvalidRSEExpression):
             rse_expression_parser.parse_expression("TEST_RSE999", **self.filter)
@@ -120,15 +120,15 @@
     def test_tag_reference(self):
         """ RSE_EXPRESSION_PARSER (CORE) Test simple RSE tag reference """
         value = sorted([t_rse['id'] for t_rse in rse_expression_parser.parse_expression(self.tag1, **self.filter)])
         expected = sorted([self.rse1_id, self.rse2_id, self.rse3_id])
         assert value == expected
 
     def test_parantheses(self):
-        """ RSE_EXPRESSION_PARSER (CORE) Test parantheses """
+        """ RSE_EXPRESSION_PARSER (CORE) Test parentheses """
         value = sorted([t_rse['id'] for t_rse in rse_expression_parser.parse_expression("(%s)" % self.tag1, **self.filter)])
         expected = sorted([self.rse1_id, self.rse2_id, self.rse3_id])
         assert value == expected
 
     def test_union(self):
         """ RSE_EXPRESSION_PARSER (CORE) Test union operator """
         value = sorted([t_rse['id'] for t_rse in rse_expression_parser.parse_expression("%s|%s" % (self.tag1, self.tag2), **self.filter)])
```

### Comparing `rucio_clients-34.2.0/tests/test_rse_lfn2path.py` & `rucio_clients-34.3.0/tests/test_rse_lfn2path.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                 'lfn2pfn_algorithm': 'static_register_custom_name',
             },
             protocol_attributes=self.protocol_attributes,
         )
         assert translator.path("foo", "bar") == "static_register_value2"
 
     def test_attr_mapping(self):
-        """LFN2PFN: Verify we can map using rse and attrs (Successs)"""
+        """LFN2PFN: Verify we can map using rse and attrs (Success)"""
         def rse_algorithm(scope, name, rse, rse_attrs, proto_attrs):
             """Test LFN2PATH function for exercising the different RSE/proto attrs."""
             tier = rse_attrs.get("tier", "T1")
             scheme = proto_attrs.get("scheme", "http")
             return "%s://%s_%s/%s/%s" % (scheme, tier, rse, scope, name)
         RSEDeterministicTranslation.register(rse_algorithm)
```

### Comparing `rucio_clients-34.2.0/tests/test_rse_protocol_gfal2.py` & `rucio_clients-34.3.0/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_rse_protocol_gfal2_impl.py` & `rucio_clients-34.3.0/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_rse_protocol_posix.py` & `rucio_clients-34.3.0/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_rse_protocol_rclone.py` & `rucio_clients-34.3.0/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_rse_protocol_rsync.py` & `rucio_clients-34.3.0/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_rse_protocol_srm.py` & `rucio_clients-34.3.0/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_rse_protocol_ssh.py` & `rucio_clients-34.3.0/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_rse_protocol_webdav.py` & `rucio_clients-34.3.0/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_rse_protocol_xrootd.py` & `rucio_clients-34.3.0/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_rse_selector.py` & `rucio_clients-34.3.0/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_rucio_server.py` & `rucio_clients-34.3.0/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_rule.py` & `rucio_clients-34.3.0/tests/test_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import pytest
 
 import rucio.api.rule
 from rucio.api.account import add_account
 from rucio.client.ruleclient import RuleClient
 from rucio.common.config import config_get_bool
+from rucio.common.constants import RseAttr
 from rucio.common.exception import (
     AccessDenied,
     DuplicateRule,
     InputValidationError,
     InsufficientAccountLimit,
     InvalidSourceReplicaExpression,
     InvalidValueForKey,
@@ -236,15 +237,15 @@
             move_rule(rule_id, rseC.name)
 
     def test_add_rule_to_file_ask_approval(self, vo, mock_scope, jdoe_account):
         """ REPLICATION RULE (CORE): Add a replication rule, asking approval"""
         rse = rse_name_generator()
         rse_id = add_rse(rse, vo=vo)
 
-        add_rse_attribute(rse_id, "rule_approvers", jdoe_account)
+        add_rse_attribute(rse_id, RseAttr.RULE_APPROVERS, jdoe_account)
 
         files = create_files(1, mock_scope, rse_id)
         output = add_rule(
             dids=files,
             account=jdoe_account,
             copies=1,
             rse_expression=str(rse),
@@ -924,15 +925,15 @@
         """ REPLICATION RULE (CORE): Delete a rule with a country admin account"""
         if get_policy() != 'atlas':
             LOG.info("Skipping atlas-specific test")
             return
 
         rse = rse_name_generator()
         rse_id = add_rse(rse, vo=vo)
-        add_rse_attribute(rse_id, 'country', 'test')
+        add_rse_attribute(rse_id, RseAttr.COUNTRY, 'test')
         set_local_account_limit(jdoe_account, rse_id, -1)
 
         files = create_files(3, mock_scope, self.rse1_id)
         dataset = did_factory.random_dataset_did()
         add_did(did_type=DIDType.DATASET, account=jdoe_account, **dataset)
         attach_dids(dids=files, account=jdoe_account, **dataset)
 
@@ -1020,15 +1021,15 @@
         """ REPLICATION RULE (CORE): Add a replication rule for scratchdisk"""
         if get_policy() != 'atlas':
             LOG.info("Skipping atlas-specific test")
             return
 
         rse = rse_name_generator()
         rse_id = add_rse(rse, vo=vo)
-        add_rse_attribute(rse_id, 'type', 'SCRATCHDISK')
+        add_rse_attribute(rse_id, RseAttr.TYPE, 'SCRATCHDISK')
         set_local_account_limit(jdoe_account, rse_id, -1)
 
         files = create_files(3, mock_scope, self.rse1_id)
         dataset = did_factory.random_dataset_did()
         add_did(did_type=DIDType.DATASET, account=jdoe_account, **dataset)
         attach_dids(dids=files, account=jdoe_account, **dataset)
 
@@ -1052,29 +1053,29 @@
         with pytest.raises(InsufficientAccountLimit):
             rule_id = add_rule(dids=[dataset], account=jdoe_account, copies=1, rse_expression='%s' % rse, grouping='DATASET', weight=None, lifetime=None, locked=False, subscription_id=None)[0]
 
         rule_id = add_rule(dids=[dataset], account=jdoe_account, copies=1, rse_expression='%s' % rse, grouping='DATASET', weight=None, lifetime=None, locked=False, subscription_id=None, ask_approval=True)[0]
         assert (get_rule(rule_id)['state'] == RuleState.WAITING_APPROVAL)
         delete_rule(rule_id=rule_id)
 
-        add_rse_attribute(rse_id, 'auto_approve_bytes', 500)
+        add_rse_attribute(rse_id, RseAttr.AUTO_APPROVE_BYTES, 500)
         rule_id = add_rule(dids=[dataset], account=jdoe_account, copies=1, rse_expression='%s' % rse, grouping='DATASET', weight=None, lifetime=None, locked=False, subscription_id=None, ask_approval=True)[0]
         assert (get_rule(rule_id)['state'] == RuleState.WAITING_APPROVAL)
         delete_rule(rule_id=rule_id)
 
-        del_rse_attribute(rse_id, 'auto_approve_bytes')
-        add_rse_attribute(rse_id, 'auto_approve_bytes', 1000)
+        del_rse_attribute(rse_id, RseAttr.AUTO_APPROVE_BYTES)
+        add_rse_attribute(rse_id, RseAttr.AUTO_APPROVE_BYTES, 1000)
         rule_id = add_rule(dids=[dataset], account=jdoe_account, copies=1, rse_expression='%s' % rse, grouping='DATASET', weight=None, lifetime=None, locked=False, subscription_id=None, ask_approval=True)[0]
         assert (get_rule(rule_id)['state'] == RuleState.INJECT)
 
     def test_add_rule_with_manual_approval_block(self, vo, mock_scope, did_factory, jdoe_account):
         """ REPLICATION RULE (CORE): Add a replication rule for a RSE with manual approval block"""
         rse = rse_name_generator()
         rse_id = add_rse(rse, vo=vo)
-        add_rse_attribute(rse_id, 'block_manual_approval', '1')
+        add_rse_attribute(rse_id, RseAttr.BLOCK_MANUAL_APPROVAL, '1')
         set_local_account_limit(jdoe_account, rse_id, -1)
 
         files = create_files(3, mock_scope, self.rse1_id)
         dataset = did_factory.random_dataset_did()
         add_did(did_type=DIDType.DATASET, account=jdoe_account, **dataset)
         attach_dids(dids=files, account=jdoe_account, **dataset)
```

### Comparing `rucio_clients-34.2.0/tests/test_schema_cms.py` & `rucio_clients-34.3.0/tests/test_schema_cms.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
             validate_schema('did', bad_2)  # CMS scope for user file
         with pytest.raises(InvalidObject):
             validate_schema('did', bad_3)  # User with wrong scope
 
     def test_attachment(self):
         """ CMS SCHEMA (COMMON): Test CMS attachment"""
 
-        # no need to re-test did pattrens
+        # no need to re-test did patterns
         dids = [{
             'scope': 'cms',
             'name': '/store/mc/Fall10/DYToMuMu_M-20_TuneZ2_7TeV-pythia6/AODSIM/START38_V12-v1/0003/C0F3344F-6EC8-DF11-8ED6-E41F13181020.root',
         }]
 
         dataset = '/DoubleMu/aburgmei-Run2012A_22Jan2013_v1_RHembedded_trans1_tau121_ptelec1_17elec2_8_v4/USER#1f1eee22-cdee-0f1b-271b-77a7f559e7dd'
```

### Comparing `rucio_clients-34.2.0/tests/test_scope.py` & `rucio_clients-34.3.0/tests/test_scope.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         for scope in scopes:
             assert scope in scopes
 
     def test_is_scope_owner(self, vo, jdoe_account):
         """ SCOPE (CORE): Is scope owner """
         scope = InternalScope(scope_name_generator(), vo=vo)
         add_scope(scope=scope, account=jdoe_account)
-        anwser = is_scope_owner(scope=scope, account=jdoe_account)
-        assert anwser is True
+        answer = is_scope_owner(scope=scope, account=jdoe_account)
+        assert answer is True
 
 
 def test_scope_success(rest_client, auth_token):
     """ SCOPE (REST): send a POST to create a new account and scope """
     acntusr = account_name_generator()
     data = {'type': 'USER', 'email': 'rucio.email.com'}
     response = rest_client.post('/accounts/' + acntusr, headers=headers(auth(auth_token)), json=data)
```

### Comparing `rucio_clients-34.2.0/tests/test_subscription.py` & `rucio_clients-34.3.0/tests/test_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from json import loads
 from json.decoder import JSONDecodeError
 
 import pytest
 
 from rucio.api.subscription import add_subscription, get_subscription_by_id, list_subscription_rule_states, list_subscriptions, update_subscription
+from rucio.common.constants import RseAttr
 from rucio.common.exception import InvalidObject, SubscriptionDuplicate, SubscriptionNotFound
 from rucio.common.schema import get_schema_value
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.common.utils import generate_uuid as uuid
 from rucio.core import subscription as subscription_core
 from rucio.core.account import add_account
 from rucio.core.did import add_did, attach_dids, list_new_dids, set_new_dids, set_status
@@ -437,16 +438,16 @@
         activity = get_schema_value('ACTIVITY')['enum'][0]
         rse1, rse1_id = rse_factory.make_mock_rse()
         rse2, rse2_id = rse_factory.make_mock_rse()
         rse3, _ = rse_factory.make_mock_rse()
         rse4, _ = rse_factory.make_mock_rse()
         rse5, _ = rse_factory.make_mock_rse()
         rse6, _ = rse_factory.make_mock_rse()
-        add_rse_attribute(rse_id=rse1_id, key='associated_sites', value='%s,%s' % (rse3, rse4))
-        add_rse_attribute(rse_id=rse2_id, key='associated_sites', value='%s,%s' % (rse5, rse6))
+        add_rse_attribute(rse_id=rse1_id, key=RseAttr.ASSOCIATED_SITES, value='%s,%s' % (rse3, rse4))
+        add_rse_attribute(rse_id=rse2_id, key=RseAttr.ASSOCIATED_SITES, value='%s,%s' % (rse5, rse6))
         rses = []
         for cnt in range(5):
             rse, _ = rse_factory.make_mock_rse()
             rses.append(rse)
         rse_expression = '%s|%s' % (rse1, rse2)
         tmp_scope = InternalScope('mock_' + uuid()[:8], vo=vo)
         add_scope(tmp_scope, root_account)
@@ -740,15 +741,15 @@
             site = sites[cnt // 2]
             if cnt % 2:
                 rse_type = 'disk'
             else:
                 rse_type = 'tape'
             add_rse_attribute(rse_id=rse_id, key='tag', value=tag_test)
             add_rse_attribute(rse_id=rse_id, key=rse_type, value='True')
-            add_rse_attribute(rse_id=rse_id, key='site', value=site)
+            add_rse_attribute(rse_id=rse_id, key=RseAttr.SITE, value=site)
             dict_rse[rse] = {'rse_id': rse_id, 'rse_type': rse_type, 'site': site}
 
         tmp_scope = InternalScope('mock_' + uuid()[:8], vo=vo)
         add_scope(tmp_scope, root_account)
         subscription_name = uuid()
         dsn_prefix = did_name_generator('dataset')
```

### Comparing `rucio_clients-34.2.0/tests/test_throttler.py` & `rucio_clients-34.3.0/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_tpc.py` & `rucio_clients-34.3.0/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_trace.py` & `rucio_clients-34.3.0/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_transfer.py` & `rucio_clients-34.3.0/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_transfer_plugins.py` & `rucio_clients-34.3.0/tests/test_transfer_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     {
         "overrides": [
             ("transfers", "fts3tape_metadata_plugins", "activity, test")
         ]
     }
 ], indirect=True)
 def test_multiple_plugin_concat(file_config_mock, did_factory, rse_factory, root_account):
-    """When multiple plugins are used (like prority and collocation), both logics are applied"""
+    """When multiple plugins are used (like priority and collocation), both logics are applied"""
 
     mock_did = did_factory.random_file_did()
     transfer_path = _make_transfer_path(mock_did, rse_factory, root_account)
 
     # Mock Transfer Tool
     fts3_tool = FTS3Transfertool(TEST_FTS_HOST)
```

### Comparing `rucio_clients-34.2.0/tests/test_undertaker.py` & `rucio_clients-34.3.0/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tests/test_upload.py` & `rucio_clients-34.3.0/tests/test_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from tempfile import TemporaryDirectory
 from unittest.mock import patch
 
 import pytest
 
 from rucio.client.uploadclient import UploadClient
 from rucio.common.config import config_add_section, config_set
+from rucio.common.constants import RseAttr
 from rucio.common.exception import InputValidationError, NoFilesUploaded, NotAllFilesUploaded
 from rucio.common.utils import adler32, generate_uuid
 from rucio.core.rse import add_protocol, add_rse_attribute
 
 
 @pytest.fixture
 def upload_client():
@@ -177,15 +178,15 @@
 
 def test_multiple_protocols_same_scheme(rse_factory, upload_client, mock_scope, file_factory):
     """ Upload (CLIENT): Ensure domain correctly selected when multiple protocols exist with the same scheme """
 
     rse, rse_id = rse_factory.make_rse()
 
     # Ensure client site and rse site are identical. So that "lan" is preferred.
-    add_rse_attribute(rse_id, 'site', 'ROAMING')
+    add_rse_attribute(rse_id, RseAttr.SITE, 'ROAMING')
 
     add_protocol(rse_id, {'scheme': 'file',
                           'hostname': 'file-wan.aperture.com',
                           'port': 0,
                           'prefix': '/prefix1/',
                           'impl': 'rucio.rse.protocols.posix.Default',
                           'domains': {
```

### Comparing `rucio_clients-34.2.0/tests/test_utils.py` & `rucio_clients-34.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.2.0/tools/merge_rucio_configs.py` & `rucio_clients-34.3.0/tools/merge_rucio_configs.py`

 * *Files identical despite different names*

