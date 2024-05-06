# Comparing `tmp/pyetp-0.0.6.tar.gz` & `tmp/pyetp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyetp-0.0.6.tar", max compression
+gzip compressed data, was "pyetp-0.0.7.tar", max compression
```

## Comparing `pyetp-0.0.6.tar` & `pyetp-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7652 2024-04-17 12:30:43.057485 pyetp-0.0.6/LICENSE.md
--rw-r--r--   0        0        0     1224 2024-04-17 12:30:43.057485 pyetp-0.0.6/README.md
--rw-r--r--   0        0        0      123 2024-04-17 12:30:43.165487 pyetp-0.0.6/pyetp/__init__.py
--rw-r--r--   0        0        0    33452 2024-04-17 12:30:43.165487 pyetp-0.0.6/pyetp/client.py
--rw-r--r--   0        0        0      879 2024-04-17 12:30:43.165487 pyetp-0.0.6/pyetp/config.py
--rw-r--r--   0        0        0    50492 2024-04-17 12:30:43.165487 pyetp-0.0.6/pyetp/resqml_objects/__init__.py
--rw-r--r--   0        0        0   783914 2024-04-17 12:30:43.169487 pyetp-0.0.6/pyetp/resqml_objects/generated.py
--rw-r--r--   0        0        0     2487 2024-04-17 12:30:43.169487 pyetp-0.0.6/pyetp/types.py
--rw-r--r--   0        0        0     2675 2024-04-17 12:30:43.169487 pyetp-0.0.6/pyetp/uri.py
--rw-r--r--   0        0        0     2248 2024-04-17 12:30:43.169487 pyetp-0.0.6/pyetp/utils_arrays.py
--rw-r--r--   0        0        0    24548 2024-04-17 12:30:43.169487 pyetp-0.0.6/pyetp/utils_xml.py
--rw-r--r--   0        0        0      877 2024-04-17 12:31:13.733986 pyetp-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pyetp-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-06 07:15:13.244960 pyetp-0.0.7/LICENSE.md
+-rw-r--r--   0        0        0     1224 2024-05-06 07:15:13.244960 pyetp-0.0.7/README.md
+-rw-r--r--   0        0        0      123 2024-05-06 07:15:13.308960 pyetp-0.0.7/pyetp/__init__.py
+-rw-r--r--   0        0        0    37477 2024-05-06 07:15:13.308960 pyetp-0.0.7/pyetp/client.py
+-rw-r--r--   0        0        0      879 2024-05-06 07:15:13.308960 pyetp-0.0.7/pyetp/config.py
+-rw-r--r--   0        0        0    50492 2024-05-06 07:15:13.308960 pyetp-0.0.7/pyetp/resqml_objects/__init__.py
+-rw-r--r--   0        0        0   783914 2024-05-06 07:15:13.312960 pyetp-0.0.7/pyetp/resqml_objects/generated.py
+-rw-r--r--   0        0        0     2487 2024-05-06 07:15:13.312960 pyetp-0.0.7/pyetp/types.py
+-rw-r--r--   0        0        0     2675 2024-05-06 07:15:13.312960 pyetp-0.0.7/pyetp/uri.py
+-rw-r--r--   0        0        0     2248 2024-05-06 07:15:13.312960 pyetp-0.0.7/pyetp/utils_arrays.py
+-rw-r--r--   0        0        0    24548 2024-05-06 07:15:13.312960 pyetp-0.0.7/pyetp/utils_xml.py
+-rw-r--r--   0        0        0      962 2024-05-06 07:15:41.452879 pyetp-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2286 1970-01-01 00:00:00.000000 pyetp-0.0.7/PKG-INFO
```

### Comparing `pyetp-0.0.6/README.md` & `pyetp-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.6/pyetp/client.py` & `pyetp-0.0.7/pyetp/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 import numpy as np
 from pydantic import SecretStr
 import websockets
 from etpproto.connection import (CommunicationProtocol, ConnectionType,
                                  ETPConnection)
 from etpproto.messages import Message, MessageFlags
 from xtgeo import RegularSurface
+import xtgeo
 
 import pyetp.resqml_objects as ro
 from pyetp.config import SETTINGS
+from pyetp.resqml_objects.generated import Grid2dPatch
 
 from . import utils_arrays, utils_xml
 from .types import *
 from .uri import DataObjectURI, DataspaceURI
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
@@ -354,15 +356,89 @@
         assert isinstance(response, DeleteDataObjectsResponse), "Expected DeleteDataObjectsResponse"
 
         return response.deleted_uris
 
     #
     # xtgeo
     #
-
+    @staticmethod
+    def check_inside(x:float,y:float,patch:Grid2dPatch):
+        xori= patch.geometry.points.supporting_geometry.origin.coordinate1
+        yori = patch.geometry.points.supporting_geometry.origin.coordinate2 
+        xmax = xori + (patch.geometry.points.supporting_geometry.offset[0].spacing.value*patch.geometry.points.supporting_geometry.offset[0].spacing.count)
+        ymax = yori + (patch.geometry.points.supporting_geometry.offset[1].spacing.value*patch.geometry.points.supporting_geometry.offset[1].spacing.count)
+        if x < xori:
+            return False
+        if y < yori:
+            return False
+        if x > xmax:
+            return False
+        if y > ymax:
+            return False  
+        return True
+    
+    @staticmethod
+    def find_closest_index(x,y,patch:Grid2dPatch):
+        x_ind = (x-patch.geometry.points.supporting_geometry.origin.coordinate1)/patch.geometry.points.supporting_geometry.offset[0].spacing.value
+        y_ind = (y-patch.geometry.points.supporting_geometry.origin.coordinate2)/patch.geometry.points.supporting_geometry.offset[1].spacing.value
+        return round(x_ind),round(y_ind)
+    
+    async def get_surface_value_x_y(self, epc_uri: T.Union[DataObjectURI , str] ,gri_uri: T.Union[DataObjectURI , str], x: T.Union[int,float], y: T.Union[int,float], method:T.Literal["bilinear","nearest"]):
+        gri, = await self.get_resqml_objects(gri_uri) # parallelized using subarray
+        xori= gri.grid2d_patch.geometry.points.supporting_geometry.origin.coordinate1
+        yori = gri.grid2d_patch.geometry.points.supporting_geometry.origin.coordinate2 
+        xinc = gri.grid2d_patch.geometry.points.supporting_geometry.offset[0].spacing.value
+        yinc = gri.grid2d_patch.geometry.points.supporting_geometry.offset[1].spacing.value
+        max_x_index_in_gri = gri.grid2d_patch.geometry.points.supporting_geometry.offset[0].spacing.count
+        max_y_index_in_gri = gri.grid2d_patch.geometry.points.supporting_geometry.offset[1].spacing.count
+        buffer = 4
+        if not self.check_inside(x,y,gri.grid2d_patch):
+            logger.info(f"Points not inside {x}:{y} {gri}")
+            return
+        uid=DataArrayIdentifier(
+                    uri=str(epc_uri), pathInResource=gri.grid2d_patch.geometry.points.zvalues.values.path_in_hdf_file
+                )
+        if max_x_index_in_gri <= 10 or max_y_index_in_gri <= 10:
+            surf = await self.get_xtgeo_surface(epc_uri,gri_uri)
+            return surf.get_value_from_xy((x,y),sampling=method)
+        
+        x_ind,y_ind=self.find_closest_index(x,y,gri.grid2d_patch)
+        if method == "nearest":
+            arr = await self.get_subarray(uid,[x_ind,y_ind],[1,1])
+            return arr[0][0]
+        min_x_ind = max(x_ind-(buffer/2),0)
+        min_y_ind = max(y_ind-(buffer/2),0)
+        count_x = min(max_x_index_in_gri-min_x_ind,buffer)
+        count_y = min(max_y_index_in_gri-min_y_ind,buffer)
+        ## shift start index to left if not enough buffer on right
+        if count_x < buffer:
+            x_index_to_add = 3- count_x
+            min_x_ind_new = max(0,min_x_ind-x_index_to_add)
+            count_x=count_x + min_x_ind-min_x_ind_new+1
+            min_x_ind = min_x_ind_new
+        if count_y < buffer:
+            y_index_to_add = 3- count_y
+            min_y_ind_new = max(0,min_y_ind-y_index_to_add)
+            count_y=count_y + min_y_ind-min_y_ind_new+1
+            min_y_ind = min_y_ind_new
+        arr = await self.get_subarray(uid,[min_x_ind,min_y_ind],[count_x,count_y])
+        new_x_ori = xori+(min_x_ind*xinc)
+        new_y_ori = yori+(min_y_ind*yinc) 
+        regridded = xtgeo.RegularSurface(
+            ncol=arr.shape[0],
+            nrow=arr.shape[1],
+            xori=new_x_ori,
+            yori=new_y_ori,
+            xinc=xinc,
+            yinc=yinc,
+            rotation=0.0,
+            values=arr.flatten(),
+        )
+        return regridded.get_value_from_xy((x,y))
+    
     async def get_xtgeo_surface(self, epc_uri: T.Union[DataObjectURI , str] ,gri_uri: T.Union[DataObjectURI , str]):
         gri, = await self.get_resqml_objects(gri_uri)
 
         # some checks
         
         assert isinstance(gri, ro.Grid2dRepresentation), "obj must be Grid2dRepresentation"
         sgeo = gri.grid2d_patch.geometry.points.supporting_geometry  # type: ignore
@@ -390,15 +466,14 @@
 
     async def put_xtgeo_surface(self, surface: RegularSurface, epsg_code=23031, dataspace: T.Union[DataspaceURI , str , None] = None):
         """Returns (epc_uri, crs_uri, gri_uri)"""
         assert surface.values is not None, "cannot upload empty surface"
 
         epc, crs, gri = utils_xml.parse_xtgeo_surface_to_resqml_grid(surface, epsg_code)
         epc_uri, crs_uri, gri_uri = await self.put_resqml_objects(epc, crs, gri, dataspace=dataspace)
-
         response = await self.put_array(
             DataArrayIdentifier(
                 uri=epc_uri.raw_uri if isinstance(epc_uri, DataObjectURI) else epc_uri,
                 pathInResource=gri.grid2d_patch.geometry.points.zvalues.values.path_in_hdf_file  # type: ignore
             ),
             surface.values.filled(np.nan).astype(np.float32)
         )
```

### Comparing `pyetp-0.0.6/pyetp/config.py` & `pyetp-0.0.7/pyetp/config.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.6/pyetp/resqml_objects/__init__.py` & `pyetp-0.0.7/pyetp/resqml_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.6/pyetp/resqml_objects/generated.py` & `pyetp-0.0.7/pyetp/resqml_objects/generated.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.6/pyetp/types.py` & `pyetp-0.0.7/pyetp/types.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.6/pyetp/uri.py` & `pyetp-0.0.7/pyetp/uri.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.6/pyetp/utils_arrays.py` & `pyetp-0.0.7/pyetp/utils_arrays.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.6/pyetp/utils_xml.py` & `pyetp-0.0.7/pyetp/utils_xml.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.6/pyproject.toml` & `pyetp-0.0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [tool.poetry]
 name = "pyetp"
-version = "0.0.6"
+version = "0.0.7"
 description = "Interface with OSDU RDDMS using ETP protocol"
 authors = ["Adam Cheng <52572642+adamchengtkc@users.noreply.github.com>"]
 readme = "README.md"
-license = "LGPL-3.0-only"
 homepage = "https://github.com/equinor/pyetp"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 numpy = "^1.26.3"
 websockets = "^12.0"
 lxml = "^4.9.4"
@@ -16,21 +15,26 @@
 redis = "^5.0.1"
 async-lru = "^2.0.4"
 pyarrow = "^15.0.0"  # added to fix pandas deprecated warning in xtgeo
 etpproto = "^1.0.5"
 httpx = "^0.26.0"
 xtgeo = "^3.8.0"
 xsdata = "^24.3.1"
-resqpy = "^4.14.3"
+resqpy = "^4.14.4"
 async-timeout = "^4.0.3"
 pillow = "^10.3.0"
 
 [tool.poetry.group.dev.dependencies]
 notebook = "^7.0.7"
 pytest = "^7.4.4"
 pytest-asyncio = "^0.23.4"
 fakeredis = "^2.21.0"
 pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
+
+classifiers = [
+  "Development Status :: 3 - Alpha",
+  "License :: OSI Approved :: Apache Software License"
+]
```

### Comparing `pyetp-0.0.6/PKG-INFO` & `pyetp-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: pyetp
-Version: 0.0.6
+Version: 0.0.7
 Summary: Interface with OSDU RDDMS using ETP protocol
 Home-page: https://github.com/equinor/pyetp
-License: LGPL-3.0-only
 Author: Adam Cheng
 Author-email: 52572642+adamchengtkc@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: async-lru (>=2.0.4,<3.0.0)
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0)
 Requires-Dist: etpproto (>=1.0.5,<2.0.0)
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: lxml (>=4.9.4,<5.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: redis (>=5.0.1,<6.0.0)
-Requires-Dist: resqpy (>=4.14.3,<5.0.0)
+Requires-Dist: resqpy (>=4.14.4,<5.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Requires-Dist: xsdata (>=24.3.1,<25.0.0)
 Requires-Dist: xtgeo (>=3.8.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 ![Build Status](https://github.com/equinor/pyetp/actions/workflows/ci.yml/badge.svg?branch=main)
 ![Build Status](https://github.com/equinor/pyetp/actions/workflows/snyk.yml/badge.svg?branch=main)
```

