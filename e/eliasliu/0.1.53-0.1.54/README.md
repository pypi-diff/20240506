# Comparing `tmp/eliasliu-0.1.53.tar.gz` & `tmp/eliasliu-0.1.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.53.tar", last modified: Mon May  6 15:31:52 2024, max compression
+gzip compressed data, was "eliasliu-0.1.54.tar", last modified: Mon May  6 15:44:28 2024, max compression
```

## Comparing `eliasliu-0.1.53.tar` & `eliasliu-0.1.54.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 15:31:52.992894 eliasliu-0.1.53/
--rw-rw-rw-   0        0        0     6990 2024-05-06 15:31:52.989923 eliasliu-0.1.53/PKG-INFO
--rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.53/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 15:31:52.913853 eliasliu-0.1.53/elias/
-drwxrwxrwx   0        0        0        0 2024-05-06 15:31:52.940037 eliasliu-0.1.53/elias/Scripts/
--rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/MysqlTool.py
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/__init__.py
--rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/douyin.py
--rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/jd.py
--rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/name_in_db.py
--rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/py_clickhouse.py
--rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/vm_clickhouse.py
--rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/youdao.py
--rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/__init__.py
--rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/check.py
--rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/config_env_variable.py
--rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datamove.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:31:52.964973 eliasliu-0.1.53/elias/datax/
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/__init__.py
--rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/auto_create_table.py
--rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/job.py
--rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/main.py
--rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/reader.py
--rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/run.py
--rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/writer.py
--rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/etl.py
--rw-rw-rw-   0        0        0     9840 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/picture.py
--rw-rw-rw-   0        0        0    77619 2024-05-06 15:23:46.000000 eliasliu-0.1.53/elias/usual.py
--rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/wechat.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:31:52.985926 eliasliu-0.1.53/eliasliu.egg-info/
--rw-rw-rw-   0        0        0     6990 2024-05-06 15:31:52.000000 eliasliu-0.1.53/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      688 2024-05-06 15:31:52.000000 eliasliu-0.1.53/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 15:31:52.000000 eliasliu-0.1.53/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2024-05-06 15:31:52.000000 eliasliu-0.1.53/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 15:31:52.000000 eliasliu-0.1.53/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 15:31:52.992894 eliasliu-0.1.53/setup.cfg
--rw-rw-rw-   0        0        0     1928 2024-05-06 15:27:34.000000 eliasliu-0.1.53/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:44:28.851775 eliasliu-0.1.54/
+-rw-rw-rw-   0        0        0     6990 2024-05-06 15:44:28.848782 eliasliu-0.1.54/PKG-INFO
+-rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.54/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 15:44:28.785058 eliasliu-0.1.54/elias/
+drwxrwxrwx   0        0        0        0 2024-05-06 15:44:28.807001 eliasliu-0.1.54/elias/Scripts/
+-rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/Scripts/MysqlTool.py
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/Scripts/__init__.py
+-rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/Scripts/douyin.py
+-rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/Scripts/jd.py
+-rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/Scripts/name_in_db.py
+-rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/Scripts/py_clickhouse.py
+-rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/Scripts/vm_clickhouse.py
+-rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/Scripts/youdao.py
+-rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/__init__.py
+-rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/check.py
+-rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/config_env_variable.py
+-rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/datamove.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:44:28.828835 eliasliu-0.1.54/elias/datax/
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/datax/__init__.py
+-rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/datax/auto_create_table.py
+-rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/datax/job.py
+-rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/datax/main.py
+-rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/datax/reader.py
+-rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/datax/run.py
+-rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/datax/writer.py
+-rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/etl.py
+-rw-rw-rw-   0        0        0     9840 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/picture.py
+-rw-rw-rw-   0        0        0    77696 2024-05-06 15:43:09.000000 eliasliu-0.1.54/elias/usual.py
+-rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.54/elias/wechat.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:44:28.846787 eliasliu-0.1.54/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0     6990 2024-05-06 15:44:28.000000 eliasliu-0.1.54/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2024-05-06 15:44:28.000000 eliasliu-0.1.54/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 15:44:28.000000 eliasliu-0.1.54/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2024-05-06 15:44:28.000000 eliasliu-0.1.54/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 15:44:28.000000 eliasliu-0.1.54/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 15:44:28.851775 eliasliu-0.1.54/setup.cfg
+-rw-rw-rw-   0        0        0     1928 2024-05-06 15:43:55.000000 eliasliu-0.1.54/setup.py
```

### Comparing `eliasliu-0.1.53/PKG-INFO` & `eliasliu-0.1.54/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.53
+Version: 0.1.54
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.53/README.md` & `eliasliu-0.1.54/README.md`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/Scripts/MysqlTool.py` & `eliasliu-0.1.54/elias/Scripts/MysqlTool.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/Scripts/douyin.py` & `eliasliu-0.1.54/elias/Scripts/douyin.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/Scripts/jd.py` & `eliasliu-0.1.54/elias/Scripts/jd.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/Scripts/name_in_db.py` & `eliasliu-0.1.54/elias/Scripts/name_in_db.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/Scripts/py_clickhouse.py` & `eliasliu-0.1.54/elias/Scripts/py_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/Scripts/vm_clickhouse.py` & `eliasliu-0.1.54/elias/Scripts/vm_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/Scripts/youdao.py` & `eliasliu-0.1.54/elias/Scripts/youdao.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/check.py` & `eliasliu-0.1.54/elias/check.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/config_env_variable.py` & `eliasliu-0.1.54/elias/config_env_variable.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/datamove.py` & `eliasliu-0.1.54/elias/datamove.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/datax/auto_create_table.py` & `eliasliu-0.1.54/elias/datax/auto_create_table.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/datax/job.py` & `eliasliu-0.1.54/elias/datax/job.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/datax/main.py` & `eliasliu-0.1.54/elias/datax/main.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/datax/reader.py` & `eliasliu-0.1.54/elias/datax/reader.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/datax/run.py` & `eliasliu-0.1.54/elias/datax/run.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/datax/writer.py` & `eliasliu-0.1.54/elias/datax/writer.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/etl.py` & `eliasliu-0.1.54/elias/etl.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/picture.py` & `eliasliu-0.1.54/elias/picture.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/elias/usual.py` & `eliasliu-0.1.54/elias/usual.py`

 * *Files 0% similar despite different names*

```diff
@@ -571,15 +571,16 @@
     import os  
     import datetime
     import time
     import pandas as pd
     from elias import wechat as w
     start = time.time()
   
-    user = os.getlogin()
+    output_user = os.getlogin()
+    output_ip = get_out_ip()
     now = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     
     if server_type == 'mysql':
         print(' \n------- mysql --------\n')
         df = mysql_select(sql, hosts)
         h = hosts['host']
         p = hosts['port']
@@ -604,18 +605,18 @@
         d = hosts['db']
     time.sleep(2)
     df.to_excel(fname+'.xlsx',index=False)
     end = time.time()
     usetime = round(end-start,2)
     rows=len(df)
     w.wechat_file(file_path = fname+'.xlsx',key=key)
-
-    content=[[user,now,server_type,fname,rows,usetime,sql,h,p,n,c,d]]
+    
+    content=[[output_user,output_ip,now,server_type,fname,rows,usetime,sql,h,p,n,c,d]]
     df_record = pd.DataFrame(content)
-    df_record.columns=['user','output_time','server_type','file_name','rows','usetime','sql','host','port','user','code','db']
+    df_record.columns=['output_user','output_ip','output_time','server_type','file_name','rows','usetime','sql','host','port','user','code','db']
     try:
         mysql_write(df_record,'pysql_output_record',update = True,hosts = host_record,wtype='a',index = False)
     except:
         print('pysql_output_record 记录表不存在，已重新创建')
         mysql_write(df_record,'pysql_output_record',update = True,hosts = host_record,wtype='r',index = False)
```

### Comparing `eliasliu-0.1.53/elias/wechat.py` & `eliasliu-0.1.54/elias/wechat.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.54/eliasliu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.53
+Version: 0.1.54
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.53/eliasliu.egg-info/SOURCES.txt` & `eliasliu-0.1.54/eliasliu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.53/setup.py` & `eliasliu-0.1.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.53',  # 版本号
+    version='0.1.54',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     long_description = long_description,
     # long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
     url='https://github.com/tenbj/elias',  # 项目的URL
```

