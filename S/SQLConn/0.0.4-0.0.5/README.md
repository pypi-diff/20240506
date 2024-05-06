# Comparing `tmp/SQLConn-0.0.4.tar.gz` & `tmp/SQLConn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLConn-0.0.4.tar", last modified: Mon May  6 09:40:59 2024, max compression
+gzip compressed data, was "SQLConn-0.0.5.tar", last modified: Mon May  6 09:44:57 2024, max compression
```

## Comparing `SQLConn-0.0.4.tar` & `SQLConn-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 09:40:59.401677 SQLConn-0.0.4/
--rw-rw-rw-   0        0        0     9260 2024-05-06 09:40:59.400017 SQLConn-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     8818 2024-05-06 08:56:32.000000 SQLConn-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 09:40:59.377308 SQLConn-0.0.4/SQLConn/
--rw-rw-rw-   0        0        0     5570 2024-05-06 09:26:10.000000 SQLConn-0.0.4/SQLConn/SQLConn.py
--rw-rw-rw-   0        0        0      293 2024-05-06 09:40:40.000000 SQLConn-0.0.4/SQLConn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:40:59.398018 SQLConn-0.0.4/SQLConn.egg-info/
--rw-rw-rw-   0        0        0     9260 2024-05-06 09:40:59.000000 SQLConn-0.0.4/SQLConn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2024-05-06 09:40:59.000000 SQLConn-0.0.4/SQLConn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 09:40:59.000000 SQLConn-0.0.4/SQLConn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-06 09:40:59.000000 SQLConn-0.0.4/SQLConn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-06 09:40:59.000000 SQLConn-0.0.4/SQLConn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 09:40:59.401677 SQLConn-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      650 2024-05-06 09:40:55.000000 SQLConn-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:44:57.818656 SQLConn-0.0.5/
+-rw-rw-rw-   0        0        0     9260 2024-05-06 09:44:57.816657 SQLConn-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8818 2024-05-06 08:56:32.000000 SQLConn-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 09:44:57.793291 SQLConn-0.0.5/SQLConn/
+-rw-rw-rw-   0        0        0     5580 2024-05-06 09:44:20.000000 SQLConn-0.0.5/SQLConn/SQLConn.py
+-rw-rw-rw-   0        0        0      293 2024-05-06 09:40:40.000000 SQLConn-0.0.5/SQLConn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:44:57.814655 SQLConn-0.0.5/SQLConn.egg-info/
+-rw-rw-rw-   0        0        0     9260 2024-05-06 09:44:57.000000 SQLConn-0.0.5/SQLConn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2024-05-06 09:44:57.000000 SQLConn-0.0.5/SQLConn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:44:57.000000 SQLConn-0.0.5/SQLConn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-06 09:44:57.000000 SQLConn-0.0.5/SQLConn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 09:44:57.000000 SQLConn-0.0.5/SQLConn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 09:44:57.818656 SQLConn-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      650 2024-05-06 09:44:53.000000 SQLConn-0.0.5/setup.py
```

### Comparing `SQLConn-0.0.4/PKG-INFO` & `SQLConn-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLConn
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package facilitates easy SQL database integration.
 Home-page: https://github.com/janyoungjin/SQLConn
 Author: janyoungjin
 Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
 Description-Content-Type: text/markdown
 Requires-Dist: mysqlclient
 Requires-Dist: pandas
```

### Comparing `SQLConn-0.0.4/README.md` & `SQLConn-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `SQLConn-0.0.4/SQLConn/SQLConn.py` & `SQLConn-0.0.5/SQLConn/SQLConn.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,66 +66,66 @@
             raise ValueError("to_sql does only supports 'select' or 'show' commands.")
         try:
             self.to_DataFrame(cmd).to_sql(name,other.engine.connect(),index=False,if_exists="replace")
         except Exception as e:
             warnings.warn(str(e))
 class MYSQLConn(SQLConn):
     def __init__(self,password:str,host:str='127.0.0.1',user:str="root",database:str="mysql",port:str|int=3306) -> None:
-        super.__init__()
+        super().__init__()
         self.__host=host
         self.__user=user
         self.__password=password
         self.__database=database
         self.__port=int(port)
         self._conn=MySQLdb.connect(host=self.__host,user=self.__user,password=self.__password,database=self.__database,port=self.__port)
         self._engine=self._makeEngine()
     @property
     def URL(self):
         return f'mysql+mysqldb://{self.__user}:{self.__password}@{self.__host}:{self.__port}/{self.__database}'
 class MSSQLConn(SQLConn):
     def __init__(self,password:str,host:str='127.0.0.1',user:str="sa",database:str="master",port:str|int=1433) -> None:
-        super.__init__()
+        super().__init__()
         self.__host=host
         self.__user=user
         self.__password=password
         self.__database=database
         self.__port=int(port)
         self._conn=pymssql.connect(host=self.__host,user=self.__user,password=self.__password,database=self.__database,port=self.__port)
         self._engine=self._makeEngine()
     @property
     def URL(self):
         return f'mssql+pyodbc://{self.__user}:{self.__password}@{self.__host}:{self.__port}/{self.__database}'
 class OracleConn(SQLConn):
     def __init__(self,password:str,host:str='127.0.0.1',user:str="system",database:str="xe",port:str|int=1521) -> None:
-        super.__init__()
+        super().__init__()
         self.__host=host
         self.__user=user
         self.__password=password
         self.__database=database
         self.__port=int(port)
         self._conn=cx_Oracle.connect(self.__user,self.__password,f'{self.__host}:{self.__port}/{self.__database}')
         self._engine=self._makeEngine()
     @property
     def URL(self):
         return f'oracle+cx_oracle://{self.__user}:{self.__password}@{self.__host}:{self.__port}/?service_name={self.__database}'
 class PostgresqlConn(SQLConn):
     def __init__(self,password:str,host:str='127.0.0.1',user:str="postgres",database:str="postgres",port:str|int=5432) -> None:
-        super.__init__()
+        super().__init__()
         self.__host=host
         self.__user=user
         self.__password=password
         self.__database=database
         self.__port=int(port)
         self._conn=psycopg2.connect(host=self.__host,user=self.__user,password=self.__password,database=self.__database,port=self.__port)
         self._engine=self._makeEngine()
     @property
     def URL(self):
         return f'postgresql://{self.__user}:{self.__password}@{self.__host}:{self.__port}/{self.__database}'
 class SQLiteConn(SQLConn):
     def __init__(self,file_path:str) -> None:
-        super.__init__()
+        super().__init__()
         self.__file_path=file_path
         self._conn=sqlite3.connect(file_path)
         self._engine=self._makeEngine()
     @property
     def URL(self):
         return f'sqlite://{self.__file_path}'
```

### Comparing `SQLConn-0.0.4/SQLConn.egg-info/PKG-INFO` & `SQLConn-0.0.5/SQLConn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLConn
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package facilitates easy SQL database integration.
 Home-page: https://github.com/janyoungjin/SQLConn
 Author: janyoungjin
 Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
 Description-Content-Type: text/markdown
 Requires-Dist: mysqlclient
 Requires-Dist: pandas
```

### Comparing `SQLConn-0.0.4/setup.py` & `SQLConn-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='SQLConn',
-    version='0.0.4',
+    version='0.0.5',
     description='This package facilitates easy SQL database integration.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='janyoungjin',
     install_requires=['mysqlclient', 'pandas', 'cx_oracle', 'psycopg2', 'pymssql','sqlalchemy'],
     packages=find_packages(exclude=[]),
     url='https://github.com/janyoungjin/SQLConn',
```

