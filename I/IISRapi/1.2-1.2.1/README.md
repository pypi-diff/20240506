# Comparing `tmp/IISRapi-1.2.tar.gz` & `tmp/IISRapi-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IISRapi-1.2.tar", last modified: Tue Apr 23 07:59:28 2024, max compression
+gzip compressed data, was "IISRapi-1.2.1.tar", last modified: Mon May  6 03:38:59 2024, max compression
```

## Comparing `IISRapi-1.2.tar` & `IISRapi-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 07:59:28.852008 IISRapi-1.2/
-drwxrwxrwx   0        0        0        0 2024-04-23 07:59:28.802603 IISRapi-1.2/IISRapi/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:53:31.000000 IISRapi-1.2/IISRapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:59:28.846024 IISRapi-1.2/IISRapi/model/
--rw-rw-rw-   0        0        0       26 2024-04-22 06:07:16.000000 IISRapi-1.2/IISRapi/model/__init__.py
--rw-rw-rw-   0        0        0      202 2024-04-22 08:37:02.000000 IISRapi-1.2/IISRapi/model/data.py
--rw-rw-rw-   0        0        0     5904 2024-04-23 07:55:52.000000 IISRapi-1.2/IISRapi/model/ner.py
--rw-rw-rw-   0        0        0     3569 2024-04-23 07:54:36.000000 IISRapi-1.2/IISRapi/model/pun.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:59:28.836051 IISRapi-1.2/IISRapi.egg-info/
--rw-rw-rw-   0        0        0      138 2024-04-23 07:59:28.000000 IISRapi-1.2/IISRapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-04-23 07:59:28.000000 IISRapi-1.2/IISRapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 07:59:28.000000 IISRapi-1.2/IISRapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-23 07:59:28.000000 IISRapi-1.2/IISRapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 07:59:28.000000 IISRapi-1.2/IISRapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      138 2024-04-23 07:59:28.849017 IISRapi-1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-23 07:59:28.852008 IISRapi-1.2/setup.cfg
--rw-rw-rw-   0        0        0      240 2024-04-23 07:59:19.000000 IISRapi-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:38:59.249205 IISRapi-1.2.1/
+drwxrwxrwx   0        0        0        0 2024-05-06 03:38:59.207369 IISRapi-1.2.1/IISRapi/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:53:31.000000 IISRapi-1.2.1/IISRapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:38:59.245627 IISRapi-1.2.1/IISRapi/model/
+-rw-rw-rw-   0        0        0       26 2024-04-22 06:07:16.000000 IISRapi-1.2.1/IISRapi/model/__init__.py
+-rw-rw-rw-   0        0        0      202 2024-04-22 08:37:02.000000 IISRapi-1.2.1/IISRapi/model/data.py
+-rw-rw-rw-   0        0        0     6003 2024-04-24 06:16:12.000000 IISRapi-1.2.1/IISRapi/model/ner.py
+-rw-rw-rw-   0        0        0     4120 2024-05-06 03:26:04.000000 IISRapi-1.2.1/IISRapi/model/pun.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:38:59.236987 IISRapi-1.2.1/IISRapi.egg-info/
+-rw-rw-rw-   0        0        0      140 2024-05-06 03:38:58.000000 IISRapi-1.2.1/IISRapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-06 03:38:58.000000 IISRapi-1.2.1/IISRapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 03:38:58.000000 IISRapi-1.2.1/IISRapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-06 03:38:58.000000 IISRapi-1.2.1/IISRapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 03:38:58.000000 IISRapi-1.2.1/IISRapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      140 2024-05-06 03:38:59.247210 IISRapi-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-06 03:38:59.250333 IISRapi-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      242 2024-05-06 03:36:29.000000 IISRapi-1.2.1/setup.py
```

### Comparing `IISRapi-1.2/IISRapi/model/ner.py` & `IISRapi-1.2.1/IISRapi/model/ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 from flair.models import SequenceTagger
 from flair.data import Sentence
 from .data import Data
 class IISRner:
     def __init__(self,dev):
         self.model_path=self.get_path()
         if(dev>=0 and torch.cuda.is_available()):
-             flair.device = torch.device('cuda:' + str(dev))
+            flair.device = torch.device('cuda:' + str(dev))
+            print(f"Running model with GPU No.{dev}")
         else:
             flair.device = torch.device('cpu')
+            print("Running model with CPU")
        
         self.model = self.load_model()
         
     def get_path(self):
         try:
             import IISRner
             path=os.path.join(os.path.dirname(IISRner.__file__),"best-model-ner.pt")
```

### Comparing `IISRapi-1.2/IISRapi/model/pun.py` & `IISRapi-1.2.1/IISRapi/model/pun.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 import subprocess
 from flair.models import SequenceTagger
 from flair.data import Sentence
 from .data import Data
 class IISRpunctuation:
     def __init__(self,dev):
         self.model_path=self.get_path()
-        self.result=Data(ori_txt="",ret_txt="")
         if(dev>=0 and torch.cuda.is_available()):
-             flair.device = torch.device('cuda:' + str(dev))
+            flair.device = torch.device('cuda:' + str(dev))
+            print(f"Running model with GPU No.{dev}")
         else:
             flair.device = torch.device('cpu')
+            print("Running model with CPU")
             
         self.model = self.load_model()
         
     def get_path(self):
         try:
             import IISRpunctuation
             path=os.path.join(os.path.dirname(IISRpunctuation.__file__),"best-model-pun.pt")
@@ -31,20 +32,34 @@
         return path
     
     def load_model(self):
         return SequenceTagger.load(self.model_path)
         
     def __call__(self,text):
         if isinstance(text, str):
-            ret_txt,punct=self.tokenize(text.split('\n'))
-            result=Data(ori_txt=text, ret_txt=ret_txt,punct=punct)
+            
+            if(len(text)==1):
+                ret_txt=text+'。'
+                punct=[('。', 0)]
+                result=Data(ori_txt=text, ret_txt=ret_txt,punct=punct)
+            else:
+                ret_txt,punct=self.tokenize(text.split('\n'))
+                result=Data(ori_txt=text, ret_txt=ret_txt,punct=punct)
             return result
+        
         elif isinstance(text,Data):
-            ret_txt,punct=self.ner(text.split('\n'))
-            result=text._replace(ori_txt=text.ori_txt,ret_txt=ret_txt,punct=punct)
+            
+            if(len(text.ori_txt)==1):
+                ret_txt=text.ori_txt+'。'
+                punct=[('。', 0)]
+                result=text._replace(ori_txt=text.ori_txt,ret_txt=ret_txt,punct=punct)
+                
+            else:
+                ret_txt,punct=self.tokenize(text.split('\n'))
+                result=text._replace(ori_txt=text.ori_txt,ret_txt=ret_txt,punct=punct)
             return result
 
     def tokenize(self,sentences):
         pos=[]
         WINDOW_SIZE = 256
         tokenized_sentences=[]
         for text in sentences:
@@ -78,11 +93,11 @@
                     with_punctuation.append('\u3002')
                     pos.append(('\u3002',curr_pos))
                 while curr_pos > curr_seg:
                     with_punctuation.pop()
                     curr_pos -= 1
             tokenized_sentences.append(''.join(with_punctuation))
             tokenized_string=''.join(tokenized_sentences)
-        return tokenized_string,pos
+            return tokenized_string,pos
 '''
 
 '''
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

