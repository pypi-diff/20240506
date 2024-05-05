# Comparing `tmp/function_sampler-0.1.3.tar.gz` & `tmp/function_sampler-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function_sampler-0.1.3.tar", max compression
+gzip compressed data, was "function_sampler-0.1.6.tar", max compression
```

## Comparing `function_sampler-0.1.3.tar` & `function_sampler-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0    11357 2024-03-09 04:12:23.354920 function_sampler-0.1.3/LICENSE
--rw-r--r--   0        0        0     5383 2024-03-09 04:54:21.915046 function_sampler-0.1.3/README.md
--rw-r--r--   0        0        0      398 2024-03-09 03:49:39.346851 function_sampler-0.1.3/function_sampler/__init__.py
--rw-r--r--   0        0        0     1132 2024-03-09 03:48:44.094848 function_sampler-0.1.3/function_sampler/cache.py
--rw-r--r--   0        0        0       77 2024-03-07 01:00:58.583010 function_sampler-0.1.3/function_sampler/config/__init__.py
--rw-r--r--   0        0        0      592 2024-03-09 04:11:27.642917 function_sampler-0.1.3/function_sampler/config/config.py
--rw-r--r--   0        0        0     5086 2024-03-04 18:41:02.228385 function_sampler-0.1.3/function_sampler/config/default_map.json
--rw-r--r--   0        0        0     2956 2024-03-07 01:00:58.587010 function_sampler-0.1.3/function_sampler/config/token_mapper.py
--rw-r--r--   0        0        0     3825 2024-03-07 01:00:58.583010 function_sampler-0.1.3/function_sampler/config/utils.py
--rw-r--r--   0        0        0      111 2024-03-06 14:15:52.151759 function_sampler-0.1.3/function_sampler/fsm/__init__.py
--rw-r--r--   0        0        0     6064 2024-03-09 04:53:59.335045 function_sampler-0.1.3/function_sampler/fsm/fsm.py
--rw-r--r--   0        0        0    18590 2024-03-07 01:00:58.587010 function_sampler-0.1.3/function_sampler/fsm/regex.py
--rw-r--r--   0        0        0     3287 2024-03-06 01:06:09.888412 function_sampler-0.1.3/function_sampler/fsm/tokenizer_fsm_patch.py
--rw-r--r--   0        0        0    14619 2024-03-09 03:48:44.098848 function_sampler-0.1.3/function_sampler/json.py
--rw-r--r--   0        0        0      330 2024-03-07 01:00:58.587010 function_sampler-0.1.3/function_sampler/logger.py
--rw-r--r--   0        0        0     2640 2024-03-07 03:58:09.031871 function_sampler-0.1.3/function_sampler/regex_constants.py
--rw-r--r--   0        0        0    13174 2024-03-09 03:48:44.098848 function_sampler-0.1.3/function_sampler/sampler.py
--rw-r--r--   0        0        0    14802 2024-03-10 01:24:28.300360 function_sampler-0.1.3/function_sampler/ts_prompt.py
--rw-r--r--   0        0        0     5636 2024-03-09 03:48:44.094848 function_sampler-0.1.3/function_sampler/utils.py
--rw-r--r--   0        0        0      631 2024-03-10 01:49:02.184289 function_sampler-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6264 1970-01-01 00:00:00.000000 function_sampler-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-05 23:25:49.696722 function_sampler-0.1.6/LICENSE
+-rw-r--r--   0        0        0     5572 2024-05-05 23:25:49.696722 function_sampler-0.1.6/README.md
+-rw-r--r--   0        0        0      454 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/__init__.py
+-rw-r--r--   0        0        0     1132 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/cache.py
+-rw-r--r--   0        0        0      126 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/config/__init__.py
+-rw-r--r--   0        0        0      633 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/config/config.py
+-rw-r--r--   0        0        0     3065 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/config/token_mapper.py
+-rw-r--r--   0        0        0     3825 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/config/utils.py
+-rw-r--r--   0        0        0      298 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/fsm/__init__.py
+-rw-r--r--   0        0        0     7015 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/fsm/fsm_utils/src/lazy_index.rs
+-rw-r--r--   0        0        0     1335 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/fsm/fsm_utils/src/lib.rs
+-rw-r--r--   0        0        0    11055 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/fsm/fsm_utils/src/tokenizer_index.rs
+-rw-r--r--   0        0        0    17640 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/fsm/fsm_utils/src/types.rs
+-rw-r--r--   0        0        0     7297 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/fsm/regex.py
+-rw-r--r--   0        0        0     3434 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/fsm/tokenizer_fsm_patch.py
+-rw-r--r--   0        0        0      658 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/fsm/utils.py
+-rw-r--r--   0        0        0    14621 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/json.py
+-rw-r--r--   0        0        0      330 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/logger.py
+-rw-r--r--   0        0        0     2640 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/regex_constants.py
+-rw-r--r--   0        0        0    15065 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/sampler.py
+-rw-r--r--   0        0        0     5675 2024-05-05 23:25:49.696722 function_sampler-0.1.6/function_sampler/utils.py
+-rw-r--r--   0        0        0     1128 2024-05-05 23:25:49.696722 function_sampler-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6758 1970-01-01 00:00:00.000000 function_sampler-0.1.6/PKG-INFO
```

### Comparing `function_sampler-0.1.3/LICENSE` & `function_sampler-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `function_sampler-0.1.3/README.md` & `function_sampler-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 # Use the model for generation
 # only need to tell it how to call the function if it is not explicitly trained for it.
 input_text = "What is the weather today in paris? respond with the word '<function>' to call the weather API."
 input_ids = tokenizer.encode(input_text, return_tensors="pt")
 output = model.generate(input_ids, max_length=200, logits_processor=[sampler])
 generated_text = tokenizer.decode(output[0])
 print(generated_text)
+# <function>  {"name": "get_reservation", "arguments": {"restaurant_name": "Maggiano's", "reservation_time": 18:00:00, "party_size": 6, "contact_number": 1234567890}} </function><|im_end|>
 ```
 
 In this example, we create an instance of the `ToolCallSampler` with the specified functions and configuration. We then attach the sampler to the model's `logits_processor` attribute. This ensures that the sampler is applied during the generation process.
 
 Finally, we use the model to generate text based on the input prompt, which includes the opening function token. The generated text will contain a valid function call adhering to the predefined schema.
 
 For more detailed usage and examples, please refer to the demo notebook provided with the library.
```

### Comparing `function_sampler-0.1.3/function_sampler/cache.py` & `function_sampler-0.1.6/function_sampler/cache.py`

 * *Files identical despite different names*

### Comparing `function_sampler-0.1.3/function_sampler/config/config.py` & `function_sampler-0.1.6/function_sampler/config/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pydantic import BaseModel, Field
-from typing import List, Dict, Optional
+from typing import Optional
 from .token_mapper import TokenMap
 
 
 class ToolCallSamplerConfig(BaseModel):
     open_func_token: Optional[str] = None
     close_func_token: Optional[str] = None
+    generate_close_func_token: Optional[bool] = True
     json_tokens: Optional[TokenMap] = None
     vocab_size: Optional[int]
     end_on_function_call: Optional[bool] = True
     top_p: Optional[float] = Field(None, ge=0, le=1)
     temperature: Optional[float] = Field(None, ge=0, le=2)
     top_k: Optional[float] = Field(None, ge=0, le=1)
     repetition_penalty: Optional[float] = Field(None, ge=0, le=2)
```

### Comparing `function_sampler-0.1.3/function_sampler/config/token_mapper.py` & `function_sampler-0.1.6/function_sampler/config/token_mapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,18 @@
-from pydantic import BaseModel, Field, ValidationError
+from pydantic import BaseModel, ValidationError
 from typing import List
 from transformers import PreTrainedTokenizer
 import json
-from .utils import *
+from .utils import (
+    calc_fn_tokens,
+    find_variant_tokens,
+    find_tokens_with_char,
+    get_int_tokens,
+    get_float_tokens,
+)
 # Ensure the necessary token finding functions are imported or defined here
 
 
 class TokenMap(BaseModel):
     """
     Default token mappings for Mistral, Mixtral, and derivatives.
     """
```

### Comparing `function_sampler-0.1.3/function_sampler/config/utils.py` & `function_sampler-0.1.6/function_sampler/config/utils.py`

 * *Files identical despite different names*

### Comparing `function_sampler-0.1.3/function_sampler/fsm/tokenizer_fsm_patch.py` & `function_sampler-0.1.6/function_sampler/fsm/tokenizer_fsm_patch.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 class Tokenizer(Protocol, Hashable):
     eos_token: str
     eos_token_id: int
     pad_token_id: int
     vocabulary: Dict[str, int]
     special_tokens: Set[int]
+    
 
     @abstractmethod
     def encode(
         self, prompt: Union[str, List[str]]
     ) -> Tuple[NDArray[np.int64], NDArray[np.int64]]:
         """Translate the input prompts into NumPy arrays of token ids and attention mask."""
         ...
@@ -37,48 +38,52 @@
         represented by the special characted `Ġ`. This prevents matching a raw
         token that includes `Ġ` with a string.
 
         """
         ...
 
 
+SPIECE_UNDERLINE = "\u2581"
+
+
 class TransformerTokenizer(Tokenizer):
     """Represents a tokenizer for models in the `transformers` library."""
 
     def __init__(self, tokenizer: "PreTrainedTokenizer", **kwargs):
         self.tokenizer = tokenizer
+        self.hash = None
         self.eos_token_id = self.tokenizer.eos_token_id
         self.eos_token = self.tokenizer.eos_token
 
         if not self.tokenizer.pad_token_id:
             self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
             self.pad_token_id = self.eos_token_id
         else:
             self.pad_token_id = self.tokenizer.pad_token_id
             self.pad_token = self.tokenizer.pad_token
 
         self.special_tokens = set(self.tokenizer.all_special_tokens)
 
         self.vocabulary = self.tokenizer.get_vocab()
 
+        self.__hash__()
+
     def encode(
         self, prompt: Union[str, List[str]], **kwargs
     ) -> Tuple[torch.LongTensor, torch.LongTensor]:
         kwargs["padding"] = True
         kwargs["return_tensors"] = "pt"
         output = self.tokenizer(prompt, **kwargs)
         return output["input_ids"], output["attention_mask"]
 
     def decode(self, token_ids: torch.LongTensor) -> List[str]:
         text = self.tokenizer.batch_decode(token_ids, skip_special_tokens=True)
         return text
 
     def convert_token_to_string(self, token: str) -> str:
-        from transformers.file_utils import SPIECE_UNDERLINE
-
         string = self.tokenizer.convert_tokens_to_string([token])
 
         # A hack to handle missing spaces to HF's Llama tokenizers
         if token.startswith(SPIECE_UNDERLINE) or token == "<0x20>":
             return " " + string
 
         return string
@@ -91,9 +96,13 @@
                 )
             else:
                 return other.tokenizer == self.tokenizer
         return NotImplemented
 
     def __hash__(self):
         from datasets.fingerprint import Hasher
-
-        return hash(Hasher.hash(self.tokenizer))
+        if self.hash is not None:
+            return self.hash
+        
+        else:
+            self.hash =  hash(Hasher.hash(self.tokenizer))
+            return self.hash
```

### Comparing `function_sampler-0.1.3/function_sampler/json.py` & `function_sampler-0.1.6/function_sampler/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     """
 
     # set whitespace pattern
     if whitespace_pattern is None:
         whitespace_pattern = WHITESPACE
 
     if "properties" in instance:
-        regex = ""
+        regex = r""
         regex += r"\{"
         properties = instance["properties"]
         required_properties = instance.get("required", [])
         is_required = [item in required_properties for item in properties]
         # If at least one property is required, we include the one in the lastest position
         # without any comma.
         # For each property before it (optional or required), we add with a comma after the property.
@@ -144,15 +144,15 @@
                     pattern += f"({subregex}{whitespace_pattern},)?"
                 pattern += property_subregexes[i]
                 for subregex in property_subregexes[i + 1 :]:
                     pattern += f"({whitespace_pattern},{subregex})?"
                 possible_patterns.append(pattern)
             regex += f"({'|'.join(possible_patterns)})?"
 
-        regex += f"{whitespace_pattern}" + r"\}"
+        regex += f"{whitespace_pattern}" + r" \}"
 
         return regex
 
     # To validate against allOf, the given data must be valid against all of the
     # given subschemas.
     elif "allOf" in instance:
         subregexes = [
```

### Comparing `function_sampler-0.1.3/function_sampler/regex_constants.py` & `function_sampler-0.1.6/function_sampler/regex_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 STRING_INNER = r'(?:[^"\\\x00-\x1f\x7f-\x9f]|\\.)'
 STRING = f'"{STRING_INNER}*"'
-INTEGER = r"(0|[1-9][0-9]*)"
-NUMBER = rf"(-)?({INTEGER})(\.[0-9]+)?([eE][+-][0-9]+)?"
+INTEGER = r"(-)?(0|[1-9][0-9]*)"
+NUMBER = rf"({INTEGER})(\.[0-9]+)?([eE][+-][0-9]+)?"
 BOOLEAN = r"(true|false)"
 NULL = r"null"
 WHITESPACE = r"[\n ]*"
 
 type_to_regex = {
     "string": STRING,
     "integer": INTEGER,
```

### Comparing `function_sampler-0.1.3/function_sampler/sampler.py` & `function_sampler-0.1.6/function_sampler/sampler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,50 @@
+"""
+Tool Call sampler.
+
+Yes I know how messy this code is. I'll clean it up when I get the chance.
+"""
+
 import functools
 import time
-from json import dumps as json_dumps
 from typing import Any, Dict, List, Union
-from concurrent.futures import ProcessPoolExecutor
+from concurrent.futures import ThreadPoolExecutor
 
 import torch
 from transformers import LogitsProcessor, PreTrainedTokenizer
 
-from .cache import cache
 from .config import TokenMap
 from .config.config import ToolCallSamplerConfig
-from .fsm import FSMState, FsmTokenizer, RegexFSM
-from .json import build_regex_from_schema
+from .fsm import FSMState, FsmTokenizer
 from .logger import get_logger
 from .utils import build_masks, bundle_sampling, tokenize_dicts, compute_fsm
 
 logger = get_logger()
 
 
 class ToolCallSampler(LogitsProcessor):
+    """
+    A logits processor designed to facilitate the generation and sampling of function calls and their arguments.
+
+    Attributes:
+        tokenizer (PreTrainedTokenizer): A tokenizer compatible with Hugging Face's Transformers library,
+            used for encoding and decoding text.
+        functions (List[Dict], optional): A list of dictionaries representing the available functions
+            and their metadata. Defaults to None.
+        config (Union[ToolCallSamplerConfig, Dict[str, Any]], optional): Configuration for the sampler,
+            either as a ToolCallSamplerConfig object or as a dictionary that can be parsed into one.
+            Defaults to None.
+
+    The class is initialized with a tokenizer for handling text encoding/decoding, a list of function
+    definitions for determining valid function calls and arguments, and a configuration object for
+    fine-tuning the sampling behavior. It extends the `LogitsProcessor` class from Hugging Face's
+    Transformers, enabling it to be integrated into the text generation pipeline to control the
+    likelihood of generating specific tokens based on the current context and predefined constraints.
+    """
+
     def __init__(
         self,
         tokenizer: PreTrainedTokenizer,
         functions: List[Dict] = None,
         config: Union[ToolCallSamplerConfig, Dict[str, Any]] = None,
         **kwargs,
     ):
@@ -43,15 +65,19 @@
             self.config.open_func_token if self.config.open_func_token else "<function>"
         )
         self.close_func_token = (
             self.config.open_func_token
             if self.config.open_func_token
             else "</function>"
         )
-
+        self.generate_close_func_token = (
+            config.generate_close_func_token
+            if config.generate_close_func_token
+            else True
+        )
         self.open_func_token_length = len(
             self.tokenizer.encode(self.open_func_token, add_special_tokens=False)
         )
 
         logger.debug(self.open_func_token)
         logger.debug(self.close_func_token)
 
@@ -82,15 +108,15 @@
 
         self.function_maps = tokenize_dicts(self.functions, self.tokenizer)
 
         # we launch computation of all FSM's at the begining,
         # if one is needed before it is finished, we block until it is done.
         # otherwise, it should be ready by the time we need it.
         self.fsm_results = {}
-        self.executor = ProcessPoolExecutor()
+        self.executor = ThreadPoolExecutor()
 
         self.fsm_tokenizer = FsmTokenizer(tokenizer)
 
         for key, function in self.function_maps.items():
             future = self.executor.submit(compute_fsm, self.fsm_tokenizer, function)
             future.add_done_callback(
                 functools.partial(self.populate_fsm_result, key=key)
@@ -214,15 +240,15 @@
         return self.tokenizer.decode(input_ids)
 
     def _encode(self, string):
         return self.tokenizer.encode(string, add_special_tokens=False)
 
     def _check_for_function_call(self, input_ids):
         input_ids = input_ids[0]
-        inputs_string = self.tokenizer.decode(input_ids[-self.open_func_token_length :])
+        inputs_string = self.tokenizer.decode(input_ids[-self.open_func_token_length:])
         if inputs_string.strip().endswith(self.open_func_token):
             return True
         else:
             return False
 
     def __call__(
         self, input_ids: torch.LongTensor, scores: torch.FloatTensor
@@ -286,35 +312,45 @@
                         self.fsm_seq_start_idx = len(self.next_tokens) + tokens_len
                         mask = self._allow_tokens(token_ids=[next_token], mask=mask)
 
                 elif self.identified_function is not None:
                     if self.fsm is None:
                         fsm_key = self.function_key
                         if fsm_key not in self.fsm_results:
+                            ## With the new rust backend, we shouldnt ever need to actually do this. 
+                            ## but it cant really hurt, as it probably accounts for edge cases I cant think of right now.
                             self.fsm = self._wait_for_fsm_result(fsm_key)
                             self.first_fsm_token = True
                         else:
                             self.fsm = self.fsm_results[fsm_key]
+                            self.fsm_state = FSMState(self.fsm.first_state())
                             self.first_fsm_token = True
 
                     if self.first_fsm_token:
                         allowed_tokens = self.fsm.allowed_token_ids(self.fsm_state)
                         self.first_fsm_token = False
                     else:
                         last_token = input_ids[0][-1]
                         self.fsm_state = self.fsm.next_state(
                             self.fsm_state, int(last_token)
                         )
+                        if self.fsm_state == -1:
+                            raise Exception("Final state achieved")
                         allowed_tokens = self.fsm.allowed_token_ids(self.fsm_state)
 
                     if allowed_tokens == [-2]:
                         mask = self._allow_tokens(token_types=["close_bracket"])
-                        self.next_tokens = self.tokenizer.encode(
-                            self.close_func_token, add_special_tokens=False
-                        ) + [self.tokenizer.eos_token_id]
+                        self.next_tokens = (
+                            self.tokenizer.encode(
+                                self.close_func_token, add_special_tokens=False
+                            )
+                            + [self.tokenizer.eos_token_id]
+                            if self.generate_close_func_token
+                            else [self.tokenizer.eos_token_id]
+                        )
                     else:
                         mask = self._allow_tokens(token_ids=allowed_tokens)
                         self.do_sample = True
 
             mask = mask.expand_as(scores)
             scores[~mask] = -float("Inf")
 
@@ -326,9 +362,8 @@
                     top_p=self.top_p,
                     top_k=self.top_k,
                     repetition_penalty=self.repetition_penalty,
                 )
 
             t = time.time() - start_time
             self.total_time += t
-            logger.debug("#### Time for iteration: " + str(time.time() - start_time))
         return scores
```

### Comparing `function_sampler-0.1.3/function_sampler/utils.py` & `function_sampler-0.1.6/function_sampler/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 from .logger import get_logger
-from .fsm import RegexFSM, FsmTokenizer
+from .fsm import FsmTokenizer, create_fsm_index_tokenizer
 from .json import build_regex_from_schema
 from json import dumps as json_dumps
 from transformers import PreTrainedTokenizer
 
 logger = get_logger()
 
 
@@ -57,15 +57,15 @@
 
 
 def compute_fsm(tokenizer: FsmTokenizer, schema):
     if isinstance(tokenizer, PreTrainedTokenizer):
         tokenizer = FsmTokenizer(tokenizer)
 
     regex = build_regex_from_schema(json_dumps(schema))
-    fsm = RegexFSM(regex, tokenizer)
+    fsm, _ = create_fsm_index_tokenizer(regex, tokenizer)
     return fsm
 
 
 def temperature_sample(scores: torch.FloatTensor, temperature) -> torch.FloatTensor:
     scores = scores / temperature
     return scores
```

### Comparing `function_sampler-0.1.3/PKG-INFO` & `function_sampler-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 Metadata-Version: 2.1
 Name: function-sampler
-Version: 0.1.3
+Version: 0.1.6
 Summary: Function calling Logit Sampler
 License: Apache 2.0
 Author: Nathan Hoos
 Author-email: thwackyy.y@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Rust
 Requires-Dist: cloudpickle (>=3.0.0,<4.0.0)
 Requires-Dist: datasets (>=2.18.0,<3.0.0)
 Requires-Dist: diskcache (>=5.6.3,<6.0.0)
-Requires-Dist: interegular (>=0.3.3,<0.4.0)
+Requires-Dist: interegular (==0.3.3)
+Requires-Dist: joblib (>=1.3.2,<2.0.0)
 Requires-Dist: jsonref (>=1.1.0,<2.0.0)
-Requires-Dist: numba (>=0.59.0,<0.60.0)
+Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: referencing (>=0.33.0,<0.34.0)
+Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: transformers (>=4.38.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Function Sampler
 
 <a target="_blank" href="https://colab.research.google.com/github/unaidedelf8777/function-sampler/blob/main/notebooks/Tool_Call_Sampler_demo.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
@@ -102,14 +108,15 @@
 # Use the model for generation
 # only need to tell it how to call the function if it is not explicitly trained for it.
 input_text = "What is the weather today in paris? respond with the word '<function>' to call the weather API."
 input_ids = tokenizer.encode(input_text, return_tensors="pt")
 output = model.generate(input_ids, max_length=200, logits_processor=[sampler])
 generated_text = tokenizer.decode(output[0])
 print(generated_text)
+# <function>  {"name": "get_reservation", "arguments": {"restaurant_name": "Maggiano's", "reservation_time": 18:00:00, "party_size": 6, "contact_number": 1234567890}} </function><|im_end|>
 ```
 
 In this example, we create an instance of the `ToolCallSampler` with the specified functions and configuration. We then attach the sampler to the model's `logits_processor` attribute. This ensures that the sampler is applied during the generation process.
 
 Finally, we use the model to generate text based on the input prompt, which includes the opening function token. The generated text will contain a valid function call adhering to the predefined schema.
 
 For more detailed usage and examples, please refer to the demo notebook provided with the library.
```

