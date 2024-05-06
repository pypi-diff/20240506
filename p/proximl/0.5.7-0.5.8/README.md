# Comparing `tmp/proximl-0.5.7.tar.gz` & `tmp/proximl-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proximl-0.5.7.tar", last modified: Fri Apr 26 21:07:09 2024, max compression
+gzip compressed data, was "proximl-0.5.8.tar", last modified: Mon May  6 15:16:30 2024, max compression
```

## Comparing `proximl-0.5.7.tar` & `proximl-0.5.8.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.794194 proximl-0.5.7/
--rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2024-04-26 21:06:15.000000 proximl-0.5.7/LICENSE
--rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-04-26 21:07:09.794030 proximl-0.5.7/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2024-04-26 21:06:15.000000 proximl-0.5.7/README.md
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.771521 proximl-0.5.7/examples/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/examples/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2024-04-26 21:06:15.000000 proximl-0.5.7/examples/create_dataset_and_training_job.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2024-04-26 21:06:15.000000 proximl-0.5.7/examples/local_storage.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2024-04-26 21:06:15.000000 proximl-0.5.7/examples/training_inference_pipeline.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.775450 proximl-0.5.7/proximl/
--rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)       59 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/__main__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8430 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/checkpoints.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.778289 proximl-0.5.7/proximl/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/checkpoint.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.780049 proximl-0.5.7/proximl/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)      592 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3606 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/data_connector.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/datastore.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/device.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/node.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/provider.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/region.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3147 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/cloudbender/service.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/connection.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/dataset.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/environment.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      883 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/gpu.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.780475 proximl-0.5.7/proximl/cli/job/
--rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/job/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/job/create.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/model.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3314 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/project.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cli/volume.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.783110 proximl-0.5.7/proximl/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)       64 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      717 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/cloudbender.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3297 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/data_connectors.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/datastores.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/device_configs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/devices.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/nodes.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/providers.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/regions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5126 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/cloudbender/services.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    20035 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/connections.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8249 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/datasets.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/environments.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/gpu_types.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    18056 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/jobs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7961 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/models.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6585 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/projects.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/proximl.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8312 2024-04-26 21:06:15.000000 proximl-0.5.7/proximl/volumes.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.776254 proximl-0.5.7/proximl.egg-info/
--rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-04-26 21:07:09.000000 proximl-0.5.7/proximl.egg-info/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     3619 2024-04-26 21:07:09.000000 proximl-0.5.7/proximl.egg-info/SOURCES.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-04-26 21:07:09.000000 proximl-0.5.7/proximl.egg-info/dependency_links.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-04-26 21:07:09.000000 proximl-0.5.7/proximl.egg-info/entry_points.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-04-26 21:07:09.000000 proximl-0.5.7/proximl.egg-info/requires.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-04-26 21:07:09.000000 proximl-0.5.7/proximl.egg-info/top_level.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)     1037 2024-04-26 21:06:15.000000 proximl-0.5.7/pyproject.toml
--rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-04-26 21:07:09.794242 proximl-0.5.7/setup.cfg
--rw-r--r--   0 akowalsk   (501) staff       (20)     1225 2024-04-26 21:06:15.000000 proximl-0.5.7/setup.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.769940 proximl-0.5.7/tests/
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.784846 proximl-0.5.7/tests/integration/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.785074 proximl-0.5.7/tests/integration/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/cloudbender/test_providers_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_checkpoints_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_datasets_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_environments_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_gpu_types_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    25117 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_jobs_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_models_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_projects_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/integration/test_volumes_integration.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.788187 proximl-0.5.7/tests/unit/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.790012 proximl-0.5.7/tests/unit/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.791510 proximl-0.5.7/tests/unit/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_device_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_node_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      781 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_provider_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_region_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1311 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_service_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      236 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      702 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_checkpoint_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      653 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      683 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_environment_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      650 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_gpu_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      611 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_job_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      629 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_model_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1688 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_project_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cli/test_cli_volume_unit.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:07:09.793670 proximl-0.5.7/tests/unit/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5783 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_data_connectors_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_datastores_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_device_configs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_devices_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_nodes_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_providers_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_regions_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5220 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/cloudbender/test_services_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    31129 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      858 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_checkpoints_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_connections_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_environments_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      906 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_gpu_types_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_jobs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_models_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10743 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_projects_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_proximl.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-04-26 21:06:15.000000 proximl-0.5.7/tests/unit/test_volumes_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.341098 proximl-0.5.8/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2024-05-06 15:15:25.000000 proximl-0.5.8/LICENSE
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-05-06 15:16:30.340949 proximl-0.5.8/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2024-05-06 15:15:25.000000 proximl-0.5.8/README.md
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.322954 proximl-0.5.8/examples/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/examples/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2024-05-06 15:15:25.000000 proximl-0.5.8/examples/create_dataset_and_training_job.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2024-05-06 15:15:25.000000 proximl-0.5.8/examples/local_storage.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2024-05-06 15:15:25.000000 proximl-0.5.8/examples/training_inference_pipeline.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.326257 proximl-0.5.8/proximl/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)       59 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/__main__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8667 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/checkpoints.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.328879 proximl-0.5.8/proximl/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/checkpoint.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.329991 proximl-0.5.8/proximl/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      592 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3606 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/data_connector.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/datastore.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/device.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/node.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/provider.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/region.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3147 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/service.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/connection.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/dataset.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/environment.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      883 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/gpu.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.330268 proximl-0.5.8/proximl/cli/job/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/job/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/job/create.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/model.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3314 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/project.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/volume.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.331869 proximl-0.5.8/proximl/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)       64 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      717 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/cloudbender.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3297 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/data_connectors.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/datastores.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/device_configs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/devices.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/nodes.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/providers.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/regions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5126 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/services.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    20035 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/connections.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8477 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/datasets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/environments.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/gpu_types.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    18056 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/jobs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8161 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/models.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6585 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/projects.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/proximl.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8312 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/volumes.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.327087 proximl-0.5.8/proximl.egg-info/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-05-06 15:16:30.000000 proximl-0.5.8/proximl.egg-info/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3619 2024-05-06 15:16:30.000000 proximl-0.5.8/proximl.egg-info/SOURCES.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-05-06 15:16:30.000000 proximl-0.5.8/proximl.egg-info/dependency_links.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-05-06 15:16:30.000000 proximl-0.5.8/proximl.egg-info/entry_points.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-05-06 15:16:30.000000 proximl-0.5.8/proximl.egg-info/requires.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-05-06 15:16:30.000000 proximl-0.5.8/proximl.egg-info/top_level.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1037 2024-05-06 15:15:25.000000 proximl-0.5.8/pyproject.toml
+-rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-05-06 15:16:30.341146 proximl-0.5.8/setup.cfg
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1225 2024-05-06 15:15:25.000000 proximl-0.5.8/setup.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.321222 proximl-0.5.8/tests/
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.333292 proximl-0.5.8/tests/integration/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.333549 proximl-0.5.8/tests/integration/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/cloudbender/test_providers_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_checkpoints_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_datasets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_environments_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_gpu_types_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    25117 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_jobs_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_models_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_projects_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_volumes_integration.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.336503 proximl-0.5.8/tests/unit/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.337892 proximl-0.5.8/tests/unit/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.338787 proximl-0.5.8/tests/unit/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_device_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_node_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      781 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_provider_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_region_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1311 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_service_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      236 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      702 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_checkpoint_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      653 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      683 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_environment_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      650 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_gpu_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      611 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_job_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      629 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_model_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1688 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_project_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_volume_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.340722 proximl-0.5.8/tests/unit/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5783 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_data_connectors_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_datastores_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_device_configs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_devices_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_nodes_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_providers_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_regions_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5220 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_services_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    31129 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      858 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_checkpoints_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_connections_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_environments_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      906 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_gpu_types_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_jobs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_models_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10743 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_projects_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_proximl.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_volumes_unit.py
```

### Comparing `proximl-0.5.7/LICENSE` & `proximl-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/PKG-INFO` & `proximl-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proximl
-Version: 0.5.7
+Version: 0.5.8
 Summary: proxiML client SDK and command line utilities
 Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML
 Author-email: support@proximl.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.proximl.ai/"><img src="https://www.proximl.ai/static/img/proxiML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proximl Version: 0.5.7 Summary: proxiML client SDK
+Metadata-Version: 2.1 Name: proximl Version: 0.5.8 Summary: proxiML client SDK
 and command line utilities Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML Author-email: support@proximl.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._p_r_o_x_i_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_p_r_o_x_i_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # proxiML Python SDK and Command Line Tools Provides programmatic access to
 [proxiML platform](https://app.proximl.ai). ## Installation Python 3.8 or above
 is required. ``` pip install proximl ``` ## Authentication ### Prerequisites
 You must have a valid [proxiML account](https://app.proximl.ai). On the
```

### Comparing `proximl-0.5.7/README.md` & `proximl-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/examples/create_dataset_and_training_job.py` & `proximl-0.5.8/examples/create_dataset_and_training_job.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/examples/local_storage.py` & `proximl-0.5.8/examples/local_storage.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/examples/training_inference_pipeline.py` & `proximl-0.5.8/examples/training_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/auth.py` & `proximl-0.5.8/proximl/auth.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/checkpoints.py` & `proximl-0.5.8/proximl/checkpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 class Checkpoint:
     def __init__(self, proximl, **kwargs):
         self.proximl = proximl
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
         return f"Checkpoint( proximl , **{self._checkpoint.__repr__()})"
 
     def __bool__(self):
```

### Comparing `proximl-0.5.7/proximl/cli/__init__.py` & `proximl-0.5.8/proximl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/checkpoint.py` & `proximl-0.5.8/proximl/cli/checkpoint.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/cloudbender/__init__.py` & `proximl-0.5.8/proximl/cli/cloudbender/__init__.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/cloudbender/data_connector.py` & `proximl-0.5.8/proximl/cli/cloudbender/data_connector.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/cloudbender/datastore.py` & `proximl-0.5.8/proximl/cli/cloudbender/datastore.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/cloudbender/device.py` & `proximl-0.5.8/proximl/cli/cloudbender/device.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/cloudbender/node.py` & `proximl-0.5.8/proximl/cli/cloudbender/node.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/cloudbender/provider.py` & `proximl-0.5.8/proximl/cli/cloudbender/provider.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/cloudbender/region.py` & `proximl-0.5.8/proximl/cli/cloudbender/region.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/cloudbender/service.py` & `proximl-0.5.8/proximl/cli/cloudbender/service.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/connection.py` & `proximl-0.5.8/proximl/cli/connection.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/dataset.py` & `proximl-0.5.8/proximl/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/environment.py` & `proximl-0.5.8/proximl/cli/environment.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/gpu.py` & `proximl-0.5.8/proximl/cli/gpu.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/job/__init__.py` & `proximl-0.5.8/proximl/cli/job/__init__.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/job/create.py` & `proximl-0.5.8/proximl/cli/job/create.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/model.py` & `proximl-0.5.8/proximl/cli/model.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/project.py` & `proximl-0.5.8/proximl/cli/project.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cli/volume.py` & `proximl-0.5.8/proximl/cli/volume.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cloudbender/cloudbender.py` & `proximl-0.5.8/proximl/cloudbender/cloudbender.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cloudbender/data_connectors.py` & `proximl-0.5.8/proximl/cloudbender/data_connectors.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cloudbender/datastores.py` & `proximl-0.5.8/proximl/cloudbender/datastores.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cloudbender/device_configs.py` & `proximl-0.5.8/proximl/cloudbender/device_configs.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cloudbender/devices.py` & `proximl-0.5.8/proximl/cloudbender/devices.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cloudbender/nodes.py` & `proximl-0.5.8/proximl/cloudbender/nodes.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cloudbender/providers.py` & `proximl-0.5.8/proximl/cloudbender/providers.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cloudbender/regions.py` & `proximl-0.5.8/proximl/cloudbender/regions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/cloudbender/services.py` & `proximl-0.5.8/proximl/cloudbender/services.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/connections.py` & `proximl-0.5.8/proximl/connections.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/datasets.py` & `proximl-0.5.8/proximl/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 class Dataset:
     def __init__(self, proximl, **kwargs):
         self.proximl = proximl
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
         return f"Dataset( proximl , **{self._dataset.__repr__()})"
 
     def __bool__(self):
```

### Comparing `proximl-0.5.7/proximl/environments.py` & `proximl-0.5.8/proximl/environments.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/exceptions.py` & `proximl-0.5.8/proximl/exceptions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/gpu_types.py` & `proximl-0.5.8/proximl/gpu_types.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/jobs.py` & `proximl-0.5.8/proximl/jobs.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/models.py` & `proximl-0.5.8/proximl/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 class Model:
     def __init__(self, proximl, **kwargs):
         self.proximl = proximl
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
         return f"Model( proximl , **{self._model.__repr__()})"
 
     def __bool__(self):
```

### Comparing `proximl-0.5.7/proximl/projects.py` & `proximl-0.5.8/proximl/projects.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/proximl.py` & `proximl-0.5.8/proximl/proximl.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl/volumes.py` & `proximl-0.5.8/proximl/volumes.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/proximl.egg-info/PKG-INFO` & `proximl-0.5.8/proximl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proximl
-Version: 0.5.7
+Version: 0.5.8
 Summary: proxiML client SDK and command line utilities
 Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML
 Author-email: support@proximl.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.proximl.ai/"><img src="https://www.proximl.ai/static/img/proxiML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proximl Version: 0.5.7 Summary: proxiML client SDK
+Metadata-Version: 2.1 Name: proximl Version: 0.5.8 Summary: proxiML client SDK
 and command line utilities Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML Author-email: support@proximl.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._p_r_o_x_i_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_p_r_o_x_i_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # proxiML Python SDK and Command Line Tools Provides programmatic access to
 [proxiML platform](https://app.proximl.ai). ## Installation Python 3.8 or above
 is required. ``` pip install proximl ``` ## Authentication ### Prerequisites
 You must have a valid [proxiML account](https://app.proximl.ai). On the
```

### Comparing `proximl-0.5.7/proximl.egg-info/SOURCES.txt` & `proximl-0.5.8/proximl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/pyproject.toml` & `proximl-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/setup.py` & `proximl-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/integration/cloudbender/test_providers_integration.py` & `proximl-0.5.8/tests/integration/cloudbender/test_providers_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/integration/conftest.py` & `proximl-0.5.8/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/integration/test_checkpoints_integration.py` & `proximl-0.5.8/tests/integration/test_checkpoints_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/integration/test_datasets_integration.py` & `proximl-0.5.8/tests/integration/test_datasets_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/integration/test_environments_integration.py` & `proximl-0.5.8/tests/integration/test_environments_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/integration/test_gpu_types_integration.py` & `proximl-0.5.8/tests/integration/test_gpu_types_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/integration/test_jobs_integration.py` & `proximl-0.5.8/tests/integration/test_jobs_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/integration/test_models_integration.py` & `proximl-0.5.8/tests/integration/test_models_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/integration/test_projects_integration.py` & `proximl-0.5.8/tests/integration/test_projects_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/integration/test_volumes_integration.py` & `proximl-0.5.8/tests/integration/test_volumes_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_datastore_unit.py` & `proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_datastore_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_device_unit.py` & `proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_device_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_node_unit.py` & `proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_node_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_provider_unit.py` & `proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_provider_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_region_unit.py` & `proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_region_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/cloudbender/test_cli_service_unit.py` & `proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_service_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/test_cli_checkpoint_unit.py` & `proximl-0.5.8/tests/unit/cli/test_cli_checkpoint_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/test_cli_datasets_unit.py` & `proximl-0.5.8/tests/unit/cli/test_cli_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/test_cli_environment_unit.py` & `proximl-0.5.8/tests/unit/cli/test_cli_environment_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/test_cli_gpu_unit.py` & `proximl-0.5.8/tests/unit/cli/test_cli_gpu_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/test_cli_job_unit.py` & `proximl-0.5.8/tests/unit/cli/test_cli_job_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/test_cli_model_unit.py` & `proximl-0.5.8/tests/unit/cli/test_cli_model_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/test_cli_project_unit.py` & `proximl-0.5.8/tests/unit/cli/test_cli_project_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cli/test_cli_volume_unit.py` & `proximl-0.5.8/tests/unit/cli/test_cli_volume_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cloudbender/test_data_connectors_unit.py` & `proximl-0.5.8/tests/unit/cloudbender/test_data_connectors_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cloudbender/test_datastores_unit.py` & `proximl-0.5.8/tests/unit/cloudbender/test_datastores_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cloudbender/test_device_configs_unit.py` & `proximl-0.5.8/tests/unit/cloudbender/test_device_configs_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cloudbender/test_devices_unit.py` & `proximl-0.5.8/tests/unit/cloudbender/test_devices_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cloudbender/test_nodes_unit.py` & `proximl-0.5.8/tests/unit/cloudbender/test_nodes_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cloudbender/test_providers_unit.py` & `proximl-0.5.8/tests/unit/cloudbender/test_providers_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cloudbender/test_regions_unit.py` & `proximl-0.5.8/tests/unit/cloudbender/test_regions_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/cloudbender/test_services_unit.py` & `proximl-0.5.8/tests/unit/cloudbender/test_services_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/conftest.py` & `proximl-0.5.8/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/test_auth.py` & `proximl-0.5.8/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/test_checkpoints_unit.py` & `proximl-0.5.8/tests/unit/test_checkpoints_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/test_connections_unit.py` & `proximl-0.5.8/tests/unit/test_connections_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/test_datasets_unit.py` & `proximl-0.5.8/tests/unit/test_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/test_environments_unit.py` & `proximl-0.5.8/tests/unit/test_environments_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/test_exceptions.py` & `proximl-0.5.8/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/test_gpu_types_unit.py` & `proximl-0.5.8/tests/unit/test_gpu_types_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/test_jobs_unit.py` & `proximl-0.5.8/tests/unit/test_jobs_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/test_models_unit.py` & `proximl-0.5.8/tests/unit/test_models_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/test_projects_unit.py` & `proximl-0.5.8/tests/unit/test_projects_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/test_proximl.py` & `proximl-0.5.8/tests/unit/test_proximl.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.7/tests/unit/test_volumes_unit.py` & `proximl-0.5.8/tests/unit/test_volumes_unit.py`

 * *Files identical despite different names*

