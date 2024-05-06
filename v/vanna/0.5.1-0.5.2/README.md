# Comparing `tmp/vanna-0.5.1.tar.gz` & `tmp/vanna-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vanna-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vanna-0.5.1.tar` & `vanna-0.5.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     8010 2024-05-02 13:17:19.261679 vanna-0.5.1/README.md
--rw-r--r--   0        0        0     1627 2024-05-02 13:17:19.277679 vanna-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     8725 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/ZhipuAI/ZhipuAI_Chat.py
--rw-r--r--   0        0        0     2849 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
--rw-r--r--   0        0        0      116 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/ZhipuAI/__init__.py
--rw-r--r--   0        0        0     9248 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/__init__.py
--rw-r--r--   0        0        0       43 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/anthropic/__init__.py
--rw-r--r--   0        0        0     2615 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/anthropic/anthropic_chat.py
--rw-r--r--   0        0        0       28 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/base/__init__.py
--rw-r--r--   0        0        0    62126 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/base/base.py
--rw-r--r--   0        0        0       50 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/chromadb/__init__.py
--rw-r--r--   0        0        0     8792 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/chromadb/chromadb_vector.py
--rw-r--r--   0        0        0      685 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/exceptions/__init__.py
--rw-r--r--   0        0        0    25192 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/flask/__init__.py
--rw-r--r--   0        0        0   187711 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/flask/assets.py
--rw-r--r--   0        0        0     1246 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/flask/auth.py
--rw-r--r--   0        0        0       41 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/google/__init__.py
--rw-r--r--   0        0        0     1584 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/google/gemini_chat.py
--rw-r--r--   0        0        0       19 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/hf/__init__.py
--rw-r--r--   0        0        0     2703 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/hf/hf.py
--rw-r--r--   0        0        0      313 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/local.py
--rw-r--r--   0        0        0       37 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/marqo/__init__.py
--rw-r--r--   0        0        0     5242 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/marqo/marqo.py
--rw-r--r--   0        0        0       29 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/mistral/__init__.py
--rw-r--r--   0        0        0     1508 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/mistral/mistral.py
--rw-r--r--   0        0        0       27 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/ollama/__init__.py
--rw-r--r--   0        0        0     3790 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/ollama/ollama.py
--rw-r--r--   0        0        0       86 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/openai/__init__.py
--rw-r--r--   0        0        0     4764 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/openai/openai_chat.py
--rw-r--r--   0        0        0     1260 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/openai/openai_embeddings.py
--rw-r--r--   0        0        0       54 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/opensearch/__init__.py
--rw-r--r--   0        0        0     9129 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/opensearch/opensearch_vector.py
--rw-r--r--   0        0        0       73 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/qdrant/__init__.py
--rw-r--r--   0        0        0    11883 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/qdrant/qdrant.py
--rw-r--r--   0        0        0     1856 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/remote.py
--rw-r--r--   0        0        0     4957 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/types/__init__.py
--rw-r--r--   0        0        0     2247 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/utils.py
--rw-r--r--   0        0        0       48 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/vannadb/__init__.py
--rw-r--r--   0        0        0     6168 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/vannadb/vannadb_vector.py
--rw-r--r--   0        0        0       23 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/vllm/__init__.py
--rw-r--r--   0        0        0     2427 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/vllm/vllm.py
--rw-r--r--   0        0        0    11248 1970-01-01 00:00:00.000000 vanna-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     8010 2024-05-06 13:24:20.218984 vanna-0.5.2/README.md
+-rw-r--r--   0        0        0     1627 2024-05-06 13:24:20.234984 vanna-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     8725 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/ZhipuAI/ZhipuAI_Chat.py
+-rw-r--r--   0        0        0     2849 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
+-rw-r--r--   0        0        0      116 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/ZhipuAI/__init__.py
+-rw-r--r--   0        0        0     9248 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/anthropic/__init__.py
+-rw-r--r--   0        0        0     2615 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/anthropic/anthropic_chat.py
+-rw-r--r--   0        0        0       28 2024-05-06 13:24:20.234984 vanna-0.5.2/src/vanna/base/__init__.py
+-rw-r--r--   0        0        0    65593 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/base/base.py
+-rw-r--r--   0        0        0       50 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/chromadb/__init__.py
+-rw-r--r--   0        0        0     8792 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/chromadb/chromadb_vector.py
+-rw-r--r--   0        0        0      685 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/exceptions/__init__.py
+-rw-r--r--   0        0        0    25192 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/flask/__init__.py
+-rw-r--r--   0        0        0   187711 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/flask/assets.py
+-rw-r--r--   0        0        0     1246 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/flask/auth.py
+-rw-r--r--   0        0        0       41 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/google/__init__.py
+-rw-r--r--   0        0        0     1584 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/google/gemini_chat.py
+-rw-r--r--   0        0        0       19 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/hf/__init__.py
+-rw-r--r--   0        0        0     2703 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/hf/hf.py
+-rw-r--r--   0        0        0      313 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/local.py
+-rw-r--r--   0        0        0       37 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/marqo/__init__.py
+-rw-r--r--   0        0        0     5242 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/marqo/marqo.py
+-rw-r--r--   0        0        0       29 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/mistral/__init__.py
+-rw-r--r--   0        0        0     1508 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/mistral/mistral.py
+-rw-r--r--   0        0        0       27 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/ollama/__init__.py
+-rw-r--r--   0        0        0     3790 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/ollama/ollama.py
+-rw-r--r--   0        0        0       86 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/openai/__init__.py
+-rw-r--r--   0        0        0     4764 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/openai/openai_chat.py
+-rw-r--r--   0        0        0     1260 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/openai/openai_embeddings.py
+-rw-r--r--   0        0        0       54 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/opensearch/__init__.py
+-rw-r--r--   0        0        0    11980 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/opensearch/opensearch_vector.py
+-rw-r--r--   0        0        0       73 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/qdrant/__init__.py
+-rw-r--r--   0        0        0    12613 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/qdrant/qdrant.py
+-rw-r--r--   0        0        0     1856 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/remote.py
+-rw-r--r--   0        0        0     4957 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/types/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/utils.py
+-rw-r--r--   0        0        0       48 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/vannadb/__init__.py
+-rw-r--r--   0        0        0     6168 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/vannadb/vannadb_vector.py
+-rw-r--r--   0        0        0       23 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/vllm/__init__.py
+-rw-r--r--   0        0        0     2427 2024-05-06 13:24:20.238984 vanna-0.5.2/src/vanna/vllm/vllm.py
+-rw-r--r--   0        0        0    11248 1970-01-01 00:00:00.000000 vanna-0.5.2/PKG-INFO
```

### Comparing `vanna-0.5.1/README.md` & `vanna-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/pyproject.toml` & `vanna-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "vanna"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `vanna-0.5.1/src/vanna/ZhipuAI/ZhipuAI_Chat.py` & `vanna-0.5.2/src/vanna/ZhipuAI/ZhipuAI_Chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/ZhipuAI/ZhipuAI_embeddings.py` & `vanna-0.5.2/src/vanna/ZhipuAI/ZhipuAI_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/__init__.py` & `vanna-0.5.2/src/vanna/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/anthropic/anthropic_chat.py` & `vanna-0.5.2/src/vanna/anthropic/anthropic_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/base/base.py` & `vanna-0.5.2/src/vanna/base/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1142,27 +1142,22 @@
             except Exception as e:
                 raise ImproperlyConfigured(e)
         else:
             print("Not using Google Colab.")
 
         conn = None
 
-        try:
-            conn = bigquery.Client(project=project_id)
-        except:
-            print("Could not found any google cloud implicit credentials")
-
-        if cred_file_path:
+        if not cred_file_path:
+            try:
+                conn = bigquery.Client(project=project_id)
+            except:
+                print("Could not found any google cloud implicit credentials")
+        else:
             # Validate file path and pemissions
             validate_config_path(cred_file_path)
-        else:
-            if not conn:
-                raise ValidationError(
-                    "Pleae provide a service account credentials json file"
-                )
 
         if not conn:
             with open(cred_file_path, "r") as f:
                 credentials = service_account.Credentials.from_service_account_info(
                     json.loads(f.read()),
                     scopes=["https://www.googleapis.com/auth/cloud-platform"],
                 )
@@ -1275,21 +1270,132 @@
 
         engine = create_engine(connection_url)
 
         def run_sql_mssql(sql: str):
             # Execute the SQL statement and return the result as a pandas DataFrame
             with engine.begin() as conn:
                 df = pd.read_sql_query(sa.text(sql), conn)
+                conn.close()
                 return df
 
             raise Exception("Couldn't run sql")
 
         self.dialect = "T-SQL / Microsoft SQL Server"
         self.run_sql = run_sql_mssql
         self.run_sql_is_set = True
+    def connect_to_presto(
+      self,
+      host: str,
+      catalog: str = 'hive',
+      schema: str = 'default',
+      user: str = None,
+      password: str = None,
+      port: int = None,
+      combined_pem_path: str = None,
+      protocol: str = 'https',
+      requests_kwargs: dict = None
+    ):
+      """
+        Connect to a Presto database using the specified parameters.
+
+        Args:
+            host (str): The host address of the Presto database.
+            catalog (str): The catalog to use in the Presto environment.
+            schema (str): The schema to use in the Presto environment.
+            user (str): The username for authentication.
+            password (str): The password for authentication.
+            port (int): The port number for the Presto connection.
+            combined_pem_path (str): The path to the combined pem file for SSL connection.
+            protocol (str): The protocol to use for the connection (default is 'https').
+            requests_kwargs (dict): Additional keyword arguments for requests.
+
+        Raises:
+            DependencyError: If required dependencies are not installed.
+            ImproperlyConfigured: If essential configuration settings are missing.
+
+        Returns:
+            None
+      """
+      try:
+        from pyhive import presto
+      except ImportError:
+        raise DependencyError(
+          "You need to install required dependencies to execute this method,"
+          " run command: \npip install pyhive"
+        )
+
+      if not host:
+        host = os.getenv("PRESTO_HOST")
+
+      if not host:
+        raise ImproperlyConfigured("Please set your presto host")
+
+      if not catalog:
+        catalog = os.getenv("PRESTO_CATALOG")
+
+      if not catalog:
+        raise ImproperlyConfigured("Please set your presto catalog")
+
+      if not user:
+        user = os.getenv("PRESTO_USER")
+
+      if not user:
+        raise ImproperlyConfigured("Please set your presto user")
+
+      if not password:
+        password = os.getenv("PRESTO_PASSWORD")
+
+      if not port:
+        port = os.getenv("PRESTO_PORT")
+
+      if not port:
+        raise ImproperlyConfigured("Please set your presto port")
+
+      conn = None
+
+      try:
+        if requests_kwargs is None and combined_pem_path is not None:
+          # use the combined pem file to verify the SSL connection
+          requests_kwargs = {
+            'verify': combined_pem_path,  # 使用转换后得到的 PEM 文件进行 SSL 验证
+          }
+        conn = presto.Connection(host=host,
+                                 username=user,
+                                 password=password,
+                                 catalog=catalog,
+                                 schema=schema,
+                                 port=port,
+                                 protocol=protocol,
+                                 requests_kwargs=requests_kwargs)
+      except presto.Error as e:
+        raise ValidationError(e)
+
+      def run_sql_presto(sql: str) -> Union[pd.DataFrame, None]:
+        if conn:
+          try:
+            cs = conn.cursor()
+            cs.execute(sql)
+            results = cs.fetchall()
+
+            # Create a pandas dataframe from the results
+            df = pd.DataFrame(
+              results, columns=[desc[0] for desc in cs.description]
+            )
+            return df
+
+          except presto.Error as e:
+            print(e)
+            raise ValidationError(e)
+
+          except Exception as e:
+            print(e)
+            raise e
+
+      self.run_sql_is_set = True
+      self.run_sql = run_sql_presto
 
     def run_sql(self, sql: str, **kwargs) -> pd.DataFrame:
         """
         Example:
         ```python
         vn.run_sql("SELECT * FROM my_table")
         ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vanna-0.5.1/src/vanna/chromadb/chromadb_vector.py` & `vanna-0.5.2/src/vanna/chromadb/chromadb_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/exceptions/__init__.py` & `vanna-0.5.2/src/vanna/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/flask/__init__.py` & `vanna-0.5.2/src/vanna/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/flask/assets.py` & `vanna-0.5.2/src/vanna/flask/assets.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/flask/auth.py` & `vanna-0.5.2/src/vanna/flask/auth.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/google/gemini_chat.py` & `vanna-0.5.2/src/vanna/google/gemini_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/hf/hf.py` & `vanna-0.5.2/src/vanna/hf/hf.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/marqo/marqo.py` & `vanna-0.5.2/src/vanna/marqo/marqo.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/mistral/mistral.py` & `vanna-0.5.2/src/vanna/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/ollama/ollama.py` & `vanna-0.5.2/src/vanna/ollama/ollama.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/openai/openai_chat.py` & `vanna-0.5.2/src/vanna/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/openai/openai_embeddings.py` & `vanna-0.5.2/src/vanna/openai/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/opensearch/opensearch_vector.py` & `vanna-0.5.2/src/vanna/opensearch/opensearch_vector.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,15 +20,85 @@
       ddl_index = config["es_ddl_index"]
     if config is not None and "es_question_sql_index" in config:
       question_sql_index = config["es_question_sql_index"]
 
     self.document_index = document_index
     self.ddl_index = ddl_index
     self.question_sql_index = question_sql_index
-    print("OpenSearch_VectorStore initialized with document_index: ", document_index, " ddl_index: ", ddl_index, " question_sql_index: ", question_sql_index)
+    print("OpenSearch_VectorStore initialized with document_index: ",
+          document_index, " ddl_index: ", ddl_index, " question_sql_index: ",
+          question_sql_index)
+
+    document_index_settings = {
+      "settings": {
+        "index": {
+          "number_of_shards": 6,
+          "number_of_replicas": 2
+        }
+      },
+      "mappings": {
+        "properties": {
+          "question": {
+            "type": "text",
+          },
+          "doc": {
+            "type": "text",
+          }
+        }
+      }
+    }
+
+    ddl_index_settings = {
+      "settings": {
+        "index": {
+          "number_of_shards": 6,
+          "number_of_replicas": 2
+        }
+      },
+      "mappings": {
+        "properties": {
+          "ddl": {
+            "type": "text",
+          },
+          "doc": {
+            "type": "text",
+          }
+        }
+      }
+    }
+
+    question_sql_index_settings = {
+      "settings": {
+        "index": {
+          "number_of_shards": 6,
+          "number_of_replicas": 2
+        }
+      },
+      "mappings": {
+        "properties": {
+          "question": {
+            "type": "text",
+          },
+          "sql": {
+            "type": "text",
+          }
+        }
+      }
+    }
+
+    if config is not None and "es_document_index_settings" in config:
+      document_index_settings = config["es_document_index_settings"]
+    if config is not None and "es_ddl_index_settings" in config:
+      ddl_index_settings = config["es_ddl_index_settings"]
+    if config is not None and "es_question_sql_index_settings" in config:
+      question_sql_index_settings = config["es_question_sql_index_settings"]
+
+    self.document_index_settings = document_index_settings
+    self.ddl_index_settings = ddl_index_settings
+    self.question_sql_index_settings = question_sql_index_settings
 
     es_urls = None
     if config is not None and "es_urls" in config:
       es_urls = config["es_urls"]
 
     # Host and port
     if config is not None and "es_host" in config:
@@ -81,14 +151,17 @@
       timeout = 60
 
     if config is not None and "es_max_retries" in config:
       max_retries = config["es_max_retries"]
     else:
       max_retries = 10
 
+    print("OpenSearch_VectorStore initialized with es_urls: ", es_urls,
+          " host: ", host, " port: ", port, " ssl: ", ssl, " verify_certs: ",
+          verify_certs, " timeout: ", timeout, " max_retries: ", max_retries)
     if es_urls is not None:
       # Initialize the OpenSearch client by passing a list of URLs
       self.client = OpenSearch(
         hosts=[es_urls],
         http_compress=True,
         use_ssl=ssl,
         verify_certs=verify_certs,
@@ -108,33 +181,55 @@
         timeout=timeout,
         max_retries=max_retries,
         retry_on_timeout=True,
         http_auth=auth,
         headers=headers
       )
 
+      print("OpenSearch_VectorStore initialized with client over ")
+
     # 执行一个简单的查询来检查连接
     try:
+      print('Connected to OpenSearch cluster:')
       info = self.client.info()
       print('OpenSearch cluster info:', info)
     except Exception as e:
       print('Error connecting to OpenSearch cluster:', e)
 
     # Create the indices if they don't exist
-    # self.create_index()
+    self.create_index_if_not_exists(self.document_index,
+                                    self.document_index_settings)
+    self.create_index_if_not_exists(self.ddl_index, self.ddl_index_settings)
+    self.create_index_if_not_exists(self.question_sql_index,
+                                    self.question_sql_index_settings)
 
   def create_index(self):
-    for index in [self.document_index, self.ddl_index, self.question_sql_index]:
+    for index in [self.document_index, self.ddl_index,
+                  self.question_sql_index]:
       try:
         self.client.indices.create(index)
       except Exception as e:
         print("Error creating index: ", e)
         print(f"opensearch index {index} already exists")
         pass
 
+  def create_index_if_not_exists(self, index_name: str,
+                                 index_settings: dict) -> bool:
+    try:
+      if not self.client.indices.exists(index_name):
+        print(f"Index {index_name} does not exist. Creating...")
+        self.client.indices.create(index=index_name, body=index_settings)
+        return True
+      else:
+        print(f"Index {index_name} already exists.")
+        return False
+    except Exception as e:
+      print(f"Error creating index: {index_name} ", e)
+      return False
+
   def add_ddl(self, ddl: str, **kwargs) -> str:
     # Assuming that you have a DDL index in your OpenSearch
     id = str(uuid.uuid4()) + "-ddl"
     ddl_dict = {
       "ddl": ddl
     }
     response = self.client.index(index=self.ddl_index, body=ddl_dict, id=id,
@@ -274,15 +369,14 @@
       print("Error deleting training dataError deleting training data: ", e)
       return False
 
   def generate_embedding(self, data: str, **kwargs) -> list[float]:
     # opensearch doesn't need to generate embeddings
     pass
 
-
 # OpenSearch_VectorStore.__init__(self, config={'es_urls':
 # "https://opensearch-node.test.com:9200", 'es_encoded_base64': True, 'es_user':
 # "admin", 'es_password': "admin", 'es_verify_certs': True})
 
 
 # OpenSearch_VectorStore.__init__(self, config={'es_host':
 # "https://opensearch-node.test.com", 'es_port': 9200, 'es_user': "admin",
```

### Comparing `vanna-0.5.1/src/vanna/qdrant/qdrant.py` & `vanna-0.5.2/src/vanna/qdrant/qdrant.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,56 +3,59 @@
 
 import pandas as pd
 from qdrant_client import QdrantClient, grpc, models
 
 from ..base import VannaBase
 from ..utils import deterministic_uuid
 
-DOCUMENTATION_COLLECTION_NAME = "documentation"
-DDL_COLLECTION_NAME = "ddl"
-SQL_COLLECTION_NAME = "sql"
 SCROLL_SIZE = 1000
 
-ID_SUFFIXES = {
-    DDL_COLLECTION_NAME: "ddl",
-    DOCUMENTATION_COLLECTION_NAME: "doc",
-    SQL_COLLECTION_NAME: "sql",
-}
-
 
 class Qdrant_VectorStore(VannaBase):
-    """Vectorstore implementation using Qdrant - https://qdrant.tech/"""
+    """
+    Vectorstore implementation using Qdrant - https://qdrant.tech/
+
+    Args:
+        - config (dict, optional): Dictionary of `Qdrant_VectorStore config` options. Defaults to `{}`.
+            - client: A `qdrant_client.QdrantClient` instance. Overrides other config options.
+            - location: If `":memory:"` - use in-memory Qdrant instance. If `str` - use it as a `url` parameter.
+            - url: Either host or str of "Optional[scheme], host, Optional[port], Optional[prefix]". Eg. `"http://localhost:6333"`.
+            - prefer_grpc: If `true` - use gPRC interface whenever possible in custom methods.
+            - https: If `true` - use HTTPS(SSL) protocol. Default: `None`
+            - api_key: API key for authentication in Qdrant Cloud. Default: `None`
+            - timeout: Timeout for REST and gRPC API requests. Defaults to 5 seconds for REST and unlimited for gRPC.
+            - path: Persistence path for QdrantLocal. Default: `None`.
+            - prefix: Prefix to the REST URL paths. Example: `service/v1` will result in `http://localhost:6333/service/v1/{qdrant-endpoint}`.
+            - n_results: Number of results to return from similarity search. Defaults to 10.
+            - fastembed_model: [Model](https://qdrant.github.io/fastembed/examples/Supported_Models/#supported-text-embedding-models) to use for `fastembed.TextEmbedding`.
+              Defaults to `"BAAI/bge-small-en-v1.5"`.
+            - collection_params: Additional parameters to pass to `qdrant_client.QdrantClient#create_collection()` method.
+            - distance_metric: Distance metric to use when creating collections. Defaults to `qdrant_client.models.Distance.COSINE`.
+            - documentation_collection_name: Name of the collection to store documentation. Defaults to `"documentation"`.
+            - ddl_collection_name: Name of the collection to store DDL. Defaults to `"ddl"`.
+            - sql_collection_name: Name of the collection to store SQL. Defaults to `"sql"`.
+
+    Raises:
+        TypeError: If config["client"] is not a `qdrant_client.QdrantClient` instance
+    """
+
+    documentation_collection_name = "documentation"
+    ddl_collection_name = "ddl"
+    sql_collection_name = "sql"
+
+    id_suffixes = {
+        ddl_collection_name: "ddl",
+        documentation_collection_name: "doc",
+        sql_collection_name: "sql",
+    }
 
     def __init__(
         self,
         config={},
     ):
-        """
-        Vectorstore implementation using Qdrant - https://qdrant.tech/
-
-        Args:
-            - config (dict, optional): Dictionary of `Qdrant_VectorStore config` options. Defaults to `{}`.
-                - client: A `qdrant_client.QdrantClient` instance. Overrides other config options.
-                - location: If `":memory:"` - use in-memory Qdrant instance. If `str` - use it as a `url` parameter.
-                - url: Either host or str of "Optional[scheme], host, Optional[port], Optional[prefix]". Eg. `"http://localhost:6333"`.
-                - prefer_grpc: If `true` - use gPRC interface whenever possible in custom methods.
-                - https: If `true` - use HTTPS(SSL) protocol. Default: `None`
-                - api_key: API key for authentication in Qdrant Cloud. Default: `None`
-                - timeout: Timeout for REST and gRPC API requests. Defaults to 5 seconds for REST and unlimited for gRPC.
-                - path: Persistence path for QdrantLocal. Default: `None`.
-                - prefix: Prefix to the REST URL paths. Example: `service/v1` will result in `http://localhost:6333/service/v1/{qdrant-endpoint}`.
-                - n_results: Number of results to return from similarity search. Defaults to 10.
-                - fastembed_model: [Model](https://qdrant.github.io/fastembed/examples/Supported_Models/#supported-text-embedding-models) to use for `fastembed.TextEmbedding`.
-                  Defaults to `"BAAI/bge-small-en-v1.5"`.
-                - collection_params: Additional parameters to pass to `qdrant_client.QdrantClient#create_collection()` method.
-                - distance_metric: Distance metric to use when creating collections. Defaults to `qdrant_client.models.Distance.COSINE`.
-
-        Raises:
-            TypeError: If config["client"] is not a `qdrant_client.QdrantClient` instance
-        """
         VannaBase.__init__(self, config=config)
         client = config.get("client")
 
         if client is None:
             self._client = QdrantClient(
                 location=config.get("location", None),
                 url=config.get("url", None),
@@ -71,115 +74,126 @@
         else:
             self._client = client
 
         self.n_results = config.get("n_results", 10)
         self.fastembed_model = config.get("fastembed_model", "BAAI/bge-small-en-v1.5")
         self.collection_params = config.get("collection_params", {})
         self.distance_metric = config.get("distance_metric", models.Distance.COSINE)
+        self.documentation_collection_name = config.get(
+            "documentation_collection_name", self.documentation_collection_name
+        )
+        self.ddl_collection_name = config.get(
+            "ddl_collection_name", self.ddl_collection_name
+        )
+        self.sql_collection_name = config.get(
+            "sql_collection_name", self.sql_collection_name
+        )
 
         self._setup_collections()
 
     def add_question_sql(self, question: str, sql: str, **kwargs) -> str:
         question_answer = "Question: {0}\n\nSQL: {1}".format(question, sql)
         id = deterministic_uuid(question_answer)
 
         self._client.upsert(
-            SQL_COLLECTION_NAME,
+            self.sql_collection_name,
             points=[
                 models.PointStruct(
                     id=id,
                     vector=self.generate_embedding(question_answer),
                     payload={
                         "question": question,
                         "sql": sql,
                     },
                 )
             ],
         )
 
-        return self._format_point_id(id, SQL_COLLECTION_NAME)
+        return self._format_point_id(id, self.sql_collection_name)
 
     def add_ddl(self, ddl: str, **kwargs) -> str:
         id = deterministic_uuid(ddl)
         self._client.upsert(
-            DDL_COLLECTION_NAME,
+            self.ddl_collection_name,
             points=[
                 models.PointStruct(
                     id=id,
                     vector=self.generate_embedding(ddl),
                     payload={
                         "ddl": ddl,
                     },
                 )
             ],
         )
-        return self._format_point_id(id, DDL_COLLECTION_NAME)
+        return self._format_point_id(id, self.ddl_collection_name)
 
     def add_documentation(self, documentation: str, **kwargs) -> str:
         id = deterministic_uuid(documentation)
 
         self._client.upsert(
-            DOCUMENTATION_COLLECTION_NAME,
+            self.documentation_collection_name,
             points=[
                 models.PointStruct(
                     id=id,
                     vector=self.generate_embedding(documentation),
                     payload={
                         "documentation": documentation,
                     },
                 )
             ],
         )
 
-        return self._format_point_id(id, DOCUMENTATION_COLLECTION_NAME)
+        return self._format_point_id(id, self.documentation_collection_name)
 
     def get_training_data(self, **kwargs) -> pd.DataFrame:
         df = pd.DataFrame()
 
-        if sql_data := self._get_all_points(SQL_COLLECTION_NAME):
+        if sql_data := self._get_all_points(self.sql_collection_name):
             question_list = [data.payload["question"] for data in sql_data]
             sql_list = [data.payload["sql"] for data in sql_data]
             id_list = [
-                self._format_point_id(data.id, SQL_COLLECTION_NAME) for data in sql_data
+                self._format_point_id(data.id, self.sql_collection_name)
+                for data in sql_data
             ]
 
             df_sql = pd.DataFrame(
                 {
                     "id": id_list,
                     "question": question_list,
                     "content": sql_list,
                 }
             )
 
             df_sql["training_data_type"] = "sql"
 
             df = pd.concat([df, df_sql])
 
-        if ddl_data := self._get_all_points(DDL_COLLECTION_NAME):
+        if ddl_data := self._get_all_points(self.ddl_collection_name):
             ddl_list = [data.payload["ddl"] for data in ddl_data]
             id_list = [
-                self._format_point_id(data.id, DDL_COLLECTION_NAME) for data in ddl_data
+                self._format_point_id(data.id, self.ddl_collection_name)
+                for data in ddl_data
             ]
 
             df_ddl = pd.DataFrame(
                 {
                     "id": id_list,
                     "question": [None for _ in ddl_list],
                     "content": ddl_list,
                 }
             )
 
             df_ddl["training_data_type"] = "ddl"
 
             df = pd.concat([df, df_ddl])
 
-        if doc_data := self._get_all_points(DOCUMENTATION_COLLECTION_NAME):
+        if doc_data := self._get_all_points(self.documentation_collection_name):
             document_list = [data.payload["documentation"] for data in doc_data]
             id_list = [
-                self._format_point_id(data.id, DOCUMENTATION_COLLECTION_NAME)
+                self._format_point_id(data.id, self.documentation_collection_name)
                 for data in doc_data
             ]
 
             df_doc = pd.DataFrame(
                 {
                     "id": id_list,
                     "question": [None for _ in document_list],
@@ -206,48 +220,48 @@
 
         Args:
             collection_name (str): sql or ddl or documentation
 
         Returns:
             bool: True if collection is deleted, False otherwise
         """
-        if collection_name in ID_SUFFIXES.keys():
+        if collection_name in self.id_suffixes.keys():
             self._client.delete_collection(collection_name)
             self._setup_collections()
             return True
         else:
             return False
 
     @cached_property
     def embeddings_dimension(self):
         return len(self.generate_embedding("ABCDEF"))
 
     def get_similar_question_sql(self, question: str, **kwargs) -> list:
         results = self._client.search(
-            SQL_COLLECTION_NAME,
+            self.sql_collection_name,
             query_vector=self.generate_embedding(question),
             limit=self.n_results,
             with_payload=True,
         )
 
         return [dict(result.payload) for result in results]
 
     def get_related_ddl(self, question: str, **kwargs) -> list:
         results = self._client.search(
-            DDL_COLLECTION_NAME,
+            self.ddl_collection_name,
             query_vector=self.generate_embedding(question),
             limit=self.n_results,
             with_payload=True,
         )
 
         return [result.payload["ddl"] for result in results]
 
     def get_related_documentation(self, question: str, **kwargs) -> list:
         results = self._client.search(
-            DOCUMENTATION_COLLECTION_NAME,
+            self.documentation_collection_name,
             query_vector=self.generate_embedding(question),
             limit=self.n_results,
             with_payload=True,
         )
 
         return [result.payload["documentation"] for result in results]
 
@@ -278,45 +292,45 @@
             )
 
             results.extend(records)
 
         return results
 
     def _setup_collections(self):
-        if not self._client.collection_exists(SQL_COLLECTION_NAME):
+        if not self._client.collection_exists(self.sql_collection_name):
             self._client.create_collection(
-                collection_name=SQL_COLLECTION_NAME,
+                collection_name=self.sql_collection_name,
                 vectors_config=models.VectorParams(
                     size=self.embeddings_dimension,
                     distance=self.distance_metric,
                 ),
                 **self.collection_params,
             )
 
-        if not self._client.collection_exists(DDL_COLLECTION_NAME):
+        if not self._client.collection_exists(self.ddl_collection_name):
             self._client.create_collection(
-                collection_name=DDL_COLLECTION_NAME,
+                collection_name=self.ddl_collection_name,
                 vectors_config=models.VectorParams(
                     size=self.embeddings_dimension,
                     distance=self.distance_metric,
                 ),
                 **self.collection_params,
             )
-        if not self._client.collection_exists(DOCUMENTATION_COLLECTION_NAME):
+        if not self._client.collection_exists(self.documentation_collection_name):
             self._client.create_collection(
-                collection_name=DOCUMENTATION_COLLECTION_NAME,
+                collection_name=self.documentation_collection_name,
                 vectors_config=models.VectorParams(
                     size=self.embeddings_dimension,
                     distance=self.distance_metric,
                 ),
                 **self.collection_params,
             )
 
     def _format_point_id(self, id: str, collection_name: str) -> str:
-        return "{0}-{1}".format(id, ID_SUFFIXES[collection_name])
+        return "{0}-{1}".format(id, self.id_suffixes[collection_name])
 
     def _parse_point_id(self, id: str) -> Tuple[str, str]:
-        id, suffix = id.rsplit("-", 1)
-        for collection_name, suffix in ID_SUFFIXES.items():
-            if type == suffix:
+        id, curr_suffix = id.rsplit("-", 1)
+        for collection_name, suffix in self.id_suffixes.items():
+            if curr_suffix == suffix:
                 return id, collection_name
         raise ValueError(f"Invalid id {id}")
```

### Comparing `vanna-0.5.1/src/vanna/remote.py` & `vanna-0.5.2/src/vanna/remote.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/types/__init__.py` & `vanna-0.5.2/src/vanna/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/utils.py` & `vanna-0.5.2/src/vanna/utils.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/vannadb/vannadb_vector.py` & `vanna-0.5.2/src/vanna/vannadb/vannadb_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/src/vanna/vllm/vllm.py` & `vanna-0.5.2/src/vanna/vllm/vllm.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.1/PKG-INFO` & `vanna-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.5.1
+Version: 0.5.2
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

