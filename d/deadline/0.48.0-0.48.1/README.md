# Comparing `tmp/deadline-0.48.0.tar.gz` & `tmp/deadline-0.48.1.tar.gz`

## Comparing `deadline-0.48.0.tar` & `deadline-0.48.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0    50578 2020-02-02 00:00:00.000000 deadline-0.48.0/THIRD_PARTY_LICENSES
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.0/_version.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/__main__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/_version.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/exceptions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/py.typed
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/__init__.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_get_storage_profile_for_queue.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_list_apis.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_loginout.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_queue_parameters.py
--rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_session.py
--rw-r--r--   0        0        0    18628 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_submit_job_bundle.py
--rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/api/_telemetry.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/__init__.py
--rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_common.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_deadline_cli.py
--rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_deadline_web_url.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/deadline_cli_main.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/deadline_dev_gui_main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/_sigint_handler.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/auth_group.py
--rw-r--r--   0        0        0    12134 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/bundle_group.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/config_group.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/farm_group.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/fleet_group.py
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/handle_web_url_command.py
--rw-r--r--   0        0        0    39347 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/job_group.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/queue_group.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/cli/_groups/worker_group.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/config/__init__.py
--rw-r--r--   0        0        0    17510 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/config/config_file.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/__init__.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/_yaml.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/adaptors.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/job_template.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/loader.py
--rw-r--r--   0        0        0    32688 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/parameters.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/job_bundle/submission.py
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/__init__.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/cli_job_submitter.py
--rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/deadline_authentication_status.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dev_application.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/job_bundle_submitter.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dataclasses/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dialogs/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dialogs/_types.py
--rw-r--r--   0        0        0    34196 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dialogs/deadline_config_dialog.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dialogs/deadline_login_dialog.py
--rw-r--r--   0        0        0    29733 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py
--rw-r--r--   0        0        0    20978 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/resources/deadline_logo.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/resources/info.svg
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/resources/blender_example_bundle/template.yaml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/resources/cli_job_bundle/template.yaml
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/__init__.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/cli_job_settings_tab.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py
--rw-r--r--   0        0        0    36343 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/host_requirements_tab.py
--rw-r--r--   0        0        0    15622 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/job_attachments_tab.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/job_bundle_settings_tab.py
--rw-r--r--   0        0        0    31193 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/openjd_parameters_widget.py
--rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/path_widgets.py
--rw-r--r--   0        0        0    23261 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/shared_job_settings_tab.py
--rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/client/ui/widgets/spinbox_widgets.py
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/README.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/__init__.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_utils.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_version.py
--rw-r--r--   0        0        0    28207 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_sync.py
--rw-r--r--   0        0        0    46754 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/download.py
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/exceptions.py
--rw-r--r--   0        0        0    10785 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/models.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/os_file_permission.py
--rw-r--r--   0        0        0    15063 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/progress_tracker.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/py.typed
--rw-r--r--   0        0        0    52996 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/upload.py
--rw-r--r--   0        0        0    21984 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/vfs.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_aws/__init__.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_aws/aws_clients.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_aws/aws_config.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_aws/deadline.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_windows/__init__.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/_windows/file.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/__init__.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/_canonical_json.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/base_manifest.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/decode.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/hash_algorithms.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/manifest_model.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/versions.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/v2023_03_03/__init__.py
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/caches/__init__.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/caches/cache_db.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/caches/hash_cache.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 deadline-0.48.0/src/deadline/job_attachments/caches/s3_check_cache.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 deadline-0.48.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline-0.48.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline-0.48.0/NOTICE
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 deadline-0.48.0/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 deadline-0.48.0/hatch.toml
--rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 deadline-0.48.0/pyproject.toml
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 deadline-0.48.0/PKG-INFO
+-rw-r--r--   0        0        0    50578 2020-02-02 00:00:00.000000 deadline-0.48.1/THIRD_PARTY_LICENSES
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.1/_version.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/__main__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/_version.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/exceptions.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/py.typed
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/__init__.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_get_storage_profile_for_queue.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_list_apis.py
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_loginout.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_queue_parameters.py
+-rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_session.py
+-rw-r--r--   0        0        0    18628 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_submit_job_bundle.py
+-rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_telemetry.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/__init__.py
+-rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_common.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_deadline_cli.py
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_deadline_web_url.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/deadline_cli_main.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/deadline_dev_gui_main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/_sigint_handler.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/auth_group.py
+-rw-r--r--   0        0        0    12134 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/bundle_group.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/config_group.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/farm_group.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/fleet_group.py
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/handle_web_url_command.py
+-rw-r--r--   0        0        0    39347 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/job_group.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/queue_group.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/worker_group.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/config/__init__.py
+-rw-r--r--   0        0        0    17510 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/config/config_file.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/__init__.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/_yaml.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/adaptors.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/job_template.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/loader.py
+-rw-r--r--   0        0        0    32688 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/parameters.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/submission.py
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/__init__.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/cli_job_submitter.py
+-rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/deadline_authentication_status.py
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dev_application.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/job_bundle_submitter.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dataclasses/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dialogs/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dialogs/_types.py
+-rw-r--r--   0        0        0    34230 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dialogs/deadline_config_dialog.py
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dialogs/deadline_login_dialog.py
+-rw-r--r--   0        0        0    29733 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py
+-rw-r--r--   0        0        0    20978 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/resources/deadline_logo.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/resources/info.svg
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/resources/blender_example_bundle/template.yaml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/resources/cli_job_bundle/template.yaml
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/__init__.py
+-rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/cli_job_settings_tab.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py
+-rw-r--r--   0        0        0    36343 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/host_requirements_tab.py
+-rw-r--r--   0        0        0    15622 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/job_attachments_tab.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/job_bundle_settings_tab.py
+-rw-r--r--   0        0        0    31193 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/openjd_parameters_widget.py
+-rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/path_widgets.py
+-rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/shared_job_settings_tab.py
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/spinbox_widgets.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/README.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/__init__.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_utils.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_version.py
+-rw-r--r--   0        0        0    28207 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_sync.py
+-rw-r--r--   0        0        0    46754 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/download.py
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/exceptions.py
+-rw-r--r--   0        0        0    10785 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/models.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/os_file_permission.py
+-rw-r--r--   0        0        0    15063 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/progress_tracker.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/py.typed
+-rw-r--r--   0        0        0    52996 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/upload.py
+-rw-r--r--   0        0        0    21984 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/vfs.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_aws/__init__.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_aws/aws_clients.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_aws/aws_config.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_aws/deadline.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_windows/__init__.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_windows/file.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/__init__.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/_canonical_json.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/base_manifest.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/decode.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/hash_algorithms.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/manifest_model.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/versions.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/v2023_03_03/__init__.py
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/caches/__init__.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/caches/cache_db.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/caches/hash_cache.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/caches/s3_check_cache.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 deadline-0.48.1/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline-0.48.1/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline-0.48.1/NOTICE
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 deadline-0.48.1/README.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 deadline-0.48.1/hatch.toml
+-rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 deadline-0.48.1/pyproject.toml
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 deadline-0.48.1/PKG-INFO
```

### Comparing `deadline-0.48.0/THIRD_PARTY_LICENSES` & `deadline-0.48.1/THIRD_PARTY_LICENSES`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/exceptions.py` & `deadline-0.48.1/src/deadline/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/api/__init__.py` & `deadline-0.48.1/src/deadline/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/api/_get_storage_profile_for_queue.py` & `deadline-0.48.1/src/deadline/client/api/_get_storage_profile_for_queue.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/api/_list_apis.py` & `deadline-0.48.1/src/deadline/client/api/_list_apis.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/api/_loginout.py` & `deadline-0.48.1/src/deadline/client/api/_loginout.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 
 
 def _login_deadline_cloud_monitor(
     on_pending_authorization: Optional[Callable],
     on_cancellation_check: Optional[Callable],
     config: Optional[ConfigParser] = None,
 ):
-    # Deadline Cloud Monitor writes the absolute path to itself to the config file
+    # Deadline Cloud monitor writes the absolute path to itself to the config file
     deadline_cloud_monitor_path = get_setting("deadline-cloud-monitor.path", config=config)
     profile_name = get_setting("defaults.aws_profile_name", config=config)
     args = [deadline_cloud_monitor_path, "login", "--profile", profile_name]
 
-    # Open Deadline Cloud Monitor, non-blocking the user will keep Deadline Cloud Monitor running in the background.
+    # Open Deadline Cloud monitor, non-blocking the user will keep Deadline Cloud monitor running in the background.
     try:
         if sys.platform.startswith("win"):
             # We don't hookup to stdin but do this to avoid issues on windows
             # See https://docs.python.org/3/library/subprocess.html#subprocess.STARTUPINFO.lpAttributeList
             p = subprocess.Popen(
                 args, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, stdin=subprocess.PIPE
             )
@@ -54,98 +54,101 @@
             )
         # Linux takes time to start DCM binary, which causes the TTY to suspend the process and send it to background job
         # With wait here, the DCM binary starts and TTY does not suspend the deadline process.
         if sys.platform == "linux":
             time.sleep(0.5)
     except FileNotFoundError:
         raise DeadlineOperationError(
-            f"Could not find Deadline Cloud Monitor at {deadline_cloud_monitor_path}. Please ensure Deadline Cloud Monitor is installed correctly and setup the {profile_name} profile again."
+            f"Could not find Deadline Cloud monitor at {deadline_cloud_monitor_path}. "
+            f"Please ensure Deadline Cloud monitor is installed correctly and set up the {profile_name} profile again."
         )
     if on_pending_authorization:
         on_pending_authorization(
             credentials_source=AwsCredentialsSource.DEADLINE_CLOUD_MONITOR_LOGIN
         )
     # And wait for the user to complete login
     while True:
-        # Deadline Cloud Monitor is a GUI app that will keep on running
+        # Deadline Cloud monitor is a GUI app that will keep on running
         # So we sit here and test that profile for validity until it works
         if check_authentication_status(config) == AwsAuthenticationStatus.AUTHENTICATED:
-            return f"Deadline Cloud Monitor Profile: {profile_name}"
+            return f"Deadline Cloud monitor profile: {profile_name}"
         if on_cancellation_check:
             # Check if the UI has signaled a cancel
             if on_cancellation_check():
                 p.kill()
                 raise Exception()
         if p.poll():
-            # Deadline Cloud Monitor has stopped, we assume it returned us an error on one line on stderr
-            # but let's be specific about Deadline Cloud Monitor failing incase the error is non-obvious
+            # Deadline Cloud monitor has stopped, we assume it returned us an error on one line on stderr
+            # but let's be specific about Deadline Cloud monitor failing incase the error is non-obvious
             # and let's tack on stdout incase it helps
             err_prefix = (
-                f"Deadline Cloud Monitor was not able to log into the {profile_name} profile: "
+                f"Deadline Cloud monitor was not able to log into the {profile_name} profile:"
             )
             out = p.stdout.read().decode("utf-8") if p.stdout else ""
-            raise DeadlineOperationError(f"{err_prefix}:\n{out}")
+            raise DeadlineOperationError(f"{err_prefix}\n{out}")
 
         time.sleep(0.5)
 
 
 def login(
     on_pending_authorization: Optional[Callable],
     on_cancellation_check: Optional[Callable],
     config: Optional[ConfigParser] = None,
 ) -> str:
     """
-    For AWS profiles created by Deadline Cloud Monitor, logs in to provide access to Deadline Cloud.
+    For AWS profiles created by Deadline Cloud monitor, logs in to provide access to Deadline Cloud.
 
     Args:
         on_pending_authorization (Callable): A callback that receives method-specific information to continue login.
             All methods: 'credentials_source' parameter of type AwsCredentialsSource
-            For Deadline Cloud Monitor: No additional parameters
+            For Deadline Cloud monitor: No additional parameters
         on_cancellation_check (Callable): A callback that allows the operation to cancel before login completes
         config (ConfigParser, optional): The AWS Deadline Cloud configuration
                 object to use instead of the config file.
     """
     credentials_source = get_credentials_source(config)
     if credentials_source == AwsCredentialsSource.DEADLINE_CLOUD_MONITOR_LOGIN:
         return _login_deadline_cloud_monitor(
             on_pending_authorization, on_cancellation_check, config
         )
     raise UnsupportedProfileTypeForLoginLogout(
-        "Logging in is only supported for AWS Profiles created by Deadline Cloud Monitor."
+        "Logging in is only supported for AWS Profiles created by Deadline Cloud monitor."
     )
 
 
 def logout(config: Optional[ConfigParser] = None) -> str:
     """
-    For AWS profiles created by Deadline Cloud Monitor, logs out of Deadline Cloud.
+    For AWS profiles created by Deadline Cloud monitor, logs out of Deadline Cloud.
 
      Args:
         config (ConfigParser, optional): The AWS Deadline Cloud configuration
                 object to use instead of the config file.
     """
     credentials_source = get_credentials_source(config)
     if credentials_source == AwsCredentialsSource.DEADLINE_CLOUD_MONITOR_LOGIN:
-        # Deadline Cloud Monitor writes the absolute path to itself to the config file
+        # Deadline Cloud monitor writes the absolute path to itself to the config file
         deadline_cloud_monitor_path = get_setting("deadline-cloud-monitor.path", config=config)
         profile_name = get_setting("defaults.aws_profile_name", config=config)
         args = [deadline_cloud_monitor_path, "logout", "--profile", profile_name]
 
-        # Open Deadline Cloud Monitor, blocking
-        # Unlike login, that opens the regular Deadline Cloud Monitor GUI, logout is a CLI command that clears the profile
+        # Open Deadline Cloud monitor, blocking
+        # Unlike login, that opens the regular Deadline Cloud monitor GUI, logout is a CLI command that clears the profile
         # This makes it easier as we can execute and look at the return cdoe
         try:
             output = subprocess.check_output(args)
         except FileNotFoundError:
             raise DeadlineOperationError(
-                f"Could not find Deadline Cloud Monitor at {deadline_cloud_monitor_path}. Please ensure Deadline Cloud Monitor is installed correctly and setup the {profile_name} profile again."
+                f"Could not find Deadline Cloud monitor at {deadline_cloud_monitor_path}. "
+                f"Please ensure Deadline Cloud monitor is installed correctly and set up the {profile_name} profile again."
             )
         except subprocess.CalledProcessError as e:
             raise DeadlineOperationError(
-                f"Deadline Cloud Monitor was unable to logout the profile {profile_name}. Return code {e.returncode}: {e.output}"
+                f"Deadline Cloud monitor was unable to log out the profile {profile_name}."
+                f"Return code {e.returncode}: {e.output}"
             )
 
         # Force a refresh of the cached boto3 Session
         invalidate_boto3_session_cache()
         return output.decode("utf8")
     raise UnsupportedProfileTypeForLoginLogout(
-        "Logging out is only supported for AWS Profiles created by Deadline Cloud Monitor."
+        "Logging out is only supported for AWS Profiles created by Deadline Cloud monitor."
     )
```

### Comparing `deadline-0.48.0/src/deadline/client/api/_queue_parameters.py` & `deadline-0.48.1/src/deadline/client/api/_queue_parameters.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/api/_session.py` & `deadline-0.48.1/src/deadline/client/api/_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,37 +111,37 @@
     """
     session = get_boto3_session(config=config)
     return session.client(service_name)
 
 
 def get_credentials_source(config: Optional[ConfigParser] = None) -> AwsCredentialsSource:
     """
-    Returns DEADLINE_CLOUD_MONITOR_LOGIN if Deadline Cloud Monitor wrote the credentials, HOST_PROVIDED otherwise.
+    Returns DEADLINE_CLOUD_MONITOR_LOGIN if Deadline Cloud monitor wrote the credentials, HOST_PROVIDED otherwise.
 
     Args:
         config (ConfigParser, optional): The AWS Deadline Cloud configuration
                 object to use instead of the config file.
     """
     try:
         session = get_boto3_session(config=config)
         profile_config = session._session.get_scoped_config()
     except ProfileNotFound:
         return AwsCredentialsSource.NOT_VALID
     if "monitor_id" in profile_config:
-        # Deadline Cloud Monitor Desktop adds the "monitor_id" key
+        # Deadline Cloud monitor Desktop adds the "monitor_id" key
         return AwsCredentialsSource.DEADLINE_CLOUD_MONITOR_LOGIN
     else:
         return AwsCredentialsSource.HOST_PROVIDED
 
 
 def get_user_and_identity_store_id(
     config: Optional[ConfigParser] = None,
 ) -> tuple[Optional[str], Optional[str]]:
     """
-    If logged in with Deadline Cloud Monitor Desktop, returns a tuple
+    If logged in with Deadline Cloud monitor Desktop, returns a tuple
     (user_id, identity_store_id), otherwise returns None.
     """
     session = get_boto3_session(config=config)
     profile_config = session._session.get_scoped_config()
 
     if "monitor_id" in profile_config:
         return (profile_config["user_id"], profile_config["identity_store_id"])
@@ -261,23 +261,23 @@
     Args:
         config (ConfigParser, optional): The AWS Deadline Cloud configuration
                 object to use instead of the config file.
 
     Returns AwsAuthenticationStatus enum value:
       - CONFIGURATION_ERROR if there is an unexpected error accessing credentials
       - AUTHENTICATED if they are fine
-      - NEEDS_LOGIN if a Deadline Cloud Monitor login is required.
+      - NEEDS_LOGIN if a Deadline Cloud monitor login is required.
     """
 
     with _modified_logging_level(logging.getLogger("botocore.credentials"), logging.ERROR):
         try:
             get_boto3_session(config=config).client("sts").get_caller_identity()
             return AwsAuthenticationStatus.AUTHENTICATED
         except Exception:
-            # We assume that the presence of a Deadline Cloud Monitor profile
+            # We assume that the presence of a Deadline Cloud monitor profile
             # means we will know everything necessary to start it and login.
 
             if get_credentials_source(config) == AwsCredentialsSource.DEADLINE_CLOUD_MONITOR_LOGIN:
                 return AwsAuthenticationStatus.NEEDS_LOGIN
             return AwsAuthenticationStatus.CONFIGURATION_ERROR
```

### Comparing `deadline-0.48.0/src/deadline/client/api/_submit_job_bundle.py` & `deadline-0.48.1/src/deadline/client/api/_submit_job_bundle.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/api/_telemetry.py` & `deadline-0.48.1/src/deadline/client/api/_telemetry.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/cli/_common.py` & `deadline-0.48.1/src/deadline/client/cli/_common.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/cli/_deadline_cli.py` & `deadline-0.48.1/src/deadline/client/cli/_deadline_cli.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/cli/_deadline_web_url.py` & `deadline-0.48.1/src/deadline/client/cli/_deadline_web_url.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/cli/deadline_dev_gui_main.py` & `deadline-0.48.1/src/deadline/client/cli/deadline_dev_gui_main.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/cli/_groups/_sigint_handler.py` & `deadline-0.48.1/src/deadline/client/cli/_groups/_sigint_handler.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/cli/_groups/auth_group.py` & `deadline-0.48.1/src/deadline/client/cli/_groups/auth_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 JSON_FIELD_AUTH_STATUS = "status"
 JSON_FIELD_CREDS_SOURCE = "source"
 JSON_FIELD_AUTH_API_AVAILABLE = "api_availability"
 
 
 def _cli_on_pending_authorization(**kwargs):
     """
-    Callback for `login`, to tell the user that Deadline Cloud Monitor is opening
+    Callback for `login`, to tell the user that Deadline Cloud monitor is opening
     """
 
     if kwargs["credentials_source"] == AwsCredentialsSource.DEADLINE_CLOUD_MONITOR_LOGIN:
-        click.echo("Opening Deadline Cloud Monitor. Please login and then return here.")
+        click.echo("Opening Deadline Cloud monitor. Please log in and then return here.")
 
 
 @click.group(name="auth")
 @_handle_error
 def cli_auth():
     """
     Commands to handle AWS Deadline Cloud authentication.
@@ -41,15 +41,15 @@
 @cli_auth.command(name="login")
 @_handle_error
 def auth_login():
     """
     Logs in to the AWS Deadline Cloud configured AWS profile.
 
     This is for any profile type that AWS Deadline Cloud knows how to login to
-    Currently only supports Deadline Cloud Monitor
+    Currently only supports Deadline Cloud monitor
     """
     click.echo(
         f"Logging into AWS Profile {config_file.get_setting('defaults.aws_profile_name')!r} for AWS Deadline Cloud"
     )
 
     message = api.login(
         on_pending_authorization=_cli_on_pending_authorization, on_cancellation_check=None
@@ -58,19 +58,19 @@
     click.echo(f"\nSuccessfully logged in: {message}\n")
 
 
 @cli_auth.command(name="logout")
 @_handle_error
 def auth_logout():
     """
-    Logs out of the Deadline Cloud Monitor configured AWS profile.
+    Logs out of the Deadline Cloud monitor configured AWS profile.
     """
     api.logout()
 
-    click.echo("Successfully logged out of all Deadline Cloud Monitor AWS profiles")
+    click.echo("Successfully logged out of all Deadline Cloud monitor AWS profiles")
 
 
 @cli_auth.command(name="status")
 @click.option("--profile", help="The AWS profile to use.")
 @click.option(
     "--output",
     type=click.Choice(
```

### Comparing `deadline-0.48.0/src/deadline/client/cli/_groups/bundle_group.py` & `deadline-0.48.1/src/deadline/client/cli/_groups/bundle_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/cli/_groups/config_group.py` & `deadline-0.48.1/src/deadline/client/cli/_groups/config_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/cli/_groups/farm_group.py` & `deadline-0.48.1/src/deadline/client/cli/_groups/farm_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/cli/_groups/fleet_group.py` & `deadline-0.48.1/src/deadline/client/cli/_groups/fleet_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/cli/_groups/handle_web_url_command.py` & `deadline-0.48.1/src/deadline/client/cli/_groups/handle_web_url_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
             farm_id = url_queries.pop("farm_id")
             queue_id = url_queries.pop("queue_id")
             job_id = url_queries.pop("job_id")
             step_id = url_queries.pop("step_id", None)
             task_id = url_queries.pop("task_id", None)
 
-            # Add the standard option "profile", using the one provided by the url (set by Deadline Cloud Monitor)
+            # Add the standard option "profile", using the one provided by the url (set by Deadline Cloud monitor)
             # or choosing a best guess based on farm and queue IDs
             aws_profile_name = url_queries.pop(
                 "profile",
                 config_file.get_best_profile_for_farm(farm_id, queue_id),
             )
 
             # Read the config, and switch the in-memory version to use the chosen AWS profile
```

### Comparing `deadline-0.48.0/src/deadline/client/cli/_groups/job_group.py` & `deadline-0.48.1/src/deadline/client/cli/_groups/job_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/cli/_groups/queue_group.py` & `deadline-0.48.1/src/deadline/client/cli/_groups/queue_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/cli/_groups/worker_group.py` & `deadline-0.48.1/src/deadline/client/cli/_groups/worker_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/config/__init__.py` & `deadline-0.48.1/src/deadline/client/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/config/config_file.py` & `deadline-0.48.1/src/deadline/client/config/config_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 # "depend"  - The setting it depends on, if any. This modifies the section name of the
 #             setting to embed the dependency value, e.g. default.farm_id goes in
 #             section [profile-{profileName} default]
 # "section_format" - How its value gets formatted into config file sections.
 SETTINGS: Dict[str, Dict[str, Any]] = {
     "deadline-cloud-monitor.path": {
         "default": "",
-        "description": "The filesystem path to Deadline Cloud Monitor, set during login process.",
+        "description": "The filesystem path to Deadline Cloud monitor, set during login process.",
     },
     "defaults.aws_profile_name": {
         "default": "(default)",
         "section_format": "profile-{}",
         "description": "The AWS profile name to use by default. Set to '' to use the default credentials."
         + " Other settings are saved with the profile.",
     },
```

### Comparing `deadline-0.48.0/src/deadline/client/job_bundle/__init__.py` & `deadline-0.48.1/src/deadline/client/job_bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/job_bundle/_yaml.py` & `deadline-0.48.1/src/deadline/client/job_bundle/_yaml.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/job_bundle/adaptors.py` & `deadline-0.48.1/src/deadline/client/job_bundle/adaptors.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/job_bundle/job_template.py` & `deadline-0.48.1/src/deadline/client/job_bundle/job_template.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/job_bundle/loader.py` & `deadline-0.48.1/src/deadline/client/job_bundle/loader.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/job_bundle/parameters.py` & `deadline-0.48.1/src/deadline/client/job_bundle/parameters.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/job_bundle/submission.py` & `deadline-0.48.1/src/deadline/client/job_bundle/submission.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/ui/__init__.py` & `deadline-0.48.1/src/deadline/client/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/ui/cli_job_submitter.py` & `deadline-0.48.1/src/deadline/client/ui/cli_job_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/ui/deadline_authentication_status.py` & `deadline-0.48.1/src/deadline/client/ui/deadline_authentication_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
    api_availability_changed: triggered when api availability changes
 
 The status includes three parts:
   1. Are credentials configured and available for use?
      This is checked with an sts:GetCallerIdentity AWS API call.
   2. Do the credentials grant access to AWS Deadline Cloud APIs?
      This is checked with a simplified deadline:ListFarms AWS API call.
-  3. Do the credentials use Deadline Cloud Monitor?
+  3. Do the credentials use Deadline Cloud monitor?
      This is checked by looking for the relevant properties
      in the AWS profile configuration.
 """
 import os
 import threading
 from configparser import ConfigParser
 from logging import getLogger
@@ -75,21 +75,19 @@
         self.__auth_status: Optional[api.AwsAuthenticationStatus] = None
         self.__api_availability: Optional[bool] = None
 
         # Load the default config
         self.config = ConfigParser()
         self.config.read_dict(config_file.read_config())
 
-        # Watch the ~/.aws path for any changes to config or credentials,
-        # the ~/.aws/sso/cache to capture "aws sso login/logout", and
+        # Watch the ~/.aws path for any changes to config or credentials, and
         # the ~/.deadline path for any changes to the AWS Deadline Cloud config.
         self.aws_creds_file_watcher = QFileSystemWatcher()
         self.aws_creds_paths = [
             os.path.expanduser(os.path.join("~", ".aws")),
-            os.path.expanduser(os.path.join("~", ".aws", "sso", "cache")),
         ]
         self.deadline_config_paths = [
             os.path.expanduser(os.path.join("~", ".deadline")),
         ]
         failed_paths = self.aws_creds_file_watcher.addPaths(
             self.aws_creds_paths + self.deadline_config_paths
         )
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/dev_application.py` & `deadline-0.48.1/src/deadline/client/ui/dev_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,32 +38,32 @@
         self.setCentralWidget(None)  # type: ignore[arg-type]
 
         self.setDockOptions(
             QMainWindow.AllowNestedDocks | QMainWindow.AllowTabbedDocks | QMainWindow.AnimatedDocks
         )
 
     def setup_ui(self):
-        submit = self.menuBar().addMenu("&Submit Job")
-        submit.addAction("Submit Job Bundle...", self.submit_job_bundle)
-        submit.addAction("Submit CLI Job...", self.submit_cli_job)
+        submit = self.menuBar().addMenu("&Submit job")
+        submit.addAction("Submit job bundle...", self.submit_job_bundle)
+        submit.addAction("Submit CLI job...", self.submit_cli_job)
         account = self.menuBar().addMenu("&Account")
-        account.addAction("AWS Deadline Cloud Workstation Configuration...", self.configure)
+        account.addAction("AWS Deadline Cloud workstation configuration...", self.configure)
         account.addAction("Log in to AWS Deadline Cloud...", self.login)
         account.addAction("Log out of AWS Deadline Cloud...", self.logout)
 
         # Set up status bar
         # self.statusBar().setStyleSheet("QStatusBar::item{ border: none; }")
         self.statusBar().showMessage("Testing!")
 
     def submit_job_bundle(self):
         input_job_bundle_dir = os.path.normpath(
             os.path.join(__file__, "../resources/cli_job_bundle")
         )
         input_job_bundle_dir = QFileDialog.getExistingDirectory(
-            self, "Choose Job Bundle Directory", input_job_bundle_dir
+            self, "Choose job bundle directory", input_job_bundle_dir
         )
         if input_job_bundle_dir:
             show_job_bundle_submitter(
                 input_job_bundle_dir=os.path.normpath(input_job_bundle_dir),
                 browse=True,
                 parent=self,
                 f=Qt.Tool,
@@ -75,15 +75,15 @@
     def configure(self):
         DeadlineConfigDialog.configure_settings(parent=self)
 
     def login(self):
         if DeadlineLoginDialog.login(parent=self):
             logger.info("Logged in successfully")
         else:
-            logger.info("Failed to login")
+            logger.info("Failed to log in")
 
     def logout(self):
         api.logout()
 
     def signal_handler(self, signal, frame):
         self.close()
 
@@ -91,15 +91,15 @@
 def app() -> None:
     app = QApplication(sys.argv)
 
     # Set the style.
     app.setStyle(QStyleFactory.create("fusion"))
 
     # Set the application info.
-    app.setApplicationName("AWS Deadline Cloud Client Test GUI")
+    app.setApplicationName("AWS Deadline Cloud client test GUI")
     app.setOrganizationName("AWS")
     app.setOrganizationDomain("https://aws.amazon.com/")
     icon = QIcon(str(Path(__file__).parent / "resources" / "deadline_logo.svg"))
     app.setWindowIcon(icon)
 
     # Apply the stylesheet.
     pal = QPalette(QColor(64, 64, 64))
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/job_bundle_submitter.py` & `deadline-0.48.1/src/deadline/client/ui/job_bundle_submitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             widget for widget in app.topLevelWidgets() if isinstance(widget, QMainWindow)  # type: ignore[union-attr]
         ]
         if main_windows:
             parent = main_windows[0]
 
     if not input_job_bundle_dir:
         input_job_bundle_dir = QFileDialog.getExistingDirectory(
-            parent, "Choose Job Bundle Directory", input_job_bundle_dir
+            parent, "Choose job bundle directory", input_job_bundle_dir
         )
         if not input_job_bundle_dir:
             return None
 
     def on_create_job_bundle_callback(
         widget: SubmitJobToDeadlineDialog,
         job_bundle_dir: str,
@@ -147,15 +147,15 @@
     template = read_yaml_or_json_object(input_job_bundle_dir, "template", True)
 
     asset_references_obj = (
         read_yaml_or_json_object(input_job_bundle_dir, "asset_references", False) or {}
     )
     asset_references = AssetReferences.from_dict(asset_references_obj)
 
-    name = "Job Bundle Submission"
+    name = "Job bundle submission"
     if template:
         name = template.get("name", name)
 
     if not os.path.isdir(input_job_bundle_dir):
         raise DeadlineOperationError(f"Input Job Bundle Dir is not valid: {input_job_bundle_dir}")
     initial_settings = JobBundleSettings(input_job_bundle_dir=input_job_bundle_dir, name=name)
     initial_settings.parameters = read_job_bundle_parameters(input_job_bundle_dir)
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/dataclasses/__init__.py` & `deadline-0.48.1/src/deadline/client/ui/dataclasses/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Settings for the Job Bundle submitter dialog.
     """
 
     # Used in UI elements and when creating the job bundle directory
     submitter_name: str = field(default="JobBundle")
 
     # Shared settings
-    name: str = field(default="Job Bundle")
+    name: str = field(default="Job bundle")
     description: str = field(default="")
 
     # Job Bundle settings
     input_job_bundle_dir: str = field(default="")
     parameters: list[JobParameter] = field(default_factory=list)
 
     # Whether to allow ability to "Load a different job bundle"
@@ -38,15 +38,15 @@
     Settings for a CLI Job.
     """
 
     # Used in UI elements and when creating the job bundle directory
     submitter_name: str = field(default="CLI")
 
     # Shared settings
-    name: str = field(default="CLI Job")
+    name: str = field(default="CLI job")
     description: str = field(default="")
 
     # CLI job settings
     bash_script_contents: str = field(
         default="""#!/usr/bin/env bash
 echo "Data Dir is {{Param.DataDir}}"
 cd "{{Param.DataDir}}"
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/dialogs/deadline_config_dialog.py` & `deadline-0.48.1/src/deadline/client/ui/dialogs/deadline_config_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         return deadline_config.changes_were_applied
 
     def __init__(self, parent=None) -> None:
         super().__init__(
             parent=parent, f=Qt.WindowSystemMenuHint | Qt.WindowTitleHint | Qt.WindowCloseButtonHint
         )
 
-        self.setWindowTitle("AWS Deadline Cloud Workstation Configuration")
+        self.setWindowTitle("AWS Deadline Cloud workstation configuration")
         self.deadline_authentication_status = DeadlineAuthenticationStatus.getInstance()
         self._build_ui()
 
     def _build_ui(self):
         self.layout = QVBoxLayout(self)
 
         self.config_box = DeadlineWorkstationConfigWidget(parent=self)
@@ -187,72 +187,74 @@
     def _build_ui(self):
         self.layout = QVBoxLayout(self)
 
         self.labels = {}
         self._refresh_callbacks: List[Callable] = []
 
         # Global settings
-        self.global_settings_group = QGroupBox(parent=self, title="Global Settings")
+        self.global_settings_group = QGroupBox(parent=self, title="Global settings")
         self.layout.addWidget(self.global_settings_group)
         global_settings_layout = QFormLayout(self.global_settings_group)
         self._build_global_settings_ui(self.global_settings_group, global_settings_layout)
 
         # AWS Profile-specific settings
-        self.profile_settings_group = QGroupBox(parent=self, title="Profile Settings")
+        self.profile_settings_group = QGroupBox(parent=self, title="Profile settings")
         self.layout.addWidget(self.profile_settings_group)
         profile_settings_layout = QFormLayout(self.profile_settings_group)
         self._build_profile_settings_ui(self.profile_settings_group, profile_settings_layout)
 
         # Farm-specific settings
-        self.farm_settings_group = QGroupBox(parent=self, title="Farm Settings")
+        self.farm_settings_group = QGroupBox(parent=self, title="Farm settings")
         self.layout.addWidget(self.farm_settings_group)
         farm_settings_layout = QFormLayout(self.farm_settings_group)
         self._build_farm_settings_ui(self.farm_settings_group, farm_settings_layout)
 
         # General settings
-        self.general_settings_group = QGroupBox(parent=self, title="General Settings")
+        self.general_settings_group = QGroupBox(parent=self, title="General settings")
         self.layout.addWidget(self.general_settings_group)
         general_settings_layout = QFormLayout(self.general_settings_group)
         self._build_general_settings_ui(self.general_settings_group, general_settings_layout)
 
         self._background_exception.connect(self.handle_background_exception)
 
     def _build_global_settings_ui(self, group, layout):
         self.aws_profiles_box = QComboBox(parent=group)
-        aws_profile_label = self.labels["defaults.aws_profile_name"] = QLabel("AWS Profile")
+        aws_profile_label = self.labels["defaults.aws_profile_name"] = QLabel("AWS profile")
         layout.addRow(aws_profile_label, self.aws_profiles_box)
         self.aws_profiles_box.currentTextChanged.connect(self.aws_profile_changed)
 
     def _build_profile_settings_ui(self, group, layout):
         self.job_history_dir_edit = DirectoryPickerWidget(
             initial_directory="",
-            directory_label="Job History Dir",
+            directory_label="Job history directory",
             parent=group,
             collapse_user_dir=True,
         )
-        job_history_dir_label = self.labels["settings.job_history_dir"] = QLabel("Job History Dir")
+        job_history_dir_label = self.labels["settings.job_history_dir"] = QLabel(
+            "Job history directory"
+        )
         layout.addRow(job_history_dir_label, self.job_history_dir_edit)
         self.job_history_dir_edit.path_changed.connect(self.job_history_dir_changed)
 
         self.default_farm_box = DeadlineFarmListComboBox(parent=group)
-        default_farm_box_label = self.labels["defaults.farm_id"] = QLabel("Default Farm")
+        default_farm_box_label = self.labels["defaults.farm_id"] = QLabel("Default farm")
         self.default_farm_box.box.currentIndexChanged.connect(self.default_farm_changed)
         self.default_farm_box.background_exception.connect(self.handle_background_exception)
         layout.addRow(default_farm_box_label, self.default_farm_box)
 
     def _build_farm_settings_ui(self, group, layout):
         self.default_queue_box = DeadlineQueueListComboBox(parent=group)
-        default_queue_box_label = self.labels["defaults.queue_id"] = QLabel("Default Queue")
+        default_queue_box_label = self.labels["defaults.queue_id"] = QLabel("Default queue")
         self.default_queue_box.box.currentIndexChanged.connect(self.default_queue_changed)
         self.default_queue_box.background_exception.connect(self.handle_background_exception)
         layout.addRow(default_queue_box_label, self.default_queue_box)
 
         self.default_storage_profile_box = DeadlineStorageProfileNameListComboBox(parent=group)
         default_storage_profile_box_label = self.labels["settings.storage_profile_id"] = QLabel(
-            "Default Storage Profile"
+            "Default storage profile"
         )
         self.default_storage_profile_box.box.currentIndexChanged.connect(
             self.default_storage_profile_name_changed
         )
         self.default_storage_profile_box.background_exception.connect(
             self.handle_background_exception
         )
@@ -269,42 +271,42 @@
             item_name_copied: "When selected, the worker downloads all job attachments to disk before rendering begins.",
             item_name_virtual: "When selected, the worker downloads attachments only when needed by each task.",
         }
         self.job_attachments_file_system_box = self._init_combobox_setting_with_tooltips(
             group=group,
             layout=layout,
             setting_name="defaults.job_attachments_file_system",
-            label_text="Job Attachments FileSystem Options",
+            label_text="Job attachments filesystem options",
             label_tooltip=job_attachments_file_system_tooltip,
             values_with_tooltips=values_with_tooltips,
         )
 
     def _build_general_settings_ui(self, group, layout):
         self.auto_accept = self._init_checkbox_setting(
-            group, layout, "settings.auto_accept", "Auto Accept Prompt Defaults"
+            group, layout, "settings.auto_accept", "Auto accept prompt defaults"
         )
         self.telemetry_opt_out = self._init_checkbox_setting(
-            group, layout, "telemetry.opt_out", "Telemetry Opt Out"
+            group, layout, "telemetry.opt_out", "Telemetry opt out"
         )
 
         self._conflict_resolution_options = [option.name for option in FileConflictResolution]
         self.conflict_resolution_box = self._init_combobox_setting(
             group,
             layout,
             "settings.conflict_resolution",
-            "Conflict Resolution Option",
+            "Conflict resolution option",
             self._conflict_resolution_options,
         )
 
         self._log_levels = ["ERROR", "WARNING", "INFO", "DEBUG"]
         self.log_level_box = self._init_combobox_setting(
             group,
             layout,
             "settings.log_level",
-            "Current Logging Level",
+            "Current logging level",
             self._log_levels,
         )
 
     def _init_checkbox_setting(
         self, group: QWidget, layout: QFormLayout, setting_name: str, label_text: str
     ) -> QCheckBox:
         """
@@ -550,15 +552,15 @@
             self.default_storage_profile_box.box.currentData()
         )
 
         for setting_name, value in self.changes.items():
             if value.startswith(NOT_VALID_MARKER):
                 QMessageBox.warning(
                     self,
-                    "Apply Changes",
+                    "Apply changes",
                     f"Cannot apply changes, {value} is not valid for setting {setting_name}",
                 )
                 return False
 
         self.config = config_file.read_config()
 
         for setting_name, value in self.changes.items():
@@ -691,15 +693,15 @@
         with block_signals(self.box):
             self.box.clear()
             self.box.addItem("<refreshing>", userData=selected_id)
 
         self.__refresh_id += 1
         self.__refresh_thread = threading.Thread(
             target=self._refresh_thread_function,
-            name=f"AWS Deadline Cloud Refresh {self.resource_name} Thread",
+            name=f"AWS Deadline Cloud refresh {self.resource_name} thread",
             args=(self.__refresh_id, config),
         )
         self.__refresh_thread.start()
 
     def handle_list_update(self, refresh_id, items_list):
         # Apply the refresh if it's still for the latest call
         if refresh_id == self.__refresh_id:
@@ -734,15 +736,15 @@
         """
         try:
             resources = self.list_resources(config=config)
             if not self.canceled:
                 self._list_update.emit(refresh_id, resources)
         except BaseException as e:
             if not self.canceled and refresh_id == self.__refresh_id:
-                self.background_exception.emit(f"Refresh {self.resource_name}s List", e)
+                self.background_exception.emit(f"Refresh {self.resource_name}s list", e)
 
 
 class DeadlineFarmListComboBox(_DeadlineResourceListComboBox):
     def __init__(self, parent=None):
         super().__init__(resource_name="Farm", setting_name="defaults.farm_id", parent=parent)
 
     def list_resources(self, config: Optional[ConfigParser]):
@@ -772,15 +774,15 @@
 class DeadlineStorageProfileNameListComboBox(_DeadlineResourceListComboBox):
     WINDOWS_OS = "windows"
     MAC_OS = "macos"
     LINUX_OS = "linux"
 
     def __init__(self, parent=None):
         super().__init__(
-            resource_name="Storage Profile",
+            resource_name="Storage profile",
             setting_name="settings.storage_profile_id",
             parent=parent,
         )
 
     def list_resources(self, config: Optional[ConfigParser]):
         default_farm_id = config_file.get_setting("defaults.farm_id", config=config)
         default_queue_id = config_file.get_setting("defaults.queue_id", config=config)
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/dialogs/deadline_login_dialog.py` & `deadline-0.48.1/src/deadline/client/ui/dialogs/deadline_login_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Provides a modal dialog box for logging in to AWS Deadline Cloud.
 
 Example code:
     from deadline.client.ui.dialogs import DeadlineLoginDialog
     if DeadlineLoginDialog.login(parent=self):
         print("Logged in successfully.")
     else:
-        print("Failed to login.")
+        print("Failed to log in.")
 """
 
 __all__ = ["DeadlineLoginDialog"]
 
 import html
 import threading
 from configparser import ConfigParser
@@ -33,15 +33,15 @@
     of the static DeadlineLoginDialog.login() and the modal exec()
     is True when the login is successful, False otherwise.
 
     Example code:
         if DeadlineLoginDialog.login(parent=self):
             print("Logged in successfully.")
         else:
-            print("Failed to login.")
+            print("Failed to log in.")
     """
 
     # This signal is sent when the background login thread raises an exception.
     login_thread_exception = Signal(BaseException)
     # This signal is sent when the background login thread wants to change the
     # displayed message.
     login_thread_message = Signal(str)
@@ -106,15 +106,15 @@
 
             def on_pending_authorization(**kwargs):
                 if (
                     kwargs["credentials_source"]
                     == AwsCredentialsSource.DEADLINE_CLOUD_MONITOR_LOGIN
                 ):
                     self.login_thread_message.emit(
-                        "Opening Deadline Cloud Monitor. Please login before returning here."
+                        "Opening Deadline Cloud monitor. Please log in before returning here."
                     )
 
             def on_cancellation_check():
                 return self.canceled
 
             success_message = api.login(
                 on_pending_authorization,
@@ -128,15 +128,15 @@
 
     def _start_login(self) -> None:
         """
         Starts the background login thread.
         """
 
         self.__login_thread = threading.Thread(
-            target=self._login_background_thread, name="AWS Deadline Cloud Login Thread"
+            target=self._login_background_thread, name="AWS Deadline Cloud login thread"
         )
         self.__login_thread.start()
 
     def handle_login_thread_exception(self, e: BaseException) -> None:
         """
         Handles the signal sent from the background login thread when
         an exception is thrown.
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py` & `deadline-0.48.1/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,33 +150,33 @@
         self.lyt = QVBoxLayout(self)
         self.lyt.setContentsMargins(5, 10, 5, 5)
         self.setMinimumWidth(450)
 
         self.status_label = QLabel("Preparing files...")
         self.status_label.setMargin(5)
         self.hashing_progress = JobAttachmentsProgressWidget(
-            initial_message="Preparing for hashing...", title="Hashing Progress", parent=self
+            initial_message="Preparing for hashing...", title="Hashing progress", parent=self
         )
         self.upload_progress = JobAttachmentsProgressWidget(
-            initial_message="Preparing for upload...", title="Upload Progress", parent=self
+            initial_message="Preparing for upload...", title="Upload progress", parent=self
         )
         self.summary_edit = QTextEdit()
         self.summary_edit.setVisible(False)
         self.summary_edit.setReadOnly(True)
         self.button_box = QDialogButtonBox(Qt.Horizontal)
         self.button_box.setStandardButtons(QDialogButtonBox.Cancel)
 
         self.lyt.setAlignment(Qt.AlignTop)
         self.lyt.addWidget(self.status_label)
         self.lyt.addWidget(self.hashing_progress)
         self.lyt.addWidget(self.upload_progress)
         self.lyt.addWidget(self.summary_edit)
         self.lyt.addWidget(self.button_box)
 
-        self.setWindowTitle("AWS Deadline Cloud Submission")
+        self.setWindowTitle("AWS Deadline Cloud submission")
 
         self.hashing_thread_progress_report.connect(self.handle_hashing_thread_progress_report)
         self.hashing_thread_succeeded.connect(self.handle_hashing_thread_succeeded)
         self.hashing_thread_exception.connect(self.handle_thread_exception)
 
         self.upload_thread_progress_report.connect(self.handle_upload_thread_progress_report)
         self.upload_thread_succeeded.connect(self.handle_upload_thread_succeeded)
@@ -407,15 +407,15 @@
         This function gets started in a background thread to call CreateJob.
         """
         try:
 
             def _continue_create_job_wait() -> bool:
                 return self._continue_submission
 
-            logger.info("Waiting for Job to be created...")
+            logger.info("Waiting for job to be created...")
 
             success = False
 
             logger.debug(json.dumps(self._create_job_args, indent=1))
             self._create_job_response = self._deadline_client.create_job(**self._create_job_args)
             logger.debug(f"CreateJob Response {self._create_job_response}")
 
@@ -430,15 +430,15 @@
                     self._queue_id,
                     job_id,
                     self._deadline_client,
                     _continue_create_job_wait,
                 )
                 message += f"\n{job_id}\n"
             else:
-                message = "CreateJob response was empty, or did not contain a Job ID."
+                message = "CreateJob response was empty, or did not contain a job ID."
             if success:
                 self.create_job_thread_succeeded.emit(success, message)
             else:
                 self.create_job_thread_exception.emit(DeadlineOperationError(message))
         except CreateJobWaiterCanceled as e:
             # If it wasn't canceled, send the exception to the dialog
             if self._continue_submission:
@@ -457,39 +457,39 @@
     ) -> None:
         """
         Starts the background hashing thread.
         """
         self.status_label.setText("Hashing job attachments...")
         self.__hashing_thread = threading.Thread(
             target=self._hashing_background_thread,
-            name="AWS Deadline Cloud Hashing Background Thread",
+            name="AWS Deadline Cloud hashing background thread",
             args=(asset_groups, total_input_files, total_input_bytes),
         )
         self.__hashing_thread.start()
 
     def _start_upload(self, asset_manifests: List[AssetRootManifest]) -> None:
         """
         Starts the background upload thread.
         """
         self.status_label.setText("Uploading job attachments...")
         self.__upload_thread = threading.Thread(
             target=self._upload_background_thread,
-            name="AWS Deadline Cloud Upload Background Thread",
+            name="AWS Deadline Cloud upload background thread",
             args=(asset_manifests,),
         )
         self.__upload_thread.start()
 
     def _start_create_job(self) -> None:
         """
         Starts the background thread to call CreateJob.
         """
-        self.status_label.setText("Waiting for Job to be created...")
+        self.status_label.setText("Waiting for job to be created...")
         self.__create_job_thread = threading.Thread(
             target=self._create_job_background_thread,
-            name="AWS Deadline Cloud CreateJob Background Thread",
+            name="AWS Deadline Cloud CreateJob background thread",
         )
         self.__create_job_thread.start()
 
     def handle_hashing_thread_progress_report(
         self, progress_metadata: ProgressReportMetadata
     ) -> None:
         """
@@ -520,15 +520,15 @@
         Handles the signal sent from the background hashing thread when the
         hashing process has completed.
         """
         api.get_deadline_cloud_library_telemetry_client().record_hashing_summary(
             hashing_summary, from_gui=True
         )
         self.summary_edit.setText(
-            f"\nHashing Summary:\n{textwrap.indent(str(hashing_summary), '    ')}"
+            f"\nHashing summary:\n{textwrap.indent(str(hashing_summary), '    ')}"
         )
         self._start_upload(asset_manifests)
 
     def handle_upload_thread_succeeded(
         self, upload_summary: SummaryStatistics, attachment_settings: Any
     ) -> None:
         """
@@ -542,15 +542,15 @@
             )
 
         api.get_deadline_cloud_library_telemetry_client().record_upload_summary(
             upload_summary, from_gui=True
         )
         self.summary_edit.setText(
             f"{self.summary_edit.toPlainText()}"
-            + f"\nUpload Summary:\n{textwrap.indent(str(upload_summary), '    ')}"
+            + f"\nUpload summary:\n{textwrap.indent(str(upload_summary), '    ')}"
         )
 
         self._start_create_job()
 
     def handle_create_job_thread_succeeded(self, success: bool, status_message: str) -> None:
         """
         Handles the signal sent from the background CreateJob thread when the
@@ -560,19 +560,19 @@
             event_type="com.amazon.rum.deadline.create_job",
             event_details={"is_success": success},
             from_gui=True,
         )
 
         if success:
             self._submission_complete = True
-            self.status_label.setText("Submission Complete")
+            self.status_label.setText("Submission complete")
             self.button_box.setStandardButtons(QDialogButtonBox.Ok)
             self.button_box.button(QDialogButtonBox.Ok).setDefault(True)
         else:
-            self.status_label.setText("Submission Error")
+            self.status_label.setText("Submission error")
             self.button_box.setStandardButtons(QDialogButtonBox.Close)
             self.button_box.button(QDialogButtonBox.Close).setDefault(True)
 
         self.summary_edit.setText(f"{status_message} {self.summary_edit.toPlainText()}")
         self.summary_edit.setVisible(True)
         self.adjustSize()
 
@@ -581,15 +581,15 @@
         Handles the signal sent from the background threads when an exception is
         thrown.
         """
         self.hashing_progress.setVisible(False)
         self.upload_progress.setVisible(False)
         self.status_label.setVisible(False)
         self.button_box.setStandardButtons(QDialogButtonBox.Close)
-        self.summary_edit.setText(f"Error Occurred: {str(e)}")
+        self.summary_edit.setText(f"Error occurred: {str(e)}")
         self.summary_edit.setVisible(True)
         self.adjustSize()
         logger.error(str(e))
 
     def _confirm_asset_references_outside_storage_profile(
         self, upload_group: AssetUploadGroup
     ) -> bool:
@@ -649,15 +649,15 @@
         if not warning_message:
             # If we don't have any warnings, add the "Do not ask again" button that acts like 'OK' but sets the config
             # setting to always auto-accept similar prompts in the future.
             dont_ask_button = QPushButton("Do not ask again", self)
             dont_ask_button.clicked.connect(lambda: set_setting("settings.auto_accept", "true"))
             message_box.addButton(dont_ask_button, QMessageBox.ActionRole)
 
-        message_box.setWindowTitle("Job Attachments Valid Files Confirmation")
+        message_box.setWindowTitle("Job attachments valid files confirmation")
         selection = message_box.exec()
 
         return selection != QMessageBox.Cancel
 
     def closeEvent(self, event: QCloseEvent) -> None:
         """
         Overrides the closeEvent function to shutdown any running threads before
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py` & `deadline-0.48.1/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         self.button_box.addButton(self.logout_button, QDialogButtonBox.ResetRole)
         self.settings_button = QPushButton("Settings...")
         self.settings_button.clicked.connect(self.on_settings_button_clicked)
         self.button_box.addButton(self.settings_button, QDialogButtonBox.ResetRole)
         self.submit_button = QPushButton("Submit")
         self.submit_button.clicked.connect(self.on_submit)
         self.button_box.addButton(self.submit_button, QDialogButtonBox.AcceptRole)
-        self.export_bundle_button = QPushButton("Export Bundle")
+        self.export_bundle_button = QPushButton("Export bundle")
         self.export_bundle_button.clicked.connect(self.on_export_bundle)
         self.button_box.addButton(self.export_bundle_button, QDialogButtonBox.AcceptRole)
 
         self.lyt.addWidget(self.button_box)
 
     def _set_submit_button_state(self):
         # Enable/disable the Submit button based on whether the
@@ -193,22 +193,22 @@
             and self.shared_job_settings.is_queue_valid()
         )
 
         self.submit_button.setEnabled(enable)
 
         if not enable:
             self.submit_button.setToolTip(
-                "Cannot submit job to deadline cloud. Nonvalid credentials or queue parameters."
+                "Cannot submit job to Deadline Cloud. Nonvalid credentials or queue parameters."
             )
         else:
             self.submit_button.setToolTip("")
 
     def refresh_deadline_settings(self):
         # Enable/disable the Login and Logout buttons based on whether
-        # the configured profile is for Deadline Cloud Monitor
+        # the configured profile is for Deadline Cloud monitor
         self.login_button.setEnabled(
             self.deadline_authentication_status.creds_source
             == api.AwsCredentialsSource.DEADLINE_CLOUD_MONITOR_LOGIN
         )
         self.logout_button.setEnabled(
             self.deadline_authentication_status.creds_source
             == api.AwsCredentialsSource.DEADLINE_CLOUD_MONITOR_LOGIN
@@ -229,52 +229,52 @@
         """
         if event.key() == Qt.Key_Return or event.key() == Qt.Key_Enter:
             return
         super().keyPressEvent(event)
 
     def _build_shared_job_settings_tab(self, initial_job_settings, initial_shared_parameter_values):
         self.shared_job_settings_tab = QScrollArea()
-        self.tabs.addTab(self.shared_job_settings_tab, "Shared Job Settings")
+        self.tabs.addTab(self.shared_job_settings_tab, "Shared job settings")
         self.shared_job_settings = SharedJobSettingsWidget(
             initial_settings=initial_job_settings,
             initial_shared_parameter_values=initial_shared_parameter_values,
             parent=self,
         )
         self.shared_job_settings.parameter_changed.connect(self.on_shared_job_parameter_changed)
         self.shared_job_settings_tab.setWidget(self.shared_job_settings)
         self.shared_job_settings_tab.setWidgetResizable(True)
         self.shared_job_settings.parameter_changed.connect(self.on_shared_job_parameter_changed)
 
     def _build_job_settings_tab(self, job_setup_widget_type, initial_job_settings):
         self.job_settings_tab = QScrollArea()
-        self.tabs.addTab(self.job_settings_tab, "Job-Specific Settings")
+        self.tabs.addTab(self.job_settings_tab, "Job-specific settings")
         self.job_settings_tab.setWidgetResizable(True)
 
         self.job_settings = job_setup_widget_type(
             initial_settings=initial_job_settings, parent=self
         )
         self.job_settings_tab.setWidget(self.job_settings)
         if hasattr(self.job_settings, "parameter_changed"):
             self.job_settings.parameter_changed.connect(self.on_job_template_parameter_changed)
 
     def _build_job_attachments_tab(
         self, auto_detected_attachments: AssetReferences, attachments: AssetReferences
     ):
         self.job_attachments_tab = QScrollArea()
-        self.tabs.addTab(self.job_attachments_tab, "Job Attachments")
+        self.tabs.addTab(self.job_attachments_tab, "Job attachments")
         self.job_attachments = JobAttachmentsWidget(
             auto_detected_attachments, attachments, parent=self
         )
         self.job_attachments_tab.setWidget(self.job_attachments)
         self.job_attachments_tab.setWidgetResizable(True)
 
     def _build_host_requirements_tab(self):
         self.host_requirements = HostRequirementsWidget()
         self.host_requirements_tab = QScrollArea()
-        self.tabs.addTab(self.host_requirements_tab, "Host Requirements")
+        self.tabs.addTab(self.host_requirements_tab, "Host requirements")
         self.host_requirements_tab.setWidget(self.host_requirements)
         self.host_requirements_tab.setWidgetResizable(True)
 
     def on_shared_job_parameter_changed(self, parameter: dict[str, Any]):
         """
         Handles an edit to a shared job parameter, for example one of the
         queue parameters.
@@ -367,23 +367,23 @@
 
             logger.info(f"Saved the submission as a job bundle: {job_history_bundle_dir}")
             if sys.platform == "win32":
                 # Open the directory in the OS's file explorer
                 os.startfile(job_history_bundle_dir)
             QMessageBox.information(
                 self,
-                f"{settings.submitter_name} Job Submission",
+                f"{settings.submitter_name} job submission",
                 f"Saved the submission as a job bundle:\n{job_history_bundle_dir}",
             )
             # Close the submitter window to signal the submission is done
             self.close()
         except Exception as exc:
             logger.exception("Error saving bundle")
             message = str(exc)
-            QMessageBox.warning(self, f"{settings.submitter_name} Job Submission", message)
+            QMessageBox.warning(self, f"{settings.submitter_name} job submission", message)
 
     def on_submit(self):
         """
         Perform a submission when the submit button is pressed
         """
         # Retrieve all the settings into the dataclass
         settings = self.job_settings_type()
@@ -475,24 +475,24 @@
                 asset_manager,
                 deadline,
                 auto_accept=str2bool(get_setting("settings.auto_accept")),
                 require_paths_exist=self.job_attachments.get_require_paths_exist(),
             )
         except UserInitiatedCancel as uic:
             logger.info("Canceling submission.")
-            QMessageBox.information(self, f"{settings.submitter_name} Job Submission", str(uic))
+            QMessageBox.information(self, f"{settings.submitter_name} job submission", str(uic))
             job_progress_dialog.close()
         except Exception as exc:
             logger.exception("error submitting job")
             api.get_deadline_cloud_library_telemetry_client().record_error(
                 event_details={"exception_scope": "on_submit"},
                 exception_type=str(type(exc)),
                 from_gui=True,
             )
-            QMessageBox.warning(self, f"{settings.submitter_name} Job Submission", str(exc))
+            QMessageBox.warning(self, f"{settings.submitter_name} job submission", str(exc))
             job_progress_dialog.close()
 
         if self.create_job_response:
             # Close the submitter window to signal the submission is done but
             # keep the standalone gui submitter open
             if settings.submitter_name != "JobBundle":
                 self.close()
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/resources/deadline_logo.svg` & `deadline-0.48.1/src/deadline/client/ui/resources/deadline_logo.svg`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/ui/resources/blender_example_bundle/template.yaml` & `deadline-0.48.1/src/deadline/client/ui/resources/blender_example_bundle/template.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,22 @@
     default: "output_####"
     description: Enter the output filename pattern (without extension).
   - name: Format
     type: STRING
     description: Choose the file format to render as.
     default: PNG
     allowedValues: [TGA, RAWTGA, JPEG, IRIS, IRIZ, PNG, HDR, TIFF, OPEN_EXR, OPEN_EXR_MULTILAYER, CINEON, DPX, DDS, JP2, WEBP]
+  - name: CondaPackages
+    type: STRING
+    default: "blender"
+    description: List the conda packages to use, separated by spaces. Needs a queue environment to consume it.
   - name: RezPackages
     type: STRING
     default: "blender"
-    description: List the rez packages to use, separated by spaces. Needs a Queue Environment to consume it.
+    description: List the rez packages to use, separated by spaces. Needs a queue environment to consume it.
 steps:
 - name: RenderBlender
   parameterSpace:
     taskParameterDefinitions:
     - name: Frame
       type: INT
       range: "{{Param.Frames}}"
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/resources/cli_job_bundle/template.yaml` & `deadline-0.48.1/src/deadline/client/ui/resources/cli_job_bundle/template.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 specificationVersion: 'jobtemplate-2023-09'
-name: Job Bundle - CLI Job Example
+name: Job bundle - CLI job example
 parameterDefinitions:
   - name: BashScript
     type: STRING
     userInterface:
       control: MULTILINE_EDIT
-      label: Bash Script
+      label: Bash script
     description: "Write your bash script code here."
     default: |
       echo "The file contents attached to this job:"
       ls
 
       # Example workload to compute hashes of all the input
       find . -type f -exec md5sum {} \; > computed_hashes.txt
   - name: DataDir
     type: PATH
     objectType: DIRECTORY
     dataFlow: INOUT
     userInterface:
       control: CHOOSE_DIRECTORY
-      label: Input/Output Data Directory
+      label: Input/Output data directory
     description: |
       This is a directory for your input files. Any output files
       that the script writes will download back to the same
       directory.
 steps:
 - name: CliScript
   script:
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml` & `deadline-0.48.1/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,161 +1,161 @@
 specificationVersion: 'jobtemplate-2023-09'
-name: Job Template GUI Control Showcase
+name: Job template GUI control showcase
 parameterDefinitions:
   - name: LineEditControl
     type: STRING
     userInterface:
       control: LINE_EDIT
-      label: Line Edit Control
-      groupLabel: Text Controls
+      label: Line edit control
+      groupLabel: Text controls
     description: "Unrestricted line of text!"
     default: Default line edit value.
   - name: MultiLineEditControl
     type: STRING
     userInterface:
       control: MULTILINE_EDIT
-      label: Multi-line Edit Control
-      groupLabel: Text Controls
+      label: Multi-line edit control
+      groupLabel: Text controls
     description: "Unrestricted text file"
     default: |
       This is a
       text file with
       multiple lines.
   - name: IntSpinner
     type: INT
     userInterface:
       control: SPIN_BOX
-      label: Default Int Spinner
-      groupLabel: Int Spinners
+      label: Default int spinner
+      groupLabel: Int spinners
     description: A default integer spinner.
     default: 42
   - name: BigStepIntSpinner
     type: INT
     userInterface:
       control: SPIN_BOX
-      label: Big Step Int Spinner
-      groupLabel: Int Spinners
+      label: Big step int spinner
+      groupLabel: Int spinners
       singleStepDelta: 30
     description: A default integer spinner.
     default: 123
   - name: BoundedIntSpinner
     type: INT
     userInterface:
       control: SPIN_BOX
-      label: Bounded Int Spinner
-      groupLabel: Int Spinners
+      label: Bounded int spinner
+      groupLabel: Int spinners
     description: A bounded integer spin box.
     minValue: -100
     maxValue: 100
     default: 25
   - name: FloatSpinner
     type: FLOAT
     userInterface:
       control: SPIN_BOX
-      label: Default Float Spinner
-      groupLabel: Float Spinners
+      label: Default float spinner
+      groupLabel: Float spinners
     description: A default float spinner.
     default: 1234.56789
   - name: FloatSpinnerOneDecimal
     type: FLOAT
     userInterface:
       control: SPIN_BOX
-      label: Float Spinner One Decimal
-      groupLabel: Float Spinners
+      label: Float spinner one decimal
+      groupLabel: Float spinners
       decimals: 1
     description: A float spinner with one decimal of precision.
     default: 100000.01
   - name: FloatSpinnerFixedStep
     type: FLOAT
     userInterface:
       control: SPIN_BOX
-      label: Float Spinner Fixed Step
-      groupLabel: Float Spinners
+      label: Float spinner fixed step
+      groupLabel: Float spinners
       singleStepDelta: 0.875
     default: 0.0
     description: A float spinner with a fixed step of .875
   - name: StringDropdown
     type: STRING
     userInterface:
       control: DROPDOWN_LIST
-      label: String Dropdown
-      groupLabel: Dropdown Controls
+      label: String dropdown
+      groupLabel: Dropdown controls
     description: A dropdown with string values.
     default: WEDNESDAY
     allowedValues: [MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY, SUNDAY]
   - name: IntDropdown
     type: INT
     userInterface:
       control: DROPDOWN_LIST
-      label: Int Dropdown
-      groupLabel: Dropdown Controls
+      label: Int dropdown
+      groupLabel: Dropdown controls
     description: A dropdown with integer values.
     default: 7
     allowedValues: [3, 8, 7, 2, 9, 1]
   - name: HiddenFieldOne
     type: INT
     userInterface:
       control: HIDDEN
     description: A hidden field that won't show on the UI
     default: 10
   - name: FloatDropdown
     type: FLOAT
     userInterface:
       control: DROPDOWN_LIST
-      label: Float Dropdown
-      groupLabel: Dropdown Controls
+      label: Float dropdown
+      groupLabel: Dropdown controls
     description: A dropdown with floating point values.
     default: 3.26
     allowedValues: [1.23, 3.26, 9.9, 1.2345]
   - name: InputFilePicker
     type: PATH
     objectType: FILE
     dataFlow: IN
     userInterface:
       control: CHOOSE_INPUT_FILE
-      label: Input File Picker
-      groupLabel: Picker Controls
+      label: Input file picker
+      groupLabel: Picker controls
       fileFilters:
-      - label: Scene Files
+      - label: Scene files
         patterns: ["*.blend", "*.mb", "*.ma", "*.nk"]
-      - label: Any Files
+      - label: Any files
         patterns: ["*"]
     description: Choose the input scene file.
   - name: OutputFilePicker
     type: PATH
     objectType: FILE
     dataFlow: OUT
     userInterface:
       control: CHOOSE_OUTPUT_FILE
-      label: Output File Picker
-      groupLabel: Picker Controls
+      label: Output file picker
+      groupLabel: Picker controls
       fileFilters:
-      - label: EXR Files
+      - label: EXR files
         patterns: ["*.exr"]
-      - label: JPEG Files
+      - label: JPEG files
         patterns: ["*.jpg", "*.jpeg"]
-      - label: PNG Files
+      - label: PNG files
         patterns: ["*.png"]
-      - label: All Files
+      - label: All files
         patterns: ["*"]
     description: Choose the output image file.
   - name: DirectoryPicker
     type: PATH
     objectType: DIRECTORY
     dataFlow: INOUT
     userInterface:
       control: CHOOSE_DIRECTORY
-      label: Directory Picker
-      groupLabel: Picker Controls
+      label: Directory picker
+      groupLabel: Picker controls
     description: Choose a directory.
   - name: CheckBox
     type: STRING
     userInterface:
       control: CHECK_BOX
-      label: Check Box "Boolean"
+      label: Check box "boolean"
     default: "True"
     allowedValues: ["True", "False"]
     description: Set a true/false value.
   - name: HiddenFieldTwo
     type: STRING
     userInterface:
       control: HIDDEN
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/widgets/cli_job_settings_tab.py` & `deadline-0.48.1/src/deadline/client/ui/widgets/cli_job_settings_tab.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def __init__(self, initial_settings: CliJobSettings, parent=None):
         super().__init__(parent=parent)
 
         self._build_ui()
         self._load_initial_settings(initial_settings)
 
     def _set_enabled_with_label(self, prop_name: str, enabled: bool):
-        """Enable/disable a control w/ its label"""
+        """Set the enabled status of a control and its label"""
         getattr(self, prop_name).setEnabled(enabled)
         getattr(self, prop_name + "_label").setEnabled(enabled)
 
     def _build_ui(self):
         layout = QGridLayout(self)
 
         self.bash_script = QTextEdit()
@@ -57,35 +57,35 @@
         font.setKerning(False)
         font.setPointSize(font.pointSize() + 1)
         self.bash_script.setCurrentFont(font)
         self.bash_script.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
 
         layout.addWidget(self.bash_script, 0, 0, 1, 2)
 
-        self.use_array_parameter_chck = QCheckBox("Use Array Parameter", self)
+        self.use_array_parameter_chck = QCheckBox("Use array parameter", self)
         self.array_parameter_name = QLineEdit(self)
         layout.addWidget(self.use_array_parameter_chck, 1, 0)
         layout.addWidget(self.array_parameter_name, 1, 1)
         self.use_array_parameter_chck.stateChanged.connect(self.use_array_parameter_changed)
 
-        self.array_parameter_values_label = QLabel("Array Parameter Values")
+        self.array_parameter_values_label = QLabel("Array parameter values")
         layout.addWidget(self.array_parameter_values_label, 2, 0)
         self.array_parameter_values = QLineEdit(self)
         layout.addWidget(self.array_parameter_values, 2, 1)
 
-        self.data_dir_label = QLabel("Data Dir")
+        self.data_dir_label = QLabel("Data directory")
         self.data_dir_edit = DirectoryPickerWidget(
             initial_directory=os.path.expanduser(os.path.join("~", "CLIJobData")),
-            directory_label="Data Dir",
+            directory_label="Data directory",
             parent=self,
         )
         layout.addWidget(self.data_dir_label, 3, 0)
         layout.addWidget(self.data_dir_edit, 3, 1)
 
-        self.file_format_label = QLabel("Template File Format")
+        self.file_format_label = QLabel("Template file format")
         self.file_format_box = QComboBox(parent=self)
         self.file_format_box.addItems(["YAML", "JSON"])
         layout.addWidget(self.file_format_label, 4, 0)
         layout.addWidget(self.file_format_box, 4, 1)
 
     def _load_initial_settings(self, initial_settings: CliJobSettings):
         self.bash_script.setPlainText(initial_settings.bash_script_contents)
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py` & `deadline-0.48.1/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,18 @@
     """
 
     def __init__(self, parent=None) -> None:
         super().__init__(parent=parent)
 
         layout = QHBoxLayout(self)
 
-        self.creds_source_group = AuthenticationStatusGroup(title="Credential Source", parent=self)
+        self.creds_source_group = AuthenticationStatusGroup(title="Credential source", parent=self)
         layout.addWidget(self.creds_source_group)
         self.auth_status_group = AuthenticationStatusGroup(
-            title="Authentication Status", parent=self
+            title="Authentication status", parent=self
         )
         layout.addWidget(self.auth_status_group)
         self.deadline_authorized_group = AuthenticationStatusGroup(
             title="AWS Deadline Cloud API", parent=self
         )
         layout.addWidget(self.deadline_authorized_group)
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/widgets/host_requirements_tab.py` & `deadline-0.48.1/src/deadline/client/ui/widgets/host_requirements_tab.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
 """
-UI widgets for the Host Requirements tab.
+UI widgets for the host requirements tab.
 """
 from typing import Any, Dict, List, Optional, Union
 from pathlib import Path
 
 from qtpy.QtCore import Qt  # type: ignore
 from qtpy.QtGui import QFont, QValidator, QIntValidator, QBrush, QIcon, QRegularExpressionValidator  # type: ignore
 from qtpy.QtWidgets import (  # type: ignore
@@ -201,16 +201,16 @@
 
     def __init__(self, parent=None):
         super().__init__("", parent=parent)
         self.layout = QVBoxLayout(self)
         self._build_ui()
 
     def _build_ui(self):
-        self.os_row = OSRequirementRowWidget("Operating System", ["linux", "macos", "windows"])
-        self.cpu_row = OSRequirementRowWidget("CPU Architecture", ["x86_64", "arm64"])
+        self.os_row = OSRequirementRowWidget("Operating system", ["linux", "macos", "windows"])
+        self.cpu_row = OSRequirementRowWidget("CPU architecture", ["x86_64", "arm64"])
 
         self.layout.addWidget(self.os_row)
         self.layout.addWidget(self.cpu_row)
 
     def get_requirements(self) -> List[Dict[str, Any]]:
         """
         Returns a list of OpenJD parameter definition dicts with
@@ -254,16 +254,16 @@
         self._build_ui()
 
     def _build_ui(self):
         # Build a custom row widget for each selectable option
         self.cpu_row = HardwareRequirementsRowWidget("vCPUs", self)
         self.memory_row = HardwareRequirementsRowWidget("Memory (GiB)", self)
         self.gpu_row = HardwareRequirementsRowWidget("GPUs", self)
-        self.gpu_memory_row = HardwareRequirementsRowWidget("GPU Memory (GiB)", self)
-        self.scratch_space_row = HardwareRequirementsRowWidget("Scratch Space", self)
+        self.gpu_memory_row = HardwareRequirementsRowWidget("GPU memory (GiB)", self)
+        self.scratch_space_row = HardwareRequirementsRowWidget("Scratch space", self)
 
         # Add all rows to layout
         self.layout.addWidget(self.cpu_row)
         self.layout.addWidget(self.memory_row)
         self.layout.addWidget(self.gpu_row)
         self.layout.addWidget(self.gpu_memory_row)
         self.layout.addWidget(self.scratch_space_row)
@@ -478,15 +478,15 @@
 
     def __init__(self, list_item: QListWidgetItem, item_number: int, parent=None):
         super().__init__(AMOUNT, list_item, item_number, parent)
         self._build_ui()
 
     def _build_ui(self):
         # Name / Value
-        self.name_label = QLabel("Amount Name")
+        self.name_label = QLabel("Amount name")
         self.name_label.setFixedWidth(LABEL_FIXED_WIDTH)
         self.name_line_edit = QLineEdit()
         self.name_line_edit.setFixedWidth(LABEL_FIXED_WIDTH)
         self.name_line_edit.setValidator(
             QRegularExpressionValidator(ATTRIBUTE_CAPABILITY_VALUE_REGEX)
         )
         assert (100 - len(AMOUNT_CAPABILITY_PREFIX)) > 0
@@ -572,15 +572,15 @@
         self, list_item: QListWidgetItem, item_number: int, parent=CustomRequirementsWidget
     ):
         super().__init__(ATTRIBUTE, list_item, item_number, parent)
         self._build_ui()
 
     def _build_ui(self):
         # Name / Value / All / Any
-        self.name_label = QLabel("Attribute Name")
+        self.name_label = QLabel("Attribute name")
         self.name_label.setFixedWidth(LABEL_FIXED_WIDTH)
         self.value_label = QLabel("Value(s)")
         self.all_of_button = QRadioButton("All")
         self.all_of_button.setChecked(True)
         self.any_of_button = QRadioButton("Any")
         self.name_line_edit = QLineEdit()
         self.name_line_edit.setFixedWidth(LABEL_FIXED_WIDTH)
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/widgets/job_attachments_tab.py` & `deadline-0.48.1/src/deadline/client/ui/widgets/job_attachments_tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
 """
-UI widgets for the Job Attachments tab.
+UI widgets for the job attachments tab.
 """
 from __future__ import annotations
 import os
 from logging import getLogger
 from typing import Optional
 
 from qtpy.QtWidgets import (  # type: ignore
@@ -57,35 +57,35 @@
 
     def _build_ui(self) -> None:
         tab_layout = QVBoxLayout(self)
 
         # Create a group box for general settings
         size_policy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         size_policy.setVerticalStretch(10)
-        self.general_group = QGroupBox("General Submission Settings", self)
+        self.general_group = QGroupBox("General submission settings", self)
         tab_layout.addWidget(self.general_group)
         self.general_group.setSizePolicy(size_policy)
         general_layout = QVBoxLayout(self.general_group)
 
         # Create a group box for each type of attachment
-        self.input_files_group = QGroupBox("Attach Input Files", self)
+        self.input_files_group = QGroupBox("Attach input files", self)
         size_policy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         size_policy.setVerticalStretch(80)
         tab_layout.addWidget(self.input_files_group)
         self.input_files_group.setSizePolicy(size_policy)
         input_files_layout = QVBoxLayout(self.input_files_group)
 
-        self.input_directories_group = QGroupBox("Attach Input Directories", self)
+        self.input_directories_group = QGroupBox("Attach input directories", self)
         size_policy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         size_policy.setVerticalStretch(10)
         self.input_directories_group.setSizePolicy(size_policy)
         tab_layout.addWidget(self.input_directories_group)
         input_directories_layout = QVBoxLayout(self.input_directories_group)
 
-        self.output_directories_group = QGroupBox("Specify Output Directories", self)
+        self.output_directories_group = QGroupBox("Specify output directories", self)
         size_policy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         size_policy.setVerticalStretch(10)
         self.output_directories_group.setSizePolicy(size_policy)
         tab_layout.addWidget(self.output_directories_group)
         output_directories_layout = QVBoxLayout(self.output_directories_group)
 
         # General settings
@@ -104,15 +104,15 @@
         self.input_files.setSortingEnabled(False)
         self.input_files.setSelectionMode(QAbstractItemView.ExtendedSelection)
         self.input_files.setAlternatingRowColors(True)
 
         input_files_layout.addWidget(self.input_files_controls)
         input_files_layout.addWidget(self.input_files)
 
-        # The "Attach Input Directories" attachments
+        # The "Attach input directories" attachments
         self.input_directories_controls = JobAttachmentsControlsWidget(self)
         self.input_directories_controls.show_auto_detected.stateChanged.connect(
             self.show_auto_detected_change
         )
         self.input_directories_controls.add.clicked.connect(self._add_input_directory)
         self.input_directories_controls.remove_selected.clicked.connect(
             self._remove_selected_input_directories
@@ -122,15 +122,15 @@
         self.input_directories.setSortingEnabled(False)
         self.input_directories.setSelectionMode(QAbstractItemView.ExtendedSelection)
         self.input_directories.setAlternatingRowColors(True)
 
         input_directories_layout.addWidget(self.input_directories_controls)
         input_directories_layout.addWidget(self.input_directories)
 
-        # The "Specify Output Directories" attachments
+        # The "Specify output directories" attachments
         self.output_directories_controls = JobAttachmentsControlsWidget(self)
         self.output_directories_controls.show_auto_detected.stateChanged.connect(
             self.show_auto_detected_change
         )
         self.output_directories_controls.add.clicked.connect(self._add_output_directory)
         self.output_directories_controls.remove_selected.clicked.connect(
             self._remove_selected_output_directories
@@ -228,15 +228,15 @@
             selected_count = len(list_widget.selectedItems())
             controls_widget.status_message.setText(
                 f"{len(auto_detected_set)} auto, {len(added_set)} added, {selected_count} selected"
             )
 
     def _add_input_files(self) -> None:
         new_files, _ = QFileDialog.getOpenFileNames(
-            self, "Select Input Files To Attach To Your Job"
+            self, "Select input files to attach to your job"
         )
 
         if new_files:
             # Normalize the paths
             paths = set(os.path.normpath(path) for path in new_files)
             # Remove any that are from the auto-detected set
             paths.difference_update(self.auto_detected_attachments.input_filenames)
@@ -256,15 +256,15 @@
             QMessageBox.warning(
                 self,
                 "Some files were not removed",
                 f"The selected files from the auto-detected list ({len(unremoved_files)} items) were not removed.",
             )
 
     def _add_input_directory(self) -> None:
-        new_dir = QFileDialog.getExistingDirectory(self, "Select a Directory To Attach To Your Job")
+        new_dir = QFileDialog.getExistingDirectory(self, "Select a directory to attach to your job")
 
         if new_dir:
             # Normalize the path
             new_dir = os.path.normpath(new_dir)
             # Check if it's in the auto-detected set
             if new_dir not in self.auto_detected_attachments.input_directories:
                 # Add it to the attachments
@@ -283,15 +283,15 @@
             QMessageBox.warning(
                 self,
                 "Some directories were not removed",
                 f"The selected directories from the auto-detected list ({len(unremoved_dirs)} items) were not removed.",
             )
 
     def _add_output_directory(self) -> None:
-        new_dir = QFileDialog.getExistingDirectory(self, "Select an Output Directory of Your Job")
+        new_dir = QFileDialog.getExistingDirectory(self, "Select an output directory of your job")
 
         if new_dir:
             # Normalize the path
             new_dir = os.path.normpath(new_dir)
             # Check if it's in the auto-detected set
             if new_dir not in self.auto_detected_attachments.output_directories:
                 # Add it to the attachments
@@ -353,17 +353,17 @@
 
         layout = QHBoxLayout(self)
         layout.setContentsMargins(0, 0, 0, 0)
 
         self.add = QPushButton("Add...", parent=self)
         layout.addWidget(self.add)
 
-        self.remove_selected = QPushButton("Remove Selected", parent=self)
+        self.remove_selected = QPushButton("Remove selected", parent=self)
         layout.addWidget(self.remove_selected)
 
         self.status_message = QLabel("0 total")
         self.status_message.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Minimum)
         layout.addWidget(self.status_message)
 
-        self.show_auto_detected = QCheckBox("Show Auto-Detected", parent=self)
+        self.show_auto_detected = QCheckBox("Show auto-detected", parent=self)
         self.show_auto_detected.setChecked(True)
         layout.addWidget(self.show_auto_detected)
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/widgets/job_bundle_settings_tab.py` & `deadline-0.48.1/src/deadline/client/ui/widgets/job_bundle_settings_tab.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
 """
-UI widgets for the Scene Settings tab.
+UI widgets for the scene settings tab.
 """
 from __future__ import annotations
 
 import os
 from logging import getLogger
 from typing import Any
 
@@ -88,15 +88,15 @@
     def on_load_bundle(self):
         """
         Browse and load the selected submission bundle
         """
         # Open the file picker dialog
         bundle_path = os.path.expanduser(config_file.get_setting("settings.job_history_dir"))
         input_job_bundle_dir = QFileDialog.getExistingDirectory(
-            self, "Choose Job Bundle Directory", bundle_path
+            self, "Choose job bundle directory", bundle_path
         )
         if not input_job_bundle_dir:
             return
 
         # Warn the user if the Job Bundle could not be loaded
         try:
             validate_directory_symlink_containment(input_job_bundle_dir)
@@ -105,24 +105,24 @@
                 read_yaml_or_json_object(input_job_bundle_dir, "asset_references", False) or {}
             )
             asset_references = AssetReferences.from_dict(asset_references_obj)
 
             # Load the template to get the bundle name
             template = read_yaml_or_json_object(input_job_bundle_dir, "template", True)
             name = (
-                template.get("name", "Job Bundle Submission")
+                template.get("name", "Job bundle submission")
                 if template
-                else "Job Bundle Submission"
+                else "Job bundle submission"
             )
             job_settings = JobBundleSettings(input_job_bundle_dir=input_job_bundle_dir, name=name)
             job_settings.parameters = read_job_bundle_parameters(input_job_bundle_dir)
 
         except Exception as e:
             msg = str(e)
-            QMessageBox.warning(self, "Could not Load Job Bundle", msg)
+            QMessageBox.warning(self, "Could not load job bundle", msg)
             logger.warning(msg)
             return
 
         if hasattr(self.parent, "refresh"):
             self.parent.refresh(
                 job_settings=job_settings,
                 auto_detected_attachments=asset_references,
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/widgets/openjd_parameters_widget.py` & `deadline-0.48.1/src/deadline/client/ui/widgets/openjd_parameters_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,26 +482,26 @@
         if "minValue" in parameter:
             min_value = parameter["minValue"]
             if isinstance(min_value, str):
                 try:
                     min_value = float(min_value)
                 except ValueError:
                     raise RuntimeError(
-                        f"Job Template parameter {parameter['name']} with FLOAT type has non-numeric 'minValue' of {min_value!r}"
+                        f"Job template parameter {parameter['name']} with FLOAT type has non-numeric 'minValue' of {min_value!r}"
                     )
             self.edit_control.setMinimum(min_value)
 
         if "maxValue" in parameter:
             max_value = parameter["maxValue"]
             if isinstance(max_value, str):
                 try:
                     max_value = float(max_value)
                 except ValueError:
                     raise RuntimeError(
-                        f"Job Template parameter {parameter['name']} with FLOAT type has non-numeric 'maxValue' of {max_value!r}"
+                        f"Job template parameter {parameter['name']} with FLOAT type has non-numeric 'maxValue' of {max_value!r}"
                     )
             self.edit_control.setMaximum(max_value)
 
         # Control customizations
         # Control customizations
         if "userInterface" in parameter:
             decimals = parameter["userInterface"].get("decimals", -1)
@@ -602,15 +602,15 @@
     OPENJD_TYPES: List[str] = ["PATH"]
     OPENJD_DEFAULT_VALUE: str = ""
     OPENJD_REQUIRED_PARAMETER_FIELDS: List[str] = []
     OPENJD_DISALLOWED_PARAMETER_FIELDS: List[str] = ["allowedValues"]
 
     def _build_ui(self, parameter):
         # Get the filters
-        filetype_filter = "Any Files (*)"
+        filetype_filter = "Any files (*)"
         selected_filter = ""
         if "userInterface" in parameter:
             file_filter_list = parameter["userInterface"].get("fileFilters")
             if file_filter_list:
                 filetype_filter = ";;".join(
                     f"{file_filter['label']} ({' '.join(file_filter['patterns'])})"
                     for file_filter in file_filter_list
@@ -740,15 +740,15 @@
         self.setLayout(layout)
 
         # Validate that 'allowedValues' is correct
         allowed_values = parameter.get("allowedValues", [])
         allowed_values_set = set(v.upper() for v in allowed_values)
         if allowed_values_set not in [set(allowed) for allowed in ALLOWED_VALUES_FOR_CHECK_BOX]:
             raise RuntimeError(
-                f"Job Template parameter {parameter['name']} with CHECK_BOX user interface control requires that 'allowedValues' be "
+                f"Job template parameter {parameter['name']} with CHECK_BOX user interface control requires that 'allowedValues' be "
                 + f"one of {ALLOWED_VALUES_FOR_CHECK_BOX} (case and order insensitive)"
             )
 
         # Determine the true/false correspondence
         true_values = [allowed[0] for allowed in ALLOWED_VALUES_FOR_CHECK_BOX]
         if allowed_values[0].upper() in true_values:
             self.true_value = allowed_values[0]
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/widgets/path_widgets.py` & `deadline-0.48.1/src/deadline/client/ui/widgets/path_widgets.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/client/ui/widgets/shared_job_settings_tab.py` & `deadline-0.48.1/src/deadline/client/ui/widgets/shared_job_settings_tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     def _handle_background_queue_parameters_exception(self, title: str, error: BaseException):
         self.__valid_queue = False
         self.valid_parameters.emit(False)
         if self.__refresh_queue_parameters_thread:
             self.canceled.set_canceled()
             self.__refresh_queue_parameters_thread.join()
         self.queue_parameters_box.rebuild_ui(
-            async_loading_state="Error Loading Queue Environments: {}\n\nError Traceback: {}".format(
+            async_loading_state="Error loading queue environments: {}\n\nError traceback: {}".format(
                 title, error
             )
         )
 
     def _start_load_queue_parameters_thread(self):
         """
         Starts a background thread to load the queue parameters.
@@ -164,15 +164,15 @@
             # If the user has not selected a farm or queue ID, don't bother starting
             # the thread.
             return
         self.__refresh_queue_parameters_id += 1
         self.canceled = CancelationFlag()
         self.__refresh_queue_parameters_thread = threading.Thread(
             target=self._load_queue_parameters_thread_function,
-            name="AWS Deadline Cloud Load Queue Parameters Thread",
+            name="AWS Deadline Cloud load queue parameters thread",
             args=(self.__refresh_queue_parameters_id, farm_id, queue_id),
         )
         self.__refresh_queue_parameters_thread.start()
 
     def is_queue_valid(self) -> bool:
         return self.__valid_queue
 
@@ -193,15 +193,15 @@
         """
         try:
             queue_parameters = get_queue_parameter_definitions(farmId=farm_id, queueId=queue_id)
             if not self.canceled:
                 self._queue_parameters_update.emit(refresh_id, queue_parameters)
         except BaseException as e:
             if not self.canceled:
-                self._background_exception.emit("Invalid Queue Parameters", e)
+                self._background_exception.emit("Invalid queue parameters", e)
 
     def update_settings(self, settings):
         self.shared_job_properties_box.update_settings(settings)
 
     def get_parameters(self):
         """
         Returns a list of OpenJD parameter definition dicts with
@@ -251,30 +251,30 @@
         self.desc_edit = QLineEdit()
         self.layout.addRow(self.desc_label, self.desc_edit)
 
         self.priority_box_label = QLabel("Priority")
         self.priority_box = QSpinBox(parent=self)
         self.layout.addRow(self.priority_box_label, self.priority_box)
 
-        self.initial_status_box_label = QLabel("Initial State")
+        self.initial_status_box_label = QLabel("Initial state")
         self.initial_status_box = QComboBox(parent=self)
         self.initial_status_box.addItems(["READY", "SUSPENDED"])
         self.layout.addRow(self.initial_status_box_label, self.initial_status_box)
 
-        self.max_failed_tasks_count_box_label = QLabel("Maximum Failed Tasks Count")
+        self.max_failed_tasks_count_box_label = QLabel("Maximum failed tasks count")
         self.max_failed_tasks_count_box_label.setToolTip(
-            "Maximum number of Tasks that can fail before the Job will be marked as failed."
+            "Maximum number of tasks that can fail before the job will be marked as failed."
         )
         self.max_failed_tasks_count_box = QSpinBox(parent=self)
         self.max_failed_tasks_count_box.setRange(0, 2147483647)
         self.layout.addRow(self.max_failed_tasks_count_box_label, self.max_failed_tasks_count_box)
 
-        self.max_retries_per_task_box_label = QLabel("Maximum Retries Per Task")
+        self.max_retries_per_task_box_label = QLabel("Maximum retries per task")
         self.max_retries_per_task_box_label.setToolTip(
-            "Maximum number of times that a Task will retry before it's marked as failed."
+            "Maximum number of times that a task will retry before it's marked as failed."
         )
         self.max_retries_per_task_box = QSpinBox(parent=self)
         self.max_retries_per_task_box.setRange(0, 2147483647)
         self.layout.addRow(self.max_retries_per_task_box_label, self.max_retries_per_task_box)
 
     def refresh_ui(self, settings: Any):
         self.sub_name_edit.setText(settings.name)
@@ -310,37 +310,37 @@
         """
         return [
             {
                 "name": "deadline:targetTaskRunStatus",
                 "type": "STRING",
                 "userInterface": {
                     "control": "DROPDOWN_LIST",
-                    "label": "Initial State",
+                    "label": "Initial state",
                 },
                 "allowedValues": ["READY", "SUSPENDED"],
                 "value": self.initial_status_box.currentText(),
             },
             {
                 "name": "deadline:maxFailedTasksCount",
                 "description": "Maximum number of Tasks that can fail before the Job will be marked as failed.",
                 "type": "INT",
                 "userInterface": {
                     "control": "SPIN_BOX",
-                    "label": "Maximum Failed Tasks Count",
+                    "label": "Maximum failed tasks count",
                 },
                 "minValue": 0,
                 "value": self.max_failed_tasks_count_box.value(),
             },
             {
                 "name": "deadline:maxRetriesPerTask",
-                "description": "Maximum number of times that a Task will retry before it's marked as failed.",
+                "description": "Maximum number of times that a task will retry before it's marked as failed.",
                 "type": "INT",
                 "userInterface": {
                     "control": "SPIN_BOX",
-                    "label": "Maximum Retries Per Task",
+                    "label": "Maximum retries per task",
                 },
                 "minValue": 0,
                 "value": self.max_retries_per_task_box.value(),
             },
             {"name": "deadline:priority", "type": "INT", "value": self.priority_box.value()},
         ]
 
@@ -350,27 +350,27 @@
         """
         settings.name = self.sub_name_edit.text()
         settings.description = self.desc_edit.text()
 
 
 class DeadlineCloudSettingsWidget(QGroupBox):
     """
-    UI component for the Deadline Render Manager.
+    UI component for the Deadline Cloud settings.
     """
 
     def __init__(self, *, parent: Optional[QWidget] = None):
-        super().__init__("Deadline Cloud Settings", parent=parent)
+        super().__init__("Deadline Cloud settings", parent=parent)
         self.deadline_settings: Dict[str, Any] = {"counter": -1}
         self.layout = QFormLayout(self)
         self.layout.setFieldGrowthPolicy(QFormLayout.AllNonFixedFieldsGrow)
 
         self._build_ui()
 
     def _set_enabled_with_label(self, prop_name: str, enabled: bool):
-        """Enable/disable a control w/ its label"""
+        """Sets the enabled status of a control and its label"""
         getattr(self, prop_name).setEnabled(enabled)
         getattr(self, prop_name + "_label").setEnabled(enabled)
 
     def _build_ui(self):
         """
         Build the UI for the Deadline settings
         """
@@ -468,15 +468,15 @@
             # Only call the AWS Deadline Cloud API if we've confirmed access
             if deadline_authorized:
                 display_name = "<refreshing> - " + display_name
 
                 self.__refresh_id += 1
                 self.__refresh_thread = threading.Thread(
                     target=self._refresh_thread_function,
-                    name=f"AWS Deadline Cloud Refresh {self.resource_name} Item Thread",
+                    name=f"AWS Deadline Cloud refresh {self.resource_name} item thread",
                     args=(self.__refresh_id,),
                 )
                 self.__refresh_thread.start()
 
             self.label.setText(display_name)
             self.label.setToolTip(self.item_description)
         else:
@@ -497,15 +497,15 @@
         """
         try:
             item = self.get_item()
             if not self.canceled:
                 self._item_update.emit(refresh_id, *item)
         except BaseException as e:
             if not self.canceled:
-                self.background_exception.emit(f"Refresh {self.resource_name} Item", e)
+                self.background_exception.emit(f"Refresh {self.resource_name} item", e)
 
 
 class DeadlineFarmDisplay(_DeadlineNamedResourceDisplay):
     def __init__(self, *, parent=None):
         super().__init__(resource_name="Farm", setting_name="defaults.farm_id", parent=parent)
 
     def get_item(self):
@@ -536,15 +536,15 @@
 class DeadlineStorageProfileNameDisplay(_DeadlineNamedResourceDisplay):
     WINDOWS_OS = "Windows"
     MAC_OS = "Macos"
     LINUX_OS = "Linux"
 
     def __init__(self, *, parent=None):
         super().__init__(
-            resource_name="Storage Profile Name",
+            resource_name="Storage profile name",
             setting_name="settings.storage_profile_id",
             parent=parent,
         )
 
     def get_item(self):
         farm_id = get_setting("defaults.farm_id")
         queue_id = get_setting("defaults.queue_id")
```

### Comparing `deadline-0.48.0/src/deadline/client/ui/widgets/spinbox_widgets.py` & `deadline-0.48.1/src/deadline/client/ui/widgets/spinbox_widgets.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/README.md` & `deadline-0.48.1/src/deadline/job_attachments/README.md`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/_utils.py` & `deadline-0.48.1/src/deadline/job_attachments/_utils.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/asset_sync.py` & `deadline-0.48.1/src/deadline/job_attachments/asset_sync.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/download.py` & `deadline-0.48.1/src/deadline/job_attachments/download.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/exceptions.py` & `deadline-0.48.1/src/deadline/job_attachments/exceptions.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/models.py` & `deadline-0.48.1/src/deadline/job_attachments/models.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/os_file_permission.py` & `deadline-0.48.1/src/deadline/job_attachments/os_file_permission.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/progress_tracker.py` & `deadline-0.48.1/src/deadline/job_attachments/progress_tracker.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/upload.py` & `deadline-0.48.1/src/deadline/job_attachments/upload.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/vfs.py` & `deadline-0.48.1/src/deadline/job_attachments/vfs.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/_aws/aws_clients.py` & `deadline-0.48.1/src/deadline/job_attachments/_aws/aws_clients.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/_aws/deadline.py` & `deadline-0.48.1/src/deadline/job_attachments/_aws/deadline.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/_windows/file.py` & `deadline-0.48.1/src/deadline/job_attachments/_windows/file.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/__init__.py` & `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/_canonical_json.py` & `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/_canonical_json.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/base_manifest.py` & `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/base_manifest.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/decode.py` & `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/decode.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/hash_algorithms.py` & `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/hash_algorithms.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/manifest_model.py` & `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/manifest_model.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json` & `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py` & `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/caches/cache_db.py` & `deadline-0.48.1/src/deadline/job_attachments/caches/cache_db.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/caches/hash_cache.py` & `deadline-0.48.1/src/deadline/job_attachments/caches/hash_cache.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/src/deadline/job_attachments/caches/s3_check_cache.py` & `deadline-0.48.1/src/deadline/job_attachments/caches/s3_check_cache.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/LICENSE` & `deadline-0.48.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/README.md` & `deadline-0.48.1/README.md`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/hatch.toml` & `deadline-0.48.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/pyproject.toml` & `deadline-0.48.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadline-0.48.0/PKG-INFO` & `deadline-0.48.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline
-Version: 0.48.0
+Version: 0.48.1
 Summary: Multi-purpose library and command line tool that implements functionality to support applications using AWS Deadline Cloud.
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```

