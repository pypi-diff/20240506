# Comparing `tmp/skillsnetwork_jupyter_extension-2.3.0rc0.tar.gz` & `tmp/skillsnetwork_jupyter_extension-2.3.0rc1.tar.gz`

## Comparing `skillsnetwork_jupyter_extension-2.3.0rc0.tar` & `skillsnetwork_jupyter_extension-2.3.0rc1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.copier-answers.yml
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.prettierignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.tool-versions
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.whitesource
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.yarnrc.yml
--rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/CHANGELOG.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/CODEOWNERS
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/RELEASE.md
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/install.json
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/setup.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/tsconfig.json
--rw-r--r--   0        0        0   227036 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/yarn.lock
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/jupyter-config/server-config/skillsnetwork_jupyter_extension.json
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/schema/toolbar.json
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/__init__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/_version.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/handlers.py
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/package.json
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json
--rw-r--r--   0        0        0    21429 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/496.9f74bf3e410d1c115cd7.js
--rw-r--r--   0        0        0    30112 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/736.1176de539f275bcd21aa.js
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/956.9f7a54c8b777ce434d6b.js
--rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.deab4c15018528576b5d.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/style.js
--rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/config.ts
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/dialog.ts
--rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/handler.ts
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/index.ts
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/sn-file-library.ts
--rw-r--r--   0        0        0    22974 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/tools.ts
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/menu/index.ts
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/theme/index.ts
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/toolbar/index.ts
--rw-r--r--   0        0        0   880991 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/static/extension_demo.gif
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/style/index.js
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/LICENSE
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/README.md
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/pyproject.toml
--rw-r--r--   0        0        0    19094 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.copier-answers.yml
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.prettierignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.tool-versions
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.whitesource
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.yarnrc.yml
+-rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/CODEOWNERS
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/RELEASE.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/install.json
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/setup.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/tsconfig.json
+-rw-r--r--   0        0        0   227036 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/yarn.lock
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/jupyter-config/server-config/skillsnetwork_jupyter_extension.json
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/schema/toolbar.json
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/_version.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/handlers.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/package.json
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json
+-rw-r--r--   0        0        0    21440 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/496.6b8b1c179401632c8943.js
+-rw-r--r--   0        0        0    30112 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/736.1176de539f275bcd21aa.js
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/956.9f7a54c8b777ce434d6b.js
+-rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.1114a7d16c81f17285d7.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/config.ts
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/dialog.ts
+-rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/handler.ts
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/index.ts
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/sn-file-library.ts
+-rw-r--r--   0        0        0    23077 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/tools.ts
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/menu/index.ts
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/theme/index.ts
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/toolbar/index.ts
+-rw-r--r--   0        0        0   880991 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/static/extension_demo.gif
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/style/index.js
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/LICENSE
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/README.md
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    19094 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/PKG-INFO
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/.copier-answers.yml` & `skillsnetwork_jupyter_extension-2.3.0rc1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/CHANGELOG.md` & `skillsnetwork_jupyter_extension-2.3.0rc1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
-## 2.3.0rc0
+## 2.3.0rc1
 
 No merged PRs
 
 <!-- <END NEW CHANGELOG ENTRY> -->
 
+## 2.3.0rc0
+
+No merged PRs
+
 ## 2.2.0
 
 ([Full Changelog](https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/compare/v2.1.0...6ecc041eaf538ff525cd250c17eed9a45350b4f6))
 
 ### Enhancements made
 
 - feat: add theme syncing and toggling [#21](https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/pull/21) ([@ElioDiNino](https://github.com/ElioDiNino))
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/CODEOWNERS` & `skillsnetwork_jupyter_extension-2.3.0rc1/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/RELEASE.md` & `skillsnetwork_jupyter_extension-2.3.0rc1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/package.json` & `skillsnetwork_jupyter_extension-2.3.0rc1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'2.3.0-rc1'"}*

```diff
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.3.0-rc0"
+    "version": "2.3.0-rc1"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/tsconfig.json` & `skillsnetwork_jupyter_extension-2.3.0rc1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/yarn.lock` & `skillsnetwork_jupyter_extension-2.3.0rc1/yarn.lock`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/schema/toolbar.json` & `skillsnetwork_jupyter_extension-2.3.0rc1/schema/toolbar.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/__init__.py` & `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/handlers.py` & `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/package.json` & `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.1114a7d16c81f17285d7.js'}}",*

 * * "'version'": "'2.3.0-rc1'"}*

```diff
@@ -111,15 +111,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.deab4c15018528576b5d.js",
+            "load": "static/remoteEntry.1114a7d16c81f17285d7.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "skillsnetwork_jupyter_extension"
                 },
@@ -207,9 +207,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.3.0-rc0"
+    "version": "2.3.0-rc1"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig` & `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'2.3.0-rc1'"}*

```diff
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.3.0-rc0"
+    "version": "2.3.0-rc1"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json` & `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/496.9f74bf3e410d1c115cd7.js` & `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/496.6b8b1c179401632c8943.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -281,15 +281,15 @@
                         c: () => b
                     });
                     var a = o(452),
                         i = o(760),
                         r = o(300),
                         l = o(628),
                         s = o(736),
-                        c = o(568),
+                        c = o(188),
                         d = o(780),
                         u = o(904),
                         h = o(96),
                         g = o(416),
                         p = o.n(g),
                         w = e([u, h]);
                     [u, h] = w.then ? (await w)() : w;
@@ -422,15 +422,15 @@
         808: (e, t, o) => {
             o.a(e, (async (e, n) => {
                 try {
                     o.d(t, {
                         c: () => k
                     });
                     var a = o(736),
-                        i = o(568),
+                        i = o(188),
                         r = o(300),
                         l = o(96),
                         s = o(508),
                         c = o(480),
                         d = o(780),
                         u = o(904),
                         h = o(416),
@@ -640,31 +640,31 @@
                     const b = (e, t) => {
                             const o = [];
                             return e.content.widgets.forEach((e => {
                                 const t = d(e);
                                 o.push(t)
                             })), JSON.stringify(o, null, 2)
                         },
-                        m = async (e, t, o, n, a, i) => {
-                            let s, c, d, u;
+                        m = async (e, t, o, n, a, s) => {
+                            let c, d, u, g;
                             if ("NO_TOKEN" !== e)({
-                                instructions_file_path: s,
-                                body: c
-                            } = await (0, l.iU)((0, l.GK)(e))), d = s, u = e;
+                                instructions_file_path: c,
+                                body: d
+                            } = await (0, l.iU)((0, l.GK)(e))), u = c, g = e;
                             else {
                                 if ("NO_TOKEN" === t) throw Error("No valid token found.");
                                 ({
-                                    labFilename: d,
-                                    body: c
-                                } = await (0, l.uU)((0, l.CU)(t), t)), u = t
+                                    labFilename: u,
+                                    body: d
+                                } = await (0, l.uU)((0, l.CU)(t), t)), g = t
                             }
-                            let g = `${d}`;
-                            "" !== o ? (g = `${o}/${g}`, await h(n, g), i.model.path !== o && (console.log(`Opening /${o} in file browser`), await i.model.cd(`/${o}`))) : await i.model.cd("/");
-                            let p, w = g;
-                            return r.Ut !== r.mW.JUPYTERLITE ? (w = `./${g}`, await v(g, a, n), await _(w, c, a, n)) : await n.deleteFile(w), r.Gq.SHOW_PUBLISH_BUTTON_FOR = g, r.Gq.TOKENS.set(g, u), p = await L(w, a) ? n.openOrReveal(g) : await y(n, g, "NO_TOKEN" !== e ? JSON.parse(c) : c), p
+                            let p = `${u}`;
+                            p = i.C.join(o, p), p.includes("/") ? (await h(n, p), s.model.path !== o && (console.log(`Opening /${o} in file browser`), await s.model.cd(`/${o}`))) : await s.model.cd("/");
+                            let w, b = p;
+                            return r.Ut !== r.mW.JUPYTERLITE ? (b = `./${p}`, await v(p, a, n), await _(b, d, a, n)) : await n.deleteFile(b), r.Gq.SHOW_PUBLISH_BUTTON_FOR = p, r.Gq.TOKENS.set(p, g), w = await L(b, a) ? n.openOrReveal(p) : await y(n, p, "NO_TOKEN" !== e ? JSON.parse(d) : d), w
                         }, f = async (e, t, o, n, i) => {
                             const r = await (0, l.Oc)(e),
                                 s = r.data;
                             if (!S(s)) throw Error(`content of ${e} is not a valid JSON! Please let the author know about this issue!`);
                             const c = Date.parse(r.headers["last-modified"] || "");
                             if (console.log(`last-modified date of ${e} extracted from headers:`, c), !(t && t.endsWith(".ipynb") || (console.log(`filePath from query (which is ${t}) is either missing or doesn't end with .ipynb. Trying to use the pathname from ${e} as filePath...`), (t = decodeURI(new URL(e).pathname)).endsWith(".ipynb")))) throw Error(`pathname of ${e} (which is ${t}) doesn't end with .ipynb. A notebook can't be created.`);
                             console.log("filePath:", t), await h(o, t), console.log(`Opening ${t} in filebrowser`), await i.model.cd(t.substring(0, t.lastIndexOf("/")));
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js` & `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js` & `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/736.1176de539f275bcd21aa.js` & `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/736.1176de539f275bcd21aa.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js` & `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.deab4c15018528576b5d.js` & `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.1114a7d16c81f17285d7.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, b, v, m, y, g, w, _, k, j, S = {
+    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, b, v, m, y, g, w, _, k, j, S = {
             344: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(944), t.e(496)]).then((() => () => t(496))),
                         "./extension": () => Promise.all([t.e(944), t.e(496)]).then((() => () => t(496))),
                         "./style": () => t.e(736).then((() => () => t(355)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -37,20 +37,20 @@
         return S[e](t, t.exports, E), t.exports
     }
     E.m = S, E.c = x, e = "function" == typeof Symbol ? Symbol("webpack queues") : "__webpack_queues__", r = "function" == typeof Symbol ? Symbol("webpack exports") : "__webpack_exports__", t = "function" == typeof Symbol ? Symbol("webpack error") : "__webpack_error__", n = e => {
         e && e.d < 1 && (e.d = 1, e.forEach((e => e.r--)), e.forEach((e => e.r-- ? e.r++ : e())))
     }, E.a = (o, a, i) => {
         var u;
         i && ((u = []).d = -1);
-        var l, s, f, d = new Set,
-            c = o.exports,
-            p = new Promise(((e, r) => {
-                f = r, s = e
+        var l, f, s, d = new Set,
+            p = o.exports,
+            c = new Promise(((e, r) => {
+                s = r, f = e
             }));
-        p[r] = c, p[e] = e => (u && e(u), d.forEach(e), p.catch((e => {}))), o.exports = p, a((o => {
+        c[r] = p, c[e] = e => (u && e(u), d.forEach(e), c.catch((e => {}))), o.exports = c, a((o => {
             var a;
             l = (o => o.map((o => {
                 if (null !== o && "object" == typeof o) {
                     if (o[e]) return o;
                     if (o.then) {
                         var a = [];
                         a.d = 0, o.then((e => {
@@ -65,40 +65,40 @@
                 var u = {};
                 return u[e] = e => {}, u[r] = o, u
             })))(o);
             var i = () => l.map((e => {
                     if (e[t]) throw e[t];
                     return e[r]
                 })),
-                s = new Promise((r => {
+                f = new Promise((r => {
                     (a = () => r(i)).r = 0;
                     var t = e => e !== u && !d.has(e) && (d.add(e), e && !e.d && (a.r++, e.push(a)));
                     l.map((r => r[e](t)))
                 }));
-            return a.r ? s : i()
-        }), (e => (e ? f(p[t] = e) : s(c), n(u)))), u && u.d < 0 && (u.d = 0)
+            return a.r ? f : i()
+        }), (e => (e ? s(c[t] = e) : f(p), n(u)))), u && u.d < 0 && (u.d = 0)
     }, E.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return E.d(r, {
             a: r
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        496: "9f74bf3e410d1c115cd7",
+        496: "6b8b1c179401632c8943",
         636: "605077303a876f967661",
         648: "64f5e2269a630e211878",
         736: "1176de539f275bcd21aa",
         944: "dddd8170d5a83693b53a",
         956: "9f7a54c8b777ce434d6b"
     } [e] + ".js?v=" + {
-        496: "9f74bf3e410d1c115cd7",
+        496: "6b8b1c179401632c8943",
         636: "605077303a876f967661",
         648: "64f5e2269a630e211878",
         736: "1176de539f275bcd21aa",
         944: "dddd8170d5a83693b53a",
         956: "9f7a54c8b777ce434d6b"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
@@ -108,28 +108,28 @@
             if ("object" == typeof window) return window
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), o = {}, a = "skillsnetwork_jupyter_extension:", E.l = (e, r, t, n) => {
         if (o[e]) o[e].push(r);
         else {
             var i, u;
             if (void 0 !== t)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == e || f.getAttribute("data-webpack") == a + t) {
-                        i = f;
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var s = l[f];
+                    if (s.getAttribute("src") == e || s.getAttribute("data-webpack") == a + t) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", a + t), i.src = e), o[e] = [r];
             var d = (r, t) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var n = o[e];
                     if (delete o[e], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(t))), r) return r(t)
                 },
-                c = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -155,15 +155,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("axios", "1.6.7", (() => E.e(636).then((() => () => E(636))))), u("form-data", "4.0.0", (() => E.e(956).then((() => () => E(956))))), u("jwt-decode", "3.1.2", (() => E.e(648).then((() => () => E(648))))), u("skillsnetwork_jupyter_extension", "2.3.0-rc0", (() => Promise.all([E.e(944), E.e(496)]).then((() => () => E(496)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("axios", "1.6.7", (() => E.e(636).then((() => () => E(636))))), u("form-data", "4.0.0", (() => E.e(956).then((() => () => E(956))))), u("jwt-decode", "3.1.2", (() => E.e(648).then((() => () => E(648))))), u("skillsnetwork_jupyter_extension", "2.3.0-rc1", (() => Promise.all([E.e(944), E.e(496)]).then((() => () => E(496)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -206,85 +206,85 @@
             a.push(0 === i ? "not(" + u() + ")" : 1 === i ? "(" + u() + " || " + u() + ")" : 2 === i ? a.pop() + " " + a.pop() : l(i))
         }
         return u();
 
         function u() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, s = (e, r) => {
+    }, f = (e, r) => {
         if (0 in e) {
             r = i(r);
             var t = e[0],
                 n = t < 0;
             n && (t = -t - 1);
             for (var o = 0, a = 1, u = !0;; a++, o++) {
-                var l, f, d = a < e.length ? (typeof e[a])[0] : "";
-                if (o >= r.length || "o" == (f = (typeof(l = r[o]))[0])) return !u || ("u" == d ? a > t && !n : "" == d != n);
-                if ("u" == f) {
+                var l, s, d = a < e.length ? (typeof e[a])[0] : "";
+                if (o >= r.length || "o" == (s = (typeof(l = r[o]))[0])) return !u || ("u" == d ? a > t && !n : "" == d != n);
+                if ("u" == s) {
                     if (!u || "u" != d) return !1
                 } else if (u)
-                    if (d == f)
+                    if (d == s)
                         if (a <= t) {
                             if (l != e[a]) return !1
                         } else {
                             if (n ? l > e[a] : l < e[a]) return !1;
                             l != e[a] && (u = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (n || a <= t) return !1;
                     u = !1, a--
                 } else {
-                    if (a <= t || f < d != n) return !1;
+                    if (a <= t || s < d != n) return !1;
                     u = !1
                 } else "s" != d && "n" != d && (u = !1, a--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (o = 1; o < e.length; o++) {
             var h = e[o];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? s(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? f(h, r) : !c())
         }
-        return !!p()
-    }, f = (e, r) => {
+        return !!c()
+    }, s = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && u(e, r) ? r : e), 0)
-    }, c = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + l(n) + ")", p = (e, r, t, n) => {
+    }, p = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + l(n) + ")", c = (e, r, t, n) => {
         var o = d(e, t);
-        return s(n, o) || b(c(e, t, o, n)), v(e[t][o])
+        return f(n, o) || b(p(e, t, o, n)), v(e[t][o])
     }, h = (e, r, t) => {
         var n = e[r];
-        return (r = Object.keys(n).reduce(((e, r) => !s(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
+        return (r = Object.keys(n).reduce(((e, r) => !f(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
     }, b = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, v = e => (e.loaded = 1, e.get()), y = (m = e => function(r, t, n, o) {
         var a = E.I(r);
         return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (f(e, t), p(r, 0, t, n)))), g = m(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (s(e, t), c(r, 0, t, n)))), g = m(((e, r, t, n, o) => {
         var a = r && E.o(r, t) && h(r, t, n);
         return a ? v(a) : o()
     })), w = {}, _ = {
+        188: () => y("default", "@jupyterlab/filebrowser", [1, 4, 1, 8]),
         300: () => y("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
         416: () => g("default", "jwt-decode", [1, 3, 1, 2], (() => E.e(648).then((() => () => E(648))))),
         420: () => y("default", "@jupyterlab/services", [1, 7, 1, 8]),
         452: () => y("default", "@jupyterlab/mainmenu", [1, 4, 1, 8]),
         468: () => y("default", "@jupyterlab/coreutils", [1, 6, 1, 8]),
         500: () => g("default", "axios", [1, 1, 6, 0], (() => E.e(636).then((() => () => E(636))))),
         508: () => y("default", "@lumino/disposable", [1, 2, 0, 0]),
-        568: () => y("default", "@jupyterlab/filebrowser", [1, 4, 1, 8]),
         628: () => y("default", "@jupyterlab/notebook", [1, 4, 1, 8]),
         637: () => g("default", "form-data", [1, 4, 0, 0], (() => E.e(956).then((() => () => E(956))))),
         736: () => y("default", "@jupyterlab/docmanager", [1, 4, 1, 8]),
         760: () => y("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0])
     }, k = {
-        496: [300, 416, 420, 452, 468, 500, 508, 568, 628, 637, 736, 760]
+        496: [188, 300, 416, 420, 452, 468, 500, 508, 628, 637, 736, 760]
     }, j = {}, E.f.consumes = (e, r) => {
         E.o(k, e) && k[e].forEach((e => {
             if (E.o(w, e)) return r.push(w[e]);
             if (!j[e]) {
                 var t = r => {
                     w[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json` & `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/src/config.ts` & `skillsnetwork_jupyter_extension-2.3.0rc1/src/config.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/src/dialog.ts` & `skillsnetwork_jupyter_extension-2.3.0rc1/src/dialog.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/src/handler.ts` & `skillsnetwork_jupyter_extension-2.3.0rc1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/src/sn-file-library.ts` & `skillsnetwork_jupyter_extension-2.3.0rc1/src/sn-file-library.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/src/tools.ts` & `skillsnetwork_jupyter_extension-2.3.0rc1/src/tools.ts`

 * *Files 2% similar despite different names*

```diff
@@ -308,17 +308,18 @@
     ));
     token = awb_token;
   } else {
     throw Error('No valid token found.');
   }
 
   let filePath = `${labFilename}`;
+  filePath = PathExt.join(dirPath, filePath);
 
-  if (dirPath !== '') {
-    filePath = `${dirPath}/${filePath}`;
+  // This allows both the dirPath and lab filename to include a path to create subfolders
+  if (filePath.includes('/')) {
     await ensureSubFoldersExist(docManager, filePath);
 
     if (fileBrowser.model.path !== dirPath) {
       console.log(`Opening /${dirPath} in file browser`);
       await fileBrowser.model.cd(`/${dirPath}`);
     }
   } else {
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/src/menu/index.ts` & `skillsnetwork_jupyter_extension-2.3.0rc1/src/menu/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/src/theme/index.ts` & `skillsnetwork_jupyter_extension-2.3.0rc1/src/theme/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/src/toolbar/index.ts` & `skillsnetwork_jupyter_extension-2.3.0rc1/src/toolbar/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/static/extension_demo.gif` & `skillsnetwork_jupyter_extension-2.3.0rc1/static/extension_demo.gif`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/.gitignore` & `skillsnetwork_jupyter_extension-2.3.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/LICENSE` & `skillsnetwork_jupyter_extension-2.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/README.md` & `skillsnetwork_jupyter_extension-2.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/pyproject.toml` & `skillsnetwork_jupyter_extension-2.3.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc0/PKG-INFO` & `skillsnetwork_jupyter_extension-2.3.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: skillsnetwork_jupyter_extension
-Version: 2.3.0rc0
+Version: 2.3.0rc1
 Dynamic: Keywords
 Summary: JupterLab/JupyerLite extension for Skills Network Labs
 Project-URL: Homepage, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension
 Project-URL: Bug Tracker, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/issues
 Project-URL: Repository, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension.git
 Author-email: IBM Skills Network <skills.network@ibm.com>
 License:                                  Apache License
```

