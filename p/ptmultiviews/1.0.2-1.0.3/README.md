# Comparing `tmp/ptmultiviews-1.0.2.tar.gz` & `tmp/ptmultiviews-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptmultiviews-1.0.2.tar", last modified: Mon Mar 18 20:37:07 2024, max compression
+gzip compressed data, was "ptmultiviews-1.0.3.tar", last modified: Mon May  6 19:27:58 2024, max compression
```

## Comparing `ptmultiviews-1.0.2.tar` & `ptmultiviews-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-03-18 20:37:07.366087 ptmultiviews-1.0.2/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-18 20:29:24.000000 ptmultiviews-1.0.2/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4146 2024-03-18 20:37:07.366087 ptmultiviews-1.0.2/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3516 2024-03-18 20:29:24.000000 ptmultiviews-1.0.2/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-03-18 20:37:07.366087 ptmultiviews-1.0.2/ptmultiviews/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2024-03-18 20:29:24.000000 ptmultiviews-1.0.2/ptmultiviews/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2024-03-18 20:35:54.000000 ptmultiviews-1.0.2/ptmultiviews/_version.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14268 2024-03-18 20:29:24.000000 ptmultiviews-1.0.2/ptmultiviews/ptmultiviews.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-03-18 20:37:07.366087 ptmultiviews-1.0.2/ptmultiviews.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4146 2024-03-18 20:37:07.000000 ptmultiviews-1.0.2/ptmultiviews.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      323 2024-03-18 20:37:07.000000 ptmultiviews-1.0.2/ptmultiviews.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-03-18 20:37:07.000000 ptmultiviews-1.0.2/ptmultiviews.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       64 2024-03-18 20:37:07.000000 ptmultiviews-1.0.2/ptmultiviews.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       28 2024-03-18 20:37:07.000000 ptmultiviews-1.0.2/ptmultiviews.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       13 2024-03-18 20:37:07.000000 ptmultiviews-1.0.2/ptmultiviews.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2024-03-18 20:37:07.366087 ptmultiviews-1.0.2/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)      989 2024-03-18 20:29:24.000000 ptmultiviews-1.0.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 19:27:58.686684 ptmultiviews-1.0.3/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2024-04-29 08:26:15.000000 ptmultiviews-1.0.3/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-06 19:27:58.686684 ptmultiviews-1.0.3/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     3596 2024-05-06 19:22:48.000000 ptmultiviews-1.0.3/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 19:27:58.686684 ptmultiviews-1.0.3/ptmultiviews/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:15.000000 ptmultiviews-1.0.3/ptmultiviews/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-04-29 08:26:15.000000 ptmultiviews-1.0.3/ptmultiviews/_version.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    15479 2024-05-06 14:04:14.000000 ptmultiviews-1.0.3/ptmultiviews/ptmultiviews.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 19:27:58.686684 ptmultiviews-1.0.3/ptmultiviews.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-06 19:27:58.000000 ptmultiviews-1.0.3/ptmultiviews.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      323 2024-05-06 19:27:58.000000 ptmultiviews-1.0.3/ptmultiviews.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-06 19:27:58.000000 ptmultiviews-1.0.3/ptmultiviews.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       64 2024-05-06 19:27:58.000000 ptmultiviews-1.0.3/ptmultiviews.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-06 19:27:58.000000 ptmultiviews-1.0.3/ptmultiviews.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2024-05-06 19:27:58.000000 ptmultiviews-1.0.3/ptmultiviews.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-06 19:27:58.686684 ptmultiviews-1.0.3/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1255 2024-05-06 19:27:44.000000 ptmultiviews-1.0.3/setup.py
```

### Comparing `ptmultiviews-1.0.2/LICENSE` & `ptmultiviews-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ptmultiviews-1.0.2/PKG-INFO` & `ptmultiviews-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: ptmultiviews
-Version: 1.0.2
+Version: 1.0.3
 Summary: Apache Multiviews Detection & Enumeration Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
-License: GPLv3+
+License: GPLv3
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptmultiviews
+Project-URL: tracker, https://github.com/penterep/ptmultiviews/issues
+Project-URL: changelog, https://github.com/penterep/ptmultiviews/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ptlibs<2,>=1.0.6
-Requires-Dist: validators
+Requires-Dist: ptlibs<2,>=1.0.7
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTMULTIVIEWS
-> Apache Multiviews Detection & Enumeration Tool
-
+## PTMULTIVIEWS - Apache Multiviews Detection & Enumeration Tool
 
 ## Installation
 ```
 pip install ptmultiviews
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
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
 source ~/.zshrc
 ```
 
 ## Usage examples
 
@@ -54,18 +55,18 @@
 ```
 
 
 ### Options:
 
 ```
 -u   --url                 <url>           Connect to URL
--f   --file                <file>          Load list of URLs from file
--d   --domain              <domain>        Domain to test (used with --file option)
+-f   --file                <file>          Load list of URLs / filepaths
+-df  --domain-file         <domain-file>   Load list of domains to mass scan (defaults to favicon.ico)
 -co  --check-only                          Check for multiviews without enumerating
--wr  --with-requested-url                  Includes requested source among enumerated results
+-wr  --with-requested-url                  Include requested source among enumerated results
 -wd  --without-domain                      Enumerated files will be printed without domain
 -t   --threads             <threads>       Set number of threads (default 20)
 -p   --proxy               <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
 -T   --timeout             <timeout>       Set timeout (default 10)
 -a   --user-agent          <agent>         Set User-Agent
 -c   --cookie              <cookie>        Set Cookie(s)
 -H   --headers             <header:value>  Set Header(s)
@@ -76,15 +77,14 @@
 -h   --help                                Show this help message and exit
 -j   --json                                Output in JSON format
 ```
 
 ## Dependencies
 
 ```
-validators
 ptlibs
 ```
 
 
 ## License
 
 Copyright (c) 2024 Penterep Security s.r.o.
```

### Comparing `ptmultiviews-1.0.2/README.md` & `ptmultiviews-1.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTMULTIVIEWS
-> Apache Multiviews Detection & Enumeration Tool
-
+## PTMULTIVIEWS - Apache Multiviews Detection & Enumeration Tool
 
 ## Installation
 ```
 pip install ptmultiviews
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
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
 source ~/.zshrc
 ```
 
 ## Usage examples
 
@@ -35,18 +33,18 @@
 ```
 
 
 ### Options:
 
 ```
 -u   --url                 <url>           Connect to URL
--f   --file                <file>          Load list of URLs from file
--d   --domain              <domain>        Domain to test (used with --file option)
+-f   --file                <file>          Load list of URLs / filepaths
+-df  --domain-file         <domain-file>   Load list of domains to mass scan (defaults to favicon.ico)
 -co  --check-only                          Check for multiviews without enumerating
--wr  --with-requested-url                  Includes requested source among enumerated results
+-wr  --with-requested-url                  Include requested source among enumerated results
 -wd  --without-domain                      Enumerated files will be printed without domain
 -t   --threads             <threads>       Set number of threads (default 20)
 -p   --proxy               <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
 -T   --timeout             <timeout>       Set timeout (default 10)
 -a   --user-agent          <agent>         Set User-Agent
 -c   --cookie              <cookie>        Set Cookie(s)
 -H   --headers             <header:value>  Set Header(s)
@@ -57,15 +55,14 @@
 -h   --help                                Show this help message and exit
 -j   --json                                Output in JSON format
 ```
 
 ## Dependencies
 
 ```
-validators
 ptlibs
 ```
 
 
 ## License
 
 Copyright (c) 2024 Penterep Security s.r.o.
```

### Comparing `ptmultiviews-1.0.2/ptmultiviews/ptmultiviews.py` & `ptmultiviews-1.0.3/ptmultiviews/ptmultiviews.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,220 +17,232 @@
     You should have received a copy of the GNU General Public License
     along with ptmultiviews.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import argparse
 import copy
 import re
-import sys; sys.path.append(__file__.rsplit("/", 1)[0])
-import typing
+import sys
+import urllib.parse; sys.path.append(__file__.rsplit("/", 1)[0])
 import urllib
 
 import requests
-import validators
 
 from _version import __version__
 from ptlibs import ptjsonlib, ptmisclib, ptnethelper, ptprinthelper, ptpathtypedetector
 from ptlibs.threads import ptthreads
 
 
 class PtMultiviews:
     def __init__(self, args):
         self.ptjsonlib            = ptjsonlib.PtJsonLib()
         self.ptthreads            = ptthreads.PtThreads()
         self.ptpathtypedetector   = ptpathtypedetector.PtPathTypeDetector()
         self.without_domain       = args.without_domain
         self.with_requested_url   = args.with_requested_url
         self.use_json             = args.json
-        self.path_list            = []
-
-        # Test type
-        self.url_test             = None # only url
-        self.file_test            = None # only file
-        self.domain_file_test     = None # domain + file combo
-
-        # Requests args
-        self.output_file          = self._get_output_file(args.output) if args.output else None
-        self.headers              = ptnethelper.get_request_headers(args)
-        self.proxies              = {"http": args.proxy, "https": args.proxy}
         self.timeout              = args.timeout
         self.cache                = args.cache
         self.redirects            = args.redirects
+        self.output_file          = args.output
+        self.proxies              = {"http": args.proxy, "https": args.proxy}
+        self.headers              = ptnethelper.get_request_headers(args)
 
-    def run(self, args):
-        """Main method"""
-        self.url_list             = self._get_urls(args)
+        # Test type
+        self.url_test             = None
+        self.file_test            = None
+        self.url_file_test        = None
+        self.domain_file_test     = None
+
+        self.url_list             = self._get_urls_and_set_test_type(args)
         self.original_url_list    = copy.copy(self.url_list)
+        self.result_path_list     = []
+
 
+    def run(self, args):
+        """Main method"""
         if self.url_test:
+            # URL only test
             if self._is_vulnerable(self.url_list[0]) and not args.check_only:
                 ptprinthelper.ptprint("Enumerated:", "TITLE", not self.use_json, newline_above=True, colortext=True)
                 self.ptthreads.threads(self.url_list, self._enumerate_files, 1)
 
-        elif self.domain_file_test:
-                ptprinthelper.ptprint("Enumerated:", "TITLE", not self.use_json, newline_above=True, colortext=True)
-                self.ptthreads.threads(self.url_list, self._enumerate_files, args.threads)
+        elif self.url_file_test:
+            # URL + Filepaths
+            ptprinthelper.ptprint("Enumerated:", "TITLE", not self.use_json, newline_above=True, colortext=True)
+            self.ptthreads.threads(self.url_list, self._enumerate_files, args.threads)
 
         elif self.file_test:
+            # URLs from file
             ptprinthelper.ptprint("Enumerated:", "TITLE", not self.use_json, newline_above=True, colortext=True)
             self.ptthreads.threads(self.url_list, self._enumerate_files, args.threads)
 
-        ptprinthelper.ptprint('\n'.join(sorted(self.path_list)), "", not self.use_json)
+        elif self.domain_file_test:
+            # Domains from file
+            ptprinthelper.ptprint("Vulnerable domains:", "TITLE", not self.use_json, newline_above=True, colortext=True)
+            self.ptthreads.threads(self.url_list, self._is_vulnerable, args.threads)
+
+        ptprinthelper.ptprint('\n'.join(sorted(self.result_path_list)), "", not self.use_json)
+
+        if not self.result_path_list:
+            ptprinthelper.ptprint("No alternatives to enumerate")
 
         if self.output_file:
-            if self.path_list:
-                self.output_file.write('\n'.join(self.path_list))
-                self.output_file.write('\n')
-                ptprinthelper.ptprint(f"Output saved successfully to: {args.output}", "", not self.use_json, newline_above=True)
-            self.output_file.close()
+            self._write_output_to_file(args.output)
 
         self.ptjsonlib.set_status("finished")
         ptprinthelper.ptprint(self.ptjsonlib.get_result_json(), condition=self.use_json)
 
     def _is_vulnerable(self, url: str) -> bool:
         """Checks whether <url> is vulnerable to multiviews"""
-        STATUS_CODES = [200, 301, 302]
         malformed_url = self._strip_url_extension(url)
         try:
             response, response_dump = ptmisclib.load_url_from_web_or_temp(url=malformed_url, method="GET", headers=self.headers, proxies=self.proxies, timeout=self.timeout, redirects=self.redirects, verify=False, cache=self.cache, dump_response=True)
         except requests.exceptions.RequestException as e:
-            self.ptjsonlib.end_error(f"Cannot connect to website: {e}", self.use_json)
+            if not self.domain_file_test: self.ptjsonlib.end_error(f"Cannot connect to website: {e}", self.use_json)
+            return
 
-        ptprinthelper.ptprint(f"Testing URL: {response.url}", "INFO", not self.use_json)
-        ptprinthelper.ptprint(f"Status code: {response.status_code}", "INFO", not self.use_json)
+        ptprinthelper.ptprint(f"Testing URL: {response.url}", "INFO", not self.use_json and not self.domain_file_test)
+        ptprinthelper.ptprint(f"Status code: {response.status_code}", "INFO", not self.use_json and not self.domain_file_test)
 
         # Checks whether multiviews enabled
-        if response.status_code in STATUS_CODES and response.headers.get("Vary") and "negotiate" in response.headers.get("Vary"):
-            ptprinthelper.ptprint(f"Multiviews: Enabled", "VULN", not self.use_json)
-            self.ptjsonlib.add_vulnerability("PTV-WEB-MULTIVIEWS", request=response_dump["request"], response=response_dump["response"])
+        if response.status_code in [200, 301, 302] and response.headers.get("Vary") and "negotiate" in response.headers.get("Vary"):
+            if self.domain_file_test:
+                ptprinthelper.ptprint(urllib.parse.urlparse(response.url).netloc, "", not self.use_json)
+            ptprinthelper.ptprint(f"Multiviews: Enabled", "VULN", not self.use_json and not self.domain_file_test)
+            self.ptjsonlib.add_vulnerability("PTV-WEB-DISCO-MVIEWS", vuln_request=response_dump["request"], vuln_response=response_dump["response"])
             return True
         else:
-            ptprinthelper.ptprint(f"Multiviews: Disabled", "NOTVULN", not self.use_json)
+            ptprinthelper.ptprint(f"Multiviews: Disabled", "NOTVULN", not self.use_json and not self.domain_file_test)
             return False
 
     def _enumerate_files(self, url: str) -> None:
         """Enumerate files from URL"""
         original_url = url
         malformed_url = self._strip_url_extension(url)
         headers = dict({"Accept": "foo/foo"}, **self.headers)
-
         try:
             response = ptmisclib.load_url_from_web_or_temp(url=malformed_url, method="GET", headers=headers, proxies=self.proxies, timeout=self.timeout, redirects=self.redirects, verify=False, cache=self.cache)
         except requests.exceptions.RequestException as e:
-            self.ptjsonlib.end_error(f"Cannot connect to: {original_url}", self.use_json)
+            if self.url_test: self.ptjsonlib.end_error(f"Cannot connect to: {original_url}", self.use_json)
+            return
 
         if response.status_code == 406:
             enumerated_files = re.findall('<a href="(.*)">', response.text)
             for found_file in enumerated_files:
                 abs_path = f"{url.rsplit('/', 1)[0]}/{found_file}"
                 rel_path = f"{url.split('/', 3)[-1]}/{found_file}"
-                if abs_path in self.original_url_list and not self.with_requested_url:
+                if abs_path == original_url and not self.with_requested_url:
                     continue
                 path = abs_path if not self.without_domain else rel_path
-                if path not in self.path_list:
-                    self.path_list.append(path)
+                if path not in self.result_path_list:
+                    self.result_path_list.append(path)
                     if self.use_json:
                         self.ptjsonlib.add_node(self.ptjsonlib.create_node_object("webpage", properties={"url": abs_path, "name": found_file, "WebPageType": self.ptpathtypedetector.get_type(path)}))
 
     def _strip_url_extension(self, url: str) -> str:
-        o = urllib.parse.urlparse(url)
-        path = o.path.rsplit("/", 1)
+        parsed = urllib.parse.urlparse(url)
+        path = parsed.path.rsplit("/", 1)
         if "." in path[-1]:
             new_path = f"{path[0]}/{path[-1].split('.', 1)[0]}"
-            o = o._replace(path=new_path)
-        return urllib.parse.urlunparse(o)
-
-    def _get_urls(self, args: argparse.Namespace) -> list:
-        """Returns list of URLs"""
+            parsed = parsed._replace(path=new_path)
+        return urllib.parse.urlunparse(parsed)
 
-        if args.url and not (args.file and args.domain):
+    def _get_urls_and_set_test_type(self, args: argparse.Namespace) -> list:
+        if args.url and not args.file and not args.domain_file:
             self.url_test = True
             return [self._parse_url(args.url)]
 
-        elif (args.domain and args.file) and not args.url:
-            self.domain_file_test = True
-            domain = self._adjust_domain(domain)
-            url_list = self._read_file(args.file, domain)
-            return url_list
+        elif (args.url and args.file) and not args.domain_file:
+            self.url_file_test = True
+            base_url =  args.url + "/" if not urllib.parse.urlparse(args.url).path.endswith("/") else args.url
+            try:
+                with open(args.file, 'r') as file:
+                    url_list = [base_url + path.strip("/").strip() for line in file for path in [self.extract_path(line.strip())] if path.strip("/")]
+                    return list(set(url_list))
+            except (IOError, FileNotFoundError) as e:
+                self.ptjsonlib.end_error(f"Cannot read file - {e}", self.use_json)
 
         elif args.file and not (args.url and args.domain):
             self.file_test = True
-            url_list = self._read_file(args.file)
-            return url_list
+            try:
+                with open(args.file, 'r') as file:
+                    url_list = [line.strip() for line in file.readlines() if self._is_valid_url(line.strip())]
+                    return list(set(url_list))
+            except (IOError, FileNotFoundError) as e:
+                self.ptjsonlib.end_error(f"Cannot read file - {e}", self.use_json)
+
+        elif args.domain_file:
+            if self.use_json: self.ptjsonlib.end_error("Cannot use --json option with -df/--domain-file", self.use_json)
+            self.domain_file_test = True
+            try:
+                with open(args.domain_file, 'r') as file:
+                    url_list = [f"https://{line.strip()}/favicon.ico" for line in file if line.strip()]
+                    return url_list
+            except (FileNotFoundError, IOError):
+                self.ptjsonlib.end_error(f"Error reading from file - {args.domain_file}", self.use_json)
 
-        elif args.domain and not args.file:
-            self.ptjsonlib.end_error("To use --domain parameter you need to supply --file parameter", self.use_json)
         else:
             self.ptjsonlib.end_error("Bad argument combination, see --help", self.use_json)
 
+    def _is_valid_url(self, url):
+        parsed = urllib.parse.urlparse(url)
+        return bool(parsed.scheme) and bool(parsed.netloc)
+
     def _adjust_domain(self, domain: str) -> str:
         """Adjusts provided <domain>"""
-        o = urllib.parse.urlparse(domain)
-        self._check_scheme(o.scheme)
-        return domain + "/" if not o.path.endswith("/") else domain
+        parsed = urllib.parse.urlparse(domain)
+        self._check_scheme(parsed.scheme)
+        return domain + "/" if not parsed.path.endswith("/") else domain
 
     def _parse_url(self, url: str) -> str:
         """Checks whether the provided url is valid"""
-        o = urllib.parse.urlparse(url)
-        self._check_scheme(o.scheme)
-        if len(o.path) in [0, 1]:
+        parsed = urllib.parse.urlparse(url)
+        self._check_scheme(parsed.scheme)
+        if len(parsed.path) in [0, 1]:
             self.ptjsonlib.end_error(f"URL with PATH to file is required (e.g. https://www.example.com/index.php)", self.use_json)
-        return f"{o.scheme}://{o.netloc}{o.path}"
+        return f"{parsed.scheme}://{parsed.netloc}{parsed.path}"
 
     def _check_scheme(self, scheme: str) -> None:
         """Checks whether provided scheme is valid"""
         if not re.match("http[s]?$", scheme):
             self.ptjsonlib.end_error(f"Missing or invalid scheme, supported schemes are: [HTTP, HTTPS]", self.use_json)
 
-    def _read_file(self, filepath: str, domain: str = None) -> list:
-        ptprinthelper.ptprint(f"Reading file: {filepath}", "TITLE", not self.use_json)
-        try:
-            with open(filepath, 'r') as fh:
-                url_list = []
-                for line in fh.readlines():
-                    line = line.strip()
-                    if domain:
-                        path = urllib.parse.urlparse(line).path
-                        while path.startswith("/"): path = path[1:]
-                        while path.endswith("/"): path = path[:-1]
-                        if not path: continue
-                        url_list.append(domain+path)
-                    else:
-                        if validators.url(line) and re.match("http[s]?$", urllib.parse.urlparse(line).scheme):
-                            url_list.append(line)
-            return list(set(url_list))
-
-        except (IOError, FileNotFoundError) as e:
-            self.ptjsonlib.end_error(f"Cannot read file - {e}", self.use_json)
+    def extract_path(self, url_or_filepath):
+        parsed = urllib.parse.urlparse(url_or_filepath)
+        return parsed.path if parsed.scheme else url_or_filepath
 
-    def _get_output_file(self, filepath: str) -> typing.TextIO:
-        """returns <output_file> file handler"""
+    def _write_output_to_file(self, output_file):
         try:
-            output_file = open(filepath, 'a')
-            return output_file
-        except IOError as e:
-            self.ptjsonlib.end_error(f"Cannot output to file - {e}", self.use_json)
+            with open(output_file, 'a') as file:
+                if self.result_path_list:
+                    file.write('\n'.join(self.result_path_list) + "\n")
+                ptprinthelper.ptprint(f"Output saved successfully to: {output_file}", "", not self.use_json, newline_above=True)
+        except (FileNotFoundError, IOError) as e:
+            ptprinthelper.ptprint(f"Cannot output to file - {e}", "ERROR", condition=not self.use_json)
+
 
 def get_help():
     return [
-        {"description": ["Apache Multiviews detection & enumeration tool"]},
+        {"description": ["Apache Multiviews Detection & Enumeration Tool"]},
         {"usage": ["ptmultiviews <options>"]},
         {"tip": ["Use this program against existing web resources (eg. https://www.example.com/index.php)"]},
         {"usage_example": [
             "ptmultiviews -u https://www.example.com/",
             "ptmultiviews -u https://www.example.com/ --check-only",
             "ptmultiviews -d https://www.example.com/ -f filepaths.txt",
             "ptmultiviews -f urlList.txt",
+            "ptmultiviews -df domainList.txt",
         ]},
         {"options": [
             ["-u",   "--url",                    "<url>",            "Connect to URL"],
-            ["-f",   "--file",                   "<file>",           "Load list of URLs from file"],
-            ["-d",   "--domain",                 "<domain>",         "Domain to test (used with --file option)"],
+            ["-f",   "--file",                   "<file>",           "Load list of URLs / filepaths"],
+            ["-df",  "--domain-file",            "<domain-file>",    "Load list of domains to mass scan (defaults to favicon.ico)"],
             ["-co",  "--check-only",             "",                 "Check for multiviews without enumerating"],
-            ["-wr",  "--with-requested-url",     "",                 "Includes requested source among enumerated results"],
+            ["-wr",  "--with-requested-url",     "",                 "Include requested source among enumerated results"],
             ["-wd",  "--without-domain",         "",                 "Enumerated files will be printed without domain"],
             ["-t",   "--threads",                "<threads>",        "Set number of threads (default 20)"],
             ["-p",   "--proxy",                  "<proxy>",          "Set proxy (e.g. http://127.0.0.1:8080)"],
             ["-T",   "--timeout",                "<timeout>",        "Set timeout (default 10)"],
             ["-a",   "--user-agent",             "<agent>",          "Set User-Agent"],
             ["-c",   "--cookie",                 "<cookie>",         "Set Cookie(s)"],
             ["-H",   "--headers",                "<header:value>",   "Set Header(s)"],
@@ -244,21 +256,22 @@
         }]
 
 
 def parse_args():
     parser = argparse.ArgumentParser(usage=f"{SCRIPTNAME} <options>")
     parser.add_argument("-u",  "--url",                  type=str)
     parser.add_argument("-d",  "--domain",               type=str)
+    parser.add_argument("-df", "--domain-file",          type=str)
     parser.add_argument("-f",  "--file",                 type=str)
     parser.add_argument("-o",  "--output",               type=str)
     parser.add_argument("-T",  "--timeout",              type=int, default=10)
     parser.add_argument("-t",  "--threads",              type=int, default=20)
     parser.add_argument("-p",  "--proxy",                type=str)
     parser.add_argument("-c",  "--cookie",               type=str)
-    parser.add_argument("-a", "--user-agent",            type=str, default="Penterep Tools")
+    parser.add_argument("-a",  "--user-agent",           type=str, default="Penterep Tools")
     parser.add_argument("-H",  "--headers",              type=ptmisclib.pairs)
     parser.add_argument("-co", "--check-only",           action="store_true")
     parser.add_argument("-wd", "--without-domain",       action="store_true")
     parser.add_argument("-wr", "--with-requested-url",   action="store_true")
     parser.add_argument("-r",  "--redirects",            action="store_true")
     parser.add_argument("-C",  "--cache",                action="store_true")
     parser.add_argument("-v",  "--version",              action="version", version=f"{SCRIPTNAME} {__version__}")
```

### Comparing `ptmultiviews-1.0.2/ptmultiviews.egg-info/PKG-INFO` & `ptmultiviews-1.0.3/ptmultiviews.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: ptmultiviews
-Version: 1.0.2
+Version: 1.0.3
 Summary: Apache Multiviews Detection & Enumeration Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
-License: GPLv3+
+License: GPLv3
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptmultiviews
+Project-URL: tracker, https://github.com/penterep/ptmultiviews/issues
+Project-URL: changelog, https://github.com/penterep/ptmultiviews/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ptlibs<2,>=1.0.6
-Requires-Dist: validators
+Requires-Dist: ptlibs<2,>=1.0.7
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTMULTIVIEWS
-> Apache Multiviews Detection & Enumeration Tool
-
+## PTMULTIVIEWS - Apache Multiviews Detection & Enumeration Tool
 
 ## Installation
 ```
 pip install ptmultiviews
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
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
 source ~/.zshrc
 ```
 
 ## Usage examples
 
@@ -54,18 +55,18 @@
 ```
 
 
 ### Options:
 
 ```
 -u   --url                 <url>           Connect to URL
--f   --file                <file>          Load list of URLs from file
--d   --domain              <domain>        Domain to test (used with --file option)
+-f   --file                <file>          Load list of URLs / filepaths
+-df  --domain-file         <domain-file>   Load list of domains to mass scan (defaults to favicon.ico)
 -co  --check-only                          Check for multiviews without enumerating
--wr  --with-requested-url                  Includes requested source among enumerated results
+-wr  --with-requested-url                  Include requested source among enumerated results
 -wd  --without-domain                      Enumerated files will be printed without domain
 -t   --threads             <threads>       Set number of threads (default 20)
 -p   --proxy               <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
 -T   --timeout             <timeout>       Set timeout (default 10)
 -a   --user-agent          <agent>         Set User-Agent
 -c   --cookie              <cookie>        Set Cookie(s)
 -H   --headers             <header:value>  Set Header(s)
@@ -76,15 +77,14 @@
 -h   --help                                Show this help message and exit
 -j   --json                                Output in JSON format
 ```
 
 ## Dependencies
 
 ```
-validators
 ptlibs
 ```
 
 
 ## License
 
 Copyright (c) 2024 Penterep Security s.r.o.
```

