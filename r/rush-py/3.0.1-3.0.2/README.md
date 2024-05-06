# Comparing `tmp/rush_py-3.0.1.tar.gz` & `tmp/rush_py-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rush_py-3.0.1.tar", max compression
+gzip compressed data, was "rush_py-3.0.2.tar", max compression
```

## Comparing `rush_py-3.0.1.tar` & `rush_py-3.0.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     9914 2024-04-14 07:42:20.019580 rush_py-3.0.1/README.md
--rw-r--r--   0        0        0     2718 2024-04-17 04:40:42.341556 rush_py-3.0.1/pyproject.toml
--rw-r--r--   0        0        0      481 2024-03-25 07:43:11.134075 rush_py-3.0.1/rush/__init__.py
--rw-r--r--   0        0        0     1569 2024-04-12 08:48:59.531260 rush_py-3.0.1/rush/async_utils.py
--rw-r--r--   0        0        0       23 2024-01-29 10:45:57.136914 rush_py-3.0.1/rush/data.py
--rw-r--r--   0        0        0     1326 2024-04-17 04:40:42.341556 rush_py-3.0.1/rush/doc.py
--rw-r--r--   0        0        0     7663 2024-04-16 06:00:37.048276 rush_py-3.0.1/rush/graphql_client/__init__.py
--rw-r--r--   0        0        0      267 2024-04-16 06:00:36.589255 rush_py-3.0.1/rush/graphql_client/argument.py
--rw-r--r--   0        0        0     1036 2024-04-16 06:00:36.599256 rush_py-3.0.1/rush/graphql_client/arguments.py
--rw-r--r--   0        0        0    12272 2024-04-17 02:47:58.375356 rush_py-3.0.1/rush/graphql_client/async_base_client.py
--rw-r--r--   0        0        0      620 2024-04-16 06:00:36.758263 rush_py-3.0.1/rush/graphql_client/base_model.py
--rw-r--r--   0        0        0      174 2024-04-16 06:00:36.547253 rush_py-3.0.1/rush/graphql_client/cancel_module_instance.py
--rw-r--r--   0        0        0    28860 2024-04-17 02:47:58.496361 rush_py-3.0.1/rush/graphql_client/client.py
--rw-r--r--   0        0        0      253 2024-02-28 07:01:47.459725 rush_py-3.0.1/rush/graphql_client/create_entity.py
--rw-r--r--   0        0        0      277 2024-02-28 07:01:47.461725 rush_py-3.0.1/rush/graphql_client/create_experiment.py
--rw-r--r--   0        0        0      259 2024-02-28 07:01:47.463725 rush_py-3.0.1/rush/graphql_client/create_project.py
--rw-r--r--   0        0        0      259 2024-02-28 07:01:47.467725 rush_py-3.0.1/rush/graphql_client/create_protein.py
--rw-r--r--   0        0        0      314 2024-02-28 07:01:47.465725 rush_py-3.0.1/rush/graphql_client/create_protein_conformer.py
--rw-r--r--   0        0        0      241 2024-02-28 07:01:47.566729 rush_py-3.0.1/rush/graphql_client/create_smol.py
--rw-r--r--   0        0        0      296 2024-02-28 07:01:47.564729 rush_py-3.0.1/rush/graphql_client/create_smol_conformer.py
--rw-r--r--   0        0        0      290 2024-02-28 07:01:47.568729 rush_py-3.0.1/rush/graphql_client/create_smol_tautomer.py
--rw-r--r--   0        0        0      271 2024-02-28 07:01:47.570730 rush_py-3.0.1/rush/graphql_client/create_structure.py
--rw-r--r--   0        0        0      341 2024-04-16 06:00:36.551254 rush_py-3.0.1/rush/graphql_client/delete_module_instance.py
--rw-r--r--   0        0        0      255 2024-04-16 06:00:36.554254 rush_py-3.0.1/rush/graphql_client/deploy.py
--rw-r--r--   0        0        0      510 2024-02-28 07:01:47.506727 rush_py-3.0.1/rush/graphql_client/entity.py
--rw-r--r--   0        0        0     1477 2024-04-17 04:40:42.341556 rush_py-3.0.1/rush/graphql_client/enums.py
--rw-r--r--   0        0        0     2411 2024-04-16 06:00:36.757263 rush_py-3.0.1/rush/graphql_client/exceptions.py
--rw-r--r--   0        0        0      679 2024-02-28 07:01:47.557729 rush_py-3.0.1/rush/graphql_client/experiment.py
--rw-r--r--   0        0        0     3769 2024-04-16 06:00:36.757263 rush_py-3.0.1/rush/graphql_client/fragments.py
--rw-r--r--   0        0        0     5332 2024-04-16 06:00:36.545253 rush_py-3.0.1/rush/graphql_client/input_types.py
--rw-r--r--   0        0        0      825 2024-04-16 06:00:36.607256 rush_py-3.0.1/rush/graphql_client/latest_modules.py
--rw-r--r--   0        0        0     2004 2024-04-17 02:47:58.096344 rush_py-3.0.1/rush/graphql_client/module_instance_details.py
--rw-r--r--   0        0        0     4300 2024-01-29 10:45:57.143915 rush_py-3.0.1/rush/graphql_client/module_instance_full.py
--rw-r--r--   0        0        0      354 2024-04-16 06:00:36.634257 rush_py-3.0.1/rush/graphql_client/module_instance_minimal.py
--rw-r--r--   0        0        0      403 2024-01-29 10:45:57.144914 rush_py-3.0.1/rush/graphql_client/module_instance_status.py
--rw-r--r--   0        0        0     3104 2024-04-17 02:47:58.134345 rush_py-3.0.1/rush/graphql_client/module_instances.py
--rw-r--r--   0        0        0     2804 2024-01-29 10:45:57.145915 rush_py-3.0.1/rush/graphql_client/module_instances_full.py
--rw-r--r--   0        0        0      686 2024-04-16 06:00:36.615257 rush_py-3.0.1/rush/graphql_client/modules.py
--rw-r--r--   0        0        0      160 2024-02-13 05:21:55.039019 rush_py-3.0.1/rush/graphql_client/object.py
--rw-r--r--   0        0        0      292 2024-04-16 06:00:36.640258 rush_py-3.0.1/rush/graphql_client/object_contents.py
--rw-r--r--   0        0        0      243 2024-04-16 06:00:36.637258 rush_py-3.0.1/rush/graphql_client/object_url.py
--rw-r--r--   0        0        0     2121 2024-02-28 07:01:47.518727 rush_py-3.0.1/rush/graphql_client/project.py
--rw-r--r--   0        0        0      604 2024-02-28 07:01:47.523728 rush_py-3.0.1/rush/graphql_client/protein.py
--rw-r--r--   0        0        0      687 2024-02-28 07:01:47.528728 rush_py-3.0.1/rush/graphql_client/protein_conformer.py
--rw-r--r--   0        0        0      234 2024-04-16 06:00:36.643258 rush_py-3.0.1/rush/graphql_client/retry.py
--rw-r--r--   0        0        0      340 2024-04-16 06:00:36.649258 rush_py-3.0.1/rush/graphql_client/run.py
--rw-r--r--   0        0        0      571 2024-02-28 07:01:47.533728 rush_py-3.0.1/rush/graphql_client/smol.py
--rw-r--r--   0        0        0      657 2024-02-28 07:01:47.537728 rush_py-3.0.1/rush/graphql_client/smol_conformer.py
--rw-r--r--   0        0        0      662 2024-02-28 07:01:47.543728 rush_py-3.0.1/rush/graphql_client/smol_tautomer.py
--rw-r--r--   0        0        0     1139 2024-02-28 07:01:47.551729 rush_py-3.0.1/rush/graphql_client/structure.py
--rw-r--r--   0        0        0      161 2024-04-16 06:00:36.651258 rush_py-3.0.1/rush/graphql_client/tag.py
--rw-r--r--   0        0        0      381 2024-04-16 06:00:36.655259 rush_py-3.0.1/rush/graphql_client/track_utilization.py
--rw-r--r--   0        0        0      165 2024-04-16 06:00:36.658259 rush_py-3.0.1/rush/graphql_client/untag.py
--rw-r--r--   0        0        0      414 2024-04-16 06:00:36.681260 rush_py-3.0.1/rush/graphql_client/update_module_instance.py
--rw-r--r--   0        0        0      328 2024-01-29 10:45:57.148915 rush_py-3.0.1/rush/graphql_client/upload.py
--rw-r--r--   0        0        0      321 2024-04-16 06:00:36.685260 rush_py-3.0.1/rush/graphql_client/upload_arg.py
--rw-r--r--   0        0        0      506 2024-04-16 06:00:36.691260 rush_py-3.0.1/rush/graphql_client/upload_object.py
--rw-r--r--   0        0        0     1226 2024-03-25 07:43:11.134075 rush_py-3.0.1/rush/legacy_types.py
--rw-r--r--   0        0        0     7403 2024-02-16 09:06:54.345722 rush_py-3.0.1/rush/local.py
--rw-r--r--   0        0        0     5733 2024-02-16 09:06:54.345722 rush_py-3.0.1/rush/protocols.py
--rw-r--r--   0        0        0    65355 2024-04-17 04:40:42.342556 rush_py-3.0.1/rush/provider.py
--rw-r--r--   0        0        0       98 2024-02-16 09:06:54.345722 rush_py-3.0.1/rush/tests/test_provider.py
--rw-r--r--   0        0        0     1070 2024-02-01 03:43:42.619708 rush_py-3.0.1/rush/tests/test_typedef.py
--rw-r--r--   0        0        0    10193 2024-04-12 08:48:59.536260 rush_py-3.0.1/rush/typedef.py
--rw-r--r--   0        0        0      747 2024-04-07 11:51:36.271482 rush_py-3.0.1/rush/types.py
--rw-r--r--   0        0        0    10796 1970-01-01 00:00:00.000000 rush_py-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     9914 2024-04-14 07:42:20.019580 rush_py-3.0.2/README.md
+-rw-r--r--   0        0        0     2769 2024-05-06 08:49:16.695069 rush_py-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0      481 2024-03-25 07:43:11.134075 rush_py-3.0.2/rush/__init__.py
+-rw-r--r--   0        0        0     1965 2024-04-25 04:28:44.728279 rush_py-3.0.2/rush/async_utils.py
+-rw-r--r--   0        0        0       23 2024-01-29 10:45:57.136914 rush_py-3.0.2/rush/data.py
+-rw-r--r--   0        0        0     1326 2024-04-17 04:40:42.341556 rush_py-3.0.2/rush/doc.py
+-rw-r--r--   0        0        0     7663 2024-04-16 06:00:37.048276 rush_py-3.0.2/rush/graphql_client/__init__.py
+-rw-r--r--   0        0        0      267 2024-04-16 06:00:36.589255 rush_py-3.0.2/rush/graphql_client/argument.py
+-rw-r--r--   0        0        0     1036 2024-04-16 06:00:36.599256 rush_py-3.0.2/rush/graphql_client/arguments.py
+-rw-r--r--   0        0        0    12272 2024-04-17 02:47:58.375356 rush_py-3.0.2/rush/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0      620 2024-04-16 06:00:36.758263 rush_py-3.0.2/rush/graphql_client/base_model.py
+-rw-r--r--   0        0        0      174 2024-04-16 06:00:36.547253 rush_py-3.0.2/rush/graphql_client/cancel_module_instance.py
+-rw-r--r--   0        0        0    28860 2024-04-17 02:47:58.496361 rush_py-3.0.2/rush/graphql_client/client.py
+-rw-r--r--   0        0        0      253 2024-02-28 07:01:47.459725 rush_py-3.0.2/rush/graphql_client/create_entity.py
+-rw-r--r--   0        0        0      277 2024-02-28 07:01:47.461725 rush_py-3.0.2/rush/graphql_client/create_experiment.py
+-rw-r--r--   0        0        0      259 2024-02-28 07:01:47.463725 rush_py-3.0.2/rush/graphql_client/create_project.py
+-rw-r--r--   0        0        0      259 2024-02-28 07:01:47.467725 rush_py-3.0.2/rush/graphql_client/create_protein.py
+-rw-r--r--   0        0        0      314 2024-02-28 07:01:47.465725 rush_py-3.0.2/rush/graphql_client/create_protein_conformer.py
+-rw-r--r--   0        0        0      241 2024-02-28 07:01:47.566729 rush_py-3.0.2/rush/graphql_client/create_smol.py
+-rw-r--r--   0        0        0      296 2024-02-28 07:01:47.564729 rush_py-3.0.2/rush/graphql_client/create_smol_conformer.py
+-rw-r--r--   0        0        0      290 2024-02-28 07:01:47.568729 rush_py-3.0.2/rush/graphql_client/create_smol_tautomer.py
+-rw-r--r--   0        0        0      271 2024-02-28 07:01:47.570730 rush_py-3.0.2/rush/graphql_client/create_structure.py
+-rw-r--r--   0        0        0      341 2024-04-16 06:00:36.551254 rush_py-3.0.2/rush/graphql_client/delete_module_instance.py
+-rw-r--r--   0        0        0      255 2024-04-16 06:00:36.554254 rush_py-3.0.2/rush/graphql_client/deploy.py
+-rw-r--r--   0        0        0      510 2024-02-28 07:01:47.506727 rush_py-3.0.2/rush/graphql_client/entity.py
+-rw-r--r--   0        0        0     1477 2024-04-17 04:40:42.341556 rush_py-3.0.2/rush/graphql_client/enums.py
+-rw-r--r--   0        0        0     2411 2024-04-16 06:00:36.757263 rush_py-3.0.2/rush/graphql_client/exceptions.py
+-rw-r--r--   0        0        0      679 2024-02-28 07:01:47.557729 rush_py-3.0.2/rush/graphql_client/experiment.py
+-rw-r--r--   0        0        0     3769 2024-04-16 06:00:36.757263 rush_py-3.0.2/rush/graphql_client/fragments.py
+-rw-r--r--   0        0        0     5332 2024-04-16 06:00:36.545253 rush_py-3.0.2/rush/graphql_client/input_types.py
+-rw-r--r--   0        0        0      825 2024-04-16 06:00:36.607256 rush_py-3.0.2/rush/graphql_client/latest_modules.py
+-rw-r--r--   0        0        0     2004 2024-04-17 02:47:58.096344 rush_py-3.0.2/rush/graphql_client/module_instance_details.py
+-rw-r--r--   0        0        0     4300 2024-01-29 10:45:57.143915 rush_py-3.0.2/rush/graphql_client/module_instance_full.py
+-rw-r--r--   0        0        0      354 2024-04-16 06:00:36.634257 rush_py-3.0.2/rush/graphql_client/module_instance_minimal.py
+-rw-r--r--   0        0        0      403 2024-01-29 10:45:57.144914 rush_py-3.0.2/rush/graphql_client/module_instance_status.py
+-rw-r--r--   0        0        0     3104 2024-04-17 02:47:58.134345 rush_py-3.0.2/rush/graphql_client/module_instances.py
+-rw-r--r--   0        0        0     2804 2024-01-29 10:45:57.145915 rush_py-3.0.2/rush/graphql_client/module_instances_full.py
+-rw-r--r--   0        0        0      686 2024-04-16 06:00:36.615257 rush_py-3.0.2/rush/graphql_client/modules.py
+-rw-r--r--   0        0        0      160 2024-02-13 05:21:55.039019 rush_py-3.0.2/rush/graphql_client/object.py
+-rw-r--r--   0        0        0      292 2024-04-16 06:00:36.640258 rush_py-3.0.2/rush/graphql_client/object_contents.py
+-rw-r--r--   0        0        0      243 2024-04-16 06:00:36.637258 rush_py-3.0.2/rush/graphql_client/object_url.py
+-rw-r--r--   0        0        0     2121 2024-02-28 07:01:47.518727 rush_py-3.0.2/rush/graphql_client/project.py
+-rw-r--r--   0        0        0      604 2024-02-28 07:01:47.523728 rush_py-3.0.2/rush/graphql_client/protein.py
+-rw-r--r--   0        0        0      687 2024-02-28 07:01:47.528728 rush_py-3.0.2/rush/graphql_client/protein_conformer.py
+-rw-r--r--   0        0        0      234 2024-04-16 06:00:36.643258 rush_py-3.0.2/rush/graphql_client/retry.py
+-rw-r--r--   0        0        0      340 2024-04-16 06:00:36.649258 rush_py-3.0.2/rush/graphql_client/run.py
+-rw-r--r--   0        0        0      571 2024-02-28 07:01:47.533728 rush_py-3.0.2/rush/graphql_client/smol.py
+-rw-r--r--   0        0        0      657 2024-02-28 07:01:47.537728 rush_py-3.0.2/rush/graphql_client/smol_conformer.py
+-rw-r--r--   0        0        0      662 2024-02-28 07:01:47.543728 rush_py-3.0.2/rush/graphql_client/smol_tautomer.py
+-rw-r--r--   0        0        0     1139 2024-02-28 07:01:47.551729 rush_py-3.0.2/rush/graphql_client/structure.py
+-rw-r--r--   0        0        0      161 2024-04-16 06:00:36.651258 rush_py-3.0.2/rush/graphql_client/tag.py
+-rw-r--r--   0        0        0      381 2024-04-16 06:00:36.655259 rush_py-3.0.2/rush/graphql_client/track_utilization.py
+-rw-r--r--   0        0        0      165 2024-04-16 06:00:36.658259 rush_py-3.0.2/rush/graphql_client/untag.py
+-rw-r--r--   0        0        0      414 2024-04-16 06:00:36.681260 rush_py-3.0.2/rush/graphql_client/update_module_instance.py
+-rw-r--r--   0        0        0      328 2024-01-29 10:45:57.148915 rush_py-3.0.2/rush/graphql_client/upload.py
+-rw-r--r--   0        0        0      321 2024-04-16 06:00:36.685260 rush_py-3.0.2/rush/graphql_client/upload_arg.py
+-rw-r--r--   0        0        0      506 2024-04-16 06:00:36.691260 rush_py-3.0.2/rush/graphql_client/upload_object.py
+-rw-r--r--   0        0        0     1226 2024-03-25 07:43:11.134075 rush_py-3.0.2/rush/legacy_types.py
+-rw-r--r--   0        0        0     7403 2024-02-16 09:06:54.345722 rush_py-3.0.2/rush/local.py
+-rw-r--r--   0        0        0     5733 2024-02-16 09:06:54.345722 rush_py-3.0.2/rush/protocols.py
+-rw-r--r--   0        0        0    66188 2024-05-06 07:32:38.957574 rush_py-3.0.2/rush/provider.py
+-rw-r--r--   0        0        0      300 2024-04-25 04:28:44.729279 rush_py-3.0.2/rush/tests/test_provider.py
+-rw-r--r--   0        0        0     1070 2024-02-01 03:43:42.619708 rush_py-3.0.2/rush/tests/test_typedef.py
+-rw-r--r--   0        0        0    10193 2024-04-12 08:48:59.536260 rush_py-3.0.2/rush/typedef.py
+-rw-r--r--   0        0        0      747 2024-04-07 11:51:36.271482 rush_py-3.0.2/rush/types.py
+-rw-r--r--   0        0        0    10796 1970-01-01 00:00:00.000000 rush_py-3.0.2/PKG-INFO
```

### Comparing `rush_py-3.0.1/README.md` & `rush_py-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/pyproject.toml` & `rush_py-3.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "rush-py"
-version = "3.0.1"
+version = "3.0.2"
 description = "Python SDK for interacting with the QDX Rush API and modules"
 authors = ["Ryan Swart <ryan.swart@qdx.co>", "Sean Laguna <sean.laguna@qdx.co>"]
 readme = "README.md"
-packages = [{include = "rush"}]
+packages = [{ include = "rush" }]
 documentation = "https://talo.github.io/rush-py"
 homepage = "https://rush.qdx.co"
 
 [tool.poetry.scripts]
 # rush = "rush.__main__:main"
 
 [tool.poetry.dependencies]
@@ -19,28 +19,28 @@
 typing-extensions = "^4.9.0"
 websockets = "^12"
 aiofiles = "^23.2.1"
 nest-asyncio = "^1.6.0"
 
 [tool.poetry.group.dev.dependencies]
 ariadne-codegen = "0.13.0"
-black = {extras = ["jupyter"], version = "~=23.9.1"}
+black = { extras = ["jupyter"], version = "~=23.9.1" }
 flake8 = "~=6.1.0"
 isort = "~=5.12.0"
 jupyter-contrib-nbextensions = "^0.7.0"
 jupyterlab = "^4.0.6"
 nbdev = "^2.3.12"
 notebook = "^7.0.7"
 parso = "^0.8.3"
-pdoc= "^14.4.0"
+pdoc = "^14.4.0"
 pip = "~=23.2.1"
 py3Dmol = "^2.0.4"
 pytest = "~=7.4.3"
 pytest-xdist = "~=3.3.1"
-qdx-py = "^0.6.2"
+qdx-py = ">0.6.2"
 pickleshare = "^0.7.5"
 jupyterlab-lsp = "^5.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
@@ -56,16 +56,28 @@
 profile = "black"
 
 [tool.pydocstyle]
 ignore = ["D202", "D105"]
 match = "(?!test_).*.py"
 
 [tool.pyright]
-exclude = ["**/node_modules", "**/__pycache__", "**/*venv*", "result", "setup.py"]
-ignore = ["**/node_modules", "**/__pycache__", "**/*venv*", "result", "setup.py"]
+exclude = [
+    "**/node_modules",
+    "**/__pycache__",
+    "**/*venv*",
+    "result",
+    "setup.py",
+]
+ignore = [
+    "**/node_modules",
+    "**/__pycache__",
+    "**/*venv*",
+    "result",
+    "setup.py",
+]
 reportIncompatibleMethodOverride = "none"
 reportIncompatibleVariableOverride = "none"
 reportMissingImports = true
 reportMissingTypeStubs = "none"
 reportUnknownMemberType = "none"
 reportUnknownVariableType = "none"
 typeCheckingMode = "strict"
```

### Comparing `rush_py-3.0.1/rush/async_utils.py` & `rush_py-3.0.2/rush/async_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 #!/usr/bin/env python3
 
 import asyncio
-from typing import Any, Coroutine, TypeVar
+from typing import Any, Coroutine, Literal, TypeVar, Union
 
 T = TypeVar("T")
 
 
 def start_background_loop(loop: asyncio.AbstractEventLoop):
     asyncio.set_event_loop(loop)
     loop.run_forever()
 
 
 LOOP = asyncio.new_event_loop()
 
+__hack_applied__ = {"_": False}
 
-def asyncio_run(coro: Coroutine[Any, Any, T]) -> T:
+
+def asyncio_run(coro: Coroutine[Any, Any, T], override: Union[Literal["task"], None] = None) -> T:
     """
     Runs the coroutine in an event loop running on a background thread,
     and blocks the current thread until it returns a result.
     This plays well with gevent, since it can yield on the Future result call.
 
     :param coro: A coroutine, typically an async method
     :param timeout: How many seconds we should wait for a result before raising an error
     """
+
     try:
         # FIXME: this is a hack to work around an annoying stall issue in Jupyter notebooks
         #        for some reason, run_coroutine_threadsafe hangs indefinitely when uploading files
         #        inside the jupyter notebook. nest_asyncio allows us to just use LOOP.run_until_complete
         __IPYTHON__  # noqa: F821
-        import nest_asyncio
+        if not __hack_applied__["_"]:
+            import nest_asyncio
+
+            nest_asyncio.apply()
+            __hack_applied__["app"] = True
+    except Exception:
+        pass
 
-        nest_asyncio.apply()
+    loop_running = False
+    try:
+        loop_running = asyncio.get_event_loop().is_running()
     except Exception:
         pass
 
+    if override == "task" and loop_running:
+        r: Any = asyncio.create_task(coro)
+        return r
+
     if LOOP.is_running():
         return asyncio.run_coroutine_threadsafe(coro, LOOP).result()
-    elif asyncio.get_event_loop().is_running():
+    elif loop_running:
         r = asyncio.run(coro)
         return r
     else:
         try:
             return LOOP.run_until_complete(coro)
         except RuntimeError:
             start_background_loop(LOOP)
             return asyncio.run_coroutine_threadsafe(coro, LOOP).result()
         except Exception as e:
-            print(e)
+            raise e
```

### Comparing `rush_py-3.0.1/rush/doc.py` & `rush_py-3.0.2/rush/doc.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/__init__.py` & `rush_py-3.0.2/rush/graphql_client/__init__.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/arguments.py` & `rush_py-3.0.2/rush/graphql_client/arguments.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/async_base_client.py` & `rush_py-3.0.2/rush/graphql_client/async_base_client.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/base_model.py` & `rush_py-3.0.2/rush/graphql_client/base_model.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/client.py` & `rush_py-3.0.2/rush/graphql_client/client.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/enums.py` & `rush_py-3.0.2/rush/graphql_client/enums.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/exceptions.py` & `rush_py-3.0.2/rush/graphql_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/experiment.py` & `rush_py-3.0.2/rush/graphql_client/experiment.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/fragments.py` & `rush_py-3.0.2/rush/graphql_client/fragments.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/input_types.py` & `rush_py-3.0.2/rush/graphql_client/input_types.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/latest_modules.py` & `rush_py-3.0.2/rush/graphql_client/latest_modules.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/module_instance_details.py` & `rush_py-3.0.2/rush/graphql_client/module_instance_details.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/module_instance_full.py` & `rush_py-3.0.2/rush/graphql_client/module_instance_full.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/module_instances.py` & `rush_py-3.0.2/rush/graphql_client/module_instances.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/module_instances_full.py` & `rush_py-3.0.2/rush/graphql_client/module_instances_full.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/modules.py` & `rush_py-3.0.2/rush/graphql_client/modules.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/project.py` & `rush_py-3.0.2/rush/graphql_client/project.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/protein.py` & `rush_py-3.0.2/rush/graphql_client/protein.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/protein_conformer.py` & `rush_py-3.0.2/rush/graphql_client/protein_conformer.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/smol.py` & `rush_py-3.0.2/rush/graphql_client/smol.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/smol_conformer.py` & `rush_py-3.0.2/rush/graphql_client/smol_conformer.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/smol_tautomer.py` & `rush_py-3.0.2/rush/graphql_client/smol_tautomer.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/graphql_client/structure.py` & `rush_py-3.0.2/rush/graphql_client/structure.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/legacy_types.py` & `rush_py-3.0.2/rush/legacy_types.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/local.py` & `rush_py-3.0.2/rush/local.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/protocols.py` & `rush_py-3.0.2/rush/protocols.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/provider.py` & `rush_py-3.0.2/rush/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,15 +412,15 @@
             page_vars.before = page_info_res.end_cursor
             result = await fn(
                 **page_vars.__dict__,
                 **variables,
             )
             page_info_res = result.page_info
             yield result or EmptyPage()
-            if len(result.edges) > 0:  # type: ignore
+            if len(result.edges) == 0:  # type: ignore
                 break
 
     async def argument(self, id: ArgId) -> ArgumentArgument:
         """
         Retrieve an argument from the database.
 
         :param id: The ID of the argument.
@@ -509,15 +509,15 @@
                 if filepath.exists() and not overwrite:
                     raise FileExistsError(f"File {filename} already exists in workspace")
 
         if filepath:
             if filepath.exists() and not overwrite:
                 raise FileExistsError(f"File {filename} already exists in workspace")
             if obj and isinstance(obj, ObjectContentsObjectPath):
-                json.dump(obj.contents, open(filepath, "w"))
+                json.dump(obj.contents, open(filepath, "w"), indent=2)
             elif obj:
                 with httpx.stream(method="get", url=obj.url) as r:
                     r.raise_for_status()
 
                     buf = ""
                     with open(filepath, "wb") as f:
                         if not decode:
@@ -593,15 +593,15 @@
         if filepath.exists() and filepath.stat().st_size > 0:
             with open(filepath, "r") as f:
                 modules = json.load(f)
             self.module_paths = modules
 
             # check against latest modules
 
-            asyncio_run(get_latest_modules(modules))
+            asyncio_run(get_latest_modules(modules), override="task")
             return modules
         else:
             raise FileNotFoundError("Lock file not found")
 
     def save_module_paths(self, modules: dict[str, str], filename: Path | None = None):
         """
         Lock all of the module versions to a file.
@@ -1204,14 +1204,16 @@
                         self.module_paths[name] = path
             self.save_module_paths(self.module_paths, self._config_dir / "rush.lock")
         else:
             paths = await self.get_latest_module_paths(names)
             self.module_paths = paths
             self.save_module_paths(self.module_paths, self._config_dir / "rush.lock")
 
+        await self.get_module_functions(names=names, tags=tags)
+
     async def delete_module_instance(self, id: ModuleInstanceId):
         """
         Delete a module instance with a given ID.
 
         :param id: The ID of the module instance to be deleted.
         :return: The ID of the deleted module instance.
         :raises RuntimeError: If the operation fails.
@@ -1299,14 +1301,16 @@
                                     self.status = module_instance.status
                                 if module_instance.status == ModuleInstanceStatus.RUNNING:
                                     if (
                                         module_instance.progress
                                         and module_instance.progress.n != self.progress.n
                                     ):
                                         print(f"Progress: {module_instance.progress}", end="\r")
+                                    else:
+                                        print("module running with no progress reported", end="\r")
                             await asyncio.sleep(5)
                         else:
                             raise e
                     else:
                         self.provider.logger.error(e.errors)
                         raise e
 
@@ -1392,14 +1396,23 @@
                                 if source:
                                     module_instance = await self.provider.module_instance(source)
                                     if module_instance.status != self.status:
                                         self.provider.logger.info(
                                             f"Argument {self.id} is now {module_instance.status}"
                                         )
                                         self.status = module_instance.status
+
+                                    if module_instance.status == ModuleInstanceStatus.RUNNING:
+                                        if (
+                                            module_instance.progress
+                                            and module_instance.progress.n != self.progress.n
+                                        ):
+                                            print(f"Progress: {module_instance.progress}", end="\r")
+                                        else:
+                                            print("module running with no progress reported", end="\r")
                                 await asyncio.sleep(1)
                     except GraphQLClientGraphQLMultiError as e:
                         if e.errors[0].message == "not found":
                             await asyncio.sleep(1)
                         else:
                             self.provider.logger.error(e.errors)
                             raise e
```

### Comparing `rush_py-3.0.1/rush/tests/test_typedef.py` & `rush_py-3.0.2/rush/tests/test_typedef.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/typedef.py` & `rush_py-3.0.2/rush/typedef.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/rush/types.py` & `rush_py-3.0.2/rush/types.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.1/PKG-INFO` & `rush_py-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rush-py
-Version: 3.0.1
+Version: 3.0.2
 Summary: Python SDK for interacting with the QDX Rush API and modules
 Home-page: https://rush.qdx.co
 Author: Ryan Swart
 Author-email: ryan.swart@qdx.co
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

