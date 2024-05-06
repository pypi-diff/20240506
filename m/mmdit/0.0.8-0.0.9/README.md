# Comparing `tmp/mmdit-0.0.8.tar.gz` & `tmp/mmdit-0.0.9.tar.gz`

## Comparing `mmdit-0.0.8.tar` & `mmdit-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.8/mmdit.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mmdit-0.0.8/mmdit/__init__.py
--rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 mmdit-0.0.8/mmdit/mmdit_generalized_pytorch.py
--rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 mmdit-0.0.8/mmdit/mmdit_pytorch.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.8/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.8/LICENSE
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 mmdit-0.0.8/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 mmdit-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.9/mmdit.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mmdit-0.0.9/mmdit/__init__.py
+-rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 mmdit-0.0.9/mmdit/mmdit_generalized_pytorch.py
+-rw-r--r--   0        0        0     9968 2020-02-02 00:00:00.000000 mmdit-0.0.9/mmdit/mmdit_pytorch.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 mmdit-0.0.9/README.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 mmdit-0.0.9/PKG-INFO
```

### Comparing `mmdit-0.0.8/mmdit.png` & `mmdit-0.0.9/mmdit.png`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.8/.github/workflows/python-publish.yml` & `mmdit-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.8/mmdit/mmdit_generalized_pytorch.py` & `mmdit-0.0.9/mmdit/mmdit_generalized_pytorch.py`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.8/mmdit/mmdit_pytorch.py` & `mmdit-0.0.9/mmdit/mmdit_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     def forward(
         self,
         *,
         text_tokens,
         image_tokens,
         text_mask = None,
         time_cond = None,
-        feedforward_text_tokens = True
+        skip_feedforward_text_tokens = True
     ):
         assert not (exists(time_cond) ^ self.has_cond), 'time condition must be passed in if dim_cond is set at init. it should not be passed in if not set'
 
         if self.has_cond:
             (
                 text_pre_attn_gamma,
                 text_post_attn_gamma,
@@ -298,15 +298,15 @@
 
         # images feedforward residual
 
         image_tokens = image_tokens + image_tokens_residual
 
         # early return, for last block in mmdit
 
-        if not feedforward_text_tokens:
+        if skip_feedforward_text_tokens:
             return text_tokens, image_tokens
 
         # text feedforward
 
         text_tokens = self.text_ff(text_tokens)
 
         # text condition feedforward output
@@ -341,21 +341,21 @@
     def forward(
         self,
         *,
         text_tokens,
         image_tokens,
         text_mask = None,
         time_cond = None,
-        omit_last_text_feedforward = True
+        should_skip_last_feedforward = True
     ):
         for ind, block in enumerate(self.blocks):
             is_last = ind == (len(self.blocks) - 1)
 
             text_tokens, image_tokens = block(
                 time_cond = time_cond,
                 text_tokens = text_tokens,
                 image_tokens = image_tokens,
                 text_mask = text_mask,
-                feedforward_text_tokens = not is_last and omit_last_text_feedforward
+                skip_feedforward_text_tokens = is_last and should_skip_last_feedforward
             )
 
         return text_tokens, image_tokens
```

### Comparing `mmdit-0.0.8/.gitignore` & `mmdit-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.8/LICENSE` & `mmdit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.8/README.md` & `mmdit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.8/pyproject.toml` & `mmdit-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mmdit"
-version = "0.0.8"
+version = "0.0.9"
 description = "MMDiT"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 license = { file = "LICENSE" }
```

### Comparing `mmdit-0.0.8/PKG-INFO` & `mmdit-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mmdit
-Version: 0.0.8
+Version: 0.0.9
 Summary: MMDiT
 Project-URL: Homepage, https://pypi.org/project/mmdit/
 Project-URL: Repository, https://github.com/lucidrains/mmdit
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: mmdit Version: 0.0.8 Summary: MMDiT Project-URL:
+Metadata-Version: 2.3 Name: mmdit Version: 0.0.9 Summary: MMDiT Project-URL:
 Homepage, https://pypi.org/project/mmdit/ Project-URL: Repository, https://
 github.com/lucidrains/mmdit Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

