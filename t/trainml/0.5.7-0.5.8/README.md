# Comparing `tmp/trainml-0.5.7.tar.gz` & `tmp/trainml-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trainml-0.5.7.tar", last modified: Fri Apr 26 21:06:51 2024, max compression
+gzip compressed data, was "trainml-0.5.8.tar", last modified: Mon May  6 15:16:27 2024, max compression
```

## Comparing `trainml-0.5.7.tar` & `trainml-0.5.8.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.385451 trainml-0.5.7/
--rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2021-01-24 17:36:29.000000 trainml-0.5.7/LICENSE
--rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-04-26 21:06:51.385277 trainml-0.5.7/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2021-09-29 15:45:34.000000 trainml-0.5.7/README.md
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.360550 trainml-0.5.7/examples/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-19 16:26:24.000000 trainml-0.5.7/examples/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2023-01-10 21:56:22.000000 trainml-0.5.7/examples/create_dataset_and_training_job.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2023-01-10 21:56:46.000000 trainml-0.5.7/examples/local_storage.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2023-01-22 22:47:55.000000 trainml-0.5.7/examples/training_inference_pipeline.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1037 2024-04-25 14:45:27.000000 trainml-0.5.7/pyproject.toml
--rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-04-26 21:06:51.385497 trainml-0.5.7/setup.cfg
--rw-r--r--   0 akowalsk   (501) staff       (20)     1226 2021-03-31 16:56:30.000000 trainml-0.5.7/setup.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.358546 trainml-0.5.7/tests/
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.363170 trainml-0.5.7/tests/integration/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:47.000000 trainml-0.5.7/tests/integration/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.363501 trainml-0.5.7/tests/integration/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-19 19:22:07.000000 trainml-0.5.7/tests/integration/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2023-06-19 19:31:30.000000 trainml-0.5.7/tests/integration/cloudbender/test_providers_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2021-06-23 16:25:57.000000 trainml-0.5.7/tests/integration/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-03-14 16:09:32.000000 trainml-0.5.7/tests/integration/test_checkpoints_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-03-19 18:31:45.000000 trainml-0.5.7/tests/integration/test_datasets_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2023-03-20 21:29:08.000000 trainml-0.5.7/tests/integration/test_environments_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2023-03-20 21:29:14.000000 trainml-0.5.7/tests/integration/test_gpu_types_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    25117 2024-04-17 17:22:21.000000 trainml-0.5.7/tests/integration/test_jobs_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-03-14 16:09:23.000000 trainml-0.5.7/tests/integration/test_models_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-02-29 23:09:06.000000 trainml-0.5.7/tests/integration/test_projects_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-02 13:07:27.000000 trainml-0.5.7/tests/integration/test_volumes_integration.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.367043 trainml-0.5.7/tests/unit/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:48.000000 trainml-0.5.7/tests/unit/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.369351 trainml-0.5.7/tests/unit/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-03-11 02:10:08.000000 trainml-0.5.7/tests/unit/cli/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.370814 trainml-0.5.7/tests/unit/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-21 01:22:34.000000 trainml-0.5.7/tests/unit/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2023-06-22 02:19:34.000000 trainml-0.5.7/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2023-06-23 19:47:44.000000 trainml-0.5.7/tests/unit/cli/cloudbender/test_cli_device_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2023-06-21 02:49:51.000000 trainml-0.5.7/tests/unit/cli/cloudbender/test_cli_node_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      781 2023-06-21 01:49:51.000000 trainml-0.5.7/tests/unit/cli/cloudbender/test_cli_provider_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2023-06-21 02:10:35.000000 trainml-0.5.7/tests/unit/cli/cloudbender/test_cli_region_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1311 2024-04-26 20:42:13.000000 trainml-0.5.7/tests/unit/cli/cloudbender/test_cli_service_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      236 2021-03-11 02:43:04.000000 trainml-0.5.7/tests/unit/cli/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      702 2023-06-22 01:39:48.000000 trainml-0.5.7/tests/unit/cli/test_cli_checkpoint_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      653 2023-06-22 01:40:30.000000 trainml-0.5.7/tests/unit/cli/test_cli_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      683 2023-06-21 00:35:39.000000 trainml-0.5.7/tests/unit/cli/test_cli_environment_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      650 2023-06-21 00:36:29.000000 trainml-0.5.7/tests/unit/cli/test_cli_gpu_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      611 2023-06-22 01:49:26.000000 trainml-0.5.7/tests/unit/cli/test_cli_job_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      629 2023-06-22 01:42:02.000000 trainml-0.5.7/tests/unit/cli/test_cli_model_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1688 2024-04-09 16:44:25.000000 trainml-0.5.7/tests/unit/cli/test_cli_project_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-03-12 15:29:44.000000 trainml-0.5.7/tests/unit/cli/test_cli_volume_unit.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.373062 trainml-0.5.7/tests/unit/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-16 16:46:40.000000 trainml-0.5.7/tests/unit/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5783 2024-04-26 20:39:34.000000 trainml-0.5.7/tests/unit/cloudbender/test_data_connectors_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2023-06-23 16:49:35.000000 trainml-0.5.7/tests/unit/cloudbender/test_datastores_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2023-06-23 16:50:27.000000 trainml-0.5.7/tests/unit/cloudbender/test_device_configs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2023-06-23 19:46:10.000000 trainml-0.5.7/tests/unit/cloudbender/test_devices_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2023-06-23 16:51:45.000000 trainml-0.5.7/tests/unit/cloudbender/test_nodes_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2023-06-23 16:52:25.000000 trainml-0.5.7/tests/unit/cloudbender/test_providers_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2023-06-23 16:53:15.000000 trainml-0.5.7/tests/unit/cloudbender/test_regions_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5220 2024-04-26 20:39:32.000000 trainml-0.5.7/tests/unit/cloudbender/test_services_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    31129 2024-04-09 16:44:31.000000 trainml-0.5.7/tests/unit/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      858 2023-07-27 15:10:38.000000 trainml-0.5.7/tests/unit/test_auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2023-03-31 21:38:18.000000 trainml-0.5.7/tests/unit/test_checkpoints_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2023-01-10 22:45:55.000000 trainml-0.5.7/tests/unit/test_connections_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2023-03-31 21:39:46.000000 trainml-0.5.7/tests/unit/test_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2023-06-04 18:32:37.000000 trainml-0.5.7/tests/unit/test_environments_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      906 2021-03-11 02:25:50.000000 trainml-0.5.7/tests/unit/test_exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2023-06-21 20:53:31.000000 trainml-0.5.7/tests/unit/test_gpu_types_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2023-06-04 18:29:09.000000 trainml-0.5.7/tests/unit/test_jobs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2023-03-31 21:39:17.000000 trainml-0.5.7/tests/unit/test_models_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10743 2024-04-18 15:31:37.000000 trainml-0.5.7/tests/unit/test_projects_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2021-03-11 02:26:10.000000 trainml-0.5.7/tests/unit/test_trainml.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-03-12 17:51:37.000000 trainml-0.5.7/tests/unit/test_volumes_unit.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.376755 trainml-0.5.7/trainml/
--rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-04-26 21:05:52.000000 trainml-0.5.7/trainml/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)       59 2021-02-24 01:47:01.000000 trainml-0.5.7/trainml/__main__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2023-09-08 15:42:01.000000 trainml-0.5.7/trainml/auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8430 2024-04-17 13:05:41.000000 trainml-0.5.7/trainml/checkpoints.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.379665 trainml-0.5.7/trainml/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-02-29 19:03:52.000000 trainml-0.5.7/trainml/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2023-06-19 19:34:08.000000 trainml-0.5.7/trainml/cli/checkpoint.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.381590 trainml-0.5.7/trainml/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)      592 2024-04-18 15:45:19.000000 trainml-0.5.7/trainml/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3606 2024-04-18 15:45:08.000000 trainml-0.5.7/trainml/cli/cloudbender/data_connector.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2023-06-22 02:11:56.000000 trainml-0.5.7/trainml/cli/cloudbender/datastore.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2023-06-25 18:44:34.000000 trainml-0.5.7/trainml/cli/cloudbender/device.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2023-06-22 02:09:01.000000 trainml-0.5.7/trainml/cli/cloudbender/node.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2023-06-22 02:09:04.000000 trainml-0.5.7/trainml/cli/cloudbender/provider.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2023-06-22 02:09:07.000000 trainml-0.5.7/trainml/cli/cloudbender/region.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3147 2024-04-26 20:42:25.000000 trainml-0.5.7/trainml/cli/cloudbender/service.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2023-06-19 19:34:11.000000 trainml-0.5.7/trainml/cli/connection.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-02-08 17:04:38.000000 trainml-0.5.7/trainml/cli/dataset.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2023-06-19 19:34:12.000000 trainml-0.5.7/trainml/cli/environment.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      883 2023-06-19 19:40:03.000000 trainml-0.5.7/trainml/cli/gpu.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.382152 trainml-0.5.7/trainml/cli/job/
--rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2023-06-19 19:34:17.000000 trainml-0.5.7/trainml/cli/job/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-02-14 15:58:34.000000 trainml-0.5.7/trainml/cli/job/create.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2023-09-08 19:00:58.000000 trainml-0.5.7/trainml/cli/model.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3314 2024-04-09 16:42:40.000000 trainml-0.5.7/trainml/cli/project.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-03-12 17:50:39.000000 trainml-0.5.7/trainml/cli/volume.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.384846 trainml-0.5.7/trainml/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)       64 2023-06-16 13:41:42.000000 trainml-0.5.7/trainml/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      717 2024-04-18 15:13:53.000000 trainml-0.5.7/trainml/cloudbender/cloudbender.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3297 2024-04-18 15:41:18.000000 trainml-0.5.7/trainml/cloudbender/data_connectors.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2023-06-23 16:22:15.000000 trainml-0.5.7/trainml/cloudbender/datastores.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2023-06-23 16:22:25.000000 trainml-0.5.7/trainml/cloudbender/device_configs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2023-06-23 16:28:32.000000 trainml-0.5.7/trainml/cloudbender/devices.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2023-06-23 16:25:10.000000 trainml-0.5.7/trainml/cloudbender/nodes.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2023-06-23 16:22:51.000000 trainml-0.5.7/trainml/cloudbender/providers.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2023-06-23 16:23:07.000000 trainml-0.5.7/trainml/cloudbender/regions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5126 2024-04-26 20:45:18.000000 trainml-0.5.7/trainml/cloudbender/services.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    20029 2023-09-08 19:03:44.000000 trainml-0.5.7/trainml/connections.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8249 2024-04-17 13:05:14.000000 trainml-0.5.7/trainml/datasets.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2023-06-21 20:39:07.000000 trainml-0.5.7/trainml/environments.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-02-29 19:05:24.000000 trainml-0.5.7/trainml/exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2023-06-23 15:24:57.000000 trainml-0.5.7/trainml/gpu_types.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    18056 2024-04-17 17:23:52.000000 trainml-0.5.7/trainml/jobs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7961 2024-04-17 13:06:47.000000 trainml-0.5.7/trainml/models.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6585 2024-04-19 18:45:25.000000 trainml-0.5.7/trainml/projects.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-02-29 19:06:10.000000 trainml-0.5.7/trainml/trainml.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8312 2024-04-17 13:07:00.000000 trainml-0.5.7/trainml/volumes.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:51.377602 trainml-0.5.7/trainml.egg-info/
--rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-04-26 21:06:51.000000 trainml-0.5.7/trainml.egg-info/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     3619 2024-04-26 21:06:51.000000 trainml-0.5.7/trainml.egg-info/SOURCES.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-04-26 21:06:51.000000 trainml-0.5.7/trainml.egg-info/dependency_links.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-04-26 21:06:51.000000 trainml-0.5.7/trainml.egg-info/entry_points.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-04-26 21:06:51.000000 trainml-0.5.7/trainml.egg-info/requires.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-04-26 21:06:51.000000 trainml-0.5.7/trainml.egg-info/top_level.txt
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.248930 trainml-0.5.8/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2021-01-24 17:36:29.000000 trainml-0.5.8/LICENSE
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-05-06 15:16:27.248795 trainml-0.5.8/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2021-09-29 15:45:34.000000 trainml-0.5.8/README.md
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.225520 trainml-0.5.8/examples/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-19 16:26:24.000000 trainml-0.5.8/examples/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2023-01-10 21:56:22.000000 trainml-0.5.8/examples/create_dataset_and_training_job.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2023-01-10 21:56:46.000000 trainml-0.5.8/examples/local_storage.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2023-01-22 22:47:55.000000 trainml-0.5.8/examples/training_inference_pipeline.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1037 2024-04-25 14:45:27.000000 trainml-0.5.8/pyproject.toml
+-rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-05-06 15:16:27.248976 trainml-0.5.8/setup.cfg
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1226 2021-03-31 16:56:30.000000 trainml-0.5.8/setup.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.223562 trainml-0.5.8/tests/
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.227768 trainml-0.5.8/tests/integration/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:47.000000 trainml-0.5.8/tests/integration/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.228102 trainml-0.5.8/tests/integration/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-19 19:22:07.000000 trainml-0.5.8/tests/integration/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2023-06-19 19:31:30.000000 trainml-0.5.8/tests/integration/cloudbender/test_providers_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2021-06-23 16:25:57.000000 trainml-0.5.8/tests/integration/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-03-14 16:09:32.000000 trainml-0.5.8/tests/integration/test_checkpoints_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-03-19 18:31:45.000000 trainml-0.5.8/tests/integration/test_datasets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2023-03-20 21:29:08.000000 trainml-0.5.8/tests/integration/test_environments_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2023-03-20 21:29:14.000000 trainml-0.5.8/tests/integration/test_gpu_types_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    25117 2024-04-17 17:22:21.000000 trainml-0.5.8/tests/integration/test_jobs_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-03-14 16:09:23.000000 trainml-0.5.8/tests/integration/test_models_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-02-29 23:09:06.000000 trainml-0.5.8/tests/integration/test_projects_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-02 13:07:27.000000 trainml-0.5.8/tests/integration/test_volumes_integration.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.231650 trainml-0.5.8/tests/unit/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:48.000000 trainml-0.5.8/tests/unit/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.233985 trainml-0.5.8/tests/unit/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-03-11 02:10:08.000000 trainml-0.5.8/tests/unit/cli/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.235355 trainml-0.5.8/tests/unit/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-21 01:22:34.000000 trainml-0.5.8/tests/unit/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2023-06-22 02:19:34.000000 trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2023-06-23 19:47:44.000000 trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_device_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2023-06-21 02:49:51.000000 trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_node_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      781 2023-06-21 01:49:51.000000 trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_provider_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2023-06-21 02:10:35.000000 trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_region_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1311 2024-04-26 20:42:13.000000 trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_service_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      236 2021-03-11 02:43:04.000000 trainml-0.5.8/tests/unit/cli/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      702 2023-06-22 01:39:48.000000 trainml-0.5.8/tests/unit/cli/test_cli_checkpoint_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      653 2023-06-22 01:40:30.000000 trainml-0.5.8/tests/unit/cli/test_cli_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      683 2023-06-21 00:35:39.000000 trainml-0.5.8/tests/unit/cli/test_cli_environment_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      650 2023-06-21 00:36:29.000000 trainml-0.5.8/tests/unit/cli/test_cli_gpu_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      611 2023-06-22 01:49:26.000000 trainml-0.5.8/tests/unit/cli/test_cli_job_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      629 2023-06-22 01:42:02.000000 trainml-0.5.8/tests/unit/cli/test_cli_model_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1688 2024-04-09 16:44:25.000000 trainml-0.5.8/tests/unit/cli/test_cli_project_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-03-12 15:29:44.000000 trainml-0.5.8/tests/unit/cli/test_cli_volume_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.237360 trainml-0.5.8/tests/unit/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-16 16:46:40.000000 trainml-0.5.8/tests/unit/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5783 2024-04-26 20:39:34.000000 trainml-0.5.8/tests/unit/cloudbender/test_data_connectors_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2023-06-23 16:49:35.000000 trainml-0.5.8/tests/unit/cloudbender/test_datastores_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2023-06-23 16:50:27.000000 trainml-0.5.8/tests/unit/cloudbender/test_device_configs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2023-06-23 19:46:10.000000 trainml-0.5.8/tests/unit/cloudbender/test_devices_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2023-06-23 16:51:45.000000 trainml-0.5.8/tests/unit/cloudbender/test_nodes_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2023-06-23 16:52:25.000000 trainml-0.5.8/tests/unit/cloudbender/test_providers_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2023-06-23 16:53:15.000000 trainml-0.5.8/tests/unit/cloudbender/test_regions_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5220 2024-04-26 20:39:32.000000 trainml-0.5.8/tests/unit/cloudbender/test_services_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    31129 2024-04-09 16:44:31.000000 trainml-0.5.8/tests/unit/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      858 2023-07-27 15:10:38.000000 trainml-0.5.8/tests/unit/test_auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2023-03-31 21:38:18.000000 trainml-0.5.8/tests/unit/test_checkpoints_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2023-01-10 22:45:55.000000 trainml-0.5.8/tests/unit/test_connections_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2023-03-31 21:39:46.000000 trainml-0.5.8/tests/unit/test_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2023-06-04 18:32:37.000000 trainml-0.5.8/tests/unit/test_environments_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      906 2021-03-11 02:25:50.000000 trainml-0.5.8/tests/unit/test_exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2023-06-21 20:53:31.000000 trainml-0.5.8/tests/unit/test_gpu_types_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2023-06-04 18:29:09.000000 trainml-0.5.8/tests/unit/test_jobs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2023-03-31 21:39:17.000000 trainml-0.5.8/tests/unit/test_models_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10743 2024-04-18 15:31:37.000000 trainml-0.5.8/tests/unit/test_projects_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2021-03-11 02:26:10.000000 trainml-0.5.8/tests/unit/test_trainml.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-03-12 17:51:37.000000 trainml-0.5.8/tests/unit/test_volumes_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.240842 trainml-0.5.8/trainml/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-05-06 15:15:01.000000 trainml-0.5.8/trainml/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)       59 2021-02-24 01:47:01.000000 trainml-0.5.8/trainml/__main__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2023-09-08 15:42:01.000000 trainml-0.5.8/trainml/auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8667 2024-05-05 19:36:12.000000 trainml-0.5.8/trainml/checkpoints.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.243653 trainml-0.5.8/trainml/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-02-29 19:03:52.000000 trainml-0.5.8/trainml/cli/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2023-06-19 19:34:08.000000 trainml-0.5.8/trainml/cli/checkpoint.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.245534 trainml-0.5.8/trainml/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      592 2024-04-18 15:45:19.000000 trainml-0.5.8/trainml/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3606 2024-04-18 15:45:08.000000 trainml-0.5.8/trainml/cli/cloudbender/data_connector.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2023-06-22 02:11:56.000000 trainml-0.5.8/trainml/cli/cloudbender/datastore.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2023-06-25 18:44:34.000000 trainml-0.5.8/trainml/cli/cloudbender/device.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2023-06-22 02:09:01.000000 trainml-0.5.8/trainml/cli/cloudbender/node.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2023-06-22 02:09:04.000000 trainml-0.5.8/trainml/cli/cloudbender/provider.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2023-06-22 02:09:07.000000 trainml-0.5.8/trainml/cli/cloudbender/region.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3147 2024-04-26 20:42:25.000000 trainml-0.5.8/trainml/cli/cloudbender/service.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2023-06-19 19:34:11.000000 trainml-0.5.8/trainml/cli/connection.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-02-08 17:04:38.000000 trainml-0.5.8/trainml/cli/dataset.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2023-06-19 19:34:12.000000 trainml-0.5.8/trainml/cli/environment.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      883 2023-06-19 19:40:03.000000 trainml-0.5.8/trainml/cli/gpu.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.246001 trainml-0.5.8/trainml/cli/job/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2023-06-19 19:34:17.000000 trainml-0.5.8/trainml/cli/job/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-02-14 15:58:34.000000 trainml-0.5.8/trainml/cli/job/create.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2023-09-08 19:00:58.000000 trainml-0.5.8/trainml/cli/model.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3314 2024-04-09 16:42:40.000000 trainml-0.5.8/trainml/cli/project.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-03-12 17:50:39.000000 trainml-0.5.8/trainml/cli/volume.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.248475 trainml-0.5.8/trainml/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)       64 2023-06-16 13:41:42.000000 trainml-0.5.8/trainml/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      717 2024-04-18 15:13:53.000000 trainml-0.5.8/trainml/cloudbender/cloudbender.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3297 2024-04-18 15:41:18.000000 trainml-0.5.8/trainml/cloudbender/data_connectors.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2023-06-23 16:22:15.000000 trainml-0.5.8/trainml/cloudbender/datastores.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2023-06-23 16:22:25.000000 trainml-0.5.8/trainml/cloudbender/device_configs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2023-06-23 16:28:32.000000 trainml-0.5.8/trainml/cloudbender/devices.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2023-06-23 16:25:10.000000 trainml-0.5.8/trainml/cloudbender/nodes.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2023-06-23 16:22:51.000000 trainml-0.5.8/trainml/cloudbender/providers.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2023-06-23 16:23:07.000000 trainml-0.5.8/trainml/cloudbender/regions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5126 2024-04-26 20:45:18.000000 trainml-0.5.8/trainml/cloudbender/services.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    20029 2023-09-08 19:03:44.000000 trainml-0.5.8/trainml/connections.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8477 2024-05-05 19:36:10.000000 trainml-0.5.8/trainml/datasets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2023-06-21 20:39:07.000000 trainml-0.5.8/trainml/environments.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-02-29 19:05:24.000000 trainml-0.5.8/trainml/exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2023-06-23 15:24:57.000000 trainml-0.5.8/trainml/gpu_types.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    18056 2024-04-17 17:23:52.000000 trainml-0.5.8/trainml/jobs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8161 2024-05-05 19:36:16.000000 trainml-0.5.8/trainml/models.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6585 2024-04-19 18:45:25.000000 trainml-0.5.8/trainml/projects.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-02-29 19:06:10.000000 trainml-0.5.8/trainml/trainml.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8312 2024-04-17 13:07:00.000000 trainml-0.5.8/trainml/volumes.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:27.241720 trainml-0.5.8/trainml.egg-info/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-05-06 15:16:27.000000 trainml-0.5.8/trainml.egg-info/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3619 2024-05-06 15:16:27.000000 trainml-0.5.8/trainml.egg-info/SOURCES.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-05-06 15:16:27.000000 trainml-0.5.8/trainml.egg-info/dependency_links.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-05-06 15:16:27.000000 trainml-0.5.8/trainml.egg-info/entry_points.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-05-06 15:16:27.000000 trainml-0.5.8/trainml.egg-info/requires.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-05-06 15:16:27.000000 trainml-0.5.8/trainml.egg-info/top_level.txt
```

### Comparing `trainml-0.5.7/LICENSE` & `trainml-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/PKG-INFO` & `trainml-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainml
-Version: 0.5.7
+Version: 0.5.8
 Summary: trainML client SDK and command line utilities
 Home-page: https://github.com/trainML/trainml-cli
 Author: trainML
 Author-email: support@trainml.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.trainml.ai/"><img src="https://www.trainml.ai/static/img/trainML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trainml Version: 0.5.7 Summary: trainML client SDK
+Metadata-Version: 2.1 Name: trainml Version: 0.5.8 Summary: trainML client SDK
 and command line utilities Home-page: https://github.com/trainML/trainml-cli
 Author: trainML Author-email: support@trainml.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._t_r_a_i_n_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_t_r_a_i_n_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # trainML Python SDK and Command Line Tools Provides programmatic access to
 [trainML platform](https://app.trainml.ai). ## Installation Python 3.8 or above
 is required. ``` pip install trainml ``` ## Authentication ### Prerequisites
 You must have a valid [trainML account](https://app.trainml.ai). On the
```

### Comparing `trainml-0.5.7/README.md` & `trainml-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/examples/create_dataset_and_training_job.py` & `trainml-0.5.8/examples/create_dataset_and_training_job.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/examples/local_storage.py` & `trainml-0.5.8/examples/local_storage.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/examples/training_inference_pipeline.py` & `trainml-0.5.8/examples/training_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/pyproject.toml` & `trainml-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/setup.py` & `trainml-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/integration/cloudbender/test_providers_integration.py` & `trainml-0.5.8/tests/integration/cloudbender/test_providers_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/integration/conftest.py` & `trainml-0.5.8/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/integration/test_checkpoints_integration.py` & `trainml-0.5.8/tests/integration/test_checkpoints_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/integration/test_datasets_integration.py` & `trainml-0.5.8/tests/integration/test_datasets_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/integration/test_environments_integration.py` & `trainml-0.5.8/tests/integration/test_environments_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/integration/test_gpu_types_integration.py` & `trainml-0.5.8/tests/integration/test_gpu_types_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/integration/test_jobs_integration.py` & `trainml-0.5.8/tests/integration/test_jobs_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/integration/test_models_integration.py` & `trainml-0.5.8/tests/integration/test_models_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/integration/test_projects_integration.py` & `trainml-0.5.8/tests/integration/test_projects_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/integration/test_volumes_integration.py` & `trainml-0.5.8/tests/integration/test_volumes_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/cloudbender/test_cli_datastore_unit.py` & `trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_datastore_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/cloudbender/test_cli_device_unit.py` & `trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_device_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/cloudbender/test_cli_node_unit.py` & `trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_node_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/cloudbender/test_cli_provider_unit.py` & `trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_provider_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/cloudbender/test_cli_region_unit.py` & `trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_region_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/cloudbender/test_cli_service_unit.py` & `trainml-0.5.8/tests/unit/cli/cloudbender/test_cli_service_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/test_cli_checkpoint_unit.py` & `trainml-0.5.8/tests/unit/cli/test_cli_checkpoint_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/test_cli_datasets_unit.py` & `trainml-0.5.8/tests/unit/cli/test_cli_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/test_cli_environment_unit.py` & `trainml-0.5.8/tests/unit/cli/test_cli_environment_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/test_cli_gpu_unit.py` & `trainml-0.5.8/tests/unit/cli/test_cli_gpu_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/test_cli_job_unit.py` & `trainml-0.5.8/tests/unit/cli/test_cli_job_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/test_cli_model_unit.py` & `trainml-0.5.8/tests/unit/cli/test_cli_model_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/test_cli_project_unit.py` & `trainml-0.5.8/tests/unit/cli/test_cli_project_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cli/test_cli_volume_unit.py` & `trainml-0.5.8/tests/unit/cli/test_cli_volume_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cloudbender/test_data_connectors_unit.py` & `trainml-0.5.8/tests/unit/cloudbender/test_data_connectors_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cloudbender/test_datastores_unit.py` & `trainml-0.5.8/tests/unit/cloudbender/test_datastores_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cloudbender/test_device_configs_unit.py` & `trainml-0.5.8/tests/unit/cloudbender/test_device_configs_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cloudbender/test_devices_unit.py` & `trainml-0.5.8/tests/unit/cloudbender/test_devices_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cloudbender/test_nodes_unit.py` & `trainml-0.5.8/tests/unit/cloudbender/test_nodes_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cloudbender/test_providers_unit.py` & `trainml-0.5.8/tests/unit/cloudbender/test_providers_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cloudbender/test_regions_unit.py` & `trainml-0.5.8/tests/unit/cloudbender/test_regions_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/cloudbender/test_services_unit.py` & `trainml-0.5.8/tests/unit/cloudbender/test_services_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/conftest.py` & `trainml-0.5.8/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/test_auth.py` & `trainml-0.5.8/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/test_checkpoints_unit.py` & `trainml-0.5.8/tests/unit/test_checkpoints_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/test_connections_unit.py` & `trainml-0.5.8/tests/unit/test_connections_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/test_datasets_unit.py` & `trainml-0.5.8/tests/unit/test_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/test_environments_unit.py` & `trainml-0.5.8/tests/unit/test_environments_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/test_exceptions.py` & `trainml-0.5.8/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/test_gpu_types_unit.py` & `trainml-0.5.8/tests/unit/test_gpu_types_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/test_jobs_unit.py` & `trainml-0.5.8/tests/unit/test_jobs_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/test_models_unit.py` & `trainml-0.5.8/tests/unit/test_models_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/test_projects_unit.py` & `trainml-0.5.8/tests/unit/test_projects_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/test_trainml.py` & `trainml-0.5.8/tests/unit/test_trainml.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/tests/unit/test_volumes_unit.py` & `trainml-0.5.8/tests/unit/test_volumes_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/auth.py` & `trainml-0.5.8/trainml/auth.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/checkpoints.py` & `trainml-0.5.8/trainml/checkpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 class Checkpoint:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
         self._checkpoint = kwargs
         self._id = self._checkpoint.get("id", self._checkpoint.get("checkpoint_uuid"))
         self._status = self._checkpoint.get("status")
         self._name = self._checkpoint.get("name")
-        self._size = self._checkpoint.get("size")
+        self._size = self._checkpoint.get("size") or self._checkpoint.get("used_size")
+        self._billed_size = self._checkpoint.get("billed_size") or self._checkpoint.get(
+            "size"
+        )
         self._project_uuid = self._checkpoint.get("project_uuid")
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
@@ -75,14 +78,18 @@
     def name(self) -> str:
         return self._name
 
     @property
     def size(self) -> int:
         return self._size
 
+    @property
+    def billed_size(self) -> int:
+        return self._billed_size
+
     def __str__(self):
         return json.dumps({k: v for k, v in self._checkpoint.items()})
 
     def __repr__(self):
         return f"Checkpoint( trainml , **{self._checkpoint.__repr__()})"
 
     def __bool__(self):
```

### Comparing `trainml-0.5.7/trainml/cli/__init__.py` & `trainml-0.5.8/trainml/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/checkpoint.py` & `trainml-0.5.8/trainml/cli/checkpoint.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/cloudbender/__init__.py` & `trainml-0.5.8/trainml/cli/cloudbender/__init__.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/cloudbender/data_connector.py` & `trainml-0.5.8/trainml/cli/cloudbender/data_connector.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/cloudbender/datastore.py` & `trainml-0.5.8/trainml/cli/cloudbender/datastore.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/cloudbender/device.py` & `trainml-0.5.8/trainml/cli/cloudbender/device.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/cloudbender/node.py` & `trainml-0.5.8/trainml/cli/cloudbender/node.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/cloudbender/provider.py` & `trainml-0.5.8/trainml/cli/cloudbender/provider.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/cloudbender/region.py` & `trainml-0.5.8/trainml/cli/cloudbender/region.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/cloudbender/service.py` & `trainml-0.5.8/trainml/cli/cloudbender/service.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/connection.py` & `trainml-0.5.8/trainml/cli/connection.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/dataset.py` & `trainml-0.5.8/trainml/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/environment.py` & `trainml-0.5.8/trainml/cli/environment.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/gpu.py` & `trainml-0.5.8/trainml/cli/gpu.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/job/__init__.py` & `trainml-0.5.8/trainml/cli/job/__init__.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/job/create.py` & `trainml-0.5.8/trainml/cli/job/create.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/model.py` & `trainml-0.5.8/trainml/cli/model.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/project.py` & `trainml-0.5.8/trainml/cli/project.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cli/volume.py` & `trainml-0.5.8/trainml/cli/volume.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cloudbender/cloudbender.py` & `trainml-0.5.8/trainml/cloudbender/cloudbender.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cloudbender/data_connectors.py` & `trainml-0.5.8/trainml/cloudbender/data_connectors.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cloudbender/datastores.py` & `trainml-0.5.8/trainml/cloudbender/datastores.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cloudbender/device_configs.py` & `trainml-0.5.8/trainml/cloudbender/device_configs.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cloudbender/devices.py` & `trainml-0.5.8/trainml/cloudbender/devices.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cloudbender/nodes.py` & `trainml-0.5.8/trainml/cloudbender/nodes.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cloudbender/providers.py` & `trainml-0.5.8/trainml/cloudbender/providers.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cloudbender/regions.py` & `trainml-0.5.8/trainml/cloudbender/regions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/cloudbender/services.py` & `trainml-0.5.8/trainml/cloudbender/services.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/connections.py` & `trainml-0.5.8/trainml/connections.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/datasets.py` & `trainml-0.5.8/trainml/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 class Dataset:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
         self._dataset = kwargs
         self._id = self._dataset.get("id", self._dataset.get("dataset_uuid"))
         self._status = self._dataset.get("status")
         self._name = self._dataset.get("name")
-        self._size = self._dataset.get("size")
+        self._size = self._dataset.get("size") or self._dataset.get("used_size")
+        self._billed_size = self._dataset.get("billed_size") or self._dataset.get(
+            "size"
+        )
         self._project_uuid = self._dataset.get("project_uuid")
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
@@ -75,14 +78,18 @@
     def name(self) -> str:
         return self._name
 
     @property
     def size(self) -> int:
         return self._size or 0
 
+    @property
+    def billed_size(self) -> int:
+        return self._billed_size
+
     def __str__(self):
         return json.dumps({k: v for k, v in self._dataset.items()})
 
     def __repr__(self):
         return f"Dataset( trainml , **{self._dataset.__repr__()})"
 
     def __bool__(self):
```

### Comparing `trainml-0.5.7/trainml/environments.py` & `trainml-0.5.8/trainml/environments.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/exceptions.py` & `trainml-0.5.8/trainml/exceptions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/gpu_types.py` & `trainml-0.5.8/trainml/gpu_types.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/jobs.py` & `trainml-0.5.8/trainml/jobs.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/models.py` & `trainml-0.5.8/trainml/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 class Model:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
         self._model = kwargs
         self._id = self._model.get("id", self._model.get("model_uuid"))
         self._status = self._model.get("status")
         self._name = self._model.get("name")
-        self._size = self._model.get("size")
+        self._size = self._model.get("size") or self._model.get("used_size")
+        self._billed_size = self._model.get("billed_size") or self._model.get("size")
         self._project_uuid = self._model.get("project_uuid")
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
@@ -68,14 +69,18 @@
     def name(self) -> str:
         return self._name
 
     @property
     def size(self) -> int:
         return self._size
 
+    @property
+    def billed_size(self) -> int:
+        return self._billed_size
+
     def __str__(self):
         return json.dumps({k: v for k, v in self._model.items()})
 
     def __repr__(self):
         return f"Model( trainml , **{self._model.__repr__()})"
 
     def __bool__(self):
```

### Comparing `trainml-0.5.7/trainml/projects.py` & `trainml-0.5.8/trainml/projects.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/trainml.py` & `trainml-0.5.8/trainml/trainml.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml/volumes.py` & `trainml-0.5.8/trainml/volumes.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.7/trainml.egg-info/PKG-INFO` & `trainml-0.5.8/trainml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainml
-Version: 0.5.7
+Version: 0.5.8
 Summary: trainML client SDK and command line utilities
 Home-page: https://github.com/trainML/trainml-cli
 Author: trainML
 Author-email: support@trainml.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.trainml.ai/"><img src="https://www.trainml.ai/static/img/trainML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trainml Version: 0.5.7 Summary: trainML client SDK
+Metadata-Version: 2.1 Name: trainml Version: 0.5.8 Summary: trainML client SDK
 and command line utilities Home-page: https://github.com/trainML/trainml-cli
 Author: trainML Author-email: support@trainml.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._t_r_a_i_n_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_t_r_a_i_n_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # trainML Python SDK and Command Line Tools Provides programmatic access to
 [trainML platform](https://app.trainml.ai). ## Installation Python 3.8 or above
 is required. ``` pip install trainml ``` ## Authentication ### Prerequisites
 You must have a valid [trainML account](https://app.trainml.ai). On the
```

### Comparing `trainml-0.5.7/trainml.egg-info/SOURCES.txt` & `trainml-0.5.8/trainml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

