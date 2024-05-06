# Comparing `tmp/pycxpress-0.0.6.tar.gz` & `tmp/pycxpress-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycxpress-0.0.6.tar", max compression
+gzip compressed data, was "pycxpress-0.0.7.tar", max compression
```

## Comparing `pycxpress-0.0.6.tar` & `pycxpress-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-04-27 06:43:40.521206 pycxpress-0.0.6/LICENSE
--rw-r--r--   0        0        0     2324 2024-04-27 06:43:40.521206 pycxpress-0.0.6/README.md
--rw-r--r--   0        0        0     4030 2024-04-27 06:43:40.521206 pycxpress-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1036 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/__init__.py
--rw-r--r--   0        0        0      947 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/__main__.py
--rw-r--r--   0        0        0     5428 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/core.py
--rw-r--r--   0        0        0     1501 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/debugger.py
--rw-r--r--   0        0        0      999 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/example/Makefile
--rw-r--r--   0        0        0     2320 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/example/main.cpp
--rw-r--r--   0        0        0     2635 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/example/model.py
--rw-r--r--   0        0        0    10312 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/include/PyCXpress/core.hpp
--rw-r--r--   0        0        0      849 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/include/PyCXpress/utils.hpp
--rw-r--r--   0        0        0     1033 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/interface.py
--rw-r--r--   0        0        0      714 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/utils.py
--rw-r--r--   0        0        0     3669 1970-01-01 00:00:00.000000 pycxpress-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-06 13:41:17.993110 pycxpress-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2324 2024-05-06 13:41:17.993110 pycxpress-0.0.7/README.md
+-rw-r--r--   0        0        0     4064 2024-05-06 13:41:17.993110 pycxpress-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1036 2024-05-06 13:41:17.993110 pycxpress-0.0.7/src/PyCXpress/__init__.py
+-rw-r--r--   0        0        0      947 2024-05-06 13:41:17.993110 pycxpress-0.0.7/src/PyCXpress/__main__.py
+-rw-r--r--   0        0        0     5558 2024-05-06 13:41:17.993110 pycxpress-0.0.7/src/PyCXpress/core.py
+-rw-r--r--   0        0        0     3319 2024-05-06 13:41:17.993110 pycxpress-0.0.7/src/PyCXpress/debugger.py
+-rw-r--r--   0        0        0     1044 2024-05-06 13:41:17.993110 pycxpress-0.0.7/src/PyCXpress/example/Makefile
+-rw-r--r--   0        0        0     2314 2024-05-06 13:41:17.993110 pycxpress-0.0.7/src/PyCXpress/example/main.cpp
+-rw-r--r--   0        0        0     2965 2024-05-06 13:41:17.993110 pycxpress-0.0.7/src/PyCXpress/example/model.py
+-rw-r--r--   0        0        0    10318 2024-05-06 13:41:17.993110 pycxpress-0.0.7/src/PyCXpress/include/PyCXpress/core.hpp
+-rw-r--r--   0        0        0      849 2024-05-06 13:41:17.993110 pycxpress-0.0.7/src/PyCXpress/include/PyCXpress/utils.hpp
+-rw-r--r--   0        0        0     1033 2024-05-06 13:41:17.993110 pycxpress-0.0.7/src/PyCXpress/interface.py
+-rw-r--r--   0        0        0      968 2024-05-06 13:41:17.993110 pycxpress-0.0.7/src/PyCXpress/utils.py
+-rw-r--r--   0        0        0     3669 1970-01-01 00:00:00.000000 pycxpress-0.0.7/PKG-INFO
```

### Comparing `pycxpress-0.0.6/LICENSE` & `pycxpress-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.6/README.md` & `pycxpress-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.6/pyproject.toml` & `pycxpress-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "PyCXpress"
-version = "0.0.6"
+version = "0.0.7"
 description = "PyCXpress is a high-performance hybrid framework that seamlessly integrates Python and C++ to harness the flexibility of Python and the speed of C++ for efficient and expressive computation, particularly in the realm of deep learning and numerical computing."
 readme = "README.md"
 authors = ["chaoqing <chaoqingwang.nick@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/chaoqing/PyCXpress"
 homepage = "https://github.com/chaoqing/PyCXpress"
 packages = [
@@ -63,14 +63,15 @@
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
 pytest-cov = "^5.0.0"
 
 [tool.poetry.group.dev.dependencies]
 debugpy = "^1.8.1"
 find-libpython = "^0.4.0"
+pydevd-pycharm = "^241.15989.155"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py38"]
 line-length = 88
 color = true
```

### Comparing `pycxpress-0.0.6/src/PyCXpress/__init__.py` & `pycxpress-0.0.7/src/PyCXpress/__init__.py`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.6/src/PyCXpress/__main__.py` & `pycxpress-0.0.7/src/PyCXpress/__main__.py`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.6/src/PyCXpress/core.py` & `pycxpress-0.0.7/src/PyCXpress/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -75,25 +75,26 @@
         mcs,
         name,
         bases,
         attrs,
         fields: Dict[str, TensorMeta],
         type: ModelAnnotationType,
         mode: ModelRuntimeType,
+        raw: bool = True,
     ):
         if type == ModelAnnotationType.Input:
             generate_property = mcs.generate_input_property
         elif type == ModelAnnotationType.Output:
             generate_property = mcs.generate_output_property
         else:
             raise NotImplementedError()
 
         for field_name, field_meta in fields.items():
             field_meta.setdefault(field_name)
-            attrs[field_name] = generate_property(field_meta)
+            attrs[field_name] = generate_property(field_meta, raw)
 
         get_buffer_shape, set_buffer_value, init_func = mcs.general_funcs(
             name, [field_meta.name for field_meta in fields.values()]
         )
 
         attrs["__init__"] = init_func
         attrs["set_buffer_value"] = set_buffer_value
@@ -102,53 +103,57 @@
         attrs.setdefault("__slots__", []).append("__buffer_data__")
 
         return super().__new__(mcs, name, bases, attrs)
 
     @staticmethod
     def general_funcs(name: str, field_names: List[str]):
         def get_buffer_shape(self, name: str) -> Tuple[int]:
-            shape: Tuple[int] = getattr(self.__buffer_data__, name).shape
+            shape: Tuple[int] = self.__buffer_data__[name].shape
             return shape
 
         def set_buffer_value(self, name: str, value: np.ndarray) -> None:
-            buffer = getattr(self.__buffer_data__, name)
-            buffer.data = value
+            self.__buffer_data__[name].data = value
 
         def init_func(self):
-            _BufferData_ = namedtuple("_BufferData_", field_names)
-            self.__buffer_data__ = _BufferData_(
-                *tuple(TensorWithShape() for _ in field_names)
-            )
+            self.__buffer_data__ = {field: TensorWithShape() for field in field_names}
 
         return get_buffer_shape, set_buffer_value, init_func
 
     @staticmethod
-    def generate_input_property(field: TensorMeta):
+    def generate_input_property(field: TensorMeta, raw: bool):
         def get_func(self):
-            return getattr(self.__buffer_data__, field.name).data
+            data = self.__buffer_data__[field.name].data
+            if raw:
+                return data
+            else:
+                import tensorflow as tf
+
+                return tf.Variable(data, name=field.name)
 
         def set_func(*_):
             raise AssertionError("Not supported for input tensor")
 
         def del_func(_):
             raise AssertionError("Not supported for input tensor")
 
         return property(fget=get_func, fset=set_func, fdel=del_func, doc=field.doc)
 
     @staticmethod
-    def generate_output_property(field: TensorMeta):
+    def generate_output_property(field: TensorMeta, raw: bool):
         def get_func(self):
             logger.warning(f"Only read the data field {field.name} in debugging mode")
-            buffer = getattr(self.__buffer_data__, field.name)
+            buffer = self.__buffer_data__[field.name]
             return buffer.data[: np.prod(buffer.shape)].reshape(buffer.shape)
 
         def set_func(self, data):
-            buffer = getattr(self.__buffer_data__, field.name)
+            buffer = self.__buffer_data__[field.name]
             buffer.shape = data.shape
-            buffer.data[: np.prod(data.shape)] = data.flatten()
+            len = np.prod(data.shape)
+            assert len <= buffer.data.size
+            buffer.data[:len] = (data if raw else data.numpy()).flatten()
 
         def del_func(_):
             raise AssertionError("Not supported for output tensor")
 
         return property(fget=get_func, fset=set_func, fdel=del_func, doc=field.doc)
```

### Comparing `pycxpress-0.0.6/src/PyCXpress/example/Makefile` & `pycxpress-0.0.7/src/PyCXpress/example/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Compiler
 CC = c++
 PYTHONPATH=../../
-LD_PRELOAD:=$(shell find_libpython)
+LD_PRELOAD:=$(shell find_libpython):/opt/conda/envs/py38/lib/libstdc++.so.6.0.29
 
 # Compiler flags
 CFLAGS = -g -Wall -std=c++17 -fPIC
 CFLAGS += $(shell python3-config --cflags --ldflags --embed)
 CFLAGS += $(shell PYTHONPATH=$(PYTHONPATH) python3 -m PyCXpress --includes)
 
 # The build target executable
```

### Comparing `pycxpress-0.0.6/src/PyCXpress/example/main.cpp` & `pycxpress-0.0.7/src/PyCXpress/example/main.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     for (size_t i = 0; i < 12; i++) {
         data[i] = i;
     }
 
     std::vector<uint8_t> shape   = {3, 4};
     void                *pBuffer = nullptr;
     size_t               nBytes  = 0;
-    std::tie(pBuffer, nBytes) = model.set_buffer("data_to_be_reshaped", {12});
+    std::tie(pBuffer, nBytes)    = model.set_buffer("input/data", {12});
     assert(data.size() * sizeof(double) == nBytes);
 
     memcpy(pBuffer, data.data(), nBytes);
     memcpy(model.set_buffer("new_2d_shape", {2}).first, shape.data(),
            shape.size() * sizeof(uint8_t));
 
     model.run();
```

### Comparing `pycxpress-0.0.6/src/PyCXpress/example/model.py` & `pycxpress-0.0.7/src/PyCXpress/example/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,27 +16,25 @@
     ModelAnnotationType,
     ModelRuntimeType,
     TensorMeta,
     convert_to_spec_tuple,
     pycxpress_debugger,
 )
 
-if "PYCXPRESS_DEBUGGER_TYPE" in os.environ:
-    pycxpress_debugger(debugger=os.environ["PYCXPRESS_DEBUGGER_TYPE"])
-
 
 def show(a: np.ndarray):
     logging.info(f"array data type: {a.dtype}")
     logging.info(f"array data shape: {a.shape}")
     logging.info(f"array data: ")
     logging.info(a)
 
 
 InputFields = dict(
     data_to_be_reshaped=TensorMeta(
+        name="input/data",
         dtype=np.float_,
         shape=(100,),
     ),
     new_2d_shape=TensorMeta(
         dtype=np.uint8,
         shape=-2,
     ),
@@ -44,14 +42,15 @@
 
 
 class InputDataSet(
     metaclass=ModelAnnotationCreator,
     fields=InputFields,
     type=ModelAnnotationType.Input,
     mode=ModelRuntimeType.EagerExecution,
+    raw=False,
 ):
     pass
 
 
 OutputFields = dict(
     output_a=TensorMeta(
         dtype=np.float_,
@@ -61,14 +60,15 @@
 
 
 class OutputDataSet(
     metaclass=ModelAnnotationCreator,
     fields=OutputFields,
     type=ModelAnnotationType.Output,
     mode=ModelRuntimeType.EagerExecution,
+    raw=False,
 ):
     pass
 
 
 class Model:
     def __init__(self):
         self.input = None
@@ -83,34 +83,47 @@
             tuple(convert_to_spec_tuple(InputFields.values(), OutputFields.values())),
         )
 
     def run(self):
         self.model(self.input, self.output)
 
     @staticmethod
-    def model(input: InputDataSet, output: OutputDataSet):
+    def model(input: InputDataSet, output: OutputDataSet, use_tensorflow: bool = True):
         with nullcontext():
             # print(input.data_to_be_reshaped)
             # print(input.new_2d_shape)
-            output.output_a = input.data_to_be_reshaped.reshape(input.new_2d_shape).T
+            if use_tensorflow:
+                import tensorflow as tf
+
+                output.output_a = tf.transpose(
+                    tf.reshape(
+                        input.data_to_be_reshaped, tf.cast(input.new_2d_shape, tf.int32)
+                    )
+                )
+            else:
+                output.output_a = input.data_to_be_reshaped.reshape(
+                    input.new_2d_shape
+                ).T
             # print(output.output_a)
 
 
 def main():
 
     model = Model()
     input_data, output_data, spec = model.initialize()
     print(spec)
 
-    input_data.set_buffer_value("data_to_be_reshaped", np.arange(12, dtype=np.float_))
+    input_data.set_buffer_value("input/data", np.arange(12, dtype=np.float_))
     print(input_data.data_to_be_reshaped)
     input_data.set_buffer_value("new_2d_shape", np.array([3, 4]).astype(np.uint8))
     print(input_data.new_2d_shape)
     output_data.set_buffer_value("output_a", np.arange(12) * 0)
 
     model.run()
     print(output_data.output_a)
     print(output_data.get_buffer_shape("output_a"))
 
+    # pycxpress_debugger()
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `pycxpress-0.0.6/src/PyCXpress/include/PyCXpress/core.hpp` & `pycxpress-0.0.7/src/PyCXpress/include/PyCXpress/core.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -158,23 +158,23 @@
         m_input  = py::none();
         m_output = py::none();
     }
 
 
     BufferPtr set_buffer(const std::string         &name,
                          const std::vector<size_t> &shape) {
-        auto &buf  = m_buffers[name];
+        auto &buf  = m_buffers.at(name);
         auto  pBuf = buf.set(shape);
         m_input.attr("set_buffer_value")(name, buf.array());
         return pBuf;
     }
 
     std::pair<BufferPtr, std::vector<size_t>> get_buffer(
         const std::string &name) {
-        auto &buf   = m_buffers[name];
+        auto &buf   = m_buffers.at(name);
         auto &array = buf.array();
 
         auto                iter = m_output_buffer_sizes.find(name);
         std::vector<size_t> shape;
         if (iter != m_output_buffer_sizes.end()) {
             shape = iter->second;
         } else {  // must be an input tensor, we do not suggest retrieve the
```

### Comparing `pycxpress-0.0.6/src/PyCXpress/include/PyCXpress/utils.hpp` & `pycxpress-0.0.7/src/PyCXpress/include/PyCXpress/utils.hpp`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.6/src/PyCXpress/interface.py` & `pycxpress-0.0.7/src/PyCXpress/interface.py`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.6/PKG-INFO` & `pycxpress-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCXpress
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyCXpress is a high-performance hybrid framework that seamlessly integrates Python and C++ to harness the flexibility of Python and the speed of C++ for efficient and expressive computation, particularly in the realm of deep learning and numerical computing.
 Home-page: https://github.com/chaoqing/PyCXpress
 License: MIT
 Keywords: CPP,Embdedding
 Author: chaoqing
 Author-email: chaoqingwang.nick@gmail.com
 Requires-Python: >=3.8,<4.0
```

