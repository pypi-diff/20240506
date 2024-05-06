# Comparing `tmp/infrable-0.1.0.tar.gz` & `tmp/infrable-0.1.1.tar.gz`

## Comparing `infrable-0.1.0.tar` & `infrable-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.0/.envrc
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/errors.py
--rw-r--r--   0        0        0     9900 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/files.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/host.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/infra.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/init.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/meta.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/paths.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/readfile.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/service.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/switch.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/template.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/cli/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/cli/files.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/cli/main.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/cli/remote.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/cli/switch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/distro/__init__.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/distro/linux.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/distro/ubuntu.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.0/LICENSE
--rw-r--r--   0        0        0    17714 2020-02-02 00:00:00.000000 infrable-0.1.0/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    31540 2020-02-02 00:00:00.000000 infrable-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.1/.envrc
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/__init__.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/errors.py
+-rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/files.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/host.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/infra.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/init.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/meta.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/paths.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/readfile.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/service.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/switch.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/template.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/cli/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/cli/files.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/cli/main.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/cli/remote.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/cli/switch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/distro/__init__.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/distro/linux.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/distro/ubuntu.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.1/LICENSE
+-rw-r--r--   0        0        0    17862 2020-02-02 00:00:00.000000 infrable-0.1.1/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    31688 2020-02-02 00:00:00.000000 infrable-0.1.1/PKG-INFO
```

### Comparing `infrable-0.1.0/infrable/errors.py` & `infrable-0.1.1/infrable/errors.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/infrable/files.py` & `infrable-0.1.1/infrable/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     hosts = {}
     for new in paths.files.glob("**/*.new"):
         old = _old_path(new)
         if not _diff(new=new, old=old):
             continue
         remote, _ = str(new.relative_to(paths.files)).removesuffix(".new").split("/", 1)
-        _, host = remote.split("@", 1)
+        host = remote.split("@", 1)[-1]
         if only and host not in only_hosts:
             continue
         if host not in hosts:
             hosts[host] = infra.get_host(host)
     return list(hosts.values())
 
 
@@ -66,20 +66,20 @@
             if i + 1 == len(meta.dest):
                 print("╰─ ", end="")
             else:
                 print("├─ ", end="")
 
             # Render the template for each destination
 
-            login, loc = dest.loc.split(":", 1)
-            _, host = login.split("@", 1)
+            remote, loc = dest.loc.split(":", 1)
+            host = remote.split("@", 1)[-1]
             if not host or host == "None" or (only and host not in only_hosts):
                 print(f"skipping {dest.loc}")
                 continue
-            outpath = paths.files / login / (loc.removeprefix("/") + ".new")
+            outpath = paths.files / remote / (loc.removeprefix("/") + ".new")
             outpath.parent.mkdir(exist_ok=True, parents=True)
             rendered = render(src, dest_loc=dest.loc, **infra.items, **dest.ctx)
             outpath.write_text(rendered)
             print(outpath)
         print()
```

### Comparing `infrable-0.1.0/infrable/host.py` & `infrable-0.1.1/infrable/host.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/infrable/infra.py` & `infrable-0.1.1/infrable/infra.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/infrable/init.py` & `infrable-0.1.1/infrable/init.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/infrable/readfile.py` & `infrable-0.1.1/infrable/readfile.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/infrable/service.py` & `infrable-0.1.1/infrable/service.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/infrable/switch.py` & `infrable-0.1.1/infrable/switch.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/infrable/template.py` & `infrable-0.1.1/infrable/template.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/infrable/util.py` & `infrable-0.1.1/infrable/util.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/infrable/cli/files.py` & `infrable-0.1.1/infrable/cli/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/infrable/cli/main.py` & `infrable-0.1.1/infrable/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import sys
 
 import typer
 
-from infrable import errors, infra, init
+from infrable import __version__, errors, infra, init
 from infrable.cli import files, remote, switch
 
 app = typer.Typer(no_args_is_help=True)
 
 
 @app.command()
+def version():
+    """Print the version."""
+    print(f"infrable {__version__}")
+
+
+@app.command()
 def hosts(format: str | None = None, repr: bool = False):
     """List all hosts in the infrastructure."""
 
     for name, host in infra.hosts.items():
         if format:
             print(host.format(name, format=format))
         elif repr:
```

### Comparing `infrable-0.1.0/infrable/cli/remote.py` & `infrable-0.1.1/infrable/cli/remote.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/infrable/distro/linux.py` & `infrable-0.1.1/infrable/distro/linux.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/infrable/distro/ubuntu.py` & `infrable-0.1.1/infrable/distro/ubuntu.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/.gitignore` & `infrable-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/LICENSE` & `infrable-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/README.md` & `infrable-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Infrable
 
 Hanny's legendary infrastructure as code solution.
 
-[![PyPI version](https://img.shields.io/pypi/v/expandvars.svg)](https://pypi.org/project/expandvars)
+[![PyPI version](https://img.shields.io/pypi/v/infrable.svg)](https://pypi.org/project/infrable)
 
 ```bash
 # Install
 pip install -U infrable  # requires python >= 3.10
 
 # Bootstrap a new project
 touch infra.py
@@ -259,16 +259,19 @@
 @dev_nginx.typer.command(name="reload")
 def reload_dev_nginx():
     """[TASK] Reload nginx: infrable dev-nginx reload"""
 
     assert dev_nginx.host, "Service must have a host to reload"
     dev_nginx.host.remote().sudo.nginx("-t")
     dev_nginx.host.remote().sudo.systemctl.reload.nginx()
+# /Tasks -----------------------------------------------------------------------
 ```
 
+Running tasks:
+
 ```bash
 infrable dev-nginx reload
 ```
 
 As she toiled to realize this vision, a brilliant idea swept over her - to
 orchestrate these tasks into coherent sequences, she christened them
 **"workflows"**, heralding the dawn of a new era in infrastructure management.
@@ -290,14 +293,16 @@
     cmd = "sudo nginx -t && sudo systemctl reload nginx && echo success || echo failed"
     tasks = [lambda: (h, h.remote().sudo(cmd)) for h in hosts]
     for host, result in parallel(tasks):
         print(f"{host}: {result}")
 # /Workflows -----------------------------------------------------------------------
 ```
 
+Running workflows:
+
 ```bash
 infrable deploy dev-nginx
 ```
 
 ## Chapter 6 - Environments and Switches
 
 The exhilaration of progress was swiftly countered by the rigors of defining **templates,
@@ -501,10 +506,12 @@
 cloud = mycloud.MyCloud(secret_api_key=readfile("secrets/mycloud/secret_api_key"))
 
 cloud.typer = typer.Typer(help="MyCloud specific workflows.")
 cloud.typer.add_typer(mycloud.workflows, name="mycloud")
 # /Clouds ----------------------------------------------------------------------
 ```
 
-```
+Running the module workflows:
+
+```bash
 infra cloud --help
 ```
```

### Comparing `infrable-0.1.0/pyproject.toml` & `infrable-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `infrable-0.1.0/PKG-INFO` & `infrable-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: infrable
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hanny's legendary infrastructure as code solution.
 Project-URL: Homepage, https://github.com/stckme/infrable
 Author-email: Arijit Basu <sayanarijit@gmail.com>
 Maintainer-email: Arijit Basu <sayanarijit@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -226,15 +226,15 @@
 Requires-Dist: twine; extra == 'devel'
 Description-Content-Type: text/markdown
 
 # Infrable
 
 Hanny's legendary infrastructure as code solution.
 
-[![PyPI version](https://img.shields.io/pypi/v/expandvars.svg)](https://pypi.org/project/expandvars)
+[![PyPI version](https://img.shields.io/pypi/v/infrable.svg)](https://pypi.org/project/infrable)
 
 ```bash
 # Install
 pip install -U infrable  # requires python >= 3.10
 
 # Bootstrap a new project
 touch infra.py
@@ -487,16 +487,19 @@
 @dev_nginx.typer.command(name="reload")
 def reload_dev_nginx():
     """[TASK] Reload nginx: infrable dev-nginx reload"""
 
     assert dev_nginx.host, "Service must have a host to reload"
     dev_nginx.host.remote().sudo.nginx("-t")
     dev_nginx.host.remote().sudo.systemctl.reload.nginx()
+# /Tasks -----------------------------------------------------------------------
 ```
 
+Running tasks:
+
 ```bash
 infrable dev-nginx reload
 ```
 
 As she toiled to realize this vision, a brilliant idea swept over her - to
 orchestrate these tasks into coherent sequences, she christened them
 **"workflows"**, heralding the dawn of a new era in infrastructure management.
@@ -518,14 +521,16 @@
     cmd = "sudo nginx -t && sudo systemctl reload nginx && echo success || echo failed"
     tasks = [lambda: (h, h.remote().sudo(cmd)) for h in hosts]
     for host, result in parallel(tasks):
         print(f"{host}: {result}")
 # /Workflows -----------------------------------------------------------------------
 ```
 
+Running workflows:
+
 ```bash
 infrable deploy dev-nginx
 ```
 
 ## Chapter 6 - Environments and Switches
 
 The exhilaration of progress was swiftly countered by the rigors of defining **templates,
@@ -729,10 +734,12 @@
 cloud = mycloud.MyCloud(secret_api_key=readfile("secrets/mycloud/secret_api_key"))
 
 cloud.typer = typer.Typer(help="MyCloud specific workflows.")
 cloud.typer.add_typer(mycloud.workflows, name="mycloud")
 # /Clouds ----------------------------------------------------------------------
 ```
 
-```
+Running the module workflows:
+
+```bash
 infra cloud --help
 ```
```

