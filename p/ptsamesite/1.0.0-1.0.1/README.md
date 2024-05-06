# Comparing `tmp/ptsamesite-1.0.0.tar.gz` & `tmp/ptsamesite-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptsamesite-1.0.0.tar", last modified: Mon Aug  7 11:48:01 2023, max compression
+gzip compressed data, was "ptsamesite-1.0.1.tar", last modified: Mon May  6 17:10:16 2024, max compression
```

## Comparing `ptsamesite-1.0.0.tar` & `ptsamesite-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 11:48:01.172405 ptsamesite-1.0.0/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35823 2023-08-07 10:48:49.000000 ptsamesite-1.0.0/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3495 2023-08-07 11:48:01.172405 ptsamesite-1.0.0/PKG-INFO
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3029 2023-08-07 11:42:39.000000 ptsamesite-1.0.0/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 11:48:01.168405 ptsamesite-1.0.0/ptsamesite/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 10:48:49.000000 ptsamesite-1.0.0/ptsamesite/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-08-07 10:48:49.000000 ptsamesite-1.0.0/ptsamesite/_version.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     7312 2023-08-07 11:36:40.000000 ptsamesite-1.0.0/ptsamesite/ptsamesite.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 11:48:01.172405 ptsamesite-1.0.0/ptsamesite.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3495 2023-08-07 11:48:01.000000 ptsamesite-1.0.0/ptsamesite.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      303 2023-08-07 11:48:01.000000 ptsamesite-1.0.0/ptsamesite.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-08-07 11:48:01.000000 ptsamesite-1.0.0/ptsamesite.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       58 2023-08-07 11:48:01.000000 ptsamesite-1.0.0/ptsamesite.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       39 2023-08-07 11:48:01.000000 ptsamesite-1.0.0/ptsamesite.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       11 2023-08-07 11:48:01.000000 ptsamesite-1.0.0/ptsamesite.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-08-07 11:48:01.172405 ptsamesite-1.0.0/setup.cfg
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1042 2023-08-07 10:48:49.000000 ptsamesite-1.0.0/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 17:10:16.712427 ptsamesite-1.0.1/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:24:58.000000 ptsamesite-1.0.1/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3681 2024-05-06 17:10:16.712427 ptsamesite-1.0.1/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2883 2024-04-29 08:24:58.000000 ptsamesite-1.0.1/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 17:10:16.712427 ptsamesite-1.0.1/ptsamesite/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:24:58.000000 ptsamesite-1.0.1/ptsamesite/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-04-29 08:24:58.000000 ptsamesite-1.0.1/ptsamesite/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     7297 2024-05-06 13:47:15.000000 ptsamesite-1.0.1/ptsamesite/ptsamesite.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 17:10:16.712427 ptsamesite-1.0.1/ptsamesite.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3681 2024-05-06 17:10:16.000000 ptsamesite-1.0.1/ptsamesite.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      303 2024-05-06 17:10:16.000000 ptsamesite-1.0.1/ptsamesite.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-06 17:10:16.000000 ptsamesite-1.0.1/ptsamesite.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       58 2024-05-06 17:10:16.000000 ptsamesite-1.0.1/ptsamesite.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       32 2024-05-06 17:10:16.000000 ptsamesite-1.0.1/ptsamesite.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       11 2024-05-06 17:10:16.000000 ptsamesite-1.0.1/ptsamesite.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-06 17:10:16.712427 ptsamesite-1.0.1/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1309 2024-05-06 17:02:21.000000 ptsamesite-1.0.1/setup.py
```

### Comparing `ptsamesite-1.0.0/LICENSE` & `ptsamesite-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ptsamesite-1.0.0/PKG-INFO` & `ptsamesite-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 Metadata-Version: 2.1
 Name: ptsamesite
-Version: 1.0.0
-Summary: Same site scripting detection tool
+Version: 1.0.1
+Summary: Same Site Scripting Detection Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
-License: GPLv3+
+License: GPLv3
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptsamesite
+Project-URL: tracker, https://github.com/penterep/ptsamesite/issues
+Project-URL: changelog, https://github.com/penterep/ptsamesite/blob/main/CHANGELOG.md
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
+Requires-Dist: dnspython>=2.1
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTSAMESITE
-
-> Same site scripting detection tool
-
-ptsamesite is a tool that tests domains for same site scripting vulnerability. <br />
-ptsamesite utilizes threading for fast parallel domain testing.
+# PTSAMESITE - Same Site Scripting Detection Tool
 
+ptsamesite is a tool designed to detect same-site scripting vulnerabilities across various domains.
 
 ## Installation
 
 ```
 pip install ptsamesite
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
 ptsamesite -d example.com                               # Test domain
 ptsamesite -d example.com example2.com                  # Test two domains
 ptsamesite -d subdomain1.subdomain2.example.com -s      # Test domain along with all subdomains
 ptsamesite -f domain_list.txt                           # Test domains from a file
-ptsamesite -f domains_list.txt -s -t 100 -V             # Test domains from a file with all present subdomains, set threads count to 100 and print only vulnerable domains
+ptsamesite -f domains_list.txt -s -t 100 -V             # Test domains from a file with all subdomains, set threads to 100 and print only vulnerable domains
 ```
 
 ## Options
 ```
 -d  --domain      <domain>   Test domain
 -f  --file        <file>     Test domains from file
 -s  --subdomains             Test all subdomains of given domain (default False)
@@ -67,31 +69,21 @@
 -h  --help                   Show this help message and exit
 -j  --json                   Output in JSON format
 ```
 
 
 ## Dependencies
 ```
-dnspython
-tldextract
 ptlibs
-```
-
-## Version History
-```
-1.0.0
-    - Code improvements
-    - Updated for ptlibs 1.0.0
-0.0.1 - 0.0.5
-    - Alpha releases
+dnspython
 ```
 
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
+Copyright (c) 2024 Penterep Security s.r.o.
 
 ptsamesite is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 ptsamesite is distributed in the hope that it will be useful,
```

### Comparing `ptsamesite-1.0.0/README.md` & `ptsamesite-1.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTSAMESITE
-
-> Same site scripting detection tool
-
-ptsamesite is a tool that tests domains for same site scripting vulnerability. <br />
-ptsamesite utilizes threading for fast parallel domain testing.
+# PTSAMESITE - Same Site Scripting Detection Tool
 
+ptsamesite is a tool designed to detect same-site scripting vulnerabilities across various domains.
 
 ## Installation
 
 ```
 pip install ptsamesite
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
 ptsamesite -d example.com                               # Test domain
 ptsamesite -d example.com example2.com                  # Test two domains
 ptsamesite -d subdomain1.subdomain2.example.com -s      # Test domain along with all subdomains
 ptsamesite -f domain_list.txt                           # Test domains from a file
-ptsamesite -f domains_list.txt -s -t 100 -V             # Test domains from a file with all present subdomains, set threads count to 100 and print only vulnerable domains
+ptsamesite -f domains_list.txt -s -t 100 -V             # Test domains from a file with all subdomains, set threads to 100 and print only vulnerable domains
 ```
 
 ## Options
 ```
 -d  --domain      <domain>   Test domain
 -f  --file        <file>     Test domains from file
 -s  --subdomains             Test all subdomains of given domain (default False)
@@ -50,31 +46,21 @@
 -h  --help                   Show this help message and exit
 -j  --json                   Output in JSON format
 ```
 
 
 ## Dependencies
 ```
-dnspython
-tldextract
 ptlibs
-```
-
-## Version History
-```
-1.0.0
-    - Code improvements
-    - Updated for ptlibs 1.0.0
-0.0.1 - 0.0.5
-    - Alpha releases
+dnspython
 ```
 
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
+Copyright (c) 2024 Penterep Security s.r.o.
 
 ptsamesite is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 ptsamesite is distributed in the hope that it will be useful,
```

### Comparing `ptsamesite-1.0.0/ptsamesite/ptsamesite.py` & `ptsamesite-1.0.1/ptsamesite/ptsamesite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python3
 """
-    Copyright (c) 2023 Penterep Security s.r.o.
+    Copyright (c) 2024 Penterep Security s.r.o.
 
-    ptsamesite - Same site scripting detection tool
+    ptsamesite - Same Site Scripting Detection Tool
 
     ptsamesite is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     ptsamesite is distributed in the hope that it will be useful,
@@ -18,47 +18,45 @@
     along with ptsamesite.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import argparse
 import sys; sys.path.append(__file__.rsplit("/", 1)[0])
 
 from _version import __version__
-from ptlibs import ptmisclib, ptjsonlib, ptprinthelper
+from ptlibs import ptmisclib, ptjsonlib, ptprinthelper, tldparser
 from ptlibs.threads import ptthreads, printlock
 
 import dns.resolver
-import tldextract
 
 
-class PtSamesite:
+class PtSameSite:
     def __init__(self, args):
-        self.ptjsonlib          = ptjsonlib.PtJsonLib()
-        self.ptthreads          = ptthreads.PtThreads()
-        self.use_json           = args.json
-        self.vulnerable         = args.vulnerable
-        self.subdomains         = args.subdomains
-        self.result_list        = []
-
+        self.ptjsonlib   = ptjsonlib.PtJsonLib()
+        self.ptthreads   = ptthreads.PtThreads()
+        self.use_json    = args.json
+        self.vulnerable  = args.vulnerable
+        self.subdomains  = args.subdomains
+        self.result_list = list()
         try:
             self.domain_list = ptmisclib.read_file(args.file) if args.file else args.domain
             self._domain_list_len = len(self.domain_list)
         except FileNotFoundError:
             self.ptjsonlib.end_error("File not found", self.use_json)
 
         if len(self.domain_list) > 1 and self.use_json:
             self.ptjsonlib.end_error("Cannot test more than 1 domain while --json parameter is present", self.use_json)
 
     def run(self, args) -> None:
         """Main method"""
         ptprinthelper.ptprint("Vulnerable domains:", "TITLE", not self.use_json and self.vulnerable)
-
         self.ptthreads.threads(self.domain_list, self._test_domain, args.threads)
         self.ptjsonlib.set_status("ok")
         ptprinthelper.ptprint(self.ptjsonlib.get_result_json(), "", self.use_json)
 
+
     def _test_domain(self, domain_list: list):
         printlock_ = printlock.PrintLock()
         subdomains = self._prepare_subdomains_for_test(domain_list)
         for subdomain in subdomains:
             self.result_list.append(self._test_subdomain(subdomain, printlock_))
         printlock_.lock_print_output(end="")
 
@@ -68,46 +66,46 @@
         try:
             resolver = dns.resolver.Resolver()
             resolver.timeout = 5
             ip = resolver.resolve(subdomain, "A", lifetime=5)[0].to_text()
             if ip == "127.0.0.1":
                 printlock_.add_string_to_output( ptprinthelper.out_ifnot(f"Vulnerable to same site scripting", "VULN", self.use_json), not self.vulnerable)
                 printlock_.add_string_to_output( ptprinthelper.out_if(subdomain, "", self.vulnerable), self.vulnerable)
-                self.ptjsonlib.add_vulnerability("PTWVSSS", note=subdomain)
+                self.ptjsonlib.add_vulnerability("PTV-SVC-DNS-SSS", note=subdomain)
                 data.update({"vulnerable": True, "ip": ip, "domain": subdomain, "status": "ok"})
             else:
                 printlock_.add_string_to_output( ptprinthelper.out_ifnot(f"Not vulnerable to same site scripting", "NOTVULN", self.use_json), not self.vulnerable)
                 data.update({"vulnerable": False, "ip": ip, "domain": subdomain, "status": "ok"})
         except dns.exception.DNSException:
             printlock_.add_string_to_output( ptprinthelper.out_ifnot(f"{str(sys.exc_info()[1]).split(':')[0]}", "INFO", self.use_json), not self.vulnerable)
             data.update({"vulnerable": False, "domain": subdomain, "status": "ok"})
         return data
 
     def _prepare_subdomains_for_test(self, domain):
-        ext = tldextract.extract(domain)
+        extract = tldparser.parse(domain)
         subdomains = []
         while domain.startswith("."):
             domain = domain[1:]
-        if self.subdomains and ext.subdomain:
-            parsed_domain = ext.subdomain.split(".")
+        if self.subdomains and extract.subdomain:
+            parsed_domain = extract.subdomain.split(".")
             if parsed_domain[0] == "localhost":
                 parsed_domain.pop(0)
             for tested_subdomain_no in range(len(parsed_domain)):
-                subdomains.append("localhost." + ".".join(parsed_domain[tested_subdomain_no:]) + "." + ext.domain + "." + ext.suffix)
-            subdomains.append("localhost." + ext.domain + "." + ext.suffix)
+                subdomains.append("localhost." + ".".join(parsed_domain[tested_subdomain_no:]) + "." + extract.domain + "." + extract.suffix)
+            subdomains.append("localhost." + extract.domain + "." + extract.suffix)
         else:
             if not domain.startswith("localhost"):
                 domain = "localhost." + domain
             subdomains.append(domain)
         return subdomains
 
 
 def get_help():
     return [
-        {"description": ["Same site scripting detection tool"]},
+        {"description": ["Same Site Scripting Detection Tool"]},
         {"usage": ["ptsamesite <options>"]},
         {"usage_example": ["ptsamesite -d example.com", "ptsamesite -d example.com example2.com", "ptsamesite -d subdomain1.subdomain2.example.com -s", "ptsamesite -f domain_list.txt", "ptsamesite -f domains_list.txt -s -V -t 100"]},
         {"options": [
             ["-d",  "--domain",           "<domain>",   "Test domain"],
             ["-f",  "--file",             "<file>",     "Test domains from file"],
             ["-s",  "--subdomains",       "",           "Test all subdomains of given domain (default False)"],
             ["-t",  "--threads",          "<threads>",  "Set number of threads (default 20)"],
@@ -139,13 +137,13 @@
     return args
 
 
 def main():
     global SCRIPTNAME
     SCRIPTNAME = "ptsamesite"
     args = parse_args()
-    script = PtSamesite(args)
+    script = PtSameSite(args)
     script.run(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ptsamesite-1.0.0/ptsamesite.egg-info/PKG-INFO` & `ptsamesite-1.0.1/ptsamesite.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 Metadata-Version: 2.1
 Name: ptsamesite
-Version: 1.0.0
-Summary: Same site scripting detection tool
+Version: 1.0.1
+Summary: Same Site Scripting Detection Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
-License: GPLv3+
+License: GPLv3
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptsamesite
+Project-URL: tracker, https://github.com/penterep/ptsamesite/issues
+Project-URL: changelog, https://github.com/penterep/ptsamesite/blob/main/CHANGELOG.md
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
+Requires-Dist: dnspython>=2.1
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTSAMESITE
-
-> Same site scripting detection tool
-
-ptsamesite is a tool that tests domains for same site scripting vulnerability. <br />
-ptsamesite utilizes threading for fast parallel domain testing.
+# PTSAMESITE - Same Site Scripting Detection Tool
 
+ptsamesite is a tool designed to detect same-site scripting vulnerabilities across various domains.
 
 ## Installation
 
 ```
 pip install ptsamesite
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
 ptsamesite -d example.com                               # Test domain
 ptsamesite -d example.com example2.com                  # Test two domains
 ptsamesite -d subdomain1.subdomain2.example.com -s      # Test domain along with all subdomains
 ptsamesite -f domain_list.txt                           # Test domains from a file
-ptsamesite -f domains_list.txt -s -t 100 -V             # Test domains from a file with all present subdomains, set threads count to 100 and print only vulnerable domains
+ptsamesite -f domains_list.txt -s -t 100 -V             # Test domains from a file with all subdomains, set threads to 100 and print only vulnerable domains
 ```
 
 ## Options
 ```
 -d  --domain      <domain>   Test domain
 -f  --file        <file>     Test domains from file
 -s  --subdomains             Test all subdomains of given domain (default False)
@@ -67,31 +69,21 @@
 -h  --help                   Show this help message and exit
 -j  --json                   Output in JSON format
 ```
 
 
 ## Dependencies
 ```
-dnspython
-tldextract
 ptlibs
-```
-
-## Version History
-```
-1.0.0
-    - Code improvements
-    - Updated for ptlibs 1.0.0
-0.0.1 - 0.0.5
-    - Alpha releases
+dnspython
 ```
 
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
+Copyright (c) 2024 Penterep Security s.r.o.
 
 ptsamesite is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 ptsamesite is distributed in the hope that it will be useful,
```

