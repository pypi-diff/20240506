# Comparing `tmp/apache_airflow_providers_apache_spark-4.8.0rc1.tar.gz` & `tmp/apache_airflow_providers_apache_spark-4.8.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_apache_spark-4.8.0rc1.tar", last modified: Mon Jan 22 08:25:41 2024, max compression
+gzip compressed data, was "apache_airflow_providers_apache_spark-4.8.0rc2.tar", last modified: Tue Apr 30 11:17:20 2024, max compression
```

## Comparing `apache_airflow_providers_apache_spark-4.8.0rc1.tar` & `apache_airflow_providers_apache_spark-4.8.0rc2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4217 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/LICENSE
--rw-r--r--   0        0        0     1587 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/__init__.py
--rw-r--r--   0        0        0      787 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/decorators/__init__.py
--rw-r--r--   0        0        0     4546 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/decorators/pyspark.py
--rw-r--r--   0        0        0     4451 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/__init__.py
--rw-r--r--   0        0        0     3192 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_connect.py
--rw-r--r--   0        0        0    11730 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py
--rw-r--r--   0        0        0     6753 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
--rw-r--r--   0        0        0     7906 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_sql.py
--rw-r--r--   0        0        0    32569 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_submit.py
--rw-r--r--   0        0        0      787 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/__init__.py
--rw-r--r--   0        0        0    10223 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/spark_jdbc.py
--rw-r--r--   0        0        0     4508 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/spark_sql.py
--rw-r--r--   0        0        0     9702 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/spark_submit.py
--rw-r--r--   0        0        0     3094 2024-01-22 08:25:41.000000 apache_airflow_providers_apache_spark-4.8.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6042 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_spark-4.8.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4222 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/LICENSE
+-rw-r--r--   0        0        0     1587 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/decorators/__init__.py
+-rw-r--r--   0        0        0     4546 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/decorators/pyspark.py
+-rw-r--r--   0        0        0     4493 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/hooks/__init__.py
+-rw-r--r--   0        0        0     3237 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/hooks/spark_connect.py
+-rw-r--r--   0        0        0    11730 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/hooks/spark_jdbc.py
+-rw-r--r--   0        0        0     6753 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
+-rw-r--r--   0        0        0     7917 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/hooks/spark_sql.py
+-rw-r--r--   0        0        0    32639 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/hooks/spark_submit.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/operators/__init__.py
+-rw-r--r--   0        0        0     8899 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/operators/spark_jdbc.py
+-rw-r--r--   0        0        0     4909 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/operators/spark_sql.py
+-rw-r--r--   0        0        0     9687 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/operators/spark_submit.py
+-rw-r--r--   0        0        0     3141 2024-04-30 11:17:20.000000 apache_airflow_providers_apache_spark-4.8.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     6099 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_spark-4.8.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/README.rst` & `apache_airflow_providers_apache_spark-4.8.0rc2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.8.0.rc1``
+Release: ``4.8.0.rc2``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -60,23 +60,23 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-spark``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``pyspark``
 ``grpcio-status``   ``>=1.59.0``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
```

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/LICENSE` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/__init__.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,12 +31,12 @@
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
-    "2.6.0"
+    "2.7.0"
 ):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-apache-spark:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-apache-spark:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/decorators/__init__.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/decorators/pyspark.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/decorators/pyspark.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/get_provider_info.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-spark",
         "name": "Apache Spark",
         "description": "`Apache Spark <https://spark.apache.org/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705911941,
+        "source-date-epoch": 1714475840,
         "versions": [
             "4.8.0",
+            "4.7.2",
+            "4.7.1",
             "4.7.0",
             "4.6.0",
             "4.5.0",
             "4.4.0",
             "4.3.0",
             "4.2.0",
             "4.1.5",
@@ -55,15 +57,15 @@
             "2.0.1",
             "2.0.0",
             "1.0.3",
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "pyspark", "grpcio-status>=1.59.0"],
+        "dependencies": ["apache-airflow>=2.7.0", "pyspark", "grpcio-status>=1.59.0"],
         "additional-extras": [
             {"name": "cncf.kubernetes", "dependencies": ["apache-airflow-providers-cncf-kubernetes>=7.4.0"]}
         ],
         "integrations": [
             {
                 "integration-name": "Apache Spark",
                 "external-doc-url": "https://spark.apache.org/",
```

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/__init__.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_connect.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/hooks/spark_connect.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,25 +35,25 @@
     conn_name_attr = "conn_id"
     default_conn_name = "spark_connect_default"
     conn_type = "spark_connect"
     hook_name = "Spark Connect"
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Return custom field behaviour."""
+        """Return custom UI field behaviour for Spark Connect connection."""
         return {
             "hidden_fields": [
                 "schema",
             ],
             "relabeling": {"password": "Token", "login": "User ID"},
         }
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Return connection widgets to add to Spark Connect connection form."""
         from flask_babel import lazy_gettext
         from wtforms import BooleanField
 
         return {
             SparkConnectHook.PARAM_USE_SSL: BooleanField(lazy_gettext("Use SSL"), default=False),
         }
```

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/hooks/spark_jdbc.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/hooks/spark_jdbc_script.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_sql.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/hooks/spark_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,23 +52,23 @@
     conn_name_attr = "conn_id"
     default_conn_name = "spark_sql_default"
     conn_type = "spark_sql"
     hook_name = "Spark SQL"
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Return custom field behaviour."""
+        """Return custom UI field behaviour for Spark SQL connection."""
         return {
             "hidden_fields": ["schema", "login", "password", "extra"],
             "relabeling": {},
         }
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Return connection widgets to add to Spark SQL connection form."""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import StringField
         from wtforms.validators import Optional
 
         return {
             "queue": StringField(
@@ -90,17 +90,16 @@
         keytab: str | None = None,
         principal: str | None = None,
         master: str | None = None,
         name: str = "default-name",
         num_executors: int | None = None,
         verbose: bool = True,
         yarn_queue: str | None = None,
-        **kwargs,
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__()
         options: dict = {}
         conn: Connection | None = None
 
         try:
             conn = self.get_connection(conn_id)
         except AirflowNotFoundException:
             conn = None
```

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/hooks/spark_submit.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/hooks/spark_submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,38 +78,38 @@
         supports yarn and k8s mode too.
     :param verbose: Whether to pass the verbose flag to spark-submit process for debugging
     :param spark_binary: The command to use for spark submit.
                          Some distros may use spark2-submit or spark3-submit.
                          (will overwrite any spark_binary defined in the connection's extra JSON)
     :param properties_file: Path to a file from which to load extra properties. If not
                               specified, this will look for conf/spark-defaults.conf.
-    :param queue: The name of the YARN queue to which the application is submitted.
+    :param yarn_queue: The name of the YARN queue to which the application is submitted.
                         (will overwrite any yarn queue defined in the connection's extra JSON)
-    :param deploy_mode: Whether to deploy your driver on the worker nodes (cluster) or locally as an    client.
+    :param deploy_mode: Whether to deploy your driver on the worker nodes (cluster) or locally as an client.
                         (will overwrite any deployment mode defined in the connection's extra JSON)
     :param use_krb5ccache: if True, configure spark to use ticket cache instead of relying
         on keytab for Kerberos login
     """
 
     conn_name_attr = "conn_id"
     default_conn_name = "spark_default"
     conn_type = "spark"
     hook_name = "Spark"
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Return custom field behaviour."""
+        """Return custom UI field behaviour for Spark connection."""
         return {
             "hidden_fields": ["schema", "login", "password", "extra"],
             "relabeling": {},
         }
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Return connection widgets to add to Spark connection form."""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import StringField
         from wtforms.validators import Optional, any_of
 
         return {
             "queue": StringField(
@@ -161,15 +161,15 @@
         num_executors: int | None = None,
         status_poll_interval: int = 1,
         application_args: list[Any] | None = None,
         env_vars: dict[str, Any] | None = None,
         verbose: bool = False,
         spark_binary: str | None = None,
         properties_file: str | None = None,
-        queue: str | None = None,
+        yarn_queue: str | None = None,
         deploy_mode: str | None = None,
         *,
         use_krb5ccache: bool = False,
     ) -> None:
         super().__init__()
         self._conf = conf or {}
         self._conn_id = conn_id
@@ -197,15 +197,15 @@
         self._env_vars = env_vars
         self._verbose = verbose
         self._submit_sp: Any | None = None
         self._yarn_application_id: str | None = None
         self._kubernetes_driver_pod: str | None = None
         self.spark_binary = spark_binary
         self._properties_file = properties_file
-        self._queue = queue
+        self._yarn_queue = yarn_queue
         self._deploy_mode = deploy_mode
         self._connection = self._resolve_connection()
         self._is_yarn = "yarn" in self._connection["master"]
         self._is_kubernetes = "k8s" in self._connection["master"]
         if self._is_kubernetes and kube_client is None:
             raise RuntimeError(
                 f"{self._connection['master']} specified by kubernetes dependencies are not installed!"
@@ -227,15 +227,15 @@
         """
         return "spark://" in self._connection["master"] and self._connection["deploy_mode"] == "cluster"
 
     def _resolve_connection(self) -> dict[str, Any]:
         # Build from connection master or default to yarn if not available
         conn_data = {
             "master": "yarn",
-            "queue": None,
+            "queue": None,  # yarn queue
             "deploy_mode": None,
             "spark_binary": self.spark_binary or DEFAULT_SPARK_BINARY,
             "namespace": None,
         }
 
         try:
             # Master can be local, yarn, spark://HOST:PORT, mesos://HOST:PORT and
@@ -244,15 +244,15 @@
             if conn.port:
                 conn_data["master"] = f"{conn.host}:{conn.port}"
             else:
                 conn_data["master"] = conn.host
 
             # Determine optional yarn queue from the extra field
             extra = conn.extra_dejson
-            conn_data["queue"] = self._queue if self._queue else extra.get("queue")
+            conn_data["queue"] = self._yarn_queue if self._yarn_queue else extra.get("queue")
             conn_data["deploy_mode"] = self._deploy_mode if self._deploy_mode else extra.get("deploy-mode")
             if not self.spark_binary:
                 self.spark_binary = extra.get("spark-binary", DEFAULT_SPARK_BINARY)
                 if self.spark_binary is not None and self.spark_binary not in ALLOWED_SPARK_BINARIES:
                     raise RuntimeError(
                         f"The spark-binary extra can be on of {ALLOWED_SPARK_BINARIES} and it"
                         f" was `{self.spark_binary}`. Please make sure your spark binary is one of the"
```

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/__init__.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/spark_jdbc.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/operators/spark_jdbc.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,31 +40,23 @@
     :param spark_conn_id: The :ref:`spark connection id <howto/connection:spark-submit>`
         as configured in Airflow administration
     :param spark_conf: Any additional Spark configuration properties
     :param spark_py_files: Additional python files used (.zip, .egg, or .py)
     :param spark_files: Additional files to upload to the container running the job
     :param spark_jars: Additional jars to upload and add to the driver and
                        executor classpath
-    :param num_executors: number of executor to run. This should be set so as to manage
-                          the number of connections made with the JDBC database
-    :param executor_cores: Number of cores per executor
-    :param executor_memory: Memory per executor (e.g. 1000M, 2G)
-    :param driver_memory: Memory allocated to the driver (e.g. 1000M, 2G)
-    :param verbose: Whether to pass the verbose flag to spark-submit for debugging
-    :param keytab: Full path to the file that contains the keytab
-    :param principal: The name of the kerberos principal used for keytab
     :param cmd_type: Which way the data should flow. 2 possible values:
                      spark_to_jdbc: data written by spark from metastore to jdbc
                      jdbc_to_spark: data written by spark from jdbc to metastore
     :param jdbc_table: The name of the JDBC table
     :param jdbc_conn_id: Connection id used for connection to JDBC database
     :param jdbc_driver: Name of the JDBC driver to use for the JDBC connection. This
                         driver (usually a jar) should be passed in the 'jars' parameter
     :param metastore_table: The name of the metastore table,
-    :param jdbc_truncate: (spark_to_jdbc only) Whether or not Spark should truncate or
+    :param jdbc_truncate: (spark_to_jdbc only) Whether Spark should truncate or
                          drop and recreate the JDBC table. This only takes effect if
                          'save_mode' is set to Overwrite. Also, if the schema is
                          different, Spark cannot truncate, and will drop and recreate
     :param save_mode: The Spark save-mode to use (e.g. overwrite, append, etc.)
     :param save_format: (jdbc_to_spark-only) The Spark save-format to use (e.g. parquet)
     :param batch_size: (spark_to_jdbc only) The size of the batch to insert per round
                        trip to the JDBC database. Defaults to 1000
@@ -87,35 +79,26 @@
     :param create_table_column_types: (spark_to_jdbc-only) The database column data types
                                       to use instead of the defaults, when creating the
                                       table. Data type information should be specified in
                                       the same format as CREATE TABLE columns syntax
                                       (e.g: "name CHAR(64), comments VARCHAR(1024)").
                                       The specified types should be valid spark sql data
                                       types.
-    :param use_krb5ccache: if True, configure spark to use ticket cache instead of relying
-                           on keytab for Kerberos login
-
+    :param kwargs: kwargs passed to SparkSubmitOperator.
     """
 
     def __init__(
         self,
         *,
         spark_app_name: str = "airflow-spark-jdbc",
         spark_conn_id: str = "spark-default",
         spark_conf: dict[str, Any] | None = None,
         spark_py_files: str | None = None,
         spark_files: str | None = None,
         spark_jars: str | None = None,
-        num_executors: int | None = None,
-        executor_cores: int | None = None,
-        executor_memory: str | None = None,
-        driver_memory: str | None = None,
-        verbose: bool = False,
-        principal: str | None = None,
-        keytab: str | None = None,
         cmd_type: str = "spark_to_jdbc",
         jdbc_table: str | None = None,
         jdbc_conn_id: str = "jdbc-default",
         jdbc_driver: str | None = None,
         metastore_table: str | None = None,
         jdbc_truncate: bool = False,
         save_mode: str | None = None,
@@ -123,31 +106,23 @@
         batch_size: int | None = None,
         fetch_size: int | None = None,
         num_partitions: int | None = None,
         partition_column: str | None = None,
         lower_bound: str | None = None,
         upper_bound: str | None = None,
         create_table_column_types: str | None = None,
-        use_krb5ccache: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
         self._spark_app_name = spark_app_name
         self._spark_conn_id = spark_conn_id
         self._spark_conf = spark_conf
         self._spark_py_files = spark_py_files
         self._spark_files = spark_files
         self._spark_jars = spark_jars
-        self._num_executors = num_executors
-        self._executor_cores = executor_cores
-        self._executor_memory = executor_memory
-        self._driver_memory = driver_memory
-        self._verbose = verbose
-        self._keytab = keytab
-        self._principal = principal
         self._cmd_type = cmd_type
         self._jdbc_table = jdbc_table
         self._jdbc_conn_id = jdbc_conn_id
         self._jdbc_driver = jdbc_driver
         self._metastore_table = metastore_table
         self._jdbc_truncate = jdbc_truncate
         self._save_mode = save_mode
@@ -156,15 +131,14 @@
         self._fetch_size = fetch_size
         self._num_partitions = num_partitions
         self._partition_column = partition_column
         self._lower_bound = lower_bound
         self._upper_bound = upper_bound
         self._create_table_column_types = create_table_column_types
         self._hook: SparkJDBCHook | None = None
-        self._use_krb5ccache = use_krb5ccache
 
     def execute(self, context: Context) -> None:
         """Call the SparkSubmitHook to run the provided spark job."""
         if self._hook is None:
             self._hook = self._get_hook()
         self._hook.submit_jdbc_job()
 
@@ -182,16 +156,16 @@
             spark_files=self._spark_files,
             spark_jars=self._spark_jars,
             num_executors=self._num_executors,
             executor_cores=self._executor_cores,
             executor_memory=self._executor_memory,
             driver_memory=self._driver_memory,
             verbose=self._verbose,
-            keytab=self._keytab,
-            principal=self._principal,
+            keytab=self.keytab,
+            principal=self.principal,
             cmd_type=self._cmd_type,
             jdbc_table=self._jdbc_table,
             jdbc_conn_id=self._jdbc_conn_id,
             jdbc_driver=self._jdbc_driver,
             metastore_table=self._metastore_table,
             jdbc_truncate=self._jdbc_truncate,
             save_mode=self._save_mode,
```

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/spark_sql.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/operators/spark_sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Sequence
 
+from deprecated import deprecated
+
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.apache.spark.hooks.spark_sql import SparkSqlHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
@@ -48,17 +51,17 @@
     :param name: Name of the job
     :param num_executors: Number of executors to launch
     :param verbose: Whether to pass the verbose flag to spark-sql
     :param yarn_queue: The YARN queue to submit to
         (Default: The ``queue`` value set in the Connection, or ``"default"``)
     """
 
-    template_fields: Sequence[str] = ("_sql",)
+    template_fields: Sequence[str] = ("sql",)
     template_ext: Sequence[str] = (".sql", ".hql")
-    template_fields_renderers = {"_sql": "sql"}
+    template_fields_renderers = {"sql": "sql"}
 
     def __init__(
         self,
         *,
         sql: str,
         conf: str | None = None,
         conn_id: str = "spark_sql_default",
@@ -71,29 +74,38 @@
         name: str = "default-name",
         num_executors: int | None = None,
         verbose: bool = True,
         yarn_queue: str | None = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
-        self._sql = sql
+        self.sql = sql
         self._conf = conf
         self._conn_id = conn_id
         self._total_executor_cores = total_executor_cores
         self._executor_cores = executor_cores
         self._executor_memory = executor_memory
         self._keytab = keytab
         self._principal = principal
         self._master = master
         self._name = name
         self._num_executors = num_executors
         self._verbose = verbose
         self._yarn_queue = yarn_queue
         self._hook: SparkSqlHook | None = None
 
+    @property
+    @deprecated(
+        reason="`_sql` is deprecated and will be removed in the future. Please use `sql` instead.",
+        category=AirflowProviderDeprecationWarning,
+    )
+    def _sql(self):
+        """Alias for ``sql``, used for compatibility (deprecated)."""
+        return self.sql
+
     def execute(self, context: Context) -> None:
         """Call the SparkSqlHook to run the provided sql query."""
         if self._hook is None:
             self._hook = self._get_hook()
         self._hook.run_query()
 
     def on_kill(self) -> None:
```

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/airflow/providers/apache/spark/operators/spark_submit.py` & `apache_airflow_providers_apache_spark-4.8.0rc2/airflow/providers/apache/spark/operators/spark_submit.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,38 +68,38 @@
     :param env_vars: Environment variables for spark-submit. It supports yarn and k8s mode too. (templated)
     :param verbose: Whether to pass the verbose flag to spark-submit process for debugging
     :param spark_binary: The command to use for spark submit.
                          Some distros may use spark2-submit or spark3-submit.
                          (will overwrite any spark_binary defined in the connection's extra JSON)
     :param properties_file: Path to a file from which to load extra properties. If not
                               specified, this will look for conf/spark-defaults.conf.
-    :param queue: The name of the YARN queue to which the application is submitted.
+    :param yarn_queue: The name of the YARN queue to which the application is submitted.
                         (will overwrite any yarn queue defined in the connection's extra JSON)
     :param deploy_mode: Whether to deploy your driver on the worker nodes (cluster) or locally as a client.
                         (will overwrite any deployment mode defined in the connection's extra JSON)
     :param use_krb5ccache: if True, configure spark to use ticket cache instead of relying
                            on keytab for Kerberos login
     """
 
     template_fields: Sequence[str] = (
-        "_application",
-        "_conf",
-        "_files",
-        "_py_files",
-        "_jars",
-        "_driver_class_path",
-        "_packages",
-        "_exclude_packages",
-        "_keytab",
-        "_principal",
-        "_proxy_user",
-        "_name",
-        "_application_args",
-        "_env_vars",
-        "_properties_file",
+        "application",
+        "conf",
+        "files",
+        "py_files",
+        "jars",
+        "driver_class_path",
+        "packages",
+        "exclude_packages",
+        "keytab",
+        "principal",
+        "proxy_user",
+        "name",
+        "application_args",
+        "env_vars",
+        "properties_file",
     )
     ui_color = WEB_COLORS["LIGHTORANGE"]
 
     def __init__(
         self,
         *,
         application: str = "",
@@ -125,88 +125,88 @@
         num_executors: int | None = None,
         status_poll_interval: int = 1,
         application_args: list[Any] | None = None,
         env_vars: dict[str, Any] | None = None,
         verbose: bool = False,
         spark_binary: str | None = None,
         properties_file: str | None = None,
-        queue: str | None = None,
+        yarn_queue: str | None = None,
         deploy_mode: str | None = None,
         use_krb5ccache: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
-        self._application = application
-        self._conf = conf
-        self._files = files
-        self._py_files = py_files
+        self.application = application
+        self.conf = conf
+        self.files = files
+        self.py_files = py_files
         self._archives = archives
-        self._driver_class_path = driver_class_path
-        self._jars = jars
+        self.driver_class_path = driver_class_path
+        self.jars = jars
         self._java_class = java_class
-        self._packages = packages
-        self._exclude_packages = exclude_packages
+        self.packages = packages
+        self.exclude_packages = exclude_packages
         self._repositories = repositories
         self._total_executor_cores = total_executor_cores
         self._executor_cores = executor_cores
         self._executor_memory = executor_memory
         self._driver_memory = driver_memory
-        self._keytab = keytab
-        self._principal = principal
-        self._proxy_user = proxy_user
-        self._name = name
+        self.keytab = keytab
+        self.principal = principal
+        self.proxy_user = proxy_user
+        self.name = name
         self._num_executors = num_executors
         self._status_poll_interval = status_poll_interval
-        self._application_args = application_args
-        self._env_vars = env_vars
+        self.application_args = application_args
+        self.env_vars = env_vars
         self._verbose = verbose
         self._spark_binary = spark_binary
-        self._properties_file = properties_file
-        self._queue = queue
+        self.properties_file = properties_file
+        self._yarn_queue = yarn_queue
         self._deploy_mode = deploy_mode
         self._hook: SparkSubmitHook | None = None
         self._conn_id = conn_id
         self._use_krb5ccache = use_krb5ccache
 
     def execute(self, context: Context) -> None:
         """Call the SparkSubmitHook to run the provided spark job."""
         if self._hook is None:
             self._hook = self._get_hook()
-        self._hook.submit(self._application)
+        self._hook.submit(self.application)
 
     def on_kill(self) -> None:
         if self._hook is None:
             self._hook = self._get_hook()
         self._hook.on_kill()
 
     def _get_hook(self) -> SparkSubmitHook:
         return SparkSubmitHook(
-            conf=self._conf,
+            conf=self.conf,
             conn_id=self._conn_id,
-            files=self._files,
-            py_files=self._py_files,
+            files=self.files,
+            py_files=self.py_files,
             archives=self._archives,
-            driver_class_path=self._driver_class_path,
-            jars=self._jars,
+            driver_class_path=self.driver_class_path,
+            jars=self.jars,
             java_class=self._java_class,
-            packages=self._packages,
-            exclude_packages=self._exclude_packages,
+            packages=self.packages,
+            exclude_packages=self.exclude_packages,
             repositories=self._repositories,
             total_executor_cores=self._total_executor_cores,
             executor_cores=self._executor_cores,
             executor_memory=self._executor_memory,
             driver_memory=self._driver_memory,
-            keytab=self._keytab,
-            principal=self._principal,
-            proxy_user=self._proxy_user,
-            name=self._name,
+            keytab=self.keytab,
+            principal=self.principal,
+            proxy_user=self.proxy_user,
+            name=self.name,
             num_executors=self._num_executors,
             status_poll_interval=self._status_poll_interval,
-            application_args=self._application_args,
-            env_vars=self._env_vars,
+            application_args=self.application_args,
+            env_vars=self.env_vars,
             verbose=self._verbose,
             spark_binary=self._spark_binary,
-            properties_file=self._properties_file,
-            queue=self._queue,
+            properties_file=self.properties_file,
+            yarn_queue=self._yarn_queue,
             deploy_mode=self._deploy_mode,
             use_krb5ccache=self._use_krb5ccache,
         )
```

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/pyproject.toml` & `apache_airflow_providers_apache_spark-4.8.0rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-apache-spark"
-version = "4.8.0.rc1"
+version = "4.8.0.rc2"
 description = "Provider package apache-airflow-providers-apache-spark for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,19 +47,20 @@
     "Framework :: Apache Airflow",
     "Framework :: Apache Airflow :: Provider",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow>=2.7.0rc0",
     "grpcio-status>=1.59.0",
     "pyspark",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.8.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.8.0/changelog.html"
@@ -69,12 +70,12 @@
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
 provider_info = "airflow.providers.apache.spark.get_provider_info:get_provider_info"
 [project.optional-dependencies]
 "cncf.kubernetes" = [
-    "apache-airflow-providers-cncf-kubernetes>=7.4.0",
+    "apache-airflow-providers-cncf-kubernetes>=7.4.0rc0",
 ]
 
 [tool.flit.module]
 name = "airflow.providers.apache.spark"
```

### Comparing `apache_airflow_providers_apache_spark-4.8.0rc1/PKG-INFO` & `apache_airflow_providers_apache_spark-4.8.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-spark
-Version: 4.8.0rc1
+Version: 4.8.0rc2
 Summary: Provider package apache-airflow-providers-apache-spark for Apache Airflow
 Keywords: airflow-provider,apache.spark,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,19 +15,20 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: grpcio-status>=1.59.0
 Requires-Dist: pyspark
-Requires-Dist: apache-airflow-providers-cncf-kubernetes>=7.4.0 ; extra == "cncf.kubernetes"
+Requires-Dist: apache-airflow-providers-cncf-kubernetes>=7.4.0rc0 ; extra == "cncf.kubernetes"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.8.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.8.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
@@ -73,15 +74,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.8.0.rc1``
+Release: ``4.8.0.rc2``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -95,23 +96,23 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-spark``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``pyspark``
 ``grpcio-status``   ``>=1.59.0``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
```

