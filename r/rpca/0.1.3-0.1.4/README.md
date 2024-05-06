# Comparing `tmp/rpca-0.1.3.tar.gz` & `tmp/rpca-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpca-0.1.3.tar", max compression
+gzip compressed data, was "rpca-0.1.4.tar", max compression
```

## Comparing `rpca-0.1.3.tar` & `rpca-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-10-01 17:54:07.546751 rpca-0.1.3/LICENSE
--rw-r--r--   0        0        0     1138 2023-10-01 18:07:33.293422 rpca-0.1.3/README.md
--rw-r--r--   0        0        0      798 2023-10-03 17:54:16.916211 rpca-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       75 2023-10-03 17:54:21.792878 rpca-0.1.3/rpca/__init__.py
--rw-r--r--   0        0        0    11688 2023-10-01 17:54:07.553418 rpca-0.1.3/rpca/rpca.py
--rw-r--r--   0        0        0      433 2023-10-01 17:54:07.553418 rpca-0.1.3/rpca/util.py
--rw-r--r--   0        0        0     2086 1970-01-01 00:00:00.000000 rpca-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-10-01 17:54:07.546751 rpca-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1138 2023-10-01 18:07:33.293422 rpca-0.1.4/README.md
+-rw-r--r--   0        0        0      798 2024-05-06 21:01:10.100419 rpca-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       75 2024-05-06 21:01:04.910419 rpca-0.1.4/rpca/__init__.py
+-rw-r--r--   0        0        0    11688 2023-10-01 17:54:07.553418 rpca-0.1.4/rpca/rpca.py
+-rw-r--r--   0        0        0      433 2023-10-01 17:54:07.553418 rpca-0.1.4/rpca/util.py
+-rw-r--r--   0        0        0     2137 1970-01-01 00:00:00.000000 rpca-0.1.4/PKG-INFO
```

### Comparing `rpca-0.1.3/LICENSE` & `rpca-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rpca-0.1.3/README.md` & `rpca-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rpca-0.1.3/pyproject.toml` & `rpca-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpca"
-version = "0.1.3"
+version = "0.1.4"
 description = "Robust PCA using Accelerated Alternating Projection"
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/loiccoyle/RPCA"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `rpca-0.1.3/rpca/rpca.py` & `rpca-0.1.4/rpca/rpca.py`

 * *Files identical despite different names*

### Comparing `rpca-0.1.3/PKG-INFO` & `rpca-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: rpca
-Version: 0.1.3
+Version: 0.1.4
 Summary: Robust PCA using Accelerated Alternating Projection
 Home-page: https://github.com/loiccoyle/RPCA
 License: MIT
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: numpy (>=1.26.0,<2.0.0)
 Requires-Dist: scipy (>=1.11.3,<2.0.0)
 Project-URL: Repository, https://github.com/loiccoyle/RPCA
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: rpca Version: 0.1.3 Summary: Robust PCA using
+Metadata-Version: 2.1 Name: rpca Version: 0.1.4 Summary: Robust PCA using
 Accelerated Alternating Projection Home-page: https://github.com/loiccoyle/RPCA
 License: MIT Author: Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-
 Python: >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: Topic :: Software Development :: Libraries ::
-Python Modules Requires-Dist: numpy (>=1.26.0,<2.0.0) Requires-Dist: scipy
-(>=1.11.3,<2.0.0) Project-URL: Repository, https://github.com/loiccoyle/RPCA
-Description-Content-Type: text/markdown # AccAltProj for robust PCA
+Python :: 3.12 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: numpy (>=1.26.0,<2.0.0) Requires-Dist: scipy (>=1.11.3,<2.0.0)
+Project-URL: Repository, https://github.com/loiccoyle/RPCA Description-Content-
+Type: text/markdown # AccAltProj for robust PCA
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_o_i_c_c_o_y_l_e_/_R_P_C_A_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_r_p_c_a_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
   [https://img.shields.io/badge/platform-linux%20%7C%20macOS%20%7C%20windows-
                                 informational]
 > Port of the AccAltProj algorithm for robust PCA to python.
 This is a python port of the [AccAltProj algorithm for robust PCA](https://
 github.com/caesarcai/AccAltProj_for_RPCA), described in this [paper](https://
```

