# Comparing `tmp/ntv_pandas-1.1.1.tar.gz` & `tmp/ntv_pandas-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntv_pandas-1.1.1.tar", last modified: Thu Jan  4 23:17:40 2024, max compression
+gzip compressed data, was "ntv_pandas-2.0.0.tar", last modified: Mon May  6 16:35:33 2024, max compression
```

## Comparing `ntv_pandas-1.1.1.tar` & `ntv_pandas-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-01-04 23:17:40.720063 ntv_pandas-1.1.1/
--rw-rw-rw-   0        0        0     6355 2024-01-04 23:17:40.719565 ntv_pandas-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5503 2024-01-04 14:31:48.000000 ntv_pandas-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-04 23:17:40.712097 ntv_pandas-1.1.1/ntv_pandas/
--rw-rw-rw-   0        0        0     1282 2023-12-29 22:43:11.000000 ntv_pandas-1.1.1/ntv_pandas/__init__.py
--rw-rw-rw-   0        0        0     2639 2024-01-04 22:10:19.000000 ntv_pandas-1.1.1/ntv_pandas/accessors.py
--rw-rw-rw-   0        0        0     4309 2023-09-18 21:58:13.000000 ntv_pandas-1.1.1/ntv_pandas/ntv_pandas.ini
--rw-rw-rw-   0        0        0     3521 2023-10-07 19:49:27.000000 ntv_pandas-1.1.1/ntv_pandas/ntv_table.ini
--rw-rw-rw-   0        0        0    28930 2024-01-04 22:13:27.000000 ntv_pandas-1.1.1/ntv_pandas/pandas_ntv_connector.py
-drwxrwxrwx   0        0        0        0 2024-01-04 23:17:40.717076 ntv_pandas-1.1.1/ntv_pandas.egg-info/
--rw-rw-rw-   0        0        0     6355 2024-01-04 23:17:40.000000 ntv_pandas-1.1.1/ntv_pandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2024-01-04 23:17:40.000000 ntv_pandas-1.1.1/ntv_pandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-04 23:17:40.000000 ntv_pandas-1.1.1/ntv_pandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-01-04 23:17:40.000000 ntv_pandas-1.1.1/ntv_pandas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-01-04 23:17:40.000000 ntv_pandas-1.1.1/ntv_pandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-01-04 23:17:40.720563 ntv_pandas-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1264 2024-01-04 23:13:35.000000 ntv_pandas-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-04 23:17:40.716579 ntv_pandas-1.1.1/tests/
--rw-rw-rw-   0        0        0     8321 2023-12-04 21:12:56.000000 ntv_pandas-1.1.1/tests/tests_ntv_pandas.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:35:33.581950 ntv_pandas-2.0.0/
+-rw-rw-rw-   0        0        0    11713 2024-05-06 16:35:33.581453 ntv_pandas-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10847 2024-05-06 12:53:21.000000 ntv_pandas-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 16:35:33.569502 ntv_pandas-2.0.0/ntv_pandas/
+-rw-rw-rw-   0        0        0     1273 2024-05-06 16:25:44.000000 ntv_pandas-2.0.0/ntv_pandas/__init__.py
+-rw-rw-rw-   0        0        0     4567 2024-05-06 16:24:28.000000 ntv_pandas-2.0.0/ntv_pandas/accessors.py
+-rw-rw-rw-   0        0        0     4309 2023-09-18 21:58:13.000000 ntv_pandas-2.0.0/ntv_pandas/ntv_pandas.ini
+-rw-rw-rw-   0        0        0     3521 2023-10-07 19:49:27.000000 ntv_pandas-2.0.0/ntv_pandas/ntv_table.ini
+-rw-rw-rw-   0        0        0    31621 2024-05-06 14:34:01.000000 ntv_pandas-2.0.0/ntv_pandas/pandas_ntv_connector.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:35:33.580457 ntv_pandas-2.0.0/ntv_pandas.egg-info/
+-rw-rw-rw-   0        0        0    11713 2024-05-06 16:35:33.000000 ntv_pandas-2.0.0/ntv_pandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2024-05-06 16:35:33.000000 ntv_pandas-2.0.0/ntv_pandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 16:35:33.000000 ntv_pandas-2.0.0/ntv_pandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-06 16:35:33.000000 ntv_pandas-2.0.0/ntv_pandas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-06 16:35:33.000000 ntv_pandas-2.0.0/ntv_pandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-06 16:35:33.582448 ntv_pandas-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1265 2024-05-06 14:10:16.000000 ntv_pandas-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:35:33.579461 ntv_pandas-2.0.0/tests/
+-rw-rw-rw-   0        0        0    10601 2024-05-06 09:49:35.000000 ntv_pandas-2.0.0/tests/tests_ntv_pandas.py
```

### Comparing `ntv_pandas-1.1.1/ntv_pandas/__init__.py` & `ntv_pandas-2.0.0/ntv_pandas/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,20 +18,17 @@
     - `ntv-pandas.ntv_pandas.pandas_ntv_connector.analysis`
     - `ntv-pandas.ntv_pandas.pandas_ntv_connector.as_def_type`
     - `ntv-pandas.ntv_pandas.pandas_ntv_connector.equals`
 
 - `ntv-pandas.ntv_pandas.accessors` :
     
     - `ntv-pandas.ntv_pandas.accessors.NpdSeriesAccessor`
-    - `ntv-pandas.ntv_pandas.accessors.NpdDataFrameAccessor`
-    
-    
+    - `ntv-pandas.ntv_pandas.accessors.NpdDataFrameAccessor`  
 """
-#from pathlib import Path
 from ntv_pandas.pandas_ntv_connector import DataFrameConnec, SeriesConnec, read_json
 from ntv_pandas.pandas_ntv_connector import to_json, as_def_type, equals, to_analysis
+from ntv_pandas.pandas_ntv_connector import from_xarray, from_scipp
 import ntv_pandas.accessors
-#import ntv_pandas.pandas_ntv_connector
 
 #path = Path(ntv_pandas.pandas_ntv_connector.__file__).parent
 
 #print('package :', __package__)
```

### Comparing `ntv_pandas-1.1.1/ntv_pandas/accessors.py` & `ntv_pandas-2.0.0/ntv_pandas/accessors.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 @author: philippe@loco-labs.io
 
 
 Accessor methods bound to pd.Series.npd, pd.DataFrame.npd
 """
 import pandas as pd
-from ntv_pandas.pandas_ntv_connector import to_json, as_def_type, equals, to_analysis, check_relation
 from tab_analysis import AnaDataset
+from ntv_numpy import Xdataset
+from ntv_pandas.pandas_ntv_connector import to_json, as_def_type, equals
+from ntv_pandas.pandas_ntv_connector import to_analysis, check_relation
 
 try:
     # delete the accessor to avoid warning
     del pd.DataFrame.npd
 except AttributeError:
     pass
 
@@ -21,39 +23,77 @@
 @pd.api.extensions.register_dataframe_accessor("npd")
 class NpdDataFrameAccessor:
     """Accessor class for methods invoked as `pd.DataFrame.npd.*`"""
 
     def __init__(self, pandas_obj):
         self._obj = pandas_obj
 
-    def analysis(self):
-        """Accessor for method `tab_analysis.AnaDataset` applied with 
+    def analysis(self, distr=False):
+        """Accessor for method `tab_analysis.AnaDataset` applied with
         `pandas_ntv_connector.to_analysis` invoked as `pd.DataFrame.npd.analysis`"""
-        return AnaDataset(to_analysis(self._obj))
+        return AnaDataset(to_analysis(self._obj, distr))
 
     def check_relation(self, parent, child, typecoupl, value=True):
-        ''' Accessor for method `pandas_ntv_connector.check_relation` invoket as 
+        ''' Accessor for method `pandas_ntv_connector.check_relation` invoket as
         `pd.DataFrame.npd.check_relation`'''
         return check_relation(self._obj, parent, child, typecoupl, value)
-    
+
     def to_json(self, **kwargs):
         """Accessor for method `pandas_ntv_connector.to_json` invoked as
-        `pd.DataFrame.npd.to_json`"""
+        `pd.DataFrame.npd.to_json`
+
+        *parameters*
+
+        - **pd_array** : Series or Dataframe to convert
+        - **encoded** : boolean (default: False) - if True return a JSON text else a JSON value
+        - **header** : boolean (default: True) - if True the JSON data is included as
+        value in a {key:value} object where key is ':field' for Series or ':tab' for DataFrame
+        - **table** : boolean (default False) - if True return TableSchema format
+        - **index** : boolean (default True) - if True the index Series is included"""
         return to_json(self._obj, **kwargs)
-    
+
     def as_def_type(self):
         """Accessor for method `pandas_ntv_connector.as_def_type` invoked as
         `pd.DataFrame.npd.as_def_type`"""
         return as_def_type(self._obj)
 
     def equals(self, other):
         """Accessor for method `pandas_ntv_connector.equals` invoked as
         `pd.DataFrame.npd.equals`"""
         return equals(self._obj, other)
 
+    def to_xarray(self, **kwargs):
+        """Accessor for method `Xdataset.from_dataframe.to_xarray` invoked as
+        `pd.DataFrame.npd.to_xarray`.
+
+        *Parameters*
+
+        - **dims**: list of string (default None) - order of dimensions to apply
+        - **dataset**: Boolean (default True) - if False and a single data_var,
+        return a sc.DataArray
+        - **datagroup**: Boolean (default True) - if True, return a sc.DataGroup
+        which contains the sc.DataArray/sc.Dataset and the other data else only
+        sc.DataArray/sc.Dataset"""
+        return Xdataset.from_dataframe(self._obj, **kwargs).to_xarray(**kwargs)
+
+    def to_scipp(self, **kwargs):
+        """Accessor for method `Xdataset.from_dataframe.to_scipp` invoked as
+        `pd.DataFrame.npd.to_scipp`.
+
+        *Parameters*
+
+        - **dims**: list of string (default None) - order of dimensions to apply
+        - **dataset**: Boolean (default True) - if False and a single data_var,
+        return a DataArray
+        - **datagroup**: Boolean (default True) - if True return a DataGroup with
+        metadata and data_arrays
+        - **ntv_type**: Boolean (default True) - if True add ntv-type to the name"""
+        return Xdataset.from_dataframe(self._obj, **kwargs).to_scipp(**kwargs)
+
+
 try:
     # delete the accessor to avoid warning
     del pd.Series.npd
 except AttributeError:
     pass
```

### Comparing `ntv_pandas-1.1.1/ntv_pandas/ntv_pandas.ini` & `ntv_pandas-2.0.0/ntv_pandas/ntv_pandas.ini`

 * *Files identical despite different names*

### Comparing `ntv_pandas-1.1.1/ntv_pandas/ntv_table.ini` & `ntv_pandas-2.0.0/ntv_pandas/ntv_table.ini`

 * *Files identical despite different names*

### Comparing `ntv_pandas-1.1.1/ntv_pandas/pandas_ntv_connector.py` & `ntv_pandas-2.0.0/ntv_pandas/pandas_ntv_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,51 +14,56 @@
 - to_obj_ntv: method - converter from JsonNTV to the object
 - to_json_ntv: method - converter from the object to JsonNTV
 
 It contains :
 
 - functions `read_json` and `to_json` to convert JSON data and pandas entities
 - function `to_analysis` to create data used by the `tab_analysis` module
-- function `check_relation` to identify rows with inconsistent relationships (`tab_dataset` function)
-- functions `as_def_type` and `equals` 
+- function `check_relation` to identify rows with inconsistent relationships
+- functions `as_def_type` and `equals`
 
 - the child classes of `NTV.json_ntv.ntv.NtvConnector` abstract class:
     - `DataFrameConnec`: 'tab'   connector
     - `SeriesConnec`:    'field' connector
 
 - an utility class with static methods : `PdUtil`
 
-The functions `to_json`, `to_analysis`, `check_relation`, `as_def_type` and 
+The functions `to_json`, `to_analysis`, `check_relation`, `as_def_type` and
 `equals` are used with the `npd` accessor.
 
 """
 import os
 import datetime
 import json
 import configparser
 from pathlib import Path
+from collections import Counter
+from io import StringIO
 import pandas as pd
 import numpy as np
 
 
 from json_ntv.ntv import Ntv, NtvConnector, NtvList, NtvSingle
 from json_ntv.ntv_util import NtvUtil
 from json_ntv.ntv_connector import ShapelyConnec
 from tab_dataset.cfield import Cfield
+from ntv_numpy import Xdataset
 
 path_ntv_pandas = Path(os.path.abspath(__file__)).parent
 
+
 def as_def_type(pd_array):
     '''convert a Series or DataFrame with default dtype'''
     if isinstance(pd_array, (pd.Series, pd.Index)):
         return pd_array.astype(SeriesConnec.deftype.get(pd_array.dtype.name, pd_array.dtype.name))
     return pd.DataFrame({col: as_def_type(pd_array[col]) for col in pd_array.columns})
 
+
 def check_relation(pd_df, parent, child, typecoupl, value=True):
-    ''' Accessor for method `cdataset.Cdataset.check_relation` invoket as 
+    ''' Accessor for method `cdataset.Cdataset.check_relation` invoket as
     `pd.DataFrame.npd.check_relation`.
     Get the inconsistent records for a relationship.
 
      *Parameters*
 
     - **child** : str - name of the child Series involved in the relation
     - **parent**: str - name of the parent Series involved in the relation
@@ -70,33 +75,25 @@
 
     - dict with inconsistent values of the Series
     - or a tuple with row of records'''
     parent_idx = SeriesConnec.to_idx(pd_df[parent])
     parent_field = Cfield(parent_idx['codec'], parent, parent_idx['keys'])
     child_idx = SeriesConnec.to_idx(pd_df[child])
     child_field = Cfield(child_idx['codec'], child, child_idx['keys'])
-    return  Cfield.check_relation(parent_field, child_field, typecoupl, value)
+    return Cfield.check_relation(parent_field, child_field, typecoupl, value)
+
 
-    
 def equals(pdself, pdother):
     '''return True if pd.equals is True and names are equal and dtype of categories are equal'''
-    equ = True
     if isinstance(pdself, pd.Series) and isinstance(pdother, pd.Series):
-        type_cat = str(pdself.dtype) == str(pdother.dtype) == 'category'
-        if type_cat:
-            equ &= equals(pdself.cat.categories, pdother.cat.categories)
-        else:
-            equ &= as_def_type(pdself).equals(as_def_type(pdother))
-        equ &= pdself.name == pdother.name
-        if not equ:
-            return False
-    elif isinstance(pdself, pd.DataFrame) and isinstance(pdother, pd.DataFrame):
-        for cself, cother in zip(pdself, pdother):
-            equ &= equals(pdself[cself], pdother[cother])
-    return equ
+        return SeriesConnec.equals(pdself, pdother)
+    if isinstance(pdself, pd.DataFrame) and isinstance(pdother, pd.DataFrame):
+        return DataFrameConnec.equals(pdself, pdother)
+    return False
+
 
 def read_json(jsn, **kwargs):
     ''' convert JSON text or JSON Value to pandas Series or Dataframe.
 
     *parameters*
 
     - **jsn** : JSON text or JSON value to convert
@@ -119,55 +116,105 @@
         return SeriesConnec.to_obj_ntv(ntv.ntv_value, **option)
     if ntv.type_str == 'tab':
         return DataFrameConnec.to_obj_ntv(ntv.ntv_value, **option)
     if option['series']:
         return SeriesConnec.to_obj_ntv(ntv, **option)
     return DataFrameConnec.to_obj_ntv(ntv.ntv_value, **option)
 
-def to_analysis(pd_df):
+
+def _dist(key1, key2, distr=False):
+    '''return default coupling codec between two keys list and optionaly if
+    the relationship is distributed'''
+    if not key1 or not key2:
+        return 0
+    k1k2 = [tuple((v1, v2)) for v1, v2 in zip(key1, key2)]
+    dist = len(list(dict.fromkeys(k1k2)))
+    if not distr:
+        return dist
+    distrib = False
+    if dist == (max(key1) + 1) * (max(key2) + 1):
+        distrib = max(Counter(k1k2).values()) == len(key1) // dist
+        # distrib = min(sum(map(lambda x: (x + i) % (max(a) + 1), a)) == sum(a)
+        # for i in range(1, max(a)+1))
+    return [dist, distrib]
+
+
+def to_analysis(pd_df, distr=False):
     '''return a dict with data used in AnaDataset module'''
 
-    keys = [list(pd_df[col].astype('category').cat.codes) for col in pd_df.columns]
-    lencodec = [ len(set(key)) for key in keys]
-    dist = [[len(set(zip(keys[i], keys[j])))
-                   for j in range(i+1, len(keys))]
-                  for i in range(len(keys)-1)]
+    keys = [list(pd_df[col].astype('category').cat.codes)
+            for col in pd_df.columns]
+    lencodec = [len(set(key)) for key in keys]
+    if distr:
+        dist = [[_dist(keys[i], keys[j], distr) for j in range(i+1, len(keys))]
+                for i in range(len(keys)-1)]
+    else:
+        dist = [[len(set(zip(keys[i], keys[j]))) for j in range(i+1, len(keys))]
+                for i in range(len(keys)-1)]
     return {'fields': [{'lencodec': lencodec[ind], 'id': pd_df.columns[ind],
                         'mincodec': lencodec[ind]}
                        for ind in range(len(pd_df.columns))],
-            'name': None, 'length': len(pd_df), 
+            'name': None, 'length': len(pd_df),
             'relations': {pd_df.columns[i]: {pd_df.columns[j+i+1]: dist[i][j]
                           for j in range(len(dist[i]))} for i in range(len(dist))}}
 
+
 def to_json(pd_array, **kwargs):
     ''' convert pandas Series or Dataframe to JSON text or JSON Value.
 
     *parameters*
 
     - **pd_array** : Series or Dataframe to convert
     - **encoded** : boolean (default: False) - if True return a JSON text else a JSON value
     - **header** : boolean (default: True) - if True the JSON data is included as
     value in a {key:value} object where key is ':field' for Series or ':tab' for DataFrame
     - **table** : boolean (default False) - if True return TableSchema format
+    - **index** : boolean (default True) - if True the index Series is included
     '''
-    option = {'encoded': False, 'header': True, 'table': False} | kwargs
+    option = {'encoded': False, 'header': True,
+              'table': False, 'index': True} | kwargs
     option['header'] = False if option['table'] else option['header']
     if isinstance(pd_array, pd.Series):
         jsn = SeriesConnec.to_json_ntv(pd_array, table=option['table'])[0]
         head = ':field'
     else:
-        jsn = DataFrameConnec.to_json_ntv(pd_array, table=option['table'])[0]
+        jsn = DataFrameConnec.to_json_ntv(pd_array, table=option['table'],
+                                          index=option['index'])[0]
         head = ':tab'
     if option['header']:
         jsn = {head: jsn}
     if option['encoded']:
         return json.dumps(jsn)
     return jsn
 
 
+def from_xarray(xdt, **kwargs):
+    ''' convert xarray.Dataset to pandas DataFrame.
+
+    *Parameters*
+
+    - **json_name**: Boolean (default True) - if False use full_name else json_name
+    - **info**: Boolean (default True) - if True add xdt.info in DataFrame.attrs
+    - **dims**: list of string (default None) - order of dimensions full_name to apply
+    '''
+    return Xdataset.from_xarray(xdt).to_dataframe(**kwargs)
+
+
+def from_scipp(sci, **kwargs):
+    ''' convert scipp.Dataset / scipp.DataArray / scipp.DataGroup to pandas DataFrame.
+
+    *Parameters*
+
+    - **json_name**: Boolean (default True) - if False use full_name else json_name
+    - **info**: Boolean (default True) - if True add xdt.info in DataFrame.attrs
+    - **dims**: list of string (default None) - order of dimensions full_name to apply
+    '''
+    return Xdataset.from_scipp(sci).to_dataframe(**kwargs)
+
+
 class DataFrameConnec(NtvConnector):
 
     '''NTV connector for pandas DataFrame.
 
     One static methods is included:
 
     - to_listidx: convert a DataFrame in categorical data
@@ -189,16 +236,15 @@
 
         ntv = Ntv.fast(ntv_value)
         lidx = [list(NtvUtil.decode_ntv_tab(ntvf, PdUtil.decode_ntv_to_val))
                 for ntvf in ntv]
         leng = max([idx[6] for idx in lidx])
         option = kwargs | {'leng': leng}
         no_keys = []
-        for ind in range(len(lidx)):
-            lind = lidx[ind]
+        for ind, lind in enumerate(lidx):
             no_keys.append(not lind[3] and not lind[4] and not lind[5])
             NtvConnector.init_ntv_keys(ind, lidx, leng)
             lind[2] = Ntv.fast(Ntv.obj_ntv(
                 lind[2], typ=lind[1], single=len(lind[2]) == 1))
         list_series = [series(lidx[ind][2], lidx[ind][0], None if no_keys[ind]
                               else lidx[ind][4], **option) for ind in range(len(lidx))]
         dfr = pd.DataFrame({ser.name: ser for ser in list_series})
@@ -209,19 +255,21 @@
         ''' convert a DataFrame (value, name, type) into NTV json (json-value, name, type).
 
         *Parameters*
 
         - **typ** : string (default None) - type of the NTV object,
         - **name** : string (default None) - name of the NTV object
         - **value** : DataFrame values
-        - **table** : boolean (default False) - if True return TableSchema format'''
-
+        - **table** : boolean (default False) - if True return TableSchema format
+        - **index** : boolean (default True) - if True the index Series is included
+        '''
         table = kwargs.get('table', False)
+        index = kwargs.get('index', True)
         if not table:
-            df2 = value.reset_index()
+            df2 = value.reset_index() if index else value
             jsn = Ntv.obj([SeriesConnec.to_json_ntv(PdUtil.unic(df2[col]))[0]
                            for col in df2.columns]).to_obj()
             return (jsn, name, DataFrameConnec.clas_typ if not typ else typ)
         df2 = pd.DataFrame({NtvUtil.from_obj_name(col)[0]: PdUtil.convert(
             SeriesConnec.to_json_ntv(value[col], table=True, no_val=True)[1],
             value[col]) for col in value.columns})
         table_val = json.loads(df2.to_json(orient='table',
@@ -239,34 +287,44 @@
 
         *Return: tuple with:*
 
         - **list** of dict (keys : 'codec', 'name, 'keys') for each column
         - **lenght** of the DataFrame'''
         return ([SeriesConnec.to_idx(ser) for name, ser in dtf.items()], len(dtf))
 
+    @staticmethod
+    def equals(pdself, pdother):
+        '''return True if columns are equals'''
+        if not (isinstance(pdself, pd.DataFrame) and isinstance(pdother, pd.DataFrame)):
+            return False
+        if len(pdself.columns) != len(pdother.columns):
+            return False
+        for cself, cother in zip(pdself, pdother):
+            if not SeriesConnec.equals(pdself[cself], pdother[cother]):
+                return False
+        return True
+
 
 class SeriesConnec(NtvConnector):
     '''NTV connector for pandas Series
 
     Two static methods are included:
 
     - to_idx: convert a Series in categorical data
     - to_series: return a Series from Field data
     '''
     clas_obj = 'Series'
     clas_typ = 'field'
     config = configparser.ConfigParser()
-    # config.read(Path(ntv_pandas.__file__).parent.joinpath('ntv_pandas.ini'))
     config.read(path_ntv_pandas.joinpath('ntv_pandas.ini'))
     types = pd.DataFrame(json.loads(config['data']['type']),
                          columns=json.loads(config['data']['column']))
     astype = json.loads(config['data']['astype'])
     deftype = {val: key for key, val in astype.items()}
     config = configparser.ConfigParser()
-    # config.read(Path(ntv_pandas.__file__).parent.joinpath('ntv_table.ini'))
     config.read(path_ntv_pandas.joinpath('ntv_table.ini'))
     table = pd.DataFrame(json.loads(config['data']['mapping']),
                          columns=json.loads(config['data']['column']))
     typtab = pd.DataFrame(json.loads(config['data']['type']),
                           columns=json.loads(config['data']['col_type']))
 
     @staticmethod
@@ -337,23 +395,24 @@
         if srs.dtype.name == 'category':
             cdc = pd.Series(srs.cat.categories)
             ntv_type = PdUtil.ntv_type(name_type, cdc.dtype.name)
             cat_value = PdUtil.ntv_val(ntv_type, cdc)
             cat_value = NtvList(cat_value, ntv_type=ntv_type)
             cod_value = list(srs.cat.codes)
             coef = NtvConnector.encode_coef(cod_value)
-            ntv_value = [cat_value, NtvList([coef]) if coef else NtvList(cod_value)]
+            ntv_value = [cat_value, NtvList(
+                [coef]) if coef else NtvList(cod_value)]
             ntv_type = None
         else:
             ntv_type = PdUtil.ntv_type(name_type, srs.dtype.name)
-            ntv_value = Ntv.from_obj(PdUtil.ntv_val(ntv_type, srs), 
+            ntv_value = Ntv.from_obj(PdUtil.ntv_val(ntv_type, srs),
                                      def_type=ntv_type).ntv_value
         if len(ntv_value) == 1:
-            ntv_value[0].set_name(ntv_name) 
-            return (ntv_value[0].to_obj(), name, 
+            ntv_value[0].set_name(ntv_name)
+            return (ntv_value[0].to_obj(), name,
                     SeriesConnec.clas_typ if not typ else typ)
         return (NtvList(ntv_value, ntv_name, ntv_type).to_obj(), name,
                 SeriesConnec.clas_typ if not typ else typ)
 
     @staticmethod
     def to_idx(ser):
         ''' convert a Series in categorical data
@@ -432,19 +491,32 @@
 
         - **data**: Json-value - data to convert in a Series
         - **dtype**: string - dtype of the Series
         - **ntv_type**: string - default type to apply to convert in dtype
         - **pd_name**: string - name of the Series including ntv_type
 
         NTVvalue and a ntv_type'''
-        srs = pd.read_json(json.dumps(data), dtype=dtype, typ='series')
+        srs = pd.read_json(StringIO(json.dumps(data)),
+                           dtype=dtype, typ='series')
         if not pd_name is None:
             srs = srs.rename(pd_name)
         return PdUtil.convert(ntv_type, srs, tojson=False)
 
+    @staticmethod
+    def equals(pdself, pdother):
+        '''return True if pd.equals is True and names are equal and dtype of categories are equal'''
+        if not (isinstance(pdself, pd.Series) and isinstance(pdother, pd.Series)):
+            return False
+        if pdself.name != pdother.name:
+            return False
+        type_cat = str(pdself.dtype) == str(pdother.dtype) == 'category'
+        if type_cat:
+            return SeriesConnec.equals(pdself.cat.categories, pdother.cat.categories)
+        return as_def_type(pdself).equals(as_def_type(pdother))
+
 
 class PdUtil:
     '''ntv-pandas utilities.
 
     This class includes static methods:
 
     Ntv and pandas
@@ -469,26 +541,26 @@
         ''' convert json TableSchema data into a DataFrame or a Series'''
         ntv_type = PdUtil.ntvtype_table(jsn['schema']['fields'])
         name = PdUtil.name_table(jsn['schema']['fields'])
         pd_name = [PdUtil.pd_name(nam, ntvtyp, table=True)[0]
                    for nam, ntvtyp in zip(name, ntv_type)]
         pd_dtype = [PdUtil.pd_name(nam, ntvtyp, table=True)[2]
                     for nam, ntvtyp in zip(name, ntv_type)]
-        dfr = pd.read_json(json.dumps(jsn['data']), orient='record')
+        dfr = pd.read_json(StringIO(json.dumps(jsn['data'])), orient='record')
         dfr = PdUtil.pd_index(dfr)
         dfr = pd.DataFrame({col: PdUtil.convert(ntv_type[ind], dfr[col], tojson=False)
                             for ind, col in enumerate(dfr.columns)})
         dfr = dfr.astype({col: pd_dtype[ind]
                          for ind, col in enumerate(dfr.columns)})
         dfr.columns = pd_name
         if len(dfr.columns) == 1:
             return dfr[dfr.columns[0]]
         return dfr
-    
-    @staticmethod 
+
+    @staticmethod
     def decode_ntv_to_val(ntv):
         ''' return a value from a ntv_field'''
         if isinstance(ntv, NtvSingle):
             return ntv.to_obj(simpleval=True)
         return [ntv_val.to_obj() for ntv_val in ntv]
 
     @staticmethod
@@ -559,15 +631,15 @@
         if ntv_type == 'geojson':
             return srs.apply(ShapelyConnec.from_geojson)
         if ntv_type == 'datetime':
             return pd.to_datetime(srs)
         if ntv_type == 'date':
             return pd.to_datetime(srs).dt.date
         if ntv_type == 'time':
-            return pd.to_datetime(srs).dt.time
+            return pd.to_datetime(srs, format='mixed').dt.time
         return srs
 
     @staticmethod
     def ntv_type(name_type, dtype, table=False):
         ''' return NTVtype from name_type and dtype of a Series .
 
         *Parameters*
@@ -589,15 +661,15 @@
     @staticmethod
     def ntv_val(ntv_type, srs):
         ''' convert a simple Series into NTV json-value.
 
         *Parameters*
 
         - **ntv_type** : string - NTVtype deduced from the Series name_type and dtype,
-        - **srs** : Series to be *converted.'''
+        - **srs** : Series to be converted.'''
         srs = PdUtil.convert(ntv_type, srs)
         if ntv_type in ['point', 'line', 'polygon', 'geometry', 'geojson']:
             return srs.to_list()
         if srs.dtype.name == 'object':
             return srs.to_list()
         return json.loads(srs.to_json(orient='records',
                                       date_format='iso', default_handler=str))
```

### Comparing `ntv_pandas-1.1.1/setup.py` & `ntv_pandas-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ntv_pandas",
-    version="1.1.1",
-    description="NTV-pandas : A tabular analyzer and a semantic, compact and reversible JSON-pandas converter",
+    version="2.0.0",
+    description="NTV-pandas : A tabular analyzer and a semantic, compact and reversible converter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/loco-philippe/ntv-pandas/blob/main/README.md",
     author="Philippe Thomy",
     author_email="philippe@loco-labs.io",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
@@ -24,9 +24,9 @@
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3"],
     keywords="pandas, JSON-NTV, semantic JSON, development, environmental data",
     packages=find_packages(include=['ntv_pandas', 'ntv_pandas.*']),
     package_data={'ntv_pandas': ['*.ini']},
     python_requires=">=3.9, <4",
-    install_requires=['tab_analysis', 'tab_dataset', 'json_ntv', 'numpy', 'pandas', 'shapely']
+    install_requires=['ntv_numpy', 'tab_analysis', 'tab_dataset', 'json_ntv', 'numpy', 'pandas', 'shapely']
 )
```

