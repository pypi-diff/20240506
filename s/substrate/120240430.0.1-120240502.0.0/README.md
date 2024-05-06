# Comparing `tmp/substrate-120240430.0.1.tar.gz` & `tmp/substrate-120240502.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-120240430.0.1.tar", max compression
+gzip compressed data, was "substrate-120240502.0.0.tar", max compression
```

## Comparing `substrate-120240430.0.1.tar` & `substrate-120240502.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240430.0.1/LICENSE
--rw-r--r--   0        0        0     2675 2024-04-30 17:24:23.830575 substrate-120240430.0.1/README.md
--rw-r--r--   0        0        0     2079 2024-04-30 22:15:29.807673 substrate-120240430.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240430.0.1/substrate/.keep
--rw-r--r--   0        0        0       17 2024-04-30 20:55:50.000000 substrate-120240430.0.1/substrate/GEN_VERSION
--rw-r--r--   0        0        0     2280 2024-04-30 20:55:51.000000 substrate-120240430.0.1/substrate/__init__.py
--rw-r--r--   0        0        0     5758 2024-04-30 17:48:32.046681 substrate-120240430.0.1/substrate/_client.py
--rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240430.0.1/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-04-30 22:12:40.533069 substrate-120240430.0.1/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-04-30 22:12:40.532830 substrate-120240430.0.1/substrate/core/_version.py
--rw-r--r--   0        0        0     1535 2024-04-30 22:12:40.533867 substrate-120240430.0.1/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-04-30 22:12:40.534837 substrate-120240430.0.1/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-04-30 22:12:40.535075 substrate-120240430.0.1/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2697 2024-04-30 22:12:40.535357 substrate-120240430.0.1/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-04-30 22:12:40.534673 substrate-120240430.0.1/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-04-30 22:12:40.533448 substrate-120240430.0.1/substrate/core/coregraph.py
--rw-r--r--   0        0        0     2212 2024-04-30 22:12:40.531322 substrate-120240430.0.1/substrate/core/corenode.py
--rw-r--r--   0        0        0     1227 2024-04-30 22:12:40.534142 substrate-120240430.0.1/substrate/core/future_directive.py
--rw-r--r--   0        0        0      894 2024-04-30 22:12:40.531093 substrate-120240430.0.1/substrate/core/id_generator.py
--rw-r--r--   0        0        0    38268 2024-04-30 22:12:40.531884 substrate-120240430.0.1/substrate/core/models.py
--rw-r--r--   0        0        0     2332 2024-04-30 22:12:40.530804 substrate-120240430.0.1/substrate/core/sb.py
--rw-r--r--   0        0        0    32553 2024-04-19 00:53:25.000000 substrate-120240430.0.1/substrate/dataclass_models.py
--rw-r--r--   0        0        0    49125 2024-04-30 20:55:49.000000 substrate-120240430.0.1/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    45754 2024-04-30 20:55:51.000000 substrate-120240430.0.1/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240430.0.1/substrate/py.typed
--rw-r--r--   0        0        0     2132 2024-04-30 17:24:23.841883 substrate-120240430.0.1/substrate/substrate.py
--rw-r--r--   0        0        0     1015 2024-04-30 17:24:23.842724 substrate-120240430.0.1/substrate/substrate_response.py
--rw-r--r--   0        0        0    38598 2024-04-30 20:55:47.000000 substrate-120240430.0.1/substrate/typeddict_models.py
--rw-r--r--   0        0        0     3312 1970-01-01 00:00:00.000000 substrate-120240430.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240502.0.0/LICENSE
+-rw-r--r--   0        0        0     2715 2024-05-01 20:59:44.017862 substrate-120240502.0.0/README.md
+-rw-r--r--   0        0        0     2079 2024-05-06 18:18:04.851419 substrate-120240502.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240502.0.0/substrate/.keep
+-rw-r--r--   0        0        0       17 2024-05-02 15:36:22.000000 substrate-120240502.0.0/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     2188 2024-05-02 15:36:23.000000 substrate-120240502.0.0/substrate/__init__.py
+-rw-r--r--   0        0        0     5727 2024-05-06 18:16:22.939060 substrate-120240502.0.0/substrate/_client.py
+-rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240502.0.0/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-05-06 18:17:22.557192 substrate-120240502.0.0/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-06 18:17:22.556974 substrate-120240502.0.0/substrate/core/_version.py
+-rw-r--r--   0        0        0     1535 2024-05-06 18:17:22.557750 substrate-120240502.0.0/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:17:22.558969 substrate-120240502.0.0/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-05-06 18:17:22.559173 substrate-120240502.0.0/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2697 2024-05-06 18:17:22.559372 substrate-120240502.0.0/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-05-06 18:17:22.558706 substrate-120240502.0.0/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-05-06 18:17:22.557488 substrate-120240502.0.0/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     2212 2024-05-06 18:17:22.552509 substrate-120240502.0.0/substrate/core/corenode.py
+-rw-r--r--   0        0        0     1587 2024-05-06 18:17:22.557988 substrate-120240502.0.0/substrate/core/future_directive.py
+-rw-r--r--   0        0        0      894 2024-05-06 18:17:22.552230 substrate-120240502.0.0/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    37176 2024-05-06 18:17:22.556197 substrate-120240502.0.0/substrate/core/models.py
+-rw-r--r--   0        0        0     3798 2024-05-06 18:17:22.551865 substrate-120240502.0.0/substrate/core/sb.py
+-rw-r--r--   0        0        0    32553 2024-04-19 00:53:25.000000 substrate-120240502.0.0/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    47757 2024-05-02 15:36:20.000000 substrate-120240502.0.0/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    42949 2024-05-02 15:36:23.000000 substrate-120240502.0.0/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240502.0.0/substrate/py.typed
+-rw-r--r--   0        0        0     2196 2024-05-06 18:16:14.492293 substrate-120240502.0.0/substrate/substrate.py
+-rw-r--r--   0        0        0     1015 2024-04-30 17:24:23.842724 substrate-120240502.0.0/substrate/substrate_response.py
+-rw-r--r--   0        0        0    37584 2024-05-02 15:36:18.000000 substrate-120240502.0.0/substrate/typeddict_models.py
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 substrate-120240502.0.0/PKG-INFO
```

### Comparing `substrate-120240430.0.1/LICENSE` & `substrate-120240502.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-120240430.0.1/README.md` & `substrate-120240502.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: substrate
+Version: 120240502.0.0
+Summary: Substrate Python SDK
+Author: vprtwn
+Author-email: ben@substrate.run
+Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: distro (>=1.8.0)
+Requires-Dist: httpx (>=0.26.0)
+Requires-Dist: networkx (>=3.2.1)
+Requires-Dist: pydantic (>=1.0.0)
+Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
+Description-Content-Type: text/markdown
+
 # ꩜ Substrate Python SDK
 
 [![PyPI version](https://img.shields.io/pypi/v/substrate.svg)](https://pypi.org/project/substrate/)
 
 The Substrate Python SDK is the recommended way to interact with the Substrate API from any Python application.
 
 ## Documentation
@@ -64,10 +83,11 @@
 ```
 
 ## Examples
 
 To run the above example as a notebook, navigate to the `examples/notebooks` directory and run:
 
 ```sh
-make ensure     # install dependencies
-make basic      # run the notebook
+make ensure                         # install dependencies
+poetry run marimo edit basic.py     # run the notebook
 ```
+
```

### Comparing `substrate-120240430.0.1/pyproject.toml` & `substrate-120240502.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "120240430.0.1"
+version = "120240502.0.0"
 description = "Substrate Python SDK"
 readme = "README.md"
 authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
```

### Comparing `substrate-120240430.0.1/substrate/__init__.py` & `substrate-120240502.0.0/substrate/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """
 ꩜ Substrate Python SDK
 
-20240430.20240430
+20240502.20240502
 """
 
 from .nodes import (
     CLIP,
     XTTSV2,
     JinaV2,
-    BigLaMa,
     RunCode,
-    DISISNet,
     FillMask,
     EmbedText,
     EmbedImage,
-    RealESRGAN,
     FetchVectors,
     Firellava13B,
     GenerateJSON,
     GenerateText,
     UpscaleImage,
     DeleteVectors,
     GenerateImage,
@@ -86,17 +83,14 @@
     "TranscribeMedia",
     "GenerateSpeech",
     "XTTSV2",
     "RemoveBackground",
     "FillMask",
     "UpscaleImage",
     "SegmentUnderPoint",
-    "DISISNet",
-    "BigLaMa",
-    "RealESRGAN",
     "SegmentAnything",
     "EmbedText",
     "MultiEmbedText",
     "EmbedImage",
     "MultiEmbedImage",
     "JinaV2",
     "CLIP",
```

### Comparing `substrate-120240430.0.1/substrate/_client.py` & `substrate-120240502.0.0/substrate/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,21 +124,21 @@
     _additional_headers: Dict[str, Any]
 
     def __init__(
         self,
         api_key: str,
         base_url: str,
         backend: str,
+        timeout: float,
         additional_headers: Dict[str, Any] = {},
     ) -> None:
         self._api_key = api_key
         self._base_url = base_url
         self._backend = backend
         self._additional_headers = additional_headers
-        timeout = httpx.Timeout(60.0)  # default is 5s
         self._client = httpx.Client(timeout=timeout)
         self._async_client = httpx.AsyncClient(timeout=timeout)
         self._version = __version__
 
     @property
     def user_agent(self) -> str:
         return f"{self.__class__.__name__}/Python {self._version}"
```

### Comparing `substrate-120240430.0.1/substrate/core/base_future.py` & `substrate-120240502.0.0/substrate/core/base_future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240430.0.1/substrate/core/client/find_futures_client.py` & `substrate-120240502.0.0/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240430.0.1/substrate/core/client/future.py` & `substrate-120240502.0.0/substrate/core/client/future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240430.0.1/substrate/core/client/graph.py` & `substrate-120240502.0.0/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240430.0.1/substrate/core/coregraph.py` & `substrate-120240502.0.0/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240430.0.1/substrate/core/corenode.py` & `substrate-120240502.0.0/substrate/core/corenode.py`

 * *Files identical despite different names*

### Comparing `substrate-120240430.0.1/substrate/core/future_directive.py` & `substrate-120240502.0.0/substrate/core/future_directive.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,15 @@
     List,
     Union,
     Literal,
     Optional,
 )
 from dataclasses import asdict, dataclass
 
-OpType = Literal["trace", "string-concat", "jq"]
-ConcatDirection = Literal["left", "right"]
+OpType = Literal["trace", "string-concat", "jq", "short-circuit"]
 
 
 class BaseDirective(ABC):
     type: OpType
 
     def to_dict(self) -> Dict:
         # noinspection PyDataclass
@@ -47,14 +46,33 @@
 @dataclass
 class JQDirective(BaseDirective):
     target: JQDirectiveTarget
     query: str
     type: Literal["jq"] = "jq"
 
 
+@dataclass
+class ShortCircuitConditionTarget:
+    future_id: Optional[str]
+    val: Optional[bool]
+
+
+@dataclass
+class ShortCircuitInputTarget:
+    future_id: Optional[str]
+    val: Optional[bool]
+
+
+@dataclass
+class ShortCircuitDirective(BaseDirective):
+    condition: ShortCircuitConditionTarget
+    input: ShortCircuitInputTarget
+    type: Literal["short-circuit"] = "short-circuit"
+
+
 TraceType = Literal["attr", "item"]
 
 
 @dataclass
 class TraceOperation:
     future_id: Optional[str]
     key: Optional[Union[str, int]]
```

### Comparing `substrate-120240430.0.1/substrate/core/id_generator.py` & `substrate-120240502.0.0/substrate/core/id_generator.py`

 * *Files identical despite different names*

### Comparing `substrate-120240430.0.1/substrate/core/models.py` & `substrate-120240502.0.0/substrate/core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,18 +163,14 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
-    """
-    Selected node.
-    """
 
 
 class BatchGenerateTextOut(BaseModel):
     outputs: List[GenerateTextOut]
     """
     Batch outputs.
     """
@@ -227,18 +223,14 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
-    """
-    Selected node.
-    """
 
 
 class BatchGenerateJSONOut(BaseModel):
     outputs: List[GenerateJSONOut]
     """
     Batch outputs.
     """
@@ -401,18 +393,14 @@
     """
     Image prompts.
     """
     max_tokens: int = 800
     """
     Maximum number of tokens to generate.
     """
-    node: Literal["Firellava13B"] = "Firellava13B"
-    """
-    Selected node.
-    """
 
 
 class GenerateTextVisionOut(BaseModel):
     text: str
     """
     Text response.
     """
@@ -445,18 +433,14 @@
     """
     Text prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
-    """
-    Selected node.
-    """
 
 
 class GenerateImageOut(BaseModel):
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -471,18 +455,14 @@
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
-    """
-    Selected node.
-    """
 
 
 class MultiGenerateImageOut(BaseModel):
     outputs: List[GenerateImageOut]
     """
     Generated images.
     """
@@ -688,18 +668,14 @@
     """
     Mask image that controls which pixels are inpainted. If unset, the entire image is edited (image-to-image).
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
-    """
-    Selected node.
-    """
 
 
 class GenerativeEditImageOut(BaseModel):
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -722,18 +698,14 @@
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
-    """
-    Selected node.
-    """
 
 
 class MultiGenerativeEditImageOut(BaseModel):
     outputs: List[GenerativeEditImageOut]
     """
     Generated images.
     """
@@ -824,18 +796,14 @@
     """
     Mask image that controls which pixels are inpainted.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["BigLaMa"] = "BigLaMa"
-    """
-    Selected node.
-    """
 
 
 class FillMaskOut(BaseModel):
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -876,18 +844,14 @@
     """
     Hex value background color. Transparent if unset.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["DISISNet"] = "DISISNet"
-    """
-    Selected node.
-    """
 
 
 class RemoveBackgroundOut(BaseModel):
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -916,18 +880,14 @@
     """
     Input image.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["RealESRGAN"] = "RealESRGAN"
-    """
-    Selected node.
-    """
 
 
 class UpscaleImageOut(BaseModel):
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -960,18 +920,14 @@
     """
     Point prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["SegmentAnything"] = "SegmentAnything"
-    """
-    Selected node.
-    """
 
 
 class SegmentUnderPointOut(BaseModel):
     mask_image_uri: str
     """
     Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -1107,18 +1063,14 @@
     """
     Input text.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
     """
-    node: Literal["XTTSV2"] = "XTTSV2"
-    """
-    Selected node.
-    """
 
 
 class GenerateSpeechOut(BaseModel):
     audio_uri: str
     """
     Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
     """
```

### Comparing `substrate-120240430.0.1/substrate/core/sb.py` & `substrate-120240502.0.0/substrate/core/sb.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,18 +6,22 @@
 from .client.future import Future
 from .future_directive import (
     JQDirective,
     JQTargetType,
     ConcatDirective,
     JQDirectiveTarget,
     ConcatDirectiveItem,
+    ShortCircuitDirective,
+    ShortCircuitInputTarget,
+    ShortCircuitConditionTarget,
 )
 
 StringConcatable = Union[str, None, Future]
 JQCompatible = Union[Future, JQTargetType]
+ConditionCompatible = Union[Future, bool]
 
 
 class sb:
     """
     Utilities for working with future references.
     """
 
@@ -60,7 +64,33 @@
         future_id = target.id if isinstance(target, Future) else None
         val = target if not isinstance(target, Future) else None
         directive = JQDirective(target=JQDirectiveTarget(future_id=future_id, val=val), query=query)
         result = Future(directive=directive)
         if isinstance(target, Future):
             result.FutureG.add_edge(target, result)
         return result  # type: ignore
+
+    @classmethod
+    def when(cls, condition: ConditionCompatible, input: Union[Future, Any]) -> Any:
+        """
+        Short-circuiting conditional edge.
+        Only evaluate the subsequent node with the provided input if the condition is true.
+        :param condition: A boolean or a future reference to a boolean.
+        :param input: A future reference to the output of another node.
+        :return: A future reference to the short-circuiting `when` operator.
+        """
+        c_future_id = condition.id if isinstance(condition, Future) else None
+        c_val = condition if not isinstance(condition, Future) else None
+        i_future_id = input.id if isinstance(input, Future) else None
+        i_val = input if not isinstance(input, Future) else None
+        directive = ShortCircuitDirective(
+            condition=ShortCircuitConditionTarget(future_id=c_future_id, val=c_val),
+            input=ShortCircuitInputTarget(future_id=i_future_id, val=i_val),
+        )
+        result = Future(directive=directive)
+        # add edge to the condition future
+        if isinstance(condition, Future):
+            result.FutureG.add_edge(condition, result)
+        # add edge to the input future
+        if isinstance(input, Future):
+            result.FutureG.add_edge(input, result)
+        return result  # type: ignore
```

### Comparing `substrate-120240430.0.1/substrate/dataclass_models.py` & `substrate-120240502.0.0/substrate/dataclass_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240430.0.1/substrate/future_dataclass_models.py` & `substrate-120240502.0.0/substrate/future_dataclass_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,19 +241,14 @@
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
-    """
-    (Future reference)
-    Selected node.
-    """
 
 
 @dataclass
 class FutureBatchGenerateTextOut:
     """
     (Future reference)
     """
@@ -338,19 +333,14 @@
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
-    """
-    (Future reference)
-    Selected node.
-    """
 
 
 @dataclass
 class FutureBatchGenerateJSONOut:
     """
     (Future reference)
     """
@@ -615,19 +605,14 @@
     Image prompts.
     """
     max_tokens: int = 800
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Literal["Firellava13B"] = "Firellava13B"
-    """
-    (Future reference)
-    Selected node.
-    """
 
 
 @dataclass
 class FutureGenerateTextVisionOut:
     """
     (Future reference)
     """
@@ -687,19 +672,14 @@
     Text prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
-    """
-    (Future reference)
-    Selected node.
-    """
 
 
 @dataclass
 class FutureGenerateImageOut:
     """
     (Future reference)
     """
@@ -728,19 +708,14 @@
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
-    """
-    (Future reference)
-    Selected node.
-    """
 
 
 @dataclass
 class FutureMultiGenerateImageOut:
     """
     (Future reference)
     """
@@ -1046,19 +1021,14 @@
     Mask image that controls which pixels are inpainted. If unset, the entire image is edited (image-to-image).
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
-    """
-    (Future reference)
-    Selected node.
-    """
 
 
 @dataclass
 class FutureGenerativeEditImageOut:
     """
     (Future reference)
     """
@@ -1097,19 +1067,14 @@
     Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
-    """
-    (Future reference)
-    Selected node.
-    """
 
 
 @dataclass
 class FutureMultiGenerativeEditImageOut:
     """
     (Future reference)
     """
@@ -1250,19 +1215,14 @@
     Mask image that controls which pixels are inpainted.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["BigLaMa"] = "BigLaMa"
-    """
-    (Future reference)
-    Selected node.
-    """
 
 
 @dataclass
 class FutureFillMaskOut:
     """
     (Future reference)
     """
@@ -1332,19 +1292,14 @@
     Hex value background color. Transparent if unset.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["DISISNet"] = "DISISNet"
-    """
-    (Future reference)
-    Selected node.
-    """
 
 
 @dataclass
 class FutureRemoveBackgroundOut:
     """
     (Future reference)
     """
@@ -1399,19 +1354,14 @@
     Input image.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["RealESRGAN"] = "RealESRGAN"
-    """
-    (Future reference)
-    Selected node.
-    """
 
 
 @dataclass
 class FutureUpscaleImageOut:
     """
     (Future reference)
     """
@@ -1471,19 +1421,14 @@
     Point prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: Literal["SegmentAnything"] = "SegmentAnything"
-    """
-    (Future reference)
-    Selected node.
-    """
 
 
 @dataclass
 class FutureSegmentUnderPointOut:
     """
     (Future reference)
     """
@@ -1693,19 +1638,14 @@
     Input text.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
     """
-    node: Literal["XTTSV2"] = "XTTSV2"
-    """
-    (Future reference)
-    Selected node.
-    """
 
 
 @dataclass
 class FutureGenerateSpeechOut:
     """
     (Future reference)
     """
```

### Comparing `substrate-120240430.0.1/substrate/nodes.py` & `substrate-120240502.0.0/substrate/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """
 ꩜ Substrate
 @GENERATED FILE
-20240430.20240430
+20240502.20240502
 """
 
 from .core.models import (
     CLIPOut,
     JinaV2Out,
     XTTSV2Out,
-    BigLaMaOut,
     RunCodeOut,
-    DISISNetOut,
     FillMaskOut,
     EmbedTextOut,
     EmbedImageOut,
-    RealESRGANOut,
     FetchVectorsOut,
     Firellava13BOut,
     GenerateJSONOut,
     GenerateTextOut,
     UpscaleImageOut,
     DeleteVectorsOut,
     GenerateImageOut,
@@ -53,21 +50,18 @@
     StableDiffusionXLControlNetOut,
 )
 from .core.corenode import CoreNode
 from .typeddict_models import (
     CLIPIn,
     JinaV2In,
     XTTSV2In,
-    BigLaMaIn,
     RunCodeIn,
-    DISISNetIn,
     FillMaskIn,
     EmbedTextIn,
     EmbedImageIn,
-    RealESRGANIn,
     FetchVectorsIn,
     Firellava13BIn,
     GenerateJSONIn,
     GenerateTextIn,
     UpscaleImageIn,
     DeleteVectorsIn,
     GenerateImageIn,
@@ -101,21 +95,18 @@
     StableDiffusionXLLightningIn,
     StableDiffusionXLControlNetIn,
 )
 from .future_dataclass_models import (
     FutureCLIPOut,
     FutureJinaV2Out,
     FutureXTTSV2Out,
-    FutureBigLaMaOut,
     FutureRunCodeOut,
-    FutureDISISNetOut,
     FutureFillMaskOut,
     FutureEmbedTextOut,
     FutureEmbedImageOut,
-    FutureRealESRGANOut,
     FutureFetchVectorsOut,
     FutureFirellava13BOut,
     FutureGenerateJSONOut,
     FutureGenerateTextOut,
     FutureUpscaleImageOut,
     FutureDeleteVectorsOut,
     FutureGenerateImageOut,
@@ -246,15 +237,15 @@
     Generate text for multiple prompts in batch using a language model.
 
     https://substrate.run/library#BatchGenerateText
     """
 
     def __init__(self, args: BatchGenerateTextIn, hide: bool = False):
         """
-        Input arguments: `prompts`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
+        Input arguments: `prompts`, `temperature` (optional), `max_tokens` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#BatchGenerateText
         """
         super().__init__(hide=hide, out_type=BatchGenerateTextOut, **args)
         self.node = "BatchGenerateText"
@@ -276,15 +267,15 @@
     Generate JSON for multiple prompts in batch using a language model.
 
     https://substrate.run/library#BatchGenerateJSON
     """
 
     def __init__(self, args: BatchGenerateJSONIn, hide: bool = False):
         """
-        Input arguments: `prompts`, `json_schema`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
+        Input arguments: `prompts`, `json_schema`, `temperature` (optional), `max_tokens` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#BatchGenerateJSON
         """
         super().__init__(hide=hide, out_type=BatchGenerateJSONOut, **args)
         self.node = "BatchGenerateJSON"
@@ -366,15 +357,15 @@
     Generate text with image input.
 
     https://substrate.run/library#GenerateTextVision
     """
 
     def __init__(self, args: GenerateTextVisionIn, hide: bool = False):
         """
-        Input arguments: `prompt`, `image_uris`, `max_tokens` (optional), `node` (optional)
+        Input arguments: `prompt`, `image_uris`, `max_tokens` (optional)
 
         Output fields: `future.text`
 
         https://substrate.run/library#GenerateTextVision
         """
         super().__init__(hide=hide, out_type=GenerateTextVisionOut, **args)
         self.node = "GenerateTextVision"
@@ -546,15 +537,15 @@
     Generate an image.
 
     https://substrate.run/library#GenerateImage
     """
 
     def __init__(self, args: GenerateImageIn, hide: bool = False):
         """
-        Input arguments: `prompt`, `store` (optional), `node` (optional)
+        Input arguments: `prompt`, `store` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerateImage
         """
         super().__init__(hide=hide, out_type=GenerateImageOut, **args)
         self.node = "GenerateImage"
@@ -576,15 +567,15 @@
     Generate multiple images.
 
     https://substrate.run/library#MultiGenerateImage
     """
 
     def __init__(self, args: MultiGenerateImageIn, hide: bool = False):
         """
-        Input arguments: `prompt`, `num_images`, `store` (optional), `node` (optional)
+        Input arguments: `prompt`, `num_images`, `store` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateImage
         """
         super().__init__(hide=hide, out_type=MultiGenerateImageOut, **args)
         self.node = "MultiGenerateImage"
@@ -606,15 +597,15 @@
     Edit an image using image generation.
 
     https://substrate.run/library#GenerativeEditImage
     """
 
     def __init__(self, args: GenerativeEditImageIn, hide: bool = False):
         """
-        Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `store` (optional), `node` (optional)
+        Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `store` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerativeEditImage
         """
         super().__init__(hide=hide, out_type=GenerativeEditImageOut, **args)
         self.node = "GenerativeEditImage"
@@ -636,15 +627,15 @@
     Edit multiple images using image generation.
 
     https://substrate.run/library#MultiGenerativeEditImage
     """
 
     def __init__(self, args: MultiGenerativeEditImageIn, hide: bool = False):
         """
-        Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `num_images`, `store` (optional), `node` (optional)
+        Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `num_images`, `store` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerativeEditImage
         """
         super().__init__(hide=hide, out_type=MultiGenerativeEditImageOut, **args)
         self.node = "MultiGenerativeEditImage"
@@ -846,15 +837,15 @@
     Generate speech from text.
 
     https://substrate.run/library#GenerateSpeech
     """
 
     def __init__(self, args: GenerateSpeechIn, hide: bool = False):
         """
-        Input arguments: `text`, `store` (optional), `node` (optional)
+        Input arguments: `text`, `store` (optional)
 
         Output fields: `future.audio_uri`
 
         https://substrate.run/library#GenerateSpeech
         """
         super().__init__(hide=hide, out_type=GenerateSpeechOut, **args)
         self.node = "GenerateSpeech"
@@ -906,15 +897,15 @@
     Remove the background from an image, with the option to return the foreground as a mask.
 
     https://substrate.run/library#RemoveBackground
     """
 
     def __init__(self, args: RemoveBackgroundIn, hide: bool = False):
         """
-        Input arguments: `image_uri`, `return_mask` (optional), `background_color` (optional), `store` (optional), `node` (optional)
+        Input arguments: `image_uri`, `return_mask` (optional), `background_color` (optional), `store` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#RemoveBackground
         """
         super().__init__(hide=hide, out_type=RemoveBackgroundOut, **args)
         self.node = "RemoveBackground"
@@ -936,15 +927,15 @@
     Fill (inpaint) part of an image, e.g. to 'remove' an object.
 
     https://substrate.run/library#FillMask
     """
 
     def __init__(self, args: FillMaskIn, hide: bool = False):
         """
-        Input arguments: `image_uri`, `mask_image_uri`, `store` (optional), `node` (optional)
+        Input arguments: `image_uri`, `mask_image_uri`, `store` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#FillMask
         """
         super().__init__(hide=hide, out_type=FillMaskOut, **args)
         self.node = "FillMask"
@@ -966,15 +957,15 @@
     Upscale an image.
 
     https://substrate.run/library#UpscaleImage
     """
 
     def __init__(self, args: UpscaleImageIn, hide: bool = False):
         """
-        Input arguments: `image_uri`, `store` (optional), `node` (optional)
+        Input arguments: `image_uri`, `store` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#UpscaleImage
         """
         super().__init__(hide=hide, out_type=UpscaleImageOut, **args)
         self.node = "UpscaleImage"
@@ -996,15 +987,15 @@
     Segment an image under a point and return the segment.
 
     https://substrate.run/library#SegmentUnderPoint
     """
 
     def __init__(self, args: SegmentUnderPointIn, hide: bool = False):
         """
-        Input arguments: `image_uri`, `point`, `store` (optional), `node` (optional)
+        Input arguments: `image_uri`, `point`, `store` (optional)
 
         Output fields: `future.mask_image_uri`
 
         https://substrate.run/library#SegmentUnderPoint
         """
         super().__init__(hide=hide, out_type=SegmentUnderPointOut, **args)
         self.node = "SegmentUnderPoint"
@@ -1017,104 +1008,14 @@
         Output fields: `future.mask_image_uri`
 
         https://substrate.run/library#SegmentUnderPoint
         """
         return super().future  # type: ignore
 
 
-class DISISNet(CoreNode[DISISNetOut]):
-    """
-    Segment image foreground using [DIS IS-Net](https://github.com/xuebinqin/DIS).
-
-    https://substrate.run/library#DISISNet
-    """
-
-    def __init__(self, args: DISISNetIn, hide: bool = False):
-        """
-        Input arguments: `image_uri`, `store` (optional)
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#DISISNet
-        """
-        super().__init__(hide=hide, out_type=DISISNetOut, **args)
-        self.node = "DISISNet"
-
-    @property
-    def future(self) -> FutureDISISNetOut:  # type: ignore
-        """
-        Future reference to this node's output.
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#DISISNet
-        """
-        return super().future  # type: ignore
-
-
-class BigLaMa(CoreNode[BigLaMaOut]):
-    """
-    Inpaint a mask using [LaMa](https://github.com/advimman/lama).
-
-    https://substrate.run/library#BigLaMa
-    """
-
-    def __init__(self, args: BigLaMaIn, hide: bool = False):
-        """
-        Input arguments: `image_uri`, `mask_image_uri`, `store` (optional)
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#BigLaMa
-        """
-        super().__init__(hide=hide, out_type=BigLaMaOut, **args)
-        self.node = "BigLaMa"
-
-    @property
-    def future(self) -> FutureBigLaMaOut:  # type: ignore
-        """
-        Future reference to this node's output.
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#BigLaMa
-        """
-        return super().future  # type: ignore
-
-
-class RealESRGAN(CoreNode[RealESRGANOut]):
-    """
-    Upscale an image using [RealESRGAN](https://github.com/xinntao/Real-ESRGAN).
-
-    https://substrate.run/library#RealESRGAN
-    """
-
-    def __init__(self, args: RealESRGANIn, hide: bool = False):
-        """
-        Input arguments: `image_uri`, `store` (optional)
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#RealESRGAN
-        """
-        super().__init__(hide=hide, out_type=RealESRGANOut, **args)
-        self.node = "RealESRGAN"
-
-    @property
-    def future(self) -> FutureRealESRGANOut:  # type: ignore
-        """
-        Future reference to this node's output.
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#RealESRGAN
-        """
-        return super().future  # type: ignore
-
-
 class SegmentAnything(CoreNode[SegmentAnythingOut]):
     """
     Segment an image using [SegmentAnything](https://github.com/facebookresearch/segment-anything).
 
     https://substrate.run/library#SegmentAnything
     """
```

### Comparing `substrate-120240430.0.1/substrate/substrate.py` & `substrate-120240502.0.0/substrate/substrate.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,24 +15,26 @@
     """
 
     def __init__(
         self,
         api_key: str,
         base_url: str = "https://api.substrate.run",
         backend: str = "v1",
+        timeout: float = 60 * 5.0,
         additional_headers: Dict[str, Any] = {},
     ):
         """
         Initialize the Substrate SDK.
         """
         self.api_key = api_key
         self._client = APIClient(
             api_key=api_key,
             base_url=base_url,
             backend=backend,
+            timeout=timeout,
             additional_headers=additional_headers,
         )
 
     def run(self, *nodes: CoreNode) -> SubstrateResponse:
         """
         Run the given nodes.
         """
```

### Comparing `substrate-120240430.0.1/substrate/substrate_response.py` & `substrate-120240502.0.0/substrate/substrate_response.py`

 * *Files identical despite different names*

### Comparing `substrate-120240430.0.1/substrate/typeddict_models.py` & `substrate-120240502.0.0/substrate/typeddict_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -165,18 +165,14 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     Maximum number of tokens to generate.
     """
-    node: NotRequired[Literal["Mistral7BInstruct"]]
-    """
-    Selected node.
-    """
 
 
 class BatchGenerateTextOut(TypedDict):
     outputs: NotRequired[List[GenerateTextOut]]
     """
     Batch outputs.
     """
@@ -229,18 +225,14 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     Maximum number of tokens to generate.
     """
-    node: NotRequired[Literal["Mistral7BInstruct"]]
-    """
-    Selected node.
-    """
 
 
 class BatchGenerateJSONOut(TypedDict):
     outputs: NotRequired[List[GenerateJSONOut]]
     """
     Batch outputs.
     """
@@ -403,18 +395,14 @@
     """
     Image prompts.
     """
     max_tokens: NotRequired[int]
     """
     Maximum number of tokens to generate.
     """
-    node: NotRequired[Literal["Firellava13B"]]
-    """
-    Selected node.
-    """
 
 
 class GenerateTextVisionOut(TypedDict):
     text: NotRequired[str]
     """
     Text response.
     """
@@ -447,18 +435,14 @@
     """
     Text prompt.
     """
     store: NotRequired[str]
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: NotRequired[Literal["StableDiffusionXL"]]
-    """
-    Selected node.
-    """
 
 
 class GenerateImageOut(TypedDict):
     image_uri: NotRequired[str]
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -473,18 +457,14 @@
     """
     Number of images to generate.
     """
     store: NotRequired[str]
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: NotRequired[Literal["StableDiffusionXL"]]
-    """
-    Selected node.
-    """
 
 
 class MultiGenerateImageOut(TypedDict):
     outputs: NotRequired[List[GenerateImageOut]]
     """
     Generated images.
     """
@@ -690,18 +670,14 @@
     """
     Mask image that controls which pixels are inpainted. If unset, the entire image is edited (image-to-image).
     """
     store: NotRequired[str]
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: NotRequired[Literal["StableDiffusionXLInpaint"]]
-    """
-    Selected node.
-    """
 
 
 class GenerativeEditImageOut(TypedDict):
     image_uri: NotRequired[str]
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -724,18 +700,14 @@
     """
     Number of images to generate.
     """
     store: NotRequired[str]
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: NotRequired[Literal["StableDiffusionXLInpaint"]]
-    """
-    Selected node.
-    """
 
 
 class MultiGenerativeEditImageOut(TypedDict):
     outputs: NotRequired[List[GenerativeEditImageOut]]
     """
     Generated images.
     """
@@ -826,18 +798,14 @@
     """
     Mask image that controls which pixels are inpainted.
     """
     store: NotRequired[str]
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: NotRequired[Literal["BigLaMa"]]
-    """
-    Selected node.
-    """
 
 
 class FillMaskOut(TypedDict):
     image_uri: NotRequired[str]
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -878,18 +846,14 @@
     """
     Hex value background color. Transparent if unset.
     """
     store: NotRequired[str]
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: NotRequired[Literal["DISISNet"]]
-    """
-    Selected node.
-    """
 
 
 class RemoveBackgroundOut(TypedDict):
     image_uri: NotRequired[str]
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -918,18 +882,14 @@
     """
     Input image.
     """
     store: NotRequired[str]
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: NotRequired[Literal["RealESRGAN"]]
-    """
-    Selected node.
-    """
 
 
 class UpscaleImageOut(TypedDict):
     image_uri: NotRequired[str]
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -962,18 +922,14 @@
     """
     Point prompt.
     """
     store: NotRequired[str]
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
-    node: NotRequired[Literal["SegmentAnything"]]
-    """
-    Selected node.
-    """
 
 
 class SegmentUnderPointOut(TypedDict):
     mask_image_uri: NotRequired[str]
     """
     Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -1109,18 +1065,14 @@
     """
     Input text.
     """
     store: NotRequired[str]
     """
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
     """
-    node: NotRequired[Literal["XTTSV2"]]
-    """
-    Selected node.
-    """
 
 
 class GenerateSpeechOut(TypedDict):
     audio_uri: NotRequired[str]
     """
     Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
     """
```

