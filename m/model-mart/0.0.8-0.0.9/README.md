# Comparing `tmp/model-mart-0.0.8.tar.gz` & `tmp/model-mart-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model-mart-0.0.8.tar", last modified: Fri Mar 22 08:24:39 2024, max compression
+gzip compressed data, was "model-mart-0.0.9.tar", last modified: Mon May  6 08:50:04 2024, max compression
```

## Comparing `model-mart-0.0.8.tar` & `model-mart-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lizhengnan   (501) staff       (20)        0 2024-03-22 08:24:39.065610 model-mart-0.0.8/
--rw-r--r--   0 lizhengnan   (501) staff       (20)      460 2024-03-22 08:24:39.065478 model-mart-0.0.8/PKG-INFO
--rw-r--r--   0 lizhengnan   (501) staff       (20)       41 2023-09-27 08:51:53.000000 model-mart-0.0.8/README.md
-drwxr-xr-x   0 lizhengnan   (501) staff       (20)        0 2024-03-22 08:24:39.064314 model-mart-0.0.8/model_mart/
--rw-r--r--   0 lizhengnan   (501) staff       (20)       41 2023-09-28 09:46:18.000000 model-mart-0.0.8/model_mart/__init__.py
--rw-r--r--   0 lizhengnan   (501) staff       (20)    22839 2024-03-22 06:44:18.000000 model-mart-0.0.8/model_mart/model_mart_utils.py
-drwxr-xr-x   0 lizhengnan   (501) staff       (20)        0 2024-03-22 08:24:39.065302 model-mart-0.0.8/model_mart.egg-info/
--rw-r--r--   0 lizhengnan   (501) staff       (20)      460 2024-03-22 08:24:39.000000 model-mart-0.0.8/model_mart.egg-info/PKG-INFO
--rw-r--r--   0 lizhengnan   (501) staff       (20)      241 2024-03-22 08:24:39.000000 model-mart-0.0.8/model_mart.egg-info/SOURCES.txt
--rw-r--r--   0 lizhengnan   (501) staff       (20)        1 2024-03-22 08:24:39.000000 model-mart-0.0.8/model_mart.egg-info/dependency_links.txt
--rw-r--r--   0 lizhengnan   (501) staff       (20)       31 2024-03-22 08:24:39.000000 model-mart-0.0.8/model_mart.egg-info/requires.txt
--rw-r--r--   0 lizhengnan   (501) staff       (20)       11 2024-03-22 08:24:39.000000 model-mart-0.0.8/model_mart.egg-info/top_level.txt
--rw-r--r--   0 lizhengnan   (501) staff       (20)       38 2024-03-22 08:24:39.065660 model-mart-0.0.8/setup.cfg
--rw-r--r--   0 lizhengnan   (501) staff       (20)      791 2024-03-22 08:23:39.000000 model-mart-0.0.8/setup.py
+drwxr-xr-x   0 lizhengnan   (501) staff       (20)        0 2024-05-06 08:50:04.133928 model-mart-0.0.9/
+-rw-r--r--   0 lizhengnan   (501) staff       (20)      460 2024-05-06 08:50:04.133792 model-mart-0.0.9/PKG-INFO
+-rw-r--r--   0 lizhengnan   (501) staff       (20)       41 2023-09-27 08:51:53.000000 model-mart-0.0.9/README.md
+drwxr-xr-x   0 lizhengnan   (501) staff       (20)        0 2024-05-06 08:50:04.132882 model-mart-0.0.9/model_mart/
+-rw-r--r--   0 lizhengnan   (501) staff       (20)       41 2023-09-28 09:46:18.000000 model-mart-0.0.9/model_mart/__init__.py
+-rw-r--r--   0 lizhengnan   (501) staff       (20)    26576 2024-05-06 08:47:15.000000 model-mart-0.0.9/model_mart/model_mart_utils.py
+drwxr-xr-x   0 lizhengnan   (501) staff       (20)        0 2024-05-06 08:50:04.133639 model-mart-0.0.9/model_mart.egg-info/
+-rw-r--r--   0 lizhengnan   (501) staff       (20)      460 2024-05-06 08:50:04.000000 model-mart-0.0.9/model_mart.egg-info/PKG-INFO
+-rw-r--r--   0 lizhengnan   (501) staff       (20)      241 2024-05-06 08:50:04.000000 model-mart-0.0.9/model_mart.egg-info/SOURCES.txt
+-rw-r--r--   0 lizhengnan   (501) staff       (20)        1 2024-05-06 08:50:04.000000 model-mart-0.0.9/model_mart.egg-info/dependency_links.txt
+-rw-r--r--   0 lizhengnan   (501) staff       (20)       31 2024-05-06 08:50:04.000000 model-mart-0.0.9/model_mart.egg-info/requires.txt
+-rw-r--r--   0 lizhengnan   (501) staff       (20)       11 2024-05-06 08:50:04.000000 model-mart-0.0.9/model_mart.egg-info/top_level.txt
+-rw-r--r--   0 lizhengnan   (501) staff       (20)       38 2024-05-06 08:50:04.133966 model-mart-0.0.9/setup.cfg
+-rw-r--r--   0 lizhengnan   (501) staff       (20)      791 2024-05-06 08:48:01.000000 model-mart-0.0.9/setup.py
```

### Comparing `model-mart-0.0.8/model_mart/model_mart_utils.py` & `model-mart-0.0.9/model_mart/model_mart_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import time
 from queue import Empty, Queue
 from threading import Thread
 
 import requests
 from minio import Minio
 from minio.error import S3Error
+import logging
+from requests import RequestException
+from urllib3.exceptions import HTTPError
 
 _BAR_SIZE = 20
 _KILOBYTE = 1024
 _FINISHED_BAR = '#'
 _REMAINING_BAR = '-'
 
 _UNKNOWN_SIZE = '?'
@@ -27,21 +30,32 @@
 _PERCENTAGE_FORMAT = '%3d%%'
 _HUMANINZED_FORMAT = '%0.2f'
 
 _DISPLAY_FORMAT = '|%s| %s/%s %s [elapsed: %s left: %s, %s MB/sec]'
 
 _REFRESH_CHAR = '\r'
 
+# 配置日志输出格式
+logging.basicConfig(level=logging.INFO, format='%(asctime)s %(levelname)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S',
+                    stream=sys.stdout)
+
 
 class PandoraBox:
     def __init__(self, username, password, admin_host):
         self.is_login = False
-        try:
-            self.admin_host = admin_host
+        self.user = None
+        self.client = None
+        self.bucket = None
+        self.endpoint = None
+        self.region = None
+        self.expire = None
+        self.session = None
+        self.admin_host = admin_host
 
+        try:
             if not username or not password:
                 raise ValueError("登录失败，用户名或密码为空")
 
             info = json.dumps({
                 'username': username,
                 'password': password
             })
@@ -54,15 +68,14 @@
 
             if resp.status_code == http.HTTPStatus.OK:
                 if not resp.text:
                     return
                 code = resp.json().get("code")
                 if code != 0:
                     raise ValueError(f"登录失败，错误消息: {resp.json().get('msg')}")
-                print(resp.json())
                 self.key = resp.json()['sts_gateway_info']['access_key']
                 self.secret = resp.json()['sts_gateway_info']['access_secret']
                 self.bucket = resp.json()['sts_gateway_info']['bucket']
                 self.endpoint = resp.json()['sts_gateway_info']['endpoint']
                 self.region = resp.json()['sts_gateway_info']['region']
                 self.expire = resp.json()['sts_gateway_info']['expire']
                 self.session = resp.json()['sts_gateway_info']['session']
@@ -73,20 +86,31 @@
                     secret_key=self.secret,
                     session_token=self.session,
                     region=self.region,
                     secure=False,
                 )
                 self.user = username
                 self.is_login = True
-                print("登录成功")
+                logging.info("登录成功")
 
         except Exception as e:
-            print(f"登录过程中发生错误: {str(e)}")
+            logging.error(f"登录过程中发生错误: {str(e)}")
+
+    def _handle_error(self, error_message):
+        logging.error(error_message)
 
-    def model_init(self, model_name, description, library, data_set, task):
+    def _handle_request_exception(self, e):
+        if isinstance(e, RequestException):
+            logging.error(f"HTTP请求错误: {str(e)}")
+        elif isinstance(e, HTTPError):
+            logging.error(f"HTTP错误: {str(e)}")
+        else:
+            logging.error(f"发生未知错误: {str(e)}")
+
+    def model_init(self, model_name, description, library, data_set, task) -> bool:
         try:
             if not self.is_login:
                 raise ValueError("用户未登录")
             if not model_name:
                 raise ValueError("参数 model_name 为空")
 
             info = json.dumps({
@@ -96,49 +120,45 @@
                 'data_set': data_set,
                 'task': task,
                 'creator': self.user,
             })
 
             resp = self._new_model_req(info)
             resp.raise_for_status()  # 引发HTTP错误
-
-            print(resp.text)
+            if resp.status_code == http.HTTPStatus.OK:
+                logging.info("模型创建成功")
+                return True
 
         except ValueError as ve:
-            print(f"Error: {str(ve)}")
-
-        except requests.RequestException as re:
-            print(f"HTTP请求错误: {str(re)}")
+            self._handle_error(f"Error: {str(ve)}")
+            return False
 
         except Exception as e:
-            print(f"发生未知错误: {str(e)}")
+            self._handle_request_exception(e)
+            return False
 
     def my_models(self):
         try:
             if not self.is_login:
                 raise ValueError("用户未登录")
 
             resp = self._get_user_model_list_req()
             resp.raise_for_status()
 
             if resp.status_code == http.HTTPStatus.OK:
                 data = resp.json().get("data")
-                print(data)
                 return data
 
         except ValueError as ve:
-            print(f"Error: {str(ve)}")
-
-        except requests.RequestException as re:
-            print(f"HTTP请求错误: {str(re)}")
+            self._handle_error(f"Error: {str(ve)}")
 
         except Exception as e:
-            print(f"发生未知错误: {str(e)}")
+            self._handle_request_exception(e)
 
-    def get_model(self, model_name, tag, destination_path):
+    def get_model(self, model_name, tag, destination_path) -> bool:
         try:
             if not self.is_login:
                 raise ValueError("用户未登录")
             if not tag:
                 raise ValueError("参数 tag 为空")
             if not model_name:
                 raise ValueError("参数 model_name 为空")
@@ -163,48 +183,92 @@
                 full_path = '/'.join(parts[3:]) if len(parts) > 3 else ''
 
                 err = self._download(obj.object_name, os.path.join(destination_path, full_path))
 
                 if err:
                     raise ValueError(f"下载文件时发生错误: {err}")
 
-            print("文件下载成功。")
+            logging.info("文件下载成功")
+            return True
 
         except ValueError as ve:
-            print(f"错误: {str(ve)}")
+            self._handle_error(f"Error: {str(ve)}")
+            return False
 
-        except requests.RequestException as re:
-            print(f"HTTP请求错误: {str(re)}")
+        except Exception as e:
+            self._handle_request_exception(e)
+            return False
+
+    def get_model_file(self, model_name, tag, rel_path, destination_path) -> bool:
+        try:
+            if not self.is_login:
+                raise ValueError("用户未登录")
+            if not tag:
+                raise ValueError("参数 tag 为空")
+            if not model_name:
+                raise ValueError("参数 model_name 为空")
+            if os.path.isfile(destination_path):
+                raise ValueError("参数 destination_path 必须是一个文件夹")
+            if not os.path.exists(destination_path):
+                raise ValueError("目标路径不存在")
+
+            resp = self._get_tag_storage_path_req(model_name, tag)
+            resp.raise_for_status()
+
+            blob_path = resp.json().get("blob_path")
+
+            object_path = os.path.join(blob_path, rel_path)
+
+            # 检查对象是否存在
+            try:
+                stat_info = self.client.stat_object(self.bucket, object_name=object_path)
+            except S3Error as e:
+                if e.code == 'NoSuchKey':
+                    raise ValueError(f"文件 {object_path} 不存在")
+                else:
+                    raise ValueError(f"检查文件时发生错误: {e}")
+            file_name = os.path.basename(object_path)
+            err = self._download(object_path, os.path.join(destination_path, file_name))
+            if err:
+                raise ValueError(f"下载文件时发生错误: {err}")
+
+            logging.info('文件下载成功')
+            return True
+
+        except ValueError as ve:
+            self._handle_error(f"Error: {str(ve)}")
+            return False
 
         except Exception as e:
-            print(f"发生未知错误: {str(e)}")
+            self._handle_request_exception(e)
+            return False
 
     def version_list(self, model_name):
         try:
             if not self.is_login:
                 raise ValueError("用户未登录")
 
             resp = self._get_model_version_list_req(model_name)
             resp.raise_for_status()
 
             if resp.status_code == http.HTTPStatus.OK:
                 version_list = resp.json().get("version_list")
-                print(version_list)
+                logging.info(version_list)
                 return version_list
 
         except ValueError as ve:
-            print(f"错误: {str(ve)}")
+            logging.error(f"错误: {str(ve)}")
 
         except requests.RequestException as re:
-            print(f"HTTP请求错误: {str(re)}")
+            logging.error(f"HTTP请求错误: {str(re)}")
 
         except Exception as e:
-            print(f"发生未知错误: {str(e)}")
+            logging.error(f"发生未知错误: {str(e)}")
 
-    def register_model(self, model_name, tag, local_path):
+    def register_model(self, model_name, tag, local_path) -> bool:
         try:
             if not self.is_login:
                 raise ValueError("用户未登录")
             if not model_name:
                 raise ValueError("参数 model_name 为空")
             if not local_path:
                 raise ValueError("参数 local_path 为空")
@@ -221,39 +285,41 @@
             file_hash = []
 
             if os.path.isfile(local_path):
                 file_info = hash_files(local_path)
                 file_hash.append(file_info)
                 file_name = os.path.basename(local_path)
                 destination_path = f"/models/{model_name}/{guid}/{file_name}"
-                err = self._upload(local_path, destination_path)
+                err = self._upload_file(local_path, destination_path)
                 if err:
                     raise ValueError(f"上传文件时发生错误: {err}")
 
                 blob_path = f"models/{model_name}/{guid}/"
-                print("文件上传成功。")
+                logging.info("文件上传成功")
 
             elif os.path.isdir(local_path):
                 local_path = os.path.abspath(local_path)
                 allfiles = _allfiles(local_path)
                 file_hash = hash_files_in_directory(local_path)
                 for file in allfiles:
                     folder_name = os.path.basename(local_path)
                     file_path = file.split(folder_name + '/')[1]
                     destination_path = os.path.join('models', model_name, guid, file_path)
                     source_path = os.path.join(local_path, file)
-                    err = self._upload(source_path, destination_path)
+                    err = self._upload_file(source_path, destination_path)
                     if err:
-                        raise ValueError(f"上传文件时发生错误: {err}")
+                        logging.error(f"上传文件时发生错误: {err}")
+                        return False
 
                 blob_path = f"models/{model_name}/{guid}/"
-                print("文件上传成功。")
+                logging.info("文件上传成功")
 
             else:
-                raise ValueError("请输入正确的路径")
+                logging.error("请输入正确的路径")
+                return False
 
             info = json.dumps({
                 'model_name': model_name,
                 'tag': tag,
                 'blob_path': blob_path,
                 'guid': str(guid),
                 'files_list': file_hash,
@@ -261,24 +327,27 @@
 
             address = self._add_model_version_req(info)
             address.raise_for_status()
 
             if address.status_code == http.HTTPStatus.BAD_REQUEST:
                 raise ValueError(address.json().get("msg"))
 
-            print("模型注册成功。")
+            logging.info(f"模型{str(model_name)}版本{str(tag)}注册成功")
+            return True
 
         except ValueError as ve:
-            print(f"错误: {str(ve)}")
+            logging.error(f"错误: {str(ve)}")
 
         except requests.RequestException as re:
-            print(f"HTTP请求错误: {str(re)}")
+            logging.error(f"HTTP请求错误: {str(re)}")
 
         except Exception as e:
-            print(f"发生未知错误: {str(e)}")
+            logging.error(f"发生未知错误: {str(e)}")
+
+        return False
 
     def get_model_file_list(self, model_name, tag):
         try:
             if not self.is_login:
                 raise ValueError("用户未登录")
             if not tag:
                 raise ValueError("参数 tag 为空")
@@ -288,50 +357,68 @@
             resp = self._get_model_tag_files_req(model_name, tag)
             resp.raise_for_status()
 
             if resp.status_code == http.HTTPStatus.OK:
                 return resp.json().get("data")
 
         except ValueError as ve:
-            print(f"错误: {str(ve)}")
+            logging.error(f"错误: {str(ve)}")
 
         except requests.RequestException as re:
-            print(f"HTTP请求错误: {str(re)}")
+            logging.error(f"HTTP请求错误: {str(re)}")
 
         except Exception as e:
-            print(f"发生未知错误: {str(e)}")
-
-    def _upload(self, local_path, destination):
-        try:
-            self.client.fput_object(
-                self.bucket,
-                destination,
-                local_path,
-                progress=Progress(),  # 在回调中调用线程对象的run方法
-            )
-            print("文件上传成功。")
-            return None
-        except S3Error as err:
-            print(f"文件上传失败: {err}")
-            return err
+            logging.error(f"发生未知错误: {str(e)}")
 
-    def _download(self, source, destination):
-        try:
-            # Download data of an object.
-            self.client.fget_object(
-                self.bucket,
-                source,
-                destination,
-                progress=Progress(),  # 在回调中调用线程对象的run方法
-            )
-            print("文件下载成功。")
-            return None
-        except S3Error as err:
-            print(f"文件下载失败: {err}")
-            return err
+    def _upload_file(self, local_path, destination, retry_count=3, sleep_interval=5):
+        attempt = 1
+        while attempt <= retry_count:
+            try:
+                self.client.fput_object(
+                    self.bucket,
+                    destination,
+                    local_path,
+                    progress=Progress(),  # 在回调中调用线程对象的run方法
+                )
+                logging.info("文件上传成功")
+                return None
+            except S3Error as err:
+                logging.error(f"文件上传失败: {err}")
+
+                if attempt < retry_count:
+                    logging.info(f"重试上传文件: 尝试次数: {attempt}/{retry_count}")
+                    attempt += 1
+                    time.sleep(sleep_interval)
+                else:
+                    logging.error(f"上传文件失败: 已达到最大重试次数")
+                    return err
+
+    def _download(self, source, destination, retry_count=3, sleep_interval=5):
+        attempt = 1
+        while attempt <= retry_count:
+            try:
+                # Download data of an object.
+                self.client.fget_object(
+                    self.bucket,
+                    source,
+                    destination,
+                    progress=Progress(),  # 在回调中调用线程对象的run方法
+                )
+                logging.info("文件下载成功")
+                return None
+            except S3Error as err:
+                logging.error(f"文件下载失败: {err}")
+
+                if attempt < retry_count:
+                    logging.info(f"重试下载文件: 尝试次数: {attempt}/{retry_count}")
+                    attempt += 1
+                    time.sleep(sleep_interval)
+                else:
+                    logging.error(f"下载文件失败: 已达到最大重试次数")
+                    return err
 
     # def _delete_model_version_req(self, model_name, model_version):
     #     base_url = "http://{host}/api/v1/model/version/{model_name}/{model_version}" \
     #         .format(host=ADMIN_HOST, model_name=model_name, model_version=model_version)
     #     resp = requests.delete(url=base_url)
     #     return resp
     #
@@ -421,20 +508,19 @@
 def _allfiles(folder):
     try:
         filepath_list = []
         for root, _, file_names in os.walk(folder):
             for file_name in file_names:
                 file_path = os.path.join(root, file_name)
                 filepath_list.append(file_path)
-                print(file_path)
         # filepath_list = sorted(filepath_list, key=str.lower)
         return filepath_list
 
     except Exception as e:
-        print(f"获取文件列表时发生错误: {str(e)}")
+        logging.error(f"获取文件列表时发生错误: {str(e)}")
         return []
 
 
 class Progress(Thread):
     """
         Constructs a :class:`Progress` object.
         :param interval: Sets the time interval to be displayed on the screen.
@@ -584,18 +670,18 @@
 
             # 返回文件名、哈希值和相对路径
             return {'file_name': os.path.basename(file_path),
                     'file_hash': hash_value,
                     'rel_path': rel_path}
 
         else:
-            print(f"The provided path '{file_path}' is not a file.")
+            logging.error(f"The provided path '{file_path}' is not a file.")
 
     except Exception as e:
-        print(f"Error processing file '{file_path}': {str(e)}")
+        logging.error(f"Error processing file '{file_path}': {str(e)}")
 
     return None
 
 
 def hash_files_in_directory(directory):
     file_hashes = []
 
@@ -615,18 +701,18 @@
                         'file_name': file,
                         'file_hash': hash_value,
                         'rel_path': rel_path
                     }
                     file_hashes.append(file_info)
 
                 except Exception as e:
-                    print(f"Error processing file '{file_path}': {str(e)}")
+                    logging.error(f"Error processing file '{file_path}': {str(e)}")
 
     except Exception as e:
-        print(f"Error accessing directory '{directory}': {str(e)}")
+        logging.error(f"Error accessing directory '{directory}': {str(e)}")
 
     return file_hashes
 
 
 def calculate_file_hash(file_path, algorithm='sha256', chunk_size=8192):
     # 使用指定哈希算法打开文件
     hasher = hashlib.new(algorithm)
```

### Comparing `model-mart-0.0.8/setup.py` & `model-mart-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = None
 
 setuptools.setup(
     name="model-mart",  # Replace with your own name
-    version="0.0.8",
+    version="0.0.9",
     author="SoutherLea",
     author_email="lizhengnan@stonewise.cn",
     description="sdk help users to use model market",
     long_description="sdk help users to use model market",
     long_description_content_type="text/markdown",
     url="https://gitlab.stonewise.cn/mlsys/model-mart.git",
     install_requires=[
```

