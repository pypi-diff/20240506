# Comparing `tmp/octodns-selectel-0.99.2.tar.gz` & `tmp/octodns_selectel-0.99.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-selectel-0.99.2.tar", last modified: Thu Mar 14 22:02:35 2024, max compression
+gzip compressed data, was "octodns_selectel-0.99.3.tar", last modified: Mon May  6 14:35:38 2024, max compression
```

## Comparing `octodns-selectel-0.99.2.tar` & `octodns_selectel-0.99.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-14 22:02:35.523376 octodns-selectel-0.99.2/
--rw-r--r--   0 ross       (501) staff       (20)     1129 2023-10-19 01:55:58.000000 octodns-selectel-0.99.2/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)     7092 2024-03-14 22:02:35.522329 octodns-selectel-0.99.2/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     6038 2024-02-01 14:54:53.000000 octodns-selectel-0.99.2/README.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-14 22:02:35.506274 octodns-selectel-0.99.2/octodns_selectel/
--rw-r--r--   0 ross       (501) staff       (20)      272 2024-02-01 15:24:08.000000 octodns-selectel-0.99.2/octodns_selectel/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)      120 2024-03-14 21:58:21.000000 octodns-selectel-0.99.2/octodns_selectel/escaping_semicolon.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-14 22:02:35.510718 octodns-selectel-0.99.2/octodns_selectel/v1/
--rw-r--r--   0 ross       (501) staff       (20)        0 2024-02-01 22:29:50.000000 octodns-selectel-0.99.2/octodns_selectel/v1/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)    12142 2024-03-14 21:58:21.000000 octodns-selectel-0.99.2/octodns_selectel/v1/provider.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-14 22:02:35.515324 octodns-selectel-0.99.2/octodns_selectel/v2/
--rw-r--r--   0 ross       (501) staff       (20)        0 2024-02-01 22:29:50.000000 octodns-selectel-0.99.2/octodns_selectel/v2/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)     3177 2024-02-01 15:24:08.000000 octodns-selectel-0.99.2/octodns_selectel/v2/dns_client.py
--rw-r--r--   0 ross       (501) staff       (20)      152 2024-02-01 14:54:53.000000 octodns-selectel-0.99.2/octodns_selectel/v2/exceptions.py
--rw-r--r--   0 ross       (501) staff       (20)     4157 2024-03-14 21:58:21.000000 octodns-selectel-0.99.2/octodns_selectel/v2/mappings.py
--rw-r--r--   0 ross       (501) staff       (20)     6495 2024-02-01 15:24:08.000000 octodns-selectel-0.99.2/octodns_selectel/v2/provider.py
--rw-r--r--   0 ross       (501) staff       (20)       70 2024-03-14 22:02:17.000000 octodns-selectel-0.99.2/octodns_selectel/version.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-14 22:02:35.517124 octodns-selectel-0.99.2/octodns_selectel.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     7092 2024-03-14 22:02:35.000000 octodns-selectel-0.99.2/octodns_selectel.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      582 2024-03-14 22:02:35.000000 octodns-selectel-0.99.2/octodns_selectel.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2024-03-14 22:02:35.000000 octodns-selectel-0.99.2/octodns_selectel.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)      246 2024-03-14 22:02:35.000000 octodns-selectel-0.99.2/octodns_selectel.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       23 2024-03-14 22:02:35.000000 octodns-selectel-0.99.2/octodns_selectel.egg-info/top_level.txt
--rw-r--r--   0 ross       (501) staff       (20)      429 2023-11-29 21:55:08.000000 octodns-selectel-0.99.2/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2024-03-14 22:02:35.523596 octodns-selectel-0.99.2/setup.cfg
--rwxr-xr-x   0 ross       (501) staff       (20)     1654 2024-02-01 15:24:08.000000 octodns-selectel-0.99.2/setup.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-03-14 22:02:35.516270 octodns-selectel-0.99.2/tests/
--rw-r--r--   0 ross       (501) staff       (20)        0 2024-02-01 14:54:53.000000 octodns-selectel-0.99.2/tests/__init__.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-05-06 14:35:38.287879 octodns_selectel-0.99.3/
+-rw-r--r--   0 ross       (501) staff       (20)     1129 2023-10-19 01:55:58.000000 octodns_selectel-0.99.3/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)     7328 2024-05-06 14:35:38.286833 octodns_selectel-0.99.3/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     6226 2024-04-17 17:26:56.000000 octodns_selectel-0.99.3/README.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-05-06 14:35:38.268424 octodns_selectel-0.99.3/octodns_selectel/
+-rw-r--r--   0 ross       (501) staff       (20)      272 2024-02-01 15:24:08.000000 octodns_selectel-0.99.3/octodns_selectel/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)      120 2024-03-14 21:58:21.000000 octodns_selectel-0.99.3/octodns_selectel/escaping_semicolon.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-05-06 14:35:38.272511 octodns_selectel-0.99.3/octodns_selectel/v1/
+-rw-r--r--   0 ross       (501) staff       (20)        0 2024-02-01 22:29:50.000000 octodns_selectel-0.99.3/octodns_selectel/v1/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)    12142 2024-03-14 21:58:21.000000 octodns_selectel-0.99.3/octodns_selectel/v1/provider.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-05-06 14:35:38.278591 octodns_selectel-0.99.3/octodns_selectel/v2/
+-rw-r--r--   0 ross       (501) staff       (20)        0 2024-02-01 22:29:50.000000 octodns_selectel-0.99.3/octodns_selectel/v2/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     3177 2024-02-01 15:24:08.000000 octodns_selectel-0.99.3/octodns_selectel/v2/dns_client.py
+-rw-r--r--   0 ross       (501) staff       (20)      152 2024-02-01 14:54:53.000000 octodns_selectel-0.99.3/octodns_selectel/v2/exceptions.py
+-rw-r--r--   0 ross       (501) staff       (20)     4763 2024-04-17 17:26:56.000000 octodns_selectel-0.99.3/octodns_selectel/v2/mappings.py
+-rw-r--r--   0 ross       (501) staff       (20)     6654 2024-04-17 17:26:56.000000 octodns_selectel-0.99.3/octodns_selectel/v2/provider.py
+-rw-r--r--   0 ross       (501) staff       (20)       70 2024-05-06 14:35:27.000000 octodns_selectel-0.99.3/octodns_selectel/version.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-05-06 14:35:38.280619 octodns_selectel-0.99.3/octodns_selectel.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)     7328 2024-05-06 14:35:38.000000 octodns_selectel-0.99.3/octodns_selectel.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      582 2024-05-06 14:35:38.000000 octodns_selectel-0.99.3/octodns_selectel.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-05-06 14:35:38.000000 octodns_selectel-0.99.3/octodns_selectel.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)      263 2024-05-06 14:35:38.000000 octodns_selectel-0.99.3/octodns_selectel.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       23 2024-05-06 14:35:38.000000 octodns_selectel-0.99.3/octodns_selectel.egg-info/top_level.txt
+-rw-r--r--   0 ross       (501) staff       (20)      429 2023-11-29 21:55:08.000000 octodns_selectel-0.99.3/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2024-05-06 14:35:38.288117 octodns_selectel-0.99.3/setup.cfg
+-rwxr-xr-x   0 ross       (501) staff       (20)     1819 2024-04-17 17:54:47.000000 octodns_selectel-0.99.3/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-05-06 14:35:38.279936 octodns_selectel-0.99.3/tests/
+-rw-r--r--   0 ross       (501) staff       (20)        0 2024-02-01 14:54:53.000000 octodns_selectel-0.99.3/tests/__init__.py
```

### Comparing `octodns-selectel-0.99.2/LICENSE` & `octodns_selectel-0.99.3/LICENSE`

 * *Files identical despite different names*

### Comparing `octodns-selectel-0.99.2/PKG-INFO` & `octodns_selectel-0.99.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-selectel
-Version: 0.99.2
+Version: 0.99.3
 Summary:  Selectel DNS provider for octoDNS
 Home-page: https://github.com/octodns/octodns-selectel
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -12,16 +12,17 @@
 Requires-Dist: octodns>=0.9.14
 Requires-Dist: requests>=2.27.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-network; extra == "dev"
 Requires-Dist: requests_mock; extra == "dev"
-Requires-Dist: black<24.0.0,>=23.1.0; extra == "dev"
+Requires-Dist: black<25.0.0,>=24.3.0; extra == "dev"
 Requires-Dist: build>=0.7.0; extra == "dev"
+Requires-Dist: docutils<=0.20.1; extra == "dev"
 Requires-Dist: isort>=5.11.5; extra == "dev"
 Requires-Dist: pyflakes>=2.2.0; extra == "dev"
 Requires-Dist: readme_renderer[md]>=26.0; extra == "dev"
 Requires-Dist: twine>=3.4.2; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -49,15 +50,15 @@
 pip install octodns octodns-selectel
 ```
 
 ## Capabilities
 
 | What              | Value                                             |
 |-------------------|---------------------------------------------------|
-| Supported records | A, AAAA, ALIAS, CNAME, MX, NS, SRV, SSHFP, TXT    |
+| Supported records | A, AAAA, ALIAS, CAA, CNAME, DNAME, MX, NS, SRV, SSHFP, TXT    |
 | Dynamic records   | ❌ |
 
 ## Configuration
 Add selectel provider to `config.yaml`.
 ```yaml
 providers:
   selectel:
@@ -137,14 +138,27 @@
       target: phone1.example.com.
       weight: 60
     - port: 5030
       priority: 20
       target: phone2.example.com.
       weight: 0     
 
+caa:
+  - ttl: 3600
+    type: CAA
+    values:
+    - flags: 0
+      tag: issue
+      value: octodns-test.com.
+
+dname:
+  - ttl: 3600
+    type: DNAME
+    value: octodns-test.com.
+
 foo:
   - ttl: 3600
     type: CNAME
     value: bar.octodns-test.com.
 
 sshfp:
   - ttl: 3600
```

### Comparing `octodns-selectel-0.99.2/README.md` & `octodns_selectel-0.99.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 pip install octodns octodns-selectel
 ```
 
 ## Capabilities
 
 | What              | Value                                             |
 |-------------------|---------------------------------------------------|
-| Supported records | A, AAAA, ALIAS, CNAME, MX, NS, SRV, SSHFP, TXT    |
+| Supported records | A, AAAA, ALIAS, CAA, CNAME, DNAME, MX, NS, SRV, SSHFP, TXT    |
 | Dynamic records   | ❌ |
 
 ## Configuration
 Add selectel provider to `config.yaml`.
 ```yaml
 providers:
   selectel:
@@ -107,14 +107,27 @@
       target: phone1.example.com.
       weight: 60
     - port: 5030
       priority: 20
       target: phone2.example.com.
       weight: 0     
 
+caa:
+  - ttl: 3600
+    type: CAA
+    values:
+    - flags: 0
+      tag: issue
+      value: octodns-test.com.
+
+dname:
+  - ttl: 3600
+    type: DNAME
+    value: octodns-test.com.
+
 foo:
   - ttl: 3600
     type: CNAME
     value: bar.octodns-test.com.
 
 sshfp:
   - ttl: 3600
```

### Comparing `octodns-selectel-0.99.2/octodns_selectel/v1/provider.py` & `octodns_selectel-0.99.3/octodns_selectel/v1/provider.py`

 * *Files identical despite different names*

### Comparing `octodns-selectel-0.99.2/octodns_selectel/v2/dns_client.py` & `octodns_selectel-0.99.3/octodns_selectel/v2/dns_client.py`

 * *Files identical despite different names*

### Comparing `octodns-selectel-0.99.2/octodns_selectel/v2/mappings.py` & `octodns_selectel-0.99.3/octodns_selectel/v2/mappings.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,28 +7,38 @@
 
 from .exceptions import SelectelException
 
 
 def to_selectel_rrset(record):
     rrset = dict(name=record.fqdn, ttl=record.ttl, type=record._type)
     rrset_records = []
+    content_caa_tmpl = Template("$flag $tag \"$value\"")
     content_mx_tmpl = Template("$preference $exchange")
     content_srv_tmpl = Template("$priority $weight $port $target")
     content_sshfp_tmpl = Template("$algorithm $fingerprint_type $fingerprint")
     if record._type in {"A", "AAAA", "NS"}:
         rrset_records = list(
             map(lambda value: {'content': value}, record.values)
         )
-    elif record._type in {"CNAME", "ALIAS"}:
+    elif record._type in {"CNAME", "ALIAS", "DNAME"}:
         rrset_records = [{'content': record.value}]
     elif record._type == "TXT":
         rrset_records = [
             dict(content=f'\"{unescape_semicolon(value)}\"')
             for value in record.values
         ]
+    elif record._type == "CAA":
+        rrset_records = [
+            dict(
+                content=content_caa_tmpl.substitute(
+                    flag=value.flags, tag=value.tag, value=value.value
+                )
+            )
+            for value in record.values
+        ]
     elif record._type == "MX":
         rrset_records = list(
             map(
                 lambda value: {
                     'content': content_mx_tmpl.substitute(
                         preference=value.preference, exchange=value.exchange
                     )
@@ -74,22 +84,28 @@
 def to_octodns_record_data(rrset):
     rrset_type = rrset["type"]
     octodns_record = dict(type=rrset_type, ttl=rrset["ttl"])
     record_values = []
     key_for_record_values = "values"
     if rrset_type in {"A", "AAAA", "NS"}:
         record_values = [r['content'] for r in rrset["records"]]
-    elif rrset_type in {"CNAME", "ALIAS"}:
+    elif rrset_type in {"CNAME", "ALIAS", "DNAME"}:
         key_for_record_values = "value"
         record_values = rrset["records"][0]["content"]
     elif rrset_type == "TXT":
         record_values = [
             escape_semicolon(r['content']).strip('"\'')
             for r in rrset["records"]
         ]
+    elif rrset_type == "CAA":
+        for record in rrset["records"]:
+            flag, tag, value = record["content"].split(" ")
+            record_values.append(
+                {'flags': flag, 'tag': tag, 'value': value.strip("\"")}
+            )
     elif rrset_type == "MX":
         for record in rrset["records"]:
             preference, exchange = record["content"].split(" ")
             record_values.append(
                 {'preference': preference, 'exchange': exchange}
             )
     elif rrset_type == "SRV":
```

### Comparing `octodns-selectel-0.99.2/octodns_selectel/v2/provider.py` & `octodns_selectel-0.99.3/octodns_selectel/v2/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,27 @@
 from .exceptions import ApiException
 from .mappings import to_octodns_record_data, to_selectel_rrset
 
 
 class SelectelProvider(BaseProvider):
     SUPPORTS_GEO = False
     SUPPORTS = set(
-        ('A', 'AAAA', 'ALIAS', 'CNAME', 'MX', 'NS', 'TXT', 'SRV', 'SSHFP')
+        (
+            'A',
+            'AAAA',
+            'ALIAS',
+            'CAA',
+            'CNAME',
+            'DNAME',
+            'MX',
+            'NS',
+            'TXT',
+            'SRV',
+            'SSHFP',
+        )
     )
     MIN_TTL = 60
 
     def __init__(self, id, token, *args, **kwargs):
         self.log = getLogger(f'SelectelProvider[{id}]')
         self.log.debug('__init__: id=%s', id)
         super().__init__(id, *args, **kwargs)
```

### Comparing `octodns-selectel-0.99.2/octodns_selectel.egg-info/PKG-INFO` & `octodns_selectel-0.99.3/octodns_selectel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-selectel
-Version: 0.99.2
+Version: 0.99.3
 Summary:  Selectel DNS provider for octoDNS
 Home-page: https://github.com/octodns/octodns-selectel
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -12,16 +12,17 @@
 Requires-Dist: octodns>=0.9.14
 Requires-Dist: requests>=2.27.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-network; extra == "dev"
 Requires-Dist: requests_mock; extra == "dev"
-Requires-Dist: black<24.0.0,>=23.1.0; extra == "dev"
+Requires-Dist: black<25.0.0,>=24.3.0; extra == "dev"
 Requires-Dist: build>=0.7.0; extra == "dev"
+Requires-Dist: docutils<=0.20.1; extra == "dev"
 Requires-Dist: isort>=5.11.5; extra == "dev"
 Requires-Dist: pyflakes>=2.2.0; extra == "dev"
 Requires-Dist: readme_renderer[md]>=26.0; extra == "dev"
 Requires-Dist: twine>=3.4.2; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -49,15 +50,15 @@
 pip install octodns octodns-selectel
 ```
 
 ## Capabilities
 
 | What              | Value                                             |
 |-------------------|---------------------------------------------------|
-| Supported records | A, AAAA, ALIAS, CNAME, MX, NS, SRV, SSHFP, TXT    |
+| Supported records | A, AAAA, ALIAS, CAA, CNAME, DNAME, MX, NS, SRV, SSHFP, TXT    |
 | Dynamic records   | ❌ |
 
 ## Configuration
 Add selectel provider to `config.yaml`.
 ```yaml
 providers:
   selectel:
@@ -137,14 +138,27 @@
       target: phone1.example.com.
       weight: 60
     - port: 5030
       priority: 20
       target: phone2.example.com.
       weight: 0     
 
+caa:
+  - ttl: 3600
+    type: CAA
+    values:
+    - flags: 0
+      tag: issue
+      value: octodns-test.com.
+
+dname:
+  - ttl: 3600
+    type: DNAME
+    value: octodns-test.com.
+
 foo:
   - ttl: 3600
     type: CNAME
     value: bar.octodns-test.com.
 
 sshfp:
   - ttl: 3600
```

### Comparing `octodns-selectel-0.99.2/octodns_selectel.egg-info/SOURCES.txt` & `octodns_selectel-0.99.3/octodns_selectel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octodns-selectel-0.99.2/setup.py` & `octodns_selectel-0.99.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,16 +29,19 @@
     extras_require={
         'dev': tests_require
         + (
             # we need to manually/explicitely bump major versions as they're
             # likely to result in formatting changes that should happen in their
             # own PR. This will basically happen yearly
             # https://black.readthedocs.io/en/stable/the_black_code_style/index.html#stability-policy
-            'black>=23.1.0,<24.0.0',
+            'black>=24.3.0,<25.0.0',
             'build>=0.7.0',
+            # docutils 0.21.x bumped to >=3.9 and 3.8 is still active. we'll
+            # have to clamp it down until we remove 3.8
+            'docutils<=0.20.1',
             'isort>=5.11.5',
             'pyflakes>=2.2.0',
             'readme_renderer[md]>=26.0',
             'twine>=3.4.2',
         ),
         'test': tests_require,
     },
```

