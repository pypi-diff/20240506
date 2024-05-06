# Comparing `tmp/notehub_py-0.0.1.tar.gz` & `tmp/notehub_py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notehub_py-0.0.1.tar", last modified: Fri May  3 20:55:03 2024, max compression
+gzip compressed data, was "notehub_py-0.0.2.tar", last modified: Mon May  6 18:35:07 2024, max compression
```

## Comparing `notehub_py-0.0.1.tar` & `notehub_py-0.0.2.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:55:03.344746 notehub_py-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    17774 2024-05-03 20:55:03.344746 notehub_py-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17320 2024-05-03 20:54:58.000000 notehub_py-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:55:03.308745 notehub_py-0.0.1/notehub_py/
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:55:03.312745 notehub_py-0.0.1/notehub_py/api/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11436 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/api/authorization_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/api/billing_account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   332797 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/api/device_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    77521 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/api/event_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/api/firmware_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53448 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/api/monitor_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   268692 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    69340 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/api/route_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26297 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15624 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:55:03.328745 notehub_py-0.0.1/notehub_py/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/billing_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/billing_account_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/body.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/clone_project_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/create_fleet_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/create_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/create_product_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/delete_device_fleets_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/device_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/device_tower_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/device_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/dfu_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/dfu_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/firmware_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/fleet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_billing_accounts200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_device_environment_variables200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_device_health_log200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_device_health_log200_response_health_log_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_device_latest200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_device_public_key200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_device_sessions200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_project_device_public_keys200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_project_device_public_keys200_response_device_public_keys_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_project_devices200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_project_events200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_project_events_by_cursor200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_project_fleets200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_project_members200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_project_products200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_projects200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/get_route_logs_by_route200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/handle_note_changes200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/handle_note_get200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/handle_note_signal200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/handle_notefile_changes200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/handle_notefile_changes_pending200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/handle_notefile_delete_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/http_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/http_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/login200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/login_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/monitor_alert_routes_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/monitor_thresholds.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/post_provision_project_device_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/product.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/project_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/put_device_fleets_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/radresponder.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/route.py
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/route_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/snowflake_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/thingworx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/tower_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/twilio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/update_fleet_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/models/user_db_route.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-05-03 20:54:58.000000 notehub_py-0.0.1/notehub_py/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:55:03.344746 notehub_py-0.0.1/notehub_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17774 2024-05-03 20:55:03.000000 notehub_py-0.0.1/notehub_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-03 20:55:03.000000 notehub_py-0.0.1/notehub_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:55:03.000000 notehub_py-0.0.1/notehub_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 20:55:03.000000 notehub_py-0.0.1/notehub_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 20:55:03.000000 notehub_py-0.0.1/notehub_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-03 20:54:58.000000 notehub_py-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 20:55:03.344746 notehub_py-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-03 20:54:58.000000 notehub_py-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:55:03.340746 notehub_py-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_authorization_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_billing_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_billing_account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_billing_account_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_clone_project_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_create_fleet_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_create_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_create_product_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_delete_device_fleets_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_device_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_device_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_device_tower_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_device_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_dfu_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_dfu_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_event_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_firmware_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_firmware_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_fleet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_billing_accounts200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_device_environment_variables200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_device_health_log200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_device_health_log200_response_health_log_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_device_latest200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_device_public_key200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_device_sessions200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_project_device_public_keys200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_project_device_public_keys200_response_device_public_keys_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_project_devices200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_project_events200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_project_events_by_cursor200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_project_fleets200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_project_members200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_project_products200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_projects200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_get_route_logs_by_route200_response_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_handle_note_changes200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_handle_note_get200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_handle_note_signal200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_handle_notefile_changes200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_handle_notefile_changes_pending200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_handle_notefile_delete_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_http_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_http_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_login200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_login_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_monitor_alert_routes_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_monitor_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_monitor_thresholds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_post_provision_project_device_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_project_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_project_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_put_device_fleets_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_radresponder.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_route_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_route_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_slack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_snowflake_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_thingworx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_tower_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_twilio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_update_fleet_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-03 20:54:58.000000 notehub_py-0.0.1/test/test_user_db_route.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:35:07.832877 notehub_py-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-05-06 18:35:07.832877 notehub_py-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17320 2024-05-06 18:35:02.000000 notehub_py-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:35:07.804877 notehub_py-0.0.2/notehub_py/
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:35:07.808877 notehub_py-0.0.2/notehub_py/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11436 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/api/authorization_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/api/billing_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   332797 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/api/device_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77521 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/api/event_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/api/firmware_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53448 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/api/monitor_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   268692 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69340 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/api/route_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26297 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15624 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:35:07.820877 notehub_py-0.0.2/notehub_py/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/billing_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/billing_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/clone_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/create_fleet_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/create_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/create_product_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/delete_device_fleets_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/device_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/device_tower_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/device_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/dfu_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/dfu_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/firmware_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/fleet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_billing_accounts200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_device_environment_variables200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_device_health_log200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_device_health_log200_response_health_log_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_device_latest200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_device_public_key200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_device_sessions200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_project_device_public_keys200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_project_device_public_keys200_response_device_public_keys_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_project_devices200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_project_events200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_project_events_by_cursor200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_project_fleets200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_project_members200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_project_products200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_projects200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/get_route_logs_by_route200_response_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/handle_note_changes200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/handle_note_get200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/handle_note_signal200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/handle_notefile_changes200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/handle_notefile_changes_pending200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/handle_notefile_delete_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/http_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/http_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/login200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/login_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/monitor_alert_routes_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/monitor_thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/post_provision_project_device_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/project_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/put_device_fleets_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/radresponder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/route_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/snowflake_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/thingworx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/tower_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/twilio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/update_fleet_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/models/user_db_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-05-06 18:35:02.000000 notehub_py-0.0.2/notehub_py/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:35:07.832877 notehub_py-0.0.2/notehub_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-05-06 18:35:07.000000 notehub_py-0.0.2/notehub_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-06 18:35:07.000000 notehub_py-0.0.2/notehub_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:35:07.000000 notehub_py-0.0.2/notehub_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 18:35:07.000000 notehub_py-0.0.2/notehub_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 18:35:07.000000 notehub_py-0.0.2/notehub_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-06 18:35:02.000000 notehub_py-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 18:35:07.832877 notehub_py-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-06 18:35:02.000000 notehub_py-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:35:07.832877 notehub_py-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_authorization_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_billing_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_billing_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_billing_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_clone_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_create_fleet_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_create_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_create_product_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_delete_device_fleets_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_device_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_device_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_device_tower_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_device_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_dfu_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_dfu_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_event_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_firmware_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_firmware_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_fleet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_billing_accounts200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_device_environment_variables200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_device_health_log200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_device_health_log200_response_health_log_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_device_latest200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_device_public_key200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_device_sessions200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_project_device_public_keys200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_project_device_public_keys200_response_device_public_keys_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_project_devices200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_project_events200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_project_events_by_cursor200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_project_fleets200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_project_members200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_project_products200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_projects200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_get_route_logs_by_route200_response_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_handle_note_changes200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_handle_note_get200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_handle_note_signal200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_handle_notefile_changes200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_handle_notefile_changes_pending200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_handle_notefile_delete_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_http_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_http_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_login200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_login_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_monitor_alert_routes_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_monitor_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_monitor_thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_post_provision_project_device_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_project_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_project_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_put_device_fleets_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_radresponder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_route_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_route_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_snowflake_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_thingworx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_tower_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_twilio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_update_fleet_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-06 18:35:02.000000 notehub_py-0.0.2/test/test_user_db_route.py
```

### Comparing `notehub_py-0.0.1/PKG-INFO` & `notehub_py-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 Metadata-Version: 2.1
 Name: notehub-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python-based library for accessing the Blues Notehub API.
 Home-page: https://github.com/blues/notehub-py
 Author: Blues Engineering
 Author-email: engineering@blues.io
 Keywords: OpenAPI,OpenAPI-Generator,Notehub API
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
 Requires-Dist: python-dateutil
 Requires-Dist: pydantic>=2
 Requires-Dist: typing-extensions>=4.7.1
 
 # notehub-py
 The OpenAPI definition for the Notehub.io API.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 0.0.1
+- Package version: 0.0.2
 - Generator version: 7.5.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://dev.blues.io/support/](https://dev.blues.io/support/)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `notehub_py-0.0.1/README.md` & `notehub_py-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # notehub-py
 The OpenAPI definition for the Notehub.io API.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 0.0.1
+- Package version: 0.0.2
 - Generator version: 7.5.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://dev.blues.io/support/](https://dev.blues.io/support/)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `notehub_py-0.0.1/notehub_py/__init__.py` & `notehub_py-0.0.2/notehub_py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: engineering@blues.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 # import apis into sdk package
 from notehub_py.api.authorization_api import AuthorizationApi
 from notehub_py.api.billing_account_api import BillingAccountApi
 from notehub_py.api.device_api import DeviceApi
 from notehub_py.api.event_api import EventApi
 from notehub_py.api.firmware_api import FirmwareApi
```

### Comparing `notehub_py-0.0.1/notehub_py/api/authorization_api.py` & `notehub_py-0.0.2/notehub_py/api/authorization_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/api/billing_account_api.py` & `notehub_py-0.0.2/notehub_py/api/billing_account_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/api/device_api.py` & `notehub_py-0.0.2/notehub_py/api/device_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/api/event_api.py` & `notehub_py-0.0.2/notehub_py/api/event_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/api/firmware_api.py` & `notehub_py-0.0.2/notehub_py/api/firmware_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/api/monitor_api.py` & `notehub_py-0.0.2/notehub_py/api/monitor_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/api/project_api.py` & `notehub_py-0.0.2/notehub_py/api/project_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/api/route_api.py` & `notehub_py-0.0.2/notehub_py/api/route_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/api_client.py` & `notehub_py-0.0.2/notehub_py/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.0.1/python'
+        self.user_agent = 'OpenAPI-Generator/0.0.2/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `notehub_py-0.0.1/notehub_py/api_response.py` & `notehub_py-0.0.2/notehub_py/api_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/configuration.py` & `notehub_py-0.0.2/notehub_py/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 0.0.1".\
+               "SDK Package Version: 0.0.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `notehub_py-0.0.1/notehub_py/exceptions.py` & `notehub_py-0.0.2/notehub_py/exceptions.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/__init__.py` & `notehub_py-0.0.2/notehub_py/models/__init__.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/aws.py` & `notehub_py-0.0.2/notehub_py/models/aws.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/azure.py` & `notehub_py-0.0.2/notehub_py/models/azure.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/billing_account.py` & `notehub_py-0.0.2/notehub_py/models/billing_account.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/billing_account_role.py` & `notehub_py-0.0.2/notehub_py/models/billing_account_role.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/body.py` & `notehub_py-0.0.2/notehub_py/models/body.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/clone_project_request.py` & `notehub_py-0.0.2/notehub_py/models/clone_project_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/contact.py` & `notehub_py-0.0.2/notehub_py/models/contact.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/create_fleet_request.py` & `notehub_py-0.0.2/notehub_py/models/create_fleet_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/create_monitor.py` & `notehub_py-0.0.2/notehub_py/models/create_monitor.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/create_product_request.py` & `notehub_py-0.0.2/notehub_py/models/create_product_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/create_project_request.py` & `notehub_py-0.0.2/notehub_py/models/create_project_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/delete_device_fleets_request.py` & `notehub_py-0.0.2/notehub_py/models/delete_device_fleets_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/device.py` & `notehub_py-0.0.2/notehub_py/models/device.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/device_session.py` & `notehub_py-0.0.2/notehub_py/models/device_session.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/device_tower_info.py` & `notehub_py-0.0.2/notehub_py/models/device_tower_info.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/device_usage.py` & `notehub_py-0.0.2/notehub_py/models/device_usage.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/dfu_env.py` & `notehub_py-0.0.2/notehub_py/models/dfu_env.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/dfu_state.py` & `notehub_py-0.0.2/notehub_py/models/dfu_state.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/environment_variables.py` & `notehub_py-0.0.2/notehub_py/models/environment_variables.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/error.py` & `notehub_py-0.0.2/notehub_py/models/error.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/event.py` & `notehub_py-0.0.2/notehub_py/models/event.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/firmware_info.py` & `notehub_py-0.0.2/notehub_py/models/firmware_info.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/fleet.py` & `notehub_py-0.0.2/notehub_py/models/fleet.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_billing_accounts200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_billing_accounts200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_device_environment_variables200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_device_environment_variables200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_device_health_log200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_device_health_log200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_device_health_log200_response_health_log_inner.py` & `notehub_py-0.0.2/notehub_py/models/get_device_health_log200_response_health_log_inner.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_device_latest200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_device_latest200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_device_public_key200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_device_public_key200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_device_sessions200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_device_sessions200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_project_device_public_keys200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_project_device_public_keys200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_project_device_public_keys200_response_device_public_keys_inner.py` & `notehub_py-0.0.2/notehub_py/models/get_project_device_public_keys200_response_device_public_keys_inner.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_project_devices200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_project_devices200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_project_events200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_project_events200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_project_events_by_cursor200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_project_events_by_cursor200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_project_fleets200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_project_fleets200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_project_members200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_project_members200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_project_products200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_project_products200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_projects200_response.py` & `notehub_py-0.0.2/notehub_py/models/get_projects200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/get_route_logs_by_route200_response_inner.py` & `notehub_py-0.0.2/notehub_py/models/get_route_logs_by_route200_response_inner.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/google.py` & `notehub_py-0.0.2/notehub_py/models/google.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/handle_note_changes200_response.py` & `notehub_py-0.0.2/notehub_py/models/handle_note_changes200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/handle_note_get200_response.py` & `notehub_py-0.0.2/notehub_py/models/handle_note_get200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/handle_note_signal200_response.py` & `notehub_py-0.0.2/notehub_py/models/handle_note_signal200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/handle_notefile_changes200_response.py` & `notehub_py-0.0.2/notehub_py/models/handle_notefile_changes200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/handle_notefile_changes_pending200_response.py` & `notehub_py-0.0.2/notehub_py/models/handle_notefile_changes_pending200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/handle_notefile_delete_request.py` & `notehub_py-0.0.2/notehub_py/models/handle_notefile_delete_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/http.py` & `notehub_py-0.0.2/notehub_py/models/http.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/http_filter.py` & `notehub_py-0.0.2/notehub_py/models/http_filter.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/http_transform.py` & `notehub_py-0.0.2/notehub_py/models/http_transform.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/location.py` & `notehub_py-0.0.2/notehub_py/models/location.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/login200_response.py` & `notehub_py-0.0.2/notehub_py/models/login200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/login_request.py` & `notehub_py-0.0.2/notehub_py/models/login_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/monitor.py` & `notehub_py-0.0.2/notehub_py/models/monitor.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/monitor_alert_routes_inner.py` & `notehub_py-0.0.2/notehub_py/models/monitor_alert_routes_inner.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/monitor_thresholds.py` & `notehub_py-0.0.2/notehub_py/models/monitor_thresholds.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/mqtt.py` & `notehub_py-0.0.2/notehub_py/models/mqtt.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/note.py` & `notehub_py-0.0.2/notehub_py/models/note.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/post_provision_project_device_request.py` & `notehub_py-0.0.2/notehub_py/models/post_provision_project_device_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/product.py` & `notehub_py-0.0.2/notehub_py/models/product.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/project.py` & `notehub_py-0.0.2/notehub_py/models/project.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/project_member.py` & `notehub_py-0.0.2/notehub_py/models/project_member.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/proxy.py` & `notehub_py-0.0.2/notehub_py/models/proxy.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/put_device_fleets_request.py` & `notehub_py-0.0.2/notehub_py/models/put_device_fleets_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/radresponder.py` & `notehub_py-0.0.2/notehub_py/models/radresponder.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/role.py` & `notehub_py-0.0.2/notehub_py/models/role.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/route.py` & `notehub_py-0.0.2/notehub_py/models/route.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/route_schema.py` & `notehub_py-0.0.2/notehub_py/models/route_schema.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/slack.py` & `notehub_py-0.0.2/notehub_py/models/slack.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/snowflake.py` & `notehub_py-0.0.2/notehub_py/models/snowflake.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/snowflake_transform.py` & `notehub_py-0.0.2/notehub_py/models/snowflake_transform.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/thingworx.py` & `notehub_py-0.0.2/notehub_py/models/thingworx.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/tower_location.py` & `notehub_py-0.0.2/notehub_py/models/tower_location.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/twilio.py` & `notehub_py-0.0.2/notehub_py/models/twilio.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/update_fleet_request.py` & `notehub_py-0.0.2/notehub_py/models/update_fleet_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/models/user_db_route.py` & `notehub_py-0.0.2/notehub_py/models/user_db_route.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py/rest.py` & `notehub_py-0.0.2/notehub_py/rest.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/notehub_py.egg-info/PKG-INFO` & `notehub_py-0.0.2/notehub_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 Metadata-Version: 2.1
 Name: notehub-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python-based library for accessing the Blues Notehub API.
 Home-page: https://github.com/blues/notehub-py
 Author: Blues Engineering
 Author-email: engineering@blues.io
 Keywords: OpenAPI,OpenAPI-Generator,Notehub API
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
 Requires-Dist: python-dateutil
 Requires-Dist: pydantic>=2
 Requires-Dist: typing-extensions>=4.7.1
 
 # notehub-py
 The OpenAPI definition for the Notehub.io API.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 0.0.1
+- Package version: 0.0.2
 - Generator version: 7.5.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://dev.blues.io/support/](https://dev.blues.io/support/)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `notehub_py-0.0.1/notehub_py.egg-info/SOURCES.txt` & `notehub_py-0.0.2/notehub_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/pyproject.toml` & `notehub_py-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notehub_py"
-version = "0.0.1"
+version = "0.0.2"
 description = "Notehub API"
 authors = ["Blues Engineering <engineering@blues.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/blues/notehub-py"
 keywords = ["blues-io", "notehub-io", "api", "python", "Notehub API"]
 include = ["notehub_py/py.typed"]
```

### Comparing `notehub_py-0.0.1/setup.py` & `notehub_py-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "notehub-py"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
@@ -44,8 +44,19 @@
     keywords=["OpenAPI", "OpenAPI-Generator", "Notehub API"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     long_description_content_type='text/markdown',
     long_description=long_description,  # noqa: E501
     package_data={"notehub_py": ["py.typed"]},
+        classifiers=[
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Intended Audience :: Developers",
+        "Natural Language :: English",
+    ],
 )
```

### Comparing `notehub_py-0.0.1/test/test_authorization_api.py` & `notehub_py-0.0.2/test/test_authorization_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_aws.py` & `notehub_py-0.0.2/test/test_aws.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_azure.py` & `notehub_py-0.0.2/test/test_azure.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_billing_account.py` & `notehub_py-0.0.2/test/test_billing_account.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_billing_account_api.py` & `notehub_py-0.0.2/test/test_billing_account_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_billing_account_role.py` & `notehub_py-0.0.2/test/test_billing_account_role.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_body.py` & `notehub_py-0.0.2/test/test_body.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_clone_project_request.py` & `notehub_py-0.0.2/test/test_clone_project_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_contact.py` & `notehub_py-0.0.2/test/test_contact.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_create_fleet_request.py` & `notehub_py-0.0.2/test/test_create_fleet_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_create_monitor.py` & `notehub_py-0.0.2/test/test_create_monitor.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_create_product_request.py` & `notehub_py-0.0.2/test/test_create_product_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_create_project_request.py` & `notehub_py-0.0.2/test/test_create_project_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_delete_device_fleets_request.py` & `notehub_py-0.0.2/test/test_delete_device_fleets_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_device.py` & `notehub_py-0.0.2/test/test_device.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_device_api.py` & `notehub_py-0.0.2/test/test_device_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_device_session.py` & `notehub_py-0.0.2/test/test_device_session.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_device_tower_info.py` & `notehub_py-0.0.2/test/test_device_tower_info.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_device_usage.py` & `notehub_py-0.0.2/test/test_device_usage.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_dfu_env.py` & `notehub_py-0.0.2/test/test_dfu_env.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_dfu_state.py` & `notehub_py-0.0.2/test/test_dfu_state.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_environment_variables.py` & `notehub_py-0.0.2/test/test_environment_variables.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_error.py` & `notehub_py-0.0.2/test/test_error.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_event.py` & `notehub_py-0.0.2/test/test_event.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_event_api.py` & `notehub_py-0.0.2/test/test_event_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_firmware_api.py` & `notehub_py-0.0.2/test/test_firmware_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_firmware_info.py` & `notehub_py-0.0.2/test/test_firmware_info.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_fleet.py` & `notehub_py-0.0.2/test/test_fleet.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_billing_accounts200_response.py` & `notehub_py-0.0.2/test/test_get_billing_accounts200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_device_environment_variables200_response.py` & `notehub_py-0.0.2/test/test_get_device_environment_variables200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_device_health_log200_response.py` & `notehub_py-0.0.2/test/test_get_device_health_log200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_device_health_log200_response_health_log_inner.py` & `notehub_py-0.0.2/test/test_get_device_health_log200_response_health_log_inner.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_device_latest200_response.py` & `notehub_py-0.0.2/test/test_get_device_latest200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_device_public_key200_response.py` & `notehub_py-0.0.2/test/test_get_device_public_key200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_device_sessions200_response.py` & `notehub_py-0.0.2/test/test_get_device_sessions200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_project_device_public_keys200_response.py` & `notehub_py-0.0.2/test/test_get_project_device_public_keys200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_project_device_public_keys200_response_device_public_keys_inner.py` & `notehub_py-0.0.2/test/test_get_project_device_public_keys200_response_device_public_keys_inner.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_project_devices200_response.py` & `notehub_py-0.0.2/test/test_get_project_devices200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_project_events200_response.py` & `notehub_py-0.0.2/test/test_get_project_events200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_project_events_by_cursor200_response.py` & `notehub_py-0.0.2/test/test_get_project_events_by_cursor200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_project_fleets200_response.py` & `notehub_py-0.0.2/test/test_get_project_fleets200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_project_members200_response.py` & `notehub_py-0.0.2/test/test_get_project_members200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_project_products200_response.py` & `notehub_py-0.0.2/test/test_get_project_products200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_projects200_response.py` & `notehub_py-0.0.2/test/test_get_projects200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_get_route_logs_by_route200_response_inner.py` & `notehub_py-0.0.2/test/test_get_route_logs_by_route200_response_inner.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_google.py` & `notehub_py-0.0.2/test/test_google.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_handle_note_changes200_response.py` & `notehub_py-0.0.2/test/test_handle_note_changes200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_handle_note_get200_response.py` & `notehub_py-0.0.2/test/test_handle_note_get200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_handle_note_signal200_response.py` & `notehub_py-0.0.2/test/test_handle_note_signal200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_handle_notefile_changes200_response.py` & `notehub_py-0.0.2/test/test_handle_notefile_changes200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_handle_notefile_changes_pending200_response.py` & `notehub_py-0.0.2/test/test_handle_notefile_changes_pending200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_handle_notefile_delete_request.py` & `notehub_py-0.0.2/test/test_handle_notefile_delete_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_http.py` & `notehub_py-0.0.2/test/test_http.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_http_filter.py` & `notehub_py-0.0.2/test/test_http_filter.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_http_transform.py` & `notehub_py-0.0.2/test/test_http_transform.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_location.py` & `notehub_py-0.0.2/test/test_location.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_login200_response.py` & `notehub_py-0.0.2/test/test_login200_response.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_login_request.py` & `notehub_py-0.0.2/test/test_login_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_monitor.py` & `notehub_py-0.0.2/test/test_monitor.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_monitor_alert_routes_inner.py` & `notehub_py-0.0.2/test/test_monitor_alert_routes_inner.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_monitor_api.py` & `notehub_py-0.0.2/test/test_monitor_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_monitor_thresholds.py` & `notehub_py-0.0.2/test/test_monitor_thresholds.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_mqtt.py` & `notehub_py-0.0.2/test/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_note.py` & `notehub_py-0.0.2/test/test_note.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_post_provision_project_device_request.py` & `notehub_py-0.0.2/test/test_post_provision_project_device_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_product.py` & `notehub_py-0.0.2/test/test_product.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_project.py` & `notehub_py-0.0.2/test/test_project.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_project_api.py` & `notehub_py-0.0.2/test/test_project_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_project_member.py` & `notehub_py-0.0.2/test/test_project_member.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_proxy.py` & `notehub_py-0.0.2/test/test_proxy.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_put_device_fleets_request.py` & `notehub_py-0.0.2/test/test_put_device_fleets_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_radresponder.py` & `notehub_py-0.0.2/test/test_radresponder.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_role.py` & `notehub_py-0.0.2/test/test_role.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_route.py` & `notehub_py-0.0.2/test/test_route.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_route_api.py` & `notehub_py-0.0.2/test/test_route_api.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_route_schema.py` & `notehub_py-0.0.2/test/test_route_schema.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_slack.py` & `notehub_py-0.0.2/test/test_slack.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_snowflake.py` & `notehub_py-0.0.2/test/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_snowflake_transform.py` & `notehub_py-0.0.2/test/test_snowflake_transform.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_thingworx.py` & `notehub_py-0.0.2/test/test_thingworx.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_tower_location.py` & `notehub_py-0.0.2/test/test_tower_location.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_twilio.py` & `notehub_py-0.0.2/test/test_twilio.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_update_fleet_request.py` & `notehub_py-0.0.2/test/test_update_fleet_request.py`

 * *Files identical despite different names*

### Comparing `notehub_py-0.0.1/test/test_user_db_route.py` & `notehub_py-0.0.2/test/test_user_db_route.py`

 * *Files identical despite different names*
