# Comparing `tmp/xbstrap_version_bumper-0.0.1.tar.gz` & `tmp/xbstrap_version_bumper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbstrap_version_bumper-0.0.1.tar", last modified: Sun May  5 16:02:53 2024, max compression
+gzip compressed data, was "xbstrap_version_bumper-0.0.2.tar", last modified: Sun May  5 22:18:34 2024, max compression
```

## Comparing `xbstrap_version_bumper-0.0.1.tar` & `xbstrap_version_bumper-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 16:02:53.811851 xbstrap_version_bumper-0.0.1/
--rw-r--r--   0 alexander  (1000) wheel      (998)      818 2024-05-05 16:02:53.811851 xbstrap_version_bumper-0.0.1/PKG-INFO
--rw-r--r--   0 alexander  (1000) wheel      (998)      181 2024-05-05 15:57:05.000000 xbstrap_version_bumper-0.0.1/README.md
--rw-r--r--   0 alexander  (1000) wheel      (998)      807 2024-05-05 15:57:16.000000 xbstrap_version_bumper-0.0.1/pyproject.toml
--rw-r--r--   0 alexander  (1000) wheel      (998)       38 2024-05-05 16:02:53.811851 xbstrap_version_bumper-0.0.1/setup.cfg
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 16:02:53.809851 xbstrap_version_bumper-0.0.1/src/
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 16:02:53.810851 xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper/
--rw-r--r--   0 alexander  (1000) wheel      (998)        0 2024-05-05 15:38:58.000000 xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper/__init__.py
--rw-r--r--   0 alexander  (1000) wheel      (998)      102 2024-05-05 15:39:00.000000 xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper/__main__.py
--rw-r--r--   0 alexander  (1000) wheel      (998)     8430 2024-05-05 12:27:48.000000 xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper/linecounted_yaml.py
--rw-r--r--   0 alexander  (1000) wheel      (998)     9906 2024-05-05 15:53:57.000000 xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper/main.py
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 16:02:53.810851 xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper.egg-info/
--rw-r--r--   0 alexander  (1000) wheel      (998)      818 2024-05-05 16:02:53.000000 xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper.egg-info/PKG-INFO
--rw-r--r--   0 alexander  (1000) wheel      (998)      486 2024-05-05 16:02:53.000000 xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper.egg-info/SOURCES.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)        1 2024-05-05 16:02:53.000000 xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper.egg-info/dependency_links.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)       76 2024-05-05 16:02:53.000000 xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper.egg-info/entry_points.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)       55 2024-05-05 16:02:53.000000 xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper.egg-info/requires.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)       23 2024-05-05 16:02:53.000000 xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper.egg-info/top_level.txt
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 22:18:34.839440 xbstrap_version_bumper-0.0.2/
+-rw-r--r--   0 alexander  (1000) wheel      (998)     1075 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.2/LICENSE
+-rw-r--r--   0 alexander  (1000) wheel      (998)      840 2024-05-05 22:18:34.839440 xbstrap_version_bumper-0.0.2/PKG-INFO
+-rw-r--r--   0 alexander  (1000) wheel      (998)      181 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.2/README.md
+-rw-r--r--   0 alexander  (1000) wheel      (998)      807 2024-05-05 22:17:48.000000 xbstrap_version_bumper-0.0.2/pyproject.toml
+-rw-r--r--   0 alexander  (1000) wheel      (998)       38 2024-05-05 22:18:34.839440 xbstrap_version_bumper-0.0.2/setup.cfg
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 22:18:34.838440 xbstrap_version_bumper-0.0.2/src/
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 22:18:34.838440 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/
+-rw-r--r--   0 alexander  (1000) wheel      (998)        0 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/__init__.py
+-rw-r--r--   0 alexander  (1000) wheel      (998)      102 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/__main__.py
+-rw-r--r--   0 alexander  (1000) wheel      (998)     8430 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/linecounted_yaml.py
+-rw-r--r--   0 alexander  (1000) wheel      (998)    11360 2024-05-05 22:16:01.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/main.py
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 22:18:34.839440 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/
+-rw-r--r--   0 alexander  (1000) wheel      (998)      840 2024-05-05 22:18:34.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/PKG-INFO
+-rw-r--r--   0 alexander  (1000) wheel      (998)      494 2024-05-05 22:18:34.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)        1 2024-05-05 22:18:34.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)       76 2024-05-05 22:18:34.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/entry_points.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)       55 2024-05-05 22:18:34.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/requires.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)       23 2024-05-05 22:18:34.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/top_level.txt
```

### Comparing `xbstrap_version_bumper-0.0.1/PKG-INFO` & `xbstrap_version_bumper-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: xbstrap_version_bumper
-Version: 0.0.1
+Version: 0.0.2
 Summary: xbstrap distro auto version bumper
 Author-email: Alexander Richards <electrodeyt@gmail.com>
 Project-URL: Homepage, https://github.com/ElectrodeYT/xbstrap_version_bumper
 Project-URL: Issues, https://github.com/ElectrodeYT/xbstrap_version_bumper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: GitPython>=3.1.43
 Requires-Dist: requests>=2.31.0
 Requires-Dist: ruamel.yaml>=0.18.6
 
 # xbstrap_version_bumper
 
 This tool allows for easier bumping of versions for simple xbstrap packages.
```

### Comparing `xbstrap_version_bumper-0.0.1/pyproject.toml` & `xbstrap_version_bumper-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xbstrap_version_bumper"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="Alexander Richards", email="electrodeyt@gmail.com" },
 ]
 requires-python = ">=3.8"
 description="xbstrap distro auto version bumper"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper/linecounted_yaml.py` & `xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/linecounted_yaml.py`

 * *Files identical despite different names*

### Comparing `xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper/main.py` & `xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,22 +24,25 @@
             max_count,
             cur_count / (max_count or 100.0),
             message or "NO MESSAGE",
         )
 
 
 class Change:
-    def __init__(self, line: int, from_str: str = "", to_str: str = "", delete_line: bool = False):
+    def __init__(self, line: int, base_str: str = "", to_str: str = "",
+                 delete_line: bool = False, insert_line: bool = False, insert_auto_indent: bool = True):
         self.line = line
-        self.from_str = from_str
+        self.base_str = base_str
         self.to_str = to_str
         self.delete_line = delete_line
+        self.insert_line = insert_line
+        self.insert_auto_indent = insert_auto_indent
 
     def apply(self, line):
-        return line.replace(self.from_str, self.to_str)
+        return line.replace(self.base_str, self.to_str)
 
 
 class StrapFile:
     def __init__(self, path):
         self.path = path
         self.yaml = global_yaml.load(pathlib.Path(path))
         self.changes = []
@@ -60,28 +63,41 @@
 
         lines = []
         with open(self.path, 'r') as f:
             for line in f:
                 lines.append(line)
 
         deleted_lines = []
+        inserted_lines = {}
 
         for change in self.changes:
             if change.delete_line:
                 print(f'----> "{lines[change.line].strip()}" -> line removed')
                 deleted_lines.append(change.line)
                 continue
+            elif change.insert_line:
+                print(f'----> "{change.base_str.strip()}" -> line inserted')
+                inserted_lines[change.line] = change
+                continue
 
             new_line = change.apply(lines[change.line])
             print(f'----> "{lines[change.line].strip()}" -> "{new_line.strip()}"')
             lines[change.line] = new_line
 
         self.changes.clear()
         with open(self.path, 'w') as f:
             for i, line in enumerate(lines):
+                if i in inserted_lines.keys():
+                    leading_spaces = 0
+                    # If we need to calculate the autoindent for this, base it of the line below the new one
+                    if inserted_lines[i].insert_auto_indent:
+                        leading_spaces = len(line) - len(line.lstrip())
+                    leading_spaces_str = ' ' * leading_spaces
+                    line_to_write = leading_spaces_str + inserted_lines[i].base_str + '\n'
+                    f.write(line_to_write)
                 if i not in deleted_lines:
                     f.write(line)
 
 
 class Distro:
     def __init__(self, dir):
         self.strapfiles = []
@@ -184,15 +200,25 @@
         else:
             assert 'from_source' in package
             strapfile, source_in_package, source = self.__locate_source(package['from_source'])
             old_version = str(source['version'])
             self.__modify_source_impl(source, strapfile, package['from_source'], new_version)
 
         if 'revision' in package:
-            changes.append(Change(package['revision'].lc.line, delete_line=True))
+            changes.append(Change(package['revision'].lc.line,
+                                  f'revision: {package['revision']}',
+                                  'revision: 1'))
+        else:
+            if 'configure' in package:
+                revision_insert_line_num = package['configure'].lc.line - 1
+            elif 'build' in package:
+                revision_insert_line_num = package['build'].lc.line - 1
+            else:
+                raise Exception('Could not find a suitable place to insert revision tag')
+            changes.append(Change(revision_insert_line_num, 'revision: 1', insert_line=True))
 
         if 'configure' in package:
             for configure in package['configure']:
                 changes += self.__args_to_changes(configure['args'], old_version, new_version)
 
         if 'build' in package:
             for build in package['build']:
```

### Comparing `xbstrap_version_bumper-0.0.1/src/xbstrap_version_bumper.egg-info/PKG-INFO` & `xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: xbstrap_version_bumper
-Version: 0.0.1
+Version: 0.0.2
 Summary: xbstrap distro auto version bumper
 Author-email: Alexander Richards <electrodeyt@gmail.com>
 Project-URL: Homepage, https://github.com/ElectrodeYT/xbstrap_version_bumper
 Project-URL: Issues, https://github.com/ElectrodeYT/xbstrap_version_bumper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: GitPython>=3.1.43
 Requires-Dist: requests>=2.31.0
 Requires-Dist: ruamel.yaml>=0.18.6
 
 # xbstrap_version_bumper
 
 This tool allows for easier bumping of versions for simple xbstrap packages.
```

