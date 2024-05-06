# Comparing `tmp/ptsecurixt-1.0.1.tar.gz` & `tmp/ptsecurixt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptsecurixt-1.0.1.tar", last modified: Fri Aug  4 12:24:10 2023, max compression
+gzip compressed data, was "ptsecurixt-1.0.2.tar", last modified: Mon May  6 16:38:08 2024, max compression
```

## Comparing `ptsecurixt-1.0.1.tar` & `ptsecurixt-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 12:24:10.046287 ptsecurixt-1.0.1/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35823 2023-08-04 11:45:39.000000 ptsecurixt-1.0.1/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3162 2023-08-04 12:24:10.046287 ptsecurixt-1.0.1/PKG-INFO
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2700 2023-08-04 12:22:03.000000 ptsecurixt-1.0.1/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 12:24:10.046287 ptsecurixt-1.0.1/ptsecurixt/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:45:39.000000 ptsecurixt-1.0.1/ptsecurixt/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-08-04 12:21:46.000000 ptsecurixt-1.0.1/ptsecurixt/_version.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6957 2023-08-04 11:45:39.000000 ptsecurixt-1.0.1/ptsecurixt/ptsecurixt.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 12:24:10.046287 ptsecurixt-1.0.1/ptsecurixt.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3162 2023-08-04 12:24:10.000000 ptsecurixt-1.0.1/ptsecurixt.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      303 2023-08-04 12:24:10.000000 ptsecurixt-1.0.1/ptsecurixt.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-08-04 12:24:10.000000 ptsecurixt-1.0.1/ptsecurixt.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       58 2023-08-04 12:24:10.000000 ptsecurixt-1.0.1/ptsecurixt.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       22 2023-08-04 12:24:10.000000 ptsecurixt-1.0.1/ptsecurixt.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       11 2023-08-04 12:24:10.000000 ptsecurixt-1.0.1/ptsecurixt.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-08-04 12:24:10.046287 ptsecurixt-1.0.1/setup.cfg
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1009 2023-08-04 11:45:39.000000 ptsecurixt-1.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 16:38:08.622414 ptsecurixt-1.0.2/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:25:17.000000 ptsecurixt-1.0.2/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3368 2024-05-06 16:38:08.622414 ptsecurixt-1.0.2/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2616 2024-05-06 16:33:40.000000 ptsecurixt-1.0.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 16:38:08.622414 ptsecurixt-1.0.2/ptsecurixt/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:25:17.000000 ptsecurixt-1.0.2/ptsecurixt/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-04-29 08:25:17.000000 ptsecurixt-1.0.2/ptsecurixt/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     6887 2024-05-06 16:33:44.000000 ptsecurixt-1.0.2/ptsecurixt/ptsecurixt.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 16:38:08.622414 ptsecurixt-1.0.2/ptsecurixt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3368 2024-05-06 16:38:08.000000 ptsecurixt-1.0.2/ptsecurixt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      303 2024-05-06 16:38:08.000000 ptsecurixt-1.0.2/ptsecurixt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-06 16:38:08.000000 ptsecurixt-1.0.2/ptsecurixt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       58 2024-05-06 16:38:08.000000 ptsecurixt-1.0.2/ptsecurixt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-06 16:38:08.000000 ptsecurixt-1.0.2/ptsecurixt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       11 2024-05-06 16:38:08.000000 ptsecurixt-1.0.2/ptsecurixt.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-06 16:38:08.622414 ptsecurixt-1.0.2/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1264 2024-05-06 16:33:40.000000 ptsecurixt-1.0.2/setup.py
```

### Comparing `ptsecurixt-1.0.1/LICENSE` & `ptsecurixt-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptsecurixt-1.0.1/PKG-INFO` & `ptsecurixt-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,86 @@
 Metadata-Version: 2.1
 Name: ptsecurixt
-Version: 1.0.1
+Version: 1.0.2
 Summary: security.txt finder
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
-License: GPLv3+
+License: GPLv3
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptsecurixt
+Project-URL: tracker, https://github.com/penterep/ptsecurixt/issues
+Project-URL: changelog, https://github.com/penterep/ptsecurixt/CHANGELOG.md
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
+Requires-Dist: ptlibs<2,>=1.0.7
 
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTSECURIXT
-> security.txt finder
+# PTSECURIXT - security.txt finder
 
-ptsecurixt is a tool that searches for security.txt file in known locations.
+ptsecurixt is an automated tool that efficiently locates 'security.txt' files in their known locations.
 
 ## Installation
 
 ```
 pip install ptsecurixt
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
 ptsecurixt -u htttps://www.example.com/
 ```
 
 ## Options
 ```
--u   --url         <url>           Connect to URL
--p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--T   --timeout                     Set timeout for HTTP requests
--c   --cookie      <cookie>        Set cookie
--ua  --user-agent  <ua>            Set User-Agent header
--H   --headers     <header:value>  Set custom header(s)
--r   --redirects                   Follow redirects (default False)
--C   --cache                       Cache HTTP communication (load from tmp in future)
--j   --json                        Output in JSON format
--v   --version                     Show script version and exit
--h   --help                        Show this help message and exit
+-u  --url         <url>           Connect to URL
+-p  --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T  --timeout                     Set timeout (default 10)
+-c  --cookie      <cookie>        Set cookie
+-a  --user-agent  <a>             Set User-Agent header
+-H  --headers     <header:value>  Set custom header(s)
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
 ptlibs
 ```
 
-## Version History
-```
-1.0.0 - 1.0.1
-    - Code improvements
-    - Updated for ptlibs 1.0.0
-0.0.4
-    - Refactored for latest ptlibs
-0.0.1 - 0.0.3
-    - Alpha releases
-```
-
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
+Copyright (c) 2024 Penterep Security s.r.o.
 
 ptsecurixt is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptsecurixt is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptsecurixt. If not, see https://www.gnu.org/licenses/.
```

### Comparing `ptsecurixt-1.0.1/README.md` & `ptsecurixt-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,64 @@
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTSECURIXT
-> security.txt finder
+# PTSECURIXT - security.txt finder
 
-ptsecurixt is a tool that searches for security.txt file in known locations.
+ptsecurixt is an automated tool that efficiently locates 'security.txt' files in their known locations.
 
 ## Installation
 
 ```
 pip install ptsecurixt
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
 ptsecurixt -u htttps://www.example.com/
 ```
 
 ## Options
 ```
--u   --url         <url>           Connect to URL
--p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--T   --timeout                     Set timeout for HTTP requests
--c   --cookie      <cookie>        Set cookie
--ua  --user-agent  <ua>            Set User-Agent header
--H   --headers     <header:value>  Set custom header(s)
--r   --redirects                   Follow redirects (default False)
--C   --cache                       Cache HTTP communication (load from tmp in future)
--j   --json                        Output in JSON format
--v   --version                     Show script version and exit
--h   --help                        Show this help message and exit
+-u  --url         <url>           Connect to URL
+-p  --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T  --timeout                     Set timeout (default 10)
+-c  --cookie      <cookie>        Set cookie
+-a  --user-agent  <a>             Set User-Agent header
+-H  --headers     <header:value>  Set custom header(s)
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
 ptlibs
 ```
 
-## Version History
-```
-1.0.0 - 1.0.1
-    - Code improvements
-    - Updated for ptlibs 1.0.0
-0.0.4
-    - Refactored for latest ptlibs
-0.0.1 - 0.0.3
-    - Alpha releases
-```
-
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
+Copyright (c) 2024 Penterep Security s.r.o.
 
 ptsecurixt is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptsecurixt is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptsecurixt. If not, see https://www.gnu.org/licenses/.
```

### Comparing `ptsecurixt-1.0.1/ptsecurixt/ptsecurixt.py` & `ptsecurixt-1.0.2/ptsecurixt/ptsecurixt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python3
 """
-    Copyright (c) 2023 Penterep Security s.r.o.
+    Copyright (c) 2024 Penterep Security s.r.o.
 
     ptsecurixt - security.txt finder
 
     ptsecurixt is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
@@ -45,17 +45,17 @@
     def run(self) -> None:
         """Main method"""
         known_places = ["security.txt", ".well-known/security.txt"]
         result = [self._find_security_txt(location) for location in known_places]
         if not any(result):
             ptprinthelper.ptprint(f"\r{' '*100}\r", "", not self.use_json, end="")
             ptprinthelper.ptprint(f"security.txt file was not found", "VULN", not self.use_json)
-            self.ptjsonlib.add_vulnerability("MISSING-SECURITY-TXT")
+            self.ptjsonlib.add_vulnerability("PTV-WEB-DISCO-SECUR")
 
-        self.ptjsonlib.set_status("ok")
+        self.ptjsonlib.set_status("finished")
         ptprinthelper.ptprint(self.ptjsonlib.get_result_json(), "", self.use_json)
 
     def _find_security_txt(self, location: str) -> bool:
         """Returns True when found"""
         url = self.url + location
         ptprinthelper.ptprint(f"\r{' '*(30+len(url))}\r[*] Searching: {url}", "TITLE", not self.use_json, end=f"", colortext=True)
         try:
@@ -93,31 +93,31 @@
             "ptsecurixt -u https://www.example.com",
         ]},
         {"options": [
             ["-u",  "--url",                    "<url>",            "Connect to URL"],
             ["-p",  "--proxy",                  "<proxy>",          "Set proxy (e.g. http://127.0.0.1:8080)"],
             ["-T",  "--timeout",                "",                 "Set timeout (default 10)"],
             ["-c",  "--cookie",                 "<cookie>",         "Set cookie"],
-            ["-ua", "--user-agent",             "<ua>",             "Set User-Agent header"],
+            ["-a", "--user-agent",              "<a>",             "Set User-Agent header"],
             ["-H",  "--headers",                "<header:value>",   "Set custom header(s)"],
             ["-r",  "--redirects",              "",                 "Follow redirects (default False)"],
             ["-C",  "--cache",                  "",                 "Cache HTTP communication (load from tmp in future)"],
             ["-v",  "--version",                "",                 "Show script version and exit"],
             ["-h",  "--help",                   "",                 "Show this help message and exit"],
             ["-j",  "--json",                   "",                 "Output in JSON format"],
         ]
         }]
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(add_help="False", description="ptseruxt <options>")
+    parser = argparse.ArgumentParser(add_help="False", description=f"{SCRIPTNAME} <options>")
     parser.add_argument("-u",  "--url",            type=str, required=True)
     parser.add_argument("-p",  "--proxy",          type=str)
     parser.add_argument("-T",  "--timeout",        type=int, default=10)
-    parser.add_argument("-ua", "--user-agent",     type=str, default="Penterep Tools")
+    parser.add_argument("-a",  "--user-agent",     type=str, default="Penterep Tools")
     parser.add_argument("-c",  "--cookie",         type=str)
     parser.add_argument("-H",  "--headers",        type=ptmisclib.pairs, nargs="+")
     parser.add_argument("-r",  "--redirects",      action="store_true")
     parser.add_argument("-C",  "--cache",          action="store_true")
     parser.add_argument("-j",  "--json",           action="store_true")
     parser.add_argument("-v",  "--version",        action='version', version=f'{SCRIPTNAME} {__version__}')
 
@@ -130,15 +130,14 @@
     return args
 
 
 def main():
     global SCRIPTNAME
     SCRIPTNAME = "ptsecurixt"
     requests.packages.urllib3.disable_warnings()
-    requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
     args = parse_args()
     script = PtSecurixt(args)
     script.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ptsecurixt-1.0.1/ptsecurixt.egg-info/PKG-INFO` & `ptsecurixt-1.0.2/ptsecurixt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,86 @@
 Metadata-Version: 2.1
 Name: ptsecurixt
-Version: 1.0.1
+Version: 1.0.2
 Summary: security.txt finder
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
-License: GPLv3+
+License: GPLv3
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptsecurixt
+Project-URL: tracker, https://github.com/penterep/ptsecurixt/issues
+Project-URL: changelog, https://github.com/penterep/ptsecurixt/CHANGELOG.md
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
+Requires-Dist: ptlibs<2,>=1.0.7
 
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTSECURIXT
-> security.txt finder
+# PTSECURIXT - security.txt finder
 
-ptsecurixt is a tool that searches for security.txt file in known locations.
+ptsecurixt is an automated tool that efficiently locates 'security.txt' files in their known locations.
 
 ## Installation
 
 ```
 pip install ptsecurixt
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
 ptsecurixt -u htttps://www.example.com/
 ```
 
 ## Options
 ```
--u   --url         <url>           Connect to URL
--p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--T   --timeout                     Set timeout for HTTP requests
--c   --cookie      <cookie>        Set cookie
--ua  --user-agent  <ua>            Set User-Agent header
--H   --headers     <header:value>  Set custom header(s)
--r   --redirects                   Follow redirects (default False)
--C   --cache                       Cache HTTP communication (load from tmp in future)
--j   --json                        Output in JSON format
--v   --version                     Show script version and exit
--h   --help                        Show this help message and exit
+-u  --url         <url>           Connect to URL
+-p  --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T  --timeout                     Set timeout (default 10)
+-c  --cookie      <cookie>        Set cookie
+-a  --user-agent  <a>             Set User-Agent header
+-H  --headers     <header:value>  Set custom header(s)
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
 ptlibs
 ```
 
-## Version History
-```
-1.0.0 - 1.0.1
-    - Code improvements
-    - Updated for ptlibs 1.0.0
-0.0.4
-    - Refactored for latest ptlibs
-0.0.1 - 0.0.3
-    - Alpha releases
-```
-
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
+Copyright (c) 2024 Penterep Security s.r.o.
 
 ptsecurixt is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptsecurixt is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptsecurixt. If not, see https://www.gnu.org/licenses/.
```

