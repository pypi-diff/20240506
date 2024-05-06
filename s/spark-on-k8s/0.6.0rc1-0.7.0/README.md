# Comparing `tmp/spark_on_k8s-0.6.0rc1.tar.gz` & `tmp/spark_on_k8s-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_on_k8s-0.6.0rc1.tar", max compression
+gzip compressed data, was "spark_on_k8s-0.7.0.tar", max compression
```

## Comparing `spark_on_k8s-0.6.0rc1.tar` & `spark_on_k8s-0.7.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0    11357 2024-05-04 14:15:07.228942 spark_on_k8s-0.6.0rc1/LICENSE
--rw-r--r--   0        0        0    11213 2024-05-04 14:15:07.228942 spark_on_k8s-0.6.0rc1/README.md
--rw-r--r--   0        0        0     2371 2024-05-04 14:15:21.952981 spark_on_k8s-0.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0       58 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/__init__.py
--rw-r--r--   0        0        0        0 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/airflow/__init__.py
--rw-r--r--   0        0        0    17061 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/airflow/operators.py
--rw-r--r--   0        0        0     3114 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/airflow/triggers.py
--rw-r--r--   0        0        0     1190 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/__init__.py
--rw-r--r--   0        0        0     1744 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/app.py
--rw-r--r--   0        0        0     1472 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/apps.py
--rw-r--r--   0        0        0      728 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/configuration.py
--rw-r--r--   0        0        0     1305 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/main.py
--rw-r--r--   0        0        0     6750 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/__init__.py
--rw-r--r--   0        0        0      587 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/static/app_logs.css
--rw-r--r--   0        0        0      758 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/static/apps.css
--rw-r--r--   0        0        0     1416 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/templates/app_logs.html
--rw-r--r--   0        0        0     2953 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/templates/apps.html
--rw-r--r--   0        0        0      368 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/templates/error.html
--rw-r--r--   0        0        0      542 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/__init__.py
--rw-r--r--   0        0        0     1621 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/api.py
--rw-r--r--   0        0        0     6601 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/app.py
--rw-r--r--   0        0        0      690 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/apps.py
--rw-r--r--   0        0        0      553 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/namespace.py
--rw-r--r--   0        0        0     8686 2024-05-04 14:15:07.232942 spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/options.py
--rw-r--r--   0        0        0    27728 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/client.py
--rw-r--r--   0        0        0        0 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/k8s/__init__.py
--rw-r--r--   0        0        0     3135 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/k8s/async_client.py
--rw-r--r--   0        0        0     2849 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/k8s/sync_client.py
--rw-r--r--   0        0        0        0 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/__init__.py
--rw-r--r--   0        0        0    19764 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/app_manager.py
--rw-r--r--   0        0        0     9617 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/async_app_manager.py
--rw-r--r--   0        0        0     4048 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/configuration.py
--rw-r--r--   0        0        0      488 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/logging_mixin.py
--rw-r--r--   0        0        0     3956 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/setup_namespace.py
--rw-r--r--   0        0        0      842 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/spark_app_status.py
--rw-r--r--   0        0        0      141 2024-05-04 14:15:07.236942 spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/types.py
--rw-r--r--   0        0        0    13063 1970-01-01 00:00:00.000000 spark_on_k8s-0.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-06 12:45:08.017305 spark_on_k8s-0.7.0/LICENSE
+-rw-r--r--   0        0        0    12033 2024-05-06 12:45:08.017305 spark_on_k8s-0.7.0/README.md
+-rw-r--r--   0        0        0     2574 2024-05-06 12:45:23.505297 spark_on_k8s-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/airflow/__init__.py
+-rw-r--r--   0        0        0     2110 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/airflow/operator_links.py
+-rw-r--r--   0        0        0    18482 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/airflow/operators.py
+-rw-r--r--   0        0        0     3114 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/airflow/triggers.py
+-rw-r--r--   0        0        0     1253 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/__init__.py
+-rw-r--r--   0        0        0     1762 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/app.py
+-rw-r--r--   0        0        0     1472 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/apps.py
+-rw-r--r--   0        0        0      728 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/configuration.py
+-rw-r--r--   0        0        0     1305 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/main.py
+-rw-r--r--   0        0        0      524 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/utils.py
+-rw-r--r--   0        0        0     6750 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/__init__.py
+-rw-r--r--   0        0        0      587 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/static/app_logs.css
+-rw-r--r--   0        0        0      758 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/static/apps.css
+-rw-r--r--   0        0        0     1416 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/templates/app_logs.html
+-rw-r--r--   0        0        0     2953 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/templates/apps.html
+-rw-r--r--   0        0        0      368 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/templates/error.html
+-rw-r--r--   0        0        0      542 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/cli/__init__.py
+-rw-r--r--   0        0        0     1621 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/cli/api.py
+-rw-r--r--   0        0        0     6601 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/cli/app.py
+-rw-r--r--   0        0        0      690 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/cli/apps.py
+-rw-r--r--   0        0        0      553 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/cli/namespace.py
+-rw-r--r--   0        0        0     8686 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/cli/options.py
+-rw-r--r--   0        0        0    27728 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/client.py
+-rw-r--r--   0        0        0        0 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/k8s/__init__.py
+-rw-r--r--   0        0        0     3135 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/k8s/async_client.py
+-rw-r--r--   0        0        0     2849 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/k8s/sync_client.py
+-rw-r--r--   0        0        0        0 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/__init__.py
+-rw-r--r--   0        0        0    19764 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/app_manager.py
+-rw-r--r--   0        0        0     9617 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/async_app_manager.py
+-rw-r--r--   0        0        0     4048 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/configuration.py
+-rw-r--r--   0        0        0      488 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/logging_mixin.py
+-rw-r--r--   0        0        0     3956 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/setup_namespace.py
+-rw-r--r--   0        0        0      842 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/spark_app_status.py
+-rw-r--r--   0        0        0      141 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/types.py
+-rw-r--r--   0        0        0    13880 1970-01-01 00:00:00.000000 spark_on_k8s-0.7.0/PKG-INFO
```

### Comparing `spark_on_k8s-0.6.0rc1/LICENSE` & `spark_on_k8s-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/README.md` & `spark_on_k8s-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+[![PyPI - Package Version](https://img.shields.io/pypi/v/spark-on-k8s)](https://pypi.org/project/spark-on-k8s)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spark-on-k8s)](https://pypi.org/project/spark-on-k8s)
+[![PyPI - Python Version](https://img.shields.io/pypi/l/spark-on-k8s)](https://github.com/hussein-awala/spark-on-k8s/blob/main/LICENSE)
+[![CI workflow](https://github.com/hussein-awala/spark-on-k8s/actions/workflows/ci.yml/badge.svg)](https://github.com/hussein-awala/spark-on-k8s/actions/workflows/ci.yml)
+[![OpenSSF Best Practices](https://www.bestpractices.dev/projects/8883/badge)](https://www.bestpractices.dev/projects/8883)
+[![codecov](https://codecov.io/gh/hussein-awala/spark-on-k8s/branch/main/graph/badge.svg?token=Z9YN7L7VMH)](https://codecov.io/gh/hussein-awala/spark-on-k8s)
+
 # Spark On Kubernetes
 
 Spark on Kubernetes is a python package that makes it easy to submit and manage spark apps on Kubernetes.
 It provides a Python client that can be used to submit apps in your API or scheduler of choice, and a CLI
 that can be used to submit apps from the command line, instead of  using spark-submit.
 
 It also provides an optional REST API with a web UI that can be used to list and manage apps, and access the
```

### Comparing `spark_on_k8s-0.6.0rc1/pyproject.toml` & `spark_on_k8s-0.7.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spark-on-k8s"
-version = "0.6.0-rc.1"
+version = "0.7.0"
 description = "A Python package to submit and manage Apache Spark applications on Kubernetes."
 authors = ["Hussein Awala <hussein@awala.fr>"]
 readme = "README.md"
 repository = "https://github.com/hussein-awala/spark-on-k8s"
 keywords = ["spark", "kubernetes", "k8s", "spark-submit", "spark-on-k8s"]
 license = "Apache-2.0"
 packages = [{include = "spark_on_k8s"}]
@@ -27,16 +27,23 @@
 pendulum = {version = "<3.0.0", python = "<3.12", optional = true}
 aiohttp = {version = ">=3.9.2", optional = true}  # CVE-2024-23829, CVE-2024-23334
 websockets = {version = "^12", optional = true}
 
 [tool.poetry.dev-dependencies]
 mock = "^5.1.0"
 pytest = "^7.4.3"
+pytest-cov = "^5.0.0"
 pre-commit = "^3"
 freezegun = "^1.4.0"
+mkdocs = "^1.6.0"
+mkdocs-material = "^9.5.21"
+mkdocstrings = {version = "^0.25.1", extras = ["python"]}
+mkdocs-gen-files = "^0.5.0"
+mkdocs-literate-nav = "^0.6.1"
+helm-mkdocs = "^0.0.5"
 
 [tool.poetry.extras]
 api = ["fastapi", "kubernetes-asyncio", "uvicorn", "httpx", "jinja2", "aiohttp", "websockets"]
 airflow = ["kubernetes-asyncio", "apache-airflow", "apache-airflow-providers-cncf-kubernetes", "pendulum"]
 
 [tool.poetry.scripts]
 spark-on-k8s = "spark_on_k8s:cli.main"
```

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/airflow/operators.py` & `spark_on_k8s-0.7.0/spark_on_k8s/airflow/operators.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import contextlib
 from enum import Enum
 from typing import TYPE_CHECKING, Any
 
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
+from spark_on_k8s.airflow.operator_links import SparkOnK8SOperatorLink
 from spark_on_k8s.airflow.triggers import SparkOnK8STrigger
 from spark_on_k8s.k8s.sync_client import KubernetesClientManager
 
 if TYPE_CHECKING:
     from typing import Literal
 
     import jinja2
@@ -68,29 +69,33 @@
             as environment variables. Defaults to None.
         volumes: List of volumes to mount to the driver and/or executors.
         driver_volume_mounts: List of volume mounts to mount to the driver.
         executor_volume_mounts: List of volume mounts to mount to the executors.
         driver_node_selector: Node selector for the driver pod.
         executor_node_selector: Node selector for the executor pods.
         driver_tolerations: Tolerations for the driver pod.
+        spark_on_k8s_service_url: URL of the Spark On K8S service. Defaults to None.
         kubernetes_conn_id (str, optional): Kubernetes connection ID. Defaults to
             "kubernetes_default".
         poll_interval (int, optional): Poll interval for checking the Spark application status.
             Defaults to 10.
         deferrable (bool, optional): Whether the operator is deferrable. Defaults to False.
         on_kill_action (Literal["keep", "delete", "kill"], optional): Action to take when the
             operator is killed. Defaults to "delete".
         **kwargs: Other keyword arguments for BaseOperator.
     """
 
     _XCOM_DRIVER_POD_NAMESPACE = "driver_pod_namespace"
     _XCOM_DRIVER_POD_NAME = "driver_pod_name"
+    XCOM_SPARK_UI_LINK = "spark_ui_link"
 
     _driver_pod_name: str | None = None
 
+    operator_extra_links = (SparkOnK8SOperatorLink(),)
+
     template_fields = (
         "image",
         "app_path",
         "namespace",
         "service_account",
         "app_name",
         "app_id_suffix",
@@ -132,14 +137,15 @@
         executor_node_selector: dict[str, str] | None = None,
         driver_labels: dict[str, str] | None = None,
         executor_labels: dict[str, str] | None = None,
         driver_annotations: dict[str, str] | None = None,
         executor_annotations: dict[str, str] | None = None,
         driver_tolerations: list[k8s.V1Toleration] | None = None,
         executor_pod_template_path: str | None = None,
+        spark_on_k8s_service_url: str | None = None,
         kubernetes_conn_id: str = "kubernetes_default",
         poll_interval: int = 10,
         deferrable: bool = False,
         on_kill_action: Literal["keep", "delete", "kill"] = OnKillAction.DELETE,
         **kwargs,
     ):
         super().__init__(**kwargs)
@@ -166,14 +172,15 @@
         self.executor_node_selector = executor_node_selector
         self.driver_labels = driver_labels
         self.executor_labels = executor_labels
         self.driver_annotations = driver_annotations
         self.executor_annotations = executor_annotations
         self.driver_tolerations = driver_tolerations
         self.executor_pod_template_path = executor_pod_template_path
+        self.spark_on_k8s_service_url = spark_on_k8s_service_url
         self.kubernetes_conn_id = kubernetes_conn_id
         self.poll_interval = poll_interval
         self.deferrable = deferrable
         self.on_kill_action = on_kill_action
 
     def _render_nested_template_fields(
         self,
@@ -202,14 +209,33 @@
 
         super()._render_nested_template_fields(content, context, jinja_env, seen_oids)
 
     def _persist_pod_name(self, context: Context):
         context["ti"].xcom_push(key=self._XCOM_DRIVER_POD_NAMESPACE, value=self.namespace)
         context["ti"].xcom_push(key=self._XCOM_DRIVER_POD_NAME, value=self._driver_pod_name)
 
+    def _persist_spark_ui_link(self, context: Context):
+        if self.spark_on_k8s_service_url:
+            SparkOnK8SOperatorLink.persist_spark_ui_link(
+                context,
+                self,
+                spark_on_k8s_service_url=self.spark_on_k8s_service_url,
+                namespace=self.namespace,
+                spark_app_id=self._driver_pod_name[: -len("-driver")],
+            )
+
+    def _persist_spark_history_ui_link(self, context: Context):
+        if self.spark_on_k8s_service_url:
+            SparkOnK8SOperatorLink.persist_spark_history_ui_link(
+                context,
+                self,
+                spark_on_k8s_service_url=self.spark_on_k8s_service_url,
+                spark_app_id=self._driver_pod_name,
+            )
+
     def _try_to_adopt_job(self, context: Context, spark_app_manager: SparkAppManager) -> bool:
         from spark_on_k8s.utils.spark_app_status import SparkAppStatus
 
         xcom_driver_namespace = context["ti"].xcom_pull(key=self._XCOM_DRIVER_POD_NAMESPACE)
         if not xcom_driver_namespace or xcom_driver_namespace != self.namespace:
             return False
         xcom_driver_pod_name = context["ti"].xcom_pull(key=self._XCOM_DRIVER_POD_NAME)
@@ -302,14 +328,15 @@
         )
         spark_app_manager = SparkAppManager(
             k8s_client_manager=k8s_client_manager,
         )
         if not self._try_to_adopt_job(context, spark_app_manager):
             self._submit_new_job(context)
             self._persist_pod_name(context)
+        self._persist_spark_ui_link(context)
         if self.app_waiter == "no_wait":
             return
         if self.deferrable:
             self.defer(
                 trigger=SparkOnK8STrigger(
                     driver_pod_name=self._driver_pod_name,
                     namespace=self.namespace,
@@ -335,14 +362,15 @@
                 pod_name=self._driver_pod_name,
                 poll_interval=1,
             )
         app_status = spark_app_manager.app_status(
             namespace=self.namespace,
             pod_name=self._driver_pod_name,
         )
+        self._persist_spark_history_ui_link(context)
         if app_status == "Succeeded":
             return app_status
         raise AirflowException(f"The job finished with status: {app_status}")
 
     def execute_complete(self, context: Context, event: dict, **kwargs):
         if self.app_waiter == "log":
             from spark_on_k8s.utils.app_manager import SparkAppManager
@@ -353,24 +381,27 @@
             spark_app_manager = SparkAppManager(
                 k8s_client_manager=k8s_client_manager,
             )
             spark_app_manager.stream_logs(
                 namespace=event["namespace"],
                 pod_name=event["pod_name"],
             )
+        self._persist_spark_history_ui_link(context)
         if event["status"] == "Succeeded":
             return event["status"]
         if event["status"] == "error":
             raise AirflowException(
                 f"SparkOnK8STrigger failed: with error: {event['error']}\n"
                 f"Stacktrace: {event['stacktrace']}"
             )
         raise AirflowException(f"The job finished with status: {event['status']}")
 
     def on_kill(self) -> None:
+        from airflow.operators.python import get_current_context
+
         if self.on_kill_action == OnKillAction.KEEP:
             return
         self.log.warning(self._driver_pod_name)
         if self._driver_pod_name:
             from spark_on_k8s.utils.app_manager import SparkAppManager
 
             k8s_client_manager = _AirflowKubernetesClientManager(
@@ -389,7 +420,9 @@
                 self.log.info("Killing Spark application...")
                 spark_app_manager.kill_app(
                     namespace=self.namespace,
                     pod_name=self._driver_pod_name,
                 )
             else:
                 raise AirflowException(f"Invalid on_kill_action: {self.on_kill_action}")
+
+            self._persist_spark_history_ui_link(get_current_context())
```

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/airflow/triggers.py` & `spark_on_k8s-0.7.0/spark_on_k8s/airflow/triggers.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/__init__.py` & `spark_on_k8s-0.7.0/spark_on_k8s/api/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
+import logging
 from typing import TYPE_CHECKING
 
 from httpx import AsyncClient
 
 from spark_on_k8s.k8s.async_client import KubernetesAsyncClientManager
 from spark_on_k8s.utils.configuration import Configuration
 
 if TYPE_CHECKING:
     from kubernetes_asyncio.client import ApiClient
 
+logger = logging.getLogger("spark_on_k8s.api")
+
 
 class KubernetesClientSingleton:
     """Kubernetes client singleton."""
 
     client_manager: KubernetesAsyncClientManager = KubernetesAsyncClientManager(
         config_file=Configuration.SPARK_ON_K8S_CONFIG_FILE,
         context=Configuration.SPARK_ON_K8S_CONTEXT,
```

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/app.py` & `spark_on_k8s-0.7.0/spark_on_k8s/api/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from fastapi import APIRouter, Response
 
 from spark_on_k8s.api import KubernetesClientSingleton
+from spark_on_k8s.api.utils import handle_exception
 from spark_on_k8s.utils.async_app_manager import AsyncSparkAppManager
 
 router = APIRouter(
     prefix="/app",
     tags=["spark-app"],
 )
 
@@ -24,15 +25,15 @@
         k8s_client_manager=KubernetesClientSingleton.client_manager
     )
     try:
         await async_spark_app_manager.kill_app(namespace=namespace, app_id=app_id)
         return Response(status_code=200)
     except Exception as e:
         # TODO: handle exceptions properly and return proper status code
-        return Response(status_code=500, content=str(e))
+        return handle_exception(e, 500)
 
 
 @router.delete(
     "/{namespace}/{app_id}",
     summary="Delete a spark application",
 )
 async def delete_app(namespace: str, app_id: str, force: bool = False):
@@ -45,8 +46,8 @@
         k8s_client_manager=KubernetesClientSingleton.client_manager
     )
     try:
         await async_spark_app_manager.delete_app(namespace=namespace, app_id=app_id)
         return Response(status_code=200)
     except Exception as e:
         # TODO: handle exceptions properly and return proper status code
-        return Response(status_code=500, content=str(e))
+        return handle_exception(e, 500)
```

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/apps.py` & `spark_on_k8s-0.7.0/spark_on_k8s/api/apps.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/configuration.py` & `spark_on_k8s-0.7.0/spark_on_k8s/api/configuration.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/main.py` & `spark_on_k8s-0.7.0/spark_on_k8s/api/main.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/__init__.py` & `spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/static/app_logs.css` & `spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/static/app_logs.css`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/static/apps.css` & `spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/static/apps.css`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/templates/app_logs.html` & `spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/templates/app_logs.html`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/api/webserver/templates/apps.html` & `spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/templates/apps.html`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/__init__.py` & `spark_on_k8s-0.7.0/spark_on_k8s/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/api.py` & `spark_on_k8s-0.7.0/spark_on_k8s/cli/api.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/app.py` & `spark_on_k8s-0.7.0/spark_on_k8s/cli/app.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/apps.py` & `spark_on_k8s-0.7.0/spark_on_k8s/cli/apps.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/namespace.py` & `spark_on_k8s-0.7.0/spark_on_k8s/cli/namespace.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/cli/options.py` & `spark_on_k8s-0.7.0/spark_on_k8s/cli/options.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/client.py` & `spark_on_k8s-0.7.0/spark_on_k8s/client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/k8s/async_client.py` & `spark_on_k8s-0.7.0/spark_on_k8s/k8s/async_client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/k8s/sync_client.py` & `spark_on_k8s-0.7.0/spark_on_k8s/k8s/sync_client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/app_manager.py` & `spark_on_k8s-0.7.0/spark_on_k8s/utils/app_manager.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/async_app_manager.py` & `spark_on_k8s-0.7.0/spark_on_k8s/utils/async_app_manager.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/configuration.py` & `spark_on_k8s-0.7.0/spark_on_k8s/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/setup_namespace.py` & `spark_on_k8s-0.7.0/spark_on_k8s/utils/setup_namespace.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/spark_on_k8s/utils/spark_app_status.py` & `spark_on_k8s-0.7.0/spark_on_k8s/utils/spark_app_status.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.6.0rc1/PKG-INFO` & `spark_on_k8s-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-on-k8s
-Version: 0.6.0rc1
+Version: 0.7.0
 Summary: A Python package to submit and manage Apache Spark applications on Kubernetes.
 Home-page: https://github.com/hussein-awala/spark-on-k8s
 License: Apache-2.0
 Keywords: spark,kubernetes,k8s,spark-submit,spark-on-k8s
 Author: Hussein Awala
 Author-email: hussein@awala.fr
 Requires-Python: >=3.8,<4.0
@@ -30,14 +30,21 @@
 Requires-Dist: uvicorn (>=0.26.0,<0.27.0) ; extra == "api"
 Requires-Dist: websockets (>=12,<13) ; extra == "api"
 Project-URL: Bug Tracker, https://github.com/hussein-awala/spark-on-k8s/issues
 Project-URL: Documentation, https://github.com/hussein-awala/spark-on-k8s/blob/main/README.md
 Project-URL: Repository, https://github.com/hussein-awala/spark-on-k8s
 Description-Content-Type: text/markdown
 
+[![PyPI - Package Version](https://img.shields.io/pypi/v/spark-on-k8s)](https://pypi.org/project/spark-on-k8s)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spark-on-k8s)](https://pypi.org/project/spark-on-k8s)
+[![PyPI - Python Version](https://img.shields.io/pypi/l/spark-on-k8s)](https://github.com/hussein-awala/spark-on-k8s/blob/main/LICENSE)
+[![CI workflow](https://github.com/hussein-awala/spark-on-k8s/actions/workflows/ci.yml/badge.svg)](https://github.com/hussein-awala/spark-on-k8s/actions/workflows/ci.yml)
+[![OpenSSF Best Practices](https://www.bestpractices.dev/projects/8883/badge)](https://www.bestpractices.dev/projects/8883)
+[![codecov](https://codecov.io/gh/hussein-awala/spark-on-k8s/branch/main/graph/badge.svg?token=Z9YN7L7VMH)](https://codecov.io/gh/hussein-awala/spark-on-k8s)
+
 # Spark On Kubernetes
 
 Spark on Kubernetes is a python package that makes it easy to submit and manage spark apps on Kubernetes.
 It provides a Python client that can be used to submit apps in your API or scheduler of choice, and a CLI
 that can be used to submit apps from the command line, instead of  using spark-submit.
 
 It also provides an optional REST API with a web UI that can be used to list and manage apps, and access the
```

