# Comparing `tmp/scbl_utils-1.14.tar.gz` & `tmp/scbl_utils-1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scbl_utils-1.14.tar", max compression
+gzip compressed data, was "scbl_utils-1.15.tar", max compression
```

## Comparing `scbl_utils-1.14.tar` & `scbl_utils-1.15.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1079 2023-12-14 16:32:13.627049 scbl_utils-1.14/LICENSE
--rw-r--r--   0        0        0     8239 2024-01-23 19:13:12.443282 scbl_utils-1.14/README.md
--rw-r--r--   0        0        0      995 2024-04-19 20:37:24.798412 scbl_utils-1.14/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 16:32:13.628638 scbl_utils-1.14/scbl_utils/__init__.py
--rw-r--r--   0        0        0     8720 2024-04-16 14:41:10.856027 scbl_utils-1.14/scbl_utils/main.py
--rw-r--r--   0        0        0     7527 2024-03-27 18:02:48.976351 scbl_utils-1.14/scbl_utils/utils/defaults.py
--rw-r--r--   0        0        0     9033 2024-04-16 14:41:03.477720 scbl_utils-1.14/scbl_utils/utils/gdrive.py
--rw-r--r--   0        0        0    14379 2024-04-19 20:36:46.028249 scbl_utils-1.14/scbl_utils/utils/samplesheet.py
--rw-r--r--   0        0        0     4049 2023-12-14 16:32:13.629985 scbl_utils-1.14/scbl_utils/utils/validate.py
--rw-r--r--   0        0        0     9353 1970-01-01 00:00:00.000000 scbl_utils-1.14/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-12-14 16:32:13.627049 scbl_utils-1.15/LICENSE
+-rw-r--r--   0        0        0     8239 2024-01-23 19:13:12.443282 scbl_utils-1.15/README.md
+-rw-r--r--   0        0        0      995 2024-05-06 14:07:11.658741 scbl_utils-1.15/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 16:32:13.628638 scbl_utils-1.15/scbl_utils/__init__.py
+-rw-r--r--   0        0        0     8720 2024-04-16 14:41:10.856027 scbl_utils-1.15/scbl_utils/main.py
+-rw-r--r--   0        0        0     7527 2024-03-27 18:02:48.976351 scbl_utils-1.15/scbl_utils/utils/defaults.py
+-rw-r--r--   0        0        0     9668 2024-05-06 14:06:50.723984 scbl_utils-1.15/scbl_utils/utils/gdrive.py
+-rw-r--r--   0        0        0    14379 2024-04-19 20:36:46.028249 scbl_utils-1.15/scbl_utils/utils/samplesheet.py
+-rw-r--r--   0        0        0     4049 2023-12-14 16:32:13.629985 scbl_utils-1.15/scbl_utils/utils/validate.py
+-rw-r--r--   0        0        0     9353 1970-01-01 00:00:00.000000 scbl_utils-1.15/PKG-INFO
```

### Comparing `scbl_utils-1.14/LICENSE` & `scbl_utils-1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.14/README.md` & `scbl_utils-1.15/README.md`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.14/pyproject.toml` & `scbl_utils-1.15/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scbl-utils"
-version = "1.14"
+version = "1.15"
 description = "A set of command-line utilities that facilitate data processing at the Single Cell Biology Lab at the Jackson Laboratory."
 authors = ["Ahmed Said <ahmed.said@jax.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/TheJacksonLaboratory/scbl-utils/"
 documentation = "https://github.com/TheJacksonLaboratory/scbl-utils/"
```

### Comparing `scbl_utils-1.14/scbl_utils/main.py` & `scbl_utils-1.15/scbl_utils/main.py`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.14/scbl_utils/utils/defaults.py` & `scbl_utils-1.15/scbl_utils/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.14/scbl_utils/utils/gdrive.py` & `scbl_utils-1.15/scbl_utils/utils/gdrive.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,28 @@
     # Get credentials, project, tool, and reference dirs
     creds = gclient.auth
     libraries, sample_name, project, tool, reference_dirs, species = (
         df_row[col]
         for col in ('libraries', 'sample_name', 'project', 'tool', 'reference_dirs', 'species')
     )
 
+    if not project:
+        params = pd.Series()
+        params['tool_version'] = get_latest_version(tool)
+
+        message = f'\nThere are no spreadsheets in the Google Drive folder at https://drive.google.com/drive/folders/{metrics_dir_id} containing the SCBL Project [bold orange1]{project}[/] and the tool [bold orange1]{tool}[/].'
+        params['reference_path'] = genomes_from_user(
+            message=message,
+            reference_dirs=reference_dirs,
+            sample_name=sample_name,
+            libraries=libraries
+        )
+
+        return params
+
     # Build service
     service = build(serviceName='drive', version='v3', credentials=creds)
 
     # Get all files in Google Drive folder matching criteria, sort
     # by modified time, and get their IDs
     result = (
         service.files()
@@ -192,14 +206,17 @@
         else:
             metrics_df = pd.concat(metrics_dfs, axis=1, join='outer')
 
         # metrics_dfs[0].join(other=metrics_dfs[1:], on='libraries', how='outer', rsuffix='1')  # type: ignore
 
         # Filter metrics_df to contain just those projects matching this
         # project and tool
+        if 'project' not in metrics_df.columns:
+            continue
+
         project_df = metrics_df[
             (metrics_df['project'] == project)
             & (metrics_df['tool'] == tool)
             & (metrics_df['reference'].str.match(genome_pattern, case=False))
         ].copy()
 
         if project_df.shape[0] < 1:
```

### Comparing `scbl_utils-1.14/scbl_utils/utils/samplesheet.py` & `scbl_utils-1.15/scbl_utils/utils/samplesheet.py`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.14/scbl_utils/utils/validate.py` & `scbl_utils-1.15/scbl_utils/utils/validate.py`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.14/PKG-INFO` & `scbl_utils-1.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scbl-utils
-Version: 1.14
+Version: 1.15
 Summary: A set of command-line utilities that facilitate data processing at the Single Cell Biology Lab at the Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/scbl-utils/
 License: MIT
 Author: Ahmed Said
 Author-email: ahmed.said@jax.org
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

