# Comparing `tmp/datafog-3.0.0b5.tar.gz` & `tmp/datafog-3.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.0.0b5.tar", last modified: Tue Apr 23 05:10:49 2024, max compression
+gzip compressed data, was "datafog-3.0.0b6.tar", last modified: Mon Apr 29 19:02:13 2024, max compression
```

## Comparing `datafog-3.0.0b5.tar` & `datafog-3.0.0b6.tar`

### file list

```diff
@@ -1,12 +1,24 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-23 05:10:49.418112 datafog-3.0.0b5/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-04-23 03:14:56.000000 datafog-3.0.0b5/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     7574 2024-04-23 05:10:49.417946 datafog-3.0.0b5/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6353 2024-04-23 03:14:56.000000 datafog-3.0.0b5/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-23 05:10:49.417725 datafog-3.0.0b5/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     7574 2024-04-23 05:10:49.000000 datafog-3.0.0b5/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      180 2024-04-23 05:10:49.000000 datafog-3.0.0b5/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-23 05:10:49.000000 datafog-3.0.0b5/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      119 2024-04-23 05:10:49.000000 datafog-3.0.0b5/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-23 05:10:49.000000 datafog-3.0.0b5/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-04-23 05:10:49.418214 datafog-3.0.0b5/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1766 2024-04-23 05:10:46.000000 datafog-3.0.0b5/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-29 19:02:13.801563 datafog-3.0.0b6/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-04-29 13:31:05.000000 datafog-3.0.0b6/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7676 2024-04-29 19:02:13.801322 datafog-3.0.0b6/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6353 2024-04-29 13:31:05.000000 datafog-3.0.0b6/README.md
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-04-29 19:02:13.801614 datafog-3.0.0b6/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1654 2024-04-29 16:44:12.000000 datafog-3.0.0b6/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-29 19:02:13.797088 datafog-3.0.0b6/src/
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-29 19:02:13.799231 datafog-3.0.0b6/src/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       30 2024-04-29 17:21:07.000000 datafog-3.0.0b6/src/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      419 2024-04-29 17:24:00.000000 datafog-3.0.0b6/src/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1256 2024-04-29 15:53:12.000000 datafog-3.0.0b6/src/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     4229 2024-04-29 17:23:58.000000 datafog-3.0.0b6/src/datafog/donuttransformer.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2970 2024-04-29 17:51:56.000000 datafog-3.0.0b6/src/datafog/main.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1744 2024-04-29 18:50:16.000000 datafog-3.0.0b6/src/datafog/pii_annotation.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-29 19:02:13.801041 datafog-3.0.0b6/src/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7676 2024-04-29 19:02:13.000000 datafog-3.0.0b6/src/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      419 2024-04-29 19:02:13.000000 datafog-3.0.0b6/src/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-29 19:02:13.000000 datafog-3.0.0b6/src/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       62 2024-04-29 19:02:13.000000 datafog-3.0.0b6/src/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-04-29 19:02:13.000000 datafog-3.0.0b6/src/datafog.egg-info/top_level.txt
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-29 19:02:13.800671 datafog-3.0.0b6/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1857 2024-04-29 19:00:17.000000 datafog-3.0.0b6/tests/test_a.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2311 2024-04-29 17:36:32.000000 datafog-3.0.0b6/tests/test_donuttransformer.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1859 2024-04-29 18:46:28.000000 datafog-3.0.0b6/tests/test_main.py
```

### Comparing `datafog-3.0.0b5/LICENSE` & `datafog-3.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.0.0b5/PKG-INFO` & `datafog-3.0.0b6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.0.0b5
+Version: 3.0.0b6
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
 Project-URL: Homepage, https://datafog.ai
 Project-URL: Documentation, https://docs.datafog.ai
 Project-URL: Discord, https://discord.gg/bzDth394R4
 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python
 Keywords: pii,redaction,nlp,rag,retrieval augmented generation
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: tox
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas==2.2.2
+Requires-Dist: Requests==2.31.0
+Requires-Dist: spacy==3.4.4
+Requires-Dist: en_spacy_pii_fast
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
@@ -162,9 +165,7 @@
 
 ```
 
 ## License
 
 This software is published under the [MIT
 license](https://en.wikipedia.org/wiki/MIT_License).
-
-
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.0.0b5 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.0.0b6 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
-pii,redaction,nlp,rag,retrieval augmented generation Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Framework :: tox
-Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: Information Technology Classifier: Intended Audience :: System
-Administrators Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE
+pii,redaction,nlp,rag,retrieval augmented generation Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Framework :: tox Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Science/Research Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+pandas==2.2.2 Requires-Dist: Requests==2.31.0 Requires-Dist: spacy==3.4.4
+Requires-Dist: en_spacy_pii_fast
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
```

### Comparing `datafog-3.0.0b5/README.md` & `datafog-3.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.0.0b5/datafog.egg-info/PKG-INFO` & `datafog-3.0.0b6/src/datafog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.0.0b5
+Version: 3.0.0b6
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
 Project-URL: Homepage, https://datafog.ai
 Project-URL: Documentation, https://docs.datafog.ai
 Project-URL: Discord, https://discord.gg/bzDth394R4
 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python
 Keywords: pii,redaction,nlp,rag,retrieval augmented generation
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: tox
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas==2.2.2
+Requires-Dist: Requests==2.31.0
+Requires-Dist: spacy==3.4.4
+Requires-Dist: en_spacy_pii_fast
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
@@ -162,9 +165,7 @@
 
 ```
 
 ## License
 
 This software is published under the [MIT
 license](https://en.wikipedia.org/wiki/MIT_License).
-
-
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.0.0b5 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.0.0b6 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
-pii,redaction,nlp,rag,retrieval augmented generation Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Framework :: tox
-Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: Information Technology Classifier: Intended Audience :: System
-Administrators Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE
+pii,redaction,nlp,rag,retrieval augmented generation Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Framework :: tox Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Science/Research Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+pandas==2.2.2 Requires-Dist: Requests==2.31.0 Requires-Dist: spacy==3.4.4
+Requires-Dist: en_spacy_pii_fast
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
```

### Comparing `datafog-3.0.0b5/setup.py` & `datafog-3.0.0b6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.0.0-beta.5"
+    return "3.0.0-beta.6"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
@@ -23,23 +23,18 @@
     version=__version__(),
     author="DataFog",
     author_email="hi@datafog.ai",
     description="Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
-        "en_spacy_pii_fast==0.0.0",
         "pandas==2.2.2",
-        "Pillow==10.3.0",
-        "pydantic==1.10.8",
-        "Requests",
-        "setuptools",
-        "torch",
-        "transformers",
-        "protobuf",
+        "Requests==2.31.0",
+        "spacy==3.4.4",
+        "en_spacy_pii_fast",
     ],
     python_requires=">=3.10",
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

