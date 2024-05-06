# Comparing `tmp/dhcptool-2024.4.1.tar.gz` & `tmp/dhcptool-2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhcptool-2024.4.1.tar", max compression
+gzip compressed data, was "dhcptool-2024.5.6.tar", max compression
```

## Comparing `dhcptool-2024.4.1.tar` & `dhcptool-2024.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2023-12-22 05:44:15.721551 dhcptool-2024.4.1/dhcptool/__init__.py
--rw-r--r--   0        0        0     2496 2024-04-01 07:05:43.010035 dhcptool-2024.4.1/dhcptool/base_dhcp_pkt.py
--rw-r--r--   0        0        0     4126 2024-04-01 07:05:42.994433 dhcptool-2024.4.1/dhcptool/code_call_exec.py
--rw-r--r--   0        0        0     6234 2024-04-01 07:05:43.010035 dhcptool-2024.4.1/dhcptool/dhcp4_controller.py
--rw-r--r--   0        0        0     4735 2023-12-22 07:58:02.688484 dhcptool-2024.4.1/dhcptool/dhcp6_controller.py
--rw-r--r--   0        0        0     3438 2023-12-22 05:51:40.991137 dhcptool-2024.4.1/dhcptool/dhcp_pkt_v4.py
--rw-r--r--   0        0        0     6561 2024-04-01 07:05:43.025661 dhcptool-2024.4.1/dhcptool/dhcp_pkt_v6.py
--rw-r--r--   0        0        0     1239 2024-04-01 03:48:22.859693 dhcptool-2024.4.1/dhcptool/dhcptool.yaml
--rw-r--r--   0        0        0      532 2023-11-01 01:49:44.357028 dhcptool-2024.4.1/dhcptool/env_args.py
--rw-r--r--   0        0        0     2276 2024-04-01 07:05:42.990311 dhcptool-2024.4.1/dhcptool/extend_tools_controller.py
--rw-r--r--   0        0        0      921 2024-04-01 07:06:08.446928 dhcptool-2024.4.1/dhcptool/Logings.py
--rw-r--r--   0        0        0     7213 2023-12-22 05:51:40.992137 dhcptool-2024.4.1/dhcptool/main.py
--rw-r--r--   0        0        0    11643 2024-04-01 07:06:08.460124 dhcptool-2024.4.1/dhcptool/options.py
--rw-r--r--   0        0        0    13542 2024-04-01 03:17:19.397976 dhcptool-2024.4.1/dhcptool/tools.py
--rw-r--r--   0        0        0      530 2024-04-01 07:06:42.101984 dhcptool-2024.4.1/pyproject.toml
--rw-r--r--   0        0        0     4026 2023-12-22 05:51:40.989138 dhcptool-2024.4.1/README.md
--rw-r--r--   0        0        0     4552 1970-01-01 00:00:00.000000 dhcptool-2024.4.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-22 05:44:15.721551 dhcptool-2024.5.6/dhcptool/__init__.py
+-rw-r--r--   0        0        0     2496 2024-04-01 07:05:43.010035 dhcptool-2024.5.6/dhcptool/base_dhcp_pkt.py
+-rw-r--r--   0        0        0     4126 2024-04-01 07:05:42.994433 dhcptool-2024.5.6/dhcptool/code_call_exec.py
+-rw-r--r--   0        0        0     6234 2024-04-01 07:05:43.010035 dhcptool-2024.5.6/dhcptool/dhcp4_controller.py
+-rw-r--r--   0        0        0     4735 2023-12-22 07:58:02.688484 dhcptool-2024.5.6/dhcptool/dhcp6_controller.py
+-rw-r--r--   0        0        0     3438 2023-12-22 05:51:40.991137 dhcptool-2024.5.6/dhcptool/dhcp_pkt_v4.py
+-rw-r--r--   0        0        0     6561 2024-04-01 07:05:43.025661 dhcptool-2024.5.6/dhcptool/dhcp_pkt_v6.py
+-rw-r--r--   0        0        0     1239 2024-04-01 03:48:22.859693 dhcptool-2024.5.6/dhcptool/dhcptool.yaml
+-rw-r--r--   0        0        0      532 2023-11-01 01:49:44.357028 dhcptool-2024.5.6/dhcptool/env_args.py
+-rw-r--r--   0        0        0     2276 2024-04-01 07:05:42.990311 dhcptool-2024.5.6/dhcptool/extend_tools_controller.py
+-rw-r--r--   0        0        0      921 2024-04-01 07:06:08.446928 dhcptool-2024.5.6/dhcptool/Logings.py
+-rw-r--r--   0        0        0     7213 2023-12-22 05:51:40.992137 dhcptool-2024.5.6/dhcptool/main.py
+-rw-r--r--   0        0        0    11858 2024-05-06 07:36:08.859709 dhcptool-2024.5.6/dhcptool/options.py
+-rw-r--r--   0        0        0    13542 2024-04-01 03:17:19.397976 dhcptool-2024.5.6/dhcptool/tools.py
+-rw-r--r--   0        0        0      539 2024-05-06 07:50:26.699509 dhcptool-2024.5.6/pyproject.toml
+-rw-r--r--   0        0        0     4026 2023-12-22 05:51:40.989138 dhcptool-2024.5.6/README.md
+-rw-r--r--   0        0        0     4561 1970-01-01 00:00:00.000000 dhcptool-2024.5.6/PKG-INFO
```

### Comparing `dhcptool-2024.4.1/dhcptool/base_dhcp_pkt.py` & `dhcptool-2024.5.6/dhcptool/base_dhcp_pkt.py`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/dhcptool/code_call_exec.py` & `dhcptool-2024.5.6/dhcptool/code_call_exec.py`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/dhcptool/dhcp4_controller.py` & `dhcptool-2024.5.6/dhcptool/dhcp4_controller.py`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/dhcptool/dhcp6_controller.py` & `dhcptool-2024.5.6/dhcptool/dhcp6_controller.py`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/dhcptool/dhcp_pkt_v4.py` & `dhcptool-2024.5.6/dhcptool/dhcp_pkt_v4.py`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/dhcptool/dhcp_pkt_v6.py` & `dhcptool-2024.5.6/dhcptool/dhcp_pkt_v6.py`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/dhcptool/dhcptool.yaml` & `dhcptool-2024.5.6/dhcptool/dhcptool.yaml`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/dhcptool/env_args.py` & `dhcptool-2024.5.6/dhcptool/env_args.py`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/dhcptool/extend_tools_controller.py` & `dhcptool-2024.5.6/dhcptool/extend_tools_controller.py`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/dhcptool/Logings.py` & `dhcptool-2024.5.6/dhcptool/Logings.py`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/dhcptool/main.py` & `dhcptool-2024.5.6/dhcptool/main.py`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/dhcptool/options.py` & `dhcptool-2024.5.6/dhcptool/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,16 @@
                     options.append(self.option_82(i[1], str(op_82_sub_key).rjust(2, '0')))
                 if int(i[0]) == 55:
                     options.append(self.option_55(param_req_list=i[1]))
                 if int(i[0]) == 50:
                     options.append(self.option_50(requested_addr=i[1]))
                 if int(i[0]) == 51:
                     options.append(self.option_51(lease_time=i[1]))
+                if int(i[0]) == 54:
+                    options.append(self.option_54(server_id=i[1]))
                 if int(i[0]) == 2:
                     options.append(self.option_2(time_zone=i[1]))
                 if int(i[0]) == 3:
                     options.append(self.option_3(router=i[1]))
                 if int(i[0]) == 13:
                     options.append(self.option_13(boot_size=i[1]))
                 if int(i[0]) == 15:
@@ -140,14 +142,18 @@
 
         :param lease_time: 租约时间
         :return:
         """
         return 'lease_time', int(lease_time)
 
     @staticmethod
+    def option_54(server_id='0.0.0.0') -> tuple:
+        return 'server_id', server_id
+
+    @staticmethod
     def option_61(client_id: str) -> tuple:
         """
 
         :param client_id: client_id
         :return:
         """
         return 'client_id', client_id
```

### Comparing `dhcptool-2024.4.1/dhcptool/tools.py` & `dhcptool-2024.5.6/dhcptool/tools.py`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/pyproject.toml` & `dhcptool-2024.5.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry.scripts]
 dhcptool = "dhcptool.main:dhcp_main"
 
 [tool.poetry]
 name = "dhcptool"
-version = "2024.4.1"
-description = "支持duid定义"
+version = "2024.5.6"
+description = "支持option54(server_id)"
 authors = ["mf.liang <mf.liang@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6.8"
 scapy = "^2.5.0"
 pyyaml = "^6.0.1"
```

### Comparing `dhcptool-2024.4.1/README.md` & `dhcptool-2024.5.6/README.md`

 * *Files identical despite different names*

### Comparing `dhcptool-2024.4.1/PKG-INFO` & `dhcptool-2024.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dhcptool
-Version: 2024.4.1
-Summary: 支持duid定义
+Version: 2024.5.6
+Summary: 支持option54(server_id)
 Author: mf.liang
 Author-email: mf.liang@outlook.com
 Requires-Python: >=3.6.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

