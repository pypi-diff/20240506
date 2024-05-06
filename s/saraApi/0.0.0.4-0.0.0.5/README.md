# Comparing `tmp/saraapi-0.0.0.4.tar.gz` & `tmp/saraapi-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saraapi-0.0.0.4.tar", last modified: Mon May  6 04:00:51 2024, max compression
+gzip compressed data, was "saraapi-0.0.0.5.tar", last modified: Mon May  6 04:11:51 2024, max compression
```

## Comparing `saraapi-0.0.0.4.tar` & `saraapi-0.0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 04:00:51.923983 saraapi-0.0.0.4/
--rw-rw-rw-   0        0        0        0 2024-05-05 23:25:57.000000 saraapi-0.0.0.4/LICENSE
--rw-rw-rw-   0        0        0     4836 2024-05-06 04:00:51.917591 saraapi-0.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4103 2024-05-06 03:57:18.000000 saraapi-0.0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 04:00:51.840642 saraapi-0.0.0.4/sara/
--rw-rw-rw-   0        0        0       81 2024-04-29 01:35:10.000000 saraapi-0.0.0.4/sara/__init__.py
--rw-rw-rw-   0        0        0      587 2024-04-29 01:33:03.000000 saraapi-0.0.0.4/sara/ext.py
--rw-rw-rw-   0        0        0     1937 2024-04-29 01:33:40.000000 saraapi-0.0.0.4/sara/nsfw.py
--rw-rw-rw-   0        0        0      626 2024-05-06 01:28:07.000000 saraapi-0.0.0.4/sara/req.py
--rw-rw-rw-   0        0        0      219 2024-04-29 01:34:39.000000 saraapi-0.0.0.4/sara/sfw.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:00:51.911617 saraapi-0.0.0.4/saraApi.egg-info/
--rw-rw-rw-   0        0        0     4836 2024-05-06 04:00:51.000000 saraapi-0.0.0.4/saraApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-06 04:00:51.000000 saraapi-0.0.0.4/saraApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 04:00:51.000000 saraapi-0.0.0.4/saraApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-06 04:00:51.000000 saraapi-0.0.0.4/saraApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-06 04:00:51.000000 saraapi-0.0.0.4/saraApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 04:00:51.925359 saraapi-0.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-05-06 03:58:47.000000 saraapi-0.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:11:51.853669 saraapi-0.0.0.5/
+-rw-rw-rw-   0        0        0        0 2024-05-05 23:25:57.000000 saraapi-0.0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4814 2024-05-06 04:11:51.845513 saraapi-0.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4081 2024-05-06 04:10:31.000000 saraapi-0.0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 04:11:51.793495 saraapi-0.0.0.5/sara/
+-rw-rw-rw-   0        0        0       81 2024-04-29 01:35:10.000000 saraapi-0.0.0.5/sara/__init__.py
+-rw-rw-rw-   0        0        0      587 2024-04-29 01:33:03.000000 saraapi-0.0.0.5/sara/ext.py
+-rw-rw-rw-   0        0        0     1937 2024-04-29 01:33:40.000000 saraapi-0.0.0.5/sara/nsfw.py
+-rw-rw-rw-   0        0        0      626 2024-05-06 01:28:07.000000 saraapi-0.0.0.5/sara/req.py
+-rw-rw-rw-   0        0        0      219 2024-04-29 01:34:39.000000 saraapi-0.0.0.5/sara/sfw.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:11:51.840990 saraapi-0.0.0.5/saraApi.egg-info/
+-rw-rw-rw-   0        0        0     4814 2024-05-06 04:11:51.000000 saraapi-0.0.0.5/saraApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-06 04:11:51.000000 saraapi-0.0.0.5/saraApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 04:11:51.000000 saraapi-0.0.0.5/saraApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 04:11:51.000000 saraapi-0.0.0.5/saraApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-06 04:11:51.000000 saraapi-0.0.0.5/saraApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 04:11:51.854391 saraapi-0.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2024-05-06 04:10:47.000000 saraapi-0.0.0.5/setup.py
```

### Comparing `saraapi-0.0.0.4/PKG-INFO` & `saraapi-0.0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saraApi
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: sara api public based akanekopy
 Home-page: https://github.com/EverGasterXd/sara_api
 Author: evergaster
 License: MIT license
 Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 <div align="center">
   <br />
   <p>
-    <a href="https://discord.gg/DxHvWwC"><img src="https://cdn.donmai.us/original/65/bd/__modeus_helltaker_drawn_by_kiyovero__65bd0b99d080bceb39fff3f4de7cc586.png" width="146" height="200" alt="Cute As Fubuki" /></a>
+    <a href="https://discord.gg/DxHvWwC"><img src="https://cdn.donmai.us/original/65/bd/__modeus_helltaker_drawn_by_kiyovero__65bd0b99d080bceb39fff3f4de7cc586.png" width="146" height="200"/></a>
   </p>
   <br />
 </div>
 sara is both a SFW and NSFW Wrapper, there's hentais for you perverts to use, however do understand that I'm the only one working on this, and I hand pick images to add, so you may get repeated images! Use it for your Discord Bot, your Self Made Console Waifu, or whatever it is :3
 
 ## NOTE: This Readme.md is from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/)
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: saraApi Version: 0.0.0.4 Summary: sara api public
+Metadata-Version: 2.1 Name: saraApi Version: 0.0.0.5 Summary: sara api public
 based akanekopy Home-page: https://github.com/EverGasterXd/sara_api Author:
 evergaster License: MIT license Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Development Status :: 4 - Beta Classifier:
 Natural Language :: English Classifier: Operating System :: Microsoft ::
 Windows :: Windows 10 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
 Requires-Python: >=3.0 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests
 
-                               _[_C_u_t_e_ _A_s_ _F_u_b_u_k_i_]
+                    _[_h_t_t_p_s_:_/_/_c_d_n_._d_o_n_m_a_i_._u_s_/_o_r_i_g_i_n_a_l_/_6_5_/_b_d_/
+  _____m_o_d_e_u_s___h_e_l_l_t_a_k_e_r___d_r_a_w_n___b_y___k_i_y_o_v_e_r_o_____6_5_b_d_0_b_9_9_d_0_8_0_b_c_e_b_3_9_f_f_f_3_f_4_d_e_7_c_c_5_8_6_._p_n_g_]
 
 sara is both a SFW and NSFW Wrapper, there's hentais for you perverts to use,
 however do understand that I'm the only one working on this, and I hand pick
 images to add, so you may get repeated images! Use it for your Discord Bot,
 your Self Made Console Waifu, or whatever it is :3 ## NOTE: This Readme.md is
 from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/) ##
 Changelogs ### v0.1 - new api ## Example(s) **Python:** ```python import sara
```

### Comparing `saraapi-0.0.0.4/README.md` & `saraapi-0.0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div align="center">
   <br />
   <p>
-    <a href="https://discord.gg/DxHvWwC"><img src="https://cdn.donmai.us/original/65/bd/__modeus_helltaker_drawn_by_kiyovero__65bd0b99d080bceb39fff3f4de7cc586.png" width="146" height="200" alt="Cute As Fubuki" /></a>
+    <a href="https://discord.gg/DxHvWwC"><img src="https://cdn.donmai.us/original/65/bd/__modeus_helltaker_drawn_by_kiyovero__65bd0b99d080bceb39fff3f4de7cc586.png" width="146" height="200"/></a>
   </p>
   <br />
 </div>
 sara is both a SFW and NSFW Wrapper, there's hentais for you perverts to use, however do understand that I'm the only one working on this, and I hand pick images to add, so you may get repeated images! Use it for your Discord Bot, your Self Made Console Waifu, or whatever it is :3
 
 ## NOTE: This Readme.md is from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/)
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 
-                               _[_C_u_t_e_ _A_s_ _F_u_b_u_k_i_]
+                    _[_h_t_t_p_s_:_/_/_c_d_n_._d_o_n_m_a_i_._u_s_/_o_r_i_g_i_n_a_l_/_6_5_/_b_d_/
+  _____m_o_d_e_u_s___h_e_l_l_t_a_k_e_r___d_r_a_w_n___b_y___k_i_y_o_v_e_r_o_____6_5_b_d_0_b_9_9_d_0_8_0_b_c_e_b_3_9_f_f_f_3_f_4_d_e_7_c_c_5_8_6_._p_n_g_]
 
 sara is both a SFW and NSFW Wrapper, there's hentais for you perverts to use,
 however do understand that I'm the only one working on this, and I hand pick
 images to add, so you may get repeated images! Use it for your Discord Bot,
 your Self Made Console Waifu, or whatever it is :3 ## NOTE: This Readme.md is
 from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/) ##
 Changelogs ### v0.1 - new api ## Example(s) **Python:** ```python import sara
```

### Comparing `saraapi-0.0.0.4/sara/ext.py` & `saraapi-0.0.0.5/sara/ext.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.0.4/sara/nsfw.py` & `saraapi-0.0.0.5/sara/nsfw.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.0.4/sara/req.py` & `saraapi-0.0.0.5/sara/req.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.0.4/saraApi.egg-info/PKG-INFO` & `saraapi-0.0.0.5/saraApi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saraApi
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: sara api public based akanekopy
 Home-page: https://github.com/EverGasterXd/sara_api
 Author: evergaster
 License: MIT license
 Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 <div align="center">
   <br />
   <p>
-    <a href="https://discord.gg/DxHvWwC"><img src="https://cdn.donmai.us/original/65/bd/__modeus_helltaker_drawn_by_kiyovero__65bd0b99d080bceb39fff3f4de7cc586.png" width="146" height="200" alt="Cute As Fubuki" /></a>
+    <a href="https://discord.gg/DxHvWwC"><img src="https://cdn.donmai.us/original/65/bd/__modeus_helltaker_drawn_by_kiyovero__65bd0b99d080bceb39fff3f4de7cc586.png" width="146" height="200"/></a>
   </p>
   <br />
 </div>
 sara is both a SFW and NSFW Wrapper, there's hentais for you perverts to use, however do understand that I'm the only one working on this, and I hand pick images to add, so you may get repeated images! Use it for your Discord Bot, your Self Made Console Waifu, or whatever it is :3
 
 ## NOTE: This Readme.md is from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/)
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: saraApi Version: 0.0.0.4 Summary: sara api public
+Metadata-Version: 2.1 Name: saraApi Version: 0.0.0.5 Summary: sara api public
 based akanekopy Home-page: https://github.com/EverGasterXd/sara_api Author:
 evergaster License: MIT license Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Development Status :: 4 - Beta Classifier:
 Natural Language :: English Classifier: Operating System :: Microsoft ::
 Windows :: Windows 10 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
 Requires-Python: >=3.0 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests
 
-                               _[_C_u_t_e_ _A_s_ _F_u_b_u_k_i_]
+                    _[_h_t_t_p_s_:_/_/_c_d_n_._d_o_n_m_a_i_._u_s_/_o_r_i_g_i_n_a_l_/_6_5_/_b_d_/
+  _____m_o_d_e_u_s___h_e_l_l_t_a_k_e_r___d_r_a_w_n___b_y___k_i_y_o_v_e_r_o_____6_5_b_d_0_b_9_9_d_0_8_0_b_c_e_b_3_9_f_f_f_3_f_4_d_e_7_c_c_5_8_6_._p_n_g_]
 
 sara is both a SFW and NSFW Wrapper, there's hentais for you perverts to use,
 however do understand that I'm the only one working on this, and I hand pick
 images to add, so you may get repeated images! Use it for your Discord Bot,
 your Self Made Console Waifu, or whatever it is :3 ## NOTE: This Readme.md is
 from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/) ##
 Changelogs ### v0.1 - new api ## Example(s) **Python:** ```python import sara
```

### Comparing `saraapi-0.0.0.4/setup.py` & `saraapi-0.0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md','r', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 install_requires = [
 	'requests'
 ]
 
-version = '0.0.0.4'
+version = '0.0.0.5'
 
 setup(
     author='evergaster',
     version=version,
     description='sara api public based akanekopy',
     install_package_data=True,
     install_requires=install_requires,
```

