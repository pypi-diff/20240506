# Comparing `tmp/diwork-1.2.3.tar.gz` & `tmp/diwork-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diwork-1.2.3.tar", last modified: Sat May  4 11:52:42 2024, max compression
+gzip compressed data, was "diwork-1.3.0.tar", last modified: Mon May  6 09:30:18 2024, max compression
```

## Comparing `diwork-1.2.3.tar` & `diwork-1.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 11:52:42.838133 diwork-1.2.3/
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2023-02-10 11:11:21.000000 diwork-1.2.3/LICENSE
--rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-04 11:52:42.838133 diwork-1.2.3/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      211 2024-05-04 08:36:38.000000 diwork-1.2.3/README.md
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 11:52:42.835133 diwork-1.2.3/diwork/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      343 2024-05-04 08:22:40.000000 diwork-1.2.3/diwork/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      115 2024-05-04 08:01:22.000000 diwork-1.2.3/diwork/__main__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)       47 2024-05-04 11:51:56.000000 diwork-1.2.3/diwork/__version__.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 11:52:42.837133 diwork-1.2.3/diwork/diwork_mains/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      734 2024-05-04 08:48:21.000000 diwork-1.2.3/diwork/diwork_mains/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5693 2024-05-04 10:26:10.000000 diwork-1.2.3/diwork/diwork_mains/diwork_archive.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5116 2024-05-04 10:48:42.000000 diwork-1.2.3/diwork/diwork_mains/diwork_clone.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     7521 2023-03-17 19:19:40.000000 diwork-1.2.3/diwork/diwork_mains/diwork_diff.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5668 2024-05-04 11:48:44.000000 diwork-1.2.3/diwork/diwork_mains/diwork_diffclone.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     3241 2023-02-18 08:20:12.000000 diwork-1.2.3/diwork/diwork_mains/diwork_difx.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     9181 2023-04-11 08:18:44.000000 diwork-1.2.3/diwork/diwork_mains/diwork_exec.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5174 2024-05-04 10:36:42.000000 diwork-1.2.3/diwork/diwork_mains/diwork_hash.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      582 2023-02-18 08:13:38.000000 diwork-1.2.3/diwork/diwork_mains/diwork_help.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     2900 2023-03-09 08:12:58.000000 diwork-1.2.3/diwork/diwork_mains/diwork_repeats.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     9064 2023-03-09 21:18:05.000000 diwork-1.2.3/diwork/diwork_mains/diwork_sshclone.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 11:52:42.838133 diwork-1.2.3/diwork/diwork_ways/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      583 2024-05-04 10:44:35.000000 diwork-1.2.3/diwork/diwork_ways/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1033 2024-05-04 10:29:33.000000 diwork-1.2.3/diwork/diwork_ways/diwork_parse.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)    10915 2024-05-04 11:35:31.000000 diwork-1.2.3/diwork/diwork_ways/diwork_sup.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1390 2024-05-04 10:12:20.000000 diwork-1.2.3/diwork/main.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 11:52:42.838133 diwork-1.2.3/diwork.egg-info/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-04 11:52:42.000000 diwork-1.2.3/diwork.egg-info/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      795 2024-05-04 11:52:42.000000 diwork-1.2.3/diwork.egg-info/SOURCES.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-05-04 11:52:42.000000 diwork-1.2.3/diwork.egg-info/dependency_links.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       44 2024-05-04 11:52:42.000000 diwork-1.2.3/diwork.egg-info/entry_points.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       14 2024-05-04 11:52:42.000000 diwork-1.2.3/diwork.egg-info/requires.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        7 2024-05-04 11:52:42.000000 diwork-1.2.3/diwork.egg-info/top_level.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       81 2024-05-04 07:49:04.000000 diwork-1.2.3/pyproject.toml
--rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-05-04 11:52:42.838133 diwork-1.2.3/setup.cfg
--rw-r--r--   0 the220th  (1000) the220th  (1000)      997 2024-05-04 08:57:56.000000 diwork-1.2.3/setup.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 09:30:18.760968 diwork-1.3.0/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2023-02-10 11:11:21.000000 diwork-1.3.0/LICENSE
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-06 09:30:18.760968 diwork-1.3.0/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      211 2024-05-04 08:36:38.000000 diwork-1.3.0/README.md
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 09:30:18.753968 diwork-1.3.0/diwork/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      343 2024-05-04 08:22:40.000000 diwork-1.3.0/diwork/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      115 2024-05-04 08:01:22.000000 diwork-1.3.0/diwork/__main__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       47 2024-05-06 09:21:12.000000 diwork-1.3.0/diwork/__version__.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 09:30:18.759968 diwork-1.3.0/diwork/diwork_mains/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      734 2024-05-04 08:48:21.000000 diwork-1.3.0/diwork/diwork_mains/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5695 2024-05-06 09:17:43.000000 diwork-1.3.0/diwork/diwork_mains/diwork_archive.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5118 2024-05-06 09:17:43.000000 diwork-1.3.0/diwork/diwork_mains/diwork_clone.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     7525 2024-05-06 09:17:44.000000 diwork-1.3.0/diwork/diwork_mains/diwork_diff.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     6710 2024-05-06 09:29:15.000000 diwork-1.3.0/diwork/diwork_mains/diwork_diffclone.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     3245 2024-05-06 09:17:43.000000 diwork-1.3.0/diwork/diwork_mains/diwork_difx.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     9183 2024-05-06 09:17:44.000000 diwork-1.3.0/diwork/diwork_mains/diwork_exec.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5176 2024-05-06 09:17:43.000000 diwork-1.3.0/diwork/diwork_mains/diwork_hash.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      582 2023-02-18 08:13:38.000000 diwork-1.3.0/diwork/diwork_mains/diwork_help.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     2902 2024-05-06 09:17:44.000000 diwork-1.3.0/diwork/diwork_mains/diwork_repeats.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     9066 2024-05-06 09:17:43.000000 diwork-1.3.0/diwork/diwork_mains/diwork_sshclone.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 09:30:18.760968 diwork-1.3.0/diwork/diwork_ways/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      613 2024-05-06 09:17:43.000000 diwork-1.3.0/diwork/diwork_ways/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1033 2024-05-04 10:29:33.000000 diwork-1.3.0/diwork/diwork_ways/diwork_parse.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)    11534 2024-05-06 09:18:41.000000 diwork-1.3.0/diwork/diwork_ways/diwork_sup.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1390 2024-05-04 10:12:20.000000 diwork-1.3.0/diwork/main.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 09:30:18.760968 diwork-1.3.0/diwork.egg-info/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-06 09:30:18.000000 diwork-1.3.0/diwork.egg-info/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      795 2024-05-06 09:30:18.000000 diwork-1.3.0/diwork.egg-info/SOURCES.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-05-06 09:30:18.000000 diwork-1.3.0/diwork.egg-info/dependency_links.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       44 2024-05-06 09:30:18.000000 diwork-1.3.0/diwork.egg-info/entry_points.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       14 2024-05-06 09:30:18.000000 diwork-1.3.0/diwork.egg-info/requires.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        7 2024-05-06 09:30:18.000000 diwork-1.3.0/diwork.egg-info/top_level.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       81 2024-05-04 07:49:04.000000 diwork-1.3.0/pyproject.toml
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-05-06 09:30:18.761968 diwork-1.3.0/setup.cfg
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      997 2024-05-04 08:57:56.000000 diwork-1.3.0/setup.py
```

### Comparing `diwork-1.2.3/LICENSE` & `diwork-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diwork-1.2.3/diwork/diwork_mains/__init__.py` & `diwork-1.3.0/diwork/diwork_mains/__init__.py`

 * *Files identical despite different names*

### Comparing `diwork-1.2.3/diwork/diwork_mains/diwork_archive.py` & `diwork-1.3.0/diwork/diwork_mains/diwork_archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     legacy_version = 1
     d = {"hashes":{}, "sizes": {}}
 
     errors = []
     folder_path_name = os.path.basename(folder_path)
     # folder_path_name = "content"
-    files = sorted(getFilesList(folder_path))
+    files = sorted(get_files_list(folder_path))
     files = [os.path.abspath(file_i) for file_i in files]
     files_rel = [rel_path(file_i, folder_path) for file_i in files]
 
     with zipfile.ZipFile(path_to_zip, mode="w") as zfd:
         gi, gN = 0, len(files)
         for file_i, file_rel_i in zip(files, files_rel):
             gi-=-1
```

### Comparing `diwork-1.2.3/diwork/diwork_mains/diwork_clone.py` & `diwork-1.3.0/diwork/diwork_mains/diwork_clone.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         dir_i_2 = os.path.join(folder2_abs, dir_i_rel)
         mkdir(dir_i_2)
         #exe_out = exe(f"mkdir -p \"{dir_i_2}\"")
         #if(exe_out[1] != ""):
         #    pout(f"ERROR: {exe_out[1]}")
         #    exit()
 
-    files_abs_1 = getFilesList(folder1_abs)
+    files_abs_1 = get_files_list(folder1_abs)
     files_abs_1 = sorted(files_abs_1)
     gi, N = 0, len(files_abs_1)
     for file_i_1 in files_abs_1:
         gi+=1
         if(os.path.islink(file_i_1) == False and is_file(file_i_1) == False):
             err_out.append(f"\"{file_i_1}\" is not file or does not exists, it will be skipped. ")
             continue
```

### Comparing `diwork-1.2.3/diwork/diwork_mains/diwork_diff.py` & `diwork-1.3.0/diwork/diwork_mains/diwork_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,16 +106,16 @@
             pout(f"\"{letter_i}\" cannot repeat. ")
             exit()
     if(len(mode) == 2 and mode[0] in "nr" and mode[1] in "nr"):
         HASH_NOT_NEEDED = True
     else:
         HASH_NOT_NEEDED = False
     d1, d2, dr1, dr2 = {}, {}, {}, {}
-    files_abs_old = sorted(getFilesList(folder_old_abs))
-    files_abs_new = sorted(getFilesList(folder_new_abs))
+    files_abs_old = sorted(get_files_list(folder_old_abs))
+    files_abs_new = sorted(get_files_list(folder_new_abs))
     gi, N = 0, len(files_abs_old)+len(files_abs_new)
     for file_i in files_abs_old:
         gi+=1
         if(is_file(file_i) == False):
             err_out.append(f"\"{file_i}\" is not file or does not exists, it will be skipped. ")
             continue
         if(HASH_NOT_NEEDED == True):
```

### Comparing `diwork-1.2.3/diwork/diwork_mains/diwork_diffclone.py` & `diwork-1.3.0/diwork/diwork_mains/diwork_diffclone.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 
 import os
 import sys
 import argparse
 import shutil
+import threading
 
 from diwork_ways import *
 
 from tqdm import tqdm
 
 
 def calc_hash_dict_of_dir(dir_path: str) -> dict:
     d = {}
     dir_path = os.path.abspath(dir_path)
-    files = getFilesList(dir_path)
+    files = get_files_list(dir_path)
     files = sorted(files)
     for file_i in tqdm(files):
         file_i_rel = os.path.relpath(file_i, dir_path)
         d[file_i_rel] = get_hash_file(file_i)
     return d
 
 
@@ -27,24 +28,27 @@
         description="This module will clone all the contents of {folder_src} to {folder_dest}, but only files, which does not already contains in {folder_dest}. "
                     "Old files will be renamed if needed.")
     parser.add_argument("folder_src", type=str, nargs=1,
                        help="Path to source directory")
     parser.add_argument("folder_dest", type=str, nargs=1,
                        help="Path to destination directory")
     parser.add_argument("--no_check_hash", default=False, action='store_true',
-                       help="Check hashes of files from {folder_dest}")
+                       help="Check hashes of files from {folder_src} and {folder_dest}")
+    parser.add_argument("--skip_copy", default=False, action='store_true',
+                       help="Skip copy phase. Only hash ckeck.")
 
     parser = common_init_parser(parser)
     args = parser.parse_args(args)
     common_init_parse(args)
 
     folder1 = args.folder_src[0]
     folder2 = args.folder_dest[0]
     err_out = []
     check_hash = not args.no_check_hash
+    skip_copy = args.skip_copy
     folder1_abs = os.path.abspath(folder1)
     folder2_abs = os.path.abspath(folder2)
     if not is_folder(folder1_abs):
         pout(f"\"{folder1_abs}\" is not folder. ")
         exit()
     if not is_folder(folder2_abs):
         pout(f"\"{folder2_abs}\" is not folder. ")
@@ -54,76 +58,91 @@
         pout(f"Directory \"{folder1_abs}\" contains directory \"{folder2_abs}\". ")
         input("Enter to continue...")
     if folder2_abs in folder1_abs:
         pout(f"Directory \"{folder2_abs}\" contains directory \"{folder1_abs}\". ")
         input("Enter to continue...")
 
     pout(f"Calculating hash tree of directory \"{folder1_abs}\"...")
-    d1 = calc_hash_dict_of_dir(folder1_abs)
+    # d1 = calc_hash_dict_of_dir(folder1_abs)
+    cp_count = 0
 
     pout("Diffclonning...")
     # 3 варианта:
     # 1. Такого файла не существует в folder2, тогда просто копируем
     # 2. Такой файл существует в folder2 и hash совпадает, тогда ничего не делаем
     # 3. Такой файл существует в folder2 и hash не совпадает, тогда старый переименовываем, а новый копируем
 
     dirs_abs_1 = getDirsList(folder1_abs)
     dirs_abs_1 = sorted(dirs_abs_1)
-    for dir_i_1 in dirs_abs_1:
-        dir_i_rel = rel_path(dir_i_1, folder1_abs)
-        dir_i_2 = os.path.join(folder2_abs, dir_i_rel)
-        if not os.path.exists(dir_i_2):
-            mkdir(dir_i_2, p=True)
-
-    files1, files2 = getFilesList(folder1_abs), getFilesList(folder2_abs)
-    for file1_i in tqdm(files1):
-        try:
-            if os.path.islink(file1_i):
-                if Global.symlink_mode == 0:
-                    continue
-
-            file1_i_rel = str(os.path.relpath(file1_i, folder1_abs))
-            file2_i = os.path.join(folder2_abs, file1_i_rel)
-            if not os.path.isfile(file2_i):  # case 1
-                if copy_file(file1_i, file2_i) in [False, None]:
-                    err_out.append(f"Cannot copy \"{file1_i}\" to \"{file2_i}\". ")
-            else:
-                file2_i_hash = get_hash_file(file2_i)
-                if d1[file1_i_rel] == file2_i_hash:  # case 2
-                    pass  # ничего не делаем
-                else:  # case 3
-                    file2_i_time = get_time_file(file2_i)
-                    os.rename(file2_i, f"{file2_i}---{file2_i_time}.bak")
+    files1, files2 = get_files_list(folder1_abs), get_files_list(folder2_abs)
+    
+    if not skip_copy:
+        for dir_i_1 in dirs_abs_1:
+            dir_i_rel = rel_path(dir_i_1, folder1_abs)
+            dir_i_2 = os.path.join(folder2_abs, dir_i_rel)
+            if not os.path.exists(dir_i_2):
+                mkdir(dir_i_2, p=True)
+
+        for file1_i in tqdm(files1):
+            try:
+                if os.path.islink(file1_i):
+                    if Global.symlink_mode == 0:
+                        continue
+
+                file1_i_rel = str(os.path.relpath(file1_i, folder1_abs))
+                file2_i = os.path.join(folder2_abs, file1_i_rel)
+                if not os.path.isfile(file2_i):  # case 1
                     if copy_file(file1_i, file2_i) in [False, None]:
                         err_out.append(f"Cannot copy \"{file1_i}\" to \"{file2_i}\". ")
-        except Exception as e:
-            pout(str(e))
-            err_out.append(f"\"{file1_i}\"")
-
-    if platform != "win32":
-        os.sync()
-    if len(err_out) != 0:
-        pout(f"\n===============\nSome troubles happened:")
-        for err_i in err_out:
-            pout(f"\t{err_i}")
-        pout(f"===============")
+                    else:
+                        cp_count += 1
+                else:
+                    x1 = ThreadWithReturnValue(1, target=get_hash_file, args=(file1_i,))
+                    x2 = ThreadWithReturnValue(2, target=get_hash_file, args=(file2_i,))
+                    x1.start(), x2.start()
+                    file1_i_hash, file2_i_hash = x1.join(), x2.join()
+                    if file1_i_hash == file2_i_hash:  # case 2
+                        pass  # ничего не делаем
+                    else:  # case 3
+                        file2_i_time = get_time_file(file2_i)
+                        os.rename(file2_i, f"{file2_i}---{file2_i_time}.bak")
+                        if copy_file(file1_i, file2_i) in [False, None]:
+                            err_out.append(f"Cannot copy \"{file1_i}\" to \"{file2_i}\". ")
+                        else:
+                            cp_count += 1
+            except Exception as e:
+                pout(str(e))
+                err_out.append(f"\"{file1_i}\"")
+
+        if platform != "win32":
+            os.sync()
+        if len(err_out) != 0:
+            pout(f"\n===============\nSome troubles happened:")
+            for err_i in err_out:
+                pout(f"\t{err_i}")
+            pout(f"===============")
+
+        pout(f"Coping done! {cp_count} copy operation total. ")
 
     IF_OK = True
     if check_hash:
         err_out = []
         pout("Checking...")
         for file1_i in tqdm(files1):
             try:
                 if os.path.islink(file1_i):
                     if Global.symlink_mode == 0:
                         continue
                 file1_i_rel = str(os.path.relpath(file1_i, folder1_abs))
                 file2_i = os.path.join(folder2_abs, file1_i_rel)
-                file2_i_hash = get_hash_file(file2_i)
-                if d1[file1_i_rel] != file2_i_hash:
+                x1 = ThreadWithReturnValue(1, target=get_hash_file, args=(file1_i,))
+                x2 = ThreadWithReturnValue(2, target=get_hash_file, args=(file2_i,))
+                x1.start(), x2.start()
+                file1_i_hash, file2_i_hash = x1.join(), x2.join()
+                if file1_i_hash != file2_i_hash:
                     buffS = (
                         f"HASHES OF FILES DOES NOT MATCH: "
                         f"\"{d1[file1_i_rel]}\" of \"{file1_i}\" and "
                         f"\"{file2_i_hash}\" of \"{file2_i}\""
                              )
                     pout(buffS)
                     err_out.append(buffS)
```

### Comparing `diwork-1.2.3/diwork/diwork_mains/diwork_difx.py` & `diwork-1.3.0/diwork/diwork_mains/diwork_difx.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     if(is_folder(folder1_abs) == False):
         pout(f"\"{folder1_abs}\" is not folder. ")
         exit()
     if(is_folder(folder2_abs) == False):
         pout(f"\"{folder2_abs}\" is not folder. ")
         exit()
 
-    files1_abs, files2_abs = sorted(getFilesList(folder1_abs)), sorted(getFilesList(folder2_abs))
+    files1_abs, files2_abs = sorted(get_files_list(folder1_abs)), sorted(get_files_list(folder2_abs))
     dr1, dr2 = {}, {}
     gi, N = 0, len(files1_abs)+len(files2_abs)
     for file_i in files1_abs:
         gi+=1
         if(is_file(file_i) == False):
             err_out.append(f"\"{file_i}\" is not file or does not exists, it will be skipped. ")
             continue
```

### Comparing `diwork-1.2.3/diwork/diwork_mains/diwork_exec.py` & `diwork-1.3.0/diwork/diwork_mains/diwork_exec.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                 #     pout(f"ERROR: {exe_out[1]}")
                 #     exit()
                 mkdir(dir_out_i_abs)
             else:
                 pout(cmd2exec)
                 
 
-    files_abs_in = getFilesList(folder_in_abs)
+    files_abs_in = get_files_list(folder_in_abs)
     files_abs_in = sorted(files_abs_in)
     gi, N = 0, len(files_abs_in)
     for file_in_i in files_abs_in:
         gi+=1
         if(is_file(file_in_i) == False):
             err_out.append(f"\"{file_in_i}\" is not file or does not exists, it will be skipped. ")
             continue
```

### Comparing `diwork-1.2.3/diwork/diwork_mains/diwork_hash.py` & `diwork-1.3.0/diwork/diwork_mains/diwork_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         RES_OUT_PREFIX_HIERARCHY = "with"
 
     dir_hashes = {}
     ggi, ggN = 0, len(folders_abs)
     for folder_i in folders_abs:
         ggi-=-1
         pout(f"\nCalculating hash of directory \"{folder_i}\":")
-        files = getFilesList(folder_i)
+        files = get_files_list(folder_i)
         files = sorted(files)
         files = exclude_files(files, files_exclude)
         hashes = []
         gi, files_len = 0, len(files)
         for file_i in files:
             gi+=1
             if(os.path.islink(file_i) == False and is_file(file_i) == False):
```

### Comparing `diwork-1.2.3/diwork/diwork_mains/diwork_help.py` & `diwork-1.3.0/diwork/diwork_mains/diwork_help.py`

 * *Files identical despite different names*

### Comparing `diwork-1.2.3/diwork/diwork_mains/diwork_repeats.py` & `diwork-1.3.0/diwork/diwork_mains/diwork_repeats.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     IF_YES = args.yes
     err_out = []
     files_to_delete = []
     folder_abs = os.path.abspath(folder)
     if(is_folder(folder_abs) == False):
         pout(f"\"{folder_abs}\" is not folder. ")
         exit()
-    files_abs = sorted(getFilesList(folder_abs))
+    files_abs = sorted(get_files_list(folder_abs))
     hashes = set()
     d = {}
     gi, N = 0, len(files_abs)
     for file_i in files_abs:
         gi+=1
         if(is_file(file_i) == False):
             err_out.append(f"\"{file_i}\" is not file or does not exists, it will be skipped. ")
```

### Comparing `diwork-1.2.3/diwork/diwork_mains/diwork_sshclone.py` & `diwork-1.3.0/diwork/diwork_mains/diwork_sshclone.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     if(exe_res[0] != "1"):
         pout(f"Directory \"{user}@{host}:{path}\" does not exists. ")
         exit()
 
     if(if_src_remote == True):
         cpfiles = get_all_files_from_remote_host(user, host, PORT, path, PSWD)
     else:
-        cpfiles = getFilesList(folder1)
+        cpfiles = get_files_list(folder1)
 
     if(if_src_remote == False):
         delete_all_if_dir_not_empty_ssh(path, user, host, PORT, PSWD)
         dirs = get_dirs_needed_for_files(cpfiles)
         for dir_i in dirs:
             dir_i_rel = rel_path(dir_i, folder1)
             dir_i_2 = os.path.join(path, dir_i_rel)
```

### Comparing `diwork-1.2.3/diwork/diwork_ways/diwork_parse.py` & `diwork-1.3.0/diwork/diwork_ways/diwork_parse.py`

 * *Files identical despite different names*

### Comparing `diwork-1.2.3/diwork/diwork_ways/diwork_sup.py` & `diwork-1.3.0/diwork/diwork_ways/diwork_sup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,45 @@
 
 import os
 import sys
 import subprocess
 import hashlib
 import datetime
 import shutil
+from threading import Thread
+
 
 class Global():
     version = None
     outfile = None
     symlink_mode = None
-    
 
-def getFilesList(dirPath: str) -> list:
+
+class ThreadWithReturnValue(Thread):
+
+    def __init__(self, index: int, group=None, target=None, name=None,
+                 args=(), kwargs={}, Verbose=None):
+        Thread.__init__(self, group, target, name, args, kwargs)
+        self._index = index
+        self._return = None
+
+    def run(self):
+        if self._target is not None:
+            self._return = self._target(*self._args,
+                                        **self._kwargs)
+
+    def get_index(self):
+        return self._index
+
+    def join(self, *args):
+        Thread.join(self, *args)
+        return self._return
+
+
+def get_files_list(dirPath: str) -> list:
     return [os.path.join(path, name) for path, subdirs, files in os.walk(dirPath) for name in files]
 
 
 def getDirsList(dirPath: str) -> list:
     dirs = [os.path.join(path, name) for path, subdirs, files in os.walk(dirPath) for name in subdirs]
     return list(set(dirs))
 
@@ -67,15 +90,15 @@
             os.remove(os.path.join(root, file_i))
         for dir in dirs:
             os.rmdir(os.path.join(root, dir))
     if(root_dir_too == True):
         os.rmdir(folder_path)
 
 
-def pout(msg : str, endl = True):
+def pout(msg: str, endl = True):
     if(endl == False):
         pout_low(msg)
     else:
         pout_low(msg + "\n")
 
 
 def pout_low(msg: str):
```

### Comparing `diwork-1.2.3/diwork/main.py` & `diwork-1.3.0/diwork/main.py`

 * *Files identical despite different names*

### Comparing `diwork-1.2.3/diwork.egg-info/SOURCES.txt` & `diwork-1.3.0/diwork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diwork-1.2.3/setup.py` & `diwork-1.3.0/setup.py`

 * *Files identical despite different names*

