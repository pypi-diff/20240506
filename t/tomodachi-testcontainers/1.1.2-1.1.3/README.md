# Comparing `tmp/tomodachi_testcontainers-1.1.2.tar.gz` & `tmp/tomodachi_testcontainers-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomodachi_testcontainers-1.1.2.tar", max compression
+gzip compressed data, was "tomodachi_testcontainers-1.1.3.tar", max compression
```

## Comparing `tomodachi_testcontainers-1.1.2.tar` & `tomodachi_testcontainers-1.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-1.1.2/LICENSE
--rw-r--r--   0        0        0     5348 2024-03-09 08:39:31.463310 tomodachi_testcontainers-1.1.2/README.md
--rw-r--r--   0        0        0     5796 2024-03-09 10:16:57.550083 tomodachi_testcontainers-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1276 2024-01-20 12:02:32.093321 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/__init__.py
--rw-r--r--   0        0        0     1874 2024-01-20 12:02:32.093525 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/assertions.py
--rw-r--r--   0        0        0     2630 2024-02-10 12:31:41.559539 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/async_probes.py
--rw-r--r--   0        0        0      162 2024-02-10 12:31:41.538492 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/clients/__init__.py
--rw-r--r--   0        0        0    10112 2024-02-29 12:23:35.986712 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/clients/snssqs.py
--rw-r--r--   0        0        0     1069 2024-01-20 12:02:32.094393 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/__init__.py
--rw-r--r--   0        0        0      352 2024-01-20 12:02:32.094662 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/common/__init__.py
--rw-r--r--   0        0        0     5436 2024-01-20 12:02:32.094844 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/common/container.py
--rw-r--r--   0        0        0     2471 2024-03-07 14:43:49.403638 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/common/database.py
--rw-r--r--   0        0        0     2879 2024-01-08 19:54:00.254890 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/common/image.py
--rw-r--r--   0        0        0     2082 2024-03-07 14:43:49.404544 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/common/web.py
--rw-r--r--   0        0        0     1519 2024-01-20 12:02:32.095426 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/dynamodb_admin.py
--rw-r--r--   0        0        0     2290 2024-01-20 12:02:32.095615 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/localstack.py
--rw-r--r--   0        0        0     2597 2024-03-07 14:43:49.405277 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/minio.py
--rw-r--r--   0        0        0     2487 2024-01-20 12:02:32.095997 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/moto.py
--rw-r--r--   0        0        0     2144 2024-02-10 12:31:41.557850 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/mysql.py
--rw-r--r--   0        0        0     1837 2024-02-29 12:23:35.987113 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/postgres.py
--rw-r--r--   0        0        0     3511 2024-03-07 14:43:49.408064 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/sftp.py
--rw-r--r--   0        0        0     2561 2024-01-20 12:02:32.096696 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/tomodachi.py
--rw-r--r--   0        0        0     2820 2024-02-10 12:31:41.571774 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/wiremock.py
--rw-r--r--   0        0        0     1996 2024-02-10 12:31:41.560335 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/__init__.py
--rw-r--r--   0        0        0     2166 2024-01-20 12:02:32.097410 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/containers.py
--rw-r--r--   0        0        0     3252 2024-03-09 08:39:43.151081 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/localstack.py
--rw-r--r--   0        0        0      722 2024-03-09 08:38:21.893971 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/minio.py
--rw-r--r--   0        0        0     3011 2024-03-09 08:38:15.356645 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/moto.py
--rw-r--r--   0        0        0      336 2024-03-09 08:38:04.306148 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/mysql.py
--rw-r--r--   0        0        0      393 2024-03-09 08:35:49.808543 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/postgres.py
--rw-r--r--   0        0        0     1542 2024-03-09 08:35:23.475100 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/sftp.py
--rw-r--r--   0        0        0      915 2024-01-20 12:02:32.098577 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/wiremock.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/py.typed
--rw-r--r--   0        0        0     2788 2024-03-07 14:43:49.412303 tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/utils.py
--rw-r--r--   0        0        0     7180 1970-01-01 00:00:00.000000 tomodachi_testcontainers-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-1.1.3/LICENSE
+-rw-r--r--   0        0        0     5348 2024-03-09 08:39:31.463310 tomodachi_testcontainers-1.1.3/README.md
+-rw-r--r--   0        0        0     5797 2024-05-06 11:04:23.840534 tomodachi_testcontainers-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1276 2024-01-20 12:02:32.093321 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/__init__.py
+-rw-r--r--   0        0        0     1874 2024-01-20 12:02:32.093525 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/assertions.py
+-rw-r--r--   0        0        0     2630 2024-02-10 12:31:41.559539 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/async_probes.py
+-rw-r--r--   0        0        0      162 2024-02-10 12:31:41.538492 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/clients/__init__.py
+-rw-r--r--   0        0        0    10112 2024-02-29 12:23:35.986712 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/clients/snssqs.py
+-rw-r--r--   0        0        0     1069 2024-01-20 12:02:32.094393 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/__init__.py
+-rw-r--r--   0        0        0      352 2024-01-20 12:02:32.094662 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/__init__.py
+-rw-r--r--   0        0        0     5436 2024-05-06 11:02:27.200947 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/container.py
+-rw-r--r--   0        0        0     2471 2024-03-07 14:43:49.403638 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/database.py
+-rw-r--r--   0        0        0     2879 2024-01-08 19:54:00.254890 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/image.py
+-rw-r--r--   0        0        0     2082 2024-03-07 14:43:49.404544 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/web.py
+-rw-r--r--   0        0        0     1519 2024-01-20 12:02:32.095426 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/dynamodb_admin.py
+-rw-r--r--   0        0        0     2290 2024-01-20 12:02:32.095615 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/localstack.py
+-rw-r--r--   0        0        0     2597 2024-03-07 14:43:49.405277 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/minio.py
+-rw-r--r--   0        0        0     2487 2024-01-20 12:02:32.095997 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/moto.py
+-rw-r--r--   0        0        0     2144 2024-02-10 12:31:41.557850 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/mysql.py
+-rw-r--r--   0        0        0     1837 2024-02-29 12:23:35.987113 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/postgres.py
+-rw-r--r--   0        0        0     3511 2024-03-07 14:43:49.408064 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/sftp.py
+-rw-r--r--   0        0        0     2561 2024-01-20 12:02:32.096696 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/tomodachi.py
+-rw-r--r--   0        0        0     2820 2024-02-10 12:31:41.571774 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/wiremock.py
+-rw-r--r--   0        0        0     1996 2024-03-13 08:33:53.123090 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/__init__.py
+-rw-r--r--   0        0        0     2166 2024-01-20 12:02:32.097410 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/containers.py
+-rw-r--r--   0        0        0     3252 2024-03-13 08:36:44.293036 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/localstack.py
+-rw-r--r--   0        0        0      722 2024-03-09 08:38:21.893971 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/minio.py
+-rw-r--r--   0        0        0     3037 2024-03-13 08:36:04.781801 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/moto.py
+-rw-r--r--   0        0        0      336 2024-03-09 08:38:04.306148 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/mysql.py
+-rw-r--r--   0        0        0      393 2024-03-09 08:35:49.808543 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/postgres.py
+-rw-r--r--   0        0        0     1542 2024-03-09 08:35:23.475100 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/sftp.py
+-rw-r--r--   0        0        0      915 2024-03-13 08:36:50.873024 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/wiremock.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/py.typed
+-rw-r--r--   0        0        0     2788 2024-03-07 14:43:49.412303 tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/utils.py
+-rw-r--r--   0        0        0     7188 1970-01-01 00:00:00.000000 tomodachi_testcontainers-1.1.3/PKG-INFO
```

### Comparing `tomodachi_testcontainers-1.1.2/LICENSE` & `tomodachi_testcontainers-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/README.md` & `tomodachi_testcontainers-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/pyproject.toml` & `tomodachi_testcontainers-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomodachi-testcontainers"
-version = "1.1.2"
+version = "1.1.3"
 description = "Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing."
 authors = ["Filips Nastins <nastinsfilips@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/filipsnastins/tomodachi-testcontainers"
 repository = "https://github.com/filipsnastins/tomodachi-testcontainers"
@@ -21,15 +21,15 @@
 aiobotocore = "^2.4.2"
 asyncssh = { version = "^2.13.2", optional = true }
 cryptography = { version = ">=41,<43", optional = true }
 protobuf = "^4.0"
 psycopg = { version = "^3.1.18", optional = true }
 pymysql = { version = "^1.1.0", optional = true }
 pytest = ">=7.1.2,<9.0.0"
-pytest-asyncio = "0.21.1" # https://github.com/pytest-dev/pytest-asyncio/issues/706
+pytest-asyncio = "~0.21.1" # https://github.com/pytest-dev/pytest-asyncio/issues/706
 requests = "^2.31.0"
 shortuuid = "^1.0.11"
 sqlalchemy = { version = ">=1.3,<3", optional = true }
 tenacity = "^8.2.2"
 testcontainers = ">=3.7.1,<5.0.0"
 types-aiobotocore = { extras = [
     "dynamodb",
```

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/__init__.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/assertions.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/assertions.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/async_probes.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/async_probes.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/clients/snssqs.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/clients/snssqs.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/__init__.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/common/container.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/container.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/common/database.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/database.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/common/image.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/image.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/common/web.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/common/web.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/dynamodb_admin.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/dynamodb_admin.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/localstack.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/localstack.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/minio.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/minio.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/moto.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/moto.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/mysql.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/mysql.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/postgres.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/postgres.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/sftp.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/sftp.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/tomodachi.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/tomodachi.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/containers/wiremock.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/containers/wiremock.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/__init__.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/containers.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/containers.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/localstack.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/localstack.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/minio.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/minio.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/moto.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/moto.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,16 @@
 def moto_container() -> Generator[DockerContainer, None, None]:
     image = os.getenv("MOTO_TESTCONTAINER_IMAGE_ID", "motoserver/moto:latest")
     with MotoContainer(image) as container:
         yield container
 
 
 @pytest.fixture()
-def reset_moto_container_on_teardown(  # noqa: PT004
-    moto_container: MotoContainer,
-) -> Generator[None, None, None]:
-    """Removes all mocked resources from Moto after each test."""
+def reset_moto_container_on_teardown(moto_container: MotoContainer) -> Generator[None, None, None]:  # noqa: PT004
+    """Removes all mocked resources from Moto after each test without restarting the container."""
     yield
     moto_container.reset_moto()
 
 
 @pytest_asyncio.fixture(scope="session")
 async def moto_dynamodb_client(moto_container: MotoContainer) -> AsyncGenerator[DynamoDBClient, None]:
     async with get_session().create_client("dynamodb", **moto_container.get_aws_client_config()) as c:
```

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/sftp.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/sftp.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/fixtures/wiremock.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/fixtures/wiremock.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/src/tomodachi_testcontainers/utils.py` & `tomodachi_testcontainers-1.1.3/src/tomodachi_testcontainers/utils.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-1.1.2/PKG-INFO` & `tomodachi_testcontainers-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomodachi-testcontainers
-Version: 1.1.2
+Version: 1.1.3
 Summary: Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing.
 Home-page: https://github.com/filipsnastins/tomodachi-testcontainers
 License: MIT
 Author: Filips Nastins
 Author-email: nastinsfilips@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 Requires-Dist: aiobotocore (>=2.4.2,<3.0.0)
 Requires-Dist: asyncssh (>=2.13.2,<3.0.0) ; extra == "sftp"
 Requires-Dist: cryptography (>=41,<43) ; extra == "mysql"
 Requires-Dist: protobuf (>=4.0,<5.0)
 Requires-Dist: psycopg (>=3.1.18,<4.0.0) ; extra == "postgres"
 Requires-Dist: pymysql (>=1.1.0,<2.0.0) ; extra == "mysql"
 Requires-Dist: pytest (>=7.1.2,<9.0.0)
-Requires-Dist: pytest-asyncio (==0.21.1)
+Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: shortuuid (>=1.0.11,<2.0.0)
 Requires-Dist: sqlalchemy (>=1.3,<3) ; extra == "db" or extra == "mysql" or extra == "postgres"
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: testcontainers (>=3.7.1,<5.0.0)
 Requires-Dist: types-aiobotocore[dynamodb,iam,lambda,s3,sns,sqs,ssm] (>=2.4.2,<3.0.0)
 Requires-Dist: wiremock (>=2.6.1,<3.0.0) ; extra == "wiremock"
```

