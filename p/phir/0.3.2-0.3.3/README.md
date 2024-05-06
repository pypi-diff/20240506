# Comparing `tmp/phir-0.3.2.tar.gz` & `tmp/phir-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phir-0.3.2.tar", last modified: Fri Mar 15 20:14:46 2024, max compression
+gzip compressed data, was "phir-0.3.3.tar", last modified: Mon May  6 10:49:39 2024, max compression
```

## Comparing `phir-0.3.2.tar` & `phir-0.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:14:46.791276 phir-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:14:46.787276 phir-0.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-15 20:14:41.000000 phir-0.3.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:14:46.787276 phir-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-15 20:14:41.000000 phir-0.3.2/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-15 20:14:41.000000 phir-0.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-15 20:14:41.000000 phir-0.3.2/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-15 20:14:41.000000 phir-0.3.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-15 20:14:41.000000 phir-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-15 20:14:41.000000 phir-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-15 20:14:41.000000 phir-0.3.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-03-15 20:14:46.791276 phir-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-15 20:14:41.000000 phir-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:14:46.787276 phir-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-15 20:14:41.000000 phir-0.3.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:14:46.787276 phir-0.3.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-03-15 20:14:41.000000 phir-0.3.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-15 20:14:41.000000 phir-0.3.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-15 20:14:41.000000 phir-0.3.2/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-15 20:14:41.000000 phir-0.3.2/docs/source/phir.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:14:46.787276 phir-0.3.2/phir/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-15 20:14:41.000000 phir-0.3.2/phir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-15 20:14:41.000000 phir-0.3.2/phir/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-03-15 20:14:41.000000 phir-0.3.2/phir/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 20:14:41.000000 phir-0.3.2/phir/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:14:46.791276 phir-0.3.2/phir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-03-15 20:14:46.000000 phir-0.3.2/phir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-15 20:14:46.000000 phir-0.3.2/phir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 20:14:46.000000 phir-0.3.2/phir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-15 20:14:46.000000 phir-0.3.2/phir.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-15 20:14:46.000000 phir-0.3.2/phir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-15 20:14:46.000000 phir-0.3.2/phir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-15 20:14:41.000000 phir-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-15 20:14:41.000000 phir-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-03-15 20:14:41.000000 phir-0.3.2/schema.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 20:14:46.791276 phir-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-03-15 20:14:41.000000 phir-0.3.2/spec.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:14:46.791276 phir-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-15 20:14:41.000000 phir-0.3.2/tests/cond_barrier_qparallel.json
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-03-15 20:14:41.000000 phir-0.3.2/tests/example.json
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-15 20:14:41.000000 phir-0.3.2/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:39.709384 phir-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:39.705384 phir-0.3.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-06 10:49:34.000000 phir-0.3.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:39.705384 phir-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-06 10:49:34.000000 phir-0.3.3/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-06 10:49:34.000000 phir-0.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 10:49:34.000000 phir-0.3.3/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-06 10:49:34.000000 phir-0.3.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-06 10:49:34.000000 phir-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-06 10:49:34.000000 phir-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-06 10:49:34.000000 phir-0.3.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-06 10:49:39.709384 phir-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-06 10:49:34.000000 phir-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:39.705384 phir-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-06 10:49:34.000000 phir-0.3.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:39.709384 phir-0.3.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-06 10:49:34.000000 phir-0.3.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-06 10:49:34.000000 phir-0.3.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-06 10:49:34.000000 phir-0.3.3/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-06 10:49:34.000000 phir-0.3.3/docs/source/phir.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:39.709384 phir-0.3.3/phir/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 10:49:34.000000 phir-0.3.3/phir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-06 10:49:34.000000 phir-0.3.3/phir/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-06 10:49:34.000000 phir-0.3.3/phir/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:34.000000 phir-0.3.3/phir/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:39.709384 phir-0.3.3/phir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-06 10:49:39.000000 phir-0.3.3/phir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-06 10:49:39.000000 phir-0.3.3/phir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:49:39.000000 phir-0.3.3/phir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 10:49:39.000000 phir-0.3.3/phir.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-06 10:49:39.000000 phir-0.3.3/phir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 10:49:39.000000 phir-0.3.3/phir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-06 10:49:34.000000 phir-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-06 10:49:34.000000 phir-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27243 2024-05-06 10:49:34.000000 phir-0.3.3/schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:49:39.709384 phir-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-05-06 10:49:34.000000 phir-0.3.3/spec.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:39.709384 phir-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 10:49:34.000000 phir-0.3.3/tests/cond_barrier_qparallel.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-06 10:49:34.000000 phir-0.3.3/tests/example.json
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-06 10:49:34.000000 phir-0.3.3/tests/test_model.py
```

### Comparing `phir-0.3.2/.github/workflows/python-app.yml` & `phir-0.3.3/.github/workflows/python-app.yml`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,14 @@
     - name: Run tests
       run: |
         python -m pytest
     - name: Sphinx documentation build
       run: |
         make docs
     - name: Deploy to GitHub Pages
-      uses: peaceiris/actions-gh-pages@v3
+      uses: peaceiris/actions-gh-pages@v4
       if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' && matrix.python-version == '3.12' }}
       with:
         publish_branch: gh-pages
         github_token: ${{ secrets.GITHUB_TOKEN }}
         publish_dir: docs/build/html/
         force_orphan: true
```

### Comparing `phir-0.3.2/.github/workflows/python-publish.yml` & `phir-0.3.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `phir-0.3.2/CHANGELOG.md` & `phir-0.3.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `phir-0.3.2/LICENSE` & `phir-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phir-0.3.2/PKG-INFO` & `phir-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phir
-Version: 0.3.2
+Version: 0.3.3
 Summary: A data model and validation tool for PHIR (PECOS High-level Intermediate Representation).
 Author-email: Kartik Singhal <kartik.singhal@quantinuum.com>, Ciarán Ryan-Anderson <ciaran.ryan-anderson@quantinuum.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Quantinuum LLC
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `phir-0.3.2/README.md` & `phir-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `phir-0.3.2/docs/Makefile` & `phir-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `phir-0.3.2/docs/source/conf.py` & `phir-0.3.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `phir-0.3.2/phir/cli.py` & `phir-0.3.3/phir/cli.py`

 * *Files identical despite different names*

### Comparing `phir-0.3.2/phir/model.py` & `phir-0.3.3/phir/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 class CVarDefine(Data):
     """Defining Classical Variables."""
 
     data: Literal["cvar_define"]
     data_type: Literal["i64", "i32", "u64", "u32"]
     variable: Sym
-    size: PositiveInt | None = Field(strict=True)
+    size: PositiveInt | None = Field(default=None, strict=True)
 
     @model_validator(mode="after")
     def check_size(self: CVarDefine) -> CVarDefine:
         """Checks whether size fits the data_type."""
         msg = "`size` is greater than what `data_type` can handle"
         if self.size:
             match self.data_type:
```

### Comparing `phir-0.3.2/phir.egg-info/PKG-INFO` & `phir-0.3.3/phir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phir
-Version: 0.3.2
+Version: 0.3.3
 Summary: A data model and validation tool for PHIR (PECOS High-level Intermediate Representation).
 Author-email: Kartik Singhal <kartik.singhal@quantinuum.com>, Ciarán Ryan-Anderson <ciaran.ryan-anderson@quantinuum.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Quantinuum LLC
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `phir-0.3.2/phir.egg-info/SOURCES.txt` & `phir-0.3.3/phir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phir-0.3.2/pyproject.toml` & `phir-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phir-0.3.2/schema.json` & `phir-0.3.3/schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999472966269841%*

 * *Differences: {"'$defs'": "{'CVarDefine': {'properties': {'size': {'default': None}}, 'required': {delete: "*

 * *            '[3]}}}'}*

```diff
@@ -182,26 +182,26 @@
                             "exclusiveMinimum": 0,
                             "type": "integer"
                         },
                         {
                             "type": "null"
                         }
                     ],
+                    "default": null,
                     "title": "Size"
                 },
                 "variable": {
                     "title": "Variable",
                     "type": "string"
                 }
             },
             "required": [
                 "data",
                 "data_type",
-                "variable",
-                "size"
+                "variable"
             ],
             "title": "CVarDefine",
             "type": "object"
         },
         "Comment": {
             "additionalProperties": false,
             "description": "Optional comment.",
```

### Comparing `phir-0.3.2/spec.md` & `phir-0.3.3/spec.md`

 * *Files identical despite different names*

### Comparing `phir-0.3.2/tests/cond_barrier_qparallel.json` & `phir-0.3.3/tests/cond_barrier_qparallel.json`

 * *Files identical despite different names*

### Comparing `phir-0.3.2/tests/example.json` & `phir-0.3.3/tests/example.json`

 * *Files identical despite different names*

### Comparing `phir-0.3.2/tests/test_model.py` & `phir-0.3.3/tests/test_model.py`

 * *Files identical despite different names*

