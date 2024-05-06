# Comparing `tmp/detect_secrets-1.4.0.tar.gz` & `tmp/detect_secrets-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detect_secrets-1.4.0.tar", last modified: Tue Oct  4 19:56:25 2022, max compression
+gzip compressed data, was "detect_secrets-1.5.0.tar", last modified: Mon May  6 17:46:14 2024, max compression
```

## Comparing `detect_secrets-1.4.0.tar` & `detect_secrets-1.5.0.tar`

### file list

```diff
@@ -1,108 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.540974 detect_secrets-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10834 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    28759 2022-10-04 19:56:25.540974 detect_secrets-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    22675 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.532974 detect_secrets-1.4.0/detect_secrets/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.536974 detect_secrets-1.4.0/detect_secrets/audit/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/audit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/audit/analytics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3345 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/audit/audit.py
--rw-r--r--   0 runner    (1001) docker     (121)     6869 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/audit/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     8770 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/audit/compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     4117 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/audit/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/audit/iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2975 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/audit/report.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.536974 detect_secrets-1.4.0/detect_secrets/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4812 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/baseline.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.536974 detect_secrets-1.4.0/detect_secrets/core/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/plugins/initialize.py
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/plugins/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     4851 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/potential_secret.py
--rw-r--r--   0 runner    (1001) docker     (121)    14197 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/scan.py
--rw-r--r--   0 runner    (1001) docker     (121)    11801 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/secrets_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.536974 detect_secrets-1.4.0/detect_secrets/core/upgrades/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/upgrades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/upgrades/v0_12.py
--rw-r--r--   0 runner    (1001) docker     (121)     4215 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/upgrades/v1_0.py
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/upgrades/v1_1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.536974 detect_secrets-1.4.0/detect_secrets/core/usage/
--rw-r--r--   0 runner    (1001) docker     (121)     6446 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3199 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/usage/audit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/usage/baseline.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/usage/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     8280 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/usage/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     5294 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/usage/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/core/usage/scan.py
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.536974 detect_secrets-1.4.0/detect_secrets/filters/
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3015 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/filters/allowlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/filters/common.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.536974 detect_secrets-1.4.0/detect_secrets/filters/gibberish/
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/filters/gibberish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8602 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/filters/gibberish/rfc.model
--rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/filters/heuristic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/filters/regex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/filters/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/filters/wordlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     5185 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.540974 detect_secrets-1.4.0/detect_secrets/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/artifactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/aws.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/azure_storage_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     8256 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     3885 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/cloudant.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/discord.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/github_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     7207 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/high_entropy_strings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/ibm_cloud_iam.py
--rw-r--r--   0 runner    (1001) docker     (121)     5345 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/ibm_cos_hmac.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)    12124 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/keyword.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/mailchimp.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/npm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2044 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/private_key.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/sendgrid.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/slack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/softlayer.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/square_oauth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/stripe.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/plugins/twilio.py
--rw-r--r--   0 runner    (1001) docker     (121)     4748 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/pre_commit_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)    10345 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.540974 detect_secrets-1.4.0/detect_secrets/transformers/
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/transformers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8682 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/transformers/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/transformers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12202 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/transformers/yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.540974 detect_secrets-1.4.0/detect_secrets/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3254 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/util/code_snippet.py
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/util/color.py
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/util/filetype.py
--rw-r--r--   0 runner    (1001) docker     (121)     1718 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/util/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     3705 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/util/importlib.py
--rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/util/inject.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/util/path.py
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/detect_secrets/util/semver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 19:56:25.532974 detect_secrets-1.4.0/detect_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    28759 2022-10-04 19:56:25.000000 detect_secrets-1.4.0/detect_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2022-10-04 19:56:25.000000 detect_secrets-1.4.0/detect_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-04 19:56:25.000000 detect_secrets-1.4.0/detect_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-10-04 19:56:25.000000 detect_secrets-1.4.0/detect_secrets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-04 19:56:25.000000 detect_secrets-1.4.0/detect_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-04 19:56:25.000000 detect_secrets-1.4.0/detect_secrets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-04 19:56:25.540974 detect_secrets-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-10-04 19:56:22.000000 detect_secrets-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.315737 detect_secrets-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28879 2024-05-06 17:46:14.315737 detect_secrets-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22770 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.303737 detect_secrets-1.5.0/detect_secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.303737 detect_secrets-1.5.0/detect_secrets/audit/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/audit/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/audit/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/audit/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/audit/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/audit/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/audit/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/audit/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.307737 detect_secrets-1.5.0/detect_secrets/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.307737 detect_secrets-1.5.0/detect_secrets/core/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/plugins/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/plugins/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/potential_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14484 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11916 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/secrets_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.307737 detect_secrets-1.5.0/detect_secrets/core/upgrades/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/upgrades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/upgrades/v0_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/upgrades/v1_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/upgrades/v1_1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.307737 detect_secrets-1.5.0/detect_secrets/core/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/usage/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/usage/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/usage/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/usage/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/usage/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/core/usage/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.307737 detect_secrets-1.5.0/detect_secrets/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/filters/allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/filters/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.311737 detect_secrets-1.5.0/detect_secrets/filters/gibberish/
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/filters/gibberish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/filters/gibberish/rfc.model
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/filters/heuristic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/filters/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/filters/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/filters/wordlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.315737 detect_secrets-1.5.0/detect_secrets/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/azure_storage_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/cloudant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/github_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/gitlab_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/high_entropy_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/ibm_cloud_iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/ibm_cos_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/ip_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/mailchimp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/npm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/pypi_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/sendgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/softlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/square_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/telegram_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/plugins/twilio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/pre_commit_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.315737 detect_secrets-1.5.0/detect_secrets/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/transformers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/transformers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/transformers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/transformers/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.315737 detect_secrets-1.5.0/detect_secrets/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/util/code_snippet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/util/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/util/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/util/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/util/importlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/util/inject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/util/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/detect_secrets/util/semver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:46:14.303737 detect_secrets-1.5.0/detect_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28879 2024-05-06 17:46:14.000000 detect_secrets-1.5.0/detect_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-06 17:46:14.000000 detect_secrets-1.5.0/detect_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:46:14.000000 detect_secrets-1.5.0/detect_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-06 17:46:14.000000 detect_secrets-1.5.0/detect_secrets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 17:46:14.000000 detect_secrets-1.5.0/detect_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 17:46:14.000000 detect_secrets-1.5.0/detect_secrets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-06 17:46:14.315737 detect_secrets-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-06 17:46:12.000000 detect_secrets-1.5.0/setup.py
```

### Comparing `detect_secrets-1.4.0/LICENSE` & `detect_secrets-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/PKG-INFO` & `detect_secrets-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: detect_secrets
-Version: 1.4.0
+Version: 1.5.0
 Summary: Tool for detecting secrets in the codebase
 Home-page: https://github.com/Yelp/detect-secrets
-Author: Aaron Loo
-Author-email: aaronloo@yelp.com
-License: Copyright Yelp, Inc. 2020
-Download-URL: https://github.com/Yelp/detect-secrets/archive/1.4.0.tar.gz
+Author: Yelp, Inc.
+Author-email: opensource@yelp.com
+License: UNKNOWN
+Download-URL: https://github.com/Yelp/detect-secrets/archive/1.5.0.tar.gz
 Description: [![Build Status](https://github.com/Yelp/detect-secrets/actions/workflows/ci.yml/badge.svg)](https://github.com/Yelp/detect-secrets/actions/workflows/ci.yml?query=branch%3Amaster++)
         [![PyPI version](https://badge.fury.io/py/detect-secrets.svg)](https://badge.fury.io/py/detect-secrets)
         [![Homebrew](https://img.shields.io/badge/dynamic/json.svg?url=https://formulae.brew.sh/api/formula/detect-secrets.json&query=$.versions.stable&label=homebrew)](https://formulae.brew.sh/formula/detect-secrets)
         [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-ff69b4.svg)](https://github.com/Yelp/detect-secrets/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22+)
         [![AMF](https://img.shields.io/badge/Donate-Charity-orange.svg)](https://www.againstmalaria.com/donation.aspx)
         
         # detect-secrets
@@ -103,28 +103,33 @@
         ArtifactoryDetector
         AWSKeyDetector
         AzureStorageKeyDetector
         BasicAuthDetector
         CloudantDetector
         DiscordBotTokenDetector
         GitHubTokenDetector
+        GitLabTokenDetector
         Base64HighEntropyString
         HexHighEntropyString
         IbmCloudIamDetector
         IbmCosHmacDetector
+        IPPublicDetector
         JwtTokenDetector
         KeywordDetector
         MailchimpDetector
         NpmDetector
+        OpenAIDetector
         PrivateKeyDetector
+        PypiTokenDetector
         SendGridDetector
         SlackDetector
         SoftlayerDetector
         SquareOAuthDetector
         StripeDetector
+        TelegramBotTokenDetector
         TwilioKeyDetector
         ```
         
         ### Disabling Plugins:
         
         ```bash
         $ detect-secrets scan --disable-plugin KeywordDetector --disable-plugin AWSKeyDetector
@@ -397,15 +402,15 @@
         We recommend setting this up as a pre-commit hook. One way to do this is by using the
         [pre-commit](https://github.com/pre-commit/pre-commit) framework:
         
         ```yaml
         # .pre-commit-config.yaml
         repos:
         -   repo: https://github.com/Yelp/detect-secrets
-            rev: v1.4.0
+            rev: v1.5.0
             hooks:
             -   id: detect-secrets
                 args: ['--baseline', '.secrets.baseline']
                 exclude: package.lock.json
         ```
         
         #### Inline Allowlisting
```

### Comparing `detect_secrets-1.4.0/README.md` & `detect_secrets-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,28 +94,33 @@
 ArtifactoryDetector
 AWSKeyDetector
 AzureStorageKeyDetector
 BasicAuthDetector
 CloudantDetector
 DiscordBotTokenDetector
 GitHubTokenDetector
+GitLabTokenDetector
 Base64HighEntropyString
 HexHighEntropyString
 IbmCloudIamDetector
 IbmCosHmacDetector
+IPPublicDetector
 JwtTokenDetector
 KeywordDetector
 MailchimpDetector
 NpmDetector
+OpenAIDetector
 PrivateKeyDetector
+PypiTokenDetector
 SendGridDetector
 SlackDetector
 SoftlayerDetector
 SquareOAuthDetector
 StripeDetector
+TelegramBotTokenDetector
 TwilioKeyDetector
 ```
 
 ### Disabling Plugins:
 
 ```bash
 $ detect-secrets scan --disable-plugin KeywordDetector --disable-plugin AWSKeyDetector
@@ -388,15 +393,15 @@
 We recommend setting this up as a pre-commit hook. One way to do this is by using the
 [pre-commit](https://github.com/pre-commit/pre-commit) framework:
 
 ```yaml
 # .pre-commit-config.yaml
 repos:
 -   repo: https://github.com/Yelp/detect-secrets
-    rev: v1.4.0
+    rev: v1.5.0
     hooks:
     -   id: detect-secrets
         args: ['--baseline', '.secrets.baseline']
         exclude: package.lock.json
 ```
 
 #### Inline Allowlisting
```

### Comparing `detect_secrets-1.4.0/detect_secrets/audit/analytics.py` & `detect_secrets-1.5.0/detect_secrets/audit/analytics.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,15 +54,22 @@
         else:
             counter.unknown += 1
 
     def _get_plugin_counter(self, secret_type: str) -> 'StatisticsCounter':
         return cast(StatisticsCounter, self.data[secret_type]['stats'])
 
     def __str__(self) -> str:
-        raise NotImplementedError
+        output = ''
+
+        for secret_type, framework in self.data.items():
+            output += f'Plugin: {get_mapping_from_secret_type_to_class()[secret_type].__name__}\n'
+            for value in framework.values():
+                output += f'Statistics: {value}\n\n'
+
+        return output
 
     def json(self) -> Dict[str, Any]:
         output = {}
         for secret_type, framework in self.data.items():
             output[get_mapping_from_secret_type_to_class()[secret_type].__name__] = {
                 key: value.json()
                 for key, value in framework.items()
@@ -73,27 +80,44 @@
 
 class StatisticsCounter:
     def __init__(self) -> None:
         self.correct: int = 0
         self.incorrect: int = 0
         self.unknown: int = 0
 
-    def __repr__(self) -> str:
+    def __str__(self) -> str:
         return (
-            f'{self.__class__.__name__}(correct={self.correct}, '
-            'incorrect={self.incorrect}, unknown={self.unknown},)'
+            f'True Positives: {self.correct}, False Positives: {self.incorrect}, '
+            f'Unknown: {self.unknown}, Precision: {self.calculate_precision()}, '
+            f'Recall: {self.calculate_recall()}'
         )
 
     def json(self) -> Dict[str, Any]:
+        return {
+            'raw': {
+                'true-positives': self.correct,
+                'false-positives': self.incorrect,
+                'unknown': self.unknown,
+            },
+            'score': {
+                'precision': self.calculate_precision(),
+                'recall': self.calculate_recall(),
+            },
+        }
+
+    def calculate_precision(self) -> float:
         precision = (
             round(float(self.correct) / (self.correct + self.incorrect), 4)
             if (self.correct and self.incorrect)
             else 0.0
         )
 
+        return precision
+
+    def calculate_recall(self) -> float:
         # NOTE(2020-11-08|domanchi): This isn't the formal definition of `recall`, however,
         # this is the definition that we're going to attribute to it.
         #
         # Rationale: If we follow the formal definition of `recall` (i.e. TP / (TP + FN)),
         # we would need some way to measure false negatives. However, this is impossible
         # since we don't know what we don't know. The only way to get proper "recall" is
         # to measure this against a known set of secrets, and see how effective our rules
@@ -120,18 +144,8 @@
         # definition of `recall` allows us to do this.
         recall = (
             round(float(self.correct) / (self.correct + self.unknown), 4)
             if (self.correct + self.unknown)
             else 0.0
         )
 
-        return {
-            'raw': {
-                'true-positives': self.correct,
-                'false-positives': self.incorrect,
-                'unknown': self.unknown,
-            },
-            'score': {
-                'precision': precision,
-                'recall': recall,
-            },
-        }
+        return recall
```

### Comparing `detect_secrets-1.4.0/detect_secrets/audit/audit.py` & `detect_secrets-1.5.0/detect_secrets/audit/audit.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if decision == io.InputOptions.QUIT:
             io.print_message('Quitting...')
             break
 
         if decision == io.InputOptions.BACK:
             iterator.step_back_on_next_iteration()
 
-        # The question asked is: "Should this be committed to the repository?"
+        # The question asked is: "Should this string be committed to the repository?"
         elif decision == io.InputOptions.NO:
             secret.is_secret = True
             has_changes = True
         elif decision == io.InputOptions.YES:
             secret.is_secret = False
             has_changes = True
         elif decision == io.InputOptions.SKIP and secret.is_secret is not None:
```

### Comparing `detect_secrets-1.4.0/detect_secrets/audit/common.py` & `detect_secrets-1.5.0/detect_secrets/audit/common.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/audit/compare.py` & `detect_secrets-1.5.0/detect_secrets/audit/compare.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/audit/io.py` & `detect_secrets-1.5.0/detect_secrets/audit/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,14 @@
         options.append(InputOptions.QUIT)
 
         self.valid_input = {option.name[0] for option in options}
         self.options = [option.name.lower() for option in options]
 
     def __str__(self) -> str:
         if 'Y' in self.valid_input:
-            output = 'Is this a secret that should be committed to this repository?'
+            output = 'Should this string be committed to the repository?'
         else:
             output = 'What would you like to do?'
 
         options = ', '.join([f'({option[0]}){option[1:]}' for option in self.options])
 
         return output + ' ' + options + ': '
```

### Comparing `detect_secrets-1.4.0/detect_secrets/audit/iterator.py` & `detect_secrets-1.5.0/detect_secrets/audit/iterator.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/audit/report.py` & `detect_secrets-1.5.0/detect_secrets/audit/report.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/core/baseline.py` & `detect_secrets-1.5.0/detect_secrets/core/baseline.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/core/log.py` & `detect_secrets-1.5.0/detect_secrets/core/log.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/core/plugins/initialize.py` & `detect_secrets-1.5.0/detect_secrets/core/plugins/initialize.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,25 @@
         raise
 
 
 def from_plugin_classname(classname: str) -> Plugin:
     """
     :raises: TypeError
     """
-    for plugin_type in get_mapping_from_secret_type_to_class().values():
+    try:
+        plugin_types = get_mapping_from_secret_type_to_class().values()
+    except FileNotFoundError as e:
+        log.error(f'Error: Failed to load `{classname}` plugin: {e}')
+        log.error(
+            'This error can occur when using a baseline that references a '
+            'custom plugin with a path that does not exist.',
+        )
+        raise
+
+    for plugin_type in plugin_types:
         if plugin_type.__name__ == classname:
             break
     else:
         log.error(f'Error: No such `{classname}` plugin to initialize.')
         log.error('Chances are you should run `pre-commit autoupdate`.')
         log.error(
             'This error can occur when using a baseline that was made by '
```

### Comparing `detect_secrets-1.4.0/detect_secrets/core/plugins/util.py` & `detect_secrets-1.5.0/detect_secrets/core/plugins/util.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/core/potential_secret.py` & `detect_secrets-1.5.0/detect_secrets/core/potential_secret.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 from ..util.color import AnsiColor
 from ..util.color import colorize
+from ..util.path import convert_local_os_path
 
 
 class PotentialSecret:
     """This custom data type represents a string found, matching the
     plugin rules defined in SecretsCollection, that has the potential
     to be a secret that we actually care about.
 
@@ -71,15 +72,15 @@
         return hashlib.sha1(secret.encode('utf-8')).hexdigest()
 
     @classmethod
     def load_secret_from_dict(cls, data: Dict[str, Union[str, int, bool]]) -> 'PotentialSecret':
         """Custom JSON decoder"""
         kwargs: Dict[str, Any] = {
             'type': str(data['type']),
-            'filename': str(data['filename']),
+            'filename': convert_local_os_path(str(data['filename'])),
             'secret': 'will be replaced',
         }
 
         # Optional parameters
         for parameter in {
             'line_number',
             'is_secret',
```

### Comparing `detect_secrets-1.4.0/detect_secrets/core/scan.py` & `detect_secrets-1.5.0/detect_secrets/core/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,16 +134,20 @@
             line=line,
             context=context,
         )
     )
 
 
 def scan_file(filename: str) -> Generator[PotentialSecret, None, None]:
-    if not get_plugins():   # pragma: no cover
-        log.error('No plugins to scan with!')
+    try:
+        if not get_plugins():   # pragma: no cover
+            log.error('No plugins to scan with!')
+            return
+    except FileNotFoundError:
+        log.error('Unable to load plugins!')
         return
 
     if _is_filtered_out(required_filter_parameters=['filename'], filename=filename):
         return
 
     try:
         has_secret = False
@@ -383,21 +387,27 @@
 
 
 def _is_filtered_out(required_filter_parameters: Iterable[str], **kwargs: Any) -> bool:
     for filter_fn in get_filters_with_parameter(*required_filter_parameters):
         try:
             if call_function_with_arguments(filter_fn, **kwargs):
                 if 'secret' in kwargs:
-                    debug_msg = f'Skipping "{kwargs["secret"]}" due to `{filter_fn.path}`.'
+                    debug_msg = f'Skipping "{0}" due to `{1}`.'.format(
+                        kwargs['secret'],
+                        filter_fn.path,
+                    )
                 elif list(kwargs.keys()) == ['filename']:
                     # We want to make sure this is only run if we're skipping files (as compared
                     # to other filters that may include `filename` as a parameter).
-                    debug_msg = f'Skipping "{kwargs["filename"]}" due to `{filter_fn.path}`'
+                    debug_msg = 'Skipping "{0}" due to `{1}`'.format(
+                        kwargs['filename'],
+                        filter_fn.path,
+                    )
                 else:
-                    debug_msg = f'Skipping secret due to `{filter_fn.path}`.'
+                    debug_msg = 'Skipping secret due to `{0}`.'.format(filter_fn.path)
 
                 log.info(debug_msg)
                 return True
         except TypeError:
             # Skipping non-compatible filters
             pass
```

### Comparing `detect_secrets-1.4.0/detect_secrets/core/secrets_collection.py` & `detect_secrets-1.5.0/detect_secrets/core/secrets_collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Generator
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 
 from . import scan
+from ..util.path import convert_local_os_path
 from .potential_secret import PotentialSecret
 from detect_secrets.settings import configure_settings_from_baseline
 from detect_secrets.settings import get_settings
 
 
 class PatchedFile:
     """This exists so that we can do typecasting, without importing unidiff."""
@@ -36,15 +37,15 @@
 
     @classmethod
     def load_from_baseline(cls, baseline: Dict[str, Any]) -> 'SecretsCollection':
         output = cls()
         for filename in baseline['results']:
             for item in baseline['results'][filename]:
                 secret = PotentialSecret.load_secret_from_dict({'filename': filename, **item})
-                output[filename].add(secret)
+                output[convert_local_os_path(filename)].add(secret)
 
         return output
 
     @property
     def files(self) -> Set[str]:
         return set(self.data.keys())
 
@@ -68,16 +69,16 @@
                 _scan_file_and_serialize,
                 [os.path.join(self.root, filename) for filename in filenames],
             ):
                 for secret in secrets:
                     self[os.path.relpath(secret.filename, self.root)].add(secret)
 
     def scan_file(self, filename: str) -> None:
-        for secret in scan.scan_file(os.path.join(self.root, filename)):
-            self[filename].add(secret)
+        for secret in scan.scan_file(os.path.join(self.root, convert_local_os_path(filename))):
+            self[convert_local_os_path(filename)].add(secret)
 
     def scan_diff(self, diff: str) -> None:
         """
         :raises: UnidiffParseError
         """
         try:
             for secret in scan.scan_diff(diff):
```

### Comparing `detect_secrets-1.4.0/detect_secrets/core/upgrades/v1_0.py` & `detect_secrets-1.5.0/detect_secrets/core/upgrades/v1_0.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/core/upgrades/v1_1.py` & `detect_secrets-1.5.0/detect_secrets/core/upgrades/v1_1.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/core/usage/__init__.py` & `detect_secrets-1.5.0/detect_secrets/core/usage/__init__.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/core/usage/audit.py` & `detect_secrets-1.5.0/detect_secrets/core/usage/audit.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/core/usage/baseline.py` & `detect_secrets-1.5.0/detect_secrets/core/usage/baseline.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/core/usage/common.py` & `detect_secrets-1.5.0/detect_secrets/core/usage/common.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/core/usage/filters.py` & `detect_secrets-1.5.0/detect_secrets/core/usage/filters.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/core/usage/plugins.py` & `detect_secrets-1.5.0/detect_secrets/core/usage/plugins.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/core/usage/scan.py` & `detect_secrets-1.5.0/detect_secrets/core/usage/scan.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/exceptions.py` & `detect_secrets-1.5.0/detect_secrets/exceptions.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/filters/allowlist.py` & `detect_secrets-1.5.0/detect_secrets/filters/allowlist.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/filters/common.py` & `detect_secrets-1.5.0/detect_secrets/filters/common.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/filters/gibberish/__init__.py` & `detect_secrets-1.5.0/detect_secrets/filters/gibberish/__init__.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/filters/gibberish/rfc.model` & `detect_secrets-1.5.0/detect_secrets/filters/gibberish/rfc.model`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/filters/heuristic.py` & `detect_secrets-1.5.0/detect_secrets/filters/heuristic.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
 
 def is_prefixed_with_dollar_sign(secret: str) -> bool:
     # NOTE: This is broken out into its own function since it has more chance of increasing
     # false negatives than `is_templated_secret` (e.g. secrets that actually start with a $).
     # This is best used with files that actually use this as a means of referencing variables.
     # TODO: More intelligent filetype handling?
-    return secret[0] == '$'
+    return bool(secret) and secret[0] == '$'
 
 
 def is_indirect_reference(line: str) -> bool:
     """
     Filters secrets that take the form of:
 
         secret = get_secret_key()
```

### Comparing `detect_secrets-1.4.0/detect_secrets/filters/regex.py` & `detect_secrets-1.5.0/detect_secrets/filters/regex.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/filters/util.py` & `detect_secrets-1.5.0/detect_secrets/filters/util.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/filters/wordlist.py` & `detect_secrets-1.5.0/detect_secrets/filters/wordlist.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/main.py` & `detect_secrets-1.5.0/detect_secrets/main.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/aws.py` & `detect_secrets-1.5.0/detect_secrets/plugins/aws.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 class AWSKeyDetector(RegexBasedDetector):
     """Scans for AWS keys."""
     secret_type = 'AWS Access Key'
 
     secret_keyword = r'(?:key|pwd|pw|password|pass|token)'
 
     denylist = (
-        re.compile(r'AKIA[0-9A-Z]{16}'),
+        re.compile(r'(?:A3T[A-Z0-9]|ABIA|ACCA|AKIA|ASIA)[0-9A-Z]{16}'),
 
         # This examines the variable name to identify AWS secret tokens.
-        # The order is important since we want to prefer finding `AKIA`-based
+        # The order is important since we want to prefer finding access
         # keys (since they can be verified), rather than the secret tokens.
 
         re.compile(
             r'aws.{{0,20}}?{secret_keyword}.{{0,20}}?[\'\"]([0-9a-zA-Z/+]{{40}})[\'\"]'.format(
                 secret_keyword=secret_keyword,
             ),
             flags=re.IGNORECASE,
```

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/base.py` & `detect_secrets-1.5.0/detect_secrets/plugins/base.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/basic_auth.py` & `detect_secrets-1.5.0/detect_secrets/plugins/basic_auth.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/cloudant.py` & `detect_secrets-1.5.0/detect_secrets/plugins/cloudant.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/high_entropy_strings.py` & `detect_secrets-1.5.0/detect_secrets/plugins/high_entropy_strings.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/ibm_cloud_iam.py` & `detect_secrets-1.5.0/detect_secrets/plugins/ibm_cloud_iam.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         response = verify_cloud_iam_api_key(secret)
 
         return VerifiedResult.VERIFIED_TRUE if response.status_code == 200 \
             else VerifiedResult.VERIFIED_FALSE
 
 
 def verify_cloud_iam_api_key(apikey: Union[str, bytes]) -> requests.Response:  # pragma: no cover
-    if type(apikey) == bytes:
+    if type(apikey) is bytes:
         apikey = apikey.decode('UTF-8')
 
     headers = {
         'Content-Type': 'application/x-www-form-urlencoded',
         'Accept': 'application/json',
     }
     response = requests.post(
```

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/ibm_cos_hmac.py` & `detect_secrets-1.5.0/detect_secrets/plugins/ibm_cos_hmac.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/jwt.py` & `detect_secrets-1.5.0/detect_secrets/plugins/jwt.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/keyword.py` & `detect_secrets-1.5.0/detect_secrets/plugins/keyword.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 #                   line breaks, comma, backticks or quotes. This allows to reduce the false
 #                   positives number and to prevent errors in the code snippet highlighting.
 SECRET = r'(?=[^\v\'\"]*)(?=\w+)[^\v\'\"]*[^\v,\'\"`]'
 SQUARE_BRACKETS = r'(\[[0-9]*\])'
 
 FOLLOWED_BY_COLON_EQUAL_SIGNS_REGEX = re.compile(
     # e.g. my_password := "bar" or my_password := bar
-    r'{denylist}({closing})?{whitespace}:=?{whitespace}({quote}?)({secret})(\3)'.format(
+    r'{denylist}({closing})?{whitespace}:={whitespace}({quote}?)({secret})(\3)'.format(
         denylist=DENYLIST_REGEX,
         closing=CLOSING,
         quote=QUOTE,
         whitespace=OPTIONAL_WHITESPACE,
         secret=SECRET,
     ),
     flags=re.IGNORECASE,
```

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/mailchimp.py` & `detect_secrets-1.5.0/detect_secrets/plugins/mailchimp.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/private_key.py` & `detect_secrets-1.5.0/detect_secrets/plugins/private_key.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/slack.py` & `detect_secrets-1.5.0/detect_secrets/plugins/slack.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/softlayer.py` & `detect_secrets-1.5.0/detect_secrets/plugins/softlayer.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/plugins/stripe.py` & `detect_secrets-1.5.0/detect_secrets/plugins/stripe.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/pre_commit_hook.py` & `detect_secrets-1.5.0/detect_secrets/pre_commit_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,18 +143,18 @@
     wrapper = textwrap.TextWrapper(
         initial_indent='  - ',
         subsequent_indent='    ',
         width=width,
     )
     for suggestion in [
         'For information about putting your secrets in a safer place, '
-        f'please ask {os.environ.get("DETECT_SECRETS_SECURITY_TEAM", "in #security")}',
+        'please ask {0}'.format(os.environ.get('DETECT_SECRETS_SECURITY_TEAM', 'in #security')),
 
         'Mark false positives with an inline '
-        f'`{color.colorize("pragma: allowlist secret", color.AnsiColor.BOLD)}` comment',
+        '`{0}` comment'.format(color.colorize('pragma: allowlist secret', color.AnsiColor.BOLD)),
     ]:
         print(wrapper.fill(suggestion))
 
     print()
     print(
         textwrap.fill(
             'If a secret has already been committed, visit '
```

### Comparing `detect_secrets-1.4.0/detect_secrets/settings.py` & `detect_secrets-1.5.0/detect_secrets/settings.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/transformers/__init__.py` & `detect_secrets-1.5.0/detect_secrets/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/transformers/base.py` & `detect_secrets-1.5.0/detect_secrets/transformers/base.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/transformers/config.py` & `detect_secrets-1.5.0/detect_secrets/transformers/config.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/transformers/yaml.py` & `detect_secrets-1.5.0/detect_secrets/transformers/yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,25 @@
         :raises: ParsingError
         """
         try:
             items = sorted(YAMLFileParser(file), key=lambda x: x.line_number)
         except yaml.YAMLError:
             raise ParsingError
 
+        seen = set()
+
         lines: List[str] = []
         for item in items:
+            # Filter out previous lines seen before. This removes duplicates when it comes
+            # to anchor & and alias * tags.
+            if item in seen:
+                continue
+            else:
+                seen.add(item)
+
             while len(lines) < item.line_number - 1:
                 lines.append('')
 
             value = item.value
             if isinstance(value, bytes):
                 # binary strings in YAML are base64 encoded. https://yaml.org/type/binary.html
                 # While the YAML parser already decodes it for us, we want to capture the *raw*
```

### Comparing `detect_secrets-1.4.0/detect_secrets/util/code_snippet.py` & `detect_secrets-1.5.0/detect_secrets/util/code_snippet.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/util/color.py` & `detect_secrets-1.5.0/detect_secrets/util/color.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/util/filetype.py` & `detect_secrets-1.5.0/detect_secrets/util/filetype.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/util/git.py` & `detect_secrets-1.5.0/detect_secrets/util/git.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/util/importlib.py` & `detect_secrets-1.5.0/detect_secrets/util/importlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import errno
 import importlib.util
 import os
 import pkgutil
 from importlib import import_module
 from types import ModuleType
 from typing import Any
 from typing import Callable
@@ -81,15 +82,16 @@
 
     The second assumption should also be pretty straight-forward: don't trust user input,
     especially if it's going to be executed as that privileged user, unless you want a privilege
     escalation vulnerability. detect-secrets is not going to do any sanitization of user input
     for you.
     """
     if not os.path.exists(filename):
-        raise FileNotFoundError
+        # Source: https://stackoverflow.com/a/36077407
+        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), filename)
 
     if not name:
         # NOTE: After several trial and error attempts, I could not discern the importance
         # of this field, in this context. Hence, I don't think it matters that much.
         name = os.path.splitext(os.path.basename(filename))[0]
 
     # Source: https://stackoverflow.com/a/67692/13340678
```

### Comparing `detect_secrets-1.4.0/detect_secrets/util/inject.py` & `detect_secrets-1.5.0/detect_secrets/util/inject.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets/util/semver.py` & `detect_secrets-1.5.0/detect_secrets/util/semver.py`

 * *Files identical despite different names*

### Comparing `detect_secrets-1.4.0/detect_secrets.egg-info/PKG-INFO` & `detect_secrets-1.5.0/detect_secrets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: detect-secrets
-Version: 1.4.0
+Version: 1.5.0
 Summary: Tool for detecting secrets in the codebase
 Home-page: https://github.com/Yelp/detect-secrets
-Author: Aaron Loo
-Author-email: aaronloo@yelp.com
-License: Copyright Yelp, Inc. 2020
-Download-URL: https://github.com/Yelp/detect-secrets/archive/1.4.0.tar.gz
+Author: Yelp, Inc.
+Author-email: opensource@yelp.com
+License: UNKNOWN
+Download-URL: https://github.com/Yelp/detect-secrets/archive/1.5.0.tar.gz
 Description: [![Build Status](https://github.com/Yelp/detect-secrets/actions/workflows/ci.yml/badge.svg)](https://github.com/Yelp/detect-secrets/actions/workflows/ci.yml?query=branch%3Amaster++)
         [![PyPI version](https://badge.fury.io/py/detect-secrets.svg)](https://badge.fury.io/py/detect-secrets)
         [![Homebrew](https://img.shields.io/badge/dynamic/json.svg?url=https://formulae.brew.sh/api/formula/detect-secrets.json&query=$.versions.stable&label=homebrew)](https://formulae.brew.sh/formula/detect-secrets)
         [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-ff69b4.svg)](https://github.com/Yelp/detect-secrets/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22+)
         [![AMF](https://img.shields.io/badge/Donate-Charity-orange.svg)](https://www.againstmalaria.com/donation.aspx)
         
         # detect-secrets
@@ -103,28 +103,33 @@
         ArtifactoryDetector
         AWSKeyDetector
         AzureStorageKeyDetector
         BasicAuthDetector
         CloudantDetector
         DiscordBotTokenDetector
         GitHubTokenDetector
+        GitLabTokenDetector
         Base64HighEntropyString
         HexHighEntropyString
         IbmCloudIamDetector
         IbmCosHmacDetector
+        IPPublicDetector
         JwtTokenDetector
         KeywordDetector
         MailchimpDetector
         NpmDetector
+        OpenAIDetector
         PrivateKeyDetector
+        PypiTokenDetector
         SendGridDetector
         SlackDetector
         SoftlayerDetector
         SquareOAuthDetector
         StripeDetector
+        TelegramBotTokenDetector
         TwilioKeyDetector
         ```
         
         ### Disabling Plugins:
         
         ```bash
         $ detect-secrets scan --disable-plugin KeywordDetector --disable-plugin AWSKeyDetector
@@ -397,15 +402,15 @@
         We recommend setting this up as a pre-commit hook. One way to do this is by using the
         [pre-commit](https://github.com/pre-commit/pre-commit) framework:
         
         ```yaml
         # .pre-commit-config.yaml
         repos:
         -   repo: https://github.com/Yelp/detect-secrets
-            rev: v1.4.0
+            rev: v1.5.0
             hooks:
             -   id: detect-secrets
                 args: ['--baseline', '.secrets.baseline']
                 exclude: package.lock.json
         ```
         
         #### Inline Allowlisting
```

### Comparing `detect_secrets-1.4.0/detect_secrets.egg-info/SOURCES.txt` & `detect_secrets-1.5.0/detect_secrets.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -60,27 +60,32 @@
 detect_secrets/plugins/aws.py
 detect_secrets/plugins/azure_storage_key.py
 detect_secrets/plugins/base.py
 detect_secrets/plugins/basic_auth.py
 detect_secrets/plugins/cloudant.py
 detect_secrets/plugins/discord.py
 detect_secrets/plugins/github_token.py
+detect_secrets/plugins/gitlab_token.py
 detect_secrets/plugins/high_entropy_strings.py
 detect_secrets/plugins/ibm_cloud_iam.py
 detect_secrets/plugins/ibm_cos_hmac.py
+detect_secrets/plugins/ip_public.py
 detect_secrets/plugins/jwt.py
 detect_secrets/plugins/keyword.py
 detect_secrets/plugins/mailchimp.py
 detect_secrets/plugins/npm.py
+detect_secrets/plugins/openai.py
 detect_secrets/plugins/private_key.py
+detect_secrets/plugins/pypi_token.py
 detect_secrets/plugins/sendgrid.py
 detect_secrets/plugins/slack.py
 detect_secrets/plugins/softlayer.py
 detect_secrets/plugins/square_oauth.py
 detect_secrets/plugins/stripe.py
+detect_secrets/plugins/telegram_token.py
 detect_secrets/plugins/twilio.py
 detect_secrets/transformers/__init__.py
 detect_secrets/transformers/base.py
 detect_secrets/transformers/config.py
 detect_secrets/transformers/exceptions.py
 detect_secrets/transformers/yaml.py
 detect_secrets/util/__init__.py
```

### Comparing `detect_secrets-1.4.0/setup.py` & `detect_secrets-1.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,16 @@
 setup(
     name='detect_secrets',
     packages=find_packages(exclude=(['test*', 'tmp*'])),
     version=VERSION,
     description='Tool for detecting secrets in the codebase',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    license='Copyright Yelp, Inc. 2020',
-    author='Aaron Loo',
-    author_email='aaronloo@yelp.com',
+    author='Yelp, Inc.',
+    author_email='opensource@yelp.com',
     url='https://github.com/Yelp/detect-secrets',
     download_url='https://github.com/Yelp/detect-secrets/archive/{}.tar.gz'.format(VERSION),
     keywords=['secret-management', 'pre-commit', 'security', 'entropy-checks'],
     install_requires=[
         'pyyaml',
         'requests',
     ],
```

