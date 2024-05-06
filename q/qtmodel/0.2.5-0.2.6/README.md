# Comparing `tmp/qtmodel-0.2.5.tar.gz` & `tmp/qtmodel-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmodel-0.2.5.tar", last modified: Thu Apr 18 09:01:21 2024, max compression
+gzip compressed data, was "qtmodel-0.2.6.tar", last modified: Mon May  6 04:02:18 2024, max compression
```

## Comparing `qtmodel-0.2.5.tar` & `qtmodel-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 09:01:21.043774 qtmodel-0.2.5/
--rw-rw-rw-   0        0        0    37853 2024-04-18 09:01:21.043774 qtmodel-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    37436 2024-04-18 08:58:14.000000 qtmodel-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 09:01:21.036265 qtmodel-0.2.5/qtmodel/
--rw-rw-rw-   0        0        0       93 2024-04-10 06:50:13.000000 qtmodel-0.2.5/qtmodel/__init__.py
--rw-rw-rw-   0        0        0    80726 2024-04-18 08:55:14.000000 qtmodel-0.2.5/qtmodel/qt_mdb.py
--rw-rw-rw-   0        0        0     3834 2024-04-10 06:52:58.000000 qtmodel-0.2.5/qtmodel/qt_odb.py
--rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.2.5/qtmodel/res_db.py
-drwxrwxrwx   0        0        0        0 2024-04-18 09:01:21.041775 qtmodel-0.2.5/qtmodel.egg-info/
--rw-rw-rw-   0        0        0    37853 2024-04-18 09:01:20.000000 qtmodel-0.2.5/qtmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-04-18 09:01:20.000000 qtmodel-0.2.5/qtmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 09:01:20.000000 qtmodel-0.2.5/qtmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 09:01:20.000000 qtmodel-0.2.5/qtmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 09:01:21.043774 qtmodel-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      747 2024-04-18 09:01:15.000000 qtmodel-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:02:18.206322 qtmodel-0.2.6/
+-rw-rw-rw-   0        0        0    37701 2024-05-06 04:02:18.205322 qtmodel-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    37273 2024-04-25 08:56:24.000000 qtmodel-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 04:02:18.198314 qtmodel-0.2.6/qtmodel/
+-rw-rw-rw-   0        0        0       93 2024-04-10 06:50:13.000000 qtmodel-0.2.6/qtmodel/__init__.py
+-rw-rw-rw-   0        0        0    80502 2024-05-06 03:52:43.000000 qtmodel-0.2.6/qtmodel/qt_mdb.py
+-rw-rw-rw-   0        0        0     3834 2024-04-10 06:52:58.000000 qtmodel-0.2.6/qtmodel/qt_odb.py
+-rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.2.6/qtmodel/res_db.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:02:18.204324 qtmodel-0.2.6/qtmodel.egg-info/
+-rw-rw-rw-   0        0        0    37701 2024-05-06 04:02:17.000000 qtmodel-0.2.6/qtmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-05-06 04:02:18.000000 qtmodel-0.2.6/qtmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 04:02:17.000000 qtmodel-0.2.6/qtmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 04:02:17.000000 qtmodel-0.2.6/qtmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 04:02:18.206322 qtmodel-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      758 2024-05-06 04:01:47.000000 qtmodel-0.2.6/setup.py
```

### Comparing `qtmodel-0.2.5/PKG-INFO` & `qtmodel-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.2.5
-Summary: python modeling for qt
+Version: 0.2.6
+Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -780,27 +780,25 @@
 ```  
 ### add_beam_load
 添加梁单元荷载
 > 参数:  
 > beam_id:单元编号  
 > case_name:荷载工况名  
 > load_type:荷载类型  
-> _ 1-集中荷载 2-集中弯矩 3-均布荷载 4-均布弯矩 5-梯形荷载 6-梯形弯矩_  
+> _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩  
 > coord_system:坐标系  
 > _1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z_  
 > list_x:荷载位置信息 ,荷载距离单元I端的相对距离  
 > list_load:荷载数值信息  
-> uniform_load:均布荷载值  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
-mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0,1],uniform_load=100)
-mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=5,list_x=[0.4,0.8],list_load=[100,200])
+mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0.4,0.8],list_load=[100,200])
 ```  
 ### remove_beam_load
 删除梁单元荷载
 > 参数:  
 > element_id:单元号  
 > case_name:荷载工况名  
 > load_type:荷载类型
```

### Comparing `qtmodel-0.2.5/README.md` & `qtmodel-0.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -766,27 +766,25 @@
 ```  
 ### add_beam_load
 添加梁单元荷载
 > 参数:  
 > beam_id:单元编号  
 > case_name:荷载工况名  
 > load_type:荷载类型  
-> _ 1-集中荷载 2-集中弯矩 3-均布荷载 4-均布弯矩 5-梯形荷载 6-梯形弯矩_  
+> _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩  
 > coord_system:坐标系  
 > _1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z_  
 > list_x:荷载位置信息 ,荷载距离单元I端的相对距离  
 > list_load:荷载数值信息  
-> uniform_load:均布荷载值  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
-mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0,1],uniform_load=100)
-mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=5,list_x=[0.4,0.8],list_load=[100,200])
+mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0.4,0.8],list_load=[100,200])
 ```  
 ### remove_beam_load
 删除梁单元荷载
 > 参数:  
 > element_id:单元号  
 > case_name:荷载工况名  
 > load_type:荷载类型
```

### Comparing `qtmodel-0.2.5/qtmodel/qt_mdb.py` & `qtmodel-0.2.6/qtmodel/qt_mdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -945,15 +945,15 @@
             qt_model.RemoveTendonGroup(name=name)
         elif index != -1:
             qt_model.RemoveTendonGroup(id=index)
         else:
             qt_model.RemoveAllStructureGroup()
 
     @staticmethod
-    def add_tendon_property(name: str = "", index: int = -1, tendon_type: str = "先张", material_id: int = 1, duct_type: int = 1,
+    def add_tendon_property(name: str = "", index: int = -1, tendon_type: int = 0, material_id: int = 1, duct_type: int = 1,
                             steel_type: int = 1, steel_detail: list[float] = None, loos_detail: tuple[int, int, int] = None,
                             slip_info: tuple[int, int] = None):
         """
         添加钢束特性
         Args:
              name:钢束特性名
              index:钢束编号,默认自动识别 (可选参数)
@@ -966,15 +966,15 @@
                 _螺纹钢筋[钢筋直径,钢束面积,孔道直径,摩阻系数,偏差系数,张拉方式(1-一次张拉 2-超张拉)]_
              loos_detail: 松弛信息[规范,张拉,松弛] (仅钢绞线需要,默认为[1,1,1])
                 _规范:1-公规 2-铁规_
                 _张拉方式:1-一次张拉 2-超张拉_
                 _松弛类型：1-一般松弛 2-低松弛_
              slip_info: 滑移信息[始端距离,末端距离] 默认为[0.006, 0.006]
         example:
-            mdb.add_tendon_property(name="钢束1",tendon_type="先张",material_id=1,duct_type=1,steel_type=1,
+            mdb.add_tendon_property(name="钢束1",tendon_type=0,material_id=1,duct_type=1,steel_type=1,
                                     steel_detail=[0.00014,0.10,0.25,0.0015],loos_detail=(1,1,1))
         Returns: 无
         """
         if steel_detail is None:
             raise Exception("操作错误，钢束特性信息不能为空")
         if loos_detail is None:
             loos_detail = (1, 1, 1)
@@ -985,15 +985,15 @@
                                    loosDetail=loos_detail, slipInfo=slip_info)
 
     @staticmethod
     def add_tendon_3d(name: str, property_name: str = "", group_name: str = "默认钢束组",
                       num: int = 1, line_type: int = 1, position_type=1,
                       control_points: list[tuple[float, float, float, float]] = None,
                       point_insert: tuple[float, float, float] = None,
-                      tendon_direction: tuple[float, float, float, float] = None,
+                      tendon_direction: tuple[float, float, float] = None,
                       rotation_angle: float = 0, track_group: str = "默认结构组", projection: bool = True):
         """
         添加三维钢束
         Args:
              name:钢束名称
              property_name:钢束特性名称
              group_name:默认钢束组
@@ -1218,37 +1218,35 @@
         example:
             mdb.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
         Returns: 无
         """
         qt_model.RemoveNodalDisplacement(caseName=case_name, nodeId=-node_id)
 
     @staticmethod
-    def add_beam_load(beam_id: int = 1, case_name: str = "", load_type: int = 1, coord_system: int = 3, list_x: list[float] = None,
-                      list_load: list[float] = None, uniform_load: float = 0, group_name="默认荷载组"):
+    def add_beam_load(beam_id: int = 1, case_name: str = "", load_type: int = 1, coord_system: int = 3, list_x: list[tuple[float,float]] = None,
+                      list_load: list[tuple[float,float]] = None, group_name="默认荷载组"):
         """
         添加梁单元荷载
         Args:
             beam_id:单元编号
             case_name:荷载工况名
             load_type:荷载类型
-               _ 1-集中荷载 2-集中弯矩 3-均布荷载 4-均布弯矩 5-梯形荷载 6-梯形弯矩_
+               _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩
             coord_system:坐标系
                 _1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z_
             list_x:荷载位置信息 ,荷载距离单元I端的相对距离
             list_load:荷载数值信息
-            uniform_load:均布荷载值
             group_name:荷载组名
         example:
             mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
-            mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0,1],uniform_load=100)
-            mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=5,list_x=[0.4,0.8],list_load=[100,200])
+            mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0.4,0.8],list_load=[100,200])
         Returns: 无
         """
         qt_model.AddBeamLoad(caseName=case_name, beamId=beam_id, loadType=load_type,
-                             coordinateSystem=coord_system, listX=list_x, listLoad=list_load, uniform=uniform_load, groupName=group_name)
+                             coordinateSystem=coord_system, listX=list_x, listLoad=list_load,  groupName=group_name)
 
     @staticmethod
     def remove_beam_load(element_id: int = 1, case_name: str = "", load_type: int = 1, group_name: str = "默认荷载组"):
         """
         删除梁单元荷载
         Args:
             element_id:单元号
```

### Comparing `qtmodel-0.2.5/qtmodel/qt_odb.py` & `qtmodel-0.2.6/qtmodel/qt_odb.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.2.5/qtmodel/res_db.py` & `qtmodel-0.2.6/qtmodel/res_db.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.2.5/qtmodel.egg-info/PKG-INFO` & `qtmodel-0.2.6/qtmodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.2.5
-Summary: python modeling for qt
+Version: 0.2.6
+Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -780,27 +780,25 @@
 ```  
 ### add_beam_load
 添加梁单元荷载
 > 参数:  
 > beam_id:单元编号  
 > case_name:荷载工况名  
 > load_type:荷载类型  
-> _ 1-集中荷载 2-集中弯矩 3-均布荷载 4-均布弯矩 5-梯形荷载 6-梯形弯矩_  
+> _ 1-集中荷载 2-集中弯矩 3-分布弯矩 4-分布弯矩  
 > coord_system:坐标系  
 > _1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z_  
 > list_x:荷载位置信息 ,荷载距离单元I端的相对距离  
 > list_load:荷载数值信息  
-> uniform_load:均布荷载值  
 > group_name:荷载组名  
 ```Python
 # 示例代码
 from qtmodel import mdb
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
-mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0,1],uniform_load=100)
-mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=5,list_x=[0.4,0.8],list_load=[100,200])
+mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0.4,0.8],list_load=[100,200])
 ```  
 ### remove_beam_load
 删除梁单元荷载
 > 参数:  
 > element_id:单元号  
 > case_name:荷载工况名  
 > load_type:荷载类型
```

### Comparing `qtmodel-0.2.5/setup.py` & `qtmodel-0.2.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 # 读取文件内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="qtmodel",
-    version="0.2.5",
+    version="0.2.6",
     author="dqy-zhj",
     author_email="1105417715@qq.com",
-    description="python modeling for qt",
+    description="python modeling for qt  24/05/06 ",
     long_description=long_description,  # 使用读取的 README.md 文件内容
     long_description_content_type="text/markdown",  # 指明内容格式为markdown
     url="https://github.com/Inface0443/pyqt",
     packages=find_packages(),
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

