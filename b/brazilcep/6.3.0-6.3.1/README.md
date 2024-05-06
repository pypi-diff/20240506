# Comparing `tmp/brazilcep-6.3.0.tar.gz` & `tmp/brazilcep-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brazilcep-6.3.0.tar", last modified: Mon May  6 01:07:56 2024, max compression
+gzip compressed data, was "brazilcep-6.3.1.tar", last modified: Mon May  6 01:17:56 2024, max compression
```

## Comparing `brazilcep-6.3.0.tar` & `brazilcep-6.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:07:56.648016 brazilcep-6.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-06 01:07:49.000000 brazilcep-6.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-05-06 01:07:56.648016 brazilcep-6.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-06 01:07:49.000000 brazilcep-6.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:07:56.644016 brazilcep-6.3.0/brazilcep/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-06 01:07:49.000000 brazilcep-6.3.0/brazilcep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-06 01:07:49.000000 brazilcep-6.3.0/brazilcep/apicep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-06 01:07:49.000000 brazilcep-6.3.0/brazilcep/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 01:07:49.000000 brazilcep-6.3.0/brazilcep/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-06 01:07:49.000000 brazilcep-6.3.0/brazilcep/viacep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:07:56.644016 brazilcep-6.3.0/brazilcep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-05-06 01:07:56.000000 brazilcep-6.3.0/brazilcep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-06 01:07:56.000000 brazilcep-6.3.0/brazilcep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 01:07:56.000000 brazilcep-6.3.0/brazilcep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 01:07:56.000000 brazilcep-6.3.0/brazilcep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 01:07:56.000000 brazilcep-6.3.0/brazilcep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-06 01:07:49.000000 brazilcep-6.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 01:07:56.648016 brazilcep-6.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:07:56.644016 brazilcep-6.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-06 01:07:49.000000 brazilcep-6.3.0/tests/test_apicep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-06 01:07:49.000000 brazilcep-6.3.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-06 01:07:49.000000 brazilcep-6.3.0/tests/test_viacep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:17:56.033950 brazilcep-6.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-06 01:17:50.000000 brazilcep-6.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-06 01:17:56.033950 brazilcep-6.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-06 01:17:50.000000 brazilcep-6.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:17:56.029950 brazilcep-6.3.1/brazilcep/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-06 01:17:50.000000 brazilcep-6.3.1/brazilcep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-06 01:17:50.000000 brazilcep-6.3.1/brazilcep/apicep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-06 01:17:50.000000 brazilcep-6.3.1/brazilcep/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 01:17:50.000000 brazilcep-6.3.1/brazilcep/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-06 01:17:50.000000 brazilcep-6.3.1/brazilcep/viacep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:17:56.033950 brazilcep-6.3.1/brazilcep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-06 01:17:56.000000 brazilcep-6.3.1/brazilcep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-06 01:17:56.000000 brazilcep-6.3.1/brazilcep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 01:17:56.000000 brazilcep-6.3.1/brazilcep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 01:17:56.000000 brazilcep-6.3.1/brazilcep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 01:17:56.000000 brazilcep-6.3.1/brazilcep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-06 01:17:50.000000 brazilcep-6.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 01:17:56.033950 brazilcep-6.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:17:56.029950 brazilcep-6.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-06 01:17:50.000000 brazilcep-6.3.1/tests/test_apicep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-06 01:17:50.000000 brazilcep-6.3.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-06 01:17:50.000000 brazilcep-6.3.1/tests/test_viacep.py
```

### Comparing `brazilcep-6.3.0/LICENSE` & `brazilcep-6.3.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 MIT License
 
-Copyright (c) 2016-2020, Michell Stuttgart
+Copyright (c) 2016-2024, Michell Stuttgart
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `brazilcep-6.3.0/PKG-INFO` & `brazilcep-6.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: brazilcep
-Version: 6.3.0
+Version: 6.3.1
 Summary: Minimalist and easy-to-use python library designed to query CEP (brazilian zip codes) data
 Author-email: Michell Stuttgart <michellstut@gmail.com>
 License: 
         MIT License
         
-        Copyright (c) 2016-2020, Michell Stuttgart
+        Copyright (c) 2016-2024, Michell Stuttgart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
@@ -27,14 +27,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Portuguese (Brazilian)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: zeep>=4.2.1
@@ -165,8 +166,8 @@
 
 ## Contribute
 
 See this *guideline* [here](https://github.com/mstuttgart/brazilcep/blob/develop/CONTRIBUTING.md).
 
 ## Credits
 
-Copyright (C) 2016-2023 by Michell Stuttgart
+Copyright (C) 2016-2024 by Michell Stuttgart
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: brazilcep Version: 6.3.0 Summary: Minimalist and
+Metadata-Version: 2.1 Name: brazilcep Version: 6.3.1 Summary: Minimalist and
 easy-to-use python library designed to query CEP (brazilian zip codes) data
 Author-email: Michell Stuttgart
-gmail.com> License: MIT License Copyright (c) 2016-2020, Michell Stuttgart
+gmail.com> License: MIT License Copyright (c) 2016-2024, Michell Stuttgart
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions: The above copyright notice and this
 permission notice shall be included in all copies or substantial portions of
@@ -23,26 +23,26 @@
 Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
 Independent Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries Classifier: Natural
-Language :: English Classifier: Natural Language :: Portuguese (Brazilian)
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: zeep>=4.2.1 Requires-Dist: requests>=2.28.2 Provides-
-Extra: dev Requires-Dist: nox>=2022.11.21; extra == "dev" Provides-Extra: test
-Requires-Dist: pytest>=7.3.1; extra == "test" Requires-Dist: requests-
-mock>=1.10.0; extra == "test" Provides-Extra: lint Requires-Dist: pylint; extra
-== "lint" Provides-Extra: coverage Requires-Dist: coveralls>=3.3.1; extra ==
-"coverage" Requires-Dist: pytest-cov>=4.0.0; extra == "coverage" Requires-Dist:
-requests-mock>=1.10.0; extra == "coverage" Provides-Extra: docs Requires-Dist:
-mkdocs-material>=9.1.6; extra == "docs" Requires-Dist: mkdocs>=1.4.2; extra ==
-"docs"
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
+Software Development :: Libraries Classifier: Natural Language :: English
+Classifier: Natural Language :: Portuguese (Brazilian) Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+zeep>=4.2.1 Requires-Dist: requests>=2.28.2 Provides-Extra: dev Requires-Dist:
+nox>=2022.11.21; extra == "dev" Provides-Extra: test Requires-Dist:
+pytest>=7.3.1; extra == "test" Requires-Dist: requests-mock>=1.10.0; extra ==
+"test" Provides-Extra: lint Requires-Dist: pylint; extra == "lint" Provides-
+Extra: coverage Requires-Dist: coveralls>=3.3.1; extra == "coverage" Requires-
+Dist: pytest-cov>=4.0.0; extra == "coverage" Requires-Dist: requests-
+mock>=1.10.0; extra == "coverage" Provides-Extra: docs Requires-Dist: mkdocs-
+material>=9.1.6; extra == "docs" Requires-Dist: mkdocs>=1.4.2; extra == "docs"
  ********** _[[_hh_tt_tt_pp_ss_::_//_//_gg_ii_tt_hh_uu_bb_.._cc_oo_mm_//_mm_ss_tt_uu_tt_tt_gg_aa_rr_tt_//_bb_rr_aa_zz_ii_ll_cc_ee_pp_//_aa_ss_ss_ee_tt_ss_//_88_11_77_44_77_44_00_//_ff_bb_77_cc_88_66_cc_88_--_66_22_66_11_--
                             _44_33_00_00_--_bb_22_ee_00_--_66_55_88_77_77_00_88_44_dd_88_66_55_]]
                                 BBrraazziillCCEEPP **********
     _[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_C_o_d_e_c_o_v_]_[_C_o_d_e_F_a_c_t_o_r_ _G_r_a_d_e_]_[_D_o_w_n_l_o_a_d_s_]_[_R_a_t_i_n_g_s_]
                                    _[_V_e_r_s_i_o_n_]
       _A_b_o_u_t | _I_n_s_t_a_l_l | _H_o_w_ _t_o_ _U_s_e | _D_o_c_u_m_e_n_t_a_t_i_o_n | _C_o_n_t_r_i_b_u_t_e | _C_r_e_d_i_t_s
 ## About **BrazilCEP** is a minimalist and easy-to-use python library designed
@@ -63,8 +63,8 @@
 *dict* object called ``address``. We can get all the address information we
 need from this object: ```python >>> address { 'district': 'rua abc', 'cep':
 '37503130', 'city': 'city ABC', 'street': 'str', 'uf': 'str', 'complement':
 'str', } ``` The CEP always must be a string. ## Documentation Documentation
 for the current version of BrazilCEP is available from the official docs [here]
 (https://brazilcep.readthedocs.io/en/stable). ## Contribute See this
 *guideline* [here](https://github.com/mstuttgart/brazilcep/blob/develop/
-CONTRIBUTING.md). ## Credits Copyright (C) 2016-2023 by Michell Stuttgart
+CONTRIBUTING.md). ## Credits Copyright (C) 2016-2024 by Michell Stuttgart
```

### Comparing `brazilcep-6.3.0/README.md` & `brazilcep-6.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -109,8 +109,8 @@
 
 ## Contribute
 
 See this *guideline* [here](https://github.com/mstuttgart/brazilcep/blob/develop/CONTRIBUTING.md).
 
 ## Credits
 
-Copyright (C) 2016-2023 by Michell Stuttgart
+Copyright (C) 2016-2024 by Michell Stuttgart
```

#### html2text {}

```diff
@@ -22,8 +22,8 @@
 *dict* object called ``address``. We can get all the address information we
 need from this object: ```python >>> address { 'district': 'rua abc', 'cep':
 '37503130', 'city': 'city ABC', 'street': 'str', 'uf': 'str', 'complement':
 'str', } ``` The CEP always must be a string. ## Documentation Documentation
 for the current version of BrazilCEP is available from the official docs [here]
 (https://brazilcep.readthedocs.io/en/stable). ## Contribute See this
 *guideline* [here](https://github.com/mstuttgart/brazilcep/blob/develop/
-CONTRIBUTING.md). ## Credits Copyright (C) 2016-2023 by Michell Stuttgart
+CONTRIBUTING.md). ## Credits Copyright (C) 2016-2024 by Michell Stuttgart
```

### Comparing `brazilcep-6.3.0/brazilcep/apicep.py` & `brazilcep-6.3.1/brazilcep/apicep.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.3.0/brazilcep/client.py` & `brazilcep-6.3.1/brazilcep/client.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.3.0/brazilcep/exceptions.py` & `brazilcep-6.3.1/brazilcep/exceptions.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.3.0/brazilcep/viacep.py` & `brazilcep-6.3.1/brazilcep/viacep.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.3.0/brazilcep.egg-info/PKG-INFO` & `brazilcep-6.3.1/brazilcep.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: brazilcep
-Version: 6.3.0
+Version: 6.3.1
 Summary: Minimalist and easy-to-use python library designed to query CEP (brazilian zip codes) data
 Author-email: Michell Stuttgart <michellstut@gmail.com>
 License: 
         MIT License
         
-        Copyright (c) 2016-2020, Michell Stuttgart
+        Copyright (c) 2016-2024, Michell Stuttgart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
@@ -27,14 +27,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Portuguese (Brazilian)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: zeep>=4.2.1
@@ -165,8 +166,8 @@
 
 ## Contribute
 
 See this *guideline* [here](https://github.com/mstuttgart/brazilcep/blob/develop/CONTRIBUTING.md).
 
 ## Credits
 
-Copyright (C) 2016-2023 by Michell Stuttgart
+Copyright (C) 2016-2024 by Michell Stuttgart
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: brazilcep Version: 6.3.0 Summary: Minimalist and
+Metadata-Version: 2.1 Name: brazilcep Version: 6.3.1 Summary: Minimalist and
 easy-to-use python library designed to query CEP (brazilian zip codes) data
 Author-email: Michell Stuttgart
-gmail.com> License: MIT License Copyright (c) 2016-2020, Michell Stuttgart
+gmail.com> License: MIT License Copyright (c) 2016-2024, Michell Stuttgart
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions: The above copyright notice and this
 permission notice shall be included in all copies or substantial portions of
@@ -23,26 +23,26 @@
 Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
 Independent Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries Classifier: Natural
-Language :: English Classifier: Natural Language :: Portuguese (Brazilian)
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: zeep>=4.2.1 Requires-Dist: requests>=2.28.2 Provides-
-Extra: dev Requires-Dist: nox>=2022.11.21; extra == "dev" Provides-Extra: test
-Requires-Dist: pytest>=7.3.1; extra == "test" Requires-Dist: requests-
-mock>=1.10.0; extra == "test" Provides-Extra: lint Requires-Dist: pylint; extra
-== "lint" Provides-Extra: coverage Requires-Dist: coveralls>=3.3.1; extra ==
-"coverage" Requires-Dist: pytest-cov>=4.0.0; extra == "coverage" Requires-Dist:
-requests-mock>=1.10.0; extra == "coverage" Provides-Extra: docs Requires-Dist:
-mkdocs-material>=9.1.6; extra == "docs" Requires-Dist: mkdocs>=1.4.2; extra ==
-"docs"
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
+Software Development :: Libraries Classifier: Natural Language :: English
+Classifier: Natural Language :: Portuguese (Brazilian) Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+zeep>=4.2.1 Requires-Dist: requests>=2.28.2 Provides-Extra: dev Requires-Dist:
+nox>=2022.11.21; extra == "dev" Provides-Extra: test Requires-Dist:
+pytest>=7.3.1; extra == "test" Requires-Dist: requests-mock>=1.10.0; extra ==
+"test" Provides-Extra: lint Requires-Dist: pylint; extra == "lint" Provides-
+Extra: coverage Requires-Dist: coveralls>=3.3.1; extra == "coverage" Requires-
+Dist: pytest-cov>=4.0.0; extra == "coverage" Requires-Dist: requests-
+mock>=1.10.0; extra == "coverage" Provides-Extra: docs Requires-Dist: mkdocs-
+material>=9.1.6; extra == "docs" Requires-Dist: mkdocs>=1.4.2; extra == "docs"
  ********** _[[_hh_tt_tt_pp_ss_::_//_//_gg_ii_tt_hh_uu_bb_.._cc_oo_mm_//_mm_ss_tt_uu_tt_tt_gg_aa_rr_tt_//_bb_rr_aa_zz_ii_ll_cc_ee_pp_//_aa_ss_ss_ee_tt_ss_//_88_11_77_44_77_44_00_//_ff_bb_77_cc_88_66_cc_88_--_66_22_66_11_--
                             _44_33_00_00_--_bb_22_ee_00_--_66_55_88_77_77_00_88_44_dd_88_66_55_]]
                                 BBrraazziillCCEEPP **********
     _[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_C_o_d_e_c_o_v_]_[_C_o_d_e_F_a_c_t_o_r_ _G_r_a_d_e_]_[_D_o_w_n_l_o_a_d_s_]_[_R_a_t_i_n_g_s_]
                                    _[_V_e_r_s_i_o_n_]
       _A_b_o_u_t | _I_n_s_t_a_l_l | _H_o_w_ _t_o_ _U_s_e | _D_o_c_u_m_e_n_t_a_t_i_o_n | _C_o_n_t_r_i_b_u_t_e | _C_r_e_d_i_t_s
 ## About **BrazilCEP** is a minimalist and easy-to-use python library designed
@@ -63,8 +63,8 @@
 *dict* object called ``address``. We can get all the address information we
 need from this object: ```python >>> address { 'district': 'rua abc', 'cep':
 '37503130', 'city': 'city ABC', 'street': 'str', 'uf': 'str', 'complement':
 'str', } ``` The CEP always must be a string. ## Documentation Documentation
 for the current version of BrazilCEP is available from the official docs [here]
 (https://brazilcep.readthedocs.io/en/stable). ## Contribute See this
 *guideline* [here](https://github.com/mstuttgart/brazilcep/blob/develop/
-CONTRIBUTING.md). ## Credits Copyright (C) 2016-2023 by Michell Stuttgart
+CONTRIBUTING.md). ## Credits Copyright (C) 2016-2024 by Michell Stuttgart
```

### Comparing `brazilcep-6.3.0/pyproject.toml` & `brazilcep-6.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brazilcep"
-version = "6.3.0"
+version = "6.3.1"
 description = "Minimalist and easy-to-use python library designed to query CEP (brazilian zip codes) data"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Michell Stuttgart", email = "michellstut@gmail.com" }]
 requires-python = ">=3.8"
 classifiers = [
   "Topic :: Software Development :: Build Tools",
@@ -20,14 +20,15 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
   "Natural Language :: English",
   "Natural Language :: Portuguese (Brazilian)",
 ]
 
 dependencies = ["zeep>=4.2.1", "requests>=2.28.2"]
```

### Comparing `brazilcep-6.3.0/tests/test_apicep.py` & `brazilcep-6.3.1/tests/test_apicep.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.3.0/tests/test_client.py` & `brazilcep-6.3.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.3.0/tests/test_viacep.py` & `brazilcep-6.3.1/tests/test_viacep.py`

 * *Files identical despite different names*

