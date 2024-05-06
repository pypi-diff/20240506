# Comparing `tmp/qwak_core-0.4.0.tar.gz` & `tmp/qwak_core-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.4.0.tar", max compression
+gzip compressed data, was "qwak_core-0.4.1.tar", max compression
```

## Comparing `qwak_core-0.4.0.tar` & `qwak_core-0.4.1.tar`

### file list

```diff
@@ -1,818 +1,818 @@
--rw-r--r--   0        0        0      264 2024-05-05 10:41:18.274960 qwak_core-0.4.0/README.md
--rw-r--r--   0        0        0        0 2024-05-05 10:43:53.597721 qwak_core-0.4.0/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5877 2024-05-05 10:43:53.625721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     7824 2024-05-05 10:43:24.025959 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.625721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0    12703 2024-05-05 10:43:53.625721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py
--rw-r--r--   0        0        0    10914 2024-05-05 10:43:24.221957 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi
--rw-r--r--   0        0        0    14681 2024-05-05 10:43:53.629721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2024-05-05 10:43:53.617721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2024-05-05 10:43:23.637962 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.621721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2024-05-05 10:43:53.621721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2024-05-05 10:43:23.829960 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.621721 qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2024-05-05 10:43:53.613721 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2024-05-05 10:43:23.053967 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2024-05-05 10:43:53.613721 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2024-05-05 10:43:53.613721 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2024-05-05 10:43:23.249965 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.613721 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4901 2024-05-05 10:43:53.617721 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5995 2024-05-05 10:43:23.445963 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.617721 qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2024-05-05 10:43:53.597721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2024-05-05 10:43:22.857968 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2024-05-05 10:43:53.597721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     7360 2024-05-05 10:43:53.597721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0    11651 2024-05-05 10:43:24.417956 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.601721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     5029 2024-05-05 10:43:53.605721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     6943 2024-05-05 10:43:24.805953 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.605721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2024-05-05 10:43:53.605721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2024-05-05 10:43:25.001951 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2024-05-05 10:43:53.609721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2024-05-05 10:43:53.601721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2024-05-05 10:43:24.609954 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.601721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6541 2024-05-05 10:43:53.609721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10595 2024-05-05 10:43:25.197950 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.609721 qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0    15382 2024-05-05 10:43:53.661720 qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    20668 2024-05-05 10:43:28.013927 qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.661720 qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2024-05-05 10:43:53.665720 qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2024-05-05 10:43:28.209925 qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2024-05-05 10:43:53.665720 qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7616 2024-05-05 10:43:53.813719 qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11995 2024-05-05 10:43:37.865847 qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.813719 qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0    14893 2024-05-05 10:43:53.817719 qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0    11812 2024-05-05 10:43:38.065846 qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    19155 2024-05-05 10:43:53.817719 qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2024-05-05 10:43:53.821719 qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2024-05-05 10:43:39.273836 qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2024-05-05 10:43:53.821719 qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8864 2024-05-05 10:43:53.817719 qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13789 2024-05-05 10:43:39.069838 qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.817719 qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2024-05-05 10:43:53.821719 qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2024-05-05 10:43:39.473835 qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.825719 qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2024-05-05 10:43:53.825719 qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2024-05-05 10:43:39.669833 qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2024-05-05 10:43:53.825719 qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    14053 2024-05-05 10:43:53.941718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    20860 2024-05-05 10:43:49.473754 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.941718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2024-05-05 10:43:53.933718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2024-05-05 10:43:49.049757 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.937718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3954 2024-05-05 10:43:53.937718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     5309 2024-05-05 10:43:49.249756 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.937718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    21176 2024-05-05 10:43:53.929718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    15049 2024-05-05 10:43:48.633761 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    25475 2024-05-05 10:43:53.929718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2024-05-05 10:43:53.933718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2024-05-05 10:43:48.845759 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.933718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2024-05-05 10:43:53.945718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2024-05-05 10:43:50.069749 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.949718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2024-05-05 10:43:53.945718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2024-05-05 10:43:49.873751 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.945718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2024-05-05 10:43:53.941718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2024-05-05 10:43:49.673752 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.941718 qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    11218 2024-05-05 10:43:53.925718 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    15584 2024-05-05 10:43:48.385763 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.929718 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2083 2024-05-05 10:43:53.921718 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1977 2024-05-05 10:43:47.949766 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.921718 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    46028 2024-05-05 10:43:53.925718 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    60013 2024-05-05 10:43:48.181764 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    32008 2024-05-05 10:43:53.925718 qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    29124 2024-05-05 10:43:53.857719 qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    24434 2024-05-05 10:43:41.861815 qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    27837 2024-05-05 10:43:53.861719 qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    33279 2024-05-05 10:43:53.857719 qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    52325 2024-05-05 10:43:41.437819 qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.857719 qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0     5757 2024-05-05 10:43:53.865719 qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py
--rw-r--r--   0        0        0     4013 2024-05-05 10:43:42.493810 qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi
--rw-r--r--   0        0        0     6783 2024-05-05 10:43:53.865719 qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py
--rw-r--r--   0        0        0     6016 2024-05-05 10:43:53.861719 qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_pb2.py
--rw-r--r--   0        0        0     7049 2024-05-05 10:43:42.285812 qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.861719 qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_pb2_grpc.py
--rw-r--r--   0        0        0    14932 2024-05-05 10:43:53.841719 qwak_core-0.4.0/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    24192 2024-05-05 10:43:41.193821 qwak_core-0.4.0/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.845719 qwak_core-0.4.0/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     5552 2024-05-05 10:43:53.845719 qwak_core-0.4.0/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     7299 2024-05-05 10:43:41.645817 qwak_core-0.4.0/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.845719 qwak_core-0.4.0/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    15672 2024-05-05 10:43:53.849719 qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0    12741 2024-05-05 10:43:42.077813 qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    16925 2024-05-05 10:43:53.849719 qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38491 2024-05-05 10:43:53.853719 qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    53557 2024-05-05 10:43:43.193805 qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2024-05-05 10:43:53.853719 qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     3508 2024-05-05 10:43:53.849719 qwak_core-0.4.0/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     2300 2024-05-05 10:43:42.709808 qwak_core-0.4.0/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0     3101 2024-05-05 10:43:53.853719 qwak_core-0.4.0/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0     2270 2024-05-05 10:43:53.869719 qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     2697 2024-05-05 10:43:43.641801 qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.873719 qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4458 2024-05-05 10:43:53.873719 qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     3113 2024-05-05 10:43:43.853799 qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2024-05-05 10:43:53.873719 qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2024-05-05 10:43:53.837719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2024-05-05 10:43:40.549826 qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.837719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11871 2024-05-05 10:43:53.837719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     8790 2024-05-05 10:43:40.761824 qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2024-05-05 10:43:53.841719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2024-05-05 10:43:53.829719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2024-05-05 10:43:40.101829 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.833719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    50041 2024-05-05 10:43:53.829719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    74372 2024-05-05 10:43:39.897831 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.829719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    46309 2024-05-05 10:43:53.833719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    40356 2024-05-05 10:43:40.337828 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    27756 2024-05-05 10:43:53.833719 qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     3345 2024-05-05 10:43:53.649720 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     4098 2024-05-05 10:43:27.001935 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.649720 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12707 2024-05-05 10:43:53.649720 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    13800 2024-05-05 10:43:27.201933 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.653720 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    17949 2024-05-05 10:43:53.653720 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    18562 2024-05-05 10:43:27.401932 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    12833 2024-05-05 10:43:53.653720 qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     6463 2024-05-05 10:43:53.769719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/backfill_pb2.py
--rw-r--r--   0        0        0     7945 2024-05-05 10:43:33.209885 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.769719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/backfill_pb2_grpc.py
--rw-r--r--   0        0        0     2971 2024-05-05 10:43:53.769719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/batch_pb2.py
--rw-r--r--   0        0        0     3266 2024-05-05 10:43:33.417883 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.773719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/batch_pb2_grpc.py
--rw-r--r--   0        0        0     2210 2024-05-05 10:43:53.773719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/deletion_pb2.py
--rw-r--r--   0        0        0     1540 2024-05-05 10:43:33.637882 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.773719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/deletion_pb2_grpc.py
--rw-r--r--   0        0        0     5793 2024-05-05 10:43:53.777719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_pb2.py
--rw-r--r--   0        0        0     7373 2024-05-05 10:43:33.849880 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.777719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_pb2_grpc.py
--rw-r--r--   0        0        0    14900 2024-05-05 10:43:53.777719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_service_pb2.py
--rw-r--r--   0        0        0    11103 2024-05-05 10:43:34.061878 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi
--rw-r--r--   0        0        0    17220 2024-05-05 10:43:53.781719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py
--rw-r--r--   0        0        0     7695 2024-05-05 10:43:53.785719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py
--rw-r--r--   0        0        0    14959 2024-05-05 10:43:34.489875 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.785719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0    19304 2024-05-05 10:43:53.785719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py
--rw-r--r--   0        0        0    16916 2024-05-05 10:43:34.689873 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    21145 2024-05-05 10:43:53.785719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     8440 2024-05-05 10:43:53.781719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py
--rw-r--r--   0        0        0    13312 2024-05-05 10:43:34.281876 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.781719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     2051 2024-05-05 10:43:53.789719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py
--rw-r--r--   0        0        0     1952 2024-05-05 10:43:34.885872 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.789719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_pb2_grpc.py
--rw-r--r--   0        0        0    12222 2024-05-05 10:43:53.789719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py
--rw-r--r--   0        0        0     7930 2024-05-05 10:43:35.081870 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi
--rw-r--r--   0        0        0    14212 2024-05-05 10:43:53.793719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py
--rw-r--r--   0        0        0     1685 2024-05-05 10:43:53.793719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py
--rw-r--r--   0        0        0     1272 2024-05-05 10:43:35.277868 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.793719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2_grpc.py
--rw-r--r--   0        0        0     6198 2024-05-05 10:43:53.797719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py
--rw-r--r--   0        0        0     7677 2024-05-05 10:43:35.473867 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.797719 qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2024-05-05 10:43:53.745720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2024-05-05 10:43:33.005887 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.745720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2024-05-05 10:43:53.741720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2024-05-05 10:43:32.805888 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2024-05-05 10:43:53.741720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2024-05-05 10:43:53.713720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2024-05-05 10:43:30.637906 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.713720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0    13825 2024-05-05 10:43:53.725720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_pb2.py
--rw-r--r--   0        0        0    19227 2024-05-05 10:43:31.617898 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.725720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_pb2_grpc.py
--rw-r--r--   0        0        0     3307 2024-05-05 10:43:53.729720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py
--rw-r--r--   0        0        0     1637 2024-05-05 10:43:31.817896 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi
--rw-r--r--   0        0        0     3293 2024-05-05 10:43:53.729720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2024-05-05 10:43:53.709720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2024-05-05 10:43:30.441907 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.713720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2024-05-05 10:43:53.701720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2024-05-05 10:43:29.829912 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.705720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2024-05-05 10:43:53.709720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2024-05-05 10:43:30.245909 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2024-05-05 10:43:53.709720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2024-05-05 10:43:53.717720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2024-05-05 10:43:30.833904 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.717720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2024-05-05 10:43:53.717720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2024-05-05 10:43:31.029903 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2024-05-05 10:43:53.721720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    26853 2024-05-05 10:43:53.705720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    39247 2024-05-05 10:43:30.037911 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.705720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2024-05-05 10:43:53.721720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2024-05-05 10:43:31.221901 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.721720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    13240 2024-05-05 10:43:53.721720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    18420 2024-05-05 10:43:31.417899 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.725720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2024-05-05 10:43:53.745720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2024-05-05 10:43:52.317731 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.745720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2024-05-05 10:43:53.749719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2024-05-05 10:43:52.533729 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2024-05-05 10:43:53.749719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     4308 2024-05-05 10:43:53.749719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     7410 2024-05-05 10:43:37.277852 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.753719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    15316 2024-05-05 10:43:53.753719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    14087 2024-05-05 10:43:37.477851 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    18465 2024-05-05 10:43:53.753719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2024-05-05 10:43:53.757719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2024-05-05 10:43:37.673849 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.757719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     5111 2024-05-05 10:43:53.765720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/management_pb2.py
--rw-r--r--   0        0        0     2739 2024-05-05 10:43:38.869840 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi
--rw-r--r--   0        0        0     5436 2024-05-05 10:43:53.765720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py
--rw-r--r--   0        0        0     5385 2024-05-05 10:43:53.761720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     7551 2024-05-05 10:43:38.469843 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.761720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    17474 2024-05-05 10:43:53.757719 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2024-05-05 10:43:38.265844 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2024-05-05 10:43:53.761720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2024-05-05 10:43:53.765720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2024-05-05 10:43:38.665841 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.765720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    27355 2024-05-05 10:43:53.729720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    43393 2024-05-05 10:43:32.017895 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.733720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5147 2024-05-05 10:43:53.733720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6208 2024-05-05 10:43:32.213893 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.733720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2024-05-05 10:43:53.737720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2024-05-05 10:43:32.413891 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2024-05-05 10:43:53.737720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11049 2024-05-05 10:43:53.737720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15942 2024-05-05 10:43:32.609890 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.741720 qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2024-05-05 10:43:53.957718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2024-05-05 10:43:50.973742 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.957718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2024-05-05 10:43:53.961718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2024-05-05 10:43:51.193740 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2024-05-05 10:43:53.961718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2024-05-05 10:43:53.961718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2024-05-05 10:43:51.425738 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.965718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2024-05-05 10:43:53.965718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2024-05-05 10:43:51.653736 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2024-05-05 10:43:53.965718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0    10469 2024-05-05 10:43:53.969718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0    11719 2024-05-05 10:43:51.893735 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     9458 2024-05-05 10:43:53.969718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     5302 2024-05-05 10:43:53.969718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     5484 2024-05-05 10:43:52.109733 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.969718 qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2975 2024-05-05 10:43:53.877719 qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     4026 2024-05-05 10:43:44.069797 qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.877719 qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4455 2024-05-05 10:43:53.877719 qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     3113 2024-05-05 10:43:44.281796 qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2024-05-05 10:43:53.881718 qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6950 2024-05-05 10:43:53.665720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    11560 2024-05-05 10:43:29.005919 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.669720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     3383 2024-05-05 10:43:53.669720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     5457 2024-05-05 10:43:29.201917 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.669720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2024-05-05 10:43:53.697720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2024-05-05 10:43:29.397916 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2024-05-05 10:43:53.697720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8504 2024-05-05 10:43:53.701720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12440 2024-05-05 10:43:29.597914 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.701720 qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2024-05-05 10:43:53.841719 qwak_core-0.4.0/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2024-05-05 10:43:40.977822 qwak_core-0.4.0/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2024-05-05 10:43:53.841719 qwak_core-0.4.0/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3876 2024-05-05 10:43:53.881718 qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4658 2024-05-05 10:43:44.497794 qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.881718 qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2024-05-05 10:43:53.885718 qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2024-05-05 10:43:44.705792 qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2024-05-05 10:43:53.885718 qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2024-05-05 10:43:53.897718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2024-05-05 10:43:45.985782 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.901718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2024-05-05 10:43:53.901718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2024-05-05 10:43:46.197780 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.901718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    25218 2024-05-05 10:43:53.905718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    31280 2024-05-05 10:43:46.421779 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.905718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13432 2024-05-05 10:43:53.905718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    22974 2024-05-05 10:43:46.633777 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.905718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12784 2024-05-05 10:43:53.909718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16585 2024-05-05 10:43:46.861775 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.909718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    51171 2024-05-05 10:43:53.913718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    40800 2024-05-05 10:43:47.105773 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    73869 2024-05-05 10:43:53.913718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2024-05-05 10:43:53.913718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2024-05-05 10:43:47.313771 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.917718 qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2024-05-05 10:43:53.889718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2024-05-05 10:43:45.133789 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.889718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2024-05-05 10:43:53.897718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2024-05-05 10:43:45.765784 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.897718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2024-05-05 10:43:53.889718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2024-05-05 10:43:45.357787 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2024-05-05 10:43:53.893718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2024-05-05 10:43:53.893718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2024-05-05 10:43:45.561786 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.893718 qwak_core-0.4.0/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    27866 2024-05-05 10:43:53.869719 qwak_core-0.4.0/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    32184 2024-05-05 10:43:43.417803 qwak_core-0.4.0/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    19830 2024-05-05 10:43:53.869719 qwak_core-0.4.0/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2024-05-05 10:43:53.645720 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2024-05-05 10:43:28.609922 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2024-05-05 10:43:53.645720 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2024-05-05 10:43:53.641720 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2024-05-05 10:43:28.409924 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.641720 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2024-05-05 10:43:53.645720 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2024-05-05 10:43:28.805920 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2024-05-05 10:43:53.649720 qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     1598 2024-05-05 10:43:53.949718 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py
--rw-r--r--   0        0        0     1221 2024-05-05 10:43:50.305747 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.949718 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2_grpc.py
--rw-r--r--   0        0        0    11437 2024-05-05 10:43:53.953718 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py
--rw-r--r--   0        0        0    12170 2024-05-05 10:43:50.741744 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi
--rw-r--r--   0        0        0     9793 2024-05-05 10:43:53.957718 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4060 2024-05-05 10:43:53.953718 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/population_pb2.py
--rw-r--r--   0        0        0     3906 2024-05-05 10:43:50.521746 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.953718 qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/population_pb2_grpc.py
--rw-r--r--   0        0        0    10804 2024-05-05 10:43:53.865719 qwak_core-0.4.0/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0    12120 2024-05-05 10:43:42.965806 qwak_core-0.4.0/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     9642 2024-05-05 10:43:53.865719 qwak_core-0.4.0/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2024-05-05 10:43:53.885718 qwak_core-0.4.0/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2024-05-05 10:43:44.917791 qwak_core-0.4.0/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2024-05-05 10:43:53.885718 qwak_core-0.4.0/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0    10718 2024-05-05 10:43:53.637720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0    12627 2024-05-05 10:43:26.213941 qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.641720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    19751 2024-05-05 10:43:53.637720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    13467 2024-05-05 10:43:26.013943 qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    24352 2024-05-05 10:43:53.637720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2024-05-05 10:43:53.629721 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2024-05-05 10:43:25.397948 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.629721 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2477 2024-05-05 10:43:53.629721 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2679 2024-05-05 10:43:25.605946 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.633720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2024-05-05 10:43:53.633720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2024-05-05 10:43:25.809944 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2024-05-05 10:43:53.633720 qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6909 2024-05-05 10:43:53.917718 qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     5186 2024-05-05 10:43:47.733768 qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2024-05-05 10:43:53.921718 qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7868 2024-05-05 10:43:53.917718 qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    12177 2024-05-05 10:43:47.525770 qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.917718 qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11396 2024-05-05 10:43:53.657720 qwak_core-0.4.0/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    15139 2024-05-05 10:43:27.601930 qwak_core-0.4.0/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.657720 qwak_core-0.4.0/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3645 2024-05-05 10:43:53.657720 qwak_core-0.4.0/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2983 2024-05-05 10:43:27.805929 qwak_core-0.4.0/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.661720 qwak_core-0.4.0/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     8648 2024-05-05 10:43:53.801719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py
--rw-r--r--   0        0        0    12852 2024-05-05 10:43:35.869864 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.801719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_pb2_grpc.py
--rw-r--r--   0        0        0    13830 2024-05-05 10:43:53.801719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py
--rw-r--r--   0        0        0    10297 2024-05-05 10:43:36.081862 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi
--rw-r--r--   0        0        0    17183 2024-05-05 10:43:53.805719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py
--rw-r--r--   0        0        0     1873 2024-05-05 10:43:53.797719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py
--rw-r--r--   0        0        0     1550 2024-05-05 10:43:35.665865 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.801719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2_grpc.py
--rw-r--r--   0        0        0     8996 2024-05-05 10:43:53.805719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/filters_pb2.py
--rw-r--r--   0        0        0    11380 2024-05-05 10:43:36.277860 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.805719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/filters_pb2_grpc.py
--rw-r--r--   0        0        0     4533 2024-05-05 10:43:53.809719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_pb2.py
--rw-r--r--   0        0        0     6103 2024-05-05 10:43:36.477859 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.809719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_pb2_grpc.py
--rw-r--r--   0        0        0     9738 2024-05-05 10:43:53.809719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py
--rw-r--r--   0        0        0    10977 2024-05-05 10:43:36.681857 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi
--rw-r--r--   0        0        0    10157 2024-05-05 10:43:53.813719 qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py
--rw-r--r--   0        0        0    10852 2024-05-05 10:43:53.973718 qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_pb2.py
--rw-r--r--   0        0        0    17043 2024-05-05 10:43:52.781727 qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-05 10:43:53.973718 qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_pb2_grpc.py
--rw-r--r--   0        0        0    21429 2024-05-05 10:43:53.973718 qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_service_pb2.py
--rw-r--r--   0        0        0    13726 2024-05-05 10:43:52.989726 qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi
--rw-r--r--   0        0        0    27193 2024-05-05 10:43:53.977718 qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py
--rw-r--r--   0        0        0     3696 2024-05-05 10:43:58.997677 qwak_core-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      585 2024-05-05 10:43:58.997677 qwak_core-0.4.0/qwak/__init__.py
--rw-r--r--   0        0        0     1522 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3228 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12456 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/automations/automations.py
--rw-r--r--   0        0        0    12907 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    26800 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     2404 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/_inner/__init__.py
--rw-r--r--   0        0        0      849 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/_inner/edge_communications.py
--rw-r--r--   0        0        0      224 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5340 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       43 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/alerts_registry/__init__.py
--rw-r--r--   0        0        0     4040 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/alerts_registry/channel.py
--rw-r--r--   0        0        0     5355 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/alerts_registry/client.py
--rw-r--r--   0        0        0       42 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2024-05-05 10:41:18.274960 qwak_core-0.4.0/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     9034 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    21054 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6882 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4209 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0      105 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0     5045 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/build_orchestrator/build_model_request_getter.py
--rw-r--r--   0        0        0    16148 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0     3981 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/build_orchestrator/internal_client.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     2401 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0      885 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/data_versioning/data_tag_filter.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6806 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     4051 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/feature_store/execution_management_client.py
--rw-r--r--   0        0        0     2635 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    16056 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     8022 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/feature_store/offline_serving_client.py
--rw-r--r--   0        0        0     5811 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     2505 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0      885 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/file_versioning/file_tag_filter.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2509 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9308 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     4431 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3581 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      102 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/vector_store/__init__.py
--rw-r--r--   0        0        0     4247 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/vector_store/management_client.py
--rw-r--r--   0        0        0     5293 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/vector_store/serving_client.py
--rw-r--r--   0        0        0       43 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/workspace_manager/__init__.py
--rw-r--r--   0        0        0     8136 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/clients/workspace_manager/client.py
--rw-r--r--   0        0        0      790 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      192 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      424 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_general_build_exception.py
--rw-r--r--   0        0        0      579 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0       54 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_load_configuration_exception.py
--rw-r--r--   0        0        0      274 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      137 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_remote_build_failed.py
--rw-r--r--   0        0        0      746 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/exceptions/qwak_suggestion_exception.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     1977 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/_common/artifact_utils.py
--rw-r--r--   0        0        0     7046 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/_common/feature_set_utils.py
--rw-r--r--   0        0        0     4707 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     6680 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/_common/packaging.py
--rw-r--r--   0        0        0     2316 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0     2694 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/base.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/__init__.py
--rw-r--r--   0        0        0      197 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/_batch.py
--rw-r--r--   0        0        0      658 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/_jdbc.py
--rw-r--r--   0        0        0    10805 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/athena.py
--rw-r--r--   0        0        0     3022 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/big_query.py
--rw-r--r--   0        0        0     2063 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/clickhouse.py
--rw-r--r--   0        0        0     1981 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/csv.py
--rw-r--r--   0        0        0     2130 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/elastic_search.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/__init__.py
--rw-r--r--   0        0        0     2828 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/aws.py
--rw-r--r--   0        0        0      245 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/base_config.py
--rw-r--r--   0        0        0     1572 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/gcp.py
--rw-r--r--   0        0        0     1874 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/utils.py
--rw-r--r--   0        0        0     1921 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/mongodb.py
--rw-r--r--   0        0        0     1595 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/mysql.py
--rw-r--r--   0        0        0     1867 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/parquet.py
--rw-r--r--   0        0        0     1648 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/postgres.py
--rw-r--r--   0        0        0     3114 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/redshift.py
--rw-r--r--   0        0        0     2579 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/snowflake.py
--rw-r--r--   0        0        0     1830 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/batch/vertica.py
--rw-r--r--   0        0        0      895 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/source_authentication.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/__init__.py
--rw-r--r--   0        0        0      181 2024-05-05 10:41:18.278960 qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/_streaming.py
--rw-r--r--   0        0        0      649 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/__init__.py
--rw-r--r--   0        0        0     3959 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/authentication.py
--rw-r--r--   0        0        0     3510 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/deserialization.py
--rw-r--r--   0        0        0     4398 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/kafka.py
--rw-r--r--   0        0        0     5984 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/data_sources/time_partition_columns.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     2313 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/execution/__init__.py
--rw-r--r--   0        0        0     6470 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/execution/backfill.py
--rw-r--r--   0        0        0    21243 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/execution/execution.py
--rw-r--r--   0        0        0     3564 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/execution/execution_query.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1636 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/_utils/_featureset_utils.py
--rw-r--r--   0        0        0     1979 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0     5285 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/base_feature_set.py
--rw-r--r--   0        0        0    16910 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1670 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0     1155 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0    23233 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/streaming.py
--rw-r--r--   0        0        0     9584 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/streaming_backfill.py
--rw-r--r--   0        0        0      733 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/aggregations/__init__.py
--rw-r--r--   0        0        0    14117 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py
--rw-r--r--   0        0        0     2253 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/aggregations/windows.py
--rw-r--r--   0        0        0      281 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/functions/__init__.py
--rw-r--r--   0        0        0     2425 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py
--rw-r--r--   0        0        0     1156 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/functions/schema.py
--rw-r--r--   0        0        0     9659 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/transformations.py
--rw-r--r--   0        0        0      173 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0     1216 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/_offline_serving_validations.py
--rw-r--r--   0        0        0      738 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28651 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0    12597 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/client_v2.py
--rw-r--r--   0        0        0      739 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/offline/feature_set_features.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0    11144 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0     2210 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/online/endpoint_utils.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/validations/__init__.py
--rw-r--r--   0        0        0     2656 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/validations/validation_options.py
--rw-r--r--   0        0        0     3783 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/validations/validation_response.py
--rw-r--r--   0        0        0     3864 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/feature_store/validations/validator.py
--rw-r--r--   0        0        0      226 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_config/__init__.py
--rw-r--r--   0        0        0    10978 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_config/build_config_v1.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/build_loggers/__init__.py
--rw-r--r--   0        0        0     1426 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/build_loggers/trigger_build_logger.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/constants/__init__.py
--rw-r--r--   0        0        0      209 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/constants/dependencies.py
--rw-r--r--   0        0        0      131 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/constants/host_resource.py
--rw-r--r--   0        0        0       94 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/constants/messages.py
--rw-r--r--   0        0        0       36 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/constants/temp_dir.py
--rw-r--r--   0        0        0      279 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/constants/upload_tag.py
--rw-r--r--   0        0        0      116 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/dependency_manager_type.py
--rw-r--r--   0        0        0     2299 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/execute_build_pipeline.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/__init__.py
--rw-r--r--   0        0        0      528 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/build_logger_interface.py
--rw-r--r--   0        0        0      675 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/build_phase.py
--rw-r--r--   0        0        0     2247 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/context_interface.py
--rw-r--r--   0        0        0     1723 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/phase_run_handler.py
--rw-r--r--   0        0        0      718 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/step_inteface.py
--rw-r--r--   0        0        0      585 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/interface/time_source.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/__init__.py
--rw-r--r--   0        0        0     1895 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/__init__.py
--rw-r--r--   0        0        0      953 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py
--rw-r--r--   0        0        0     2067 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/__init__.py
--rw-r--r--   0        0        0     5057 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/__init__.py
--rw-r--r--   0        0        0     5944 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py
--rw-r--r--   0        0        0     1424 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/__init__.py
--rw-r--r--   0        0        0     2258 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py
--rw-r--r--   0        0        0     5399 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py
--rw-r--r--   0        0        0    10894 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py
--rw-r--r--   0        0        0     1186 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/__init__.py
--rw-r--r--   0        0        0      618 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py
--rw-r--r--   0        0        0     1599 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py
--rw-r--r--   0        0        0     9553 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py
--rw-r--r--   0        0        0     1244 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/phases/phases_pipeline.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/run_handlers/__init__.py
--rw-r--r--   0        0        0     3484 2024-05-05 10:41:18.282960 qwak_core-0.4.0/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/build_logic/tools/__init__.py
--rw-r--r--   0        0        0     2498 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/build_logic/tools/dependencies_tools.py
--rw-r--r--   0        0        0     8228 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/build_logic/tools/files.py
--rw-r--r--   0        0        0      750 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/build_logic/tools/ignore_files.py
--rw-r--r--   0        0        0      188 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/build_logic/tools/text.py
--rw-r--r--   0        0        0      200 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/build_logic/trigger_build_context.py
--rw-r--r--   0        0        0     1084 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/const.py
--rw-r--r--   0        0        0     1595 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0      242 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0     1018 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      414 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/instance_template/__init__.py
--rw-r--r--   0        0        0     1916 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/instance_template/verify_template_id.py
--rw-r--r--   0        0        0     2933 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0       70 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/provider.py
--rw-r--r--   0        0        0      281 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      545 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3830 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      361 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     6897 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      422 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0     1686 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/protobuf_factory.py
--rw-r--r--   0        0        0      435 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     4200 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6976 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/__init__.py
--rw-r--r--   0        0        0     4762 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/_entity_extraction.py
--rw-r--r--   0        0        0     1739 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      322 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      321 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/base.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1938 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/decorators/api.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/decorators/impl/__init__.py
--rw-r--r--   0        0        0      993 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/decorators/impl/api_implementation.py
--rw-r--r--   0        0        0      215 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/decorators/impl/timer_implementation.py
--rw-r--r--   0        0        0      739 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/decorators/timer.py
--rw-r--r--   0        0        0     1503 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0     1981 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/schema.py
--rw-r--r--   0        0        0     2411 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      786 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     2176 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0     1560 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2712 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      798 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0     2289 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2938 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5472 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0     1757 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/batch_jobs/execution.py
--rw-r--r--   0        0        0     1531 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/batch_jobs/task.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/build_api_helpers/__init__.py
--rw-r--r--   0        0        0     1886 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/build_api_helpers/build_api_steps.py
--rw-r--r--   0        0        0      184 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/build_api_helpers/messages.py
--rw-r--r--   0        0        0     2355 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/build_api_helpers/trigger_build_api.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    26693 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/data_versioning/__init__.py
--rw-r--r--   0        0        0      806 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/data_versioning/data_tag.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13288 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/file_versioning/__init__.py
--rw-r--r--   0        0        0      806 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/file_versioning/file_tag.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.286960 qwak_core-0.4.0/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0     1191 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2247 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/utils/__init__.py
--rw-r--r--   0        0        0      581 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/utils/datetime_utils.py
--rw-r--r--   0        0        0      120 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/__init__.py
--rw-r--r--   0        0        0     6040 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/client.py
--rw-r--r--   0        0        0    16916 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/collection.py
--rw-r--r--   0        0        0     8209 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/filters.py
--rw-r--r--   0        0        0     3711 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/inference_client.py
--rw-r--r--   0        0        0     2658 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/rest_helpers.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/utils/__init__.py
--rw-r--r--   0        0        0      837 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/utils/filter_utils.py
--rw-r--r--   0        0        0     7459 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak/vector_store/utils/upsert_utils.py
--rw-r--r--   0        0        0       46 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2263 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/alert_registry_service_api.py
--rw-r--r--   0        0        0     2129 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1189 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    13129 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3686 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     4984 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     1264 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py
--rw-r--r--   0        0        0     5226 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     2453 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    20753 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1608 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0      886 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/execution_management_service.py
--rw-r--r--   0        0        0     3207 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     3400 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3712 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     6800 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     2592 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     1635 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/fs_offline_serving_service.py
--rw-r--r--   0        0        0     4567 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     1046 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/internal_build_orchestrator_service.py
--rw-r--r--   0        0        0     2696 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     4153 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     5500 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0     5722 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/vector_serving_api.py
--rw-r--r--   0        0        0     3594 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/vectors_management_api.py
--rw-r--r--   0        0        0     7591 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/mocks/workspace_manager_service_mock.py
--rw-r--r--   0        0        0    17551 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2024-05-05 10:41:18.290960 qwak_core-0.4.0/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     7299 1970-01-01 00:00:00.000000 qwak_core-0.4.0/setup.py
--rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 qwak_core-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      264 2024-05-05 15:10:06.930597 qwak_core-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 15:12:42.855743 qwak_core-0.4.1/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5877 2024-05-05 15:12:42.887743 qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     7824 2024-05-05 15:12:14.403534 qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.887743 qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0    12703 2024-05-05 15:12:42.887743 qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py
+-rw-r--r--   0        0        0    10914 2024-05-05 15:12:14.599536 qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi
+-rw-r--r--   0        0        0    14681 2024-05-05 15:12:42.891743 qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2024-05-05 15:12:42.879743 qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2024-05-05 15:12:14.007532 qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.883743 qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2024-05-05 15:12:42.883743 qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2024-05-05 15:12:14.203533 qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.883743 qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2024-05-05 15:12:42.875743 qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2024-05-05 15:12:13.415527 qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2024-05-05 15:12:42.875743 qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2024-05-05 15:12:42.875743 qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2024-05-05 15:12:13.611528 qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.879743 qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4901 2024-05-05 15:12:42.879743 qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5995 2024-05-05 15:12:13.807530 qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.879743 qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2024-05-05 15:12:42.859743 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2024-05-05 15:12:13.215525 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2024-05-05 15:12:42.859743 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7360 2024-05-05 15:12:42.859743 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0    11651 2024-05-05 15:12:14.799537 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.863743 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     5029 2024-05-05 15:12:42.867743 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     6943 2024-05-05 15:12:15.203540 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.867743 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2024-05-05 15:12:42.867743 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2024-05-05 15:12:15.403542 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2024-05-05 15:12:42.871743 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2024-05-05 15:12:42.863743 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2024-05-05 15:12:14.999539 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.863743 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6541 2024-05-05 15:12:42.871743 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10595 2024-05-05 15:12:15.599543 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.871743 qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0    15382 2024-05-05 15:12:42.923743 qwak_core-0.4.1/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    20668 2024-05-05 15:12:18.423564 qwak_core-0.4.1/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.923743 qwak_core-0.4.1/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2024-05-05 15:12:42.927744 qwak_core-0.4.1/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2024-05-05 15:12:18.623566 qwak_core-0.4.1/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2024-05-05 15:12:42.927744 qwak_core-0.4.1/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7616 2024-05-05 15:12:43.071745 qwak_core-0.4.1/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11995 2024-05-05 15:12:28.311637 qwak_core-0.4.1/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.071745 qwak_core-0.4.1/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0    14893 2024-05-05 15:12:43.071745 qwak_core-0.4.1/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0    11812 2024-05-05 15:12:28.515638 qwak_core-0.4.1/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    19155 2024-05-05 15:12:43.071745 qwak_core-0.4.1/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2024-05-05 15:12:43.075744 qwak_core-0.4.1/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2024-05-05 15:12:29.747647 qwak_core-0.4.1/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2024-05-05 15:12:43.079745 qwak_core-0.4.1/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8864 2024-05-05 15:12:43.075744 qwak_core-0.4.1/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13789 2024-05-05 15:12:29.539646 qwak_core-0.4.1/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.075744 qwak_core-0.4.1/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2024-05-05 15:12:43.079745 qwak_core-0.4.1/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2024-05-05 15:12:29.951649 qwak_core-0.4.1/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.079745 qwak_core-0.4.1/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2024-05-05 15:12:43.083745 qwak_core-0.4.1/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2024-05-05 15:12:30.147650 qwak_core-0.4.1/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2024-05-05 15:12:43.083745 qwak_core-0.4.1/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    14053 2024-05-05 15:12:43.199746 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    20860 2024-05-05 15:12:39.287717 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.199746 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2024-05-05 15:12:43.191745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2024-05-05 15:12:38.887714 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.195745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3954 2024-05-05 15:12:43.195745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     5309 2024-05-05 15:12:39.083715 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.195745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    21176 2024-05-05 15:12:43.187745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    15049 2024-05-05 15:12:38.487711 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    25475 2024-05-05 15:12:43.187745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2024-05-05 15:12:43.191745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2024-05-05 15:12:38.691712 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.191745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2024-05-05 15:12:43.203745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2024-05-05 15:12:39.875721 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.207745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2024-05-05 15:12:43.203745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2024-05-05 15:12:39.679720 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.203745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2024-05-05 15:12:43.199746 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2024-05-05 15:12:39.483718 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.203745 qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    11218 2024-05-05 15:12:43.183745 qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    15584 2024-05-05 15:12:38.279709 qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.187745 qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2083 2024-05-05 15:12:43.179745 qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1977 2024-05-05 15:12:37.871707 qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.179745 qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    46028 2024-05-05 15:12:43.183745 qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    60013 2024-05-05 15:12:38.079708 qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    32008 2024-05-05 15:12:43.183745 qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    29124 2024-05-05 15:12:43.115745 qwak_core-0.4.1/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    24434 2024-05-05 15:12:32.191665 qwak_core-0.4.1/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    27837 2024-05-05 15:12:43.115745 qwak_core-0.4.1/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    33279 2024-05-05 15:12:43.111745 qwak_core-0.4.1/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    52325 2024-05-05 15:12:31.791662 qwak_core-0.4.1/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.115745 qwak_core-0.4.1/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0     5757 2024-05-05 15:12:43.119745 qwak_core-0.4.1/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py
+-rw-r--r--   0        0        0     4013 2024-05-05 15:12:32.779669 qwak_core-0.4.1/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi
+-rw-r--r--   0        0        0     6783 2024-05-05 15:12:43.123745 qwak_core-0.4.1/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py
+-rw-r--r--   0        0        0     6016 2024-05-05 15:12:43.119745 qwak_core-0.4.1/_qwak_proto/qwak/build_settings/build_settings_pb2.py
+-rw-r--r--   0        0        0     7049 2024-05-05 15:12:32.583668 qwak_core-0.4.1/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.119745 qwak_core-0.4.1/_qwak_proto/qwak/build_settings/build_settings_pb2_grpc.py
+-rw-r--r--   0        0        0    14932 2024-05-05 15:12:43.099745 qwak_core-0.4.1/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    24192 2024-05-05 15:12:31.579661 qwak_core-0.4.1/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.103745 qwak_core-0.4.1/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     5552 2024-05-05 15:12:43.103745 qwak_core-0.4.1/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     7299 2024-05-05 15:12:31.987664 qwak_core-0.4.1/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.103745 qwak_core-0.4.1/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    15672 2024-05-05 15:12:43.103745 qwak_core-0.4.1/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0    12741 2024-05-05 15:12:32.387667 qwak_core-0.4.1/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    16925 2024-05-05 15:12:43.107745 qwak_core-0.4.1/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38491 2024-05-05 15:12:43.111745 qwak_core-0.4.1/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    53557 2024-05-05 15:12:33.403674 qwak_core-0.4.1/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2024-05-05 15:12:43.111745 qwak_core-0.4.1/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     3508 2024-05-05 15:12:43.107745 qwak_core-0.4.1/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     2300 2024-05-05 15:12:32.975671 qwak_core-0.4.1/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0     3101 2024-05-05 15:12:43.107745 qwak_core-0.4.1/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2270 2024-05-05 15:12:43.127745 qwak_core-0.4.1/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     2697 2024-05-05 15:12:33.815677 qwak_core-0.4.1/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.131745 qwak_core-0.4.1/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4458 2024-05-05 15:12:43.131745 qwak_core-0.4.1/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     3113 2024-05-05 15:12:34.007678 qwak_core-0.4.1/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2024-05-05 15:12:43.131745 qwak_core-0.4.1/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2024-05-05 15:12:43.091745 qwak_core-0.4.1/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2024-05-05 15:12:30.991656 qwak_core-0.4.1/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.095745 qwak_core-0.4.1/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11871 2024-05-05 15:12:43.095745 qwak_core-0.4.1/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     8790 2024-05-05 15:12:31.187658 qwak_core-0.4.1/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2024-05-05 15:12:43.095745 qwak_core-0.4.1/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2024-05-05 15:12:43.087745 qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2024-05-05 15:12:30.575653 qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.087745 qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    50041 2024-05-05 15:12:43.083745 qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    74372 2024-05-05 15:12:30.367652 qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.087745 qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    46309 2024-05-05 15:12:43.091745 qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    40356 2024-05-05 15:12:30.791655 qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    27756 2024-05-05 15:12:43.091745 qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3345 2024-05-05 15:12:42.911743 qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     4098 2024-05-05 15:12:17.403556 qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.911743 qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12707 2024-05-05 15:12:42.915743 qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    13800 2024-05-05 15:12:17.611558 qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.915743 qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    17949 2024-05-05 15:12:42.915743 qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    18562 2024-05-05 15:12:17.819560 qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    12833 2024-05-05 15:12:42.919743 qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6463 2024-05-05 15:12:43.023744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/backfill_pb2.py
+-rw-r--r--   0        0        0     7945 2024-05-05 15:12:23.679603 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.023744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/backfill_pb2_grpc.py
+-rw-r--r--   0        0        0     2971 2024-05-05 15:12:43.027744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/batch_pb2.py
+-rw-r--r--   0        0        0     3266 2024-05-05 15:12:23.875604 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.027744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     2210 2024-05-05 15:12:43.027744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/deletion_pb2.py
+-rw-r--r--   0        0        0     1540 2024-05-05 15:12:24.071606 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.031744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/deletion_pb2_grpc.py
+-rw-r--r--   0        0        0     5793 2024-05-05 15:12:43.031744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/execution_pb2.py
+-rw-r--r--   0        0        0     7373 2024-05-05 15:12:24.271607 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.031744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    14900 2024-05-05 15:12:43.035744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/execution_service_pb2.py
+-rw-r--r--   0        0        0    11103 2024-05-05 15:12:24.475609 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi
+-rw-r--r--   0        0        0    17220 2024-05-05 15:12:43.035744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7695 2024-05-05 15:12:43.039744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py
+-rw-r--r--   0        0        0    14959 2024-05-05 15:12:24.875612 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.039744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0    19304 2024-05-05 15:12:43.043744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0    16916 2024-05-05 15:12:25.075613 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    21145 2024-05-05 15:12:43.043744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8440 2024-05-05 15:12:43.035744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py
+-rw-r--r--   0        0        0    13312 2024-05-05 15:12:24.675610 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.039744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     2051 2024-05-05 15:12:43.043744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py
+-rw-r--r--   0        0        0     1952 2024-05-05 15:12:25.271615 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.047744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/execution_state_pb2_grpc.py
+-rw-r--r--   0        0        0    12222 2024-05-05 15:12:43.047744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py
+-rw-r--r--   0        0        0     7930 2024-05-05 15:12:25.463616 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi
+-rw-r--r--   0        0        0    14212 2024-05-05 15:12:43.047744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1685 2024-05-05 15:12:43.047744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py
+-rw-r--r--   0        0        0     1272 2024-05-05 15:12:25.667617 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.051744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2_grpc.py
+-rw-r--r--   0        0        0     6198 2024-05-05 15:12:43.051744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py
+-rw-r--r--   0        0        0     7677 2024-05-05 15:12:25.867619 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.051744 qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2024-05-05 15:12:42.999744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2024-05-05 15:12:23.479601 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.999744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2024-05-05 15:12:42.995744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2024-05-05 15:12:23.283600 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2024-05-05 15:12:42.999744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2024-05-05 15:12:42.967744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2024-05-05 15:12:21.083584 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.967744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0    13825 2024-05-05 15:12:42.979744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/deployment_pb2.py
+-rw-r--r--   0        0        0    19227 2024-05-05 15:12:22.075591 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.983744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     3307 2024-05-05 15:12:42.983744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py
+-rw-r--r--   0        0        0     1637 2024-05-05 15:12:22.275593 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0     3293 2024-05-05 15:12:42.983744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2024-05-05 15:12:42.963744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2024-05-05 15:12:20.883582 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.967744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2024-05-05 15:12:42.959744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2024-05-05 15:12:20.255578 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.959744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2024-05-05 15:12:42.963744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2024-05-05 15:12:20.683581 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2024-05-05 15:12:42.963744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2024-05-05 15:12:42.971744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2024-05-05 15:12:21.279585 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.971744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2024-05-05 15:12:42.971744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2024-05-05 15:12:21.479587 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2024-05-05 15:12:42.975744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    26853 2024-05-05 15:12:42.959744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    39247 2024-05-05 15:12:20.467579 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.959744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2024-05-05 15:12:42.975744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2024-05-05 15:12:21.675588 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.975744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    13240 2024-05-05 15:12:42.979744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    18420 2024-05-05 15:12:21.879590 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.979744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2024-05-05 15:12:42.999744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2024-05-05 15:12:41.859736 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.003744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2024-05-05 15:12:43.003744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2024-05-05 15:12:42.063737 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2024-05-05 15:12:43.003744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4308 2024-05-05 15:12:43.007744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     7410 2024-05-05 15:12:27.703632 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.007744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    15316 2024-05-05 15:12:43.007744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    14087 2024-05-05 15:12:27.907634 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    18465 2024-05-05 15:12:43.011744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2024-05-05 15:12:43.011744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2024-05-05 15:12:28.111635 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.011744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     5111 2024-05-05 15:12:43.023744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/management_pb2.py
+-rw-r--r--   0        0        0     2739 2024-05-05 15:12:29.335644 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi
+-rw-r--r--   0        0        0     5436 2024-05-05 15:12:43.023744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py
+-rw-r--r--   0        0        0     5385 2024-05-05 15:12:43.015744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     7551 2024-05-05 15:12:28.927641 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.019744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    17474 2024-05-05 15:12:43.015744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2024-05-05 15:12:28.719640 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2024-05-05 15:12:43.015744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2024-05-05 15:12:43.019744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2024-05-05 15:12:29.123643 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.019744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    27355 2024-05-05 15:12:42.987744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    43393 2024-05-05 15:12:22.479594 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.987744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5147 2024-05-05 15:12:42.987744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6208 2024-05-05 15:12:22.679596 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.991744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2024-05-05 15:12:42.991744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2024-05-05 15:12:22.883597 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2024-05-05 15:12:42.991744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11049 2024-05-05 15:12:42.995744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15942 2024-05-05 15:12:23.083598 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.995744 qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2024-05-05 15:12:43.215746 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2024-05-05 15:12:40.659727 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.215746 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2024-05-05 15:12:43.219746 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2024-05-05 15:12:40.855728 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2024-05-05 15:12:43.219746 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2024-05-05 15:12:43.219746 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2024-05-05 15:12:41.051730 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.223746 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2024-05-05 15:12:43.223746 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2024-05-05 15:12:41.255731 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2024-05-05 15:12:43.223746 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10469 2024-05-05 15:12:43.227746 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0    11719 2024-05-05 15:12:41.463733 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     9458 2024-05-05 15:12:43.227746 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5302 2024-05-05 15:12:43.227746 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     5484 2024-05-05 15:12:41.659734 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.227746 qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2975 2024-05-05 15:12:43.135745 qwak_core-0.4.1/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     4026 2024-05-05 15:12:34.207680 qwak_core-0.4.1/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.135745 qwak_core-0.4.1/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4455 2024-05-05 15:12:43.135745 qwak_core-0.4.1/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     3113 2024-05-05 15:12:34.411681 qwak_core-0.4.1/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2024-05-05 15:12:43.135745 qwak_core-0.4.1/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6950 2024-05-05 15:12:42.927744 qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    11560 2024-05-05 15:12:19.439571 qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.931743 qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     3383 2024-05-05 15:12:42.931743 qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     5457 2024-05-05 15:12:19.643573 qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.931743 qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2024-05-05 15:12:42.935743 qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2024-05-05 15:12:19.847575 qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2024-05-05 15:12:42.935743 qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8504 2024-05-05 15:12:42.955744 qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12440 2024-05-05 15:12:20.047576 qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.955744 qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2024-05-05 15:12:43.099745 qwak_core-0.4.1/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2024-05-05 15:12:31.383659 qwak_core-0.4.1/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2024-05-05 15:12:43.099745 qwak_core-0.4.1/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3876 2024-05-05 15:12:43.139745 qwak_core-0.4.1/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4658 2024-05-05 15:12:34.607683 qwak_core-0.4.1/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.139745 qwak_core-0.4.1/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2024-05-05 15:12:43.139745 qwak_core-0.4.1/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2024-05-05 15:12:34.803684 qwak_core-0.4.1/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2024-05-05 15:12:43.143745 qwak_core-0.4.1/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2024-05-05 15:12:43.155745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2024-05-05 15:12:35.987693 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.159745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2024-05-05 15:12:43.159745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2024-05-05 15:12:36.195694 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.159745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    25218 2024-05-05 15:12:43.159745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    31280 2024-05-05 15:12:36.407696 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.163745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13432 2024-05-05 15:12:43.163745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    22974 2024-05-05 15:12:36.615697 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.163745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12784 2024-05-05 15:12:43.167745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16585 2024-05-05 15:12:36.831699 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.167745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    51171 2024-05-05 15:12:43.167745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    40800 2024-05-05 15:12:37.059701 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    73869 2024-05-05 15:12:43.171745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2024-05-05 15:12:43.171745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2024-05-05 15:12:37.263702 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.171745 qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2024-05-05 15:12:43.147745 qwak_core-0.4.1/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2024-05-05 15:12:35.195687 qwak_core-0.4.1/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.147745 qwak_core-0.4.1/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2024-05-05 15:12:43.155745 qwak_core-0.4.1/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2024-05-05 15:12:35.783691 qwak_core-0.4.1/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.155745 qwak_core-0.4.1/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2024-05-05 15:12:43.147745 qwak_core-0.4.1/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2024-05-05 15:12:35.391688 qwak_core-0.4.1/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2024-05-05 15:12:43.151745 qwak_core-0.4.1/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2024-05-05 15:12:43.151745 qwak_core-0.4.1/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2024-05-05 15:12:35.587690 qwak_core-0.4.1/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.151745 qwak_core-0.4.1/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    27866 2024-05-05 15:12:43.127745 qwak_core-0.4.1/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    32184 2024-05-05 15:12:33.619675 qwak_core-0.4.1/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    19830 2024-05-05 15:12:43.127745 qwak_core-0.4.1/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2024-05-05 15:12:42.907743 qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2024-05-05 15:12:19.035569 qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2024-05-05 15:12:42.907743 qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2024-05-05 15:12:42.903743 qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2024-05-05 15:12:18.831567 qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.903743 qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2024-05-05 15:12:42.907743 qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2024-05-05 15:12:19.239570 qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2024-05-05 15:12:42.911743 qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1598 2024-05-05 15:12:43.207745 qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py
+-rw-r--r--   0        0        0     1221 2024-05-05 15:12:40.067723 qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.207745 qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2_grpc.py
+-rw-r--r--   0        0        0    11437 2024-05-05 15:12:43.211746 qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py
+-rw-r--r--   0        0        0    12170 2024-05-05 15:12:40.463725 qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi
+-rw-r--r--   0        0        0     9793 2024-05-05 15:12:43.215746 qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4060 2024-05-05 15:12:43.211746 qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/population_pb2.py
+-rw-r--r--   0        0        0     3906 2024-05-05 15:12:40.263724 qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.211746 qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/population_pb2_grpc.py
+-rw-r--r--   0        0        0    10804 2024-05-05 15:12:43.123745 qwak_core-0.4.1/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0    12120 2024-05-05 15:12:33.183672 qwak_core-0.4.1/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     9642 2024-05-05 15:12:43.123745 qwak_core-0.4.1/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2024-05-05 15:12:43.143745 qwak_core-0.4.1/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2024-05-05 15:12:34.999686 qwak_core-0.4.1/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2024-05-05 15:12:43.143745 qwak_core-0.4.1/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10718 2024-05-05 15:12:42.899743 qwak_core-0.4.1/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0    12627 2024-05-05 15:12:16.599551 qwak_core-0.4.1/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.903743 qwak_core-0.4.1/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    19751 2024-05-05 15:12:42.899743 qwak_core-0.4.1/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    13467 2024-05-05 15:12:16.399549 qwak_core-0.4.1/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    24352 2024-05-05 15:12:42.899743 qwak_core-0.4.1/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2024-05-05 15:12:42.891743 qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2024-05-05 15:12:15.795545 qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.891743 qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2477 2024-05-05 15:12:42.895743 qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2679 2024-05-05 15:12:15.995546 qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.895743 qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2024-05-05 15:12:42.895743 qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2024-05-05 15:12:16.195548 qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2024-05-05 15:12:42.895743 qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6909 2024-05-05 15:12:43.175745 qwak_core-0.4.1/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     5186 2024-05-05 15:12:37.675705 qwak_core-0.4.1/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2024-05-05 15:12:43.179745 qwak_core-0.4.1/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7868 2024-05-05 15:12:43.175745 qwak_core-0.4.1/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    12177 2024-05-05 15:12:37.471704 qwak_core-0.4.1/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.175745 qwak_core-0.4.1/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    11396 2024-05-05 15:12:42.919743 qwak_core-0.4.1/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    15139 2024-05-05 15:12:18.023561 qwak_core-0.4.1/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.919743 qwak_core-0.4.1/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3645 2024-05-05 15:12:42.923743 qwak_core-0.4.1/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2983 2024-05-05 15:12:18.219563 qwak_core-0.4.1/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:42.923743 qwak_core-0.4.1/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     8648 2024-05-05 15:12:43.055745 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py
+-rw-r--r--   0        0        0    12852 2024-05-05 15:12:26.275622 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.059744 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/collection_pb2_grpc.py
+-rw-r--r--   0        0        0    13830 2024-05-05 15:12:43.059744 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py
+-rw-r--r--   0        0        0    10297 2024-05-05 15:12:26.483623 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi
+-rw-r--r--   0        0        0    17183 2024-05-05 15:12:43.059744 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1873 2024-05-05 15:12:43.055745 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py
+-rw-r--r--   0        0        0     1550 2024-05-05 15:12:26.067620 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.055745 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2_grpc.py
+-rw-r--r--   0        0        0     8996 2024-05-05 15:12:43.063744 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/filters_pb2.py
+-rw-r--r--   0        0        0    11380 2024-05-05 15:12:26.691625 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.063744 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/filters_pb2_grpc.py
+-rw-r--r--   0        0        0     4533 2024-05-05 15:12:43.063744 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/vector_pb2.py
+-rw-r--r--   0        0        0     6103 2024-05-05 15:12:26.895626 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.067745 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/vector_pb2_grpc.py
+-rw-r--r--   0        0        0     9738 2024-05-05 15:12:43.067745 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py
+-rw-r--r--   0        0        0    10977 2024-05-05 15:12:27.099628 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi
+-rw-r--r--   0        0        0    10157 2024-05-05 15:12:43.067745 qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10852 2024-05-05 15:12:43.231746 qwak_core-0.4.1/_qwak_proto/qwak/workspace/workspace_pb2.py
+-rw-r--r--   0        0        0    17043 2024-05-05 15:12:42.263739 qwak_core-0.4.1/_qwak_proto/qwak/workspace/workspace_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-05 15:12:43.231746 qwak_core-0.4.1/_qwak_proto/qwak/workspace/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0    21429 2024-05-05 15:12:43.231746 qwak_core-0.4.1/_qwak_proto/qwak/workspace/workspace_service_pb2.py
+-rw-r--r--   0        0        0    13726 2024-05-05 15:12:42.467740 qwak_core-0.4.1/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi
+-rw-r--r--   0        0        0    27193 2024-05-05 15:12:43.235746 qwak_core-0.4.1/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3696 2024-05-05 15:12:45.047759 qwak_core-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      585 2024-05-05 15:12:45.047759 qwak_core-0.4.1/qwak/__init__.py
+-rw-r--r--   0        0        0     1522 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3228 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12456 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/automations/automations.py
+-rw-r--r--   0        0        0    12907 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    26800 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     2404 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/_inner/__init__.py
+-rw-r--r--   0        0        0      849 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/_inner/edge_communications.py
+-rw-r--r--   0        0        0      224 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5340 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       43 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/alerts_registry/__init__.py
+-rw-r--r--   0        0        0     4040 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/alerts_registry/channel.py
+-rw-r--r--   0        0        0     5355 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/alerts_registry/client.py
+-rw-r--r--   0        0        0       42 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     9034 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    21054 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6882 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4209 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0      105 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0     5045 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/build_orchestrator/build_model_request_getter.py
+-rw-r--r--   0        0        0    16148 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0     3981 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/build_orchestrator/internal_client.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     2401 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0      885 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/data_versioning/data_tag_filter.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6806 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     4051 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/feature_store/execution_management_client.py
+-rw-r--r--   0        0        0     2635 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    16056 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     8022 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/feature_store/offline_serving_client.py
+-rw-r--r--   0        0        0     5811 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     2505 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0      885 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/file_versioning/file_tag_filter.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2509 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9308 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     4431 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3581 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      102 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/vector_store/__init__.py
+-rw-r--r--   0        0        0     4247 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/vector_store/management_client.py
+-rw-r--r--   0        0        0     5293 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/vector_store/serving_client.py
+-rw-r--r--   0        0        0       43 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/workspace_manager/__init__.py
+-rw-r--r--   0        0        0     8136 2024-05-05 15:10:06.934597 qwak_core-0.4.1/qwak/clients/workspace_manager/client.py
+-rw-r--r--   0        0        0      790 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      192 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      424 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/qwak_general_build_exception.py
+-rw-r--r--   0        0        0      579 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0       54 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/qwak_load_configuration_exception.py
+-rw-r--r--   0        0        0      274 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      137 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/qwak_remote_build_failed.py
+-rw-r--r--   0        0        0      746 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/exceptions/qwak_suggestion_exception.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     1977 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/_common/artifact_utils.py
+-rw-r--r--   0        0        0     7046 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/_common/feature_set_utils.py
+-rw-r--r--   0        0        0     4707 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     6680 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/_common/packaging.py
+-rw-r--r--   0        0        0     2316 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0     2694 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/base.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/_batch.py
+-rw-r--r--   0        0        0      658 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/_jdbc.py
+-rw-r--r--   0        0        0    10805 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/athena.py
+-rw-r--r--   0        0        0     3022 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/big_query.py
+-rw-r--r--   0        0        0     2063 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/clickhouse.py
+-rw-r--r--   0        0        0     1981 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/csv.py
+-rw-r--r--   0        0        0     2130 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/elastic_search.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/filesystem/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/filesystem/aws.py
+-rw-r--r--   0        0        0      245 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/filesystem/base_config.py
+-rw-r--r--   0        0        0     1572 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/filesystem/gcp.py
+-rw-r--r--   0        0        0     1874 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/filesystem/utils.py
+-rw-r--r--   0        0        0     1921 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/mongodb.py
+-rw-r--r--   0        0        0     1595 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/mysql.py
+-rw-r--r--   0        0        0     1867 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/parquet.py
+-rw-r--r--   0        0        0     1648 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/postgres.py
+-rw-r--r--   0        0        0     3114 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/redshift.py
+-rw-r--r--   0        0        0     2579 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/snowflake.py
+-rw-r--r--   0        0        0     1830 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/batch/vertica.py
+-rw-r--r--   0        0        0      895 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/source_authentication.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/streaming/__init__.py
+-rw-r--r--   0        0        0      181 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/streaming/_streaming.py
+-rw-r--r--   0        0        0      649 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/streaming/kafka/__init__.py
+-rw-r--r--   0        0        0     3959 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/streaming/kafka/authentication.py
+-rw-r--r--   0        0        0     3510 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/streaming/kafka/deserialization.py
+-rw-r--r--   0        0        0     4398 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/streaming/kafka/kafka.py
+-rw-r--r--   0        0        0     5984 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/data_sources/time_partition_columns.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     2313 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/execution/__init__.py
+-rw-r--r--   0        0        0     6470 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/execution/backfill.py
+-rw-r--r--   0        0        0    21243 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/execution/execution.py
+-rw-r--r--   0        0        0     3564 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/execution/execution_query.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1636 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/_utils/_featureset_utils.py
+-rw-r--r--   0        0        0     1979 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0     5285 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/base_feature_set.py
+-rw-r--r--   0        0        0    16910 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1670 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0     1155 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0    23233 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/streaming.py
+-rw-r--r--   0        0        0     9584 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/streaming_backfill.py
+-rw-r--r--   0        0        0      733 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/aggregations/__init__.py
+-rw-r--r--   0        0        0    14117 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py
+-rw-r--r--   0        0        0     2253 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/aggregations/windows.py
+-rw-r--r--   0        0        0      281 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/functions/__init__.py
+-rw-r--r--   0        0        0     2425 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py
+-rw-r--r--   0        0        0     1156 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/functions/schema.py
+-rw-r--r--   0        0        0     9659 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/transformations.py
+-rw-r--r--   0        0        0      173 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0     1216 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/offline/_offline_serving_validations.py
+-rw-r--r--   0        0        0      738 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28651 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0    12597 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/offline/client_v2.py
+-rw-r--r--   0        0        0      739 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/offline/feature_set_features.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0    11144 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0     2210 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/online/endpoint_utils.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.938597 qwak_core-0.4.1/qwak/feature_store/validations/__init__.py
+-rw-r--r--   0        0        0     2656 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/feature_store/validations/validation_options.py
+-rw-r--r--   0        0        0     3783 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/feature_store/validations/validation_response.py
+-rw-r--r--   0        0        0     3864 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/feature_store/validations/validator.py
+-rw-r--r--   0        0        0      226 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_config/__init__.py
+-rw-r--r--   0        0        0    10978 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_config/build_config_v1.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/build_loggers/__init__.py
+-rw-r--r--   0        0        0     1426 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/build_loggers/trigger_build_logger.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/constants/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/constants/dependencies.py
+-rw-r--r--   0        0        0      131 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/constants/host_resource.py
+-rw-r--r--   0        0        0       94 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/constants/messages.py
+-rw-r--r--   0        0        0       36 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/constants/temp_dir.py
+-rw-r--r--   0        0        0      279 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/constants/upload_tag.py
+-rw-r--r--   0        0        0      116 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/dependency_manager_type.py
+-rw-r--r--   0        0        0     2299 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/execute_build_pipeline.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/interface/__init__.py
+-rw-r--r--   0        0        0      528 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/interface/build_logger_interface.py
+-rw-r--r--   0        0        0      675 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/interface/build_phase.py
+-rw-r--r--   0        0        0     2247 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/interface/context_interface.py
+-rw-r--r--   0        0        0     1723 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/interface/phase_run_handler.py
+-rw-r--r--   0        0        0      718 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/interface/step_inteface.py
+-rw-r--r--   0        0        0      585 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/interface/time_source.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/__init__.py
+-rw-r--r--   0        0        0     1895 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/__init__.py
+-rw-r--r--   0        0        0      953 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py
+-rw-r--r--   0        0        0     2067 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/__init__.py
+-rw-r--r--   0        0        0     5057 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/__init__.py
+-rw-r--r--   0        0        0     5944 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py
+-rw-r--r--   0        0        0     1424 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/__init__.py
+-rw-r--r--   0        0        0     2258 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py
+-rw-r--r--   0        0        0     5399 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py
+-rw-r--r--   0        0        0    10894 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py
+-rw-r--r--   0        0        0     1186 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/__init__.py
+-rw-r--r--   0        0        0      618 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py
+-rw-r--r--   0        0        0     1599 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py
+-rw-r--r--   0        0        0     9553 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py
+-rw-r--r--   0        0        0     1244 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/phases/phases_pipeline.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/run_handlers/__init__.py
+-rw-r--r--   0        0        0     3484 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/tools/__init__.py
+-rw-r--r--   0        0        0     2498 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/tools/dependencies_tools.py
+-rw-r--r--   0        0        0     8228 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/tools/files.py
+-rw-r--r--   0        0        0      750 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/tools/ignore_files.py
+-rw-r--r--   0        0        0      188 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/tools/text.py
+-rw-r--r--   0        0        0      200 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/build_logic/trigger_build_context.py
+-rw-r--r--   0        0        0     1084 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/const.py
+-rw-r--r--   0        0        0     1595 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0      242 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0     1018 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      414 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/instance_template/__init__.py
+-rw-r--r--   0        0        0     1916 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/instance_template/verify_template_id.py
+-rw-r--r--   0        0        0     2933 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0       70 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/provider.py
+-rw-r--r--   0        0        0      281 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      545 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3830 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      361 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     6897 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      422 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0     1686 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/tool/protobuf_factory.py
+-rw-r--r--   0        0        0      435 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     4200 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6976 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/__init__.py
+-rw-r--r--   0        0        0     4762 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/_entity_extraction.py
+-rw-r--r--   0        0        0     1739 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      322 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      321 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1938 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/decorators/impl/__init__.py
+-rw-r--r--   0        0        0      993 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/decorators/impl/api_implementation.py
+-rw-r--r--   0        0        0      215 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/decorators/impl/timer_implementation.py
+-rw-r--r--   0        0        0      739 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/decorators/timer.py
+-rw-r--r--   0        0        0     1503 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0     1981 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/schema.py
+-rw-r--r--   0        0        0     2411 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      786 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     2176 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.942597 qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0     1560 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2712 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      798 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0     2289 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2938 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5472 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0     1757 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/batch_jobs/execution.py
+-rw-r--r--   0        0        0     1531 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/batch_jobs/task.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/build_api_helpers/__init__.py
+-rw-r--r--   0        0        0     1886 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/build_api_helpers/build_api_steps.py
+-rw-r--r--   0        0        0      184 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/build_api_helpers/messages.py
+-rw-r--r--   0        0        0     2355 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/build_api_helpers/trigger_build_api.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    26693 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/data_versioning/__init__.py
+-rw-r--r--   0        0        0      806 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/data_versioning/data_tag.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13288 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/file_versioning/__init__.py
+-rw-r--r--   0        0        0      806 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/file_versioning/file_tag.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0     1191 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/utils/__init__.py
+-rw-r--r--   0        0        0      581 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/utils/datetime_utils.py
+-rw-r--r--   0        0        0      120 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/vector_store/__init__.py
+-rw-r--r--   0        0        0     6040 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/vector_store/client.py
+-rw-r--r--   0        0        0    16916 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/vector_store/collection.py
+-rw-r--r--   0        0        0     8209 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/vector_store/filters.py
+-rw-r--r--   0        0        0     3711 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/vector_store/inference_client.py
+-rw-r--r--   0        0        0     2658 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/vector_store/rest_helpers.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/vector_store/utils/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/vector_store/utils/filter_utils.py
+-rw-r--r--   0        0        0     7459 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak/vector_store/utils/upsert_utils.py
+-rw-r--r--   0        0        0       46 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2263 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/alert_registry_service_api.py
+-rw-r--r--   0        0        0     2129 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1189 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    13129 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3686 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     4984 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     1264 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py
+-rw-r--r--   0        0        0     5226 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     2453 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    20753 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1608 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0      886 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/execution_management_service.py
+-rw-r--r--   0        0        0     3207 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     3400 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3712 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     6800 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     2592 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     1635 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/fs_offline_serving_service.py
+-rw-r--r--   0        0        0     4567 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     1046 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/internal_build_orchestrator_service.py
+-rw-r--r--   0        0        0     2696 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     4153 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     5500 2024-05-05 15:10:06.946597 qwak_core-0.4.1/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2024-05-05 15:10:06.950597 qwak_core-0.4.1/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2024-05-05 15:10:06.950597 qwak_core-0.4.1/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2024-05-05 15:10:06.950597 qwak_core-0.4.1/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.950597 qwak_core-0.4.1/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-05 15:10:06.950597 qwak_core-0.4.1/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0     5722 2024-05-05 15:10:06.950597 qwak_core-0.4.1/qwak_services_mock/mocks/vector_serving_api.py
+-rw-r--r--   0        0        0     3594 2024-05-05 15:10:06.950597 qwak_core-0.4.1/qwak_services_mock/mocks/vectors_management_api.py
+-rw-r--r--   0        0        0     7591 2024-05-05 15:10:06.950597 qwak_core-0.4.1/qwak_services_mock/mocks/workspace_manager_service_mock.py
+-rw-r--r--   0        0        0    17551 2024-05-05 15:10:06.950597 qwak_core-0.4.1/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:10:06.950597 qwak_core-0.4.1/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2024-05-05 15:10:06.950597 qwak_core-0.4.1/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     7299 1970-01-01 00:00:00.000000 qwak_core-0.4.1/setup.py
+-rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 qwak_core-0.4.1/PKG-INFO
```

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/build_settings/build_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/backfill_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/backfill_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/batch_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/batch_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/deletion_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/deletion_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/execution_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/management_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/management_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/population_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/population_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/filters_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/filters_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/vector_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/workspace/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/workspace/workspace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_service_pb2.py` & `qwak_core-0.4.1/_qwak_proto/qwak/workspace/workspace_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi` & `qwak_core-0.4.1/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py` & `qwak_core-0.4.1/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/pyproject.toml` & `qwak_core-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.4.0"
+version = "0.4.1"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.4.0/qwak/__init__.py` & `qwak_core-0.4.1/qwak/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for qwak-core."""
 
 __author__ = "Qwak.ai"
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 from qwak.inner.di_configuration import wire_dependencies
 from qwak.model.experiment_tracking import log_metric, log_param
 from qwak.model_loggers.artifact_logger import load_file, log_file
 from qwak.model_loggers.data_logger import load_data, log_data
 from qwak.model_loggers.model_logger import load_model, log_model
```

### Comparing `qwak_core-0.4.0/qwak/automations/__init__.py` & `qwak_core-0.4.1/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/automations/automation_executions.py` & `qwak_core-0.4.1/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/automations/automations.py` & `qwak_core-0.4.1/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/automations/batch_execution_action.py` & `qwak_core-0.4.1/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.4.1/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/automations/common.py` & `qwak_core-0.4.1/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/_inner/edge_communications.py` & `qwak_core-0.4.1/qwak/clients/_inner/edge_communications.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.4.1/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/administration/authentication/client.py` & `qwak_core-0.4.1/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.4.1/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/administration/environment/client.py` & `qwak_core-0.4.1/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/administration/self_service/client.py` & `qwak_core-0.4.1/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/alert_management/client.py` & `qwak_core-0.4.1/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/alerts_registry/channel.py` & `qwak_core-0.4.1/qwak/clients/alerts_registry/channel.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/alerts_registry/client.py` & `qwak_core-0.4.1/qwak/clients/alerts_registry/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/analytics/client.py` & `qwak_core-0.4.1/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/audience/client.py` & `qwak_core-0.4.1/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/automation_management/client.py` & `qwak_core-0.4.1/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/autoscaling/client.py` & `qwak_core-0.4.1/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/batch_job_management/client.py` & `qwak_core-0.4.1/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.4.1/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/batch_job_management/results.py` & `qwak_core-0.4.1/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/build_management/client.py` & `qwak_core-0.4.1/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/build_orchestrator/build_model_request_getter.py` & `qwak_core-0.4.1/qwak/clients/build_orchestrator/build_model_request_getter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.4.1/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/build_orchestrator/internal_client.py` & `qwak_core-0.4.1/qwak/clients/build_orchestrator/internal_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/data_versioning/client.py` & `qwak_core-0.4.1/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/data_versioning/data_tag_filter.py` & `qwak_core-0.4.1/qwak/clients/data_versioning/data_tag_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/deployment/client.py` & `qwak_core-0.4.1/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/feature_store/execution_management_client.py` & `qwak_core-0.4.1/qwak/clients/feature_store/execution_management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.4.1/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/feature_store/management_client.py` & `qwak_core-0.4.1/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/feature_store/offline_serving_client.py` & `qwak_core-0.4.1/qwak/clients/feature_store/offline_serving_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.4.1/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/file_versioning/client.py` & `qwak_core-0.4.1/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/file_versioning/file_tag_filter.py` & `qwak_core-0.4.1/qwak/clients/file_versioning/file_tag_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/instance_template/client.py` & `qwak_core-0.4.1/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.4.1/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/logging_client/client.py` & `qwak_core-0.4.1/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/model_management/client.py` & `qwak_core-0.4.1/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/project/client.py` & `qwak_core-0.4.1/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/secret_service/client.py` & `qwak_core-0.4.1/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/user_application_instance/client.py` & `qwak_core-0.4.1/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/vector_store/management_client.py` & `qwak_core-0.4.1/qwak/clients/vector_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/vector_store/serving_client.py` & `qwak_core-0.4.1/qwak/clients/vector_store/serving_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/clients/workspace_manager/client.py` & `qwak_core-0.4.1/qwak/clients/workspace_manager/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/exceptions/__init__.py` & `qwak_core-0.4.1/qwak/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/exceptions/quiet_error.py` & `qwak_core-0.4.1/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.4.1/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/exceptions/qwak_suggestion_exception.py` & `qwak_core-0.4.1/qwak/exceptions/qwak_suggestion_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/_common/artifact_utils.py` & `qwak_core-0.4.1/qwak/feature_store/_common/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/_common/feature_set_utils.py` & `qwak_core-0.4.1/qwak/feature_store/_common/feature_set_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.4.1/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/_common/functions.py` & `qwak_core-0.4.1/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/_common/packaging.py` & `qwak_core-0.4.1/qwak/feature_store/_common/packaging.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/base.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/_jdbc.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/athena.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/athena.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/big_query.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/clickhouse.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/clickhouse.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/csv.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/elastic_search.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/aws.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/filesystem/aws.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/gcp.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/filesystem/gcp.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/filesystem/utils.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/filesystem/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/mongodb.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/mysql.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/parquet.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/postgres.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/redshift.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/snowflake.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/batch/vertica.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/batch/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/source_authentication.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/source_authentication.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/__init__.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/streaming/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/authentication.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/streaming/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/deserialization.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/streaming/kafka/deserialization.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/streaming/kafka/kafka.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/streaming/kafka/kafka.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/data_sources/time_partition_columns.py` & `qwak_core-0.4.1/qwak/feature_store/data_sources/time_partition_columns.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/entities/entity.py` & `qwak_core-0.4.1/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/execution/backfill.py` & `qwak_core-0.4.1/qwak/feature_store/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/execution/execution.py` & `qwak_core-0.4.1/qwak/feature_store/execution/execution.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/execution/execution_query.py` & `qwak_core-0.4.1/qwak/feature_store/execution/execution_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/_utils/_featureset_utils.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/_utils/_featureset_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/base_feature_set.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/base_feature_set.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/streaming.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/streaming.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/streaming_backfill.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/streaming_backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/__init__.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/aggregations/windows.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/aggregations/windows.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/functions/schema.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/functions/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/feature_sets/transformations/transformations.py` & `qwak_core-0.4.1/qwak/feature_store/feature_sets/transformations/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/offline/_offline_serving_validations.py` & `qwak_core-0.4.1/qwak/feature_store/offline/_offline_serving_validations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.4.1/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.4.1/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/offline/client.py` & `qwak_core-0.4.1/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/offline/client_v2.py` & `qwak_core-0.4.1/qwak/feature_store/offline/client_v2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/offline/feature_set_features.py` & `qwak_core-0.4.1/qwak/feature_store/offline/feature_set_features.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/online/client.py` & `qwak_core-0.4.1/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/online/endpoint_utils.py` & `qwak_core-0.4.1/qwak/feature_store/online/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/validations/validation_options.py` & `qwak_core-0.4.1/qwak/feature_store/validations/validation_options.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/validations/validation_response.py` & `qwak_core-0.4.1/qwak/feature_store/validations/validation_response.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/feature_store/validations/validator.py` & `qwak_core-0.4.1/qwak/feature_store/validations/validator.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_config/build_config_v1.py` & `qwak_core-0.4.1/qwak/inner/build_config/build_config_v1.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/build_loggers/trigger_build_logger.py` & `qwak_core-0.4.1/qwak/inner/build_logic/build_loggers/trigger_build_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/execute_build_pipeline.py` & `qwak_core-0.4.1/qwak/inner/build_logic/execute_build_pipeline.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/interface/build_logger_interface.py` & `qwak_core-0.4.1/qwak/inner/build_logic/interface/build_logger_interface.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/interface/build_phase.py` & `qwak_core-0.4.1/qwak/inner/build_logic/interface/build_phase.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/interface/context_interface.py` & `qwak_core-0.4.1/qwak/inner/build_logic/interface/context_interface.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/interface/phase_run_handler.py` & `qwak_core-0.4.1/qwak/inner/build_logic/interface/phase_run_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/interface/step_inteface.py` & `qwak_core-0.4.1/qwak/inner/build_logic/interface/step_inteface.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/interface/time_source.py` & `qwak_core-0.4.1/qwak/inner/build_logic/interface/time_source.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/phases/phases_pipeline.py` & `qwak_core-0.4.1/qwak/inner/build_logic/phases/phases_pipeline.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py` & `qwak_core-0.4.1/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/tools/dependencies_tools.py` & `qwak_core-0.4.1/qwak/inner/build_logic/tools/dependencies_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/tools/files.py` & `qwak_core-0.4.1/qwak/inner/build_logic/tools/files.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/build_logic/tools/ignore_files.py` & `qwak_core-0.4.1/qwak/inner/build_logic/tools/ignore_files.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/const.py` & `qwak_core-0.4.1/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.4.1/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/di_configuration/account.py` & `qwak_core-0.4.1/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/di_configuration/containers.py` & `qwak_core-0.4.1/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/instance_template/verify_template_id.py` & `qwak_core-0.4.1/qwak/inner/instance_template/verify_template_id.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/model_loggers_utils.py` & `qwak_core-0.4.1/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/runtime_di/containers.py` & `qwak_core-0.4.1/qwak/inner/runtime_di/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/singleton_meta.py` & `qwak_core-0.4.1/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/tool/auth.py` & `qwak_core-0.4.1/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.4.1/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/tool/protobuf_factory.py` & `qwak_core-0.4.1/qwak/inner/tool/protobuf_factory.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/tool/run_config/base.py` & `qwak_core-0.4.1/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.4.1/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/_entity_extraction.py` & `qwak_core-0.4.1/qwak/model/_entity_extraction.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/adapters/__init__.py` & `qwak_core-0.4.1/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.4.1/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.4.1/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.4.1/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.4.1/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.4.1/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/base.py` & `qwak_core-0.4.1/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/decorators/api.py` & `qwak_core-0.4.1/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/decorators/impl/api_implementation.py` & `qwak_core-0.4.1/qwak/model/decorators/impl/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/decorators/timer.py` & `qwak_core-0.4.1/qwak/model/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/experiment_tracking.py` & `qwak_core-0.4.1/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/schema.py` & `qwak_core-0.4.1/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/schema_entities.py` & `qwak_core-0.4.1/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/__init__.py` & `qwak_core-0.4.1/qwak/model/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.4.1/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/adapters/input.py` & `qwak_core-0.4.1/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.4.1/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/adapters/output.py` & `qwak_core-0.4.1/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.4.1/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.4.1/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.4.1/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.4.1/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model/tools/run_model_locally.py` & `qwak_core-0.4.1/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.4.1/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model_loggers/data_logger.py` & `qwak_core-0.4.1/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/model_loggers/model_logger.py` & `qwak_core-0.4.1/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/batch_jobs/execution.py` & `qwak_core-0.4.1/qwak/qwak_client/batch_jobs/execution.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/batch_jobs/task.py` & `qwak_core-0.4.1/qwak/qwak_client/batch_jobs/task.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/build_api_helpers/build_api_steps.py` & `qwak_core-0.4.1/qwak/qwak_client/build_api_helpers/build_api_steps.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/build_api_helpers/trigger_build_api.py` & `qwak_core-0.4.1/qwak/qwak_client/build_api_helpers/trigger_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/builds/build.py` & `qwak_core-0.4.1/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.4.1/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.4.1/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/client.py` & `qwak_core-0.4.1/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/data_versioning/data_tag.py` & `qwak_core-0.4.1/qwak/qwak_client/data_versioning/data_tag.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.4.1/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/file_versioning/file_tag.py` & `qwak_core-0.4.1/qwak/qwak_client/file_versioning/file_tag.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/models/model.py` & `qwak_core-0.4.1/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.4.1/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/qwak_client/projects/project.py` & `qwak_core-0.4.1/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/tools/logger/logger.py` & `qwak_core-0.4.1/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/tools/logger/logging.yml` & `qwak_core-0.4.1/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/utils/datetime_utils.py` & `qwak_core-0.4.1/qwak/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/vector_store/client.py` & `qwak_core-0.4.1/qwak/vector_store/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/vector_store/collection.py` & `qwak_core-0.4.1/qwak/vector_store/collection.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/vector_store/filters.py` & `qwak_core-0.4.1/qwak/vector_store/filters.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/vector_store/inference_client.py` & `qwak_core-0.4.1/qwak/vector_store/inference_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/vector_store/rest_helpers.py` & `qwak_core-0.4.1/qwak/vector_store/rest_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/vector_store/utils/filter_utils.py` & `qwak_core-0.4.1/qwak/vector_store/utils/filter_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak/vector_store/utils/upsert_utils.py` & `qwak_core-0.4.1/qwak/vector_store/utils/upsert_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/alert_registry_service_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/alert_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/execution_management_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/execution_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/fs_offline_serving_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/fs_offline_serving_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/internal_build_orchestrator_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/internal_build_orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/vector_serving_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/vector_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/vectors_management_api.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/vectors_management_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/mocks/workspace_manager_service_mock.py` & `qwak_core-0.4.1/qwak_services_mock/mocks/workspace_manager_service_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/qwak_services_mock/services_mock.py` & `qwak_core-0.4.1/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.0/setup.py` & `qwak_core-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 {':extra == "feature-store"': ['cloudpickle==2.2.1'],
  ':python_full_version >= "3.7.1" and python_version < "3.10"': ['protobuf>=3.10,<4'],
  ':python_version >= "3.10"': ['protobuf>=4.21.6'],
  'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.4.0/PKG-INFO` & `qwak_core-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.4.0
+Version: 0.4.1
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

