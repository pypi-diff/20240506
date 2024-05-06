# Comparing `tmp/xarray_graph-0.2.1.tar.gz` & `tmp/xarray_graph-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_graph-0.2.1.tar", last modified: Tue Apr 30 22:56:35 2024, max compression
+gzip compressed data, was "xarray_graph-0.2.2.tar", last modified: Mon May  6 21:13:11 2024, max compression
```

## Comparing `xarray_graph-0.2.1.tar` & `xarray_graph-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-01-11 15:44:26.780358 xarray_graph-0.2.1/LICENSE
--rw-r--r--   0        0        0      238 2024-04-30 22:54:33.783557 xarray_graph-0.2.1/README.md
--rw-r--r--   0        0        0     1393 2024-04-30 22:56:35.753132 xarray_graph-0.2.1/pyproject.toml
--rw-r--r--   0        0        0   101127 2024-04-30 22:51:22.849653 xarray_graph-0.2.1/src/xarray_graph/XarrayGraph.py
--rw-r--r--   0        0        0       48 2024-01-11 15:44:26.782449 xarray_graph-0.2.1/src/xarray_graph/__init__.py
--rw-r--r--   0        0        0     2274 2024-04-30 22:51:19.174738 xarray_graph-0.2.1/src/xarray_graph/__main__.py
--rw-r--r--   0        0        0     1841 2024-04-30 14:22:30.897258 xarray_graph-0.2.1/src/xarray_graph/tmp/RegionsManager.py
--rw-r--r--   0        0        0        0 2024-01-11 15:44:26.782628 xarray_graph-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 xarray_graph-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-11 15:44:26.780358 xarray_graph-0.2.2/LICENSE
+-rw-r--r--   0        0        0      238 2024-04-30 22:54:33.783557 xarray_graph-0.2.2/README.md
+-rw-r--r--   0        0        0     1393 2024-05-06 21:13:11.601174 xarray_graph-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0   100555 2024-05-03 22:59:36.397265 xarray_graph-0.2.2/src/xarray_graph/XarrayGraph.py
+-rw-r--r--   0        0        0       48 2024-01-11 15:44:26.782449 xarray_graph-0.2.2/src/xarray_graph/__init__.py
+-rw-r--r--   0        0        0     2274 2024-04-30 22:51:19.174738 xarray_graph-0.2.2/src/xarray_graph/__main__.py
+-rw-r--r--   0        0        0     1841 2024-04-30 14:22:30.897258 xarray_graph-0.2.2/src/xarray_graph/tmp/RegionsManager.py
+-rw-r--r--   0        0        0        0 2024-01-11 15:44:26.782628 xarray_graph-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 xarray_graph-0.2.2/PKG-INFO
```

### Comparing `xarray_graph-0.2.1/LICENSE` & `xarray_graph-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray_graph-0.2.1/pyproject.toml` & `xarray_graph-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 ]
 requires-python = ">=3.9"
 dependencies = [
     "numpy>=1.26.2",
     "xarray>=2023.12.0",
     "qtpy>=2.4.1",
     "qtawesome>=1.3.0",
-    "pyqt-ext>=1.2.0",
+    "pyqt-ext>=1.2.1",
     "pyqtgraph-ext>=1.2.0",
-    "xarray-treeview>=1.2.0",
+    "xarray-treeview>=1.2.2",
     "scipy>=1.11.4",
     "lmfit>=1.2.2",
 ]
 readme = "README.md"
 keywords = [
     "PyQt",
     "PySide",
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-version = "0.2.1"
+version = "0.2.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/marcel-goldschen-ohm/xarray-graph"
 repository = "https://github.com/marcel-goldschen-ohm/xarray-graph"
```

### Comparing `xarray_graph-0.2.1/src/xarray_graph/XarrayGraph.py` & `xarray_graph-0.2.2/src/xarray_graph/XarrayGraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,19 +38,14 @@
 from pyqtgraph_ext import *
 from xarray_treeview import *
 
 
 # version info (stored in metadata in case needed later)
 from importlib.metadata import version
 XARRAY_GRAPH_VERSION = version('xarray-graph')
-try:
-    i = re.search(r'[a-zA-Z]', XARRAY_GRAPH_VERSION).start()
-    XARRAY_GRAPH_VERSION = XARRAY_GRAPH_VERSION[:i].rstrip('.')
-except Exception:
-    pass
 
 
 # Currently, color is handled by the widgets themselves.
 # pg.setConfigOption('background', (240, 240, 240))
 # pg.setConfigOption('foreground', (0, 0, 0))
 
 
@@ -116,24 +111,24 @@
     
     @data.setter
     def data(self, data: DataTree | xr.Dataset | xr.DataArray | np.ndarray | list[np.ndarray] | tuple[np.ndarray] | None):
         if not isinstance(data, DataTree):
             if data is None:
                 data = DataTree()
             elif isinstance(data, xr.Dataset):
-                data = DataTree(ds=data)
+                data = DataTree(data=data)
             elif isinstance(data, xr.DataArray):
-                data = DataTree(ds=xr.Dataset(data_vars={data.name: data}))
+                data = DataTree(data=xr.Dataset(data_vars={data.name: data}))
             elif isinstance(data, np.ndarray):
-                data = DataTree(ds=xr.Dataset(data_vars={'data': data}))
+                data = DataTree(data=xr.Dataset(data_vars={'data': data}))
             else:
                 # assume list or tuple of two np.ndarrays (x, y)
                 try:
                     x, y = data
-                    data = DataTree(ds=xr.Dataset(data_vars={'y': ('x', y)}, coords={'x': ('x', x)}))
+                    data = DataTree(data=xr.Dataset(data_vars={'y': ('x', y)}, coords={'x': ('x', x)}))
                 except Exception:
                     raise ValueError('XarrayGraph.data.setter: Invalid input.')
         
         # set xarray tree
         self._data = data
         
         # update data tree view
@@ -147,14 +142,20 @@
         # reset xdim in case dims have changed.
         # This also updates selected coords, dim spinboxes and plot grid
         self.xdim = self.xdim
 
         # metadata
         self.attrs['xarray-graph-version'] = XARRAY_GRAPH_VERSION
 
+        # regions tree view
+        self._region_treeview.model().setRoot(AxisRegionTreeItem(self.regions))
+
+        # notes
+        self._notes_edit.setPlainText(self.attrs.get('notes', ''))
+
         # populate array math selections
         # self._update_array_math_comboboxes()
     
     @property
     def dims(self) -> list[str]:
         dims = []
         for node in self.data.subtree:
@@ -273,15 +274,15 @@
         win.show()
     
     def load(self, filepath: str = '') -> None:
         if filepath == '':
             filepath = QFileDialog.getExistingDirectory(self, 'Open from Xarray data store...')
             if filepath == '':
                 return None
-        self.data = open_datatree(filepath)
+        self.data = open_datatree(filepath, 'zarr')
         self._filepath = filepath
         self.setWindowTitle(os.path.split(filepath)[1])
     
     def save(self) -> None:
         if hasattr(self, '_filepath'):
             self.save_as(self._filepath)
         else:
@@ -293,39 +294,28 @@
             if filepath == '':
                 return None
         self.data.to_zarr(filepath)
         self._filepath = filepath
         self.setWindowTitle(os.path.split(filepath)[1])
     
     def import_data(self, filepath: str = '', filetype: str = '') -> None:
-        # ds: xr.Dataset | None = None
-        # if filetype == 'pCLAMP':
-        #     # TODO: implement
-        #     QMessageBox.warning(self, 'Import pCLAMP', 'Importing pCLAMP files is not yet implemented.')
-        #     return
-        # elif filetype == 'HEKA':
-        #     # TODO: implement
-        #     QMessageBox.warning(self, 'Import HEKA', 'Importing HEKA files is not yet implemented.')
-        #     return
-        # elif filetype == 'GOLab TEVC':
-        #     ds, filepath = import_golab_tevc(filepath)
-        # if ds is None:
-        #     return
-        # self.set_data(ds)
-        # if 'regions' in ds.attrs:
-        #     self.metadata['regions'] = ds.attrs['regions']
-        #     del ds.attrs['regions']
-        #     region_labels = [region['label'] for region in self.metadata['regions']]
-        #     self._region_label_list.clear()
-        #     self._region_label_list.addItems(region_labels)
-        #     self.set_selected_region_labels(region_labels)
-        # if 'notes' in ds.attrs:
-        #     self.metadata['notes'] = ds.attrs['notes']
-        #     del ds.attrs['notes']
-        #     self.load_notes(self.metadata['notes'])
+        ds: xr.Dataset | None = None
+        if filetype == 'pCLAMP':
+            # TODO: implement
+            QMessageBox.warning(self, 'Import pCLAMP', 'Importing pCLAMP files is not yet implemented.')
+            return
+        elif filetype == 'HEKA':
+            # TODO: implement
+            QMessageBox.warning(self, 'Import HEKA', 'Importing HEKA files is not yet implemented.')
+            return
+        elif filetype == 'GOLab TEVC':
+            ds, filepath = import_golab_tevc(filepath)
+        if ds is None:
+            return
+        self.data = ds
         self._filepath = os.path.splitext(filepath)[0]
         self.setWindowTitle(os.path.split(filepath)[1])
     
     def autoscale_plots(self, plots: list[Plot] = None) -> None:
         if plots is None:
             plots = self._plots()
         for plot in plots:
@@ -1050,32 +1040,34 @@
         button.setIcon(qta.icon('ph.eye', options=[{'opacity': 0.5}]))
         button.setCheckable(True)
         button.setChecked(False)
         button.setToolTip('Data browser')
         button.released.connect(lambda i=self._control_panel.count(): self._toggle_control_panel_at(i))
         self._control_panel_toolbar.addWidget(button)
 
-        self._data_treeview = XarrayTreeView()
+        self._data_treeviewer = XarrayTreeViewer()
+        self._data_treeview = self._data_treeviewer.view()
         self._data_treeview.setSelectionMode(QAbstractItemView.SelectionMode.ExtendedSelection)
         root: XarrayTreeItem = XarrayTreeItem(node=self.data, key=None)
         model: XarrayTreeModel = XarrayTreeModel(root)
         model.setShowDetailsColumn(False)
         self._data_treeview.setShowCoords(False)
         self._data_treeview.setModel(model)
         self._data_treeview.selectionWasChanged.connect(self._on_tree_selection_changed)
+        self._data_treeviewer.setSizes([100, 1])
 
         self._xdim_combobox = QComboBox()
         self._xdim_combobox.currentTextChanged.connect(self.set_xdim)
 
         panel = QWidget()
         vbox = QVBoxLayout(panel)
         vbox.setContentsMargins(0, 0, 0, 0)
         vbox.setSpacing(0)
 
-        vbox.addWidget(self._data_treeview)
+        vbox.addWidget(self._data_treeviewer)
 
         form = QFormLayout()
         form.setContentsMargins(5, 3, 0, 3)
         form.setSpacing(0)
         form.setHorizontalSpacing(5)
         form.addRow('X axis', self._xdim_combobox)
         vbox.addLayout(form)
@@ -2203,51 +2195,49 @@
                 index = None
                 break
             else:
                 index[dim] = 0
     return permutations
 
 
-# def import_golab_tevc(filepath: str = '', parent: QWidget = None) -> tuple[xr.Dataset, str]:
-#     if filepath == '':
-#         filepath, _filter = QFileDialog.getOpenFileName(parent, 'Import GoLab TEVC', '', 'GoLab TEVC (*.mat)')
-#         if filepath == '':
-#             return None
-#     matdict = sp.io.loadmat(filepath, simplify_cells=True)
-#     # print(matdict)
-#     current = matdict['current']
-#     current_units = matdict['current_units']
-#     if len(current_units) > 1:
-#         prefix = current_units[0]
-#         if prefix in metric_scale_factors:
-#             current *= metric_scale_factors[prefix]
-#             current_units = current_units[1:]
-#     time = np.arange(len(current)) * matdict['time_interval_sec']
-#     ds = xr.Dataset(
-#         data_vars={
-#             'current': (['time'], current, {'units': current_units}),
-#         },
-#         coords={
-#             'time': (['time'], time, {'units': 's'}),
-#         },
-#     )
-#     if 'events' in matdict and matdict['events']:
-#         ds.attrs['regions'] = []
-#         for event in matdict['events']:
-#             time = event['time_sec']
-#             text = event['text']
-#             ds.attrs['regions'].append({
-#                 'dim': 'time',
-#                 'label': f'{time:.6f}',
-#                 'region': [time, time],
-#                 'text': text,
-#             })
-#     if 'notes' in matdict:
-#         ds.attrs['notes'] = matdict['notes']
-#     return ds, filepath
+def import_golab_tevc(filepath: str = '', parent: QWidget = None) -> tuple[xr.Dataset, str]:
+    if filepath == '':
+        filepath, _filter = QFileDialog.getOpenFileName(parent, 'Import GoLab TEVC', '', 'GoLab TEVC (*.mat)')
+        if filepath == '':
+            return None
+    matdict = sp.io.loadmat(filepath, simplify_cells=True)
+    # print(matdict)
+    current = matdict['current']
+    current_units = matdict['current_units']
+    if len(current_units) > 1:
+        prefix = current_units[0]
+        if prefix in metric_scale_factors:
+            current *= metric_scale_factors[prefix]
+            current_units = current_units[1:]
+    time = np.arange(len(current)) * matdict['time_interval_sec']
+    ds = xr.Dataset(
+        data_vars={
+            'current': (['time'], current, {'units': current_units}),
+        },
+        coords={
+            'time': (['time'], time, {'units': 's'}),
+        },
+    )
+    if 'events' in matdict and matdict['events']:
+        ds.attrs['regions'] = []
+        for event in matdict['events']:
+            time = event['time_sec']
+            text = event['text']
+            ds.attrs['regions'].append({
+                'region': {'time': [time, time]},
+                'text': text,
+            })
+    if 'notes' in matdict:
+        ds.attrs['notes'] = matdict['notes']
+    return ds, filepath
 
 
 def test_live():
     app = QApplication()
 
     ui = XarrayGraph()
     ui.setWindowTitle(ui.__class__.__name__)
```

### Comparing `xarray_graph-0.2.1/src/xarray_graph/__main__.py` & `xarray_graph-0.2.2/src/xarray_graph/__main__.py`

 * *Files identical despite different names*

### Comparing `xarray_graph-0.2.1/src/xarray_graph/tmp/RegionsManager.py` & `xarray_graph-0.2.2/src/xarray_graph/tmp/RegionsManager.py`

 * *Files identical despite different names*

### Comparing `xarray_graph-0.2.1/PKG-INFO` & `xarray_graph-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-graph
-Version: 0.2.1
+Version: 0.2.2
 Summary: PyQt/PySide UI for graphing (x,y) slices of Xarray datasets.
 Keywords: PyQt,PySide,xarray,graph
 Home-page: https://github.com/marcel-goldschen-ohm/xarray-graph
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,17 +18,17 @@
 Project-URL: Homepage, https://github.com/marcel-goldschen-ohm/xarray-graph
 Project-URL: Repository, https://github.com/marcel-goldschen-ohm/xarray-graph
 Requires-Python: >=3.9
 Requires-Dist: numpy>=1.26.2
 Requires-Dist: xarray>=2023.12.0
 Requires-Dist: qtpy>=2.4.1
 Requires-Dist: qtawesome>=1.3.0
-Requires-Dist: pyqt-ext>=1.2.0
+Requires-Dist: pyqt-ext>=1.2.1
 Requires-Dist: pyqtgraph-ext>=1.2.0
-Requires-Dist: xarray-treeview>=1.2.0
+Requires-Dist: xarray-treeview>=1.2.2
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: lmfit>=1.2.2
 Description-Content-Type: text/markdown
 
 # xarray-graph
 PyQt/PySide UI for graphing (x,y) slices of Xarray datasets.
```

