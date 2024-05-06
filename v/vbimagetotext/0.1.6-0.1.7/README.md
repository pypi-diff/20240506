# Comparing `tmp/vbimagetotext-0.1.6.tar.gz` & `tmp/vbimagetotext-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbimagetotext-0.1.6.tar", max compression
+gzip compressed data, was "vbimagetotext-0.1.7.tar", max compression
```

## Comparing `vbimagetotext-0.1.6.tar` & `vbimagetotext-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717635 vbimagetotext-0.1.6/README.md
--rw-r--r--   0        0        0      588 2024-05-06 13:54:19.679481 vbimagetotext-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717586 vbimagetotext-0.1.6/vbimagetotext/__init__.py
--rw-r--r--   0        0        0       55 2024-04-16 08:45:08.023791 vbimagetotext-0.1.6/vbimagetotext/__main__.py
--rw-r--r--   0        0        0     1236 2024-04-16 08:47:47.097235 vbimagetotext-0.1.6/vbimagetotext/choice_option.py
--rw-r--r--   0        0        0     1518 2024-05-01 23:15:21.290644 vbimagetotext-0.1.6/vbimagetotext/copyprompt.py
--rw-r--r--   0        0        0     5109 2024-05-01 23:24:09.689153 vbimagetotext-0.1.6/vbimagetotext/functions.py
--rw-r--r--   0        0        0     2776 2024-04-26 07:27:12.309253 vbimagetotext-0.1.6/vbimagetotext/geminivision.py
--rw-r--r--   0        0        0     1611 2024-05-01 23:17:13.262619 vbimagetotext-0.1.6/vbimagetotext/gptvision.py
--rw-r--r--   0        0        0      428 2024-05-01 23:23:16.539392 vbimagetotext-0.1.6/vbimagetotext/main.py
--rw-r--r--   0        0        0     9068 2024-05-06 13:54:14.000465 vbimagetotext-0.1.6/vbimagetotext/prompts.py
--rw-r--r--   0        0        0     1070 2024-05-02 11:19:07.184507 vbimagetotext-0.1.6/vbimagetotext/solution.py
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 vbimagetotext-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717635 vbimagetotext-0.1.7/README.md
+-rw-r--r--   0        0        0      588 2024-05-06 13:57:19.777799 vbimagetotext-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717586 vbimagetotext-0.1.7/vbimagetotext/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-16 08:45:08.023791 vbimagetotext-0.1.7/vbimagetotext/__main__.py
+-rw-r--r--   0        0        0     1236 2024-04-16 08:47:47.097235 vbimagetotext-0.1.7/vbimagetotext/choice_option.py
+-rw-r--r--   0        0        0     1518 2024-05-01 23:15:21.290644 vbimagetotext-0.1.7/vbimagetotext/copyprompt.py
+-rw-r--r--   0        0        0     5109 2024-05-01 23:24:09.689153 vbimagetotext-0.1.7/vbimagetotext/functions.py
+-rw-r--r--   0        0        0     2776 2024-04-26 07:27:12.309253 vbimagetotext-0.1.7/vbimagetotext/geminivision.py
+-rw-r--r--   0        0        0     1611 2024-05-01 23:17:13.262619 vbimagetotext-0.1.7/vbimagetotext/gptvision.py
+-rw-r--r--   0        0        0      428 2024-05-01 23:23:16.539392 vbimagetotext-0.1.7/vbimagetotext/main.py
+-rw-r--r--   0        0        0     9081 2024-05-06 13:57:13.429263 vbimagetotext-0.1.7/vbimagetotext/prompts.py
+-rw-r--r--   0        0        0     1070 2024-05-02 11:19:07.184507 vbimagetotext-0.1.7/vbimagetotext/solution.py
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 vbimagetotext-0.1.7/PKG-INFO
```

### Comparing `vbimagetotext-0.1.6/pyproject.toml` & `vbimagetotext-0.1.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vbimagetotext"
-version = "0.1.6"
+version = "0.1.7"
 description = "A cli tool to convert image to text using openai's GPT-Vision API and google's Gemini Vision API"
 authors = ["vaibhavblayer <vaibhavblayer@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 click = "^8.1.7"
```

### Comparing `vbimagetotext-0.1.6/vbimagetotext/choice_option.py` & `vbimagetotext-0.1.7/vbimagetotext/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.6/vbimagetotext/copyprompt.py` & `vbimagetotext-0.1.7/vbimagetotext/copyprompt.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.6/vbimagetotext/functions.py` & `vbimagetotext-0.1.7/vbimagetotext/functions.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.6/vbimagetotext/geminivision.py` & `vbimagetotext-0.1.7/vbimagetotext/geminivision.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.6/vbimagetotext/gptvision.py` & `vbimagetotext-0.1.7/vbimagetotext/gptvision.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.6/vbimagetotext/prompts.py` & `vbimagetotext-0.1.7/vbimagetotext/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         &= m\left(\dfrac{3}{4}v_0\hat{i}\right)-m\left(v_0\hat{i}\right)\\
         &= -\dfrac{1}{4}mv_0\hat{i}\\
         &= -\dfrac{5}{4}mv_0\hat{i}
         \interttext{Option (a) is correct.}
     \end{align*}
 \end{solution}
 
-Try not to use any derived formula if possible, go with fundamentals and basics also do not put numerical value at every step derive expression then at the end put numerical values. Also if possible use align* environment for solutions. You can add descriptive text in between using \intertext{} command.
+Try not to use any derived formula if possible, go with fundamentals and basics also do not put numerical value at every step derive expression symbolically then at the end put numerical values. Also if possible use align* environment for solutions. You can add descriptive text in between using \intertext{} command.
 
 Please provide only the solution part of the LaTeX file, not the whole LaTeX file.
 """
 
 
 def switch_prompt(value):
     if value == "match":
```

### Comparing `vbimagetotext-0.1.6/vbimagetotext/solution.py` & `vbimagetotext-0.1.7/vbimagetotext/solution.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.6/PKG-INFO` & `vbimagetotext-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbimagetotext
-Version: 0.1.6
+Version: 0.1.7
 Summary: A cli tool to convert image to text using openai's GPT-Vision API and google's Gemini Vision API
 Author: vaibhavblayer
 Author-email: vaibhavblayer@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

