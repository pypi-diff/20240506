# Comparing `tmp/datafog-3.0.0b6.tar.gz` & `tmp/datafog-3.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.0.0b6.tar", last modified: Mon Apr 29 19:02:13 2024, max compression
+gzip compressed data, was "datafog-3.0.1b1.tar", last modified: Mon May  6 17:48:55 2024, max compression
```

## Comparing `datafog-3.0.0b6.tar` & `datafog-3.0.1b1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-29 19:02:13.801563 datafog-3.0.0b6/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-04-29 13:31:05.000000 datafog-3.0.0b6/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     7676 2024-04-29 19:02:13.801322 datafog-3.0.0b6/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6353 2024-04-29 13:31:05.000000 datafog-3.0.0b6/README.md
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-04-29 19:02:13.801614 datafog-3.0.0b6/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1654 2024-04-29 16:44:12.000000 datafog-3.0.0b6/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-29 19:02:13.797088 datafog-3.0.0b6/src/
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-29 19:02:13.799231 datafog-3.0.0b6/src/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       30 2024-04-29 17:21:07.000000 datafog-3.0.0b6/src/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      419 2024-04-29 17:24:00.000000 datafog-3.0.0b6/src/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1256 2024-04-29 15:53:12.000000 datafog-3.0.0b6/src/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     4229 2024-04-29 17:23:58.000000 datafog-3.0.0b6/src/datafog/donuttransformer.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2970 2024-04-29 17:51:56.000000 datafog-3.0.0b6/src/datafog/main.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1744 2024-04-29 18:50:16.000000 datafog-3.0.0b6/src/datafog/pii_annotation.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-29 19:02:13.801041 datafog-3.0.0b6/src/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     7676 2024-04-29 19:02:13.000000 datafog-3.0.0b6/src/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      419 2024-04-29 19:02:13.000000 datafog-3.0.0b6/src/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-29 19:02:13.000000 datafog-3.0.0b6/src/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       62 2024-04-29 19:02:13.000000 datafog-3.0.0b6/src/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-04-29 19:02:13.000000 datafog-3.0.0b6/src/datafog.egg-info/top_level.txt
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-29 19:02:13.800671 datafog-3.0.0b6/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1857 2024-04-29 19:00:17.000000 datafog-3.0.0b6/tests/test_a.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2311 2024-04-29 17:36:32.000000 datafog-3.0.0b6/tests/test_donuttransformer.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1859 2024-04-29 18:46:28.000000 datafog-3.0.0b6/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-06 17:48:55.022077 datafog-3.0.1b1/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-06 15:35:25.000000 datafog-3.0.1b1/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7843 2024-05-06 17:48:55.021793 datafog-3.0.1b1/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6349 2024-05-06 15:35:48.000000 datafog-3.0.1b1/README.md
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-06 17:48:55.022127 datafog-3.0.1b1/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1792 2024-05-06 17:48:48.000000 datafog-3.0.1b1/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-06 17:48:55.016617 datafog-3.0.1b1/src/
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-06 17:48:55.019067 datafog-3.0.1b1/src/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       22 2024-05-06 17:46:59.000000 datafog-3.0.1b1/src/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      436 2024-05-06 15:51:40.000000 datafog-3.0.1b1/src/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1273 2024-05-06 15:35:48.000000 datafog-3.0.1b1/src/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     4324 2024-05-06 15:35:48.000000 datafog-3.0.1b1/src/datafog/donuttransformer.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     3017 2024-05-06 15:51:40.000000 datafog-3.0.1b1/src/datafog/main.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1709 2024-05-06 15:35:48.000000 datafog-3.0.1b1/src/datafog/pii_annotation.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-06 17:48:55.021420 datafog-3.0.1b1/src/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7843 2024-05-06 17:48:54.000000 datafog-3.0.1b1/src/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      434 2024-05-06 17:48:54.000000 datafog-3.0.1b1/src/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-06 17:48:54.000000 datafog-3.0.1b1/src/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      128 2024-05-06 17:48:54.000000 datafog-3.0.1b1/src/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-06 17:48:54.000000 datafog-3.0.1b1/src/datafog.egg-info/top_level.txt
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-06 17:48:55.021051 datafog-3.0.1b1/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1217 2024-05-06 15:35:49.000000 datafog-3.0.1b1/tests/test_donuttransformer.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1978 2024-05-06 15:35:49.000000 datafog-3.0.1b1/tests/test_main.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1926 2024-05-06 15:51:40.000000 datafog-3.0.1b1/tests/test_textpiiannotator.py
```

### Comparing `datafog-3.0.0b6/LICENSE` & `datafog-3.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.0.0b6/PKG-INFO` & `datafog-3.0.1b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.0.0b6
+Version: 3.0.1b1
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
@@ -27,14 +27,21 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas==2.2.2
 Requires-Dist: Requests==2.31.0
 Requires-Dist: spacy==3.4.4
 Requires-Dist: en_spacy_pii_fast
+Requires-Dist: transformers
+Requires-Dist: torch
+Requires-Dist: pyspark
+Requires-Dist: pydantic
+Requires-Dist: Pillow
+Requires-Dist: sentencepiece
+Requires-Dist: protobuf
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
@@ -57,15 +64,14 @@
 
 DataFog is an open-source DevSecOps platform that lets you scan and redact Personally Identifiable Information (PII) out of your Generative AI applications.
 
 ### Core Problem
 
 ![image](https://github.com/DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
 
-
 How do you keep:
 
 - Customer PII
 - Employee PII
 - Sensitive company information pertaining to org changes or restructurings
 - Pending M&A activity
 - Conversations with external counsel on material corporate matters (i.e. product recall, etc)
@@ -75,29 +81,27 @@
 
 **That's where DataFog comes in.**
 
 ### How it works
 
 ![image](https://github.com/DataFog/datafog-python/assets/61345237/91f4634a-8a9f-4621-81bc-09930feda78a)
 
-
 ### There's lots of PII tools out there; why DataFog?
 
 If you look at the landscape of PII detection tools, their very existence was in many cases driven by regulatory requirements (i.e. 'comply with CCPA/GDPR/HIPAA').
 In this scenario, there's a very defined problem, a specific set of immutable entities to look for, and a relatively static universe of document schema to work with. What that means as an end-result is that the products
 are purpose-built for the problem that they are solving.
 
 However, Generative AI changes how we think about privacy. There's now a changing set of privacy requirements (new M&A deals, internal discussions means new terms to scan/redact) as well as different and varying document sources to contend with. PII detection is no longer just about compliance, it's an active - and for some, new - internal security threat for CISOs and Eng Leaders to contend with. We want DataFog to be built and driven to meet the needs of the open-source community as they tackle this challenge.
 
 ### Roadmap
-DataFog is an active project with regular weekly releases to production (typically on/around Monday evenings US PT).  Here's a snapshot of our coming roadmap; if you have questions or would like to weigh in, join our discord and let us know what we can do to make the product better!
-
-![image](https://github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-0cc99de2ba92)
 
+DataFog is an active project with regular weekly releases to production (typically on/around Monday evenings US PT). Here's a snapshot of our coming roadmap; if you have questions or would like to weigh in, join our discord and let us know what we can do to make the product better!
 
+![image](https://github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-0cc99de2ba92)
 
 ## Installation
 
 DataFog can be installed via pip:
 
 ```bash
 pip install datafog
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.0.0b6 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.0.1b1 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
@@ -11,15 +11,17 @@
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Framework :: tox Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pandas==2.2.2 Requires-Dist: Requests==2.31.0 Requires-Dist: spacy==3.4.4
-Requires-Dist: en_spacy_pii_fast
+Requires-Dist: en_spacy_pii_fast Requires-Dist: transformers Requires-Dist:
+torch Requires-Dist: pyspark Requires-Dist: pydantic Requires-Dist: Pillow
+Requires-Dist: sentencepiece Requires-Dist: protobuf
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
```

### Comparing `datafog-3.0.0b6/README.md` & `datafog-3.0.1b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 DataFog is an open-source DevSecOps platform that lets you scan and redact Personally Identifiable Information (PII) out of your Generative AI applications.
 
 ### Core Problem
 
 ![image](https://github.com/DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
 
-
 How do you keep:
 
 - Customer PII
 - Employee PII
 - Sensitive company information pertaining to org changes or restructurings
 - Pending M&A activity
 - Conversations with external counsel on material corporate matters (i.e. product recall, etc)
@@ -41,29 +40,27 @@
 
 **That's where DataFog comes in.**
 
 ### How it works
 
 ![image](https://github.com/DataFog/datafog-python/assets/61345237/91f4634a-8a9f-4621-81bc-09930feda78a)
 
-
 ### There's lots of PII tools out there; why DataFog?
 
 If you look at the landscape of PII detection tools, their very existence was in many cases driven by regulatory requirements (i.e. 'comply with CCPA/GDPR/HIPAA').
 In this scenario, there's a very defined problem, a specific set of immutable entities to look for, and a relatively static universe of document schema to work with. What that means as an end-result is that the products
 are purpose-built for the problem that they are solving.
 
 However, Generative AI changes how we think about privacy. There's now a changing set of privacy requirements (new M&A deals, internal discussions means new terms to scan/redact) as well as different and varying document sources to contend with. PII detection is no longer just about compliance, it's an active - and for some, new - internal security threat for CISOs and Eng Leaders to contend with. We want DataFog to be built and driven to meet the needs of the open-source community as they tackle this challenge.
 
 ### Roadmap
-DataFog is an active project with regular weekly releases to production (typically on/around Monday evenings US PT).  Here's a snapshot of our coming roadmap; if you have questions or would like to weigh in, join our discord and let us know what we can do to make the product better!
-
-![image](https://github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-0cc99de2ba92)
 
+DataFog is an active project with regular weekly releases to production (typically on/around Monday evenings US PT). Here's a snapshot of our coming roadmap; if you have questions or would like to weigh in, join our discord and let us know what we can do to make the product better!
 
+![image](https://github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-0cc99de2ba92)
 
 ## Installation
 
 DataFog can be installed via pip:
 
 ```bash
 pip install datafog
```

### Comparing `datafog-3.0.0b6/setup.py` & `datafog-3.0.1b1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.0.0-beta.6"
+    return "3.0.1b1"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
@@ -27,14 +27,21 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "pandas==2.2.2",
         "Requests==2.31.0",
         "spacy==3.4.4",
         "en_spacy_pii_fast",
+        "transformers",
+        "torch",
+        "pyspark",
+        "pydantic",
+        "Pillow",
+        "sentencepiece",
+        "protobuf",
     ],
     python_requires=">=3.10",
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `datafog-3.0.0b6/src/datafog/config.py` & `datafog-3.0.1b1/src/datafog/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 from enum import Enum
+from typing import Optional
+
 from pydantic import BaseModel
-from typing import Optional, Dict, List
+
 
 class PipelineOperationType(Enum):
-    READ_IMAGE = 'read_image'
-    PARSE_IMAGE = 'parse_image'
-    TEXT_PII_ANNOTATION = 'text_pii_annotation'
-    TEXT_PII_ANNOTATION_WITH_IMAGE = 'text_pii_annotation_with_image'
+    READ_IMAGE = "read_image"
+    PARSE_IMAGE = "parse_image"
+    TEXT_PII_ANNOTATION = "text_pii_annotation"
+    TEXT_PII_ANNOTATION_WITH_IMAGE = "text_pii_annotation_with_image"
+
 
 class ModelConfig(BaseModel):
     model: str
     processor: str
 
+
 class OperationConfig(BaseModel):
     operation_type: PipelineOperationType
     config: Optional[ModelConfig] = None
 
     @classmethod
     def model_validator(cls, v, values):
         configs = {
             "read_image": ModelConfig(
                 model="naver-clova-ix/donut-base-finetuned-rvlcdip",
-                processor="naver-clova-ix/donut-base-finetuned-rvlcdip"),
+                processor="naver-clova-ix/donut-base-finetuned-rvlcdip",
+            ),
             "parse_image": ModelConfig(
                 model="naver-clova-ix/donut-base-finetuned-cord-v2",
-                processor="naver-clova-ix/donut-base-finetuned-cord-v2")
+                processor="naver-clova-ix/donut-base-finetuned-cord-v2",
+            ),
         }
-        operation_type = values.get('operation_type')
+        operation_type = values.get("operation_type")
         if operation_type and operation_type.value in configs:
             return configs[operation_type.value]
         return v
-    
+
     class Config:
         use_enum_values = True
         validate_assignment = True
         arbitrary_types_allowed = True
```

### Comparing `datafog-3.0.0b6/src/datafog/donuttransformer.py` & `datafog-3.0.1b1/src/datafog/donuttransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from pydantic import HttpUrl
-from transformers import DonutProcessor, VisionEncoderDecoderModel
-from PIL import Image
+import re
 import warnings
 from io import BytesIO
-import re
-import torch
-from enum import Enum
+
+from PIL import Image
+from transformers import DonutProcessor, VisionEncoderDecoderModel
+
 from .config import OperationConfig, PipelineOperationType
 
 
 class DonutImageProcessor:
     """
     A class to process images using the Donut model for different operations like classification, parsing, and question answering.
 
@@ -31,45 +30,56 @@
 
         question_image(image: Image.Image, question: str) -> dict:
             Processes the image to answer a question about the image using the Donut model.
 
         _process_image(image: Image.Image, operation_type_prompt: str) -> dict:
             A helper method to process the image with the model using a specific operation type prompt.
     """
+
     def __init__(self, operation_type: PipelineOperationType):
         self.operation_type = operation_type
-        model_config = OperationConfig.model_validator(None, {'operation_type': operation_type})
+        model_config = OperationConfig.model_validator(
+            None, {"operation_type": operation_type}
+        )
         self.processor = DonutProcessor.from_pretrained(model_config.processor)
         self.model = VisionEncoderDecoderModel.from_pretrained(model_config.model)
         self.device = "cpu"
         self.model.to(self.device)
 
     @staticmethod
     def read_image(file: bytes) -> Image.Image:
         try:
             image = Image.open(BytesIO(file))
             if image.mode != "RGB":
                 warnings.warn("Image mode is not RGB. Converting to RGB.")
                 image = image.convert("RGB")
             return image
         except IOError as e:
-            raise ValueError(f"Unable to read the image file: {e}. Ensure it is a valid image.")
+            raise ValueError(
+                f"Unable to read the image file: {e}. Ensure it is a valid image."
+            )
 
     def classify_image(self, image: Image.Image) -> dict:
         return self._process_image(image, operation_type_prompt="<s_rvlcdip>")
 
     def parse_image(self, image: Image.Image) -> dict:
         return self._process_image(image, operation_type_prompt="<s_cord-v2>")
 
-    def question_image(self, image: Image.Image, question: str = "what is shown in this image?") -> dict:
-        operation_type_prompt = f"<s_docvqa><s_question>{question}</s_question><s_answer>"
+    def question_image(
+        self, image: Image.Image, question: str = "what is shown in this image?"
+    ) -> dict:
+        operation_type_prompt = (
+            f"<s_docvqa><s_question>{question}</s_question><s_answer>"
+        )
         return self._process_image(image, operation_type_prompt=operation_type_prompt)
 
     def _process_image(self, image: Image.Image, operation_type_prompt: str) -> dict:
-        decoder_input_ids = self.processor.tokenizer(operation_type_prompt, add_special_tokens=False, return_tensors="pt").input_ids
+        decoder_input_ids = self.processor.tokenizer(
+            operation_type_prompt, add_special_tokens=False, return_tensors="pt"
+        ).input_ids
         pixel_values = self.processor(image, return_tensors="pt").pixel_values
 
         outputs = self.model.generate(
             pixel_values.to(self.device),
             decoder_input_ids=decoder_input_ids.to(self.device),
             max_length=self.model.decoder.config.max_position_embeddings,
             early_stopping=True,
@@ -78,11 +88,15 @@
             use_cache=True,
             num_beams=1,
             bad_words_ids=[[self.processor.tokenizer.unk_token_id]],
             return_dict_in_generate=True,
         )
 
         sequence = self.processor.batch_decode(outputs.sequences)[0]
-        sequence = sequence.replace(self.processor.tokenizer.eos_token, "").replace(self.processor.tokenizer.pad_token, "")
-        sequence = re.sub(r"<.*?>", "", sequence, count=1).strip()  # remove first operation_type start token
+        sequence = sequence.replace(self.processor.tokenizer.eos_token, "").replace(
+            self.processor.tokenizer.pad_token, ""
+        )
+        sequence = re.sub(
+            r"<.*?>", "", sequence, count=1
+        ).strip()  # remove first operation_type start token
 
         return self.processor.token2json(sequence)
```

### Comparing `datafog-3.0.0b6/src/datafog/main.py` & `datafog-3.0.1b1/src/datafog/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from .donuttransformer import DonutImageProcessor,  PipelineOperationType
-from PIL import Image
-from .pii_annotation import PIIAnnotationModel, PIIAnnotationRequest, PIIAnnotationPipeline
-from typing import Any, List, Optional, Tuple
-from enum import Enum
-
-
+from .donuttransformer import DonutImageProcessor, PipelineOperationType
+from .pii_annotation import (
+    PIIAnnotationModel,
+    PIIAnnotationPipeline,
+    PIIAnnotationRequest,
+)
 
 
 class DataFog:
     """
     A class to process data using the Donut model for image operations and the Spacy model for text operations.
 
     Attributes:
@@ -22,46 +21,51 @@
 
         process_image(file: bytes) -> dict:
             Processes the image for different operations using the Donut model.
 
         process_image_with_text(file: bytes, text: str) -> dict:
             Processes the image for different operations using the Donut model and text for PII entities using the Spacy model.
     """
-    def __init__(self, operation_type: PipelineOperationType, text_pii_annotation: bool = True, image_processor: bool = False):
+
+    def __init__(
+        self,
+        operation_type: PipelineOperationType,
+        text_pii_annotation: bool = True,
+        image_processor: bool = False,
+    ):
         self.text_pii_annotation = text_pii_annotation
         if text_pii_annotation:
             self.text_annotator = PIIAnnotationModel()
         self.image_processor = None
         if image_processor:
             self.image_processor = DonutImageProcessor(operation_type=operation_type)
 
-
     def process_text(self, text: str) -> list:
         request = PIIAnnotationRequest(text=text)
         workflow = PIIAnnotationPipeline(request=request, model=self.text_annotator)
         entities = workflow.process_request()
         return entities
-    
 
     def process_image(self, file: bytes) -> dict:
         image = DonutImageProcessor.read_image(file)
         if self.image_processor.operation_type == PipelineOperationType.READ_IMAGE:
             result = self.image_processor.classify_image(image)
         elif self.image_processor.operation_type == PipelineOperationType.PARSE_IMAGE:
             result = self.image_processor.parse_image(image)
         else:
-            raise ValueError(f"Unsupported operation type: {self.image_processor.operation_type}")
+            raise ValueError(
+                f"Unsupported operation type: {self.image_processor.operation_type}"
+            )
         return result
 
     def annotate_pii_in_images(self, file: bytes) -> dict:
         result = self.process_image(file)
         if self.text_pii_annotation:
             # Iterate over the result and annotate PII into a new dictionary
             for key, value in result.items():
                 if isinstance(value, list):
                     for item in value:
-                        if 'nm' in item:
-                            item['entities'] = self.process_text(item['nm'])  # Store entities directly within the item
+                        if "nm" in item:
+                            item["entities"] = self.process_text(
+                                item["nm"]
+                            )  # Store entities directly within the item
         return result  # Return the modified result dictionary
-
-
-
```

### Comparing `datafog-3.0.0b6/src/datafog/pii_annotation.py` & `datafog-3.0.1b1/src/datafog/pii_annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Description: Define the data models for the PII Detection Workflow
 
-from typing import Any, List, Optional, Tuple
+from typing import Any, List, Tuple
+
 import en_spacy_pii_fast
-import requests
-from pydantic import BaseModel, HttpUrl, FilePath, DirectoryPath
+from pydantic import BaseModel, DirectoryPath, FilePath, HttpUrl
 
 
 class PIIAnnotationModel(BaseModel):
     nlp: Any = None
 
     def load_model(self):
         if self.nlp is None:
@@ -28,16 +28,15 @@
     directory_path: DirectoryPath = None
 
     # add conditional that if none of the fields are filled out, to return an error
     def validate_fields(self):
         if not any([self.text, self.file_path, self.url, self.directory_path]):
             raise ValueError("At least one of the fields must be filled out")
         return True
-    
-    
+
 
 class PIIAnnotationResponse(BaseModel):
     text: str
     entities: List[Tuple[str, str]]
 
 
 class PIIAnnotationPipeline(BaseModel):
@@ -53,8 +52,7 @@
     def run(self):
         entities = self.process_request()
         response = PIIAnnotationResponse(text=self.request.text, entities=entities)
         return response
 
     class Config:
         arbitrary_types_allowed = True
-
```

### Comparing `datafog-3.0.0b6/src/datafog.egg-info/PKG-INFO` & `datafog-3.0.1b1/src/datafog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.0.0b6
+Version: 3.0.1b1
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
@@ -27,14 +27,21 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas==2.2.2
 Requires-Dist: Requests==2.31.0
 Requires-Dist: spacy==3.4.4
 Requires-Dist: en_spacy_pii_fast
+Requires-Dist: transformers
+Requires-Dist: torch
+Requires-Dist: pyspark
+Requires-Dist: pydantic
+Requires-Dist: Pillow
+Requires-Dist: sentencepiece
+Requires-Dist: protobuf
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
@@ -57,15 +64,14 @@
 
 DataFog is an open-source DevSecOps platform that lets you scan and redact Personally Identifiable Information (PII) out of your Generative AI applications.
 
 ### Core Problem
 
 ![image](https://github.com/DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
 
-
 How do you keep:
 
 - Customer PII
 - Employee PII
 - Sensitive company information pertaining to org changes or restructurings
 - Pending M&A activity
 - Conversations with external counsel on material corporate matters (i.e. product recall, etc)
@@ -75,29 +81,27 @@
 
 **That's where DataFog comes in.**
 
 ### How it works
 
 ![image](https://github.com/DataFog/datafog-python/assets/61345237/91f4634a-8a9f-4621-81bc-09930feda78a)
 
-
 ### There's lots of PII tools out there; why DataFog?
 
 If you look at the landscape of PII detection tools, their very existence was in many cases driven by regulatory requirements (i.e. 'comply with CCPA/GDPR/HIPAA').
 In this scenario, there's a very defined problem, a specific set of immutable entities to look for, and a relatively static universe of document schema to work with. What that means as an end-result is that the products
 are purpose-built for the problem that they are solving.
 
 However, Generative AI changes how we think about privacy. There's now a changing set of privacy requirements (new M&A deals, internal discussions means new terms to scan/redact) as well as different and varying document sources to contend with. PII detection is no longer just about compliance, it's an active - and for some, new - internal security threat for CISOs and Eng Leaders to contend with. We want DataFog to be built and driven to meet the needs of the open-source community as they tackle this challenge.
 
 ### Roadmap
-DataFog is an active project with regular weekly releases to production (typically on/around Monday evenings US PT).  Here's a snapshot of our coming roadmap; if you have questions or would like to weigh in, join our discord and let us know what we can do to make the product better!
-
-![image](https://github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-0cc99de2ba92)
 
+DataFog is an active project with regular weekly releases to production (typically on/around Monday evenings US PT). Here's a snapshot of our coming roadmap; if you have questions or would like to weigh in, join our discord and let us know what we can do to make the product better!
 
+![image](https://github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-0cc99de2ba92)
 
 ## Installation
 
 DataFog can be installed via pip:
 
 ```bash
 pip install datafog
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.0.0b6 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.0.1b1 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
@@ -11,15 +11,17 @@
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Framework :: tox Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pandas==2.2.2 Requires-Dist: Requests==2.31.0 Requires-Dist: spacy==3.4.4
-Requires-Dist: en_spacy_pii_fast
+Requires-Dist: en_spacy_pii_fast Requires-Dist: transformers Requires-Dist:
+torch Requires-Dist: pyspark Requires-Dist: pydantic Requires-Dist: Pillow
+Requires-Dist: sentencepiece Requires-Dist: protobuf
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
```

### Comparing `datafog-3.0.0b6/tests/test_a.py` & `datafog-3.0.1b1/tests/test_textpiiannotator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 import pytest
-from datafog import PIIAnnotationModel, PIIAnnotationRequest, PIIAnnotationPipeline
+
+from datafog import PIIAnnotationModel, PIIAnnotationPipeline, PIIAnnotationRequest
+
 
 @pytest.fixture
 def pii_annotation_pipeline():
     model = PIIAnnotationModel()
     request = PIIAnnotationRequest(file_path="tests/test-invoice.png")
     return PIIAnnotationPipeline(request=request, model=model)
 
+
 @pytest.fixture
 def pii_annotation_model():
     model = PIIAnnotationModel()
     model.load_model()
     return model
 
+
 def test_pii_annotation_model_loading(pii_annotation_model):
     # Ensure the model is loaded correctly
-    assert hasattr(pii_annotation_model, 'nlp') and pii_annotation_model.nlp is not None, "Model should be loaded"
+    assert (
+        hasattr(pii_annotation_model, "nlp") and pii_annotation_model.nlp is not None
+    ), "Model should be loaded"
+
 
 def test_pii_annotation_request_validation():
     # Test with no fields filled
     with pytest.raises(ValueError):
         PIIAnnotationRequest().validate_fields()
 
     # Test with one field filled
-    assert PIIAnnotationRequest(text="Sample text").validate_fields() is True, "Validation should pass when text is provided"
+    assert (
+        PIIAnnotationRequest(text="Sample text").validate_fields() is True
+    ), "Validation should pass when text is provided"
+
 
 def test_pii_annotation_pipeline_processing(pii_annotation_pipeline):
     # Mock text processing
     pii_annotation_pipeline.request.text = "John Doe lives in Springfield."
     entities = pii_annotation_pipeline.process_request()
     assert len(entities) > 0, "Should detect entities"
     assert any("PER" in entity for entity in entities), "Should detect person entities"
 
+
 def test_pii_annotation_pipeline_run(pii_annotation_pipeline):
     # Mock text for running the full pipeline
     pii_annotation_pipeline.request.text = "Jane Doe works at DataFog."
     response = pii_annotation_pipeline.run()
-    assert response.text == "Jane Doe works at DataFog.", "Response text should match the request text"
+    assert (
+        response.text == "Jane Doe works at DataFog."
+    ), "Response text should match the request text"
     assert len(response.entities) > 0, "Should return detected entities"
-    assert any("ORG" in entity for entity in response.entities), "Should detect organization entities"
+    assert any(
+        "ORG" in entity for entity in response.entities
+    ), "Should detect organization entities"
```

### Comparing `datafog-3.0.0b6/tests/test_main.py` & `datafog-3.0.1b1/tests/test_main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,62 @@
 # unittest below in comments
 import pytest
+
 from datafog import DataFog, PipelineOperationType
 
+
 @pytest.fixture
 def datafog():
-    return DataFog(operation_type=PipelineOperationType.PARSE_IMAGE, image_processor=True, text_pii_annotation=True)
+    return DataFog(
+        operation_type=PipelineOperationType.PARSE_IMAGE,
+        image_processor=True,
+        text_pii_annotation=True,
+    )
+
 
 def test_process_text(datafog):
     text = "John Smith lives in Wonderland."
     entities = datafog.process_text(text)
     assert len(entities) > 0
-    assert ('John Smith', 'PER') in entities
-    assert ('Wonderland', 'LOC') in entities
+    assert ("John Smith", "PER") in entities
+    assert ("Wonderland", "LOC") in entities
+
 
 def test_process_image(datafog):
     sample_image_path = "tests/test-invoice.png"
     with open(sample_image_path, "rb") as image_file:
         image_data = image_file.read()
     result = datafog.process_image(image_data)
     assert isinstance(result, dict)
-    names = [item['nm'] for sublist in result.values() if isinstance(sublist, list) for item in sublist]
-    unit_prices = [item['price']['unitprice'] for sublist in result.values() if isinstance(sublist, list) for item in sublist if 'unitprice' in item['price']]
-    assert 'MEDICAL BILLING INVOICE' in names
-    assert '12245' in unit_prices
-    assert 'Full Check Up' in names
-    assert 'Ear & Throat Examination' in names
+    names = [
+        item["nm"]
+        for sublist in result.values()
+        if isinstance(sublist, list)
+        for item in sublist
+    ]
+    unit_prices = [
+        item["price"]["unitprice"]
+        for sublist in result.values()
+        if isinstance(sublist, list)
+        for item in sublist
+        if "unitprice" in item["price"]
+    ]
+    assert "MEDICAL BILLING INVOICE" in names
+    assert "12245" in unit_prices
+    assert "Full Check Up" in names
+    assert "Ear & Throat Examination" in names
+
 
 def test_annotate_pii_in_images(datafog):
     sample_image_path = "tests/test-invoice.png"
     with open(sample_image_path, "rb") as image_file:
         image_data = image_file.read()
     annotated_result = datafog.annotate_pii_in_images(image_data)
 
     # Check if 'entities' is added and contains expected PII entity types.
     for sublist in annotated_result.values():
         if isinstance(sublist, list):
             for item in sublist:
-                if 'nm' in item:
-                    print("Item Name:", item['nm'], "Entities:", item.get('entities'))
-                    assert 'entities' in item
+                if "nm" in item:
+                    print("Item Name:", item["nm"], "Entities:", item.get("entities"))
+                    assert "entities" in item
                     # Check for at least one 'ORG' or 'LOC' entity in each item
-
```

