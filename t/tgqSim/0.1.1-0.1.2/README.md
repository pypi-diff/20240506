# Comparing `tmp/tgqSim-0.1.1.tar.gz` & `tmp/tgqSim-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgqSim-0.1.1.tar", last modified: Mon Apr 22 05:59:12 2024, max compression
+gzip compressed data, was "tgqSim-0.1.2.tar", last modified: Mon May  6 06:10:07 2024, max compression
```

## Comparing `tgqSim-0.1.1.tar` & `tgqSim-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:59:12.418388 tgqSim-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-04-22 05:59:11.000000 tgqSim-0.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-22 05:59:11.000000 tgqSim-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      752 2024-04-22 05:59:12.418388 tgqSim-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-22 05:59:11.000000 tgqSim-0.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 05:59:12.418388 tgqSim-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-22 05:59:11.000000 tgqSim-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:59:12.415388 tgqSim-0.1.1/tgqSim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:59:12.417388 tgqSim-0.1.1/tgqSim/GateSimulation/
--rw-rw-rw-   0 root         (0) root         (0)     3793 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/GateSimulation/DoubleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/GateSimulation/SingleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/GateSimulation/TripleGate.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/GateSimulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16519 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/QuantumCircuit.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18468 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/draw_circuit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:59:12.418388 tgqSim-0.1.1/tgqSim/lib/
--rw-rw-rw-   0 root         (0) root         (0)    67288 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/lib/tgq_simulator.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:59:12.417388 tgqSim-0.1.1/tgqSim.egg-info/
--rw-r--r--   0 root         (0) root         (0)      752 2024-04-22 05:59:12.000000 tgqSim-0.1.1/tgqSim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      430 2024-04-22 05:59:12.000000 tgqSim-0.1.1/tgqSim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 05:59:12.000000 tgqSim-0.1.1/tgqSim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-22 05:59:12.000000 tgqSim-0.1.1/tgqSim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-22 05:59:12.000000 tgqSim-0.1.1/tgqSim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:10:07.921466 tgqSim-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-06 06:10:06.000000 tgqSim-0.1.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-06 06:10:06.000000 tgqSim-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      752 2024-05-06 06:10:07.920466 tgqSim-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-06 06:10:06.000000 tgqSim-0.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 06:10:07.921466 tgqSim-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2024-05-06 06:10:07.000000 tgqSim-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:10:07.918466 tgqSim-0.1.2/tgqSim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:10:07.920466 tgqSim-0.1.2/tgqSim/GateSimulation/
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/GateSimulation/DoubleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/GateSimulation/SingleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/GateSimulation/TripleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/GateSimulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21020 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/QuantumCircuit.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-06 06:10:07.000000 tgqSim-0.1.2/tgqSim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/draw_circuit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:10:07.920466 tgqSim-0.1.2/tgqSim/lib/
+-rw-rw-rw-   0 root         (0) root         (0)    67288 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/lib/tgq_simulator.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:10:07.919466 tgqSim-0.1.2/tgqSim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      752 2024-05-06 06:10:07.000000 tgqSim-0.1.2/tgqSim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-06 06:10:07.000000 tgqSim-0.1.2/tgqSim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 06:10:07.000000 tgqSim-0.1.2/tgqSim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-06 06:10:07.000000 tgqSim-0.1.2/tgqSim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-06 06:10:07.000000 tgqSim-0.1.2/tgqSim.egg-info/top_level.txt
```

### Comparing `tgqSim-0.1.1/LICENSE` & `tgqSim-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.1/PKG-INFO` & `tgqSim-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.1
+Version: 0.1.2
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,cetc,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `tgqSim-0.1.1/setup.py` & `tgqSim-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tgqSim',
-    version='0.1.1',
+    version='0.1.2',
     description='TGQ量子模拟器',  # 包描述
     long_description="Python for quantum simulation http://www.tiangongqs.com",  # 详细描述
     long_description_content_type='text/markdown',
     author='tiangongqs',  # 作者姓名
     license='MIT',  # 许可证
     package=find_packages(),
     include_package_data=True,
```

### Comparing `tgqSim-0.1.1/tgqSim/GateSimulation/DoubleGate.py` & `tgqSim-0.1.2/tgqSim/GateSimulation/DoubleGate.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,16 @@
                         psi[i1], psi[i2] = psi[i2],  psi[i1]
                 elif Gate_type == 'iswap':
                         psi[i1], psi[i2] = 1j * psi[i2], 1j * psi[i1]
                 elif Gate_type == 'cz':
                         psi[i3] = -1.0 * psi[i3]
                 elif Gate_type == 'cp':
                         psi[i3] = cm.exp(1j * Angles[0]) * psi[i3]
+                elif Gate_type == 'syc':
+                      psi[i1], psi[i2], psi[i3] = 1j * psi[i2], 1j * psi[i1], cm.exp(-1j * np.pi / 6) * psi[i3]
                 elif Gate_type == 'rxx':
                         psi[i0], psi[i3] = cm.cos(Angles[0] / 2.0) *  psi[i0] + (-1j) * cm.sin(
                             Angles[0] / 2.0) *  psi[i3], \
                                                     cm.cos(Angles[0] / 2.0) *  psi[i3] + (-1j) * cm.sin(
                                                         Angles[0] / 2.0) *  psi[i0]
                         psi[i1], psi[i2] = cm.cos(Angles[0] / 2.0) * psi[i1] + (-1j) * cm.sin(
                             Angles[0] / 2.0) *  psi[i2], \
```

### Comparing `tgqSim-0.1.1/tgqSim/GateSimulation/SingleGate.py` & `tgqSim-0.1.2/tgqSim/GateSimulation/SingleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.1/tgqSim/GateSimulation/TripleGate.py` & `tgqSim-0.1.2/tgqSim/GateSimulation/TripleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.1/tgqSim/QuantumCircuit.py` & `tgqSim-0.1.2/tgqSim/QuantumCircuit.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 """
 @author: Yuchen He
 @contact: heyuchen@tgqs.net
 @version: 1.0.1
 @file: QuantumCircuit.py
 @time: 2024/1/16 17:16
+
+@Modifider: Zhiqiang Wang
+@contact: wangzhiqiang@tgqs.net
+@version: 0.1.1
+@file: QuantumCircuit.py
+@time: 2024/04/19 15:36
 """
 from tgqSim.GateSimulation import SingleGate, DoubleGate, TripleGate
 from typing import Union
 import random, os, ctypes
 import numpy as np
 import tgqSim.draw_circuit_tools as tools
 import matplotlib.pyplot as plt
@@ -55,21 +61,25 @@
 class QuantumCircuit:
     def __init__(self, qbit_number=None):
         self.qbit_list = [] if not qbit_number else self.add_qubits(number=qbit_number)
         self.cbit_list = []
         self.gate_list = []
         self.qbit_register = {}
         self.base_single_gate = ['h', 'x', 'y', 'z', 'rx', 'ry', 'rz', 'u3', 's', 'sdg', 't', 'tdg']
-        self.base_double_gate = ['cx', 'swap', 'iswap', 'cz', 'cp', 'rxx', 'ryy', 'rzz']
+        self.base_double_gate = ['cx', 'swap', 'iswap', 'cz', 'cp', 'rxx', 'ryy', 'rzz', 'syc']
         self.base_triple_gate = ['ccx', 'cswap']
+        self.noise_mapper = {"bit_flip": "BF", "asymmetric_depolarization": "ADP", "depolarize": "DP", "phase_flip": "PF"}
         self.width = 0
         self.state = []
         self.circuit_diag = []
         self.isgpu = False
         self.deviceid = []
+        self.noise_circuit = []
+        self.current_gate_info = ()
+        self.prob_result = {}
 
     def add_qubits(self, number: int, name: str = 'p'):
         """
         添加量子比特
         :param number: 比特数量
         :param name: 比特名称
         :return:
@@ -92,15 +102,18 @@
         :return:
         """
         if isinstance(gate_pos, int):
             gatename = gate_info[0].upper()
             self.circuit_diag.append([(gatename, gate_pos)])
         else:
             self.circuit_diag.append([(gatename, int(gate_pos))])
-        return self.gate_list.append((gate_pos, gate_info))
+        self.current_gate_info = (gate_pos, gate_info)
+        self.gate_list.append((gate_pos, gate_info))
+        # print("over")
+        return self
         # todo 通过比特名称访问
         # if isinstance(gate_pos, str):
         #     return self.gate_list.append((gate_pos, gate_type))
 
     def add_double_gate(self, gate_pos_0, gate_pos_1, *gate_info):
         """
         添加两比特门序列
@@ -109,39 +122,42 @@
         :param gate_info: 门类型，门参数
         :return:
         """
         if gate_info[0] in ["rxx", 'ryy', 'rzz', 'iswap', 'syc']:
             self.circuit_diag.append([(gate_info[0].upper(), (gate_pos_1, gate_pos_0))])
         else:
             self.circuit_diag.append([(gate_info[0].upper(), gate_pos_1, gate_pos_0)])
-        return self.gate_list.append(([gate_pos_0, gate_pos_1], gate_info))
+        self.current_gate_info = ([gate_pos_0, gate_pos_1], gate_info)
+        self.gate_list.append(([gate_pos_0, gate_pos_1], gate_info))
+        return self
 
     def add_triple_gate(self, gate_pos, *gate_info):
         """
         添加三比特门序列
         :param gate_pos:
         :param gate_info:
         :return:
         """
         self.circuit_diag.append([(gate_info[0].upper(), gate_pos[2], gate_pos[0], gate_pos[1])])
-        return self.gate_list.append((gate_pos, gate_info))
+        self.current_gate_info = (gate_pos, gate_info)
+        self.gate_list.append((gate_pos, gate_info))
+        return self
     
     def setdevice(self, deviceList: Union[int, list]):
         gpus = GPUtil.getGPUs()
         gpuidList = [gpu.id for gpu in gpus]
         if isinstance(deviceList, int):
             deviceList = [deviceList]
         for deviceid in deviceList:
             if deviceid not in gpuidList:
                 raise ValueError("设置设备ID不存在")
         self.isgpu = True
         self.deviceid = deviceList
     
     def _run_with_device(self):
-        # 未测试
         dll_path = os.path.abspath('./lib/tgq_simulator.so')
         lib = ctypes.CDLL(dll_path)
         lib.execute_circuit.argtypes = [
             ctypes.POINTER(Float2),
             ctypes.POINTER(GateInfo),
             ctypes.c_int,
             ctypes.c_int,
@@ -167,20 +183,41 @@
         gateInfoCData = (GateInfo * len(gateInfo))(*gateInfo)
         initial_state = [Float2(1.0, 0.0) if i == 0 else Float2(0.0, 0.0) for i in range(2 ** self.width)]
         psi = (Float2 * len(initial_state))(*initial_state)
         lib.execute_circuit(psi, gateInfoCData, len(gateInfo), self.width, self.deviceid[0])
         for i, ele in enumerate(psi):
             self.state[i] = ele.x + 1j * ele.y
 
+    def run_with_noise(self, shots:int=1000):
+        noise_type = ["bit_flip", "asymmetric_depolarization", "depolarize", "phase_flip"]
+        result_dict = {}
+        for _ in range(shots):
+            new_circuit = []
+            for (gate_pos, gate_info) in self.noise_circuit:
+                if gate_info[0] in noise_type:
+                    noise_gate = QuantumCircuit.parse_noise(noise_type=gate_info[0], gate_pos=gate_pos, error_rate=gate_info[1])
+                    if noise_gate is not None:
+                        new_circuit.append(noise_gate)
+                else:
+                    new_circuit.append((gate_pos, gate_info))
+            self.gate_list = new_circuit
+            result = self.measure(measure_bits_list=[i for i in range(self.width)], shots=1)
+            key = list(result.keys())[0]
+            if key in result_dict:
+                result_dict[key] += 1
+            else:
+                result_dict[key] = 1
+        self.prob_result = result_dict
+
     def run_statevector(self):
         """
         根据线路的门序列计算末态的量子态
         :return:
         """
-        self.state = [1 if a == 0 else 0 for a in range(2**self.width)]
+        self.state = [1 if a == 0 else 0 for a in range(2**self.width)]            
         if not self.isgpu:
             for (gate_pos, gate_info) in self.gate_list:
                 gate_type = gate_info[0]
                 angle = tuple(gate_info[1:])
                 if gate_type in self.base_single_gate:
                     self.state = SingleGate.ActOn_State(self.state, self.width, gate_type, gate_pos, *angle)
 
@@ -195,14 +232,94 @@
                         raise SimulationError(f"Gate position cannot be the same: "
                                             f"{gate_pos[0]}, {gate_pos[1]} and {gate_pos[2]}")
                     self.state = TripleGate.ActOn_State(self.state, self.width, gate_type, gate_pos, *angle)
                 else:
                     raise SimulationError(f"Unkown gate type: {gate_type}")
         else:
             self._run_with_device()
+        
+    def with_noise(self, noise_type:str, error_rate:Union[float, list]):
+        """
+        将当前的所有控制门都加上noise_type类型的噪声
+
+        Args:
+            noise_type (str): 噪声类型
+            error_rate (Union[float, list]): 错误率
+        """
+        self.noise_circuit += [self.current_gate_info]
+        gate_pos = self.current_gate_info[0]
+        if isinstance(gate_pos, int):
+            self.noise_circuit += [(gate_pos, (noise_type, error_rate))]
+            self.circuit_diag.append([(self.noise_mapper[noise_type], gate_pos)])
+        else:
+            for gate in gate_pos:
+                self.noise_circuit += [(gate, (noise_type, error_rate))]
+                self.circuit_diag.append([(self.noise_mapper[noise_type], gate)])
+    
+    @staticmethod
+    def parse_noise(noise_type: str,  gate_pos: int, error_rate: Union[float, list]):
+        """
+        对于不同的噪声类型，返回不同的信息
+
+        Args:
+            noise_type (str): 噪声类型
+            error_rate Union[float, list]: 门错误率信息
+        """
+        gate_name = "I"
+        if "bit_flip" == noise_type:
+            gate_name = QuantumCircuit.bit_flip(error_rate)
+        elif "asymmetric_depolarization" == noise_type:
+            gate_name = QuantumCircuit.asymmetric_depolarization(error_rate)
+        elif "depolarize" == noise_type:
+            gate_name = QuantumCircuit.depolarize(error_rate)
+        elif "phase_flip" == noise_type:
+            gate_name = QuantumCircuit.phase_flip(error_rate)
+        else:
+            raise ValueError("Please check noise model name")
+        if gate_name == "I":
+            return None
+        return (gate_pos, (gate_name))
+    
+    @staticmethod
+    def bit_flip(error_rate: float):
+        random_value = random.uniform(0, 1)
+        gate_name = "I"
+        if random_value < error_rate:
+            gate_name = "x"
+        return gate_name
+    
+    @staticmethod
+    def asymmetric_depolarization(error_rate: Union[list, tuple]):
+        if len(error_rate) != 3:
+            raise ValueError("Length of error must be 3")
+        gate_name = "I"
+        thredhold = sum(error_rate)
+        random_value = random.uniform(0, 1)
+        if random_value < thredhold:
+            if random_value < error_rate[0]:
+                gate_name = "x"
+            elif random_value < sum(error_rate[:2]):
+                gate_name = "y"
+            else:
+                gate_name = "z"
+        return gate_name
+    
+    @staticmethod
+    def depolarize(error_rate: float):
+        pxyz = [error_rate / 3] * 3
+        return QuantumCircuit.asymmetric_depolarization(error_rate=pxyz)
+
+    @staticmethod
+    def phase_flip(error_rate: float):
+        random_value = random.uniform(0, 1)
+        gate_name = "I"
+        if random_value < error_rate:
+            gate_name = "z"
+        return gate_name
+
     
     def random_circuit(self, num_qubits, num_gates: Union[int, list]):
         """
         生成随机线路
         :param num_qubits:
         :param num_gates: 门数量，列表表示单比特，多比特门数量
         :return:
@@ -360,14 +477,15 @@
         Args:
             measure_bits_list: 测量比特列表，传入比特位置或列表位置
             shots: 测量次数
         Returns:
             返回测量结果
         """
         # 首先通过执行操作得到所有的状态
+        # print(self.gate_list)
         self.run_statevector()
         state = np.array(self.state)
         prob = np.real(state.conjugate() * state)
         count = {format(i, f'0{self.width}b'): prob[i] for i in range(len(prob))}
         distribution = {}
 
         if isinstance(measure_bits_list, int):
```

### Comparing `tgqSim-0.1.1/tgqSim/draw_circuit_tools.py` & `tgqSim-0.1.2/tgqSim/draw_circuit_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.1/tgqSim/lib/tgq_simulator.so` & `tgqSim-0.1.2/tgqSim/lib/tgq_simulator.so`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.1/tgqSim.egg-info/PKG-INFO` & `tgqSim-0.1.2/tgqSim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.1
+Version: 0.1.2
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,cetc,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

