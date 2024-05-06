# Comparing `tmp/rucio_webui-34.2.0.tar.gz` & `tmp/rucio_webui-34.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio_webui-34.2.0.tar", last modified: Tue Apr 16 10:35:12 2024, max compression
+gzip compressed data, was "rucio_webui-34.3.0.tar", last modified: Mon May  6 12:44:14 2024, max compression
```

## Comparing `rucio_webui-34.2.0.tar` & `rucio_webui-34.3.0.tar`

### file list

```diff
@@ -1,267 +1,267 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.380100 rucio_webui-34.2.0/
--rwxr-xr-x   0 root         (0) root         (0)     4487 2024-03-19 15:04:29.000000 rucio_webui-34.2.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      484 2024-04-16 10:35:08.000000 rucio_webui-34.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      866 2024-04-16 10:35:12.380100 rucio_webui-34.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2024-04-16 07:53:27.000000 rucio_webui-34.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.335100 rucio_webui-34.2.0/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.337100 rucio_webui-34.2.0/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      660 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/alembicrevision.py
--rw-r--r--   0 root         (0) root         (0)      244 2024-04-16 07:53:37.000000 rucio_webui-34.2.0/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1577 2024-04-08 15:22:52.000000 rucio_webui-34.2.0/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.337100 rucio_webui-34.2.0/lib/rucio/web/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.338100 rucio_webui-34.2.0/lib/rucio/web/ui/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.338100 rucio_webui-34.2.0/lib/rucio/web/ui/flask/
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6178 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/bp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.338100 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/
--rwxr-xr-x   0 root         (0) root         (0)      618 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.339100 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/
--rw-r--r--   0 root         (0) root         (0)      990 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/advanced_settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.339100 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/certs/
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/certs/README
--rw-r--r--   0 root         (0) root         (0)      656 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/settings.json
--rw-r--r--   0 root         (0) root         (0)    27943 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/utils.py
--rw-r--r--   0 root         (0) root         (0)      893 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.346100 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/
--rw-r--r--   0 root         (0) root         (0)     3705 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account.html
--rw-r--r--   0 root         (0) root         (0)     1292 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account_rse_usage.html
--rw-r--r--   0 root         (0) root         (0)     1825 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account_usage.html
--rw-r--r--   0 root         (0) root         (0)     1234 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account_usage_history.html
--rw-r--r--   0 root         (0) root         (0)      857 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/accounting.html
--rw-r--r--   0 root         (0) root         (0)      996 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/accounts.html
--rw-r--r--   0 root         (0) root         (0)     4233 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/add_rse.html
--rw-r--r--   0 root         (0) root         (0)     4109 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/approve_rules.html
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/atlas_index.html
--rw-r--r--   0 root         (0) root         (0)     2880 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/backlog_mon.html
--rw-r--r--   0 root         (0) root         (0)     1207 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/bad_replicas.html
--rw-r--r--   0 root         (0) root         (0)     1678 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html
--rw-r--r--   0 root         (0) root         (0)     8979 2024-03-13 10:19:28.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/base.html
--rw-r--r--   0 root         (0) root         (0)     2652 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/cond.html
--rw-r--r--   0 root         (0) root         (0)     2678 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/dbrelease.html
--rw-r--r--   0 root         (0) root         (0)     2628 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/did.html
--rw-r--r--   0 root         (0) root         (0)     4970 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/dumps.html
--rw-r--r--   0 root         (0) root         (0)     1230 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/heartbeats.html
--rw-r--r--   0 root         (0) root         (0)      585 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/index.html
--rw-r--r--   0 root         (0) root         (0)     1789 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/infrastructure.html
--rw-r--r--   0 root         (0) root         (0)     3499 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/lifetime_exception.html
--rw-r--r--   0 root         (0) root         (0)     1270 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html
--rw-r--r--   0 root         (0) root         (0)     6608 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/list_rules.html
--rw-r--r--   0 root         (0) root         (0)     4440 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/login.html
--rw-r--r--   0 root         (0) root         (0)     1276 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/no_certificate.html
--rw-r--r--   0 root         (0) root         (0)      803 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/problem.html
--rw-r--r--   0 root         (0) root         (0)    16321 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/request_rule.html
--rw-r--r--   0 root         (0) root         (0)     4124 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse.html
--rw-r--r--   0 root         (0) root         (0)     2380 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_account_usage.html
--rw-r--r--   0 root         (0) root         (0)     7277 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_add_protocol.html
--rw-r--r--   0 root         (0) root         (0)     1547 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_locks.html
--rw-r--r--   0 root         (0) root         (0)     1363 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_usage.html
--rw-r--r--   0 root         (0) root         (0)     1796 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rses.html
--rw-r--r--   0 root         (0) root         (0)     1919 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rule.html
--rw-r--r--   0 root         (0) root         (0)     2079 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rules.html
--rw-r--r--   0 root         (0) root         (0)     2164 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/search.html
--rw-r--r--   0 root         (0) root         (0)     5125 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/select_login_method.html
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscription.html
--rw-r--r--   0 root         (0) root         (0)      956 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscriptionrules.html
--rw-r--r--   0 root         (0) root         (0)     1562 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscriptions.html
--rw-r--r--   0 root         (0) root         (0)     5327 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscriptions_editor.html
--rw-r--r--   0 root         (0) root         (0)     3024 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/suspicious_replicas.html
--rw-r--r--   0 root         (0) root         (0)      717 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/lib/rucio/web/ui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.348100 rucio_webui-34.2.0/lib/rucio/web/ui/media/
--rwxr-xr-x   0 root         (0) root         (0)   135652 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/RucioUI.png
--rw-r--r--   0 root         (0) root         (0)      686 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/details_close.png
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/details_open.png
--rw-r--r--   0 root         (0) root         (0)    84798 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/error.jpg
--rw-r--r--   0 root         (0) root         (0)    10510 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.349100 rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/
--rwxr-xr-x   0 root         (0) root         (0)     3400 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.eot
--rwxr-xr-x   0 root         (0) root         (0)     9218 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.svg
--rwxr-xr-x   0 root         (0) root         (0)     3236 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.ttf
--rwxr-xr-x   0 root         (0) root         (0)     3312 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.woff
--rw-r--r--   0 root         (0) root         (0)      753 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/get_info.png
--rw-r--r--   0 root         (0) root         (0)    56517 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/logo.png
--rw-r--r--   0 root         (0) root         (0)    19563 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/rucio_logo.png
--rw-r--r--   0 root         (0) root         (0)    32246 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/media/spinner.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.362100 rucio_webui-34.2.0/lib/rucio/web/ui/static/
--rw-r--r--   0 root         (0) root         (0)     6764 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/account.js
--rw-r--r--   0 root         (0) root         (0)     8084 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/account_rse_usage.js
--rw-r--r--   0 root         (0) root         (0)    12181 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/account_usage.js
--rw-r--r--   0 root         (0) root         (0)     7667 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/account_usage_history.js
--rw-r--r--   0 root         (0) root         (0)     4998 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/accounting.js
--rw-r--r--   0 root         (0) root         (0)     1352 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/accounts.js
--rw-r--r--   0 root         (0) root         (0)     2468 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/add_rse.js
--rw-r--r--   0 root         (0) root         (0)    12226 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/approve_rules.js
--rw-r--r--   0 root         (0) root         (0)     2229 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/atlas_index.js
--rw-r--r--   0 root         (0) root         (0)    15169 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/backlog_mon.js
--rw-r--r--   0 root         (0) root         (0)     1054 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/bad_replicas.js
--rw-r--r--   0 root         (0) root         (0)    11540 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/bad_replicas_summary.js
--rw-r--r--   0 root         (0) root         (0)     7366 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/base.js
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen-sprite.png
--rw-r--r--   0 root         (0) root         (0)      738 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen-sprite@2x.png
--rw-r--r--   0 root         (0) root         (0)    13270 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.css
--rw-r--r--   0 root         (0) root         (0)    44811 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.jquery.js
--rw-r--r--   0 root         (0) root         (0)    28401 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    11061 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.min.css
--rw-r--r--   0 root         (0) root         (0)    45100 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.proto.js
--rw-r--r--   0 root         (0) root         (0)    28757 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.proto.min.js
--rw-r--r--   0 root         (0) root         (0)     5641 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/cond.js
--rw-r--r--   0 root         (0) root         (0)     5758 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/dbrelease.js
--rw-r--r--   0 root         (0) root         (0)    43648 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/did.js
--rw-r--r--   0 root         (0) root         (0)     1396 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/filesize.min.js
--rw-r--r--   0 root         (0) root         (0)    19507 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.css
--rw-r--r--   0 root         (0) root         (0)    54568 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.eot
--rw-r--r--   0 root         (0) root         (0)   150251 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.svg
--rw-r--r--   0 root         (0) root         (0)    56976 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.ttf
--rw-r--r--   0 root         (0) root         (0)    32020 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.woff
--rw-r--r--   0 root         (0) root         (0)     1359 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/heartbeats.js
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring.css
--rw-r--r--   0 root         (0) root         (0)    12386 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_account_details.js
--rw-r--r--   0 root         (0) root         (0)     3525 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_accounts.js
--rw-r--r--   0 root         (0) root         (0)     5294 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js
--rw-r--r--   0 root         (0) root         (0)     3795 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_apiclasses.js
--rw-r--r--   0 root         (0) root         (0)     3555 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_index.js
--rw-r--r--   0 root         (0) root         (0)     3043 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_resources.js
--rw-r--r--   0 root         (0) root         (0)     8872 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js
--rw-r--r--   0 root         (0) root         (0)     3055 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_scriptids.js
--rw-r--r--   0 root         (0) root         (0)    10028 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_utils.js
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/index.js
--rw-r--r--   0 root         (0) root         (0)    23108 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.multiple.select.js
--rw-r--r--   0 root         (0) root         (0)    20021 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.multiple.select2.js
--rw-r--r--   0 root         (0) root         (0)     4151 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.quicksearch.js
--rw-r--r--   0 root         (0) root         (0)     6966 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.storageapi.min.js
--rw-r--r--   0 root         (0) root         (0)    11881 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/lifetime_exception.js
--rw-r--r--   0 root         (0) root         (0)     4060 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/list_lifetime_exceptions.js
--rw-r--r--   0 root         (0) root         (0)    13472 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/list_rules.js
--rw-r--r--   0 root         (0) root         (0)      324 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/login.js
--rw-r--r--   0 root         (0) root         (0)     4279 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/multiple-select.css
--rw-r--r--   0 root         (0) root         (0)     3342 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/multiple-select.png
--rw-r--r--   0 root         (0) root         (0)     2233 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/multiple-select2.css
--rw-r--r--   0 root         (0) root         (0)    54419 2024-03-13 10:19:28.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/request_rule.js
--rw-r--r--   0 root         (0) root         (0)     7089 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rse.js
--rw-r--r--   0 root         (0) root         (0)    23373 2024-03-13 10:19:28.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_account_usage.js
--rw-r--r--   0 root         (0) root         (0)     7076 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_add_protocol.js
--rw-r--r--   0 root         (0) root         (0)     6559 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_locks.js
--rw-r--r--   0 root         (0) root         (0)    10905 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_usage.js
--rw-r--r--   0 root         (0) root         (0)     1632 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rses.js
--rw-r--r--   0 root         (0) root         (0)     2598 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rucio.css
--rw-r--r--   0 root         (0) root         (0)    63519 2024-03-13 10:19:28.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rucio.js
--rw-r--r--   0 root         (0) root         (0)    23335 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rule.js
--rw-r--r--   0 root         (0) root         (0)     1341 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/rules.js
--rw-r--r--   0 root         (0) root         (0)     6323 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/search.js
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/select_login_method.css
--rw-r--r--   0 root         (0) root         (0)     7637 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/subscription.js
--rw-r--r--   0 root         (0) root         (0)     3071 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/subscriptionrules.js
--rw-r--r--   0 root         (0) root         (0)     4946 2024-03-13 10:19:28.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/subscriptions.js
--rw-r--r--   0 root         (0) root         (0)    13983 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/subscriptions_editor.js
--rw-r--r--   0 root         (0) root         (0)     9784 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/suspicious_replicas.js
--rw-r--r--   0 root         (0) root         (0)      540 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/switch.png
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-27 12:40:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/version.js
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-16 07:53:37.000000 rucio_webui-34.2.0/lib/rucio/web/ui/static/webui_version
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.379100 rucio_webui-34.2.0/lib/rucio_webui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8846 2024-04-16 10:35:12.000000 rucio_webui-34.2.0/lib/rucio_webui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2024-03-13 10:19:28.000000 rucio_webui-34.2.0/pylintrc
--rw-r--r--   0 root         (0) root         (0)     1235 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5048 2024-04-16 07:53:27.000000 rucio_webui-34.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2024-04-16 10:35:12.381100 rucio_webui-34.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2128 2024-04-16 10:35:08.000000 rucio_webui-34.2.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     4778 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 10:35:12.379100 rucio_webui-34.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3682 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10677 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3229 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15920 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20523 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13352 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4074 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2181 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4201 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    15058 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3464 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23264 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12425 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107413 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2065 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     8398 2024-04-08 15:14:19.000000 rucio_webui-34.2.0/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1865 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6942 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    96558 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    23797 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7679 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7337 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2618 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28187 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2736 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    58823 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29517 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4185 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7118 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16419 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10867 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3082 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38301 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7953 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10106 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5819 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18584 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57223 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5258 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22277 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20428 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12180 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6299 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2034 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54264 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2759 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11582 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   108356 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7583 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2741 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2023 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27487 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6440 2024-03-21 13:32:51.000000 rucio_webui-34.2.0/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62385 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    38873 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22741 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    17184 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    12978 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75019 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13184 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8941 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4277 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3267 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3690 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4799 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     3979 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3780 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7746 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    91864 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)    13848 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_schema_cms.py
--rw-r--r--   0 root         (0) root         (0)     7486 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48328 2024-04-02 11:36:32.000000 rucio_webui-34.2.0/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)    55587 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3181 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    25254 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8923 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_transfer_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8412 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15526 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     7427 2024-03-21 13:32:52.000000 rucio_webui-34.2.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.867814 rucio_webui-34.3.0/
+-rwxr-xr-x   0 root         (0) root         (0)     4487 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      484 2024-05-06 12:44:11.000000 rucio_webui-34.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      866 2024-05-06 12:44:14.867814 rucio_webui-34.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.821813 rucio_webui-34.3.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.824813 rucio_webui-34.3.0/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/alembicrevision.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-05-06 11:04:02.000000 rucio_webui-34.3.0/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.824813 rucio_webui-34.3.0/lib/rucio/web/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.825814 rucio_webui-34.3.0/lib/rucio/web/ui/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.825814 rucio_webui-34.3.0/lib/rucio/web/ui/flask/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/bp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.825814 rucio_webui-34.3.0/lib/rucio/web/ui/flask/common/
+-rwxr-xr-x   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.826814 rucio_webui-34.3.0/lib/rucio/web/ui/flask/common/saml/
+-rw-r--r--   0 root         (0) root         (0)      990 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/common/saml/advanced_settings.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.826814 rucio_webui-34.3.0/lib/rucio/web/ui/flask/common/saml/certs/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/common/saml/certs/README
+-rw-r--r--   0 root         (0) root         (0)      656 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/common/saml/settings.json
+-rw-r--r--   0 root         (0) root         (0)    27943 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/common/utils.py
+-rw-r--r--   0 root         (0) root         (0)      893 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.833814 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/
+-rw-r--r--   0 root         (0) root         (0)     3706 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/account.html
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/account_rse_usage.html
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/account_usage.html
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/account_usage_history.html
+-rw-r--r--   0 root         (0) root         (0)      857 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/accounting.html
+-rw-r--r--   0 root         (0) root         (0)      996 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/accounts.html
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/add_rse.html
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/approve_rules.html
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/atlas_index.html
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/backlog_mon.html
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/bad_replicas.html
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html
+-rw-r--r--   0 root         (0) root         (0)     8979 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)     2652 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/cond.html
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/dbrelease.html
+-rw-r--r--   0 root         (0) root         (0)     2628 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/did.html
+-rw-r--r--   0 root         (0) root         (0)     4970 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/dumps.html
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/heartbeats.html
+-rw-r--r--   0 root         (0) root         (0)      585 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/index.html
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/infrastructure.html
+-rw-r--r--   0 root         (0) root         (0)     3499 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/lifetime_exception.html
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html
+-rw-r--r--   0 root         (0) root         (0)     6608 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/list_rules.html
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/login.html
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/no_certificate.html
+-rw-r--r--   0 root         (0) root         (0)      803 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/problem.html
+-rw-r--r--   0 root         (0) root         (0)    16321 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/request_rule.html
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rse.html
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rse_account_usage.html
+-rw-r--r--   0 root         (0) root         (0)     7276 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rse_add_protocol.html
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rse_locks.html
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rse_usage.html
+-rw-r--r--   0 root         (0) root         (0)     1796 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rses.html
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rule.html
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rules.html
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/search.html
+-rw-r--r--   0 root         (0) root         (0)     5125 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/select_login_method.html
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/subscription.html
+-rw-r--r--   0 root         (0) root         (0)      956 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/subscriptionrules.html
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/subscriptions.html
+-rw-r--r--   0 root         (0) root         (0)     5327 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/subscriptions_editor.html
+-rw-r--r--   0 root         (0) root         (0)     3024 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/suspicious_replicas.html
+-rw-r--r--   0 root         (0) root         (0)      717 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.835814 rucio_webui-34.3.0/lib/rucio/web/ui/media/
+-rwxr-xr-x   0 root         (0) root         (0)   135652 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/RucioUI.png
+-rw-r--r--   0 root         (0) root         (0)      686 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/details_close.png
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/details_open.png
+-rw-r--r--   0 root         (0) root         (0)    84798 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/error.jpg
+-rw-r--r--   0 root         (0) root         (0)    10510 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.836814 rucio_webui-34.3.0/lib/rucio/web/ui/media/fonts/
+-rwxr-xr-x   0 root         (0) root         (0)     3400 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/fonts/login_icons.eot
+-rwxr-xr-x   0 root         (0) root         (0)     9218 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/fonts/login_icons.svg
+-rwxr-xr-x   0 root         (0) root         (0)     3236 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/fonts/login_icons.ttf
+-rwxr-xr-x   0 root         (0) root         (0)     3312 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/fonts/login_icons.woff
+-rw-r--r--   0 root         (0) root         (0)      753 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/get_info.png
+-rw-r--r--   0 root         (0) root         (0)    56517 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/logo.png
+-rw-r--r--   0 root         (0) root         (0)    19563 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/rucio_logo.png
+-rw-r--r--   0 root         (0) root         (0)    32246 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/media/spinner.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.850814 rucio_webui-34.3.0/lib/rucio/web/ui/static/
+-rw-r--r--   0 root         (0) root         (0)     6764 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/account.js
+-rw-r--r--   0 root         (0) root         (0)     8084 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/account_rse_usage.js
+-rw-r--r--   0 root         (0) root         (0)    12181 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/account_usage.js
+-rw-r--r--   0 root         (0) root         (0)     7667 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/account_usage_history.js
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/accounting.js
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/accounts.js
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/add_rse.js
+-rw-r--r--   0 root         (0) root         (0)    12226 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/approve_rules.js
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/atlas_index.js
+-rw-r--r--   0 root         (0) root         (0)    15169 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/backlog_mon.js
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/bad_replicas.js
+-rw-r--r--   0 root         (0) root         (0)    11540 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/bad_replicas_summary.js
+-rw-r--r--   0 root         (0) root         (0)     7366 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/base.js
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen-sprite.png
+-rw-r--r--   0 root         (0) root         (0)      738 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen-sprite@2x.png
+-rw-r--r--   0 root         (0) root         (0)    13270 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen.css
+-rw-r--r--   0 root         (0) root         (0)    44811 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen.jquery.js
+-rw-r--r--   0 root         (0) root         (0)    28401 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen.jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    11061 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen.min.css
+-rw-r--r--   0 root         (0) root         (0)    45100 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen.proto.js
+-rw-r--r--   0 root         (0) root         (0)    28757 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen.proto.min.js
+-rw-r--r--   0 root         (0) root         (0)     5641 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/cond.js
+-rw-r--r--   0 root         (0) root         (0)     5758 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/dbrelease.js
+-rw-r--r--   0 root         (0) root         (0)    43654 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/did.js
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/filesize.min.js
+-rw-r--r--   0 root         (0) root         (0)    19507 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/foundation-icons.css
+-rw-r--r--   0 root         (0) root         (0)    54568 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/foundation-icons.eot
+-rw-r--r--   0 root         (0) root         (0)   150251 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/foundation-icons.svg
+-rw-r--r--   0 root         (0) root         (0)    56976 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/foundation-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    32020 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/foundation-icons.woff
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/heartbeats.js
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring.css
+-rw-r--r--   0 root         (0) root         (0)    12377 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_account_details.js
+-rw-r--r--   0 root         (0) root         (0)     3516 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_accounts.js
+-rw-r--r--   0 root         (0) root         (0)     5285 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js
+-rw-r--r--   0 root         (0) root         (0)     3783 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_apiclasses.js
+-rw-r--r--   0 root         (0) root         (0)     3555 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_index.js
+-rw-r--r--   0 root         (0) root         (0)     3034 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_resources.js
+-rw-r--r--   0 root         (0) root         (0)     8863 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js
+-rw-r--r--   0 root         (0) root         (0)     3043 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_scriptids.js
+-rw-r--r--   0 root         (0) root         (0)    10027 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_utils.js
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/index.js
+-rw-r--r--   0 root         (0) root         (0)    23108 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/jquery.multiple.select.js
+-rw-r--r--   0 root         (0) root         (0)    20021 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/jquery.multiple.select2.js
+-rw-r--r--   0 root         (0) root         (0)     4152 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/jquery.quicksearch.js
+-rw-r--r--   0 root         (0) root         (0)     6966 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/jquery.storageapi.min.js
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/lifetime_exception.js
+-rw-r--r--   0 root         (0) root         (0)     4060 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/list_lifetime_exceptions.js
+-rw-r--r--   0 root         (0) root         (0)    13472 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/list_rules.js
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/login.js
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/multiple-select.css
+-rw-r--r--   0 root         (0) root         (0)     3342 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/multiple-select.png
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/multiple-select2.css
+-rw-r--r--   0 root         (0) root         (0)    54419 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/request_rule.js
+-rw-r--r--   0 root         (0) root         (0)     7089 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/rse.js
+-rw-r--r--   0 root         (0) root         (0)    23377 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/rse_account_usage.js
+-rw-r--r--   0 root         (0) root         (0)     7076 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/rse_add_protocol.js
+-rw-r--r--   0 root         (0) root         (0)     6559 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/rse_locks.js
+-rw-r--r--   0 root         (0) root         (0)    10905 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/rse_usage.js
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/rses.js
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/rucio.css
+-rw-r--r--   0 root         (0) root         (0)    63519 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/rucio.js
+-rw-r--r--   0 root         (0) root         (0)    23337 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/rule.js
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/rules.js
+-rw-r--r--   0 root         (0) root         (0)     6323 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/search.js
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/select_login_method.css
+-rw-r--r--   0 root         (0) root         (0)     7637 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/subscription.js
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/subscriptionrules.js
+-rw-r--r--   0 root         (0) root         (0)     4946 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/subscriptions.js
+-rw-r--r--   0 root         (0) root         (0)    13983 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/subscriptions_editor.js
+-rw-r--r--   0 root         (0) root         (0)     9784 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/suspicious_replicas.js
+-rw-r--r--   0 root         (0) root         (0)      540 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/switch.png
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-27 12:40:37.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/version.js
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-06 11:04:02.000000 rucio_webui-34.3.0/lib/rucio/web/ui/static/webui_version
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.866814 rucio_webui-34.3.0/lib/rucio_webui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8846 2024-05-06 12:44:14.000000 rucio_webui-34.3.0/lib/rucio_webui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/pylintrc
+-rw-r--r--   0 root         (0) root         (0)     4349 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5235 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-06 12:44:14.868814 rucio_webui-34.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2128 2024-05-06 12:44:11.000000 rucio_webui-34.3.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:14.866814 rucio_webui-34.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10677 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15923 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    14964 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23265 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12425 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107450 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6942 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    96724 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    23870 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7728 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28183 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    58823 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29517 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16419 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10869 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38301 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10106 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57290 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5258 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22277 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20429 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54332 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   108359 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7662 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27487 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62453 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    38868 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22796 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    17257 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    13033 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75080 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13184 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8940 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4799 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     3979 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7746 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    91949 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)    13848 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_schema_cms.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48389 2024-05-06 11:03:53.000000 rucio_webui-34.3.0/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    55587 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    25254 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8924 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_transfer_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    15575 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2024-05-06 09:19:47.000000 rucio_webui-34.3.0/tests/test_utils.py
```

### Comparing `rucio_webui-34.2.0/AUTHORS.rst` & `rucio_webui-34.3.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/LICENSE` & `rucio_webui-34.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/PKG-INFO` & `rucio_webui-34.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio-webui
-Version: 34.2.0
+Version: 34.3.0
 Summary: Rucio WebUI Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rucio_webui-34.2.0/README.rst` & `rucio_webui-34.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/__init__.py` & `rucio_webui-34.3.0/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/alembicrevision.py` & `rucio_webui-34.3.0/lib/rucio/alembicrevision.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/version.py` & `rucio_webui-34.3.0/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/__init__.py` & `rucio_webui-34.3.0/lib/rucio/web/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/__init__.py` & `rucio_webui-34.3.0/lib/rucio/web/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/__init__.py` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/bp.py` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/bp.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/__init__.py` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/advanced_settings.json` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/common/saml/advanced_settings.json`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/saml/settings.json` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/common/saml/settings.json`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/common/utils.py` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/common/utils.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/main.py` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/main.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/account.html`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     <div class="row">
       <div class="large-1 columns"><a class="button postfix" href="#" data-reveal-id="attrmodal">Add</a></div>
       <div class="large-10 columns"></div>
       <div class="large-1 columns"><a class="alert button postfix" id="del_attr">Delete</a></div>
     </div>
   </div>
 
-  <div id="identites" class="columns panel">
+  <div id="identities" class="columns panel">
     <h4>Account Identities</h4>
     <div id="loading_id">
       <div class="row"><div class="small-1 small-centered columns">
           <img src="/media/spinner.gif">
         </div>
       </div>
     </div>
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account_rse_usage.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/account_rse_usage.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account_usage.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/account_usage.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/account_usage_history.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/account_usage_history.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/accounting.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/accounting.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/accounts.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/accounts.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/add_rse.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/add_rse.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/approve_rules.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/approve_rules.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/atlas_index.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/atlas_index.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/backlog_mon.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/backlog_mon.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/bad_replicas.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/bad_replicas.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/bad_replicas_summary.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/base.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/base.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/cond.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/cond.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/dbrelease.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/dbrelease.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/did.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/did.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/dumps.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/dumps.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/heartbeats.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/heartbeats.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/index.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/index.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/infrastructure.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/infrastructure.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/lifetime_exception.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/lifetime_exception.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/list_lifetime_exceptions.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/list_rules.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/list_rules.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/login.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/login.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/no_certificate.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/no_certificate.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/problem.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/problem.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/request_rule.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/request_rule.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rse.html`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 <script src="/static/rse.js"></script>
 {%- endblock head %}
 
 {% block content -%}
 {{ super() }}
 <div id="result" class="row" data-equalizer>
     <div id="rse_info" class="columns panel">
-        <h4>Informations</h4>
+        <h4>Information</h4>
         <div class="row" id="loadingInfo">
             <div class="small-1 small-centered columns">
                 <img src="/media/spinner.gif">
             </div>
         </div>
         <table id="t_metadata" style="word-wrap: break-word;">
         </table>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends 'base.html' %} {% block head -%} {{ super() }}
 {%- endblock head %} {% block content -%} {{ super() }}
-****** IInnffoorrmmaattiioonnss ******
+****** IInnffoorrmmaattiioonn ******
 [/media/spinner.gif]
 ****** PPrroottooccoollss ******
 [/media/spinner.gif]
 [/media/spinner.gif]
 Add protocol
 ****** AAttttrriibbuutteess ******
 [/media/spinner.gif]
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_account_usage.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rse_account_usage.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_add_protocol.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rse_add_protocol.html`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                             <input type="number" id="wan_write" placeholder="">
                         </div>
                     </div>
                 </div>
             </div>
             <br>
             <div>
-                <h3>Informations</h3>
+                <h3>Information</h3>
                 <div class="row collapse">
                     <div class="large-1 columns">
                         <label for="hostname" class="left inline">Hostname</label>
                     </div>
                     <div class="large-10 columns">
                         <input type="text" id="hostname" placeholder="">
                     </div>
```

#### html2text {}

```diff
@@ -16,15 +16,15 @@
 Third party copy read
 [Unknown INPUT type]
 Third party copy write
 [Unknown INPUT type]
 Write
 [Unknown INPUT type]
 
-******** IInnffoorrmmaattiioonnss ********
+******** IInnffoorrmmaattiioonn ********
 Hostname
 [                    ]
 Implementation
 [                    ]
 Port
 [Unknown INPUT type]
 Prefix
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_locks.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rse_locks.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rse_usage.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rse_usage.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rses.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rses.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rule.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rule.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/rules.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/rules.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/search.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/search.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/select_login_method.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/select_login_method.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscription.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/subscription.html`

 * *Files 0% similar despite different names*

```diff
@@ -27,13 +27,13 @@
     <h4>Subscription metadata</h4>
     <table id="t_metadata" style="word-wrap: break-word;">
     </table>
   </div>
 </div>
 <div class="row">
   <div class="columns large-1">
-     <div id="subscription_editor" class="button small expand">Edit subcription</div>
+     <div id="subscription_editor" class="button small expand">Edit subscription</div>
  </div>
 </div>
 
 <div id="problem_details" style="margin: 2em;"></div>
 {%- endblock content %}
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 {% extends 'base.html' %} {% block head -%} {{ super() }}
 {%- endblock head %} {% block content -%} {{ super() }}
 ****** SSuubbssccrriippttiioonn mmeettaaddaattaa ******
-Edit subcription
+Edit subscription
 {%- endblock content %}
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscriptionrules.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/subscriptionrules.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscriptions.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/subscriptions.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/subscriptions_editor.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/subscriptions_editor.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/flask/templates/suspicious_replicas.html` & `rucio_webui-34.3.0/lib/rucio/web/ui/flask/templates/suspicious_replicas.html`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/main.py` & `rucio_webui-34.3.0/lib/rucio/web/ui/main.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/RucioUI.png` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/RucioUI.png`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/details_close.png` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/details_close.png`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/details_open.png` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/details_open.png`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/error.jpg` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/error.jpg`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/favicon.ico` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/favicon.ico`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.eot` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/fonts/login_icons.eot`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.svg` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/fonts/login_icons.svg`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.ttf` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/fonts/login_icons.ttf`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/fonts/login_icons.woff` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/fonts/login_icons.woff`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/get_info.png` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/get_info.png`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/logo.png` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/logo.png`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/rucio_logo.png` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/rucio_logo.png`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/media/spinner.gif` & `rucio_webui-34.3.0/lib/rucio/web/ui/media/spinner.gif`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/account.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/account.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/account_rse_usage.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/account_rse_usage.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/account_usage.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/account_usage.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/account_usage_history.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/account_usage_history.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/accounting.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/accounting.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/accounts.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/accounts.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/add_rse.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/add_rse.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/approve_rules.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/approve_rules.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/atlas_index.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/atlas_index.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/backlog_mon.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/backlog_mon.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/bad_replicas.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/bad_replicas.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/bad_replicas_summary.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/bad_replicas_summary.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/base.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/base.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen-sprite.png` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen-sprite@2x.png` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.css` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen.css`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.jquery.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen.jquery.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.jquery.min.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.min.css` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen.min.css`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.proto.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen.proto.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/chosen.proto.min.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/chosen.proto.min.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/cond.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/cond.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/dbrelease.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/dbrelease.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/did.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/did.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -698,15 +698,15 @@
                                                 'dids': dids,
                                                 success: function(data2) {
                                                     console.log('Attached correct files, moving now...');
                                                     move_did(scope, name + '.' + found_dataset_list[0]['timestamp'], true, dids.length);
                                                 },
                                                 error: function(jqXHR, textStatus, errorThrown) {
                                                     console.log(jqXHR);
-                                                    alert('An error has ocurred: Could not attach correct files to temporary dataset.');
+                                                    alert('An error has occurred: Could not attach correct files to temporary dataset.');
                                                 }
                                             });
                                         },
                                         error: function(jqXHR, textStatus, errorThrown) {
                                             console.log(jqXHR);
                                             console.log('Could not detach dids, removing dataset from storage and creating it again...');
                                             removeDatasetFromStorage(scope, name);
@@ -719,15 +719,15 @@
                                     console.log('All necessary files contained in dataset, moving now...');
                                     move_did(scope, name + '.' + found_dataset_list[0]['timestamp'], true, dids.length);
                                 }
                             });
                         },
                         error: function(jqXHR, textStatus, errorThrown) {
                             console.log(jqXHR);
-                            alert('An error has ocurred: Could not get files for dataset.');
+                            alert('An error has occurred: Could not get files for dataset.');
                         }
                     });
                 } else {
                     // Rule exists, check if enough files are being moved
                     console.log('Dataset rule exists. Checking if files correct...');
                     r.get_replica_lock_for_rule_id({
                         'rule_id': data[0]['id'],
@@ -753,22 +753,22 @@
                                 if (index == dids.length - 1) { // all dids contained in rule
                                     alert('This Dataset is already being moved. Please come back later.');
                                 };
                             });
                         },
                         error: function(jqXHR, textStatus, errorThrown) {
                             console.log(jqXHR);
-                            alert('An error has ocurred: Could not determine locks for replication rule.');
+                            alert('An error has occurred: Could not determine locks for replication rule.');
                         }
                     });
                 }
             },
             error: function(jqXHR, textStatus, errorThrown) {
                 console.log(jqXHR);
-                alert('An error has ocurred. Could not check whether rule already exists.');
+                alert('An error has occurred. Could not check whether rule already exists.');
             }
         });
     } else {
         var ts = Date.now();
         storage_list.push({
             id: scope + ':' + name,
             timestamp: ts
@@ -786,22 +786,22 @@
                     'dids': dids,
                     success: function(data2) {
                         move_did(scope, name + '.' + ts, true, dids.length);
                     },
                     error: function(jqXHR, textStatus, errorThrown) {
                         console.log(jqXHR);
                         removeDatasetFromStorage(scope, name);
-                        alert('An error has ocurred: Could not attach files to newly created temporary dataset.');
+                        alert('An error has occurred: Could not attach files to newly created temporary dataset.');
                     }
                 });
             },
             error: function(jqXHR, textStatus, errorThrown) {
                 console.log(jqXHR);
                 removeDatasetFromStorage(scope, name);
-                alert('An error has ocurred: Could not create temporary dataset.');
+                alert('An error has occurred: Could not create temporary dataset.');
             }
         });
     }
 };
 
 handle_container = function(scope, name) {
     load_rules(scope, name);
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/filesize.min.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/filesize.min.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.css` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.eot` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.svg` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.ttf` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/foundation-icons.woff` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/heartbeats.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/heartbeats.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring.css` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring.css`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_account_details.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_account_details.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -197,17 +197,17 @@
             $('#resources > .chart.sec').html($('<img/>').attr('src', '/media/error.jpg'));
         }
     });
 }
 
 function fillTable(csv, date) {
     var tbl_data = [],
-        splitted = csv.split('\n');
-    for (var i = 0; i < splitted.length; i++) {
-        cols = splitted[i].split('\t');
+        split = csv.split('\n');
+    for (var i = 0; i < split.length; i++) {
+        cols = split[i].split('\t');
         if (cols[0] == "") continue;
         var caption = '';
         if (/^\w+\s+\/(dids|replicas)\/\S+?\/.+$/.test(cols[2])) {
             caption = '<a target="_blank" href="/search?scope=' + cols[2].match(/^\w+\s+\/(dids|replicas)\/(.*?)\/.*$/)[2] + '&name=' + cols[2].match(/^\w+\s+\/(dids|replicas)\/.*?\/(.*?)(\?.*)?$/)[2] + '">' + cols[2] + '</a>';
         } else if (/^PUT\s\/rules\/\w+$/.test(cols[2])) {
             caption = '<a target="_blank" href="/rule?rule_id=' + cols[2].match(/^PUT\s\/rules\/(\w+)$/)[2] + '">' + cols[2] + '</a>';
         } else {
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_accounts.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_accounts.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -42,17 +42,17 @@
             $('#accounts2 > .chart.sec').html($('<img/>').attr('src', '/media/error.jpg'));
         }
     });
 }
 
 function fillTable(csv, date) {
     var tbl_data = [],
-        splitted = csv.split('\n');
-    for (var i = 0; i < splitted.length; i++) {
-        cols = splitted[i].split('\t');
+        split = csv.split('\n');
+    for (var i = 0; i < split.length; i++) {
+        cols = split[i].split('\t');
         if ((cols.length < 5) || (isNaN(cols[2])) || (isNaN(cols[3])) || (isNaN(cols[4])))
             continue;
         if (cols[0] == "") continue;
         tbl_data.push(["<a href=\"/webstats/accounts/" + cols[1] + "?date=" + date + "\">" + cols[1] + "</a>",
             Number(cols[2]),
             (Number(cols[3]) / 1024 / 1024).toFixed(2),
             (Number(cols[4]) / 1000000).toFixed(2)
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -45,17 +45,17 @@
             data.push(lines[i]);
     }
     return data.join('\n');
 }
 
 function fillTable(csv, date) {
     var tbl_data = [],
-        splitted = csv.split('\n');
-    for (var i = 0; i < splitted.length; i++) {
-        cols = splitted[i].split('\t');
+        split = csv.split('\n');
+    for (var i = 0; i < split.length; i++) {
+        cols = split[i].split('\t');
         if ((cols.length < 7) || (isNaN(cols[4])) || (isNaN(cols[5])) || (isNaN(cols[6])))
             continue;
         tbl_data.push([
             '<a href ="/webstats/accounts/' + cols[1] + '?date=' + date + '">' + cols[1] + '</a>',
             //'<a href ="/webstats/useragents/'+cols[2]+'?date='+date+'">'+cols[2]+'</a>',
             cols[3],
             Number(cols[4]),
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_apiclasses.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_apiclasses.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -51,19 +51,19 @@
     });
 }
 
 function fillTable(csv, date) {
     var tbl_data = [],
         cols = undefined,
         classID = undefined,
-        splitted = csv.split('\n'),
+        split = csv.split('\n'),
         aggregatedData = {};
-    for (var i = 0; i < splitted.length; i++) {
-        if (splitted == '') continue;
-        cols = splitted[i].split('\t');
+    for (var i = 0; i < split.length; i++) {
+        if (split == '') continue;
+        cols = split[i].split('\t');
         if ((cols.length < 7) || (isNaN(cols[4])) || (isNaN(cols[5])) || (isNaN(cols[6])))
             continue;
         classID = cols[2].match(/^(\w+\.\w+)/)[1];
         if (aggregatedData[classID] == undefined) aggregatedData[classID] = {
             'hits': 0,
             'mb': 0,
             'sec': 0
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_index.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_index.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_resources.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_resources.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -28,17 +28,17 @@
             $('#resources > .chart.sec').html($('<img/>').attr('src', '/media/error.jpg'));
         }
     });
 }
 
 function fillTable(csv, date) {
     var tbl_data = [],
-        splitted = csv.split('\n');
-    for (var i = 0; i < splitted.length; i++) {
-        cols = splitted[i].split('\t');
+        split = csv.split('\n');
+    for (var i = 0; i < split.length; i++) {
+        cols = split[i].split('\t');
         if ((cols.length < 5) || (isNaN(cols[2])) || (isNaN(cols[3])) || (isNaN(cols[4])))
             continue
         var caption = '';
         if (/^\w+\s+\/(dids|replicas)\/\S+?\/.+$/.test(cols[1])) {
             caption = '<a target="_blank" href="/search?scope=' + cols[1].match(/^\w+\s+\/(dids|replicas)\/(.*?)\/.*$/)[2] + '&name=' + cols[1].match(/^\w+\s+\/(dids|replicas)\/.*?\/(.*?)(\?.*)?$/)[2] + '">' + cols[1] + '</a>';
         } else if (/^PUT\s\/rules\/\w+$/.test(cols[1])) {
             caption = '<a target="_blank" href="/rule?rule_id=' + cols[1].match(/^PUT\s\/rules\/(\w+)$/)[1] + '">' + cols[1] + '</a>';
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -132,17 +132,17 @@
             data.push(lines[i]);
     }
     return data.join('\n');
 }
 
 function fillTable(csv, date) {
     var tbl_data = [],
-        splitted = csv.split('\n');
-    for (var i = 0; i < splitted.length; i++) {
-        cols = splitted[i].split('\t');
+        split = csv.split('\n');
+    for (var i = 0; i < split.length; i++) {
+        cols = split[i].split('\t');
         if ((cols.length < 7) || (isNaN(cols[4])) || (isNaN(cols[5])) || (isNaN(cols[6])))
             continue;
         tbl_data.push([
             '<a href ="/webstats/accounts/' + cols[1] + '?date=' + date + '">' + cols[1] + '</a>',
             '<a href ="/webstats/apiclasses/' + cols[2] + '?date=' + date + '">' + cols[2] + '</a>',
             Number(cols[4]),
             (Number(cols[5]) / 1024 / 1024).toFixed(2),
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_scriptids.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_scriptids.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -30,19 +30,19 @@
     });
 }
 
 function fillTable(csv, date) {
     var tbl_data = [],
         cols = undefined,
         scriptID = undefined,
-        splitted = csv.split('\n'),
+        split = csv.split('\n'),
         aggregatedData = {};
-    for (var i = 0; i < splitted.length; i++) {
-        if (splitted == '') continue;
-        cols = splitted[i].split('\t');
+    for (var i = 0; i < split.length; i++) {
+        if (split == '') continue;
+        cols = split[i].split('\t');
         if ((cols.length < 7) || (isNaN(cols[4])) || (isNaN(cols[5])) || (isNaN(cols[6])))
             continue;
         scriptID = cols[3];
         if (aggregatedData[scriptID] == undefined) aggregatedData[scriptID] = {
             'hits': 0,
             'mb': 0,
             'sec': 0
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/http_monitoring_utils.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/http_monitoring_utils.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -63,15 +63,15 @@
     data.sort(function(a, b) {
         return (b[1] - a[1]);
     });
     if (sum != 0) data.push(["Others (Pos: " + top + " - " + (entries == 0 ? dataMatrix.length : entries) + ")", sum]);;
     return data;
 }
 
-function drawDoubleChart(traget, title, main, sub, series, top) {
+function drawDoubleChart(target, title, main, sub, series, top) {
     var colors = Highcharts.getOptions().colors,
         data = {},
         mainData = [],
         subData = [],
         mainCategoryCounter = 0,
         j,
         total = 0,
@@ -149,15 +149,15 @@
                 y: data[mainCategory].drilldown.data[j],
                 color: Highcharts.Color(data[mainCategory].color).brighten(brightness).get()
             });
         }
     }
 
     // Create the chart
-    $(traget).highcharts({
+    $(target).highcharts({
         chart: {
             type: 'pie'
         },
         title: {
             text: title
         },
         yAxis: {
@@ -330,15 +330,15 @@
                 if (RegExp(id + '$', 'i').test(panelID)) {
                     $(this).addClass('active');
                 } else {
                     $(this).removeClass('active');
                 }
             });
             $('#drilldowns > li.active > a').first().click();
-            //Toggeling columns in summary table
+            //Toggling columns in summary table
             summaryTable = $(summaryTableSelector).DataTable();
             summaryTable.columns([1, 2, 3]).visible(false);;
             summaryTable.column($(this).attr('data-column')).visible(true);
             summaryTable.column($(this).attr('data-column')).order('desc');
             summaryTable.draw();
         });
     });
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.multiple.select.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/jquery.multiple.select.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.multiple.select2.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/jquery.multiple.select2.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.quicksearch.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/jquery.quicksearch.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -65,15 +65,15 @@
             this.loader(false);
             options.onAfter();
 
             return this;
         };
 
         /*
-         * 		 * External API so that users can perform search programatically.
+         * 		 * External API so that users can perform search programmatically.
          * 		 		 * */
         this.search = function(submittedVal) {
             val = submittedVal;
             e.trigger();
         };
 
         /*
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/jquery.storageapi.min.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/jquery.storageapi.min.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/lifetime_exception.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/lifetime_exception.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/list_lifetime_exceptions.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/list_lifetime_exceptions.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/list_rules.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/list_rules.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/multiple-select.css` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/multiple-select.css`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/multiple-select.png` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/multiple-select.png`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/multiple-select2.css` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/multiple-select2.css`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/request_rule.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/request_rule.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/rse.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/rse.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_account_usage.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/rse_account_usage.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -462,15 +462,15 @@
         new_bytes = 0;
     }
 
     delta_bytes = new_bytes - old_bytes;
     container.removeClass('editing');
     $("#resulttable").DataTable().cell(container).data(new_bytes);
 
-    // Check if value changed, and thus cell should be marked as 'updated' i.e. if delta greate than 1%
+    // Check if value changed, and thus cell should be marked as 'updated' i.e. if delta is greater than 1%
     if (delta_bytes && (new_bytes > 0)) {
         container.addClass('updated');
         container.attr('data-info', 'Delta: ' + filesize(delta_bytes, {
             'base': 10
         }));
     } else if (new_bytes == 0) {
         //container.attr('data-info', 'Read-Only access');
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_add_protocol.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/rse_add_protocol.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_locks.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/rse_locks.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/rse_usage.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/rse_usage.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/rses.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/rses.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/rucio.css` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/rucio.css`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/rucio.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/rucio.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -524,15 +524,15 @@
     };
     if (options.lifetime == '') {
         options.lifetime = null;
     };
     if (options.source_replica_expression == '') {
         options.source_replica_expression = null;
     };
-    if (options.nofity == '') {
+    if (options.notify == '') {
         options.notify = null;
     };
     jQuery.ajax({
         url: url,
         crossDomain: true,
         type: 'POST',
         headers: this.headers,
@@ -1370,15 +1370,15 @@
         },
         error: function(jqXHR, textStatus, errorThrown) {
             options.error(jqXHR, textStatus, errorThrown);
         }
     });
 };
 
-/* retrieve a singel data identifier */
+/* retrieve a single data identifier */
 RucioClient.prototype.get_did = function(options) {
     check_token();
     var url = this.url + '/dids/' + options.scope + '/' + options.name;
     if (options.dynamic) {
         url += '?dynamic=' + options.dynamic;
     }
     if (options.async == null) {
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/rule.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/rule.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -430,16 +430,16 @@
                 $('#boost_message').html('<font color="green">Successfully updated rule priority</font>');
             },
             error: function(jqXHR, textStatus, errorThrown) {
                 if (jqXHR.status == 500) {
                     $('#boost_message').html('<font color="red">Cannot increase priority at the moment.</font>');
                     return;
                 }
-                excpt = JSON.parse(jqXHR.responseText)
-                $('#boost_message').html('<font color="red">' + excpt['ExceptionMessage'] + '</font>');
+                except = JSON.parse(jqXHR.responseText)
+                $('#boost_message').html('<font color="red">' + except['ExceptionMessage'] + '</font>');
             }
         })
     });
 }
 
 function load_examine() {
     $("#show_examine").html('<div class="row"><div class="large-1 large-centered columns"><img src="/media/spinner.gif"></div></div>');
```

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/rules.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/rules.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/search.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/search.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/select_login_method.css` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/select_login_method.css`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/subscription.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/subscription.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/subscriptionrules.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/subscriptionrules.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/subscriptions.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/subscriptions.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/subscriptions_editor.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/subscriptions_editor.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/suspicious_replicas.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/suspicious_replicas.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/switch.png` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/switch.png`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio/web/ui/static/version.js` & `rucio_webui-34.3.0/lib/rucio/web/ui/static/version.js`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/lib/rucio_webui.egg-info/SOURCES.txt` & `rucio_webui-34.3.0/lib/rucio_webui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/pylintrc` & `rucio_webui-34.3.0/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/requirements.txt` & `rucio_webui-34.3.0/requirements.txt`

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

### Comparing `rucio_webui-34.2.0/setup.py` & `rucio_webui-34.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/setuputil.py` & `rucio_webui-34.3.0/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_abacus_account.py` & `rucio_webui-34.3.0/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_abacus_collection_replica.py` & `rucio_webui-34.3.0/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_abacus_rse.py` & `rucio_webui-34.3.0/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_account.py` & `rucio_webui-34.3.0/tests/test_account.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_account_limits.py` & `rucio_webui-34.3.0/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_api_external_representation.py` & `rucio_webui-34.3.0/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_archive.py` & `rucio_webui-34.3.0/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_auditor.py` & `rucio_webui-34.3.0/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_auditor_hdfs.py` & `rucio_webui-34.3.0/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_auditor_srmdumps.py` & `rucio_webui-34.3.0/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_authentication.py` & `rucio_webui-34.3.0/tests/test_authentication.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_automatix.py` & `rucio_webui-34.3.0/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_bad_replica.py` & `rucio_webui-34.3.0/tests/test_bad_replica.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_bb8.py` & `rucio_webui-34.3.0/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_belleii.py` & `rucio_webui-34.3.0/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_bin_rucio.py` & `rucio_webui-34.3.0/tests/test_bin_rucio.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_boolean.py` & `rucio_webui-34.3.0/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_clients.py` & `rucio_webui-34.3.0/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_common_types.py` & `rucio_webui-34.3.0/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_config.py` & `rucio_webui-34.3.0/tests/test_config.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_conveyor.py` & `rucio_webui-34.3.0/tests/test_conveyor.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_conveyor_submitter.py` & `rucio_webui-34.3.0/tests/test_conveyor_submitter.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_counter.py` & `rucio_webui-34.3.0/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_credential.py` & `rucio_webui-34.3.0/tests/test_credential.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_curl.py` & `rucio_webui-34.3.0/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_daemons.py` & `rucio_webui-34.3.0/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_dataset_replicas.py` & `rucio_webui-34.3.0/tests/test_dataset_replicas.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_db.py` & `rucio_webui-34.3.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_did.py` & `rucio_webui-34.3.0/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_did_meta_plugins.py` & `rucio_webui-34.3.0/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_didtype.py` & `rucio_webui-34.3.0/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_download.py` & `rucio_webui-34.3.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_dumper.py` & `rucio_webui-34.3.0/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_dumper_consistency.py` & `rucio_webui-34.3.0/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_dumper_data_model.py` & `rucio_webui-34.3.0/tests/test_dumper_data_model.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_dumper_path_parsing.py` & `rucio_webui-34.3.0/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_filter_engine.py` & `rucio_webui-34.3.0/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_heartbeat.py` & `rucio_webui-34.3.0/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_hermes.py` & `rucio_webui-34.3.0/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_identity.py` & `rucio_webui-34.3.0/tests/test_identity.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_impl_upload_download.py` & `rucio_webui-34.3.0/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_import_export.py` & `rucio_webui-34.3.0/tests/test_import_export.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_judge_cleaner.py` & `rucio_webui-34.3.0/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_judge_evaluator.py` & `rucio_webui-34.3.0/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_judge_injector.py` & `rucio_webui-34.3.0/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_judge_repairer.py` & `rucio_webui-34.3.0/tests/test_judge_repairer.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_lifetime.py` & `rucio_webui-34.3.0/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_message.py` & `rucio_webui-34.3.0/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_meta_conventions.py` & `rucio_webui-34.3.0/tests/test_meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_meta_did.py` & `rucio_webui-34.3.0/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_module_import.py` & `rucio_webui-34.3.0/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_monitor.py` & `rucio_webui-34.3.0/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_multi_vo.py` & `rucio_webui-34.3.0/tests/test_multi_vo.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_naming_convention.py` & `rucio_webui-34.3.0/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_oauthmanager.py` & `rucio_webui-34.3.0/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_oidc.py` & `rucio_webui-34.3.0/tests/test_oidc.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_permission.py` & `rucio_webui-34.3.0/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_pfns.py` & `rucio_webui-34.3.0/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_ping.py` & `rucio_webui-34.3.0/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_preparer.py` & `rucio_webui-34.3.0/tests/test_preparer.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_qos.py` & `rucio_webui-34.3.0/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_quarantined_replica.py` & `rucio_webui-34.3.0/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_reaper.py` & `rucio_webui-34.3.0/tests/test_reaper.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_redirect.py` & `rucio_webui-34.3.0/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_replica.py` & `rucio_webui-34.3.0/tests/test_replica.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_replica_recoverer.py` & `rucio_webui-34.3.0/tests/test_replica_recoverer.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_replica_sorting.py` & `rucio_webui-34.3.0/tests/test_replica_sorting.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_request.py` & `rucio_webui-34.3.0/tests/test_request.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_root_proxy.py` & `rucio_webui-34.3.0/tests/test_root_proxy.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_rse.py` & `rucio_webui-34.3.0/tests/test_rse.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_rse_expression_parser.py` & `rucio_webui-34.3.0/tests/test_rse_expression_parser.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_rse_lfn2path.py` & `rucio_webui-34.3.0/tests/test_rse_lfn2path.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_rse_protocol_gfal2.py` & `rucio_webui-34.3.0/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_rse_protocol_gfal2_impl.py` & `rucio_webui-34.3.0/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_rse_protocol_posix.py` & `rucio_webui-34.3.0/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_rse_protocol_rclone.py` & `rucio_webui-34.3.0/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_rse_protocol_rsync.py` & `rucio_webui-34.3.0/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_rse_protocol_srm.py` & `rucio_webui-34.3.0/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_rse_protocol_ssh.py` & `rucio_webui-34.3.0/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_rse_protocol_webdav.py` & `rucio_webui-34.3.0/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_rse_protocol_xrootd.py` & `rucio_webui-34.3.0/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_rse_selector.py` & `rucio_webui-34.3.0/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_rucio_server.py` & `rucio_webui-34.3.0/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_rule.py` & `rucio_webui-34.3.0/tests/test_rule.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_schema_cms.py` & `rucio_webui-34.3.0/tests/test_schema_cms.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_scope.py` & `rucio_webui-34.3.0/tests/test_scope.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_subscription.py` & `rucio_webui-34.3.0/tests/test_subscription.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_throttler.py` & `rucio_webui-34.3.0/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_tpc.py` & `rucio_webui-34.3.0/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_trace.py` & `rucio_webui-34.3.0/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_transfer.py` & `rucio_webui-34.3.0/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_transfer_plugins.py` & `rucio_webui-34.3.0/tests/test_transfer_plugins.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_undertaker.py` & `rucio_webui-34.3.0/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio_webui-34.2.0/tests/test_upload.py` & `rucio_webui-34.3.0/tests/test_upload.py`

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

### Comparing `rucio_webui-34.2.0/tests/test_utils.py` & `rucio_webui-34.3.0/tests/test_utils.py`

 * *Files identical despite different names*

