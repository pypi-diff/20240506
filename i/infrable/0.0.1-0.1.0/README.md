# Comparing `tmp/infrable-0.0.1.tar.gz` & `tmp/infrable-0.1.0.tar.gz`

## Comparing `infrable-0.0.1.tar` & `infrable-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.0.1/.envrc
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 infrable-0.0.1/.null-ls_882832_README.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/errors.py
--rw-r--r--   0        0        0     9900 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/files.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/host.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/infra.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/init.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/meta.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/paths.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/readfile.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/service.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/switch.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/template.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/cli/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/cli/files.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/cli/main.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/cli/remote.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/cli/switch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/distro/__init__.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/distro/linux.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.0.1/infrable/distro/ubuntu.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 infrable-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.0.1/LICENSE
--rw-r--r--   0        0        0    10060 2020-02-02 00:00:00.000000 infrable-0.0.1/README.md
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 infrable-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    23847 2020-02-02 00:00:00.000000 infrable-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.0/.envrc
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/__init__.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/errors.py
+-rw-r--r--   0        0        0     9900 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/files.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/host.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/infra.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/init.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/meta.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/paths.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/readfile.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/service.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/switch.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/template.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/cli/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/cli/files.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/cli/main.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/cli/remote.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/cli/switch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/distro/__init__.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/distro/linux.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.0/infrable/distro/ubuntu.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.0/LICENSE
+-rw-r--r--   0        0        0    17714 2020-02-02 00:00:00.000000 infrable-0.1.0/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    31540 2020-02-02 00:00:00.000000 infrable-0.1.0/PKG-INFO
```

### Comparing `infrable-0.0.1/infrable/errors.py` & `infrable-0.1.0/infrable/errors.py`

 * *Files identical despite different names*

### Comparing `infrable-0.0.1/infrable/files.py` & `infrable-0.1.0/infrable/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.0.1/infrable/host.py` & `infrable-0.1.0/infrable/host.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import asdict, dataclass, field
 
 from sh import Command, ssh
 from typer import Typer
 
 from infrable.meta import Meta
-from infrable.util import template
+from infrable.util import formatter
 
 
 @dataclass(unsafe_hash=True, order=True, eq=True)
 class Host:
     """A generic host in the infrastructure."""
 
     ip: str  # The only required field
@@ -20,12 +20,12 @@
 
     def remote(self, login=None) -> Command:
         login = login or self.admin
         address = f"{login}@{self.ip}"
         return ssh.bake(address, "-o", "StrictHostKeyChecking=no")
 
     def format(self, name: str, format) -> str:
-        return template(format).render(name=name, **asdict(self))
+        return formatter(format).render(name=name, **asdict(self))
 
     def __str__(self) -> str:
         host = self.fqdn or self.ip
         return f"{self.admin}@{host}"
```

### Comparing `infrable-0.0.1/infrable/infra.py` & `infrable-0.1.0/infrable/infra.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,14 +72,18 @@
             continue
         elif isinstance(item, Typer):
             typers[name] = item
             continue
         elif isinstance(item, list) and item and isinstance(item[0], Host):
             host_groups[name] = item
             continue
+        elif t := getattr(item, "typer", None):
+            if isinstance(t, Typer):
+                typers[name] = t
+            continue
         else:
             continue
 
 
 def get_host(name: str) -> Host | None:
     """Get a host by name, FQDN, IP or service name."""
```

### Comparing `infrable-0.0.1/infrable/readfile.py` & `infrable-0.1.0/infrable/readfile.py`

 * *Files identical despite different names*

### Comparing `infrable-0.0.1/infrable/service.py` & `infrable-0.1.0/infrable/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from dataclasses import asdict, dataclass, field
 
 from typer import Typer
 
 from infrable.host import Host
 from infrable.meta import Meta
-from infrable.util import template
+from infrable.util import formatter
 
 
 @dataclass(unsafe_hash=True, order=True, eq=True)
 class Service:
     """A generic service, maybe running on a host."""
 
     host: Host | None = None
     port: int | None = None
     meta: Meta = field(default_factory=Meta)
     typer: Typer | None = None
 
     def format(self, name: str, format) -> str:
-        return template(format).render(name=name, **asdict(self))
+        return formatter(format).render(name=name, **asdict(self))
 
     def __str__(self) -> str:
         return f'{self.host or ""}:{self.port or ""}'
```

### Comparing `infrable-0.0.1/infrable/switch.py` & `infrable-0.1.0/infrable/switch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from dataclasses import asdict, dataclass
+from dataclasses import asdict, dataclass, field
 from typing import Any
 
 from typer import Typer
 
 from infrable import errors, paths
-from infrable.util import template
+from infrable.meta import Meta
+from infrable.util import formatter
 
 
 @dataclass(unsafe_hash=True, order=True, eq=True)
 class Switch:
     """A switch for the infrastructure."""
 
     options: set[str]
     init: str
+
     typer: Typer | None = None
+    meta: Meta = field(default_factory=Meta)
 
     def __post_init__(self):
         self.path = paths.switches / "-".join(sorted(self.options))
         if not self.path.exists():
             self.set(self.init)
 
     def __call__(self, **cases: Any) -> Any:
@@ -38,11 +41,11 @@
             self.path.write_text(value)
             return
 
         self.path.unlink(missing_ok=True)
         raise errors.SwitchValueError(self.path, value=value, options=self.options)
 
     def format(self, name: str, format) -> str:
-        return template(format).render(name=name, **asdict(self))
+        return formatter(format).render(name=name, **asdict(self))
 
     def __str__(self) -> str:
         return self()
```

### Comparing `infrable-0.0.1/infrable/template.py` & `infrable-0.1.0/infrable/template.py`

 * *Files identical despite different names*

### Comparing `infrable-0.0.1/infrable/cli/files.py` & `infrable-0.1.0/infrable/cli/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.0.1/infrable/cli/main.py` & `infrable-0.1.0/infrable/cli/main.py`

 * *Files identical despite different names*

### Comparing `infrable-0.0.1/infrable/cli/remote.py` & `infrable-0.1.0/infrable/cli/remote.py`

 * *Files identical despite different names*

### Comparing `infrable-0.0.1/infrable/distro/linux.py` & `infrable-0.1.0/infrable/distro/linux.py`

 * *Files identical despite different names*

### Comparing `infrable-0.0.1/infrable/distro/ubuntu.py` & `infrable-0.1.0/infrable/distro/ubuntu.py`

 * *Files identical despite different names*

### Comparing `infrable-0.0.1/.gitignore` & `infrable-0.1.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -160,7 +160,8 @@
 #.idea/
 
 # Test files
 /.infrable/
 /infra.py
 /templates/
 /secrets/
+/lib/
```

### Comparing `infrable-0.0.1/LICENSE` & `infrable-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `infrable-0.0.1/pyproject.toml` & `infrable-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   'python-box'
 ]
 
 [project.urls]
 Homepage = 'https://github.com/stckme/infrable'
 
 [project.optional-dependencies]
-devel = ['tox', 'pytest', 'pytest-cov', 'black', 'isort', 'build']
+devel = ['tox', 'pytest', 'pytest-cov', 'black', 'isort', 'build', 'twine']
 
 [project.scripts]
 infrable = 'infrable.cli.main:app'
 
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
```

### Comparing `infrable-0.0.1/PKG-INFO` & `infrable-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: infrable
-Version: 0.0.1
+Version: 0.1.0
 Summary: Hanny's legendary infrastructure as code solution.
 Project-URL: Homepage, https://github.com/stckme/infrable
 Author-email: Arijit Basu <sayanarijit@gmail.com>
 Maintainer-email: Arijit Basu <sayanarijit@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -219,69 +219,78 @@
 Provides-Extra: devel
 Requires-Dist: black; extra == 'devel'
 Requires-Dist: build; extra == 'devel'
 Requires-Dist: isort; extra == 'devel'
 Requires-Dist: pytest; extra == 'devel'
 Requires-Dist: pytest-cov; extra == 'devel'
 Requires-Dist: tox; extra == 'devel'
+Requires-Dist: twine; extra == 'devel'
 Description-Content-Type: text/markdown
 
 # Infrable
 
 Hanny's legendary infrastructure as code solution.
 
+[![PyPI version](https://img.shields.io/pypi/v/expandvars.svg)](https://pypi.org/project/expandvars)
+
 ```bash
+# Install
 pip install -U infrable  # requires python >= 3.10
+
+# Bootstrap a new project
+touch infra.py
+infrable init
 ```
 
 # Table of contents
 
-1. [Infrable](#infrable)
-   1. [Preface](#preface)
-   2. [Chapter 1 - Chaos](#chapter-1---chaos)
-   3. [Chapter 2 - Hosts and services](#chapter-2---hosts-and-services)
-   4. [Chapter 3 - Templates](#chapter-3---templates)
-   5. [Chapter 4 - The Deploy or Recover Workflow](#chapter-4---the-deploy-or-recover-workflow)
-      1. [Deploy workflow](#deploy-workflow)
-      2. [Recover workflow](#recover-workflow)
+1. [Prologue](#prologue)
+2. [Chapter 1 - Chaos](#chapter-1---chaos)
+3. [Chapter 2 - Hosts and Services](#chapter-2---hosts-and-services)
+4. [Chapter 3 - Templates](#chapter-3---templates)
+5. [Chapter 4 - The Deploy or Recover Workflow](#chapter-4---the-deploy-or-recover-workflow)
+6. [Chapter 5 - Commands, Tasks and Workflows](#chapter-5---commands,-tasks-and-workflows)
+7. [Chapter 6 - Environments and Switches](#chapter-6---environments-and-switches)
+8. [Chapter 7 - Meta and Secrets](#chapter-7---meta-and-secrets)
+9. [Chapter 8 - Custom Modules](#chapter-8---custom-modules)
 
-### Preface
+## Prologue
 
 In an infinite void surrounded by blinking lights, Hanny woke up with her memory hollow,
 only her name echoing in the dark corners of her mind. She found herself floating in a
-realm between the tangible world of Python code and the ethereal cosmos of the space. A
-synthetic voice resonated around her about a crucial **infrastructure migration project**
-but it was all Greek to her. Her memory, once the key to the **Python** kingdom, failed to
+realm between the tangible world of **Python** code and the ethereal cosmos of the space. A
+synthetic voice resonated around her about a crucial **infrastructure** migration project
+but it was all Greek to her. Her memory, once the key to the Python kingdom, failed to
 provide any answers. She was stuck in an interstellar labyrinth, entrusted with a
 technology mission she could not recall, her only anchors being a mechanical keyboard and
 lines of code whizzing past on the nearby screen.
 
-### Chapter 1 - Chaos
+## Chapter 1 - Chaos
 
 In the void of her discontent, Hanny started to recall fragments of a past life: back on
 Earth, where a looming infrastructure migration project threatened to upend everything.
-Humanity grappled with a **chaotic infrastructure** and an ill-prepared toolkit. Python
+Humanity grappled with a **chaotic infrastructure** and an **ill-prepared toolkit**. Python
 developers fought with convoluted tools, while the desperate search for **declarative
 configuration management** proved futile. Amidst this disarray, Hanny was catapulted into
 the cosmos, a reluctant knight tasked with an unenviable quest: to find an
 **uncomplicated yet competent solution** capable of taming this looming catastrophe.
 
-### Chapter 2 - Hosts and services
+## Chapter 2 - Hosts and Services
 
 In a moment of revelation, Hanny grasped the intricacies of infrastructure: **hosts and the
 services** they housed, the vital backbone of any system. She understood the criticality of
 maintaining **a single reference source, a complete, harmonious documentation capturing
 these elemental relationships**. Committing herself to uphold this single source of truth
 principle, she began the painstaking process of documentation, pouring every detail into
-a consolidated testament christened **infra.py**.
+a consolidated testament christened **"infra.py"**.
 
 **infra.py**
 
 ```python
-template_prefix = "https://github.com/username/repo/blob/main"
+from infrable import Host, Service
 
 # Hosts/ -----------------------------------------------------------------------
 dev_host = Host(fqdn="dev.example.com", ip="127.0.0.1")
 beta_host = Host(fqdn="beta.example.com", ip="127.0.0.1")
 prod_host = Host(fqdn="prod.example.com", ip="127.0.0.1")
 # /Hosts -----------------------------------------------------------------------
 
@@ -293,108 +302,164 @@
 
 dev_nginx = Service(host=dev_host, port=80)
 beta_nginx = Service(host=beta_host, port=80)
 prod_nginx = Service(host=prod_host, port=80)
 # /Services --------------------------------------------------------------------
 ```
 
-### Chapter 3 - Templates
+## Chapter 3 - Templates
 
 Gradually piecing together her fragmented memories, Hanny realized configuration files
 for the host deployments ought to be maintained as **templates, drawing values as
 needed from "infra.py"**. Back on Earth, the challenge had been a lack of a coherent
-system to document the path of these files, a problem of organization that posed a
+system to document the destination of these files, a problem of organization that posed a
 significant hurdle. Then, in a moment of genius, Hanny conceived a groundbreaking
 solution. She'd document the files' path directly within the configuration templates
 themselves. And so, with renewed vigor, she started adding crucial details as **header
 comments nestled within the configuration files**, a legendary stroke promising to
 transform the face of infrastructure migration.
 
+**infra.py**
+
+```python
+template_prefix = "https://github.com/username/repository/blob/main"
+```
+
 **templates/nginx/web.j2**
 
 ```nginx
 # vim: syn=nginx
 
 # ---
 # src: {{ template_prefix }}/{{ _template.src }}
 # dest: {{ dev_nginx.host }}:/etc/nginx/sites-enabled/web
 # chmod: 644
 # chown: root:root
 # ---
 
 server {
-    listen 80;
-    listen [::]:80;
+    listen {{ dev_nginx.port }};
+    listen [::]:{{ dev_nginx.port }}
 
     server_name {{ dev_nginx.host.fqdn }} www.{{ dev_nginx.host.fqdn }};
 
     location / {
-        proxy_pass http://localhost:{{ dev_web.port }};
+        proxy_pass http://127.0.0.1:{{ dev_web.port }};
         include proxy_params;
     }
 }
 ```
 
-### Chapter 4 - The Deploy or Recover Workflow
+NOTE: The `_template.src` is a special variable, available in all templates.
+
+## Chapter 4 - The Deploy or Recover Workflow
 
 In the vast expanse of uncertainty, one thing became crystal clear to Hanny: the
-importance of reviewing the files made through "infra.py" and **comparing these with the
-currently deployed configurations before pushing them**. This process would **intercept
-any live changes and ensure their inclusion in the templates**. Her cautious nature also
+importance of **reviewing the files made through "infra.py" and comparing these with the
+currently deployed configurations before pushing them**. This process would intercept
+any **live changes** and ensure their inclusion in the templates. Her cautious nature also
 recognized the essential function of maintaining **local backups** of the utilized
 configurations, providing an insurance of sorts. To address any complications, she
 conceived a failsafe measure: **The Deploy or Recover Workflow**. It promised relief from
 human error while ensuring an approach to **easily revert and recover** the service,
 another triumphant stride in Hanny’s cosmic saga.
 
-#### Deploy workflow
+Deploy workflow:
 
 ```bash
-infrable files deploy
+infrable files deploy [path]
 
-## same as
-# infrable files gen
+## Same as
+# infrable files gen [path]
 # infrable files pull
 # infrable files backup
 # infrable files push
 ```
 
+For snake folks:
+
+```python
+from infrable import files
+
+files.deploy(path)
+
+## Same as
+# files.gen(path)
+# files.pull()
+# files.backup()
+# files.push()
+```
+
 ```mermaid
 flowchart TD;
     A[gen: generate artifacts from templates and infra.py as .new files] --> B[pull: for each generated artifact pull the currently deployed version from server as .old files];
     B --> C[backup: copy the artifacts in a local backup directory for easy recovery in case of failure];
     C --> E[diff: compare the .new and .old files];
     E -- push: for each result --> F{is there any difference?};
     F -- yes --> H[display the diff];
     F -- no --> G[skip and delete artifacts];
     H --> I{confirm push?};
     I -- yes --> J[push the file onto the server];
     I -- no --> K[skip and delete artifacts];
 ```
 
-#### Recover workflow
+Diff example:
+
+```diff
+--- .infrable/files/root@dev.example.com/etc/monit/conf.d/system.cfg.old
+
++++ .infrable/files/root@dev.example.com/etc/monit/conf.d/system.cfg.new
+
+@@ -1,13 +1,14 @@
+
+ check system dev.example.com
+-    if memory usage > 85% then alert
++    # if memory usage > 85% then alert
+     if cpu usage (user) > 80% for 3 cycles then alert
+     if cpu usage (system) > 80% for 3 cycles then alert
+
+Push? (y, n, all) [y]:
+```
+
+Recover workflow:
 
 ```bash
-infrable files recover
+infrable files recover [path]
 
-## same as
-# infrable files revert
+## Same as
+# infrable files revert [path]
 # infrable files push
 ```
 
+For snake folks:
+
+```python
+from infrable import files
+
+files.recover(path)
+
+## Same as
+# files.revert(path)
+# files.push()
+```
+
 ```mermaid
 flowchart TD;
 
     A[revert: copy the artifacts from the given or latest backup directory into artifacts directory but in reverse order] --> B[diff: compare the .new and .old files];
     B --> C[push: run the steps for the push workflow]
 ```
 
-### Chapter 5 - Commands and Tasks
+## Chapter 5 - Commands, Tasks and Workflows
 
-TODO: Document commands
+As Hanny delved deeper into the complexities of infrastructure migration, she encountered
+a critical realization: the need to extend beyond mere configuration pushing. To attain a
+seamless transition, testing, service restarts, and other post-deployment actions were
+imperative. With relentless determination, she integrated a feature within "infra.py" to
+**execute remote commands** on hosts, a capability enhancing the deployment process.
 
 ```bash
 # Run a command on a host by name
 infrable remote dev_host "sudo systemctl reload nginx"
 
 # Or by service name
 infrable remote dev_nginx "sudo systemctl reload nginx"
@@ -402,150 +467,272 @@
 # Or all affected hosts (as per files diff)
 infrable remote affected-hosts "sudo systemctl reload nginx"
 
 # Or
 infrable files affected-hosts | infrable remote - "sudo systemctl reload nginx"
 ```
 
-TODO: Document tasks
+But Hanny's pursuit of excellence didn't halt there; she grasped the inadequacy of loose
+command execution, acknowledging the necessity for structured organization. Thus, she
+envisioned a novel concept - the creation of **"Tasks"**, groups of related commands
+designed to streamline operations.
 
 **infra.py**
 
 ```python
-nginx_dev.typer = typer.Typer()
-@nginx_dev.typer.command()
-def reload(test: bool = True):
-    assert nginx.host, "Service must have a host to reload"
-    if test:
-        nginx.host.remote().sudo.nginx("-t")
-    nginx.host.remote().sudo.systemctl.reload.nginx()
+import typer
+
+# Tasks/ -----------------------------------------------------------------------
+dev_nginx.typer = typer.Typer(help="dev_nginx specific tasks.")
+
+@dev_nginx.typer.command(name="reload")
+def reload_dev_nginx():
+    """[TASK] Reload nginx: infrable dev-nginx reload"""
+
+    assert dev_nginx.host, "Service must have a host to reload"
+    dev_nginx.host.remote().sudo.nginx("-t")
+    dev_nginx.host.remote().sudo.systemctl.reload.nginx()
 ```
 
 ```bash
-infrable nginx-dev reload --test
+infrable dev-nginx reload
 ```
 
-Or define a global reload task
+As she toiled to realize this vision, a brilliant idea swept over her - to
+orchestrate these tasks into coherent sequences, she christened them
+**"workflows"**, heralding the dawn of a new era in infrastructure management.
 
 **infra.py**
 
 ```python
-reload = typer.Typer()
-@reload.command()
-def nginx_dev(test: bool = True):
-    assert nginx.host, "Service must have a host to reload"
-    if test:
-        nginx.host.remote().sudo.nginx("-t")
-    nginx.host.remote().sudo.systemctl.reload.nginx()
+from infrable import parallel, paths
+
+# Workflows/ -----------------------------------------------------------------------
+deploy = typer.Typer(help="Deployment workflows.")
+
+@deploy.command(name="dev-nginx")
+def deploy_dev_nginx():
+    """[WORKFLOW] Deploy dev_nginx files: infrable deploy dev-nginx"""
+
+    files.deploy(paths.templates / "nginx")
+    hosts = files.affected_hosts()
+    cmd = "sudo nginx -t && sudo systemctl reload nginx && echo success || echo failed"
+    tasks = [lambda: (h, h.remote().sudo(cmd)) for h in hosts]
+    for host, result in parallel(tasks):
+        print(f"{host}: {result}")
+# /Workflows -----------------------------------------------------------------------
 ```
 
 ```bash
-infrable reload nginx-dev --test
+infrable deploy dev-nginx
 ```
 
-### Chapter 6 - Environments and switches
+## Chapter 6 - Environments and Switches
 
-TODO: Document environments
+The exhilaration of progress was swiftly countered by the rigors of defining **templates,
+tasks, and workflows independently for every host within multiple environments**. Hanny's
+keen eyes blinked tiredly at lines of Python code, her fingers aching from relentless
+typing. It was then that she stumbled upon another vital realization: **the service and
+host relationship hinged upon the environment**. The environment — "dev", "beta", "prod",
+among others — determined where services were deployed. Wondering **if environments could
+be switchable**, she pondered a pivotal question: What if the "infra.py" file could
+adjust values based on the environment? This would phenomenally simplify the deployment
+process, **utilizing the same template, task, and workflow definitions across different
+hosts**. Seizing on this insight, Hanny developed **'Switch'**, an ingenious mechanism
+allowing **environment-dependent value adjustment within "infra.py"**. With 'Switch',
+infrastructure migration wasn't a labyrinth to navigate but a journey of exploration and
+innovation. The weight of her mission lightened with every line of code she churned out.
+And so Hanny, engulfed by the silence of the cosmos, marched on, her spirit indomitable,
+her zeal untamed.
 
 **infra.py**
 
-```bash
+```python
+from infrable import Switch, Host, Service
+
 # Environments/ ----------------------------------------------------------------
 dev = "dev"
 beta = "beta"
 prod = "prod"
 
 environments = {dev, beta, prod}
-env = Switch(environments, init=dev)  # <-- defining a switch between different environments
+env = Switch(environments, init=dev)  # <-- Defining a switch for different environments
 current_env = env()
 # /Environments ----------------------------------------------------------------
 
 # Hosts/ -----------------------------------------------------------------------
 dev_host = Host(fqdn="dev.example.com", ip="127.0.0.1")
 beta_host = Host(fqdn="beta.example.com", ip="127.0.0.1")
 prod_host = Host(fqdn="prod.example.com", ip="127.0.0.1")
 
-managed_hosts = env(  # <-- defining hosts for different environments
+managed_hosts = env(  # <-- Switching hosts based on the environment
     dev=[dev_host],
     beta=[beta_host],
     prod=[prod_host],
 )
 # /Hosts -----------------------------------------------------------------------
 
 # Services/ --------------------------------------------------------------------
 web = Service(
-    host=env(dev=dev_host, beta=beta_host, prod=prod_host),
+    host=env(dev=dev_host, beta=beta_host, prod=prod_host),  # <-- Switching host
     port=8080,
 )
 
-nginx = Service(
-    port=80,
-    host=env(dev=dev_host, beta=beta_host, prod=prod_host),
-)
+nginx = Service(port=80, host=web.host)  # <-- No need to use switch here
 # /Services --------------------------------------------------------------------
 ```
 
-Update templates to use the environment specific values hosts:
+Updating the templates to use the switchable values:
 
 **templates/nginx/proxy_params.j2**
 
 ```nginx
 # vim: syn=nginx
 
 # ---
 # src: {{ template_prefix }}/{{ _template.src }}
 # dest:
-# {% for host in managed_hosts %}
+# {% for host in managed_hosts %}  # <-- Yes, you can
 #   - loc: {{ host }}:/etc/nginx/proxy_params
 # {% endfor %}
 # chmod: 644
 # chown: root:root
 # ---
 proxy_set_header Host $http_host;
 proxy_set_header X-Real-IP $remote_addr;
 proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
 proxy_set_header X-Forwarded-Proto $scheme;
 ```
 
-Switch management:
+Managing switches:
 
 ```bash
 # Switch current environment
 infrable switch env [dev|beta|prod]
 
 # Check all switch values
 infrable switches
 ```
 
-### Chapter 6 - Meta and Secrets
+## Chapter 7 - Meta and Secrets
 
-TODO: Document secrets
+Chapter 7 - The Secret Keeper
+
+A veil of mystery cloaked Hanny's latest quest. She coveted the ability to access **secret
+values, untouched by the eyes of version control systems, and juxtapose these to hosts
+and services**. It was a daunting challenge — to embed securely these secret keys within
+the Python labyrinth without heightening complexity. She mused, her gaze focused on the
+stars scattered across the cosmos. If simplicity was the mother of invention, Hanny would
+be its devoted disciple. She engaged in the great **Pythonic tradition of simplicity**,
+armed with wisdom acquired from prior challenges, plunging into the task at hand. She
+devised an elegant strategy. Her solution was a poet’s dream and a programmer’s delight,
+the relief of her achievement echoing in the cosmic silence.
 
 **infra.py**
 
 ```python
-common_ssh_key = readfile("secrets/common/ssh_key")  # <-- read a secret file
+from infrable import Meta, readfile
+
+common_secret_key = readfile("secrets/common/secret_key")  # <-- Read a secret file
 
 web = Service(
-    meta=Meta(secret_key=common_ssh_key),  # <-- attach metadata to items
+    meta=Meta(secret_key=common_secret_key),  # <-- Attach metadata to items
     host=env(dev=dev_host, beta=beta_host, prod=prod_host),
     port=8080,
 )
 ```
 
 Managing secrets:
 
 ```bash
+# Hide secrets from git
+echo /secrets/ >> .gitignore
+
+# Update the secrets by hand
 vim secrets/web/secret_key
 ```
 
-### Chapter 7 - The Python Shell
+## Chapter 8 - Custom Modules
+
+As the celestial silence enveloped her, Hanny stared at the last line of code and
+finally, exhaled. The Python maestro had defied the odds, charting a path through the
+sprawling galaxy of infrastructure migration. In her hands, humanity held the weapon to
+combat the specter of inevitable infrastructure displacement, not just once but
+potentially countless times henceforth. No longer would they flounder in the face of
+migration, for **'infrable'** was here.
+
+But if the endless cosmos stood as a testament to anything, it was the **limitless
+potential for growth**. Hanny, ever the visionary, saw beyond the painstaking creation of
+a toolkit. She envisioned a continuously evolving mechanism, a collaborative system
+enhanced by the collective genius of Python peers worldwide. That's when it struck her.
+Like a supernova in the silent night, she realized the adaptability imbued within Python.
+Fellow programmers could craft **Python modules** and stitch them into the existing
+"infra.py", thus **extending and elevating its functionality**, a synergy of skills and
+codes enhancing 'infrable' to uncharted territories.
 
-Import in a Python shell
+**lib/modules/mycloud.py**
 
 ```python
-from infrable import files
-import infra
+from dataclasses import dataclass
+from typer import Typer
+from infrable import infra
+from infrable.distro.ubuntu import UbuntuLatestHost
+
+@dataclass
+class MyCloud:
+    """MyCloud Python library."""
+
+    secret_api_key: str
+    typer: Typer | None = None
+
+    def provision_ubuntu_host(self, fqdn: str):
+        ip = self.api.create_ubuntu_host(fqdn)
+        return MyCloudUbuntuHost(fqdn=fqdn, ip=ip)
+
+@dataclass
+class MyCloudUbuntuHost(UbuntuLatestHost):
+    """MyCloud's customized Ubuntu server."""
+
+    def setup(self, as_root: bool = False):
+        super().setup(as_root=as_root)
+        self.install_mycloud_agent()
 
-files.deploy()
-infra.nginx.host.remote().sudo.systemctl.reload.nginx()
+    def install_mycloud_agent(self):
+        raise NotImplementedError
+
+workflows = Typer()
+
+@workflows.command()
+def provision_ubuntu_host(fqdn: str, setup: bool = True):
+    """[WORKFLOW] Provision Ubuntu host."""
+
+    # Get the MyCloud instance from infra.py
+    cloud = next(iter(infra.item_types[MyCloud].values()))
+
+    # Provision the host
+    host = cloud.provision_ubuntu_host(fqdn)
+    if setup:
+        host.setup(as_root=True)
+
+    name = fqdn.split(".")[0]
+    print("Add the host to the infra.py file.")
+    print(f"{name} = {host}")
+```
+
+Plugging the module in infra.py:
+
+**infra.py**
+
+```python
+from lib.modules import mycloud
+
+# Clouds/ ----------------------------------------------------------------------
+cloud = mycloud.MyCloud(secret_api_key=readfile("secrets/mycloud/secret_api_key"))
+
+cloud.typer = typer.Typer(help="MyCloud specific workflows.")
+cloud.typer.add_typer(mycloud.workflows, name="mycloud")
+# /Clouds ----------------------------------------------------------------------
+```
+
+```
+infra cloud --help
 ```
```

