# Comparing `tmp/commit_msg_git_hook-0.6.0.tar.gz` & `tmp/commit_msg_git_hook-0.6.1.tar.gz`

## Comparing `commit_msg_git_hook-0.6.0.tar` & `commit_msg_git_hook-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/__builtins__.pyi
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/src/commit_msg_git_hook/__init__.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/src/commit_msg_git_hook/commit_msg.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/src/commit_msg_git_hook/scan_git.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/src/commit_msg_git_hook/setup.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/src/commit_msg_git_hook/templates/commit-msg.config.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/src/commit_msg_git_hook/templates/darwin/commit-msg
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/src/commit_msg_git_hook/templates/linux/commit-msg
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/src/commit_msg_git_hook/templates/win32/commit-msg
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/LICENSE
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/README.md
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/__builtins__.pyi
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/__init__.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/commit_msg.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/scan_git.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/setup.py
+-rw-r--r--   0        0        0    26665 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/assets/Exemplo-mensagem-inválida.png
+-rw-r--r--   0        0        0     9973 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/assets/Exemplo-mensagem-muito-longa.png
+-rw-r--r--   0        0        0    23803 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/assets/commit-msg.config.json.png
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/templates/commit-msg.config.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/templates/darwin/commit-msg
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/templates/linux/commit-msg
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/templates/win32/commit-msg
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/README.md
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 commit_msg_git_hook-0.6.1/PKG-INFO
```

### Comparing `commit_msg_git_hook-0.6.0/src/commit_msg_git_hook/commit_msg.py` & `commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/commit_msg.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     return regex
 
 
 def get_commit_file_first_line() -> str:
     commit_file = sys.argv[1]
 
     f = open(commit_file, "r")
-    first_line = f.readline()
+    first_line = f.readline().rstrip()
     f.close()
 
     return first_line
 
 
 def check_msg_empty(msg) -> None:
     if msg == "" or msg == "\n":
```

### Comparing `commit_msg_git_hook-0.6.0/src/commit_msg_git_hook/scan_git.py` & `commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/scan_git.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.6.0/src/commit_msg_git_hook/setup.py` & `commit_msg_git_hook-0.6.1/src/commit_msg_git_hook/setup.py`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.6.0/LICENSE` & `commit_msg_git_hook-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commit_msg_git_hook-0.6.0/pyproject.toml` & `commit_msg_git_hook-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "commit_msg_git_hook"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="Lucio Meira David", email="lucio.meira@om30.com.br" },
 ]
 description = "A set of tools to validate git Conventional Commit messages."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

