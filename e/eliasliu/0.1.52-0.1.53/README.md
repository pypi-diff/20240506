# Comparing `tmp/eliasliu-0.1.52.tar.gz` & `tmp/eliasliu-0.1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.52.tar", last modified: Wed Apr 17 23:25:08 2024, max compression
+gzip compressed data, was "eliasliu-0.1.53.tar", last modified: Mon May  6 15:31:52 2024, max compression
```

## Comparing `eliasliu-0.1.52.tar` & `eliasliu-0.1.53.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 23:25:08.330547 eliasliu-0.1.52/
--rw-rw-rw-   0        0        0     7039 2024-04-17 23:25:08.328566 eliasliu-0.1.52/PKG-INFO
--rw-rw-rw-   0        0        0     5851 2023-08-17 12:07:05.000000 eliasliu-0.1.52/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 23:25:08.275508 eliasliu-0.1.52/elias/
-drwxrwxrwx   0        0        0        0 2024-04-17 23:25:08.293520 eliasliu-0.1.52/elias/Scripts/
--rw-rw-rw-   0        0        0     2788 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/MysqlTool.py
--rw-rw-rw-   0        0        0      131 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/__init__.py
--rw-rw-rw-   0        0        0     6723 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/douyin.py
--rw-rw-rw-   0        0        0     5118 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/jd.py
--rw-rw-rw-   0        0        0     2407 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/name_in_db.py
--rw-rw-rw-   0        0        0    15915 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/py_clickhouse.py
--rw-rw-rw-   0        0        0    15332 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/vm_clickhouse.py
--rw-rw-rw-   0        0        0     3396 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/Scripts/youdao.py
--rw-rw-rw-   0        0        0      368 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/__init__.py
--rw-rw-rw-   0        0        0    30771 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/check.py
--rw-rw-rw-   0        0        0     1376 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/config_env_variable.py
--rw-rw-rw-   0        0        0     9670 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datamove.py
-drwxrwxrwx   0        0        0        0 2024-04-17 23:25:08.310532 eliasliu-0.1.52/elias/datax/
--rw-rw-rw-   0        0        0      131 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/__init__.py
--rw-rw-rw-   0        0        0    15834 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/auto_create_table.py
--rw-rw-rw-   0        0        0     3493 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/job.py
--rw-rw-rw-   0        0        0     4138 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/main.py
--rw-rw-rw-   0        0        0     5480 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/reader.py
--rw-rw-rw-   0        0        0     1756 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/run.py
--rw-rw-rw-   0        0        0     3588 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/datax/writer.py
--rw-rw-rw-   0        0        0    92990 2024-04-17 23:23:15.000000 eliasliu-0.1.52/elias/etl.py
--rw-rw-rw-   0        0        0     9840 2024-01-25 16:31:22.000000 eliasliu-0.1.52/elias/picture.py
--rw-rw-rw-   0        0        0    76919 2024-01-25 16:06:05.000000 eliasliu-0.1.52/elias/usual.py
--rw-rw-rw-   0        0        0    13040 2023-12-06 03:39:07.000000 eliasliu-0.1.52/elias/wechat.py
-drwxrwxrwx   0        0        0        0 2024-04-17 23:25:08.326572 eliasliu-0.1.52/eliasliu.egg-info/
--rw-rw-rw-   0        0        0     7039 2024-04-17 23:25:08.000000 eliasliu-0.1.52/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      688 2024-04-17 23:25:08.000000 eliasliu-0.1.52/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 23:25:08.000000 eliasliu-0.1.52/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2024-04-17 23:25:08.000000 eliasliu-0.1.52/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-17 23:25:08.000000 eliasliu-0.1.52/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 23:25:08.330547 eliasliu-0.1.52/setup.cfg
--rw-rw-rw-   0        0        0     1924 2024-04-17 23:24:35.000000 eliasliu-0.1.52/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:31:52.992894 eliasliu-0.1.53/
+-rw-rw-rw-   0        0        0     6990 2024-05-06 15:31:52.989923 eliasliu-0.1.53/PKG-INFO
+-rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.53/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 15:31:52.913853 eliasliu-0.1.53/elias/
+drwxrwxrwx   0        0        0        0 2024-05-06 15:31:52.940037 eliasliu-0.1.53/elias/Scripts/
+-rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/MysqlTool.py
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/__init__.py
+-rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/douyin.py
+-rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/jd.py
+-rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/name_in_db.py
+-rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/py_clickhouse.py
+-rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/vm_clickhouse.py
+-rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/Scripts/youdao.py
+-rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/__init__.py
+-rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/check.py
+-rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/config_env_variable.py
+-rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datamove.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:31:52.964973 eliasliu-0.1.53/elias/datax/
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/__init__.py
+-rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/auto_create_table.py
+-rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/job.py
+-rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/main.py
+-rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/reader.py
+-rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/run.py
+-rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/datax/writer.py
+-rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/etl.py
+-rw-rw-rw-   0        0        0     9840 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/picture.py
+-rw-rw-rw-   0        0        0    77619 2024-05-06 15:23:46.000000 eliasliu-0.1.53/elias/usual.py
+-rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.53/elias/wechat.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:31:52.985926 eliasliu-0.1.53/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0     6990 2024-05-06 15:31:52.000000 eliasliu-0.1.53/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2024-05-06 15:31:52.000000 eliasliu-0.1.53/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 15:31:52.000000 eliasliu-0.1.53/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2024-05-06 15:31:52.000000 eliasliu-0.1.53/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 15:31:52.000000 eliasliu-0.1.53/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 15:31:52.992894 eliasliu-0.1.53/setup.cfg
+-rw-rw-rw-   0        0        0     1928 2024-05-06 15:27:34.000000 eliasliu-0.1.53/setup.py
```

### Comparing `eliasliu-0.1.52/PKG-INFO` & `eliasliu-0.1.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.52
+Version: 0.1.53
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,19 +21,17 @@
 Requires-Dist: sqlalchemy
 Requires-Dist: mysql-connector
 Requires-Dist: requests
 Requires-Dist: mysql-connector-python
 Requires-Dist: impyla
 Requires-Dist: clickhouse_sqlalchemy
 Requires-Dist: clickhouse_driver
-Requires-Dist: odps
 Requires-Dist: bs4
 Requires-Dist: selenium
 Requires-Dist: loguru
-Requires-Dist: googletrans
 Requires-Dist: pillow
 Requires-Dist: opencv-python
 
 0 安装
 找到终端，再终端内输入以下代码
 安装
 pip install elias
```

### Comparing `eliasliu-0.1.52/README.md` & `eliasliu-0.1.53/README.md`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/Scripts/MysqlTool.py` & `eliasliu-0.1.53/elias/Scripts/MysqlTool.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/Scripts/douyin.py` & `eliasliu-0.1.53/elias/Scripts/douyin.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/Scripts/jd.py` & `eliasliu-0.1.53/elias/Scripts/jd.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/Scripts/name_in_db.py` & `eliasliu-0.1.53/elias/Scripts/name_in_db.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/Scripts/py_clickhouse.py` & `eliasliu-0.1.53/elias/Scripts/py_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/Scripts/vm_clickhouse.py` & `eliasliu-0.1.53/elias/Scripts/vm_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/Scripts/youdao.py` & `eliasliu-0.1.53/elias/Scripts/youdao.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/check.py` & `eliasliu-0.1.53/elias/check.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/config_env_variable.py` & `eliasliu-0.1.53/elias/config_env_variable.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/datamove.py` & `eliasliu-0.1.53/elias/datamove.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/datax/auto_create_table.py` & `eliasliu-0.1.53/elias/datax/auto_create_table.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/datax/job.py` & `eliasliu-0.1.53/elias/datax/job.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/datax/main.py` & `eliasliu-0.1.53/elias/datax/main.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/datax/reader.py` & `eliasliu-0.1.53/elias/datax/reader.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/datax/run.py` & `eliasliu-0.1.53/elias/datax/run.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/datax/writer.py` & `eliasliu-0.1.53/elias/datax/writer.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/etl.py` & `eliasliu-0.1.53/elias/etl.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/picture.py` & `eliasliu-0.1.53/elias/picture.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/elias/usual.py` & `eliasliu-0.1.53/elias/usual.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,15 +612,15 @@
     content=[[user,now,server_type,fname,rows,usetime,sql,h,p,n,c,d]]
     df_record = pd.DataFrame(content)
     df_record.columns=['user','output_time','server_type','file_name','rows','usetime','sql','host','port','user','code','db']
     try:
         mysql_write(df_record,'pysql_output_record',update = True,hosts = host_record,wtype='a',index = False)
     except:
         print('pysql_output_record 记录表不存在，已重新创建')
-        mysql_write(df_record,'pysql_output_record',update = True,hosts = host_record,wtype='w',index = False)
+        mysql_write(df_record,'pysql_output_record',update = True,hosts = host_record,wtype='r',index = False)
 
 
 # ================================================================================
 
 # Part 3 connect database
 # ================================================================================
 
@@ -2218,7 +2218,27 @@
     
     with open(file_path, "w") as json_file:
         json.dump(data, json_file, indent=4)  # 设置indent参数为4，表示使用4个空格缩进
 
     print("JSON数据已写入文件：", file_path)
    
     return file_path
+
+
+def convert_html_to_markdown(html_content):
+    
+    import html2text
+    import re
+    # 在转换前预处理HTML，例如插入额外的空行
+    html_content = re.sub(r'</p>', r'</p>\n\n', html_content)  # 在每个段落后增加额外的空行
+
+    h = html2text.HTML2Text()
+    h.body_width = 0  # 设置为0以防止自动换行
+    h.ignore_emphasis = False
+    h.ignore_links = False
+
+    markdown_content = h.handle(html_content)
+
+    # 在转换后处理Markdown，例如确保加粗不会在中间断开
+    markdown_content = re.sub(r'\*\*(.*?)\*\*', lambda match: '**' + match.group(1).replace('\n', ' ') + '**', markdown_content)
+    
+    return markdown_content
```

### Comparing `eliasliu-0.1.52/elias/wechat.py` & `eliasliu-0.1.53/elias/wechat.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.53/eliasliu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.52
+Version: 0.1.53
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,19 +21,17 @@
 Requires-Dist: sqlalchemy
 Requires-Dist: mysql-connector
 Requires-Dist: requests
 Requires-Dist: mysql-connector-python
 Requires-Dist: impyla
 Requires-Dist: clickhouse_sqlalchemy
 Requires-Dist: clickhouse_driver
-Requires-Dist: odps
 Requires-Dist: bs4
 Requires-Dist: selenium
 Requires-Dist: loguru
-Requires-Dist: googletrans
 Requires-Dist: pillow
 Requires-Dist: opencv-python
 
 0 安装
 找到终端，再终端内输入以下代码
 安装
 pip install elias
```

### Comparing `eliasliu-0.1.52/eliasliu.egg-info/SOURCES.txt` & `eliasliu-0.1.53/eliasliu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.52/setup.py` & `eliasliu-0.1.53/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.52',  # 版本号
+    version='0.1.53',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     long_description = long_description,
     # long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
     url='https://github.com/tenbj/elias',  # 项目的URL
@@ -29,19 +29,19 @@
         'sqlalchemy',
         'mysql-connector',
         'requests',
         'mysql-connector-python',
         'impyla',
         'clickhouse_sqlalchemy',
         'clickhouse_driver',
-        'odps',
+        # 'odps',
         'bs4',
         'selenium',
         'loguru',
-        'googletrans',
+        # 'googletrans',
         'pillow',
         'opencv-python'
     ],
     classifiers=[  # 包的分类标签
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

