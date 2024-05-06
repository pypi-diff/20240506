# Comparing `tmp/r3xa-2024.4.dev2.tar.gz` & `tmp/r3xa-2024.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r3xa-2024.4.dev2.tar", max compression
+gzip compressed data, was "r3xa-2024.5.dev1.tar", max compression
```

## Comparing `r3xa-2024.4.dev2.tar` & `r3xa-2024.5.dev1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      778 2024-04-30 09:24:50.435803 r3xa-2024.4.dev2/README.md
--rw-r--r--   0        0        0     1758 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-30 09:24:50.461803 r3xa-2024.4.dev2/r3xa/__init__.py
--rw-r--r--   0        0        0    26052 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/r3xa/gui.py
--rw-r--r--   0        0        0    10884 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/r3xa/metadata.py
--rw-r--r--   0        0        0     2644 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/r3xa/scripts.py
--rw-r--r--   0        0        0     3183 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/r3xa/utils.py
--rw-r--r--   0        0        0      517 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/r3xa/validation.py
--rw-r--r--   0        0        0     3468 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/r3xa/visualisation.py
--rw-r--r--   0        0        0    33678 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/resources/schema.json
--rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 r3xa-2024.4.dev2/PKG-INFO
+-rw-r--r--   0        0        0      778 2024-05-06 14:46:43.521691 r3xa-2024.5.dev1/README.md
+-rw-r--r--   0        0        0     1758 2024-05-06 14:46:43.521691 r3xa-2024.5.dev1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 14:46:43.547690 r3xa-2024.5.dev1/r3xa/__init__.py
+-rw-r--r--   0        0        0    37619 2024-05-06 14:46:43.521691 r3xa-2024.5.dev1/r3xa/gui.py
+-rw-r--r--   0        0        0    11708 2024-05-06 14:46:43.521691 r3xa-2024.5.dev1/r3xa/metadata.py
+-rw-r--r--   0        0        0     2644 2024-05-06 14:46:43.521691 r3xa-2024.5.dev1/r3xa/scripts.py
+-rw-r--r--   0        0        0     3701 2024-05-06 14:46:43.522691 r3xa-2024.5.dev1/r3xa/utils.py
+-rw-r--r--   0        0        0     1183 2024-05-06 14:46:43.522691 r3xa-2024.5.dev1/r3xa/validation.py
+-rw-r--r--   0        0        0     3468 2024-05-06 14:46:43.522691 r3xa-2024.5.dev1/r3xa/visualisation.py
+-rw-r--r--   0        0        0    29007 2024-05-06 14:46:43.522691 r3xa-2024.5.dev1/resources/schema.json
+-rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 r3xa-2024.5.dev1/PKG-INFO
```

### Comparing `r3xa-2024.4.dev2/README.md` & `r3xa-2024.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `r3xa-2024.4.dev2/pyproject.toml` & `r3xa-2024.5.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "r3xa"
-version = "2024.4.dev2"
+version = "2024.5.dev1"
 description = "Remember, Reuse and Replicate eXperiments and Analyses"
 authors = ["Emmanuel Roubin <emmanuel.roubin@univ-grenoble-alpes.fr>"]
 maintainers = ["Emmanuel Roubin <emmanuel.roubin@univ-grenoble-alpes.fr>"]
 homepage = "https://photomecanics.gitlab.io/r3xa/doc"
 repository = "https://gitlab.com/photomecanics/r3xa"
 keywords = []
 readme = "README.md"
```

### Comparing `r3xa-2024.4.dev2/r3xa/metadata.py` & `r3xa-2024.5.dev1/r3xa/metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import slugify
 import json
 import os
 
-from r3xa.utils import get_schema, random_slug, obj, obj_iter, slugify_file_name, highlight_json, to_float_or_none
+from r3xa.utils import get_schema, random_slug, obj, obj_is_true, obj_iter, slugify_file_name, highlight_json, to_float_or_none
 from r3xa.validation import validate
 
 #####################
 # Meta data classes #
 #####################
 
 
@@ -45,18 +45,29 @@
         "filename": {"type": "string"},
         "delimiter": {"type": "string", "enum": [":", ",", ...]},
         "data_range": {"type": "array", "items": {"type": "string"}}
     }
     ```
     """
 
-    def __init__(self, filename: str, data_range: list, delimiter: str = ";"):
-        self.filename = filename
-        self.data_range = data_range
-        self.delimiter = delimiter
+    def __init__(self, **kwargs):
+        schema = get_schema()
+        dsf = schema["$defs"]["types"]["data_set_file"]["properties"]
+        # required = schema["$defs"]["types"]["unit"]["required"]
+
+        for k, v in dsf.items():
+            if "const" in v:
+                to_assign = v["const"]
+            else:
+                to_assign = kwargs.get(k, v.get("default"))
+
+            if v["type"] == "number":
+                to_assign = to_float_or_none(to_assign)
+
+            setattr(self, k, to_assign)
 
     def __iter__(self):
         for k, v in obj_iter(self):
             yield k, v
 
     def __str__(self):
         return highlight_json(self)
@@ -74,15 +85,15 @@
         # if payload given load then delete key
         if "payload" in kwargs:
             self.load(kwargs["payload"])
             del kwargs["payload"]
 
         # get all attributes from the kwargs and set them
         for k, v in kwargs.items():
-            if obj(v):
+            if obj_is_true(v):
                 setattr(self, k, obj(v))
             # setattr(self, k, v)
 
         # define an ID of the data as the slugified title appended with and random slug
         if not hasattr(self, "id"):
             self.id = random_slug(n=24)
 
@@ -117,40 +128,45 @@
         #         -> each element of the must fall into CASE 1, 2 or 3
 
         def handle_cases_123(k, v):
             v = obj(v)
 
             # handle lists
             if isinstance(v, list):
-                return [handle_cases_123(k, _) for _ in v if obj(_)]
+                return [handle_cases_123(k, _) for _ in v if obj_is_true(_)]
 
             elif isinstance(v, dict):
                 kind = v.get("kind")
 
                 # handle units
-                if v.get("kind") == "unit":
+                if kind == "unit":
                     o = Unit(**v)
                     # return value to assign
                     return o
 
+                elif kind == "data_set_file":
+                    f = DataSetFile(**v)
+                    return f
+
                 raise TypeError(f"Objects of kind {kind} are not handled")
 
             else:
                 # set valid attribute
                 return v
 
         for k, v in payload.items():
             to_be_assigned = handle_cases_123(k, v)
 
             # case value is empty, delete if already set in the past
-            if not to_be_assigned:
+            if not obj_is_true(to_be_assigned):
                 if hasattr(self, k):
                     delattr(self, k)
                 continue
 
+            print(k, to_be_assigned)
             setattr(self, k, to_be_assigned)
 
     def guess_kind(self, data_type):
         # check for data_sets, data_sources and settings
         schema = get_schema()
 
         # get all attributes
@@ -209,24 +225,27 @@
         super().__init__("settings", check, **kwargs)
 
 
 class DataSource(Data):
     def __init__(self, **kwargs):
         super().__init__("data_sources", **kwargs)
 
-    def add_data_set(self, data_set: Data):
-        self.input_data_set = data_set.id
+    def add_input_data_set(self, data_set: Data):
+        if not hasattr(self, "input_data_sets") or not isinstance(getattr(self, "input_data_sets"), list):
+            self.input_data_sets = []
+        self.input_data_sets.append(data_set.id)
+        # self.input_data_set = data_set.id
 
 
 class DataSet(Data):
     def __init__(self, **kwargs):
         super().__init__("data_sets", **kwargs)
 
     def add_data_source(self, data_source: Data):
-        if not hasattr(self, "data_sources"):
+        if not hasattr(self, "data_sources") or not isinstance(getattr(self, "data_sources"), list):
             self.data_sources = []
         self.data_sources.append(data_source.id)
         # self.data_sources = datasource.id
 
 
 class MetaData:
     def __init__(self, **kwargs):
@@ -234,28 +253,28 @@
 
         # if payload given load then delete key
         if "payload" in kwargs:
             self.load(kwargs["payload"])
             del kwargs["payload"]
 
         for k, v in kwargs.items():
-            if obj(v):
+            if obj_is_true(v):
                 setattr(self, k, v)
 
         # add by default settings / data_sources and data_sets
         for k in ["settings", "data_sources", "data_sets"]:
             if not hasattr(self, k):
                 setattr(self, k, [])
 
             # sanity check to remove duplicated ID
             data = {d.id: d for d in getattr(self, k)}
             setattr(self, k, list(data.values()))
 
         # enforce version from schema
-        self.version = schema["properties"]["version"]["const"]
+        self.version = str(schema["properties"]["version"]["const"])
 
     def __iter__(self):
         for k, v in obj_iter(self):
             yield k, v
 
     def __str__(self):
         return highlight_json(self)
@@ -289,19 +308,21 @@
         # set global attributes
         for k, v in payload.items():
             # ignore case of list of settings or data_sources or data_sets
             if k in ["settings", "data_sources", "data_sets"]:
                 continue
 
             # case object is empty, delete if already set in the past
-            if not obj(v):
+            if not obj_is_true(v):
                 if hasattr(self, k):
                     delattr(self, k)
                 continue
 
+            # match type
+
             # set valid attribute
             setattr(self, k, obj(v))
 
         # set settings
         for p in payload.get("settings", []):
             # discard empty objects
             if not len(p):
@@ -310,24 +331,24 @@
             self.add_setting(s)
 
         # set data sources
         for p in payload.get("data_sources", []):
             # discard empty objects
             if not len(p):
                 continue
-
-            print("WARNING: load data_sources is not implemented yet")
+            d = DataSource(payload=p)
+            self.add_data_source(d)
 
         # set data sets
         for p in payload.get("data_sets", []):
             # discard empty objects
             if not len(p):
                 continue
-
-            print("WARNING: load data_sets is not implemented yet")
+            d = DataSet(payload=p)
+            self.add_data_set(d)
 
     def save_json(self, name: str = None, folder: str = None, check: bool = True):
         """Appends .json to name"""
         # check validity
         if check:
             validate(dict(self))
```

### Comparing `r3xa-2024.4.dev2/r3xa/scripts.py` & `r3xa-2024.5.dev1/r3xa/scripts.py`

 * *Files identical despite different names*

### Comparing `r3xa-2024.4.dev2/r3xa/utils.py` & `r3xa-2024.5.dev1/r3xa/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,54 +22,78 @@
 
 
 def obj(value):
     """Convert a value as a dictionary if possible.
     This function is used in the meta data classes to convert them to json parsable objects.
     It implies that the object have their `self.__iter__` functions implemented.
     """
+    if isinstance(value, int):
+        return value
+
     if isinstance(value, str) and value.strip() == "":
         return None
 
     # check if only kind is set and return None
     # this can happen with hidden field in the gui
     if isinstance(value, dict) and "kind" in value and len(value) == 1:
         return None
 
     if isinstance(value, list):
-        return [obj(v) for v in value]
+        return [obj(v) for v in value if obj_is_true(v)]
 
     if isinstance(value, dict):
-        return {k: obj(v) for k, v in value.items() if obj(v)}
+        return {k: obj(v) for k, v in value.items() if obj_is_true(v)}
 
     try:
         return obj(dict(value))
     except (TypeError, ValueError):
         return value
 
 
+def obj_is_true(value):
+    """Determine if a value is true or not basically used to have int 0 == True"""
+    if isinstance(value, int):
+        return value >= 0
+
+    if isinstance(value, float):
+        return True
+
+    if isinstance(value, dict):
+        if "kind" in value and len(value) == 1:
+            return False
+
+    return value
+
+    # if isinstance(value, list):
+    #     return any([obj(v) for v in value])
+    #
+    # if isinstance(value, dict):
+    #     return any([obj(v) for v in value.values()])
+    #
+    # r = True if value else False
+    # return r
+
+
 def obj_iter(instance):
     """Defines the conversion between instance and dictionnary
     It does not ouput unset values and convert list of Iterable to dict if possible.
     """
     for k, v in instance.__dict__.items():
-        # print("obj_iter", k, v, obj(v), end=" ")
-        # ignore unset values
-        if obj(v) is None:
-            # print("doesn't yield")
-            continue
-
+        # return empty lists
         # convert list of Iterable to list of dict if possible
         # used for our own classes where __iter__ is defined
         if isinstance(v, list):
-            # print("list 1", v, end=" ")
-            v = [obj(_) for _ in v if obj(v)]
-            # print("list 2", v, end=" ")
+            v = [obj(_) for _ in v if obj_is_true(v)]
+            yield k, obj(v)
+
+        # ignore unset values
+        if not obj_is_true(v):
+            continue
 
         # yield the key: value pair
-        # print("return", obj(v))
         yield k, obj(v)
 
 
 def get_schema():
     """Reads the current json schema of meta data located in `resources/schema.json`.
     and returns it as a dictionary.
     """
```

### Comparing `r3xa-2024.4.dev2/r3xa/visualisation.py` & `r3xa-2024.5.dev1/r3xa/visualisation.py`

 * *Files identical despite different names*

### Comparing `r3xa-2024.4.dev2/resources/schema.json` & `r3xa-2024.5.dev1/resources/schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9822015579063105%*

 * *Differences: {"'$defs'": "{'settings': {'generic': {'description': 'Experimental parameters should be the "*

 * *            'specimen, patterning technique and machines used (light, testing rig, environmental '*

 * *            'chamber...). Describe the experimental techniques/apparatus and devices used / light '*

 * *            "/ environment chamber ...'}, 'specimen': {'description': 'A specimen.', 'properties': "*

 * *            "{'cad': OrderedDict([('title', 'CAD'), ('description', 'Path to the design of the "*

 * *            "specime […]*

```diff
@@ -2,22 +2,22 @@
     "$defs": {
         "data_sets": {
             "file": {
                 "additionalProperties": false,
                 "description": "When all the data is stored in a single table like file (csv, txt)",
                 "properties": {
                     "data": {
-                        "$ref": "#/$defs/types/data set_file",
-                        "description": "Link and range to the data file",
+                        "$ref": "#/$defs/types/data_set_file",
+                        "description": "Path and range to the data file",
                         "title": "Data"
                     },
                     "data_sources": {
                         "description": "List if IDs of the data sources",
                         "items": {
-                            "type": "string"
+                            "$ref": "#/$defs/types/data_source_id"
                         },
                         "title": "Data sources",
                         "type": "array"
                     },
                     "description": {
                         "description": "The description of the data set",
                         "title": "Description",
@@ -32,14 +32,22 @@
                         "type": "string"
                     },
                     "id": {
                         "description": "ID of the data set",
                         "title": "ID",
                         "type": "string"
                     },
+                    "keywords": {
+                        "description": "A list of keywords",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Keywords",
+                        "type": "array"
+                    },
                     "kind": {
                         "const": "data_sets/file",
                         "description": "Only required for specs implementation purposes",
                         "title": "Kind of data source",
                         "type": "string"
                     },
                     "path": {
@@ -47,80 +55,82 @@
                         "examples": [
                             "..",
                             "my_folder"
                         ],
                         "title": "Path",
                         "type": "string"
                     },
+                    "time_reference": {
+                        "description": "The reference time",
+                        "title": "Time reference",
+                        "type": "number"
+                    },
                     "timestamps": {
-                        "$ref": "#/$defs/types/data set_file",
-                        "description": "Link and range to the timestamps file",
+                        "$ref": "#/$defs/types/data_set_file",
+                        "description": "Path and range to the timestamps file",
                         "title": "Timesamps"
                     },
                     "title": {
                         "description": "The title of the data set",
                         "title": "Title",
                         "type": "string"
-                    },
-                    "units": {
-                        "description": "The units of the output fields",
-                        "items": {
-                            "$ref": "#/$defs/types/unit"
-                        },
-                        "title": "Units",
-                        "type": "array"
                     }
                 },
                 "required": [
                     "id",
                     "kind",
                     "title",
                     "description",
+                    "data_sources",
                     "file_type",
+                    "time_reference",
                     "timestamps",
                     "data"
                 ],
                 "title": "Data set (file)",
                 "type": "object"
             },
             "list": {
                 "additionalProperties": false,
                 "description": "When all the data is stored in separated files (like a list of images)",
                 "properties": {
                     "data": {
-                        "$ref": "#/$defs/types/data set_list",
                         "description": "List of the data files",
-                        "title": "Data"
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Data",
+                        "type": "array"
                     },
                     "data_sources": {
                         "description": "List if IDs of the data sources",
                         "items": {
-                            "type": "string"
+                            "$ref": "#/$defs/types/data_source_id"
                         },
                         "title": "Data sources",
                         "type": "array"
                     },
                     "description": {
                         "description": "The description of the data set",
                         "title": "Description",
                         "type": "string"
                     },
-                    "file_type": {
-                        "description": "MIME of the file",
-                        "examples": [
-                            "text/csv"
-                        ],
-                        "title": "Fiel type",
-                        "type": "string"
-                    },
                     "id": {
-                        "description": "ID of data set",
+                        "description": "ID of the data set",
                         "title": "ID",
                         "type": "string"
                     },
+                    "keywords": {
+                        "description": "A list of keywords",
+                        "items": {
+                            "type": "string"
+                        },
+                        "title": "Keywords",
+                        "type": "array"
+                    },
                     "kind": {
                         "const": "data_sets/list",
                         "description": "Only required for specs implementation purposes",
                         "title": "Kind of data source",
                         "type": "string"
                     },
                     "path": {
@@ -128,38 +138,40 @@
                         "examples": [
                             "..",
                             "my_folder"
                         ],
                         "title": "Path",
                         "type": "string"
                     },
+                    "time_reference": {
+                        "description": "The reference time",
+                        "title": "Time reference",
+                        "type": "number"
+                    },
                     "timestamps": {
-                        "$ref": "#/$defs/types/data set_list",
                         "description": "List of the timestamps",
-                        "title": "Timesamps"
+                        "items": {
+                            "type": "number"
+                        },
+                        "title": "Timesamps",
+                        "type": "array"
                     },
                     "title": {
                         "description": "The title of the data set",
                         "title": "Title",
                         "type": "string"
-                    },
-                    "units": {
-                        "description": "The units of the output fields",
-                        "items": {
-                            "$ref": "#/$defs/types/unit"
-                        },
-                        "title": "Units",
-                        "type": "array"
                     }
                 },
                 "required": [
                     "id",
                     "kind",
                     "title",
                     "description",
+                    "data_sources",
+                    "time_reference",
                     "timestamps",
                     "data"
                 ],
                 "title": "Data set (list)",
                 "type": "object"
             }
         },
@@ -176,30 +188,28 @@
                     },
                     "description": {
                         "description": "The description of your data source",
                         "title": "Description",
                         "type": "string"
                     },
                     "documentation": {
-                        "$ref": "#/$defs/types/uri",
                         "description": "Name, path or ULR of the documentation (no spaces, no accents)",
-                        "title": "Documentation"
+                        "title": "Documentation",
+                        "type": "string"
                     },
                     "exposure": {
                         "$ref": "#/$defs/types/unit",
                         "description": "Exposure time in ms",
                         "title": "Exposure time"
                     },
                     "field_of_view": {
                         "description": "Size of the field of view in m times m",
                         "items": {
                             "$ref": "#/$defs/types/unit"
                         },
-                        "maxItems": 2,
-                        "minItems": 2,
                         "title": "Field of view",
                         "type": "array"
                     },
                     "filter": {
                         "description": "Filter type, manufacturer and model",
                         "title": "Camera or lens filter",
                         "type": "string"
@@ -220,26 +230,27 @@
                         "title": "Image scale"
                     },
                     "image_size": {
                         "description": "Size of the image in pix times pix",
                         "items": {
                             "$ref": "#/$defs/types/unit"
                         },
-                        "maxItems": 2,
-                        "minItems": 2,
                         "title": "Image size",
                         "type": "array"
                     },
-                    "input_data_set": {
-                        "description": "The data set ID serving as an input source",
-                        "title": "Input data set",
-                        "type": "string"
+                    "input_data_sets": {
+                        "description": "The data sets IDs serving as an input to the source",
+                        "items": {
+                            "$ref": "#/$defs/types/data_set_id"
+                        },
+                        "title": "List of the data sets",
+                        "type": "array"
                     },
                     "kind": {
-                        "const": "data_sources/camera",
+                        "const": "data_sources/generic",
                         "description": "Only required for specs implementation purposes",
                         "title": "Kind of data source",
                         "type": "string"
                     },
                     "lens": {
                         "description": "Camera lens manufacturer and model",
                         "title": "Camera lens",
@@ -247,15 +258,15 @@
                     },
                     "manufacturer": {
                         "description": "Manufacturer / vendor / software editor",
                         "title": "Manufacturer",
                         "type": "string"
                     },
                     "model": {
-                        "description": "Model or software version",
+                        "description": "model or software version",
                         "title": "Model",
                         "type": "string"
                     },
                     "noise": {
                         "$ref": "#/$defs/types/unit",
                         "description": "Quantity of noise of the camera",
                         "title": "Noise level"
@@ -296,184 +307,67 @@
                     }
                 },
                 "required": [
                     "id",
                     "kind",
                     "title",
                     "description",
-                    "output_dimension",
                     "output_components",
-                    "image_size",
-                    "field_of_view",
+                    "output_dimension",
+                    "output_units",
+                    "manufacturer",
+                    "model",
                     "image_size"
                 ],
                 "title": "Camera",
                 "type": "object"
             },
             "generic": {
                 "additionalProperties": false,
-                "description": "A data_source is a procedure or a system that generates a data_set. If it is a sensor then his parameters must be specified. If it is an analysis specifies his parameters are specified along with the input parameters. It also indicates the dimension, the number of components and the unit of the output data.",
+                "description": "A data source is a procedure or a system that generates a data set. If it is a sensor then his parameters must be specified. If it is an analysis specifies his parameters are specified along with the input parameters. It also indicates the dimension, the number of components and the unit of the output data.",
                 "properties": {
                     "description": {
                         "description": "The description of your data source",
                         "title": "Description",
                         "type": "string"
                     },
                     "documentation": {
-                        "$ref": "#/$defs/types/uri",
                         "description": "Name, path or ULR of the documentation (no spaces, no accents)",
-                        "title": "Documentation"
-                    },
-                    "id": {
-                        "description": "ID of the data source",
-                        "title": "ID",
-                        "type": "string"
-                    },
-                    "input_data_set": {
-                        "description": "The data set ID serving as an input source",
-                        "title": "Input data set",
-                        "type": "string"
-                    },
-                    "kind": {
-                        "const": "data_sources/generic",
-                        "description": "Only required for specs implementation purposes",
-                        "title": "Kind of data source",
-                        "type": "string"
-                    },
-                    "manufacturer": {
-                        "description": "Manufacturer / vendor / software editor",
-                        "title": "Manufacturer",
-                        "type": "string"
-                    },
-                    "model": {
-                        "description": "Model or software version",
-                        "title": "Model",
+                        "title": "Documentation",
                         "type": "string"
                     },
-                    "output_components": {
-                        "$ref": "#/$defs/types/uint",
-                        "description": "Number of componants / channels of the ouput data",
-                        "title": "Output components"
-                    },
-                    "output_dimension": {
-                        "description": "Dimension of the output data",
-                        "enum": [
-                            "point",
-                            "curve",
-                            "surface",
-                            "volume"
-                        ],
-                        "title": "Output dimension",
-                        "type": "string"
-                    },
-                    "output_units": {
-                        "description": "Unit of the output data",
-                        "items": {
-                            "$ref": "#/$defs/types/unit"
-                        },
-                        "title": "Output units",
-                        "type": "array"
-                    },
-                    "title": {
-                        "description": "The title of your data source",
-                        "title": "Title",
-                        "type": "string"
-                    }
-                },
-                "required": [
-                    "id",
-                    "kind",
-                    "title",
-                    "description",
-                    "output_dimension",
-                    "output_components"
-                ],
-                "title": "Generic data source",
-                "type": "object"
-            },
-            "tomograph": {
-                "additionalProperties": false,
-                "description": "A tomograph daaah",
-                "properties": {
-                    "angular_amplitude": {
-                        "$ref": "#/$defs/types/unit",
-                        "description": "Angular amplitude in degrees",
-                        "title": "Angular amplitude"
-                    },
-                    "current": {
-                        "$ref": "#/$defs/types/unit",
-                        "description": "Source current in \u03bcA",
-                        "title": "Current"
-                    },
-                    "description": {
-                        "description": "The description of your data source",
-                        "title": "Description",
-                        "type": "string"
-                    },
-                    "documentation": {
-                        "$ref": "#/$defs/types/uri",
-                        "description": "Name, path or ULR of the documentation (no spaces, no accents)",
-                        "title": "Documentation"
-                    },
-                    "field_of_view": {
-                        "description": "Size of the field of view in m times m",
-                        "items": {
-                            "$ref": "#/$defs/types/unit"
-                        },
-                        "maxItems": 2,
-                        "minItems": 2,
-                        "title": "Field of view",
-                        "type": "array"
-                    },
                     "id": {
                         "description": "ID of the data source",
                         "title": "ID",
                         "type": "string"
                     },
-                    "image_scale": {
-                        "$ref": "#/$defs/types/unit",
-                        "description": "Scale of the image in vox / m",
-                        "title": "Image scale"
-                    },
-                    "image_size": {
-                        "description": "Size of the image in vox times vox times vox",
+                    "input_data_sets": {
+                        "description": "The data sets IDs serving as an input to the source",
                         "items": {
-                            "$ref": "#/$defs/types/unit"
+                            "$ref": "#/$defs/types/data_set_id"
                         },
-                        "maxItems": 3,
-                        "minItems": 3,
-                        "title": "Image size",
+                        "title": "List of the data sets",
                         "type": "array"
                     },
-                    "input_data_set": {
-                        "description": "The data set ID serving as an input source",
-                        "title": "Input data set",
-                        "type": "string"
-                    },
                     "kind": {
-                        "const": "data_sources/tomograph",
+                        "const": "data_sources/generic",
                         "description": "Only required for specs implementation purposes",
                         "title": "Kind of data source",
                         "type": "string"
                     },
                     "manufacturer": {
                         "description": "Manufacturer / vendor / software editor",
                         "title": "Manufacturer",
                         "type": "string"
                     },
                     "model": {
-                        "description": "Model or software version",
+                        "description": "model or software version",
                         "title": "Model",
                         "type": "string"
                     },
-                    "number_of_projections": {
-                        "$ref": "#/$defs/types/uint",
-                        "description": "Number of projection",
-                        "title": "Number of projections"
-                    },
                     "output_components": {
                         "$ref": "#/$defs/types/uint",
                         "description": "Number of componants / channels of the ouput data",
                         "title": "Output components"
                     },
                     "output_dimension": {
                         "description": "Dimension of the output data",
@@ -494,40 +388,35 @@
                         "title": "Output units",
                         "type": "array"
                     },
                     "title": {
                         "description": "The title of your data source",
                         "title": "Title",
                         "type": "string"
-                    },
-                    "voltage": {
-                        "$ref": "#/$defs/types/unit",
-                        "description": "Source voltage in kV",
-                        "title": "Voltage"
                     }
                 },
                 "required": [
                     "id",
                     "kind",
                     "title",
                     "description",
-                    "output_dimension",
                     "output_components",
-                    "image_size",
-                    "field_of_view",
-                    "image_scale"
+                    "output_dimension",
+                    "output_units",
+                    "manufacturer",
+                    "model"
                 ],
-                "title": "Tomograph",
+                "title": "Generic data source",
                 "type": "object"
             }
         },
         "settings": {
             "generic": {
                 "additionalProperties": false,
-                "description": "A generic setting with minimal number of fields",
+                "description": "Experimental parameters should be the specimen, patterning technique and machines used (light, testing rig, environmental chamber...). Describe the experimental techniques/apparatus and devices used / light / environment chamber ...",
                 "properties": {
                     "description": {
                         "description": "The description of your setting",
                         "title": "Description",
                         "type": "string"
                     },
                     "id": {
@@ -554,16 +443,24 @@
                     "description"
                 ],
                 "title": "Generic setting",
                 "type": "object"
             },
             "specimen": {
                 "additionalProperties": false,
-                "description": "A specimen",
+                "description": "A specimen.",
                 "properties": {
+                    "cad": {
+                        "description": "Path to the design of the specimen",
+                        "examples": [
+                            "my-specimen.vtk"
+                        ],
+                        "title": "CAD",
+                        "type": "string"
+                    },
                     "description": {
                         "description": "The description of your setting",
                         "title": "Description",
                         "type": "string"
                     },
                     "id": {
                         "description": "ID of the setting",
@@ -572,26 +469,26 @@
                     },
                     "kind": {
                         "const": "settings/specimen",
                         "description": "Only required for specs implementation purposes",
                         "title": "Kind of object",
                         "type": "string"
                     },
-                    "names": {
-                        "description": "The names of the specimen",
-                        "items": {
-                            "type": "string"
-                        },
-                        "title": "Names",
-                        "type": "array"
-                    },
-                    "size": {
+                    "patterning_feature_size": {
                         "$ref": "#/$defs/types/unit",
-                        "description": "The size of the specimen",
-                        "title": "Size"
+                        "description": "The characteristic size of the pattern",
+                        "title": "Patterning feature size"
+                    },
+                    "patterning_technique": {
+                        "description": "The patterning technique used on the specimen",
+                        "examples": [
+                            "Base coat of white spray paint with ink stamped speckles"
+                        ],
+                        "title": "Patterning technique",
+                        "type": "string"
                     },
                     "sizes": {
                         "description": "The sizes of the specimen",
                         "items": {
                             "$ref": "#/$defs/types/unit"
                         },
                         "title": "Sizes",
@@ -604,79 +501,72 @@
                     }
                 },
                 "required": [
                     "id",
                     "kind",
                     "title",
                     "description",
-                    "size"
+                    "sizes"
                 ],
                 "title": "Specimen",
                 "type": "object"
             }
         },
         "types": {
-            "data set_file": {
+            "data_set_file": {
                 "examples": [
                     {
                         "delimiter": ":",
                         "filename": "results.csv",
-                        "range": [
-                            "B52",
-                            "B421"
-                        ]
+                        "range": "B52:B421"
                     }
                 ],
                 "properties": {
                     "data_range": {
                         "examples": [
-                            [
-                                "B42",
-                                "B421"
-                            ]
+                            "B42:B421"
                         ],
-                        "items": {
-                            "type": "string"
-                        },
-                        "maxItems": 2,
-                        "minItems": 2,
-                        "type": "array"
+                        "type": "string"
                     },
                     "delimiter": {
                         "default": ";",
-                        "enum": [
+                        "examples": [
                             ";",
                             ",",
                             ":",
-                            "\t",
-                            " "
+                            "\t"
                         ],
                         "type": "string"
                     },
                     "filename": {
                         "type": "string"
+                    },
+                    "kind": {
+                        "const": "data_set_file",
+                        "description": "Only required for specs implementation purposes",
+                        "title": "Kind of object",
+                        "type": "string"
                     }
                 },
+                "required": [
+                    "filename",
+                    "kind"
+                ],
                 "type": "object"
             },
-            "data set_list": {
-                "items": {
-                    "oneOf": [
-                        {
-                            "type": "string"
-                        },
-                        {
-                            "type": "number"
-                        }
-                    ]
-                },
-                "type": "array"
+            "data_set_id": {
+                "description": "The ID of a data set",
+                "type": "string"
+            },
+            "data_source_id": {
+                "description": "The ID of a data source",
+                "type": "string"
             },
-            "string": {
-                "minLength": 4,
+            "setting_id": {
+                "description": "The ID of a setting",
                 "type": "string"
             },
             "uint": {
                 "description": "Unsigned int",
                 "minimum": 0,
                 "title": "uint",
                 "type": "integer"
@@ -686,15 +576,16 @@
                     "kind": {
                         "const": "unit",
                         "description": "Only required for specs implementation purposes",
                         "title": "Kind of object",
                         "type": "string"
                     },
                     "scale": {
-                        "description": "Ratio of the unit with respact to the SI",
+                        "description": "Factor with respect to the standard system",
+                        "title": "Scale",
                         "type": "number"
                     },
                     "title": {
                         "description": "The title of the unit",
                         "examples": [
                             "length",
                             "width",
@@ -721,34 +612,29 @@
                     }
                 },
                 "required": [
                     "kind",
                     "unit"
                 ],
                 "type": "object"
-            },
-            "uri": {
-                "$comment": "regex to prohibit spaces and accents.",
-                "description": "Name, path or ULR of the file (no spaces, no accents)",
-                "type": "string"
             }
         }
     },
     "additionalProperties": false,
     "description": "This is the specs for the R3XA experiments and analysis meta data template.",
     "properties": {
         "authors": {
-            "$ref": "#/$defs/types/string",
             "description": "Authors of the data sets",
             "examples": [
                 "M. Palin, J. Cleese",
                 "ORCID",
                 "HAL-ID"
             ],
-            "title": "Author"
+            "title": "Author",
+            "type": "string"
         },
         "data_sets": {
             "description": "The data sets :)",
             "items": {
                 "anyOf": [
                     {
                         "$ref": "#/$defs/data_sets/file"
@@ -766,17 +652,14 @@
             "items": {
                 "anyOf": [
                     {
                         "$ref": "#/$defs/data_sources/generic"
                     },
                     {
                         "$ref": "#/$defs/data_sources/camera"
-                    },
-                    {
-                        "$ref": "#/$defs/data_sources/tomograph"
                     }
                 ]
             },
             "title": "Data sources",
             "type": "array"
         },
         "date": {
@@ -785,42 +668,42 @@
                 "2020-03-17"
             ],
             "pattern": "^[1-2]{1}[0-9]{3}-(0[1-9]|1[0-2])-(0[1-9]|[12][0-9]|3[01])$",
             "title": "Date",
             "type": "string"
         },
         "description": {
-            "$ref": "#/$defs/types/string",
             "description": "The description of the data sets",
-            "title": "Description"
+            "title": "Description",
+            "type": "string"
         },
         "documentation": {
-            "$ref": "#/$defs/types/uri",
             "description": "URI to the documentation (pdf)",
             "examples": [
                 "./doc/my_doc.pdf",
                 "https://zenodo.org/records/42/doc/my_doc.pdf"
             ],
-            "title": "Documentation"
+            "title": "Documentation",
+            "type": "string"
         },
         "license": {
             "description": "License of the data sets",
             "examples": [
                 "Creative common"
             ],
             "title": "License",
             "type": "string"
         },
         "repository": {
-            "$ref": "#/$defs/types/uri",
             "description": "URL to the repository where the data sets are stored",
             "examples": [
                 "https://zenodo.org/records/42"
             ],
-            "title": "Repository"
+            "title": "Repository",
+            "type": "string"
         },
         "settings": {
             "description": "List of parameters, devices or software that don't explicitly interact with the data sets",
             "items": {
                 "anyOf": [
                     {
                         "$ref": "#/$defs/settings/generic"
@@ -830,25 +713,24 @@
                     }
                 ]
             },
             "title": "Settings",
             "type": "array"
         },
         "title": {
-            "$ref": "#/$defs/types/string",
             "description": "The title of the data sets",
             "example": [
                 "DICComposite2.0",
                 "My awesome data sets"
             ],
             "title": "Title",
             "type": "string"
         },
         "version": {
-            "const": "2024.4.dev2",
+            "const": "2024.5.dev1",
             "description": "Version of the schema used",
             "title": "Version",
             "type": "string"
         }
     },
     "required": [
         "title",
```

### Comparing `r3xa-2024.4.dev2/PKG-INFO` & `r3xa-2024.5.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r3xa
-Version: 2024.4.dev2
+Version: 2024.5.dev1
 Summary: Remember, Reuse and Replicate eXperiments and Analyses
 Home-page: https://photomecanics.gitlab.io/r3xa/doc
 Author: Emmanuel Roubin
 Author-email: emmanuel.roubin@univ-grenoble-alpes.fr
 Maintainer: Emmanuel Roubin
 Maintainer-email: emmanuel.roubin@univ-grenoble-alpes.fr
 Requires-Python: >=3.8.1,<4.0.0
```

