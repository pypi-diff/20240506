# Comparing `tmp/shadowsocks_manager-0.1.4.tar.gz` & `tmp/shadowsocks_manager-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowsocks_manager-0.1.4.tar", last modified: Mon Apr 29 19:12:34 2024, max compression
+gzip compressed data, was "shadowsocks_manager-0.1.5.tar", last modified: Mon May  6 05:00:24 2024, max compression
```

## Comparing `shadowsocks_manager-0.1.4.tar` & `shadowsocks_manager-0.1.5.tar`

### file list

```diff
@@ -1,124 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.864405 shadowsocks_manager-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20803 2024-04-29 19:12:34.864405 shadowsocks_manager-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.848405 shadowsocks_manager-0.1.4/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/bin/ssm-dev-start
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/bin/ssm-dev-stop
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/bin/ssm-setup
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/bin/ssm-test
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-29 19:12:30.000000 shadowsocks_manager-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-29 19:12:34.864405 shadowsocks_manager-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.848405 shadowsocks_manager-0.1.4/shadowsocks_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/.env
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.852405 shadowsocks_manager-0.1.4/shadowsocks_manager/args_formatter/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/args_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/args_formatter/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.852405 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.852405 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/fixtures/nameserver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.852405 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.852405 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.852405 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.856405 shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/auth.group.json
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/sites.site.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.856405 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.856405 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/fixtures/template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.856405 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.856405 shadowsocks_manager-0.1.4/shadowsocks_manager/retry/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/retry/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.856405 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/fixtures/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36795 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    21089 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.864405 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/createsuperuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/uwsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.864405 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20803 2024-04-29 19:12:34.000000 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-29 19:12:34.000000 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:12:34.000000 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-29 19:12:34.000000 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-29 19:12:34.000000 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 19:12:34.000000 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.388720 shadowsocks_manager-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-05-06 05:00:24.388720 shadowsocks_manager-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.372721 shadowsocks_manager-0.1.5/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/bin/ssm-dev-start
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/bin/ssm-dev-stop
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/bin/ssm-setup
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/bin/ssm-test
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-05-06 05:00:20.000000 shadowsocks_manager-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-06 05:00:24.392721 shadowsocks_manager-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.372721 shadowsocks_manager-0.1.5/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.376721 shadowsocks_manager-0.1.5/shadowsocks_manager/args_formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/args_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/args_formatter/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.376721 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.376721 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/fixtures/nameserver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.376721 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.376721 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.380720 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.380720 shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/auth.group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/sites.site.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.380720 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.380720 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/fixtures/template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.380720 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.380720 shadowsocks_manager-0.1.5/shadowsocks_manager/retry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/retry/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/fixtures/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/management/commands/shadowsocks_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36237 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21055 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.388720 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.388720 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.388720 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/createsuperuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/uwsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.388720 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-05-06 05:00:24.000000 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-06 05:00:24.000000 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 05:00:24.000000 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-06 05:00:24.000000 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-06 05:00:24.000000 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 05:00:24.000000 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/top_level.txt
```

### Comparing `shadowsocks_manager-0.1.4/LICENSE` & `shadowsocks_manager-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/PKG-INFO` & `shadowsocks_manager-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.4
+Version: 0.1.5
 Summary: A shadowsocks manager for multi-user and traffic statistics
 Home-page: https://github.com/alexzhangs/shadowsocks-manager
 Author: Alex
 Author-email: Alex <alexzhangs@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Alex Zhang
@@ -133,19 +133,19 @@
         * ~~Pre-installed, and have a builtin service manager.~~
         * No builtin service manager, you need to install it and start the service by yourself.
 
 Code in Python, base on Django, Django REST framework, Celery, and SQLite.
 
 The development status can be found at: [project home](https://github.com/alexzhangs/shadowsocks-manager/projects/1).
 
-Node List:
-![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-list.png)
+Shadowsocks Node List:
+![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-list.png)
 
-Node's Shadowsocks Manager:
-![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-ssmanager.png)
+Add Shadowsocks Node:
+![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-add.png)
 
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
 * Docker
@@ -396,14 +396,20 @@
 1. Link the project code in your workspace to the Python environment
 
     ```sh
     cd shadowsocks-manager
     pip install -e .
     ```
 
+1. Set the SSM_DATA_HOME environment variable (optional, default is Django root directory)
+
+    ```sh
+    export SSM_DATA_HOME=~/.ssm-dev-data
+    ```
+
 1. Configure the shadowsocks-manager
 
     ```sh
     ssm-setup -c -m -l -u admin -p yourpassword
     ```
 
 1. Run the development server
@@ -422,14 +428,17 @@
 
 1. Test the Django code
 
     Make sure the memcached and rabbitmq are running, and also the 3 shadowsocks-libev node are running.
 
     ```sh
     ssm-test -t
+
+    # or use the django test command directly for more options
+    ssm-manage test --no-input -v 2
     ```
 
 1. Test the Django code with coverage
 
     ```sh
     pip install coverage
     ssm-test -c
```

### Comparing `shadowsocks_manager-0.1.4/README.md` & `shadowsocks_manager-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,19 @@
         * ~~Pre-installed, and have a builtin service manager.~~
         * No builtin service manager, you need to install it and start the service by yourself.
 
 Code in Python, base on Django, Django REST framework, Celery, and SQLite.
 
 The development status can be found at: [project home](https://github.com/alexzhangs/shadowsocks-manager/projects/1).
 
-Node List:
-![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-list.png)
+Shadowsocks Node List:
+![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-list.png)
 
-Node's Shadowsocks Manager:
-![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-ssmanager.png)
+Add Shadowsocks Node:
+![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-add.png)
 
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
 * Docker
@@ -301,14 +301,20 @@
 1. Link the project code in your workspace to the Python environment
 
     ```sh
     cd shadowsocks-manager
     pip install -e .
     ```
 
+1. Set the SSM_DATA_HOME environment variable (optional, default is Django root directory)
+
+    ```sh
+    export SSM_DATA_HOME=~/.ssm-dev-data
+    ```
+
 1. Configure the shadowsocks-manager
 
     ```sh
     ssm-setup -c -m -l -u admin -p yourpassword
     ```
 
 1. Run the development server
@@ -327,14 +333,17 @@
 
 1. Test the Django code
 
     Make sure the memcached and rabbitmq are running, and also the 3 shadowsocks-libev node are running.
 
     ```sh
     ssm-test -t
+
+    # or use the django test command directly for more options
+    ssm-manage test --no-input -v 2
     ```
 
 1. Test the Django code with coverage
 
     ```sh
     pip install coverage
     ssm-test -c
```

### Comparing `shadowsocks_manager-0.1.4/bin/ssm-dev-start` & `shadowsocks_manager-0.1.5/bin/ssm-dev-start`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/bin/ssm-setup` & `shadowsocks_manager-0.1.5/bin/ssm-setup`

 * *Files 3% similar despite different names*

```diff
@@ -8,57 +8,52 @@
 #? Usage:
 #?   ssm-setup.sh [-e ENV ...]
 #?                [-c] [-m] [-l] [-u USERNAME -p PASSWORD [-M EMAIL]] [-r PORT_BEGIN] [-R PORT_END] [-h]
 #?
 #? Options:
 #?   [-e ENV ...]
 #?
-#?   Set the environment variables in KEY=VALUE format for .env file.
-#?   The .env file is used by Django settings.
+#?   Set the environment variables in KEY=VALUE format for .ssm-env file.
+#?   The .ssm-env file is used by Django settings.
 #?   This option can be used multiple times.
 #?
 #?   The valid KEYs are:
 #?
 #?   - SSM_SECRET_KEY
 #?
 #?     Set Django's SECRET_KEY.
-#?     The default value is hardcoded in the .env file and Django's settings.
+#?     The default value is hardcoded in the .ssm-env file and Django's settings.
 #?     Do not use the default value in production environment.
 #?     Below command will generate a random SECRET_KEY:
 #?     ```sh
 #?     $ od -vN 25 -An -tx1 /dev/urandom | tr -d ' \n'
 #?     ```
 #?
 #?   - SSM_DEBUG
 #?
 #?     Set Django's DEBUG.
 #?     The value can be 'True' or 'False'.
-#?     The default value depends on the .env file and Django's settings.
+#?     The default value depends on the .ssm-env file and Django's settings.
 #?     Do not use value SSM_DEBUG=True in production environment.
 #?
 #?   - SSM_TIME_ZONE
 #?
 #?     Set Django's TIME_ZONE.
 #?     The value can be any valid timezone name.
-#?     The default value depends on the .env file and Django's settings.
-#?
-#?   - SSM_DATA_HOME
-#?
-#?     Set the base directory for the Django database and static files.
-#?     The default value depends on the .env file and Django's settings.
+#?     The default value depends on the .ssm-env file and Django's settings.
 #?
 #?   - SSM_MEMCACHED_HOST, SSM_MEMCACHED_PORT
 #?
 #?     Set the Memcached server's host and port which are used by Django cache.
-#?     The default value depends on the .env file and Django's settings.
+#?     The default value depends on the .ssm-env file and Django's settings.
 #? 
 #?   - SSM_RABBITMQ_HOST, SSM_RABBITMQ_PORT
 #?
 #?     Set the RabbitMQ server's host and port which are used by Celery.
-#?     The default value depends on the .env file and Django's settings.
+#?     The default value depends on the .ssm-env file and Django's settings.
 #?
 #?   However, this script will not check the validity of the KEYs and VALUEs.
 #?
 #?   [-c]
 #?
 #?   Collect Django static files.
 #?   This is necessary for the first time setup.
```

### Comparing `shadowsocks_manager-0.1.4/bin/ssm-test` & `shadowsocks_manager-0.1.5/bin/ssm-test`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/pyproject.toml` & `shadowsocks_manager-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shadowsocks-manager"
-version = "0.1.4"
+version = "0.1.5"
 requires-python = ">=2.7"
 dependencies = [
     "future",
     "six",
     "boto3",
     "celery",
     "Django<4",
@@ -130,21 +130,21 @@
     "bin/ssm-test",
 ]
 
 [tool.setuptools.packages]
 find = {}
 
 [tool.setuptools.package-data]
-shadowsocks_manager = ["fixtures/*", "**/fixtures/*", ".env"]
+shadowsocks_manager = ["fixtures/*", "**/fixtures/*"]
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [tool.bumpversion]
-current_version = "0.1.4"
+current_version = "0.1.5"
 parse = """
     (?P<major>\\d+)\\.
     (?P<minor>\\d+)\\.
     (?P<patch>\\d+)
     (
         \\-                         # separator
         (?P<suffix>[0-9]\\d*)       # suffix Number
```

### Comparing `shadowsocks_manager-0.1.4/setup.cfg` & `shadowsocks_manager-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shadowsocks-manager
-version = 0.1.4
+version = 0.1.5
 description = A shadowsocks manager for multi-user and traffic statistics
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Alex
 author_email = alexzhangs@gmail.com
 url = https://github.com/alexzhangs/shadowsocks-manager
 license = MIT
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/__main__.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/args_formatter/__init__.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/args_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/args_formatter/tests.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/args_formatter/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/domain/admin.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/domain/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/domain/models.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/domain/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from django.db import models
 from django.db.models.signals import post_save, post_delete
 from django.dispatch import receiver
 from django.contrib.sites.models import Site
 from django.conf import settings
 
 
-logger = logging.getLogger('django')
+logger = logging.getLogger(__name__)
 
 
 # Create your models here.
 
 class Site(Site):
 
     class Meta:
@@ -31,18 +31,23 @@
 
     def __init__(self, user, credential, *args, **kwargs):
         super(BaseNsApi, self).__init__(*args, **kwargs)
         self.user = user
         self.credential = credential
 
     def call_api(self, url, method='get', data=None):
+        if not self.user or not self.credential:
+            logger.error('{0}: User and Credential are required.'.format(self.__class__.__name__))
+            return
+
         response = getattr(requests, method)(
             url,
             auth=(self.user, self.credential),
-            json=data
+            json=data,
+            timeout=30
         )
         return response.json()
 
     def create_record(self, *args, **kwargs):
         pass
 
     def list_records(self, *args, **kwargs):
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/domain/serializers.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/domain/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/domain/tests.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/domain/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 from abc import abstractmethod
 from django.test import TestCase
 
 from domain import models, serializers
 
 
 import logging
-# disable logging for the test module to make the output clean
-logging.disable(logging.CRITICAL)
+# Get a logger for this module
+logger = logging.getLogger(__name__)
+# Set the logging level to make the output clean
+logger.setLevel(logging.ERROR)
 
 
 class BaseTestCase(TestCase):
     """
     A base test case for current app.
     This class is inherited from Django TestCase class, and provides the following features:
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/domain/views.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/domain/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/models.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import six
 
 import types, importlib
 import logging
 from django.db import models
 
 
-logger = logging.getLogger('django')
+logger = logging.getLogger(__name__)
 
 
 # Create your models here.
 
 class DynamicMethodModel(object):
 
     """
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json` & `shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json` & `shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989583333333333%*

 * *Differences: {'3': "{'fields': {'task': 'shadowsocks.tasks.port_heartbeat'}}"}*

```diff
@@ -95,14 +95,14 @@
             "name": "Shadowsocks Port Heartbeat",
             "one_off": false,
             "priority": null,
             "queue": null,
             "routing_key": null,
             "solar": null,
             "start_time": null,
-            "task": "shadowsocksz.tasks.port_heartbeat",
+            "task": "shadowsocks.tasks.port_heartbeat",
             "total_run_count": 0
         },
         "model": "django_celery_beat.periodictask",
         "pk": 5
     }
 ]
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/manage.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/notification/fixtures/template.json` & `shadowsocks_manager-0.1.5/shadowsocks_manager/notification/fixtures/template.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/notification/models.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/notification/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 import subprocess
 from subprocess import PIPE
 from django.db import models
 from django.template import engines
 
 
-logger = logging.getLogger('django')
+logger = logging.getLogger(__name__)
 
 
 # Create your models here.
 
 class Template(models.Model):
     type = models.CharField(max_length=32, choices=[('account_created', 'Account Created')])
     content = models.TextField()
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/notification/tests.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/notification/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 from abc import abstractmethod
 from django.test import TestCase
 
 from notification import models, serializers
 
 
 import logging
-# disable logging for the test module to make the output clean
-logging.disable(logging.CRITICAL)
+# Get a logger for this module
+logger = logging.getLogger(__name__)
+# Set the logging level to make the output clean
+logger.setLevel(logging.ERROR)
 
 
 class BaseTestCase(TestCase):
     """
     A base test case for current app.
     This class is inherited from Django TestCase class, and provides the following features:
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/retry/__init__.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/retry/tests.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/retry/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 
 from unittest import TestCase
 
 from retry import retry
 
 
 import logging
-# disable logging for the test module to make the output clean
-logging.disable(logging.CRITICAL)
+# Get a logger for this module
+logger = logging.getLogger(__name__)
+# Set the logging level to make the output clean
+logger.setLevel(logging.CRITICAL)
 
 
 # Create your tests here.
 class RetryTestCase(TestCase):
     def test_retry_positive(self):
         self.assertTrue(self.call_retryee(n=1, count=0))
         self.assertTrue(self.call_retryee(n=4, count=3))
@@ -27,15 +29,15 @@
     def call_retryee(self, n, count):
         """
         Set the decorator @retry(count=count) on retryee(). Call the retryee(n=n).
         """
         # reset the global counter before calling retryee()
         self.RETRYING = 0
 
-        @retry(count=count, delay=0.1)
+        @retry(count=count, delay=0.1, logger=logger)
         def retryee(n):
             """
             Return True on the Nth time call of this function, return False on otherwise.
             """
             self.RETRYING += 1
             return True if self.RETRYING == n else False
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/celery.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/settings.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,23 +9,36 @@
 For the full list of settings and their values, see
 https://docs.djangoproject.com/en/1.11/ref/settings/
 """
 
 # py2.7 and py3 compatibility imports
 from __future__ import unicode_literals
 
-from decouple import config
+from decouple import Config, RepositoryEnv
 
 import os
 
 
-# Build paths inside the project like this: os.path.join(BASE_DIR, ...)
-BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+def get_env_file(ssm_data_home):
+    env_file = os.path.join(ssm_data_home, '.ssm-env')
+    if not os.path.exists(env_file):
+        # create the .ssm-env file if it does not exist
+        with open(env_file, 'w') as f:
+            f.write('')
+    return env_file
+
+
+# get SSM_DATA_HOME from environment, or use Django root directory as default
+DATA_HOME = os.getenv('SSM_DATA_HOME') or os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+
+# create the DATA_HOME directory if it does not exist
+if not os.path.exists(DATA_HOME):
+    os.makedirs(DATA_HOME)
 
-DATA_HOME = config('SSM_DATA_HOME', default=BASE_DIR)
+config = Config(RepositoryEnv(get_env_file(DATA_HOME)))
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/1.11/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = config('SSM_SECRET_KEY', default='ef24ff499c58a21711385e8a6b31a7680fb41765b8ca0cb451')
 
@@ -56,15 +69,15 @@
     'django.contrib.staticfiles',
     'django.contrib.sites',
     'django_celery_beat',
     'django_celery_results',
     'import_export',
     'rest_framework',
     'django_filters',
-    'shadowsocksz',
+    'shadowsocks',
     'statistic',
     'notification',
     'domain',
 ]
 
 MIDDLEWARE = [
     'django.middleware.security.SecurityMiddleware',
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/urls.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 from django.contrib import admin
 
 
 urlpatterns = [
     url(r'^admin/', admin.site.urls),
     url(r'^api-auth/', include('rest_framework.urls', namespace='rest_framework')),
     url(r'^', include('notification.urls')),
-    url(r'^', include('shadowsocksz.urls')),
+    url(r'^', include('shadowsocks.urls')),
     url(r'^', include('statistic.urls')),
     url(r'^', include('domain.urls')),
 ]
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/admin.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 
 class SSManagerInline(admin.TabularInline):
     model = SSManager
     extra = 1
     max_num = 1
 
-    fields = ('interface', 'port', 'encrypt', 'timeout', 'fastopen', 'is_accessible',
+    fields = ('interface', 'port', 'encrypt', 'is_accessible',
               'server_edition', 'is_v2ray_enabled',)
     readonly_fields = ('is_accessible', 'is_v2ray_enabled', 'dt_created', 'dt_updated')
 
     def is_accessible(self, obj):
         return obj.is_accessible
 
     is_accessible.boolean = True
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/management/commands/shadowsocks_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.core.management.base import BaseCommand
-from shadowsocksz.models import Config
+from shadowsocks.models import Config
 
 class Command(BaseCommand):
-    help = 'Set shadowsocksz config parameters'
+    help = 'Set shadowsocks config parameters'
     django_default_options = ('verbosity', 'settings', 'pythonpath', 'traceback', 'no_color', 
                        'force_color', 'skip_checks')
 
     def add_arguments(self, parser):
         parser.add_argument('--port-begin', type=int, nargs='?')
         parser.add_argument('--port-end', type=int, nargs='?')
         parser.add_argument('--timeout-remote', type=float, nargs='?')
@@ -17,8 +17,8 @@
         for key, value in options.items():
             if key in self.django_default_options:
                 # skip django default options
                 continue
 
             if value is not None:
                 Config.objects.update(**{key: value})
-                self.stdout.write(self.style.SUCCESS(f'Successfully set shadowsocksz.config.{key} to {value}'))
+                self.stdout.write(self.style.SUCCESS(f'Successfully set shadowsocks.config.{key} to {value}'))
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/models.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from retry import retry
 from singleton.models import SingletonModel
 from dynamicmethod.models import DynamicMethodModel
 from notification.models import Template, Notify
 from domain.models import Record
 
 
-logger = logging.getLogger('django')
+logger = logging.getLogger(__name__)
 
 
 # Create your models here.
 
 class Config(SingletonModel):
     port_begin = models.PositiveIntegerField('Begin port', default=8381,
         help_text='Port range allowed for all Shadowsocks nodes, make sure they are opened '
@@ -543,19 +543,14 @@
         help_text='Port number bound to Manager API.')
     encrypt = models.CharField(max_length=32, default='aes-256-cfb',
         help_text='Encrypt method: rc4-md5, aes-128-gcm, aes-192-gcm, aes-256-gcm, '
             'aes-128-cfb, aes-192-cfb, aes-256-cfb, aes-128-ctr, aes-192-ctr, aes-256-ctr, '
             'camellia-128-cfb, camellia-192-cfb, camellia-256-cfb, bf-cfb, chacha20-ietf-poly1305, '
             'xchacha20-ietf-poly1305, salsa20, chacha20 and chacha20-ietf. '
             'The changes made here will not affect the plugin status on server.')
-    timeout = models.PositiveIntegerField(default=30,
-        help_text='Socket timeout in seconds for Shadowsocks client. '
-            'The changes made here will not affect the plugin status on server.')
-    fastopen = models.BooleanField('Fast Open', default=False,
-        help_text='Enable TCP fast open, with Linux kernel > 3.7.0.')
     server_edition = enum.EnumField(ServerEditionList, default=ServerEditionList.LIBEV,
         help_text='The Shadowsocks server edition. The libev edition is recommended.')
     is_v2ray_enabled = models.BooleanField(default=False,
         help_text='Whether the v2ray-plugin is enabled for Shadowsocks server. The changes made here will not '
             'affect the plugin status on server.')
     dt_created = models.DateTimeField('Created', auto_now_add=True)
     dt_updated = models.DateTimeField('Updated', auto_now=True)
@@ -814,16 +809,15 @@
     This class is used to manage the local Shadowsocks server python edition.
     The usage of this class is removed from the SSManager model.
     """
 
     def __init__(self, manager, *args, **kwargs):
         super(SSServer, self).__init__(*args, **kwargs)
         self.manager = manager
-        # the lift_pip_shadowsocks is no longer needed after the django app shadowsocks was renamed to shadowsocksz
-        # self.lift_pip_shadowsocks()
+        self.lift_pip_shadowsocks()
 
     def pidfile(self, original=False):
         return '/tmp/shadowsocks-{}.pid'.format(self.manager._original_port if original else self.manager.port)
 
     def logfile(self, original=False):
         return '/tmp/shadowsocks-{}.log'.format(self.manager._original_port if original else self.manager.port)
 
@@ -952,16 +946,14 @@
             '--manager-address', '{}:{}'.format(self.manager._ip, self.manager.port),  # the options order matters
             # The shadowsocks python edition does not support to run the manager without a server port.
             # So, the server port is set to 65500, which is not supposed to be used by any client.
             # And the password is set to a random string, which is not supposed to be known by any client.
             '-p 65500',  
             '-k', self.random_password(),
             '-m', self.manager.encrypt,
-            '-t', str(self.manager.timeout),
-            '--fast-open', str(self.manager.fastopen),
         ]
         """
         * close_fds=True: For Python 2.7, should not inherit the parent process's fds. The inherit fds won't be released
                           after the parent process was exited but the child process remains.
                           Here's the Django server's process that's bound with a port.
         """
         (rc, stdout, stderr) = self.call(command, close_fds=True)
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/serializers.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,11 +31,11 @@
         model = models.NodeAccount
         fields = ('id', 'node', 'account', 'is_active', 'dt_created', 'dt_updated')
 
 
 class SSManagerSerializer(serializers.ModelSerializer):
     class Meta:
         model = models.SSManager
-        fields = ('id', 'node', 'interface', 'port', 'encrypt', 'timeout', 'fastopen', 'server_edition', 'is_v2ray_enabled', 'dt_created', 'dt_updated')
+        fields = ('id', 'node', 'interface', 'port', 'encrypt', 'server_edition', 'is_v2ray_enabled', 'dt_created', 'dt_updated')
 
     interface = EnumField(models.InterfaceList)
     server_edition = EnumField(models.ServerEditionList)
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/tests.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 from abc import abstractmethod
 from django.test import TestCase
 from django.core.exceptions import ValidationError
 
 from domain.models import Record
 from domain.tests import AppTestCase as DomainAppTestCase
 from notification.tests import AppTestCase as NotificationAppTestCase
-from shadowsocksz import models, serializers
+from shadowsocks import models, serializers
 
 
 import logging
-# disable logging for the test module to make the output clean
-logging.disable(logging.CRITICAL)
+# Get a logger for this module
+logger = logging.getLogger(__name__)
+# Set the logging level to make the output clean
+logger.setLevel(logging.ERROR)
 
 
 import socket
 def get_local_ip():
     """
     Get the local ip address.
     https://github.com/mayermakes/Get_IP
@@ -436,15 +438,14 @@
         #   --name ssm-ss-libev-localhost shadowsocks/shadowsocks-libev:edge \
         #   ss-manager --manager-address 0.0.0.0:$MGR_PORT --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
 
         models.SSManager(
             node=models.Node.objects.get(name='ss-libev-localhost'),
             interface=models.InterfaceList.LOCALHOST,
             port=6001,
-            fastopen=False,
             encrypt='aes-256-cfb',
             server_edition=models.ServerEditionList.LIBEV,
             is_v2ray_enabled=False,
         ).save()
 
         # Add a libev edition manager to the private node
         # Make sure this manager is running and accessible at private ip before the test.
@@ -453,15 +454,14 @@
         # docker run -d -p <private_ip>:$MGR_PORT:$MGR_PORT/UDP -p <private_ip>:$SS_PORTS:$SS_PORTS/UDP -p <private_ip>:$SS_PORTS:$SS_PORTS \
         #   --name ssm-ss-libev-private shadowsocks/shadowsocks-libev:edge \
         #   ss-manager --manager-address 0.0.0.0:$MGR_PORT --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
         models.SSManager(
             node=models.Node.objects.get(name='ss-libev-private'),
             interface=models.InterfaceList.PRIVATE,
             port=6002,
-            fastopen=False,
             encrypt='aes-256-cfb',
             server_edition=models.ServerEditionList.LIBEV,
             is_v2ray_enabled=False,
         ).save()
 
         # Add a libev edition manager to the public node
         # Make sure this manager is running and accessible at private ip before the test.
@@ -470,15 +470,14 @@
         # docker run -d -p <private_ip>:$MGR_PORT:$MGR_PORT/UDP -p <private_ip>:$SS_PORTS:$SS_PORTS/UDP -p <private_ip>:$SS_PORTS:$SS_PORTS \
         #   --name ssm-ss-libev-public shadowsocks/shadowsocks-libev:edge \
         #   ss-manager --manager-address 0.0.0.0:$MGR_PORT --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
         models.SSManager(
             node=models.Node.objects.get(name='ss-libev-public'),
             interface=models.InterfaceList.PUBLIC,
             port=6003,
-            fastopen=False,
             encrypt='aes-256-cfb',
             server_edition=models.ServerEditionList.LIBEV,
             is_v2ray_enabled=False,
         ).save()
 
     @classmethod
     def setUpTestData(cls):
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/urls.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from django.conf.urls import url, include
 from rest_framework import routers
 
 from . import views
 
 
 router = routers.DefaultRouter()
-router.register(r'shadowsocksz/config', views.ConfigViewSet)
-router.register(r'shadowsocksz/account', views.AccountViewSet)
-router.register(r'shadowsocksz/node', views.NodeViewSet)
-router.register(r'shadowsocksz/nodeaccount', views.NodeAccountViewSet)
-router.register(r'shadowsocksz/ssmanager', views.SSManagerViewSet)
+router.register(r'shadowsocks/config', views.ConfigViewSet)
+router.register(r'shadowsocks/account', views.AccountViewSet)
+router.register(r'shadowsocks/node', views.NodeViewSet)
+router.register(r'shadowsocks/nodeaccount', views.NodeAccountViewSet)
+router.register(r'shadowsocks/ssmanager', views.SSManagerViewSet)
 
 urlpatterns = [
     url(r'^', include(router.urls)),
 ]
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/views.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/models.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import unicode_literals
 
 import logging
 from django.db import models
 from django.core.cache import cache
 
 
-logger = logging.getLogger('django')
+logger = logging.getLogger(__name__)
 
 
 # Create your models here.
 
 class SingletonModel(models.Model):
 
     class Meta:
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/admin.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/models.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import logging
 from django.db import models
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.utils import timezone
 from django_lock import lock
 
-from shadowsocksz.models import Node, Account, NodeAccount
+from shadowsocks.models import Node, Account, NodeAccount
 
 
-logger = logging.getLogger('django')
+logger = logging.getLogger(__name__)
 
 
 # Create your models here.
 
 class Period(models.Model):
     year = models.PositiveIntegerField(null=True, blank=True)
     month = models.PositiveIntegerField(null=True, blank=True)
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/serializers.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/tests.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from __future__ import unicode_literals
 from __future__ import absolute_import
 
 import json
 from abc import abstractmethod
 from django.test import TestCase
 
-from shadowsocksz.tests import AppTestCase as ShadowsockszAppTestCase
+from shadowsocks.tests import AppTestCase as shadowsocksAppTestCase
 from statistic import models, serializers
 
 
 import logging
-# disable logging for the test module to make the output clean
-logging.disable(logging.CRITICAL)
+# Get a logger for this module
+logger = logging.getLogger(__name__)
+# Set the logging level to make the output clean
+logger.setLevel(logging.ERROR)
 
 
 class BaseTestCase(TestCase):
     """
     A base test case for current app.
     This class is inherited from Django TestCase class, and provides the following features:
 
@@ -69,28 +71,28 @@
         """
         for testcase in [globals().get(name) for name in cls.testcases]:
             method = getattr(testcase or {}, 'down', None)
             if method: method()
 
 
 class AppTestCase(BaseTestCase):
-    fixtures = ShadowsockszAppTestCase.fixtures
+    fixtures = shadowsocksAppTestCase.fixtures
     testcases = []
 
 
 class PeriodTestCase(AppTestCase):
     def test_period_serializer(self):
         obj = serializers.PeriodSerializer()
         json.loads(json.dumps(obj.to_representation(models.Period.objects.first())))
 
 
 class StatisticTestCase(AppTestCase):
     @classmethod
     def setUpTestData(cls):
-        ShadowsockszAppTestCase.allup()
+        shadowsocksAppTestCase.allup()
 
     def test_statistic_statistic(self):
         # no statistics data is asserted, cause there's no Manager API really called.
         models.Statistic.statistic()
 
         obj = serializers.StatisticSerializer()
         json.loads(json.dumps(obj.to_representation(models.Statistic.objects.first())))
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/views.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/utils/celery.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/utils/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/utils/createsuperuser.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/utils/createsuperuser.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     -p --password=PASSWORD     Password for the superuser account.
     -e --email=EMAIL           Email for the superuser account.
 
 Returns:
     None
 
 Example:
-    ssm-createsuperuser -u admin -p admin123 -e admin@example.com
+    $ ssm-createsuperuser -u admin -p admin123 -e admin@example.com
 """
 import os
 import sys
 from docopt import docopt
 
 
 def create_superuser(username, password, email):
@@ -36,15 +36,15 @@
     import django
     django.setup()
 
     from django.contrib.auth.models import User
     User.objects.filter(username=username).delete()
     User.objects.create_superuser(username, email, password)
 
-    print("Superuser '{username}' created successfully.")
+    print("Superuser '{0}' created successfully.".format(username))
 
 
 def main():
     arguments = docopt(__doc__)
 
     username = arguments["--username"]
     password = arguments["--password"]
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager/utils/manage.py` & `shadowsocks_manager-0.1.5/shadowsocks_manager/utils/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/PKG-INFO` & `shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.4
+Version: 0.1.5
 Summary: A shadowsocks manager for multi-user and traffic statistics
 Home-page: https://github.com/alexzhangs/shadowsocks-manager
 Author: Alex
 Author-email: Alex <alexzhangs@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Alex Zhang
@@ -133,19 +133,19 @@
         * ~~Pre-installed, and have a builtin service manager.~~
         * No builtin service manager, you need to install it and start the service by yourself.
 
 Code in Python, base on Django, Django REST framework, Celery, and SQLite.
 
 The development status can be found at: [project home](https://github.com/alexzhangs/shadowsocks-manager/projects/1).
 
-Node List:
-![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-list.png)
+Shadowsocks Node List:
+![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-list.png)
 
-Node's Shadowsocks Manager:
-![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-ssmanager.png)
+Add Shadowsocks Node:
+![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-add.png)
 
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
 * Docker
@@ -396,14 +396,20 @@
 1. Link the project code in your workspace to the Python environment
 
     ```sh
     cd shadowsocks-manager
     pip install -e .
     ```
 
+1. Set the SSM_DATA_HOME environment variable (optional, default is Django root directory)
+
+    ```sh
+    export SSM_DATA_HOME=~/.ssm-dev-data
+    ```
+
 1. Configure the shadowsocks-manager
 
     ```sh
     ssm-setup -c -m -l -u admin -p yourpassword
     ```
 
 1. Run the development server
@@ -422,14 +428,17 @@
 
 1. Test the Django code
 
     Make sure the memcached and rabbitmq are running, and also the 3 shadowsocks-libev node are running.
 
     ```sh
     ssm-test -t
+
+    # or use the django test command directly for more options
+    ssm-manage test --no-input -v 2
     ```
 
 1. Test the Django code with coverage
 
     ```sh
     pip install coverage
     ssm-test -c
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/SOURCES.txt` & `shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 setup.cfg
 setup.py
 bin/ssm-dev-start
 bin/ssm-dev-stop
 bin/ssm-setup
 bin/ssm-test
-shadowsocks_manager/.env
 shadowsocks_manager/__init__.py
 shadowsocks_manager/__main__.py
 shadowsocks_manager/manage.py
 shadowsocks_manager.egg-info/PKG-INFO
 shadowsocks_manager.egg-info/SOURCES.txt
 shadowsocks_manager.egg-info/dependency_links.txt
 shadowsocks_manager.egg-info/entry_points.txt
@@ -49,33 +48,33 @@
 shadowsocks_manager/notification/tests.py
 shadowsocks_manager/notification/urls.py
 shadowsocks_manager/notification/views.py
 shadowsocks_manager/notification/fixtures/template.json
 shadowsocks_manager/notification/migrations/__init__.py
 shadowsocks_manager/retry/__init__.py
 shadowsocks_manager/retry/tests.py
+shadowsocks_manager/shadowsocks/__init__.py
+shadowsocks_manager/shadowsocks/admin.py
+shadowsocks_manager/shadowsocks/apps.py
+shadowsocks_manager/shadowsocks/models.py
+shadowsocks_manager/shadowsocks/serializers.py
+shadowsocks_manager/shadowsocks/tasks.py
+shadowsocks_manager/shadowsocks/tests.py
+shadowsocks_manager/shadowsocks/urls.py
+shadowsocks_manager/shadowsocks/views.py
+shadowsocks_manager/shadowsocks/fixtures/config.json
+shadowsocks_manager/shadowsocks/management/__init__.py
+shadowsocks_manager/shadowsocks/management/commands/__init__.py
+shadowsocks_manager/shadowsocks/management/commands/shadowsocks_config.py
+shadowsocks_manager/shadowsocks/migrations/__init__.py
 shadowsocks_manager/shadowsocks_manager/__init__.py
 shadowsocks_manager/shadowsocks_manager/celery.py
 shadowsocks_manager/shadowsocks_manager/settings.py
 shadowsocks_manager/shadowsocks_manager/urls.py
 shadowsocks_manager/shadowsocks_manager/wsgi.py
-shadowsocks_manager/shadowsocksz/__init__.py
-shadowsocks_manager/shadowsocksz/admin.py
-shadowsocks_manager/shadowsocksz/apps.py
-shadowsocks_manager/shadowsocksz/models.py
-shadowsocks_manager/shadowsocksz/serializers.py
-shadowsocks_manager/shadowsocksz/tasks.py
-shadowsocks_manager/shadowsocksz/tests.py
-shadowsocks_manager/shadowsocksz/urls.py
-shadowsocks_manager/shadowsocksz/views.py
-shadowsocks_manager/shadowsocksz/fixtures/config.json
-shadowsocks_manager/shadowsocksz/management/__init__.py
-shadowsocks_manager/shadowsocksz/management/commands/__init__.py
-shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py
-shadowsocks_manager/shadowsocksz/migrations/__init__.py
 shadowsocks_manager/singleton/__init__.py
 shadowsocks_manager/singleton/admin.py
 shadowsocks_manager/singleton/apps.py
 shadowsocks_manager/singleton/models.py
 shadowsocks_manager/singleton/tests.py
 shadowsocks_manager/singleton/views.py
 shadowsocks_manager/singleton/migrations/__init__.py
```

### Comparing `shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/requires.txt` & `shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/requires.txt`

 * *Files identical despite different names*

