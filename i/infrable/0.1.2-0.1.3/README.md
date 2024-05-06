# Comparing `tmp/infrable-0.1.2.tar.gz` & `tmp/infrable-0.1.3.tar.gz`

## Comparing `infrable-0.1.2.tar` & `infrable-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.2/.envrc
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/__init__.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/errors.py
--rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/files.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/host.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/infra.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/init.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/meta.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/paths.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/readfile.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/service.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/switch.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/template.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/cli/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/cli/files.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/cli/main.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/cli/remote.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/cli/switch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/distro/__init__.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/distro/linux.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/distro/ubuntu.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.2/LICENSE
--rw-r--r--   0        0        0    17862 2020-02-02 00:00:00.000000 infrable-0.1.2/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    31688 2020-02-02 00:00:00.000000 infrable-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.3/.envrc
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/__init__.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/errors.py
+-rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/files.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/host.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/infra.py
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/init.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/meta.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/paths.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/readfile.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/service.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/switch.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/template.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/cli/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/cli/files.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/cli/main.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/cli/remote.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/cli/switch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/distro/__init__.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/distro/linux.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.3/infrable/distro/ubuntu.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.3/LICENSE
+-rw-r--r--   0        0        0    17868 2020-02-02 00:00:00.000000 infrable-0.1.3/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    31694 2020-02-02 00:00:00.000000 infrable-0.1.3/PKG-INFO
```

### Comparing `infrable-0.1.2/infrable/errors.py` & `infrable-0.1.3/infrable/errors.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/files.py` & `infrable-0.1.3/infrable/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/host.py` & `infrable-0.1.3/infrable/host.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/infra.py` & `infrable-0.1.3/infrable/infra.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/init.py` & `infrable-0.1.3/infrable/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     prod=[prod_host],
 )
 # /Hosts -----------------------------------------------------------------------
 
 
 # Services/ --------------------------------------------------------------------
 web = Service(
-    host=env(dev=dev_host, beta=beta_host, prod=prod_host),
+    host=env.strict(dev=dev_host, beta=beta_host, prod=prod_host),
     meta=Meta(secret_key=readfile("secrets/web/secret_key")),
     port=8080,
 )
 
 nginx = Service(port=80, host=web.host)
 # /Services --------------------------------------------------------------------
```

### Comparing `infrable-0.1.2/infrable/readfile.py` & `infrable-0.1.3/infrable/readfile.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/service.py` & `infrable-0.1.3/infrable/service.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/switch.py` & `infrable-0.1.3/infrable/switch.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/template.py` & `infrable-0.1.3/infrable/template.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/util.py` & `infrable-0.1.3/infrable/util.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/cli/files.py` & `infrable-0.1.3/infrable/cli/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/cli/main.py` & `infrable-0.1.3/infrable/cli/main.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/cli/remote.py` & `infrable-0.1.3/infrable/cli/remote.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/distro/linux.py` & `infrable-0.1.3/infrable/distro/linux.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/infrable/distro/ubuntu.py` & `infrable-0.1.3/infrable/distro/ubuntu.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/.gitignore` & `infrable-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/LICENSE` & `infrable-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/README.md` & `infrable-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
     beta=[beta_host],
     prod=[prod_host],
 )
 # /Hosts -----------------------------------------------------------------------
 
 # Services/ --------------------------------------------------------------------
 web = Service(
-    host=env(dev=dev_host, beta=beta_host, prod=prod_host),  # <-- Switching host
+    host=env.strict(dev=dev_host, beta=beta_host, prod=prod_host),  # <-- Strict switch
     port=8080,
 )
 
 nginx = Service(port=80, host=web.host)  # <-- No need to use switch here
 # /Services --------------------------------------------------------------------
 ```
```

### Comparing `infrable-0.1.2/pyproject.toml` & `infrable-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `infrable-0.1.2/PKG-INFO` & `infrable-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: infrable
-Version: 0.1.2
+Version: 0.1.3
 Summary: Hanny's legendary infrastructure as code solution.
 Project-URL: Homepage, https://github.com/stckme/infrable
 Author-email: Arijit Basu <sayanarijit@gmail.com>
 Maintainer-email: Arijit Basu <sayanarijit@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -574,15 +574,15 @@
     beta=[beta_host],
     prod=[prod_host],
 )
 # /Hosts -----------------------------------------------------------------------
 
 # Services/ --------------------------------------------------------------------
 web = Service(
-    host=env(dev=dev_host, beta=beta_host, prod=prod_host),  # <-- Switching host
+    host=env.strict(dev=dev_host, beta=beta_host, prod=prod_host),  # <-- Strict switch
     port=8080,
 )
 
 nginx = Service(port=80, host=web.host)  # <-- No need to use switch here
 # /Services --------------------------------------------------------------------
 ```
```

