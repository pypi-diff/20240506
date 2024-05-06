# Comparing `tmp/ilds-2024.3.1.tar.gz` & `tmp/ilds-2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ilds-2024.3.1.tar", last modified: Fri Mar  1 04:04:23 2024, max compression
+gzip compressed data, was "dist\ilds-2024.5.6.tar", last modified: Mon May  6 03:26:57 2024, max compression
```

## Comparing `ilds-2024.3.1.tar` & `ilds-2024.5.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-03-01 04:04:23.000000 ilds-2024.3.1/
-drwxrwxrwx   0        0        0        0 2024-03-01 04:04:23.000000 ilds-2024.3.1/ilds/
--rw-rw-rw-   0        0        0     1797 2021-09-26 05:21:21.000000 ilds-2024.3.1/ilds/cmd.py
-drwxrwxrwx   0        0        0        0 2024-03-01 04:04:23.000000 ilds-2024.3.1/ilds/django/
--rw-rw-rw-   0        0        0     3407 2019-10-30 05:10:14.000000 ilds-2024.3.1/ilds/django/admin.py
--rw-rw-rw-   0        0        0    14906 2019-10-30 03:18:15.000000 ilds-2024.3.1/ilds/django/import_export.py
--rw-rw-rw-   0        0        0    15417 2019-11-27 09:35:07.000000 ilds-2024.3.1/ilds/django/model.py
--rw-rw-rw-   0        0        0     1840 2019-04-12 05:15:43.000000 ilds-2024.3.1/ilds/django/user.py
--rw-rw-rw-   0        0        0     2085 2021-09-28 08:04:39.000000 ilds-2024.3.1/ilds/django/util.py
--rw-rw-rw-   0        0        0        0 2018-08-07 03:24:52.000000 ilds-2024.3.1/ilds/django/__init__.py
--rw-rw-rw-   0        0        0     9150 2021-12-06 10:18:15.000000 ilds-2024.3.1/ilds/everything.py
--rw-rw-rw-   0        0        0     9470 2019-03-29 08:26:49.000000 ilds-2024.3.1/ilds/excel_xlrd.py
--rw-rw-rw-   0        0        0     9462 2023-05-16 08:14:48.000000 ilds-2024.3.1/ilds/excel_xlsx.py
--rw-rw-rw-   0        0        0    27737 2024-01-16 03:04:03.000000 ilds-2024.3.1/ilds/file.py
-drwxrwxrwx   0        0        0        0 2024-03-01 04:04:23.000000 ilds-2024.3.1/ilds/lib/
--rw-rw-rw-   0        0        0    13740 2018-11-26 09:16:44.000000 ilds-2024.3.1/ilds/lib/browsercookie.py
-drwxrwxrwx   0        0        0        0 2024-03-01 04:04:23.000000 ilds-2024.3.1/ilds/lib/configobj/
--rw-rw-rw-   0        0        0    46989 2019-05-06 20:45:36.000000 ilds-2024.3.1/ilds/lib/configobj/validate.py
--rw-rw-rw-   0        0        0       44 2019-05-06 20:45:36.000000 ilds-2024.3.1/ilds/lib/configobj/_version.py
--rw-rw-rw-   0        0        0    88030 2019-05-06 20:45:36.000000 ilds-2024.3.1/ilds/lib/configobj/__init__.py
--rw-rw-rw-   0        0        0    13829 2018-10-24 05:15:43.000000 ilds-2024.3.1/ilds/lib/hexdump.py
--rw-rw-rw-   0        0        0        0 2018-10-24 05:29:38.000000 ilds-2024.3.1/ilds/lib/__init__.py
--rw-rw-rw-   0        0        0    18061 2024-03-01 04:03:02.000000 ilds-2024.3.1/ilds/match_data.py
--rw-rw-rw-   0        0        0     7121 2019-11-18 03:49:54.000000 ilds-2024.3.1/ilds/md.py
--rw-rw-rw-   0        0        0     4832 2022-09-07 09:59:12.000000 ilds-2024.3.1/ilds/md5summer.py
--rw-rw-rw-   0        0        0     3513 2019-10-11 11:13:36.000000 ilds-2024.3.1/ilds/mycsv.py
--rw-rw-rw-   0        0        0     5123 2022-12-12 02:45:33.000000 ilds-2024.3.1/ilds/net.py
--rw-rw-rw-   0        0        0     9177 2023-12-01 06:55:05.000000 ilds-2024.3.1/ilds/pd.py
--rw-rw-rw-   0        0        0     8238 2024-01-18 09:17:32.000000 ilds-2024.3.1/ilds/spider.py
--rw-rw-rw-   0        0        0    13238 2021-03-05 07:49:55.000000 ilds-2024.3.1/ilds/time.py
--rw-rw-rw-   0        0        0     7637 2022-10-08 10:21:44.000000 ilds-2024.3.1/ilds/util.py
--rw-rw-rw-   0        0        0      422 2024-03-01 04:03:02.000000 ilds-2024.3.1/ilds/versions.py
--rw-rw-rw-   0        0        0        0 2018-07-04 06:42:08.000000 ilds-2024.3.1/ilds/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-01 04:04:23.000000 ilds-2024.3.1/ilds.egg-info/
--rw-rw-rw-   0        0        0        1 2024-03-01 04:04:22.000000 ilds-2024.3.1/ilds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1316 2024-03-01 04:04:22.000000 ilds-2024.3.1/ilds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       82 2024-03-01 04:04:22.000000 ilds-2024.3.1/ilds.egg-info/requires.txt
--rw-rw-rw-   0        0        0      695 2024-03-01 04:04:22.000000 ilds-2024.3.1/ilds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        5 2024-03-01 04:04:22.000000 ilds-2024.3.1/ilds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1316 2024-03-01 04:04:23.000000 ilds-2024.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      456 2019-10-24 10:28:45.000000 ilds-2024.3.1/README.rst
--rw-rw-rw-   0        0        0       42 2024-03-01 04:04:23.000000 ilds-2024.3.1/setup.cfg
--rw-rw-rw-   0        0        0     6481 2024-01-16 03:08:05.000000 ilds-2024.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:26:57.000000 ilds-2024.5.6/
+drwxrwxrwx   0        0        0        0 2024-05-06 03:26:57.000000 ilds-2024.5.6/ilds/
+-rw-rw-rw-   0        0        0     1797 2021-09-26 05:21:21.000000 ilds-2024.5.6/ilds/cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:26:57.000000 ilds-2024.5.6/ilds/django/
+-rw-rw-rw-   0        0        0     3407 2019-10-30 05:10:14.000000 ilds-2024.5.6/ilds/django/admin.py
+-rw-rw-rw-   0        0        0    14906 2019-10-30 03:18:15.000000 ilds-2024.5.6/ilds/django/import_export.py
+-rw-rw-rw-   0        0        0    15417 2019-11-27 09:35:07.000000 ilds-2024.5.6/ilds/django/model.py
+-rw-rw-rw-   0        0        0     1840 2019-04-12 05:15:43.000000 ilds-2024.5.6/ilds/django/user.py
+-rw-rw-rw-   0        0        0     2085 2021-09-28 08:04:39.000000 ilds-2024.5.6/ilds/django/util.py
+-rw-rw-rw-   0        0        0        0 2018-08-07 03:24:52.000000 ilds-2024.5.6/ilds/django/__init__.py
+-rw-rw-rw-   0        0        0     9150 2021-12-06 10:18:15.000000 ilds-2024.5.6/ilds/everything.py
+-rw-rw-rw-   0        0        0     9470 2019-03-29 08:26:49.000000 ilds-2024.5.6/ilds/excel_xlrd.py
+-rw-rw-rw-   0        0        0     9462 2023-05-16 08:14:48.000000 ilds-2024.5.6/ilds/excel_xlsx.py
+-rw-rw-rw-   0        0        0    27737 2024-01-16 03:04:03.000000 ilds-2024.5.6/ilds/file.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:26:57.000000 ilds-2024.5.6/ilds/lib/
+-rw-rw-rw-   0        0        0    13740 2018-11-26 09:16:44.000000 ilds-2024.5.6/ilds/lib/browsercookie.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:26:57.000000 ilds-2024.5.6/ilds/lib/configobj/
+-rw-rw-rw-   0        0        0    46989 2019-05-06 20:45:36.000000 ilds-2024.5.6/ilds/lib/configobj/validate.py
+-rw-rw-rw-   0        0        0       44 2019-05-06 20:45:36.000000 ilds-2024.5.6/ilds/lib/configobj/_version.py
+-rw-rw-rw-   0        0        0    88030 2019-05-06 20:45:36.000000 ilds-2024.5.6/ilds/lib/configobj/__init__.py
+-rw-rw-rw-   0        0        0    13829 2018-10-24 05:15:43.000000 ilds-2024.5.6/ilds/lib/hexdump.py
+-rw-rw-rw-   0        0        0        0 2018-10-24 05:29:38.000000 ilds-2024.5.6/ilds/lib/__init__.py
+-rw-rw-rw-   0        0        0    18063 2024-03-01 06:06:21.000000 ilds-2024.5.6/ilds/match_data.py
+-rw-rw-rw-   0        0        0     7121 2019-11-18 03:49:54.000000 ilds-2024.5.6/ilds/md.py
+-rw-rw-rw-   0        0        0     4832 2022-09-07 09:59:12.000000 ilds-2024.5.6/ilds/md5summer.py
+-rw-rw-rw-   0        0        0     3513 2019-10-11 11:13:36.000000 ilds-2024.5.6/ilds/mycsv.py
+-rw-rw-rw-   0        0        0     5123 2022-12-12 02:45:33.000000 ilds-2024.5.6/ilds/net.py
+-rw-rw-rw-   0        0        0     9246 2024-05-06 03:25:14.000000 ilds-2024.5.6/ilds/pd.py
+-rw-rw-rw-   0        0        0     8238 2024-01-18 09:17:32.000000 ilds-2024.5.6/ilds/spider.py
+-rw-rw-rw-   0        0        0    13238 2021-03-05 07:49:55.000000 ilds-2024.5.6/ilds/time.py
+-rw-rw-rw-   0        0        0     7637 2022-10-08 10:21:44.000000 ilds-2024.5.6/ilds/util.py
+-rw-rw-rw-   0        0        0      422 2024-05-06 03:25:39.000000 ilds-2024.5.6/ilds/versions.py
+-rw-rw-rw-   0        0        0        0 2018-07-04 06:42:08.000000 ilds-2024.5.6/ilds/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:26:57.000000 ilds-2024.5.6/ilds.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-06 03:26:56.000000 ilds-2024.5.6/ilds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1316 2024-05-06 03:26:56.000000 ilds-2024.5.6/ilds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2024-05-06 03:26:56.000000 ilds-2024.5.6/ilds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      695 2024-05-06 03:26:56.000000 ilds-2024.5.6/ilds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        5 2024-05-06 03:26:56.000000 ilds-2024.5.6/ilds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1316 2024-05-06 03:26:57.000000 ilds-2024.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2019-10-24 10:28:45.000000 ilds-2024.5.6/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-06 03:26:57.000000 ilds-2024.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     6481 2024-01-16 03:08:05.000000 ilds-2024.5.6/setup.py
```

### Comparing `ilds-2024.3.1/ilds/cmd.py` & `ilds-2024.5.6/ilds/cmd.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/django/admin.py` & `ilds-2024.5.6/ilds/django/admin.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/django/import_export.py` & `ilds-2024.5.6/ilds/django/import_export.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/django/model.py` & `ilds-2024.5.6/ilds/django/model.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/django/user.py` & `ilds-2024.5.6/ilds/django/user.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/django/util.py` & `ilds-2024.5.6/ilds/django/util.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/everything.py` & `ilds-2024.5.6/ilds/everything.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/excel_xlrd.py` & `ilds-2024.5.6/ilds/excel_xlrd.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/excel_xlsx.py` & `ilds-2024.5.6/ilds/excel_xlsx.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/file.py` & `ilds-2024.5.6/ilds/file.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/lib/browsercookie.py` & `ilds-2024.5.6/ilds/lib/browsercookie.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/lib/configobj/validate.py` & `ilds-2024.5.6/ilds/lib/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/lib/configobj/__init__.py` & `ilds-2024.5.6/ilds/lib/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/lib/hexdump.py` & `ilds-2024.5.6/ilds/lib/hexdump.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/match_data.py` & `ilds-2024.5.6/ilds/match_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
                 # print(df_neirong[replace_columns_index[columns_i]])
                 # 把找到的歌曲放在字典里面
                 neirong = df_neirong[replace_columns_index[columns_i]]
                 replace_column = replace_columns[columns_i]
                 # if neirong:
                 if replace_column in replace_dict and neirong != replace_dict[replace_column]:
                     info = f'重复（{replace_column}）: {neirong}'
-                    print(info)
+                    # print(info)
                     infos.append(info)
                 else:
                     replace_dict[replace_column] = neirong
                     # print(f'匹配：{ch} ------------- 找到 {replace_column}: {neirong}')
         # 处理找到的结果
         # print(df_line)
         # if replace_dict:
```

### Comparing `ilds-2024.3.1/ilds/md.py` & `ilds-2024.5.6/ilds/md.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/md5summer.py` & `ilds-2024.5.6/ilds/md5summer.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/mycsv.py` & `ilds-2024.5.6/ilds/mycsv.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/net.py` & `ilds-2024.5.6/ilds/net.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/pd.py` & `ilds-2024.5.6/ilds/pd.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,16 @@
     :param dst_dir: 拆分文件的保存目录
     :return:
     """
     file = Path(file)
 
     if dst_dir is None:
         dst_dir = file.parent / f'{file.stem} - 拆分'
+    elif isinstance(dst_dir, str):
+        dst_dir = Path(dst_dir)
 
     if not dst_dir.exists():
         dst_dir.mkdir()
 
     xlsx = pd.ExcelFile(file)
     sheet_names = xlsx.sheet_names
     print('sheet_names', sheet_names)
```

### Comparing `ilds-2024.3.1/ilds/spider.py` & `ilds-2024.5.6/ilds/spider.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/time.py` & `ilds-2024.5.6/ilds/time.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds/util.py` & `ilds-2024.5.6/ilds/util.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/ilds.egg-info/PKG-INFO` & `ilds-2024.5.6/ilds.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ilds
-Version: 2024.3.1
+Version: 2024.5.6
 Summary: 常用模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/ilds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/ilds
 Description: ====================
```

### Comparing `ilds-2024.3.1/ilds.egg-info/SOURCES.txt` & `ilds-2024.5.6/ilds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ilds-2024.3.1/PKG-INFO` & `ilds-2024.5.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ilds
-Version: 2024.3.1
+Version: 2024.5.6
 Summary: 常用模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/ilds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/ilds
 Description: ====================
```

### Comparing `ilds-2024.3.1/setup.py` & `ilds-2024.5.6/setup.py`

 * *Files identical despite different names*

