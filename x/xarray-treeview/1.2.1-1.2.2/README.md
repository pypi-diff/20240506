# Comparing `tmp/xarray_treeview-1.2.1.tar.gz` & `tmp/xarray_treeview-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_treeview-1.2.1.tar", last modified: Tue Apr 30 22:56:15 2024, max compression
+gzip compressed data, was "xarray_treeview-1.2.2.tar", last modified: Mon May  6 21:12:49 2024, max compression
```

## Comparing `xarray_treeview-1.2.1.tar` & `xarray_treeview-1.2.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1077 2024-01-11 16:04:45.274505 xarray_treeview-1.2.1/LICENSE
--rw-r--r--   0        0        0      210 2024-01-29 19:36:00.736104 xarray_treeview-1.2.1/README.md
--rw-r--r--   0        0        0     1261 2024-04-30 22:56:15.940983 xarray_treeview-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     7671 2024-04-24 22:17:08.019833 xarray_treeview-1.2.1/src/xarray_treeview/XarrayTreeItem.py
--rw-r--r--   0        0        0     5999 2024-03-08 22:47:30.993487 xarray_treeview-1.2.1/src/xarray_treeview/XarrayTreeModel.py
--rw-r--r--   0        0        0    10664 2024-04-26 15:47:20.923676 xarray_treeview-1.2.1/src/xarray_treeview/XarrayTreeView.py
--rw-r--r--   0        0        0      195 2024-02-08 22:49:32.523681 xarray_treeview-1.2.1/src/xarray_treeview/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 16:04:45.276303 xarray_treeview-1.2.1/tests/__init__.py
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 xarray_treeview-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-11 16:04:45.274505 xarray_treeview-1.2.2/LICENSE
+-rw-r--r--   0        0        0      210 2024-01-29 19:36:00.736104 xarray_treeview-1.2.2/README.md
+-rw-r--r--   0        0        0     1261 2024-05-06 21:12:49.447039 xarray_treeview-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7781 2024-05-02 17:20:29.148732 xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeItem.py
+-rw-r--r--   0        0        0     5999 2024-05-02 18:10:19.300488 xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeModel.py
+-rw-r--r--   0        0        0    10751 2024-05-02 18:19:08.766975 xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeView.py
+-rw-r--r--   0        0        0     3977 2024-05-02 18:19:50.460886 xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeViewer.py
+-rw-r--r--   0        0        0      257 2024-05-02 18:13:58.486880 xarray_treeview-1.2.2/src/xarray_treeview/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 16:04:45.276303 xarray_treeview-1.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 xarray_treeview-1.2.2/PKG-INFO
```

### Comparing `xarray_treeview-1.2.1/LICENSE` & `xarray_treeview-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray_treeview-1.2.1/pyproject.toml` & `xarray_treeview-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-version = "1.2.1"
+version = "1.2.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/marcel-goldschen-ohm/xarray-treeview"
 repository = "https://github.com/marcel-goldschen-ohm/xarray-treeview"
```

### Comparing `xarray_treeview-1.2.1/src/xarray_treeview/XarrayTreeItem.py` & `xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeItem.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,22 +146,24 @@
                 return '(' + ', '.join([f'{dim}: {size}' for dim, size in sizes.items()]) + ')'
             if self.is_var():
                 rep = str(self.node.ds)
                 i = rep.find('Data variables:')
                 i = rep.find(self.key, i)  # find var
                 i = rep.find(') ', i) + 2  # skip dimensions
                 i = rep.find(' ', i) + 1  # skip dtype
+                i = rep.find(' ', i) + 1  # skip bytes
                 j = rep.find('\n', i)
                 return rep[i:j] if j > 0 else rep[i:]
             if self.is_coord():
                 rep = str(self.node.ds)
                 i = rep.find('Coordinates:')
                 i = rep.find(self.key, i)  # find coord
                 i = rep.find(') ', i) + 2  # skip dimensions
                 i = rep.find(' ', i) + 1  # skip dtype
+                i = rep.find(' ', i) + 1  # skip bytes
                 j = rep.find('\n', i)
                 return rep[i:j] if j > 0 else rep[i:]
     
     def set_data(self, column: int, value) -> bool:
         if column == 0:
             try:
                 if value == self.name:
```

### Comparing `xarray_treeview-1.2.1/src/xarray_treeview/XarrayTreeModel.py` & `xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeModel.py`

 * *Files identical despite different names*

### Comparing `xarray_treeview-1.2.1/src/xarray_treeview/XarrayTreeView.py` & `xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeView.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from datatree import DataTree
 from pyqt_ext.tree import TreeView, KeyValueTreeItem, KeyValueTreeModel, KeyValueTreeView
 from xarray_treeview import XarrayTreeItem, XarrayTreeModel
 
 
 class XarrayTreeView(TreeView):
 
+    finishedEditingAttrs = Signal()
+
     def __init__(self, parent: QObject = None) -> None:
         TreeView.__init__(self, parent)
 
         self.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectRows)
 
         self._showVarsAction = QAction('Show Vars')
         self._showVarsAction.setCheckable(True)
@@ -144,14 +146,16 @@
             return
         
         attrs = model.root().value
         if item.is_node():
             item.node.attrs = attrs
         elif item.is_var() or item.is_coord():
             item.node[item.key].attrs = attrs
+        
+        self.finishedEditingAttrs.emit()
     
     def popupItemInfo(self, item: XarrayTreeItem):
         if item.is_node():
             text = str(item.node.ds)
         elif item.is_var() or item.is_coord():
             text = str(item.node[item.key])
         else:
```

### Comparing `xarray_treeview-1.2.1/PKG-INFO` & `xarray_treeview-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-treeview
-Version: 1.2.1
+Version: 1.2.2
 Summary: PyQt/PySide model/view for tree of Xarray datasets.
 Keywords: PyQt,PySide,xarray,tree
 Home-page: https://github.com/marcel-goldschen-ohm/xarray-treeview
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

