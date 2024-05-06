# Comparing `tmp/mergoo-0.0.8.tar.gz` & `tmp/mergoo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergoo-0.0.8.tar", last modified: Sat Apr 27 21:50:51 2024, max compression
+gzip compressed data, was "mergoo-0.0.9.tar", last modified: Mon May  6 13:25:55 2024, max compression
```

## Comparing `mergoo-0.0.8.tar` & `mergoo-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:50:51.696316 mergoo-0.0.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7651 2024-04-27 21:28:42.000000 mergoo-0.0.8/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9732 2024-04-27 21:50:51.696316 mergoo-0.0.8/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:50:51.696316 mergoo-0.0.8/mergoo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1412 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/compose_experts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9272 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/compose_layers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:50:51.696316 mergoo-0.0.8/mergoo/composers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/composers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7253 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/composers/composer_lora_moe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8279 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/composers/composer_moe.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:50:51.696316 mergoo-0.0.8/mergoo/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    85074 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/models/modeling_bert.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    71732 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/models/modeling_llama.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    64002 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/models/modeling_mistral.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9649 2024-04-27 21:28:42.000000 mergoo-0.0.8/mergoo/safe_saving.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-27 21:50:51.696316 mergoo-0.0.8/mergoo.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9732 2024-04-27 21:50:51.000000 mergoo-0.0.8/mergoo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      467 2024-04-27 21:50:51.000000 mergoo-0.0.8/mergoo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-27 21:50:51.000000 mergoo-0.0.8/mergoo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      163 2024-04-27 21:50:51.000000 mergoo-0.0.8/mergoo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-04-27 21:50:51.000000 mergoo-0.0.8/mergoo.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1013 2024-04-27 21:50:32.000000 mergoo-0.0.8/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-27 21:50:51.696316 mergoo-0.0.8/setup.cfg
+drwxrwxr-x   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-05-06 13:25:55.019693 mergoo-0.0.9/
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     7651 2024-05-06 13:21:32.000000 mergoo-0.0.9/LICENSE
+-rw-r--r--   0 alirezamsh  (1000) alirezamsh  (1000)    18252 2024-05-06 13:25:55.019693 mergoo-0.0.9/PKG-INFO
+drwxrwxr-x   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-05-06 13:25:55.015693 mergoo-0.0.9/mergoo/
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     1412 2024-05-06 13:21:32.000000 mergoo-0.0.9/mergoo/compose_experts.py
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     9272 2024-05-06 13:21:32.000000 mergoo-0.0.9/mergoo/compose_layers.py
+drwxrwxr-x   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-05-06 13:25:55.019693 mergoo-0.0.9/mergoo/composers/
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-05-06 13:21:32.000000 mergoo-0.0.9/mergoo/composers/__init__.py
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     7341 2024-05-06 13:21:32.000000 mergoo-0.0.9/mergoo/composers/composer_lora_moe.py
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     8367 2024-05-06 13:21:32.000000 mergoo-0.0.9/mergoo/composers/composer_moe.py
+drwxrwxr-x   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-05-06 13:25:55.019693 mergoo-0.0.9/mergoo/models/
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-05-06 13:21:32.000000 mergoo-0.0.9/mergoo/models/__init__.py
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)    85074 2024-05-06 13:21:32.000000 mergoo-0.0.9/mergoo/models/modeling_bert.py
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)    71732 2024-05-06 13:21:32.000000 mergoo-0.0.9/mergoo/models/modeling_llama.py
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)    64002 2024-05-06 13:21:32.000000 mergoo-0.0.9/mergoo/models/modeling_mistral.py
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)    83252 2024-05-06 13:21:32.000000 mergoo-0.0.9/mergoo/models/modeling_phi3.py
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     9649 2024-05-06 13:21:32.000000 mergoo-0.0.9/mergoo/safe_saving.py
+drwxrwxr-x   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-05-06 13:25:55.019693 mergoo-0.0.9/mergoo.egg-info/
+-rw-r--r--   0 alirezamsh  (1000) alirezamsh  (1000)    18252 2024-05-06 13:25:55.000000 mergoo-0.0.9/mergoo.egg-info/PKG-INFO
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)      508 2024-05-06 13:25:55.000000 mergoo-0.0.9/mergoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)        1 2024-05-06 13:25:55.000000 mergoo-0.0.9/mergoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)      163 2024-05-06 13:25:55.000000 mergoo-0.0.9/mergoo.egg-info/requires.txt
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)        7 2024-05-06 13:25:55.000000 mergoo-0.0.9/mergoo.egg-info/top_level.txt
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     1013 2024-05-06 13:23:04.000000 mergoo-0.0.9/pyproject.toml
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     8519 2024-05-06 13:21:32.000000 mergoo-0.0.9/readme.md
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)       38 2024-05-06 13:25:55.019693 mergoo-0.0.9/setup.cfg
```

### Comparing `mergoo-0.0.8/LICENSE` & `mergoo-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.8/mergoo/compose_experts.py` & `mergoo-0.0.9/mergoo/compose_experts.py`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.8/mergoo/compose_layers.py` & `mergoo-0.0.9/mergoo/compose_layers.py`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.8/mergoo/composers/composer_lora_moe.py` & `mergoo-0.0.9/mergoo/composers/composer_lora_moe.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,24 +69,25 @@
         return False
 
     def _load_base_model(self, model_id):
         try:
             mps = torch.backends.mps.is_available()
         except:
             mps = False
-        config = AutoConfig.from_pretrained(model_id)
+        config = AutoConfig.from_pretrained(model_id, trust_remote_code=True)
         if config.model_type == "bert":
             model = self.model_cls.from_pretrained(
-                model_id, torch_dtype=self.torch_dtype
+                model_id, torch_dtype=self.torch_dtype, trust_remote_code=True
             )
         else:
             model = self.model_cls.from_pretrained(
                 model_id,
                 torch_dtype=self.torch_dtype,
                 device_map=None if mps else self.device_map,
+                trust_remote_code=True,
             )
         if mps:
             return model.to(self.device)
         return model
 
     def compose(self):
         """
```

### Comparing `mergoo-0.0.8/mergoo/composers/composer_moe.py` & `mergoo-0.0.9/mergoo/composers/composer_moe.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,24 +70,25 @@
         return False
 
     def _load_base_model(self, model_id):
         try:
             mps = torch.backends.mps.is_available()
         except:
             mps = False
-        config = AutoConfig.from_pretrained(model_id)
+        config = AutoConfig.from_pretrained(model_id, trust_remote_code=True)
         if config.model_type == "bert":
             model = self.model_cls.from_pretrained(
-                model_id, torch_dtype=self.torch_dtype
+                model_id, torch_dtype=self.torch_dtype, trust_remote_code=True
             )
         else:
             model = self.model_cls.from_pretrained(
                 model_id,
                 torch_dtype=self.torch_dtype,
                 device_map=None if mps else self.device_map,
+                trust_remote_code=True,
             )
         if mps:
             return model.to(self.device)
         return model
 
     def compose(self):
         """
```

### Comparing `mergoo-0.0.8/mergoo/models/modeling_bert.py` & `mergoo-0.0.9/mergoo/models/modeling_bert.py`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.8/mergoo/models/modeling_llama.py` & `mergoo-0.0.9/mergoo/models/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.8/mergoo/models/modeling_mistral.py` & `mergoo-0.0.9/mergoo/models/modeling_mistral.py`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.8/mergoo/safe_saving.py` & `mergoo-0.0.9/mergoo/safe_saving.py`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.8/pyproject.toml` & `mergoo-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mergoo"
-version = "0.0.8"
+version = "0.0.9"
 description = "Impelementation of Leeroo LLM composer."
 authors = [{ name = "Leeroo Team", email = "support@leeroo.com" }]
-readme = "README.md"
+readme = "readme.md"
 keywords = ["LLM", "compose", "MoE", "router", "mixture-of-adapters", "merge"]
 license = {file = "LICENSE"}
 dependencies = [
     "torch>=2.0.0",
     "tqdm==4.66.2",
     "safetensors~=0.4.2",
     "accelerate~=0.27.2",
```

