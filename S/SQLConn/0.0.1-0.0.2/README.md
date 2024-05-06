# Comparing `tmp/SQLConn-0.0.1.tar.gz` & `tmp/SQLConn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLConn-0.0.1.tar", last modified: Mon May  6 08:52:54 2024, max compression
+gzip compressed data, was "SQLConn-0.0.2.tar", last modified: Mon May  6 09:15:09 2024, max compression
```

## Comparing `SQLConn-0.0.1.tar` & `SQLConn-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 08:52:54.259603 SQLConn-0.0.1/
--rw-rw-rw-   0        0        0     9233 2024-05-06 08:52:54.256136 SQLConn-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8818 2024-05-06 07:51:49.000000 SQLConn-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 08:52:54.232191 SQLConn-0.0.1/SQLConn/
--rw-rw-rw-   0        0        0     2565 2024-05-06 07:22:05.000000 SQLConn-0.0.1/SQLConn/SQLConn.py
--rw-rw-rw-   0        0        0      290 2024-05-06 08:47:30.000000 SQLConn-0.0.1/SQLConn/__init__.py
--rw-rw-rw-   0        0        0      699 2024-05-06 07:13:25.000000 SQLConn-0.0.1/SQLConn/mssql.py
--rw-rw-rw-   0        0        0      696 2024-05-06 07:39:09.000000 SQLConn-0.0.1/SQLConn/mysql.py
--rw-rw-rw-   0        0        0      693 2024-05-06 07:06:09.000000 SQLConn-0.0.1/SQLConn/oracle.py
--rw-rw-rw-   0        0        0      707 2024-05-06 07:39:09.000000 SQLConn-0.0.1/SQLConn/postgresql.py
--rw-rw-rw-   0        0        0      350 2024-05-06 08:49:51.000000 SQLConn-0.0.1/SQLConn/sqlite.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:52:54.253136 SQLConn-0.0.1/SQLConn.egg-info/
--rw-rw-rw-   0        0        0     9233 2024-05-06 08:52:54.000000 SQLConn-0.0.1/SQLConn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-05-06 08:52:54.000000 SQLConn-0.0.1/SQLConn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 08:52:54.000000 SQLConn-0.0.1/SQLConn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-06 08:52:54.000000 SQLConn-0.0.1/SQLConn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-06 08:52:54.000000 SQLConn-0.0.1/SQLConn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 08:52:54.260603 SQLConn-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      637 2024-05-06 08:45:21.000000 SQLConn-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:15:09.138839 SQLConn-0.0.2/
+-rw-rw-rw-   0        0        0     9260 2024-05-06 09:15:09.136823 SQLConn-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8818 2024-05-06 08:56:32.000000 SQLConn-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 09:15:09.116820 SQLConn-0.0.2/SQLConn/
+-rw-rw-rw-   0        0        0     2565 2024-05-06 07:22:05.000000 SQLConn-0.0.2/SQLConn/SQLConn.py
+-rw-rw-rw-   0        0        0      290 2024-05-06 08:47:30.000000 SQLConn-0.0.2/SQLConn/__init__.py
+-rw-rw-rw-   0        0        0      699 2024-05-06 07:13:25.000000 SQLConn-0.0.2/SQLConn/mssql.py
+-rw-rw-rw-   0        0        0      696 2024-05-06 07:39:09.000000 SQLConn-0.0.2/SQLConn/mysql.py
+-rw-rw-rw-   0        0        0      693 2024-05-06 08:58:38.000000 SQLConn-0.0.2/SQLConn/oracle.py
+-rw-rw-rw-   0        0        0      707 2024-05-06 07:39:09.000000 SQLConn-0.0.2/SQLConn/postgresql.py
+-rw-rw-rw-   0        0        0      350 2024-05-06 08:49:51.000000 SQLConn-0.0.2/SQLConn/sqlite.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:15:09.133931 SQLConn-0.0.2/SQLConn.egg-info/
+-rw-rw-rw-   0        0        0     9260 2024-05-06 09:15:08.000000 SQLConn-0.0.2/SQLConn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-05-06 09:15:08.000000 SQLConn-0.0.2/SQLConn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:15:08.000000 SQLConn-0.0.2/SQLConn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-06 09:15:08.000000 SQLConn-0.0.2/SQLConn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 09:15:08.000000 SQLConn-0.0.2/SQLConn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 09:15:09.139917 SQLConn-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      650 2024-05-06 09:15:06.000000 SQLConn-0.0.2/setup.py
```

### Comparing `SQLConn-0.0.1/PKG-INFO` & `SQLConn-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: SQLConn
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package facilitates easy SQL database integration.
 Home-page: https://github.com/janyoungjin/SQLConn
 Author: janyoungjin
 Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
 Description-Content-Type: text/markdown
 Requires-Dist: mysqlclient
 Requires-Dist: pandas
 Requires-Dist: cx_oracle
 Requires-Dist: psycopg2
 Requires-Dist: pymssql
+Requires-Dist: sqlalchemy
 
 # SQLConn
 ## 한국어 버전(Korean Version)
 SQLConn은 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하여 데이터를 쉽게 조작하고 관리할 수 있는 Python 패키지입니다. 이 패키지는 MySQL, PostgreSQL, Microsoft SQL Server, Oracle 및 SQLite 데이터베이스에 대한 지원을 포함합니다.
 
 ### 기능
 
@@ -53,16 +54,16 @@
 |--------------|--------------------------------------------------------------|------------------------------|
 | `to_DataFrame` | SQL 쿼리를 실행하고 결과를 pandas DataFrame으로 반환합니다. | Show, Select 커맨드만 가능    |
 | `execute`      | 데이터베이스에서 SQL 쿼리를 실행하되 결과를 반환하지 않습니다. | Show, Select 커맨드 사용 불가능 |
 | `to_csv`       | SQL 쿼리 결과를 CSV 파일로 저장합니다.                       | Show, Select 커맨드만 가능    |
 | `to_excel`     | SQL 쿼리 결과를 Excel 파일로 저장합니다.                     | Show, Select 커맨드만 가능    |
 | `to_tsv`       | SQL 쿼리 결과를 TSV 파일로 저장합니다.                       | Show, Select 커맨드만 가능    |
 | `to_sql`       | 다른 데이터베이스에 SQL 쿼리 결과를 저장합니다.              | Show, Select 커맨드만 가능    |
-| `URL`          | 데이터베이스 연결 URL을 제공합니다.                          | 쓰기용 프로퍼티               |
-| `engine`       | 데이터베이스 연결을 위한 SQLAlchemy 엔진을 제공합니다.       | 쓰기용 프로퍼티               |
+| `URL`          | 데이터베이스 연결 URL을 제공합니다.                          | 읽기용 프로퍼티               |
+| `engine`       | 데이터베이스 연결을 위한 SQLAlchemy 엔진을 제공합니다.       | 읽기용 프로퍼티               |
 
 
 ### 사용예제
 각 데이터베이스 연결 객체를 생성하고 사용하는 기본적인 방법은 다음과 같습니다:
 ```py
 from SQLConn import MySQLConn, PostgreSQLConn
```

### Comparing `SQLConn-0.0.1/README.md` & `SQLConn-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 |--------------|--------------------------------------------------------------|------------------------------|
 | `to_DataFrame` | SQL 쿼리를 실행하고 결과를 pandas DataFrame으로 반환합니다. | Show, Select 커맨드만 가능    |
 | `execute`      | 데이터베이스에서 SQL 쿼리를 실행하되 결과를 반환하지 않습니다. | Show, Select 커맨드 사용 불가능 |
 | `to_csv`       | SQL 쿼리 결과를 CSV 파일로 저장합니다.                       | Show, Select 커맨드만 가능    |
 | `to_excel`     | SQL 쿼리 결과를 Excel 파일로 저장합니다.                     | Show, Select 커맨드만 가능    |
 | `to_tsv`       | SQL 쿼리 결과를 TSV 파일로 저장합니다.                       | Show, Select 커맨드만 가능    |
 | `to_sql`       | 다른 데이터베이스에 SQL 쿼리 결과를 저장합니다.              | Show, Select 커맨드만 가능    |
-| `URL`          | 데이터베이스 연결 URL을 제공합니다.                          | 쓰기용 프로퍼티               |
-| `engine`       | 데이터베이스 연결을 위한 SQLAlchemy 엔진을 제공합니다.       | 쓰기용 프로퍼티               |
+| `URL`          | 데이터베이스 연결 URL을 제공합니다.                          | 읽기용 프로퍼티               |
+| `engine`       | 데이터베이스 연결을 위한 SQLAlchemy 엔진을 제공합니다.       | 읽기용 프로퍼티               |
 
 
 ### 사용예제
 각 데이터베이스 연결 객체를 생성하고 사용하는 기본적인 방법은 다음과 같습니다:
 ```py
 from SQLConn import MySQLConn, PostgreSQLConn
```

### Comparing `SQLConn-0.0.1/SQLConn/SQLConn.py` & `SQLConn-0.0.2/SQLConn/SQLConn.py`

 * *Files identical despite different names*

### Comparing `SQLConn-0.0.1/SQLConn/mssql.py` & `SQLConn-0.0.2/SQLConn/mssql.py`

 * *Files identical despite different names*

### Comparing `SQLConn-0.0.1/SQLConn/mysql.py` & `SQLConn-0.0.2/SQLConn/mysql.py`

 * *Files identical despite different names*

### Comparing `SQLConn-0.0.1/SQLConn/oracle.py` & `SQLConn-0.0.2/SQLConn/oracle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cx_Oracle
-from SQLconn import SQLconn
-class OracleConn(SQLconn):
+from SQLConn import SQLConn
+class OracleConn(SQLConn):
     def __init__(self,password:str,host:str='127.0.0.1',user:str="system",database:str="xe",port:str|int=1521) -> None:
         super.__init__()
         self.__host=host
         self.__user=user
         self.__password=password
         self.__database=database
         self.__port=int(port)
```

### Comparing `SQLConn-0.0.1/SQLConn/postgresql.py` & `SQLConn-0.0.2/SQLConn/postgresql.py`

 * *Files identical despite different names*

### Comparing `SQLConn-0.0.1/SQLConn.egg-info/PKG-INFO` & `SQLConn-0.0.2/SQLConn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: SQLConn
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package facilitates easy SQL database integration.
 Home-page: https://github.com/janyoungjin/SQLConn
 Author: janyoungjin
 Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
 Description-Content-Type: text/markdown
 Requires-Dist: mysqlclient
 Requires-Dist: pandas
 Requires-Dist: cx_oracle
 Requires-Dist: psycopg2
 Requires-Dist: pymssql
+Requires-Dist: sqlalchemy
 
 # SQLConn
 ## 한국어 버전(Korean Version)
 SQLConn은 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하여 데이터를 쉽게 조작하고 관리할 수 있는 Python 패키지입니다. 이 패키지는 MySQL, PostgreSQL, Microsoft SQL Server, Oracle 및 SQLite 데이터베이스에 대한 지원을 포함합니다.
 
 ### 기능
 
@@ -53,16 +54,16 @@
 |--------------|--------------------------------------------------------------|------------------------------|
 | `to_DataFrame` | SQL 쿼리를 실행하고 결과를 pandas DataFrame으로 반환합니다. | Show, Select 커맨드만 가능    |
 | `execute`      | 데이터베이스에서 SQL 쿼리를 실행하되 결과를 반환하지 않습니다. | Show, Select 커맨드 사용 불가능 |
 | `to_csv`       | SQL 쿼리 결과를 CSV 파일로 저장합니다.                       | Show, Select 커맨드만 가능    |
 | `to_excel`     | SQL 쿼리 결과를 Excel 파일로 저장합니다.                     | Show, Select 커맨드만 가능    |
 | `to_tsv`       | SQL 쿼리 결과를 TSV 파일로 저장합니다.                       | Show, Select 커맨드만 가능    |
 | `to_sql`       | 다른 데이터베이스에 SQL 쿼리 결과를 저장합니다.              | Show, Select 커맨드만 가능    |
-| `URL`          | 데이터베이스 연결 URL을 제공합니다.                          | 쓰기용 프로퍼티               |
-| `engine`       | 데이터베이스 연결을 위한 SQLAlchemy 엔진을 제공합니다.       | 쓰기용 프로퍼티               |
+| `URL`          | 데이터베이스 연결 URL을 제공합니다.                          | 읽기용 프로퍼티               |
+| `engine`       | 데이터베이스 연결을 위한 SQLAlchemy 엔진을 제공합니다.       | 읽기용 프로퍼티               |
 
 
 ### 사용예제
 각 데이터베이스 연결 객체를 생성하고 사용하는 기본적인 방법은 다음과 같습니다:
 ```py
 from SQLConn import MySQLConn, PostgreSQLConn
```

### Comparing `SQLConn-0.0.1/setup.py` & `SQLConn-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='SQLConn',
-    version='0.0.1',
+    version='0.0.2',
     description='This package facilitates easy SQL database integration.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='janyoungjin',
-    install_requires=['mysqlclient', 'pandas', 'cx_oracle', 'psycopg2', 'pymssql'],
+    install_requires=['mysqlclient', 'pandas', 'cx_oracle', 'psycopg2', 'pymssql','sqlalchemy'],
     packages=find_packages(exclude=[]),
     url='https://github.com/janyoungjin/SQLConn',
     keywords=['mysql', 'postgresql', 'sqlite', 'mssql', 'oracle', 'sql']
 )
```

