# Comparing `tmp/rucio-34.2.0.tar.gz` & `tmp/rucio-34.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-34.2.0.tar", last modified: Tue Apr 16 10:35:03 2024, max compression
+gzip compressed data, was "rucio-34.3.0.tar", last modified: Mon May  6 12:44:06 2024, max compression
```

## Comparing `rucio-34.2.0.tar` & `rucio-34.3.0.tar`

### file list

```diff
@@ -1,650 +1,650 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.839003 rucio-34.2.0/
--rwxr-xr-x   0 root         (0) root         (0)     4487 2024-03-19 15:04:29.000000 rucio-34.2.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-34.2.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-34.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      934 2024-04-16 10:34:59.000000 rucio-34.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2799 2024-04-16 10:35:03.839003 rucio-34.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2024-04-16 07:53:27.000000 rucio-34.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.696002 rucio-34.2.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)   127117 2024-04-09 08:44:02.000000 rucio-34.2.0/bin/rucio
--rwxr-xr-x   0 root         (0) root         (0)     2820 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-abacus-account
--rwxr-xr-x   0 root         (0) root         (0)     1823 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-abacus-collection-replica
--rwxr-xr-x   0 root         (0) root         (0)     2567 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-abacus-rse
--rwxr-xr-x   0 root         (0) root         (0)   133531 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-admin
--rwxr-xr-x   0 root         (0) root         (0)     3185 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-atropos
--rwxr-xr-x   0 root         (0) root         (0)     5849 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-auditor
--rwxr-xr-x   0 root         (0) root         (0)     2008 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-automatix
--rwxr-xr-x   0 root         (0) root         (0)     3103 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-bb8
--rwxr-xr-x   0 root         (0) root         (0)     6100 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-c3po
--rwxr-xr-x   0 root         (0) root         (0)     5060 2024-04-08 15:35:56.000000 rucio-34.2.0/bin/rucio-cache-client
--rwxr-xr-x   0 root         (0) root         (0)     1362 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-cache-consumer
--rwxr-xr-x   0 root         (0) root         (0)     2346 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-finisher
--rwxr-xr-x   0 root         (0) root         (0)     2839 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-poller
--rwxr-xr-x   0 root         (0) root         (0)     1759 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-preparer
--rwxr-xr-x   0 root         (0) root         (0)     1682 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-receiver
--rwxr-xr-x   0 root         (0) root         (0)     3385 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-stager
--rwxr-xr-x   0 root         (0) root         (0)     6750 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-submitter
--rwxr-xr-x   0 root         (0) root         (0)     3859 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-conveyor-throttler
--rwxr-xr-x   0 root         (0) root         (0)     2546 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-dark-reaper
--rwxr-xr-x   0 root         (0) root         (0)     6463 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-dumper
--rwxr-xr-x   0 root         (0) root         (0)     1414 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-follower
--rwxr-xr-x   0 root         (0) root         (0)     1987 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-hermes
--rwxr-xr-x   0 root         (0) root         (0)     4649 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-judge-cleaner
--rwxr-xr-x   0 root         (0) root         (0)     7470 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-judge-evaluator
--rwxr-xr-x   0 root         (0) root         (0)     1671 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-judge-injector
--rwxr-xr-x   0 root         (0) root         (0)     1675 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-judge-repairer
--rwxr-xr-x   0 root         (0) root         (0)     1782 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-kronos
--rwxr-xr-x   0 root         (0) root         (0)     2260 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-minos
--rwxr-xr-x   0 root         (0) root         (0)     1997 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-minos-temporary-expiration
--rwxr-xr-x   0 root         (0) root         (0)     5625 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-necromancer
--rwxr-xr-x   0 root         (0) root         (0)     2788 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-oauth-manager
--rwxr-xr-x   0 root         (0) root         (0)     4070 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-reaper
--rwxr-xr-x   0 root         (0) root         (0)    18989 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-replica-recoverer
--rwxr-xr-x   0 root         (0) root         (0)     2351 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-rse-decommissioner
--rwxr-xr-x   0 root         (0) root         (0)     3920 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-storage-consistency-actions
--rwxr-xr-x   0 root         (0) root         (0)     3364 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-transmogrifier
--rwxr-xr-x   0 root         (0) root         (0)     2720 2024-03-21 13:32:52.000000 rucio-34.2.0/bin/rucio-undertaker
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.698001 rucio-34.2.0/etc/
--rw-r--r--   0 root         (0) root         (0)     1764 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/alembic.ini.template
--rw-r--r--   0 root         (0) root         (0)     1922 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/alembic_offline.ini.template
--rw-r--r--   0 root         (0) root         (0)       96 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/globus-config.yml.template
--rw-r--r--   0 root         (0) root         (0)      807 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/ldap.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.700002 rucio-34.2.0/etc/mail_templates/
--rw-r--r--   0 root         (0) root         (0)     1210 2024-03-13 10:19:28.000000 rucio-34.2.0/etc/mail_templates/rule_approval_request.tmpl
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/mail_templates/rule_approved_admin.tmpl
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/mail_templates/rule_approved_user.tmpl
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/mail_templates/rule_denied_admin.tmpl
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/mail_templates/rule_denied_user.tmpl
--rw-r--r--   0 root         (0) root         (0)      546 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/mail_templates/rule_ok_notification.tmpl
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/rse-accounts.cfg.template
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio-34.2.0/etc/rucio.cfg.atlas.client.template
--rw-r--r--   0 root         (0) root         (0)     8534 2024-03-13 10:19:28.000000 rucio-34.2.0/etc/rucio.cfg.template
--rw-r--r--   0 root         (0) root         (0)     7477 2024-03-13 10:19:28.000000 rucio-34.2.0/etc/rucio_multi_vo.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.674001 rucio-34.2.0/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.701002 rucio-34.2.0/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/alembicrevision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.708002 rucio-34.2.0/lib/rucio/api/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9292 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/account.py
--rw-r--r--   0 root         (0) root         (0)    11395 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/account_limit.py
--rw-r--r--   0 root         (0) root         (0)    12890 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/authentication.py
--rw-r--r--   0 root         (0) root         (0)     8654 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/config.py
--rw-r--r--   0 root         (0) root         (0)     2908 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/credential.py
--rw-r--r--   0 root         (0) root         (0)    28937 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/did.py
--rw-r--r--   0 root         (0) root         (0)     3206 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/dirac.py
--rw-r--r--   0 root         (0) root         (0)     2105 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/exporter.py
--rw-r--r--   0 root         (0) root         (0)     2651 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/heartbeat.py
--rw-r--r--   0 root         (0) root         (0)     6830 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/identity.py
--rw-r--r--   0 root         (0) root         (0)     1731 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/importer.py
--rw-r--r--   0 root         (0) root         (0)     3685 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/lifetime_exception.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/lock.py
--rw-r--r--   0 root         (0) root         (0)     3573 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     2665 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/permission.py
--rw-r--r--   0 root         (0) root         (0)     2495 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    22398 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/replica.py
--rw-r--r--   0 root         (0) root         (0)    10550 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/request.py
--rw-r--r--   0 root         (0) root         (0)    23582 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/rse.py
--rw-r--r--   0 root         (0) root         (0)    15938 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/rule.py
--rw-r--r--   0 root         (0) root         (0)     3003 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/scope.py
--rw-r--r--   0 root         (0) root         (0)    10537 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/subscription.py
--rw-r--r--   0 root         (0) root         (0)     4559 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/api/vo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.715002 rucio-34.2.0/lib/rucio/client/
--rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16353 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/accountclient.py
--rw-r--r--   0 root         (0) root         (0)     5961 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/accountlimitclient.py
--rw-r--r--   0 root         (0) root         (0)    47980 2024-04-08 15:35:56.000000 rucio-34.2.0/lib/rucio/client/baseclient.py
--rw-r--r--   0 root         (0) root         (0)     3079 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/client.py
--rw-r--r--   0 root         (0) root         (0)     4401 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/configclient.py
--rw-r--r--   0 root         (0) root         (0)     1989 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/credentialclient.py
--rw-r--r--   0 root         (0) root         (0)    28378 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/didclient.py
--rw-r--r--   0 root         (0) root         (0)     2114 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/diracclient.py
--rw-r--r--   0 root         (0) root         (0)    86092 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/client/downloadclient.py
--rw-r--r--   0 root         (0) root         (0)     1575 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/exportclient.py
--rw-r--r--   0 root         (0) root         (0)     1610 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/fileclient.py
--rw-r--r--   0 root         (0) root         (0)     1469 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/importclient.py
--rw-r--r--   0 root         (0) root         (0)     2822 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/lifetimeclient.py
--rw-r--r--   0 root         (0) root         (0)     3914 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/lockclient.py
--rw-r--r--   0 root         (0) root         (0)     5195 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/metaconventionsclient.py
--rw-r--r--   0 root         (0) root         (0)     1390 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/pingclient.py
--rw-r--r--   0 root         (0) root         (0)    19284 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/replicaclient.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/requestclient.py
--rw-r--r--   0 root         (0) root         (0)    27124 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/rseclient.py
--rw-r--r--   0 root         (0) root         (0)    12682 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/ruleclient.py
--rw-r--r--   0 root         (0) root         (0)     3147 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/scopeclient.py
--rw-r--r--   0 root         (0) root         (0)     7971 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/subscriptionclient.py
--rw-r--r--   0 root         (0) root         (0)     2642 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/touchclient.py
--rw-r--r--   0 root         (0) root         (0)    46563 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/client/uploadclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.719002 rucio-34.2.0/lib/rucio/common/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2234 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/common/cache.py
--rw-r--r--   0 root         (0) root         (0)    24284 2024-04-08 15:14:19.000000 rucio-34.2.0/lib/rucio/common/config.py
--rw-r--r--   0 root         (0) root         (0)     3300 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/constants.py
--rw-r--r--   0 root         (0) root         (0)      726 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/constraints.py
--rwxr-xr-x   0 root         (0) root         (0)     6291 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/didtype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.721002 rucio-34.2.0/lib/rucio/common/dumper/
--rw-r--r--   0 root         (0) root         (0)     9762 2024-04-10 15:37:02.000000 rucio-34.2.0/lib/rucio/common/dumper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15982 2024-04-08 15:35:56.000000 rucio-34.2.0/lib/rucio/common/dumper/consistency.py
--rw-r--r--   0 root         (0) root         (0)     9687 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/dumper/data_models.py
--rw-r--r--   0 root         (0) root         (0)     1923 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/dumper/path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    32345 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/exception.py
--rw-r--r--   0 root         (0) root         (0)     1398 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/extra.py
--rw-r--r--   0 root         (0) root         (0)    15046 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/logging.py
--rw-r--r--   0 root         (0) root         (0)    45297 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/common/pcache.py
--rw-r--r--   0 root         (0) root         (0)     6056 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/common/plugins.py
--rw-r--r--   0 root         (0) root         (0)     3013 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.723002 rucio-34.2.0/lib/rucio/common/schema/
--rw-r--r--   0 root         (0) root         (0)     5152 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15589 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/atlas.py
--rw-r--r--   0 root         (0) root         (0)    15406 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/belleii.py
--rw-r--r--   0 root         (0) root         (0)    18523 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/cms.py
--rw-r--r--   0 root         (0) root         (0)    14987 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/domatpc.py
--rw-r--r--   0 root         (0) root         (0)    15926 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/escape.py
--rw-r--r--   0 root         (0) root         (0)    16241 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/generic.py
--rw-r--r--   0 root         (0) root         (0)    15468 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)    15277 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/icecube.py
--rw-r--r--   0 root         (0) root         (0)    15885 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/schema/lsst.py
--rw-r--r--   0 root         (0) root         (0)     5414 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/stomp_utils.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     4935 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)     5069 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/common/types.py
--rw-r--r--   0 root         (0) root         (0)    79128 2024-04-08 15:14:19.000000 rucio-34.2.0/lib/rucio/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.737002 rucio-34.2.0/lib/rucio/core/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14952 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/account.py
--rw-r--r--   0 root         (0) root         (0)     6293 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/account_counter.py
--rw-r--r--   0 root         (0) root         (0)    14278 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/account_limit.py
--rw-r--r--   0 root         (0) root         (0)    19785 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/authentication.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/config.py
--rw-r--r--   0 root         (0) root         (0)     8161 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/credential.py
--rw-r--r--   0 root         (0) root         (0)   125614 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.739002 rucio-34.2.0/lib/rucio/core/did_meta_plugins/
--rw-r--r--   0 root         (0) root         (0)    11733 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17475 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/did_column_meta.py
--rw-r--r--   0 root         (0) root         (0)     4078 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py
--rw-r--r--   0 root         (0) root         (0)    29313 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     9245 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/json_meta.py
--rw-r--r--   0 root         (0) root         (0)     7453 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/mongo_meta.py
--rw-r--r--   0 root         (0) root         (0)    13727 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/did_meta_plugins/postgres_meta.py
--rw-r--r--   0 root         (0) root         (0)     9406 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/dirac.py
--rw-r--r--   0 root         (0) root         (0)     5695 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/distance.py
--rw-r--r--   0 root         (0) root         (0)     1875 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/exporter.py
--rw-r--r--   0 root         (0) root         (0)    10340 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    11836 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/identity.py
--rw-r--r--   0 root         (0) root         (0)    14114 2024-04-09 11:14:59.000000 rucio-34.2.0/lib/rucio/core/importer.py
--rw-r--r--   0 root         (0) root         (0)    15235 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/lifetime_exception.py
--rw-r--r--   0 root         (0) root         (0)    22807 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/lock.py
--rw-r--r--   0 root         (0) root         (0)     9693 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/message.py
--rw-r--r--   0 root         (0) root         (0)     8691 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)    15768 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/monitor.py
--rw-r--r--   0 root         (0) root         (0)     5395 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/naming_convention.py
--rw-r--r--   0 root         (0) root         (0)     4890 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/nongrid_trace.py
--rw-r--r--   0 root         (0) root         (0)    69761 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/core/oidc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.742002 rucio-34.2.0/lib/rucio/core/permission/
--rw-r--r--   0 root         (0) root         (0)     3910 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55427 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/atlas.py
--rw-r--r--   0 root         (0) root         (0)    46908 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/belleii.py
--rw-r--r--   0 root         (0) root         (0)    46757 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/cms.py
--rw-r--r--   0 root         (0) root         (0)    43104 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/escape.py
--rw-r--r--   0 root         (0) root         (0)    45307 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/generic.py
--rw-r--r--   0 root         (0) root         (0)    45853 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/permission/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     8029 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)   177321 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/core/replica.py
--rw-r--r--   0 root         (0) root         (0)    15420 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/replica_sorter.py
--rw-r--r--   0 root         (0) root         (0)   116256 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/core/request.py
--rw-r--r--   0 root         (0) root         (0)    67929 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/rse.py
--rw-r--r--   0 root         (0) root         (0)     5510 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/rse_counter.py
--rw-r--r--   0 root         (0) root         (0)    15369 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)    13946 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/core/rse_selector.py
--rw-r--r--   0 root         (0) root         (0)   208340 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/rule.py
--rw-r--r--   0 root         (0) root         (0)    92255 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/rule_grouping.py
--rw-r--r--   0 root         (0) root         (0)     5364 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/scope.py
--rw-r--r--   0 root         (0) root         (0)    15232 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/subscription.py
--rw-r--r--   0 root         (0) root         (0)    18667 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/topology.py
--rw-r--r--   0 root         (0) root         (0)    13107 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/trace.py
--rw-r--r--   0 root         (0) root         (0)    64150 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/transfer.py
--rw-r--r--   0 root         (0) root         (0)     5613 2024-04-08 15:24:34.000000 rucio-34.2.0/lib/rucio/core/vo.py
--rw-r--r--   0 root         (0) root         (0)     5070 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/core/volatile_replica.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.742002 rucio-34.2.0/lib/rucio/daemons/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.743002 rucio-34.2.0/lib/rucio/daemons/abacus/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/abacus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3736 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/abacus/account.py
--rw-r--r--   0 root         (0) root         (0)     3856 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/abacus/collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/abacus/rse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.744002 rucio-34.2.0/lib/rucio/daemons/atropos/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/atropos/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10574 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/atropos/atropos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.745002 rucio-34.2.0/lib/rucio/daemons/auditor/
--rw-r--r--   0 root         (0) root         (0)     9998 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/auditor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2865 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/auditor/hdfs.py
--rw-r--r--   0 root         (0) root         (0)    10248 2024-04-10 15:37:02.000000 rucio-34.2.0/lib/rucio/daemons/auditor/srmdumps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.745002 rucio-34.2.0/lib/rucio/daemons/automatix/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/automatix/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9973 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/automatix/automatix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.746002 rucio-34.2.0/lib/rucio/daemons/badreplicas/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/badreplicas/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15768 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/badreplicas/minos.py
--rw-r--r--   0 root         (0) root         (0)     8626 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py
--rw-r--r--   0 root         (0) root         (0)     9892 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/badreplicas/necromancer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.748002 rucio-34.2.0/lib/rucio/daemons/bb8/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/bb8/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13071 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/bb8/bb8.py
--rw-r--r--   0 root         (0) root         (0)    26597 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/bb8/common.py
--rw-r--r--   0 root         (0) root         (0)     6644 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py
--rw-r--r--   0 root         (0) root         (0)     6522 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/bb8/t2_background_rebalance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.748002 rucio-34.2.0/lib/rucio/daemons/c3po/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.750002 rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4571 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/simple.py
--rw-r--r--   0 root         (0) root         (0)     4651 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py
--rw-r--r--   0 root         (0) root         (0)     4774 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py
--rw-r--r--   0 root         (0) root         (0)    12151 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py
--rw-r--r--   0 root         (0) root         (0)    15009 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/c3po.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.751002 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3261 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/agis.py
--rw-r--r--   0 root         (0) root         (0)     2094 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/free_space.py
--rw-r--r--   0 root         (0) root         (0)     1648 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/jedi_did.py
--rw-r--r--   0 root         (0) root         (0)     1339 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/mock_did.py
--rw-r--r--   0 root         (0) root         (0)     2068 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/network_metrics.py
--rw-r--r--   0 root         (0) root         (0)     3818 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/collectors/workload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.753002 rucio-34.2.0/lib/rucio/daemons/c3po/utils/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1386 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/utils/dataset_cache.py
--rw-r--r--   0 root         (0) root         (0)     1523 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py
--rw-r--r--   0 root         (0) root         (0)     1596 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/utils/expiring_list.py
--rw-r--r--   0 root         (0) root         (0)     2440 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/utils/popularity.py
--rw-r--r--   0 root         (0) root         (0)     2087 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/c3po/utils/timeseries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.753002 rucio-34.2.0/lib/rucio/daemons/cache/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-34.2.0/lib/rucio/daemons/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6744 2024-03-13 10:19:28.000000 rucio-34.2.0/lib/rucio/daemons/cache/consumer.py
--rw-r--r--   0 root         (0) root         (0)    14947 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.756002 rucio-34.2.0/lib/rucio/daemons/conveyor/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25768 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/common.py
--rw-r--r--   0 root         (0) root         (0)    23644 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/finisher.py
--rw-r--r--   0 root         (0) root         (0)    16242 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/poller.py
--rw-r--r--   0 root         (0) root         (0)     7462 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/preparer.py
--rw-r--r--   0 root         (0) root         (0)     8289 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/receiver.py
--rw-r--r--   0 root         (0) root         (0)     3827 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/stager.py
--rw-r--r--   0 root         (0) root         (0)    16333 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/submitter.py
--rw-r--r--   0 root         (0) root         (0)    20351 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/conveyor/throttler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.757002 rucio-34.2.0/lib/rucio/daemons/follower/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/follower/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3355 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/follower/follower.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.757002 rucio-34.2.0/lib/rucio/daemons/hermes/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/hermes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26436 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/hermes/hermes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.759002 rucio-34.2.0/lib/rucio/daemons/judge/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/judge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5772 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/judge/cleaner.py
--rw-r--r--   0 root         (0) root         (0)     7170 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/judge/evaluator.py
--rw-r--r--   0 root         (0) root         (0)     6394 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/judge/injector.py
--rw-r--r--   0 root         (0) root         (0)     5310 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/judge/repairer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.759002 rucio-34.2.0/lib/rucio/daemons/oauthmanager/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/oauthmanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8815 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/oauthmanager/oauthmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.760002 rucio-34.2.0/lib/rucio/daemons/reaper/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/reaper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11222 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/reaper/dark_reaper.py
--rw-r--r--   0 root         (0) root         (0)    35532 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/reaper/reaper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.760002 rucio-34.2.0/lib/rucio/daemons/replicarecoverer/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/replicarecoverer/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    33150 2024-04-05 14:57:55.000000 rucio-34.2.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.761002 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2671 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.763002 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/
--rw-r--r--   0 root         (0) root         (0)      863 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2221 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py
--rw-r--r--   0 root         (0) root         (0)    16231 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py
--rw-r--r--   0 root         (0) root         (0)     2927 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py
--rw-r--r--   0 root         (0) root         (0)    10358 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.763002 rucio-34.2.0/lib/rucio/daemons/storage/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.763002 rucio-34.2.0/lib/rucio/daemons/storage/consistency/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/storage/consistency/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29563 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/storage/consistency/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.764002 rucio-34.2.0/lib/rucio/daemons/tracer/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/tracer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23764 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/tracer/kronos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.765002 rucio-34.2.0/lib/rucio/daemons/transmogrifier/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/transmogrifier/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30528 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/transmogrifier/transmogrifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.765002 rucio-34.2.0/lib/rucio/daemons/undertaker/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/daemons/undertaker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5230 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/daemons/undertaker/undertaker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.766002 rucio-34.2.0/lib/rucio/db/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.769002 rucio-34.2.0/lib/rucio/db/sqla/
--rw-r--r--   0 root         (0) root         (0)     2130 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4151 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.769002 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3545 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.801003 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/
--rw-r--r--   0 root         (0) root         (0)     3340 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py
--rw-r--r--   0 root         (0) root         (0)     1821 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py
--rw-r--r--   0 root         (0) root         (0)     2640 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py
--rw-r--r--   0 root         (0) root         (0)     1533 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     5272 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py
--rw-r--r--   0 root         (0) root         (0)     3659 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py
--rw-r--r--   0 root         (0) root         (0)     1548 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py
--rw-r--r--   0 root         (0) root         (0)     2816 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py
--rw-r--r--   0 root         (0) root         (0)     1260 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py
--rw-r--r--   0 root         (0) root         (0)     1678 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py
--rw-r--r--   0 root         (0) root         (0)     2675 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     1314 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py
--rw-r--r--   0 root         (0) root         (0)     8494 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py
--rw-r--r--   0 root         (0) root         (0)     3277 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     3782 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py
--rw-r--r--   0 root         (0) root         (0)     1546 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py
--rw-r--r--   0 root         (0) root         (0)     1692 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py
--rw-r--r--   0 root         (0) root         (0)     4360 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py
--rw-r--r--   0 root         (0) root         (0)     3014 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     1497 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
--rw-r--r--   0 root         (0) root         (0)     2781 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
--rw-r--r--   0 root         (0) root         (0)     2297 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1535 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     2274 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
--rw-r--r--   0 root         (0) root         (0)     1219 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
--rw-r--r--   0 root         (0) root         (0)     1723 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py
--rw-r--r--   0 root         (0) root         (0)     2206 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
--rw-r--r--   0 root         (0) root         (0)     1787 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py
--rw-r--r--   0 root         (0) root         (0)     2837 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
--rw-r--r--   0 root         (0) root         (0)     1554 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
--rw-r--r--   0 root         (0) root         (0)     1571 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py
--rw-r--r--   0 root         (0) root         (0)     1308 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py
--rw-r--r--   0 root         (0) root         (0)     2019 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py
--rw-r--r--   0 root         (0) root         (0)     3882 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py
--rw-r--r--   0 root         (0) root         (0)     2513 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     3997 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     2817 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py
--rw-r--r--   0 root         (0) root         (0)     7527 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py
--rw-r--r--   0 root         (0) root         (0)     2396 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py
--rw-r--r--   0 root         (0) root         (0)     3592 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py
--rw-r--r--   0 root         (0) root         (0)     2687 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py
--rw-r--r--   0 root         (0) root         (0)     2777 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1287 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     1644 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py
--rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py
--rw-r--r--   0 root         (0) root         (0)     1420 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py
--rw-r--r--   0 root         (0) root         (0)     2424 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py
--rw-r--r--   0 root         (0) root         (0)     1666 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py
--rw-r--r--   0 root         (0) root         (0)     1585 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py
--rw-r--r--   0 root         (0) root         (0)     2008 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py
--rw-r--r--   0 root         (0) root         (0)     1272 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py
--rw-r--r--   0 root         (0) root         (0)     2757 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py
--rw-r--r--   0 root         (0) root         (0)     1598 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py
--rw-r--r--   0 root         (0) root         (0)     2476 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py
--rw-r--r--   0 root         (0) root         (0)     1542 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py
--rw-r--r--   0 root         (0) root         (0)     1417 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     1526 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py
--rw-r--r--   0 root         (0) root         (0)     2363 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py
--rw-r--r--   0 root         (0) root         (0)     1701 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     6101 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py
--rw-r--r--   0 root         (0) root         (0)     2266 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py
--rw-r--r--   0 root         (0) root         (0)     1666 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py
--rw-r--r--   0 root         (0) root         (0)     1969 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     1363 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py
--rw-r--r--   0 root         (0) root         (0)     5023 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py
--rw-r--r--   0 root         (0) root         (0)     3568 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py
--rw-r--r--   0 root         (0) root         (0)     1889 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py
--rw-r--r--   0 root         (0) root         (0)     1661 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py
--rw-r--r--   0 root         (0) root         (0)     1715 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py
--rw-r--r--   0 root         (0) root         (0)     3118 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1749 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py
--rw-r--r--   0 root         (0) root         (0)     5038 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py
--rw-r--r--   0 root         (0) root         (0)     1938 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py
--rw-r--r--   0 root         (0) root         (0)     3689 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py
--rw-r--r--   0 root         (0) root         (0)     2614 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py
--rw-r--r--   0 root         (0) root         (0)     3117 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py
--rw-r--r--   0 root         (0) root         (0)     5836 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py
--rw-r--r--   0 root         (0) root         (0)     2595 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     2195 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py
--rw-r--r--   0 root         (0) root         (0)     2173 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     1883 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1546 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py
--rw-r--r--   0 root         (0) root         (0)     1348 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py
--rw-r--r--   0 root         (0) root         (0)     1585 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py
--rw-r--r--   0 root         (0) root         (0)     7344 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py
--rw-r--r--   0 root         (0) root         (0)     3704 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py
--rw-r--r--   0 root         (0) root         (0)     2091 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py
--rw-r--r--   0 root         (0) root         (0)     2934 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py
--rw-r--r--   0 root         (0) root         (0)     2784 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py
--rw-r--r--   0 root         (0) root         (0)     1747 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     9561 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py
--rw-r--r--   0 root         (0) root         (0)     4748 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py
--rw-r--r--   0 root         (0) root         (0)     1736 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1594 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py
--rw-r--r--   0 root         (0) root         (0)     5263 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py
--rw-r--r--   0 root         (0) root         (0)     2429 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py
--rw-r--r--   0 root         (0) root         (0)     4865 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py
--rw-r--r--   0 root         (0) root         (0)      897 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py
--rw-r--r--   0 root         (0) root         (0)     2947 2024-03-21 13:32:52.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py
--rw-r--r--   0 root         (0) root         (0)     1949 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py
--rw-r--r--   0 root         (0) root         (0)     1110 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py
--rw-r--r--   0 root         (0) root         (0)     1896 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py
--rw-r--r--   0 root         (0) root         (0)     1599 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py
--rw-r--r--   0 root         (0) root         (0)   112135 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/models.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/sautils.py
--rw-r--r--   0 root         (0) root         (0)    17773 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/session.py
--rw-r--r--   0 root         (0) root         (0)     6088 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/types.py
--rw-r--r--   0 root         (0) root         (0)    21427 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/db/sqla/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.801003 rucio-34.2.0/lib/rucio/rse/
--rw-r--r--   0 root         (0) root         (0)     3303 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.805003 rucio-34.2.0/lib/rucio/rse/protocols/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7198 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/bittorrent.py
--rw-r--r--   0 root         (0) root         (0)     4603 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/cache.py
--rw-r--r--   0 root         (0) root         (0)     4225 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/dummy.py
--rw-r--r--   0 root         (0) root         (0)    29093 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/gfal.py
--rw-r--r--   0 root         (0) root         (0)     9680 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/globus.py
--rw-r--r--   0 root         (0) root         (0)     3409 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/gsiftp.py
--rw-r--r--   0 root         (0) root         (0)     2975 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/http_cache.py
--rw-r--r--   0 root         (0) root         (0)     4495 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/mock.py
--rw-r--r--   0 root         (0) root         (0)     7224 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/ngarc.py
--rw-r--r--   0 root         (0) root         (0)    10394 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/posix.py
--rw-r--r--   0 root         (0) root         (0)    22650 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/protocol.py
--rw-r--r--   0 root         (0) root         (0)    15256 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/rclone.py
--rw-r--r--   0 root         (0) root         (0)     5499 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/rfio.py
--rw-r--r--   0 root         (0) root         (0)    14651 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/srm.py
--rw-r--r--   0 root         (0) root         (0)    17467 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/ssh.py
--rw-r--r--   0 root         (0) root         (0)     8127 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/storm.py
--rw-r--r--   0 root         (0) root         (0)    22166 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/webdav.py
--rw-r--r--   0 root         (0) root         (0)    12567 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/protocols/xrootd.py
--rw-r--r--   0 root         (0) root         (0)    37238 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/rse/rsemanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.805003 rucio-34.2.0/lib/rucio/tests/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8879 2024-04-08 15:35:57.000000 rucio-34.2.0/lib/rucio/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     5045 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/tests/common_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.807003 rucio-34.2.0/lib/rucio/transfertool/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8299 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/bittorrent.py
--rw-r--r--   0 root         (0) root         (0)     1711 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/bittorrent_driver.py
--rw-r--r--   0 root         (0) root         (0)     4940 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py
--rw-r--r--   0 root         (0) root         (0)    72072 2024-04-02 11:45:21.000000 rucio-34.2.0/lib/rucio/transfertool/fts3.py
--rw-r--r--   0 root         (0) root         (0)     6136 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/fts3_plugins.py
--rw-r--r--   0 root         (0) root         (0)     7656 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/globus.py
--rw-r--r--   0 root         (0) root         (0)     8411 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/globus_library.py
--rw-r--r--   0 root         (0) root         (0)     2859 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/mock.py
--rw-r--r--   0 root         (0) root         (0)     7753 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/transfertool/transfertool.py
--rw-r--r--   0 root         (0) root         (0)      244 2024-04-16 07:53:37.000000 rucio-34.2.0/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1577 2024-04-08 15:22:52.000000 rucio-34.2.0/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.807003 rucio-34.2.0/lib/rucio/web/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.808003 rucio-34.2.0/lib/rucio/web/rest/
--rwxr-xr-x   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.808003 rucio-34.2.0/lib/rucio/web/rest/flaskapi/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.814003 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7790 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py
--rw-r--r--   0 root         (0) root         (0)    36983 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/accounts.py
--rw-r--r--   0 root         (0) root         (0)     3344 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/archives.py
--rw-r--r--   0 root         (0) root         (0)    61575 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/auth.py
--rw-r--r--   0 root         (0) root         (0)    16147 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/common.py
--rw-r--r--   0 root         (0) root         (0)    10143 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/config.py
--rw-r--r--   0 root         (0) root         (0)     7718 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/credentials.py
--rw-r--r--   0 root         (0) root         (0)    80863 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/dids.py
--rw-r--r--   0 root         (0) root         (0)     4706 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/dirac.py
--rw-r--r--   0 root         (0) root         (0)     2656 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/export.py
--rw-r--r--   0 root         (0) root         (0)     4620 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     7894 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/identities.py
--rw-r--r--   0 root         (0) root         (0)     5257 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/import.py
--rw-r--r--   0 root         (0) root         (0)    12007 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12990 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/locks.py
--rw-r--r--   0 root         (0) root         (0)     2861 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/main.py
--rw-r--r--   0 root         (0) root         (0)     7784 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1250 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/metrics.py
--rw-r--r--   0 root         (0) root         (0)     3131 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py
--rw-r--r--   0 root         (0) root         (0)     3096 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/ping.py
--rw-r--r--   0 root         (0) root         (0)    13331 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/redirect.py
--rw-r--r--   0 root         (0) root         (0)    72710 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/replicas.py
--rw-r--r--   0 root         (0) root         (0)    41600 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/requests.py
--rw-r--r--   0 root         (0) root         (0)    81945 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/rses.py
--rw-r--r--   0 root         (0) root         (0)    31870 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/rules.py
--rw-r--r--   0 root         (0) root         (0)     5068 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/scopes.py
--rw-r--r--   0 root         (0) root         (0)    24149 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.815003 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/templates/
--rw-r--r--   0 root         (0) root         (0)     2254 2023-07-27 12:40:37.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html
--rw-r--r--   0 root         (0) root         (0)     2139 2023-07-27 12:40:37.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html
--rw-r--r--   0 root         (0) root         (0)     3213 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/traces.py
--rw-r--r--   0 root         (0) root         (0)     9154 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/vos.py
--rw-r--r--   0 root         (0) root         (0)      725 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/main.py
--rw-r--r--   0 root         (0) root         (0)     1016 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/metrics.py
--rw-r--r--   0 root         (0) root         (0)     1010 2024-03-21 13:32:51.000000 rucio-34.2.0/lib/rucio/web/rest/ping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.834003 rucio-34.2.0/lib/rucio.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25997 2024-04-16 10:35:03.000000 rucio-34.2.0/lib/rucio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2024-03-13 10:19:28.000000 rucio-34.2.0/pylintrc
--rw-r--r--   0 root         (0) root         (0)     1235 2024-03-21 13:32:52.000000 rucio-34.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5048 2024-04-16 07:53:27.000000 rucio-34.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2024-04-16 10:35:03.840003 rucio-34.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2932 2024-04-16 10:34:59.000000 rucio-34.2.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     4778 2024-03-21 13:32:51.000000 rucio-34.2.0/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.833003 rucio-34.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10677 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3229 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15920 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20523 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13352 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4074 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2181 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4201 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    15058 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3464 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23264 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12425 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107413 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2065 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     8398 2024-04-08 15:14:19.000000 rucio-34.2.0/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1865 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6942 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    96558 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    23797 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7679 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7337 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2618 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28187 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2736 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    58823 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29517 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4185 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7118 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16419 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10867 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3082 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38301 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7953 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10106 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5819 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18584 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57223 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5258 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22277 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20428 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12180 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6299 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2034 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54264 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2759 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11582 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   108356 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7583 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2741 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2023 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27487 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6440 2024-03-21 13:32:51.000000 rucio-34.2.0/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62385 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    38873 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22741 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    17184 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    12978 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75019 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13184 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8941 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4277 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3267 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3690 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4799 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     3979 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3780 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7746 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    91864 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)    13848 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_schema_cms.py
--rw-r--r--   0 root         (0) root         (0)     7486 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48328 2024-04-02 11:36:32.000000 rucio-34.2.0/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)    55587 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3181 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    25254 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8923 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_transfer_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8412 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15526 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     7427 2024-03-21 13:32:52.000000 rucio-34.2.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:03.834003 rucio-34.2.0/tools/
--rwxr-xr-x   0 root         (0) root         (0)     1259 2024-03-21 13:32:51.000000 rucio-34.2.0/tools/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     6163 2024-03-21 13:32:51.000000 rucio-34.2.0/tools/merge_rucio_configs.py
--rwxr-xr-x   0 root         (0) root         (0)     1351 2024-03-21 13:32:51.000000 rucio-34.2.0/tools/reset_database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.093713 rucio-34.3.0/
+-rwxr-xr-x   0 root         (0) root         (0)     4487 2024-05-06 09:19:47.000000 rucio-34.3.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-34.3.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-34.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      934 2024-05-06 12:44:02.000000 rucio-34.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2799 2024-05-06 12:44:06.093713 rucio-34.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-05-06 11:03:53.000000 rucio-34.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:05.993712 rucio-34.3.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)   127119 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio
+-rwxr-xr-x   0 root         (0) root         (0)     2820 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-abacus-account
+-rwxr-xr-x   0 root         (0) root         (0)     1823 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-abacus-collection-replica
+-rwxr-xr-x   0 root         (0) root         (0)     2567 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-abacus-rse
+-rwxr-xr-x   0 root         (0) root         (0)   133582 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-admin
+-rwxr-xr-x   0 root         (0) root         (0)     3185 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-atropos
+-rwxr-xr-x   0 root         (0) root         (0)     5850 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-auditor
+-rwxr-xr-x   0 root         (0) root         (0)     2010 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-automatix
+-rwxr-xr-x   0 root         (0) root         (0)     3103 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-bb8
+-rwxr-xr-x   0 root         (0) root         (0)     6100 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-c3po
+-rwxr-xr-x   0 root         (0) root         (0)     5060 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-cache-client
+-rwxr-xr-x   0 root         (0) root         (0)     1362 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-cache-consumer
+-rwxr-xr-x   0 root         (0) root         (0)     2347 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-finisher
+-rwxr-xr-x   0 root         (0) root         (0)     2839 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-poller
+-rwxr-xr-x   0 root         (0) root         (0)     1759 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-preparer
+-rwxr-xr-x   0 root         (0) root         (0)     1682 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-receiver
+-rwxr-xr-x   0 root         (0) root         (0)     3385 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-stager
+-rwxr-xr-x   0 root         (0) root         (0)     6752 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-submitter
+-rwxr-xr-x   0 root         (0) root         (0)     3859 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-throttler
+-rwxr-xr-x   0 root         (0) root         (0)     2546 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-dark-reaper
+-rwxr-xr-x   0 root         (0) root         (0)     6463 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-dumper
+-rwxr-xr-x   0 root         (0) root         (0)     1414 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-follower
+-rwxr-xr-x   0 root         (0) root         (0)     1987 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-hermes
+-rwxr-xr-x   0 root         (0) root         (0)     4649 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-judge-cleaner
+-rwxr-xr-x   0 root         (0) root         (0)     7472 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-judge-evaluator
+-rwxr-xr-x   0 root         (0) root         (0)     1671 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-judge-injector
+-rwxr-xr-x   0 root         (0) root         (0)     1675 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-judge-repairer
+-rwxr-xr-x   0 root         (0) root         (0)     1782 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-kronos
+-rwxr-xr-x   0 root         (0) root         (0)     2260 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-minos
+-rwxr-xr-x   0 root         (0) root         (0)     1997 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-minos-temporary-expiration
+-rwxr-xr-x   0 root         (0) root         (0)     5626 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-necromancer
+-rwxr-xr-x   0 root         (0) root         (0)     2790 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-oauth-manager
+-rwxr-xr-x   0 root         (0) root         (0)     4070 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-reaper
+-rwxr-xr-x   0 root         (0) root         (0)    18988 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-replica-recoverer
+-rwxr-xr-x   0 root         (0) root         (0)     2351 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-rse-decommissioner
+-rwxr-xr-x   0 root         (0) root         (0)     3920 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-storage-consistency-actions
+-rwxr-xr-x   0 root         (0) root         (0)     3364 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-transmogrifier
+-rwxr-xr-x   0 root         (0) root         (0)     2720 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-undertaker
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:05.994711 rucio-34.3.0/etc/
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/alembic.ini.template
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/alembic_offline.ini.template
+-rw-r--r--   0 root         (0) root         (0)       96 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/globus-config.yml.template
+-rw-r--r--   0 root         (0) root         (0)      806 2024-05-06 09:19:47.000000 rucio-34.3.0/etc/ldap.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:05.995712 rucio-34.3.0/etc/mail_templates/
+-rw-r--r--   0 root         (0) root         (0)     1210 2024-05-06 09:19:47.000000 rucio-34.3.0/etc/mail_templates/rule_approval_request.tmpl
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/mail_templates/rule_approved_admin.tmpl
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/mail_templates/rule_approved_user.tmpl
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/mail_templates/rule_denied_admin.tmpl
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/mail_templates/rule_denied_user.tmpl
+-rw-r--r--   0 root         (0) root         (0)      546 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/mail_templates/rule_ok_notification.tmpl
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/rse-accounts.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/rucio.cfg.atlas.client.template
+-rw-r--r--   0 root         (0) root         (0)     8534 2024-05-06 09:19:47.000000 rucio-34.3.0/etc/rucio.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     7477 2024-05-06 09:19:47.000000 rucio-34.3.0/etc/rucio_multi_vo.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:05.980711 rucio-34.3.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:05.996712 rucio-34.3.0/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/alembicrevision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:05.999712 rucio-34.3.0/lib/rucio/api/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9292 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/account.py
+-rw-r--r--   0 root         (0) root         (0)    11394 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/account_limit.py
+-rw-r--r--   0 root         (0) root         (0)    12890 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/authentication.py
+-rw-r--r--   0 root         (0) root         (0)     9085 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/config.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/credential.py
+-rw-r--r--   0 root         (0) root         (0)    28964 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/did.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/exporter.py
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)     6830 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/identity.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/importer.py
+-rw-r--r--   0 root         (0) root         (0)     3685 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/lifetime_exception.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/lock.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/permission.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    22398 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/replica.py
+-rw-r--r--   0 root         (0) root         (0)    10550 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/request.py
+-rw-r--r--   0 root         (0) root         (0)    23582 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/rse.py
+-rw-r--r--   0 root         (0) root         (0)    15938 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/rule.py
+-rw-r--r--   0 root         (0) root         (0)     3003 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/scope.py
+-rw-r--r--   0 root         (0) root         (0)    10537 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     4817 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/vo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.004712 rucio-34.3.0/lib/rucio/client/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16352 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/accountclient.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/accountlimitclient.py
+-rw-r--r--   0 root         (0) root         (0)    48007 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/baseclient.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     4401 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/configclient.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/credentialclient.py
+-rw-r--r--   0 root         (0) root         (0)    28378 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/didclient.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/diracclient.py
+-rw-r--r--   0 root         (0) root         (0)    86094 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/downloadclient.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/exportclient.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/fileclient.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/importclient.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/lifetimeclient.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/lockclient.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/metaconventionsclient.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/pingclient.py
+-rw-r--r--   0 root         (0) root         (0)    19284 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/replicaclient.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/requestclient.py
+-rw-r--r--   0 root         (0) root         (0)    27121 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/rseclient.py
+-rw-r--r--   0 root         (0) root         (0)    12734 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/ruleclient.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/scopeclient.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/subscriptionclient.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/touchclient.py
+-rw-r--r--   0 root         (0) root         (0)    46627 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/uploadclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.007712 rucio-34.3.0/lib/rucio/common/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/cache.py
+-rw-r--r--   0 root         (0) root         (0)    24636 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/constants.py
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/constraints.py
+-rwxr-xr-x   0 root         (0) root         (0)     6545 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/didtype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.008712 rucio-34.3.0/lib/rucio/common/dumper/
+-rw-r--r--   0 root         (0) root         (0)    10796 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/dumper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15985 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/dumper/consistency.py
+-rw-r--r--   0 root         (0) root         (0)     9693 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/dumper/data_models.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/dumper/path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    32345 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/exception.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/extra.py
+-rw-r--r--   0 root         (0) root         (0)    15046 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/logging.py
+-rw-r--r--   0 root         (0) root         (0)    45296 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/pcache.py
+-rw-r--r--   0 root         (0) root         (0)     6071 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.010712 rucio-34.3.0/lib/rucio/common/schema/
+-rw-r--r--   0 root         (0) root         (0)     5384 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15589 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    18523 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/cms.py
+-rw-r--r--   0 root         (0) root         (0)    14987 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/domatpc.py
+-rw-r--r--   0 root         (0) root         (0)    15926 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/escape.py
+-rw-r--r--   0 root         (0) root         (0)    16241 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/generic.py
+-rw-r--r--   0 root         (0) root         (0)    15468 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)    15277 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/icecube.py
+-rw-r--r--   0 root         (0) root         (0)    15885 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/lsst.py
+-rw-r--r--   0 root         (0) root         (0)     5414 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/stomp_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)     5427 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/types.py
+-rw-r--r--   0 root         (0) root         (0)    79121 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.018712 rucio-34.3.0/lib/rucio/core/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14952 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/account.py
+-rw-r--r--   0 root         (0) root         (0)     6289 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/account_counter.py
+-rw-r--r--   0 root         (0) root         (0)    14274 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/account_limit.py
+-rw-r--r--   0 root         (0) root         (0)    20045 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/authentication.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/config.py
+-rw-r--r--   0 root         (0) root         (0)     8211 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/credential.py
+-rw-r--r--   0 root         (0) root         (0)   125584 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.019712 rucio-34.3.0/lib/rucio/core/did_meta_plugins/
+-rw-r--r--   0 root         (0) root         (0)    11733 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17445 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/did_column_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4932 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py
+-rw-r--r--   0 root         (0) root         (0)    29313 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     9215 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/json_meta.py
+-rw-r--r--   0 root         (0) root         (0)     7431 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/mongo_meta.py
+-rw-r--r--   0 root         (0) root         (0)    13727 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/postgres_meta.py
+-rw-r--r--   0 root         (0) root         (0)     9402 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     5695 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/distance.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/exporter.py
+-rw-r--r--   0 root         (0) root         (0)    10986 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    12099 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/identity.py
+-rw-r--r--   0 root         (0) root         (0)    14169 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/importer.py
+-rw-r--r--   0 root         (0) root         (0)    15254 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/lifetime_exception.py
+-rw-r--r--   0 root         (0) root         (0)    22857 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/lock.py
+-rw-r--r--   0 root         (0) root         (0)     9693 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/message.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)    15984 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/nongrid_trace.py
+-rw-r--r--   0 root         (0) root         (0)    69763 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/oidc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.020712 rucio-34.3.0/lib/rucio/core/permission/
+-rw-r--r--   0 root         (0) root         (0)     4070 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55734 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    46969 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    46848 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/cms.py
+-rw-r--r--   0 root         (0) root         (0)    43171 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/escape.py
+-rw-r--r--   0 root         (0) root         (0)    48439 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/generic.py
+-rw-r--r--   0 root         (0) root         (0)    45926 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     8030 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)   177379 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/replica.py
+-rw-r--r--   0 root         (0) root         (0)    15420 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/replica_sorter.py
+-rw-r--r--   0 root         (0) root         (0)   116306 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/request.py
+-rw-r--r--   0 root         (0) root         (0)    68025 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/rse.py
+-rw-r--r--   0 root         (0) root         (0)     5506 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/rse_counter.py
+-rw-r--r--   0 root         (0) root         (0)    15368 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)    13941 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)   208510 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/rule.py
+-rw-r--r--   0 root         (0) root         (0)    92320 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/rule_grouping.py
+-rw-r--r--   0 root         (0) root         (0)     5364 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/scope.py
+-rw-r--r--   0 root         (0) root         (0)    15235 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    18930 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/topology.py
+-rw-r--r--   0 root         (0) root         (0)    13107 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/trace.py
+-rw-r--r--   0 root         (0) root         (0)    64200 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/transfer.py
+-rw-r--r--   0 root         (0) root         (0)     5585 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/vo.py
+-rw-r--r--   0 root         (0) root         (0)     5066 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/volatile_replica.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.021712 rucio-34.3.0/lib/rucio/daemons/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.022712 rucio-34.3.0/lib/rucio/daemons/abacus/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/abacus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/abacus/account.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/abacus/collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/abacus/rse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.022712 rucio-34.3.0/lib/rucio/daemons/atropos/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/atropos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10574 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/atropos/atropos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.022712 rucio-34.3.0/lib/rucio/daemons/auditor/
+-rw-r--r--   0 root         (0) root         (0)    10003 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/auditor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/auditor/hdfs.py
+-rw-r--r--   0 root         (0) root         (0)    10314 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/auditor/srmdumps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.023712 rucio-34.3.0/lib/rucio/daemons/automatix/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/automatix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9974 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/automatix/automatix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.023712 rucio-34.3.0/lib/rucio/daemons/badreplicas/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/badreplicas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15769 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/badreplicas/minos.py
+-rw-r--r--   0 root         (0) root         (0)     8626 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py
+-rw-r--r--   0 root         (0) root         (0)     9892 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/badreplicas/necromancer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.024712 rucio-34.3.0/lib/rucio/daemons/bb8/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/bb8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13071 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/bb8/bb8.py
+-rw-r--r--   0 root         (0) root         (0)    26598 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/bb8/common.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py
+-rw-r--r--   0 root         (0) root         (0)     6571 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/bb8/t2_background_rebalance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.025712 rucio-34.3.0/lib/rucio/daemons/c3po/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.025712 rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/simple.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py
+-rw-r--r--   0 root         (0) root         (0)    12212 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py
+-rw-r--r--   0 root         (0) root         (0)    15009 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/c3po.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.027712 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/agis.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/free_space.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/jedi_did.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/mock_did.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/network_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3818 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/workload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.027712 rucio-34.3.0/lib/rucio/daemons/c3po/utils/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/utils/dataset_cache.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/utils/expiring_list.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/utils/popularity.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/utils/timeseries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.028712 rucio-34.3.0/lib/rucio/daemons/cache/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-34.3.0/lib/rucio/daemons/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6744 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/cache/consumer.py
+-rw-r--r--   0 root         (0) root         (0)    14947 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.029712 rucio-34.3.0/lib/rucio/daemons/conveyor/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25817 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/common.py
+-rw-r--r--   0 root         (0) root         (0)    23645 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/finisher.py
+-rw-r--r--   0 root         (0) root         (0)    16241 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/poller.py
+-rw-r--r--   0 root         (0) root         (0)     7462 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/preparer.py
+-rw-r--r--   0 root         (0) root         (0)     8289 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/receiver.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/stager.py
+-rw-r--r--   0 root         (0) root         (0)    16333 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/submitter.py
+-rw-r--r--   0 root         (0) root         (0)    20351 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/throttler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.030712 rucio-34.3.0/lib/rucio/daemons/follower/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/follower/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/follower/follower.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.030712 rucio-34.3.0/lib/rucio/daemons/hermes/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/hermes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26475 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/hermes/hermes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.031712 rucio-34.3.0/lib/rucio/daemons/judge/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/judge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5772 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/judge/cleaner.py
+-rw-r--r--   0 root         (0) root         (0)     7170 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/judge/evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     6394 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/judge/injector.py
+-rw-r--r--   0 root         (0) root         (0)     5310 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/judge/repairer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.031712 rucio-34.3.0/lib/rucio/daemons/oauthmanager/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/oauthmanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8817 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/oauthmanager/oauthmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.032712 rucio-34.3.0/lib/rucio/daemons/reaper/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/reaper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11222 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/reaper/dark_reaper.py
+-rw-r--r--   0 root         (0) root         (0)    35602 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/reaper/reaper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.032712 rucio-34.3.0/lib/rucio/daemons/replicarecoverer/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/replicarecoverer/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    33152 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.033712 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.033712 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/
+-rw-r--r--   0 root         (0) root         (0)      863 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    16280 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py
+-rw-r--r--   0 root         (0) root         (0)    10413 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.033712 rucio-34.3.0/lib/rucio/daemons/storage/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.034712 rucio-34.3.0/lib/rucio/daemons/storage/consistency/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/storage/consistency/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29562 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/storage/consistency/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.034712 rucio-34.3.0/lib/rucio/daemons/tracer/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/tracer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23764 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/tracer/kronos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.035712 rucio-34.3.0/lib/rucio/daemons/transmogrifier/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/transmogrifier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30581 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/transmogrifier/transmogrifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.035712 rucio-34.3.0/lib/rucio/daemons/undertaker/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/undertaker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/undertaker/undertaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.035712 rucio-34.3.0/lib/rucio/db/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.036712 rucio-34.3.0/lib/rucio/db/sqla/
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4151 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.037712 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.058712 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/
+-rw-r--r--   0 root         (0) root         (0)     3340 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     5272 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py
+-rw-r--r--   0 root         (0) root         (0)     1678 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py
+-rw-r--r--   0 root         (0) root         (0)     8494 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     3782 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     4360 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py
+-rw-r--r--   0 root         (0) root         (0)     3882 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2817 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)     7527 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py
+-rw-r--r--   0 root         (0) root         (0)     3592 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py
+-rw-r--r--   0 root         (0) root         (0)     2777 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     6101 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py
+-rw-r--r--   0 root         (0) root         (0)     5023 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py
+-rw-r--r--   0 root         (0) root         (0)     3568 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py
+-rw-r--r--   0 root         (0) root         (0)     5038 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py
+-rw-r--r--   0 root         (0) root         (0)     3689 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py
+-rw-r--r--   0 root         (0) root         (0)     2614 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py
+-rw-r--r--   0 root         (0) root         (0)     3117 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py
+-rw-r--r--   0 root         (0) root         (0)     5836 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py
+-rw-r--r--   0 root         (0) root         (0)     7344 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py
+-rw-r--r--   0 root         (0) root         (0)     2934 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     9561 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py
+-rw-r--r--   0 root         (0) root         (0)     4748 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py
+-rw-r--r--   0 root         (0) root         (0)     5263 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py
+-rw-r--r--   0 root         (0) root         (0)     4865 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py
+-rw-r--r--   0 root         (0) root         (0)   112134 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/db/sqla/models.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/sautils.py
+-rw-r--r--   0 root         (0) root         (0)    17773 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/session.py
+-rw-r--r--   0 root         (0) root         (0)     6088 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/types.py
+-rw-r--r--   0 root         (0) root         (0)    21426 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.058712 rucio-34.3.0/lib/rucio/rse/
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.062712 rucio-34.3.0/lib/rucio/rse/protocols/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7199 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/bittorrent.py
+-rw-r--r--   0 root         (0) root         (0)     4603 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/dummy.py
+-rw-r--r--   0 root         (0) root         (0)    29100 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/gfal.py
+-rw-r--r--   0 root         (0) root         (0)     9730 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/globus.py
+-rw-r--r--   0 root         (0) root         (0)     3411 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/gsiftp.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/http_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/ngarc.py
+-rw-r--r--   0 root         (0) root         (0)    10400 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/posix.py
+-rw-r--r--   0 root         (0) root         (0)    22703 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    15260 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/rclone.py
+-rw-r--r--   0 root         (0) root         (0)     5501 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/rfio.py
+-rw-r--r--   0 root         (0) root         (0)    14655 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/srm.py
+-rw-r--r--   0 root         (0) root         (0)    17473 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     8127 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/storm.py
+-rw-r--r--   0 root         (0) root         (0)    22168 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/webdav.py
+-rw-r--r--   0 root         (0) root         (0)    12571 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/xrootd.py
+-rw-r--r--   0 root         (0) root         (0)    37238 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/rsemanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.062712 rucio-34.3.0/lib/rucio/tests/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8907 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/tests/common_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.064712 rucio-34.3.0/lib/rucio/transfertool/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8342 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/bittorrent.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/bittorrent_driver.py
+-rw-r--r--   0 root         (0) root         (0)     4966 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py
+-rw-r--r--   0 root         (0) root         (0)    72157 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/fts3.py
+-rw-r--r--   0 root         (0) root         (0)     6156 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/fts3_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     7716 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/globus.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/globus_library.py
+-rw-r--r--   0 root         (0) root         (0)     2859 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7752 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/transfertool.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-05-06 11:04:02.000000 rucio-34.3.0/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.064712 rucio-34.3.0/lib/rucio/web/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.065712 rucio-34.3.0/lib/rucio/web/rest/
+-rwxr-xr-x   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.065712 rucio-34.3.0/lib/rucio/web/rest/flaskapi/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.071713 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7791 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py
+-rw-r--r--   0 root         (0) root         (0)    36983 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/accounts.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/archives.py
+-rw-r--r--   0 root         (0) root         (0)    61047 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/auth.py
+-rw-r--r--   0 root         (0) root         (0)    16148 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/common.py
+-rw-r--r--   0 root         (0) root         (0)    10143 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/config.py
+-rw-r--r--   0 root         (0) root         (0)     7714 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/credentials.py
+-rw-r--r--   0 root         (0) root         (0)    80867 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/dids.py
+-rw-r--r--   0 root         (0) root         (0)     4706 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/export.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     7894 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/identities.py
+-rw-r--r--   0 root         (0) root         (0)     5259 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/import.py
+-rw-r--r--   0 root         (0) root         (0)    12009 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12990 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/locks.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/main.py
+-rw-r--r--   0 root         (0) root         (0)     7785 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/ping.py
+-rw-r--r--   0 root         (0) root         (0)    13331 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/redirect.py
+-rw-r--r--   0 root         (0) root         (0)    72711 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/replicas.py
+-rw-r--r--   0 root         (0) root         (0)    41622 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/requests.py
+-rw-r--r--   0 root         (0) root         (0)    81948 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/rses.py
+-rw-r--r--   0 root         (0) root         (0)    32189 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/rules.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/scopes.py
+-rw-r--r--   0 root         (0) root         (0)    24151 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.071713 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/templates/
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-07-27 12:40:37.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-07-27 12:40:37.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/traces.py
+-rw-r--r--   0 root         (0) root         (0)     9154 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/vos.py
+-rw-r--r--   0 root         (0) root         (0)      725 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/main.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/ping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.089713 rucio-34.3.0/lib/rucio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25997 2024-05-06 12:44:05.000000 rucio-34.3.0/lib/rucio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2024-05-06 09:19:47.000000 rucio-34.3.0/pylintrc
+-rw-r--r--   0 root         (0) root         (0)     4349 2024-05-06 09:19:47.000000 rucio-34.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5235 2024-05-06 11:03:53.000000 rucio-34.3.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-06 12:44:06.095713 rucio-34.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-05-06 12:44:02.000000 rucio-34.3.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-05-06 09:19:47.000000 rucio-34.3.0/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.088713 rucio-34.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10677 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15923 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    14964 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23265 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12425 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107450 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6942 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    96724 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    23870 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7728 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28183 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    58823 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29517 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16419 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10869 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38301 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10106 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57290 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5258 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22277 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20429 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54332 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   108359 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7662 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27487 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62453 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    38868 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22796 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    17257 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    13033 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75080 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13184 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8940 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4799 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     3979 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7746 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    91949 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)    13848 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_schema_cms.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48389 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    55587 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    25254 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8924 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_transfer_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    15575 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.089713 rucio-34.3.0/tools/
+-rwxr-xr-x   0 root         (0) root         (0)     1259 2024-05-06 09:19:47.000000 rucio-34.3.0/tools/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     6163 2024-05-06 09:19:47.000000 rucio-34.3.0/tools/merge_rucio_configs.py
+-rwxr-xr-x   0 root         (0) root         (0)     1351 2024-05-06 09:19:47.000000 rucio-34.3.0/tools/reset_database.py
```

### Comparing `rucio-34.2.0/AUTHORS.rst` & `rucio-34.3.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/LICENSE` & `rucio-34.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/MANIFEST.in` & `rucio-34.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/PKG-INFO` & `rucio-34.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio
-Version: 34.2.0
+Version: 34.3.0
 Summary: Rucio Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rucio-34.2.0/README.rst` & `rucio-34.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio` & `rucio-34.3.0/bin/rucio`

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

### Comparing `rucio-34.2.0/bin/rucio-abacus-account` & `rucio-34.3.0/bin/rucio-abacus-account`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-abacus-collection-replica` & `rucio-34.3.0/bin/rucio-abacus-collection-replica`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-abacus-rse` & `rucio-34.3.0/bin/rucio-abacus-rse`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-admin` & `rucio-34.3.0/bin/rucio-admin`

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

### Comparing `rucio-34.2.0/bin/rucio-atropos` & `rucio-34.3.0/bin/rucio-atropos`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-auditor` & `rucio-34.3.0/bin/rucio-auditor`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
             for rse in rses:
                 queue.put((rse, 1))
 
             time.sleep(RETRY_AFTER)
 
             # Avoid infinite loop if an alternative check() implementation doesn't
-            # decrement the number of attemps and keeps pushing failed checks.
+            # decrement the number of attempts and keeps pushing failed checks.
             tmp_list = []
             while not retry.empty():
                 tmp_list.append(retry.get())
 
             for each in tmp_list:
                 queue.put(each)
 
@@ -145,15 +145,15 @@
         proc.join()
 
 
 def get_parser():
     """
     Returns the argparse parser.
     """
-    parser = argparse.ArgumentParser(description="The auditor daemon is the one responsable for the detection of inconsistencies on storage, i.e.: dark data discovery.",
+    parser = argparse.ArgumentParser(description="The auditor daemon is the one responsible for the detection of inconsistencies on storage, i.e.: dark data discovery.",
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument(
         '--nprocs',
         help='Number subprocess, each subprocess check a fraction of the DDM '
              'Endpoints in sequence (default: 1).',
         default=1,
         type=int,
```

### Comparing `rucio-34.2.0/bin/rucio-automatix` & `rucio-34.3.0/bin/rucio-automatix`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from rucio.daemons.automatix.automatix import run, stop
 
 
 def get_parser():
     """
     Returns the argparse parser.
     """
-    parser = argparse.ArgumentParser(description="Automatix is a daemon used to inject random generated files to an RSE. It is used to continuosly check that an RSE is reachable and operating as spected.")
+    parser = argparse.ArgumentParser(description="Automatix is a daemon used to inject random generated files to an RSE. It is used to continuously check that an RSE is reachable and operating as expected.")
     parser.add_argument("--run-once", action="store_true", default=False, help='Runs one loop iteration')
     parser.add_argument("--input-file", action="store", default="/opt/rucio/etc/automatix.json", type=str, help='Automatix configuration')
     parser.add_argument("--threads-per-process", action="store", default=1, type=int, help='Total number of workers per process')
     parser.add_argument('--sleep-time', action="store", default=-1, type=int, help='Concurrency control: thread sleep time after each chunk of work')
     return parser
```

### Comparing `rucio-34.2.0/bin/rucio-bb8` & `rucio-34.3.0/bin/rucio-bb8`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-c3po` & `rucio-34.3.0/bin/rucio-c3po`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-cache-client` & `rucio-34.3.0/bin/rucio-cache-client`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-cache-consumer` & `rucio-34.3.0/bin/rucio-cache-consumer`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-conveyor-finisher` & `rucio-34.3.0/bin/rucio-conveyor-finisher`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from rucio.daemons.conveyor.finisher import run, stop
 
 
 def get_parser():
     """
     Returns the argparse parser.
     """
-    parser = argparse.ArgumentParser(description="Conveyor is a group of daemons to manage file transfers. The conveyor-finisher is the resposible to update Rucio internal state after the transfer has finished.")
+    parser = argparse.ArgumentParser(description="Conveyor is a group of daemons to manage file transfers. The conveyor-finisher is the responsible to update Rucio internal state after the transfer has finished.")
     parser.add_argument("--run-once", action="store_true", default=False,
                         help='One iteration only')
     parser.add_argument("--total-threads", action="store", default=1, type=int,
                         help='Concurrency control: total number of threads per process')
     parser.add_argument("--db-bulk", action="store", default=1000, type=int,
                         help='Bulk control: number of transfers per db query')
     parser.add_argument("--bulk", action="store", default=100, type=int,
```

### Comparing `rucio-34.2.0/bin/rucio-conveyor-poller` & `rucio-34.3.0/bin/rucio-conveyor-poller`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-conveyor-preparer` & `rucio-34.3.0/bin/rucio-conveyor-preparer`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-conveyor-receiver` & `rucio-34.3.0/bin/rucio-conveyor-receiver`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-conveyor-stager` & `rucio-34.3.0/bin/rucio-conveyor-stager`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-conveyor-submitter` & `rucio-34.3.0/bin/rucio-conveyor-submitter`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     parser = argparse.ArgumentParser(description="The Conveyor-Submitter daemon is responsible for managing non-tape file transfers. It prepares transfer jobs and submits them to the transfertool.", epilog='''
 Upload a file and create a replication rule::
 
   $ rucio upload --scope mock --rse MOCK --name file filename.txt
   $ rucio add-rule mock:file 1 MOCK2
   $ rucio-admin rse add-distance MOCK2 MOCK --distance 1
 
-The rule should replicate the file from RSE MOCK to RSE MOCK2. Therefor a distance between these RSEs is needed.
+The rule should replicate the file from RSE MOCK to RSE MOCK2. Therefore a distance between these RSEs is needed.
 
 Check transfer requests for the DID::
 
     $ python
     from rucio.db.sqla import session,models
     session.get_session().query(models.Request).filter_by(scope='mock', name='file').first()
     # {'request_type': TRANSFER, 'state': QUEUED', ...}
@@ -52,15 +52,15 @@
 Check again the transfer requests for the DID::
 
     $ python
     from rucio.db.sqla import session,models
     session.get_session().query(models.Request).filter_by(scope='mock', name='file').first()
     # {'request_type': TRANSFER, 'state': SUBMITTED', ...}
 
-A tranfer request got created by executing the transfer. Depending on the transfer submission, the request state can be different. In this example the transfer got submitted successfully.
+A transfer request got created by executing the transfer. Depending on the transfer submission, the request state can be different. In this example the transfer got submitted successfully.
 
 When run in multi-VO mode, by default the daemon will run on RSEs from all VOs::
 
   $ rucio-conveyor-submitter --run-once
   2020-07-29 13:51:09,436 5784    INFO    This instance will work on VOs: def, abc, xyz, 123
   2020-07-29 13:51:13,315 5784    INFO    RSE selection: automatic for relevant VOs
   2020-07-29 13:51:13,316 5784    INFO    starting submitter threads
```

### Comparing `rucio-34.2.0/bin/rucio-conveyor-throttler` & `rucio-34.3.0/bin/rucio-conveyor-throttler`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-dark-reaper` & `rucio-34.3.0/bin/rucio-dark-reaper`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-dumper` & `rucio-34.3.0/bin/rucio-dumper`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-follower` & `rucio-34.3.0/bin/rucio-follower`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-hermes` & `rucio-34.3.0/bin/rucio-hermes`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-judge-cleaner` & `rucio-34.3.0/bin/rucio-judge-cleaner`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-judge-evaluator` & `rucio-34.3.0/bin/rucio-judge-evaluator`

 * *Files 0% similar despite different names*

```diff
@@ -109,19 +109,19 @@
 
 Check the replicas for the DID mock:file::
 
   $ python
   from rucio.db.sqla import session, models
   session.get_session().query(models.RSEFileAssociation).filter_by(name='file', scope='mock').first()
   // [{'name': 'file','lock_cnt': 1, 'state': COPYING, 'scope': 'mock', 'rse_id': 'f81f366593754c01b0c340fa5ea0ab90'},
-  //  {'scope': 'mock', 'rse_id': '1330d5daee37474c88ba888101d7b859', 'name': 'file', 'state': AVAIABLE, 'lock_cnt': 1}]
+  //  {'scope': 'mock', 'rse_id': '1330d5daee37474c88ba888101d7b859', 'name': 'file', 'state': AVAILABLE, 'lock_cnt': 1}]
 
 The DID mock:file has now two replicas with one lock each.
 As the file replica is attached to the dataset and the rule for the dataset specifies another RSE MOCK instead of the upload RSE, it has to be replicated to this RSE.
-Therefor a second replica in state COPYING got created on RSE MOCK.
+Therefore a second replica in state COPYING got created on RSE MOCK.
     ''', formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("--run-once", action="store_true", default=False, help='One iteration only')
     parser.add_argument("--threads", action="store", default=1, type=int, help='Concurrency control: total number of threads for this process')
     parser.add_argument('--sleep-time', action="store", default=30, type=int, help='Concurrency control: thread sleep time after each chunk of work')
     parser.add_argument("--did-limit", action="store", default=100, type=int, help='Maximum number of dids to evaluate')
     return parser
```

### Comparing `rucio-34.2.0/bin/rucio-judge-injector` & `rucio-34.3.0/bin/rucio-judge-injector`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-judge-repairer` & `rucio-34.3.0/bin/rucio-judge-repairer`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-kronos` & `rucio-34.3.0/bin/rucio-kronos`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-minos` & `rucio-34.3.0/bin/rucio-minos`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-minos-temporary-expiration` & `rucio-34.3.0/bin/rucio-minos-temporary-expiration`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-necromancer` & `rucio-34.3.0/bin/rucio-necromancer`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 def get_parser():
     """
     Returns the argparse parser.
     """
     parser = argparse.ArgumentParser(description="The Necromancer daemon is responsible for managing bad replicas. If a replica that got declared bad has other replicas, it will try to recover it by requesting a new transfer. If there are no replicas anymore, then the file gets marked as lost.", epilog='''
 Lost replica:
 In this example the file gets uploaded and will only have this replica as there are no replication rules. If it gets declared bad, there will be no replica to recover from.
-Therefor the replica gets marked as lost.
+Therefore the replica gets marked as lost.
 
 Upload a file::
 
   $ rucio upload --scope mock --rse MOCK --name file filename.txt
 
 Check replicas::
```

### Comparing `rucio-34.2.0/bin/rucio-oauth-manager` & `rucio-34.3.0/bin/rucio-oauth-manager`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-OAuth Manager is a daemon which is reponsible for:
+OAuth Manager is a daemon which is responsible for:
 - deletion of expired access tokens (in case there is a valid refresh token, expired access tokens will be kept until refresh_token expires as well.)
 - deletion of expired OAuth session parameters
 - refreshing access tokens via their refresh tokens.
 """
 
 import argparse
 import signal
@@ -28,15 +28,15 @@
 
 def get_parser():
     """
     Returns the argparse parser.
     """
     parser = argparse.ArgumentParser(description='''
 
-OAuth Manager is a daemon which is reponsible for:
+OAuth Manager is a daemon which is responsible for:
 - deletion of expired access tokens (in case there is a valid refresh token,
   expired access tokens will be kept until refresh_token expires as well.)
 - deletion of expired OAuth session parameters
 - refreshing access tokens via their refresh tokens.
 
 These 3 actions run consequently one after another in a loop with a sleeptime of 'looprate' seconds.
 The maximum number of DB rows (tokens, parameters, refresh tokens) on which the script will operate
```

### Comparing `rucio-34.2.0/bin/rucio-reaper` & `rucio-34.3.0/bin/rucio-reaper`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-replica-recoverer` & `rucio-34.3.0/bin/rucio-replica-recoverer`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 Only file_available_suspicious should be the one on which the daemon takes action and declares it as bad.
 
 $ id0=`uuidgen`
 $ id1=`uuidgen`
 $ id2=`uuidgen`
 $ id3=`uuidgen`
-$ echo "file available on MOCK_RECOVERY and decalred suspicious on MOCK_SUSPICIOUS  (11 times)" > /tmp/file_available_suspicious'_'$id1
+$ echo "file available on MOCK_RECOVERY and declared suspicious on MOCK_SUSPICIOUS  (11 times)" > /tmp/file_available_suspicious'_'$id1
 $ echo "file available on MOCK_RECOVERY and declared suspicious on MOCK_SUSPICIOUS  (11 times) and 1 time bad/deleted/lost on MOCK_SUSPICIOUS" > /tmp/file_available_suspicious_and_bad'_'$id2
 $ echo "file declared as unavailable on MOCK_RECOVERY and declared as suspicious 11 times on MOCK_SUSPICIOUS" > /tmp/file_notavailable_suspicious'_'$id3
 
 Uploading the files created above to rucio:
 -------------------------------------------------------------------
 
 rucio add-dataset mock:dataset_of_suspicious_replicas'_'$id0
@@ -224,15 +224,15 @@
 
 Note that attempting the use the ``--vos`` argument when in single-VO mode will have no affect::
 
   $ rucio-replica-recoverer --run-once --vos abc xyz
   2020-07-28 15:21:33,349 5488    WARNING Ignoring argument vos, this is only applicable in a multi-VO setup.
 ''', formatter_class=argparse.RawDescriptionHelpFormatter)  # NOQA: E501
     parser.add_argument("--nattempts", action="store", default=5, help='Minimum count of suspicious file replica appearance in bad_replicas table. Default value is 5.')
-    parser.add_argument("--younger-than", action="store", default=5, help='Consider all file replicas logged in bad_replicas table since speicified number of younger-than days. Default value is 5.')
+    parser.add_argument("--younger-than", action="store", default=5, help='Consider all file replicas logged in bad_replicas table since specified number of younger-than days. Default value is 5.')
     parser.add_argument('--vos', nargs='+', type=str, help='Optional list of VOs to consider. Only used in multi-VO mode.')
     parser.add_argument("--run-once", action="store_true", default=False, help='One iteration only.')
     parser.add_argument("--limit-suspicious-files-on-rse", action="store", default=5, help='Maximum number of suspicious replicas on an RSE before that RSE is considered problematic and the suspicious replicas on that RSE are declared "TEMPORARY_UNAVAILABLE". Default value is 5.')
     parser.add_argument('--json-file-name', action="store", default="/opt/rucio/etc/suspicious_replica_recoverer.json", type=str, help='Name of the json file that that contains the policies which will be used by the suspicious replica recoverer.')
     parser.add_argument('--sleep-time', action="store", default=3600, type=int, help='Concurrency control: Thread sleep time after each chunk of work.')
     parser.add_argument('--active-mode', action="store_true", default=False, help='If NOT specified, the daemon will run without taking any actions on any files. In either case, the log file will be produced normally.')
     return parser
```

### Comparing `rucio-34.2.0/bin/rucio-rse-decommissioner` & `rucio-34.3.0/bin/rucio-rse-decommissioner`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-storage-consistency-actions` & `rucio-34.3.0/bin/rucio-storage-consistency-actions`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-transmogrifier` & `rucio-34.3.0/bin/rucio-transmogrifier`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/bin/rucio-undertaker` & `rucio-34.3.0/bin/rucio-undertaker`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/etc/alembic.ini.template` & `rucio-34.3.0/etc/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/etc/alembic_offline.ini.template` & `rucio-34.3.0/etc/alembic_offline.ini.template`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/etc/ldap.cfg.template` & `rucio-34.3.0/etc/ldap.cfg.template`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # - Cheng-Hsi Chao, <cheng-hsi.chaos@cern.ch>, 2014
 
 [ldap]
 ldap_host = ldap-host.domain.name
 baseDN = dc=foo,dc=bar,dc=domain,dc=
 searchFilter = (objectClass=OpenLDAPperson)
 
-# set as DEFAULT to use annonymous bind
+# set as DEFAULT to use anonymous bind
 username = DEFAULT
 # Leave blank for prompt
 password =
 
 cacertfile = /etc/grid-security/certificates
 certfile = /etc/grid-security/hostcert.pem
 keyfile = /etc/grid-security/hostkey.pem
```

### Comparing `rucio-34.2.0/etc/mail_templates/rule_approval_request.tmpl` & `rucio-34.3.0/etc/mail_templates/rule_approval_request.tmpl`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/etc/mail_templates/rule_ok_notification.tmpl` & `rucio-34.3.0/etc/mail_templates/rule_ok_notification.tmpl`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/etc/rse-accounts.cfg.template` & `rucio-34.3.0/etc/rse-accounts.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/etc/rucio.cfg.atlas.client.template` & `rucio-34.3.0/etc/rucio.cfg.atlas.client.template`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/etc/rucio.cfg.template` & `rucio-34.3.0/etc/rucio.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/etc/rucio_multi_vo.cfg.template` & `rucio-34.3.0/etc/rucio_multi_vo.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/__init__.py` & `rucio-34.3.0/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/alembicrevision.py` & `rucio-34.3.0/lib/rucio/alembicrevision.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/__init__.py` & `rucio-34.3.0/lib/rucio/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/account.py` & `rucio-34.3.0/lib/rucio/api/account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/account_limit.py` & `rucio-34.3.0/lib/rucio/api/account_limit.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 def get_rse_account_usage(rse, vo='def', *, session: "Session"):
     """
     Returns the account limit and usage for all for all accounts on a RSE.
 
     :param rse:      The RSE name.
     :param vo:       The VO to act on.
     :param session:  The database session in use.
-    :return:         List of dictionnaries.
+    :return:         List of dictionaries.
     """
     rse_id = get_rse_id(rse=rse, vo=vo, session=session)
 
     return [api_update_return_dict(d, session=session) for d in account_limit_core.get_rse_account_usage(rse_id=rse_id, session=session)]
 
 
 @read_session
```

### Comparing `rucio-34.2.0/lib/rucio/api/authentication.py` & `rucio-34.3.0/lib/rucio/api/authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/config.py` & `rucio-34.3.0/lib/rucio/api/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Optional
 
 from rucio.api import permission
 from rucio.common import exception
 from rucio.common.config import convert_to_any_type
 from rucio.core import config
 from rucio.db.sqla.session import read_session, transactional_session
 
@@ -28,15 +28,15 @@
 
 - File handling methods unnecessary.
 - Convenience methods getint/getfloat/getboolean are superseded by auto-coercing get.
 """
 
 
 @read_session
-def sections(issuer=None, vo='def', *, session: "Session"):
+def sections(issuer: Optional[str] = None, vo: str = 'def', *, session: "Session") -> list[str]:
     """
     Return a list of the sections available.
 
     :param issuer: The issuer account.
     :param vo: The VO to act on.
     :param session: The database session in use.
     :returns: ['section_name', ...]
@@ -45,15 +45,15 @@
     kwargs = {'issuer': issuer}
     if not permission.has_permission(issuer=issuer, vo=vo, action='config_sections', kwargs=kwargs, session=session):
         raise exception.AccessDenied('%s cannot retrieve sections' % issuer)
     return config.sections(session=session)
 
 
 @transactional_session
-def add_section(section, issuer=None, vo='def', *, session: "Session"):
+def add_section(section: str, issuer: Optional[str] = None, vo: str = 'def', *, session: "Session") -> None:
     """
     Add a section to the configuration.
 
     :param section: The name of the section.
     :param issuer: The issuer account.
     :param session: The database session in use.
     :param vo: The VO to act on.
@@ -62,15 +62,15 @@
     kwargs = {'issuer': issuer, 'section': section}
     if not permission.has_permission(issuer=issuer, vo=vo, action='config_add_section', kwargs=kwargs, session=session):
         raise exception.AccessDenied('%s cannot add section %s' % (issuer, section))
     return config.add_section(section, session=session)
 
 
 @read_session
-def has_section(section, issuer=None, vo='def', *, session: "Session"):
+def has_section(section: str, issuer: Optional[str] = None, vo: str = 'def', *, session: "Session") -> bool:
     """
     Indicates whether the named section is present in the configuration.
 
     :param section: The name of the section.
     :param issuer: The issuer account.
     :param vo: The VO to act on.
     :param session: The database session in use.
@@ -80,15 +80,15 @@
     kwargs = {'issuer': issuer, 'section': section}
     if not permission.has_permission(issuer=issuer, vo=vo, action='config_has_section', kwargs=kwargs, session=session):
         raise exception.AccessDenied('%s cannot check existence of section %s' % (issuer, section))
     return config.has_section(section, session=session)
 
 
 @read_session
-def options(section, issuer=None, vo='def', *, session: "Session"):
+def options(section: str, issuer: Optional[str] = None, vo: str = 'def', *, session: "Session") -> list[str]:
     """
     Returns a list of options available in the specified section.
 
     :param section: The name of the section.
     :param issuer: The issuer account.
     :param vo: The VO to act on.
     :param session: The database session in use.
@@ -98,15 +98,15 @@
     kwargs = {'issuer': issuer, 'section': section}
     if not permission.has_permission(issuer=issuer, vo=vo, action='config_options', kwargs=kwargs, session=session):
         raise exception.AccessDenied('%s cannot retrieve options from section %s' % (issuer, section))
     return config.options(section, session=session)
 
 
 @read_session
-def has_option(section, option, issuer=None, vo='def', *, session: "Session"):
+def has_option(section: str, option: str, issuer: Optional[str] = None, vo: str = 'def', *, session: "Session") -> bool:
     """
     Check if the given section exists and contains the given option.
 
     :param section: The name of the section.
     :param option: The name of the option.
     :param issuer: The issuer account.
     :param vo: The VO to act on.
@@ -117,15 +117,15 @@
     kwargs = {'issuer': issuer, 'section': section, 'option': option}
     if not permission.has_permission(issuer=issuer, vo=vo, action='config_has_option', kwargs=kwargs, session=session):
         raise exception.AccessDenied('%s cannot check existence of option %s from section %s' % (issuer, option, section))
     return config.has_option(section, option, session=session)
 
 
 @read_session
-def get(section, option, issuer=None, vo='def', *, session: "Session"):
+def get(section: str, option: str, issuer: Optional[str] = None, vo: str = 'def', *, session: "Session") -> Any:
     """
     Get an option value for the named section. Value can be auto-coerced to int, float, and bool; string otherwise.
 
     Caveat emptor: Strings, regardless the case, matching 'on'/off', 'true'/'false', 'yes'/'no' are converted to bool.
                    0/1 are converted to int, and not to bool.
 
     :param section: The name of the section.
@@ -139,15 +139,15 @@
     kwargs = {'issuer': issuer, 'section': section, 'option': option}
     if not permission.has_permission(issuer=issuer, vo=vo, action='config_get', kwargs=kwargs, session=session):
         raise exception.AccessDenied('%s cannot retrieve option %s from section %s' % (issuer, option, section))
     return config.get(section, option, session=session, convert_type_fnc=convert_to_any_type)
 
 
 @read_session
-def items(section, issuer=None, vo='def', *, session: "Session"):
+def items(section: str, issuer: Optional[str] = None, vo: str = 'def', *, session: "Session") -> list[tuple[str, Any]]:
     """
     Return a list of (option, value) pairs for each option in the given section. Values are auto-coerced as in get().
 
     :param section: The name of the section.
     :param value: The content of the value.
     :param issuer: The issuer account.
     :param vo: The VO to act on.
@@ -158,15 +158,15 @@
     kwargs = {'issuer': issuer, 'section': section}
     if not permission.has_permission(issuer=issuer, vo=vo, action='config_items', kwargs=kwargs, session=session):
         raise exception.AccessDenied('%s cannot retrieve options and values from section %s' % (issuer, section))
     return config.items(section, session=session, convert_type_fnc=convert_to_any_type)
 
 
 @transactional_session
-def set(section, option, value, issuer=None, vo='def', *, session: "Session"):
+def set(section: str, option: str, value: Any, issuer: Optional[str] = None, vo: str = 'def', *, session: "Session") -> None:
     """
     Set the given option to the specified value.
 
     :param section: The name of the section.
     :param option: The name of the option.
     :param value: The content of the value.
     :param issuer: The issuer account.
@@ -177,15 +177,15 @@
     kwargs = {'issuer': issuer, 'section': section, 'option': option, 'value': value}
     if not permission.has_permission(issuer=issuer, vo=vo, action='config_set', kwargs=kwargs, session=session):
         raise exception.AccessDenied('%s cannot set option %s to %s in section %s' % (issuer, option, value, section))
     return config.set(section, option, value, session=session)
 
 
 @transactional_session
-def remove_section(section, issuer=None, vo='def', *, session: "Session"):
+def remove_section(section: str, issuer: Optional[str] = None, vo: str = 'def', *, session: "Session") -> bool:
     """
     Remove the specified option from the specified section.
 
     :param section: The name of the section.
     :param issuer: The issuer account.
     :param vo: The VO to act on.
     :param session: The database session in use.
@@ -195,15 +195,15 @@
     kwargs = {'issuer': issuer, 'section': section}
     if not permission.has_permission(issuer=issuer, vo=vo, action='config_remove_section', kwargs=kwargs, session=session):
         raise exception.AccessDenied('%s cannot remove section %s' % (issuer, section))
     return config.remove_section(section, session=session)
 
 
 @transactional_session
-def remove_option(section, option, issuer=None, vo='def', *, session: "Session"):
+def remove_option(section: str, option: str, issuer: Optional[str] = None, vo: str = 'def', *, session: "Session") -> bool:
     """
     Remove the specified section from the configuration.
 
     :param section: The name of the section.
     :param option: The name of the option.
     :param issuer: The issuer account.
     :param vo: The VO to act on.
```

### Comparing `rucio-34.2.0/lib/rucio/api/credential.py` & `rucio-34.3.0/lib/rucio/api/credential.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/did.py` & `rucio-34.3.0/lib/rucio/api/did.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from collections.abc import Iterator
 from copy import deepcopy
 from typing import TYPE_CHECKING
 
 import rucio.api.permission
 from rucio.common.constants import RESERVED_KEYS
 from rucio.common.exception import RucioException
 from rucio.common.schema import validate_schema
@@ -24,15 +25,15 @@
 from rucio.core import did, naming_convention
 from rucio.core import meta_conventions as meta_convention_core
 from rucio.core.rse import get_rse_id
 from rucio.db.sqla.constants import DIDType
 from rucio.db.sqla.session import read_session, stream_session, transactional_session
 
 if TYPE_CHECKING:
-    from typing import Any, Iterator, Optional
+    from typing import Any, Optional
 
     from sqlalchemy.orm import Session
 
 
 @stream_session
 def list_dids(scope, filters, did_type='collection', ignore_case=False, limit=None, offset=None, long=False, recursive=False, vo='def', *, session: "Session"):
     """
```

### Comparing `rucio-34.2.0/lib/rucio/api/dirac.py` & `rucio-34.3.0/lib/rucio/api/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/exporter.py` & `rucio-34.3.0/lib/rucio/api/exporter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/heartbeat.py` & `rucio-34.3.0/lib/rucio/api/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/identity.py` & `rucio-34.3.0/lib/rucio/api/identity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/importer.py` & `rucio-34.3.0/lib/rucio/api/importer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/lifetime_exception.py` & `rucio-34.3.0/lib/rucio/api/lifetime_exception.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/lock.py` & `rucio-34.3.0/lib/rucio/api/lock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/meta_conventions.py` & `rucio-34.3.0/lib/rucio/api/meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/permission.py` & `rucio-34.3.0/lib/rucio/api/permission.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/quarantined_replica.py` & `rucio-34.3.0/lib/rucio/api/quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/replica.py` & `rucio-34.3.0/lib/rucio/api/replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/request.py` & `rucio-34.3.0/lib/rucio/api/request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/rse.py` & `rucio-34.3.0/lib/rucio/api/rse.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
     Returns all matching protocols (including detailed information) for the given RSE.
 
     :param rse: The RSE name.
     :param issuer: The issuer account.
     :param vo: The VO to act on.
     :param session: The database session in use.
 
-    :returns: A dict with all supported protocols and their attibutes.
+    :returns: A dict with all supported protocols and their attributes.
     """
     rse_id = rse_module.get_rse_id(rse=rse, vo=vo, session=session)
     return rse_module.get_rse_protocols(rse_id, session=session)
 
 
 @transactional_session
 def del_protocols(rse, scheme, issuer, vo='def', hostname=None, port=None, *, session: "Session"):
@@ -436,15 +436,15 @@
 
 @transactional_session
 def update_rse(rse, parameters, issuer, vo='def', *, session: "Session"):
     """
     Update RSE properties like availability or name.
 
     :param rse: the name of the new rse.
-    :param parameters: A dictionnary with property (name, read, write, delete as keys).
+    :param parameters: A dictionary with property (name, read, write, delete as keys).
     :param issuer: The issuer account.
     :param vo: The VO to act on.
     :param session: The database session in use.
 
     :raises RSENotFound: If RSE is not found.
     """
     rse_id = rse_module.get_rse_id(rse=rse, vo=vo, session=session)
```

### Comparing `rucio-34.2.0/lib/rucio/api/rule.py` & `rucio-34.3.0/lib/rucio/api/rule.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/scope.py` & `rucio-34.3.0/lib/rucio/api/scope.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/subscription.py` & `rucio-34.3.0/lib/rucio/api/subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/api/vo.py` & `rucio-34.3.0/lib/rucio/api/vo.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Optional
 
 from rucio.api.permission import has_permission
 from rucio.common import exception
 from rucio.common.schema import validate_schema
 from rucio.common.types import InternalAccount
 from rucio.core import identity
 from rucio.core import vo as vo_core
@@ -24,15 +24,15 @@
 from rucio.db.sqla.session import read_session, transactional_session
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
 
 @transactional_session
-def add_vo(new_vo, issuer, description=None, email=None, vo='def', *, session: "Session"):
+def add_vo(new_vo: str, issuer: str, description: Optional[str] = None, email: Optional[str] = None, vo: str = 'def', *, session: "Session") -> None:
     '''
     Add a new VO.
 
     :param new_vo: The name/tag of the VO to add (3 characters).
     :param description: A description of the VO. e.g the full name or a brief description
     :param email: A contact for the VO.
     :param issuer: The user issuing the command.
@@ -47,15 +47,15 @@
     if not has_permission(issuer=issuer, action='add_vo', kwargs=kwargs, vo=vo, session=session):
         raise exception.AccessDenied('Account {} cannot add a VO'.format(issuer))
 
     vo_core.add_vo(vo=new_vo, description=description, email=email, session=session)
 
 
 @read_session
-def list_vos(issuer, vo='def', *, session: "Session"):
+def list_vos(issuer: str, vo: str = 'def', *, session: "Session") -> list[dict[str, Any]]:
     '''
     List the VOs.
 
     :param issuer: The user issuing the command.
     :param vo: The vo of the user issuing the command.
     :param session: The database session in use.
     '''
@@ -63,15 +63,26 @@
     if not has_permission(issuer=issuer, action='list_vos', kwargs=kwargs, vo=vo, session=session):
         raise exception.AccessDenied('Account {} cannot list VOs'.format(issuer))
 
     return vo_core.list_vos(session=session)
 
 
 @transactional_session
-def recover_vo_root_identity(root_vo, identity_key, id_type, email, issuer, default=False, password=None, vo='def', *, session: "Session"):
+def recover_vo_root_identity(
+    root_vo: str,
+    identity_key: str,
+    id_type: str,
+    email: str,
+    issuer: str,
+    default: bool = False,
+    password: Optional[str] = None,
+    vo: str = 'def',
+    *,
+    session: "Session"
+) -> None:
     """
     Adds a membership association between identity and the root account for given VO.
 
     :param root_vo: The VO whose root needs recovery
     :param identity_key: The identity key name. For example x509 DN, or a username.
     :param id_type: The type of the authentication (x509, gss, userpass, ssh, saml).
     :param email: The Email address associated with the identity.
@@ -89,15 +100,15 @@
     account = InternalAccount('root', vo=root_vo)
 
     return identity.add_account_identity(identity=identity_key, type_=IdentityType[id_type.upper()], default=default,
                                          email=email, account=account, password=password, session=session)
 
 
 @transactional_session
-def update_vo(updated_vo, parameters, issuer, vo='def', *, session: "Session"):
+def update_vo(updated_vo: str, parameters: dict[str, Any], issuer: str, vo: str = 'def', *, session: "Session") -> None:
     """
     Update VO properties (email, description).
 
     :param updated_vo: The VO to update.
     :param parameters: A dictionary with the new properties.
     :param issuer: The user issuing the command.
     :param vo: The VO of the user issusing the command.
```

### Comparing `rucio-34.2.0/lib/rucio/client/__init__.py` & `rucio-34.3.0/lib/rucio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/accountclient.py` & `rucio-34.3.0/lib/rucio/client/accountclient.py`

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

### Comparing `rucio-34.2.0/lib/rucio/client/accountlimitclient.py` & `rucio-34.3.0/lib/rucio/client/accountlimitclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/baseclient.py` & `rucio-34.3.0/lib/rucio/client/baseclient.py`

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

### Comparing `rucio-34.2.0/lib/rucio/client/client.py` & `rucio-34.3.0/lib/rucio/client/client.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/configclient.py` & `rucio-34.3.0/lib/rucio/client/configclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/credentialclient.py` & `rucio-34.3.0/lib/rucio/client/credentialclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/didclient.py` & `rucio-34.3.0/lib/rucio/client/didclient.py`

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

### Comparing `rucio-34.2.0/lib/rucio/client/diracclient.py` & `rucio-34.3.0/lib/rucio/client/diracclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/downloadclient.py` & `rucio-34.3.0/lib/rucio/client/downloadclient.py`

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

### Comparing `rucio-34.2.0/lib/rucio/client/exportclient.py` & `rucio-34.3.0/lib/rucio/client/exportclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/fileclient.py` & `rucio-34.3.0/lib/rucio/client/fileclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/importclient.py` & `rucio-34.3.0/lib/rucio/client/importclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/lifetimeclient.py` & `rucio-34.3.0/lib/rucio/client/lifetimeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/lockclient.py` & `rucio-34.3.0/lib/rucio/client/lockclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/metaconventionsclient.py` & `rucio-34.3.0/lib/rucio/client/metaconventionsclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/pingclient.py` & `rucio-34.3.0/lib/rucio/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/replicaclient.py` & `rucio-34.3.0/lib/rucio/client/replicaclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/requestclient.py` & `rucio-34.3.0/lib/rucio/client/requestclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/rseclient.py` & `rucio-34.3.0/lib/rucio/client/rseclient.py`

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

### Comparing `rucio-34.2.0/lib/rucio/client/ruleclient.py` & `rucio-34.3.0/lib/rucio/client/ruleclient.py`

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

### Comparing `rucio-34.2.0/lib/rucio/client/scopeclient.py` & `rucio-34.3.0/lib/rucio/client/scopeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/subscriptionclient.py` & `rucio-34.3.0/lib/rucio/client/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/touchclient.py` & `rucio-34.3.0/lib/rucio/client/touchclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/client/uploadclient.py` & `rucio-34.3.0/lib/rucio/client/uploadclient.py`

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

### Comparing `rucio-34.2.0/lib/rucio/common/__init__.py` & `rucio-34.3.0/lib/rucio/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/cache.py` & `rucio-34.3.0/lib/rucio/common/cache.py`

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

### Comparing `rucio-34.2.0/lib/rucio/common/config.py` & `rucio-34.3.0/lib/rucio/common/config.py`

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

### Comparing `rucio-34.2.0/lib/rucio/common/constraints.py` & `rucio-34.3.0/lib/rucio/common/constraints.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/didtype.py` & `rucio-34.3.0/lib/rucio/common/didtype.py`

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

### Comparing `rucio-34.2.0/lib/rucio/common/dumper/__init__.py` & `rucio-34.3.0/lib/rucio/common/dumper/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,87 +17,98 @@
 import datetime
 import gzip
 import logging
 import os
 import re
 import sys
 import tempfile
+from typing import TYPE_CHECKING, Any, Literal, Optional, Union
 
 import gfal2
 import magic
 import requests
 
 from rucio.common import config
 from rucio.core.rse import get_rse_id, get_rse_protocols
 
+if TYPE_CHECKING:
+    from collections.abc import Iterator
+    from multiprocessing.connection import Connection
+    from types import ModuleType
+    from typing import IO, TextIO
+
+    from _typeshed import FileDescriptorOrPath, GenericPath, StrOrBytesPath
+
+    from rucio.common.types import RSEProtocolDict
+
 
 class HTTPDownloadFailed(Exception):
-    def __init__(self, msg='', code=None):
+    def __init__(self, msg: str = '', code: Optional[str] = None):
         self.code = code
         if code is not None:
             msg = '{0} (Status {1})'.format(msg, code)
         super(HTTPDownloadFailed, self).__init__(msg)
 
 
 class LogPipeHandler(logging.Handler):
-    def __init__(self, pipe):
+    def __init__(self, pipe: "Connection"):
         super(LogPipeHandler, self).__init__()
         self.pipe = pipe
 
-    def emit(self, record):
+    def emit(self, record: logging.LogRecord) -> None:
         self.pipe.send(self.format(record))
 
-    def close(self):
+    def close(self) -> None:
         super(LogPipeHandler, self).close()
         self.pipe.close()
 
 
-def error(text, exit_code=1):
+def error(text: str, exit_code: int = 1) -> None:
     '''
     Log and print `text` error. This function ends the execution of the program with exit code
     `exit_code` (defaults to 1).
     '''
     logger = logging.getLogger('dumper.__init__')
     logger.error(text)
     sys.stderr.write(text + '\n')
     exit(1)
 
 
-def mkdir(dir_):
+def mkdir(dir_: "StrOrBytesPath") -> None:
     '''
     This functions creates the `dir_` directory if it doesn't exist. If `dir_`
     already exists this function does nothing.
     '''
     try:
         os.mkdir(dir_)
     except OSError as error:
         assert error.errno == 17
 
 
-def cacert_config(config, rucio_home):
+def cacert_config(config: "ModuleType", rucio_home: str) -> Optional[Union["FileDescriptorOrPath", Literal[False]]]:
     logger = logging.getLogger('dumper.__init__')
     try:
         cacert = config.config_get('client', 'ca_cert').replace('$RUCIO_HOME', rucio_home)
     except KeyError:
         cacert = None
 
     if cacert is None or not os.path.exists(cacert):
         logger.warning('Configured CA Certificate file "%s" not found: Host certificate verification disabled', cacert)
         cacert = False
 
     return cacert
 
 
-def rucio_home():
+def rucio_home() -> str:
     return os.environ.get('RUCIO_HOME', '/opt/rucio')
 
 
-def get_requests_session():
+def get_requests_session() -> requests.Session:
     requests_session = requests.Session()
-    requests_session.verify = cacert_config(config, rucio_home())
+    requests_session.verify = cacert_config(config, rucio_home())  # type: ignore
     requests_session.stream = True
     return requests_session
 
 
 DUMPS_CACHE_DIR = 'cache'
 RESULTS_DIR = 'results'
 CHUNK_SIZE = 4194304  # 4MiB
@@ -111,24 +122,24 @@
     _mime.load()
     mimetype = _mime.file
 else:
     mimetype = lambda filename: magic.from_file(filename, mime=True)  # NOQA
 # pylint: enable=no-member
 
 
-def isplaintext(filename):
+def isplaintext(filename: "GenericPath") -> bool:
     '''
     Returns True if `filename` has mimetype == 'text/plain'.
     '''
     if os.path.islink(filename):
         filename = os.readlink(filename)
     return mimetype(filename).split(';')[0] == 'text/plain'
 
 
-def smart_open(filename):
+def smart_open(filename: "GenericPath") -> Optional[Union["TextIO", gzip.GzipFile]]:
     '''
     Returns an open file object if `filename` is plain text, else assumes
     it is a bzip2 compressed file and returns a file-like object to
     handle it.
     '''
     f = None
     if isplaintext(filename):
@@ -141,22 +152,26 @@
             f = bz2.open(filename, 'rt')
         else:
             pass  # Not supported format
     return f
 
 
 @contextlib.contextmanager
-def temp_file(directory, final_name=None, binary=False):
+def temp_file(
+    directory: str,
+    final_name: Optional[str] = None,
+    binary: bool = False
+) -> "Iterator[tuple[IO[Any], StrOrBytesPath]]":
     '''
     Allows to create a temporal file to store partial results, when the
     file is complete it is renamed to `final_name`.
 
     - `directory`: working path to create the temporal and the final file.
     - `final_name`: Path of the final file, relative to `directory`.
-       If the `final_name` is omitted or None the renaming step is ommited,
+       If the `final_name` is omitted or None the renaming step is omitted,
        leaving the temporal file with the results.
     - `binary`: whether to open the file in binary mode (default: False).
 
     Important: `directory` and `final_name` must be in the same filesystem as
     a hardlink is used to rename the temporal file.
 
     Example:
@@ -188,15 +203,15 @@
 
 
 DATETIME_FORMAT = '%Y-%m-%d %H:%M:%S'
 DATETIME_FORMAT_FULL = '%Y-%m-%dT%H:%M:%S'
 MILLISECONDS_RE = re.compile(r'\.(\d{3})Z$')
 
 
-def to_datetime(str_or_datetime):
+def to_datetime(str_or_datetime: Union[datetime.datetime, str]) -> Optional[datetime.datetime]:
     """
     Convert string to datetime. The format is somewhat flexible.
     Timezone information is ignored.
     """
     logger = logging.getLogger('dumper.__init__')
     if isinstance(str_or_datetime, datetime.datetime):
         return str_or_datetime
@@ -216,35 +231,35 @@
             DATETIME_FORMAT,
         )
     except ValueError:
         logger.debug(
             'Trying to parse "%s" date with resolution of milliseconds',
             str_or_datetime,
         )
-        miliseconds = int(MILLISECONDS_RE.search(str_or_datetime).group(1))
+        milliseconds = int(MILLISECONDS_RE.search(str_or_datetime).group(1))
         str_or_datetime = MILLISECONDS_RE.sub('', str_or_datetime)
         date = datetime.datetime.strptime(
             str_or_datetime,
             DATETIME_FORMAT,
         )
-        date = date + datetime.timedelta(microseconds=miliseconds * 1000)
+        date = date + datetime.timedelta(microseconds=milliseconds * 1000)
     return date
 
 
-def ddmendpoint_preferred_protocol(ddmendpoint):
+def ddmendpoint_preferred_protocol(ddmendpoint: str) -> "RSEProtocolDict":
     return next(p for p in get_rse_protocols(get_rse_id(ddmendpoint))['protocols'] if p['domains']['wan']['read'] == 1)
 
 
-def ddmendpoint_url(ddmendpoint):
+def ddmendpoint_url(ddmendpoint: str) -> str:
     preferred_protocol = ddmendpoint_preferred_protocol(ddmendpoint)
     prefix = re.sub(r'rucio/$', '', preferred_protocol['prefix'])
     return '{scheme}://{hostname}:{port}'.format(**preferred_protocol) + prefix
 
 
-def http_download_to_file(url, file_, session=None):
+def http_download_to_file(url: str, file_: "IO", session: Optional[requests.Session] = None) -> None:
     '''
     Download the file in `url` storing it in the `file_` file-like
     object.
     If given `session` must be a requests.Session instance, and will be
     used to download the file, otherwise requests.get() will be used.
     '''
     def _do_download(url, file_, session, try_decode=False):
@@ -255,15 +270,15 @@
 
         if response.status_code != 200:
             logging.error(
                 'Retrieving %s returned %d status code',
                 url,
                 response.status_code,
             )
-            raise HTTPDownloadFailed('Error downloading ' + url, response.status_code)
+            raise HTTPDownloadFailed('Error downloading ' + url, str(response.status_code))
 
         if try_decode:
             if response.encoding is None:
                 response.encoding = 'utf-8'
             for chunk in response.iter_content(CHUNK_SIZE, decode_unicode=True):
                 file_.write(chunk)
         else:
@@ -274,46 +289,46 @@
         # try without decoding first
         _do_download(url, file_, session, False)
     except TypeError:
         # if that fails due to writing binary data to text file, try to force decode
         _do_download(url, file_, session, True)
 
 
-def http_download(url, filename):
+def http_download(url: str, filename: "FileDescriptorOrPath") -> None:
     '''
     Download the file in `url` storing it in the path given by `filename`.
     '''
     with open(filename, 'w') as f:
         http_download_to_file(url, f)
 
 
-def gfal_download_to_file(url, file_):
+def gfal_download_to_file(url: str, file_: "IO") -> None:
     '''
     Download the file in `url` storing it in the `file_` file-like
     object.
     '''
     logger = logging.getLogger('dumper.__init__')
     ctx = gfal2.creat_context()  # pylint: disable=no-member
     infile = ctx.open(url, 'r')
 
     try:
         chunk = infile.read(CHUNK_SIZE)
     except gfal2.GError as e:
         if e.code == 70:
-            logger.debug('GError(70) raised, using GRIDFTP PLUGIN:STAT_ON_OPEN=False workarround to download %s', url)
+            logger.debug('GError(70) raised, using GRIDFTP PLUGIN:STAT_ON_OPEN=False workaround to download %s', url)
             ctx.set_opt_boolean('GRIDFTP PLUGIN', 'STAT_ON_OPEN', False)
             infile = ctx.open(url, 'r')
             chunk = infile.read(CHUNK_SIZE)
         else:
             raise
 
     while chunk:
         file_.write(chunk)
         chunk = infile.read(CHUNK_SIZE)
 
 
-def gfal_download(url, filename):
+def gfal_download(url: str, filename: "FileDescriptorOrPath") -> None:
     '''
     Download the file in `url` storing it in the path given by `filename`.
     '''
     with open(filename, 'w') as f:
         gfal_download_to_file(url, f)
```

### Comparing `rucio-34.2.0/lib/rucio/common/dumper/consistency.py` & `rucio-34.3.0/lib/rucio/common/dumper/consistency.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             return ','.join((path, status))
 
         def strip_storage_dump(line):
             '''
             Parser to have consistent paths in storage dumps.
 
             :param line: String with one line of a dump.
-            :returns: Path formated as in the Rucio Replica Dumps.
+            :returns: Path formatted as in the Rucio Replica Dumps.
             '''
             relative = path_parsing.remove_prefix(
                 prefix_components,
                 path_parsing.components(line),
             )
             if relative[0] == 'rucio':
                 relative = relative[1:]
@@ -287,15 +287,15 @@
     '''
     Sort the file with path `file_path` using the GNU sort command, the
     original file is unchanged, the output file is saved with path
     <cache_dir>/<prefix>_sorted.
 
     :param prefix: If given the output file will be named <prefix>_sorted.
     Otherwise the prefix is the name of the input file.
-    :param delimiter: Delimiter character if the data is formated in
+    :param delimiter: Delimiter character if the data is formatted in
     columns (argument of -t in the sort command).
     :param fieldspec: String with the specification of column or columns
     to be used to sort (argument -k in the sort command).
     :param cachedir: Working dir where the output file will be placed.
 
     Note: Using GNU sort to sort large files is convenient as it has low
     memory and it is relatively fast if used with the environment variable
@@ -325,15 +325,15 @@
     os.link(tfile.name, sorted_path)
     os.unlink(tfile.name)
 
     return sorted_path
 
 
 def populate_args(argparser):
-    # Option to download the rucio replica dumps automaticaly
+    # Option to download the rucio replica dumps automatically
     parser = argparser.add_parser(
         'consistency',
         help='Consistency check to verify possible lost files and dark data '
              '(replica dumps are downloaded automatically)'
     )
     parser.add_argument('ddm_endpoint')
     parser.add_argument('storage_dump')
```

### Comparing `rucio-34.2.0/lib/rucio/common/dumper/data_models.py` & `rucio-34.3.0/lib/rucio/common/dumper/data_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     SCHEMA = []
     URI = None
     name = None
 
     def __init__(self, *args):
         if len(args) != len(self.SCHEMA):
             raise TypeError(
-                'Wrong number of parameters (fields) to initalize {0} '
+                'Wrong number of parameters (fields) to initialize {0} '
                 'instance. {1} given, {2} expected:\n{3}'.format(
                     type(self).__name__,
                     len(args),
                     len(self.SCHEMA),
                     args,
                 )
             )
@@ -182,15 +182,15 @@
             response = requests_session.head(url)
             if response.status_code != 200:
                 logger.error(
                     'Retrieving %s returned %d status code',
                     url,
                     response.status_code,
                 )
-                raise HTTPDownloadFailed('Downloading {0} dump'.format(cls.__name__), code=response.status_code)
+                raise HTTPDownloadFailed('Downloading {0} dump'.format(cls.__name__), code=str(response.status_code))
 
             with temp_file(cache_dir, final_name=filename) as (tfile, _):
                 http_download_to_file(url, tfile, session=requests_session)
 
         return path
 
     @classmethod
```

### Comparing `rucio-34.2.0/lib/rucio/common/dumper/path_parsing.py` & `rucio-34.3.0/lib/rucio/common/dumper/path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/exception.py` & `rucio-34.3.0/lib/rucio/common/exception.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/extra.py` & `rucio-34.3.0/lib/rucio/common/extra.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/logging.py` & `rucio-34.3.0/lib/rucio/common/logging.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/pcache.py` & `rucio-34.3.0/lib/rucio/common/pcache.py`

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

### Comparing `rucio-34.2.0/lib/rucio/common/plugins.py` & `rucio-34.3.0/lib/rucio/common/plugins.py`

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

### Comparing `rucio-34.2.0/lib/rucio/common/policy.py` & `rucio-34.3.0/lib/rucio/common/policy.py`

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

### Comparing `rucio-34.2.0/lib/rucio/common/schema/__init__.py` & `rucio-34.3.0/lib/rucio/common/schema/__init__.py`

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

### Comparing `rucio-34.2.0/lib/rucio/common/schema/atlas.py` & `rucio-34.3.0/lib/rucio/common/schema/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/schema/belleii.py` & `rucio-34.3.0/lib/rucio/common/schema/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/schema/cms.py` & `rucio-34.3.0/lib/rucio/common/schema/cms.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/schema/domatpc.py` & `rucio-34.3.0/lib/rucio/common/schema/domatpc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/schema/escape.py` & `rucio-34.3.0/lib/rucio/common/schema/escape.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/schema/generic.py` & `rucio-34.3.0/lib/rucio/common/schema/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/schema/generic_multi_vo.py` & `rucio-34.3.0/lib/rucio/common/schema/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/schema/icecube.py` & `rucio-34.3.0/lib/rucio/common/schema/icecube.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/schema/lsst.py` & `rucio-34.3.0/lib/rucio/common/schema/lsst.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/stomp_utils.py` & `rucio-34.3.0/lib/rucio/common/stomp_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/stopwatch.py` & `rucio-34.3.0/lib/rucio/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/test_rucio_server.py` & `rucio-34.3.0/lib/rucio/common/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/common/types.py` & `rucio-34.3.0/lib/rucio/common/types.py`

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

### Comparing `rucio-34.2.0/lib/rucio/common/utils.py` & `rucio-34.3.0/lib/rucio/common/utils.py`

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

### Comparing `rucio-34.2.0/lib/rucio/core/__init__.py` & `rucio-34.3.0/lib/rucio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/core/account.py` & `rucio-34.3.0/lib/rucio/core/account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/core/account_counter.py` & `rucio-34.3.0/lib/rucio/core/account_counter.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 from typing import TYPE_CHECKING
 
 from sqlalchemy import insert, literal, select
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.exc import NoResultFound
 
 from rucio.db.sqla import filter_thread_work, models
 from rucio.db.sqla.session import read_session, transactional_session
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
```

### Comparing `rucio-34.2.0/lib/rucio/core/account_limit.py` & `rucio-34.3.0/lib/rucio/core/account_limit.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TYPE_CHECKING
 
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.exc import NoResultFound
 from sqlalchemy.sql import func, literal, select
 from sqlalchemy.sql.expression import and_, or_
 
 from rucio.core.account import get_all_rse_usages_per_account
 from rucio.core.rse import get_rse_name
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.db.sqla import models
```

### Comparing `rucio-34.2.0/lib/rucio/core/authentication.py` & `rucio-34.3.0/lib/rucio/core/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,23 +216,28 @@
 def get_auth_token_ssh(account, signature, appid, ip=None, *, session: "Session"):
     """
     Authenticate a Rucio account temporarily via SSH key exchange.
 
     The token lifetime is 1 hour.
 
     :param account: Account identifier as a string.
-    :param signature: Response to server challenge signed with SSH private key as string.
+    :param signature: Response to server challenge signed with SSH private key as a base64 encoded string.
     :param appid: The application identifier as a string.
     :param ip: IP address of the client as a string.
     :param session: The database session in use.
 
     :returns: A dict with token and expires_at entries.
     """
-    if not isinstance(signature, bytes):
-        signature = signature.encode()
+
+    # decode the signature which must come in base64 encoded
+    try:
+        signature += '=' * ((4 - len(signature) % 4) % 4)  # adding required padding
+        signature = b64decode(signature)
+    except TypeError:
+        raise CannotAuthenticate(f'Cannot authenticate to account {account} with malformed signature')
 
     # Make sure the account exists
     if not account_exists(account, session=session):
         return None
 
     # get all active challenge tokens for the requested account
     query = select(
@@ -510,15 +515,15 @@
     cache_key = token.replace(' ', '')
 
     # Check if token ca be found in cache region
     value: "Union[NO_VALUE, dict[str, Any]]" = TOKENREGION.get(cache_key)
     if value is NO_VALUE:  # no cached entry found
         value = query_token(token, session=session)
         if not value:
-            # identify JWT access token and validte
+            # identify JWT access token and validate
             # & save it in Rucio if scope and audience are correct
             if len(token.split(".")) == 3:
                 value = validate_jwt(token, session=session)
             else:
                 raise CannotAuthenticate(traceback.format_exc())
         # save token in the cache
         TOKENREGION.set(cache_key, value)
```

### Comparing `rucio-34.2.0/lib/rucio/core/config.py` & `rucio-34.3.0/lib/rucio/core/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/core/credential.py` & `rucio-34.3.0/lib/rucio/core/credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,29 +22,30 @@
 import boto3
 from botocore.client import Config
 from dogpile.cache.api import NO_VALUE
 from google.oauth2.service_account import Credentials
 
 from rucio.common.cache import make_region_memcached
 from rucio.common.config import config_get, get_rse_credentials
+from rucio.common.constants import RseAttr
 from rucio.common.exception import UnsupportedOperation
 from rucio.core.monitor import MetricManager
 from rucio.core.rse import get_rse_attribute
 
 CREDS_GCS = None
 
 REGION = make_region_memcached(expiration_time=900)
 METRICS = MetricManager(module=__name__)
 
 
 def get_signed_url(rse_id: str, service: str, operation: str, url: str, lifetime: int = 600) -> str:
     """
     Get a signed URL for a particular service and operation.
 
-    The signed URL will be valid for 1 hour but can be overriden.
+    The signed URL will be valid for 1 hour but can be overridden.
 
     :param rse_id: The ID of the RSE that the URL points to.
     :param service: The service to authorise, either 'gcs', 's3' or 'swift'.
     :param operation: The operation to sign, either 'read', 'write', or 'delete'.
     :param url: The URL to sign.
     :param lifetime: Lifetime of the signed URL in seconds.
     :returns: Signed URL as a variable-length string.
@@ -107,15 +108,15 @@
         )
 
     elif service == 's3':
 
         # get RSE S3 URL style (path or host)
         # path-style: https://s3.region-code.amazonaws.com/bucket-name/key-name
         # host-style: https://bucket-name.s3.region-code.amazonaws.com/key-name
-        s3_url_style = get_rse_attribute(rse_id, 's3_url_style')
+        s3_url_style = get_rse_attribute(rse_id, RseAttr.S3_URL_STYLE)
 
         # no S3 URL style specified, assume path-style
         if s3_url_style is None:
             s3_url_style = "path"
 
         # split URL to get hostname, bucket and key
         components = urlparse(url)
```

### Comparing `rucio-34.2.0/lib/rucio/core/did.py` & `rucio-34.3.0/lib/rucio/core/did.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 from datetime import datetime, timedelta
 from enum import Enum
 from hashlib import md5
 from re import match
 from typing import TYPE_CHECKING
 
 from sqlalchemy import and_, delete, exists, insert, or_, update
-from sqlalchemy.exc import DatabaseError, IntegrityError
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.exc import DatabaseError, IntegrityError, NoResultFound
 from sqlalchemy.sql import func, not_
 from sqlalchemy.sql.expression import bindparam, case, false, null, select, true
 
 import rucio.core.replica  # import add_replicas
 import rucio.core.rule
 from rucio.common import exception
 from rucio.common.config import config_get_bool, config_get_int
@@ -338,15 +337,15 @@
                 parent_dids.append({'scope': parent_did.scope,
                                     'name': parent_did.name,
                                     'rule_evaluation_action': DIDReEvaluation.ATTACH})
         except NoResultFound:
             raise exception.DataIdentifierNotFound("Data identifier '%s:%s' not found" % (attachment['scope'], attachment['name']))
         first_iteration = False
 
-    # Remove all duplicated dictionnaries from the list
+    # Remove all duplicated dictionaries from the list
     # (convert the list of dictionaries into a list of tuple, then to a set of tuple
     # to remove duplicates, then back to a list of unique dictionaries)
     parent_dids = [dict(tup) for tup in set(tuple(dictionary.items()) for dictionary in parent_dids)]
     if parent_dids:
         session.execute(insert(models.UpdatedDID), parent_dids)
 
 
@@ -474,15 +473,15 @@
             )
             session.execute(stmt)
         session.flush()
     except IntegrityError as error:
         raise exception.RucioException(error.args)
 
     if not parent_did.is_archive:
-        # mark tha archive file as is_archive
+        # mark the archive file as is_archive
         parent_did.is_archive = True
 
         # mark parent datasets as is_archive = True
         stmt = update(
             models.DataIdentifier
         ).where(
             exists(
@@ -856,15 +855,15 @@
     ).where(
         models.DataIdentifier.did_type == DIDType.FILE,
         models.DataIdentifier.scope == scope,
         models.DataIdentifier.name == name,
     )
     archive_did = session.execute(stmt).scalar()
     if not archive_did.is_archive:
-        # mark tha archive file as is_archive
+        # mark the archive file as is_archive
         archive_did.is_archive = True
 
         # mark parent datasets as is_archive = True
         stmt = update(
             models.DataIdentifier
         ).where(
             exists(
@@ -2881,15 +2880,15 @@
     except NoResultFound:
         raise exception.DataIdentifierNotFound("Data identifier '%s:%s' not found" % (did['scope'], did['name']))
 
 
 @transactional_session
 def trigger_event(scope, name, event_type, payload, *, session: "Session"):
     """
-    Records changes occuring in the did to the FollowEvents table
+    Records changes occurring in the did to the FollowEvents table
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param event_type: The type of event affecting the did.
     :param payload: Any message to be stored along with the event.
     :param session: The database session in use.
     """
@@ -2897,15 +2896,15 @@
         stmt = select(
             models.DidsFollowed
         ).filter_by(
             scope=scope,
             name=name
         )
         for did in session.execute(stmt).scalars().all():
-            # Create a new event using teh specified parameters.
+            # Create a new event using the specified parameters.
             new_event = models.FollowEvents(scope=scope, name=name, account=did.account,
                                             did_type=did.did_type, event_type=event_type, payload=payload)
             new_event.save(session=session, flush=False)
 
         session.flush()
     except IntegrityError as error:
         raise exception.RucioException(error.args)
@@ -2921,15 +2920,15 @@
     # Query the FollowEvents table
     stmt = select(
         models.FollowEvents
     ).order_by(
         models.FollowEvents.created_at
     )
 
-    # Use hearbeat mechanism to select a chunck of events based on the hashed account
+    # Use heartbeat mechanism to select a chunk of events based on the hashed account
     stmt = filter_thread_work(session=session, query=stmt, total_threads=total_workers, thread_id=worker_number, hash_variable='account')
 
     try:
         events = session.execute(stmt).scalars().all()
         # If events exist for an account then create a report.
         if events:
             body = '''
```

### Comparing `rucio-34.2.0/lib/rucio/core/did_meta_plugins/__init__.py` & `rucio-34.3.0/lib/rucio/core/did_meta_plugins/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     :param long: Long format option to display more information for each DID.
     :param recursive: Recursively list DIDs content.
     :param ignore_dids: List of DIDs to refrain from yielding.
     :param session: The database session in use.
     :returns: List of dids satisfying metadata criteria.
     :raises: InvalidMetadata
     """
-    # backwards compatability for filters as single {}.
+    # backwards compatibility for filters as single {}.
     if isinstance(filters, dict):
         filters = [filters]
 
     required_unique_plugins = set()                 # keep track of which plugins are required
     for or_group in filters:
         for key in or_group.keys():
             if key == 'name':                       # [name] is always passed through, and needs to be in schema of all plugins
```

### Comparing `rucio-34.2.0/lib/rucio/core/did_meta_plugins/did_column_meta.py` & `rucio-34.3.0/lib/rucio/core/did_meta_plugins/did_column_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 # limitations under the License.
 
 import operator
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING
 
 from sqlalchemy import inspect, update
-from sqlalchemy.exc import CompileError, InvalidRequestError
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.exc import CompileError, InvalidRequestError, NoResultFound
 from sqlalchemy.sql import func
 from sqlalchemy.sql.expression import true
 
 from rucio.common import exception
 from rucio.core import account_counter, rse_counter
 from rucio.core.did_meta_plugins.did_meta_plugin_interface import DidMetaPlugin
 from rucio.core.did_meta_plugins.filter_engine import FilterEngine
@@ -194,15 +193,15 @@
             'all': [DIDType.CONTAINER, DIDType.DATASET, DIDType.FILE],
             'collection': [DIDType.CONTAINER, DIDType.DATASET],
             'container': [DIDType.CONTAINER],
             'dataset': [DIDType.DATASET],
             'file': [DIDType.FILE]
         }
 
-        # backwards compatability for filters as single {}.
+        # backwards compatibility for filters as single {}.
         if isinstance(filters, dict):
             filters = [filters]
 
         # for each or_group, make sure there is a mapped "did_type" filter.
         # if type maps to many DIDTypes, the corresponding or_group will be copied the required number of times to satisfy all the logical possibilities.
         filters_tmp = []
         for or_group in filters:
```

### Comparing `rucio-34.2.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py` & `rucio-34.3.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,91 +9,135 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import ABCMeta, abstractmethod
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
 
 from rucio.db.sqla.session import transactional_session
 
 if TYPE_CHECKING:
-    from typing import Optional
+    from collections.abc import Iterator
+    from typing import Any, Optional, Union
 
     from sqlalchemy.orm import Session
 
+    from rucio.common.types import InternalScope
+
 
 class DidMetaPlugin(metaclass=ABCMeta):
     """
     Interface for plugins managing metadata of DIDs
     """
 
     def __init__(self):
         """
         Initializes the plugin
         """
         pass
 
     @abstractmethod
-    def get_metadata(self, scope, name, *, session: "Optional[Session]" = None):
+    def get_metadata(
+        self,
+        scope: "InternalScope",
+        name: str,
+        *,
+        session: "Optional[Session]" = None
+    ) -> "Any":
         """
         Get data identifier metadata
 
         :param scope: The scope name.
         :param name: The data identifier name.
         :param session: The database session in use.
         """
         pass
 
     @abstractmethod
-    def set_metadata(self, scope, name, key, value, recursive=False, *, session: "Optional[Session]" = None):
+    def set_metadata(
+        self,
+        scope: "InternalScope",
+        name: str,
+        key: str,
+        value: str,
+        recursive: bool = False,
+        *,
+        session: "Optional[Session]" = None
+    ) -> None:
         """
         Add metadata to data identifier.
 
         :param scope: The scope name.
         :param name: The data identifier name.
         :param key: the key.
         :param value: the value.
         :param did: The data identifier info.
         :param recursive: Option to propagate the metadata change to content.
         :param session: The database session in use.
         """
         pass
 
     @transactional_session
-    def set_metadata_bulk(self, scope, name, meta, recursive=False, *, session: "Optional[Session]" = None):
+    def set_metadata_bulk(
+        self,
+        scope: "InternalScope",
+        name: str,
+        meta: dict[str, "Any"],
+        recursive: bool = False,
+        *,
+        session: "Optional[Session]" = None
+    ) -> None:
         """
         Add metadata to data identifier in bulk.
 
         :param scope: The scope name.
         :param name: The data identifier name.
         :param meta: all key-values to set.
         :type meta: dict
         :param recursive: Option to propagate the metadata change to content.
         :param session: The database session in use.
         """
         for key, value in meta.items():
             self.set_metadata(scope, name, key, value, recursive=recursive, session=session)
 
     @abstractmethod
-    def delete_metadata(self, scope, name, key, *, session: "Session" = None):
+    def delete_metadata(
+        self,
+        scope: "InternalScope",
+        name: str,
+        key: str,
+        *,
+        session: "Optional[Session]" = None
+    ) -> None:
         """
         Deletes the metadata stored for the given key.
 
         :param scope: The scope of the did.
         :param name: The name of the did.
         :param key: Key of the metadata.
         :param session: The database session in use.
         """
         pass
 
     @abstractmethod
-    def list_dids(self, scope, filters, did_type='collection', ignore_case=False, limit=None,
-                  offset=None, long=False, recursive=False, *, session: "Optional[Session]" = None):
+    def list_dids(
+        self,
+        scope: "InternalScope",
+        filters: dict[str, "Any"],
+        did_type: Literal['all', 'collection', 'dataset', 'container', 'file'] = 'collection',
+        ignore_case: bool = False,
+        limit: "Optional[int]" = None,
+        offset: "Optional[int]" = None,
+        long: bool = False,
+        recursive: bool = False,
+        *,
+        session: "Optional[Session]" = None
+    ) -> "Iterator[Union[str, dict[str, Any]]]":
         """
         Search data identifiers
 
         :param scope: the scope name.
         :param filters: dictionary of attributes by which the results should be filtered.
         :param did_type: the type of the did: all(container, dataset, file), collection(dataset or container), dataset, container, file.
         :param ignore_case: ignore case distinctions.
@@ -102,15 +146,20 @@
         :param long: Long format option to display more information for each DID.
         :param session: The database session in use.
         :param recursive: Recursively list DIDs content.
         """
         pass
 
     @abstractmethod
-    def manages_key(self, key, *, session: "Optional[Session]" = None):
+    def manages_key(
+        self,
+        key: str,
+        *,
+        session: "Optional[Session]" = None
+    ) -> bool:
         """
         Returns whether key is managed by this plugin or not.
         :param key: Key of the metadata.
         :param session: The database session in use.
         :returns (Boolean)
         """
         pass
```

### Comparing `rucio-34.2.0/lib/rucio/core/did_meta_plugins/filter_engine.py` & `rucio-34.3.0/lib/rucio/core/did_meta_plugins/filter_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     def _coerce_filter_word_to_model_attribute(self, word, model_class, strict=True):
         """
         Attempts to coerce a filter word to an attribute of a <model_class>.
 
         :param model_class: The word.
         :param model_class: The SQL model class.
-        :params: strict: Enforce that keywords must be coercable to a model attribute.
+        :params: strict: Enforce that keywords must be coercible to a model attribute.
         :returns: The coerced attribute if successful or (if strict is False) the word if not.
         :raises: KeyNotFound
         """
         if isinstance(word, str):
             if hasattr(model_class, word):
                 return getattr(model_class, word)
             else:
@@ -195,15 +195,15 @@
 
         replacing all filter operator suffixes with python equivalents using the LUT, <OPERATORS_CONVERSION_LUT>, and
         coercing all filter words to their corresponding <model_class> attribute.
 
         Typecasting of values is also attempted.
 
         :param model_class: The SQL model class.
-        :param strict_coerce: Enforce that keywords must be coercable to a model attribute.
+        :param strict_coerce: Enforce that keywords must be coercible to a model attribute.
         :returns: The set of mandatory model attributes to be used in the filter query.
         :raises: MissingModuleException, DIDFilterSyntaxError
         """
         if model_class:
             try:
                 import_module(model_class.__module__)
             except ModuleNotFoundError:
```

### Comparing `rucio-34.2.0/lib/rucio/core/did_meta_plugins/json_meta.py` & `rucio-34.3.0/lib/rucio/core/did_meta_plugins/json_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json as json_lib
 import operator
 from typing import TYPE_CHECKING, Any, cast
 
-from sqlalchemy.exc import DataError
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.exc import DataError, NoResultFound
 
 from rucio.common import exception
 from rucio.core.did_meta_plugins.did_meta_plugin_interface import DidMetaPlugin
 from rucio.core.did_meta_plugins.filter_engine import FilterEngine
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import DIDType
 from rucio.db.sqla.session import read_session, stream_session, transactional_session
@@ -140,15 +139,15 @@
                   offset=None, long=False, recursive=False, ignore_dids=None, *, session: "Session"):
         if not json_implemented(session=session):
             raise NotImplementedError
 
         if not ignore_dids:
             ignore_dids = set()
 
-        # backwards compatability for filters as single {}.
+        # backwards compatibility for filters as single {}.
         if isinstance(filters, dict):
             filters = [filters]
 
         # instantiate fe and create sqla query, note that coercion to a model keyword
         # is not appropriate here as the filter words are stored in a single json column.
         fe = FilterEngine(filters, model_class=models.DidMeta, strict_coerce=False)
         query = fe.create_sqla_query(
```

### Comparing `rucio-34.2.0/lib/rucio/core/did_meta_plugins/mongo_meta.py` & `rucio-34.3.0/lib/rucio/core/did_meta_plugins/mongo_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             raise exception.DataIdentifierNotFound(e)
 
     def list_dids(self, scope, filters, did_type='collection', ignore_case=False, limit=None,
                   offset=None, long=False, recursive=False, ignore_dids=None, *, session: "Optional[Session]" = None):
         if not ignore_dids:
             ignore_dids = set()
 
-        # backwards compatability for filters as single {}.
+        # backwards compatibility for filters as single {}.
         if isinstance(filters, dict):
             filters = [filters]
 
         # instantiate fe and create mongo query
         fe = FilterEngine(filters, model_class=None, strict_coerce=False)
         mongo_query_str = fe.create_mongo_query(
             additional_filters=[
@@ -162,30 +162,30 @@
             ))
 
         if long:
             query_result = self.col.find(mongo_query_str)
             if limit:
                 query_result = query_result.limit(limit)
             for did in query_result:
-                did_full = did_full = "{}:{}".format(did['scope'], did['name'])
+                did_full = "{}:{}".format(did['scope'], did['name'])
                 if did_full not in ignore_dids:         # aggregating recursive queries may contain duplicate DIDs
                     ignore_dids.add(did_full)
                     yield {
                         'scope': InternalScope(did['scope']),
                         'name': did['name'],
                         'did_type': "N/A",
                         'bytes': "N/A",
                         'length': "N/A"
                     }
         else:
             query_result = self.col.find(mongo_query_str)
             if limit:
                 query_result = query_result.limit(limit)
             for did in query_result:
-                did_full = did_full = "{}:{}".format(did['scope'], did['name'])
+                did_full = "{}:{}".format(did['scope'], did['name'])
                 if did_full not in ignore_dids:         # aggregating recursive queries may contain duplicate DIDs
                     ignore_dids.add(did_full)
                     yield did['name']
 
     def manages_key(self, key, *, session: "Optional[Session]" = None):
         return True
```

### Comparing `rucio-34.2.0/lib/rucio/core/did_meta_plugins/postgres_meta.py` & `rucio-34.3.0/lib/rucio/core/did_meta_plugins/postgres_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 
     def list_dids(self, scope, filters, did_type='collection', ignore_case=False, limit=None,
                   offset=None, long=False, recursive=False, ignore_dids=None, *, session: "Optional[Session]" = None):
 
         if not ignore_dids:
             ignore_dids = set()
 
-        # backwards compatability for filters as single {}.
+        # backwards compatibility for filters as single {}.
         if isinstance(filters, dict):
             filters = [filters]
 
         try:
             # instantiate fe and create postgres query
             fe = FilterEngine(filters, model_class=None, strict_coerce=False)
             postgres_query_str = fe.create_postgres_query(
```

### Comparing `rucio-34.2.0/lib/rucio/core/dirac.py` & `rucio-34.3.0/lib/rucio/core/dirac.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 import re
 from json import loads
 from json.decoder import JSONDecodeError
 from typing import TYPE_CHECKING, Optional
 
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.exc import NoResultFound
 
 from rucio.common.config import config_get
 from rucio.common.exception import ConfigNotFound, InvalidType, RucioException, UnsupportedOperation
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.common.utils import extract_scope
 from rucio.core.did import add_did, attach_dids_to_dids
 from rucio.core.replica import add_replicas
```

### Comparing `rucio-34.2.0/lib/rucio/core/distance.py` & `rucio-34.3.0/lib/rucio/core/distance.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/core/exporter.py` & `rucio-34.3.0/lib/rucio/core/exporter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/core/heartbeat.py` & `rucio-34.3.0/lib/rucio/core/heartbeat.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,34 +10,54 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
 import hashlib
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
-from sqlalchemy import func
+from sqlalchemy import func, select
 from sqlalchemy.sql import distinct
 
 from rucio.common.exception import DatabaseException
 from rucio.common.utils import pid_exists
 from rucio.db.sqla.models import Heartbeats
 from rucio.db.sqla.session import read_session, transactional_session
 
 if TYPE_CHECKING:
+    from threading import Thread
+    from typing import TypedDict
+
     from sqlalchemy.orm import Session
 
+    class HeartbeatDict(TypedDict):
+        readable: Optional[str]
+        hostname: str
+        pid: int
+        thread_name: Optional[str]
+        updated_at: datetime.datetime
+        created_at: datetime.datetime
+        payload: Optional[str]
+        test: int
 
 DEFAULT_EXPIRATION_DELAY = datetime.timedelta(days=1).total_seconds()
 
 
 @transactional_session
-def sanity_check(executable, hostname, hash_executable=None, pid=None, thread=None,
-                 expiration_delay=DEFAULT_EXPIRATION_DELAY, *, session: "Session"):
+def sanity_check(
+    executable: str,
+    hostname: str,
+    hash_executable: Optional[str] = None,
+    pid: Optional[int] = None,
+    thread: Optional["Thread"] = None,
+    expiration_delay: float = DEFAULT_EXPIRATION_DELAY,
+    *,
+    session: "Session"
+) -> None:
     """
     sanity_check wrapper to ignore DatabaseException errors.
 
     :param executable: Executable name as a string, e.g., conveyor-submitter.
     :param hostname: Hostname as a string, e.g., rucio-daemon-prod-01.cern.ch.
     :param hash_executable: Hash of the executable.
     :param pid: UNIX Process ID as a number, e.g., 1234.
@@ -52,15 +72,22 @@
             live(executable=executable, hostname=hostname,
                  pid=pid, thread=thread, session=session)
     except DatabaseException:
         pass
 
 
 @transactional_session
-def _sanity_check(executable, hostname, hash_executable=None, expiration_delay=DEFAULT_EXPIRATION_DELAY, *, session: "Session"):
+def _sanity_check(
+    executable: str,
+    hostname: str,
+    hash_executable: Optional[str] = None,
+    expiration_delay: float = DEFAULT_EXPIRATION_DELAY,
+    *,
+    session: "Session"
+) -> None:
     """
     Check if processes on the host are still running.
 
     :param executable: Executable name as a string, e.g., conveyor-submitter.
     :param hostname: Hostname as a string, e.g., rucio-daemon-prod-01.cern.ch.
     :param hash_executable: Hash of the executable.
     :param expiration_delay: time (in seconds) after which any inactive health check will be removed
@@ -79,15 +106,25 @@
                 session.query(Heartbeats).filter_by(hostname=hostname, pid=pid).delete()
 
     if expiration_delay:
         cardiac_arrest(older_than=expiration_delay, session=session)
 
 
 @transactional_session
-def live(executable, hostname, pid, thread=None, older_than=600, hash_executable=None, payload=None, *, session: "Session"):
+def live(
+    executable: str,
+    hostname: str,
+    pid: int,
+    thread: Optional["Thread"] = None,
+    older_than: int = 600,
+    hash_executable: Optional[str] = None,
+    payload: Optional[str] = None,
+    *,
+    session: "Session"
+) -> dict[str, int]:
     """
     Register a heartbeat for a process/thread on a given node.
     The executable name is used for the calculation of thread assignments.
     Removal of stale heartbeats is done as a scheduled database job.
 
     TODO: Returns an assignment dictionary for the given executable.
 
@@ -152,27 +189,34 @@
             break
 
     return {'assign_thread': assign_thread,
             'nr_threads': len(result)}
 
 
 @transactional_session
-def die(executable, hostname, pid, thread, older_than=None, hash_executable=None, *, session: "Session"):
+def die(
+    executable: str,
+    hostname: str,
+    pid: int,
+    thread: "Thread",
+    older_than: Optional[int] = None,
+    hash_executable: Optional[str] = None,
+    *,
+    session: "Session"
+) -> None:
     """
     Remove a single heartbeat older than specified.
 
     :param executable: Executable name as a string, e.g., conveyor-submitter
     :param hostname: Hostname as a string, e.g., rucio-daemon-prod-01.cern.ch
     :param pid: UNIX Process ID as a number, e.g., 1234
     :param thread: Python Thread Object
     :param older_than: Removes specified heartbeats older than specified nr of seconds
     :param hash_executable: Hash of the executable.
     :param session: The database session in use.
-
-    :returns heartbeats: Dictionary {assign_thread, nr_threads}
     """
     if not hash_executable:
         hash_executable = calc_hash(executable)
 
     query = session.query(Heartbeats).filter_by(executable=hash_executable,
                                                 hostname=hostname,
                                                 pid=pid,
@@ -181,15 +225,15 @@
     if older_than:
         query = query.filter(Heartbeats.updated_at < datetime.datetime.utcnow() - datetime.timedelta(seconds=older_than))
 
     query.delete()
 
 
 @transactional_session
-def cardiac_arrest(older_than=None, *, session: "Session"):
+def cardiac_arrest(older_than: Optional[int] = None, *, session: "Session") -> None:
     """
     Removes all heartbeats older than specified.
 
     :param older_than: Removes all heartbeats older than specified nr of seconds
     :param session: The database session in use.
     """
 
@@ -198,65 +242,75 @@
     if older_than:
         query = query.filter(Heartbeats.updated_at < datetime.datetime.utcnow() - datetime.timedelta(seconds=older_than))
 
     query.delete()
 
 
 @read_session
-def list_heartbeats(*, session: "Session"):
+def list_heartbeats(*, session: "Session") -> list["HeartbeatDict"]:
     """
     List all heartbeats.
 
     :param session: The database session in use.
 
-    :returns: List of tuples
+    :returns: List of dicts
     """
 
-    query = session.query(Heartbeats.readable,
-                          Heartbeats.hostname,
-                          Heartbeats.pid,
-                          Heartbeats.thread_name,
-                          Heartbeats.updated_at,
-                          Heartbeats.created_at,
-                          Heartbeats.payload).order_by(Heartbeats.readable,
-                                                       Heartbeats.hostname,
-                                                       Heartbeats.thread_name)
+    stmt = select(
+        Heartbeats.readable,
+        Heartbeats.hostname,
+        Heartbeats.pid,
+        Heartbeats.thread_name,
+        Heartbeats.updated_at,
+        Heartbeats.created_at,
+        Heartbeats.payload
+    ).order_by(
+        Heartbeats.readable,
+        Heartbeats.hostname,
+        Heartbeats.thread_name
+    )
 
-    result = query.all()
+    result = session.execute(stmt).all()
     json_result = []
     for element in result:
         json_result.append(element._asdict())
     return json_result
 
 
 @read_session
-def list_payload_counts(executable, older_than=600, hash_executable=None, *, session: "Session"):
+def list_payload_counts(
+    executable: str,
+    older_than: int = 600,
+    hash_executable: Optional[str] = None,
+    *,
+    session: "Session"
+) -> dict[str, int]:
     """
     Give the counts of number of threads per payload for a certain executable.
 
     :param executable: Executable name as a string, e.g., conveyor-submitter
     :param older_than: Removes specified heartbeats older than specified nr of seconds
     :param hash_executable: Hash of the executable.
     :param session: The database session in use.
 
-    :returns: List of tuples
+    :returns: Dict
     """
 
     if not hash_executable:
         hash_executable = calc_hash(executable)
     query = session.query(Heartbeats.payload,
                           func.count(Heartbeats.payload))\
                    .filter(Heartbeats.executable == hash_executable)\
                    .filter(Heartbeats.updated_at >= datetime.datetime.utcnow() - datetime.timedelta(seconds=older_than))\
                    .group_by(Heartbeats.payload)\
                    .order_by(Heartbeats.payload)
 
     return dict((payload, count) for payload, count in query.all() if payload)
 
 
-def calc_hash(executable):
+def calc_hash(executable: str) -> str:
     """
     Calculates a SHA256 hash.
 
     return: String of hexadecimal hash
     """
     return hashlib.sha256(executable.encode('utf-8')).hexdigest()
```

### Comparing `rucio-34.2.0/lib/rucio/core/identity.py` & `rucio-34.3.0/lib/rucio/core/identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,22 @@
 from rucio.common.types import InternalAccount
 from rucio.core.account import account_exists
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import IdentityType
 from rucio.db.sqla.session import read_session, transactional_session
 
 if TYPE_CHECKING:
+    from collections.abc import Sequence
+
+    from sqlalchemy import Row
     from sqlalchemy.orm import Session
 
 
 @transactional_session
-def add_identity(identity: str, type_: IdentityType, email: str, password: Optional[str] = None, *, session: "Session"):
+def add_identity(identity: str, type_: IdentityType, email: str, password: Optional[str] = None, *, session: "Session") -> None:
     """
     Creates a user identity.
 
     :param identity: The identity key name. For example x509 DN, or a username.
     :param type_: The type of the authentication (x509, gss, userpass, ssh, saml, oidc)
     :param email: The Email address associated with the identity.
     :param password: If type==userpass, this sets the password.
@@ -97,15 +100,15 @@
             raise exception.IdentityNotFound('Password does not match for userpass identity \'%s\'!' % identity)
         return True
     else:
         raise NotImplementedError('Identity type \'%s\' is not implemented!' % type_)
 
 
 @transactional_session
-def del_identity(identity: str, type_: IdentityType, *, session: "Session"):
+def del_identity(identity: str, type_: IdentityType, *, session: "Session") -> None:
     """
     Deletes a user identity.
 
     :param identity: The identity key name. For example x509 DN, or a username.
     :param type_: The type of the authentication (x509, gss, userpass, saml, oidc).
     :param session: The database session in use.
     """
@@ -119,15 +122,24 @@
     id_ = session.execute(query).scalar()
     if id_ is None:
         raise exception.IdentityError('Identity (\'%s\',\'%s\') does not exist!' % (identity, type_))
     id_.delete(session=session)
 
 
 @transactional_session
-def add_account_identity(identity: str, type_: IdentityType, account: InternalAccount, email: str, default: bool = False, password: str = None, *, session: "Session"):
+def add_account_identity(
+    identity: str,
+    type_: IdentityType,
+    account: InternalAccount,
+    email: str,
+    default: bool = False,
+    password: Optional[str] = None,
+    *,
+    session: "Session"
+) -> None:
     """
     Adds a membership association between identity and account.
 
     :param identity: The identity key name. For example x509 DN, or a username.
     :param type_: The type of the authentication (x509, gss, userpass, ssh, saml, oidc).
     :param account: The account name.
     :param email: The Email address associated with the identity.
@@ -161,15 +173,15 @@
                 or match('.*IntegrityError.*duplicate key value violates unique constraint.*', error.args[0]) \
                 or match('.*UniqueViolation.*duplicate key value violates unique constraint.*', error.args[0]) \
                 or match('.*IntegrityError.*columns? .*not unique.*', error.args[0]):
             raise exception.Duplicate('Identity pair \'%s\',\'%s\' already exists!' % (identity, type_))
 
 
 @read_session
-def exist_identity_account(identity: str, type_: IdentityType, account: InternalAccount, *, session: "Session"):
+def exist_identity_account(identity: str, type_: IdentityType, account: InternalAccount, *, session: "Session") -> bool:
     """
     Check if an identity is mapped to an account.
 
     :param identity: The user identity as string.
     :param type_: The type of identity as a string, e.g. userpass, x509, gss, saml, oidc ...
     :param account: The account as an InternalAccount.
     :param session: The database session in use.
@@ -183,21 +195,21 @@
         models.IdentityAccountAssociation.identity_type == type_,
         models.IdentityAccountAssociation.account == account
     )
     return session.execute(query).scalar() is not None
 
 
 @read_session
-def get_default_account(identity: str, type_: IdentityType, oldest_if_none: bool = False, *, session: "Session"):
+def get_default_account(identity: str, type_: IdentityType, oldest_if_none: bool = False, *, session: "Session") -> Optional[InternalAccount]:
     """
     Retrieves the default account mapped to an identity.
 
     :param identity: The identity key name. For example, x509DN, or a username.
     :param type_: The type of the authentication (x509, gss, userpass, saml, oidc).
-    :param oldest_if_none: If True and no default account it found the oldes known
+    :param oldest_if_none: If True and no default account it found the oldest known
                            account of that identity will be chosen, if False and
                            no default account is found, exception will be raised.
     :param session: The database session to use.
     :returns: The default account name, None otherwise.
     """
 
     query = select(
@@ -224,15 +236,15 @@
         else:
             raise exception.IdentityError('There is no default account for identity (%s, %s)' % (identity, type_))
 
     return tmp.account
 
 
 @transactional_session
-def del_account_identity(identity: str, type_: IdentityType, account: InternalAccount, *, session: "Session"):
+def del_account_identity(identity: str, type_: IdentityType, account: InternalAccount, *, session: "Session") -> None:
     """
     Removes a membership association between identity and account.
 
     :param identity: The identity key name. For example x509 DN, or a username.
     :param type_: The type of the authentication (x509, gss, userpass, saml, oidc).
     :param account: The account name.
     :param session: The database session in use.
@@ -247,15 +259,15 @@
     aid = session.execute(query).scalar()
     if aid is None:
         raise exception.IdentityError('Identity (\'%s\',\'%s\') does not exist!' % (identity, type_))
     aid.delete(session=session)
 
 
 @read_session
-def list_identities(*, session: "Session", **kwargs):
+def list_identities(*, session: "Session", **kwargs) -> "Sequence[Row[tuple[str, IdentityType]]]":
     """
     Returns a list of all identities.
 
     :param session: The database session in use.
 
     returns: A list of all identities.
     """
@@ -265,15 +277,15 @@
     ).order_by(
         models.Identity.identity
     )
     return session.execute(query).all()
 
 
 @read_session
-def list_accounts_for_identity(identity: str, type_: IdentityType, *, session: "Session"):
+def list_accounts_for_identity(identity: str, type_: IdentityType, *, session: "Session") -> "Sequence[InternalAccount]":
     """
     Returns a list of all accounts for an identity.
 
     :param identity: The identity key name. For example x509 DN, or a username.
     :param type_: The type of the authentication (x509, gss, userpass, saml, oidc).
     :param session: The database session in use.
```

### Comparing `rucio-34.2.0/lib/rucio/core/importer.py` & `rucio-34.3.0/lib/rucio/core/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Iterable
 from typing import TYPE_CHECKING, Any
 
 from rucio.common.config import config_get
+from rucio.common.constants import RseAttr
 from rucio.common.exception import RSEOperationNotSupported
 from rucio.common.types import InternalAccount
 from rucio.core import account as account_module
 from rucio.core import distance as distance_module
 from rucio.core import identity as identity_module
 from rucio.core import rse as rse_module
 from rucio.db.sqla import models
@@ -103,16 +104,16 @@
             if limit:
                 if limit_name in old_limits:
                     rse_module.delete_rse_limits(rse_id=rse_id, name=limit_name, session=session)
                 rse_module.set_rse_limits(rse_id=rse_id, name=limit_name, value=limit, session=session)
 
         # Attributes
         attributes = rse.get('attributes', {})
-        attributes['lfn2pfn_algorithm'] = rse.get('lfn2pfn_algorithm')
-        attributes['verify_checksum'] = rse.get('verify_checksum')
+        attributes[RseAttr.LFN2PFN_ALGORITHM] = rse.get('lfn2pfn_algorithm')
+        attributes[RseAttr.VERIFY_CHECKSUM] = rse.get('verify_checksum')
 
         old_attributes = rse_module.list_rse_attributes(rse_id=rse_id, session=session)
         missing_attributes = [attribute for attribute in old_attributes if attribute not in attributes]
 
         for attr in attributes:
             value = attributes[attr]
             if value is not None:
```

### Comparing `rucio-34.2.0/lib/rucio/core/lifetime_exception.py` & `rucio-34.3.0/lib/rucio/core/lifetime_exception.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 from configparser import NoSectionError
 from datetime import datetime, timedelta
 from re import match
 from typing import TYPE_CHECKING
 
 from sqlalchemy import or_, select, update
-from sqlalchemy.exc import IntegrityError
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.exc import IntegrityError, NoResultFound
 
 import rucio.common.policy
 from rucio.common.config import config_get, config_get_int, config_get_list
+from rucio.common.constants import RseAttr
 from rucio.common.exception import ConfigNotFound, LifetimeExceptionDuplicate, LifetimeExceptionNotFound, RucioException, UnsupportedOperation
 from rucio.common.utils import generate_uuid, str_to_date
 from rucio.core.message import add_message
 from rucio.core.rse import list_rse_attributes
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import DIDType, LifetimeExceptionsState
 from rucio.db.sqla.session import read_session, stream_session, transactional_session
@@ -280,15 +280,15 @@
     :param session:  The database session in use.
     """
     policy = rucio.common.policy.get_policy()
     if policy != 'atlas':
         return None
 
     # Check if on ATLAS managed space
-    if [rse for rse in rses if list_rse_attributes(rse_id=rse['id'], session=session).get('type') in ['LOCALGROUPDISK', 'LOCALGROUPTAPE', 'GROUPDISK', 'GROUPTAPE']]:
+    if [rse for rse in rses if list_rse_attributes(rse_id=rse['id'], session=session).get(RseAttr.TYPE) in ['LOCALGROUPDISK', 'LOCALGROUPTAPE', 'GROUPDISK', 'GROUPTAPE']]:
         return None
     # Now check the lifetime policy
     try:
         query = select(
             models.DataIdentifier
         ).where(
             models.DataIdentifier.scope == scope,
```

### Comparing `rucio-34.2.0/lib/rucio/core/lock.py` & `rucio-34.3.0/lib/rucio/core/lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import TYPE_CHECKING
 
 from sqlalchemy.exc import DatabaseError
 from sqlalchemy.sql.expression import and_, or_
 
 import rucio.core.did
 import rucio.core.rule
+from rucio.common.constants import RseAttr
 from rucio.common.exception import DataIdentifierNotFound
 from rucio.common.types import InternalScope
 from rucio.core.lifetime_exception import define_eol
 from rucio.core.rse import get_rse_attribute, get_rse_name
 from rucio.db.sqla import filter_thread_work, models
 from rucio.db.sqla.constants import DIDType, LockState, RuleGrouping, RuleNotification, RuleState
 from rucio.db.sqla.session import read_session, stream_session, transactional_session
@@ -210,15 +211,15 @@
 def get_files_and_replica_locks_of_dataset(scope, name, nowait=False, restrict_rses=None, only_stuck=False,
                                            total_threads=None, thread_id=None,
                                            *, session: "Session"):
     """
     Get all the files of a dataset and, if existing, all locks of the file.
 
     :param scope:          Scope of the dataset
-    :param name:           Name of the datset
+    :param name:           Name of the dataset
     :param nowait:         Nowait parameter for the FOR UPDATE statement
     :param restrict_rses:  Possible RSE_ids to filter on.
     :param only_stuck:     If true, only get STUCK locks.
     :param total_threads:  Total threads
     :param thread_id:      This thread
     :param session:        The db session.
     :return:               Dictionary with keys: (scope, name)
@@ -395,15 +396,15 @@
     :param error_message:   The error why this transfer failed.
     :param broken_rule_id:  Id of the rule which will be suspended.
     :param broken_message:  Error message for the suspended rule.
     :param nowait:          Nowait parameter for the for_update queries.
     :param session:         The database session in use.
     """
 
-    staging_required = get_rse_attribute(rse_id, 'staging_required', session=session)
+    staging_required = get_rse_attribute(rse_id, RseAttr.STAGING_REQUIRED, session=session)
     if staging_required:
         rse_name = get_rse_name(rse_id=rse_id, session=session)
         logger(logging.DEBUG, f'Destination RSE {rse_name} is type staging_required so do not update other OK replica locks.')
         locks = session.query(models.ReplicaLock).with_for_update(nowait=nowait).filter_by(scope=scope, name=name, rse_id=rse_id, state=LockState.REPLICATING)
     else:
         locks = session.query(models.ReplicaLock).with_for_update(nowait=nowait).filter_by(scope=scope, name=name, rse_id=rse_id)
```

### Comparing `rucio-34.2.0/lib/rucio/core/message.py` & `rucio-34.3.0/lib/rucio/core/message.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/core/meta_conventions.py` & `rucio-34.3.0/lib/rucio/core/meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/core/monitor.py` & `rucio-34.3.0/lib/rucio/core/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,31 +22,34 @@
 import string
 from abc import abstractmethod
 from collections.abc import Callable, Iterable, Sequence
 from datetime import datetime, timedelta
 from functools import wraps
 from pathlib import Path
 from threading import Lock
-from typing import Any, Optional, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Optional, TypeVar, Union
 
 from prometheus_client import REGISTRY, CollectorRegistry, Counter, Gauge, Histogram, generate_latest, multiprocess, push_to_gateway, start_http_server, values
 from statsd import StatsClient
 
 import __main__ as main
 from rucio.common.config import config_get, config_get_bool, config_get_int
 from rucio.common.stopwatch import Stopwatch
 from rucio.common.utils import retrying
 
+if TYPE_CHECKING:
+    from rucio.common.types import LoggerFunction
+
 _T = TypeVar('_T')
 _M = TypeVar('_M', bound="_MultiMetric")
 
 PROMETHEUS_MULTIPROC_DIR = os.environ.get('PROMETHEUS_MULTIPROC_DIR', os.environ.get('prometheus_multiproc_dir', None))
 
 
-def cleanup_prometheus_files_at_exit():
+def cleanup_prometheus_files_at_exit() -> None:
     if PROMETHEUS_MULTIPROC_DIR:
         multiprocess.mark_process_dead(os.getpid())
 
 
 class MultiprocessMutexValue(values.MultiProcessValue()):
     """
     MultiprocessValue protected by mutex
@@ -95,15 +98,20 @@
 TIMINGS = {}
 METRICS_LOCK = Lock()
 
 
 _HISTOGRAM_DEFAULT_BUCKETS = Histogram.DEFAULT_BUCKETS
 
 
-def _cleanup_old_prometheus_files(path, file_pattern, cleanup_delay, logger):
+def _cleanup_old_prometheus_files(
+        path: str,
+        file_pattern: str,
+        cleanup_delay: float,
+        logger: "LoggerFunction"
+) -> None:
     """cleanup behind processes which didn't finish gracefully."""
 
     oldest_accepted_mtime = datetime.now() - timedelta(seconds=cleanup_delay)
     for file in Path(path).glob(file_pattern):
         if not file.is_file():
             continue
 
@@ -114,25 +122,25 @@
             try:
                 os.remove(file)
             except FileNotFoundError:
                 # Probably file already removed by another concurrent process
                 pass
 
 
-def cleanup_old_prometheus_files(logger=logging.log):
+def cleanup_old_prometheus_files(logger: "LoggerFunction" = logging.log) -> None:
     path = PROMETHEUS_MULTIPROC_DIR
     if path:
         _cleanup_old_prometheus_files(path, file_pattern='gauge_live*.db', cleanup_delay=timedelta(hours=1).total_seconds(), logger=logger)
         _cleanup_old_prometheus_files(path, file_pattern='*.db', cleanup_delay=timedelta(days=7).total_seconds(), logger=logger)
 
 
 @retrying(retry_on_exception=lambda _: True,
           wait_fixed=500,
           stop_max_attempt_number=2)
-def generate_prometheus_metrics():
+def generate_prometheus_metrics() -> bytes:
     cleanup_old_prometheus_files()
 
     registry = CollectorRegistry()
     multiprocess.MultiProcessCollector(registry)
     return generate_latest(registry)
 
 
@@ -203,26 +211,26 @@
 
     def inc(self, delta=1):
         delta = abs(delta)
         self._prom.inc(delta)
         if STATSD_CLIENT:
             STATSD_CLIENT.incr(self._statsd, delta)
 
-    def init_prometheus_metric(self, name: str, documentation: Optional[str], labelnames: Sequence[str] = ()):
+    def init_prometheus_metric(self, name: str, documentation: str, labelnames: Sequence[str] = ()) -> Counter:
         return Counter(name, documentation, labelnames=labelnames, registry=self._registry)
 
 
 class _MultiGauge(_MultiMetric):
 
     def set(self, value):
         self._prom.set(value)
         if STATSD_CLIENT:
             STATSD_CLIENT.gauge(self._statsd, value)
 
-    def init_prometheus_metric(self, name: str, documentation: Optional[str], labelnames: Sequence[str] = ()):
+    def init_prometheus_metric(self, name: str, documentation: str, labelnames: Sequence[str] = ()) -> Gauge:
         return Gauge(name, documentation, labelnames=labelnames, registry=self._registry)
 
 
 class _MultiTiming(_MultiMetric):
 
     def __init__(
             self,
@@ -238,15 +246,15 @@
         super().__init__(statsd, prom, documentation, labelnames, registry)
 
     def observe(self, value: float):
         self._prom.observe(value)
         if STATSD_CLIENT:
             STATSD_CLIENT.timing(self._statsd, value * 1000)
 
-    def init_prometheus_metric(self, name: str, documentation: Optional[str], labelnames: Sequence[str] = ()):
+    def init_prometheus_metric(self, name: str, documentation: str, labelnames: Sequence[str] = ()) -> Histogram:
         return Histogram(name, documentation, labelnames=labelnames, registry=self._registry, buckets=self._histogram_buckets)
 
     def __enter__(self):
         self._stopwatch = Stopwatch()
         return self
 
     def __exit__(self, typ, value, tb):
@@ -330,15 +338,15 @@
         elif module:
             self.prefix = module
         else:
             self.prefix = None
         self.registry = registry or REGISTRY
         self.push_gateways = push_gateways or []
 
-    def full_name(self, name: str):
+    def full_name(self, name: str) -> str:
         if self.prefix:
             return f'{self.prefix}.{name}'
         return name
 
     def get_registry(self) -> CollectorRegistry:
         return self.registry
```

### Comparing `rucio-34.2.0/lib/rucio/core/naming_convention.py` & `rucio-34.3.0/lib/rucio/core/naming_convention.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,33 +10,47 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from re import compile, error, match
 from traceback import format_exc
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Optional, cast
 
 from dogpile.cache.api import NO_VALUE
 from sqlalchemy.exc import IntegrityError
 
 from rucio.common.cache import make_region_memcached
 from rucio.common.exception import Duplicate, InvalidObject, RucioException
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import KeyType
 from rucio.db.sqla.session import read_session, transactional_session
 
 if TYPE_CHECKING:
+    from typing import TypedDict
+
     from sqlalchemy.orm import Session
 
+    from rucio.common.types import InternalScope
+
+    class NamingConventionDict(TypedDict):
+        scope: InternalScope
+        regexp: str
+
 REGION = make_region_memcached(expiration_time=900)
 
 
 @transactional_session
-def add_naming_convention(scope, regexp, convention_type, *, session: "Session"):
+def add_naming_convention(
+    scope: "InternalScope",
+    regexp: str,
+    convention_type: KeyType,
+    *,
+    session: "Session"
+) -> None:
     """
     add a naming convention for a given scope
 
     :param scope: the name for the scope.
     :param regexp: the regular expression to validate the name.
     :param convention_type: the did_type on which the regexp should apply.
     :param session: The database session in use.
@@ -55,15 +69,20 @@
     except IntegrityError:
         raise Duplicate('Naming convention already exists!')
     except:
         raise RucioException(str(format_exc()))
 
 
 @read_session
-def get_naming_convention(scope, convention_type, *, session: "Session"):
+def get_naming_convention(
+    scope: "InternalScope",
+    convention_type: KeyType,
+    *,
+    session: "Session"
+) -> Optional[str]:
     """
     Get the naming convention for a given scope
 
     :param scope: the name for the scope.
     :param convention_type: the did_type on which the regexp should apply.
     :param session: The database session in use.
 
@@ -73,74 +92,88 @@
         filter(models.NamingConvention.scope == scope).\
         filter(models.NamingConvention.convention_type == convention_type)
     for row in query:
         return row[0]
 
 
 @transactional_session
-def delete_naming_convention(scope, convention_type, *, session: "Session"):
+def delete_naming_convention(
+    scope: "InternalScope",
+    convention_type: KeyType,
+    *,
+    session: "Session"
+) -> int:
     """
     delete a naming convention for a given scope
 
     :param scope: the name for the scope.
     :param regexp: the regular expression to validate the name. (DEPRECATED)
     :param convention_type: the did_type on which the regexp should apply.
     :param session: The database session in use.
     """
-    REGION.delete(scope.internal)
+    if scope.internal is not None:
+        REGION.delete(scope.internal)
     return session.query(models.NamingConvention) \
         .filter_by(scope=scope, convention_type=convention_type) \
         .delete()
 
 
 @read_session
-def list_naming_conventions(*, session: "Session"):
+def list_naming_conventions(*, session: "Session") -> list["NamingConventionDict"]:
     """
     List all naming conventions.
 
     :param session: The database session in use.
 
     :returns: a list of dictionaries.
     """
     query = session.query(models.NamingConvention.scope,
                           models.NamingConvention.regexp)
-    return [row._asdict() for row in query]
+    return [cast("NamingConventionDict", row._asdict()) for row in query]
 
 
 @read_session
-def validate_name(scope, name, did_type, *, session: "Session"):
+def validate_name(
+    scope: "InternalScope",
+    name: str,
+    did_type: str,
+    *,
+    session: "Session"
+) -> Optional[dict[str, Any]]:
     """
     Validate a name according to a naming convention.
 
     :param scope: the name for the scope.
     :param name: the name.
     :param did_type: the type of did.
 
     :param session: The database session in use.
 
     :returns: a dictionary with metadata.
     """
-    if scope.external.startswith('user'):
-        return {'project': 'user'}
-    elif scope.external.startswith('group'):
-        return {'project': 'group'}
+    if scope.external is not None:
+        if scope.external.startswith('user'):
+            return {'project': 'user'}
+        elif scope.external.startswith('group'):
+            return {'project': 'group'}
 
     # Check if naming convention can be found in cache region
     regexp = REGION.get(scope.internal)
     if regexp is NO_VALUE:  # no cached entry found
         regexp = get_naming_convention(scope=scope,
                                        convention_type=KeyType.DATASET,
                                        session=session)
-        regexp and REGION.set(scope.internal, regexp)
+        if scope.internal is not None:
+            regexp and REGION.set(scope.internal, regexp)
 
     if not regexp:
         return
 
     # Validate with regexp
-    groups = match(regexp, str(name))
+    groups = match(regexp, str(name))  # type: ignore
     if groups:
         meta = groups.groupdict()
         # Hack to get task_id from version
         if 'version' in meta and meta['version']:
             matched = match(r'(?P<version>\w+)_tid(?P<task_id>\d+)_\w+$', meta['version'])
             if matched:
                 meta['version'] = matched.groupdict()['version']
```

### Comparing `rucio-34.2.0/lib/rucio/core/nongrid_trace.py` & `rucio-34.3.0/lib/rucio/core/nongrid_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/core/oidc.py` & `rucio-34.3.0/lib/rucio/core/oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
     :param ip: IP address of the client as a string.
     :param session: The database session in use.
 
     :returns: User & Rucio OIDC Client specific Authorization or Redirection URL as a string
               OR a redirection url to be used in user's browser for authentication.
     """
     # TO-DO - implement a check if that account already has a valid
-    # token withthe required scope and audience and return such token !
+    # token with the required scope and audience and return such token !
     auth_scope = kwargs.get('auth_scope', EXPECTED_OIDC_SCOPE)
     if not auth_scope:
         auth_scope = EXPECTED_OIDC_SCOPE
     audience = kwargs.get('audience', EXPECTED_OIDC_AUDIENCE)
     if not audience:
         audience = EXPECTED_OIDC_AUDIENCE
     # checking that minimal audience and scope requirements (required by Rucio) are satisfied !
@@ -752,29 +752,29 @@
         account_tokens = session.execute(query).scalars().all()
 
         # for Rucio Admin account we ask IdP for a token via client_credential grant
         # for each user account OIDC identity there is an OIDC issuer that must be, by construction,
         # supported by Rucio server (have OIDC admin client registered as well)
         # that is why we take the issuer of the account identity that has an active/valid token
         # and look for admin account identity which has this issuer assigned
-        # requestor should always have at least one active subject token unless it is root
-        # this is why we first discover if the requestor is root or not
+        # requester should always have at least one active subject token unless it is root
+        # this is why we first discover if the requester is root or not
         get_token_for_adminacc = False
         admin_identity = None
         admin_issuer = None
         admin_iss_acc_idt_dict = __get_admin_account_for_issuer(session=session)
 
         # check if preferred issuer exists - if multiple present last one is taken
         preferred_issuer = None
         for token in account_tokens:
             preferred_issuer = token.identity.split(", ")[1].split("=")[1]
-        # loop through all OIDC identities registerd for the account of the requestor
+        # loop through all OIDC identities registered for the account of the requester
         for identity in identities:
             issuer = identity.split(", ")[1].split("=")[1]
-            # compare the account of the requestor with the account of the admin
+            # compare the account of the requester with the account of the admin
             if account == admin_iss_acc_idt_dict[issuer][0]:
                 # take first matching case which means root is requesting OIDC authentication
                 admin_identity = admin_iss_acc_idt_dict[issuer][1]
                 if preferred_issuer and preferred_issuer != issuer:
                     continue
                 else:
                     admin_issuer = issuer
```

### Comparing `rucio-34.2.0/lib/rucio/core/permission/__init__.py` & `rucio-34.3.0/lib/rucio/core/permission/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import importlib
 from configparser import NoOptionError, NoSectionError
 from os import environ
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from rucio.common import config, exception
 from rucio.common.utils import check_policy_package_version
 
 if TYPE_CHECKING:
     from typing import Optional
 
     from sqlalchemy.orm import Session
 
+    from rucio.common.types import InternalAccount
+
 # dictionary of permission modules for each VO
 permission_modules = {}
 
 try:
     multivo = config.config_get_bool('common', 'multi_vo')
 except (NoOptionError, NoSectionError):
     multivo = False
@@ -68,15 +70,15 @@
         module = importlib.import_module(POLICY)
     except ImportError:
         raise exception.PolicyPackageNotFound('Module ' + POLICY + ' not found')
 
     permission_modules["def"] = module
 
 
-def load_permission_for_vo(vo):
+def load_permission_for_vo(vo: str) -> None:
     GENERIC_FALLBACK = 'generic_multi_vo'
     if config.config_has_section('policy'):
         try:
             env_name = 'RUCIO_POLICY_PACKAGE_' + vo.upper()
             if env_name in environ:
                 POLICY = environ[env_name]
             else:
@@ -97,11 +99,17 @@
         module = importlib.import_module(POLICY)
     except ImportError:
         raise exception.PolicyPackageNotFound('Module ' + POLICY + ' not found')
 
     permission_modules[vo] = module
 
 
-def has_permission(issuer, action, kwargs, *, session: "Optional[Session]" = None):
+def has_permission(
+        issuer: "InternalAccount",
+        action: str,
+        kwargs: dict[str, Any],
+        *,
+        session: "Optional[Session]" = None
+) -> bool:
     if issuer.vo not in permission_modules:
         load_permission_for_vo(issuer.vo)
     return permission_modules[issuer.vo].has_permission(issuer, action, kwargs, session=session)
```

### Comparing `rucio-34.2.0/lib/rucio/core/permission/atlas.py` & `rucio-34.3.0/lib/rucio/core/permission/atlas.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TYPE_CHECKING
 
 import rucio.core.did
 import rucio.core.scope
+from rucio.common.constants import RseAttr
 from rucio.core.account import has_account_attribute, list_account_attributes
 from rucio.core.identity import exist_identity_account
 from rucio.core.rse import list_rse_attributes
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.core.rule import get_rule
 from rucio.db.sqla.constants import BadPFNStatus, IdentityType
 
@@ -209,22 +210,22 @@
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
-    if kwargs['key'] in ['rule_deleters', 'auto_approve_bytes', 'auto_approve_files', 'rule_approvers', 'default_account_limit_bytes', 'default_limit_files', 'block_manual_approve']:
+    if kwargs['key'] in [RseAttr.RULE_DELETERS, RseAttr.AUTO_APPROVE_BYTES, RseAttr.AUTO_APPROVE_FILES, RseAttr.RULE_APPROVERS, RseAttr.DEFAULT_ACCOUNT_LIMIT_BYTES, RseAttr.DEFAULT_LIMIT_FILES, RseAttr.BLOCK_MANUAL_APPROVE]:
         # Check if user is a country admin
         admin_in_country = []
         for kv in list_account_attributes(account=issuer, session=session):
             if kv['key'].startswith('country-') and kv['value'] == 'admin':
                 admin_in_country.append(kv['key'].partition('-')[2])
         if admin_in_country:
-            if list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get('country') in admin_in_country:
+            if list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
                 return True
     return False
 
 
 def perm_del_rse_attribute(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can delete a RSE attribute.
@@ -232,22 +233,22 @@
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
-    if kwargs['key'] in ['rule_deleters', 'auto_approve_bytes', 'auto_approve_files', 'rule_approvers', 'default_account_limit_bytes', 'default_limit_files', 'block_manual_approve']:
+    if kwargs['key'] in [RseAttr.RULE_DELETERS, RseAttr.AUTO_APPROVE_BYTES, RseAttr.AUTO_APPROVE_FILES, RseAttr.RULE_APPROVERS, RseAttr.DEFAULT_ACCOUNT_LIMIT_BYTES, RseAttr.DEFAULT_LIMIT_FILES, RseAttr.BLOCK_MANUAL_APPROVE]:
         # Check if user is a country admin
         admin_in_country = []
         for kv in list_account_attributes(account=issuer, session=session):
             if kv['key'].startswith('country-') and kv['value'] == 'admin':
                 admin_in_country.append(kv['key'].partition('-')[2])
         if admin_in_country:
-            if list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get('country') in admin_in_country:
+            if list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
                 return True
     return False
 
 
 def perm_del_rse(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can delete a RSE.
@@ -513,22 +514,22 @@
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.append(kv['key'].partition('-')[2])
 
     rule = get_rule(rule_id=kwargs['rule_id'], session=session)
     rses = parse_expression(rule['rse_expression'], filter_={'vo': issuer.vo}, session=session)
     if admin_in_country:
         for rse in rses:
-            if list_rse_attributes(rse_id=rse['id'], session=session).get('country') in admin_in_country:
+            if list_rse_attributes(rse_id=rse['id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
                 return True
 
     # DELETERS can approve the rule
     for rse in rses:
         rse_attr = list_rse_attributes(rse_id=rse['id'], session=session)
-        if rse_attr.get('rule_deleters'):
-            if issuer.external in rse_attr.get('rule_deleters').split(','):
+        if rse_attr.get(RseAttr.RULE_DELETERS):
+            if issuer.external in rse_attr.get(RseAttr.RULE_DELETERS).split(','):
                 return True
 
     return False
 
 
 def perm_update_rule(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
@@ -553,15 +554,15 @@
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.append(kv['key'].partition('-')[2])
 
     rule = get_rule(rule_id=kwargs['rule_id'], session=session)
     rses = parse_expression(rule['rse_expression'], filter_={'vo': issuer.vo}, session=session)
     if admin_in_country:
         for rse in rses:
-            if list_rse_attributes(rse_id=rse['id'], session=session).get('country') in admin_in_country:
+            if list_rse_attributes(rse_id=rse['id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
                 return True
 
     # Only admin and country-admin are allowed to change locked state of rule
     if 'locked' in kwargs['options']:
         return False
 
     # Owner can change the rest of a rule
@@ -593,21 +594,21 @@
     admin_source = False
     admin_destination = False
 
     if admin_in_country:
         rule = get_rule(rule_id=kwargs['rule_id'], session=session)
         rses = parse_expression(rule['rse_expression'], filter_={'vo': issuer.vo}, session=session)
         for rse in rses:
-            if list_rse_attributes(rse_id=rse['id'], session=session).get('country') in admin_in_country:
+            if list_rse_attributes(rse_id=rse['id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
                 admin_source = True
                 break
 
         rses = parse_expression(kwargs['rse_expression'], filter_={'vo': issuer.vo}, session=session)
         for rse in rses:
-            if list_rse_attributes(rse_id=rse['id'], session=session).get('country') in admin_in_country:
+            if list_rse_attributes(rse_id=rse['id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
                 admin_destination = True
                 break
 
         if admin_source and admin_destination:
             return True
 
     return False
@@ -628,40 +629,40 @@
 
     rule = get_rule(rule_id=kwargs['rule_id'], session=session)
     rses = parse_expression(rule['rse_expression'], filter_={'vo': issuer.vo}, session=session)
 
     # APPROVERS can approve the rule
     for rse in rses:
         rse_attr = list_rse_attributes(rse_id=rse['id'], session=session)
-        if rse_attr.get('rule_approvers'):
-            if issuer.external in rse_attr.get('rule_approvers').split(','):
+        if rse_attr.get(RseAttr.RULE_APPROVERS):
+            if issuer.external in rse_attr.get(RseAttr.RULE_APPROVERS).split(','):
                 return True
 
     # LOCALGROUPDISK/LOCALGROUPTAPE admins can approve the rule
     admin_in_country = []
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.append(kv['key'].partition('-')[2])
     if admin_in_country:
         for rse in rses:
             rse_attr = list_rse_attributes(rse_id=rse['id'], session=session)
-            if rse_attr.get('type', '') in ('LOCALGROUPDISK', 'LOCALGROUPTAPE'):
-                if rse_attr.get('country', '') in admin_in_country:
+            if rse_attr.get(RseAttr.TYPE, '') in ('LOCALGROUPDISK', 'LOCALGROUPTAPE'):
+                if rse_attr.get(RseAttr.COUNTRY, '') in admin_in_country:
                     return True
 
     # GROUPDISK admins can approve the rule
     admin_for_phys_group = []
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('group-') and kv['value'] == 'admin':
             admin_for_phys_group.append(kv['key'].partition('-')[2])
     if admin_for_phys_group:
         for rse in rses:
             rse_attr = list_rse_attributes(rse_id=rse['id'], session=session)
-            if rse_attr.get('type', '') == 'GROUPDISK':
-                if rse_attr.get('physgroup', '') in admin_for_phys_group:
+            if rse_attr.get(RseAttr.TYPE, '') == 'GROUPDISK':
+                if rse_attr.get(RseAttr.PHYSGROUP, '') in admin_for_phys_group:
                     return True
 
     return False
 
 
 def perm_reduce_rule(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
@@ -849,22 +850,22 @@
     group = []
 
     for kv in list_account_attributes(account=issuer, session=session):
         if (kv['key'].startswith('group-') or kv['key'].startswith('country-')) and kv['value'] in ['admin', 'user']:
             group.append(kv['key'].partition('-')[2])
     rse_attr = list_rse_attributes(rse_id=rse_id, session=session)
     if group:
-        if rse_attr.get('type', '') == 'GROUPDISK':
-            if rse_attr.get('physgroup', '') in group:
+        if rse_attr.get(RseAttr.TYPE, '') == 'GROUPDISK':
+            if rse_attr.get(RseAttr.PHYSGROUP, '') in group:
                 return True
-        if rse_attr.get('type', '') == 'LOCALGROUPDISK':
-            if rse_attr.get('country', '') in group:
+        if rse_attr.get(RseAttr.TYPE, '') == 'LOCALGROUPDISK':
+            if rse_attr.get(RseAttr.COUNTRY, '') in group:
                 return True
 
-    return rse_attr.get('type', '') in ['SCRATCHDISK', 'MOCK', 'TEST']\
+    return rse_attr.get(RseAttr.TYPE, '') in ['SCRATCHDISK', 'MOCK', 'TEST']\
         or _is_root(issuer)\
         or has_account_attribute(account=issuer, key='admin', session=session)
 
 
 def perm_skip_availability_check(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can skip the availabity check to add/delete file replicas.
@@ -902,22 +903,22 @@
     group = []
 
     for kv in list_account_attributes(account=issuer, session=session):
         if (kv['key'].startswith('group-') or kv['key'].startswith('country-')) and kv['value'] in ['admin', 'user']:
             group.append(kv['key'].partition('-')[2])
     rse_attr = list_rse_attributes(rse_id=rse_id, session=session)
     if group:
-        if rse_attr.get('type', '') == 'GROUPDISK':
-            if rse_attr.get('physgroup', '') in group:
+        if rse_attr.get(RseAttr.TYPE, '') == 'GROUPDISK':
+            if rse_attr.get(RseAttr.PHYSGROUP, '') in group:
                 return True
-        if rse_attr.get('type', '') == 'LOCALGROUPDISK':
-            if rse_attr.get('country', '') in group:
+        if rse_attr.get(RseAttr.TYPE, '') == 'LOCALGROUPDISK':
+            if rse_attr.get(RseAttr.COUNTRY, '') in group:
                 return True
 
-    return rse_attr.get('type', '') in ['SCRATCHDISK', 'MOCK', 'TEST']\
+    return rse_attr.get(RseAttr.TYPE, '') in ['SCRATCHDISK', 'MOCK', 'TEST']\
         or _is_root(issuer)\
         or has_account_attribute(account=issuer, key='admin', session=session)
 
 
 def perm_queue_requests(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can submit transfer or deletion requests on destination RSEs for data identifiers.
@@ -1015,17 +1016,17 @@
         return True
     # Check if user is a country admin
     admin_in_country = []
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.append(kv['key'].partition('-')[2])
     rse_attr = list_rse_attributes(rse_id=kwargs['rse_id'], session=session)
-    if admin_in_country and rse_attr.get('country') in admin_in_country:
+    if admin_in_country and rse_attr.get(RseAttr.COUNTRY) in admin_in_country:
         return True
-    quota_approvers = rse_attr.get('quota_approvers', None)
+    quota_approvers = rse_attr.get(RseAttr.QUOTA_APPROVERS, None)
     if quota_approvers and issuer.external in quota_approvers.split(','):
         return True
     return False
 
 
 def perm_set_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
@@ -1039,15 +1040,15 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # Check if user is a country admin
     admin_in_country = set()
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.add(kv['key'].partition('-')[2])
-    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get('country')
+    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
                               for rse in parse_expression(kwargs['rse_expression'], filter_={'vo': issuer.vo}, session=session)}
     if resolved_rse_countries.issubset(admin_in_country):
         return True
     return False
 
 
 def perm_delete_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
@@ -1062,15 +1063,15 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # Check if user is a country admin
     admin_in_country = set()
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.add(kv['key'].partition('-')[2])
-    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get('country')
+    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
                               for rse in parse_expression(kwargs['rse_expression'], filter_={'vo': issuer.vo}, session=session)}
     if resolved_rse_countries.issubset(admin_in_country):
         return True
     return False
 
 
 def perm_delete_local_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
@@ -1086,17 +1087,17 @@
         return True
     # Check if user is a country admin
     admin_in_country = []
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.append(kv['key'].partition('-')[2])
     rse_attr = list_rse_attributes(rse_id=kwargs['rse_id'], session=session)
-    if admin_in_country and rse_attr.get('country') in admin_in_country:
+    if admin_in_country and rse_attr.get(RseAttr.COUNTRY) in admin_in_country:
         return True
-    quota_approvers = rse_attr.get('quota_approvers', None)
+    quota_approvers = rse_attr.get(RseAttr.QUOTA_APPROVERS, None)
     if quota_approvers and issuer.external in quota_approvers.split(','):
         return True
     return False
 
 
 def perm_config(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
```

### Comparing `rucio-34.2.0/lib/rucio/core/permission/belleii.py` & `rucio-34.3.0/lib/rucio/core/permission/belleii.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TYPE_CHECKING
 
 import rucio.core.scope
 from rucio.common.config import config_get
+from rucio.common.constants import RseAttr
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.core.account import has_account_attribute, list_account_attributes
 from rucio.core.did import get_metadata
 from rucio.core.identity import exist_identity_account
 from rucio.core.lifetime_exception import list_exceptions
 from rucio.core.rse import list_rse_attributes
 from rucio.core.rse_expression_parser import parse_expression
@@ -128,15 +129,15 @@
 def _perm_country(issuer: "InternalAccount", rses: list, roles: list, *, session: "Optional[Session]" = None) -> bool:
     admin_in_country = []
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.append(kv['key'].partition('-')[2])
     if admin_in_country:
         for rse in rses:
-            if list_rse_attributes(rse_id=rse['id'], session=session).get('country') in admin_in_country:
+            if list_rse_attributes(rse_id=rse['id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
                 return True
     return False
 
 
 def perm_default(issuer: "InternalAccount", kwargs: dict, *, session: "Optional[Session]" = None) -> bool:
     """
     Default permission.
@@ -506,16 +507,16 @@
     # Check if user is a country admin
     if _perm_country(issuer=issuer, rses=rses, roles=['admin', ], session=session):
         return True
 
     # DELETERS can delete the rule
     for rse in rses:
         rse_attr = list_rse_attributes(rse_id=rse['id'], session=session)
-        if rse_attr.get('rule_deleters'):
-            if issuer.external in rse_attr.get('rule_deleters').split(','):
+        if rse_attr.get(RseAttr.RULE_DELETERS):
+            if issuer.external in rse_attr.get(RseAttr.RULE_DELETERS).split(','):
                 return True
     return perm_default(issuer, kwargs, session=session)\
         or has_account_attribute(account=issuer, key='rule_admin', session=session)\
         or get_rule(kwargs['rule_id'], session=session)['account'] == issuer
 
 
 def perm_update_rule(issuer: "InternalAccount", kwargs: dict, *, session: "Optional[Session]" = None) -> bool:
```

### Comparing `rucio-34.2.0/lib/rucio/core/permission/cms.py` & `rucio-34.3.0/lib/rucio/core/permission/cms.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TYPE_CHECKING
 
 import rucio.core.scope
+from rucio.common.constants import RseAttr
 from rucio.core.account import has_account_attribute
 from rucio.core.identity import exist_identity_account
 from rucio.core.permission.generic import perm_get_global_account_usage
 from rucio.core.rse import list_rse_attributes
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.core.rule import get_rule
 from rucio.db.sqla.constants import IdentityType
@@ -185,15 +186,15 @@
     if isinstance(repr(issuer), str) and repr(issuer).startswith('sync_'):  # noqa
         return True
 
     # Anyone can use _Temp RSEs if a lifetime is set and under a month
     all_temp = True
     for rse in rses:
         rse_attr = list_rse_attributes(rse_id=rse['id'], session=session)
-        rse_type = rse_attr.get('cms_type', None)
+        rse_type = rse_attr.get(RseAttr.CMS_TYPE, None)
         if rse_type not in ['temp']:
             all_temp = False
 
     if all_temp and kwargs['lifetime'] is not None and kwargs['lifetime'] < 31 * 24 * 60 * 60:
         return True
 
     if kwargs['account'] == issuer and not kwargs['locked']:
@@ -544,15 +545,15 @@
 
     rule = get_rule(rule_id=kwargs['rule_id'])
     rses = parse_expression(rule['rse_expression'], filter_={'vo': issuer.vo}, session=session)
 
     # Those in rule_approvers can approve the rule
     for rse in rses:
         rse_attr = list_rse_attributes(rse_id=rse['id'], session=session)
-        rule_approvers = rse_attr.get('rule_approvers', None)
+        rule_approvers = rse_attr.get(RseAttr.RULE_APPROVERS, None)
         if rule_approvers and issuer.external in rule_approvers.split(','):
             return True
 
     return False
 
 
 def perm_reduce_rule(issuer, kwargs, *, session: "Optional[Session]" = None):
@@ -865,20 +866,20 @@
         return True
     # # Check if user is a country admin
     # admin_in_country = []
     # from rucio.core.account import has_account_attribute, list_account_attributes
     # for kv in list_account_attributes(account=issuer, session=session):
     #     if kv['key'].startswith('country-') and kv['value'] == 'admin':
     #         admin_in_country.append(kv['key'].partition('-')[2])
-    # if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get('country') in admin_in_country:
+    # if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
     #     return True
 
     # Those listed as quota approvers can add to quotas
     rse_attr = list_rse_attributes(rse_id=kwargs['rse_id'], session=session)
-    quota_approvers = rse_attr.get('quota_approvers', None)
+    quota_approvers = rse_attr.get(RseAttr.QUOTA_APPROVERS, None)
     if quota_approvers and issuer.external in quota_approvers.split(','):
         return True
 
     return False
 
 
 def perm_set_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
@@ -893,15 +894,15 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # # Check if user is a country admin
     # admin_in_country = set()
     # for kv in list_account_attributes(account=issuer, session=session):
     #     if kv['key'].startswith('country-') and kv['value'] == 'admin':
     #         admin_in_country.add(kv['key'].partition('-')[2])
-    # resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get('country')
+    # resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
     #                           for rse in parse_expression(kwargs['rse_expression'], filter={'vo': issuer.vo}, session=session)}
     # if resolved_rse_countries.issubset(admin_in_country):
     #     return True
     return False
 
 
 def perm_delete_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
@@ -917,15 +918,15 @@
         return True
     # # Check if user is a country admin
     # admin_in_country = set()
     # for kv in list_account_attributes(account=issuer, session=session):
     #     if kv['key'].startswith('country-') and kv['value'] == 'admin':
     #         admin_in_country.add(kv['key'].partition('-')[2])
     # if admin_in_country:
-    #     resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get('country')
+    #     resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
     #                               for rse in parse_expression(kwargs['rse_expression'], filter={'vo': issuer.vo}, session=session)}
     #     if resolved_rse_countries.issubset(admin_in_country):
     #         return True
     return False
 
 
 def perm_delete_local_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
@@ -940,19 +941,19 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # # Check if user is a country admin
     # admin_in_country = []
     # for kv in list_account_attributes(account=issuer, session=session):
     #     if kv['key'].startswith('country-') and kv['value'] == 'admin':
     #         admin_in_country.append(kv['key'].partition('-')[2])
-    # if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get('country') in admin_in_country:
+    # if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
     #     return True
 
     rse_attr = list_rse_attributes(rse_id=kwargs['rse_id'], session=session)
-    quota_approvers = rse_attr.get('quota_approvers', None)
+    quota_approvers = rse_attr.get(RseAttr.QUOTA_APPROVERS, None)
     if quota_approvers and issuer.external in quota_approvers.split(','):
         return True
 
     return False
 
 
 def perm_config(issuer, kwargs, *, session: "Optional[Session]" = None):
```

### Comparing `rucio-34.2.0/lib/rucio/core/permission/escape.py` & `rucio-34.3.0/lib/rucio/core/permission/escape.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TYPE_CHECKING
 
 import rucio.core.scope
+from rucio.common.constants import RseAttr
 from rucio.core.account import has_account_attribute, list_account_attributes
 from rucio.core.identity import exist_identity_account
 from rucio.core.lifetime_exception import list_exceptions
 from rucio.core.rse import list_rse_attributes
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.db.sqla.constants import IdentityType
 
@@ -811,15 +812,15 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # Check if user is a country admin
     admin_in_country = []
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.append(kv['key'].partition('-')[2])
-    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get('country') in admin_in_country:
+    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
         return True
     return False
 
 
 def perm_set_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can set a global account limit.
@@ -832,15 +833,15 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # Check if user is a country admin
     admin_in_country = set()
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.add(kv['key'].partition('-')[2])
-    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get('country')
+    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
                               for rse in parse_expression(kwargs['rse_expression'], filter_={'vo': issuer.vo}, session=session)}
     if resolved_rse_countries.issubset(admin_in_country):
         return True
     return False
 
 
 def perm_delete_local_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
@@ -855,15 +856,15 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # Check if user is a country admin
     admin_in_country = []
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.append(kv['key'].partition('-')[2])
-    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get('country') in admin_in_country:
+    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
         return True
     return False
 
 
 def perm_delete_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can delete a global account limit.
@@ -877,15 +878,15 @@
         return True
     # Check if user is a country admin
     admin_in_country = set()
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.add(kv['key'].partition('-')[2])
     if admin_in_country:
-        resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get('country')
+        resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
                                   for rse in parse_expression(kwargs['rse_expression'], filter_={'vo': issuer.vo}, session=session)}
         if resolved_rse_countries.issubset(admin_in_country):
             return True
     return False
 
 
 def perm_config(issuer, kwargs, *, session: "Optional[Session]" = None):
```

### Comparing `rucio-34.2.0/lib/rucio/core/permission/generic.py` & `rucio-34.3.0/lib/rucio/core/permission/generic_multi_vo.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TYPE_CHECKING
 
 import rucio.core.scope
+from rucio.common.constants import RseAttr
 from rucio.core.account import has_account_attribute, list_account_attributes
 from rucio.core.identity import exist_identity_account
 from rucio.core.lifetime_exception import list_exceptions
 from rucio.core.rse import list_rse_attributes
 from rucio.core.rse_expression_parser import parse_expression
+from rucio.core.rule import get_rule
 from rucio.db.sqla.constants import IdentityType
 
 if TYPE_CHECKING:
     from typing import Optional
 
     from sqlalchemy.orm import Session
 
@@ -48,16 +50,14 @@
             'add_subscription': perm_add_subscription,
             'add_scope': perm_add_scope,
             'add_rse': perm_add_rse,
             'update_rse': perm_update_rse,
             'add_protocol': perm_add_protocol,
             'del_protocol': perm_del_protocol,
             'update_protocol': perm_update_protocol,
-            'add_qos_policy': perm_add_qos_policy,
-            'delete_qos_policy': perm_delete_qos_policy,
             'declare_bad_file_replicas': perm_declare_bad_file_replicas,
             'declare_suspicious_file_replicas': perm_declare_suspicious_file_replicas,
             'add_replicas': perm_add_replicas,
             'delete_replicas': perm_delete_replicas,
             'skip_availability_check': perm_skip_availability_check,
             'update_replicas_states': perm_update_replicas_states,
             'add_rse_attribute': perm_add_rse_attribute,
@@ -77,15 +77,14 @@
             'add_did': perm_add_did,
             'add_dids': perm_add_dids,
             'attach_dids': perm_attach_dids,
             'detach_dids': perm_detach_dids,
             'attach_dids_to_dids': perm_attach_dids_to_dids,
             'create_did_sample': perm_create_did_sample,
             'set_metadata': perm_set_metadata,
-            'set_metadata_bulk': perm_set_metadata_bulk,
             'set_status': perm_set_status,
             'queue_requests': perm_queue_requests,
             'set_rse_usage': perm_set_rse_usage,
             'set_rse_limits': perm_set_rse_limits,
             'list_requests': perm_list_requests,
             'list_requests_history': perm_list_requests_history,
             'get_request_by_did': perm_get_request_by_did,
@@ -116,15 +115,19 @@
             'get_auth_token_ssh': perm_get_auth_token_ssh,
             'get_signed_url': perm_get_signed_url,
             'add_bad_pfns': perm_add_bad_pfns,
             'del_account_identity': perm_del_account_identity,
             'del_identity': perm_del_identity,
             'remove_did_from_followed': perm_remove_did_from_followed,
             'remove_dids_from_followed': perm_remove_dids_from_followed,
-            'export': perm_export}
+            'add_vo': perm_add_vo,
+            'list_vos': perm_list_vos,
+            'recover_vo_root_identity': perm_recover_vo_root_identity,
+            'update_vo': perm_update_vo,
+            'access_rule_vo': perm_access_rule_vo}
 
     return perm.get(action, perm_default)(issuer=issuer, kwargs=kwargs, session=session)
 
 
 def _is_root(issuer):
     return issuer.external == 'root'
 
@@ -562,26 +565,14 @@
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return perm_attach_dids(issuer, kwargs, session=session)
 
 
-def perm_set_metadata_bulk(issuer: "InternalAccount", kwargs: dict, *, session: "Optional[Session]" = None) -> bool:
-    """
-    Checks if an account can set a metadata on a data identifier.
-
-    :param issuer: Account identifier which issues the command.
-    :param kwargs: List of arguments for the action.
-    :param session: The DB session to use
-    :returns: True if account is allowed, otherwise False
-    """
-    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session) or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)
-
-
 def perm_set_metadata(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can set a metadata on a data identifier.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
@@ -638,38 +629,14 @@
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_add_qos_policy(issuer, kwargs, *, session: "Optional[Session]" = None):
-    """
-    Checks if an account can add QoS policies to an RSE.
-
-    :param issuer: Account identifier which issues the command.
-    :param kwargs: List of arguments for the action.
-    :param session: The DB session to use
-    :returns: True if account is allowed, otherwise False
-    """
-    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
-
-
-def perm_delete_qos_policy(issuer, kwargs, *, session: "Optional[Session]" = None):
-    """
-    Checks if an account can delete QoS policies from an RSE.
-
-    :param issuer: Account identifier which issues the command.
-    :param kwargs: List of arguments for the action.
-    :param session: The DB session to use
-    :returns: True if account is allowed, otherwise False
-    """
-    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
-
-
 def perm_declare_bad_file_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can declare bad file replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
@@ -863,15 +830,15 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # Check if user is a country admin
     admin_in_country = []
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.append(kv['key'].partition('-')[2])
-    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get('country') in admin_in_country:
+    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
         return True
     return False
 
 
 def perm_set_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can set a global account limit.
@@ -884,15 +851,15 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # Check if user is a country admin
     admin_in_country = set()
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.add(kv['key'].partition('-')[2])
-    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get('country')
+    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
                               for rse in parse_expression(kwargs['rse_expression'], filter_={'vo': issuer.vo}, session=session)}
     if resolved_rse_countries.issubset(admin_in_country):
         return True
     return False
 
 
 def perm_delete_local_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
@@ -907,15 +874,15 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # Check if user is a country admin
     admin_in_country = []
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.append(kv['key'].partition('-')[2])
-    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get('country') in admin_in_country:
+    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
         return True
     return False
 
 
 def perm_delete_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can delete a global account limit.
@@ -929,15 +896,15 @@
         return True
     # Check if user is a country admin
     admin_in_country = set()
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.add(kv['key'].partition('-')[2])
     if admin_in_country:
-        resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get('country')
+        resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
                                   for rse in parse_expression(kwargs['rse_expression'], filter_={'vo': issuer.vo}, session=session)}
         if resolved_rse_countries.issubset(admin_in_country):
             return True
     return False
 
 
 def perm_config(issuer, kwargs, *, session: "Optional[Session]" = None):
@@ -979,17 +946,23 @@
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session) or kwargs.get('account') == issuer:
         return True
 
     # Check if user is a country admin for all involved countries
+    admin_in_country = set()
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
-            return True
+            admin_in_country.add(kv['key'].partition('-')[2])
+    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
+                              for rse in parse_expression(kwargs['rse_exp'], filter_={'vo': issuer.vo}, session=session)}
+
+    if resolved_rse_countries.issubset(admin_in_country):
+        return True
     return False
 
 
 def perm_add_account_attribute(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can add attributes to accounts.
 
@@ -1113,17 +1086,65 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     if not kwargs['account'] == issuer:
         return False
     return True
 
 
-def perm_export(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_vo(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
-    Checks if an account can export the RSE info.
+    Checks if an account can add a VO.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-    return _is_root(issuer)
+    return (issuer.internal == 'super_root')
+
+
+def perm_list_vos(issuer, kwargs, *, session: "Optional[Session]" = None):
+    """
+    Checks if an account can list a VO.
+
+    :param issuer: Account identifier which issues the command.
+    :param kwargs: List of arguments for the action.
+    :param session: The DB session to use
+    :returns: True if account is allowed, otherwise False
+    """
+    return (issuer.internal == 'super_root')
+
+
+def perm_recover_vo_root_identity(issuer, kwargs, *, session: "Optional[Session]" = None):
+    """
+    Checks if an account can recover identities for VOs.
+
+    :param issuer: Account identifier which issues the command.
+    :param kwargs: List of arguments for the action.
+    :param session: The DB session to use
+    :returns: True if account is allowed, otherwise False
+    """
+    return (issuer.internal == 'super_root')
+
+
+def perm_update_vo(issuer, kwargs, *, session: "Optional[Session]" = None):
+    """
+    Checks if an account can update a VO.
+
+    :param issuer: Account identifier which issues the command.
+    :param kwargs: List of arguments for the action.
+    :param session: The DB session to use
+    :returns: True if account is allowed, otherwise False
+    """
+    return (issuer.internal == 'super_root')
+
+
+def perm_access_rule_vo(issuer, kwargs, *, session: "Optional[Session]" = None):
+    """
+    Checks if we're at the same VO as the rule_id's
+
+    :param issuer: Account identifier which issues the command.
+    :param kwargs: List of arguments for the action.
+    :param session: The DB session to use
+    :returns: True if account is allowed, otherwise False
+    """
+    return get_rule(kwargs['rule_id'])['scope'].vo == issuer.vo
```

### Comparing `rucio-34.2.0/lib/rucio/core/permission/generic_multi_vo.py` & `rucio-34.3.0/lib/rucio/core/permission/generic.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 import rucio.core.scope
+from rucio.common.constants import RseAttr
 from rucio.core.account import has_account_attribute, list_account_attributes
 from rucio.core.identity import exist_identity_account
 from rucio.core.lifetime_exception import list_exceptions
 from rucio.core.rse import list_rse_attributes
 from rucio.core.rse_expression_parser import parse_expression
-from rucio.core.rule import get_rule
 from rucio.db.sqla.constants import IdentityType
 
 if TYPE_CHECKING:
     from typing import Optional
 
     from sqlalchemy.orm import Session
 
     from rucio.common.types import InternalAccount
 
 
-def has_permission(issuer, action, kwargs, *, session: "Optional[Session]" = None):
+def has_permission(issuer: "InternalAccount", action: str, kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account has the specified permission to
     execute an action with parameters.
 
     :param issuer: Account identifier which issues the command..
     :param action:  The action(API call) called by the account.
     :param kwargs: List of arguments for the action.
@@ -49,14 +49,16 @@
             'add_subscription': perm_add_subscription,
             'add_scope': perm_add_scope,
             'add_rse': perm_add_rse,
             'update_rse': perm_update_rse,
             'add_protocol': perm_add_protocol,
             'del_protocol': perm_del_protocol,
             'update_protocol': perm_update_protocol,
+            'add_qos_policy': perm_add_qos_policy,
+            'delete_qos_policy': perm_delete_qos_policy,
             'declare_bad_file_replicas': perm_declare_bad_file_replicas,
             'declare_suspicious_file_replicas': perm_declare_suspicious_file_replicas,
             'add_replicas': perm_add_replicas,
             'delete_replicas': perm_delete_replicas,
             'skip_availability_check': perm_skip_availability_check,
             'update_replicas_states': perm_update_replicas_states,
             'add_rse_attribute': perm_add_rse_attribute,
@@ -76,14 +78,15 @@
             'add_did': perm_add_did,
             'add_dids': perm_add_dids,
             'attach_dids': perm_attach_dids,
             'detach_dids': perm_detach_dids,
             'attach_dids_to_dids': perm_attach_dids_to_dids,
             'create_did_sample': perm_create_did_sample,
             'set_metadata': perm_set_metadata,
+            'set_metadata_bulk': perm_set_metadata_bulk,
             'set_status': perm_set_status,
             'queue_requests': perm_queue_requests,
             'set_rse_usage': perm_set_rse_usage,
             'set_rse_limits': perm_set_rse_limits,
             'list_requests': perm_list_requests,
             'list_requests_history': perm_list_requests_history,
             'get_request_by_did': perm_get_request_by_did,
@@ -114,64 +117,60 @@
             'get_auth_token_ssh': perm_get_auth_token_ssh,
             'get_signed_url': perm_get_signed_url,
             'add_bad_pfns': perm_add_bad_pfns,
             'del_account_identity': perm_del_account_identity,
             'del_identity': perm_del_identity,
             'remove_did_from_followed': perm_remove_did_from_followed,
             'remove_dids_from_followed': perm_remove_dids_from_followed,
-            'add_vo': perm_add_vo,
-            'list_vos': perm_list_vos,
-            'recover_vo_root_identity': perm_recover_vo_root_identity,
-            'update_vo': perm_update_vo,
-            'access_rule_vo': perm_access_rule_vo}
+            'export': perm_export}
 
     return perm.get(action, perm_default)(issuer=issuer, kwargs=kwargs, session=session)
 
 
-def _is_root(issuer):
+def _is_root(issuer) -> bool:
     return issuer.external == 'root'
 
 
-def perm_default(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_default(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Default permission.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_add_rse(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_rse(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can add a RSE.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_update_rse(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_update_rse(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can update a RSE.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_add_rule(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_rule(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can add a replication rule.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
@@ -179,212 +178,212 @@
     if kwargs['account'] == issuer and not kwargs['locked']:
         return True
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     return False
 
 
-def perm_add_subscription(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_subscription(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can add a subscription.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     return False
 
 
-def perm_add_rse_attribute(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_rse_attribute(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can add a RSE attribute.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     return False
 
 
-def perm_del_rse_attribute(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_del_rse_attribute(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can delete a RSE attribute.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     return False
 
 
-def perm_del_rse(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_del_rse(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can delete a RSE.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_add_account(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_account(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can add an account.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer)
 
 
-def perm_del_account(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_del_account(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can del an account.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer)
 
 
-def perm_update_account(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_update_account(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can update an account.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_add_scope(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_scope(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can add a scop to a account.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_get_auth_token_user_pass(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_get_auth_token_user_pass(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if a user can request a token with user_pass for an account.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if exist_identity_account(identity=kwargs['username'], type_=IdentityType.USERPASS, account=kwargs['account'], session=session):
         return True
     return False
 
 
-def perm_get_auth_token_gss(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_get_auth_token_gss(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if a user can request a token with user_pass for an account.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if exist_identity_account(identity=kwargs['gsscred'], type_=IdentityType.GSS, account=kwargs['account'], session=session):
         return True
     return False
 
 
-def perm_get_auth_token_x509(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_get_auth_token_x509(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if a user can request a token with user_pass for an account.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if exist_identity_account(identity=kwargs['dn'], type_=IdentityType.X509, account=kwargs['account'], session=session):
         return True
     return False
 
 
-def perm_get_auth_token_saml(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_get_auth_token_saml(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if a user can request a token with user_pass for an account.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if exist_identity_account(identity=kwargs['saml_nameid'], type_=IdentityType.SAML, account=kwargs['account'], session=session):
         return True
     return False
 
 
-def perm_add_account_identity(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_account_identity(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can add an identity to an account.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
 
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_del_account_identity(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_del_account_identity(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can delete an identity to an account.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
 
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_del_identity(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_del_identity(issuer: "InternalAccount", kwargs, *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can delete an identity.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
 
     return _is_root(issuer) or issuer.external in kwargs.get('accounts')
 
 
-def perm_add_did(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_did(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can add an data identifier to a scope.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
@@ -397,15 +396,15 @@
 
     return _is_root(issuer)\
         or has_account_attribute(account=issuer, key='admin', session=session)\
         or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)\
         or kwargs['scope'].external == 'mock'
 
 
-def perm_add_dids(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_dids(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can bulk add data identifiers.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
@@ -416,30 +415,30 @@
             for rule in did.get('rules', []):
                 if rule['account'] != issuer:
                     return False
 
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_attach_dids(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_attach_dids(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can append an data identifier to the other data identifier.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer)\
         or has_account_attribute(account=issuer, key='admin', session=session)\
         or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)\
         or kwargs['scope'].external == 'mock'
 
 
-def perm_attach_dids_to_dids(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_attach_dids_to_dids(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can append an data identifier to the other data identifier.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
@@ -452,139 +451,151 @@
         scopes = list(set(scopes))
         for scope in scopes:
             if not rucio.core.scope.is_scope_owner(scope, issuer, session=session):
                 return False
         return True
 
 
-def perm_create_did_sample(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_create_did_sample(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can create a sample of a data identifier collection.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer)\
         or has_account_attribute(account=issuer, key='admin', session=session)\
         or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)\
         or kwargs['scope'].external == 'mock'
 
 
-def perm_del_rule(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_del_rule(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an issuer can delete a replication rule.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     return False
 
 
-def perm_update_rule(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_update_rule(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an issuer can update a replication rule.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     return False
 
 
-def perm_approve_rule(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_approve_rule(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an issuer can approve a replication rule.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     return False
 
 
-def perm_reduce_rule(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_reduce_rule(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an issuer can reduce a replication rule.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     return False
 
 
-def perm_move_rule(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_move_rule(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an issuer can move a replication rule.
 
     :param issuer:   Account identifier which issues the command.
     :param kwargs:   List of arguments for the action.
     :param session: The DB session to use
     :returns:        True if account is allowed to call the API call, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     return False
 
 
-def perm_update_subscription(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_update_subscription(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can update a subscription.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
 
     return False
 
 
-def perm_detach_dids(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_detach_dids(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can detach an data identifier from the other data identifier.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return perm_attach_dids(issuer, kwargs, session=session)
 
 
-def perm_set_metadata(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_set_metadata_bulk(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can set a metadata on a data identifier.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session) or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)
 
 
-def perm_set_status(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_set_metadata(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
+    """
+    Checks if an account can set a metadata on a data identifier.
+
+    :param issuer: Account identifier which issues the command.
+    :param kwargs: List of arguments for the action.
+    :param session: The DB session to use
+    :returns: True if account is allowed, otherwise False
+    """
+    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session) or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)
+
+
+def perm_set_status(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can set status on an data identifier.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
@@ -592,75 +603,99 @@
     if kwargs.get('open', False):
         if not _is_root(issuer) and not has_account_attribute(account=issuer, key='admin', session=session):
             return False
 
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session) or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)
 
 
-def perm_add_protocol(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_protocol(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can add a protocol to an RSE.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_del_protocol(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_del_protocol(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can delete protocols from an RSE.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_update_protocol(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_update_protocol(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can update protocols of an RSE.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_declare_bad_file_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_qos_policy(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
+    """
+    Checks if an account can add QoS policies to an RSE.
+
+    :param issuer: Account identifier which issues the command.
+    :param kwargs: List of arguments for the action.
+    :param session: The DB session to use
+    :returns: True if account is allowed, otherwise False
+    """
+    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
+
+
+def perm_delete_qos_policy(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
+    """
+    Checks if an account can delete QoS policies from an RSE.
+
+    :param issuer: Account identifier which issues the command.
+    :param kwargs: List of arguments for the action.
+    :param session: The DB session to use
+    :returns: True if account is allowed, otherwise False
+    """
+    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
+
+
+def perm_declare_bad_file_replicas(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can declare bad file replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer)
 
 
-def perm_declare_suspicious_file_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_declare_suspicious_file_replicas(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can declare suspicious file replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return True
 
 
-def perm_add_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_replicas(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can add replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
@@ -669,159 +704,159 @@
         or str(kwargs.get('rse', '')).endswith('USERDISK')\
         or str(kwargs.get('rse', '')).endswith('MOCK')\
         or str(kwargs.get('rse', '')).endswith('LOCALGROUPDISK')\
         or _is_root(issuer)\
         or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_skip_availability_check(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_skip_availability_check(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can skip the availabity check to add/delete file replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_delete_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_delete_replicas(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can delete replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return False
 
 
-def perm_update_replicas_states(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_update_replicas_states(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can delete replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_queue_requests(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_queue_requests(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can submit transfer or deletion requests on destination RSEs for data identifiers.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer)
 
 
-def perm_list_requests(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_list_requests(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can list requests.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_list_requests_history(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_list_requests_history(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can list historical requests.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_get_request_by_did(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_get_request_by_did(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can get a request by DID.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return True
 
 
-def perm_get_request_history_by_did(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_get_request_history_by_did(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can get a historical request by DID.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_cancel_request(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_cancel_request(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can cancel a request.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer)
 
 
-def perm_get_next(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_get_next(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can retrieve the next request matching the request type and state.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer)
 
 
-def perm_set_rse_usage(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_set_rse_usage(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can set RSE usage information.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     return _is_root(issuer)
 
 
-def perm_set_rse_limits(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_set_rse_limits(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can set RSE limits.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_set_local_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_set_local_account_limit(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can set an account limit.
 
     :param account: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
@@ -829,20 +864,20 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # Check if user is a country admin
     admin_in_country = []
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.append(kv['key'].partition('-')[2])
-    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get('country') in admin_in_country:
+    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
         return True
     return False
 
 
-def perm_set_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_set_global_account_limit(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can set a global account limit.
 
     :param account: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
@@ -850,22 +885,22 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # Check if user is a country admin
     admin_in_country = set()
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.add(kv['key'].partition('-')[2])
-    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get('country')
+    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
                               for rse in parse_expression(kwargs['rse_expression'], filter_={'vo': issuer.vo}, session=session)}
     if resolved_rse_countries.issubset(admin_in_country):
         return True
     return False
 
 
-def perm_delete_local_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_delete_local_account_limit(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can delete an account limit.
 
     :param account: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
@@ -873,20 +908,20 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     # Check if user is a country admin
     admin_in_country = []
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.append(kv['key'].partition('-')[2])
-    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get('country') in admin_in_country:
+    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
         return True
     return False
 
 
-def perm_delete_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_delete_global_account_limit(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can delete a global account limit.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
@@ -895,34 +930,34 @@
         return True
     # Check if user is a country admin
     admin_in_country = set()
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             admin_in_country.add(kv['key'].partition('-')[2])
     if admin_in_country:
-        resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get('country')
+        resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
                                   for rse in parse_expression(kwargs['rse_expression'], filter_={'vo': issuer.vo}, session=session)}
         if resolved_rse_countries.issubset(admin_in_country):
             return True
     return False
 
 
-def perm_config(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_config(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can read/write the configuration.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_get_local_account_usage(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_get_local_account_usage(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can get the account usage of an account.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
@@ -932,88 +967,82 @@
     # Check if user is a country admin
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
             return True
     return False
 
 
-def perm_get_global_account_usage(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_get_global_account_usage(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can get the account usage of an account.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session) or kwargs.get('account') == issuer:
         return True
 
     # Check if user is a country admin for all involved countries
-    admin_in_country = set()
     for kv in list_account_attributes(account=issuer, session=session):
         if kv['key'].startswith('country-') and kv['value'] == 'admin':
-            admin_in_country.add(kv['key'].partition('-')[2])
-    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get('country')
-                              for rse in parse_expression(kwargs['rse_exp'], filter_={'vo': issuer.vo}, session=session)}
-
-    if resolved_rse_countries.issubset(admin_in_country):
-        return True
+            return True
     return False
 
 
-def perm_add_account_attribute(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_account_attribute(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can add attributes to accounts.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_del_account_attribute(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_del_account_attribute(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can add attributes to accounts.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     return perm_add_account_attribute(issuer, kwargs, session=session)
 
 
-def perm_list_heartbeats(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_list_heartbeats(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can list heartbeats.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     return _is_root(issuer)
 
 
-def perm_resurrect(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_resurrect(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can resurrect DIDS.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_update_lifetime_exceptions(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_update_lifetime_exceptions(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can approve/reject Lifetime Model exceptions.
 
     :param issuer: Account identifier which issues the command.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
@@ -1031,53 +1060,53 @@
     :param issuer: Account identifier which issues the command.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     return True
 
 
-def perm_get_signed_url(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_get_signed_url(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can request a signed URL.
 
     :param issuer: Account identifier which issues the command.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     return _is_root(issuer)
 
 
-def perm_add_bad_pfns(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_bad_pfns(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can declare bad PFNs.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer)
 
 
-def perm_remove_did_from_followed(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_remove_did_from_followed(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can remove did from followed table.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer)\
         or has_account_attribute(account=issuer, key='admin', session=session)\
         or kwargs['account'] == issuer\
         or kwargs['scope'].external == 'mock'
 
 
-def perm_remove_dids_from_followed(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_remove_dids_from_followed(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can bulk remove dids from followed table.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
@@ -1085,65 +1114,17 @@
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     if not kwargs['account'] == issuer:
         return False
     return True
 
 
-def perm_add_vo(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_export(issuer: "InternalAccount", kwargs: dict[str, Any], *, session: "Optional[Session]" = None) -> bool:
     """
-    Checks if an account can add a VO.
+    Checks if an account can export the RSE info.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-    return (issuer.internal == 'super_root')
-
-
-def perm_list_vos(issuer, kwargs, *, session: "Optional[Session]" = None):
-    """
-    Checks if an account can list a VO.
-
-    :param issuer: Account identifier which issues the command.
-    :param kwargs: List of arguments for the action.
-    :param session: The DB session to use
-    :returns: True if account is allowed, otherwise False
-    """
-    return (issuer.internal == 'super_root')
-
-
-def perm_recover_vo_root_identity(issuer, kwargs, *, session: "Optional[Session]" = None):
-    """
-    Checks if an account can recover identities for VOs.
-
-    :param issuer: Account identifier which issues the command.
-    :param kwargs: List of arguments for the action.
-    :param session: The DB session to use
-    :returns: True if account is allowed, otherwise False
-    """
-    return (issuer.internal == 'super_root')
-
-
-def perm_update_vo(issuer, kwargs, *, session: "Optional[Session]" = None):
-    """
-    Checks if an account can update a VO.
-
-    :param issuer: Account identifier which issues the command.
-    :param kwargs: List of arguments for the action.
-    :param session: The DB session to use
-    :returns: True if account is allowed, otherwise False
-    """
-    return (issuer.internal == 'super_root')
-
-
-def perm_access_rule_vo(issuer, kwargs, *, session: "Optional[Session]" = None):
-    """
-    Checks if we're at the same VO as the rule_id's
-
-    :param issuer: Account identifier which issues the command.
-    :param kwargs: List of arguments for the action.
-    :param session: The DB session to use
-    :returns: True if account is allowed, otherwise False
-    """
-    return get_rule(kwargs['rule_id'])['scope'].vo == issuer.vo
+    return _is_root(issuer)
```

### Comparing `rucio-34.2.0/lib/rucio/core/quarantined_replica.py` & `rucio-34.3.0/lib/rucio/core/quarantined_replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     Bulk add quarantined file replicas.
 
     :param rse_id:      The rse id.
     :param replicas: A list of dicts with the replica information.
     :param session:  The database session in use.
     """
 
-    # Exlude files that have a registered replica.  This is a
+    # Exclude files that have a registered replica.  This is a
     # safeguard against potential issues in the Auditor.
     file_clause = []
     for replica in replicas:
         if "scope" in replica and "name" in replica:
             file_clause.append(and_(models.RSEFileAssociation.scope == replica['scope'],
                                     models.RSEFileAssociation.name == replica['name'],
                                     models.RSEFileAssociation.rse_id == rse_id))
```

### Comparing `rucio-34.2.0/lib/rucio/core/replica.py` & `rucio-34.3.0/lib/rucio/core/replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 import copy
 import heapq
 import logging
 import math
 import random
 from collections import defaultdict, namedtuple
 from curses.ascii import isprint
@@ -37,15 +38,15 @@
 from sqlalchemy.sql.expression import case, false, literal, literal_column, null, select, text, true
 
 import rucio.core.did
 import rucio.core.lock
 from rucio.common import exception
 from rucio.common.cache import make_region_memcached
 from rucio.common.config import config_get, config_get_bool
-from rucio.common.constants import SuspiciousAvailability
+from rucio.common.constants import RseAttr, SuspiciousAvailability
 from rucio.common.types import InternalScope
 from rucio.common.utils import add_url_query, chunks, clean_surls, str_to_date
 from rucio.core.credential import get_signed_url
 from rucio.core.message import add_messages
 from rucio.core.monitor import MetricManager
 from rucio.core.rse import get_rse, get_rse_attribute, get_rse_name, get_rse_vo, list_rses
 from rucio.core.rse_counter import decrease, increase
@@ -790,34 +791,34 @@
         logger=logging.log,
         *,
         session: "Session",
 ) -> str:
     """
     Generate the PFN for the given scope/name on the rse.
     If needed, sign the PFN url
-    If relevant, add the server-side root proxy to te pfn url
+    If relevant, add the server-side root proxy to the pfn url
     """
     pfn: str = list(protocol.lfns2pfns(lfns={'scope': scope.external,
                                              'name': name,
                                              'path': path}).values())[0]
 
     # do we need to sign the URLs?
     if sign_urls and protocol.attributes['scheme'] == 'https':
-        service = get_rse_attribute(rse_id, 'sign_url', session=session)
+        service = get_rse_attribute(rse_id, RseAttr.SIGN_URL, session=session)
         if service:
             pfn = get_signed_url(rse_id=rse_id, service=service, operation='read', url=pfn, lifetime=signature_lifetime)
 
     # server side root proxy handling if location is set.
     # supports root and http destinations
     # cannot be pushed into protocols because we need to lookup rse attributes.
     # ultra-conservative implementation.
     if domain == 'wan' and protocol.attributes['scheme'] in ['root', 'http', 'https'] and client_location:
 
         if 'site' in client_location and client_location['site']:
-            replica_site = get_rse_attribute(rse_id, 'site', session=session)
+            replica_site = get_rse_attribute(rse_id, RseAttr.SITE, session=session)
 
             # does it match with the client? if not, it's an outgoing connection
             # therefore the internal proxy must be prepended
             if client_location['site'] != replica_site:
                 cache_site = config_get('clientcachemap', client_location['site'], default='', session=session)
                 if cache_site != '':
                     # print('client', client_location['site'], 'has cache:', cache_site)
@@ -838,25 +839,25 @@
                         #       For now -> skip prepending XCache for GCS.
                         if 'storage.googleapis.com' in pfn or 'atlas-google-cloud.cern.ch' in pfn or 'amazonaws.com' in pfn:
                             pass  # ATLAS HACK
                         else:
                             # don't forget to mangle gfal-style davs URL into generic https URL
                             pfn = f"root://{root_proxy_internal}//{pfn.replace('davs://', 'https://')}"
 
-    simulate_multirange = get_rse_attribute(rse_id, 'simulate_multirange')
+    simulate_multirange = get_rse_attribute(rse_id, RseAttr.SIMULATE_MULTIRANGE)
 
     if simulate_multirange is not None:
         try:
             # cover values that cannot be cast to int
             simulate_multirange = int(simulate_multirange)
         except ValueError:
             simulate_multirange = 1
-            logger(logging.WARNING, 'Value encountered when retrieving RSE attribute "simulate_multirange" not compatible with "int", used default value "1".')
+            logger(logging.WARNING, 'Value encountered when retrieving RSE attribute "%s" not compatible with "int", used default value "1".', RseAttr.SIMULATE_MULTIRANGE)
         if simulate_multirange <= 0:
-            logger(logging.WARNING, f'Value {simulate_multirange} encountered when retrieving RSE attribute "simulate_multirange" is <= 0, used default value "1".')
+            logger(logging.WARNING, f'Value {simulate_multirange} encountered when retrieving RSE attribute "{RseAttr.SIMULATE_MULTIRANGE}" is <= 0, used default value "1".')
             simulate_multirange = 1
         pfn += f'&#multirange=false&nconnections={simulate_multirange}'
 
     return pfn
 
 
 def _list_replicas(replicas, show_pfns, schemes, files_wo_replica, client_location, domain,
@@ -931,15 +932,15 @@
                 if is_archive:
                     t_scope = archive_scope
                     t_name = archive_name
                 else:
                     t_scope = scope
                     t_name = name
 
-                if 'determinism_type' in protocol.attributes:  # PFN is cachable
+                if 'determinism_type' in protocol.attributes:  # PFN is cacheable
                     try:
                         path = pfns_cache['%s:%s:%s' % (protocol.attributes['determinism_type'], t_scope.internal, t_name)]
                     except KeyError:  # No cache entry scope:name found for this protocol
                         path = protocol._get_path(t_scope, t_name)
                         pfns_cache['%s:%s:%s' % (protocol.attributes['determinism_type'], t_scope.internal, t_name)] = path
 
                 try:
@@ -1320,15 +1321,15 @@
         ).order_by(
             literal_column('dbms_random.value') if session.bind.dialect.name == 'oracle' else func.random()
         ).limit(
             # slightly overshoot to reduce the probability that python-side filtering will
             # leave us with less than nrandom replicas.
             nrandom * 4
         )
-        # Re-use input temp table. We don't need its content anymore
+        # Reuse input temp table. We don't need its content anymore
         random_dids_temp_table = input_dids_temp_table
         session.execute(delete(random_dids_temp_table))
         session.execute(insert(random_dids_temp_table).from_select(['scope', 'name'], stmt))
 
         # Fetch all replicas for randomly selected dids and apply filters on python side
         stmt = _list_replicas_for_collection_files_stmt(random_dids_temp_table, replicas_subquery)
         stmt = stmt.order_by('scope', 'name')
@@ -1486,15 +1487,15 @@
         condition.append(and_(models.RSEFileAssociation.scope == f['scope'], models.RSEFileAssociation.name == f['name'], models.RSEFileAssociation.rse_id == rse_id))
 
     query = session.query(models.RSEFileAssociation.scope, models.RSEFileAssociation.name, models.RSEFileAssociation.rse_id).\
         with_hint(models.RSEFileAssociation, text="INDEX(REPLICAS REPLICAS_PK)", dialect_name='oracle').\
         filter(or_(*condition))
     available_replicas = [dict([(column, getattr(row, column)) for column in row._fields]) for row in query]
 
-    default_tombstone_delay = get_rse_attribute(rse_id, 'tombstone_delay', session=session)
+    default_tombstone_delay = get_rse_attribute(rse_id, RseAttr.TOMBSTONE_DELAY, session=session)
     default_tombstone = tombstone_from_delay(default_tombstone_delay)
 
     new_replicas = []
     for file in files:
         found = False
         for available_replica in available_replicas:
             if file['scope'] == available_replica['scope'] and file['name'] == available_replica['name'] and rse_id == available_replica['rse_id']:
@@ -2465,15 +2466,15 @@
                 query = query.filter(or_(*rse_clause))
     return query.with_for_update(nowait=nowait).all()
 
 
 @transactional_session
 def get_source_replicas(scope, name, source_rses=None, *, session: "Session"):
     """
-    Get soruce replicas for a specific scope:name.
+    Get source replicas for a specific scope:name.
 
     :param scope:          The scope of the did.
     :param name:           The name of the did.
     :param soruce_rses:    Possible RSE_ids to filter on.
     :param session:        The db session in use.
     :returns:              List of SQLAlchemy Replica Objects
     """
@@ -3431,15 +3432,15 @@
     Gets a list of replicas from bad_replicas table which are: declared more than <nattempts> times since <younger_than> date,
     present on the RSE specified by the <rse_expression> and do not have a state in <exclude_states> list.
     Selected replicas can also be required to be <available_elsewhere> on another RSE than the one declared in bad_replicas table and/or
     be declared as <is_suspicious> in the bad_replicas table.
     Keyword Arguments:
     :param younger_than: Datetime object to select the replicas which were declared since younger_than date. Default value = 10 days ago.
     :param nattempts: The minimum number of replica appearances in the bad_replica DB table from younger_than date. Default value = 0.
-    :param nattempts_exact: If True, then only replicas with exactly 'nattempts' appearences in the bad_replica DB table are retrieved. Replicas with more appearences are ignored.
+    :param nattempts_exact: If True, then only replicas with exactly 'nattempts' appearances in the bad_replica DB table are retrieved. Replicas with more appearances are ignored.
     :param rse_expression: The RSE expression where the replicas are located.
     :param filter_: Dictionary of attributes by which the RSE results should be filtered. e.g.: {'availability_write': True}
     :param exclude_states: List of states which eliminates replicas from search result if any of the states in the list
                             was declared for a replica since younger_than date. Allowed values
                             = ['B', 'R', 'D', 'L', 'T', 'S'] (meaning 'BAD', 'RECOVERED', 'DELETED', 'LOST', 'TEMPORARY_UNAVAILABLE', 'SUSPICIOUS').
     :param available_elsewhere: Default: SuspiciousAvailability["ALL"].value, all suspicious replicas are returned.
                                  If SuspiciousAvailability["EXIST_COPIES"].value, only replicas that additionally have copies declared as AVAILABLE on at least one other RSE
@@ -3520,15 +3521,15 @@
                                                        models.BadReplicas.rse_id == bad_replicas_alias.rse_id,
                                                        models.BadReplicas.state.in_(exclude_states_clause))))
     query = query.filter(not_(other_states_present))
 
     # finally, the results are grouped by RSE, scope, name and required to have
     # at least 'nattempts' occurrences in the result of the query per replica.
     # If nattempts_exact, then only replicas are required to have exactly
-    # 'nattempts' occurences.
+    # 'nattempts' occurrences.
     if nattempts_exact:
         query_result = query.group_by(models.RSEFileAssociation.rse_id, bad_replicas_alias.scope, bad_replicas_alias.name).having(func.count() == nattempts).all()
     else:
         query_result = query.group_by(models.RSEFileAssociation.rse_id, bad_replicas_alias.scope, bad_replicas_alias.name).having(func.count() > nattempts).all()
 
     # translating the rse_id to RSE name and assembling the return list of dictionaries
     result = []
```

### Comparing `rucio-34.2.0/lib/rucio/core/replica_sorter.py` & `rucio-34.3.0/lib/rucio/core/replica_sorter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/core/request.py` & `rucio-34.3.0/lib/rucio/core/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from sqlalchemy import and_, delete, exists, insert, or_, select, update
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.orm import aliased
 from sqlalchemy.sql.expression import asc, false, func, null, true
 from sqlalchemy.sql.functions import coalesce
 
 from rucio.common.config import config_get_bool, config_get_int
+from rucio.common.constants import RseAttr
 from rucio.common.exception import InvalidRSEExpression, RequestNotFound, RucioException, UnsupportedOperation
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.common.utils import chunks, generate_uuid
 from rucio.core.distance import get_distances
 from rucio.core.message import add_message, add_messages
 from rucio.core.monitor import MetricManager
 from rucio.core.rse import RseCollection, RseData, get_rse_attribute, get_rse_name, get_rse_vo
@@ -617,15 +618,15 @@
             request = RequestWithSources(id_=request_id, request_type=req_type, rule_id=rule_id, scope=scope, name=name,
                                          md5=md5, adler32=adler32, byte_count=byte_count, activity=activity, attributes=attributes,
                                          previous_attempt_id=previous_attempt_id, dest_rse=rse_collection[dest_rse_id],
                                          account=account, retry_count=retry_count, priority=priority, transfertool=transfertool,
                                          requested_at=requested_at)
             requests_by_id[request_id] = request
             # if STAGEIN and destination RSE is QoS make sure the source is included
-            if request.request_type == RequestType.STAGEIN and get_rse_attribute(rse_id=dest_rse_id, key='staging_required', session=session):
+            if request.request_type == RequestType.STAGEIN and get_rse_attribute(rse_id=dest_rse_id, key=RseAttr.STAGING_REQUIRED, session=session):
                 source = RequestSource(rse=rse_collection[dest_rse_id])
                 request.sources.append(source)
 
         if replica_rse_id is not None:
             replica_rse = rse_collection[replica_rse_id]
             replica_rse.name = replica_rse_name
             source = RequestSource(rse=replica_rse, file_path=file_path,
@@ -1288,15 +1289,15 @@
             models.Request.scope == scope,
             models.Request.name == name,
             models.Request.dest_rse_id == dest_rse_id,
             models.Request.request_type == request_type
         )
         reqs = session.execute(stmt).all()
         if not reqs:
-            logger(logging.WARNING, 'Tried to cancel non-existant request for DID %s:%s at RSE %s' % (scope, name, get_rse_name(rse_id=dest_rse_id, session=session)))
+            logger(logging.WARNING, 'Tried to cancel non-existent request for DID %s:%s at RSE %s' % (scope, name, get_rse_name(rse_id=dest_rse_id, session=session)))
     except IntegrityError as error:
         raise RucioException(error.args)
 
     transfers_to_cancel = {}
     for req in reqs:
         # is there a transfer already in transfertool? if so, schedule to cancel them
         if req[1] is not None:
@@ -2050,15 +2051,15 @@
         session: "Session"
 ):
     """
     Release waiting requests if they fit in available transfer volume. If the DID of a request is attached to a dataset, the volume will be checked for the whole dataset as all requests related to this dataset will be released.
 
     :param dest_rse_id: The destination RSE id.
     :param source_rse_id: The source RSE id
-    :param volume: The maximum volume in bytes that should be transfered.
+    :param volume: The maximum volume in bytes that should be transferred.
     :param session: The database session.
     """
 
     dialect = session.bind.dialect.name
     if dialect == 'mysql' or dialect == 'sqlite':
         coalesce_func = func.ifnull
     elif dialect == 'oracle':
@@ -2132,15 +2133,15 @@
     if dialect == 'mysql' or dialect == 'sqlite':
         coalesce_func = func.ifnull
     elif dialect == 'oracle':
         coalesce_func = func.nvl
     else:  # dialect == 'postgresql'
         coalesce_func = func.coalesce
 
-    # query DIDs that are attached to a collection and add a column indicating the order of attachment in case of mulitple attachments
+    # query DIDs that are attached to a collection and add a column indicating the order of attachment in case of multiple attachments
     attachment_order_subquery = select(
         models.DataIdentifierAssociation.child_name,
         models.DataIdentifierAssociation.child_scope,
         models.DataIdentifierAssociation.name,
         models.DataIdentifierAssociation.scope,
         func.row_number().over(
             partition_by=(models.DataIdentifierAssociation.child_name,
@@ -2275,21 +2276,21 @@
         deadline: int = 1,
         volume: int = 0,
         *,
         session: "Session"
 ):
     """
     Release waiting requests. Transfer requests that were requested first, get released first (FIFO).
-    Also all requests to DIDs that are attached to the same dataset get released, if one children of the dataset is choosed to be released (Grouped FIFO).
+    Also all requests to DIDs that are attached to the same dataset get released, if one children of the dataset is chosen to be released (Grouped FIFO).
 
     :param dest_rse_id: The destination rse id
     :param source_rse_id: The source RSE id.
     :param count: The count to be released. If None, release all waiting requests.
     :param deadline: Maximal waiting time in hours until a dataset gets released.
-    :param volume: The maximum volume in bytes that should be transfered.
+    :param volume: The maximum volume in bytes that should be transferred.
     :param session: The database session.
     """
 
     amount_updated_requests = 0
 
     # Release requests that exceeded waiting time
     if deadline and source_rse_id is not None:
```

### Comparing `rucio-34.2.0/lib/rucio/core/rse.py` & `rucio-34.3.0/lib/rucio/core/rse.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from sqlalchemy.orm import aliased
 from sqlalchemy.orm.exc import FlushError
 from sqlalchemy.sql.expression import and_, delete, desc, false, func, or_, select, true
 
 from rucio.common import exception, types, utils
 from rucio.common.cache import make_region_memcached
 from rucio.common.config import get_lfn2pfn_algorithm_default
+from rucio.common.constants import RseAttr
 from rucio.common.utils import CHECKSUM_KEY, GLOBALLY_SUPPORTED_CHECKSUMS, Availability
 from rucio.core.rse_counter import add_counter, get_counter
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import ReplicaState, RSEType
 from rucio.db.sqla.session import read_session, stream_session, transactional_session
 from rucio.db.sqla.util import temp_table_mngr
 
@@ -115,20 +116,20 @@
 
     def __eq__(self, other):
         if other is None:
             return False
         return self.id == other.id
 
     def is_tape(self):
-        if self.info['rse_type'] == RSEType.TAPE or self.info['rse_type'] == 'TAPE' or self.attributes.get('staging_required', False):
+        if self.info['rse_type'] == RSEType.TAPE or self.info['rse_type'] == 'TAPE' or self.attributes.get(RseAttr.STAGING_REQUIRED, False):
             return True
         return False
 
     def is_tape_or_staging_required(self):
-        if self.is_tape() or self.attributes.get('staging_required', False):
+        if self.is_tape() or self.attributes.get(RseAttr.STAGING_REQUIRED, False):
             return True
         return False
 
     @read_session
     def ensure_loaded(self, load_name=False, load_columns=False, load_attributes=False,
                       load_info=False, load_usage=False, load_limits=False, load_transfer_limits=False, *, session: "Session"):
         if self._columns is None and load_columns:
@@ -199,15 +200,15 @@
         temp_table = temp_table_mngr(session).create_id_table()
         session.bulk_insert_mappings(temp_table, ({'id': rse_id} for rse_id in rse_ids_to_load))
 
         # We need to ensure that all rses exist and are not deleted. We could check this with a specialized
         # query, but this seems wasteful under normal operation: the caller of the current function probably
         # got the list of RSE IDs from list_rses (or another source which checks for deleted rses).
         #
-        # Instead, directly fetch all RSEs, which allows to reduce the number (and complexity) of other queries bellow
+        # Instead, directly fetch all RSEs, which allows to reduce the number (and complexity) of other queries below
         stmt = select(
             models.RSE
         ).join_from(
             temp_table,
             models.RSE,
             models.RSE.id == temp_table.id
         )
@@ -1384,33 +1385,33 @@
         db_protocols: Iterable[models.RSEProtocols],
         rse_attributes: Optional[dict[str, Any]] = None,
         *,
         session: "Session"
 ) -> types.RSESettingsDict:
     _rse = rse
     if rse_attributes:
-        lfn2pfn_algorithm = rse_attributes.get('lfn2pfn_algorithm')
+        lfn2pfn_algorithm = rse_attributes.get(RseAttr.LFN2PFN_ALGORITHM)
     else:
-        lfn2pfn_algorithm = get_rse_attribute(_rse['id'], 'lfn2pfn_algorithm', session=session)
+        lfn2pfn_algorithm = get_rse_attribute(_rse['id'], RseAttr.LFN2PFN_ALGORITHM, session=session)
     # Resolve LFN2PFN default algorithm as soon as possible.  This way, we can send back the actual
     # algorithm name in response to REST queries.
     if not lfn2pfn_algorithm:
         lfn2pfn_algorithm = get_lfn2pfn_algorithm_default()
 
     # Copy verify_checksum from the attributes, later: assume True if not specified
     if rse_attributes:
-        verify_checksum = rse_attributes.get('verify_checksum')
+        verify_checksum = rse_attributes.get(RseAttr.VERIFY_CHECKSUM)
     else:
-        verify_checksum = get_rse_attribute(_rse['id'], 'verify_checksum', session=session)
+        verify_checksum = get_rse_attribute(_rse['id'], RseAttr.VERIFY_CHECKSUM, session=session)
 
     # Copy sign_url from the attributes
     if rse_attributes:
-        sign_url = rse_attributes.get('sign_url')
+        sign_url = rse_attributes.get(RseAttr.SIGN_URL)
     else:
-        sign_url = get_rse_attribute(_rse['id'], 'sign_url', session=session)
+        sign_url = get_rse_attribute(_rse['id'], RseAttr.SIGN_URL, session=session)
 
     info = {'availability_delete': _rse['availability_delete'],
             'availability_read': _rse['availability_read'],
             'availability_write': _rse['availability_write'],
             'credentials': None,
             'deterministic': _rse['deterministic'],
             'domain': utils.rse_supported_protocol_domains(),
@@ -1874,12 +1875,12 @@
         if protocol['scheme'] != 'davs':
             continue
         # Remove base path from prefix.  Storages typically map an issuer (i.e.
         # a VO) to a particular area.  If so, then the path to that area acts as
         # a base which should be removed from the prefix (in order for '/' to
         # mean the entire resource associated with that issuer).
         prefix = protocol['prefix']
-        if base_path := get_rse_attribute(rse_id, 'oidc_base_path'):
+        if base_path := get_rse_attribute(rse_id, RseAttr.OIDC_BASE_PATH):
             prefix = prefix.removeprefix(base_path)
         filtered_prefixes.add(prefix)
     all_scopes = [f'{s}:{p}' for s in scopes for p in filtered_prefixes] + list(extra_scopes)
     return ' '.join(sorted(all_scopes))
```

### Comparing `rucio-34.2.0/lib/rucio/core/rse_counter.py` & `rucio-34.3.0/lib/rucio/core/rse_counter.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import TYPE_CHECKING
 
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.exc import NoResultFound
 
 from rucio.common.exception import CounterNotFound
 from rucio.db.sqla import filter_thread_work, models
 from rucio.db.sqla.session import read_session, transactional_session
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
```

### Comparing `rucio-34.2.0/lib/rucio/core/rse_expression_parser.py` & `rucio-34.3.0/lib/rucio/core/rse_expression_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,17 @@
         parantheses_close_count = 0
         for char in expression:
             if (char == '('):
                 parantheses_open_count += 1
             elif (char == ')'):
                 parantheses_close_count += 1
             if (parantheses_close_count > parantheses_open_count):
-                raise InvalidRSEExpression('Problem with parantheses.')
+                raise InvalidRSEExpression('Problem with parentheses.')
         if (parantheses_open_count != parantheses_close_count):
-            raise InvalidRSEExpression('Problem with parantheses.')
+            raise InvalidRSEExpression('Problem with parentheses.')
 
         # Check the expression pattern
         match = re.match(PATTERN, expression)
         if match is None:
             raise InvalidRSEExpression('Expression does not comply to RSE Expression syntax')
         else:
             if match.group() != expression:
@@ -165,15 +165,15 @@
                 continue
 
 
 def __resolve_primitive_expression(expression):
     """
     Resolve a primitive expression and return a RSEAttribute object
 
-    :param expression:    String of the expresssion
+    :param expression:    String of the expression
     :returns:             Tuple of RSEAttribute, primitive expression
     """
     primitiveexpression = re.match(PRIMITIVE, expression).group()
     if ('=' in primitiveexpression):
         keyvalue = primitiveexpression.split("=")
         return (RSEAttributeEqualCheck(keyvalue[0], keyvalue[1]), primitiveexpression)
     elif ('<' in primitiveexpression):
@@ -186,15 +186,15 @@
         return (RSEAll(), primitiveexpression)
     else:
         return (RSEAttributeEqualCheck(key=primitiveexpression), primitiveexpression)
 
 
 def __extract_term(expression):
     """
-    Extract a term from an expression with parantheses
+    Extract a term from an expression with parentheses
 
     :param expression:  The expression starting with a '('
     :return:            The extracted term string
     """
     open_parantheses = 0
     i = 0
     for char in expression:
```

### Comparing `rucio-34.2.0/lib/rucio/core/rse_selector.py` & `rucio-34.3.0/lib/rucio/core/rse_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                             rse['space_left'] = float('inf')
                         else:
                             rse['space_left'] = space_limit - get_rse_counter(rse_id=rse['rse_id'], session=session)['bytes']
                         rses_with_enough_quota.append(rse)
 
         self.rses = rses_with_enough_quota
         if len(self.rses) < self.copies:
-            raise InsufficientAccountLimit('There is insufficient quota on any of the target RSE\'s to fullfill the operation.')
+            raise InsufficientAccountLimit('There is insufficient quota on any of the target RSE\'s to fulfill the operation.')
 
         # don't consider removing rses based on the total space here - because files already on the RSE are taken into account
         # it is possible to have no space but still be able to fulfil the rule
 
     def select_rse(self, size, preferred_rse_ids, copies=0, blocklist=[], prioritize_order_over_weight=False, existing_rse_size=None):
         """
         Select n RSEs to replicate data to.
@@ -158,42 +158,42 @@
             raise InsufficientTargetRSEs('There are not enough target RSEs to fulfil the request at this time.')
 
         # Remove rses which do not have enough space, accounting for the files already at each rse
         if existing_rse_size is None:
             existing_rse_size = {}
         rses = [rse for rse in rses if rse['space_left'] >= size - existing_rse_size.get(rse['rse_id'], 0)]
         if len(rses) < count:
-            raise RSEOverQuota('There is insufficient space on any of the target RSE\'s to fullfill the operation.')
+            raise RSEOverQuota('There is insufficient space on any of the target RSE\'s to fulfill the operation.')
 
         # Remove rses which do not have enough local quota
         rses = [rse for rse in rses if rse['quota_left'] > size]
         if len(rses) < count:
-            raise InsufficientAccountLimit('There is insufficient quota on any of the target RSE\'s to fullfill the operation.')
+            raise InsufficientAccountLimit('There is insufficient quota on any of the target RSE\'s to fulfill the operation.')
 
         # Remove rses which do not have enough global quota
         rses_with_enough_quota = []
         for rse in rses:
             enough_global_quota = True
             for rse_expression in rse.get('global_quota_left', []):
                 if rse['global_quota_left'][rse_expression] < size:
                     enough_global_quota = False
                     break
             if enough_global_quota:
                 rses_with_enough_quota.append(rse)
         rses = rses_with_enough_quota
         if len(rses) < count:
-            raise InsufficientAccountLimit('There is insufficient quota on any of the target RSE\'s to fullfill the operation.')
+            raise InsufficientAccountLimit('There is insufficient quota on any of the target RSE\'s to fulfill the operation.')
 
         for copy in range(count):
             # Remove rses already in the result set
             rses = [rse for rse in rses if rse['rse_id'] not in [item[0] for item in result]]
             rses_dict = {}
             for rse in rses:
                 rses_dict[rse['rse_id']] = rse
-            # Prioritize the preffered rses
+            # Prioritize the preferred rses
             preferred_rses = [rses_dict[rse_id] for rse_id in preferred_rse_ids if rse_id in rses_dict]
             if prioritize_order_over_weight and preferred_rses:
                 rse = (preferred_rses[0]['rse_id'], preferred_rses[0]['staging_area'], preferred_rses[0]['availability_write'])
             elif preferred_rses:
                 rse = self.__choose_rse(preferred_rses)
             else:
                 rse = self.__choose_rse(rses)
@@ -213,15 +213,15 @@
         return rse_dict
 
     def __update_quota(self, rse, size):
         """
         Update the internal quota value.
 
         :param rse:      RSE tuple to update.
-        :param size:     Size to substract.
+        :param size:     Size to subtract.
         """
 
         for element in self.rses:
             if element['rse_id'] == rse[0]:
                 element['quota_left'] -= size
                 for rse_expression in element.get('global_quota_left', []):
                     element['global_quota_left'][rse_expression] -= size
```

### Comparing `rucio-34.2.0/lib/rucio/core/rule.py` & `rucio-34.3.0/lib/rucio/core/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import logging
-from collections.abc import Iterator, Sequence
+from collections.abc import Callable, Iterator, Sequence
 from configparser import NoOptionError, NoSectionError
 from copy import deepcopy
 from datetime import datetime, timedelta
 from os import path
 from re import match
 from string import Template
-from typing import TYPE_CHECKING, Any, Callable, Literal, Optional, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Literal, Optional, TypeVar, Union
 
 from dogpile.cache.api import NoValue
 from sqlalchemy import delete, desc, select, update
 from sqlalchemy.exc import (
     IntegrityError,
     NoResultFound,  # https://pydoc.dev/sqlalchemy/latest/sqlalchemy.exc.NoResultFound.html
     StatementError,
@@ -34,14 +34,15 @@
 from sqlalchemy.sql.expression import and_, false, null, or_, true, tuple_
 
 import rucio.core.did
 import rucio.core.lock  # import get_replica_locks, get_files_and_replica_locks_of_dataset
 import rucio.core.replica  # import get_and_lock_file_replicas, get_and_lock_file_replicas_for_dataset
 from rucio.common.cache import make_region_memcached
 from rucio.common.config import config_get
+from rucio.common.constants import RseAttr
 from rucio.common.exception import (
     DataIdentifierNotFound,
     DuplicateRule,
     InputValidationError,
     InsufficientAccountLimit,
     InsufficientTargetRSEs,
     InvalidObject,
@@ -108,27 +109,27 @@
     def evaluate(self) -> bool:
         """
         Evaluate the auto-approve algorithm
         """
         return self.get_configured_algorithm()(self.rule, self.did, self.session)
 
     @classmethod
-    def get_configured_algorithm(cls: Type[AutoApproveT]) -> Callable[[models.ReplicationRule, models.DataIdentifier, 'Session'], bool]:
+    def get_configured_algorithm(cls: type[AutoApproveT]) -> Callable[[models.ReplicationRule, models.DataIdentifier, 'Session'], bool]:
         """
         Get the configured auto-approve algorithm
         """
         try:
             configured_algorithm: str = str(config_get('rules', cls._algorithm_type, default='default'))
         except (NoOptionError, NoSectionError, RuntimeError):
             configured_algorithm = 'default'
 
         return super()._get_one_algorithm(cls._algorithm_type, configured_algorithm)
 
     @classmethod
-    def register(cls: Type[AutoApproveT], name: str, fn_auto_approve: Callable[[models.ReplicationRule, models.DataIdentifier, 'Session'], bool]) -> None:
+    def register(cls: type[AutoApproveT], name: str, fn_auto_approve: Callable[[models.ReplicationRule, models.DataIdentifier, 'Session'], bool]) -> None:
         """
         Register a new auto-approve algorithm
         """
         algorithm_dict = {name: fn_auto_approve}
         super()._register(cls._algorithm_type, algorithm_dict)
 
     @staticmethod
@@ -145,20 +146,20 @@
         # Block manual approval for multi-rse rules
         if len(rses) > 1:
             raise InvalidReplicationRule('Ask approval is not allowed for rules with multiple RSEs')
         if len(rses) == 1 and not did.is_open and did.bytes is not None and did.length is not None:
             # This rule can be considered for auto-approval:
             rse_attr = list_rse_attributes(rse_id=rses[0]['id'], session=session)
             auto_approve = False
-            if 'auto_approve_bytes' in rse_attr and 'auto_approve_files' in rse_attr:
-                if did.bytes < int(rse_attr.get('auto_approve_bytes')) and did.length < int(rse_attr.get('auto_approve_files')):
+            if RseAttr.AUTO_APPROVE_BYTES in rse_attr and RseAttr.AUTO_APPROVE_FILES in rse_attr:
+                if did.bytes < int(rse_attr.get(RseAttr.AUTO_APPROVE_BYTES)) and did.length < int(rse_attr.get(RseAttr.AUTO_APPROVE_FILES)):
                     auto_approve = True
-            elif did.bytes < int(rse_attr.get('auto_approve_bytes', -1)):
+            elif did.bytes < int(rse_attr.get(RseAttr.AUTO_APPROVE_BYTES, -1)):
                 auto_approve = True
-            elif did.length < int(rse_attr.get('auto_approve_files', -1)):
+            elif did.length < int(rse_attr.get(RseAttr.AUTO_APPROVE_FILES, -1)):
                 auto_approve = True
 
         return auto_approve
 
 
 @transactional_session
 def add_rule(
@@ -251,15 +252,15 @@
             if not locked and lifetime is None:
                 if [rse for rse in rses if rse.get('rse_type', RSEType.DISK) == RSEType.TAPE]:
                     locked = True
 
             # Block manual approval if RSE does not allow it
             if ask_approval:
                 for rse in rses:
-                    if list_rse_attributes(rse_id=rse['id'], session=session).get('block_manual_approval', False):
+                    if list_rse_attributes(rse_id=rse['id'], session=session).get(RseAttr.BLOCK_MANUAL_APPROVAL, False):
                         raise ManualRuleApprovalBlocked()
 
             if source_replica_expression:
                 try:
                     source_rses = parse_expression(source_replica_expression, filter_={'vo': vo}, session=session)
                 except InvalidRSEExpression as exc:
                     raise InvalidSourceReplicaExpression from exc
@@ -619,15 +620,15 @@
                     if not rule.get('locked', False) and rule.get('lifetime', None) is None:
                         if [rse for rse in rses if rse.get('rse_type', RSEType.DISK) == RSEType.TAPE]:
                             rule['locked'] = True
 
                     # Block manual approval if RSE does not allow it
                     if rule.get('ask_approval', False):
                         for rse in rses:
-                            if list_rse_attributes(rse_id=rse['id'], session=session).get('block_manual_approval', False):
+                            if list_rse_attributes(rse_id=rse['id'], session=session).get(RseAttr.BLOCK_MANUAL_APPROVAL, False):
                                 raise ManualRuleApprovalBlocked()
 
                     if rule.get('source_replica_expression'):
                         source_rses = parse_expression(rule.get('source_replica_expression'), filter_={'vo': vo}, session=session)
                     else:
                         source_rses = []
 
@@ -689,20 +690,20 @@
                         # Block manual approval for multi-rse rules
                         if len(rses) > 1:
                             raise InvalidReplicationRule('Ask approval is not allowed for rules with multiple RSEs')
                         if len(rses) == 1 and not did.is_open and did.bytes is not None and did.length is not None:
                             # This rule can be considered for auto-approval:
                             rse_attr = list_rse_attributes(rse_id=rses[0]['id'], session=session)
                             auto_approve = False
-                            if 'auto_approve_bytes' in rse_attr and 'auto_approve_files' in rse_attr:
-                                if did.bytes < int(rse_attr.get('auto_approve_bytes')) and did.length < int(rse_attr.get('auto_approve_bytes')):
+                            if RseAttr.AUTO_APPROVE_BYTES in rse_attr and RseAttr.AUTO_APPROVE_FILES in rse_attr:
+                                if did.bytes < int(rse_attr.get(RseAttr.AUTO_APPROVE_BYTES)) and did.length < int(rse_attr.get(RseAttr.AUTO_APPROVE_BYTES)):
                                     auto_approve = True
-                            elif did.bytes < int(rse_attr.get('auto_approve_bytes', -1)):
+                            elif did.bytes < int(rse_attr.get(RseAttr.AUTO_APPROVE_BYTES, -1)):
                                 auto_approve = True
-                            elif did.length < int(rse_attr.get('auto_approve_files', -1)):
+                            elif did.length < int(rse_attr.get(RseAttr.AUTO_APPROVE_FILES, -1)):
                                 auto_approve = True
                             if auto_approve:
                                 logger(logging.DEBUG, "Auto approving rule %s", str(new_rule.id))
                                 logger(logging.DEBUG, "Created rule %s for injection", str(new_rule.id))
                                 approve_rule(rule_id=new_rule.id, notify_approvers=False, session=session)
                                 continue
                         logger(logging.DEBUG, "Created rule %s in waiting for approval", str(new_rule.id))
@@ -1098,15 +1099,15 @@
     List replication rules a file is affected from.
 
     :param scope:   Scope of the file.
     :param name:    Name of the file.
     :param session: The database session in use.
     :raises:        RucioException
     """
-    rucio.core.did.get_did(scope=scope, name=name, session=session)  # Check if the did acually exists
+    rucio.core.did.get_did(scope=scope, name=name, session=session)  # Check if the did actually exists
     stmt = select(
         models.ReplicationRule,
         models.DataIdentifier.bytes
     ).distinct(
     ).join(
         models.ReplicaLock,
         models.ReplicationRule.id == models.ReplicaLock.rule_id
@@ -1249,16 +1250,16 @@
 
     :param rule_id:   The rule to repair.
     :param session:   The database session in use.
     :param logger:    Optional decorated logger that can be passed from the calling daemons or servers.
     """
 
     # Rule error cases:
-    # (A) A rule get's an exception on rule-creation. This can only be the MissingSourceReplica exception.
-    # (B) A rule get's an error when re-evaluated: InvalidRSEExpression, InvalidRuleWeight, InsufficientTargetRSEs, RSEWriteBlocked
+    # (A) A rule gets an exception on rule-creation. This can only be the MissingSourceReplica exception.
+    # (B) A rule gets an error when re-evaluated: InvalidRSEExpression, InvalidRuleWeight, InsufficientTargetRSEs, RSEWriteBlocked
     #     InsufficientAccountLimit. The re-evaluation has to be done again and potential missing locks have to be
     #     created.
     # (C) Transfers fail and mark locks (and the rule) as STUCK. All STUCK locks have to be repaired.
     # (D) Files are declared as BAD.
 
     # start_time = time.time()
     try:
@@ -2742,15 +2743,15 @@
 
                                 add_message(event_type='DATASETLOCK_OK', payload=payload, session=session)
 
                     except DataIdentifierNotFound:
                         pass
 
     elif rule.state == RuleState.REPLICATING and rule.notification == RuleNotification.PROGRESS and replicating_locks_before:
-        # For RuleNotification PROGRESS rules, also notifiy when REPLICATING thresholds are passed
+        # For RuleNotification PROGRESS rules, also notify when REPLICATING thresholds are passed
         if __progress_class(replicating_locks_before, total_locks) != __progress_class(rule.locks_replicating_cnt, total_locks):
             try:
                 did = rucio.core.did.get_did(scope=rule.scope, name=rule.name, session=session)
                 if not did['open']:
                     payload = {'scope': rule.scope.external,
                                'name': rule.name,
                                'rule_id': rule.id,
@@ -2812,15 +2813,15 @@
         except ValueError as ex:
             logger(logging.ERROR, "Invalid mail template.", exc_info=ex)
             return
 
         add_message(event_type='email',
                     payload={'body': email_body,
                              'to': [email],
-                             'subject': '[RUCIO] Replication rule %s has been succesfully transferred' % (str(rule.id))},
+                             'subject': '[RUCIO] Replication rule %s has been successfully transferred' % (str(rule.id))},
                     session=session)
 
 
 @transactional_session
 def insert_rule_history(
     rule: models.ReplicationRule,
     recent: bool = True,
@@ -3004,15 +3005,15 @@
     session: "Session"
 ) -> dict[str, Any]:
     """
     Examine a replication rule for transfer errors.
 
     :param rule_id:            Replication rule id
     :param session:            Session of the db.
-    :returns:                  Dictionary of informations
+    :returns:                  Dictionary of information
     """
     result = {'rule_error': None,
               'transfers': []}
 
     try:
         stmt = select(
             models.ReplicationRule
@@ -3226,15 +3227,15 @@
 
     :param datasetfiles:       Sequence of dicts holding all datasets and files.
     :param locks:              Dict holding locks.
     :param replicas:           Dict holding replicas.
     :param source_replicas:    Dict holding source replicas.
     :param rseselector:        The RSESelector to be used.
     :param rule:               The rule.
-    :param source_rses:        RSE ids for eglible source RSEs.
+    :param source_rses:        RSE ids for eligible source RSEs.
     :param session:            Session of the db.
     :param logger:             Optional decorated logger that can be passed from the calling daemons or servers.
     :raises:                   InsufficientAccountLimit, IntegrityError, InsufficientTargetRSEs
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
 
     logger(logging.DEBUG, "Finding missing locks for rule %s [%d/%d/%d]", str(rule.id), rule.locks_ok_cnt, rule.locks_replicating_cnt, rule.locks_stuck_cnt)
@@ -3335,15 +3336,15 @@
 
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding locks.
     :param replicas:           Dict holding replicas.
     :param source_replicas:    Dict holding source replicas.
     :param rseselector:        The RSESelector to be used.
     :param rule:               The rule.
-    :param source_rses:        RSE ids of eglible source RSEs.
+    :param source_rses:        RSE ids of eligible source RSEs.
     :param session:            Session of the db.
     :param logger:             Optional decorated logger that can be passed from the calling daemons or servers.
     :raises:                   InsufficientAccountLimit, IntegrityError, InsufficientTargetRSEs
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
 
     logger(logging.DEBUG, "Finding and repairing stuck locks for rule %s [%d/%d/%d]", str(rule.id), rule.locks_ok_cnt, rule.locks_replicating_cnt, rule.locks_stuck_cnt)
@@ -3551,15 +3552,15 @@
 def __evaluate_did_attach(
     eval_did: models.DataIdentifier,
     *,
     session: "Session",
     logger: LoggerFunction = logging.log
 ) -> None:
     """
-    Evaluate a parent did which has new childs
+    Evaluate a parent did which has new children
 
     :param eval_did:  The did object in use.
     :param session:   The database session in use.
     :param logger:    Optional decorated logger that can be passed from the calling daemons or servers.
     :raises:          ReplicationRuleCreationTemporaryFailed
     """
 
@@ -3803,15 +3804,15 @@
     *,
     session: "Session"
 ) -> tuple[list[dict[str, Any]],
            dict[tuple[str, str], models.ReplicaLock],
            dict[tuple[str, str], models.RSEFileAssociation],
            dict[tuple[str, str], str]]:
     """
-    Resolves a did to its constituent childs and reads the locks and replicas of all the constituent files.
+    Resolves a did to its constituent children and reads the locks and replicas of all the constituent files.
 
     :param did:            The db object of the did the rule is applied on.
     :param nowait:         Nowait parameter for the FOR UPDATE statement.
     :param restrict_rses:  Possible rses of the rule, so only these replica/locks should be considered.
     :param source_rses:    Source rses for this rule. These replicas are not row-locked.
     :param only_stuck:     Get results only for STUCK locks, if True.
     :param session:        Session of the db.
@@ -3910,15 +3911,15 @@
     *,
     session: "Session"
 ) -> tuple[list[dict[str, Any]],
            dict[tuple[str, str], models.ReplicaLock],
            dict[tuple[str, str], models.RSEFileAssociation],
            dict[tuple[str, str], str]]:
     """
-    Resolves a list of dids to its constituent childs and reads the locks and replicas of all the constituent files.
+    Resolves a list of dids to its constituent children and reads the locks and replicas of all the constituent files.
 
     :param dids:           The list of DataIdentifierAssociation objects.
     :param nowait:         Nowait parameter for the FOR UPDATE statement.
     :param restrict_rses:  Possible rses of the rule, so only these replica/locks should be considered.
     :param source_rses:    Source rses for this rule. These replicas are not row-locked.
     :param session:        Session of the db.
     :returns:              (datasetfiles, locks, replicas, source_replicas)
@@ -4090,15 +4091,15 @@
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding locks.
     :param replicas:           Dict holding replicas.
     :param source_replicas:    Dict holding source replicas.
     :param rseselector:        The RSESelector to be used.
     :param rule:               The rule.
     :param preferred_rse_ids:  Preferred RSE's to select.
-    :param source_rses:        RSE ids of eglible source replicas.
+    :param source_rses:        RSE ids of eligible source replicas.
     :param session:            Session of the db.
     :param logger:             Optional decorated logger that can be passed from the calling daemons or servers.
     :raises:                   InsufficientAccountLimit, IntegrityError, InsufficientTargetRSEs, RSEOverQuota
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
 
     logger(logging.DEBUG, "Creating locks and replicas for rule %s [%d/%d/%d]", str(rule.id), rule.locks_ok_cnt, rule.locks_replicating_cnt, rule.locks_stuck_cnt)
@@ -4293,34 +4294,34 @@
 
     recipients: list[tuple] = []  # (eMail, account)
 
     # APPROVERS-LIST
     # If there are accounts in the approvers-list of any of the RSEs only these should be used
     for rse in parse_expression(rse_expression, filter_=filter_, session=session):
         rse_attr = list_rse_attributes(rse_id=rse['id'], session=session)
-        if rse_attr.get('rule_approvers'):
-            for account in rse_attr.get('rule_approvers').split(','):
+        if rse_attr.get(RseAttr.RULE_APPROVERS):
+            for account in rse_attr.get(RseAttr.RULE_APPROVERS).split(','):
                 account = InternalAccount(account)
                 try:
                     email = get_account(account=account, session=session).email
                     if email:
                         recipients.append((email, account))
                 except Exception:
                     pass
 
     # LOCALGROUPDISK/LOCALGROUPTAPE
     if not recipients:
         for rse in parse_expression(rse_expression, filter_=filter_, session=session):
             rse_attr = list_rse_attributes(rse_id=rse['id'], session=session)
-            if rse_attr.get('type', '') in ('LOCALGROUPDISK', 'LOCALGROUPTAPE'):
+            if rse_attr.get(RseAttr.TYPE, '') in ('LOCALGROUPDISK', 'LOCALGROUPTAPE'):
 
                 query = select(
                     models.AccountAttrAssociation.account
                 ).where(
-                    models.AccountAttrAssociation.key == f'country-{rse_attr.get("country", "")}',
+                    models.AccountAttrAssociation.key == f'country-{rse_attr.get(RseAttr.COUNTRY, "")}',
                     models.AccountAttrAssociation.value == 'admin'
                 )
 
                 for account in session.execute(query).scalars().all():
                     try:
                         email = get_account(account=account, session=session).email
                         if email:
@@ -4328,20 +4329,20 @@
                     except Exception:
                         pass
 
     # GROUPDISK
     if not recipients:
         for rse in parse_expression(rse_expression, filter_=filter_, session=session):
             rse_attr = list_rse_attributes(rse_id=rse['id'], session=session)
-            if rse_attr.get('type', '') == 'GROUPDISK':
+            if rse_attr.get(RseAttr.TYPE, '') == 'GROUPDISK':
 
                 query = select(
                     models.AccountAttrAssociation.account
                 ).where(
-                    models.AccountAttrAssociation.key == f'group-{rse_attr.get("physgroup", "")}',
+                    models.AccountAttrAssociation.key == f'group-{rse_attr.get(RseAttr.PHYSGROUP, "")}',
                     models.AccountAttrAssociation.value == 'admin'
                 )
 
                 for account in session.execute(query).scalars().all():
                     try:
                         email = get_account(account=account, session=session).email
                         if email:
@@ -4466,10 +4467,10 @@
     :param session:  The database session in use.
     """
 
     scratchdisk_lifetime = get_scratchdisk_lifetime()
     # Check SCRATCHDISK Policy
     if not has_account_attribute(account=account, key='admin', session=session) and (lifetime is None or lifetime > 60 * 60 * 24 * scratchdisk_lifetime):
         # Check if one of the rses is a SCRATCHDISK:
-        if [rse for rse in rses if list_rse_attributes(rse_id=rse['id'], session=session).get('type') == 'SCRATCHDISK']:
+        if [rse for rse in rses if list_rse_attributes(rse_id=rse['id'], session=session).get(RseAttr.TYPE) == 'SCRATCHDISK']:
             lifetime = 60 * 60 * 24 * scratchdisk_lifetime - 1
     return lifetime
```

### Comparing `rucio-34.2.0/lib/rucio/core/rule_grouping.py` & `rucio-34.3.0/lib/rucio/core/rule_grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 
 import logging
 from collections.abc import Sequence
 from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
 from sqlalchemy import func
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.exc import NoResultFound
 
 import rucio.core.did
 import rucio.core.lock
 import rucio.core.replica
 from rucio.common.config import config_get_int
+from rucio.common.constants import RseAttr
 from rucio.common.exception import InsufficientTargetRSEs
 from rucio.common.types import InternalScope
 from rucio.core import account_counter, rse_counter
 from rucio.core import request as request_core
 from rucio.core.rse import get_rse, get_rse_attribute, get_rse_name
 from rucio.core.rse_selector import RSESelector
 from rucio.db.sqla import models
@@ -58,15 +59,15 @@
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding all locks.
     :param replicas:           Dict holding all replicas.
     :param source_replicas:    Dict holding all source_replicas.
     :param rseselector:        The RSESelector to be used.
     :param rule:               The rule object.
     :param preferred_rse_ids:  Preferred RSE's to select.
-    :param source_rses:        RSE ids of eglible source replicas.
+    :param source_rses:        RSE ids of eligible source replicas.
     :param session:            Session of the db.
     :returns:                  Dict of replicas to create, Dict of locks to create, List of transfers to create
     :raises:                   InsufficientQuota, InsufficientTargetRSEs, RSEOverQuota
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
 
     # locks_to_create =     {'rse_id': [locks]}
@@ -129,15 +130,15 @@
 
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding all locks.
     :param replicas:           Dict holding all replicas.
     :param source_replicas:    Dict holding all source_replicas.
     :param rseselector:        The RSESelector to be used.
     :param rule:               The rule object.
-    :param source_rses:        RSE ids of eglible source_rses.
+    :param source_rses:        RSE ids of eligible source_rses.
     :param session:            Session of the db.
     :returns:                  List of replicas to create, List of locks to create, List of transfers to create, List of locks to Delete
     :raises:                   InsufficientQuota, InsufficientTargetRSEs
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
 
     # locks_to_create =     {'rse_id': [locks]}
@@ -230,15 +231,15 @@
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding all locks.
     :param replicas:           Dict holding all replicas.
     :param source_replicas:    Dict holding all source_replicas.
     :param rseselector:        The RSESelector to be used.
     :param rule:               The rule object.
     :param preferred_rse_ids:  Preferred RSE's to select.
-    :param source_rses:        RSE ids of eglible source replicas.
+    :param source_rses:        RSE ids of eligible source replicas.
     :param session:            Session of the db.
     :returns:                  replicas_to_create, locks_to_create, transfers_to_create
     :raises:                   InsufficientAccountLimit, InsufficientTargetRSEs
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
     locks_to_create = {}            # {'rse_id': [locks]}
     replicas_to_create = {}         # {'rse_id': [replicas]}
@@ -311,15 +312,15 @@
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding all locks.
     :param replicas:           Dict holding all replicas.
     :param source_replicas:    Dict holding all source_replicas.
     :param rseselector:        The RSESelector to be used.
     :param rule:               The rule object.
     :param preferred_rse_ids:  Preferred RSE's to select.
-    :param source_rses:        RSE ids of eglible source replicas.
+    :param source_rses:        RSE ids of eligible source replicas.
     :param session:            Session of the db.
     :returns:                  replicas_to_create, locks_to_create, transfers_to_create
     :raises:                   InsufficientQuota, InsufficientTargetRSEs
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
 
     locks_to_create = {}            # {'rse_id': [locks]}
@@ -431,15 +432,15 @@
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding all locks.
     :param replicas:           Dict holding all replicas.
     :param source_replicas:    Dict holding all source replicas.
     :param rseselector:        The RSESelector to be used.
     :param rule:               The rule object.
     :param preferred_rse_ids:  Preferred RSE's to select.
-    :param source_rses:        RSE ids of eglible source replicas.
+    :param source_rses:        RSE ids of eligible source replicas.
     :param session:            Session of the db.
     :returns:                  replicas_to_create, locks_to_create, transfers_to_create
     :raises:                   InsufficientQuota, InsufficientTargetRSEs
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
     locks_to_create = {}            # {'rse_id': [locks]}
     replicas_to_create = {}         # {'rse_id': [replicas]}
@@ -548,15 +549,15 @@
 
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding all locks.
     :param replicas:           Dict holding all replicas.
     :param source_replicas:    Dict holding all source_replicas.
     :param rseselector:        The RSESelector to be used.
     :param rule:               The rule object.
-    :param source_rses:        RSE ids of eglible source replicas.
+    :param source_rses:        RSE ids of eligible source replicas.
     :param session:            Session of the db.
     :param logger:             Optional decorated logger that can be passed from the calling daemons or servers.
     :returns:                  replicas_to_create, locks_to_create, transfers_to_create, locks_to_delete
     :raises:                   InsufficientAccountLimit, InsufficientTargetRSEs
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
 
@@ -591,15 +592,15 @@
                     associated_replica = [replica for replica in replicas[(file['scope'], file['name'])] if replica.state in [ReplicaState.AVAILABLE, ReplicaState.TEMPORARY_UNAVAILABLE] and replica.rse_id == lock.rse_id][0]
                     associated_replica.tombstone = None
                     associated_replica.lock_cnt = session.query(func.count(models.ReplicaLock.rule_id)).filter_by(scope=associated_replica.scope, name=associated_replica.name, rse_id=lock.rse_id).one()[0]
                     continue
                 # Check if this is a STUCK lock due to source_replica filtering
                 if source_rses:
                     associated_replica = [replica for replica in replicas[(file['scope'], file['name'])] if replica.rse_id == lock.rse_id][0]
-                    # Check if there is an eglible source replica for this lock
+                    # Check if there is an eligible source replica for this lock
                     if set(source_replicas.get((file['scope'], file['name']), [])).intersection(source_rses) and (selector_rse_dict.get(lock.rse_id, {}).get('availability_write', True) or rule.ignore_availability):
                         __update_lock_replica_and_create_transfer(lock=lock,
                                                                   replica=associated_replica,
                                                                   rule=rule,
                                                                   dataset=dataset,
                                                                   transfers_to_create=transfers_to_create,
                                                                   session=session)
@@ -655,15 +656,15 @@
 
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding all locks.
     :param replicas:           Dict holding all replicas.
     :param source_replicas:    Dict holding all source_replicas.
     :param rseselector:        The RSESelector to be used.
     :param rule:               The rule object.
-    :param source_rses:        RSE ids of eglible source replicas.
+    :param source_rses:        RSE ids of eligible source replicas.
     :param session:            Session of the db.
     :param logger:             Optional decorated logger that can be passed from the calling daemons or servers.
     :returns:                  replicas_to_create, locks_to_create, transfers_to_create, locks_to_delete
     :raises:                   InsufficientAccountLimit, InsufficientTargetRSEs
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
 
@@ -698,15 +699,15 @@
                     associated_replica = [replica for replica in replicas[(file['scope'], file['name'])] if replica.state in [ReplicaState.AVAILABLE, ReplicaState.TEMPORARY_UNAVAILABLE] and replica.rse_id == lock.rse_id][0]
                     associated_replica.tombstone = None
                     associated_replica.lock_cnt = session.query(func.count(models.ReplicaLock.rule_id)).filter_by(scope=associated_replica.scope, name=associated_replica.name, rse_id=lock.rse_id).one()[0]
                     continue
                 # Check if this is a STUCK lock due to source_replica filtering
                 if source_rses:
                     associated_replica = [replica for replica in replicas[(file['scope'], file['name'])] if replica.rse_id == lock.rse_id][0]
-                    # Check if there is an eglible source replica for this lock
+                    # Check if there is an eligible source replica for this lock
                     if set(source_replicas.get((file['scope'], file['name']), [])).intersection(source_rses) and (selector_rse_dict.get(lock.rse_id, {}).get('availability_write', True) or rule.ignore_availability):
                         __update_lock_replica_and_create_transfer(lock=lock,
                                                                   replica=associated_replica,
                                                                   rule=rule,
                                                                   dataset=dataset,
                                                                   transfers_to_create=transfers_to_create,
                                                                   session=session)
@@ -731,15 +732,15 @@
 
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding all locks.
     :param replicas:           Dict holding all replicas.
     :param source_replicas:    Dict holding all source_replicas.
     :param rseselector:        The RSESelector to be used.
     :param rule:               The rule object.
-    :param source_rses:        RSE ids of eglible source replicas.
+    :param source_rses:        RSE ids of eligible source replicas.
     :param session:            Session of the db.
     :param logger:             Optional decorated logger that can be passed from the calling daemons or servers.
     :returns:                  replicas_to_create, locks_to_create, transfers_to_create, locks_to_delete
     :raises:                   InsufficientAccountLimit, InsufficientTargetRSEs
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
 
@@ -774,15 +775,15 @@
                     associated_replica = [replica for replica in replicas[(file['scope'], file['name'])] if replica.state in [ReplicaState.AVAILABLE, ReplicaState.TEMPORARY_UNAVAILABLE] and replica.rse_id == lock.rse_id][0]
                     associated_replica.tombstone = None
                     associated_replica.lock_cnt = session.query(func.count(models.ReplicaLock.rule_id)).filter_by(scope=associated_replica.scope, name=associated_replica.name, rse_id=lock.rse_id).one()[0]
                     continue
                 # Check if this is a STUCK lock due to source_replica filtering
                 if source_rses:
                     associated_replica = [replica for replica in replicas[(file['scope'], file['name'])] if replica.rse_id == lock.rse_id][0]
-                    # Check if there is an eglible source replica for this lock
+                    # Check if there is an eligible source replica for this lock
                     if set(source_replicas.get((file['scope'], file['name']), [])).intersection(source_rses) and (selector_rse_dict.get(lock.rse_id, {}).get('availability_write', True) or rule.ignore_availability):
                         __update_lock_replica_and_create_transfer(lock=lock,
                                                                   replica=associated_replica,
                                                                   rule=rule,
                                                                   dataset=dataset,
                                                                   transfers_to_create=transfers_to_create,
                                                                   session=session)
@@ -841,15 +842,15 @@
     :param dataset:              Dataset dictionary holding the dataset information.
     :param rule:                 Rule object.
     :param rse_id:               RSE id the lock and replica should be created at.
     :param staging_area:         Boolean variable if the RSE is a staging area.
     :param availability_write:   Boolean variable if the RSE is write enabled.
     :param locks_to_create:      Dictionary of the locks to create.
     :param locks:                Dictionary of all locks.
-    :param source_rses:          RSE ids of eglible source replicas.
+    :param source_rses:          RSE ids of eligible source replicas.
     :param replicas_to_create:   Dictionary of the replicas to create.
     :param replicas:             Dictionary of the replicas.
     :param source_replicas:      Dictionary of the source replicas.
     :param transfers_to_create:  List of transfers to create.
     :param session:              The db session in use.
     :param logger:               Optional decorated logger that can be passed from the calling daemons or servers.
     :returns:                    True, if the created lock is replicating, False otherwise.
@@ -874,16 +875,16 @@
                                                         adler32=file['adler32'],
                                                         ds_scope=dataset['scope'],
                                                         ds_name=dataset['name'],
                                                         copy_pin_lifetime=copy_pin_lifetime,
                                                         session=session))
 
     # If staging_required type RSE then set pin to RSE attribute maximum_pin_lifetime
-    staging_required = get_rse_attribute(rse_id, 'staging_required', session=session)
-    maximum_pin_lifetime = get_rse_attribute(rse_id, 'maximum_pin_lifetime', session=session)
+    staging_required = get_rse_attribute(rse_id, RseAttr.STAGING_REQUIRED, session=session)
+    maximum_pin_lifetime = get_rse_attribute(rse_id, RseAttr.MAXIMUM_PIN_LIFETIME, session=session)
 
     if staging_required:
         if (not copy_pin_lifetime and maximum_pin_lifetime) or (copy_pin_lifetime and maximum_pin_lifetime and copy_pin_lifetime < int(maximum_pin_lifetime)):
             copy_pin_lifetime = maximum_pin_lifetime
         rse_name = get_rse_name(rse_id=rse_id, session=session)
         logger(logging.DEBUG, f'Destination RSE {rse_name} is type staging_required with pin value: {copy_pin_lifetime}')
 
@@ -923,15 +924,15 @@
                                                             session=session))
 
         # Replica is not available -- UNAVAILABLE
         elif existing_replica.state == ReplicaState.UNAVAILABLE:
             available_source_replica = True
             if source_rses:
                 available_source_replica = False
-                # Check if there is an eglible source replica for this lock
+                # Check if there is an eligible source replica for this lock
                 if set(source_replicas.get((file['scope'], file['name']), [])).intersection(source_rses):
                     available_source_replica = True
             new_lock = __create_lock(rule=rule,
                                      rse_id=rse_id,
                                      scope=file['scope'],
                                      name=file['name'],
                                      bytes_=file['bytes'],
@@ -970,15 +971,15 @@
             locks_to_create[rse_id].append(new_lock)
             locks[(file['scope'], file['name'])].append(new_lock)
             return True
     else:  # Replica has to be created
         available_source_replica = True
         if source_rses:
             available_source_replica = False
-            # Check if there is an eglible source replica for this lock
+            # Check if there is an eligible source replica for this lock
             if set(source_replicas.get((file['scope'], file['name']), [])).intersection(source_rses):
                 available_source_replica = True
 
         new_replica = __create_replica(rse_id=rse_id,
                                        scope=file['scope'],
                                        name=file['name'],
                                        bytes_=file['bytes'],
@@ -1304,15 +1305,15 @@
         # handle dataset case by converting it to singleton container case
         # NOTE: this will handle DATASET/ALL as if it was DATASET/DATASET
         datasets = []  # [(scope,name)]
         if did.did_type == DIDType.DATASET:
             datasets.append((did.scope, did.name, ))
         elif did.did_type == DIDType.CONTAINER:
             for child_dataset in rucio.core.did.list_child_datasets(scope=did.scope, name=did.name, session=session):
-                # ensure theer are no duplicates
+                # ensure there are no duplicates
                 newds = (child_dataset['scope'], child_dataset['name'], )
                 if newds not in datasets:
                     datasets.append(newds)
         # sort alphabetically for deterministic order
         try:
             datasets = sorted(datasets)
         except Exception:
```

### Comparing `rucio-34.2.0/lib/rucio/core/scope.py` & `rucio-34.3.0/lib/rucio/core/scope.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/core/subscription.py` & `rucio-34.3.0/lib/rucio/core/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 import logging
 import re
 from configparser import NoOptionError, NoSectionError
 from json import dumps
 from typing import TYPE_CHECKING
 
 from sqlalchemy import func
-from sqlalchemy.exc import IntegrityError, StatementError
+from sqlalchemy.exc import IntegrityError, NoResultFound, StatementError
 from sqlalchemy.orm import aliased
-from sqlalchemy.orm.exc import NoResultFound
 
 from rucio.common.config import config_get
 from rucio.common.exception import RucioException, SubscriptionDuplicate, SubscriptionNotFound
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import SubscriptionState
 from rucio.db.sqla.session import read_session, stream_session, transactional_session
 
@@ -226,15 +225,15 @@
     :raises:                   exception.NotFound if subscription is not found
     """
     query = session.query(models.Subscription)
     try:
         if name:
             query = query.filter_by(name=name)
         if account:
-            if '*' in account.internal:
+            if account.internal is not None and '*' in account.internal:
                 account_str = account.internal.replace('*', '%')
                 query = query.filter(models.Subscription.account.like(account_str))
             else:
                 query = query.filter_by(account=account)
         if state:
             query = query.filter_by(state=state)
     except IntegrityError as error:
```

### Comparing `rucio-34.2.0/lib/rucio/core/topology.py` & `rucio-34.3.0/lib/rucio/core/topology.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,23 +28,25 @@
 from rucio.common.utils import PriorityQueue
 from rucio.core.rse import RseCollection, RseData
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.db.sqla import models
 from rucio.db.sqla.session import read_session, transactional_session
 from rucio.rse import rsemanager as rsemgr
 
-LoggerFunction = Callable[..., Any]
 _Number = Union[int, Decimal]
 TN = TypeVar("TN", bound="Node")
 TE = TypeVar("TE", bound="Edge")
 
 if TYPE_CHECKING:
     from typing import Protocol
 
     from sqlalchemy.orm import Session
+    from typing_extensions import Self
+
+    from rucio.common.types import HopDict, LoggerFunction
 
     class _StateProvider(Protocol):
         @property
         def cost(self) -> _Number:
             ...
 
         @property
@@ -77,19 +79,19 @@
         self._dst_node = weakref.ref(dst_node)
 
         self.cost: _Number = 1
         self.enabled: bool = True
 
         self.add_to_nodes()
 
-    def add_to_nodes(self):
+    def add_to_nodes(self) -> None:
         self.src_node.out_edges[self.dst_node] = self
         self.dst_node.in_edges[self.src_node] = self
 
-    def remove_from_nodes(self):
+    def remove_from_nodes(self) -> None:
         self.src_node.out_edges.pop(self.dst_node, None)
         self.dst_node.in_edges.pop(self.src_node, None)
 
     @property
     def src_node(self) -> TN:
         node = self._src_node()
         if node is None:
@@ -101,20 +103,20 @@
     def dst_node(self) -> TN:
         node = self._dst_node()
         if node is None:
             # This shouldn't happen if the Node list is correctly managed by the Topology object.
             raise ReferenceError("weak reference returned None")
         return node
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, self.__class__):
             return False
         return self._src_node == other._src_node and self._dst_node == other._dst_node
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f'{self._src_node}-->{self._dst_node}'
 
 
 class Topology(RseCollection, Generic[TN, TE]):
     """
     Helper private class used to easily fetch topological information for a subset of RSEs.
     """
@@ -123,15 +125,15 @@
             rse_ids: Optional[Iterable[str]] = None,
             ignore_availability: bool = False,
             node_cls: type[TN] = Node,
             edge_cls: type[TE] = Edge,
     ):
         super().__init__(rse_ids=rse_ids, rse_data_cls=node_cls)
         self._edge_cls = edge_cls
-        self._edges = {}
+        self._edges: dict[tuple[TN, TN], TE] = {}
         self._edges_loaded = False
         self._multihop_nodes = set()
         self._hop_penalty = DEFAULT_HOP_PENALTY
         self.ignore_availability = ignore_availability
 
         self._lock = threading.RLock()
 
@@ -144,15 +146,15 @@
             load_attributes: bool = False,
             load_info: bool = False,
             load_usage: bool = False,
             load_limits: bool = False,
             include_deleted: bool = False,
             *,
             session: "Session",
-    ):
+    ) -> None:
 
         if not rse_ids:
             with self._lock:
                 rse_ids = list(self.rse_id_to_data_map)
         super().ensure_loaded(
             rse_ids=rse_ids,
             load_name=load_name,
@@ -173,15 +175,15 @@
                 if not rse_data:
                     self.rse_id_to_data_map[rse_id] = rse_data = self._rse_data_cls(rse_id)
                     # A new node added. Edges which were already loaded are probably incomplete now.
                     self._edges_loaded = False
         return rse_data
 
     @property
-    def edges(self):
+    def edges(self) -> dict[tuple[TN, TN], TE]:
         with self._lock:
             return copy.copy(self._edges)
 
     def edge(self, src_node: TN, dst_node: TN) -> "Optional[TE]":
         return self._edges.get((src_node, dst_node))
 
     def get_or_create_edge(self, src_node: TN, dst_node: TN) -> "TE":
@@ -189,29 +191,29 @@
         if not edge:
             with self._lock:
                 edge = self._edges.get((src_node, dst_node))
                 if not edge:
                     self._edges[src_node, dst_node] = edge = self._edge_cls(src_node, dst_node)
         return edge
 
-    def delete_edge(self, src_node: TN, dst_node: TN):
+    def delete_edge(self, src_node: TN, dst_node: TN) -> None:
         with self._lock:
             edge = self._edges[src_node, dst_node]
             edge.remove_from_nodes()
 
     @property
     def multihop_enabled(self) -> bool:
         return True if self._multihop_nodes else False
 
     @read_session
-    def configure_multihop(self, multihop_rse_ids: Optional[set[str]] = None, *, session: "Session", logger: LoggerFunction = logging.log):
+    def configure_multihop(self, multihop_rse_ids: Optional[set[str]] = None, *, session: "Session", logger: "LoggerFunction" = logging.log) -> "Self":
         with self._lock:
             return self._configure_multihop(multihop_rse_ids=multihop_rse_ids, session=session, logger=logger)
 
-    def _configure_multihop(self, multihop_rse_ids: Optional[set[str]] = None, *, session: "Session", logger: LoggerFunction = logging.log):
+    def _configure_multihop(self, multihop_rse_ids: Optional[set[str]] = None, *, session: "Session", logger: "LoggerFunction" = logging.log) -> "Self":
 
         if multihop_rse_ids is None:
             multihop_rse_expression = config_get('transfers', 'multihop_rse_expression', default='available_for_multihop=true', expiration_time=600, session=session)
 
             multihop_rse_ids = set()
             if multihop_rse_expression.strip():
                 try:
@@ -232,25 +234,25 @@
                 node.used_for_multihop = True
                 self._multihop_nodes.add(node)
 
         self._hop_penalty = config_get_int('transfers', 'hop_penalty', default=DEFAULT_HOP_PENALTY, session=session)
         return self
 
     @read_session
-    def ensure_edges_loaded(self, *, session: "Session"):
+    def ensure_edges_loaded(self, *, session: "Session") -> None:
         """
         Ensure that all edges are loaded for the (sub-)set of nodes known by this topology object
         """
         if self._edges_loaded:
             return
 
         with self._lock:
             return self._ensure_edges_loaded(session=session)
 
-    def _ensure_edges_loaded(self, *, session: "Session"):
+    def _ensure_edges_loaded(self, *, session: "Session") -> None:
         stmt = select(
             models.Distance
         ).where(
             and_(
                 models.Distance.src_rse_id.in_(self.rse_id_to_data_map.keys()),
                 models.Distance.dest_rse_id.in_(self.rse_id_to_data_map.keys()),
             )
@@ -277,15 +279,15 @@
                 self.delete_edge(src_node, dst_node)
 
         self._edges_loaded = True
 
     @read_session
     def search_shortest_paths(
             self,
-            src_nodes: list[TN],
+            src_nodes: Iterable[TN],
             dst_node: TN,
             operation_src: str,
             operation_dest: str,
             domain: str,
             limit_dest_schemes: list[str],
             *,
             session: "Session",
@@ -430,15 +432,15 @@
     def __init__(self, ttl, new_obj_fnc):
         self._lock = threading.Lock()
         self._object = None
         self._creation_time = None
         self._new_obj_fnc = new_obj_fnc
         self._ttl = ttl
 
-    def get(self, logger=logging.log):
+    def get(self, logger: "LoggerFunction" = logging.log) -> object:
         with self._lock:
             if not self._object \
                     or not self._creation_time \
                     or datetime.datetime.utcnow() - self._creation_time > datetime.timedelta(seconds=self._ttl):
                 self._object = self._new_obj_fnc()
                 self._creation_time = datetime.datetime.utcnow()
                 logger(logging.INFO, "Refreshed topology object")
@@ -448,15 +450,15 @@
 @transactional_session
 def get_hops(
         source_rse_id: str,
         dest_rse_id: str,
         multihop_rse_ids: Optional[set[str]] = None,
         limit_dest_schemes: Optional[list[str]] = None,
         *, session: "Session",
-):
+) -> list["HopDict"]:
     """
     Get a list of hops needed to transfer date from source_rse_id to dest_rse_id.
     Ideally, the list will only include one item (dest_rse_id) since no hops are needed.
     :param source_rse_id:       Source RSE id of the transfer.
     :param dest_rse_id:         Dest RSE id of the transfer.
     :param multihop_rse_ids:    List of RSE ids that can be used for multihop. If empty, multihop is disabled.
     :param limit_dest_schemes:  List of destination schemes the matching scheme algorithm should be limited to for a single hop.
```

### Comparing `rucio-34.2.0/lib/rucio/core/trace.py` & `rucio-34.3.0/lib/rucio/core/trace.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/core/transfer.py` & `rucio-34.3.0/lib/rucio/core/transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from dogpile.cache import make_region
 from dogpile.cache.api import NoValue
 from sqlalchemy import select, update
 from sqlalchemy.exc import IntegrityError
 
 from rucio.common import constants
 from rucio.common.config import config_get, config_get_list
-from rucio.common.constants import SUPPORTED_PROTOCOLS
+from rucio.common.constants import SUPPORTED_PROTOCOLS, RseAttr
 from rucio.common.exception import InvalidRSEExpression, RequestNotFound, RSEProtocolNotSupported, RucioException, UnsupportedOperation
 from rucio.common.utils import construct_surl
 from rucio.core import did
 from rucio.core import message as message_core
 from rucio.core import request as request_core
 from rucio.core.account import list_accounts
 from rucio.core.monitor import MetricManager
@@ -48,15 +48,15 @@
 from rucio.transfertool.fts3 import FTS3Transfertool
 from rucio.transfertool.globus import GlobusTransferTool
 from rucio.transfertool.mock import MockTransfertool
 from rucio.transfertool.transfertool import TransferStatusReport, Transfertool
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
-    from typing import Any, Optional, Type
+    from typing import Any, Optional
 
     from sqlalchemy.orm import Session
 
     from rucio.common.types import InternalAccount
     from rucio.core.topology import Topology
     from rucio.rse.protocols.protocol import RSEProtocol
 
@@ -71,15 +71,15 @@
 REGION_ACCOUNTS = make_region().configure('dogpile.cache.memory', expiration_time=600)
 METRICS = MetricManager(module=__name__)
 
 WEBDAV_TRANSFER_MODE = config_get('conveyor', 'webdav_transfer_mode', False, None)
 
 DEFAULT_MULTIHOP_TOMBSTONE_DELAY = int(datetime.timedelta(hours=2).total_seconds())
 
-TRANSFERTOOL_CLASSES_BY_NAME: "dict[str, Type[Transfertool]]" = {
+TRANSFERTOOL_CLASSES_BY_NAME: "dict[str, type[Transfertool]]" = {
     FTS3Transfertool.external_name: FTS3Transfertool,
     GlobusTransferTool.external_name: GlobusTransferTool,
     MockTransfertool.external_name: MockTransfertool,
     BittorrentTransfertool.external_name: BittorrentTransfertool,
 }
 
 
@@ -204,16 +204,16 @@
         """
         Generate the source url which will be used as origin to copy the file from request rws towards the given dst endpoint
         """
         # Get source protocol
         protocol = protocol_factory.protocol(src.rse, src.scheme, operation)
 
         # Compute the source URL
-        source_sign_url = src.rse.attributes.get('sign_url', None)
-        dest_sign_url = dst.rse.attributes.get('sign_url', None)
+        source_sign_url = src.rse.attributes.get(RseAttr.SIGN_URL, None)
+        dest_sign_url = dst.rse.attributes.get(RseAttr.SIGN_URL, None)
         source_url = list(protocol.lfns2pfns(lfns={'scope': rws.scope.external, 'name': rws.name, 'path': src.file_path}).values())[0]
         source_url = cls.__rewrite_source_url(source_url, source_sign_url=source_sign_url, dest_sign_url=dest_sign_url, source_scheme=src.scheme)
         return source_url
 
     @classmethod
     def _generate_dest_url(cls, dst: TransferDestination, rws: RequestWithSources, protocol_factory: ProtocolFactory, operation: str):
         """
@@ -225,23 +225,23 @@
         if dst.rse.info['deterministic']:
             dest_url = list(protocol.lfns2pfns(lfns={'scope': rws.scope.external, 'name': rws.name}).values())[0]
         else:
             # compute dest url in case of non deterministic
             # naming convention, etc.
             dsn = get_dsn(rws.scope, rws.name, rws.attributes.get('dsn', None))
             # DQ2 path always starts with /, but prefix might not end with /
-            naming_convention = dst.rse.attributes.get('naming_convention', None)
+            naming_convention = dst.rse.attributes.get(RseAttr.NAMING_CONVENTION, None)
             dest_path = construct_surl(dsn, rws.scope.external, rws.name, naming_convention)
             if dst.rse.is_tape():
                 if rws.retry_count or rws.activity == 'Recovery':
                     dest_path = '%s_%i' % (dest_path, int(time.time()))
 
             dest_url = list(protocol.lfns2pfns(lfns={'scope': rws.scope.external, 'name': rws.name, 'path': dest_path}).values())[0]
 
-        dest_sign_url = dst.rse.attributes.get('sign_url', None)
+        dest_sign_url = dst.rse.attributes.get(RseAttr.SIGN_URL, None)
         dest_url = cls.__rewrite_dest_url(dest_url, dest_sign_url=dest_sign_url)
         return dest_url
 
 
 class StageinTransferImplementation(DirectTransferImplementation):
     """
     A definition of a transfer which triggers a stagein operation.
@@ -256,15 +256,15 @@
             rws: RequestWithSources,
             protocol_factory: ProtocolFactory,
             operation_src: str,
             operation_dest: str
     ):
         if not source.rse.is_tape() or destination.rse.is_tape():
             # allow staging_required QoS RSE to be TAPE to TAPE for pin
-            if not destination.rse.attributes.get('staging_required', None):
+            if not destination.rse.attributes.get(RseAttr.STAGING_REQUIRED, None):
                 raise RucioException("Stageing request {} must be from TAPE to DISK rse. Got {} and {}.".format(rws, source, destination))
         super().__init__(source, destination, rws, protocol_factory, operation_src, operation_dest)
 
     @property
     def dest_url(self) -> str:
         if not self._dest_url:
             self._dest_url = self.src.url if self.src.url else self._generate_source_url(self.src,
@@ -980,15 +980,15 @@
 class SkipRestrictedRSEs(SourceFilterStrategy):
 
     def __init__(self, admin_accounts: "Optional[set[InternalAccount]]" = None):
         super().__init__()
         self.admin_accounts = admin_accounts if admin_accounts is not None else []
 
     def apply(self, ctx: RequestRankingContext, source: RequestSource) -> "Optional[int | _SkipSource]":
-        if source.rse.attributes.get('restricted_read') and ctx.rws.account not in self.admin_accounts:
+        if source.rse.attributes.get(RseAttr.RESTRICTED_READ) and ctx.rws.account not in self.admin_accounts:
             return SKIP_SOURCE
 
 
 class SkipBlocklistedRSEs(SourceFilterStrategy):
 
     def __init__(self, topology: "Topology"):
         super().__init__()
@@ -999,15 +999,15 @@
         if not source.rse.columns['availability_read'] and not self.topology.ignore_availability:
             return SKIP_SOURCE
 
 
 class EnforceStagingBuffer(SourceFilterStrategy):
     def apply(self, ctx: RequestRankingContext, source: RequestSource) -> "Optional[int | _SkipSource]":
         # For staging requests, the staging_buffer attribute must be correctly set
-        if ctx.rws.request_type == RequestType.STAGEIN and source.rse.attributes.get('staging_buffer') != ctx.rws.dest_rse.name:
+        if ctx.rws.request_type == RequestType.STAGEIN and source.rse.attributes.get(RseAttr.STAGING_BUFFER) != ctx.rws.dest_rse.name:
             return SKIP_SOURCE
 
 
 class RestrictTapeSources(SourceFilterStrategy):
     def apply(self, ctx: RequestRankingContext, source: RequestSource) -> "Optional[int | _SkipSource]":
         # Ignore tape sources if they are not desired
         if source.rse.is_tape_or_staging_required() and not ctx.rws.attributes.get("allow_tape_source", True):
@@ -1102,15 +1102,15 @@
 
 class SkipSchemeMissmatch(PathDistance):
     filter_only = True
 
     def apply(self, ctx: RequestRankingContext, source: RequestSource) -> "Optional[int | _SkipSource]":
         path = cast(PathDistance._RankingContext, ctx).paths_for_rws.get(source.rse)
         # path == None means that there is no path;
-        # path == [] means that a path exists (according to distances) but cannot be used (scheme missmatch)
+        # path == [] means that a path exists (according to distances) but cannot be used (scheme mismatch)
         if path is not None and not path:
             return SKIP_SOURCE
 
 
 class SkipIntermediateTape(PathDistance):
     filter_only = True
 
@@ -1227,15 +1227,15 @@
                ','.join('{}:{}:{}'.format(src.rse, src.ranking, src.distance) for src in all_sources[:num_sources_in_logs]),
                '... and %d others' % (len(all_sources) - num_sources_in_logs) if len(all_sources) > num_sources_in_logs else '')
 
         # Check if destination is blocked
         if not (topology.ignore_availability or rws.dest_rse.columns['availability_write']):
             logger(logging.WARNING, '%s: dst RSE is blocked for write. Will skip the submission of new jobs', rws.request_id)
             continue
-        if rws.account not in admin_accounts and rws.dest_rse.attributes.get('restricted_write'):
+        if rws.account not in admin_accounts and rws.dest_rse.attributes.get(RseAttr.RESTRICTED_WRITE):
             logger(logging.WARNING, '%s: dst RSE is restricted for write. Will skip the submission', rws.request_id)
             continue
 
         if rws.transfertool and transfertools and rws.transfertool not in transfertools:
             # The request explicitly asks for a transfertool which this submitter doesn't support
             logger(logging.INFO, '%s: unsupported transfertool. Skipping.', rws.request_id)
             reqs_unsupported_transfertool.add(rws.request_id)
```

### Comparing `rucio-34.2.0/lib/rucio/core/vo.py` & `rucio-34.3.0/lib/rucio/core/vo.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 from typing import TYPE_CHECKING, Any
 
-from sqlalchemy.exc import DatabaseError, IntegrityError
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.exc import DatabaseError, IntegrityError, NoResultFound
 
 from rucio.common import exception
 from rucio.common.config import config_get, config_get_bool
 from rucio.common.types import InternalAccount
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import AccountType, IdentityType
 from rucio.db.sqla.session import read_session, transactional_session
@@ -48,15 +47,15 @@
 @transactional_session
 def add_vo(vo: str, description: str, email: str, *, session: "Session") -> None:
     """
     Add a VO and setup a new root user.
     New root user will have account name 'root' and a userpass identity with username: 'root@<vo>' and password: 'password'
 
     :param vo: 3-letter unique tag for a VO.
-    :param descrition: Descriptive string for the VO (e.g. Full name).
+    :param description: Descriptive string for the VO (e.g. Full name).
     :param email: Contact email for the VO.
     :param session: The db session in use.
     """
     if not config_get_bool('common', 'multi_vo', raise_exception=False, default=False):
         raise exception.UnsupportedOperation('VO operations cannot be performed in single VO mode.')
 
     if len(vo) != 3:
@@ -136,15 +135,15 @@
 
 
 def map_vo(vo: str) -> str:
     """
     Converts a long VO name into the internal short (three letter)
     tag mapping.
     Mappings are loaded from the vo-map section of the config database table.
-    If a mapping is not found, the orignal is returned unchanged.
+    If a mapping is not found, the original is returned unchanged.
     :param vo: The long VO name string.
     :returns: The short VO name string.
     """
     # Newline is ignored by regexp if at end of string, so test for that as well.
     if not LONG_VO_RE.match(vo) or '\n' in vo:
         raise exception.RucioException('Invalid characters in VO name.')
     return config_get("vo-map", vo, raise_exception=False, default=vo)
```

### Comparing `rucio-34.2.0/lib/rucio/core/volatile_replica.py` & `rucio-34.3.0/lib/rucio/core/volatile_replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from collections.abc import Iterable
 from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
 from sqlalchemy import and_, exists, insert, or_, update
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.exc import NoResultFound
 from sqlalchemy.sql.expression import select
 
 from rucio.common import exception
 from rucio.core.rse import get_rse_name
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import ReplicaState
 from rucio.db.sqla.session import transactional_session
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/abacus/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/abacus/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/abacus/account.py` & `rucio-34.3.0/lib/rucio/daemons/abacus/account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/abacus/collection_replica.py` & `rucio-34.3.0/lib/rucio/daemons/abacus/collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/abacus/rse.py` & `rucio-34.3.0/lib/rucio/daemons/abacus/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/atropos/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/atropos/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/atropos/atropos.py` & `rucio-34.3.0/lib/rucio/daemons/atropos/atropos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/auditor/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/auditor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,42 +204,42 @@
 
     delta = timedelta(days=delta_in_days)
 
     configuration = srmdumps.parse_configuration()
 
     while not terminate.is_set():
         try:
-            rse, attemps = queue.get(timeout=30)
+            rse, attempts = queue.get(timeout=30)
         except Queue.Empty:
             continue
         start = datetime.now()
         try:
             logger.debug('Checking "%s"', rse)
             output = consistency(rse, delta, configuration, cache_dir,
                                  results_dir)
             if output:
                 process_output(output)
         except:
             elapsed = (datetime.now() - start).total_seconds() / 60
-            logger.error('Check of "%s" failed in %d minutes, %d remaining attemps', rse, elapsed, attemps, exc_info=True)
+            logger.error('Check of "%s" failed in %d minutes, %d remaining attempts', rse, elapsed, attempts, exc_info=True)
             success = False
         else:
             elapsed = (datetime.now() - start).total_seconds() / 60
             logger.info('SUCCESS checking "%s" in %d minutes', rse, elapsed)
             success = True
 
         if not keep_dumps:
             remove = glob.glob(os.path.join(cache_dir, 'replicafromhdfs_{0}_*'.format(rse)))
             remove.extend(glob.glob(os.path.join(cache_dir, 'ddmendpoint_{0}_*'.format(rse))))
             logger.debug('Removing: %s', remove)
             for fil in remove:
                 os.remove(fil)
 
-        if not success and attemps > 0:
-            retry.put((rse, attemps - 1))
+        if not success and attempts > 0:
+            retry.put((rse, attempts - 1))
 
 
 def activity_logger(logpipes, logfilename, terminate):
     handler = logging.handlers.RotatingFileHandler(
         logfilename,
         maxBytes=20971520,
         backupCount=10,
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/auditor/hdfs.py` & `rucio-34.3.0/lib/rucio/daemons/auditor/hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/auditor/srmdumps.py` & `rucio-34.3.0/lib/rucio/daemons/auditor/srmdumps.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import os
 import re
 
 import gfal2
 import requests
 
 from rucio.common.config import get_config_dirs
+from rucio.common.constants import RseAttr
 from rucio.common.dumper import DUMPS_CACHE_DIR, HTTPDownloadFailed, ddmendpoint_url, gfal_download_to_file, http_download_to_file, temp_file
 from rucio.core.credential import get_signed_url
 from rucio.core.rse import get_rse_id, list_rse_attributes
 
 CHUNK_SIZE = 10485760
 
 __DUMPERCONFIGDIRS = (os.path.join(confdir, 'auditor') for confdir in get_config_dirs())
@@ -37,15 +38,15 @@
 
 OBJECTSTORE_NUM_TRIES = 30
 
 
 class Parser(ConfigParser.RawConfigParser):
     '''
     RawConfigParser subclass that doesn't modify the the name of the options
-    and removes any quotes arround the string values.
+    and removes any quotes around the string values.
     '''
     remove_quotes_re = re.compile(r"^'(.+)'$")
     remove_double_quotes_re = re.compile(r'^"(.+)"$')
 
     def optionxform(self, optionstr):
         return optionstr
 
@@ -214,23 +215,23 @@
         configuration.read(glob.glob(conf_dir + '/*.cfg'))
     return configuration
 
 
 def download_rse_dump(rse, configuration, date=None, destdir=DUMPS_CACHE_DIR):
     '''
     Downloads the dump for the given ddmendpoint. If this endpoint does not
-    follow the standarized method to publish the dumps it should have an
+    follow the standardized method to publish the dumps it should have an
     entry in the `configuration` object describing how to download the dump.
 
     `rse` is the DDMEndpoint name.
 
     `configuration` is a RawConfigParser subclass.
 
     `date` is a datetime instance with the date of the desired dump or None
-    to download the lastest available dump.
+    to download the latest available dump.
 
     `destdir` is the directory where the dump will be saved (the final component
     in the path is created if it doesn't exist).
 
     Return value: a tuple with the filename and a datetime instance with
     the date of the dump.
     '''
@@ -239,15 +240,15 @@
 
     if not os.path.isdir(destdir):
         os.mkdir(destdir)
 
     # check for objectstores, which need to be handled differently
     rse_id = get_rse_id(rse)
     rse_attr = list_rse_attributes(rse_id)
-    if 'is_object_store' in rse_attr and rse_attr['is_object_store'] is not False:
+    if RseAttr.IS_OBJECT_STORE in rse_attr and rse_attr[RseAttr.IS_OBJECT_STORE] is not False:
         tries = 1
         if date is None:
             # on objectstores, can't list dump files, so try the last N dates
             date = datetime.datetime.now()
             tries = OBJECTSTORE_NUM_TRIES
         path = ''
         while tries > 0:
@@ -259,16 +260,16 @@
                 date.strftime('%d-%m-%Y'),
                 hashlib.sha1(url.encode()).hexdigest()
             )
             filename = re.sub(r'\W', '-', filename)
             path = os.path.join(destdir, filename)
             if not os.path.exists(path):
                 logger.debug('Trying to download: "%s"', url)
-                if 'sign_url' in rse_attr:
-                    url = get_signed_url(rse_id, rse_attr['sign_url'], 'read', url)
+                if RseAttr.SIGN_URL in rse_attr:
+                    url = get_signed_url(rse_id, rse_attr[RseAttr.SIGN_URL], 'read', url)
                 try:
                     with temp_file(destdir, final_name=filename) as (f, _):
                         download(url, f)
                     tries = 0
                 except (HTTPDownloadFailed, gfal2.GError):
                     tries -= 1
                     date = date - datetime.timedelta(1)
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/automatix/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/automatix/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/automatix/automatix.py` & `rucio-34.3.0/lib/rucio/daemons/automatix/automatix.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
                 if dataset_lifetime:
                     file_["dataset_meta"]["lifetime"] = dataset_lifetime
             files.append(file_)
         logger(logging.INFO, "Upload %s:%s to %s", scope, dsn, rse)
         upload_client = UploadClient(client)
         ret = upload_client.upload(files)
         if ret == 0:
-            logger(logging.INFO, "%s sucessfully registered" % dsn)
+            logger(logging.INFO, "%s successfully registered" % dsn)
             METRICS.counter(name="addnewdataset.done").inc()
             METRICS.counter(name="addnewfile.done").inc(nbfiles)
             METRICS.timer(name='datasetinjection').observe(stopwatch.elapsed)
         else:
             logger(logging.INFO, "Error uploading files")
         for physical_fname in physical_fnames:
             remove(physical_fname)
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/badreplicas/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/badreplicas/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/badreplicas/minos.py` & `rucio-34.3.0/lib/rucio/daemons/badreplicas/minos.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         bulk_delete_bad_pfns(pfns=unknown_replicas, session=None)
     return dict_rse
 
 
 def __update_temporary_unavailable(chunk: list, reason: str, expires_at: datetime, account: "InternalAccount", logger: "Callable") -> None:
     """
     Update temporary unavailable replicas one by one
-    :param chunk: List of unvailable replicas to update
+    :param chunk: List of unavailable replicas to update
     :param reason: Reason of the temporary unavailable replica
     :param expires_at: Expiration date of the temporary unavailability
     :param account: Account who declared the replica
     :param logger: The logger
 
     """
     for rep in chunk:
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py` & `rucio-34.3.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/badreplicas/necromancer.py` & `rucio-34.3.0/lib/rucio/daemons/badreplicas/necromancer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/bb8/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/bb8/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/bb8/bb8.py` & `rucio-34.3.0/lib/rucio/daemons/bb8/bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/bb8/common.py` & `rucio-34.3.0/lib/rucio/daemons/bb8/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -700,15 +700,15 @@
             rebalanced_files += length
             rebalanced_datasets.append(
                 (scope, name, bytes_, length, target_rse_exp, rule_id, child_rule_id)
             )
         except Exception as error:
             logger(
                 logging.ERROR,
-                "Exception %s occured while rebalancing %s:%s, rule_id: %s!",
+                "Exception %s occurred while rebalancing %s:%s, rule_id: %s!",
                 str(error),
                 scope,
                 name,
                 str(rule_id),
             )
 
     logger(
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py` & `rucio-34.3.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """
 This script is to be used to background rebalance ATLAS t2 datadisks
 """
 
 from sqlalchemy import or_
 
+from rucio.common.constants import RseAttr
 from rucio.core.rse import get_rse_attribute, get_rse_usage
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.daemons.bb8.common import rebalance_rse
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import RuleState
 from rucio.db.sqla.session import get_session
 
@@ -55,15 +56,15 @@
 # Calculate the current ratios
 rses = parse_expression("(datapolicynucleus=true|tier=1)&type=DATADISK\\bb8-enabled=false")
 total_primary = 0
 total_secondary = 0
 total_total = 0
 global_ratio = float(0)
 for rse in rses:
-    site_name = get_rse_attribute(rse['id'], 'site')
+    site_name = get_rse_attribute(rse['id'], RseAttr.SITE)
     rse['groupdisk'] = group_space(site_name)
     rse['primary'] = get_rse_usage(rse_id=rse['id'], source='rucio')[0]['used'] - get_rse_usage(rse_id=rse['id'], source='expired')[0]['used']
     rse['primary'] += rse['groupdisk']
     rse['secondary'] = get_rse_usage(rse_id=rse['id'], source='expired')[0]['used']
     rse['total'] = get_rse_usage(rse_id=rse['id'], source='storage')[0]['total'] - get_rse_usage(rse_id=rse['id'], source='min_free_space')[0]['used']
     rse['ratio'] = float(rse['primary']) / float(rse['total'])
     total_primary += rse['primary']
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/bb8/t2_background_rebalance.py` & `rucio-34.3.0/lib/rucio/daemons/bb8/t2_background_rebalance.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """
 This script is to be used to background rebalance ATLAS t2 datadisks
 """
 
 from sqlalchemy import or_
 
+from rucio.common.constants import RseAttr
 from rucio.core.rse import get_rse_attribute, get_rse_usage
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.daemons.bb8.common import rebalance_rse
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import RuleState
 from rucio.db.sqla.session import get_session
 
@@ -55,15 +56,15 @@
 # Calculate the current ratios
 rses = parse_expression("datapolicynucleus=false&tier=2&type=DATADISK\\bb8-enabled=false")
 total_primary = 0
 total_secondary = 0
 total_total = 0
 global_ratio = float(0)
 for rse in rses:
-    site_name = get_rse_attribute(rse['id'], 'site')
+    site_name = get_rse_attribute(rse['id'], RseAttr.SITE)
     rse['groupdisk'] = group_space(site_name)
     rse['primary'] = get_rse_usage(rse_id=rse['id'], source='rucio')[0]['used'] - get_rse_usage(rse_id=rse['id'], source='expired')[0]['used']
     rse['primary'] += rse['groupdisk']
     rse['secondary'] = get_rse_usage(rse_id=rse['id'], source='expired')[0]['used']
     rse['total'] = get_rse_usage(rse_id=rse['id'], source='storage')[0]['total'] - get_rse_usage(rse_id=rse['id'], source='min_free_space')[0]['used']
     rse['ratio'] = float(rse['primary']) / float(rse['total'])
     total_primary += rse['primary']
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/simple.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/simple.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from operator import itemgetter
 
 from rucio.common.config import config_get, config_get_int
+from rucio.common.constants import RseAttr
 from rucio.common.exception import DataIdentifierNotFound
 from rucio.core.did import get_did
 from rucio.core.replica import list_dataset_replicas
 from rucio.core.rse import get_rse, get_rse_name, list_rse_attributes
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.daemons.c3po.collectors.free_space import FreeSpaceCollector
 from rucio.daemons.c3po.collectors.network_metrics import NetworkMetricsCollector
@@ -56,15 +57,15 @@
 
         self._rses = {}
         self._sites = {}
         for rse in rses:
             rse_attrs = list_rse_attributes(rse_id=rse['id'])
             rse_attrs['rse_id'] = rse['id']
             self._rses[rse['id']] = rse_attrs
-            self._sites[rse_attrs['site']] = rse_attrs
+            self._sites[rse_attrs[RseAttr.SITE]] = rse_attrs
 
         self._dst_penalties = {}
         self._src_penalties = {}
 
         self._print_params()
 
     def _print_params(self):
@@ -161,18 +162,18 @@
         reps = list_dataset_replicas(did[0], did[1])
         num_reps = 0
         space_info = self._fsc.get_rse_space()
         max_mbps = 0.0
         for rep in reps:
             rse_attr = list_rse_attributes(rep['rse_id'])
             src_rse_id = rep['rse_id']
-            if 'site' not in rse_attr:
+            if RseAttr.SITE not in rse_attr:
                 continue
 
-            src_site = rse_attr['site']
+            src_site = rse_attr[RseAttr.SITE]
             src_rse_info = get_rse(rse_id=src_rse_id)
 
             if 'type' not in rse_attr:
                 continue
             if rse_attr['type'] != 'DATADISK':
                 continue
             if not src_rse_info['availability_read']:
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/c3po.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/c3po.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/agis.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/agis.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/free_space.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/free_space.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/jedi_did.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/jedi_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/mock_did.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/mock_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/network_metrics.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/network_metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/collectors/workload.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/workload.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/utils/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/utils/dataset_cache.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/utils/dataset_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/utils/expiring_list.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/utils/expiring_list.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/utils/popularity.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/utils/popularity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/c3po/utils/timeseries.py` & `rucio-34.3.0/lib/rucio/daemons/c3po/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/cache/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/cache/consumer.py` & `rucio-34.3.0/lib/rucio/daemons/cache/consumer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/common.py` & `rucio-34.3.0/lib/rucio/daemons/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     Simple contextmanager which sets a heartbeat and associated logger on entry and cleans up the heartbeat on exit.
     """
 
     def __init__(self, executable: str, renewal_interval: int):
         """
         :param executable: the executable name which will be set in heartbeats
         :param renewal_interval: the interval at which the heartbeat will be renewed in the database.
-        Calls to live() in-between intervals will re-use the locally cached heartbeat.
+        Calls to live() in-between intervals will reuse the locally cached heartbeat.
         """
         self.executable = executable
         self._hash_executable = None
         self.renewal_interval = renewal_interval
         self.older_than = renewal_interval * 10 if renewal_interval and renewal_interval > 0 else None  # 10 was chosen without any particular reason
 
         self.hostname = socket.getfqdn()
@@ -175,15 +175,15 @@
     Used to wrap a function for interacting with the database as a work queue: i.e. to select
     a set of rows and perform some work on those rows while ensuring that two instances running in parallel don't
     work on the same set of rows. The last condition is ensured by using heartbeats to keep track of currently
     active workers.
 
     :param once: Whether to stop after one iteration
     :param graceful_stop: the threading.Event() object used for graceful stop of the daemon
-    :param executable: the name of the executable used for hearbeats
+    :param executable: the name of the executable used for heartbeats
     :param partition_wait_time: time to wait for database partition rebalancing before starting the actual daemon loop
     :param sleep_time: time to sleep between the iterations of the daemon
     :param activities: optional list of activities on which to work. The run_once_fnc will be called on activities one by one.
     """
 
     def _decorate(run_once_fnc: Callable[..., Optional[Union[bool, tuple[bool, T]]]]) -> Callable[[], Iterator[Optional[T]]]:
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/conveyor/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/conveyor/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/conveyor/common.py` & `rucio-34.3.0/lib/rucio/daemons/conveyor/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import functools
 import itertools
 import logging
 import re
 from typing import TYPE_CHECKING
 
 from rucio.common.config import config_get_bool
+from rucio.common.constants import RseAttr
 from rucio.common.exception import DatabaseException, DuplicateFileTransferSubmission, InvalidRSEExpression, RequestNotFound, TransferToolTimeout, TransferToolWrongAnswer, VONotFound
 from rucio.common.stopwatch import Stopwatch
 from rucio.core import request as request_core
 from rucio.core import transfer as transfer_core
 from rucio.core.monitor import MetricManager
 from rucio.core.replica import add_replicas, tombstone_from_delay, update_replica_state
 from rucio.core.request import queue_requests, transition_request_state
@@ -37,16 +38,16 @@
 from rucio.core.vo import list_vos
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import ReplicaState, RequestState
 from rucio.db.sqla.session import transactional_session
 from rucio.rse import rsemanager as rsemgr
 
 if TYPE_CHECKING:
-    from collections.abc import Callable, Sequence
-    from typing import Mapping, Optional
+    from collections.abc import Callable, Mapping, Sequence
+    from typing import Optional
 
     from sqlalchemy.orm import Session
 
     from rucio.common.types import InternalAccount
     from rucio.core.request import DirectTransfer, RequestWithSources
     from rucio.core.topology import Topology
     from rucio.core.transfer import ProtocolFactory
@@ -320,15 +321,15 @@
     # next_hop.rws.request_id will always be initialized when handling the current hop.
     for i in reversed(range(len(transfer_path))):
         hop = transfer_path[i]
         rws = hop.rws
         if rws.request_id:
             continue
 
-        tombstone_delay = rws.dest_rse.attributes.get('multihop_tombstone_delay', default_tombstone_delay)
+        tombstone_delay = rws.dest_rse.attributes.get(RseAttr.MULTIHOP_TOMBSTONE_DELAY, default_tombstone_delay)
         try:
             tombstone = tombstone_from_delay(tombstone_delay)
         except ValueError:
             logger(logging.ERROR, "%s: Cannot parse multihop tombstone delay %s", initial_request_id, tombstone_delay)
             creation_successful = False
             break
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/conveyor/finisher.py` & `rucio-34.3.0/lib/rucio/daemons/conveyor/finisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
     """
 
     GRACEFUL_STOP.set()
 
 
 def run(once=False, total_threads=1, sleep_time=60, activities=None, bulk=100, db_bulk=1000):
     """
-    Starts up the conveyer threads.
+    Starts up the conveyor threads.
     """
     setup_logging(process_name=DAEMON_NAME)
 
     if rucio.db.sqla.util.is_old_db():
         raise DatabaseException('Database was not updated, daemon won\'t start')
 
     cached_topology = ExpiringObjectCache(ttl=300, new_obj_fnc=lambda: Topology())
@@ -412,15 +412,15 @@
             except Exception:
                 logger(logging.ERROR, "Something unexpected happened when handling replicas on %s rule %s", req_type, rule_id, exc_info=True)
 
 
 @transactional_session
 def __update_bulk_replicas(replicas, *, session, logger=logging.log):
     """
-    Used by finisher to handle available and unavailable replicas blongs to same rule in bulk way.
+    Used by finisher to handle available and unavailable replicas belongs to same rule in bulk way.
 
     :param replicas:              List of replicas.
     :param session:               The database session to use.
     :returns commit_or_rollback:  Boolean.
     """
     try:
         replica_core.update_replicas_states(replicas, nowait=True, session=session)
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/conveyor/poller.py` & `rucio-34.3.0/lib/rucio/daemons/conveyor/poller.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 import datetime
 import itertools
 import json
 import logging
 import re
 import threading
 import time
-from collections.abc import Sequence
+from collections.abc import Mapping, Sequence
 from itertools import groupby
 from types import FrameType
-from typing import TYPE_CHECKING, Any, Mapping, Optional
+from typing import TYPE_CHECKING, Any, Optional
 
 from requests.exceptions import RequestException
 from sqlalchemy.exc import DatabaseError
 
 import rucio.db.sqla.util
 from rucio.common.config import config_get, config_get_bool
 from rucio.common.exception import DatabaseException, TransferToolTimeout, TransferToolWrongAnswer
@@ -90,15 +90,15 @@
         transfertool=filter_transfertool,
     )
 
     if transfertool and not filter_transfertool:
         # only keep transfers which don't have any transfertool set, or have one equal to TRANSFER_TOOL
         transfs_tmp = [t for t in transfs if not t['transfertool'] or t['transfertool'] == transfertool]
         if len(transfs_tmp) != len(transfs):
-            logger(logging.INFO, 'Skipping %i transfers because of missmatched transfertool', len(transfs) - len(transfs_tmp))
+            logger(logging.INFO, 'Skipping %i transfers because of mismatched transfertool', len(transfs) - len(transfs_tmp))
         transfs = transfs_tmp
 
     if transfs:
         logger(logging.DEBUG, 'Polling %i transfers for activity %s' % (len(transfs), activity))
 
     must_sleep = False
     if len(transfs) < db_bulk / 2:
@@ -250,15 +250,15 @@
         fts_bulk=100,
         db_bulk=1000,
         older_than=60,
         activity_shares: Optional[str] = None,
         total_threads=1
 ):
     """
-    Starts up the conveyer threads.
+    Starts up the conveyor threads.
     """
     setup_logging(process_name=DAEMON_NAME)
 
     if rucio.db.sqla.util.is_old_db():
         raise DatabaseException('Database was not updated, daemon won\'t start')
 
     parsed_activity_shares = None
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/conveyor/preparer.py` & `rucio-34.3.0/lib/rucio/daemons/conveyor/preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/conveyor/receiver.py` & `rucio-34.3.0/lib/rucio/daemons/conveyor/receiver.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/conveyor/stager.py` & `rucio-34.3.0/lib/rucio/daemons/conveyor/stager.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         vos=None,
         bulk=100,
         source_strategy=None,
         activities=[],
         sleep_time=600
 ):
     """
-    Starts up the conveyer threads.
+    Starts up the conveyor threads.
     """
     setup_logging(process_name=DAEMON_NAME)
 
     if rucio.db.sqla.util.is_old_db():
         raise exception.DatabaseException('Database was not updated, daemon won\'t start')
 
     multi_vo = config_get_bool('common', 'multi_vo', raise_exception=False, default=False)
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/conveyor/submitter.py` & `rucio-34.3.0/lib/rucio/daemons/conveyor/submitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
         sleep_time=600,
         max_sources=4,
         archive_timeout_override=None,
         total_threads=1,
         **_kwargs
 ):
     """
-    Starts up the conveyer threads.
+    Starts up the conveyor threads.
     """
     setup_logging(process_name=DAEMON_NAME)
 
     if rucio.db.sqla.util.is_old_db():
         raise exception.DatabaseException('Database was not updated, daemon won\'t start')
 
     multi_vo = config_get_bool('common', 'multi_vo', raise_exception=False, default=False)
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/conveyor/throttler.py` & `rucio-34.3.0/lib/rucio/daemons/conveyor/throttler.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     """
 
     GRACEFUL_STOP.set()
 
 
 def run(once=False, sleep_time=600):
     """
-    Starts up the conveyer threads.
+    Starts up the conveyor threads.
     """
     setup_logging(process_name=DAEMON_NAME)
 
     if rucio.db.sqla.util.is_old_db():
         raise exception.DatabaseException('Database was not updated, daemon won\'t start')
 
     throttler(once=once, sleep_time=sleep_time)
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/follower/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/follower/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/follower/follower.py` & `rucio-34.3.0/lib/rucio/daemons/follower/follower.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/hermes/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/hermes/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/hermes/hermes.py` & `rucio-34.3.0/lib/rucio/daemons/hermes/hermes.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,14 +145,16 @@
         logger(
             logging.INFO,
             "[broker] Could not find use_ssl in configuration -- please update your rucio.cfg",
         )
 
     port = config_get_int("messaging-hermes", "port")
     vhost = config_get("messaging-hermes", "broker_virtual_host", raise_exception=False)
+    username = None
+    password = None
     if not use_ssl:
         username = config_get("messaging-hermes", "username")
         password = config_get("messaging-hermes", "password")
         port = config_get_int("messaging-hermes", "nonssl_port")
 
     conns = []
     for broker in brokers_resolved:
@@ -385,15 +387,15 @@
     messages: list[dict], bin_size: int, endpoint: str, logger: "Callable"
 ) -> int:
     """
     Aggregate a list of message using a certain bin_size
     and submit them to a InfluxDB endpoint
 
     :param messages:           The list of messages.
-    :param bin_size:           The size of the bins for the aggreagation (e.g. 10m, 1h, etc.).
+    :param bin_size:           The size of the bins for the aggregation (e.g. 10m, 1h, etc.).
     :param endpoint:           The InfluxDB endpoint were to send the messages.
     :param logger:             The logger object.
 
     :returns:                  HTTP status code. 200 and 204 OK. Rest is failure.
     """
     bins = {}
     dtime = datetime.datetime.now()
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/judge/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/judge/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/judge/cleaner.py` & `rucio-34.3.0/lib/rucio/daemons/judge/cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/judge/evaluator.py` & `rucio-34.3.0/lib/rucio/daemons/judge/evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/judge/injector.py` & `rucio-34.3.0/lib/rucio/daemons/judge/injector.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/judge/repairer.py` & `rucio-34.3.0/lib/rucio/daemons/judge/repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/oauthmanager/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/oauthmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/oauthmanager/oauthmanager.py` & `rucio-34.3.0/lib/rucio/daemons/oauthmanager/oauthmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-OAuth Manager is a daemon which is reponsible for:
+OAuth Manager is a daemon which is responsible for:
 - deletion of expired access tokens (in case there is a valid refresh token,
   expired access tokens will be kept until refresh_token expires as well.)
 - deletion of expired OAuth session parameters
 - refreshing access tokens via their refresh tokens.
 
 These 3 actions run consequently one after another in a loop with a sleeptime of 'looprate' seconds.
 The maximum number of DB rows (tokens, parameters, refresh tokens) on which the script will operate
@@ -110,15 +110,15 @@
             logger(logging.WARNING, traceback.format_exc())
             METRICS.counter('exceptions.{exception}').labels(exception=err.__class__.__name__).inc()
         else:
             logger(logging.CRITICAL, traceback.format_exc())
             METRICS.counter('exceptions.{exception}').labels(exception=err.__class__.__name__).inc()
 
     try:
-        # waiting 1 sec as DBs does not store milisecond and tokens
+        # waiting 1 sec as DBs does not store millisecond and tokens
         # eligible for deletion after refresh might not get deleted otherwise
         graceful_stop.wait(1)
 
         # make a heartbeat
         worker_number, total_workers, logger = heartbeat_handler.live()
 
         # EXPIRED TOKEN DELETION
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/reaper/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/reaper/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/reaper/dark_reaper.py` & `rucio-34.3.0/lib/rucio/daemons/reaper/dark_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/reaper/reaper.py` & `rucio-34.3.0/lib/rucio/daemons/reaper/reaper.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 from dogpile.cache.api import NoValue
 from sqlalchemy.exc import DatabaseError, IntegrityError
 
 import rucio.db.sqla.util
 from rucio.common.cache import make_region_memcached
 from rucio.common.config import config_get_bool, config_get_int
+from rucio.common.constants import RseAttr
 from rucio.common.exception import DatabaseException, ReplicaNotFound, ReplicaUnAvailable, ResourceTemporaryUnavailable, RSEAccessDenied, RSENotFound, RSEProtocolNotSupported, ServiceUnavailable, SourceNotFound, VONotFound
 from rucio.common.logging import setup_logging
 from rucio.common.stopwatch import Stopwatch
 from rucio.common.utils import chunks
 from rucio.core.credential import get_signed_url
 from rucio.core.heartbeat import list_payload_counts
 from rucio.core.message import add_message
@@ -191,15 +192,15 @@
                 duration = stopwatch.elapsed
                 logger(logging.WARNING, 'Deletion NOACCESS of %s:%s as %s on %s: %s in %.2f', replica['scope'], replica['name'], replica['pfn'], rse_name, str(error), duration)
                 deletion_dict['reason'] = str(error)
                 deletion_dict['duration'] = duration
                 add_message('deletion-failed', deletion_dict)
                 noaccess_attempts += 1
                 if noaccess_attempts >= auto_exclude_threshold:
-                    logger(logging.INFO, 'Too many (%d) NOACCESS attempts for %s. RSE will be temporarly excluded.', noaccess_attempts, rse_name)
+                    logger(logging.INFO, 'Too many (%d) NOACCESS attempts for %s. RSE will be temporarily excluded.', noaccess_attempts, rse_name)
                     REGION.set('temporary_exclude_%s' % rse_id, True)
                     METRICS.gauge('excluded_rses.{rse}').labels(rse=rse_name).set(1)
 
                     EXCLUDED_RSE_GAUGE.labels(rse=rse_name).set(1)
                     break
 
             except Exception as error:
@@ -223,15 +224,15 @@
                        'bytes': replica['bytes'],
                        'url': replica['pfn'],
                        'reason': str(error),
                        'protocol': prot.attributes['scheme']}
             if replica['scope'].vo != 'def':
                 payload['vo'] = replica['scope'].vo
             add_message('deletion-failed', payload)
-        logger(logging.INFO, 'Cannot connect to %s. RSE will be temporarly excluded.', rse_name)
+        logger(logging.INFO, 'Cannot connect to %s. RSE will be temporarily excluded.', rse_name)
         REGION.set('temporary_exclude_%s' % rse_id, True)
         EXCLUDED_RSE_GAUGE.labels(rse=rse_name).set(1)
     finally:
         prot.close()
     return deleted_files
 
 
@@ -338,20 +339,20 @@
     available_sources['used'] = {key['source']: key['used'] for key in rse.usage}
 
     # Get RSE limits
     min_free_space = rse.limits.get('MinFreeSpace', 0)
 
     # Check from which sources to get used and total spaces (default storage)
     # If specified sources do not exist, only delete obsolete
-    source_for_total_space = rse.attributes.get('source_for_total_space', 'storage')
+    source_for_total_space = rse.attributes.get(RseAttr.SOURCE_FOR_TOTAL_SPACE, 'storage')
     if source_for_total_space not in available_sources['total']:
         logger(logging.WARNING, 'RSE: %s, \'%s\' requested for source_for_total_space but cannot be found. Will only delete obsolete',
                rse.name, source_for_total_space)
         return 0, True
-    source_for_used_space = rse.attributes.get('source_for_used_space', 'storage')
+    source_for_used_space = rse.attributes.get(RseAttr.SOURCE_FOR_USED_SPACE, 'storage')
     if source_for_used_space not in available_sources['used']:
         logger(logging.WARNING, 'RSE: %s, \'%s\' requested for source_for_used_space but cannot be found. Will only delete obsolete',
                rse.name, source_for_used_space)
         return 0, True
 
     logger(logging.DEBUG, 'RSE: %s, source_for_total_space: %s, source_for_used_space: %s',
            rse.name, source_for_total_space, source_for_used_space)
@@ -485,15 +486,15 @@
     tot_needed_free_space = 0
     for rse in rses_to_process:
         # Check if RSE is blocklisted
         if not rse.columns['availability_delete']:
             logger(logging.DEBUG, 'RSE %s is blocklisted for delete', rse.name)
             continue
         rse.ensure_loaded(load_attributes=True)
-        enable_greedy = rse.attributes.get('greedyDeletion', False) or greedy
+        enable_greedy = rse.attributes.get(RseAttr.GREEDYDELETION, False) or greedy
         needed_free_space, only_delete_obsolete = __check_rse_usage_cached(rse, greedy=enable_greedy, logger=logger)
         if needed_free_space:
             dict_rses[rse] = [needed_free_space, only_delete_obsolete, enable_greedy]
             tot_needed_free_space += needed_free_space
         elif only_delete_obsolete:
             dict_rses[rse] = [needed_free_space, only_delete_obsolete, enable_greedy]
         else:
@@ -517,15 +518,15 @@
         if not isinstance(result, NoValue):
             paused_rses.append(rse.name)
             logger(logging.DEBUG, 'Not enough replicas to delete on %s during the previous cycle. Deletion paused for a while', rse.name)
             continue
 
         result = REGION.get('temporary_exclude_%s' % rse.id, expiration_time=auto_exclude_timeout)
         if not isinstance(result, NoValue):
-            logger(logging.WARNING, 'Too many failed attempts for %s in last cycle. RSE is temporarly excluded.', rse.name)
+            logger(logging.WARNING, 'Too many failed attempts for %s in last cycle. RSE is temporarily excluded.', rse.name)
             EXCLUDED_RSE_GAUGE.labels(rse=rse.name).set(1)
             continue
         EXCLUDED_RSE_GAUGE.labels(rse=rse.name).set(0)
 
         percent = 0
         if tot_needed_free_space:
             percent = needed_free_space / tot_needed_free_space * 100
@@ -571,15 +572,15 @@
         except Exception:
             logger(logging.CRITICAL, 'Exception', exc_info=True)
             continue
         # Physical  deletion will take place there
         try:
             rse.ensure_loaded(load_info=True, load_attributes=True)
             prot = rsemgr.create_protocol(rse.info, 'delete', scheme=scheme, logger=logger)
-            if rse.attributes.get('oidc_support') is True and prot.attributes['scheme'] == 'davs':
+            if rse.attributes.get(RseAttr.OIDC_SUPPORT) is True and prot.attributes['scheme'] == 'davs':
                 audience = determine_audience_for_rse(rse.id)
                 # FIXME: At the time of writing, StoRM requires `storage.read`
                 # in order to perform a stat operation.
                 scope = determine_scope_for_rse(rse.id, scopes=['storage.modify', 'storage.read'])
                 auth_token = request_token(audience, scope)
                 if auth_token:
                     logger(logging.INFO, 'Using a token to delete on RSE %s', rse.name)
@@ -605,15 +606,15 @@
                 is_staging = rse.columns['staging_area']
                 deleted_files = delete_from_storage(heartbeat_handler, hb_payload, file_replicas, prot, rse.info, is_staging, auto_exclude_threshold, logger=logger)
                 logger(logging.INFO, '%i files processed in %s seconds', len(file_replicas), time.time() - del_start_time)
 
                 # Then finally delete the replicas
                 del_start = time.time()
                 delete_replicas(rse_id=rse.id, files=deleted_files)
-                logger(logging.DEBUG, 'delete_replicas successed on %s : %s replicas in %s seconds', rse.name, len(deleted_files), time.time() - del_start)
+                logger(logging.DEBUG, 'delete_replicas succeeded on %s : %s replicas in %s seconds', rse.name, len(deleted_files), time.time() - del_start)
                 METRICS.counter('deletion.done').inc(len(deleted_files))
         except RSEProtocolNotSupported:
             logger(logging.WARNING, 'Protocol %s not supported on %s', scheme, rse.name)
         except Exception:
             logger(logging.CRITICAL, 'Exception', exc_info=True)
 
     if paused_rses:
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/replicarecoverer/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/replicarecoverer/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py` & `rucio-34.3.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
     start = time.time()
 
     try:
         json_file = open(json_file_name, mode="r")
         logger(logging.INFO, "JSON file has been opened.")
     except:
-        logger(logging.WARNING, "An error occured while trying to open the JSON file.")
+        logger(logging.WARNING, "An error occurred while trying to open the JSON file.")
         must_sleep = True
         return must_sleep
 
     try:
         json_data = json.load(json_file)
     except ValueError as e:
         logger(logging.WARNING, "No JSON object could be decoded. Error: %s", e)
@@ -404,15 +404,15 @@
 
         # Checking that everything is still working properly
         worker_number, total_workers, logger = heartbeat_handler.live()
 
         auditor = 0
         checksum = 0
 
-        # Label suspicious replicas as bad if they have oher copies on other RSEs (that aren't also marked as suspicious).
+        # Label suspicious replicas as bad if they have other copies on other RSEs (that aren't also marked as suspicious).
         # If they are the last remaining copies, deal with them differently.
         for rse_key in list(recoverable_replicas[vo].keys()):
             files_to_be_declared_bad = []
             files_to_be_ignored = []
             files_dry_run_monitoring = []
             # Remove RSEs from dictionary that don't have any suspicious replicas
             if len(recoverable_replicas[vo][rse_key]) == 0:
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/config.py` & `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """Functions to manage decommissioning configurations."""
 
 from enum import Enum
 from typing import Any
 
+from rucio.common.constants import RseAttr
 from rucio.core.rse import add_rse_attribute, get_rse_attribute
 
 
 class DecommissioningStatus(Enum):
     """Decommissioning status flags."""
 
     PROCESSING = 'processing'
@@ -70,11 +71,11 @@
     status: DecommissioningStatus
 ) -> None:
     """Update the decommission attribute of the RSE.
 
     :param rse_id: RSE ID.
     :param status: RSE decommissioning status.
     """
-    config = attr_to_config(get_rse_attribute(rse_id, 'decommission'))
+    config = attr_to_config(get_rse_attribute(rse_id, RseAttr.DECOMMISSION))
     config['status'] = status
     # add_rse_attribute can handle updating existing entries too
-    add_rse_attribute(rse_id, 'decommission', config_to_attr(config))
+    add_rse_attribute(rse_id, RseAttr.DECOMMISSION, config_to_attr(config))
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py` & `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py` & `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import logging
 from collections.abc import Callable, Iterable
 from datetime import datetime, timedelta
 from typing import Any
 
 from sqlalchemy.exc import NoResultFound
 
+from rucio.common.constants import RseAttr
 from rucio.common.exception import Duplicate, ReplicaNotFound, RequestNotFound, RucioException, RuleNotFound, RuleReplaceFailed, UnsupportedOperation
 from rucio.core.lock import get_replica_locks, get_replica_locks_for_rule_id
 from rucio.core.replica import list_replicas_per_rse, set_tombstone, update_replica_state
 from rucio.core.request import get_request_by_did
 from rucio.core.rse import add_rse_attribute, update_rse
 from rucio.core.rule import list_rules_for_rse_decommissioning, move_rule, update_rule
 from rucio.db.sqla.constants import ReplicaState
@@ -120,15 +121,15 @@
         'availability_read': True,
         'availability_write': False,
         'availability_delete': True
     }
     update_rse(rse['id'], parameters)
 
     try:
-        add_rse_attribute(rse['id'], 'greedyDeletion', True)
+        add_rse_attribute(rse['id'], RseAttr.GREEDYDELETION, True)
     except Duplicate:
         pass
 
 
 def _generic_discover(
     rse: dict[str, Any],
     *,
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py` & `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py` & `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import socket
 import threading
 from collections.abc import Callable
 from types import FrameType
 from typing import TYPE_CHECKING, Any, Optional, Union
 
 from rucio.common.config import config_get_int
+from rucio.common.constants import RseAttr
 from rucio.common.exception import RucioException
 from rucio.common.logging import setup_logging
 from rucio.core.heartbeat import sanity_check
 from rucio.core.rse import get_rse_attribute, get_rses_with_attribute
 from rucio.daemons.common import run_daemon
 from rucio.db.sqla.constants import RuleState
 
@@ -85,20 +86,20 @@
 
     if worker_number != 0:
         logger(logging.INFO, 'RSE decommissioner thread id is not 0, will sleep.'
                ' Only thread 0 will work')
         return True
 
     # Collect all RSEs with the 'decommission' attribute
-    rses = get_rses_with_attribute('decommission')
+    rses = get_rses_with_attribute(RseAttr.DECOMMISSION)
     random.shuffle(rses)
 
     for rse in rses:
         # Get the decommission attribute (encodes the decommissioning config)
-        attr = get_rse_attribute(rse['id'], 'decommission')
+        attr = get_rse_attribute(rse['id'], RseAttr.DECOMMISSION)
         try:
             config = attr_to_config(attr)
         except InvalidStatusName:
             logger(logging.ERROR, 'RSE %s has an invalid decommissioning status',
                    rse['rse'])
             continue
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/storage/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/storage/consistency/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/storage/consistency/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/storage/consistency/actions.py` & `rucio-34.3.0/lib/rucio/daemons/storage/consistency/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -607,15 +607,15 @@
                 logger(logging.INFO, 'The first  %d days older run is: %s'
                        % (minagedark, old_enough_run))
 
                 process_dark_files(path, scope, rse, latest_run, max_dark_fraction,
                                    max_files_at_site, old_enough_run, force_proceed)
             else:
                 logger(logging.INFO, 'There is no other run for this RSE at least %d days older,\
-                 so cannot safely proceed with dark files deleteion.' % minagedark)
+                 so cannot safely proceed with dark files deletion.' % minagedark)
 
             process_miss_files(path, scope, rse, latest_run, max_miss_fraction,
                                max_files_at_site, old_enough_run, force_proceed)
 
         else:
             # This run was already processed
             logger(logging.INFO, 'Nothing to do here')
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/tracer/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/tracer/kronos.py` & `rucio-34.3.0/lib/rucio/daemons/tracer/kronos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/transmogrifier/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/transmogrifier/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/transmogrifier/transmogrifier.py` & `rucio-34.3.0/lib/rucio/daemons/transmogrifier/transmogrifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from collections.abc import Callable
 from datetime import datetime
 from json import dumps, loads
 from typing import TYPE_CHECKING
 
 import rucio.db.sqla.util
 from rucio.common.config import config_get
+from rucio.common.constants import RseAttr
 from rucio.common.exception import (
     DatabaseException,
     DuplicateRule,
     InsufficientAccountLimit,
     InsufficientTargetRSEs,
     InvalidReplicationRule,
     InvalidRSEExpression,
@@ -65,15 +66,15 @@
 RULES_COMMENT_LENGTH = 255
 
 
 def __get_rule_dict(rule_dict: dict, subscription: dict) -> dict:
     """
     Internal method to clean and enrich the rule_dict coming from the subscription.
 
-    :param rule_dict: The rule dictionnary coming from a subscription.
+    :param rule_dict: The rule dictionary coming from a subscription.
     :param subscription: The subscription associated to the rule.
     :return: A dictionary that contains all the parameters associated to the rule.
     """
     source_replica_expression = rule_dict.get("source_replica_expression", None)
     rule_dict["source_replica_expression"] = source_replica_expression
     locked = rule_dict.get("locked", None)
     if locked == "True":
@@ -210,15 +211,15 @@
     if len(preferred_rses) - len(preferred_unmatched) >= copies:
         create_rule = False
     return selected_rses, create_rule, wont_reevaluate
 
 
 def get_subscriptions(logger: Callable = logging.log) -> list[dict]:
     """
-    A method to extract the list of active subscriptions and exclued the one that have bad RSE expression.
+    A method to extract the list of active subscriptions and exclude the one that have bad RSE expression.
     :param logger: The logger.
     :return: The list of active subscriptions.
     """
     subscriptions = []
     try:
         sub_dict = {3: []}
         #  Get the list of subscriptions. The default priority of the subscription is 3. 0 is the highest priority, 5 the lowest
@@ -293,15 +294,15 @@
 
 def __is_matching_subscription(subscription, did, metadata):
     """
     Internal method to identify if a DID matches a subscription.
 
     :param subscription: The subscription dictionary.
     :param did: The DID dictionary
-    :param metadata: The metadata dictionnary for the DID
+    :param metadata: The metadata dictionary for the DID
     :return: True/False
     """
     if metadata["hidden"]:
         return False
     try:
         filter_string = loads(subscription["filter"])
     except ValueError as error:
@@ -395,15 +396,15 @@
         logging.debug("In select_algorithm, %s", str(rule))
         rse = rule["rse_expression"]
         vo = rule["account"].vo
         if rse_exists(rse, vo=vo):
             rse_id = get_rse_id(rse, vo=vo)
             rse_attributes = list_rse_attributes(rse_id)
             if algorithm == "associated_site":
-                associated_sites = rse_attributes.get("associated_sites", None)
+                associated_sites = rse_attributes.get(RseAttr.ASSOCIATED_SITES, None)
                 associated_site_idx = params.get("associated_site_idx", None)
                 if not associated_site_idx:
                     raise SubscriptionWrongParameter(
                         "Missing parameter associated_site_idx"
                     )
                 if associated_sites:
                     associated_sites = associated_sites.split(",")
@@ -413,15 +414,15 @@
                         )
                     associated_site = associated_sites[associated_site_idx - 1]
                     selected_rses[associated_site] = {
                         "source_replica_expression": rse,
                         "weight": None,
                     }
             if algorithm == "exclude_site":
-                site = rse_attributes.get("site", None)
+                site = rse_attributes.get(RseAttr.SITE, None)
                 rse_expression = params['rse_expression'] + '\\site=%s' % site
                 (
                     selected_rses,
                     create_rule,
                     wont_reevaluate,
                 ) = __split_rule_select_rses(
                     subscription_id=params["subscription_id"],
```

### Comparing `rucio-34.2.0/lib/rucio/daemons/undertaker/__init__.py` & `rucio-34.3.0/lib/rucio/daemons/undertaker/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/daemons/undertaker/undertaker.py` & `rucio-34.3.0/lib/rucio/daemons/undertaker/undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/__init__.py` & `rucio-34.3.0/lib/rucio/db/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/__init__.py` & `rucio-34.3.0/lib/rucio/db/sqla/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import TYPE_CHECKING, Optional, TypeVar
+
 from sqlalchemy.sql.expression import bindparam, text
 
+if TYPE_CHECKING:
+    from sqlalchemy.orm import Session
+    from sqlalchemy.orm.query import RowReturningQuery
+    from sqlalchemy.sql.selectable import Select
+
+    Q = TypeVar('Q', RowReturningQuery, Select)
+
 
-def filter_thread_work(session, query, total_threads, thread_id, hash_variable=None):
+def filter_thread_work(
+        session: "Session",
+        query: "Q",
+        total_threads: Optional[int],
+        thread_id: Optional[int],
+        hash_variable: Optional[str] = None
+) -> "Q":
     """ Filters a query to partition thread workloads based on the thread id and total number of threads """
     if thread_id is not None and total_threads is not None and (total_threads - 1) > 0:
         if session.bind.dialect.name == 'oracle':
             bindparams = [bindparam('thread_id', thread_id), bindparam('total_threads', total_threads - 1)]
             if not hash_variable:
                 query = query.filter(text('ORA_HASH(id, :total_threads) = :thread_id').bindparams(*bindparams))
             else:
```

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/constants.py` & `rucio-34.3.0/lib/rucio/db/sqla/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/__init__.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/env.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/env.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py` & `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/models.py` & `rucio-34.3.0/lib/rucio/db/sqla/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -869,15 +869,15 @@
 
 
 class RSEProtocols(BASE, ModelBase):
     """Represents supported protocols of RSEs (Rucio Storage Elements)"""
     __tablename__ = 'rse_protocols'
     rse_id: Mapped[uuid.UUID] = mapped_column(GUID())
     scheme: Mapped[str] = mapped_column(String(255))
-    hostname: Mapped[str] = mapped_column(String(255), server_default='')  # For protocol without host e.g. POSIX on local file systems localhost is assumed as beeing default
+    hostname: Mapped[str] = mapped_column(String(255), server_default='')  # For protocol without host e.g. POSIX on local file systems localhost is assumed as being default
     port: Mapped[int] = mapped_column(Integer, server_default='0')  # like host, for local protocol the port 0 is assumed to be default
     prefix: Mapped[Optional[str]] = mapped_column(String(1024), nullable=True)
     impl: Mapped[str] = mapped_column(String(255), nullable=False)
     read_lan: Mapped[int] = mapped_column(Integer, server_default='0')  # if no value is provided, 0 i.e. not supported is assumed as default value
     write_lan: Mapped[int] = mapped_column(Integer, server_default='0')  # if no value is provided, 0 i.e. not supported is assumed as default value
     delete_lan: Mapped[int] = mapped_column(Integer, server_default='0')  # if no value is provided, 0 i.e. not supported is assumed as default value
     read_wan: Mapped[int] = mapped_column(Integer, server_default='0')  # if no value is provided, 0 i.e. not supported is assumed as default value
```

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/sautils.py` & `rucio-34.3.0/lib/rucio/db/sqla/sautils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/session.py` & `rucio-34.3.0/lib/rucio/db/sqla/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     DEC2FLOAT = psycopg2.extensions.new_type(psycopg2.extensions.DECIMAL.values,
                                              'DEC2FLOAT',
                                              lambda value, curs: float(value) if value is not None else None)
     psycopg2.extensions.register_type(DEC2FLOAT)
 
 
 def my_on_connect(dbapi_con, connection_record):
-    """ Adds information to track performance and ressource by module.
+    """ Adds information to track performance and resource by module.
         Info are recorded in the V$SESSION and V$SQLAREA views.
     """
     caller = basename(sys.argv[0])
     dbapi_con.clientinfo = caller
     dbapi_con.client_identifier = caller
     dbapi_con.module = caller
     dbapi_con.action = caller
@@ -319,15 +319,15 @@
     return False
 
 
 def _update_session_wrapper(wrapper, wrapped):
     """
     In addition to the work done by functools.update_wrapper, this function also preservers
     the signature of the initial function. With the exception that the 'session' parameter
-    is overriden to have a default value of 'None'.
+    is overridden to have a default value of 'None'.
 
     wrapper is the function to be updated
     wrapped is the original function
 
     To simplify the implementation of this function, we require 'session' be a
     keyword-only argument in the wrapped function.
     """
```

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/types.py` & `rucio-34.3.0/lib/rucio/db/sqla/types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/db/sqla/util.py` & `rucio-34.3.0/lib/rucio/db/sqla/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,15 @@
         primary_key = columns[0]
     if not hasattr(primary_key, '__iter__'):
         primary_key = (primary_key, )
 
     oracle_table_is_global = False
     if session.bind.dialect.name == 'oracle':
         # Retrieve the list of global temporary tables on oracle.
-        # If the requested table is found to be global, re-use it,
+        # If the requested table is found to be global, reuse it,
         # otherwise create a private temporary table with random name
         global_temp_tables = list_oracle_global_temp_tables(session=session)
         if oracle_global_name is None:
             oracle_global_name = name
         if oracle_global_name.upper() in global_temp_tables:
             oracle_table_is_global = True
             additional_kwargs = {
```

### Comparing `rucio-34.2.0/lib/rucio/rse/__init__.py` & `rucio-34.3.0/lib/rucio/rse/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/__init__.py` & `rucio-34.3.0/lib/rucio/rse/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/bittorrent.py` & `rucio-34.3.0/lib/rucio/rse/protocols/bittorrent.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/cache.py` & `rucio-34.3.0/lib/rucio/rse/protocols/cache.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/dummy.py` & `rucio-34.3.0/lib/rucio/rse/protocols/dummy.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/gfal.py` & `rucio-34.3.0/lib/rucio/rse/protocols/gfal.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/globus.py` & `rucio-34.3.0/lib/rucio/rse/protocols/globus.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/gsiftp.py` & `rucio-34.3.0/lib/rucio/rse/protocols/gsiftp.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/http_cache.py` & `rucio-34.3.0/lib/rucio/rse/protocols/http_cache.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/mock.py` & `rucio-34.3.0/lib/rucio/rse/protocols/mock.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/ngarc.py` & `rucio-34.3.0/lib/rucio/rse/protocols/ngarc.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/posix.py` & `rucio-34.3.0/lib/rucio/rse/protocols/posix.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/protocol.py` & `rucio-34.3.0/lib/rucio/rse/protocols/protocol.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/rclone.py` & `rucio-34.3.0/lib/rucio/rse/protocols/rclone.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/rfio.py` & `rucio-34.3.0/lib/rucio/rse/protocols/rfio.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/srm.py` & `rucio-34.3.0/lib/rucio/rse/protocols/srm.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/ssh.py` & `rucio-34.3.0/lib/rucio/rse/protocols/ssh.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/storm.py` & `rucio-34.3.0/lib/rucio/rse/protocols/storm.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/webdav.py` & `rucio-34.3.0/lib/rucio/rse/protocols/webdav.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/protocols/xrootd.py` & `rucio-34.3.0/lib/rucio/rse/protocols/xrootd.py`

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

### Comparing `rucio-34.2.0/lib/rucio/rse/rsemanager.py` & `rucio-34.3.0/lib/rucio/rse/rsemanager.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/tests/__init__.py` & `rucio-34.3.0/lib/rucio/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/tests/common.py` & `rucio-34.3.0/lib/rucio/tests/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 
 import contextlib
 import itertools
 import json
 import os
 import tempfile
 from collections import namedtuple
+from collections.abc import Callable, Iterable
 from functools import wraps
 from os import rename
 from random import choice, choices
 from string import ascii_letters, ascii_uppercase, digits
-from typing import Any, Callable, Iterable, Optional
+from typing import Any, Optional
 
 import pytest
 import requests
 
 from rucio.common.config import config_get, config_get_bool, get_config_dirs
 from rucio.common.utils import execute
 from rucio.common.utils import generate_uuid as uuid
@@ -152,15 +153,15 @@
     execute('dd if=/dev/urandom of={0} count={1} bs=1'.format(fn, size))
     return fn
 
 
 def make_temp_file(dir_: str, data: str) -> str:
     """
     Creates a temporal file and write `data` on it.
-    :param data: String to be writen on the created file.
+    :param data: String to be written on the created file.
     :returns: Name of the temporal file.
     """
     fd, path = tempfile.mkstemp(dir=dir_)
     with os.fdopen(fd, 'w', encoding='utf-8') as f:
         f.write(data)
     return path
```

### Comparing `rucio-34.2.0/lib/rucio/tests/common_server.py` & `rucio-34.3.0/lib/rucio/tests/common_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             synchronize_session=False
         )
 
         session.execute(stmt)
 
 
 def reset_config_table():
-    """ Clear the config table and install any default entires needed for the tests.
+    """ Clear the config table and install any default entries needed for the tests.
     """
     db_session = get_session()
     db_session.query(models.Config).delete()
     db_session.commit()
     core_config.set("vo-map", "testvo1", "tst")
     core_config.set("vo-map", "testvo2", "ts2")
```

### Comparing `rucio-34.2.0/lib/rucio/transfertool/__init__.py` & `rucio-34.3.0/lib/rucio/transfertool/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/transfertool/bittorrent.py` & `rucio-34.3.0/lib/rucio/transfertool/bittorrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,33 +10,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import base64
 import logging
-from collections.abc import Sequence
+from collections.abc import Mapping, Sequence
 from os import path
-from typing import TYPE_CHECKING, Any, Mapping, Optional, Type
+from typing import TYPE_CHECKING, Any, Optional
 
 from rucio.common import types
 from rucio.common.config import config_get
+from rucio.common.constants import RseAttr
 from rucio.common.extra import import_extras
 from rucio.common.utils import construct_torrent
 from rucio.core.did_meta_plugins import get_metadata
 from rucio.transfertool.transfertool import TransferStatusReport, Transfertool, TransferToolBuilder
 
 from .bittorrent_driver import BittorrentDriver
 
 if TYPE_CHECKING:
     from rucio.core.request import DirectTransfer
     from rucio.core.rse import RseData
 
 DRIVER_NAME_RSE_ATTRIBUTE = 'bittorrent_driver'
-DRIVER_CLASSES_BY_NAME: dict[str, Type[BittorrentDriver]] = {}
+DRIVER_CLASSES_BY_NAME: dict[str, type[BittorrentDriver]] = {}
 
 EXTRA_MODULES = import_extras(['qbittorrentapi'])
 
 if EXTRA_MODULES['qbittorrentapi']:
     from .bittorrent_driver_qbittorrent import QBittorrentDriver
     DRIVER_CLASSES_BY_NAME[QBittorrentDriver.external_name] = QBittorrentDriver
 
@@ -55,15 +56,15 @@
 
         self._drivers_by_rse_id = {}
         self.ca_cert, self.ca_key = None, None
 
         self.tracker = config_get('transfers', 'bittorrent_tracker_addr', raise_exception=False, default=None)
 
     @classmethod
-    def _pick_management_api_driver_cls(cls: "Type[BittorrentTransfertool]", rse: "RseData") -> Optional[Type[BittorrentDriver]]:
+    def _pick_management_api_driver_cls(cls: "type[BittorrentTransfertool]", rse: "RseData") -> Optional[type[BittorrentDriver]]:
         driver_cls = DRIVER_CLASSES_BY_NAME.get(rse.attributes.get(DRIVER_NAME_RSE_ATTRIBUTE, ''))
         if driver_cls is None:
             return None
         if not all(rse.attributes.get(attribute) is not None for attribute in driver_cls.required_rse_attrs):
             return None
         return driver_cls
 
@@ -86,15 +87,15 @@
         pieces_root = base64.b64decode(meta.get('bittorrent_pieces_root', ''))
         pieces_layers = base64.b64decode(meta.get('bittorrent_pieces_layers', ''))
         piece_length = meta.get('bittorrent_piece_length', 0)
         return pieces_root, pieces_layers, piece_length
 
     @classmethod
     def submission_builder_for_path(
-            cls: "Type[BittorrentTransfertool]",
+            cls: "type[BittorrentTransfertool]",
             transfer_path: "list[DirectTransfer]",
             logger: types.LoggerFunction = logging.log
     ) -> "tuple[list[DirectTransfer], Optional[TransferToolBuilder]]":
         hop = transfer_path[0]
         if hop.rws.byte_count == 0:
             logger(logging.INFO, f"Bittorrent cannot transfer fully empty torrents. Skipping {hop}")
             return [], None
@@ -128,15 +129,15 @@
         for driver in peers_drivers:
             driver.add_peers(torrent_id=torrent_id, peers=peer_addr)
 
     def submit(self, transfers: "Sequence[DirectTransfer]", job_params: dict[str, str], timeout: Optional[int] = None) -> str:
         [transfer] = transfers
         rws = transfer.rws
 
-        tracker = transfer.dst.rse.attributes.get('bittorrent_tracker_addr', self.tracker)
+        tracker = transfer.dst.rse.attributes.get(RseAttr.BITTORRENT_TRACKER_ADDR, self.tracker)
 
         src_drivers = {}
         for source in transfer.sources:
             driver = self._driver_for_rse(source.rse)
             if driver:
                 src_drivers[source] = driver
```

### Comparing `rucio-34.2.0/lib/rucio/transfertool/bittorrent_driver.py` & `rucio-34.3.0/lib/rucio/transfertool/bittorrent_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 from abc import ABCMeta, abstractmethod
 from collections.abc import Sequence
 from typing import TYPE_CHECKING
 
 from rucio.common import types
 
 if TYPE_CHECKING:
-    from typing import Optional, Type
+    from typing import Optional
 
     from rucio.core.rse import RseData
     from rucio.transfertool.transfertool import TransferStatusReport
 
 
 class BittorrentDriver(metaclass=ABCMeta):
     external_name = ''
     required_rse_attrs = tuple()
 
     @classmethod
     @abstractmethod
-    def make_driver(cls: "Type[BittorrentDriver]", rse: "RseData", logger: types.LoggerFunction = logging.log) -> "Optional[BittorrentDriver]":
+    def make_driver(cls: "type[BittorrentDriver]", rse: "RseData", logger: types.LoggerFunction = logging.log) -> "Optional[BittorrentDriver]":
         pass
 
     @abstractmethod
     def listen_addr(self) -> tuple[str, int]:
         pass
 
     @abstractmethod
```

### Comparing `rucio-34.2.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py` & `rucio-34.3.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,23 @@
 from typing import TYPE_CHECKING, Optional, cast
 from urllib.parse import urlparse
 
 import qbittorrentapi
 
 from rucio.common import types
 from rucio.common.config import get_rse_credentials
+from rucio.common.constants import RseAttr
 from rucio.common.utils import resolve_ip
 from rucio.core.oidc import request_token
 from rucio.db.sqla.constants import RequestState
 from rucio.transfertool.transfertool import TransferStatusReport
 
 from .bittorrent_driver import BittorrentDriver
 
 if TYPE_CHECKING:
-    from typing import Type
-
     from sqlalchemy.orm import Session
 
     from rucio.core.rse import RseData
 
 
 class QBittorrentTransferStatusReport(TransferStatusReport):
 
@@ -62,20 +61,20 @@
     def get_monitor_msg_fields(self, session: "Session", logger: types.LoggerFunction = logging.log) -> dict[str, str]:
         return {'protocol': 'qbittorrent'}
 
 
 class QBittorrentDriver(BittorrentDriver):
 
     external_name = 'qbittorrent'
-    required_rse_attrs = ('qbittorrent_management_address', )
+    required_rse_attrs = (RseAttr.QBITTORRENT_MANAGEMENT_ADDRESS, )
 
     @classmethod
-    def make_driver(cls: "Type[QBittorrentDriver]", rse: "RseData", logger: types.LoggerFunction = logging.log) -> "Optional[BittorrentDriver]":
+    def make_driver(cls: "type[QBittorrentDriver]", rse: "RseData", logger: types.LoggerFunction = logging.log) -> "Optional[BittorrentDriver]":
 
-        address = rse.attributes.get('qbittorrent_management_address')
+        address = rse.attributes.get(RseAttr.QBITTORRENT_MANAGEMENT_ADDRESS)
         if not address:
             return None
 
         url = urlparse(address)
         token = None
         if url.scheme.lower() == 'https':
             token = request_token(audience=url.hostname, scope='qbittorrent_admin')
```

### Comparing `rucio-34.2.0/lib/rucio/transfertool/fts3.py` & `rucio-34.3.0/lib/rucio/transfertool/fts3.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import requests
 from dogpile.cache.api import NoValue
 from requests.adapters import ReadTimeout
 from requests.packages.urllib3 import disable_warnings  # pylint: disable=import-error
 
 from rucio.common.cache import make_region_memcached
 from rucio.common.config import config_get, config_get_bool, config_get_int, config_get_list
-from rucio.common.constants import FTS_COMPLETE_STATE, FTS_JOB_TYPE, FTS_STATE
+from rucio.common.constants import FTS_COMPLETE_STATE, FTS_JOB_TYPE, FTS_STATE, RseAttr
 from rucio.common.exception import DuplicateFileTransferSubmission, TransferToolTimeout, TransferToolWrongAnswer
 from rucio.common.stopwatch import Stopwatch
 from rucio.common.utils import PREFERRED_CHECKSUM, APIEncoder, chunks, deep_merge_dict
 from rucio.core.monitor import MetricManager
 from rucio.core.oidc import request_token
 from rucio.core.request import get_source_rse, get_transfer_error
 from rucio.core.rse import determine_audience_for_rse, determine_scope_for_rse, get_rse_supported_checksums_from_attributes
@@ -200,21 +200,21 @@
 def _available_checksums(
         transfer: "DirectTransfer",
 ) -> tuple[set[str], set[str]]:
     """
     Get checksums which can be used for file validation on the source and the destination RSE
     """
     src_attributes = transfer.src.rse.attributes
-    if src_attributes.get('verify_checksum', True):
+    if src_attributes.get(RseAttr.VERIFY_CHECKSUM, True):
         src_checksums = set(get_rse_supported_checksums_from_attributes(src_attributes))
     else:
         src_checksums = set()
 
     dst_attributes = transfer.dst.rse.attributes
-    if dst_attributes.get('verify_checksum', True):
+    if dst_attributes.get(RseAttr.VERIFY_CHECKSUM, True):
         dst_checksums = set(get_rse_supported_checksums_from_attributes(dst_attributes))
     else:
         dst_checksums = set()
 
     return src_checksums, dst_checksums
 
 
@@ -299,15 +299,15 @@
 def _use_tokens(transfer_hop: "DirectTransfer"):
     """Whether a transfer can be performed with tokens.
 
     In order to be so, all the involved RSEs must have it explicitly enabled
     and the protocol being used must be WebDAV.
     """
     for endpoint in [*transfer_hop.sources, transfer_hop.dst]:
-        if (endpoint.rse.attributes.get('oidc_support') is not True
+        if (endpoint.rse.attributes.get(RseAttr.OIDC_SUPPORT) is not True
                 or endpoint.scheme != 'davs'):
             return False
     return True
 
 
 def build_job_params(
         transfer_path: list["DirectTransfer"],
@@ -335,16 +335,16 @@
     # Get dest space token
     dest_protocol = last_hop.protocol_factory.protocol(last_hop.dst.rse, last_hop.dst.scheme, last_hop.operation_dest)
     dest_spacetoken = None
     if dest_protocol.attributes and 'extended_attributes' in dest_protocol.attributes and \
             dest_protocol.attributes['extended_attributes'] and 'space_token' in dest_protocol.attributes['extended_attributes']:
         dest_spacetoken = dest_protocol.attributes['extended_attributes']['space_token']
 
-    strict_copy = last_hop.dst.rse.attributes.get('strict_copy', False)
-    archive_timeout = last_hop.dst.rse.attributes.get('archive_timeout', None)
+    strict_copy = last_hop.dst.rse.attributes.get(RseAttr.STRICT_COPY, False)
+    archive_timeout = last_hop.dst.rse.attributes.get(RseAttr.ARCHIVE_TIMEOUT, None)
 
     job_params = {'account': last_hop.rws.account,
                   'verify_checksum': _path_checksum_validation_strategy(transfer_path, logger=logger),
                   'copy_pin_lifetime': last_hop.rws.attributes.get('lifetime', default_lifetime),
                   'bring_online': bring_online_local,
                   'job_metadata': {
                       'issuer': 'rucio',
@@ -358,25 +358,25 @@
         job_params['job_metadata']['multihop'] = True
     elif len(last_hop.sources) > 1:
         job_params['job_metadata']['multi_sources'] = True
     if strict_copy:
         job_params['strict_copy'] = strict_copy
     if dest_spacetoken:
         job_params['spacetoken'] = dest_spacetoken
-    if (last_hop.dst.rse.attributes.get('use_ipv4', False)
-            or any(src.rse.attributes.get('use_ipv4', False) for src in last_hop.sources)):
+    if (last_hop.dst.rse.attributes.get(RseAttr.USE_IPV4, False)
+            or any(src.rse.attributes.get(RseAttr.USE_IPV4, False) for src in last_hop.sources)):
         job_params['ipv4'] = True
         job_params['ipv6'] = False
 
     # assume s3alternate True (path-style URL S3 RSEs)
     job_params['s3alternate'] = True
-    src_rse_s3_url_style = first_hop.src.rse.attributes.get('s3_url_style', None)
+    src_rse_s3_url_style = first_hop.src.rse.attributes.get(RseAttr.S3_URL_STYLE, None)
     if src_rse_s3_url_style == "host":
         job_params['s3alternate'] = False
-    dst_rse_s3_url_style = last_hop.dst.rse.attributes.get('s3_url_style', None)
+    dst_rse_s3_url_style = last_hop.dst.rse.attributes.get(RseAttr.S3_URL_STYLE, None)
     if dst_rse_s3_url_style == "host":
         job_params['s3alternate'] = False
 
     if archive_timeout and last_hop.dst.rse.is_tape():
         try:
             archive_timeout = int(archive_timeout)
             if archive_timeout_override is None:
@@ -415,15 +415,15 @@
         source_strategy: Optional[str] = None,
         max_time_in_queue: Optional[dict] = None,
         logger: Callable = logging.log,
         archive_timeout_override: Optional[int] = None,
         bring_online: Optional[int] = None,
         default_lifetime: Optional[int] = None) -> list[dict[str, Any]]:
     """
-    Group transfers in bulk based on certain criterias
+    Group transfers in bulk based on certain criteria
 
     :param transfer_paths:           List of transfer paths to group. Each path is a list of single-hop transfers.
     :param policy:                   Policy to use to group.
     :param group_bulk:               Bulk sizes.
     :param source_strategy:          Strategy to group sources
     :param max_time_in_queue:        Maximum time in queue
     :param archive_timeout_override: Override the archive_timeout parameter for any transfers with it set (0 to unset)
@@ -518,15 +518,15 @@
         self._multi_sources = None
         self._src_url = None
         self._dst_url = None
         # Initialized in child class initialize():
         self._reason = None
         self._src_rse = None
         self._fts_address = self.external_host
-        # Supported db fields bellow:
+        # Supported db fields below:
         self.state = None
         self.external_id = None
         self.started_at = None
         self.transferred_at = None
         self.staging_started_at = None
         self.staging_finished_at = None
         self.source_rse_id = None
@@ -801,15 +801,15 @@
 
 class FTS3Transfertool(Transfertool):
     """
     FTS3 implementation of a Rucio transfertool
     """
 
     external_name = 'fts3'
-    required_rse_attrs = ('fts', )
+    required_rse_attrs = (RseAttr.FTS, )
     supported_schemes = Transfertool.supported_schemes.union(('mock', ))
 
     def __init__(self, external_host, oidc_account=None, oidc_support: bool = False, vo=None, group_bulk=1, group_policy='rule', source_strategy=None,
                  max_time_in_queue=None, bring_online=43200, default_lifetime=172800, archive_timeout_override=None,
                  logger=logging.log):
         """
         Initializes the transfertool
@@ -857,21 +857,21 @@
         self.scitags_exp_id, self.scitags_activity_ids = _scitags_ids(logger=logger)
 
     @classmethod
     def _pick_fts_servers(cls, source_rse: "RseData", dest_rse: "RseData"):
         """
         Pick fts servers to use for submission between the two given rse
         """
-        source_servers = source_rse.attributes.get('fts', None)
-        dest_servers = dest_rse.attributes.get('fts', None)
+        source_servers = source_rse.attributes.get(RseAttr.FTS, None)
+        dest_servers = dest_rse.attributes.get(RseAttr.FTS, None)
         if source_servers is None or dest_servers is None:
             return None
 
         servers_to_use = dest_servers
-        if source_rse.attributes.get('sign_url', None) == 'gcs':
+        if source_rse.attributes.get(RseAttr.SIGN_URL, None) == 'gcs':
             servers_to_use = source_servers
 
         return servers_to_use.split(',')
 
     @classmethod
     def can_perform_transfer(cls, source_rse: "RseData", dest_rse: "RseData"):
         if cls._pick_fts_servers(source_rse, dest_rse):
@@ -1229,15 +1229,15 @@
 
         return responses
 
     def list_se_status(self):
         """
         Get the list of banned Storage Elements.
 
-        :returns: Detailed dictionnary of banned Storage Elements.
+        :returns: Detailed dictionary of banned Storage Elements.
         """
 
         try:
             result = requests.get('%s/ban/se' % self.external_host,
                                   verify=self.verify,
                                   cert=self.cert,
                                   headers=self.headers,
@@ -1455,15 +1455,15 @@
             if job_response['http_status'] == '200 Ok':
                 files_response = job_response['files']
                 multi_sources = job_response['job_metadata'].get('multi_sources', False)
                 if multi_sources and job_response['job_state'] not in [FTS_STATE.FAILED,
                                                                        FTS_STATE.FINISHEDDIRTY,
                                                                        FTS_STATE.CANCELED,
                                                                        FTS_STATE.FINISHED]:
-                    # multipe source replicas jobs is still running. should wait
+                    # multiple source replicas jobs is still running. should wait
                     responses[transfer_id] = {}
                     continue
 
                 resps = {}
                 for file_resp in files_response:
                     file_state = file_resp['file_state']
                     # for multiple source replicas jobs, the file_metadata(request_id) will be the same.
```

### Comparing `rucio-34.2.0/lib/rucio/transfertool/fts3_plugins.py` & `rucio-34.3.0/lib/rucio/transfertool/fts3_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import logging
 import sys
+from collections.abc import Callable
 from configparser import NoSectionError
-from typing import Any, Callable, Optional, Type, TypeVar
+from typing import Any, Optional, TypeVar
 
 from rucio.common.config import config_get_int, config_get_items
 from rucio.common.exception import InvalidRequest
 from rucio.common.plugins import PolicyPackageAlgorithms
 
 FTS3TapeMetadataPluginType = TypeVar('FTS3TapeMetadataPluginType', bound='FTS3TapeMetadataPlugin')
 
@@ -33,15 +34,15 @@
 
     ALGORITHM_NAME = "fts3_tape_metadata_plugins"
     _HINTS_NAME = "fts3_plugins_init"
     DEFAULT = "def"
 
     def __init__(self, policy_algorithm: str) -> None:
         """
-        :param policy_algorithm: policy algorithm indentifier - choose from any of the policy package algorithms registered under the `fts3_tape_metadata_plugins` group.
+        :param policy_algorithm: policy algorithm identifier - choose from any of the policy package algorithms registered under the `fts3_tape_metadata_plugins` group.
         """
         super().__init__()
         self.transfer_limit = config_get_int(
             "transfers",
             option="metadata_byte_limit",
             raise_exception=False,
             default=4096,
@@ -55,24 +56,24 @@
         # If the policy has a supplied and registered init function
         if self._supports(self._HINTS_NAME, policy_algorithm):
             self._get_one_algorithm(self._HINTS_NAME, name=policy_algorithm)()
 
         self.set_in_hints = self._get_one_algorithm(self.ALGORITHM_NAME, name=policy_algorithm)
 
     @classmethod
-    def _module_init(cls: Type[FTS3TapeMetadataPluginType]) -> None:
+    def _module_init(cls: type[FTS3TapeMetadataPluginType]) -> None:
         cls.register(
             "activity",
             func=lambda x: cls._activity_hints(cls, x),  # type: ignore
             init_func=lambda: cls._init_instance_activity_hints(cls))  # type: ignore
         cls.register(cls.DEFAULT, func=lambda x: cls._collocation(cls, cls._default, x))  # type: ignore
         cls.register("test", func=lambda x: cls._collocation(cls, cls._test_collocation, x))  # type: ignore
 
     @classmethod
-    def register(cls: Type[FTS3TapeMetadataPluginType], name: str, func: Callable, init_func: Optional[Callable] = None) -> None:
+    def register(cls: type[FTS3TapeMetadataPluginType], name: str, func: Callable, init_func: Optional[Callable] = None) -> None:
         """
         Register a fts3 transfer plugin
 
         :param name: name to register under
         :param func: function called by the plugin
         :param init_func: Initialization requirements for the plugin, defaults to None
         """
```

### Comparing `rucio-34.2.0/lib/rucio/transfertool/globus.py` & `rucio-34.3.0/lib/rucio/transfertool/globus.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 
+from rucio.common.constants import RseAttr
 from rucio.common.utils import chunks
 from rucio.db.sqla.constants import RequestState
 from rucio.transfertool.transfertool import TransferStatusReport, Transfertool, TransferToolBuilder
 
 from .globus_library import bulk_check_xfers, bulk_submit_xfer, submit_xfer
 
 
 def bulk_group_transfers(transfer_paths, policy='single', group_bulk=200):
     """
-    Group transfers in bulk based on certain criterias
+    Group transfers in bulk based on certain criteria
 
     :param transfer_paths:  List of (potentially multihop) transfer paths to group. Each path is a list of single-hop transfers.
     :param policy:          Policy to use to group.
     :param group_bulk:      Bulk sizes.
     :return:                List of transfer groups
     """
     if policy == 'single':
@@ -78,15 +79,15 @@
 
 class GlobusTransferTool(Transfertool):
     """
     Globus implementation of Transfertool abstract base class
     """
 
     external_name = 'globus'
-    required_rse_attrs = ('globus_endpoint_id', )
+    required_rse_attrs = (RseAttr.GLOBUS_ENDPOINT_ID, )
 
     def __init__(self, external_host, logger=logging.log, group_bulk=200, group_policy='single'):
         """
         Initializes the transfertool
 
         :param external_host:   The external host where the transfertool API is running
         """
@@ -157,16 +158,16 @@
                 'sources': [transfer.source_url(s) for s in transfer.sources],
                 'destinations': [transfer.dest_url],
                 'metadata': {
                     'src_rse': transfer.src.rse.name,
                     'dst_rse': transfer.dst.rse.name,
                     'scope': str(transfer.rws.scope),
                     'name': transfer.rws.name,
-                    'source_globus_endpoint_id': transfer.src.rse.attributes['globus_endpoint_id'],
-                    'dest_globus_endpoint_id': transfer.dst.rse.attributes['globus_endpoint_id'],
+                    'source_globus_endpoint_id': transfer.src.rse.attributes[RseAttr.GLOBUS_ENDPOINT_ID],
+                    'dest_globus_endpoint_id': transfer.dst.rse.attributes[RseAttr.GLOBUS_ENDPOINT_ID],
                     'filesize': transfer.rws.byte_count,
                 },
             }
             for transfer in transfers
         ]
         self.logger(logging.DEBUG, '... Starting globus xfer ...')
         self.logger(logging.DEBUG, 'job_files: %s' % submitjob)
```

### Comparing `rucio-34.2.0/lib/rucio/transfertool/globus_library.py` & `rucio-34.3.0/lib/rucio/transfertool/globus_library.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/transfertool/mock.py` & `rucio-34.3.0/lib/rucio/transfertool/mock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/transfertool/transfertool.py` & `rucio-34.3.0/lib/rucio/transfertool/transfertool.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     ]
 
     def __init__(self, request_id, request=None):
         self.request_id = request_id
         self.__request = request  # Optional: DB request. If provided, saves us a database call to fetch it by request_id
         self.__initialized = False
 
-        # Supported db fields bellow
+        # Supported db fields below
         self.state = None
 
     @abstractmethod
     def initialize(self, session, logger=logging.log):
         """
         Initialize all fields from self.supported_update_fields
         """
```

### Comparing `rucio-34.2.0/lib/rucio/version.py` & `rucio-34.3.0/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/__init__.py` & `rucio-34.3.0/lib/rucio/web/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/__init__.py` & `rucio-34.3.0/lib/rucio/web/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/__init__.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/__init__.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from rucio.web.rest.flaskapi.v1.common import ErrorHandlingMethodView, generate_http_error_flask, json_parameters, param_get, response_headers
 
 
 class LocalAccountLimit(ErrorHandlingMethodView):
     def post(self, account, rse):
         """
         ---
-        summary: Create or update a local accont limit
+        summary: Create or update a local account limit
         tags:
           - Account Limit
         parameters:
         - name: account
           in: path
           description: The account for the accountlimit.
           schema:
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/accounts.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,16 +566,16 @@
 
 
 class GlobalAccountLimits(ErrorHandlingMethodView):
     @check_accept_header_wrapper_flask(['application/json'])
     def get(self, account, rse_expression=None):
         """
         ---
-        summary: Get gloabl limit
-        description: Get the current gloabl limits for an account on a specific RSE expression.
+        summary: Get global limit
+        description: Get the current global limits for an account on a specific RSE expression.
         tags:
           - Account
         parameters:
         - name: account
           in: path
           description: The account identifier.
           schema:
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/archives.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/archives.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/auth.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/auth.py`

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
 import json
 import logging
 import time
 from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 
 from flask import Blueprint, Flask, Response, redirect, render_template, request
@@ -1211,26 +1210,14 @@
 
         vo = extract_vo(request.headers)
         account = request.headers.get('X-Rucio-Account', default=None)
         signature = request.headers.get('X-Rucio-SSH-Signature', default=None)
         appid = request.headers.get('X-Rucio-AppID', default='unknown')
         ip = request.headers.get('X-Forwarded-For', default=request.remote_addr)
 
-        # decode the signature which must come in base64 encoded
-        try:
-            signature += '=' * ((4 - len(signature) % 4) % 4)  # adding required padding
-            signature = base64.b64decode(signature)
-        except TypeError:
-            return generate_http_error_flask(
-                status_code=401,
-                exc=CannotAuthenticate.__name__,
-                exc_msg=f'Cannot authenticate to account {account} with malformed signature',
-                headers=headers
-            )
-
         try:
             result = get_auth_token_ssh(account, signature, appid, ip, vo=vo)
         except AccessDenied:
             return generate_http_error_flask(
                 status_code=401,
                 exc=CannotAuthenticate.__name__,
                 exc_msg=f'Cannot authenticate to account {account} with given credentials',
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/common.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                 )
             else:
                 msg = f'DatabaseException in {self.__class__.__module__} {self.__class__.__name__} {flask.request.method}'
                 logging.debug(msg, exc_info=True)
                 return generate_http_error_flask(
                     status_code=500,
                     exc=error.__class__.__name__,
-                    exc_msg='An unknown Database Exception has ocurred.',
+                    exc_msg='An unknown Database Exception has occurred.',
                     headers=headers
                 )
 
         except RucioException as error:
             # should be caught in the flask view and generate_http_error_flask with a proper HTTP status code returned
             msg = f'Uncaught RucioException in {self.__class__.__module__} {self.__class__.__name__} {flask.request.method}'
             # logged, because this should be the __exception__
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/config.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/credentials.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,30 +56,30 @@
               Access-Control-Allow-Origin:
                 schema:
                   type: string
                 description: The http origin.
               Access-Control-Allow-Headers:
                 schema:
                   type: string
-                description: The http access controll request headers.
+                description: The http access control request headers.
               Access-Control-Allow-Methods:
                 schema:
                   type: string
                   enum: ['*']
                 description: The allowed methods.
               Access-Control-Allow-Credentials:
                 schema:
                   type: string
                   enum: ['true']
                 description: If credentials are allowed.
               Access-Control-Expose-Headers:
                 schema:
                   type: string
                   enum: ['X-Rucio-Auth-Token']
-                description: The exposed access controll header.
+                description: The exposed access control header.
           404:
             description: Not found
         """
         return '', 200, self.get_headers()
 
     @check_accept_header_wrapper_flask(['application/octet-stream'])
     def get(self):
@@ -112,15 +112,15 @@
           in: query
           description: The operation.
           schema:
             type: string
           required: false
         - name: url
           in: query
-          description: The Url of the authentification.
+          description: The Url of the authentication.
           schema:
             type: string
           required: true
         requestBody:
           content:
             'application/octet-stream':
               schema:
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/dids.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/dids.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                     type: boolean
         responses:
           200:
             description: OK
             content:
               application/x-json-stream:
                 schema:
-                  description: Line seperated dictionary of dids.
+                  description: Line separated dictionary of dids.
                   type: array
                   items:
                     type: object
                     description: Data identifier
                     properties:
                       scope:
                         type: string
@@ -255,15 +255,15 @@
           409:
             description: Wrong did type
         """
         filters = request.args.get('filters', default=None)
         if filters is not None:
             filters = ast.literal_eval(filters)
         else:
-            # backwards compatability for created*, length* and name filters passed through as request args
+            # backwards compatibility for created*, length* and name filters passed through as request args
             filters = {}
             for arg, value in request.args.copy().items():
                 if arg not in ['type', 'limit', 'long', 'recursive']:
                     filters[arg] = value
             filters = [filters]
 
         did_type = request.args.get('type', default=None)
@@ -777,15 +777,15 @@
           style: simple
         responses:
           200:
             description: Did found
             content:
               application/x-json-stream:
                 schema:
-                  description: The contents of a did. Items are line seperated.
+                  description: The contents of a did. Items are line separated.
                   type: array
                   items:
                     type: object
                     required:
                       - scope
                       - name
                       - type
@@ -990,15 +990,15 @@
           style: simple
         responses:
           200:
             description: Did found
             content:
               application/x-json-stream:
                 schema:
-                  description: The dids with their information and history. Elements are seperated by new line characters.
+                  description: The dids with their information and history. Elements are separated by new line characters.
                   type: array
                   items:
                     type: object
                     description: A single did with history data.
                     properties:
                       scope:
                         description: The scope of the did.
@@ -1098,15 +1098,15 @@
                           events:
                             description: The number of events of the did.
                             type: integer
                           adler32:
                             description: The adler32 checksum.
                             type: string
                           lumiblocknr:
-                            description: The lumi block nr. Only availabe if `long` is defined in the query.
+                            description: The lumi block nr. Only available if `long` is defined in the query.
                             type: integer
                     - description: All replica information.
                       type: array
                       items:
                         type: object
                         properties:
                           scope:
@@ -1314,15 +1314,15 @@
             default: DID_COLUMN
         responses:
           200:
             description: OK
             content:
               application/json:
                 schema:
-                  description: A data identifer with all attributes.
+                  description: A data identifier with all attributes.
                   type: object
           401:
             description: Invalid Auth Token
           404:
             description: Did not found
           406:
             description: Not acceptable
@@ -1358,15 +1358,15 @@
             'application/json':
               schema:
                 type: object
                 required:
                 - meta
                 properties:
                   meta:
-                    description: The metadata to add. A dictionary containg the metadata name as key and the value as value.
+                    description: The metadata to add. A dictionary containing the metadata name as key and the value as value.
                     type: object
                   recursive:
                     description: Flag if the metadata should be applied recirsively to children.
                     type: boolean
                     default: false
         responses:
           201:
@@ -1505,15 +1505,15 @@
           401:
             description: Invalid Auth Token
           404:
             description: Did not found
           406:
             description: Not acceptable
           409:
-            description: Matadata already exists
+            description: Metadata already exists
           400:
             description: Invalid key or value
         """
         try:
             scope, name = parse_scope_name(scope_name, request.environ.get('vo'))
         except ValueError as error:
             return generate_http_error_flask(400, error)
@@ -1695,15 +1695,15 @@
                     default: false
         responses:
           200:
             description: OK
             content:
               application/json:
                 schema:
-                  description: A list of metadata identifiers for the dids. Seperated by new lines.
+                  description: A list of metadata identifiers for the dids. Separated by new lines.
                   type: array
                   items:
                     description: The metadata for one did.
                     type: object
           400:
             description: Cannot decode json parameter list
           401:
@@ -1731,15 +1731,15 @@
 
 class AssociatedRules(ErrorHandlingMethodView):
 
     @check_accept_header_wrapper_flask(['application/x-json-stream'])
     def get(self, scope_name):
         """
         ---
-        summary: Get accociated rules
+        summary: Get associated rules
         description: Gets all associated rules for a file.
         tags:
           - Data Identifiers
         parameters:
         - name: scope_name
           in: path
           description: The scope and the name of the did.
@@ -1748,15 +1748,15 @@
           style: simple
         responses:
           200:
             description: OK
             content:
               application/x-json-stream:
                 schema:
-                  description: All associated rules for a file. Items are seperated by new line character.
+                  description: All associated rules for a file. Items are separated by new line character.
                   type: array
                   items:
                     description: A replication rule associated with the file. Has more fields than listed here.
                     type: object
                     properties:
                       id:
                         description: The id of the rule.
@@ -1819,15 +1819,15 @@
           style: simple
         responses:
           200:
             description: OK
             content:
               application/x-json-stream:
                 schema:
-                  description: A list of all datasets associated with the guid. Items are seperated by new line character.
+                  description: A list of all datasets associated with the guid. Items are separated by new line character.
                   type: array
                   items:
                     description: A dataset associated with a guid.
                     type: object
                     properties:
                       scope:
                         description: The scope of the dataset.
@@ -2023,15 +2023,15 @@
           required: false
         responses:
           200:
             description: OK
             content:
               application/x-json-stream:
                 schema:
-                  description: A list of the recent dids. Items are seperated by new line characters.
+                  description: A list of the recent dids. Items are separated by new line characters.
                   type: array
                   items:
                     description: A did.
                     type: object
                     properties:
                       scope:
                         description: The scope of the did.
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/dirac.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/export.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/export.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/identities.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/identities.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/import.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/import.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                         account:
                           description: The account identifier.
                           type: string
                         email:
                           description: The email of an account.
                           type: string
                         identities:
-                          description: The identiies accociated with an account. Deletes old identites and adds the newly defined ones.
+                          description: The identities associated with an account. Deletes old identities and adds the newly defined ones.
                           type: array
                           items:
                             description: One identity associated with an account.
                             type: object
                             properties:
                               type:
                                 description: The type of the identity.
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,18 +56,18 @@
                         description: The name of the lifetime exception.
                         type: string
                       did_type:
                         description: The type of the did.
                         type: string
                         enum: ['F', 'D', 'C', 'A', 'X', 'Y', 'Z']
                       account:
-                        description: The account accociated with the lifetime exception.
+                        description: The account associated with the lifetime exception.
                         type: string
                       pattern:
-                        description: The patter of the lifetime exception.
+                        description: The pattern of the lifetime exception.
                         type: string
                       comments:
                         description: The comments of the lifetime exception.
                         type: string
                       state:
                         description: The state of the lifetime exception.
                         type: string
@@ -204,15 +204,15 @@
                         description: The type of the did.
                         type: string
                         enum: ['F', 'D', 'C', 'A', 'X', 'Y', 'Z']
                       account:
                         description: The account associated with the lifetime exception.
                         type: string
                       pattern:
-                        description: The patter of the lifetime exception.
+                        description: The pattern of the lifetime exception.
                         type: string
                       comments:
                         description: The comments of the lifetime exception.
                         type: string
                       state:
                         description: The state of the lifetime exception.
                         type: string
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/locks.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/locks.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/main.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ]
 
 
 def apply_endpoints(app, modules):
     for blueprint_module in modules:
         # Legacy patch - TODO Remove in 38.0.0
         if blueprint_module == "meta":
-            logging.log(logging.WARNING, "Endpoint `meta` is depreciated and will be removed in future releaases")
+            logging.log(logging.WARNING, "Endpoint `meta` is depreciated and will be removed in future releases")
             blueprint_module = "meta_conventions"
         try:
             # searches for module names locally
             blueprint_module = importlib.import_module('.' + blueprint_module,
                                                        package='rucio.web.rest.flaskapi.v1')
         except ImportError:
             raise ConfigurationError(f'Could not load "{blueprint_module}" provided in the endpoints configuration value')
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         responses:
           200:
             description: OK
             content:
               application/json:
                 schema:
                   type: array
-                  descripton: List of all DID keys.
+                  description: List of all DID keys.
                   items:
                     type: string
                     description: Data Itentifier key
           401:
             description: Invalid Auth Token
           406:
             description: Not acceptable
@@ -65,15 +65,15 @@
         requestBody:
           content:
             application/json:
               schema:
                 type: object
                 properties:
                   key_type:
-                    description: The key tpye.
+                    description: The key type.
                     type: string
                   value_type:
                     description: The value type.
                     type: string
                   value_regexp:
                     description: The value regexpression.
                     type: string
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/metrics.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/ping.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/ping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/redirect.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/replicas.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/replicas.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,15 @@
                         state:
                           description: The pfn of the replica.
                           type: string
                         path:
                           description: The pfn of the replica.
                           type: string
                         error_message:
-                          description: The error message if an error occured.
+                          description: The error message if an error occurred.
                           type: string
                         broken_rule_id:
                           description: The id of the broken rule if one was found.
                           type: string
                         broken_message:
                           description: The message of the broken rule.
                           type: string
@@ -1122,26 +1122,26 @@
                   description: A list of all result replicas.
                   type: array
                   items:
                     oneOf:
                       - type: object
                         properties:
                           scope:
-                            description: The scope fo the replica.
+                            description: The scope of the replica.
                             type: string
                           name:
                             description: The name of the replica.
                             type: string
                           type:
                             description: The type of the replica.
                             type: string
                       - type: object
                         properties:
                           scope:
-                            description: The scope fo the replica.
+                            description: The scope of the replica.
                             type: string
                           name:
                             description: The name of the replica.
                             type: string
                           rse:
                             description: The name of the associated rse.
                             type: string
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/requests.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 from rucio.common.utils import APIEncoder, render_json
 from rucio.core.rse import get_rses_with_attribute_value
 from rucio.db.sqla.constants import RequestState
 from rucio.web.rest.flaskapi.authenticated_bp import AuthenticatedBlueprint
 from rucio.web.rest.flaskapi.v1.common import ErrorHandlingMethodView, check_accept_header_wrapper_flask, generate_http_error_flask, parse_scope_name, response_headers, try_stream
 
 if TYPE_CHECKING:
-    from typing import Iterator
+    from collections.abc import Iterator
 
 
 class RequestGet(ErrorHandlingMethodView):
     """ REST API to get requests. """
 
     @check_accept_header_wrapper_flask(['application/json'])
     def get(self, scope_name, rse):
         """
         ---
         summary: Get Request
-        description: Get a request for a given DID to a destinaion RSE.
+        description: Get a request for a given DID to a destination RSE.
         tags:
           - Requests
         parameters:
         - name: scope_name
           in: path
           description: Data identifier (scope)/(name).
           schema:
@@ -98,15 +98,15 @@
                     external_host:
                       description: External host of the request.
                       type: string
                     retry_count:
                       description: The numbers of attempted retires.
                       type: integer
                     err_msg:
-                      description: An error message if one occured.
+                      description: An error message if one occurred.
                       type: string
                     previous_attempt_id:
                       description: The id of the previous attempt.
                       type: string
                     rule_id:
                       description: The id of the associated replication rule.
                       type: string
@@ -128,27 +128,27 @@
                     submitted_at:
                       description: The time the request got submitted.
                       type: string
                     started_at:
                       description: The time the request got started.
                       type: string
                     transferred_at:
-                      description: The time the request got transfered.
+                      description: The time the request got transferred.
                       type: string
                     estimated_at:
                       description: The time the request got estimated.
                       type: string
                     submitter_id:
                       description: The id of the submitter.
                       type: string
                     estimated_stated_at:
                       description: The estimation of the started at value.
                       type: string
                     estimated_transferred_at:
-                      description: The estimation of the transfered at value.
+                      description: The estimation of the transferred at value.
                       type: string
                     staging_started_at:
                       description: The time the staging got started.
                       type: string
                     staging_finished_at:
                       description: The time the staging got finished.
                       type: string
@@ -199,15 +199,15 @@
     """ REST API to get historical requests. """
 
     @check_accept_header_wrapper_flask(['application/json'])
     def get(self, scope_name, rse):
         """
         ---
         summary: Get Historical Request
-        description: List a hostorical request for a given DID to a destination RSE.
+        description: List a historical request for a given DID to a destination RSE.
         tags:
           - Requests
         parameters:
         - name: scope_name
           in: path
           description: Data identifier (scope)/(name).
           schema:
@@ -263,15 +263,15 @@
                     external_host:
                       description: External host of the request.
                       type: string
                     retry_count:
                       description: The numbers of attempted retires.
                       type: integer
                     err_msg:
-                      description: An error message if one occured.
+                      description: An error message if one occurred.
                       type: string
                     previous_attempt_id:
                       description: The id of the previous attempt.
                       type: string
                     rule_id:
                       description: The id of the associated replication rule.
                       type: string
@@ -293,27 +293,27 @@
                     submitted_at:
                       description: The time the request got submitted.
                       type: string
                     started_at:
                       description: The time the request got started.
                       type: string
                     transferred_at:
-                      description: The time the request got transfered.
+                      description: The time the request got transferred.
                       type: string
                     estimated_at:
                       description: The time the request got estimated.
                       type: string
                     submitter_id:
                       description: The id of the submitter.
                       type: string
                     estimated_stated_at:
                       description: The estimation of the started at value.
                       type: string
                     estimated_transferred_at:
-                      description: The estimation of the transfered at value.
+                      description: The estimation of the transferred at value.
                       type: string
                     staging_started_at:
                       description: The time the staging got started.
                       type: string
                     staging_finished_at:
                       description: The time the staging got finished.
                       type: string
@@ -415,15 +415,15 @@
             type: string
         responses:
           200:
             description: OK
             content:
               application/x-json-stream:
                 schema:
-                  description: All requests matching the arguments. Seperated by the new line character.
+                  description: All requests matching the arguments. Separated by the new line character.
                   type: array
                   items:
                     description: A request.
                     type: object
                     properties:
                       id:
                         description: The id of the request.
@@ -460,15 +460,15 @@
                       external_host:
                         description: External host of the request.
                         type: string
                       retry_count:
                         description: The numbers of attempted retires.
                         type: integer
                       err_msg:
-                        description: An error message if one occured.
+                        description: An error message if one occurred.
                         type: string
                       previous_attempt_id:
                         description: The id of the previous attempt.
                         type: string
                       rule_id:
                         description: The id of the associated replication rule.
                         type: string
@@ -490,27 +490,27 @@
                       submitted_at:
                         description: The time the request got submitted.
                         type: string
                       started_at:
                         description: The time the request got started.
                         type: string
                       transferred_at:
-                        description: The time the request got transfered.
+                        description: The time the request got transferred.
                         type: string
                       estimated_at:
                         description: The time the request got estimated.
                         type: string
                       submitter_id:
                         description: The id of the submitter.
                         type: string
                       estimated_stated_at:
                         description: The estimation of the started at value.
                         type: string
                       estimated_transferred_at:
-                        description: The estimation of the transfered at value.
+                        description: The estimation of the transferred at value.
                         type: string
                       staging_started_at:
                         description: The time the staging got started.
                         type: string
                       staging_finished_at:
                         description: The time the staging got finished.
                         type: string
@@ -650,15 +650,15 @@
             default: 100
         responses:
           200:
             description: OK
             content:
               application/x-json-stream:
                 schema:
-                  description: All requests matching the arguments. Seperated by a new line character.
+                  description: All requests matching the arguments. Separated by a new line character.
                   type: array
                   items:
                     description: A request.
                     type: object
                     properties:
                       id:
                         description: The id of the request.
@@ -695,15 +695,15 @@
                       external_host:
                         description: External host of the request.
                         type: string
                       retry_count:
                         description: The numbers of attempted retires.
                         type: integer
                       err_msg:
-                        description: An error message if one occured.
+                        description: An error message if one occurred.
                         type: string
                       previous_attempt_id:
                         description: The id of the previous attempt.
                         type: string
                       rule_id:
                         description: The id of the associated replication rule.
                         type: string
@@ -725,27 +725,27 @@
                       submitted_at:
                         description: The time the request got submitted.
                         type: string
                       started_at:
                         description: The time the request got started.
                         type: string
                       transferred_at:
-                        description: The time the request got transfered.
+                        description: The time the request got transferred.
                         type: string
                       estimated_at:
                         description: The time the request got estimated.
                         type: string
                       submitter_id:
                         description: The id of the submitter.
                         type: string
                       estimated_stated_at:
                         description: The estimation of the started at value.
                         type: string
                       estimated_transferred_at:
-                        description: The estimation of the transfered at value.
+                        description: The estimation of the transferred at value.
                         type: string
                       staging_started_at:
                         description: The time the staging got started.
                         type: string
                       staging_finished_at:
                         description: The time the staging got finished.
                         type: string
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/rses.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/rses.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,16 +236,16 @@
                   ISP:
                     description: The internet service provider of the RSE.
                     type: string
                   rse_type:
                     description: The rse type.
                     type: string
                     enum: ["DISK", "TAPE"]
-                  latitute:
-                    description: The latitute of the RSE.
+                  latitude:
+                    description: The latitude of the RSE.
                     type: number
                   longitude:
                     description: The longitude of the RSE.
                     type: number
                   ASN:
                     description: The access service network of the RSE.
                     type: string
@@ -377,16 +377,16 @@
                   time_zone:
                     description: The time zone of the RSE.
                     type: string
                   rse_type:
                     description: The rse type.
                     type: string
                     enum: ["DISK", "TAPE"]
-                  latitute:
-                    description: The latitute of the RSE.
+                  latitude:
+                    description: The latitude of the RSE.
                     type: number
                   longitude:
                     description: The longitude of the RSE.
                     type: number
         responses:
           201:
             description: OK
@@ -471,16 +471,16 @@
                     ISP:
                       description: The internet service provider of the RSE.
                       type: string
                     rse_type:
                       description: The rse type.
                       type: string
                       enum: ["DISK", "TAPE"]
-                    latitute:
-                      description: The latitute of the RSE.
+                    latitude:
+                      description: The latitude of the RSE.
                       type: number
                     longitude:
                       description: The longitude of the RSE.
                       type: number
                     ASN:
                       description: The access service network of the RSE.
                       type: string
@@ -818,15 +818,15 @@
                                     type: integer
                           extended_attributes:
                             description: The extended attributes of the protocol.
                             type: string
           401:
             description: Invalid Auth Token
           404:
-            description: RSE not found or RSE Operation, RSE Protocal Doman, RSE Protocol not supported
+            description: RSE not found or RSE Operation, RSE Protocol Domain, RSE Protocol not supported
           406:
             description: Not acceptable
         """
         try:
             p_list = get_rse_protocols(rse, issuer=request.environ.get('issuer'), vo=request.environ.get('vo'))
         except (RSEOperationNotSupported, RSENotFound, RSEProtocolNotSupported, RSEProtocolDomainNotSupported) as error:
             return generate_http_error_flask(404, error)
@@ -869,15 +869,15 @@
         - name: domain
           in: query
           description: Optional argument used to select the protocol for wan or lan use cases.
           schema:
             type: string
         - name: operation
           in: query
-          description: Optional query argument to select the protoco for read-vs-writes.
+          description: Optional query argument to select the protocol for read-vs-writes.
           schema:
             type: string
         responses:
           200:
             description: OK
             content:
               application/json:
@@ -886,15 +886,15 @@
                   type: object
                   additionalProperties:
                     type:
                       string
           401:
             description: Invalid Auth Token
           404:
-            description: RSE not found or RSE Protocol or RSE Protocl Domain not supported
+            description: RSE not found or RSE Protocol or RSE Protocol Domain not supported
           406:
             description: Not acceptable
         """
         lfns = request.args.getlist('lfn')
         lfns = list(map(lambda lfn: lfn.split(":", 1), lfns))
         if any(filter(lambda info: len(info) != 2, lfns)):
             invalid_lfns = ', '.join(filter(lambda info: len(info) != 2, lfns))
@@ -1346,15 +1346,15 @@
 
         return '', 200
 
     def delete(self, rse, scheme, hostname=None, port=None):
         """
         ---
         summary: Delete Protocol Attributes
-        description: Delete all protocol attibutes.
+        description: Delete all protocol attributes.
         tags:
           - Rucio Storage Elements
         parameters:
         - name: rse
           in: path
           description: The name of the Rucio Storage Element name.
           schema:
@@ -1844,15 +1844,15 @@
             content:
               application/json:
                 schema:
                   description: The distances between the Rses.
                   type: array
                   items:
                     type: object
-                    description: One distance betweeen source and destination.
+                    description: One distance between source and destination.
                     properties:
                       src_rse_id:
                         description: The source rse id.
                         type: string
                       dest_rse_id:
                         description: The destination rse id.
                         type: string
@@ -2171,15 +2171,15 @@
             content:
               application/json:
                 schema:
                   description: A list with all the QoS policies for an Rse.
                   type: array
                   items:
                     type: object
-                    porperties:
+                    properties:
                       rse_id:
                         description: The rse id.
                         type: string
                       qos_policy:
                         description: The qos policy.
                         type: string
           401:
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/rules.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,22 @@
                 - copies
                 - rse_expression
                 properties:
                   dids:
                     description: The list of data identifiers.
                     type: array
                     items:
-                      type: string
+                      type: object
+                      properties:
+                        scope:
+                          description: The scope of the data identifier
+                          type: string
+                        name:
+                          description: The name of the data identifier
+                          type: string
                   account:
                     description: The account of the issuer.
                     type: string
                   copies:
                     description: The number of replicas.
                     type: integer
                   rse_expression:
@@ -782,24 +789,24 @@
                             type: string
                             description: The scope of the transfer.
                           name:
                             type: string
                             description: The name of the lock.
                           rse_id:
                             type: string
-                            description: The rse_id of the transfered lock.
+                            description: The rse_id of the transferred lock.
                           rse:
                             type: object
-                            description: Information about the rse of the transfered lock.
+                            description: Information about the rse of the transferred lock.
                           attempts:
                             type: integer
                             description: The number of attempts.
                           last_error:
                             type: string
-                            description: The last error that occured.
+                            description: The last error that occurred.
                           last_source:
                             type: string
                             description: The last source.
                           sources:
                             type: array
                             description: All available rse sources.
                           last_time:
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/scopes.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/scopes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             application/json:
               schema:
                 type: object
                 required:
                   - options
                 properties:
                   options:
-                    description: The values for the new subcription.
+                    description: The values for the new subscription.
                     type: object
                     properties:
                       filter:
                         description: The filter for the subscription.
                         type: string
                       replication_rules:
                         description: The replication rules for the subscription.
@@ -160,15 +160,15 @@
                         description: The comments for the subscription.
                         type: string
                       lifetime:
                         description: The lifetime for the subscription.
                         type: string
                         format: date-time
                       retroactive:
-                        description: If the retroactive is actiavted for a subscription.
+                        description: If the retroactive is activated for a subscription.
                         type: boolean
                       priority:
                         description: The priority/policyid for the subscription. Stored as policyid.
                         type: integer
         responses:
           201:
             description: OK
@@ -230,15 +230,15 @@
             application/json:
               schema:
                 type: object
                 required:
                   - options
                 properties:
                   options:
-                    description: The values for the new subcription.
+                    description: The values for the new subscription.
                     type: object
                     required:
                       - filter
                       - replication_rules
                       - comments
                       - lifetime
                       - retroactive
@@ -253,15 +253,15 @@
                         description: The comments for the subscription.
                         type: string
                       lifetime:
                         description: The lifetime for the subscription.
                         type: string
                         format: date-time
                       retroactive:
-                        description: If the retroactive is actiavted for a subscription.
+                        description: If the retroactive is activated for a subscription.
                         type: boolean
                       priority:
                         description: The priority/policyid for the subscription. Stored as policyid.
                         type: integer
                       dry_run:
                         description: The priority/policyid for the subscription. Stored as policyid.
                         type: boolean
```

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/traces.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/traces.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/flaskapi/v1/vos.py` & `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/vos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/main.py` & `rucio-34.3.0/lib/rucio/web/rest/main.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/metrics.py` & `rucio-34.3.0/lib/rucio/web/rest/metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio/web/rest/ping.py` & `rucio-34.3.0/lib/rucio/web/rest/ping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/lib/rucio.egg-info/SOURCES.txt` & `rucio-34.3.0/lib/rucio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/pylintrc` & `rucio-34.3.0/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/requirements.txt` & `rucio-34.3.0/requirements.txt`

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

### Comparing `rucio-34.2.0/setup.py` & `rucio-34.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/setuputil.py` & `rucio-34.3.0/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_abacus_account.py` & `rucio-34.3.0/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_abacus_collection_replica.py` & `rucio-34.3.0/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_abacus_rse.py` & `rucio-34.3.0/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_account.py` & `rucio-34.3.0/tests/test_account.py`

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

### Comparing `rucio-34.2.0/tests/test_account_limits.py` & `rucio-34.3.0/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_api_external_representation.py` & `rucio-34.3.0/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_archive.py` & `rucio-34.3.0/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_auditor.py` & `rucio-34.3.0/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_auditor_hdfs.py` & `rucio-34.3.0/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_auditor_srmdumps.py` & `rucio-34.3.0/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_authentication.py` & `rucio-34.3.0/tests/test_authentication.py`

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

### Comparing `rucio-34.2.0/tests/test_automatix.py` & `rucio-34.3.0/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_bad_replica.py` & `rucio-34.3.0/tests/test_bad_replica.py`

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

### Comparing `rucio-34.2.0/tests/test_bb8.py` & `rucio-34.3.0/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_belleii.py` & `rucio-34.3.0/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_bin_rucio.py` & `rucio-34.3.0/tests/test_bin_rucio.py`

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

### Comparing `rucio-34.2.0/tests/test_boolean.py` & `rucio-34.3.0/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_clients.py` & `rucio-34.3.0/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_common_types.py` & `rucio-34.3.0/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_config.py` & `rucio-34.3.0/tests/test_config.py`

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

### Comparing `rucio-34.2.0/tests/test_conveyor.py` & `rucio-34.3.0/tests/test_conveyor.py`

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

### Comparing `rucio-34.2.0/tests/test_conveyor_submitter.py` & `rucio-34.3.0/tests/test_conveyor_submitter.py`

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

### Comparing `rucio-34.2.0/tests/test_counter.py` & `rucio-34.3.0/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_credential.py` & `rucio-34.3.0/tests/test_credential.py`

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

### Comparing `rucio-34.2.0/tests/test_curl.py` & `rucio-34.3.0/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_daemons.py` & `rucio-34.3.0/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_dataset_replicas.py` & `rucio-34.3.0/tests/test_dataset_replicas.py`

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

### Comparing `rucio-34.2.0/tests/test_db.py` & `rucio-34.3.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_did.py` & `rucio-34.3.0/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_did_meta_plugins.py` & `rucio-34.3.0/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_didtype.py` & `rucio-34.3.0/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_download.py` & `rucio-34.3.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_dumper.py` & `rucio-34.3.0/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_dumper_consistency.py` & `rucio-34.3.0/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_dumper_data_model.py` & `rucio-34.3.0/tests/test_dumper_data_model.py`

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

### Comparing `rucio-34.2.0/tests/test_dumper_path_parsing.py` & `rucio-34.3.0/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_filter_engine.py` & `rucio-34.3.0/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_heartbeat.py` & `rucio-34.3.0/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_hermes.py` & `rucio-34.3.0/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_identity.py` & `rucio-34.3.0/tests/test_identity.py`

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

### Comparing `rucio-34.2.0/tests/test_impl_upload_download.py` & `rucio-34.3.0/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_import_export.py` & `rucio-34.3.0/tests/test_import_export.py`

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

### Comparing `rucio-34.2.0/tests/test_judge_cleaner.py` & `rucio-34.3.0/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_judge_evaluator.py` & `rucio-34.3.0/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_judge_injector.py` & `rucio-34.3.0/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_judge_repairer.py` & `rucio-34.3.0/tests/test_judge_repairer.py`

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

### Comparing `rucio-34.2.0/tests/test_lifetime.py` & `rucio-34.3.0/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_message.py` & `rucio-34.3.0/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_meta_conventions.py` & `rucio-34.3.0/tests/test_meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_meta_did.py` & `rucio-34.3.0/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_module_import.py` & `rucio-34.3.0/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_monitor.py` & `rucio-34.3.0/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_multi_vo.py` & `rucio-34.3.0/tests/test_multi_vo.py`

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

### Comparing `rucio-34.2.0/tests/test_naming_convention.py` & `rucio-34.3.0/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_oauthmanager.py` & `rucio-34.3.0/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_oidc.py` & `rucio-34.3.0/tests/test_oidc.py`

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

### Comparing `rucio-34.2.0/tests/test_permission.py` & `rucio-34.3.0/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_pfns.py` & `rucio-34.3.0/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_ping.py` & `rucio-34.3.0/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_preparer.py` & `rucio-34.3.0/tests/test_preparer.py`

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

### Comparing `rucio-34.2.0/tests/test_qos.py` & `rucio-34.3.0/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_quarantined_replica.py` & `rucio-34.3.0/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_reaper.py` & `rucio-34.3.0/tests/test_reaper.py`

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

### Comparing `rucio-34.2.0/tests/test_redirect.py` & `rucio-34.3.0/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_replica.py` & `rucio-34.3.0/tests/test_replica.py`

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

### Comparing `rucio-34.2.0/tests/test_replica_recoverer.py` & `rucio-34.3.0/tests/test_replica_recoverer.py`

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

### Comparing `rucio-34.2.0/tests/test_replica_sorting.py` & `rucio-34.3.0/tests/test_replica_sorting.py`

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

### Comparing `rucio-34.2.0/tests/test_request.py` & `rucio-34.3.0/tests/test_request.py`

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

### Comparing `rucio-34.2.0/tests/test_root_proxy.py` & `rucio-34.3.0/tests/test_root_proxy.py`

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

### Comparing `rucio-34.2.0/tests/test_rse.py` & `rucio-34.3.0/tests/test_rse.py`

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

### Comparing `rucio-34.2.0/tests/test_rse_expression_parser.py` & `rucio-34.3.0/tests/test_rse_expression_parser.py`

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

### Comparing `rucio-34.2.0/tests/test_rse_lfn2path.py` & `rucio-34.3.0/tests/test_rse_lfn2path.py`

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

### Comparing `rucio-34.2.0/tests/test_rse_protocol_gfal2.py` & `rucio-34.3.0/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_rse_protocol_gfal2_impl.py` & `rucio-34.3.0/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_rse_protocol_posix.py` & `rucio-34.3.0/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_rse_protocol_rclone.py` & `rucio-34.3.0/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_rse_protocol_rsync.py` & `rucio-34.3.0/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_rse_protocol_srm.py` & `rucio-34.3.0/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_rse_protocol_ssh.py` & `rucio-34.3.0/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_rse_protocol_webdav.py` & `rucio-34.3.0/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_rse_protocol_xrootd.py` & `rucio-34.3.0/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_rse_selector.py` & `rucio-34.3.0/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_rucio_server.py` & `rucio-34.3.0/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_rule.py` & `rucio-34.3.0/tests/test_rule.py`

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

### Comparing `rucio-34.2.0/tests/test_schema_cms.py` & `rucio-34.3.0/tests/test_schema_cms.py`

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

### Comparing `rucio-34.2.0/tests/test_scope.py` & `rucio-34.3.0/tests/test_scope.py`

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

### Comparing `rucio-34.2.0/tests/test_subscription.py` & `rucio-34.3.0/tests/test_subscription.py`

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

### Comparing `rucio-34.2.0/tests/test_throttler.py` & `rucio-34.3.0/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_tpc.py` & `rucio-34.3.0/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_trace.py` & `rucio-34.3.0/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_transfer.py` & `rucio-34.3.0/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_transfer_plugins.py` & `rucio-34.3.0/tests/test_transfer_plugins.py`

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

### Comparing `rucio-34.2.0/tests/test_undertaker.py` & `rucio-34.3.0/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tests/test_upload.py` & `rucio-34.3.0/tests/test_upload.py`

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

### Comparing `rucio-34.2.0/tests/test_utils.py` & `rucio-34.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tools/bootstrap.py` & `rucio-34.3.0/tools/bootstrap.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tools/merge_rucio_configs.py` & `rucio-34.3.0/tools/merge_rucio_configs.py`

 * *Files identical despite different names*

### Comparing `rucio-34.2.0/tools/reset_database.py` & `rucio-34.3.0/tools/reset_database.py`

 * *Files identical despite different names*

