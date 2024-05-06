# Comparing `tmp/AutoCython-jianjun-1.3.3.tar.gz` & `tmp/autocython_jianjun-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCython-jianjun-1.3.3.tar", last modified: Mon May  8 12:01:39 2023, max compression
+gzip compressed data, was "autocython_jianjun-1.3.4.tar", last modified: Mon May  6 04:48:19 2024, max compression
```

## Comparing `AutoCython-jianjun-1.3.3.tar` & `autocython_jianjun-1.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 12:01:39.496991 AutoCython-jianjun-1.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-08 12:01:39.492004 AutoCython-jianjun-1.3.3/AutoCython/
--rw-rw-rw-   0        0        0    24051 2023-05-08 12:00:42.000000 AutoCython-jianjun-1.3.3/AutoCython/AutoCython.py
--rw-rw-rw-   0        0        0      456 2023-05-08 12:00:59.000000 AutoCython-jianjun-1.3.3/AutoCython/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 12:01:39.495994 AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/
--rw-rw-rw-   0        0        0     4437 2023-05-08 12:01:39.000000 AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-08 12:01:39.000000 AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 12:01:39.000000 AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-08 12:01:39.000000 AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 12:01:39.000000 AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18431 2021-04-19 08:51:39.000000 AutoCython-jianjun-1.3.3/LICENSE
--rw-rw-rw-   0        0        0     4437 2023-05-08 12:01:39.496991 AutoCython-jianjun-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     4126 2023-03-24 08:02:16.000000 AutoCython-jianjun-1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 12:01:39.496991 AutoCython-jianjun-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      706 2023-05-08 12:01:04.000000 AutoCython-jianjun-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:48:19.003976 autocython_jianjun-1.3.4/
+drwxrwxrwx   0        0        0        0 2024-05-06 04:48:18.977989 autocython_jianjun-1.3.4/AutoCython/
+-rw-rw-rw-   0        0        0    24067 2024-05-06 04:47:41.000000 autocython_jianjun-1.3.4/AutoCython/AutoCython.py
+-rw-rw-rw-   0        0        0      456 2024-05-06 02:05:41.000000 autocython_jianjun-1.3.4/AutoCython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:48:18.982975 autocython_jianjun-1.3.4/AutoCython_jianjun.egg-info/
+-rw-rw-rw-   0        0        0     6123 2024-05-06 04:48:18.000000 autocython_jianjun-1.3.4/AutoCython_jianjun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-06 04:48:18.000000 autocython_jianjun-1.3.4/AutoCython_jianjun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 04:48:18.000000 autocython_jianjun-1.3.4/AutoCython_jianjun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-06 04:48:18.000000 autocython_jianjun-1.3.4/AutoCython_jianjun.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-06 04:48:18.000000 autocython_jianjun-1.3.4/AutoCython_jianjun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2024-05-06 03:14:53.000000 autocython_jianjun-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0     6123 2024-05-06 04:48:19.003042 autocython_jianjun-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4195 2024-05-06 02:09:25.000000 autocython_jianjun-1.3.4/README.md
+-rw-rw-rw-   0        0        0      824 2024-05-06 04:28:13.000000 autocython_jianjun-1.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 04:48:19.003976 autocython_jianjun-1.3.4/setup.cfg
```

### Comparing `AutoCython-jianjun-1.3.3/AutoCython/AutoCython.py` & `autocython_jianjun-1.3.4/AutoCython/AutoCython.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,19 +225,14 @@
             # Popen('python AutoCython_DataServerClient_Alice.py build_ext --inplace', stdout=PIPE, stderr=PIPE, cwd='build_test/test1\\')
             cython_popen = Popen(self._Popen_cmd.format(setup_file).split(" "), stdout=PIPE, stderr=PIPE, cwd=dirname)
 
             if delete:
                 delete_tmp_file_th = Thread(target=delete_tmp_file, args=(cython_popen, dirname, filename, setup_file, delete, complicating))
                 delete_tmp_file_th.start()
 
-            if wait:
-                cython_popen.wait()
-                if not complicating and os.path.isfile(os.path.join(dirname, "___init__.py")):
-                    os.rename(os.path.join(dirname, "___init__.py"), os.path.join(dirname, "__init__.py"))
-
             if not complicating and cython_popen.wait() != 0:
                 # 错误是输出
                 err_po = Popen_out(cython_popen, file_path)
                 print('\033[0;37;41m' + file_path, ':\033[0m')
                 print(err_po.out)
                 print(err_po.err)
                 print()
@@ -245,14 +240,19 @@
             return cython_popen, file_path
 
         except Exception as err:
             print('\033[0;37;41m', file_path, "编译运行失败!\033[0m")
             traceback.print_exc()
             print(err)
             return None
+        finally:
+            if wait:
+                cython_popen.wait()
+                if not complicating and os.path.isfile(os.path.join(dirname, "___init__.py")):
+                    os.rename(os.path.join(dirname, "___init__.py"), os.path.join(dirname, "__init__.py"))
 
     def compile(self, wait=True, delete=[], log=True) -> None:
         """ 编译所有文件 """
         def compile_th(delete):
             if self._compile_lock.locked():
                 print("Waiting for the end of the previous task")
 
@@ -373,15 +373,15 @@
         self.delete = ['b','p','c']
         self.python_cmd = "python"
 
         # a file
         self.file_path = ''
         self.a_file_flag = False
 
-        self.version = 'AutoCython V1.3.2'
+        self.version = 'AutoCython V1.3.4'
         # 像这样写格式好看一点
         self.help_info =(
                         "Usage: AutoCython [options] ...\n"+
                         "Options:\n"+
                         "  -f -F --file                Compile only a .py file.\n"+
                         "  -c -C --compile             Compile and assemble all .py files under the path.\n"+
                         "  -e -E --exclude             Excluded .py files or all .py files in a path, Used ';' split file or path.\n"+
```

### Comparing `AutoCython-jianjun-1.3.3/AutoCython_jianjun.egg-info/PKG-INFO` & `autocython_jianjun-1.3.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: AutoCython-jianjun
-Version: 1.3.3
-Summary: 自动Cython，使用Cython批量编译.py文件为.pyd文件！
-Home-page: https://github.com/EVA-JianJun/AutoCython
-Author: jianjun
-Author-email: 910667956@qq.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AutoCython
 
 **自动 Cython, 使用 Cython 批量编译 `.py` 文件为 `.pyd` 文件！**
 ![py_pyd][1]
 
 ## 安装
 
@@ -98,19 +88,20 @@
 在不需要编译的文件 **头两行** 任意一行写上 `# AucoCython No Compile` 则该文件会跳过编译.
 
 ## 更新记录
 1. 20220613 更新对Linux的支持, Linux下需要配置gcc&g++
 2. 20221123 可以通过文件头手动指定不编译的文件
 3. 20230306 更新可以指定命令行头如 `Python310` 以此支持非Widnows系统下编译
 4. 20230324 更新文档
+5. 20240506 修复编译失败时遗漏复原 __init__.py 的问题
 
   [1]: https://raw.githubusercontent.com/EVA-JianJun/GitPigBed/master/blog_files/img/AutoCython_20210824.png
   [2]: https://raw.githubusercontent.com/EVA-JianJun/GitPigBed/master/blog_files/img/AutoCython_20200316_2.jpg
   [3]: https://raw.githubusercontent.com/EVA-JianJun/GitPigBed/master/blog_files/img/AutoCython_20200316_3.jpg
   [4]: https://raw.githubusercontent.com/EVA-JianJun/GitPigBed/master/blog_files/img/AutoCython_20200316_4.jpg
   [5]: https://raw.githubusercontent.com/EVA-JianJun/GitPigBed/master/blog_files/img/AutoCython_20200316_5.jpg
   [6]: https://raw.githubusercontent.com/EVA-JianJun/GitPigBed/master/blog_files/img/AutoCython_20200316_6.jpg
   [7]: https://raw.githubusercontent.com/EVA-JianJun/GitPigBed/master/blog_files/img/AutoCython_20200316_7.jpg
   [8]: https://raw.githubusercontent.com/EVA-JianJun/GitPigBed/master/blog_files/img/AutoCython_20200316_8.jpg
   [9]: https://github.com/EVA-JianJun/AutoCython/releases
   [10]: https://raw.githubusercontent.com/EVA-JianJun/GitPigBed/master/blog_files/img/AutoCython_20200316_10.jpg
-  [11]: https://raw.githubusercontent.com/EVA-JianJun/GitPigBed/master/blog_files/img/AutoCython_20200316_11.jpg
+  [11]: https://raw.githubusercontent.com/EVA-JianJun/GitPigBed/master/blog_files/img/AutoCython_20200316_11.jpg
```

