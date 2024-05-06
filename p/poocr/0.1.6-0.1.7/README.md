# Comparing `tmp/poocr-0.1.6.tar.gz` & `tmp/poocr-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poocr-0.1.6.tar", last modified: Mon Apr 22 14:22:43 2024, max compression
+gzip compressed data, was "poocr-0.1.7.tar", last modified: Mon May  6 13:41:22 2024, max compression
```

## Comparing `poocr-0.1.6.tar` & `poocr-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 14:22:43.910076 poocr-0.1.6/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     3542 2024-04-22 14:22:43.910076 poocr-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2864 2024-04-22 14:21:35.000000 poocr-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 14:22:43.843027 poocr-0.1.6/poocr/
--rw-rw-rw-   0        0        0      810 2024-02-26 13:41:46.000000 poocr-0.1.6/poocr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:22:43.882064 poocr-0.1.6/poocr/api/
--rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.1.6/poocr/api/__init__.py
--rw-rw-rw-   0        0        0    25192 2023-07-25 15:11:46.000000 poocr-0.1.6/poocr/api/ocr.py
--rw-rw-rw-   0        0        0     8291 2024-04-22 14:16:51.000000 poocr-0.1.6/poocr/api/ocr2excel.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:22:43.886075 poocr-0.1.6/poocr/core/
--rw-rw-rw-   0        0        0     4271 2023-07-25 15:06:57.000000 poocr-0.1.6/poocr/core/OCR.py
--rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.1.6/poocr/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:22:43.898078 poocr-0.1.6/poocr/lib/
--rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.1.6/poocr/lib/CommonUtils.py
--rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.1.6/poocr/lib/Config.py
--rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.1.6/poocr/lib/Const.py
--rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.1.6/poocr/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:22:43.906070 poocr-0.1.6/poocr.egg-info/
--rw-rw-rw-   0        0        0     3542 2024-04-22 14:22:43.000000 poocr-0.1.6/poocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2024-04-22 14:22:43.000000 poocr-0.1.6/poocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 14:22:43.000000 poocr-0.1.6/poocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 14:21:59.000000 poocr-0.1.6/poocr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       61 2024-04-22 14:22:43.000000 poocr-0.1.6/poocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-22 14:22:43.000000 poocr-0.1.6/poocr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      759 2024-04-22 14:22:43.919462 poocr-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:22:43.902077 poocr-0.1.6/tests/
--rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0     1214 2024-04-22 14:14:10.000000 poocr-0.1.6/tests/test_tencent.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.243298 poocr-0.1.7/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     3823 2024-05-06 13:41:22.237785 poocr-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3145 2024-04-30 17:27:09.000000 poocr-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.175894 poocr-0.1.7/poocr/
+-rw-rw-rw-   0        0        0      810 2024-02-26 13:41:46.000000 poocr-0.1.7/poocr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.211552 poocr-0.1.7/poocr/api/
+-rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.1.7/poocr/api/__init__.py
+-rw-rw-rw-   0        0        0    25370 2024-05-06 13:35:11.000000 poocr-0.1.7/poocr/api/ocr.py
+-rw-rw-rw-   0        0        0     9163 2024-05-06 13:14:21.000000 poocr-0.1.7/poocr/api/ocr2excel.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.217412 poocr-0.1.7/poocr/core/
+-rw-rw-rw-   0        0        0     1815 2024-05-06 13:38:21.000000 poocr-0.1.7/poocr/core/BaiduOCR.py
+-rw-rw-rw-   0        0        0     4271 2023-07-25 15:06:57.000000 poocr-0.1.7/poocr/core/OCR.py
+-rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.1.7/poocr/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.227708 poocr-0.1.7/poocr/lib/
+-rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.1.7/poocr/lib/CommonUtils.py
+-rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.1.7/poocr/lib/Config.py
+-rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.1.7/poocr/lib/Const.py
+-rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.1.7/poocr/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.237785 poocr-0.1.7/poocr.egg-info/
+-rw-rw-rw-   0        0        0     3823 2024-05-06 13:41:21.000000 poocr-0.1.7/poocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2024-05-06 13:41:22.000000 poocr-0.1.7/poocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:41:21.000000 poocr-0.1.7/poocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 14:21:59.000000 poocr-0.1.7/poocr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       61 2024-05-06 13:41:21.000000 poocr-0.1.7/poocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-06 13:41:21.000000 poocr-0.1.7/poocr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      759 2024-05-06 13:41:22.248565 poocr-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.232731 poocr-0.1.7/tests/
+-rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     1150 2024-04-30 17:30:56.000000 poocr-0.1.7/tests/test_tencent.py
```

### Comparing `poocr-0.1.6/LICENSE` & `poocr-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `poocr-0.1.6/PKG-INFO` & `poocr-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.1.6
+Version: 0.1.7
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
@@ -62,14 +62,19 @@
 
 
 poocr 是一个文字识别的第三方库。
 
 
 -  💻所有功能的讲解👉[5讲OCR批量识别后自动保存为Excel，给小白的Python入门课又增加了！](https://www.bilibili.com/video/BV13J4m1s7L7/)
 
+<p align="center" id='5讲OCR-banner'>
+    <a target="_blank" href='https://www.python-office.com/course-002/5-poocr/5-poocr.html'>
+    <img src="https://course-1300615378.cos.ap-guangzhou.myqcloud.com/poocr%2F%E5%B0%81%E9%9D%A2-%E6%A8%AA.jpg" width="100%"/>
+    </a>   
+</p>
 
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.1.6 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.1.7 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: toml Requires-
 Dist: tencentcloud-sdk-python Requires-Dist: poprogress Requires-Dist: pofile
@@ -14,21 +14,24 @@
   _[_g_i_t_h_u_b_ _s_t_a_r_]_[_g_i_t_e_e_ _s_t_a_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Q_Q_-_1_6_3_4_3_4_4_1_3_-_o_r_a_n_g_e_]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_E_5_%_B_E_%_A_E_%_E_4_%_B_F_%_A_1_-_%_E_4_%_B_A_%_A_4_%_E_6_%_B_5_%_8_1_%_E_7_%_B_E_%_A_4_-
                                  _b_r_i_g_h_t_g_r_e_e_n_]
 ------------------------------------------------------------------------------
 - ## ðç®ä» poocr æ¯ä¸ä¸ªæå­è¯å«çç¬¬ä¸æ¹åºã -
 ð»ææåè½çè®²è§£ð
 [5è®²OCRæ¹éè¯å«åèªå¨ä¿å­ä¸ºExcelï¼ç»å°ç½çPythonå¥é¨è¯¾åå¢å äºï¼]
-(https://www.bilibili.com/video/BV13J4m1s7L7/) --------------------------------
------------------------------------------------ ## ð¦å®è£ ### ðpip
-èªå¨ä¸è½½&æ´æ° ``` pip install -i https://mirrors.aliyun.com/pypi/simple/
-poocr -U ``` ------------------------------------------------------------------
-------------- ## ðå®ç½ - [ðPythonèªå¨ååå¬çå®ç½ðhttps://
-www.python-office.com/](https://www.python-office.com/) ## ðï¸æ·»ç å ç¦
-### ðPRçå»ºè®® poocræ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ã ###
+(https://www.bilibili.com/video/BV13J4m1s7L7/)
+           _[_h_t_t_p_s_:_/_/_c_o_u_r_s_e_-_1_3_0_0_6_1_5_3_7_8_._c_o_s_._a_p_-_g_u_a_n_g_z_h_o_u_._m_y_q_c_l_o_u_d_._c_o_m_/
+                   _p_o_o_c_r_%_2_F_%_E_5_%_B_0_%_8_1_%_E_9_%_9_D_%_A_2_-_%_E_6_%_A_8_%_A_A_._j_p_g_]
+------------------------------------------------------------------------------
+- ## ð¦å®è£ ### ðpip èªå¨ä¸è½½&æ´æ° ``` pip install -i https://
+mirrors.aliyun.com/pypi/simple/ poocr -U ``` ----------------------------------
+--------------------------------------------- ## ðå®ç½ -
+[ðPythonèªå¨ååå¬çå®ç½ðhttps://www.python-office.com/](https://
+www.python-office.com/) ## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®®
+poocræ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ã ###
 ðæä¾bugåé¦æå»ºè®®
 æäº¤é®é¢åé¦æ¶ï¼è¯·å¡å¿å¡«ååpoocrä»£ç æ¬èº«æå³çé®é¢ï¼ä¸è¿è¡æå³pythonå­¦ä¹ ï¼çè³æ¯ä¸ªäººç»ä¹ çç¥è¯ç­çåè®¨è®ºã
 - [Github issue](https://github.com/CoderWanFeng/poocr/issues) ----------------
 --------------------------------------------------------------- ##
 ðèç³»ä½è
 _[_h_t_t_p_s_:_/_/_p_y_t_h_o_n_-_o_f_f_i_c_e_-_1_3_0_0_6_1_5_3_7_8_._c_o_s_._a_p_-_c_h_o_n_g_q_i_n_g_._m_y_q_c_l_o_u_d_._c_o_m_/_p_y_t_h_o_n_-_o_f_f_i_c_e_-
                                     _q_r_._j_p_g_]
```

### Comparing `poocr-0.1.6/README.md` & `poocr-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,19 @@
 
 
 poocr 是一个文字识别的第三方库。
 
 
 -  💻所有功能的讲解👉[5讲OCR批量识别后自动保存为Excel，给小白的Python入门课又增加了！](https://www.bilibili.com/video/BV13J4m1s7L7/)
 
+<p align="center" id='5讲OCR-banner'>
+    <a target="_blank" href='https://www.python-office.com/course-002/5-poocr/5-poocr.html'>
+    <img src="https://course-1300615378.cos.ap-guangzhou.myqcloud.com/poocr%2F%E5%B0%81%E9%9D%A2-%E6%A8%AA.jpg" width="100%"/>
+    </a>   
+</p>
 
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
```

#### html2text {}

```diff
@@ -5,21 +5,24 @@
   _[_g_i_t_h_u_b_ _s_t_a_r_]_[_g_i_t_e_e_ _s_t_a_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Q_Q_-_1_6_3_4_3_4_4_1_3_-_o_r_a_n_g_e_]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_E_5_%_B_E_%_A_E_%_E_4_%_B_F_%_A_1_-_%_E_4_%_B_A_%_A_4_%_E_6_%_B_5_%_8_1_%_E_7_%_B_E_%_A_4_-
                                  _b_r_i_g_h_t_g_r_e_e_n_]
 ------------------------------------------------------------------------------
 - ## ðç®ä» poocr æ¯ä¸ä¸ªæå­è¯å«çç¬¬ä¸æ¹åºã -
 ð»ææåè½çè®²è§£ð
 [5è®²OCRæ¹éè¯å«åèªå¨ä¿å­ä¸ºExcelï¼ç»å°ç½çPythonå¥é¨è¯¾åå¢å äºï¼]
-(https://www.bilibili.com/video/BV13J4m1s7L7/) --------------------------------
------------------------------------------------ ## ð¦å®è£ ### ðpip
-èªå¨ä¸è½½&æ´æ° ``` pip install -i https://mirrors.aliyun.com/pypi/simple/
-poocr -U ``` ------------------------------------------------------------------
-------------- ## ðå®ç½ - [ðPythonèªå¨ååå¬çå®ç½ðhttps://
-www.python-office.com/](https://www.python-office.com/) ## ðï¸æ·»ç å ç¦
-### ðPRçå»ºè®® poocræ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ã ###
+(https://www.bilibili.com/video/BV13J4m1s7L7/)
+           _[_h_t_t_p_s_:_/_/_c_o_u_r_s_e_-_1_3_0_0_6_1_5_3_7_8_._c_o_s_._a_p_-_g_u_a_n_g_z_h_o_u_._m_y_q_c_l_o_u_d_._c_o_m_/
+                   _p_o_o_c_r_%_2_F_%_E_5_%_B_0_%_8_1_%_E_9_%_9_D_%_A_2_-_%_E_6_%_A_8_%_A_A_._j_p_g_]
+------------------------------------------------------------------------------
+- ## ð¦å®è£ ### ðpip èªå¨ä¸è½½&æ´æ° ``` pip install -i https://
+mirrors.aliyun.com/pypi/simple/ poocr -U ``` ----------------------------------
+--------------------------------------------- ## ðå®ç½ -
+[ðPythonèªå¨ååå¬çå®ç½ðhttps://www.python-office.com/](https://
+www.python-office.com/) ## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®®
+poocræ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ã ###
 ðæä¾bugåé¦æå»ºè®®
 æäº¤é®é¢åé¦æ¶ï¼è¯·å¡å¿å¡«ååpoocrä»£ç æ¬èº«æå³çé®é¢ï¼ä¸è¿è¡æå³pythonå­¦ä¹ ï¼çè³æ¯ä¸ªäººç»ä¹ çç¥è¯ç­çåè®¨è®ºã
 - [Github issue](https://github.com/CoderWanFeng/poocr/issues) ----------------
 --------------------------------------------------------------- ##
 ðèç³»ä½è
 _[_h_t_t_p_s_:_/_/_p_y_t_h_o_n_-_o_f_f_i_c_e_-_1_3_0_0_6_1_5_3_7_8_._c_o_s_._a_p_-_c_h_o_n_g_q_i_n_g_._m_y_q_c_l_o_u_d_._c_o_m_/_p_y_t_h_o_n_-_o_f_f_i_c_e_-
                                     _q_r_._j_p_g_]
```

### Comparing `poocr-0.1.6/poocr/__init__.py` & `poocr-0.1.7/poocr/__init__.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.6/poocr/api/ocr.py` & `poocr-0.1.7/poocr/api/ocr.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @Blog      ：www.python-office.com
 @Date    ：2023/1/22 15:23
 @Description     ：
 '''
 
 import sys
 
+from poocr.core.BaiduOCR import BaiduOCR
 from poocr.core.OCR import OCR
 from poocr.lib.CommonUtils import img2base64
 
 
 def get_ocr(configPath, id, key):
     ocr = OCR()
     ocr.set_config(configPath, id, key)
@@ -644,14 +645,18 @@
 def WaybillOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
                   configPath=configPath,
                   id=id, key=key)
 
+
+def social_security_card(img_path, id, key):
+    baidu_ocr = BaiduOCR(id, key)
+    return baidu_ocr.social_security_card(img_path)
 # def VatInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
 #     """
 #     增值税发票的识别
 #     :param img_path: 必填，发票的图片位置
 #     :param configPath: 选填，配置文件的位置，有默认值
 #     :return:
 #     """
```

### Comparing `poocr-0.1.6/poocr/api/ocr2excel.py` & `poocr-0.1.7/poocr/api/ocr2excel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # -*- coding: UTF-8 -*-
 '''
 @作者 ：B站/抖音/微博/小红书/公众号，都叫：程序员晚枫
 @微信 ：CoderWanFeng : https://mp.weixin.qq.com/s/yFcocJbfS9Hs375NhE8Gbw
 @个人网站 ：www.python-office.com
 @Date    ：2023/3/25 18:53
 @Description     ：
+- id和key：
+    - 开通和使用👉[免费教程](https://curl.qcloud.com/fuOGcm2R)
+
 '''
 import json
 from pathlib import Path
 
 import pandas as pd
 from pofile import get_files, mkdir
 from poprogress import simple_progress
 
 import poocr
 from poocr.api.ocr import VatInvoiceOCR, IDCardOCR
 
 
 def VatInvoiceOCR2Excel(input_path, output_path=None, output_excel='VatInvoiceOCR2Excel.xlsx', img_url=None,
-                        configPath=None, id=None, key=None):
+                        configPath=None, id=None, key=None, file_name=False, trans=False):
     """
     批量识别发票，并保存在Excel中
     :param input_path: 发票存放位置，可以填单个文件，也可以填一个目录
     :param output_path:
     :param output_excel:
     :param img_url:
     :param configPath:
@@ -45,21 +48,39 @@
         try:
             api_res = VatInvoiceOCR(img_path=str(vat_img), img_url=img_url, configPath=configPath, id=id, key=key)
             api_res_json = json.loads(str(api_res))
             VatInvoiceInfos = api_res_json['VatInvoiceInfos']
             dict_pandas = {}  # 存放一行数据
             # 读返回值的第一个key
             for VatInvoiceInfo in VatInvoiceInfos:
+                if file_name:
+                    dict_pandas['文件名'] = Path(vat_img).name  # 增加文件名作为一列
+
                 dict_pandas[VatInvoiceInfo['Name']] = VatInvoiceInfo['Value']
             # 读返回值的第二个key
+            key_trans_history = {}
+            new_item_json = []
             Items = api_res_json['Items']
-            for Item in Items:
+            if trans:
+                import wftools
+
+                for i in Items:
+                    new_i = {}
+                    for k, v in i.items():
+                        if key_trans_history.get(k, None) == None:
+                            key_trans_history[k] = wftools.transtools(k, to_lang='zh', from_lang='en')
+                        new_i[key_trans_history.get(k)] = v
+                    new_item_json.append(new_i)
+            else:
+                new_item_json = Items
+            for Item in new_item_json:
                 dict_pandas.update(Item)
                 res_df.append(pd.DataFrame(dict_pandas, index=[0]))
-        except:
+        except Exception as e:
+            print(e)
             continue
     # 整理全部识别结果
     if len(res_df) > 0:
         res_excel = res_df[0]
         for index, line_df in enumerate(res_df):
             if index == 0:
                 continue
```

### Comparing `poocr-0.1.6/poocr/core/OCR.py` & `poocr-0.1.7/poocr/core/OCR.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.6/poocr/lib/CommonUtils.py` & `poocr-0.1.7/poocr/lib/CommonUtils.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.6/poocr/lib/Config.py` & `poocr-0.1.7/poocr/lib/Config.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.6/poocr/lib/Const.py` & `poocr-0.1.7/poocr/lib/Const.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.6/poocr.egg-info/PKG-INFO` & `poocr-0.1.7/poocr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.1.6
+Version: 0.1.7
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
@@ -62,14 +62,19 @@
 
 
 poocr 是一个文字识别的第三方库。
 
 
 -  💻所有功能的讲解👉[5讲OCR批量识别后自动保存为Excel，给小白的Python入门课又增加了！](https://www.bilibili.com/video/BV13J4m1s7L7/)
 
+<p align="center" id='5讲OCR-banner'>
+    <a target="_blank" href='https://www.python-office.com/course-002/5-poocr/5-poocr.html'>
+    <img src="https://course-1300615378.cos.ap-guangzhou.myqcloud.com/poocr%2F%E5%B0%81%E9%9D%A2-%E6%A8%AA.jpg" width="100%"/>
+    </a>   
+</p>
 
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.1.6 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.1.7 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: toml Requires-
 Dist: tencentcloud-sdk-python Requires-Dist: poprogress Requires-Dist: pofile
@@ -14,21 +14,24 @@
   _[_g_i_t_h_u_b_ _s_t_a_r_]_[_g_i_t_e_e_ _s_t_a_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Q_Q_-_1_6_3_4_3_4_4_1_3_-_o_r_a_n_g_e_]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_E_5_%_B_E_%_A_E_%_E_4_%_B_F_%_A_1_-_%_E_4_%_B_A_%_A_4_%_E_6_%_B_5_%_8_1_%_E_7_%_B_E_%_A_4_-
                                  _b_r_i_g_h_t_g_r_e_e_n_]
 ------------------------------------------------------------------------------
 - ## ðç®ä» poocr æ¯ä¸ä¸ªæå­è¯å«çç¬¬ä¸æ¹åºã -
 ð»ææåè½çè®²è§£ð
 [5è®²OCRæ¹éè¯å«åèªå¨ä¿å­ä¸ºExcelï¼ç»å°ç½çPythonå¥é¨è¯¾åå¢å äºï¼]
-(https://www.bilibili.com/video/BV13J4m1s7L7/) --------------------------------
------------------------------------------------ ## ð¦å®è£ ### ðpip
-èªå¨ä¸è½½&æ´æ° ``` pip install -i https://mirrors.aliyun.com/pypi/simple/
-poocr -U ``` ------------------------------------------------------------------
-------------- ## ðå®ç½ - [ðPythonèªå¨ååå¬çå®ç½ðhttps://
-www.python-office.com/](https://www.python-office.com/) ## ðï¸æ·»ç å ç¦
-### ðPRçå»ºè®® poocræ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ã ###
+(https://www.bilibili.com/video/BV13J4m1s7L7/)
+           _[_h_t_t_p_s_:_/_/_c_o_u_r_s_e_-_1_3_0_0_6_1_5_3_7_8_._c_o_s_._a_p_-_g_u_a_n_g_z_h_o_u_._m_y_q_c_l_o_u_d_._c_o_m_/
+                   _p_o_o_c_r_%_2_F_%_E_5_%_B_0_%_8_1_%_E_9_%_9_D_%_A_2_-_%_E_6_%_A_8_%_A_A_._j_p_g_]
+------------------------------------------------------------------------------
+- ## ð¦å®è£ ### ðpip èªå¨ä¸è½½&æ´æ° ``` pip install -i https://
+mirrors.aliyun.com/pypi/simple/ poocr -U ``` ----------------------------------
+--------------------------------------------- ## ðå®ç½ -
+[ðPythonèªå¨ååå¬çå®ç½ðhttps://www.python-office.com/](https://
+www.python-office.com/) ## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®®
+poocræ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ã ###
 ðæä¾bugåé¦æå»ºè®®
 æäº¤é®é¢åé¦æ¶ï¼è¯·å¡å¿å¡«ååpoocrä»£ç æ¬èº«æå³çé®é¢ï¼ä¸è¿è¡æå³pythonå­¦ä¹ ï¼çè³æ¯ä¸ªäººç»ä¹ çç¥è¯ç­çåè®¨è®ºã
 - [Github issue](https://github.com/CoderWanFeng/poocr/issues) ----------------
 --------------------------------------------------------------- ##
 ðèç³»ä½è
 _[_h_t_t_p_s_:_/_/_p_y_t_h_o_n_-_o_f_f_i_c_e_-_1_3_0_0_6_1_5_3_7_8_._c_o_s_._a_p_-_c_h_o_n_g_q_i_n_g_._m_y_q_c_l_o_u_d_._c_o_m_/_p_y_t_h_o_n_-_o_f_f_i_c_e_-
                                     _q_r_._j_p_g_]
```

### Comparing `poocr-0.1.6/setup.cfg` & `poocr-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f6f 6372 0d0a 7665 7273 696f   = poocr..versio
-00000020: 6e20 3d20 302e 312e 360d 0a64 6573 6372  n = 0.1.6..descr
+00000020: 6e20 3d20 302e 312e 370d 0a64 6573 6372  n = 0.1.7..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f6f 6372 0d0a 6c6f 6e67  tall poocr..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `poocr-0.1.6/tests/test_tencent.py` & `poocr-0.1.7/tests/test_tencent.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from poocr.api.ocr2excel import *
 
 
 class TestTencent(unittest.TestCase):
 
     def setUp(self):
-        self.SecretId = 'AKIDITXZTE65a7Ujy77EScqy9D7nESSEmKoC'
-        self.SecretKey = 'V4eI2f6A8vYBiECEFU2NUP8uXxEHOafh'
+        # self.SecretId = ''
+        # self.SecretKey = ''
 
     def test_vin_ocr(self):
         r = VatInvoiceOCR(img_path=r'C:\Users\Lenovo\Desktop\temp\增值税发票-test.jpg')
         print(r)
 
     def test_idcard_ocr(self):
         res = IDCardOCR(
```

