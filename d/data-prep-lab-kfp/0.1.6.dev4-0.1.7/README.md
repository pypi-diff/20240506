# Comparing `tmp/data_prep_lab_kfp-0.1.6.dev4.tar.gz` & `tmp/data_prep_lab_kfp-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_lab_kfp-0.1.6.dev4.tar", last modified: Mon May  6 20:15:46 2024, max compression
+gzip compressed data, was "data_prep_lab_kfp-0.1.7.tar", last modified: Mon May  6 12:19:57 2024, max compression
```

## Comparing `data_prep_lab_kfp-0.1.6.dev4.tar` & `data_prep_lab_kfp-0.1.7.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-05-06 20:15:46.745025 data_prep_lab_kfp-0.1.6.dev4/
--rw-r--r--   0 alexey     (501) staff       (20)     2453 2024-05-06 14:47:48.000000 data_prep_lab_kfp-0.1.6.dev4/Makefile
--rw-r--r--   0 alexey     (501) staff       (20)     2700 2024-05-06 20:15:46.744653 data_prep_lab_kfp-0.1.6.dev4/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)     1889 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/README.md
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-05-06 20:15:46.735780 data_prep_lab_kfp-0.1.6.dev4/doc/
--rw-r--r--   0 alexey     (501) staff       (20)      452 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/doc/kfp_support_library.md
--rw-r--r--   0 alexey     (501) staff       (20)     1215 2024-05-06 20:14:59.000000 data_prep_lab_kfp-0.1.6.dev4/pyproject.toml
--rw-r--r--   0 alexey     (501) staff       (20)       38 2024-05-06 20:15:46.745090 data_prep_lab_kfp-0.1.6.dev4/setup.cfg
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-05-06 20:15:46.734087 data_prep_lab_kfp-0.1.6.dev4/src/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-05-06 20:15:46.743544 data_prep_lab_kfp-0.1.6.dev4/src/data_prep_lab_kfp.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)     2700 2024-05-06 20:15:46.000000 data_prep_lab_kfp-0.1.6.dev4/src/data_prep_lab_kfp.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)     1142 2024-05-06 20:15:46.000000 data_prep_lab_kfp-0.1.6.dev4/src/data_prep_lab_kfp.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2024-05-06 20:15:46.000000 data_prep_lab_kfp-0.1.6.dev4/src/data_prep_lab_kfp.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)      164 2024-05-06 20:15:46.000000 data_prep_lab_kfp-0.1.6.dev4/src/data_prep_lab_kfp.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)       12 2024-05-06 20:15:46.000000 data_prep_lab_kfp-0.1.6.dev4/src/data_prep_lab_kfp.egg-info/top_level.txt
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-05-06 20:15:46.734381 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-05-06 20:15:46.737629 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/
--rw-r--r--   0 alexey     (501) staff       (20)      238 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/README.md
--rw-r--r--   0 alexey     (501) staff       (20)       67 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/__init__.py
--rw-r--r--   0 alexey     (501) staff       (20)    27165 2024-05-06 20:14:10.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/kuberay_apis.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-05-06 20:15:46.740319 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/
--rw-r--r--   0 alexey     (501) staff       (20)     1259 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/__init__.py
--rw-r--r--   0 alexey     (501) staff       (20)    11445 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/cluster.py
--rw-r--r--   0 alexey     (501) staff       (20)     5390 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/environmentvariables.py
--rw-r--r--   0 alexey     (501) staff       (20)     7528 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/headnode.py
--rw-r--r--   0 alexey     (501) staff       (20)     6367 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/jobsubmission.py
--rw-r--r--   0 alexey     (501) staff       (20)     7491 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/templates.py
--rw-r--r--   0 alexey     (501) staff       (20)    14921 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/volumes.py
--rw-r--r--   0 alexey     (501) staff       (20)     7884 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/workernode.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-05-06 20:15:46.740565 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/workflow_support/
--rw-r--r--   0 alexey     (501) staff       (20)     2698 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/workflow_support/README.md
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-05-06 20:15:46.740994 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/workflow_support/utils/
--rw-r--r--   0 alexey     (501) staff       (20)      192 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/workflow_support/utils/__init__.py
--rw-r--r--   0 alexey     (501) staff       (20)    28107 2024-05-06 19:30:58.000000 data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/workflow_support/utils/workflow_utils.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2024-05-06 20:15:46.742668 data_prep_lab_kfp-0.1.6.dev4/test/
--rw-r--r--   0 alexey     (501) staff       (20)    14416 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/test/api_params_test.py
--rw-r--r--   0 alexey     (501) staff       (20)     2319 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/test/configmaps.py
--rw-r--r--   0 alexey     (501) staff       (20)     9967 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/test/kuberay_api_test.py
--rw-r--r--   0 alexey     (501) staff       (20)     1401 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/test/pipeline_utils_test.py
--rw-r--r--   0 alexey     (501) staff       (20)     3154 2024-05-02 19:46:36.000000 data_prep_lab_kfp-0.1.6.dev4/test/ray_remote_jobs_test.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-06 12:19:57.133005 data_prep_lab_kfp-0.1.7/
+-rw-r--r--   0 eres      (1000) eres      (1000)     2109 2024-05-05 17:12:08.000000 data_prep_lab_kfp-0.1.7/Makefile
+-rw-r--r--   0 eres      (1000) eres      (1000)     2695 2024-05-06 12:19:57.133005 data_prep_lab_kfp-0.1.7/PKG-INFO
+-rw-r--r--   0 eres      (1000) eres      (1000)     1889 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/README.md
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-06 12:19:57.123005 data_prep_lab_kfp-0.1.7/doc/
+-rw-r--r--   0 eres      (1000) eres      (1000)      452 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/doc/kfp_support_library.md
+-rw-r--r--   0 eres      (1000) eres      (1000)     1210 2024-05-06 12:18:42.000000 data_prep_lab_kfp-0.1.7/pyproject.toml
+-rw-r--r--   0 eres      (1000) eres      (1000)       38 2024-05-06 12:19:57.133005 data_prep_lab_kfp-0.1.7/setup.cfg
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-06 12:19:57.113005 data_prep_lab_kfp-0.1.7/src/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-06 12:19:57.133005 data_prep_lab_kfp-0.1.7/src/data_prep_lab_kfp.egg-info/
+-rw-r--r--   0 eres      (1000) eres      (1000)     2695 2024-05-06 12:19:56.000000 data_prep_lab_kfp-0.1.7/src/data_prep_lab_kfp.egg-info/PKG-INFO
+-rw-r--r--   0 eres      (1000) eres      (1000)     1206 2024-05-06 12:19:57.000000 data_prep_lab_kfp-0.1.7/src/data_prep_lab_kfp.egg-info/SOURCES.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)        1 2024-05-06 12:19:56.000000 data_prep_lab_kfp-0.1.7/src/data_prep_lab_kfp.egg-info/dependency_links.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)      164 2024-05-06 12:19:56.000000 data_prep_lab_kfp-0.1.7/src/data_prep_lab_kfp.egg-info/requires.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)       12 2024-05-06 12:19:56.000000 data_prep_lab_kfp-0.1.7/src/data_prep_lab_kfp.egg-info/top_level.txt
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-06 12:19:57.113005 data_prep_lab_kfp-0.1.7/src/kfp_support/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-06 12:19:57.123005 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/
+-rw-r--r--   0 eres      (1000) eres      (1000)      238 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/README.md
+-rw-r--r--   0 eres      (1000) eres      (1000)       67 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    26996 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/kuberay_apis.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-06 12:19:57.123005 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/
+-rw-r--r--   0 eres      (1000) eres      (1000)     1259 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    11445 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/cluster.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     5390 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/environmentvariables.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7528 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/headnode.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     6367 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/jobsubmission.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7491 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/templates.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    14921 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/volumes.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7884 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/workernode.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-06 12:19:57.123005 data_prep_lab_kfp-0.1.7/src/kfp_support/workflow_support/
+-rw-r--r--   0 eres      (1000) eres      (1000)     2698 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/workflow_support/README.md
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-06 12:19:57.133005 data_prep_lab_kfp-0.1.7/src/kfp_support/workflow_support/utils/
+-rw-r--r--   0 eres      (1000) eres      (1000)      192 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/workflow_support/utils/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     3913 2024-05-06 02:18:35.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    29337 2024-05-06 06:02:51.000000 data_prep_lab_kfp-0.1.7/src/kfp_support/workflow_support/utils/workflow_utils.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-06 12:19:57.133005 data_prep_lab_kfp-0.1.7/test/
+-rw-r--r--   0 eres      (1000) eres      (1000)    14416 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/test/api_params_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     2319 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/test/configmaps.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     9967 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/test/kuberay_api_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     1401 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/test/pipeline_utils_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     3154 2024-05-01 23:13:01.000000 data_prep_lab_kfp-0.1.7/test/ray_remote_jobs_test.py
```

### Comparing `data_prep_lab_kfp-0.1.6.dev4/Makefile` & `data_prep_lab_kfp-0.1.7/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 # Define the root of the local git clone for the common rules to be able
 # know where they are running from.
 REPOROOT=../..
 include ${REPOROOT}/.make.versions
+include ${REPOROOT}/kfp/requirements.env
 
-
-IGNORE := $(shell bash -c "sed -n /=/p  ${REPOROOT}/kfp/requirements.env | sed 's/=/:=/' | sed 's/^/export /' > makeenv")
-
-include makeenv
 # Include the common rules.
 # Use "make help" to see them.
 include ../../.make.defaults
 
-PYTHON=python
-PIP=$(PYTHON) -m pip
 # Command to run pytest
-PYTEST=pytest -s
 PYTHON_VERSION=$(shell $(PYTHON) --version)
 VENV_ACTIVATE=venv/bin/activate
 
-DEPLOY_KUBEFLOW ?=0
+DEPLOY_KUBEFLOW ?= 0
 
 clean::
 	@# Help: Clean up the distribution build and the venv 
 	rm -r dist venv || true
 	rm -rf src/*egg-info || true
-	rm makeenv || true
 
 .check-env:: .check_python_version
 	@echo "Checks passed"
 
 update-toml:: .check-env
 	@# Help: Copy the Makefile distribution version into the pyproject.toml
 	sed -i.back 's/^version[ ]*=.*/version = "'${DPL_LIB_KFP_VERSION}'"/' pyproject.toml
@@ -44,23 +37,21 @@
 
 publish:: .check-env
 publish::
 	@# Help: Publish the wheel to testpypi
 	if [ -d "dist"]; then rm -r dist; fi
 	${PYTHON} -m pip install --upgrade build
 	${PYTHON} -m twine check dist/*
-	${PYTHON} -m twine upload --verbose  dist/*
+	${PYTHON} -m twine upload --verbose --non-interactive dist/*
 
 venv::	pyproject.toml .check-env
 	@# Help: Create the virtual environment using pyproject.toml 
-	sed -i.back "s/data-prep-lab-kfp==[0-9].*/data-prep-lab-kfp==${DPL_LIB_KFP_VERSION}/" ../kfp_ray_components/requirements.txt
 	rm -rf venv
 	$(PYTHON) -m venv venv
 	. ${VENV_ACTIVATE};     \
-        pip install -r ../kfp_ray_components/requirements.txt ;\
 	pip install -e .;		\
 	pip install ray==${RAY} \
 	pip install pytest pytest-cov 
 
 test:: 	venv
 	@# Help: Use the already-built virtual environment to run pytest on the test directory.
 	. ${VENV_ACTIVATE}; export PYTHONPATH=../src; cd test;  $(PYTEST) api_params_test.py;
```

### Comparing `data_prep_lab_kfp-0.1.6.dev4/PKG-INFO` & `data_prep_lab_kfp-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_prep_lab_kfp
-Version: 0.1.6.dev4
+Version: 0.1.7
 Summary: Data Preparation Laboratory Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kfp==1.8.22
 Requires-Dist: requests
```

### Comparing `data_prep_lab_kfp-0.1.6.dev4/README.md` & `data_prep_lab_kfp-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/pyproject.toml` & `data_prep_lab_kfp-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "data_prep_lab_kfp"
-version = "0.1.6.dev4"
+version = "0.1.7"
 requires-python = ">=3.10"
 description = "Data Preparation Laboratory Library. KFP support"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
     { name = "Alexey Roytman", email = "roytman@il.ibm.com" },
```

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/data_prep_lab_kfp.egg-info/PKG-INFO` & `data_prep_lab_kfp-0.1.7/src/data_prep_lab_kfp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_prep_lab_kfp
-Version: 0.1.6.dev4
+Version: 0.1.7
 Summary: Data Preparation Laboratory Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kfp==1.8.22
 Requires-Dist: requests
```

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/data_prep_lab_kfp.egg-info/SOURCES.txt` & `data_prep_lab_kfp-0.1.7/src/data_prep_lab_kfp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,13 +16,14 @@
 src/kfp_support/api_server_client/params/headnode.py
 src/kfp_support/api_server_client/params/jobsubmission.py
 src/kfp_support/api_server_client/params/templates.py
 src/kfp_support/api_server_client/params/volumes.py
 src/kfp_support/api_server_client/params/workernode.py
 src/kfp_support/workflow_support/README.md
 src/kfp_support/workflow_support/utils/__init__.py
+src/kfp_support/workflow_support/utils/pipelines_tests_utils.py
 src/kfp_support/workflow_support/utils/workflow_utils.py
 test/api_params_test.py
 test/configmaps.py
 test/kuberay_api_test.py
 test/pipeline_utils_test.py
 test/ray_remote_jobs_test.py
```

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/kuberay_apis.py` & `data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/kuberay_apis.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
 
 logger = get_logger(__name__)
 
 
 _headers = {"Content-Type": "application/json", "accept": "application/json"}
 
-CONNECT_TIMEOUT = 120
-READ_TIMEOUT = 120
+CONNECT_TIMEOUT = 50
+READ_TIMEOUT = 50
 TIMEOUT = (CONNECT_TIMEOUT, READ_TIMEOUT)
 
 
 class KubeRayAPIs:
     """
     This class implements KubeRay APIs based on the API server.
     To create a class, the following parameters are required:
@@ -253,28 +253,28 @@
             message - only returned if http return code is not equal to 200
             list of clusters
         """
         status = 200
         message = None
         # Execute HTTP request
         url = self.server_url + self.api_base + f"namespaces/{ns}/clusters"
-        #for i in range(self.http_retries):
-        try:
-            response = requests.get(url, headers=_headers, timeout=TIMEOUT)
-            if response.status_code // 100 == 2:
-                return response.status_code, None, clusters_decoder(response.json())
-            else:
-                logger.warning(f"Failed to list clusters in namespace {ns}, status : {response.status_code}")
-                status = response.status_code
-                message = response.json()["message"]
-        except Exception as e:
-            logger.warning(f"Failed to list clusters in namespace {ns}, exception : {e}")
-            status = 500
-            message = str(e)
-        #    time.sleep(1)
+        for i in range(self.http_retries):
+            try:
+                response = requests.get(url, headers=_headers, timeout=TIMEOUT)
+                if response.status_code // 100 == 2:
+                    return response.status_code, None, clusters_decoder(response.json())
+                else:
+                    logger.warning(f"Failed to list clusters in namespace {ns}, status : {response.status_code}")
+                    status = response.status_code
+                    message = response.json()["message"]
+            except Exception as e:
+                logger.warning(f"Failed to list clusters in namespace {ns}, exception : {e}")
+                status = 500
+                message = str(e)
+            time.sleep(1)
         return status, message, None
 
     def get_cluster(self, ns: str, name: str) -> tuple[int, str, Cluster]:
         """
         get cluster
         :param ns: namespace
         :param name: name of the cluster
@@ -441,24 +441,21 @@
         """
         status = 200
         message = None
         # Execute HTTP request
         url = self.server_url + self.api_base + f"namespaces/{ns}/jobsubmissions/{name}"
         for i in range(self.http_retries):
             try:
-                print(f"before job submission {time.time()}")
-                response = requests.post(url, json=job_request.to_dict(), headers=_headers)
-                print(f"after job submission {time.time()} status : {response.status_code} ")
-                print(f"response {response}")
+                response = requests.post(url, json=job_request.to_dict(), headers=_headers, timeout=TIMEOUT)
                 if response.status_code // 100 == 2:
                     return response.status_code, None, response.json()["submissionId"]
                 else:
                     logger.warning(
                         f"Failed to submit job to the cluster {name} in namespace {ns}, "
-                        f"status : {response.status_code} reason : {response.reason} "
+                        f"status : {response.status_code}"
                     )
                     status = response.status_code
                     message = response.json()["message"]
             except Exception as e:
                 logger.warning(f"Failed to submit job to the cluster {name} in namespace {ns}, exception : {e}")
                 status = 500
                 message = str(e)
```

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/__init__.py` & `data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/__init__.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/cluster.py` & `data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/cluster.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/environmentvariables.py` & `data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/environmentvariables.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/headnode.py` & `data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/headnode.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/jobsubmission.py` & `data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/jobsubmission.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/templates.py` & `data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/templates.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/volumes.py` & `data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/volumes.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/api_server_client/params/workernode.py` & `data_prep_lab_kfp-0.1.7/src/kfp_support/api_server_client/params/workernode.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/workflow_support/README.md` & `data_prep_lab_kfp-0.1.7/src/kfp_support/workflow_support/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/src/kfp_support/workflow_support/utils/workflow_utils.py` & `data_prep_lab_kfp-0.1.7/src/kfp_support/workflow_support/utils/workflow_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,14 +138,50 @@
 
     def __init__(self, host: str = "http://localhost:8080"):
         """
         Initialization
         :param host: host to connect to
         """
         self.kfp_client = Client(host=host)
+    
+    def upload_pipeline(
+        self,
+        pipeline_package_path: str = None,
+        pipeline_name: str = None,
+        description: str = None,
+    ) -> models.api_pipeline.ApiPipeline:
+        """
+        Uploads the pipeline
+        :param pipeline_package_path: Local path to the pipeline package.
+        :param pipeline_name: Optional. Name of the pipeline to be shown in the UI.
+        :param description: Optional. Description of the pipeline to be shown in the UI.
+        :return: Server response object containing pipleine id and other information.
+        """
+        try:
+            p = self.kfp_client.upload_pipeline(pipeline_package_path, pipeline_name, description)
+            logger.info("Pipeline uploaded")
+            return p
+        except Exception as e:
+            logger.warning(f"Exception uploading pipeline {e}")
+            return None
+
+    def delete_pipeline(self, pipeline_id):
+        """
+        Delete pipeline.
+
+        :param pipeline_id: id of the pipeline.
+        :return
+
+        Returns:
+          Object. If the method is called asynchronously, returns the request thread.
+
+        Raises:
+          kfp_server_api.ApiException: If pipeline is not found.
+        """
+        return self.kfp_client.delete_pipeline(pipeline_id)
 
     def start_pipeline(
             self,
             pipeline: models.api_pipeline.ApiPipeline,
             experiment: models.api_experiment.ApiExperiment,
             params: Optional[dict[str, Any]],
     ) -> str:
@@ -157,15 +193,15 @@
         :return: the id of the run object
         """
         job_name = pipeline.name + " " + datetime.datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
         try:
             run_id = self.kfp_client.run_pipeline(
                 experiment_id=experiment.id, job_name=job_name, pipeline_id=pipeline.id, params=params
             )
-            logger.info("Pipeline submitted")
+            logger.info(f"Pipeline run {job_name} submitted")
             return run_id.id
         except Exception as e:
             logger.warning(f"Exception starting pipeline {e}")
             return None
 
     def get_experiment_by_name(self, name: str = "Default") -> models.api_experiment.ApiExperiment:
         """
@@ -474,15 +510,14 @@
             message - only returned if http return code is not equal to 200
             submission id - submission id
         """
         # Build job request
         job_request = RayJobRequest(entrypoint=KFPUtils.dict_to_req(d=request, executor=executor))
         if runtime_env is not None:
             job_request.runtime_env = runtime_env
-        print(f" before calling api_server_client.submit_job {time.time()}")
         return self.api_server_client.submit_job(ns=namespace, name=name, job_request=job_request)
 
     def _get_job_status(self, name: str, namespace: str, submission_id: str) -> tuple[int, str, str]:
         """
         Get job status
         :param name: cluster name
         :param namespace: cluster namespace
@@ -594,15 +629,15 @@
     Class containing methods supporting building pipelines
     """
 
     @staticmethod
     def add_settings_to_component(
             component: dsl.ContainerOp,
             timeout: int,
-            image_pull_policy: str = "Always",
+            image_pull_policy: str = "IfNotPresent",
             cache_strategy: str = "P0D",
     ) -> None:
         """
         Add settings to kfp component
         :param component: kfp component
         :param timeout: timeout to set to the component in seconds
         :param image_pull_policy: pull policy to set to the component
```

### Comparing `data_prep_lab_kfp-0.1.6.dev4/test/api_params_test.py` & `data_prep_lab_kfp-0.1.7/test/api_params_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/test/configmaps.py` & `data_prep_lab_kfp-0.1.7/test/configmaps.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/test/kuberay_api_test.py` & `data_prep_lab_kfp-0.1.7/test/kuberay_api_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/test/pipeline_utils_test.py` & `data_prep_lab_kfp-0.1.7/test/pipeline_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.6.dev4/test/ray_remote_jobs_test.py` & `data_prep_lab_kfp-0.1.7/test/ray_remote_jobs_test.py`

 * *Files identical despite different names*

