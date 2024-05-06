# Comparing `tmp/pyqt_ext-1.2.0.tar.gz` & `tmp/pyqt_ext-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt_ext-1.2.0.tar", last modified: Tue Apr 30 21:46:12 2024, max compression
+gzip compressed data, was "pyqt_ext-1.2.1.tar", last modified: Mon May  6 21:11:57 2024, max compression
```

## Comparing `pyqt_ext-1.2.0.tar` & `pyqt_ext-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1077 2024-01-29 19:11:38.968151 pyqt_ext-1.2.0/LICENSE
--rw-r--r--   0        0        0      576 2024-03-01 20:13:41.411647 pyqt_ext-1.2.0/README.md
--rw-r--r--   0        0        0     1123 2024-04-30 21:46:12.129666 pyqt_ext-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 18:05:49.614382 pyqt_ext-1.2.0/src/pyqt_ext/__init__.py
--rw-r--r--   0        0        0    15661 2024-04-30 21:40:30.459705 pyqt_ext-1.2.0/src/pyqt_ext/graph/GraphStyle.py
--rw-r--r--   0        0        0       81 2024-02-26 18:05:49.615491 pyqt_ext-1.2.0/src/pyqt_ext/graph/__init__.py
--rw-r--r--   0        0        0     4933 2024-02-26 18:05:49.616028 pyqt_ext-1.2.0/src/pyqt_ext/tmp/Chart.py
--rw-r--r--   0        0        0    14436 2024-04-23 20:40:53.301852 pyqt_ext-1.2.0/src/pyqt_ext/tree/AbstractTreeItem.py
--rw-r--r--   0        0        0    14629 2024-04-22 17:42:52.732350 pyqt_ext-1.2.0/src/pyqt_ext/tree/AbstractTreeModel.py
--rw-r--r--   0        0        0     6553 2024-03-04 20:57:48.587337 pyqt_ext-1.2.0/src/pyqt_ext/tree/KeyValueTreeItem.py
--rw-r--r--   0        0        0     2896 2024-02-26 18:33:33.713144 pyqt_ext-1.2.0/src/pyqt_ext/tree/KeyValueTreeModel.py
--rw-r--r--   0        0        0     3501 2024-03-04 20:57:48.587786 pyqt_ext-1.2.0/src/pyqt_ext/tree/KeyValueTreeView.py
--rw-r--r--   0        0        0    11058 2024-04-30 14:22:19.549036 pyqt_ext-1.2.0/src/pyqt_ext/tree/TreeView.py
--rw-r--r--   0        0        0      392 2024-02-26 18:05:49.619082 pyqt_ext-1.2.0/src/pyqt_ext/tree/__init__.py
--rw-r--r--   0        0        0     1624 2024-04-25 15:58:28.549088 pyqt_ext-1.2.0/src/pyqt_ext/utils/Color.py
--rw-r--r--   0        0        0       64 2024-02-26 18:05:49.619812 pyqt_ext-1.2.0/src/pyqt_ext/utils/__init__.py
--rw-r--r--   0        0        0     5452 2024-04-23 18:11:10.293878 pyqt_ext-1.2.0/src/pyqt_ext/widgets/CollapsibleSection.py
--rw-r--r--   0        0        0     2415 2024-02-29 22:56:53.609934 pyqt_ext-1.2.0/src/pyqt_ext/widgets/ColorButton.py
--rw-r--r--   0        0        0    11883 2024-04-30 18:28:21.131390 pyqt_ext-1.2.0/src/pyqt_ext/widgets/MultiValueSpinBox.py
--rw-r--r--   0        0        0      184 2024-03-05 15:06:04.507342 pyqt_ext-1.2.0/src/pyqt_ext/widgets/__init__.py
--rw-r--r--   0        0        0        0 2024-01-29 19:11:38.971696 pyqt_ext-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 pyqt_ext-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-29 19:11:38.968151 pyqt_ext-1.2.1/LICENSE
+-rw-r--r--   0        0        0      576 2024-03-01 20:13:41.411647 pyqt_ext-1.2.1/README.md
+-rw-r--r--   0        0        0     1123 2024-05-06 21:11:57.060206 pyqt_ext-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-26 18:05:49.614382 pyqt_ext-1.2.1/src/pyqt_ext/__init__.py
+-rw-r--r--   0        0        0    15661 2024-04-30 21:40:30.459705 pyqt_ext-1.2.1/src/pyqt_ext/graph/GraphStyle.py
+-rw-r--r--   0        0        0       81 2024-02-26 18:05:49.615491 pyqt_ext-1.2.1/src/pyqt_ext/graph/__init__.py
+-rw-r--r--   0        0        0     4933 2024-02-26 18:05:49.616028 pyqt_ext-1.2.1/src/pyqt_ext/tmp/Chart.py
+-rw-r--r--   0        0        0    14436 2024-04-23 20:40:53.301852 pyqt_ext-1.2.1/src/pyqt_ext/tree/AbstractTreeItem.py
+-rw-r--r--   0        0        0    14629 2024-04-22 17:42:52.732350 pyqt_ext-1.2.1/src/pyqt_ext/tree/AbstractTreeModel.py
+-rw-r--r--   0        0        0     6553 2024-03-04 20:57:48.587337 pyqt_ext-1.2.1/src/pyqt_ext/tree/KeyValueTreeItem.py
+-rw-r--r--   0        0        0     2896 2024-02-26 18:33:33.713144 pyqt_ext-1.2.1/src/pyqt_ext/tree/KeyValueTreeModel.py
+-rw-r--r--   0        0        0     3501 2024-03-04 20:57:48.587786 pyqt_ext-1.2.1/src/pyqt_ext/tree/KeyValueTreeView.py
+-rw-r--r--   0        0        0    11058 2024-04-30 14:22:19.549036 pyqt_ext-1.2.1/src/pyqt_ext/tree/TreeView.py
+-rw-r--r--   0        0        0      392 2024-02-26 18:05:49.619082 pyqt_ext-1.2.1/src/pyqt_ext/tree/__init__.py
+-rw-r--r--   0        0        0     1624 2024-04-25 15:58:28.549088 pyqt_ext-1.2.1/src/pyqt_ext/utils/Color.py
+-rw-r--r--   0        0        0       64 2024-02-26 18:05:49.619812 pyqt_ext-1.2.1/src/pyqt_ext/utils/__init__.py
+-rw-r--r--   0        0        0     5452 2024-04-23 18:11:10.293878 pyqt_ext-1.2.1/src/pyqt_ext/widgets/CollapsibleSection.py
+-rw-r--r--   0        0        0     2415 2024-02-29 22:56:53.609934 pyqt_ext-1.2.1/src/pyqt_ext/widgets/ColorButton.py
+-rw-r--r--   0        0        0    11804 2024-05-03 14:12:30.627760 pyqt_ext-1.2.1/src/pyqt_ext/widgets/MultiValueSpinBox.py
+-rw-r--r--   0        0        0      184 2024-03-05 15:06:04.507342 pyqt_ext-1.2.1/src/pyqt_ext/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-29 19:11:38.971696 pyqt_ext-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 pyqt_ext-1.2.1/PKG-INFO
```

### Comparing `pyqt_ext-1.2.0/LICENSE` & `pyqt_ext-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/README.md` & `pyqt_ext-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/pyproject.toml` & `pyqt_ext-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-version = "1.2.0"
+version = "1.2.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/marcel-goldschen-ohm/pyqt-ext"
 repository = "https://github.com/marcel-goldschen-ohm/pyqt-ext"
```

### Comparing `pyqt_ext-1.2.0/src/pyqt_ext/graph/GraphStyle.py` & `pyqt_ext-1.2.1/src/pyqt_ext/graph/GraphStyle.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/src/pyqt_ext/tmp/Chart.py` & `pyqt_ext-1.2.1/src/pyqt_ext/tmp/Chart.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/src/pyqt_ext/tree/AbstractTreeItem.py` & `pyqt_ext-1.2.1/src/pyqt_ext/tree/AbstractTreeItem.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/src/pyqt_ext/tree/AbstractTreeModel.py` & `pyqt_ext-1.2.1/src/pyqt_ext/tree/AbstractTreeModel.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/src/pyqt_ext/tree/KeyValueTreeItem.py` & `pyqt_ext-1.2.1/src/pyqt_ext/tree/KeyValueTreeItem.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/src/pyqt_ext/tree/KeyValueTreeModel.py` & `pyqt_ext-1.2.1/src/pyqt_ext/tree/KeyValueTreeModel.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/src/pyqt_ext/tree/KeyValueTreeView.py` & `pyqt_ext-1.2.1/src/pyqt_ext/tree/KeyValueTreeView.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/src/pyqt_ext/tree/TreeView.py` & `pyqt_ext-1.2.1/src/pyqt_ext/tree/TreeView.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/src/pyqt_ext/utils/Color.py` & `pyqt_ext-1.2.1/src/pyqt_ext/utils/Color.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/src/pyqt_ext/widgets/CollapsibleSection.py` & `pyqt_ext-1.2.1/src/pyqt_ext/widgets/CollapsibleSection.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/src/pyqt_ext/widgets/ColorButton.py` & `pyqt_ext-1.2.1/src/pyqt_ext/widgets/ColorButton.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.0/src/pyqt_ext/widgets/MultiValueSpinBox.py` & `pyqt_ext-1.2.1/src/pyqt_ext/widgets/MultiValueSpinBox.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         self.setSizePolicy(QSizePolicy.Expanding, self.sizePolicy().verticalPolicy())
 
         self.editingFinished.connect(self.onTextEdited)
 
         self.setToolTip('index/slice (+Shift: page up/down)')
 
-        # self.setPlaceholderText(self.textFromValues(self._indexed_values))
+        self.lineEdit().setPlaceholderText(self.textFromValues(self._indexed_values))
     
     def indices(self) -> np.ndarray[int]:
         mask = (0 <= self._indices) & (self._indices < len(self._indexed_values))
         return self._indices[mask]
     
     def setIndices(self, indices: list[int] | np.ndarray[int]):
         # print('set_indices:', indices, 'into', self._indexed_values)
@@ -65,15 +65,15 @@
     
     def setIndexedValues(self, values: list | np.ndarray):
         if not isinstance(values, np.ndarray):
             dtype = type(values[0])
             values = np.array(values, dtype=dtype)
         self._indexed_values = values
         self.setIndices(self.indices())
-        # self.setPlaceholderText(self.textFromValues(self._indexed_values))
+        self.lineEdit().setPlaceholderText(self.textFromValues(self._indexed_values))
     
     def selectedValues(self) -> np.ndarray:
         return self._indexed_values[self.indices()]
     
     def setSelectedValues(self, values: list | np.ndarray):
         indices = self.indicesFromValues(values)
         self.setIndices(indices)
@@ -121,18 +121,17 @@
         for field in fields:
             try:
                 field = field.strip()
                 if field == '':
                     continue
                 if field == ':':
                     return self._indexed_values
-                if ':' in field or '-' in field:
-                    # first:last or first-last inclusive
-                    delimeter = ':' if ':' in field else '-'
-                    first, last = [dtype(arg) if len(arg.strip()) else None for arg in field.split(delimeter)]
+                if ':' in field:
+                    # first:last inclusive
+                    first, last = [dtype(arg) if len(arg.strip()) else None for arg in field.split(':')]
                     if first is None:
                         start_index: int = 0
                     else:
                         start_index: int = self.indicesFromValues([first])[0]
                     if last is None:
                         stop_index: int = len(self._indexed_values)
                     else:
@@ -172,15 +171,15 @@
                 last_value = self._indexed_values[index_range[-1]]
                 if np.issubdtype(self._indexed_values.dtype, np.floating):
                     first_value_text = f'{first_value:.6f}'.rstrip('0').rstrip('.')
                     last_value_text = f'{last_value:.6f}'.rstrip('0').rstrip('.')
                 else:
                     first_value_text = str(first_value)
                     last_value_text = str(last_value)
-                texts.append(first_value_text + '-' + last_value_text)
+                texts.append(first_value_text + ':' + last_value_text)
         text = ','.join(texts)
         return text
     
     @Slot()
     def onTextEdited(self):
         text = self.lineEdit().text()
         try:
```

### Comparing `pyqt_ext-1.2.0/PKG-INFO` & `pyqt_ext-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-ext
-Version: 1.2.0
+Version: 1.2.1
 Summary: Collection of PyQt/PySide widgets/tools
 Keywords: PyQt,PySide
 Home-page: https://github.com/marcel-goldschen-ohm/pyqt-ext
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

