# Comparing `tmp/mantik-0.4.9.tar.gz` & `tmp/mantik-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mantik-0.4.9.tar", max compression
+gzip compressed data, was "mantik-0.5.0.tar", max compression
```

## Comparing `mantik-0.4.9.tar` & `mantik-0.5.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
--rw-r--r--   0        0        0     1092 2024-03-13 12:44:54.087934 mantik-0.4.9/LICENSE
--rw-r--r--   0        0        0     1328 2024-03-13 12:44:54.087934 mantik-0.4.9/README.md
--rw-r--r--   0        0        0      183 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/__init__.py
--rw-r--r--   0        0        0      103 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/authentication/__init__.py
--rw-r--r--   0        0        0     1944 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/authentication/api.py
--rw-r--r--   0        0        0     1813 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/authentication/auth.py
--rw-r--r--   0        0        0     2394 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/authentication/tokens.py
--rw-r--r--   0        0        0      132 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/__init__.py
--rw-r--r--   0        0        0      514 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/_callbacks.py
--rw-r--r--   0        0        0     2864 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/_options.py
--rw-r--r--   0        0        0     1257 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/init.py
--rw-r--r--   0        0        0       95 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/main.py
--rw-r--r--   0        0        0       32 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/models/__init__.py
--rw-r--r--   0        0        0     5891 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/models/models.py
--rw-r--r--   0        0        0      113 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/remote_file_service/__init__.py
--rw-r--r--   0        0        0      343 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/remote_file_service/_arguments.py
--rw-r--r--   0        0        0      743 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/remote_file_service/_options.py
--rw-r--r--   0        0        0     6130 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/remote_file_service/s3_file_service.py
--rw-r--r--   0        0        0     6364 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/remote_file_service/unicore_file_service.py
--rw-r--r--   0        0        0       59 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/runs/__init__.py
--rw-r--r--   0        0        0     1388 2024-03-13 12:44:54.125934 mantik-0.4.9/mantik/cli/runs/_options.py
--rw-r--r--   0        0        0     3407 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/cli/runs/local.py
--rw-r--r--   0        0        0      854 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/cli/runs/runs.py
--rw-r--r--   0        0        0     3384 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/cli/runs/submit.py
--rw-r--r--   0        0        0      887 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/cli/utils.py
--rw-r--r--   0        0        0      116 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/__init__.py
--rw-r--r--   0        0        0     8569 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/client.py
--rw-r--r--   0        0        0      369 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/config/__init__.py
--rw-r--r--   0        0        0     1025 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/config/_base.py
--rw-r--r--   0        0        0     2371 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/config/_utils.py
--rw-r--r--   0        0        0     9298 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/config/core.py
--rw-r--r--   0        0        0     9115 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/config/environment.py
--rw-r--r--   0        0        0      197 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/config/exceptions.py
--rw-r--r--   0        0        0     7515 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/config/executable.py
--rw-r--r--   0        0        0     1020 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/config/firecrest.py
--rw-r--r--   0        0        0     1262 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/config/read.py
--rw-r--r--   0        0        0     5973 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/config/resources.py
--rw-r--r--   0        0        0     5049 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/config/validate.py
--rw-r--r--   0        0        0     2313 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/compute_backend/credentials.py
--rw-r--r--   0        0        0     8433 2024-03-13 12:44:54.126934 mantik-0.4.9/mantik/mlflow.py
--rw-r--r--   0        0        0       27 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/models/__init__.py
--rw-r--r--   0        0        0     2228 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/models/image.py
--rw-r--r--   0        0        0        0 2024-03-13 12:44:54.189934 mantik-0.4.9/mantik/py.typed
--rw-r--r--   0        0        0       56 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/remote_file_service/__init__.py
--rw-r--r--   0        0        0     2824 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/remote_file_service/abstract_file_service.py
--rw-r--r--   0        0        0    10210 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/remote_file_service/data_client.py
--rw-r--r--   0        0        0     8775 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/remote_file_service/s3_file_service.py
--rw-r--r--   0        0        0     9071 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/remote_file_service/unicore_file_service.py
--rw-r--r--   0        0        0       52 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/runs/__init__.py
--rw-r--r--   0        0        0     1573 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/runs/artifacts.py
--rw-r--r--   0        0        0     6375 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/runs/local.py
--rw-r--r--   0        0        0     1160 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/runs/schemas.py
--rw-r--r--   0        0        0      315 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/testing/__init__.py
--rw-r--r--   0        0        0     8518 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/testing/cognito.py
--rw-r--r--   0        0        0     4756 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/testing/config.py
--rw-r--r--   0        0        0     1248 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/testing/env.py
--rw-r--r--   0        0        0     5937 2024-03-13 12:44:54.127934 mantik-0.4.9/mantik/testing/firecrest.py
--rw-r--r--   0        0        0    12345 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/testing/mlflow_server.py
--rw-r--r--   0        0        0     5892 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/testing/pyunicore.py
--rw-r--r--   0        0        0     2182 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/testing/remote_file_service.py
--rw-r--r--   0        0        0      927 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/testing/requests.py
--rw-r--r--   0        0        0     1942 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/testing/stress.py
--rw-r--r--   0        0        0      991 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/testing/token.py
--rw-r--r--   0        0        0       29 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/tracking/__init__.py
--rw-r--r--   0        0        0      920 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/tracking/environment.py
--rw-r--r--   0        0        0     1075 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/tracking/track.py
--rw-r--r--   0        0        0      167 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/__init__.py
--rw-r--r--   0        0        0     2391 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/env.py
--rw-r--r--   0        0        0      341 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/env_vars.py
--rw-r--r--   0        0        0      135 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/formatting.py
--rw-r--r--   0        0        0       73 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/mantik_api/__init__.py
--rw-r--r--   0        0        0     3957 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/mantik_api/client.py
--rw-r--r--   0        0        0     1208 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/mantik_api/code_repository.py
--rw-r--r--   0        0        0     1526 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/mantik_api/connection.py
--rw-r--r--   0        0        0     1259 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/mantik_api/credentials.py
--rw-r--r--   0        0        0     2507 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/mantik_api/data_repository.py
--rw-r--r--   0        0        0     1931 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/mantik_api/experiment_repository.py
--rw-r--r--   0        0        0     4713 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/mantik_api/models.py
--rw-r--r--   0        0        0     1505 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/mantik_api/run.py
--rw-r--r--   0        0        0      359 2024-03-13 12:44:54.128934 mantik-0.4.9/mantik/utils/mantik_api/user.py
--rw-r--r--   0        0        0      946 2024-03-13 12:44:54.129934 mantik-0.4.9/mantik/utils/mlflow.py
--rw-r--r--   0        0        0       67 2024-03-13 12:44:54.129934 mantik-0.4.9/mantik/utils/unicore/__init__.py
--rw-r--r--   0        0        0     2069 2024-03-13 12:44:54.129934 mantik-0.4.9/mantik/utils/unicore/upload.py
--rw-r--r--   0        0        0      771 2024-03-13 12:44:54.129934 mantik-0.4.9/mantik/utils/unicore/zip.py
--rw-r--r--   0        0        0     1120 2024-03-13 12:44:54.129934 mantik-0.4.9/mantik/utils/urls.py
--rw-r--r--   0        0        0     2868 2024-03-13 12:45:18.354892 mantik-0.4.9/pyproject.toml
--rw-r--r--   0        0        0      997 2024-03-13 12:44:54.131934 mantik-0.4.9/tests/conftest.py
--rw-r--r--   0        0        0     1534 2024-03-13 12:44:54.131934 mantik-0.4.9/tests/integration/mantik/s3_file_service/conftest.py
--rw-r--r--   0        0        0     6203 2024-03-13 12:44:54.131934 mantik-0.4.9/tests/integration/mantik/s3_file_service/test_s3_file_service_integration.py
--rw-r--r--   0        0        0       11 2024-03-13 12:44:54.131934 mantik-0.4.9/tests/integration/mantik/s3_file_service/workspace/sample-directory/hello-world.txt
--rw-r--r--   0        0        0      703 2024-03-13 12:44:54.131934 mantik-0.4.9/tests/integration/mantik_compute_backend/unicore/conftest.py
--rw-r--r--   0        0        0     8426 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/integration/mantik_compute_backend/unicore/test_backend_integration.py
--rw-r--r--   0        0        0      232 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/broken-project/MLproject
--rw-r--r--   0        0        0       77 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/broken-project/README.md
--rw-r--r--   0        0        0      246 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/broken-project/compute-backend-config.md
--rw-r--r--   0        0        0      574 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/cognito/auth-response.json
--rw-r--r--   0        0        0      159 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/cognito/different-client.json
--rw-r--r--   0        0        0      649 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/cognito/incorrect-login-credentials-response.json
--rw-r--r--   0        0        0      578 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/cognito/refresh-response.json
--rw-r--r--   0        0        0      631 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/cognito/refresh-token-expired-response.json
--rw-r--r--   0        0        0      623 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/cognito/refresh-token-invalid-response.json
--rw-r--r--   0        0        0      614 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/cognito/user-not-found-response.json
--rw-r--r--   0        0        0       57 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/test-project/Dockerfile
--rw-r--r--   0        0        0      488 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/test-project/MLproject
--rw-r--r--   0        0        0      244 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/test-project/compute-backend-config.json
--rw-r--r--   0        0        0      142 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/test-project/compute-backend-config.yaml
--rw-r--r--   0        0        0      383 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/test-project/compute-backend-firecrest-config.json
--rw-r--r--   0        0        0      253 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/test-project/compute-backend-firecrest-config.yaml
--rw-r--r--   0        0        0      121 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/test-project/config-with-errors.yaml
--rw-r--r--   0        0        0      536 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/test-project/main.py
--rw-r--r--   0        0        0        0 2024-03-13 12:44:54.195933 mantik-0.4.9/tests/resources/test-project/mantik-test.sif
--rw-r--r--   0        0        0       50 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/test-project/recipe.def
--rw-r--r--   0        0        0     1142 2024-03-13 12:44:54.132934 mantik-0.4.9/tests/resources/test-project/run.py
--rw-r--r--   0        0        0        0 2024-03-13 12:44:54.195933 mantik-0.4.9/tests/resources/test-project/test_subfolder/test.py
--rw-r--r--   0        0        0     2879 2024-03-13 12:44:54.133934 mantik-0.4.9/tests/resources/unicore-responses/job-property-response.json
--rw-r--r--   0        0        0     2558 2024-03-13 12:44:54.133934 mantik-0.4.9/tests/stress/mlflow_tracking_server/README.md
--rw-r--r--   0        0        0     5941 2024-03-13 12:44:54.133934 mantik-0.4.9/tests/stress/mlflow_tracking_server/increasing_artifact_file_size.py
--rw-r--r--   0        0        0     4870 2024-03-13 12:44:54.133934 mantik-0.4.9/tests/stress/mlflow_tracking_server/increasing_number_of_parallel_runs.py
--rw-r--r--   0        0        0     5398 2024-03-13 12:44:54.133934 mantik-0.4.9/tests/stress/mlflow_tracking_server/increasing_number_of_requests.py
--rw-r--r--   0        0        0   139300 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/stress/mlflow_tracking_server/results.ipynb
--rw-r--r--   0        0        0     3222 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/conftest.py
--rw-r--r--   0        0        0     1837 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/athentication/test_credentials.py
--rw-r--r--   0        0        0     2409 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/athentication/test_server_api.py
--rw-r--r--   0        0        0     1125 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/athentication/test_tokens.py
--rw-r--r--   0        0        0      298 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/cli/conftest.py
--rw-r--r--   0        0        0     6793 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/cli/remote_file_service/test_cli_unicore_file_service.py
--rw-r--r--   0        0        0     1980 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/cli/runs/test_local_runs.py
--rw-r--r--   0        0        0      921 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/cli/runs/test_runs.py
--rw-r--r--   0        0        0     5387 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/cli/runs/test_submit.py
--rw-r--r--   0        0        0      780 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/cli/test_init.py
--rw-r--r--   0        0        0     8542 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/cli/test_training_models.py
--rw-r--r--   0        0        0     2251 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/cli/test_utils.py
--rw-r--r--   0        0        0     3040 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/compute_backend/config/conftest.py
--rw-r--r--   0        0        0      805 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_base.py
--rw-r--r--   0        0        0    34021 2024-03-13 12:44:54.134934 mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_core.py
--rw-r--r--   0        0        0    16436 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_environment.py
--rw-r--r--   0        0        0     5109 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_executable.py
--rw-r--r--   0        0        0     2118 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_read.py
--rw-r--r--   0        0        0     2470 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_resources.py
--rw-r--r--   0        0        0     1995 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_utils_config.py
--rw-r--r--   0        0        0    10991 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_validate.py
--rw-r--r--   0        0        0      213 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/compute_backend/conftest.py
--rw-r--r--   0        0        0     2545 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/compute_backend/test_compute_backend_client.py
--rw-r--r--   0        0        0     2943 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/conftest.py
--rw-r--r--   0        0        0     1587 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/remote_file_service/conftest.py
--rw-r--r--   0        0        0    10376 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/remote_file_service/test_data_client.py
--rw-r--r--   0        0        0     1020 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/remote_file_service/test_s3_file_service.py
--rw-r--r--   0        0        0      591 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/remote_file_service/test_unicore_file_service.py
--rw-r--r--   0        0        0        0 2024-03-13 12:44:54.196934 mantik-0.4.9/tests/unit/mantik/runs/conftest.py
--rw-r--r--   0        0        0     1065 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/runs/test_artifacts.py
--rw-r--r--   0        0        0     5799 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/runs/test_local.py
--rw-r--r--   0        0        0      349 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/test_mlflow_not_installed.py
--rw-r--r--   0        0        0     5831 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/tracking/test_track.py
--rw-r--r--   0        0        0      835 2024-03-13 12:44:54.135934 mantik-0.4.9/tests/unit/mantik/utils/conftest.py
--rw-r--r--   0        0        0     5916 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik/utils/mantik_api/test_mantik_api.py
--rw-r--r--   0        0        0     1113 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik/utils/mantik_api/test_mantik_api_code.py
--rw-r--r--   0        0        0     1887 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik/utils/mantik_api/test_mantik_api_experiment.py
--rw-r--r--   0        0        0     7067 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik/utils/mantik_api/test_mantik_api_models.py
--rw-r--r--   0        0        0     2873 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik/utils/mantik_api/test_mantik_run.py
--rw-r--r--   0        0        0      713 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik/utils/test_env.py
--rw-r--r--   0        0        0     2326 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik/utils/test_urls.py
--rw-r--r--   0        0        0     5719 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik/utils/unicore/test_upload.py
--rw-r--r--   0        0        0     8424 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik_compute_backend/conftest.py
--rw-r--r--   0        0        0     5378 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik_compute_backend/firecrest_backend/test_firecrest_client.py
--rw-r--r--   0        0        0     1152 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik_compute_backend/firecrest_backend/test_firecrest_connect.py
--rw-r--r--   0        0        0      491 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik_compute_backend/firecrest_backend/test_firecrest_job.py
--rw-r--r--   0        0        0     6262 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik_compute_backend/test_api.py
--rw-r--r--   0        0        0      594 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik_compute_backend/test_app.py
--rw-r--r--   0        0        0     8247 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik_compute_backend/test_backend.py
--rw-r--r--   0        0        0     8074 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik_compute_backend/test_backend_firecrest.py
--rw-r--r--   0        0        0     6991 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik_compute_backend/test_backend_unicore.py
--rw-r--r--   0        0        0     2545 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik_compute_backend/test_client.py
--rw-r--r--   0        0        0    12314 2024-03-13 12:44:54.136934 mantik-0.4.9/tests/unit/mantik_compute_backend/test_exception_handler.py
--rw-r--r--   0        0        0     1348 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mantik_compute_backend/test_handle_submit_run.py
--rw-r--r--   0        0        0      393 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mantik_compute_backend/test_models.py
--rw-r--r--   0        0        0     3546 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mantik_compute_backend/test_submitted_run.py
--rw-r--r--   0        0        0        0 2024-03-13 12:44:54.196934 mantik-0.4.9/tests/unit/mantik_compute_backend/unicore/conftest.py
--rw-r--r--   0        0        0      417 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mantik_compute_backend/unicore/test_exceptions.py
--rw-r--r--   0        0        0     1910 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mantik_compute_backend/unicore/test_unicore_connect.py
--rw-r--r--   0        0        0      478 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mantik_compute_backend/unicore/test_unicore_credentials.py
--rw-r--r--   0        0        0      301 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mantik_compute_backend/utils/test_temp_dir.py
--rw-r--r--   0        0        0     3556 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mantik_with_mlflow/test_mlflow_installed.py
--rw-r--r--   0        0        0     1585 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mlflow_tracking_server/conftest.py
--rw-r--r--   0        0        0      193 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mlflow_tracking_server/flask/api/test_health_api.py
--rw-r--r--   0        0        0     4210 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mlflow_tracking_server/flask/conftest.py
--rw-r--r--   0        0        0     1864 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mlflow_tracking_server/flask/test_after_request.py
--rw-r--r--   0        0        0     1532 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mlflow_tracking_server/flask/test_flask_app.py
--rw-r--r--   0        0        0     1876 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mlflow_tracking_server/flask/test_rbac.py
--rw-r--r--   0        0        0      471 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mlflow_tracking_server/flask/test_skip.py
--rw-r--r--   0        0        0      393 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/mlflow_tracking_server/gunicorn/test_run.py
--rw-r--r--   0        0        0     2768 2024-03-13 12:44:54.137934 mantik-0.4.9/tests/unit/tokens/test_verifier.py
--rw-r--r--   0        0        0     3196 1970-01-01 00:00:00.000000 mantik-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-06 15:34:26.919654 mantik-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1389 2024-05-06 15:34:26.919654 mantik-0.5.0/README.md
+-rw-r--r--   0        0        0      183 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/authentication/__init__.py
+-rw-r--r--   0        0        0     1944 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/authentication/api.py
+-rw-r--r--   0        0        0     1813 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/authentication/auth.py
+-rw-r--r--   0        0        0     2394 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/authentication/tokens.py
+-rw-r--r--   0        0        0      132 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/__init__.py
+-rw-r--r--   0        0        0      514 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/_callbacks.py
+-rw-r--r--   0        0        0     2864 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/_options.py
+-rw-r--r--   0        0        0     1257 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/init.py
+-rw-r--r--   0        0        0       95 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/main.py
+-rw-r--r--   0        0        0       32 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/models/__init__.py
+-rw-r--r--   0        0        0     5893 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/models/models.py
+-rw-r--r--   0        0        0      113 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/remote_file_service/__init__.py
+-rw-r--r--   0        0        0      343 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/remote_file_service/_arguments.py
+-rw-r--r--   0        0        0      743 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/remote_file_service/_options.py
+-rw-r--r--   0        0        0     6130 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/remote_file_service/s3_file_service.py
+-rw-r--r--   0        0        0     6364 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/remote_file_service/unicore_file_service.py
+-rw-r--r--   0        0        0       59 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/runs/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/runs/_options.py
+-rw-r--r--   0        0        0     3407 2024-05-06 15:34:26.960654 mantik-0.5.0/mantik/cli/runs/local.py
+-rw-r--r--   0        0        0      854 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/cli/runs/runs.py
+-rw-r--r--   0        0        0     3384 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/cli/runs/submit.py
+-rw-r--r--   0        0        0      887 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/cli/utils.py
+-rw-r--r--   0        0        0      116 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/__init__.py
+-rw-r--r--   0        0        0     8569 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/client.py
+-rw-r--r--   0        0        0      369 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/config/__init__.py
+-rw-r--r--   0        0        0     1025 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/config/_base.py
+-rw-r--r--   0        0        0     2371 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/config/_utils.py
+-rw-r--r--   0        0        0     9492 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/config/core.py
+-rw-r--r--   0        0        0    12324 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/config/environment.py
+-rw-r--r--   0        0        0      197 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/config/exceptions.py
+-rw-r--r--   0        0        0     7515 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/config/executable.py
+-rw-r--r--   0        0        0     1020 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/config/firecrest.py
+-rw-r--r--   0        0        0     1262 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/config/read.py
+-rw-r--r--   0        0        0     5973 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/config/resources.py
+-rw-r--r--   0        0        0     5049 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/config/validate.py
+-rw-r--r--   0        0        0     2313 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/compute_backend/credentials.py
+-rw-r--r--   0        0        0     8433 2024-05-06 15:34:26.961654 mantik-0.5.0/mantik/mlflow.py
+-rw-r--r--   0        0        0       27 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/models/__init__.py
+-rw-r--r--   0        0        0     2228 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/models/image.py
+-rw-r--r--   0        0        0        0 2024-05-06 15:34:27.024653 mantik-0.5.0/mantik/py.typed
+-rw-r--r--   0        0        0       56 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/remote_file_service/__init__.py
+-rw-r--r--   0        0        0     2824 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/remote_file_service/abstract_file_service.py
+-rw-r--r--   0        0        0    10210 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/remote_file_service/data_client.py
+-rw-r--r--   0        0        0     8775 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/remote_file_service/s3_file_service.py
+-rw-r--r--   0        0        0     9071 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/remote_file_service/unicore_file_service.py
+-rw-r--r--   0        0        0       52 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/runs/__init__.py
+-rw-r--r--   0        0        0     1573 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/runs/artifacts.py
+-rw-r--r--   0        0        0     6375 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/runs/local.py
+-rw-r--r--   0        0        0     1160 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/runs/schemas.py
+-rw-r--r--   0        0        0      315 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/testing/__init__.py
+-rw-r--r--   0        0        0     8518 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/testing/cognito.py
+-rw-r--r--   0        0        0     4764 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/testing/config.py
+-rw-r--r--   0        0        0     1248 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/testing/env.py
+-rw-r--r--   0        0        0     5937 2024-05-06 15:34:26.962654 mantik-0.5.0/mantik/testing/firecrest.py
+-rw-r--r--   0        0        0    12345 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/testing/mlflow_server.py
+-rw-r--r--   0        0        0     5892 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/testing/pyunicore.py
+-rw-r--r--   0        0        0     2182 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/testing/remote_file_service.py
+-rw-r--r--   0        0        0      927 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/testing/requests.py
+-rw-r--r--   0        0        0     1942 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/testing/stress.py
+-rw-r--r--   0        0        0      991 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/testing/token.py
+-rw-r--r--   0        0        0       29 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/tracking/__init__.py
+-rw-r--r--   0        0        0      920 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/tracking/environment.py
+-rw-r--r--   0        0        0     1075 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/tracking/track.py
+-rw-r--r--   0        0        0      167 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/__init__.py
+-rw-r--r--   0        0        0     2391 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/env.py
+-rw-r--r--   0        0        0      341 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/env_vars.py
+-rw-r--r--   0        0        0      135 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/formatting.py
+-rw-r--r--   0        0        0       73 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/mantik_api/__init__.py
+-rw-r--r--   0        0        0     3957 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/mantik_api/client.py
+-rw-r--r--   0        0        0     1208 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/mantik_api/code_repository.py
+-rw-r--r--   0        0        0     1526 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/mantik_api/connection.py
+-rw-r--r--   0        0        0     1259 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/mantik_api/credentials.py
+-rw-r--r--   0        0        0     2507 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/mantik_api/data_repository.py
+-rw-r--r--   0        0        0     1931 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/mantik_api/experiment_repository.py
+-rw-r--r--   0        0        0     5852 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/mantik_api/models.py
+-rw-r--r--   0        0        0     1505 2024-05-06 15:34:26.963654 mantik-0.5.0/mantik/utils/mantik_api/run.py
+-rw-r--r--   0        0        0      359 2024-05-06 15:34:26.964654 mantik-0.5.0/mantik/utils/mantik_api/user.py
+-rw-r--r--   0        0        0      950 2024-05-06 15:34:26.964654 mantik-0.5.0/mantik/utils/mlflow.py
+-rw-r--r--   0        0        0       67 2024-05-06 15:34:26.964654 mantik-0.5.0/mantik/utils/unicore/__init__.py
+-rw-r--r--   0        0        0     2069 2024-05-06 15:34:26.964654 mantik-0.5.0/mantik/utils/unicore/upload.py
+-rw-r--r--   0        0        0      771 2024-05-06 15:34:26.964654 mantik-0.5.0/mantik/utils/unicore/zip.py
+-rw-r--r--   0        0        0     1120 2024-05-06 15:34:26.964654 mantik-0.5.0/mantik/utils/urls.py
+-rw-r--r--   0        0        0     2868 2024-05-06 15:34:26.966654 mantik-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      997 2024-05-06 15:34:26.966654 mantik-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1534 2024-05-06 15:34:26.966654 mantik-0.5.0/tests/integration/mantik/s3_file_service/conftest.py
+-rw-r--r--   0        0        0     6203 2024-05-06 15:34:26.966654 mantik-0.5.0/tests/integration/mantik/s3_file_service/test_s3_file_service_integration.py
+-rw-r--r--   0        0        0       11 2024-05-06 15:34:26.966654 mantik-0.5.0/tests/integration/mantik/s3_file_service/workspace/sample-directory/hello-world.txt
+-rw-r--r--   0        0        0      703 2024-05-06 15:34:26.966654 mantik-0.5.0/tests/integration/mantik_compute_backend/unicore/conftest.py
+-rw-r--r--   0        0        0     8503 2024-05-06 15:34:26.966654 mantik-0.5.0/tests/integration/mantik_compute_backend/unicore/test_backend_integration.py
+-rw-r--r--   0        0        0      232 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/broken-project/MLproject
+-rw-r--r--   0        0        0       77 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/broken-project/README.md
+-rw-r--r--   0        0        0      246 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/broken-project/compute-backend-config.md
+-rw-r--r--   0        0        0      574 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/cognito/auth-response.json
+-rw-r--r--   0        0        0      159 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/cognito/different-client.json
+-rw-r--r--   0        0        0      649 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/cognito/incorrect-login-credentials-response.json
+-rw-r--r--   0        0        0      578 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/cognito/refresh-response.json
+-rw-r--r--   0        0        0      631 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/cognito/refresh-token-expired-response.json
+-rw-r--r--   0        0        0      623 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/cognito/refresh-token-invalid-response.json
+-rw-r--r--   0        0        0      614 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/cognito/user-not-found-response.json
+-rw-r--r--   0        0        0       57 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/test-project/Dockerfile
+-rw-r--r--   0        0        0      488 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/test-project/MLproject
+-rw-r--r--   0        0        0      244 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/test-project/compute-backend-config.json
+-rw-r--r--   0        0        0      488 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/test-project/compute-backend-config.yaml
+-rw-r--r--   0        0        0      383 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/test-project/compute-backend-firecrest-config.json
+-rw-r--r--   0        0        0      253 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/test-project/compute-backend-firecrest-config.yaml
+-rw-r--r--   0        0        0      121 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/test-project/config-with-errors.yaml
+-rw-r--r--   0        0        0      536 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/test-project/main.py
+-rw-r--r--   0        0        0        0 2024-05-06 15:34:27.030653 mantik-0.5.0/tests/resources/test-project/mantik-test.sif
+-rw-r--r--   0        0        0       50 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/test-project/recipe.def
+-rw-r--r--   0        0        0     1142 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/test-project/run.py
+-rw-r--r--   0        0        0        0 2024-05-06 15:34:27.030653 mantik-0.5.0/tests/resources/test-project/test_subfolder/test.py
+-rw-r--r--   0        0        0     2879 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/resources/unicore-responses/job-property-response.json
+-rw-r--r--   0        0        0     2558 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/stress/mlflow_tracking_server/README.md
+-rw-r--r--   0        0        0     5941 2024-05-06 15:34:26.967654 mantik-0.5.0/tests/stress/mlflow_tracking_server/increasing_artifact_file_size.py
+-rw-r--r--   0        0        0     4870 2024-05-06 15:34:26.968654 mantik-0.5.0/tests/stress/mlflow_tracking_server/increasing_number_of_parallel_runs.py
+-rw-r--r--   0        0        0     5398 2024-05-06 15:34:26.968654 mantik-0.5.0/tests/stress/mlflow_tracking_server/increasing_number_of_requests.py
+-rw-r--r--   0        0        0   139300 2024-05-06 15:34:26.968654 mantik-0.5.0/tests/stress/mlflow_tracking_server/results.ipynb
+-rw-r--r--   0        0        0     3222 2024-05-06 15:34:26.968654 mantik-0.5.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0     1837 2024-05-06 15:34:26.968654 mantik-0.5.0/tests/unit/mantik/athentication/test_credentials.py
+-rw-r--r--   0        0        0     2409 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/athentication/test_server_api.py
+-rw-r--r--   0        0        0     1125 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/athentication/test_tokens.py
+-rw-r--r--   0        0        0      298 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/cli/conftest.py
+-rw-r--r--   0        0        0     6793 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/cli/remote_file_service/test_cli_unicore_file_service.py
+-rw-r--r--   0        0        0     1980 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/cli/runs/test_local_runs.py
+-rw-r--r--   0        0        0      921 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/cli/runs/test_runs.py
+-rw-r--r--   0        0        0     5387 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/cli/runs/test_submit.py
+-rw-r--r--   0        0        0      780 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/cli/test_init.py
+-rw-r--r--   0        0        0     8542 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/cli/test_training_models.py
+-rw-r--r--   0        0        0     2251 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/cli/test_utils.py
+-rw-r--r--   0        0        0     3040 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/compute_backend/config/conftest.py
+-rw-r--r--   0        0        0      805 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_base.py
+-rw-r--r--   0        0        0    34019 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_core.py
+-rw-r--r--   0        0        0    18387 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_environment.py
+-rw-r--r--   0        0        0     5109 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_executable.py
+-rw-r--r--   0        0        0     3472 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_read.py
+-rw-r--r--   0        0        0     2470 2024-05-06 15:34:26.969654 mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_resources.py
+-rw-r--r--   0        0        0     1995 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_utils_config.py
+-rw-r--r--   0        0        0    10991 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_validate.py
+-rw-r--r--   0        0        0      213 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/compute_backend/conftest.py
+-rw-r--r--   0        0        0     2545 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/compute_backend/test_compute_backend_client.py
+-rw-r--r--   0        0        0     2943 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/conftest.py
+-rw-r--r--   0        0        0     1587 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/remote_file_service/conftest.py
+-rw-r--r--   0        0        0    10376 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/remote_file_service/test_data_client.py
+-rw-r--r--   0        0        0     1020 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/remote_file_service/test_s3_file_service.py
+-rw-r--r--   0        0        0      591 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/remote_file_service/test_unicore_file_service.py
+-rw-r--r--   0        0        0        0 2024-05-06 15:34:27.031653 mantik-0.5.0/tests/unit/mantik/runs/conftest.py
+-rw-r--r--   0        0        0     1065 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/runs/test_artifacts.py
+-rw-r--r--   0        0        0     5799 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/runs/test_local.py
+-rw-r--r--   0        0        0      349 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/test_mlflow_not_installed.py
+-rw-r--r--   0        0        0     5831 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/tracking/test_track.py
+-rw-r--r--   0        0        0      835 2024-05-06 15:34:26.970654 mantik-0.5.0/tests/unit/mantik/utils/conftest.py
+-rw-r--r--   0        0        0     5916 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik/utils/mantik_api/test_mantik_api.py
+-rw-r--r--   0        0        0     1113 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik/utils/mantik_api/test_mantik_api_code.py
+-rw-r--r--   0        0        0     1887 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik/utils/mantik_api/test_mantik_api_experiment.py
+-rw-r--r--   0        0        0     8499 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik/utils/mantik_api/test_mantik_api_models.py
+-rw-r--r--   0        0        0     2873 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik/utils/mantik_api/test_mantik_run.py
+-rw-r--r--   0        0        0      713 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik/utils/test_env.py
+-rw-r--r--   0        0        0     2326 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik/utils/test_urls.py
+-rw-r--r--   0        0        0     5719 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik/utils/unicore/test_upload.py
+-rw-r--r--   0        0        0     8432 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik_compute_backend/conftest.py
+-rw-r--r--   0        0        0     5378 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik_compute_backend/firecrest_backend/test_firecrest_client.py
+-rw-r--r--   0        0        0     1152 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik_compute_backend/firecrest_backend/test_firecrest_connect.py
+-rw-r--r--   0        0        0      491 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik_compute_backend/firecrest_backend/test_firecrest_job.py
+-rw-r--r--   0        0        0     6262 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik_compute_backend/test_api.py
+-rw-r--r--   0        0        0      594 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik_compute_backend/test_app.py
+-rw-r--r--   0        0        0     8247 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik_compute_backend/test_backend.py
+-rw-r--r--   0        0        0     8310 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik_compute_backend/test_backend_firecrest.py
+-rw-r--r--   0        0        0     7030 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik_compute_backend/test_backend_unicore.py
+-rw-r--r--   0        0        0     2545 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik_compute_backend/test_client.py
+-rw-r--r--   0        0        0    12314 2024-05-06 15:34:26.971654 mantik-0.5.0/tests/unit/mantik_compute_backend/test_exception_handler.py
+-rw-r--r--   0        0        0     1348 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mantik_compute_backend/test_handle_submit_run.py
+-rw-r--r--   0        0        0      393 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mantik_compute_backend/test_models.py
+-rw-r--r--   0        0        0     3546 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mantik_compute_backend/test_submitted_run.py
+-rw-r--r--   0        0        0        0 2024-05-06 15:34:27.031653 mantik-0.5.0/tests/unit/mantik_compute_backend/unicore/conftest.py
+-rw-r--r--   0        0        0      417 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mantik_compute_backend/unicore/test_exceptions.py
+-rw-r--r--   0        0        0     1910 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mantik_compute_backend/unicore/test_unicore_connect.py
+-rw-r--r--   0        0        0      478 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mantik_compute_backend/unicore/test_unicore_credentials.py
+-rw-r--r--   0        0        0      301 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mantik_compute_backend/utils/test_temp_dir.py
+-rw-r--r--   0        0        0     3556 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mantik_with_mlflow/test_mlflow_installed.py
+-rw-r--r--   0        0        0     1585 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mlflow_tracking_server/conftest.py
+-rw-r--r--   0        0        0      193 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mlflow_tracking_server/flask/api/test_health_api.py
+-rw-r--r--   0        0        0     4210 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mlflow_tracking_server/flask/conftest.py
+-rw-r--r--   0        0        0     1864 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mlflow_tracking_server/flask/test_after_request.py
+-rw-r--r--   0        0        0     1532 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mlflow_tracking_server/flask/test_flask_app.py
+-rw-r--r--   0        0        0     1876 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mlflow_tracking_server/flask/test_rbac.py
+-rw-r--r--   0        0        0      471 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mlflow_tracking_server/flask/test_skip.py
+-rw-r--r--   0        0        0      393 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/mlflow_tracking_server/gunicorn/test_run.py
+-rw-r--r--   0        0        0     2768 2024-05-06 15:34:26.972653 mantik-0.5.0/tests/unit/tokens/test_verifier.py
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 mantik-0.5.0/PKG-INFO
```

### Comparing `mantik-0.4.9/LICENSE` & `mantik-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/README.md` & `mantik-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# mantik - plugin for MLflow with HPC (UNICORE)
+# Mantik - Enhancing Machine Learning Development on HPC
 
 Mantik allows to manage the full Machine Learning workflow on HPC by
-supporting MLflow and deployment of applications to HPC.
+supporting MLflow and deployment of applications to HPC via the [Mantik platform](https://cloud.mantik.ai).
 
 For a quickstart see [our documentation](https://mantik-ai.gitlab.io/mantik/client-quickstart.html)
 
 ## Extra Dependencies
 
 By default, mantik only installs the core dependencies required to use the Mantik API.
 However, additional extras are provided and can be installed:
@@ -34,7 +34,8 @@
   pip install "mantik[docker]"
   ```
 
 ## Helpdesk
 
 For bug reports or feature requests, please email our helpdesk.
 Details can be found [here](https://mantik-ai.gitlab.io/mantik/helpdesk.html).
+
```

### Comparing `mantik-0.4.9/mantik/authentication/api.py` & `mantik-0.5.0/mantik/authentication/api.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/authentication/auth.py` & `mantik-0.5.0/mantik/authentication/auth.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/authentication/tokens.py` & `mantik-0.5.0/mantik/authentication/tokens.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/cli/_callbacks.py` & `mantik-0.5.0/mantik/cli/_callbacks.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/cli/_options.py` & `mantik-0.5.0/mantik/cli/_options.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/cli/init.py` & `mantik-0.5.0/mantik/cli/init.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/cli/models/models.py` & `mantik-0.5.0/mantik/cli/models/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,16 @@
         token=utils.access_token_from_env_vars(),
     )
 
 
 @cli.command("add")
 @_options.PROJECT_ID
 @_options.get_name_option(required=True, help_option="Model name.")
-@click.option("--uri", type=str, required=True)
-@click.option("--location", type=str, required=True)
+@click.option("--uri", type=str, required=False)
+@click.option("--location", type=str, required=False)
 @_options.get_connection_id(required=False)
 @click.option(
     "--mlflow-parameters",
     type=str,
     required=False,
     help="""JSON data as a string.""",
     callback=mlflow_parameters_decoder,
```

### Comparing `mantik-0.4.9/mantik/cli/remote_file_service/_options.py` & `mantik-0.5.0/mantik/cli/remote_file_service/_options.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/cli/remote_file_service/s3_file_service.py` & `mantik-0.5.0/mantik/cli/remote_file_service/s3_file_service.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/cli/remote_file_service/unicore_file_service.py` & `mantik-0.5.0/mantik/cli/remote_file_service/unicore_file_service.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/cli/runs/_options.py` & `mantik-0.5.0/mantik/cli/runs/_options.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/cli/runs/local.py` & `mantik-0.5.0/mantik/cli/runs/local.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/cli/runs/runs.py` & `mantik-0.5.0/mantik/cli/runs/runs.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/cli/runs/submit.py` & `mantik-0.5.0/mantik/cli/runs/submit.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/cli/utils.py` & `mantik-0.5.0/mantik/cli/utils.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/compute_backend/client.py` & `mantik-0.5.0/mantik/compute_backend/client.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/compute_backend/config/_base.py` & `mantik-0.5.0/mantik/compute_backend/config/_base.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/compute_backend/config/_utils.py` & `mantik-0.5.0/mantik/compute_backend/config/_utils.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/compute_backend/config/core.py` & `mantik-0.5.0/mantik/compute_backend/config/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,18 +151,18 @@
             "Resources": self.resources,
             # Write stderr/stdout to given file to allow access to logs
             "Stdout": APPLICATION_LOGS_FILE,
             "Stderr": APPLICATION_LOGS_FILE,
             **environment,
         }
 
-    def to_unicore_job_description(self, arguments: str) -> t.Dict:
+    def to_unicore_job_description(self, bash_script_name: str) -> t.Dict:
         """Convert to UNICORE job description."""
         environment = (
-            self.environment.to_unicore_job_description(arguments)
+            self.environment.to_unicore_job_description(bash_script_name)
             if self.environment is not None
             else {}
         )
         return {
             **self.to_dict(),
             **environment,
         }
@@ -174,15 +174,15 @@
 
         firecREST only allows to submit jobs via batch scripts, which has to be
         manually constructed.
 
         """
         return "\n".join(
             [
-                "#!/bin/bash",
+                "#!/bin/bash -l",
                 f"#SBATCH --job-name='mantik-{run_id}'",
                 self.resources.to_slurm_batch_script(),
                 f"#SBATCH --output={run_dir}/mantik.log",
                 f"#SBATCH --error={run_dir}/mantik.log",
                 # The `--chdir` option is ignored by firecREST.
                 # We could propose this feature, but for now we will
                 # stick to manually changing the directory.
@@ -190,19 +190,23 @@
                 'echo "Submitted batch script:"',
                 "cat $(pwd)/script.batch",
                 # _Must_ cd after cat, otherwise the `script.batch` file will
                 # not be available.
                 f'echo "Changing to Mantik run directory {run_dir}"',
                 f"cd {run_dir}",
                 self.environment.to_slurm_batch_script(
-                    entry_point_arguments=arguments
+                    entry_point_arguments=arguments, run_dir=run_dir
                 ),
             ]
         )
 
+    def to_bash_script(self, arguments: str) -> str:
+        """Create a bash script for UNICORE."""
+        return self.environment.to_bash_script(arguments)
+
     def execution_environment_given(self) -> bool:
         return (
             self.environment is not None and self.environment.execution_given()
         )
 
     def add_env_vars(self, env_vars: t.Dict) -> None:
         self.environment.add_env_vars(env_vars)
```

### Comparing `mantik-0.4.9/mantik/compute_backend/config/environment.py` & `mantik-0.5.0/mantik/compute_backend/config/environment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import copy
 import dataclasses
 import os
+import pathlib
 import re
 import typing as t
 
 import mantik.compute_backend.config._base as _base
 import mantik.compute_backend.config._utils as _utils
 import mantik.compute_backend.config.exceptions as exceptions
 import mantik.compute_backend.config.executable as _executable
@@ -22,51 +24,60 @@
 class Environment(_base.ConfigObject):
     """Part of the backend-config where all variables
     concerning the running environment are stored."""
 
     execution: t.Optional[_executable.Execution] = None
     variables: t.Optional[t.Dict] = None
     modules: t.Optional[t.List] = None
-    pre_run_command_on_login_node: t.Optional[str] = None
-    pre_run_command_on_compute_node: t.Optional[str] = None
-    post_run_command_on_compute_node: t.Optional[str] = None
-    post_run_command_on_login_node: t.Optional[str] = None
+    pre_run_command_on_login_node: t.Optional[list] = None
+    pre_run_command_on_compute_node: t.Optional[list] = None
+    post_run_command_on_compute_node: t.Optional[list] = None
+    post_run_command_on_login_node: t.Optional[list] = None
 
     @classmethod
     def _from_dict(cls, config: t.Dict) -> "Environment":
         execution = _get_execution_environment(config)
         variables = _utils.get_optional_config_value(
             name="Variables",
             value_type=dict,
             config=config,
         )
         modules = _utils.get_optional_config_value(
             name="Modules",
             value_type=list,
             config=config,
         )
+
         preRunCommandOnLoginNode = _utils.get_optional_config_value(
             name="PreRunCommandOnLoginNode",
-            value_type=str,
-            config=config,
+            value_type=list,
+            config=_cast_run_command_str_to_list(
+                config, "PreRunCommandOnLoginNode"
+            ),
         )
         preRunCommandOnComputeNode = _utils.get_optional_config_value(
             name="PreRunCommandOnComputeNode",
-            value_type=str,
-            config=config,
+            value_type=list,
+            config=_cast_run_command_str_to_list(
+                config, "PreRunCommandOnComputeNode"
+            ),
         )
         postRunCommandOnComputeNode = _utils.get_optional_config_value(
             name="PostRunCommandOnComputeNode",
-            value_type=str,
-            config=config,
+            value_type=list,
+            config=_cast_run_command_str_to_list(
+                config, "PostRunCommandOnComputeNode"
+            ),
         )
         postRunCommandOnLoginNode = _utils.get_optional_config_value(
             name="PostRunCommandOnLoginNode",
-            value_type=str,
-            config=config,
+            value_type=list,
+            config=_cast_run_command_str_to_list(
+                config, "PostRunCommandOnLoginNode"
+            ),
         )
 
         return cls(
             execution=execution,
             modules=modules,
             variables=variables,
             pre_run_command_on_login_node=preRunCommandOnLoginNode,
@@ -78,33 +89,52 @@
     def __post_init__(self):
         """Add all MLflow environment variables to the environment."""
         self.variables = _add_mlflow_env_vars(self.variables)
 
     def _to_dict(self) -> t.Dict:
         return {
             "Environment": self.variables,
-            "User precommand": self.pre_run_command_on_login_node,
+            "User precommand": self._create_login_node_command(
+                self.pre_run_command_on_login_node
+            ),
             "RunUserPrecommandOnLoginNode": True,
             "Arguments": [],
-            "User postcommand": self.post_run_command_on_login_node,
+            "User postcommand": self._create_login_node_command(
+                self.post_run_command_on_login_node
+            ),
             "RunUserPostcommandOnLoginNode": True,
         }
 
+    def _create_login_node_command(
+        self, commands: t.Optional[list]
+    ) -> t.Optional[str]:
+        # Login node commands are only allowed by UNICORE, and it allows
+        # only single strings as commands. Thus, we concatenate multiple
+        # commands using `&&`. This makes the command fail if any of
+        # the given commands fails.
+        return _concatenate_commands(commands, concatenation_str=" && ")
+
+    def _create_compute_node_command(
+        self, commands: t.Optional[list]
+    ) -> t.Optional[str]:
+        return _concatenate_commands(commands, concatenation_str="\n")
+
     def _create_pre_run_command_on_compute_node(self) -> t.Optional[str]:
         # Venv MUST be loaded before modules
         # see https://gitlab.com/mantik-ai/mantik/issues/140
-        precommand = (
-            self.pre_run_command_on_compute_node
+        return (
+            self._create_compute_node_command(
+                [
+                    self._create_modules_command(),
+                    *self.pre_run_command_on_compute_node,
+                ],
+            )
             if self.pre_run_command_on_compute_node
-            else None
-        )
-        joined_str = " && ".join(
-            filter(None, [self._create_modules_command(), precommand])
+            else self._create_modules_command()
         )
-        return joined_str or None
 
     def _create_modules_command(self) -> t.Optional[str]:
         return f"module load {' '.join(self.modules)}" if self.modules else None
 
     def _create_execution_command(self) -> t.Optional[str]:
         if self.execution is not None:
             execution_command = self.execution.get_execution_command()
@@ -149,19 +179,21 @@
             filter(
                 None, [self._create_execution_command(), entry_point_arguments]
             )
         )
         list_to_join = [
             self._create_pre_run_command_on_compute_node(),
             execution_command_arguments_string,
-            self.post_run_command_on_compute_node,
+            self._create_compute_node_command(
+                self.post_run_command_on_compute_node
+            ),
         ]
         return " && ".join(filter(None, list_to_join))
 
-    def to_unicore_job_description(self, arguments: str) -> t.Dict:
+    def to_unicore_job_description(self, bash_script_name: str) -> t.Dict:
         """Convert to UNICORE job description.
 
         Parameters
         ----------
         arguments : str
             Arguments to pass to the executable.
 
@@ -170,51 +202,71 @@
         dict
             The UNICORE job description.
 
             For details see https://sourceforge.net/p/unicore/wiki/Job_Description  # noqa: E501
 
 
         """
-        return {
+        job_description = {
             **self.to_dict(),
-            "Executable": self._create_execution_command_with_arguments(
-                arguments
-            ),
+            "Executable": f'source $(dirname "$(realpath "$0")")/{bash_script_name}',  # noqa E501
         }
+        job_description["Environment"] = job_description.get("Environment", {})
+        job_description["Environment"].update(
+            {"MANTIK_WORKING_DIRECTORY": "$UC_WORKING_DIRECTORY"}
+        )
+
+        return job_description
 
     def execution_given(self) -> bool:
         return self.execution is not None
 
     def add_env_vars(self, env_vars: t.Dict) -> None:
         if self.variables is None:
             self.variables = env_vars
         else:
             self.variables.update(env_vars)
 
-    def to_slurm_batch_script(self, entry_point_arguments: str) -> str:
+    def to_slurm_batch_script(
+        self, entry_point_arguments: str, run_dir: pathlib.Path
+    ) -> str:
         # Setting env vars via the firecREST API is only supported from
         # version >= v1.14.0. Hence, we set them explicitly.
+        env_vars_list = [f"export MANTIK_WORKING_DIRECTORY={run_dir}"]
         if self.variables is not None:
-            env_vars_list = [
-                f"export {key}={value}" for key, value in self.variables.items()
-            ]
-            env_vars_str = "\n".join(env_vars_list)
-        else:
-            env_vars_str = None
-
-        job_script = "\n".join(
-            filter(
-                None,
+            env_vars_list.extend(
                 [
-                    env_vars_str,
-                    self._create_execution_command_with_arguments(
-                        entry_point_arguments
-                    ),
-                ],
+                    f"export {key}={value}"
+                    for key, value in self.variables.items()
+                ]
             )
+        env_vars_str = _concatenate_commands(env_vars_list, "\n")
+
+        job_script = _concatenate_commands(
+            commands=[
+                env_vars_str,
+                self._create_execution_command_with_arguments(
+                    entry_point_arguments
+                ),
+            ],
+            concatenation_str="\n",
+        )
+        return job_script
+
+    def to_bash_script(self, entry_point_arguments: str) -> str:
+        """Create a bash script for UNICORE."""
+        job_script = _concatenate_commands(
+            commands=[
+                "echo 'Submitted bash script'",
+                'cat "$(realpath "$0")"',
+                self._create_execution_command_with_arguments(
+                    entry_point_arguments
+                ),
+            ],
+            concatenation_str="\n",
         )
         return job_script
 
 
 def _get_execution_environment(
     config: t.Dict,
 ) -> t.Optional[_executable.Execution]:
@@ -257,7 +309,40 @@
 def _get_mlflow_env_vars() -> t.Dict:
     pattern = re.compile(rf"{_MLFLOW_ENV_VAR_PREFIX}\w+")
     return {
         key: value
         for key, value in os.environ.items()
         if pattern.match(key) and key not in mlflow.CONFLICTING_ENV_VARS
     }
+
+
+def _concatenate_commands(
+    commands: t.Optional[list], concatenation_str: str
+) -> t.Optional[str]:
+    return concatenation_str.join(filter(None, commands)) if commands else None
+
+
+def _cast_run_command_str_to_list(
+    config: t.Dict, run_command_name: str
+) -> t.Dict:
+    """
+    Converts the Pre/PostRunCommands specified in the config from a string
+    to list format. This ensures the backward compatibility with configs
+    that allow strings in the run commands.
+    """
+    config = copy.deepcopy(config)
+    run_command_value = config.get(run_command_name, None)
+    if run_command_value is not None:
+        if isinstance(run_command_value, str):
+            config[run_command_name] = [run_command_value]
+            return config
+        elif isinstance(run_command_value, list):
+            config[run_command_name] = [
+                str(command) for command in run_command_value
+            ]
+            return config
+        else:
+            raise exceptions.ConfigValidationError(
+                f"Config value for {run_command_name!r} has to be of type str "
+                "or list"
+            )
+    return config
```

### Comparing `mantik-0.4.9/mantik/compute_backend/config/executable.py` & `mantik-0.5.0/mantik/compute_backend/config/executable.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/compute_backend/config/firecrest.py` & `mantik-0.5.0/mantik/compute_backend/config/firecrest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/compute_backend/config/read.py` & `mantik-0.5.0/mantik/compute_backend/config/read.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/compute_backend/config/resources.py` & `mantik-0.5.0/mantik/compute_backend/config/resources.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/compute_backend/config/validate.py` & `mantik-0.5.0/mantik/compute_backend/config/validate.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/compute_backend/credentials.py` & `mantik-0.5.0/mantik/compute_backend/credentials.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/mlflow.py` & `mantik-0.5.0/mantik/mlflow.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/models/image.py` & `mantik-0.5.0/mantik/models/image.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/remote_file_service/abstract_file_service.py` & `mantik-0.5.0/mantik/remote_file_service/abstract_file_service.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/remote_file_service/data_client.py` & `mantik-0.5.0/mantik/remote_file_service/data_client.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/remote_file_service/s3_file_service.py` & `mantik-0.5.0/mantik/remote_file_service/s3_file_service.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/remote_file_service/unicore_file_service.py` & `mantik-0.5.0/mantik/remote_file_service/unicore_file_service.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/runs/artifacts.py` & `mantik-0.5.0/mantik/runs/artifacts.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/runs/local.py` & `mantik-0.5.0/mantik/runs/local.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/runs/schemas.py` & `mantik-0.5.0/mantik/runs/schemas.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/testing/cognito.py` & `mantik-0.5.0/mantik/testing/cognito.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/testing/config.py` & `mantik-0.5.0/mantik/testing/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 
 
 def _create_apptainer_environment(
     path: pathlib.Path,
     type: str = None,
     variables: t.Optional[t.Dict] = None,
     modules: t.Optional[t.List] = None,
-    pre_run_command_on_login_node: t.Optional[str] = None,
-    pre_run_command_on_compute_node: t.Optional[str] = None,
-    post_run_command_on_compute_node: t.Optional[str] = None,
-    post_run_command_on_login_node: t.Optional[str] = None,
+    pre_run_command_on_login_node: t.Optional[list] = None,
+    pre_run_command_on_compute_node: t.Optional[list] = None,
+    post_run_command_on_compute_node: t.Optional[list] = None,
+    post_run_command_on_login_node: t.Optional[list] = None,
     include_mlflow_env_vars: bool = True,
 ) -> config.environment.Environment:
     if type is None:
         type = "local"
     if include_mlflow_env_vars:
         variables = _include_mlflow_env_vars(variables)
 
@@ -60,18 +60,18 @@
     )
 
 
 def _create_python_environment(
     path: pathlib.Path,
     variables: t.Optional[t.Dict] = None,
     modules: t.Optional[t.List] = None,
-    pre_run_command_on_login_node: t.Optional[str] = None,
-    pre_run_command_on_compute_node: t.Optional[str] = None,
-    post_run_command_on_compute_node: t.Optional[str] = None,
-    post_run_command_on_login_node: t.Optional[str] = None,
+    pre_run_command_on_login_node: t.Optional[list] = None,
+    pre_run_command_on_compute_node: t.Optional[list] = None,
+    post_run_command_on_compute_node: t.Optional[list] = None,
+    post_run_command_on_login_node: t.Optional[list] = None,
     include_mlflow_env_vars: bool = True,
 ) -> config.environment.Environment:
     if include_mlflow_env_vars:
         variables = _include_mlflow_env_vars(variables)
 
     return config.environment.Environment(
         config.executable.Python(
```

### Comparing `mantik-0.4.9/mantik/testing/env.py` & `mantik-0.5.0/mantik/testing/env.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/testing/firecrest.py` & `mantik-0.5.0/mantik/testing/firecrest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/testing/mlflow_server.py` & `mantik-0.5.0/mantik/testing/mlflow_server.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/testing/pyunicore.py` & `mantik-0.5.0/mantik/testing/pyunicore.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/testing/remote_file_service.py` & `mantik-0.5.0/mantik/testing/remote_file_service.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/testing/requests.py` & `mantik-0.5.0/mantik/testing/requests.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/testing/stress.py` & `mantik-0.5.0/mantik/testing/stress.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/testing/token.py` & `mantik-0.5.0/mantik/testing/token.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/tracking/environment.py` & `mantik-0.5.0/mantik/tracking/environment.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/tracking/track.py` & `mantik-0.5.0/mantik/tracking/track.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/utils/env.py` & `mantik-0.5.0/mantik/utils/env.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/utils/mantik_api/client.py` & `mantik-0.5.0/mantik/utils/mantik_api/client.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/utils/mantik_api/code_repository.py` & `mantik-0.5.0/mantik/utils/mantik_api/code_repository.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/utils/mantik_api/connection.py` & `mantik-0.5.0/mantik/utils/mantik_api/connection.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/utils/mantik_api/credentials.py` & `mantik-0.5.0/mantik/utils/mantik_api/credentials.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/utils/mantik_api/data_repository.py` & `mantik-0.5.0/mantik/utils/mantik_api/data_repository.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/utils/mantik_api/experiment_repository.py` & `mantik-0.5.0/mantik/utils/mantik_api/experiment_repository.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/utils/mantik_api/run.py` & `mantik-0.5.0/mantik/utils/mantik_api/run.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/utils/mlflow.py` & `mantik-0.5.0/mantik/utils/mlflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 EXPERIMENT_ID_ENV_VAR = "MLFLOW_EXPERIMENT_ID"
 
 CONFLICTING_ENV_VARS = (
     TRACKING_USERNAME_ENV_VAR,
     TRACKING_PASSWORD_ENV_VAR,
 )
 
-DEFAULT_TRACKING_URI = "https://tracking.cloud.mantik.ai/"
+DEFAULT_TRACKING_URI = "https://api.cloud.mantik.ai/tracking/"
 
 
 def unset_conflicting_env_vars() -> None:
     env.unset_env_vars(CONFLICTING_ENV_VARS)
```

### Comparing `mantik-0.4.9/mantik/utils/unicore/upload.py` & `mantik-0.5.0/mantik/utils/unicore/upload.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/utils/unicore/zip.py` & `mantik-0.5.0/mantik/utils/unicore/zip.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/mantik/utils/urls.py` & `mantik-0.5.0/mantik/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/pyproject.toml` & `mantik-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mantik"
-version = "0.4.9"
+version = "0.5.0"
 description = "mantik for mlflow"
 authors = [
     "Fabian Emmerich <fabian.emmerich@4-cast.de>",
     "Thomas Seidler <thomas.seidler@ambrosys.de>",
 ]
 maintainers = [
     "Elia Boscaini <elia.boscaini@ambrosys.de>",
```

### Comparing `mantik-0.4.9/tests/conftest.py` & `mantik-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/integration/mantik/s3_file_service/conftest.py` & `mantik-0.5.0/tests/integration/mantik/s3_file_service/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/integration/mantik/s3_file_service/test_s3_file_service_integration.py` & `mantik-0.5.0/tests/integration/mantik/s3_file_service/test_s3_file_service_integration.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/integration/mantik_compute_backend/unicore/conftest.py` & `mantik-0.5.0/tests/integration/mantik_compute_backend/unicore/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/integration/mantik_compute_backend/unicore/test_backend_integration.py` & `mantik-0.5.0/tests/integration/mantik_compute_backend/unicore/test_backend_integration.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,35 +70,37 @@
                 {
                     "Environment": {
                         "Variables": {"TEST_VAR": "test_value"},
                         "Apptainer": {
                             "Path": "/does/not/exist.sif",
                             "Type": "remote",
                         },
-                        "PreRunCommandOnLoginNode": "echo precommand login node\n echo again",  # noqa E501
-                        "PostRunCommandOnLoginNode": "echo postcommand login node",  # noqa E501
-                        "PreRunCommandOnComputeNode": "echo precommand compute node",  # noqa E501
-                        "PostRunCommandOnComputeNode": "echo postcommand compute node",  # noqa E501
+                        "PreRunCommandOnLoginNode": [
+                            "echo precommand login node",
+                            "echo again",
+                        ],
+                        "PostRunCommandOnLoginNode": [
+                            "echo postcommand login node"
+                        ],
+                        "PreRunCommandOnComputeNode": [
+                            "echo precommand compute node"
+                        ],
+                        "PostRunCommandOnComputeNode": [
+                            "echo postcommand compute node"
+                        ],
                     },
                     "Resources": RESOURCES,
                 },
                 entities.RunStatus.FAILED,
                 [
                     *EXPECTED_RESOURCE_MESSAGES,
                     "MLFLOW_RUN_ID=",
                     "; export MLFLOW_RUN_ID",
                     'TEST_VAR="test_value"; export TEST_VAR',
-                    "echo precommand login node\n echo again",
-                    (
-                        "echo precommand compute node && "
-                        "srun apptainer run "
-                        "/does/not/exist.sif "
-                        "python main.py test && "
-                        "echo postcommand compute node"
-                    ),
+                    'source $(dirname "$(realpath "$0")")/mantik.sh',
                 ],
             ),
             # Test case: Python with 1 env var
             #
             # * Test case will fail since no venv present in UNICORE container,
             #   thus the post command on login node won't be executed
             (
@@ -106,34 +108,39 @@
                 {"print": "test"},
                 {
                     "Environment": {
                         "Variables": {"TEST_VAR": "test_value"},
                         "Python": {
                             "Path": "/does/not/exist",
                         },
-                        "PreRunCommandOnLoginNode": "echo precommand login node\n echo again",  # noqa E501
-                        "PostRunCommandOnLoginNode": "echo postcommand login node",  # noqa E501
-                        "PreRunCommandOnComputeNode": "echo precommand compute node",  # noqa E501
-                        "PostRunCommandOnComputeNode": "echo postcommand compute node",  # noqa E501
+                        "PreRunCommandOnLoginNode": [
+                            "echo precommand login node",
+                            "echo again",
+                        ],
+                        "PostRunCommandOnLoginNode": [
+                            "echo postcommand login node"
+                        ],
+                        "PreRunCommandOnComputeNode": [
+                            "echo precommand compute node"
+                        ],
+                        "PostRunCommandOnComputeNode": [
+                            "echo postcommand compute node"
+                        ],
                     },
                     "Resources": RESOURCES,
                 },
                 entities.RunStatus.FAILED,
                 [
                     *EXPECTED_RESOURCE_MESSAGES,
                     "MLFLOW_RUN_ID=",
                     "; export MLFLOW_RUN_ID",
                     'TEST_VAR="test_value"; export TEST_VAR',
-                    "echo precommand login node\n echo again",
-                    (
-                        "echo precommand compute node && "
-                        "source /does/not/exist/bin/activate && "
-                        "python main.py test && "
-                        "echo postcommand compute node"
-                    ),
+                    "echo precommand login node",
+                    "echo again",
+                    'source $(dirname "$(realpath "$0")")/mantik.sh',
                 ],
             ),
             # Test case: No execution environment and echo entry point
             #
             # * Should succeed
             # * Pre/postcommand will be executed on login node, hence no modules
             #   loaded here. Modules would make the pre command fail (no modules
@@ -141,31 +148,36 @@
             #   executed, as well as the post command.
             (
                 "echo",
                 {"output": "test"},
                 {
                     "Environment": {
                         "Variables": {"TEST_VAR": "test_value"},
-                        "PreRunCommandOnLoginNode": "echo precommand login node\n echo again",  # noqa E501
-                        "PostRunCommandOnLoginNode": "echo postcommand login node",  # noqa E501
+                        "PreRunCommandOnLoginNode": [
+                            "echo precommand login node",
+                            "echo again",
+                        ],
+                        "PostRunCommandOnLoginNode": [
+                            "echo postcommand login node"
+                        ],
                     },
                     "Resources": RESOURCES,
                 },
                 entities.RunStatus.FINISHED,
                 [
-                    "Launched pre command <echo precommand login node\n "
+                    "Launched pre command <echo precommand login node && "
                     "echo again>\n",
-                    "Executing command: echo precommand login node\n "
+                    "Executing command: echo precommand login node && "
                     "echo again",
                     "Execution on login node",
                     *EXPECTED_RESOURCE_MESSAGES,
                     'TEST_VAR="test_value"; export TEST_VAR',
                     "MLFLOW_RUN_ID=",
                     "; export MLFLOW_RUN_ID",
-                    "echo test",
+                    'source $(dirname "$(realpath "$0")")/mantik.sh',
                 ],
             ),
         ],
     )
     def test_run(
         self,
         tmp_path,
@@ -212,11 +224,10 @@
                 experiment_id=None,
             )
             # Wait for job to fail or succeed
             result.wait()
             # For the structure of the UNICORE job properties responce, see
             # `tests/resources/unicore-responses/job-property-response.json`.
             result_log_messages = "\n".join(result._job._job.properties["log"])
-
         for exp in expected_log_messages:
             assert exp in result_log_messages, f"Message {exp!r} not in logs"
         assert result.get_status() == expected_job_status
```

### Comparing `mantik-0.4.9/tests/resources/cognito/auth-response.json` & `mantik-0.5.0/tests/resources/cognito/auth-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/resources/cognito/incorrect-login-credentials-response.json` & `mantik-0.5.0/tests/resources/cognito/incorrect-login-credentials-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/resources/cognito/refresh-response.json` & `mantik-0.5.0/tests/resources/cognito/refresh-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/resources/cognito/refresh-token-expired-response.json` & `mantik-0.5.0/tests/resources/cognito/refresh-token-expired-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/resources/cognito/refresh-token-invalid-response.json` & `mantik-0.5.0/tests/resources/cognito/refresh-token-invalid-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/resources/cognito/user-not-found-response.json` & `mantik-0.5.0/tests/resources/cognito/user-not-found-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/resources/test-project/main.py` & `mantik-0.5.0/tests/resources/test-project/main.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/resources/test-project/run.py` & `mantik-0.5.0/tests/resources/test-project/run.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/resources/unicore-responses/job-property-response.json` & `mantik-0.5.0/tests/resources/unicore-responses/job-property-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/stress/mlflow_tracking_server/README.md` & `mantik-0.5.0/tests/stress/mlflow_tracking_server/README.md`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/stress/mlflow_tracking_server/increasing_artifact_file_size.py` & `mantik-0.5.0/tests/stress/mlflow_tracking_server/increasing_artifact_file_size.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/stress/mlflow_tracking_server/increasing_number_of_parallel_runs.py` & `mantik-0.5.0/tests/stress/mlflow_tracking_server/increasing_number_of_parallel_runs.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/stress/mlflow_tracking_server/increasing_number_of_requests.py` & `mantik-0.5.0/tests/stress/mlflow_tracking_server/increasing_number_of_requests.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/stress/mlflow_tracking_server/results.ipynb` & `mantik-0.5.0/tests/stress/mlflow_tracking_server/results.ipynb`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/conftest.py` & `mantik-0.5.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/athentication/test_credentials.py` & `mantik-0.5.0/tests/unit/mantik/athentication/test_credentials.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/athentication/test_server_api.py` & `mantik-0.5.0/tests/unit/mantik/athentication/test_server_api.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/athentication/test_tokens.py` & `mantik-0.5.0/tests/unit/mantik/athentication/test_tokens.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/cli/remote_file_service/test_cli_unicore_file_service.py` & `mantik-0.5.0/tests/unit/mantik/cli/remote_file_service/test_cli_unicore_file_service.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/cli/runs/test_local_runs.py` & `mantik-0.5.0/tests/unit/mantik/cli/runs/test_local_runs.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/cli/runs/test_runs.py` & `mantik-0.5.0/tests/unit/mantik/cli/runs/test_runs.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/cli/runs/test_submit.py` & `mantik-0.5.0/tests/unit/mantik/cli/runs/test_submit.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/cli/test_init.py` & `mantik-0.5.0/tests/unit/mantik/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/cli/test_training_models.py` & `mantik-0.5.0/tests/unit/mantik/cli/test_training_models.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/cli/test_utils.py` & `mantik-0.5.0/tests/unit/mantik/cli/test_utils.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/compute_backend/config/conftest.py` & `mantik-0.5.0/tests/unit/mantik/compute_backend/config/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_base.py` & `mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_base.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_core.py` & `mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -787,22 +787,21 @@
                     ),
                 ),
                 {
                     "Project": "test-project",
                     "Resources": {"Queue": "batch", "CPUsPerNode": 1},
                     "Stdout": "mantik.log",
                     "Stderr": "mantik.log",
-                    "Environment": {"TEST": "test", "SRUN_CPUS_PER_TASK": "1"},
+                    "Environment": {
+                        "TEST": "test",
+                        "SRUN_CPUS_PER_TASK": "1",
+                        "MANTIK_WORKING_DIRECTORY": "$UC_WORKING_DIRECTORY",
+                    },
                     "RunUserPrecommandOnLoginNode": True,
-                    "Executable": (
-                        "echo precommand on compute node && "
-                        "srun apptainer run test-image "
-                        "python main.py arg1 arg2 && "
-                        "echo postcommand on compute node"
-                    ),
+                    "Executable": 'source $(dirname "$(realpath "$0")")/mantik.sh',  # noqa E501
                     "Arguments": [],
                     "RunUserPostcommandOnLoginNode": True,
                 },
             ),
             (
                 compute_backend.config.core.Config(
                     unicore_api_url="not_included",
@@ -823,20 +822,24 @@
                     ),
                 ),
                 {
                     "Project": "test-project",
                     "Resources": {"Queue": "batch", "CPUsPerNode": 1},
                     "Stdout": "mantik.log",
                     "Stderr": "mantik.log",
-                    "Environment": {"TEST": "test", "SRUN_CPUS_PER_TASK": "1"},
+                    "Environment": {
+                        "TEST": "test",
+                        "SRUN_CPUS_PER_TASK": "1",
+                        "MANTIK_WORKING_DIRECTORY": "$UC_WORKING_DIRECTORY",
+                    },
                     "RunUserPrecommandOnLoginNode": True,
                     "Arguments": [],
-                    "Executable": "echo precommand on compute node && source /venv/bin/activate && python main.py arg1 arg2 && echo postcommand on compute node",  # noqa E501
+                    "Executable": 'source $(dirname "$(realpath "$0")")/mantik.sh',  # noqa E501
                     "RunUserPostcommandOnLoginNode": True,
                 },
             ),
         ],
     )
     def test_to_job_description(self, test_config, expected):
-        test_arguments_string = "python main.py arg1 arg2"
-        result = test_config.to_unicore_job_description(test_arguments_string)
+        bash_script_name = "mantik.sh"
+        result = test_config.to_unicore_job_description(bash_script_name)
         assert result == expected
```

### Comparing `mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_environment.py` & `mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_environment.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,18 +45,20 @@
                     "PreRunCommandOnLoginNode": "precommand login node",
                     "PostRunCommandOnLoginNode": "postcommand login node",
                     "PreRunCommandOnComputeNode": "precommand compute node",
                     "PostRunCommandOnComputeNode": "postcommand compute node",
                 },
                 testing.config._create_python_environment(
                     path=pathlib.Path("/path/to/venv"),
-                    pre_run_command_on_login_node="precommand login node",
-                    post_run_command_on_login_node="postcommand login node",
-                    pre_run_command_on_compute_node="precommand compute node",
-                    post_run_command_on_compute_node="postcommand compute node",
+                    pre_run_command_on_login_node=["precommand login node"],
+                    post_run_command_on_login_node=["postcommand login node"],
+                    pre_run_command_on_compute_node=["precommand compute node"],
+                    post_run_command_on_compute_node=[
+                        "postcommand compute node"
+                    ],
                 ),
             ),
         ],
     )
     def test_from_dict(
         self, monkeypatch, expect_raise_if_exception, env_vars, d, expected
     ):
@@ -119,141 +121,170 @@
                 None,
             ),
             # Test case: Apptainer with no modules and precommand
             (
                 testing.config._create_apptainer_environment(
                     modules=None,
                     path=pathlib.Path("/path/to/venv"),
-                    pre_run_command_on_compute_node="a precommand",
+                    pre_run_command_on_compute_node=[
+                        "a precommand",
+                        "another precommand",
+                    ],
                 ),
-                "a precommand",
+                "a precommand\nanother precommand",
             ),
             # Test case: Apptainer with 1 module and no precommand
             (
                 testing.config._create_apptainer_environment(
                     modules=["Module"], path=pathlib.Path("/path/to/venv")
                 ),
                 "module load Module",
             ),
             # Test case: Apptainer with 1 module and precommand
             (
                 testing.config._create_apptainer_environment(
                     modules=["Module"],
                     path=pathlib.Path("/path/to/venv"),
-                    pre_run_command_on_compute_node="a precommand",
+                    pre_run_command_on_compute_node=[
+                        "a precommand",
+                        "another precommand",
+                    ],
                 ),
-                "module load Module && a precommand",
+                "module load Module\na precommand\nanother precommand",
             ),
             # Test case: Apptainer with 2 modules and no precommand
             (
                 testing.config._create_apptainer_environment(
                     modules=["Module"], path=pathlib.Path("/path/to/venv")
                 ),
                 "module load Module",
             ),
-            # Test case: Apptainer with 2 modules and precommand
+            # Test case: Apptainer with 2 modules and precommand as a list
             (
                 testing.config._create_apptainer_environment(
                     modules=["Module1", "Module2"],
                     path=pathlib.Path("/path/to/venv"),
-                    pre_run_command_on_compute_node="a precommand",
+                    pre_run_command_on_compute_node=[
+                        "a precommand",
+                        "another precommand",
+                    ],
                 ),
-                "module load Module1 Module2 && a precommand",
+                "module load Module1 Module2\na precommand\n"
+                "another precommand",
             ),
             # Test case: Python with no modules and no precommand
             (
                 testing.config._create_python_environment(
                     modules=None, path=pathlib.Path("/path/to/venv")
                 ),
                 None,
             ),
             # Test case: Python with no modules and precommand
             (
                 testing.config._create_python_environment(
                     modules=None,
                     path=pathlib.Path("/path/to/venv"),
-                    pre_run_command_on_compute_node="a precommand",
+                    pre_run_command_on_compute_node=[
+                        "a precommand",
+                        "another precommand",
+                    ],
                 ),
-                "a precommand",
+                "a precommand\nanother precommand",
             ),
             # Test case: Python with 1 module and no precommand
             (
                 testing.config._create_python_environment(
                     modules=["Module"],
                     path=pathlib.Path("/path/to/venv"),
                 ),
                 "module load Module",
             ),
             # Test case: Python with 1 module and precommand
             (
                 testing.config._create_python_environment(
                     modules=["Module"],
                     path=pathlib.Path("/path/to/venv"),
-                    pre_run_command_on_compute_node="a precommand",
+                    pre_run_command_on_compute_node=[
+                        "a precommand",
+                        "another precommand",
+                    ],
                 ),
-                "module load Module && a precommand",
+                "module load Module\na precommand\nanother precommand",
             ),
             # Test case: Python with 2 modules and no precommand
             (
                 testing.config._create_python_environment(
                     modules=["Module1", "Module2"],
                     path=pathlib.Path("/path/to/venv"),
                 ),
                 "module load Module1 Module2",
             ),
             # Test case: Python with 2 modules and precommand
             (
                 testing.config._create_python_environment(
                     modules=["Module1", "Module2"],
                     path=pathlib.Path("/path/to/venv"),
-                    pre_run_command_on_compute_node="a precommand",
+                    pre_run_command_on_compute_node=[
+                        "a precommand",
+                        "another precommand",
+                    ],
                 ),
-                "module load Module1 Module2 && a precommand",
+                "module load Module1 Module2\na precommand\n"
+                "another precommand",
             ),
             # Test case: No execution environment
             (
                 environment.Environment(
                     modules=["Module1", "Module2"],
-                    pre_run_command_on_compute_node="a precommand",
+                    pre_run_command_on_compute_node=[
+                        "a precommand",
+                        "another precommand",
+                    ],
                 ),
-                "module load Module1 Module2 && a precommand",
+                "module load Module1 Module2\na precommand\n"
+                "another precommand",
             ),
         ],
     )
     def test_create_precommand_on_compute_node(self, env, expected):
         result = env._create_pre_run_command_on_compute_node()
 
         assert expected == result
 
     def test_create_postcommand_on_login_node(self):
-        expected = "a postcommand"
+        expected = "a postcommand && another postcommand"
         env = testing.config._create_python_environment(
             path=pathlib.Path("/path/to/venv"),
-            post_run_command_on_login_node="a postcommand",
+            post_run_command_on_login_node=[
+                "a postcommand",
+                "another postcommand",
+            ],
         )
 
-        result = env.post_run_command_on_login_node
+        result = env._create_login_node_command(
+            env.post_run_command_on_login_node
+        )
 
         assert expected == result
 
     @pytest.mark.parametrize(
         (
             "env",
             "expected",
         ),
         [
             # Test case: No execution environment
             (
                 environment.Environment(
                     modules=["Module1", "Module2"],
-                    pre_run_command_on_compute_node="a precommand",
-                    post_run_command_on_compute_node="a postcommand",
+                    pre_run_command_on_compute_node=["a precommand"],
+                    post_run_command_on_compute_node=["a postcommand"],
                 ),
                 (
-                    "module load Module1 Module2 && "
+                    "module load Module1 Module2\n"
                     "a precommand && "
                     "python main.py test && "
                     "a postcommand"
                 ),
             ),
             # Test case: Apptainer with no precommand, no postcommand, no modules # noqa E501
             (
@@ -263,20 +294,21 @@
                 "srun apptainer run venv python main.py test",
             ),
             # Test case: Apptainer with a precommand, a postcommand and modules
             (
                 testing.config._create_apptainer_environment(
                     path=pathlib.Path("/path/to/venv"),
                     modules=["Module1", "Module2"],
-                    pre_run_command_on_compute_node="a precommand",
-                    post_run_command_on_compute_node="a postcommand",
+                    pre_run_command_on_compute_node=["a precommand"],
+                    post_run_command_on_compute_node=["a postcommand"],
                 ),
                 (
-                    "module load Module1 Module2 && "
-                    "a precommand && srun apptainer run venv "
+                    "module load Module1 Module2\n"
+                    "a precommand && "
+                    "srun apptainer run venv "
                     "python main.py test && "
                     "a postcommand"
                 ),
             ),
             # Test case: Python with no precommand, no postcommand, no modules
             (
                 testing.config._create_python_environment(
@@ -285,21 +317,23 @@
                 "source /path/to/venv/bin/activate && python main.py test",
             ),
             # Test case: Python with a precommand, a postcommand and modules
             (
                 testing.config._create_python_environment(
                     path=pathlib.Path("/path/to/venv"),
                     modules=["Module1", "Module2"],
-                    pre_run_command_on_compute_node="a precommand",
-                    post_run_command_on_compute_node="a postcommand",
+                    pre_run_command_on_compute_node=["a precommand"],
+                    post_run_command_on_compute_node=["a postcommand"],
                 ),
                 (
-                    "module load Module1 Module2 && "
-                    "a precommand && source /path/to/venv/bin/activate && "
-                    "python main.py test && a postcommand"
+                    "module load Module1 Module2\n"
+                    "a precommand && "
+                    "source /path/to/venv/bin/activate && "
+                    "python main.py test && "
+                    "a postcommand"
                 ),
             ),
         ],
     )
     def test_create_execution_command_with_arguments(self, env, expected):
         entry_point_arguments = "python main.py test"
         result = env._create_execution_command_with_arguments(
@@ -375,68 +409,80 @@
             # Test case: Apptainer with no modules and no env vars
             (
                 testing.config._create_apptainer_environment(
                     modules=None,
                     path=pathlib.Path("/path/to/venv"),
                     include_mlflow_env_vars=False,
                 ),
-                "srun apptainer run venv python main.py test",
+                (
+                    "export MANTIK_WORKING_DIRECTORY=/test-scratch-dir/test-user-name/mantik/test-run-dir\n"  # noqa E501
+                    "srun apptainer run venv python main.py test"
+                ),
             ),
             # Test case: Apptainer with 1 module and env vars
             (
                 testing.config._create_apptainer_environment(
                     modules=["Module"],
                     path=pathlib.Path("/path/to/venv"),
                     variables={"TEST_ENV_VAR": "test-value"},
                     include_mlflow_env_vars=False,
                 ),
                 (
+                    "export MANTIK_WORKING_DIRECTORY=/test-scratch-dir/test-user-name/mantik/test-run-dir\n"  # noqa E501
                     "export TEST_ENV_VAR=test-value\n"
                     "module load Module && "
                     "srun apptainer run venv python main.py test"
                 ),
             ),
             # Test case: Python with no modules and no env vars
             (
                 testing.config._create_python_environment(
                     modules=None,
                     path=pathlib.Path("/path/to/venv"),
                     include_mlflow_env_vars=False,
                 ),
-                "source /path/to/venv/bin/activate && python main.py test",
+                (
+                    "export MANTIK_WORKING_DIRECTORY=/test-scratch-dir/test-user-name/mantik/test-run-dir\n"  # noqa E501
+                    "source /path/to/venv/bin/activate && python main.py test"
+                ),
             ),
             # Test case: Python with 1 module and env vars
             (
                 testing.config._create_python_environment(
                     modules=["Module"],
                     path=pathlib.Path("/path/to/venv"),
                     variables={"TEST_ENV_VAR": "test-value"},
                     include_mlflow_env_vars=False,
                 ),
                 (
+                    "export MANTIK_WORKING_DIRECTORY=/test-scratch-dir/test-user-name/mantik/test-run-dir\n"  # noqa E501
                     "export TEST_ENV_VAR=test-value\n"
                     "module load Module && "
                     "source /path/to/venv/bin/activate && "
                     "python main.py test"
                 ),
             ),
             # Test case: No execution environment
             (
                 environment.Environment(
                     modules=["Module1", "Module2"],
                     variables={"TEST_ENV_VAR": "test-value"},
                 ),
                 (
+                    "export MANTIK_WORKING_DIRECTORY=/test-scratch-dir/test-user-name/mantik/test-run-dir\n"  # noqa E501
                     "export TEST_ENV_VAR=test-value\n"
                     "module load Module1 Module2 && "
                     "python main.py test"
                 ),
             ),
         ],
     )
     def test_to_slurm_batch_script(self, env, expected):
         entry_point_arguments = "python main.py test"
         result = env.to_slurm_batch_script(
-            entry_point_arguments=entry_point_arguments
+            entry_point_arguments=entry_point_arguments,
+            run_dir=pathlib.Path(
+                "/test-scratch-dir/test-user-name/mantik/test-run-dir"
+            ),
         )
 
         assert result == expected
```

### Comparing `mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_executable.py` & `mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_executable.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_resources.py` & `mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_resources.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_utils_config.py` & `mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_utils_config.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/compute_backend/config/test_validate.py` & `mantik-0.5.0/tests/unit/mantik/compute_backend/config/test_validate.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/compute_backend/test_compute_backend_client.py` & `mantik-0.5.0/tests/unit/mantik/compute_backend/test_compute_backend_client.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/conftest.py` & `mantik-0.5.0/tests/unit/mantik/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/remote_file_service/conftest.py` & `mantik-0.5.0/tests/unit/mantik/remote_file_service/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/remote_file_service/test_data_client.py` & `mantik-0.5.0/tests/unit/mantik/remote_file_service/test_data_client.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/remote_file_service/test_s3_file_service.py` & `mantik-0.5.0/tests/unit/mantik/remote_file_service/test_s3_file_service.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/remote_file_service/test_unicore_file_service.py` & `mantik-0.5.0/tests/unit/mantik/remote_file_service/test_unicore_file_service.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/runs/test_artifacts.py` & `mantik-0.5.0/tests/unit/mantik/runs/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/runs/test_local.py` & `mantik-0.5.0/tests/unit/mantik/runs/test_local.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/tracking/test_track.py` & `mantik-0.5.0/tests/unit/mantik/tracking/test_track.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/utils/conftest.py` & `mantik-0.5.0/tests/unit/mantik/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/utils/mantik_api/test_mantik_api.py` & `mantik-0.5.0/tests/unit/mantik/utils/mantik_api/test_mantik_api.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/utils/mantik_api/test_mantik_api_code.py` & `mantik-0.5.0/tests/unit/mantik/utils/mantik_api/test_mantik_api_code.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/utils/mantik_api/test_mantik_api_experiment.py` & `mantik-0.5.0/tests/unit/mantik/utils/mantik_api/test_mantik_api_experiment.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/utils/mantik_api/test_mantik_api_models.py` & `mantik-0.5.0/tests/unit/mantik/utils/mantik_api/test_mantik_api_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import uuid
 
 import pytest
 import requests
 
 import mantik.utils.mantik_api.models as models
 
@@ -124,48 +125,97 @@
         )
     if error:
         assert any(
             "Call to Mantik API" in message for message in info_caplog.messages
         )
 
 
-def test_create_model_entry(
+@pytest.mark.parametrize(
+    ("model", "error", "extra_logs"),
+    [
+        (
+            models.PostPutModel(
+                uri="s3://bucket/item.type",
+                location="S3",
+                connection_id=uuid.uuid4(),
+                mlflow_parameters={},
+                name="test-name",
+            ),
+            None,
+            None,
+        ),
+        (
+            models.PostPutModel(
+                connection_id=uuid.uuid4(),
+                mlflow_parameters={},
+                name="test-name",
+                run_id=uuid.uuid4(),
+            ),
+            None,
+            None,
+        ),
+        (
+            models.PostPutModel(
+                connection_id=uuid.uuid4(),
+                mlflow_parameters={},
+                name="test-name",
+            ),
+            models.InvalidModelError,
+            None,
+        ),
+        (
+            models.PostPutModel(
+                uri="s3://bucket/item.type",
+                location="S3",
+                connection_id=uuid.uuid4(),
+                mlflow_parameters={},
+                name="test-name",
+                run_id=uuid.uuid4(),
+            ),
+            None,
+            "If both (run ID) and "
+            "(uri and location) are defined the (run ID) takes precedence, "
+            "and (uri and location) will be overwritten.",
+        ),
+    ],
+)
+def test_add_model_entry(
     mock_mantik_api_request,
     add_data_repository,
     info_caplog,
     project_id,
     model_id,
+    model,
+    error,
+    extra_logs,
 ):
-    new_model_schema = models.PostPutModel(
-        uri="s3://bucket/item.type",
-        location="S3",
-        connection_id=uuid.uuid4(),
-        mlflow_parameters={},
-        run_id=None,
-        name="test-name",
-    )
-
-    with mock_mantik_api_request(
-        method="POST",
-        end_point=f"/projects/{str(project_id)}/models/trained",
-        status_code=201,
-        json_response={"modelId": str(model_id)},
-        expected_error=None,
-    ):
-        new_model_id = models.add(
-            new_model_schema=new_model_schema,
-            project_id=project_id,
-            token="test_token",
-        )
-        assert new_model_id == model_id
-
-        assert any(
-            f"A model with ID: {model_id} has been created" in message
-            for message in info_caplog.messages
-        )
+    ctx = contextlib.nullcontext()
+    if error:
+        ctx = pytest.raises(error)
+    with ctx:
+        with mock_mantik_api_request(
+            method="POST",
+            end_point=f"/projects/{str(project_id)}/models/trained",
+            status_code=201,
+            json_response={"modelId": str(model_id)},
+            expected_error=None,
+        ):
+            new_model_id = models.add(
+                new_model_schema=model,
+                project_id=project_id,
+                token="test_token",
+            )
+            assert new_model_id == model_id
+
+            assert any(
+                f"A model with ID: {model_id} has been created" in message
+                for message in info_caplog.messages
+            )
+            if extra_logs:
+                assert extra_logs in info_caplog.messages
 
 
 @pytest.mark.parametrize(
     ("status_code", "expected"), [(200, None), (404, requests.HTTPError())]
 )
 def test_update_model(
     mock_mantik_api_request,
```

### Comparing `mantik-0.4.9/tests/unit/mantik/utils/mantik_api/test_mantik_run.py` & `mantik-0.5.0/tests/unit/mantik/utils/mantik_api/test_mantik_run.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/utils/test_env.py` & `mantik-0.5.0/tests/unit/mantik/utils/test_env.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/utils/test_urls.py` & `mantik-0.5.0/tests/unit/mantik/utils/test_urls.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik/utils/unicore/test_upload.py` & `mantik-0.5.0/tests/unit/mantik/utils/unicore/test_upload.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/conftest.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,16 +112,16 @@
         user="user",
         password="password",
         project="test-project",
         environment=compute_backend.config.environment.Environment(
             execution=compute_backend.config.executable.Python(
                 path=pathlib.Path("/venv"),
             ),
-            pre_run_command_on_compute_node="precommand compute node",
-            post_run_command_on_compute_node="postcommand compute node",
+            pre_run_command_on_compute_node=["precommand compute node"],
+            post_run_command_on_compute_node=["postcommand compute node"],
         ),
         resources=compute_backend.config.resources.Resources(queue="batch"),
         exclude=["*.sif"],
     )
 
 
 @pytest.fixture(scope="function")
@@ -192,16 +192,16 @@
         user="user",
         password="password",
         project="test-project",
         environment=compute_backend.config.environment.Environment(
             execution=compute_backend.config.executable.Python(
                 path=pathlib.Path("/venv"),
             ),
-            pre_run_command_on_compute_node="precommand compute node",
-            post_run_command_on_compute_node="postcommand compute node",
+            pre_run_command_on_compute_node=["precommand compute node"],
+            post_run_command_on_compute_node=["postcommand compute node"],
         ),
         resources=compute_backend.config.resources.Resources(
             queue="batch", node_constraints="gpu"
         ),
         exclude=["*.sif"],
     )
```

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/firecrest_backend/test_firecrest_client.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/firecrest_backend/test_firecrest_client.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/firecrest_backend/test_firecrest_connect.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/firecrest_backend/test_firecrest_connect.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/test_api.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/test_api.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/test_app.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/test_app.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/test_backend.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/test_backend.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/test_backend_firecrest.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/test_backend_firecrest.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,25 +86,26 @@
     entry_point = example_project.get_entry_point("main")
     parameters = {"print": "whatever"}
     storage_dir = "test-dir"
     run_id = str(uuid.uuid4())
     run_dir = pathlib.Path("test-dir")
     expected = "\n".join(
         [
-            "#!/bin/bash",
+            "#!/bin/bash -l",
             f"#SBATCH --job-name='mantik-{run_id}'",
             "#SBATCH --partition=batch",
             "#SBATCH --constraint=gpu",
             f"#SBATCH --output={run_dir}/mantik.log",
             f"#SBATCH --error={run_dir}/mantik.log",
             'echo "firecREST working directory is $(pwd)"',
             'echo "Submitted batch script:"',
             "cat $(pwd)/script.batch",
             'echo "Changing to Mantik run directory test-dir"',
             f"cd {run_dir}",
+            "export MANTIK_WORKING_DIRECTORY=test-dir",
             "srun apptainer run mantik-test.sif python main.py whatever",
         ]
     )
 
     arguments = backend._create_arguments(
         entry_point=entry_point, parameters=parameters, storage_dir=storage_dir
     )
@@ -125,15 +126,15 @@
     entry_point = example_project.get_entry_point("main")
     parameters = {"print": "whatever"}
     storage_dir = "test-dir"
     run_id = str(uuid.uuid4())
     run_dir = pathlib.Path("test-dir")
     expected = "\n".join(
         [
-            "#!/bin/bash",
+            "#!/bin/bash -l",
             f"#SBATCH --job-name='mantik-{run_id}'",
             "#SBATCH --partition=batch",
             "#SBATCH --time=0-01:00:00",
             "#SBATCH --nodes=1",
             "#SBATCH --ntasks=1",
             "#SBATCH --ntasks-per-node=1",
             "#SBATCH --gpus-per-node=1",
@@ -144,14 +145,15 @@
             "#SBATCH --output=test-dir/mantik.log",
             "#SBATCH --error=test-dir/mantik.log",
             'echo "firecREST working directory is $(pwd)"',
             'echo "Submitted batch script:"',
             "cat $(pwd)/script.batch",
             'echo "Changing to Mantik run directory test-dir"',
             f"cd {run_dir}",
+            "export MANTIK_WORKING_DIRECTORY=test-dir",
             "export SRUN_CPUS_PER_TASK=1",
             "srun apptainer run mantik-test.sif python main.py whatever",
         ]
     )
 
     arguments = backend._create_arguments(
         entry_point=entry_point, parameters=parameters, storage_dir=storage_dir
@@ -171,25 +173,26 @@
     entry_point = example_project.get_entry_point("multi-line")
     parameters = {"print": "whatever"}
     storage_dir = "test-dir"
     run_id = str(uuid.uuid4())
     run_dir = pathlib.Path("test-dir")
     expected = "\n".join(
         [
-            "#!/bin/bash",
+            "#!/bin/bash -l",
             f"#SBATCH --job-name='mantik-{run_id}'",
             "#SBATCH --partition=batch",
             "#SBATCH --constraint=gpu",
             f"#SBATCH --output={run_dir}/mantik.log",
             f"#SBATCH --error={run_dir}/mantik.log",
             'echo "firecREST working directory is $(pwd)"',
             'echo "Submitted batch script:"',
             "cat $(pwd)/script.batch",
             'echo "Changing to Mantik run directory test-dir"',
             f"cd {run_dir}",
+            "export MANTIK_WORKING_DIRECTORY=test-dir",
             (
                 "srun apptainer run mantik-test.sif python main.py whatever  "
                 "--o option1  --i option2"
             ),
         ]
     )
 
@@ -210,28 +213,29 @@
     entry_point = example_project.get_entry_point("main")
     parameters = {"print": "whatever"}
     storage_dir = "test-dir"
     run_id = str(uuid.uuid4())
     run_dir = pathlib.Path("test-dir")
     expected = "\n".join(
         [
-            "#!/bin/bash",
+            "#!/bin/bash -l",
             f"#SBATCH --job-name='mantik-{run_id}'",
             "#SBATCH --partition=batch",
             "#SBATCH --constraint=gpu",
             f"#SBATCH --output={run_dir}/mantik.log",
             f"#SBATCH --error={run_dir}/mantik.log",
             'echo "firecREST working directory is $(pwd)"',
             'echo "Submitted batch script:"',
             "cat $(pwd)/script.batch",
             'echo "Changing to Mantik run directory test-dir"',
             f"cd {run_dir}",
-            "precommand compute node && "
-            "source /venv/bin/activate && python main.py whatever && "
-            "postcommand compute node",
+            "export MANTIK_WORKING_DIRECTORY=test-dir",
+            "precommand compute node && source /venv/bin/activate "
+            "&& python main.py "
+            "whatever && postcommand compute node",
         ]
     )
 
     arguments = backend._create_arguments(
         entry_point=entry_point, parameters=parameters, storage_dir=storage_dir
     )
     result = example_firecrest_config_for_python.to_slurm_batch_script(
```

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/test_backend_unicore.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/test_backend_unicore.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import functools
 import json
 import pathlib
 
 import mlflow.projects as projects
+import pytest
 import pyunicore.client
 
 import mantik.compute_backend.config.core as core
 import mantik.compute_backend.credentials as _credentials
 import mantik.testing as testing
 import mantik.utils as mantik_utils
 import mantik_compute_backend.backend as backend
@@ -95,121 +96,135 @@
     )
     parameters = {"print": "test"}
     apptainer_image = example_project_path / "mantik-test.sif"
     backend._submit_job_and_upload_input_files(
         project=example_project,
         entry_point="main",
         parameters=parameters,
+        project_dir=example_project_path,
         storage_dir="",
         input_files=[apptainer_image],
         config=example_unicore_config,
         run_id="example_run_id",
     )
 
+    assert pathlib.Path(example_project_path / "mantik.sh").exists()
+
 
 def test_create_job_description_apptainer(
     example_project_path, example_project, example_unicore_config
 ):
-    entry_point = example_project.get_entry_point("main")
-    parameters = {"print": "whatever"}
-    storage_dir = "test-dir"
     expected = {
-        "Executable": (
-            "srun apptainer run mantik-test.sif python main.py whatever"
-        ),
+        "Executable": 'source $(dirname "$(realpath "$0")")/mantik.sh',
         "Arguments": [],
         "Project": "test-project",
         "Resources": {"Queue": "batch"},
         "RunUserPrecommandOnLoginNode": True,
         "RunUserPostcommandOnLoginNode": True,
         "Stderr": "mantik.log",
         "Stdout": "mantik.log",
     }
-    arguments = backend._create_arguments(
-        entry_point=entry_point, parameters=parameters, storage_dir=storage_dir
-    )
+
     result = example_unicore_config.to_unicore_job_description(
-        arguments=arguments
+        bash_script_name="mantik.sh"
     )
 
     # Environment contains additional MLFLOW env vars,
     # which depend on the execution environment
-    expected_environment = {"SRUN_CPUS_PER_TASK": 100}
+    expected_environment = {
+        "SRUN_CPUS_PER_TASK": 100,
+        "MANTIK_WORKING_DIRECTORY": "$UC_WORKING_DIRECTORY",
+    }
     actual_environment = result.pop("Environment")
     assert all(
         actual_environment[key] == value
         for key, value in expected_environment.items()
     )
 
     assert result == expected
 
 
-def test_create_job_description_apptainer_entry_point_multi_line(
-    example_project_path, example_project, example_unicore_config
+def test_create_job_description_python(
+    example_project_path, example_project, example_unicore_config_for_python
 ):
-    entry_point = example_project.get_entry_point("multi-line")
-    parameters = {"print": "whatever"}
-    storage_dir = "test-dir"
     expected = {
-        "Executable": (
-            "srun apptainer run mantik-test.sif python main.py whatever  "
-            "--o option1  --i option2"
-        ),
+        "Executable": 'source $(dirname "$(realpath "$0")")/mantik.sh',
         "Arguments": [],
         "Project": "test-project",
         "Resources": {"Queue": "batch"},
         "RunUserPrecommandOnLoginNode": True,
         "RunUserPostcommandOnLoginNode": True,
         "Stderr": "mantik.log",
         "Stdout": "mantik.log",
     }
-    arguments = backend._create_arguments(
-        entry_point=entry_point, parameters=parameters, storage_dir=storage_dir
-    )
-    result = example_unicore_config.to_unicore_job_description(
-        arguments=arguments
+    result = example_unicore_config_for_python.to_unicore_job_description(
+        bash_script_name="mantik.sh"
     )
 
     # Environment contains additional MLFLOW env vars,
     # which depend on the execution environment
-    expected_environment = {"SRUN_CPUS_PER_TASK": 100}
+    expected_environment = {"MANTIK_WORKING_DIRECTORY": "$UC_WORKING_DIRECTORY"}
     actual_environment = result.pop("Environment")
     assert all(
         actual_environment[key] == value
         for key, value in expected_environment.items()
     )
 
     assert result == expected
 
 
-def test_create_job_description_python(
-    example_project_path, example_project, example_unicore_config_for_python
+@pytest.mark.parametrize(
+    ("entry_point", "config", "expected"),
+    [
+        (
+            "main",
+            "example_unicore_config_for_python",
+            (
+                "echo 'Submitted bash script'\n"
+                'cat "$(realpath "$0")"\n'
+                "precommand compute node && source /venv/bin/activate "
+                "&& python main.py "
+                "whatever && postcommand compute node"
+            ),
+        ),
+        (
+            "main",
+            "example_unicore_config",
+            (
+                "echo 'Submitted bash script'\n"
+                'cat "$(realpath "$0")"\n'
+                "srun apptainer run mantik-test.sif python main.py whatever"
+            ),
+        ),
+        (
+            "multi-line",
+            "example_unicore_config",
+            (
+                "echo 'Submitted bash script'\n"
+                'cat "$(realpath "$0")"\n'
+                "srun apptainer run mantik-test.sif python main.py whatever  "
+                "--o option1  --i option2"
+            ),
+        ),
+    ],
+)
+def test_to_bash_script(
+    request,
+    example_project_path,
+    example_project,
+    entry_point,
+    config,
+    expected,
 ):
-    entry_point = example_project.get_entry_point("main")
+    config = request.getfixturevalue(config)
+
+    entry_point = example_project.get_entry_point(entry_point)
     parameters = {"print": "whatever"}
     storage_dir = "test-dir"
-    expected = {
-        "Executable": (
-            "precommand compute node && "
-            "source /venv/bin/activate && python main.py whatever && "
-            "postcommand compute node"
-        ),
-        "Arguments": [],
-        "Project": "test-project",
-        "Resources": {"Queue": "batch"},
-        "RunUserPrecommandOnLoginNode": True,
-        "RunUserPostcommandOnLoginNode": True,
-        "Stderr": "mantik.log",
-        "Stdout": "mantik.log",
-    }
+
     arguments = backend._create_arguments(
         entry_point=entry_point, parameters=parameters, storage_dir=storage_dir
     )
-    result = example_unicore_config_for_python.to_unicore_job_description(
-        arguments=arguments
-    )
 
-    # Removing Environment for assertion since it contains additional MLFLOW
-    # env vars, which depend on the execution environment
-    result.pop("Environment", None)
+    result = config.to_bash_script(arguments)
 
     assert result == expected
```

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/test_client.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/test_client.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/test_exception_handler.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/test_exception_handler.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/test_handle_submit_run.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/test_handle_submit_run.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/test_submitted_run.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/test_submitted_run.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik_compute_backend/unicore/test_unicore_connect.py` & `mantik-0.5.0/tests/unit/mantik_compute_backend/unicore/test_unicore_connect.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mantik_with_mlflow/test_mlflow_installed.py` & `mantik-0.5.0/tests/unit/mantik_with_mlflow/test_mlflow_installed.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mlflow_tracking_server/conftest.py` & `mantik-0.5.0/tests/unit/mlflow_tracking_server/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mlflow_tracking_server/flask/conftest.py` & `mantik-0.5.0/tests/unit/mlflow_tracking_server/flask/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mlflow_tracking_server/flask/test_after_request.py` & `mantik-0.5.0/tests/unit/mlflow_tracking_server/flask/test_after_request.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mlflow_tracking_server/flask/test_flask_app.py` & `mantik-0.5.0/tests/unit/mlflow_tracking_server/flask/test_flask_app.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/mlflow_tracking_server/flask/test_rbac.py` & `mantik-0.5.0/tests/unit/mlflow_tracking_server/flask/test_rbac.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/tests/unit/tokens/test_verifier.py` & `mantik-0.5.0/tests/unit/tokens/test_verifier.py`

 * *Files identical despite different names*

### Comparing `mantik-0.4.9/PKG-INFO` & `mantik-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mantik
-Version: 0.4.9
+Version: 0.5.0
 Summary: mantik for mlflow
 Home-page: https://mantik.ai/
 License: MIT
 Keywords: mlflow,machine learning,hpc,unicore
 Author: Fabian Emmerich
 Author-email: fabian.emmerich@4-cast.de
 Maintainer: Elia Boscaini
@@ -38,18 +38,18 @@
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: pyunicore[crypto,fs,fuse] (>=0.15.0,<0.16.0) ; extra == "unicore" or extra == "all"
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Project-URL: Documentation, https://mantik-ai.gitlab.io/mantik
 Project-URL: Repository, https://gitlab.com/mantik-ai/mantik
 Description-Content-Type: text/markdown
 
-# mantik - plugin for MLflow with HPC (UNICORE)
+# Mantik - Enhancing Machine Learning Development on HPC
 
 Mantik allows to manage the full Machine Learning workflow on HPC by
-supporting MLflow and deployment of applications to HPC.
+supporting MLflow and deployment of applications to HPC via the [Mantik platform](https://cloud.mantik.ai).
 
 For a quickstart see [our documentation](https://mantik-ai.gitlab.io/mantik/client-quickstart.html)
 
 ## Extra Dependencies
 
 By default, mantik only installs the core dependencies required to use the Mantik API.
 However, additional extras are provided and can be installed:
@@ -79,7 +79,8 @@
   ```
 
 ## Helpdesk
 
 For bug reports or feature requests, please email our helpdesk.
 Details can be found [here](https://mantik-ai.gitlab.io/mantik/helpdesk.html).
 
+
```

