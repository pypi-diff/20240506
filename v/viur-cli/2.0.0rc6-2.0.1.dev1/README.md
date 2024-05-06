# Comparing `tmp/viur_cli-2.0.0rc6.tar.gz` & `tmp/viur_cli-2.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur_cli-2.0.0rc6.tar", last modified: Fri Mar 22 14:06:43 2024, max compression
+gzip compressed data, was "viur_cli-2.0.1.dev1.tar", last modified: Mon May  6 14:30:10 2024, max compression
```

## Comparing `viur_cli-2.0.0rc6.tar` & `viur_cli-2.0.1.dev1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.633774 viur_cli-2.0.0rc6/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-03-22 14:06:43.633774 viur_cli-2.0.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-22 14:06:43.633774 viur_cli-2.0.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.621774 viur_cli-2.0.0rc6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.625774 viur_cli-2.0.0rc6/src/viur_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    26913 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.629774 viur_cli-2.0.0rc6/src/viur_cli/scriptor/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.629774 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/csvwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/viur.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.629774 viur_cli-2.0.0rc6/src/viur_cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scripts/get_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/scripts/viur_2to3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-22 14:06:31.000000 viur_cli-2.0.0rc6/src/viur_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:06:43.629774 viur_cli-2.0.0rc6/src/viur_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-03-22 14:06:43.000000 viur_cli-2.0.0rc6/src/viur_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-22 14:06:43.000000 viur_cli-2.0.0rc6/src/viur_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:06:43.000000 viur_cli-2.0.0rc6/src/viur_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-22 14:06:43.000000 viur_cli-2.0.0rc6/src/viur_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-22 14:06:43.000000 viur_cli-2.0.0rc6/src/viur_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-22 14:06:43.000000 viur_cli-2.0.0rc6/src/viur_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:30:10.565757 viur_cli-2.0.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-05-06 14:30:10.565757 viur_cli-2.0.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-06 14:30:10.565757 viur_cli-2.0.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:30:10.557757 viur_cli-2.0.1.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:30:10.561757 viur_cli-2.0.1.dev1/src/viur_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27487 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:30:10.561757 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:30:10.561757 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/csvwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/viur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:30:10.561757 viur_cli-2.0.1.dev1/src/viur_cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scripts/get_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/scripts/viur_2to3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 14:30:06.000000 viur_cli-2.0.1.dev1/src/viur_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:30:10.565757 viur_cli-2.0.1.dev1/src/viur_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-05-06 14:30:10.000000 viur_cli-2.0.1.dev1/src/viur_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-06 14:30:10.000000 viur_cli-2.0.1.dev1/src/viur_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:30:10.000000 viur_cli-2.0.1.dev1/src/viur_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-06 14:30:10.000000 viur_cli-2.0.1.dev1/src/viur_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-06 14:30:10.000000 viur_cli-2.0.1.dev1/src/viur_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 14:30:10.000000 viur_cli-2.0.1.dev1/src/viur_cli.egg-info/top_level.txt
```

### Comparing `viur_cli-2.0.0rc6/LICENSE` & `viur_cli-2.0.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/PKG-INFO` & `viur_cli-2.0.1.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: viur_cli
-Version: 2.0.0rc6
+Version: 2.0.1.dev1
 Summary: Command-line interface for ViUR application maintenance.
 Home-page: https://github.com/viur-framework/viur-cli
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: app_server==0.9.9
-Requires-Dist: click==8.1.7
-Requires-Dist: pipfile-requirements==0.3.0
-Requires-Dist: requests==2.31.0
-Requires-Dist: semver==3.0.2
+Requires-Dist: app_server~=0.9
+Requires-Dist: click~=8.1.7
+Requires-Dist: pipfile-requirements~=0.3
+Requires-Dist: requests~=2.31
+Requires-Dist: semver~=3.0
 
 <div align="center">
     <img src="https://github.com/viur-framework/viur-artwork/raw/main/icons/icon-cli.svg" height="196" alt="A hexagonal logo of the viur-cli" title="viur-cli">
     <h1>viur-cli</h1>
     <a href="https://pypi.org/project/viur-cli/">
         <img alt="Badge showing current PyPI version" title="PyPI" src="https://img.shields.io/pypi/v/viur-cli">
     </a>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: viur_cli Version: 2.0.0rc6 Summary: Command-line
+Metadata-Version: 2.1 Name: viur_cli Version: 2.0.1.dev1 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.11 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: app_server==0.9.9 Requires-Dist: click==8.1.7 Requires-Dist:
-pipfile-requirements==0.3.0 Requires-Dist: requests==2.31.0 Requires-Dist:
-semver==3.0.2
+Requires-Dist: app_server~=0.9 Requires-Dist: click~=8.1.7 Requires-Dist:
+pipfile-requirements~=0.3 Requires-Dist: requests~=2.31 Requires-Dist:
+semver~=3.0
                       [A hexagonal logo of the viur-cli]
                             ************ vviiuurr--ccllii ************
       _[_B_a_d_g_e_ _s_h_o_w_i_n_g_ _c_u_r_r_e_n_t_ _P_y_P_I_ _v_e_r_s_i_o_n_]_[_B_a_d_g_e_ _d_i_s_p_l_a_y_i_n_g_ _t_h_e_ _l_i_c_e_n_s_e_]
         Command-line interface for _V_i_U_R_ _f_r_a_m_e_w_o_r_k project maintenance.
 ## What does it do? `viur-cli` allows to control, maintain, develop and deploy
 a ViUR project from one central location by using the `viur` command. ##
 Installation To use `viur-cli` in your ViUR projects, install the [PyPI package
```

### Comparing `viur_cli-2.0.0rc6/README.md` & `viur_cli-2.0.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/setup.cfg` & `viur_cli-2.0.1.dev1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.11
 install_requires = 
-	app_server==0.9.9
-	click==8.1.7
-	pipfile-requirements==0.3.0
-	requests==2.31.0
-	semver==3.0.2
+	app_server~=0.9
+	click~=8.1.7
+	pipfile-requirements~=0.3
+	requests~=2.31
+	semver~=3.0
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	viur = viur_cli:cli
```

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/build.py` & `viur_cli-2.0.1.dev1/src/viur_cli/build.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/cli.py` & `viur_cli-2.0.1.dev1/src/viur_cli/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/cloud.py` & `viur_cli-2.0.1.dev1/src/viur_cli/cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,24 +83,41 @@
 
     print('Success! It may take a while until you can use Gcloud Backups')
 
 @cloud.command(context_settings={"ignore_unknown_options": True})
 @click.argument("service", type=click.Choice(["gcloud"]), default="gcloud")
 @click.argument("profile", default="default")
 def init(service, profile):
+    """
+    Initializes the cloud service deployment.
+
+    Parameters:
+        - service (str): The cloud service to be initialized. Expected values are 'gcloud'.
+        - profile (str): The profile name to be used for initialization. Default value is 'default'.
+
+    """
     deployments = ["cron", "queue", "cron"]
     if service == "gcloud":
         for element in deployments:
             os.system(f"viur cloud deploy {element} {profile} -y")
 
 @cloud.command(context_settings={"ignore_unknown_options": True})
 @click.argument("service", type=click.Choice(["gcloud"]), default="gcloud")
 @click.argument("option", type=click.Choice(["datastore"]), default="datastore")
 @click.argument("profile", default="default")
 def cleanup(service, option, profile):
+    """
+    Cleans up the indexes in the specified service and option.
+
+    Parameters:
+    - service (str): The service to clean up the indexes for.
+    - option (str): The option to clean up the indexes for.
+    - profile (str): The profile to use for configuration.
+
+    """
     conf = config.get_profile(profile)
 
     if service == "gcloud" and option == "datastore":
         run_command(f"gcloud datastore indexes cleanup deploy/index.yaml --project={conf['application_name']}")
 
 
 @cloud.command(context_settings={"ignore_unknown_options": True})
@@ -568,15 +585,16 @@
                 echo_error(f"{yaml_file} not found")
                 return
             except ValueError:
                 echo_error(f"{yaml_file} is not a valid")
                 return
 
         os.system(
-            f'gcloud app deploy --project={conf["application_name"]} {" ".join(additional_args)} {yaml_file}')
+            f'gcloud app deploy --project={conf["application_name"]} {" ".join(additional_args)} {yaml_file} {"-q" if yes else ""}')
+
 
 
 def build_deploy_command(name, conf):
     """
 
     Builds a deployment command for a cloud function.
```

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/conf.py` & `viur_cli-2.0.1.dev1/src/viur_cli/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
+from pprint import pprint
+
 import click
 import requests
 import difflib
 from .utils import *
 from .version import __version__ as cli_version
 
+
 PROJECT_CONFIG_FILE = "project.json"
 PROJECT_CONFIG_VERSION = "2.0.0"
 LAST_VERSION = ""
 
 
 class ProjectConfig(dict):
 
@@ -82,15 +85,48 @@
         configname = click.prompt('name')
         try:
             del self[configname]
             self.save()
         except:
             raise click.ClickException(click.style(f"{configname} not found", fg="red"))
 
+    def find_key(self, dictionary, target_key, target, keep=False):
+        if target_key in dictionary:
+            if keep:
+                value = dictionary[target_key]
+            else:
+                value = dictionary.pop(target_key)
+            if not target:
+                self[target_key] = value
+            else:
+                self.setdefault(target, {})[target_key] = value
+        else:
+            for value in list(dictionary.values()):
+                if isinstance(value, dict):
+
+                    self.find_key(value, target_key, target, keep=keep)
+
+    def remove_key(self, dictionary, target_key):
+        if target_key in dictionary:
+            del dictionary[target_key]
+
+        for value in list(dictionary.values()):
+            if isinstance(value, dict):
+                self.remove_key(value, target_key)
+
     def migrate(self):
+
+        if "application_name" not in self["default"]:
+            self.find_key(self, target_key="application_name", target="default", keep=True)
+            if "application_name" in self:
+                del self["application_name"]
+
+        self.remove_key(self, target_key="core")
+
+
         if old_format := self["default"].get("format"):
             self["format"] = old_format
             del self["default"]["format"]
 
         assert self["format"] in ["1.0.0", "1.0.1", "1.1.0", "1.1.1", "1.2.0", PROJECT_CONFIG_VERSION], \
             "Invalid formatversion, you have to fix it manually"
 
@@ -114,25 +150,14 @@
             self["format"] = "1.1.1"
             builds = self["default"].get("builds", {}).copy()
             for k, v in builds.items():
                 if builds[k]["kind"] == "script":
                     builds[k]["kind"] = "exec"
             self["default"]["builds"] = builds
 
-        # Version 1.2.0
-        """
-            Convert versions in the configuration to builds.
-
-            This method iterates through the provided version list and updates the project configuration
-            by converting versions to builds.
-
-            :param version_list: list
-                List of versions to convert to builds.
-            :return: None
-        """
         # Check if Builds is in the project.json
         if "builds" not in self["default"].keys():
             self["default"]["builds"] = {}
 
         if self["format"] == "1.1.1":
             self["format"] = "2.0.0"
             format_version_updated = True
@@ -155,35 +180,20 @@
             response = click.prompt(
                 text="Do you want to enforce use of admin only? (yes/no/keep)",
                 type=click.Choice(["yes", "no", "keep"]),
                 default="yes"
             )
 
             if response == "yes":
-                del self["default"]["builds"]["vi"]
+                self["default"]["builds"].pop("vi", None)
+                echo_info("You are using the ViUR Admin")
             elif response == "no":
-                del self["default"]["builds"]["admin"]
-
-        """
-             Fetch the version of the 'viur-core' package.
-
-             This method is responsible for fetching the version of the 'viur-core' package using 'pip list' and updating
-             the project configuration accordingly.
-
-             :return: None
-        """
-        try:
-            result = os.popen('pip list --format=json').read()
-            core_version = [x for x in json.loads(result) if x["name"] == "viur-core"][0]["version"]
-            self["default"]["core"] = core_version
-
-        except:
-            self["default"]["core"] = "submodule"
+                self["default"]["builds"].pop("admin", None)
+                echo_info("You are using the Vi Administration")
 
-        # conf updates must increase format version
         self.save()
 
 
 def print_changelog_from_github(user, repo, last_version):
     version_url = f"https://raw.githubusercontent.com/{user}/{repo}/main/CHANGELOG.md"
     response = requests.get(version_url)
```

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/local.py` & `viur_cli-2.0.1.dev1/src/viur_cli/local.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import click
 import os
 import shutil
 import subprocess
 
 from viur_cli import echo_info, echo_warning
 from .conf import config
-from . import cli, echo_error, utils
+from . import cli, echo_error, utils, echo_fatal
 from requests import get
 from .package import vi as vi_install
 from types import SimpleNamespace
 
 
 def get_user_info():
     gcloud_auth_process = subprocess.run(['gcloud', 'auth', 'application-default', 'print-access-token'],
@@ -19,33 +19,40 @@
                                          text=True)
 
     auth_token = gcloud_auth_process.stdout.strip()  # Extract auth token
 
     curl_command = f'curl -X GET -H "Authorization: Bearer {auth_token}" "https://www.googleapis.com/oauth2/v1/userinfo?alt=json"'
 
     curl_process = subprocess.run(curl_command,
-                                  capture_output=True, shell = True,
+                                  capture_output=True, shell=True,
                                   text=True)
     user_info = json.loads(curl_process.stdout)
 
     return user_info
 
 
 @cli.command(context_settings={"ignore_unknown_options": True})
 @click.argument("profile", default='default')
 @click.argument("additional_args", nargs=-1)
 def run(profile, additional_args):
     """
         Start your application locally.
         The 'run' command launches your ViUR application locally specified configuration and optional arguments.
+        This Enforces the Usage of gcloud tool
     """
-    echo_warning(f"You are using the development Server with your default account: {get_user_info()['email']}")
+    try:
+        echo_warning(f"You are using the development Server with your default account: {get_user_info()['email']}")
+    except:
+        echo_fatal(f"It seems you are not Using an appropriate account. "
+                   f"Please install the 'gcloud' tool or Log in with an appropriate account.")
+
     conf = config.get_profile(profile)
+    utils.system(
+        f'app_server -A={conf["application_name"]} {conf["distribution_folder"]} {" ".join(additional_args)}')
 
-    utils.system(f'app_server -A={conf["application_name"]} {conf["distribution_folder"]} {" ".join(additional_args)}')
 
 @cli.command()
 @click.argument("profile", default="default")
 def env(profile):
     """
        Check the local environment for ViUR development.
 
@@ -145,18 +152,19 @@
                 line = " - " + line
             versionList.append(line)
         versionString = '\n'.join(versionList)
         click.echo(f"{valid_icon} {versionString}")
     else:
         click.echo(f"{failed_icon} gcloud")
 
-    click.echo(f"Your default gcloud user Info:")
-    for k,v in get_user_info().items():
+    click.echo(f"\nYour default gcloud user Info:\n--------------------------------")
+    for k, v in get_user_info().items():
         click.echo(f"{k}: {v}")
 
+
 @cli.command()
 @click.option('--dev', '-d', is_flag=True, default=False)
 def check(dev):
     """
     Perform security checks for vulnerabilities.
     The 'check' command helps you identify and address security vulnerabilities in your project's dependencies.
     """
```

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/package.py` & `viur_cli-2.0.1.dev1/src/viur_cli/package.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/scriptor/cli.py` & `viur_cli-2.0.1.dev1/src/viur_cli/scriptor/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/__init__.py` & `viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/csvwriter.py` & `viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/csvwriter.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/dialog.py` & `viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/dialog.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/logger.py` & `viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/logger.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/module.py` & `viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/module.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/network.py` & `viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/network.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/readers.py` & `viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/readers.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/viur.py` & `viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/viur.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/scriptor/scriptor/writer.py` & `viur_cli-2.0.1.dev1/src/viur_cli/scriptor/scriptor/writer.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/scripts/get_pyodide.py` & `viur_cli-2.0.1.dev1/src/viur_cli/scripts/get_pyodide.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/scripts/viur_2to3.py` & `viur_cli-2.0.1.dev1/src/viur_cli/scripts/viur_2to3.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     "getEmtpyValueFunc": "getEmptyValueFunc",
     "isLocalDevelopmentServer": "conf[\"viur.instance.is_dev_server\"]",
     "onItemAdded": "onAdded",
     "onItemDeleted": "onDeleted",
     "onItemEdited": "onEdited",
     "projectID": "conf[\"viur.instance.project_id\"]",
     "utils.currentLanguage": "current.language",
-    "utils.currentRequest": "current.request",
     "utils.currentRequestData": "current.request_data",
+    "utils.currentRequest": "current.request",
     "utils.currentSession": "current.session",
     "utils.getCurrentUser": "current.user.get",
     "utils.isLocalDevelopmentServer": "conf[\"viur.instance.is_dev_server\"]",
     "utils.projectID": "conf[\"viur.instance.project_id\"]",
     "clearUpdateTag=True": "update_relations=False",
     "seoLanguageMap": "seo_language_map",  # 800
     "forcePost": "force_post",  # 800
```

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/setup.py` & `viur_cli-2.0.1.dev1/src/viur_cli/setup.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/tool.py` & `viur_cli-2.0.1.dev1/src/viur_cli/tool.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/update.py` & `viur_cli-2.0.1.dev1/src/viur_cli/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 import os
 import sys
 import re
 from .conf import config
-from . import cli, echo_error, echo_positive, echo_info, utils
+from . import cli, echo_error, echo_info, utils
 
 
 @cli.command(context_settings={"ignore_unknown_options": True})
 @click.argument("action", type=click.Choice(["requirements"]))
 @click.argument("profile", default='default')
 @click.argument("additional_args", nargs=-1)
 def update(action, profile, additional_args):
@@ -16,28 +16,22 @@
 
     This command allows you to update project-specific files and dependencies for a specified project configuration.
     Currently, it supports the 'requirements' action, which is used to update the requirements.
     The `update` command performs the specified 'action' to update project-specific files or dependencies. It ensures
     that the specified project configuration exists.
 
     Note:
-
         - Ensure that the specified project configuration ('name') is valid and defined in your project's configuration.
-
         - Additional arguments can be used to customize the update process if supported by the action.
-
     """
-    conf = config.get_profile(profile)
 
     if action == "requirements":
         create_req(True, profile)
 
 
-
-
 def create_req(yes, profile, confirm_value=True):
     """
     Load project's pipenv and build a requirements.txt.
 
     This function generates a requirements.txt file based on the project's pipenv environment. It offers the option
     to confirm the regeneration of the requirements.txt file.
 
@@ -49,35 +43,36 @@
     - It prompts for confirmation to regenerate the requirements.txt file.
     - If errors are detected, it provides an option to continue or exit the script.
 
     :return: None
     """
     conf = config.get_profile(profile)
     dist_folder = conf["distribution_folder"]
-    if conf["core"] != "submodule":
-        if yes or click.confirm(
-                text=f"Do you want to regenerate the requirements.txt located in the {dist_folder}?",
-                default=confirm_value):
-            os.system(f"pipfile2req  --hashes > {dist_folder}/requirements.txt")
-            file_object = open(f"{dist_folder}/requirements.txt", 'r')
-            generated_requirements = file_object.read()
-            for line in generated_requirements.splitlines():
-                if "]==" in line:
-                    # we got a dependency with extras
-                    generated_requirements += re.sub(r"\[.*?\]", "", line) + "\n"
-            file_object.close()
-
-            file_obj = open(f"{dist_folder}/requirements.txt", 'w')
-            file_obj.write(generated_requirements)
-            file_obj.close()
-            echo_info("requirements.txt successfully generated")
-
-        if check_req(f"{dist_folder}/requirements.txt"):
-            if not click.confirm(f"There are some depencency errors, are you sure you want to continue?"):
-                sys.exit(0)
+
+    if yes or click.confirm( text=f"Do you want to regenerate the requirements.txt located in the {dist_folder}?",
+                             default=confirm_value):
+        os.system(f"pipfile2req  --hashes > {dist_folder}/requirements.txt")
+        file_object = open(f"{dist_folder}/requirements.txt", 'r')
+        generated_requirements = file_object.read()
+
+        for line in generated_requirements.splitlines():
+            if "]==" in line:
+                # we got a dependency with extras
+                generated_requirements += re.sub(r"\[.*?\]", "", line) + "\n"
+        file_object.close()
+
+
+        file_obj = open(f"{dist_folder}/requirements.txt", 'w')
+        file_obj.write(generated_requirements)
+        file_obj.close()
+        echo_info("requirements.txt successfully generated")
+
+    if check_req(f"{dist_folder}/requirements.txt"):
+        if not click.confirm(f"There are some depencency errors, are you sure you want to continue?"):
+            sys.exit(0)
 
 
 def check_req(projects_requirements_path):
     """
     Check project's requirements against core requirements.
 
     This function checks the project's requirements to validate package versions and hashes.
```

### Comparing `viur_cli-2.0.0rc6/src/viur_cli/utils.py` & `viur_cli-2.0.1.dev1/src/viur_cli/utils.py`

 * *Files identical despite different names*

### Comparing `viur_cli-2.0.0rc6/src/viur_cli.egg-info/PKG-INFO` & `viur_cli-2.0.1.dev1/src/viur_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: viur_cli
-Version: 2.0.0rc6
+Version: 2.0.1.dev1
 Summary: Command-line interface for ViUR application maintenance.
 Home-page: https://github.com/viur-framework/viur-cli
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: app_server==0.9.9
-Requires-Dist: click==8.1.7
-Requires-Dist: pipfile-requirements==0.3.0
-Requires-Dist: requests==2.31.0
-Requires-Dist: semver==3.0.2
+Requires-Dist: app_server~=0.9
+Requires-Dist: click~=8.1.7
+Requires-Dist: pipfile-requirements~=0.3
+Requires-Dist: requests~=2.31
+Requires-Dist: semver~=3.0
 
 <div align="center">
     <img src="https://github.com/viur-framework/viur-artwork/raw/main/icons/icon-cli.svg" height="196" alt="A hexagonal logo of the viur-cli" title="viur-cli">
     <h1>viur-cli</h1>
     <a href="https://pypi.org/project/viur-cli/">
         <img alt="Badge showing current PyPI version" title="PyPI" src="https://img.shields.io/pypi/v/viur-cli">
     </a>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: viur_cli Version: 2.0.0rc6 Summary: Command-line
+Metadata-Version: 2.1 Name: viur_cli Version: 2.0.1.dev1 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.11 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: app_server==0.9.9 Requires-Dist: click==8.1.7 Requires-Dist:
-pipfile-requirements==0.3.0 Requires-Dist: requests==2.31.0 Requires-Dist:
-semver==3.0.2
+Requires-Dist: app_server~=0.9 Requires-Dist: click~=8.1.7 Requires-Dist:
+pipfile-requirements~=0.3 Requires-Dist: requests~=2.31 Requires-Dist:
+semver~=3.0
                       [A hexagonal logo of the viur-cli]
                             ************ vviiuurr--ccllii ************
       _[_B_a_d_g_e_ _s_h_o_w_i_n_g_ _c_u_r_r_e_n_t_ _P_y_P_I_ _v_e_r_s_i_o_n_]_[_B_a_d_g_e_ _d_i_s_p_l_a_y_i_n_g_ _t_h_e_ _l_i_c_e_n_s_e_]
         Command-line interface for _V_i_U_R_ _f_r_a_m_e_w_o_r_k project maintenance.
 ## What does it do? `viur-cli` allows to control, maintain, develop and deploy
 a ViUR project from one central location by using the `viur` command. ##
 Installation To use `viur-cli` in your ViUR projects, install the [PyPI package
```

### Comparing `viur_cli-2.0.0rc6/src/viur_cli.egg-info/SOURCES.txt` & `viur_cli-2.0.1.dev1/src/viur_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 src/viur_cli/__init__.py
 src/viur_cli/build.py
 src/viur_cli/cli.py
 src/viur_cli/cloud.py
 src/viur_cli/conf.py
+src/viur_cli/deprecated.py
 src/viur_cli/local.py
 src/viur_cli/package.py
 src/viur_cli/setup.py
 src/viur_cli/tool.py
 src/viur_cli/update.py
 src/viur_cli/utils.py
 src/viur_cli/version.py
```

