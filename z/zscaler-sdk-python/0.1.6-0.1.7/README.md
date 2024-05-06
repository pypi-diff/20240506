# Comparing `tmp/zscaler_sdk_python-0.1.6.tar.gz` & `tmp/zscaler_sdk_python-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_sdk_python-0.1.6.tar", max compression
+gzip compressed data, was "zscaler_sdk_python-0.1.7.tar", max compression
```

## Comparing `zscaler_sdk_python-0.1.6.tar` & `zscaler_sdk_python-0.1.7.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1113 2024-04-30 22:36:42.985087 zscaler_sdk_python-0.1.6/LICENSE.md
--rw-r--r--   0        0        0    15746 2024-04-30 22:36:42.985087 zscaler_sdk_python-0.1.6/README.md
--rw-r--r--   0        0        0     2290 2024-04-30 22:37:19.933497 zscaler_sdk_python-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1277 2024-04-30 22:37:19.937497 zscaler_sdk_python-0.1.6/zscaler/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/cache/__init__.py
--rw-r--r--   0        0        0     3195 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/cache/cache.py
--rw-r--r--   0        0        0     1479 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/cache/no_op_cache.py
--rw-r--r--   0        0        0     4967 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/cache/zscaler_cache.py
--rw-r--r--   0        0        0      738 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/constants.py
--rw-r--r--   0        0        0        0 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/errors/__init__.py
--rw-r--r--   0        0        0      172 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/errors/error.py
--rw-r--r--   0        0        0      638 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/errors/http_error.py
--rw-r--r--   0        0        0      628 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/errors/zscaler_api_error.py
--rw-r--r--   0        0        0       63 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/exceptions/__init__.py
--rw-r--r--   0        0        0     2025 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/exceptions/exceptions.py
--rw-r--r--   0        0        0     2099 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/logger.py
--rw-r--r--   0        0        0        0 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/ratelimiter/__init__.py
--rw-r--r--   0        0        0     1473 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/ratelimiter/ratelimiter.py
--rw-r--r--   0        0        0      639 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/user_agent.py
--rw-r--r--   0        0        0    19073 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/utils.py
--rw-r--r--   0        0        0    21568 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/zia/__init__.py
--rw-r--r--   0        0        0     1534 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/zia/activate.py
--rw-r--r--   0        0        0    14194 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/zia/admin_and_role_management.py
--rw-r--r--   0        0        0     2372 2024-04-30 22:36:43.005087 zscaler_sdk_python-0.1.6/zscaler/zia/apptotal.py
--rw-r--r--   0        0        0     2992 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/audit_logs.py
--rw-r--r--   0        0        0     3140 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/authentication_settings.py
--rw-r--r--   0        0        0     2754 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/client.py
--rw-r--r--   0        0        0    18513 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/cloud_apps.py
--rw-r--r--   0        0        0     2872 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/device_management.py
--rw-r--r--   0        0        0    27473 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/dlp.py
--rw-r--r--   0        0        0      794 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/errors.py
--rw-r--r--   0        0        0    39908 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/firewall.py
--rw-r--r--   0        0        0    11686 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/forwarding_control.py
--rw-r--r--   0        0        0     2909 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/isolation_profile.py
--rw-r--r--   0        0        0     5835 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/labels.py
--rw-r--r--   0        0        0    30762 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/locations.py
--rw-r--r--   0        0        0     6724 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/sandbox.py
--rw-r--r--   0        0        0     6792 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/security.py
--rw-r--r--   0        0        0     5298 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/ssl_inspection.py
--rw-r--r--   0        0        0    30729 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/traffic.py
--rw-r--r--   0        0        0    14484 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/url_categories.py
--rw-r--r--   0        0        0    14319 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/url_filtering.py
--rw-r--r--   0        0        0    13735 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/users.py
--rw-r--r--   0        0        0    12376 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/web_dlp.py
--rw-r--r--   0        0        0     1897 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/workload_groups.py
--rw-r--r--   0        0        0     6842 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zia/zpa_gateway.py
--rw-r--r--   0        0        0     2709 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/README.md
--rw-r--r--   0        0        0    24470 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/__init__.py
--rw-r--r--   0        0        0    13187 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/app_segments.py
--rw-r--r--   0        0        0    12445 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/app_segments_inspection.py
--rw-r--r--   0        0        0    12019 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/app_segments_pra.py
--rw-r--r--   0        0        0     7942 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/certificates.py
--rw-r--r--   0        0        0     3844 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/client.py
--rw-r--r--   0        0        0     2667 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/cloud_connector_groups.py
--rw-r--r--   0        0        0    20849 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/connectors.py
--rw-r--r--   0        0        0     6189 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/emergency_access.py
--rw-r--r--   0        0        0      844 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/errors.py
--rw-r--r--   0        0        0     2764 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/idp.py
--rw-r--r--   0        0        0    34309 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/inspection.py
--rw-r--r--   0        0        0     3176 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/isolation_profile.py
--rw-r--r--   0        0        0    21697 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/lss.py
--rw-r--r--   0        0        0     2734 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/machine_groups.py
--rw-r--r--   0        0        0    31747 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/policies.py
--rw-r--r--   0        0        0     4317 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/posture_profiles.py
--rw-r--r--   0        0        0    32017 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/privileged_remote_access.py
--rw-r--r--   0        0        0     9887 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/provisioning.py
--rw-r--r--   0        0        0     3632 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/saml_attributes.py
--rw-r--r--   0        0        0     4172 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/scim_attributes.py
--rw-r--r--   0        0        0     5041 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/scim_groups.py
--rw-r--r--   0        0        0     6103 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/segment_groups.py
--rw-r--r--   0        0        0     7776 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/server_groups.py
--rw-r--r--   0        0        0     6477 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/servers.py
--rw-r--r--   0        0        0    15428 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/service_edges.py
--rw-r--r--   0        0        0     4377 2024-04-30 22:36:43.009087 zscaler_sdk_python-0.1.6/zscaler/zpa/trusted_networks.py
--rw-r--r--   0        0        0    17514 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1113 2024-05-06 07:40:30.079598 zscaler_sdk_python-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0    15746 2024-05-06 07:40:30.079598 zscaler_sdk_python-0.1.7/README.md
+-rw-r--r--   0        0        0     2292 2024-05-06 07:41:09.675720 zscaler_sdk_python-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1277 2024-05-06 07:41:09.679720 zscaler_sdk_python-0.1.7/zscaler/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/cache/__init__.py
+-rw-r--r--   0        0        0     3195 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/cache/cache.py
+-rw-r--r--   0        0        0     1479 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/cache/no_op_cache.py
+-rw-r--r--   0        0        0     4967 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/cache/zscaler_cache.py
+-rw-r--r--   0        0        0      738 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/constants.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/errors/__init__.py
+-rw-r--r--   0        0        0      172 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/errors/error.py
+-rw-r--r--   0        0        0      638 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/errors/http_error.py
+-rw-r--r--   0        0        0      628 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/errors/zscaler_api_error.py
+-rw-r--r--   0        0        0       63 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/exceptions/__init__.py
+-rw-r--r--   0        0        0     2025 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/exceptions/exceptions.py
+-rw-r--r--   0        0        0     2099 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/logger.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/ratelimiter/__init__.py
+-rw-r--r--   0        0        0     1473 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/ratelimiter/ratelimiter.py
+-rw-r--r--   0        0        0      639 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/user_agent.py
+-rw-r--r--   0        0        0    19073 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/utils.py
+-rw-r--r--   0        0        0    21568 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/__init__.py
+-rw-r--r--   0        0        0     1534 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/activate.py
+-rw-r--r--   0        0        0    14194 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/admin_and_role_management.py
+-rw-r--r--   0        0        0     2372 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/apptotal.py
+-rw-r--r--   0        0        0     2992 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/audit_logs.py
+-rw-r--r--   0        0        0     3140 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/authentication_settings.py
+-rw-r--r--   0        0        0     2754 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/client.py
+-rw-r--r--   0        0        0    18513 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/cloud_apps.py
+-rw-r--r--   0        0        0     2872 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/device_management.py
+-rw-r--r--   0        0        0    27473 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/dlp.py
+-rw-r--r--   0        0        0      794 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/errors.py
+-rw-r--r--   0        0        0    39908 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/firewall.py
+-rw-r--r--   0        0        0    11686 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/forwarding_control.py
+-rw-r--r--   0        0        0     2909 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/isolation_profile.py
+-rw-r--r--   0        0        0     5835 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/labels.py
+-rw-r--r--   0        0        0    30762 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/locations.py
+-rw-r--r--   0        0        0     6724 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/sandbox.py
+-rw-r--r--   0        0        0     6792 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/security.py
+-rw-r--r--   0        0        0     5298 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/ssl_inspection.py
+-rw-r--r--   0        0        0    30729 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/traffic.py
+-rw-r--r--   0        0        0    14484 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/url_categories.py
+-rw-r--r--   0        0        0    14319 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/url_filtering.py
+-rw-r--r--   0        0        0    13735 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/users.py
+-rw-r--r--   0        0        0    12376 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/web_dlp.py
+-rw-r--r--   0        0        0     1897 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/workload_groups.py
+-rw-r--r--   0        0        0     6842 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/zpa_gateway.py
+-rw-r--r--   0        0        0     2709 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/README.md
+-rw-r--r--   0        0        0    24470 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/__init__.py
+-rw-r--r--   0        0        0    13187 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/app_segments.py
+-rw-r--r--   0        0        0    12445 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/app_segments_inspection.py
+-rw-r--r--   0        0        0    12019 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/app_segments_pra.py
+-rw-r--r--   0        0        0     7942 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/certificates.py
+-rw-r--r--   0        0        0     3844 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/client.py
+-rw-r--r--   0        0        0     2667 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/cloud_connector_groups.py
+-rw-r--r--   0        0        0    20849 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/connectors.py
+-rw-r--r--   0        0        0     6189 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/emergency_access.py
+-rw-r--r--   0        0        0      844 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/errors.py
+-rw-r--r--   0        0        0     2764 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/idp.py
+-rw-r--r--   0        0        0    34309 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/inspection.py
+-rw-r--r--   0        0        0     3176 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/isolation_profile.py
+-rw-r--r--   0        0        0    21697 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/lss.py
+-rw-r--r--   0        0        0     2734 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/machine_groups.py
+-rw-r--r--   0        0        0    31747 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/policies.py
+-rw-r--r--   0        0        0     4317 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/posture_profiles.py
+-rw-r--r--   0        0        0    32017 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/privileged_remote_access.py
+-rw-r--r--   0        0        0     9887 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/provisioning.py
+-rw-r--r--   0        0        0     3632 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/saml_attributes.py
+-rw-r--r--   0        0        0     4172 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/scim_attributes.py
+-rw-r--r--   0        0        0     5041 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/scim_groups.py
+-rw-r--r--   0        0        0     6103 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/segment_groups.py
+-rw-r--r--   0        0        0     7776 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/server_groups.py
+-rw-r--r--   0        0        0     6477 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/servers.py
+-rw-r--r--   0        0        0    15428 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/service_edges.py
+-rw-r--r--   0        0        0     4377 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/trusted_networks.py
+-rw-r--r--   0        0        0    17518 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.1.7/PKG-INFO
```

### Comparing `zscaler_sdk_python-0.1.6/LICENSE.md` & `zscaler_sdk_python-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/README.md` & `zscaler_sdk_python-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/pyproject.toml` & `zscaler_sdk_python-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zscaler-sdk-python"
-version = "0.1.6"
+version = "0.1.7"
 description = "Official Python SDK for the Zscaler Products (Beta)"
 authors = ["Zscaler, Inc. <devrel@zscaler.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/zscaler/zscaler-sdk-python"
 repository = "https://github.com/zscaler/zscaler-sdk-python"
 documentation = "https://zscaler-sdk-python.readthedocs.io"
@@ -29,15 +29,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 arrow = "*"
 certifi = "*"
 charset-normalizer = "*"
 idna = "*"
-python-box = "^5.4"
+python-box = "^7.1.1"
 python-dateutil = "*"
 requests = "*"
 responses = "*"
 restfly = "*"
 six = "*"
 urllib3 = "*"
 flatdict = "*"
```

### Comparing `zscaler_sdk_python-0.1.6/zscaler/__init__.py` & `zscaler_sdk_python-0.1.7/zscaler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 
 __author__ = "Zscaler Inc"
 __email__ = "devrel@zscaler.com"
 __license__ = "MIT"
 __contributors__ = [
     "William Guilherme",
 ]
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 
 from zscaler.zia import ZIAClientHelper  # noqa
 from zscaler.zpa import ZPAClientHelper  # noqa
```

### Comparing `zscaler_sdk_python-0.1.6/zscaler/cache/cache.py` & `zscaler_sdk_python-0.1.7/zscaler/cache/cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/cache/no_op_cache.py` & `zscaler_sdk_python-0.1.7/zscaler/cache/no_op_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/cache/zscaler_cache.py` & `zscaler_sdk_python-0.1.7/zscaler/cache/zscaler_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/constants.py` & `zscaler_sdk_python-0.1.7/zscaler/constants.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/errors/http_error.py` & `zscaler_sdk_python-0.1.7/zscaler/errors/http_error.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/errors/zscaler_api_error.py` & `zscaler_sdk_python-0.1.7/zscaler/errors/zscaler_api_error.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/exceptions/exceptions.py` & `zscaler_sdk_python-0.1.7/zscaler/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/logger.py` & `zscaler_sdk_python-0.1.7/zscaler/logger.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/ratelimiter/ratelimiter.py` & `zscaler_sdk_python-0.1.7/zscaler/ratelimiter/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/user_agent.py` & `zscaler_sdk_python-0.1.7/zscaler/user_agent.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/utils.py` & `zscaler_sdk_python-0.1.7/zscaler/utils.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/__init__.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/activate.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/activate.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/admin_and_role_management.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/admin_and_role_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/apptotal.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/apptotal.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/audit_logs.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/audit_logs.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/authentication_settings.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/authentication_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/client.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/client.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/cloud_apps.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/cloud_apps.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/device_management.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/device_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/dlp.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/errors.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/firewall.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/firewall.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/forwarding_control.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/forwarding_control.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/isolation_profile.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/labels.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/labels.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/locations.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/locations.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/sandbox.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/sandbox.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/security.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/security.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/ssl_inspection.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/ssl_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/traffic.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/traffic.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/url_categories.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/url_filtering.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/url_filtering.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/users.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/users.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/web_dlp.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/web_dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/workload_groups.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/workload_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zia/zpa_gateway.py` & `zscaler_sdk_python-0.1.7/zscaler/zia/zpa_gateway.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/README.md` & `zscaler_sdk_python-0.1.7/zscaler/zpa/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/__init__.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/app_segments.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/app_segments.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/app_segments_inspection.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/app_segments_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/app_segments_pra.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/app_segments_pra.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/certificates.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/certificates.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/client.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/client.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/cloud_connector_groups.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/cloud_connector_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/connectors.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/connectors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/emergency_access.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/emergency_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/errors.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/idp.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/idp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/inspection.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/isolation_profile.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/lss.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/lss.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/machine_groups.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/machine_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/policies.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/policies.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/posture_profiles.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/posture_profiles.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/privileged_remote_access.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/privileged_remote_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/provisioning.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/provisioning.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/saml_attributes.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/saml_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/scim_attributes.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/scim_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/scim_groups.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/scim_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/segment_groups.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/segment_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/server_groups.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/server_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/servers.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/servers.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/service_edges.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/service_edges.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/zscaler/zpa/trusted_networks.py` & `zscaler_sdk_python-0.1.7/zscaler/zpa/trusted_networks.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.6/PKG-INFO` & `zscaler_sdk_python-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler-sdk-python
-Version: 0.1.6
+Version: 0.1.7
 Summary: Official Python SDK for the Zscaler Products (Beta)
 Home-page: https://github.com/zscaler/zscaler-sdk-python
 License: MIT
 Keywords: zscaler,sdk,zpa,zia,zdx,zcc,zcon
 Author: Zscaler, Inc.
 Author-email: devrel@zscaler.com
 Requires-Python: >=3.8,<4.0
@@ -27,15 +27,15 @@
 Requires-Dist: certifi
 Requires-Dist: charset-normalizer
 Requires-Dist: flake8
 Requires-Dist: flatdict
 Requires-Dist: idna
 Requires-Dist: pycryptodomex
 Requires-Dist: pydash ; extra == "dev"
-Requires-Dist: python-box (>=5.4,<6.0)
+Requires-Dist: python-box (>=7.1.1,<8.0.0)
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: responses
 Requires-Dist: restfly
 Requires-Dist: six
```

