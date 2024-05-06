# Comparing `tmp/pepperpepper-0.0.7.3.tar.gz` & `tmp/pepperpepper-0.0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.7.3.tar", last modified: Mon May  6 04:22:26 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.7.4.tar", last modified: Mon May  6 04:34:48 2024, max compression
```

## Comparing `pepperpepper-0.0.7.3.tar` & `pepperpepper-0.0.7.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 04:22:26.423112 pepperpepper-0.0.7.3/
--rw-rw-rw-   0        0        0      433 2024-05-06 04:22:26.423112 pepperpepper-0.0.7.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 04:22:26.375640 pepperpepper-0.0.7.3/PepperPepper/
--rw-rw-rw-   0        0        0     5237 2024-05-05 14:53:33.000000 pepperpepper-0.0.7.3/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:22:26.393783 pepperpepper-0.0.7.3/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.7.3/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.7.3/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.7.3/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:22:26.409473 pepperpepper-0.0.7.3/PepperPepper/core/
--rw-rw-rw-   0        0        0     1219 2024-05-05 15:06:09.000000 pepperpepper-0.0.7.3/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.7.3/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     4636 2024-05-06 04:22:13.000000 pepperpepper-0.0.7.3/PepperPepper/core/text_utils.py
--rw-rw-rw-   0        0        0     7067 2024-05-05 14:53:16.000000 pepperpepper-0.0.7.3/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:22:26.409473 pepperpepper-0.0.7.3/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1075 2024-05-04 04:08:04.000000 pepperpepper-0.0.7.3/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0     1016 2024-05-04 04:01:31.000000 pepperpepper-0.0.7.3/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.7.3/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.7.3/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      126 2024-05-05 14:57:43.000000 pepperpepper-0.0.7.3/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:22:26.413098 pepperpepper-0.0.7.3/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.7.3/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.7.3/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.7.3/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.7.3/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:22:26.413098 pepperpepper-0.0.7.3/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.7.3/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.7.3/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.7.3/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:22:26.423112 pepperpepper-0.0.7.3/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.7.3/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.7.3/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:22:26.423112 pepperpepper-0.0.7.3/PepperPepper/models/
--rw-rw-rw-   0        0        0     1359 2024-05-03 11:01:15.000000 pepperpepper-0.0.7.3/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    29938 2024-05-04 02:20:17.000000 pepperpepper-0.0.7.3/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.7.3/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.7.3/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.7.3/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:22:26.423112 pepperpepper-0.0.7.3/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.7.3/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.7.3/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.7.3/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:22:26.423112 pepperpepper-0.0.7.3/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-06 04:22:26.000000 pepperpepper-0.0.7.3/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1257 2024-05-06 04:22:26.000000 pepperpepper-0.0.7.3/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 04:22:26.000000 pepperpepper-0.0.7.3/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-06 04:22:26.000000 pepperpepper-0.0.7.3/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-06 04:22:26.000000 pepperpepper-0.0.7.3/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.7.3/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-06 04:22:26.423112 pepperpepper-0.0.7.3/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-06 04:22:21.000000 pepperpepper-0.0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.887399 pepperpepper-0.0.7.4/
+-rw-rw-rw-   0        0        0      433 2024-05-06 04:34:48.887399 pepperpepper-0.0.7.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.855240 pepperpepper-0.0.7.4/PepperPepper/
+-rw-rw-rw-   0        0        0     5237 2024-05-05 14:53:33.000000 pepperpepper-0.0.7.4/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.871272 pepperpepper-0.0.7.4/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.7.4/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.7.4/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.7.4/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.871272 pepperpepper-0.0.7.4/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1219 2024-05-05 15:06:09.000000 pepperpepper-0.0.7.4/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.7.4/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     4514 2024-05-06 04:34:26.000000 pepperpepper-0.0.7.4/PepperPepper/core/text_utils.py
+-rw-rw-rw-   0        0        0     7067 2024-05-05 14:53:16.000000 pepperpepper-0.0.7.4/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.871272 pepperpepper-0.0.7.4/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1075 2024-05-04 04:08:04.000000 pepperpepper-0.0.7.4/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0     1016 2024-05-04 04:01:31.000000 pepperpepper-0.0.7.4/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.7.4/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.7.4/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      126 2024-05-05 14:57:43.000000 pepperpepper-0.0.7.4/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.871272 pepperpepper-0.0.7.4/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.7.4/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.7.4/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.7.4/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.7.4/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.871272 pepperpepper-0.0.7.4/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.7.4/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.7.4/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.7.4/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.886930 pepperpepper-0.0.7.4/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.7.4/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.7.4/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.887399 pepperpepper-0.0.7.4/PepperPepper/models/
+-rw-rw-rw-   0        0        0     1359 2024-05-03 11:01:15.000000 pepperpepper-0.0.7.4/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    29938 2024-05-04 02:20:17.000000 pepperpepper-0.0.7.4/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.7.4/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.7.4/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.7.4/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.887399 pepperpepper-0.0.7.4/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.7.4/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.7.4/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.7.4/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.887399 pepperpepper-0.0.7.4/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-06 04:34:48.000000 pepperpepper-0.0.7.4/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1257 2024-05-06 04:34:48.000000 pepperpepper-0.0.7.4/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 04:34:48.000000 pepperpepper-0.0.7.4/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-06 04:34:48.000000 pepperpepper-0.0.7.4/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 04:34:48.000000 pepperpepper-0.0.7.4/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.7.4/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-06 04:34:48.887399 pepperpepper-0.0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-06 04:34:42.000000 pepperpepper-0.0.7.4/setup.py
```

### Comparing `pepperpepper-0.0.7.3/PepperPepper/__init__.py` & `pepperpepper-0.0.7.4/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.7.4/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.7.4/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/core/__init__.py` & `pepperpepper-0.0.7.4/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/core/text_utils.py` & `pepperpepper-0.0.7.4/PepperPepper/core/text_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,35 +34,14 @@
 Attributes:
         _token_freqs (list): 按词频降序排列的词元及其频率的列表。
         idx_to_token (list): 索引到词元的映射列表。
         token_to_idx (dict): 词元到索引的映射字典。
 """
 class Vocab:
 
-    def count_corpus(tokens):
-        """
-        统计词元的频率。
-
-        Parameters:
-            tokens (list): 用于统计的词元列表，可以是一维或二维列表。
-
-        Returns:
-            counter (collections.Counter): 词元及其频率的计数器。
-        """
-        # 如果 tokens 是二维列表，将其展平成一维列表
-        if len(tokens) == 0 or isinstance(tokens[0], list):
-            tokens = [token for line in tokens for token in line]
-
-        # 统计词元的频率并返回计数器
-        return collections.Counter(tokens)
-
-
-
-
-
     def __init__(self, tokens=None, min_freq=0, reserved_tokens=None):
         if tokens is None:
             tokens = []
         if reserved_tokens is None:
             reserved_tokens = []
 
 
@@ -82,52 +61,68 @@
         for token, freq in self._token_freqs:
             if freq < min_freq:
                 break
             if token not in self.token_to_idx:
                 self.idx_to_token.append(token)
                 self.token_to_idx[token] = len(self.idx_to_token) - 1
 
-        def __len__(self):
-            """返回词表中的词元数量"""
-            return len(self.idx_to_token)
-
-        def __getitem__(self, tokens):
-            """
-            返回给定词元的索引。
-
-            Parameters:
-                tokens (str or list): 单个词元或词元列表。
-
-            Returns:
-                idx (int or list): 词元对应的索引或索引列表。
-            """
-            # 如果 tokens 是单个词元，返回其索引；如果是词元列表，则返回对应的索引列表
-            if not isinstance(tokens, (list, tuple)):
-                return self.token_to_idx.get(tokens, self.unk)
-            return [self.__getitem__(token) for token in tokens]
-
-        def to_tokens(self, indices):
-            """
-            返回给定索引对应的词元。
-
-            Parameters:
-                indices (int or list): 单个索引或索引列表。
-
-            Returns:
-                tokens (str or list): 索引对应的词元或词元列表。
-            """
-            # 如果 indices 是单个索引，返回对应的词元；如果是索引列表，则返回对应的词元列表
-            if not isinstance(indices, (list, tuple)):
-                return self.idx_to_token[indices]
-            return [self.idx_to_token[index] for index in indices]
-
-        @property
-        def unk(self):
-            """返回未知词元的索引"""
-            return 0
-
-        @property
-        def token_freqs(self):
-            """返回词元及其频率的列表"""
-            return self._token_freqs
+    def __len__(self):
+        """返回词表中的词元数量"""
+        return len(self.idx_to_token)
+
+    def __getitem__(self, tokens):
+        """
+        返回给定词元的索引。
+
+        Parameters:
+            tokens (str or list): 单个词元或词元列表。
 
+        Returns:
+            idx (int or list): 词元对应的索引或索引列表。
+        """
+        # 如果 tokens 是单个词元，返回其索引；如果是词元列表，则返回对应的索引列表
+        if not isinstance(tokens, (list, tuple)):
+            return self.token_to_idx.get(tokens, self.unk)
+        return [self.__getitem__(token) for token in tokens]
+
+    def to_tokens(self, indices):
+        """
+        返回给定索引对应的词元。
+
+        Parameters:
+            indices (int or list): 单个索引或索引列表。
+
+        Returns:
+            tokens (str or list): 索引对应的词元或词元列表。
+        """
+        # 如果 indices 是单个索引，返回对应的词元；如果是索引列表，则返回对应的词元列表
+        if not isinstance(indices, (list, tuple)):
+            return self.idx_to_token[indices]
+        return [self.idx_to_token[index] for index in indices]
+
+    @property
+    def unk(self):
+        """返回未知词元的索引"""
+        return 0
+
+    @property
+    def token_freqs(self):
+        """返回词元及其频率的列表"""
+        return self._token_freqs
+
+    def count_corpus(self, tokens):  # 改为实例方法
+        """
+        统计词元的频率。
+
+        Parameters:
+            tokens (list): 用于统计的词元列表，可以是一维或二维列表。
+
+        Returns:
+            counter (collections.Counter): 词元及其频率的计数器。
+        """
+        # 如果 tokens 是二维列表，将其展平成一维列表
+        if len(tokens) == 0 or isinstance(tokens[0], list):
+            tokens = [token for line in tokens for token in line]
+
+        # 统计词元的频率并返回计数器
+        return collections.Counter(tokens)
```

### Comparing `pepperpepper-0.0.7.3/PepperPepper/core/utils.py` & `pepperpepper-0.0.7.4/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.7.4/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/datasets/custom_dataset.py` & `pepperpepper-0.0.7.4/PepperPepper/datasets/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.7.4/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.7.4/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.7.4/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.7.4/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/models/__init__.py` & `pepperpepper-0.0.7.4/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/models/cnn.py` & `pepperpepper-0.0.7.4/PepperPepper/models/cnn.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.7.4/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.7.4/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.3/setup.py` & `pepperpepper-0.0.7.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.7.3",
+    version="0.0.7.4",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

