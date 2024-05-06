# Comparing `tmp/vvm_lib-1.0.2.tar.gz` & `tmp/vvm_lib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvm_lib-1.0.2.tar", last modified: Wed Apr 24 07:14:21 2024, max compression
+gzip compressed data, was "vvm_lib-1.0.3.tar", last modified: Mon May  6 09:30:16 2024, max compression
```

## Comparing `vvm_lib-1.0.2.tar` & `vvm_lib-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 07:14:21.760422 vvm_lib-1.0.2/
--rw-rw-rw-   0        0        0      513 2024-04-24 07:14:21.759424 vvm_lib-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4707 2024-04-23 05:44:57.000000 vvm_lib-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 07:14:21.766421 vvm_lib-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-04-24 07:10:50.000000 vvm_lib-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:14:21.714396 vvm_lib-1.0.2/vvm_lib/
-drwxrwxrwx   0        0        0        0 2024-04-24 07:14:21.756424 vvm_lib-1.0.2/vvm_lib/DB/
--rw-rw-rw-   0        0        0       30 2024-04-22 09:33:28.000000 vvm_lib-1.0.2/vvm_lib/DB/__init__.py
--rw-rw-rw-   0        0        0     6351 2024-04-24 07:13:44.000000 vvm_lib-1.0.2/vvm_lib/DB/db.py
--rw-rw-rw-   0        0        0      229 2024-04-20 07:29:21.000000 vvm_lib-1.0.2/vvm_lib/__init__.py
--rw-rw-rw-   0        0        0     2747 2024-04-20 07:29:21.000000 vvm_lib-1.0.2/vvm_lib/google_book.py
--rw-rw-rw-   0        0        0     3545 2024-04-20 07:29:21.000000 vvm_lib-1.0.2/vvm_lib/greenplum.py
--rw-rw-rw-   0        0        0      654 2024-04-20 07:29:21.000000 vvm_lib-1.0.2/vvm_lib/mssql.py
--rw-rw-rw-   0        0        0      855 2024-04-20 07:29:21.000000 vvm_lib-1.0.2/vvm_lib/vault.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:14:21.758423 vvm_lib-1.0.2/vvm_lib.egg-info/
--rw-rw-rw-   0        0        0      513 2024-04-24 07:14:21.000000 vvm_lib-1.0.2/vvm_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2024-04-24 07:14:21.000000 vvm_lib-1.0.2/vvm_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 07:14:21.000000 vvm_lib-1.0.2/vvm_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 08:57:19.000000 vvm_lib-1.0.2/vvm_lib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      121 2024-04-24 07:14:21.000000 vvm_lib-1.0.2/vvm_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 07:14:21.000000 vvm_lib-1.0.2/vvm_lib.egg-info/top_level.txt
+drwxrwxr-x   0 vazhinskiy  (1000) vazhinskiy  (1000)        0 2024-05-06 09:30:16.740663 vvm_lib-1.0.3/
+-rw-r--r--   0 vazhinskiy  (1000) vazhinskiy  (1000)      494 2024-05-06 09:30:16.740663 vvm_lib-1.0.3/PKG-INFO
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)     4571 2024-05-06 09:01:07.000000 vvm_lib-1.0.3/README.md
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)       38 2024-05-06 09:30:16.740663 vvm_lib-1.0.3/setup.cfg
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)      767 2024-05-06 09:30:15.000000 vvm_lib-1.0.3/setup.py
+drwxrwxr-x   0 vazhinskiy  (1000) vazhinskiy  (1000)        0 2024-05-06 09:30:16.739663 vvm_lib-1.0.3/vvm_lib/
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)      225 2024-05-06 09:01:07.000000 vvm_lib-1.0.3/vvm_lib/__init__.py
+drwxrwxr-x   0 vazhinskiy  (1000) vazhinskiy  (1000)        0 2024-05-06 09:30:16.740663 vvm_lib-1.0.3/vvm_lib/db/
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)       29 2024-05-06 09:01:07.000000 vvm_lib-1.0.3/vvm_lib/db/__init__.py
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)     6186 2024-05-06 09:01:07.000000 vvm_lib-1.0.3/vvm_lib/db/db.py
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)     2687 2024-05-06 09:01:07.000000 vvm_lib-1.0.3/vvm_lib/google_book.py
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)     3465 2024-05-06 09:01:07.000000 vvm_lib-1.0.3/vvm_lib/greenplum.py
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)      635 2024-05-06 09:01:07.000000 vvm_lib-1.0.3/vvm_lib/mssql.py
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)      834 2024-05-06 09:01:07.000000 vvm_lib-1.0.3/vvm_lib/vault.py
+drwxrwxr-x   0 vazhinskiy  (1000) vazhinskiy  (1000)        0 2024-05-06 09:30:16.740663 vvm_lib-1.0.3/vvm_lib.egg-info/
+-rw-r--r--   0 vazhinskiy  (1000) vazhinskiy  (1000)      494 2024-05-06 09:30:16.000000 vvm_lib-1.0.3/vvm_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)      350 2024-05-06 09:30:16.000000 vvm_lib-1.0.3/vvm_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)        1 2024-05-06 09:30:16.000000 vvm_lib-1.0.3/vvm_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)        1 2024-05-06 09:29:55.000000 vvm_lib-1.0.3/vvm_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)      121 2024-05-06 09:30:16.000000 vvm_lib-1.0.3/vvm_lib.egg-info/requires.txt
+-rw-rw-r--   0 vazhinskiy  (1000) vazhinskiy  (1000)        8 2024-05-06 09:30:16.000000 vvm_lib-1.0.3/vvm_lib.egg-info/top_level.txt
```

### Comparing `vvm_lib-1.0.2/README.md` & `vvm_lib-1.0.3/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-Устанавливается
-pip install vvm-lib
-
-
-Основные функции:
-```
-from vvm_lib.vault import read_secret_data
-from vvm_lib.greenplum import postgres_query_read, insert_greenplum, select_postgres
-from vvm_lib.google_book import get_google_sheets, update_worksheet, clear_worksheet
-from vvm_lib.mssql import pymssql
-from vvm_lib.db import DB #new version 1.0
-```
-
-read_secret_data:
- Функция для получения доступов из vault
-
-    :param secret_path: Название секрета в DAS_team
-    :param vault_token_env: токент доступа
-    :param url: url vault
-    :return: Словарь с секретами
- 
-    пример:
-        secret_data = read_secret_data('ИМЯ', token_vault)
-
-
-postgres_query_read:
-    Функция для выполнения sql запросов не требующих вывода DF в базах greenplum и postgres
-
-    :param sql: drop table table_name;
-    :param connect: {'dbname': 'dwh', 'user': LOGIN,
-                  'password': PASSWORD, 'port': 5432,
-                  'host': 'greenplum.ru'}
-    :param name: уведомление об окончании запроса
-    :return: print(f'Запрос выполнен {name}'
- 
-    Пример:
-    postgres_query_read('''
-            drop table if exists ext_das.das_crm_task;
-            CREATE TABLE ext_das.das_crm_task (
-            "due_date" DATE,
-              "status" TEXT);''', conn, name='das_crm_task')
-
-
-insert_greenplum:
-  Функция для выполнения insert запросов для баз greenplum и postgres
-   
-```
-:param df: df - который необходимо записать в БД
-    :param table: название таблицы "scheme.table"
-    :param conn: {'dbname': 'dwh', 'user': LOGIN,
-                  'password': PASSWORD, 'port': 5432,
-                  'host': 'greenplum.ru'}
-    :return: уведомление о завершении
-    Пример:
-        insert_greenplum(total_df, 'scheme.table', conn)
-```
-select_postgres:
- Функция для select из greenplum и postgres
-
-    :param sql: select * from table;
-    :param connect: {'dbname': 'dwh', 'user': LOGIN,
-                  'password': PASSWORD, 'port': 5432,
-                  'host': 'greenplum.ru'}
-    :return: DataFrame
- 
-    Пример:
-        df = select_postgres("select * from table;", connect)
-
-
-get_google_sheets:
-
-```
-Функция получает данные из гугл таблицы
-    :param file_id: file_id
-    :param sheet_id: sheet_id
-    :param accesses: accesses - доступы
-    :return: DataFrame
- ```
-    Пример:
-        df = get_google_sheets(book_id='1Ws3QZFo2av', worksheet_id=0, accesses=accesses)
-
-
-update_worksheet:
- Функция для записи DataFrame в гугл таблицу
- 
-```
-  :param df: DataFrame
-    :param book_id: book_id, если записываем на ранее созданный лист, при создании нового не указываем,
-        None - по умолчанию
-    :param accesses:  accesses - Доступы
-    :param worksheet_id:  worksheet_id
-    :param create_new_sheet: Если нужно создать новый лист и записать в него, то ставим True, по умолчанию False
-    :param new_sheet: Если нужно создать новый лист указываем его имя
-    :return:
- ```
-    Пример:
-        update_worksheet(total,'1Ws3QZFo2av-', accesses, worksheet_id=0)
-
-clear_worksheet:
-  Функция для удаления всех данных с листа
- 
-
-```
-    :param book_id:  book_id
-    :param worksheet_id:  worksheet_id
-    :param accesses: accesses
-    :return:
- 
-   Пример:
-        clear_worksheet(book_id='1Ws3QZFo2av', worksheet_id=0, accesses=accesses)```
-```
-select_mssql:
- Функция для select из mssql
-    
-```
-:param sql: select * from table;
-    :param conn: {'server': 'master', 'user': f"domen\\{LOGIN}",
-               'password': PASSWORD, 'host': 'ms-sql.ru'}
-    :return: DataFrame
- 
-    Пример:
-        df = select_mssql("select * from table;", conn)
-```
-
-Новый модуль DB для работы с БД 'postgresql' , 'mssql', 'clickhouse':
-```
-mssql = DB(**creds_mssql, what_db='mssql')
-postg = DB(**creds_posgresql)
-click = DB(**creds_posgresql, what_db='clickhouse')
-
-select:
-postg.select(sql) -> pd.Dataframe
-
-postg.insert(pd.Dataframe, "название таблицы")
-
-```
+Устанавливается
+pip install vvm-lib
+
+
+Основные функции:
+```
+from vvm_lib.vault import read_secret_data
+from vvm_lib.greenplum import postgres_query_read, insert_greenplum, select_postgres
+from vvm_lib.google_book import get_google_sheets, update_worksheet, clear_worksheet
+from vvm_lib.mssql import pymssql
+from vvm_lib.db import DB #new version 1.0
+```
+
+read_secret_data:
+ Функция для получения доступов из vault
+
+    :param secret_path: Название секрета в DAS_team
+    :param vault_token_env: токент доступа
+    :param url: url vault
+    :return: Словарь с секретами
+ 
+    пример:
+        secret_data = read_secret_data('ИМЯ', token_vault)
+
+
+postgres_query_read:
+    Функция для выполнения sql запросов не требующих вывода DF в базах greenplum и postgres
+
+    :param sql: drop table table_name;
+    :param connect: {'dbname': 'dwh', 'user': LOGIN,
+                  'password': PASSWORD, 'port': 5432,
+                  'host': 'greenplum.ru'}
+    :param name: уведомление об окончании запроса
+    :return: print(f'Запрос выполнен {name}'
+ 
+    Пример:
+    postgres_query_read('''
+            drop table if exists ext_das.das_crm_task;
+            CREATE TABLE ext_das.das_crm_task (
+            "due_date" DATE,
+              "status" TEXT);''', conn, name='das_crm_task')
+
+
+insert_greenplum:
+  Функция для выполнения insert запросов для баз greenplum и postgres
+   
+```
+:param df: df - который необходимо записать в БД
+    :param table: название таблицы "scheme.table"
+    :param conn: {'dbname': 'dwh', 'user': LOGIN,
+                  'password': PASSWORD, 'port': 5432,
+                  'host': 'greenplum.ru'}
+    :return: уведомление о завершении
+    Пример:
+        insert_greenplum(total_df, 'scheme.table', conn)
+```
+select_postgres:
+ Функция для select из greenplum и postgres
+
+    :param sql: select * from table;
+    :param connect: {'dbname': 'dwh', 'user': LOGIN,
+                  'password': PASSWORD, 'port': 5432,
+                  'host': 'greenplum.ru'}
+    :return: DataFrame
+ 
+    Пример:
+        df = select_postgres("select * from table;", connect)
+
+
+get_google_sheets:
+
+```
+Функция получает данные из гугл таблицы
+    :param file_id: file_id
+    :param sheet_id: sheet_id
+    :param accesses: accesses - доступы
+    :return: DataFrame
+ ```
+    Пример:
+        df = get_google_sheets(book_id='1Ws3QZFo2av', worksheet_id=0, accesses=accesses)
+
+
+update_worksheet:
+ Функция для записи DataFrame в гугл таблицу
+ 
+```
+  :param df: DataFrame
+    :param book_id: book_id, если записываем на ранее созданный лист, при создании нового не указываем,
+        None - по умолчанию
+    :param accesses:  accesses - Доступы
+    :param worksheet_id:  worksheet_id
+    :param create_new_sheet: Если нужно создать новый лист и записать в него, то ставим True, по умолчанию False
+    :param new_sheet: Если нужно создать новый лист указываем его имя
+    :return:
+ ```
+    Пример:
+        update_worksheet(total,'1Ws3QZFo2av-', accesses, worksheet_id=0)
+
+clear_worksheet:
+  Функция для удаления всех данных с листа
+ 
+
+```
+    :param book_id:  book_id
+    :param worksheet_id:  worksheet_id
+    :param accesses: accesses
+    :return:
+ 
+   Пример:
+        clear_worksheet(book_id='1Ws3QZFo2av', worksheet_id=0, accesses=accesses)```
+```
+select_mssql:
+ Функция для select из mssql
+    
+```
+:param sql: select * from table;
+    :param conn: {'server': 'master', 'user': f"domen\\{LOGIN}",
+               'password': PASSWORD, 'host': 'ms-sql.ru'}
+    :return: DataFrame
+ 
+    Пример:
+        df = select_mssql("select * from table;", conn)
+```
+
+Новый модуль DB для работы с БД 'postgresql' , 'mssql', 'clickhouse':
+```
+mssql = DB(**creds_mssql, what_db='mssql')
+postg = DB(**creds_posgresql)
+click = DB(**creds_posgresql, what_db='clickhouse')
+
+select:
+postg.select(sql) -> pd.Dataframe
+
+postg.insert(pd.Dataframe, "название таблицы")
+
+```
 Описание в работе
```

### Comparing `vvm_lib-1.0.2/setup.py` & `vvm_lib-1.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from setuptools import setup
-
-
-setup(name='vvm_lib',
-      version='1.0.2',
-      description='my frequently used functions',
-      packages=[
-          'vvm_lib',
-          "vvm_lib.db",
-          ],
-      package_dir={
-        "vvm_lib": "vvm_lib",
-        "vvm_lib.db": "vvm_lib/db",
-    },
-      author_email='v.vazhinskiy@yandex.ru',
-      author="vvazhinskiy",
-      url="https://github.com/VazhikVM/vvm_lib",
-      zip_safe=False,
-      install_requires=[
-          "pandas",
-          "numpy",
-          "psycopg2-binary",
-          "hvac",
-          "openpyxl",
-          "requests-ntlm",
-          "oauth2client",
-          "gspread",
-          "pymssql",
-          "urllib3",
-          "clickhouse-connect",
-          "tzlocal",
-          ],
-      
+from setuptools import setup
+
+
+setup(name='vvm_lib',
+      version='1.0.3',
+      description='my frequently used functions',
+      packages=[
+          'vvm_lib',
+          "vvm_lib.db",
+          ],
+      package_dir={
+        "vvm_lib": "vvm_lib",
+        "vvm_lib.db": "vvm_lib/db",
+    },
+      author_email='v.vazhinskiy@yandex.ru',
+      author="vvazhinskiy",
+      url="https://github.com/VazhikVM/vvm_lib",
+      zip_safe=False,
+      install_requires=[
+          "pandas",
+          "numpy",
+          "psycopg2-binary",
+          "hvac",
+          "openpyxl",
+          "requests-ntlm",
+          "oauth2client",
+          "gspread",
+          "pymssql",
+          "urllib3",
+          "clickhouse-connect",
+          "tzlocal",
+          ],
+      
       )
```

### Comparing `vvm_lib-1.0.2/vvm_lib/DB/db.py` & `vvm_lib-1.0.3/vvm_lib/db/db.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-import pandas as pd
-import psycopg2
-import io
-import pymssql
-from clickhouse_connect import get_client, driver
-
-
-class DB:
-    """
-    Класс для работы с базами данных postgresql и mssql для моего личного пользования
-    для  'mssql', 'clickhouse' доступен только select
-    """
-
-    def __init__(self, dbname, user, password, port, host, what_db='postgresql') -> None:
-        """
-        :param dbname: Название БД
-        :param user: пользователь
-        :param password: пароль
-        :param port: порт
-        :param host: хост
-        :param what_db: 'postgresql' , 'mssql', 'clickhouse'
-        """
-        self.dbname = dbname
-        self.user = user
-        self.password = password
-        self.port = port
-        self.host = host
-        self.what_db = what_db
-
-    def open_connect(self):
-        """
-        :return: объект соединения
-        """
-        if self.what_db == 'postgresql':
-            return psycopg2.connect(dbname=self.dbname, user=self.user, password=self.password
-                                    , port=self.port, host=self.host)
-        elif self.what_db == 'mssql':
-            return pymssql.connect(server=self.dbname, user=self.user, password=self.password
-                                   , port=self.port, host=self.host)
-        elif self.what_db == 'clickhouse':
-            return get_client(database=self.dbname, user=self.user, password=self.password
-                              , port=self.port, host=self.host)
-
-    @staticmethod
-    def close_connect(connect):
-        """
-        :param connect:
-        :return: закрытие соединения
-        """
-        connect.close()
-        # print(f"Соединение закрыто")
-
-    def select(self, sql: str) -> pd.DataFrame:
-        """
-        Если нужно получить DATAFRAME
-        :param sql: запрос SQL
-        :return: pd.Dastaframe
-        """
-        connect = self.open_connect()
-        if self.what_db == 'clickhouse':
-            try:
-                result = connect.query_df(sql)
-            except driver.exceptions.ProgrammingError as error:
-                raise print(error)
-            finally:
-                self.close_connect(connect)
-            return result
-        else:
-            try:
-                with connect.cursor() as cursor:
-                    cursor.execute(sql)
-                    result = pd.DataFrame(cursor.fetchall(), columns=[col[0] for col in cursor.description])
-            except psycopg2.ProgrammingError as error:
-                raise print(error)
-            finally:
-                self.close_connect(connect)
-            return result
-
-    def insert(self, df: pd.DataFrame, table: str):
-        """
-        Вставка данных
-        :param df:
-        :param table:
-        :return:
-        """
-        csv_io = io.StringIO()
-        df.to_csv(csv_io, sep='\t', header=False, index=False)
-        csv_io.seek(0)
-        connect = self.open_connect()
-        with connect.cursor() as cursor:
-            cursor.copy_expert(f"""COPY {table} {str(tuple(df.columns)).replace("'", '"')} FROM STDIN  with (
-                                        format csv,delimiter '\t', force_null {str(tuple(df.columns))})""", csv_io)
-            connect.commit()
-        self.close_connect(connect)
-        print(f'Данные успешно записаны в {table} объем {len(df)} - cursor.rowcount {cursor.rowcount}')
-
-    def arbitrary_request(self, sql: str, query_name: str):
-        """
-        Свободный запрос без возврата данных
-        :param sql: запрос
-        :param query_name: название запроса
-        :return: print
-        """
-        connect = self.open_connect()
-        try:
-            with connect.cursor() as cursor:
-                cursor.execute(sql)
-                connect.commit()
-        except psycopg2.ProgrammingError as error:
-            raise print(error)
-        finally:
-            self.close_connect(connect)
-        print(f'Запрос выполнен {query_name}')
-
-    def drop(self, table_name: str):
-        """
-        Удаление таблицы
-        :param table_name: название таблицы со схемой
-        :return: print()
-        """
-        connect = self.open_connect()
-        try:
-            with connect.cursor() as cursor:
-                cursor.execute(f'drop table {table_name}')
-                connect.commit()
-        except psycopg2.ProgrammingError as error:
-            raise print(error)
-        finally:
-            self.close_connect(connect)
-        print(f'Таблица {table_name} удалена')
-
-    def grand(self, table_name: str, users: list):
-        """
-        Для предоставление прав на чтение
-        :param table_name: название таблицы
-        :param users: список пользователей, которым надо предоставить доступ
-        :return: print()
-        """
-        connect = self.open_connect()
-        try:
-            with connect.cursor() as cursor:
-                cursor.execute(f'grant select on {table_name} to {",".join(users)}')
-                connect.commit()
-        except psycopg2.ProgrammingError as error:
-            raise print(error)
-        finally:
-            self.close_connect(connect)
-        print(f'grant select к таблице {table_name} предоставлен для {" ,".join(users)}')
-
-    def truncate(self, table_name: str):
-        """
-        truncate таблицы
-        :param table_name: название таблицы
-        :return:  print()
-        """
-        connect = self.open_connect()
-        try:
-            with connect.cursor() as cursor:
-                cursor.execute(f'truncate table  {table_name}')
-                connect.commit()
-        except psycopg2.ProgrammingError as error:
-            raise print(error)
-        finally:
-            self.close_connect(connect)
-        print(f'Таблица {table_name} очищена')
+import pandas as pd
+import psycopg2
+import io
+import pymssql
+from clickhouse_connect import get_client, driver
+
+
+class DB:
+    """
+    Класс для работы с базами данных postgresql и mssql для моего личного пользования
+    для  'mssql', 'clickhouse' доступен только select
+    """
+
+    def __init__(self, dbname, user, password, port, host, what_db='postgresql') -> None:
+        """
+        :param dbname: Название БД
+        :param user: пользователь
+        :param password: пароль
+        :param port: порт
+        :param host: хост
+        :param what_db: 'postgresql' , 'mssql', 'clickhouse'
+        """
+        self.dbname = dbname
+        self.user = user
+        self.password = password
+        self.port = port
+        self.host = host
+        self.what_db = what_db
+
+    def open_connect(self):
+        """
+        :return: объект соединения
+        """
+        if self.what_db == 'postgresql':
+            return psycopg2.connect(dbname=self.dbname, user=self.user, password=self.password
+                                    , port=self.port, host=self.host)
+        elif self.what_db == 'mssql':
+            return pymssql.connect(server=self.dbname, user=self.user, password=self.password
+                                   , port=self.port, host=self.host)
+        elif self.what_db == 'clickhouse':
+            return get_client(database=self.dbname, user=self.user, password=self.password
+                              , port=self.port, host=self.host)
+
+    @staticmethod
+    def close_connect(connect):
+        """
+        :param connect:
+        :return: закрытие соединения
+        """
+        connect.close()
+        # print(f"Соединение закрыто")
+
+    def select(self, sql: str) -> pd.DataFrame:
+        """
+        Если нужно получить DATAFRAME
+        :param sql: запрос SQL
+        :return: pd.Dastaframe
+        """
+        connect = self.open_connect()
+        if self.what_db == 'clickhouse':
+            try:
+                result = connect.query_df(sql)
+            except driver.exceptions.ProgrammingError as error:
+                raise print(error)
+            finally:
+                self.close_connect(connect)
+            return result
+        else:
+            try:
+                with connect.cursor() as cursor:
+                    cursor.execute(sql)
+                    result = pd.DataFrame(cursor.fetchall(), columns=[col[0] for col in cursor.description])
+            except psycopg2.ProgrammingError as error:
+                raise print(error)
+            finally:
+                self.close_connect(connect)
+            return result
+
+    def insert(self, df: pd.DataFrame, table: str):
+        """
+        Вставка данных
+        :param df:
+        :param table:
+        :return:
+        """
+        csv_io = io.StringIO()
+        df.to_csv(csv_io, sep='\t', header=False, index=False)
+        csv_io.seek(0)
+        connect = self.open_connect()
+        with connect.cursor() as cursor:
+            cursor.copy_expert(f"""COPY {table} {str(tuple(df.columns)).replace("'", '"')} FROM STDIN  with (
+                                        format csv,delimiter '\t', force_null {str(tuple(df.columns))})""", csv_io)
+            connect.commit()
+        self.close_connect(connect)
+        print(f'Данные успешно записаны в {table} объем {len(df)} - cursor.rowcount {cursor.rowcount}')
+
+    def arbitrary_request(self, sql: str, query_name: str):
+        """
+        Свободный запрос без возврата данных
+        :param sql: запрос
+        :param query_name: название запроса
+        :return: print
+        """
+        connect = self.open_connect()
+        try:
+            with connect.cursor() as cursor:
+                cursor.execute(sql)
+                connect.commit()
+        except psycopg2.ProgrammingError as error:
+            raise print(error)
+        finally:
+            self.close_connect(connect)
+        print(f'Запрос выполнен {query_name}')
+
+    def drop(self, table_name: str):
+        """
+        Удаление таблицы
+        :param table_name: название таблицы со схемой
+        :return: print()
+        """
+        connect = self.open_connect()
+        try:
+            with connect.cursor() as cursor:
+                cursor.execute(f'drop table {table_name}')
+                connect.commit()
+        except psycopg2.ProgrammingError as error:
+            raise print(error)
+        finally:
+            self.close_connect(connect)
+        print(f'Таблица {table_name} удалена')
+
+    def grand(self, table_name: str, users: list):
+        """
+        Для предоставление прав на чтение
+        :param table_name: название таблицы
+        :param users: список пользователей, которым надо предоставить доступ
+        :return: print()
+        """
+        connect = self.open_connect()
+        try:
+            with connect.cursor() as cursor:
+                cursor.execute(f'grant select on {table_name} to {",".join(users)}')
+                connect.commit()
+        except psycopg2.ProgrammingError as error:
+            raise print(error)
+        finally:
+            self.close_connect(connect)
+        print(f'grant select к таблице {table_name} предоставлен для {" ,".join(users)}')
+
+    def truncate(self, table_name: str):
+        """
+        truncate таблицы
+        :param table_name: название таблицы
+        :return:  print()
+        """
+        connect = self.open_connect()
+        try:
+            with connect.cursor() as cursor:
+                cursor.execute(f'truncate table  {table_name}')
+                connect.commit()
+        except psycopg2.ProgrammingError as error:
+            raise print(error)
+        finally:
+            self.close_connect(connect)
+        print(f'Таблица {table_name} очищена')
```

### Comparing `vvm_lib-1.0.2/vvm_lib/google_book.py` & `vvm_lib-1.0.3/vvm_lib/google_book.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import pandas as pd
-import gspread
-from oauth2client.service_account import ServiceAccountCredentials
-
-
-def get_google_sheets(file_id: str, sheet_id: str, accesses: dict) -> pd.DataFrame:
-    """
-    Функция получает данные из гугл таблицы
-    :param file_id: file_id
-    :param sheet_id: sheet_id
-    :param accesses: accesses - доступы
-    :return: DataFrame
-    """
-    credentials = ServiceAccountCredentials.from_json_keyfile_dict(accesses)
-    gc = gspread.authorize(credentials)
-    return pd.DataFrame(gc.open_by_key(file_id).get_worksheet_by_id(sheet_id).get_all_records())
-
-
-def update_worksheet(df: pd.DataFrame, book_id: str, accesses: dict, worksheet_id: str = None
-                     , create_new_sheet: bool = False, new_sheet: str = None):
-    """
-    Функция для записи DataFrame в гугл таблицу
-    :param df: DataFrame
-    :param book_id: book_id, если записываем на ранее созданный лист, при создании нового не указываем,
-        None - по умолчанию
-    :param accesses:  accesses - Доступы
-    :param worksheet_id:  worksheet_id
-    :param create_new_sheet: Если нужно создать новый лист и записать в него, то ставим True, по умолчанию False
-    :param new_sheet: Если нужно создать новый лист указываем его имя
-    :return:
-    """
-    credentials = ServiceAccountCredentials.from_json_keyfile_dict(accesses)
-    client = gspread.authorize(credentials)
-    spreadsheet = client.open_by_key(book_id)
-    if create_new_sheet:
-        worksheet = spreadsheet.add_worksheet(new_sheet, rows=len(df.columns), cols=len(df.columns))
-    else:
-        worksheet = spreadsheet.get_worksheet_by_id(worksheet_id)
-    for i in df.columns:
-        df[i] = df[i].astype('str')
-
-    worksheet.update(range_name=f'1:{len(df.columns)}{len(df) + 1}',
-                     values=[df.columns.values.tolist()] + df.values.tolist())
-    print('Готово')
-
-
-def clear_worksheet(book_id: str, worksheet_id: str, accesses: dict):
-    """
-    Функция для удаления всех данных с листа
-    :param book_id:  book_id
-    :param worksheet_id:  worksheet_id
-    :param accesses: accesses
-    :return:
-    """
-    credentials = ServiceAccountCredentials.from_json_keyfile_dict(accesses)
-    client = gspread.authorize(credentials)
-    spreadsheet = client.open_by_key(book_id)
-    worksheet = spreadsheet.get_worksheet_by_id(worksheet_id)
-    worksheet.clear()
-    print(f'Лист {worksheet_id} очищен')
+import pandas as pd
+import gspread
+from oauth2client.service_account import ServiceAccountCredentials
+
+
+def get_google_sheets(file_id: str, sheet_id: str, accesses: dict) -> pd.DataFrame:
+    """
+    Функция получает данные из гугл таблицы
+    :param file_id: file_id
+    :param sheet_id: sheet_id
+    :param accesses: accesses - доступы
+    :return: DataFrame
+    """
+    credentials = ServiceAccountCredentials.from_json_keyfile_dict(accesses)
+    gc = gspread.authorize(credentials)
+    return pd.DataFrame(gc.open_by_key(file_id).get_worksheet_by_id(sheet_id).get_all_records())
+
+
+def update_worksheet(df: pd.DataFrame, book_id: str, accesses: dict, worksheet_id: str = None
+                     , create_new_sheet: bool = False, new_sheet: str = None):
+    """
+    Функция для записи DataFrame в гугл таблицу
+    :param df: DataFrame
+    :param book_id: book_id, если записываем на ранее созданный лист, при создании нового не указываем,
+        None - по умолчанию
+    :param accesses:  accesses - Доступы
+    :param worksheet_id:  worksheet_id
+    :param create_new_sheet: Если нужно создать новый лист и записать в него, то ставим True, по умолчанию False
+    :param new_sheet: Если нужно создать новый лист указываем его имя
+    :return:
+    """
+    credentials = ServiceAccountCredentials.from_json_keyfile_dict(accesses)
+    client = gspread.authorize(credentials)
+    spreadsheet = client.open_by_key(book_id)
+    if create_new_sheet:
+        worksheet = spreadsheet.add_worksheet(new_sheet, rows=len(df.columns), cols=len(df.columns))
+    else:
+        worksheet = spreadsheet.get_worksheet_by_id(worksheet_id)
+    for i in df.columns:
+        df[i] = df[i].astype('str')
+
+    worksheet.update(range_name=f'1:{len(df.columns)}{len(df) + 1}',
+                     values=[df.columns.values.tolist()] + df.values.tolist())
+    print('Готово')
+
+
+def clear_worksheet(book_id: str, worksheet_id: str, accesses: dict):
+    """
+    Функция для удаления всех данных с листа
+    :param book_id:  book_id
+    :param worksheet_id:  worksheet_id
+    :param accesses: accesses
+    :return:
+    """
+    credentials = ServiceAccountCredentials.from_json_keyfile_dict(accesses)
+    client = gspread.authorize(credentials)
+    spreadsheet = client.open_by_key(book_id)
+    worksheet = spreadsheet.get_worksheet_by_id(worksheet_id)
+    worksheet.clear()
+    print(f'Лист {worksheet_id} очищен')
```

### Comparing `vvm_lib-1.0.2/vvm_lib/greenplum.py` & `vvm_lib-1.0.3/vvm_lib/greenplum.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import pandas as pd
-import psycopg2
-import io
-from collections import defaultdict
-
-
-def select_greenplum(query_sql, connect=None, types=defaultdict(str, A="int", B="float")):
-    # with psycopg2.connect(**connect) as postgres_conn:
-    #     with postgres_conn.cursor() as postgres_cursor:
-    #         output = io.BytesIO()
-    #         postgres_cursor.copy_expert(f"COPY ({query_sql}) TO STDOUT (FORMAT 'csv', HEADER true)", output)
-    #         output.seek(0)
-    # return pd.read_csv(output, engine="python", encoding='utf-8')
-    pass
-
-
-def select_postgres(sql: str, connect: dict) -> pd.DataFrame:
-    """
-    Функция для select из greenplum и postgres
-    :param sql: select * from table;
-    :param connect: {'dbname': 'dwh', 'user': LOGIN,
-                  'password': PASSWORD, 'port': 5432,
-                  'host': 'greenplum.ru'}
-    :return: DataFrame
-
-    Пример:
-        df = select_postgres("select * from table;", connect)
-    """
-    with psycopg2.connect(**connect) as postgres_conn:
-        with postgres_conn.cursor() as postgres_cursor:
-            postgres_cursor.execute(sql)
-            result = pd.DataFrame(postgres_cursor.fetchall(), columns=[col[0] for col in postgres_cursor.description])
-    return result
-
-
-def postgres_query_read(sql: str, connect: dict, name: str = 'task_1'):
-    """
-    Функция для выполнения sql запросов не требующих вывода DF в базах greenplum и postgres
-    :param sql: drop table table_name;
-    :param connect: {'dbname': 'dwh', 'user': LOGIN,
-                  'password': PASSWORD, 'port': 5432,
-                  'host': 'greenplum.ru'}
-    :param name: уведомление об окончании запроса
-    :return: print(f'Запрос выполнен {name}'
-
-    Пример:
-    postgres_query_read('''
-            drop table if exists ext_das.das_crm_task;
-            CREATE TABLE ext_das.das_crm_task (
-            "due_date" DATE,
-              "status" TEXT);''', conn, name='das_crm_task')
-    """
-    with psycopg2.connect(**connect) as postgres_conn:
-        with postgres_conn.cursor() as postgres_cursor:
-            postgres_cursor.execute(sql)
-            postgres_conn.commit()
-    print(f'Запрос выполнен {name}')
-
-
-def insert_greenplum(df: pd.DataFrame, table: str, conn: dict):
-    """
-    Функция для выполнения insert запросов для баз greenplum и postgres
-    :param df: df - который необходимо записать в БД
-    :param table: название таблицы "scheme.table"
-    :param conn: {'dbname': 'dwh', 'user': LOGIN,
-                  'password': PASSWORD, 'port': 5432,
-                  'host': 'greenplum.ru'}
-    :return: уведомление о завершении
-    Пример:
-        insert_greenplum(total_df, 'scheme.table', conn)
-    """
-    csv_io = io.StringIO()
-    df.to_csv(csv_io, sep='\t', header=False, index=False)
-    csv_io.seek(0)
-    with psycopg2.connect(**conn) as conn_green:
-        with conn_green.cursor() as greenplum:
-            greenplum.copy_expert(f"""COPY {table} {str(tuple(df.columns)).replace("'", '"')} FROM STDIN  with (
-                                    format csv,delimiter '\t', force_null {str(tuple(df.columns))})""", csv_io)
-            conn_green.commit()
-    print(f'Данные успешно записаны в {table} объем {len(df)}')
+import pandas as pd
+import psycopg2
+import io
+from collections import defaultdict
+
+
+def select_greenplum(query_sql, connect=None, types=defaultdict(str, A="int", B="float")):
+    # with psycopg2.connect(**connect) as postgres_conn:
+    #     with postgres_conn.cursor() as postgres_cursor:
+    #         output = io.BytesIO()
+    #         postgres_cursor.copy_expert(f"COPY ({query_sql}) TO STDOUT (FORMAT 'csv', HEADER true)", output)
+    #         output.seek(0)
+    # return pd.read_csv(output, engine="python", encoding='utf-8')
+    pass
+
+
+def select_postgres(sql: str, connect: dict) -> pd.DataFrame:
+    """
+    Функция для select из greenplum и postgres
+    :param sql: select * from table;
+    :param connect: {'dbname': 'dwh', 'user': LOGIN,
+                  'password': PASSWORD, 'port': 5432,
+                  'host': 'greenplum.ru'}
+    :return: DataFrame
+
+    Пример:
+        df = select_postgres("select * from table;", connect)
+    """
+    with psycopg2.connect(**connect) as postgres_conn:
+        with postgres_conn.cursor() as postgres_cursor:
+            postgres_cursor.execute(sql)
+            result = pd.DataFrame(postgres_cursor.fetchall(), columns=[col[0] for col in postgres_cursor.description])
+    return result
+
+
+def postgres_query_read(sql: str, connect: dict, name: str = 'task_1'):
+    """
+    Функция для выполнения sql запросов не требующих вывода DF в базах greenplum и postgres
+    :param sql: drop table table_name;
+    :param connect: {'dbname': 'dwh', 'user': LOGIN,
+                  'password': PASSWORD, 'port': 5432,
+                  'host': 'greenplum.ru'}
+    :param name: уведомление об окончании запроса
+    :return: print(f'Запрос выполнен {name}'
+
+    Пример:
+    postgres_query_read('''
+            drop table if exists ext_das.das_crm_task;
+            CREATE TABLE ext_das.das_crm_task (
+            "due_date" DATE,
+              "status" TEXT);''', conn, name='das_crm_task')
+    """
+    with psycopg2.connect(**connect) as postgres_conn:
+        with postgres_conn.cursor() as postgres_cursor:
+            postgres_cursor.execute(sql)
+            postgres_conn.commit()
+    print(f'Запрос выполнен {name}')
+
+
+def insert_greenplum(df: pd.DataFrame, table: str, conn: dict):
+    """
+    Функция для выполнения insert запросов для баз greenplum и postgres
+    :param df: df - который необходимо записать в БД
+    :param table: название таблицы "scheme.table"
+    :param conn: {'dbname': 'dwh', 'user': LOGIN,
+                  'password': PASSWORD, 'port': 5432,
+                  'host': 'greenplum.ru'}
+    :return: уведомление о завершении
+    Пример:
+        insert_greenplum(total_df, 'scheme.table', conn)
+    """
+    csv_io = io.StringIO()
+    df.to_csv(csv_io, sep='\t', header=False, index=False)
+    csv_io.seek(0)
+    with psycopg2.connect(**conn) as conn_green:
+        with conn_green.cursor() as greenplum:
+            greenplum.copy_expert(f"""COPY {table} {str(tuple(df.columns)).replace("'", '"')} FROM STDIN  with (
+                                    format csv,delimiter '\t', force_null {str(tuple(df.columns))})""", csv_io)
+            conn_green.commit()
+    print(f'Данные успешно записаны в {table} объем {len(df)}')
```

### Comparing `vvm_lib-1.0.2/vvm_lib/mssql.py` & `vvm_lib-1.0.3/vvm_lib/mssql.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import pandas as pd
-import pymssql
-
-
-def select_mssql(sql: str, conn: dict) -> pd.DataFrame:
-    """
-    Функция для select из mssql
-    :param sql: select * from table;
-    :param conn: {'server': 'master', 'user': f"domen\\{LOGIN}",
-               'password': PASSWORD, 'host': 'ms-sql.ru'}
-    :return: DataFrame
-
-    Пример:
-        df = select_mssql("select * from table;", conn)
-    """
-    with pymssql.connect(**conn, as_dict=True) as conn_mssql:
-        with conn_mssql.cursor() as mssql_cursor:
-            mssql_cursor.execute(sql)
-            return pd.DataFrame([row for row in mssql_cursor.fetchall()])
+import pandas as pd
+import pymssql
+
+
+def select_mssql(sql: str, conn: dict) -> pd.DataFrame:
+    """
+    Функция для select из mssql
+    :param sql: select * from table;
+    :param conn: {'server': 'master', 'user': f"domen\\{LOGIN}",
+               'password': PASSWORD, 'host': 'ms-sql.ru'}
+    :return: DataFrame
+
+    Пример:
+        df = select_mssql("select * from table;", conn)
+    """
+    with pymssql.connect(**conn, as_dict=True) as conn_mssql:
+        with conn_mssql.cursor() as mssql_cursor:
+            mssql_cursor.execute(sql)
+            return pd.DataFrame([row for row in mssql_cursor.fetchall()])
```

