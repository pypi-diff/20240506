# Comparing `tmp/ptprssi-1.0.0.tar.gz` & `tmp/ptprssi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptprssi-1.0.0.tar", last modified: Mon Aug  7 10:19:17 2023, max compression
+gzip compressed data, was "ptprssi-1.0.1.tar", last modified: Mon May  6 18:52:55 2024, max compression
```

## Comparing `ptprssi-1.0.0.tar` & `ptprssi-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 10:19:17.428537 ptprssi-1.0.0/
--rwxrw-rw-   0 daniel    (1000) daniel    (1000)    35823 2023-01-11 20:44:27.000000 ptprssi-1.0.0/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3146 2023-08-07 10:19:17.424537 ptprssi-1.0.0/PKG-INFO
--rwxrw-rw-   0 daniel    (1000) daniel    (1000)     2659 2023-08-07 09:48:59.000000 ptprssi-1.0.0/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 10:19:17.424537 ptprssi-1.0.0/ptprssi/
--rwxrw-rw-   0 daniel    (1000) daniel    (1000)        0 2023-01-11 20:44:27.000000 ptprssi-1.0.0/ptprssi/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-04-19 12:46:57.000000 ptprssi-1.0.0/ptprssi/_version.py
--rwxrw-rw-   0 daniel    (1000) daniel    (1000)     7854 2023-08-07 10:06:43.000000 ptprssi-1.0.0/ptprssi/ptprssi.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 10:19:17.424537 ptprssi-1.0.0/ptprssi.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3146 2023-08-07 10:19:17.000000 ptprssi-1.0.0/ptprssi.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      273 2023-08-07 10:19:17.000000 ptprssi-1.0.0/ptprssi.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-08-07 10:19:17.000000 ptprssi-1.0.0/ptprssi.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       49 2023-08-07 10:19:17.000000 ptprssi-1.0.0/ptprssi.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       31 2023-08-07 10:19:17.000000 ptprssi-1.0.0/ptprssi.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        8 2023-08-07 10:19:17.000000 ptprssi-1.0.0/ptprssi.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-08-07 10:19:17.428537 ptprssi-1.0.0/setup.cfg
--rwxrw-rw-   0 daniel    (1000) daniel    (1000)      998 2023-08-07 10:00:47.000000 ptprssi-1.0.0/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 18:52:55.976677 ptprssi-1.0.1/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-28 10:49:37.000000 ptprssi-1.0.1/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3623 2024-05-06 18:52:55.976677 ptprssi-1.0.1/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2817 2024-04-28 10:49:37.000000 ptprssi-1.0.1/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 18:52:55.966677 ptprssi-1.0.1/ptprssi/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-28 10:49:37.000000 ptprssi-1.0.1/ptprssi/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-06 18:50:13.000000 ptprssi-1.0.1/ptprssi/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    10572 2024-05-06 18:46:14.000000 ptprssi-1.0.1/ptprssi/ptprssi.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 18:52:55.976677 ptprssi-1.0.1/ptprssi.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3623 2024-05-06 18:52:55.000000 ptprssi-1.0.1/ptprssi.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      273 2024-05-06 18:52:55.000000 ptprssi-1.0.1/ptprssi.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-06 18:52:55.000000 ptprssi-1.0.1/ptprssi.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2024-05-06 18:52:55.000000 ptprssi-1.0.1/ptprssi.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       22 2024-05-06 18:52:55.000000 ptprssi-1.0.1/ptprssi.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        8 2024-05-06 18:52:55.000000 ptprssi-1.0.1/ptprssi.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-06 18:52:55.976677 ptprssi-1.0.1/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1257 2024-05-06 18:46:42.000000 ptprssi-1.0.1/setup.py
```

### Comparing `ptprssi-1.0.0/LICENSE` & `ptprssi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ptprssi-1.0.0/PKG-INFO` & `ptprssi-1.0.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,93 @@
 Metadata-Version: 2.1
 Name: ptprssi
-Version: 1.0.0
-Summary: Path-relative style sheet import testing tool
+Version: 1.0.1
+Summary: Path-Relative Style Sheet Import Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
-License: GPLv3+
+License: GPLv3
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptprssi
+Project-URL: tracker, https://github.com/penterep/ptprssi/issues
+Project-URL: changelog, https://github.com/penterep/ptprssi/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.6
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ptlibs<2,>=1
+Requires-Dist: bs4
+Requires-Dist: lxml
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTPRSSI
-> Path-relative style sheet import testing tool
+## PTPRSSI - Path-Relative Style Sheet Import Testing Tool
+
+ptprssi is a tool that tests domains for path relative style sheet import vulnerabilities. <br />
+This tool utilizes threading for fast parallel domain testing.
 
 ## Installation
 ```
 pip install ptprssi
 ```
 
-## Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+## Adding to PATH
+If you're unable to invoke the script from your terminal, it's likely because it's not included in your PATH. You can resolve this issue by executing the following commands, depending on the shell you're using:
 
-> Add to PATH for Bash
+For Bash Users
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
-> Add to PATH for ZSH
+For ZSH Users
 ```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
-source ~/.zshhrc
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
+source ~/.zshrc
 ```
 
 ## Usage examples
 ```
 ptprssi -u https://www.example.com/
-ptprssi -u https://www.example.com/ --redirects
+ptprssi -l domainList.txt
 ```
 
 ## Options
 ```
--u   --url         <url>           Connect to URL
--p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--H   --headers     <header:value>  Set custom header(s)
--T   --timeout     <timeout>       Set timeout (default 10s)
--ua  --user-agent  <ua>            Set User-Agent header
--c   --cookie      <cookie>        Set cookie
--r   --redirects                   Follow redirects (default False)
--C   --cache                       Cache HTTP communication (load from tmp in future)
--v   --version                     Show script version and exit
--h   --help                        Show this help message and exit
--j   --json                        Output in JSON format
+-u  --url         <url>           Connect to URL
+-l  --list        <list>          Test list of domains
+-p  --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T  --timeout     <timeout>       Set timeout (default 10s)
+-H  --headers     <header:value>  Set Header(s)
+-a  --user-agent  <agent>         Set User-Agent
+-c  --cookie      <cookie>        Set Cookie(s)
+-t  --threads     <threads>       Set threads count
+-r  --redirects                   Follow redirects (default False)
+-C  --cache                       Cache HTTP communication (load from tmp in future)
+-v  --version                     Show script version and exit
+-h  --help                        Show this help message and exit
+-j  --json                        Output in JSON format
+
 ```
 
 ## Dependencies
 ```
-requests
+ptlibs
 bs4
 lxml
-ptlibs
-```
-
-## Version History
-```
-1.0.0
-    - Code improvements
-    - Updated for ptlibs 1.0.0
-0.0.1 - 0.0.4
-    - Alpha releases
 ```
 
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
+Copyright (c) 2024 Penterep Security s.r.o.
 
 ptprssi is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptprssi is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptprssi. If not, see https://www.gnu.org/licenses/.
```

### Comparing `ptprssi-1.0.0/README.md` & `ptprssi-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,69 @@
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTPRSSI
-> Path-relative style sheet import testing tool
+## PTPRSSI - Path-Relative Style Sheet Import Testing Tool
+
+ptprssi is a tool that tests domains for path relative style sheet import vulnerabilities. <br />
+This tool utilizes threading for fast parallel domain testing.
 
 ## Installation
 ```
 pip install ptprssi
 ```
 
-## Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+## Adding to PATH
+If you're unable to invoke the script from your terminal, it's likely because it's not included in your PATH. You can resolve this issue by executing the following commands, depending on the shell you're using:
 
-> Add to PATH for Bash
+For Bash Users
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
-> Add to PATH for ZSH
+For ZSH Users
 ```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
-source ~/.zshhrc
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
+source ~/.zshrc
 ```
 
 ## Usage examples
 ```
 ptprssi -u https://www.example.com/
-ptprssi -u https://www.example.com/ --redirects
+ptprssi -l domainList.txt
 ```
 
 ## Options
 ```
--u   --url         <url>           Connect to URL
--p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--H   --headers     <header:value>  Set custom header(s)
--T   --timeout     <timeout>       Set timeout (default 10s)
--ua  --user-agent  <ua>            Set User-Agent header
--c   --cookie      <cookie>        Set cookie
--r   --redirects                   Follow redirects (default False)
--C   --cache                       Cache HTTP communication (load from tmp in future)
--v   --version                     Show script version and exit
--h   --help                        Show this help message and exit
--j   --json                        Output in JSON format
+-u  --url         <url>           Connect to URL
+-l  --list        <list>          Test list of domains
+-p  --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T  --timeout     <timeout>       Set timeout (default 10s)
+-H  --headers     <header:value>  Set Header(s)
+-a  --user-agent  <agent>         Set User-Agent
+-c  --cookie      <cookie>        Set Cookie(s)
+-t  --threads     <threads>       Set threads count
+-r  --redirects                   Follow redirects (default False)
+-C  --cache                       Cache HTTP communication (load from tmp in future)
+-v  --version                     Show script version and exit
+-h  --help                        Show this help message and exit
+-j  --json                        Output in JSON format
+
 ```
 
 ## Dependencies
 ```
-requests
+ptlibs
 bs4
 lxml
-ptlibs
-```
-
-## Version History
-```
-1.0.0
-    - Code improvements
-    - Updated for ptlibs 1.0.0
-0.0.1 - 0.0.4
-    - Alpha releases
 ```
 
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
+Copyright (c) 2024 Penterep Security s.r.o.
 
 ptprssi is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptprssi is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptprssi. If not, see https://www.gnu.org/licenses/.
```

### Comparing `ptprssi-1.0.0/ptprssi.egg-info/PKG-INFO` & `ptprssi-1.0.1/ptprssi.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,93 @@
 Metadata-Version: 2.1
 Name: ptprssi
-Version: 1.0.0
-Summary: Path-relative style sheet import testing tool
+Version: 1.0.1
+Summary: Path-Relative Style Sheet Import Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
-License: GPLv3+
+License: GPLv3
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptprssi
+Project-URL: tracker, https://github.com/penterep/ptprssi/issues
+Project-URL: changelog, https://github.com/penterep/ptprssi/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.6
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ptlibs<2,>=1
+Requires-Dist: bs4
+Requires-Dist: lxml
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTPRSSI
-> Path-relative style sheet import testing tool
+## PTPRSSI - Path-Relative Style Sheet Import Testing Tool
+
+ptprssi is a tool that tests domains for path relative style sheet import vulnerabilities. <br />
+This tool utilizes threading for fast parallel domain testing.
 
 ## Installation
 ```
 pip install ptprssi
 ```
 
-## Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+## Adding to PATH
+If you're unable to invoke the script from your terminal, it's likely because it's not included in your PATH. You can resolve this issue by executing the following commands, depending on the shell you're using:
 
-> Add to PATH for Bash
+For Bash Users
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
-> Add to PATH for ZSH
+For ZSH Users
 ```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
-source ~/.zshhrc
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
+source ~/.zshrc
 ```
 
 ## Usage examples
 ```
 ptprssi -u https://www.example.com/
-ptprssi -u https://www.example.com/ --redirects
+ptprssi -l domainList.txt
 ```
 
 ## Options
 ```
--u   --url         <url>           Connect to URL
--p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--H   --headers     <header:value>  Set custom header(s)
--T   --timeout     <timeout>       Set timeout (default 10s)
--ua  --user-agent  <ua>            Set User-Agent header
--c   --cookie      <cookie>        Set cookie
--r   --redirects                   Follow redirects (default False)
--C   --cache                       Cache HTTP communication (load from tmp in future)
--v   --version                     Show script version and exit
--h   --help                        Show this help message and exit
--j   --json                        Output in JSON format
+-u  --url         <url>           Connect to URL
+-l  --list        <list>          Test list of domains
+-p  --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T  --timeout     <timeout>       Set timeout (default 10s)
+-H  --headers     <header:value>  Set Header(s)
+-a  --user-agent  <agent>         Set User-Agent
+-c  --cookie      <cookie>        Set Cookie(s)
+-t  --threads     <threads>       Set threads count
+-r  --redirects                   Follow redirects (default False)
+-C  --cache                       Cache HTTP communication (load from tmp in future)
+-v  --version                     Show script version and exit
+-h  --help                        Show this help message and exit
+-j  --json                        Output in JSON format
+
 ```
 
 ## Dependencies
 ```
-requests
+ptlibs
 bs4
 lxml
-ptlibs
-```
-
-## Version History
-```
-1.0.0
-    - Code improvements
-    - Updated for ptlibs 1.0.0
-0.0.1 - 0.0.4
-    - Alpha releases
 ```
 
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
+Copyright (c) 2024 Penterep Security s.r.o.
 
 ptprssi is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptprssi is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptprssi. If not, see https://www.gnu.org/licenses/.
```

### Comparing `ptprssi-1.0.0/setup.py` & `ptprssi-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,26 +3,32 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ptprssi",
     version=__version__,
-    description="Path-relative style sheet import testing tool",
+    description="Path-Relative Style Sheet Import Testing Tool",
     author="Penterep",
     author_email="info@penterep.com",
     url="https://www.penterep.com/",
-    license="GPLv3+",
+    license="GPLv3",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: Implementation :: CPython",
         "Environment :: Console",
         "Topic :: Security",
-        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
-    python_requires='>=3.6',
-    install_requires=["ptlibs>=1,<2", "requests", "lxml", "bs4"],
+    python_requires='>=3.9',
+    install_requires=["ptlibs>=1,<2", "bs4", "lxml"],
     entry_points = {'console_scripts': ['ptprssi = ptprssi.ptprssi:main']},
     long_description=long_description,
     long_description_content_type="text/markdown",
+    project_urls = {
+    "homepage":   "https://www.penterep.com/",
+    "repository": "https://github.com/penterep/ptprssi",
+    "tracker":    "https://github.com/penterep/ptprssi/issues",
+    "changelog":  "https://github.com/penterep/ptprssi/blob/main/CHANGELOG.md",
+    }
 )
```

