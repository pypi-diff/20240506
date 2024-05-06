# Comparing `tmp/brazilcep-6.2.0.tar.gz` & `tmp/brazilcep-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brazilcep-6.2.0.tar", max compression
+gzip compressed data, was "brazilcep-6.3.0.tar", last modified: Mon May  6 01:07:56 2024, max compression
```

## Comparing `brazilcep-6.2.0.tar` & `brazilcep-6.3.0.tar`

### file list

```diff
@@ -1,10 +1,22 @@
--rw-r--r--   0        0        0     6026 2023-10-01 20:45:00.087435 brazilcep-6.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-10-01 09:35:43.911475 brazilcep-6.2.0/LICENSE
--rw-r--r--   0        0        0     3446 2023-10-01 20:45:00.087435 brazilcep-6.2.0/README.md
--rw-r--r--   0        0        0      497 2023-10-01 09:35:43.911475 brazilcep-6.2.0/brazilcep/__init__.py
--rw-r--r--   0        0        0     1754 2023-10-01 20:45:00.087435 brazilcep-6.2.0/brazilcep/apicep.py
--rw-r--r--   0        0        0     2808 2023-10-01 20:45:00.087435 brazilcep-6.2.0/brazilcep/client.py
--rw-r--r--   0        0        0      543 2023-10-01 09:35:43.911475 brazilcep-6.2.0/brazilcep/exceptions.py
--rw-r--r--   0        0        0     1538 2023-10-01 20:45:00.087435 brazilcep-6.2.0/brazilcep/viacep.py
--rw-r--r--   0        0        0     2179 2023-10-01 20:45:46.242177 brazilcep-6.2.0/pyproject.toml
--rw-r--r--   0        0        0     4947 1970-01-01 00:00:00.000000 brazilcep-6.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:07:56.648016 brazilcep-6.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-06 01:07:49.000000 brazilcep-6.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-05-06 01:07:56.648016 brazilcep-6.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-06 01:07:49.000000 brazilcep-6.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:07:56.644016 brazilcep-6.3.0/brazilcep/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-06 01:07:49.000000 brazilcep-6.3.0/brazilcep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-06 01:07:49.000000 brazilcep-6.3.0/brazilcep/apicep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-06 01:07:49.000000 brazilcep-6.3.0/brazilcep/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 01:07:49.000000 brazilcep-6.3.0/brazilcep/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-06 01:07:49.000000 brazilcep-6.3.0/brazilcep/viacep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:07:56.644016 brazilcep-6.3.0/brazilcep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-05-06 01:07:56.000000 brazilcep-6.3.0/brazilcep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-06 01:07:56.000000 brazilcep-6.3.0/brazilcep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 01:07:56.000000 brazilcep-6.3.0/brazilcep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 01:07:56.000000 brazilcep-6.3.0/brazilcep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 01:07:56.000000 brazilcep-6.3.0/brazilcep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-06 01:07:49.000000 brazilcep-6.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 01:07:56.648016 brazilcep-6.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:07:56.644016 brazilcep-6.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-06 01:07:49.000000 brazilcep-6.3.0/tests/test_apicep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-06 01:07:49.000000 brazilcep-6.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-06 01:07:49.000000 brazilcep-6.3.0/tests/test_viacep.py
```

### Comparing `brazilcep-6.2.0/LICENSE` & `brazilcep-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brazilcep-6.2.0/README.md` & `brazilcep-6.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 
-<p align="center">
+<h2 align="center">
   <a href="https://pypi.org/project/brazilcep/">
-    <img src="https://raw.githubusercontent.com/mstuttgart/brazilcep/develop/docs/static/logo.png" width="80%">
+    <img src="https://github.com/mstuttgart/brazilcep/assets/8174740/fb7c86c8-6261-4300-b2e0-65877084d865" width="15%">
   </a>
-</p>
+  <br>
+      BrazilCEP
+</h2>
 
 <p align="center">
 
   <a href="https://github.com/mstuttgart/brazilcep/actions?query=workflow%3A%22Github+CI%22">
-    <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/mstuttgart/brazilcep/test-package.yml?color=3771a1&branch=develop&style=flat-square">
+    <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/mstuttgart/brazilcep/test.yml?color=fcd800&branch=main">
   </a>
 
-  <a href="https://coveralls.io/github/mstuttgart/brazilcep">
-    <img alt="Coveralls github" src="https://img.shields.io/coveralls/github/mstuttgart/brazilcep?color=fcd800&style=flat-square">
-  </a>
+ <a href="https://codecov.io/gh/mstuttgart/brazilcep" > 
+ <img alt="Codecov" src="https://img.shields.io/codecov/c/github/mstuttgart/brazilcep?color=fcd800">
+ </a>
 
   <a href="https://www.codefactor.io/repository/github/mstuttgart/brazilcep">
-    <img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/mstuttgart/brazilcep/develop?color=fcd800&style=flat-square">
+    <img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/mstuttgart/brazilcep/main?color=fcd800">
   </a>
 
   <a href="https://pypi.org/project/brazilcep">
-    <img src="https://img.shields.io/pypi/dm/brazilcep?color=fcd800&style=flat-square" alt="Downloads">
+    <img src="https://img.shields.io/pypi/dm/brazilcep?color=fcd800" alt="Downloads">
   </a>
 
   <a href="https://pypi.org/project/brazilcep">
-    <img src="https://img.shields.io/pypi/v/brazilcep.svg?style=flat-square" alt="Ratings">
+    <img src="https://img.shields.io/pypi/v/brazilcep.svg?" alt="Ratings">
   </a>
 
   <a href="https://pypi.org/project/brazilcep/">
-    <img src="https://img.shields.io/pypi/pyversions/brazilcep.svg?style=flat-square" alt="Version">
+    <img src="https://img.shields.io/pypi/pyversions/brazilcep.svg" alt="Version">
   </a>
 
 </p>
 
 <p align="center">
   <a href="#about">About</a> |
   <a href="#install">Install</a> |
   <a href="#how-to-use">How to Use</a> |
-  <a href="#documentation">Documentation</a>
-  <a href="#contribute">Contribute</a>
+  <a href="#documentation">Documentation</a> |
+  <a href="#contribute">Contribute</a> |
   <a href="#credits">Credits</a>
 </p>
 
 ## About
 
 **BrazilCEP** is a minimalist and easy-to-use python library designed to query CEP (brazilian zip codes) data.
 
@@ -50,28 +52,29 @@
 the integration of Python applications with these services.
 
 Currently supports several CEP API's:
 
 - [ViaCEP](https://viacep.com.br)
 - [ApiCEP (WideNet)](https://apicep.com)
 
+> [!NOTE]
 > **BrazilCEP** is the new name of former **PyCEPCorreio** python library.
   If you want to migrate the old code to the new version, please see the [migrate](https://brazilcep.readthedocs.io/en/latest/migrate/) section in docs.
 
 ## Install
 
 The recommended way to get BrazilCEP is to **install the latest stable release**
 via [pip](http://pip-installer.org>):
 
 ```sh
 pip install brazilcep
 ```
 
-We currently support **Python 3.8+ only**. Users on older interpreter versions
-are urged to upgrade.
+> [!NOTE]
+> We currently support **Python 3.8+ only**. Users on older interpreter versions are urged to upgrade.
 
 ## How to Use
 
 Making a request is very simple. Begin by importing the BrazilCEP module:
 
 ```python
 >>> import brazilcep
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
- _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_m_s_t_u_t_t_g_a_r_t_/_b_r_a_z_i_l_c_e_p_/_d_e_v_e_l_o_p_/_d_o_c_s_/_s_t_a_t_i_c_/
-                                   _l_o_g_o_._p_n_g_]
-    _[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_l_l_s_ _g_i_t_h_u_b_]_[_C_o_d_e_F_a_c_t_o_r_ _G_r_a_d_e_]_[_D_o_w_n_l_o_a_d_s_]
-                              _[_R_a_t_i_n_g_s_]_[_V_e_r_s_i_o_n_]
-        _A_b_o_u_t | _I_n_s_t_a_l_l | _H_o_w_ _t_o_ _U_s_e | _D_o_c_u_m_e_n_t_a_t_i_o_n _C_o_n_t_r_i_b_u_t_e _C_r_e_d_i_t_s
+ ********** _[[_hh_tt_tt_pp_ss_::_//_//_gg_ii_tt_hh_uu_bb_.._cc_oo_mm_//_mm_ss_tt_uu_tt_tt_gg_aa_rr_tt_//_bb_rr_aa_zz_ii_ll_cc_ee_pp_//_aa_ss_ss_ee_tt_ss_//_88_11_77_44_77_44_00_//_ff_bb_77_cc_88_66_cc_88_--_66_22_66_11_--
+                            _44_33_00_00_--_bb_22_ee_00_--_66_55_88_77_77_00_88_44_dd_88_66_55_]]
+                                BBrraazziillCCEEPP **********
+    _[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_C_o_d_e_c_o_v_]_[_C_o_d_e_F_a_c_t_o_r_ _G_r_a_d_e_]_[_D_o_w_n_l_o_a_d_s_]_[_R_a_t_i_n_g_s_]
+                                   _[_V_e_r_s_i_o_n_]
+      _A_b_o_u_t | _I_n_s_t_a_l_l | _H_o_w_ _t_o_ _U_s_e | _D_o_c_u_m_e_n_t_a_t_i_o_n | _C_o_n_t_r_i_b_u_t_e | _C_r_e_d_i_t_s
 ## About **BrazilCEP** is a minimalist and easy-to-use python library designed
 to query CEP (brazilian zip codes) data. Its objective is to provide a common
 query interface to all these search services, facilitating the integration of
 Python applications with these services. Currently supports several CEP API's:
 - [ViaCEP](https://viacep.com.br) - [ApiCEP (WideNet)](https://apicep.com) >
-**BrazilCEP** is the new name of former **PyCEPCorreio** python library. If you
-want to migrate the old code to the new version, please see the [migrate]
-(https://brazilcep.readthedocs.io/en/latest/migrate/) section in docs. ##
-Install The recommended way to get BrazilCEP is to **install the latest stable
-release** via [pip](http://pip-installer.org>): ```sh pip install brazilcep ```
-We currently support **Python 3.8+ only**. Users on older interpreter versions
-are urged to upgrade. ## How to Use Making a request is very simple. Begin by
-importing the BrazilCEP module: ```python >>> import brazilcep ``` Now, call
-the `get_address_from_cep` to query any CEP: ```python >>> address =
-brazilcep.get_address_from_cep('37503-130') ``` Now, we have a *dict* object
-called ``address``. We can get all the address information we need from this
-object: ```python >>> address { 'district': 'rua abc', 'cep': '37503130',
-'city': 'city ABC', 'street': 'str', 'uf': 'str', 'complement': 'str', } ```
-The CEP always must be a string. ## Documentation Documentation for the current
-version of BrazilCEP is available from the official docs [here](https://
-brazilcep.readthedocs.io/en/stable). ## Contribute See this *guideline* [here]
-(https://github.com/mstuttgart/brazilcep/blob/develop/CONTRIBUTING.md). ##
-Credits Copyright (C) 2016-2023 by Michell Stuttgart
+[!NOTE] > **BrazilCEP** is the new name of former **PyCEPCorreio** python
+library. If you want to migrate the old code to the new version, please see the
+[migrate](https://brazilcep.readthedocs.io/en/latest/migrate/) section in docs.
+## Install The recommended way to get BrazilCEP is to **install the latest
+stable release** via [pip](http://pip-installer.org>): ```sh pip install
+brazilcep ``` > [!NOTE] > We currently support **Python 3.8+ only**. Users on
+older interpreter versions are urged to upgrade. ## How to Use Making a request
+is very simple. Begin by importing the BrazilCEP module: ```python >>> import
+brazilcep ``` Now, call the `get_address_from_cep` to query any CEP: ```python
+>>> address = brazilcep.get_address_from_cep('37503-130') ``` Now, we have a
+*dict* object called ``address``. We can get all the address information we
+need from this object: ```python >>> address { 'district': 'rua abc', 'cep':
+'37503130', 'city': 'city ABC', 'street': 'str', 'uf': 'str', 'complement':
+'str', } ``` The CEP always must be a string. ## Documentation Documentation
+for the current version of BrazilCEP is available from the official docs [here]
+(https://brazilcep.readthedocs.io/en/stable). ## Contribute See this
+*guideline* [here](https://github.com/mstuttgart/brazilcep/blob/develop/
+CONTRIBUTING.md). ## Credits Copyright (C) 2016-2023 by Michell Stuttgart
```

### Comparing `brazilcep-6.2.0/brazilcep/apicep.py` & `brazilcep-6.3.0/brazilcep/apicep.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.2.0/brazilcep/client.py` & `brazilcep-6.3.0/brazilcep/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 This module implements the BrazilCEP client.
 This is the main module of BrazilCEP.
 
 :copyright: (c) 2023 by Michell Stuttgart.
 :license: MIT, see LICENSE for more details.
 """
-import warnings
+
 import enum
 import re
+import warnings
 
 from . import apicep, viacep
 
 NUMBERS = re.compile(r"[^0-9]")
 DEFAULT_TIMEOUT = 5  # in seconds
```

### Comparing `brazilcep-6.2.0/brazilcep/exceptions.py` & `brazilcep-6.3.0/brazilcep/exceptions.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.2.0/brazilcep/viacep.py` & `brazilcep-6.3.0/brazilcep/viacep.py`

 * *Files identical despite different names*

