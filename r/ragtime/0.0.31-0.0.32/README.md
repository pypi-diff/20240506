# Comparing `tmp/ragtime-0.0.31.tar.gz` & `tmp/ragtime-0.0.32.tar.gz`

## Comparing `ragtime-0.0.31.tar` & `ragtime-0.0.32.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 ragtime-0.0.31/CHANGELOG.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 ragtime-0.0.31/CONTRIBUTING.md
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.31/deploy/deploy.py
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.31/img/Ragtime_logo.png
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/api.py
--rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/config.py
--rw-r--r--   0        0        0    20347 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/expe.py
--rw-r--r--   0        0        0    39001 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/generators.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/README.md
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/classes.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/main.py
--rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/res/html_templates/basic_template.jinja
--rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
--rw-r--r--   0        0        0    31095 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
--rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 ragtime-0.0.31/tests/full_test.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.31/tests/run_tests.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.31/tests/test_quest.json
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ragtime-0.0.31/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.31/LICENSE
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 ragtime-0.0.31/README.md
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 ragtime-0.0.31/pyproject.toml
--rw-r--r--   0        0        0     7184 2020-02-02 00:00:00.000000 ragtime-0.0.31/PKG-INFO
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 ragtime-0.0.32/CHANGELOG.md
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 ragtime-0.0.32/CONTRIBUTING.md
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.32/deploy/deploy.py
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.32/img/Ragtime_logo.png
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/api.py
+-rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/config.py
+-rw-r--r--   0        0        0    20377 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/expe.py
+-rw-r--r--   0        0        0    40177 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/generators.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/README.md
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/classes.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/main.py
+-rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/res/html_templates/basic_template.jinja
+-rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
+-rw-r--r--   0        0        0    27626 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
+-rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx
+-rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 ragtime-0.0.32/tests/full_test.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.32/tests/run_tests.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.32/tests/test_quest.json
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ragtime-0.0.32/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.32/LICENSE
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ragtime-0.0.32/README.md
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 ragtime-0.0.32/pyproject.toml
+-rw-r--r--   0        0        0     7473 2020-02-02 00:00:00.000000 ragtime-0.0.32/PKG-INFO
```

### Comparing `ragtime-0.0.31/CHANGELOG.md` & `ragtime-0.0.32/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# v0.0.32 - May 6th 2024
+- generation in async
+- logs more precise
+- `basic_template.xlsx` updated
+
 # v0.0.31
 - added "update_from_spreadsheet"
 - updates in config.py regarding column numbers
 - renamed Answer Prompters
 - minor updates in README.md
 
 # v0.0.30
```

### Comparing `ragtime-0.0.31/img/Ragtime_logo.png` & `ragtime-0.0.32/img/Ragtime_logo.png`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/src/ragtime/__init__.py` & `ragtime-0.0.32/src/ragtime/__init__.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/src/ragtime/api.py` & `ragtime-0.0.32/src/ragtime/api.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/src/ragtime/config.py` & `ragtime-0.0.32/src/ragtime/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     # # # Spreadheet
     DEFAULT_SPREADSHEET_TEMPLATE = FOLDER_SST_TEMPLATES / 'basic_template.xlsx'
     DEFAULT_WORKSHEET = "Expe"
     DEFAULT_HEADER_SIZE = 2
     DEFAULT_QUESTION_COL = 2
     DEFAULT_FACTS_COL = 4
     DEFAULT_ANSWERS_COL = 11
-    DEFAULT_HUMAN_EVAL_COL = 25
+    DEFAULT_HUMAN_EVAL_COL = 24
     # # # LLMs
     DEFAULT_LITELLM_RETRIES = 3
     DEFAULT_LITELLM_TEMP = 0
 
     ####################
     # LOGGING
     # You can choose the file where the logs are written in "log_conf" dict, key "handlers"/"file"/"filename" - default is "logs/logs.txt"
@@ -140,19 +140,14 @@
     inspect_stack = inspect.stack()
     class_name:str = inspect_stack[1][0].f_locals["self"].__class__.__name__
     return f'[{class_name}.{inspect.stack()[1][3]}()] {msg}'
 
 def div0(num:float, denom:float) -> float:
     return float(num/denom) if denom else 0.0
 
-class InitType(IntEnum):
-	globals_only = 0 # do not touch the files, only initiates the global variables (logger, folder variables...)
-	copy_base_files = 1 # globals_only + copy files to create base_folder, raise an exception if already exists
-	delete_if_exists = 2 # copy_base_files + remove folder if existing before copying base_folder
-    
 def init_project(name:str, init_type:Literal["globals_only", "copy_base_files", "delete_if_exists"]="globals_only", dest_path:Path = None):
     """Initiates a project : copy base files and and set global variables
     Args:
     - init_type
         "globals_only" = 0 # do not touch the files, only initiates the global variables (logger, folder variables...)
         "copy_base_files" = 1 # globals_only + copy files to create base_folder, raise an exception if already exists
         "delete_if_exists" = 2 # copy_base_files + remove folder if existing before copying base_folder"""
```

### Comparing `ragtime-0.0.31/src/ragtime/expe.py` & `ragtime-0.0.32/src/ragtime/expe.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     user:Optional[str] = ""
     system:Optional[str] = ""
 
 class LLMAnswer(RagtimeText):
     prompt:Optional[Prompt] = None
     name:Optional[str] = None
     full_name:Optional[str] = None
-    timestamp: datetime = Field(default_factory=lambda: datetime.now())  # timestamp indicating when the question has been sent to the LLM
+    timestamp: datetime = Optional[datetime]  # timestamp indicating when the question has been sent to the LLM
     duration: Optional[float] = None # time to get the answer in seconds
     cost: Optional[float] = None
 
 class WithLLMAnswer(BaseModel):
     llm_answer:Optional[LLMAnswer] = None
 
 class Eval(RagtimeText, WithLLMAnswer):
@@ -168,15 +168,15 @@
         return name
 
     def _file_check_before_writing(self, path:Path=None, b_overwrite:bool=False, b_add_suffix:bool = True, force_ext:str=None) -> Path:
         if not path:
             if self.json_path:
                 path = Path(self.json_path.parent) / self.json_path.stem
             else:
-                raise RagtimeException(f'Cannot save since no json_path is stored in expe and no path has been provided')        
+                raise RagtimeException(f'Cannot save to JSON since no json_path is stored in expe and not path has been provided in argument.')        
 
         # Make sure at least 1 QA is here
         if len(self) == 0:
             raise Exception("""The Expe object you're trying to write is empty! Please add at least one QA""")
         
         # Check and prepare the destination file path
         if not(path):
@@ -282,28 +282,29 @@
                         new_facts.append(Fact(text=data_in_ws))
                     elif update_type == UpdateTypes.human_eval: # Update HUMAN EVAL
                         answer_text:str = row[answer_col].value
                         cur_ans:Answer = next((a for a in cur_qa.answers if a.text == answer_text), None)
                         if cur_ans: # corresponding Answer has been found
                             try:
                                 human_eval:int = int(data_in_ws)
+                                cur_ans.eval.human = human_eval
                             except (TypeError, ValueError):
                                 logger.warn(f'Human eval should be a value between 0 and 1 - cannot use "{data_in_ws}" as found in line {i}')
-                            cur_ans.eval.human = human_eval
                         else:
                             logger.warn(f'Cannot find Answer corresponding with the human eval "{data_in_ws}" - Answer should contain the text "{answer_text}"')
                         
 
     def save_to_json(self, path:Path=None, b_overwrite:bool=False, b_add_suffix:bool = True) -> Path:
         """Saves Expe to JSON - can generate a suffix for the filename
         Returns the Path of the file actually saved"""
         path:Path = self._file_check_before_writing(path, b_overwrite=b_overwrite, 
                                                     b_add_suffix=b_add_suffix, force_ext='.json')
         with open(path, mode='w', encoding='utf-8') as file:
             file.write(self.model_dump_json(indent=2))
+        self.json_path = path
         logger.info(f'Expe saved as JSON to {path}')
         return path
 
     def save_to_html(self, path:Path=None, render_params:dict[str,bool]=DEFAULT_HTML_RENDERING,
                      template_path:Path=DEFAULT_HTML_TEMPLATE, b_overwrite:bool=False, b_add_suffix:bool = True):
         """Saves Expe to an HTML file from a Jinja template - can generate a suffix for the filename
         Returns the Path of the file actually saved"""
```

### Comparing `ragtime-0.0.31/src/ragtime/generators.py` & `ragtime-0.0.32/src/ragtime/generators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from abc import ABC, abstractmethod
+from datetime import datetime
 from pathlib import Path
+import time
 from langdetect import detect
 import json
 from unidecode import unidecode
 from enum import IntEnum
 from typing import Optional, Union
 from ragtime.expe import Answer, Answers, Chunks, Eval, Expe, Fact, Facts, LLMAnswer, Question, RagtimeBase, QA, Prompt, WithLLMAnswer
-from litellm import completion_cost, completion
+from litellm import completion_cost, acompletion
+from litellm.exceptions import RateLimitError
 from ragtime.config import RagtimeException, logger, div0
 import re
+import asyncio
 
 import litellm
 litellm.telemetry = False
 
 #################################
 ## CONSTANTS
 #################################
@@ -254,14 +258,15 @@
         # compute metrics
         precision:float = div0(len(true_facts_in_answer), len(facts_in_answer)+nb_false_facts_in_answer)
         recall:float = div0(len(true_facts_in_answer), len(true_facts))
         cur_obj.meta["precision"] = precision
         cur_obj.meta["recall"] = recall
         cur_obj.meta["hallus"] = nb_false_facts_in_answer
         cur_obj.meta["missing"] = ', '.join(list(true_facts_not_in_answer))
+        cur_obj.meta["nb_missing"] = len(cur_obj.meta["missing"])
         cur_obj.meta["facts_in_ans"] = str(sorted(facts_in_answer))
         cur_obj.auto = div0(2*precision*recall, precision+recall)
         cur_obj.text = answer
 
 class PptrSimpleEvalFR(Prompter):
     def get_prompt(self, answer:Answer, facts:Facts) -> Prompt:
         result:Prompt = Prompt()
@@ -342,15 +347,15 @@
     Class deriving from LLM must implement `complete`.
     A Prompter must be provided at creation time.
     Instantiates a get_prompt so as to be able change the prompt LLM-wise.
     """
     name:Optional[str] = None
     prompter:Prompter
 
-    def generate(self, cur_obj:WithLLMAnswer, prev_obj:WithLLMAnswer, qa:QA,
+    async def generate(self, cur_obj:WithLLMAnswer, prev_obj:WithLLMAnswer, qa:QA,
                 start_from:StartFrom, b_missing_only:bool, **kwargs) -> WithLLMAnswer:
         """Generate prompt and execute LLM
         Returns the retrieved or created object containing the LLMAnswer
         If None, LLMAnswer retrieval or generation went wrong and post-processing
         must be skipped"""
         
         assert not prev_obj or (cur_obj.__class__ == prev_obj.__class__)
@@ -366,15 +371,15 @@
             prompt = prev_obj.llm_answer.prompt
 
         # Generates text
         result:WithLLMAnswer = cur_obj
         if not(prev_obj and prev_obj.llm_answer) or (start_from <= StartFrom.llm and not b_missing_only):
             logger.debug(f'Either no {cur_class_name} / LLMAnswer exists yet, or you asked to regenerate it ==> generate LLMAnswer')
             try:
-                result.llm_answer = self.complete(prompt)
+                result.llm_answer = await self.complete(prompt)
             except Exception as e:
                 logger.exception(f'Exception while generating - skip it\n{e}')
                 result = None
         else:
             logger.debug(f'Reuse existing LLMAnswer in {cur_class_name}')
             result = prev_obj
 
@@ -384,44 +389,55 @@
             self.prompter.post_process(qa=qa, cur_obj=result)
         else:
             logger.debug('Reuse post-processing')            
 
         return result
     
     @abstractmethod
-    def complete(self, prompt:Prompt) -> LLMAnswer:
+    async def complete(self, prompt:Prompt) -> LLMAnswer:
         raise NotImplementedError('Must implement this!')
 
 class LiteLLM(LLM):
     """Simple extension of LLM based on the litellm library.
     Allows to call LLMs by their name in a stantardized way.
     The default get_prompt method is not changed.
     The generate method uses the standard litellm completion method.
     Default values of temperature (0.0) and number of retries when calling the API (3) can be changed.
     The proper API keys and endpoints have to be specified in the keys.py module.
     """
     name:str
     temperature:float = 0.0
     num_retries:int = 3
 
-    def complete(self, prompt:Prompt) -> LLMAnswer:
+    async def complete(self, prompt:Prompt) -> LLMAnswer:
         messages:list[dict] = [{"content":prompt.system, "role":"system"},
                                {"content":prompt.user, "role":"user"}]
-        try:
-            ans:dict = completion(messages=messages, model=self.name,
-                                    temperature=self.temperature, num_retries=self.num_retries)
-        except Exception as e:
-            logger.exception(f'The following exception occurred with prompt {prompt}' + '\n' + str(e))
-            return None
+        retry:int = 1
+        wait_step:float = 3.0
+        start_ts:datetime = datetime.now()
+        while retry:
+            try:
+                time_to_wait:float = wait_step
+                ans:dict = await acompletion(messages=messages, model=self.name,
+                                        temperature=self.temperature, num_retries=self.num_retries)
+                retry = 0
+            except RateLimitError as e:
+                logger.debug(f'Rate limit reached - will retry in {time_to_wait:.2f}s ({str(e)})')
+                asyncio.sleep(time_to_wait)
+                retry += 1
+            except Exception as e:
+                logger.exception(f'The following exception occurred with prompt {prompt}' + '\n' + str(e))
+                return None
         
         llm_ans:LLMAnswer = LLMAnswer(prompt=prompt,
                                       text=ans['choices'][0]['message']['content'],
                                       name=self.name,
                                       full_name=ans['model'],
-                                      duration=ans._response_ms/1000,
+                                      timestamp=start_ts,
+                                      duration=ans._response_ms/1000 if hasattr(ans, "_response_ms") else None, # sometimes _response_ms is not present
                                       cost=float(completion_cost(ans)))
         return llm_ans
 
 #################################
 ## TEXT GENERATORS
 #################################
 class TextGenerator(RagtimeBase, ABC):
@@ -456,15 +472,15 @@
         """Helper function to get the first LLM when only one is provided (like for EvalGenerator and FactGenerator)"""
         if self.llms:
             return self.llms[0]
         else:
             return None
     
     def generate(self, expe:Expe, start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, 
-                 only_llms:list[str] = None, save_every:int=0) -> bool:
+                 only_llms:list[str] = None, save_every:int=0):
         """Main method calling "gen_for_qa" for each QA in an Expe. Returns False if completed with error, True otherwise
         The main step in generation are :
         - beginning: start of the process - when start_from=beginning, the whole process is executed
 	    - chunks: only for Answer generation - chunk retrieval, if a Retriever is associated with the Answer Generator object
         Takes a Question and returns the Chunks
         - prompt: prompt generation, either directly using the question or with the chunks if any
         Takes a Question + optional Chunks and return a Prompt
@@ -477,35 +493,39 @@
             - start_from: allows to start generation from a specific step in the process
             - b_missing_only: True to execute the steps only when the value is absent, False to execute everything
             even if a value already exists
             - only_llms: restrict the llms to be computed again - used in conjunction with start_from -
             if start from beginning, chunks or prompts, compute prompts and llm answers for the list only -
             if start from llm, recompute llm answers for these llm only - has not effect if start 
             """
+
         nb_q:int = len(expe)
-        try:
-            for num_q, qa in enumerate(expe, start=1):
-                logger.prefix = f"({num_q}/{nb_q})"
-                logger.info(f'*** {self.__class__.__name__} for question "{qa.question.text}"')
-                self.gen_for_qa(qa=qa, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms)
-                logger.info(f'End question "{qa.question.text}"')
-                if save_every and (num_q % save_every == 0): expe.save_to_json()
-        except Exception as e:
-            logger.exception(f"Exception caught - saving what has been done so far:\n{e}")
-            expe.save_temp(name=f"Stopped_at_{num_q}_of_{nb_q}_")
-            return False
-        
-        return True
+        async def generate_for_qa(num_q:int, qa:QA):
+            logger.prefix = f"({num_q}/{nb_q})"
+            logger.info(f'*** {self.__class__.__name__} for question "{qa.question.text}"')
+            try:
+                await self.gen_for_qa(qa=qa, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms)
+            except Exception as e:
+                logger.exception(f"Exception caught - saving what has been done so far:\n{e}")
+                expe.save_temp(name=f"Stopped_at_{num_q}_of_{nb_q}_")
+                return
+            logger.info(f'End question "{qa.question.text}"')
+            if save_every and (num_q % save_every == 0): expe.save_to_json()
+
+        loop = asyncio.get_event_loop()
+        tasks = [generate_for_qa(num_q, qa) for num_q, qa in enumerate(expe, start=1)]
+        logger.info(f'{len(tasks)} tasks created')
+        all_qa = loop.run_until_complete(asyncio.gather(*tasks))
 
     def write_chunks(self, qa:QA):
         """Write chunks in the current qa if a Retriever has been given when creating the object. Ignore otherwise"""
         raise NotImplementedError('Must implement this if you want to use it!')
     
     @abstractmethod
-    def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, 
+    async def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, 
                    b_missing_only:bool = True, only_llms:list[str] = None):
         """Method to be implemented to generate Answer, Fact and Eval"""
         raise NotImplementedError('Must implement this!')
 
 class AnsGenerator(TextGenerator):
     """Object to write answers in the expe
     To use a Retriever, first implement one and give it as parameter when constructing the object
@@ -528,15 +548,15 @@
 
     def write_chunks(self, qa:QA):
         """Write chunks in the current qa if a Retriever has been given when creating the object. Ignore otherwise"""
         if self.retriever:
             qa.chunks.empty()
             self.retriever.retrieve(qa=qa)
     
-    def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, b_missing_only:bool=False, only_llms:list[str] = None):
+    async def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, b_missing_only:bool=False, only_llms:list[str] = None):
         """
         Args
         - qa (QA) : the QA (expe row) to work on
         - start_from : a value in the StartFrom Enum, among:
             - beginning: retrieve chunks (if a Retriever is given, ignore otherwise), compute prompts,
         computer llm answers, compute meta on answers
             - prompt: reuse chunks, compute prompts, llm answers and meta
@@ -544,40 +564,43 @@
             - post_process: reuse chunks, prompts and llm answers, compute meta only
         - b_missing_only: True to generate LLM Answers only when the Answer object has no "llm_answer"
         Useful to complete a previous experiment where all the Answers have not been generated (happens sometimes due
         to external server failures)
         - only_llms: restrict the llms to be computed again - used in conjunction with start_from - if start from beginning, chunks or prompts, compute prompts and llm answers for the list only - if start from llm, recompute llm answers for these llm only - has not effect if start 
         """
         # Get chunks -> fills the Chunks in the QA
+        logger.prefix += '[AnsGen]'
         if self.retriever:
             # Compute chunks if there are not any or there are some and user asked to start à Chunks step or before and did not mention to
             # complete only the missing ones
             if (not qa.chunks) or (qa.chunks and start_from <= StartFrom.chunks and not b_missing_only):
                 logger.info(f'Compute chunks')
                 self.write_chunks(qa=qa)
             else: # otherwise reuse the chunks already in the QA object
                 logger.info(f'Reuse existing chunks')
 
         # Generation loop, for each LLM -> fills the Answers in the QA
         # Get list of LLMs sto actually use, if only_llms defined
         new_answers:Answer = Answers()
         actual_llms:list[LLM] = [l for l in self.llms if l in only_llms] if only_llms else self.llms
+        original_prefix:str = logger.prefix
         for llm in actual_llms:
-            logger.info(f'* Start with LLM "{llm.name}"')
+            logger.prefix = f'{original_prefix}[{llm.name}]'
+            logger.info(f'* Start with LLM')
 
             # Get existing Answer if any
             prev_ans:Optional[Answer] = [a for a in qa.answers if a.llm_answer and (a.llm_answer.name == llm.name or a.llm_answer.full_name == llm.name)]
             if prev_ans:
                 prev_ans = prev_ans[0] # prev_ans is None if no previous Answer has been generated for the current LLM
                 logger.debug(f'An Answer has already been generated with this LLM')
             else:
                 prev_ans = None
 
             # Get Answer from LLM
-            ans:Answer = llm.generate(cur_obj=Answer(), prev_obj=prev_ans,
+            ans:Answer = await llm.generate(cur_obj=Answer(), prev_obj=prev_ans,
                                       qa=qa, start_from=start_from,
                                       b_missing_only=b_missing_only,
                                       question=qa.question,
                                       chunks=qa.chunks)
            
             # get previous human eval if any
             if prev_ans and prev_ans.eval:
@@ -587,55 +610,57 @@
        
         # end of the per LLM loop, answers have been generated or retrieved, write them in qa
         qa.answers = new_answers
 
 class FactGenerator(TextGenerator):
     """Generate Facts from existing Answers"""
 
-    def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, b_missing_only:bool=False, only_llms:list[str] = None):
+    async def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, b_missing_only:bool=False, only_llms:list[str] = None):
         """Create Facts based on the first Answer in the QA having human Eval equals 1 """
        
         ans:Answer = next((a for a in qa.answers if a.eval and a.eval.human == 1.0))
         if ans:
+            logger.prefix += f'[FactGen][{self.llm.name}]'
             model_str:str = f" associated with answer from model {ans.llm_answer.full_name}" if ans.llm_answer else ""
             logger.info(f'Generate Facts since it has a human validated answer (eval.human == 1.0){model_str}')
             prev_facts:Facts = qa.facts
 
             #2.a. and 2.b : prompt generation + Text generation with LLM 
-            qa.facts = self.llm.generate(cur_obj=Facts(), prev_obj=prev_facts,
+            qa.facts = await self.llm.generate(cur_obj=Facts(), prev_obj=prev_facts,
                                     qa=qa, start_from=start_from,
                                     b_missing_only=b_missing_only,
                                     answer=ans)
         else:
             logger.debug(f'No fact has been generated since no answer has been validated (human=1.0) for this question')
 
 class EvalGenerator(TextGenerator):
     """Generate Eval from Answers and Facts.
     For a given QA, send the Answer and the Facts to the LLM to get the prompt back
     The default prompt returns all the valid facts given an answer, i.e. 1 prompt -> 1 Eval
     That could be overridden to have e.g. 1 prompt per Fact, i.e. N prompt -> 1 Eval
     The conversion between the LLM answer and the Eval is made in post_process"""
 
-    def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, b_missing_only:bool=False, only_llms:list[str] = None):
+    async def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, b_missing_only:bool=False, only_llms:list[str] = None):
         """Create Eval for each QA where Facts are available"""
 
         if len(qa.answers) == 0:
             logger.error(f'No Answers, cannot generate Evals'); return
         if len(qa.facts) == 0:
             logger.error(f'No Facts, cannot generate Evals'); return
         
         # Eval loop
+        logger.prefix += f'[EvalGen][{self.llm.name}]'
         for ans in (a for a in qa.answers if a.text):
             llm_name:str = ans.llm_answer.name if ans.llm_answer else UNKOWN_LLM
             if only_llms and llm_name not in only_llms and llm_name != UNKOWN_LLM: continue
             logger.debug(f'Generate Eval for answer generated with "{llm_name}"')
             prev_eval:Eval = ans.eval
     
             #2.a. and 2.b : prompt generation + Text generation with LLM 
-            ans.eval = self.llm.generate(cur_obj=Eval(), prev_obj=prev_eval,
+            ans.eval = await self.llm.generate(cur_obj=Eval(), prev_obj=prev_eval,
                                     qa=qa, start_from=start_from,
                                     b_missing_only=b_missing_only,
                                     answer=ans, facts=qa.facts)          
 
             # save previous human eval if any
             if prev_eval and prev_eval.human: ans.eval.human = prev_eval.human
 
@@ -646,73 +671,66 @@
     def __init__(self, llms:list[LLM] = None):
         super().__init__(llms=llms)
         if len(self.llms) < 2:
             raise RagtimeException("""Need at least 2 LLMs to run this generator!
                                    1st LLM is used to generate Facts from the Answer.
                                    2nd LLM is used to generate Eval from the golden Facts and the Facts from the Answer.""")
 
-    def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, b_missing_only:bool=False):
+    async def gen_for_qa(self, qa:QA, start_from:StartFrom=StartFrom.beginning, b_missing_only:bool=False):
         """Create Eval for each QA where Facts are available"""
 
         if len(qa.answers) == 0:
             logger.error(f'No Answers, cannot generate Evals'); return
         if len(qa.facts) == 0:
             logger.error(f'No Facts, cannot generate Evals'); return
         
         # Eval loop
         for ans in (a for a in qa.answers if a.text):
             llm_name:str = ans.llm_answer.name if ans.llm_answer else "unkown LLM (manual ?)"
             logger.debug(f'Generate Facts for answer generated with "{llm_name}"')
             prev_eval:Eval = ans.eval
     
             # Use 1st LLM to generate facts from the Answer
-            ans_facts:Facts = self.llms[0].generate(cur_obj=Facts(), prev_obj=None,
+            ans_facts:Facts = await self.llms[0].generate(cur_obj=Facts(), prev_obj=None,
                                     qa=qa, start_from=start_from,
                                     b_missing_only=b_missing_only,
                                     answer=ans)    
                       
             # Use 2nd LLM to generate Eval
             logger.debug(f'Then generate Eval using answer facts and gold facts')
             cur_eval:Eval = Eval()
             cur_eval.meta['answer_facts'] = [af.text for af in ans_facts] # stores the answer's facts in the current eval
-            ans.eval = self.llms[1].generate(cur_obj=cur_eval, prev_obj=prev_eval,
+            ans.eval = await self.llms[1].generate(cur_obj=cur_eval, prev_obj=prev_eval,
                                     qa=qa, start_from=start_from,
                                     b_missing_only=b_missing_only,
                                     answer_facts=ans_facts, gold_facts=qa.facts)
 
             # save previous human eval if any
             if prev_eval and prev_eval.human: ans.eval.human = prev_eval.human
 
 def gen_Answers(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str], retriever:Retriever=None, 
                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
   """Standard function to generate answers - returns the updated Expe or None if an error occurred"""
   expe:Expe = Expe(json_path=folder_in / json_file)
   ans_gen:AnsGenerator = AnsGenerator(retriever=retriever, llm_names=llm_names, prompter=prompter)
-  if ans_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms,
-                      save_every=save_every):
-    expe.save_to_json(path=folder_out / json_file)
-    return expe
-  else:
-    return None
+  ans_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
+  expe.save_to_json(path=folder_out / json_file)
+  return expe
   
 
 def gen_Facts(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str],
                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
   """Standard function to generate facts - returns the updated Expe or None if an error occurred"""
   expe:Expe = Expe(json_path=folder_in / json_file)
   fact_gen:FactGenerator = FactGenerator(llm_names=llm_names, prompter=prompter)
-  if fact_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every):
-    expe.save_to_json(path=folder_out / json_file)
-    return expe
-  else:
-    return None
+  fact_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
+  expe.save_to_json(path=folder_out / json_file)
+  return expe
 
 def gen_Evals(folder_in:Path, folder_out:Path, json_file: Union[Path,str], prompter:Prompter, llm_names:list[str],
                 start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0) -> Expe:
   """Standard function to generate evals - returns the updated Expe or None if an error occurred"""
   expe:Expe = Expe(json_path=folder_in / json_file)
   eval_gen:EvalGenerator = EvalGenerator(llm_names=llm_names, prompter=prompter)
-  if eval_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every):
-    expe.save_to_json(path=folder_out / json_file)
-    return expe
-  else:
-    return None
+  eval_gen.generate(expe, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
+  expe.save_to_json(path=folder_out / json_file)
+  return expe
```

### Comparing `ragtime-0.0.31/src/ragtime/base_folder/.gitignore` & `ragtime-0.0.32/src/ragtime/base_folder/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/src/ragtime/base_folder/LICENSE` & `ragtime-0.0.32/src/ragtime/base_folder/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/src/ragtime/base_folder/classes.py` & `ragtime-0.0.32/src/ragtime/base_folder/classes.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/src/ragtime/base_folder/main.py` & `ragtime-0.0.32/src/ragtime/base_folder/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,12 +5,13 @@
 from ragtime.expe import QA, Chunks, Prompt, Question, WithLLMAnswer
 
 # always start with init_project before importing ragtime.config values since they are updated
 # with init_project and import works by value and not by reference, so values imported before
 # calling init_project are not updated after the function call
 ragtime.config.init_project(name=PROJECT_NAME, init_type="globals_only")
 from ragtime.config import FOLDER_ANSWERS, FOLDER_QUESTIONS, logger
-# If you're using Windows, make your environment variables for LLM providers accessible with the following instruction
-# ragtime.config.init_win_env(['OPENAI_API_KEY', 'ALEPHALPHA_API_KEY', 'MISTRAL_API_KEY'])
 
 # Note: the logger can be used only *after* ragtime.config.init_project
-logger.debug(f'{PROJECT_NAME} STARTS')
+logger.debug(f'{PROJECT_NAME} STARTS')
+
+# If you're using Windows, make your environment variables for LLM providers accessible with the following instruction
+# ragtime.config.init_win_env(['OPENAI_API_KEY', 'ALEPHALPHA_API_KEY', 'MISTRAL_API_KEY'])
```

### Comparing `ragtime-0.0.31/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx` & `ragtime-0.0.32/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/src/ragtime/base_folder/res/html_templates/basic_template.jinja` & `ragtime-0.0.32/src/ragtime/base_folder/res/html_templates/basic_template.jinja`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx` & `ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/basic_template.xlsx` & `ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-00000000: 504b 0304 1400 0600 0800 0000 2100 7fd5  PK..........!...
-00000010: effa f201 0000 640a 0000 1300 0802 5b43  ......d.......[C
+00000000: 504b 0304 1400 0600 0800 0000 2100 64d1  PK..........!.d.
+00000010: 1d0f de01 0000 cf09 0000 1300 0802 5b43  ..............[C
 00000020: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
 00000030: 6c20 a204 0228 a000 0200 0000 0000 0000  l ...(..........
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -29,49 +29,49 @@
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 00cc 96cf 6edb 300c  ............n.0.
-00000240: c6ef 03f6 0e86 ae43 acb4 0386 6188 d343  .......C....a..C
-00000250: b79d f6a7 40bb 0760 2526 1622 4b82 c4b6  ....@..`%&."K...
-00000260: c9db 8f56 9c22 18d2 b889 3d6c 9738 8ecd  ...V."....=l.8..
-00000270: eff7 910a 45cd aed6 8d2d 1e31 26e3 5d25  ....E....-.1&.]%
-00000280: 2eca a928 d029 af8d 5b56 e2d7 ddd7 c947  ...(.)..[V.....G
-00000290: 5124 02a7 c17a 8795 d860 1257 f3b7 6f66  Q$...z...`.W..of
-000002a0: 779b 80a9 e068 972a 5113 854f 5226 5563  w....h.*Q..OR&Uc
-000002b0: 03a9 f401 1d3f 59f8 d800 f16d 5cca 006a  .....?Y....m\..j
-000002c0: 054b 9497 d3e9 07a9 bc23 7434 a156 43cc  .K.......#t4.VC.
-000002d0: 679f 7101 0f96 8a2f 6bfe 79eb e4de 3851  g.q..../k.y...8Q
-000002e0: 5c6f df6b 5195 8010 ac51 406c 543e 3afd  \o.kQ....Q@lT>:.
-000002f0: 0764 e217 0ba3 507b f5d0 b074 9942 44d0  .d....P{...t.BD.
-00000300: a946 a4c6 9621 1a26 c65b 24e2 c492 9007  .F...!.&.[$.....
-00000310: 9911 6d3a 0dda 6555 7264 3696 6a13 d23b  ..m:..eUrd6.j..;
-00000320: 4efd 0542 fbe4 e5ac bab8 9fbc 1cd1 682c  N..B..........h,
-00000330: 6e20 d20f 6838 77b9 b6f2 c9c7 d5bd f7ab  n ..h8w.........
-00000340: f2b8 c8a9 a5c9 252a 1b30 6ee7 fb08 3fbf  ......%*.0n...?.
-00000350: 9c64 be5c 8c6c a4cd 2f0b 9fe8 e3f2 3ff1  .d.\.l../.....?.
-00000360: f1fe 1ff9 406e 9ae8 c07e 336e 95e4 fedd  ....@n...~3n....
-00000370: d82b b4af ddb3 48c4 1b01 cafc 39dc 4596  .+....H.....9.E.
-00000380: e901 26da 584c 63f7 4616 ed23 d710 51df  ..&.XLc.F..#..Q.
-00000390: 126f 31cb d10d ec6b f7f8 6890 4003 c1df  .o1....k..h.@...
-000003a0: d81f be77 da3d 1674 84a7 b60a b2fb 327c  ...w.=.t......2|
-000003b0: e93b a11e aee2 3251 92f9 321a 93c7 4616  .;....2Q..2...F.
-000003c0: 3c81 3d7c 2bea f23d 833d 7cfb 398b 9dfb  <.=|+..=.=|.9...
-000003d0: ee35 356f 5237 a2b7 55cd 71af 2cad b73e  .55oR7..U.q.,..>
-000003e0: a633 182a 07b6 3ddc 0702 abae 6b1e 8123  .3.*..=.....k..#
-000003f0: f78e dae9 1ee3 f391 e526 fac0 7f5f 1ff1  .........&..._..
-00000400: 7403 bb23 481b 3d09 2c84 910c 3e1f 420e  t..#H.=.,...>.B.
-00000410: 0df3 6722 1fa9 0667 dc0e 05a7 511f 60cb  ..g"...g....Q.`.
-00000420: 7c46 9cff 0600 00ff ff03 0050 4b03 0414  |F.........PK...
-00000430: 0006 0008 0000 0021 00b5 5530 23f4 0000  .......!..U0#...
-00000440: 004c 0200 000b 0008 025f 7265 6c73 2f2e  .L......._rels/.
-00000450: 7265 6c73 20a2 0402 28a0 0002 0000 0000  rels ...(.......
+00000230: 0000 0000 0000 0000 00cc 96c1 6edb 300c  ............n.0.
+00000240: 86ef 03f6 0e86 ae43 acb4 0386 6188 d343  .......C....a..C
+00000250: b7dd b615 68f7 00aa c4c4 4264 4910 d936  ....h.....BdI..6
+00000260: 79fb d18a 530c 431a d7b1 87ed 623b b1f9  y...S.C.....b;..
+00000270: 7f3f 29d3 d4e2 6adb b8e2 1112 dae0 2b71  .?)...j.......+q
+00000280: 51ce 4501 5e07 63fd ba12 3fef bece 3e8a  Q.E.^.c...?...>.
+00000290: 0249 79a3 5cf0 5089 1da0 b85a be7d b3b8  .Iy.\.P....Z.}..
+000002a0: db45 c082 a33d 56a2 268a 9fa4 445d 43a3  .E...=V.&...D]C.
+000002b0: b00c 113c df59 85d4 28e2 9f69 2da3 d21b  ...<.Y..(..i-...
+000002c0: b506 7939 9f7f 903a 7802 4f33 6a35 c472  ..y9...:x.O3j5.r
+000002d0: f119 56ea c151 f165 cb7f ef9d dc5b 2f8a  ..V..Q.e.....[/.
+000002e0: ebfd 732d aa12 2a46 67b5 2236 2a1f bdf9  ..s-..*Fg."6*...
+000002f0: 0332 0bab 95d5 6082 7e68 58ba c498 4019  .2....`.~hX...@.
+00000300: ac01 a871 654c 9689 e916 8838 3114 f228  ...qeL.....81..(
+00000310: 3381 c361 d02e ab92 23b3 31ac 6dc4 779c  3..a....#.1.m.w.
+00000320: fa0b 84f6 cecb 5975 713f 7839 9235 50dc  ......Yuq?x9.5P.
+00000330: a844 df55 c3b9 cbad 934f 216d ee43 d894  .D.U.....O!m.C..
+00000340: a745 8696 2697 a86c 94f5 07df 27f8 f961  .E..&..l....'..a
+00000350: 94f9 7431 b191 36bf 2c3c d0c7 e57f e2e3  ..t1..6.,<......
+00000360: fd3f f241 dc73 20f3 71fc 9264 999e 0540  .?.A.s .q..d...@
+00000370: da39 c0a9 5fc3 2cda 47ae 5502 734b dccd  .9.._.,.G.U.sK..
+00000380: ebc9 0dfc aedd e3a3 0152 4691 fa1b adf8  .........RF.....
+00000390: add3 eeb1 6092 7a6a ab20 bb8b f14b df09  ....`.zj. ...K..
+000003a0: f570 3597 8950 e6d3 644c fe42 67c1 01ec  .p5..P..dL.Bg...
+000003b0: f15d dfe5 7b06 7b7c a79f c5ce 7df7 9a9a  .]..{.{|....}...
+000003c0: 37d8 4dc3 7d55 73dc 2b4b 1b5c 4878 0643  7.M.}Us.+K.\Hx.C
+000003d0: e7c0 b687 fb40 cae9 eb9a a7cd c4bd a30f  .....@..........
+000003e0: baa7 f8bc 3bb8 4921 f2eb 1b12 0c37 7098  ....;.I!.....7p.
+000003f0: f66d f42c b210 24b2 f03c ef8f cdcd 6722  .m.,..$..<....g"
+00000400: ef5e 4667 0ced f6c8 8039 c296 793b b6fc  .^Fg.....9..y;..
+00000410: 0500 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+00000420: 0000 0021 00b5 5530 23f4 0000 004c 0200  ...!..U0#....L..
+00000430: 000b 0008 025f 7265 6c73 2f2e 7265 6c73  ....._rels/.rels
+00000440: 20a2 0402 28a0 0002 0000 0000 0000 0000   ...(...........
+00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -94,1851 +94,1780 @@
 000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000650: 0000 0000 0000 0000 0000 0000 ac92 4d4f  ..............MO
-00000660: c330 0c86 ef48 fc87 c8f7 d5dd 9010 424b  .0...H........BK
-00000670: 7741 48bb 2154 7e80 49dc 0fb5 8da3 241b  wAH.!T~.I.....$.
-00000680: ddbf 271c 1054 1a83 0347 7fbd 7efc cadb  ..'..T...G..~...
-00000690: dd3c 8dea c821 f6e2 34ac 8b12 143b 23b6  .<...!..4....;#.
-000006a0: 77ad 8697 fa71 7507 2a26 7296 4671 ace1  w....qu.*&r.Fq..
-000006b0: c411 76d5 f5d5 f699 474a 7928 76bd 8f2a  ..v.....GJy(v..*
-000006c0: abb8 a8a1 4bc9 df23 46d3 f144 b110 cf2e  ....K..#F..D....
-000006d0: 571a 0913 a51c 8616 3d99 815a c64d 59de  W.......=..Z.MY.
-000006e0: 62f8 ae01 d542 53ed ad86 b0b7 37a0 ea93  b....BS.....7...
-000006f0: cf9b 7fd7 96a6 e90d 3f88 394c ecd2 9915  ........?.9L....
-00000700: c873 6267 d9ae 7cc8 6c21 f5f9 1a55 5368  .sbg..|.l!...USh
-00000710: 3969 b062 9e72 3a22 795f 646c c0f3 449b  9i.b.r:"y_dl..D.
-00000720: bf13 fd7c 2d4e 9cc8 5222 3412 f832 cf47  ...|-N..R"4..2.G
-00000730: c725 a0f5 7f5a b434 f1cb 9d79 c437 09c3  .%...Z.4...y.7..
-00000740: abc8 f0c9 828b 1fa8 de01 0000 ffff 0300  ................
-00000750: 504b 0304 1400 0600 0800 0000 2100 d865  PK..........!..e
-00000760: bac6 9e04 0000 0c0d 0000 0f00 0000 786c  ..............xl
-00000770: 2f77 6f72 6b62 6f6f 6b2e 786d 6ca4 575b  /workbook.xml.W[
-00000780: 6fe2 3814 7e5f 69ff 4326 db87 59a9 69e2  o.8.~_i.C&..Y.i.
-00000790: 708f 0aa3 1012 1595 9696 4b3b bbcb 2a72  p.........K;..*r
-000007a0: 1303 5673 5bc7 b454 a3f9 ef7b 1c08 2550  ..Vs[..T...{..%P
-000007b0: 6dd8 19d4 3ad8 3edf b9f9 3bc7 e1f2 cb3a  m...:.>...;....:
-000007c0: 0ca4 17c2 521a 476d 195d 68b2 4422 2ff6  ....R.Gm.]h.D"/.
-000007d0: 69b4 68cb d389 a334 6529 e538 f271 1047  i.h....4e).8.q.G
-000007e0: a42d bf91 54fe d2f9 f597 cbd7 983d 3fc5  .-..T........=?.
-000007f0: f1b3 040a a2b4 2d2f 394f 0c55 4dbd 2509  ......-/9O.UM.%.
-00000800: 717a 1127 2482 9d79 cc42 cc61 ca16 6a9a  qz.'$..y.B.a..j.
-00000810: 3082 fd74 4908 0f03 55d7 b4ba 1a62 1ac9  0..tI...U....b..
-00000820: 1b0d 063b 4547 3c9f 538f f462 6f15 9288  ...;EG<.S..bo...
-00000830: 6f94 3012 600e eea7 4b9a a4b9 b6d0 3b45  o.0.`...K.....;E
-00000840: 5d88 d9f3 2a51 bc38 4c40 c513 0d28 7fcb  ]...*Q.8L@...(..
-00000850: 94ca 52e8 19fd 4514 33fc 1440 d86b 5493  ..R...E.3..@.kT.
-00000860: d60c feea f08f 3418 f4dc 126c 1d99 0aa9  ......4....l....
-00000870: c7e2 349e f30b 50ad 6e9c 3e8a 1f69 2a42  ..4...P.n.>..i*B
-00000880: 8514 ac8f 7370 9aa6 aaca c80b 1567 b8f3  ....sp.......g..
-00000890: 8ad5 7fd0 abfa 4e57 fd5d 19d2 7e5a 1b02  ......NW.]..~Z..
-000008a0: 6a65 5c31 2079 3fa8 adb6 f34d 973b 9773  je\1 y?....M.;.s
-000008b0: 1a90 870d 7525 9c24 b738 1427 15c8 5280  ....u%.$.8.'..R.
-000008c0: 536e fb94 13bf 2d37 601a bf92 c202 5b25  Sn....-7`.....[%
-000008d0: dd15 0d60 576f 54f4 a6ac 7676 74be 6392  ...`WoT...vvt.c.
-000008e0: 4fe6 7815 f009 1039 570f 9551 afb7 f49a  O.x....9W..Q....
-000008f0: 9004 6298 0127 2cc2 9c58 71c4 8187 dbb8  ..b..',..Xq.....
-00000900: 7e96 7399 6e6b 1903 c3a5 11f9 6745 1981  ~.s.nk......gE..
-00000910: c202 7e41 ac30 62cf c04f e91d e64b 69c5  ..~A.0b..O...Ki.
-00000920: 82b6 6c19 b369 0ae1 cf16 3408 48ea 32e2  ..l..i....4.H.2.
-00000930: 518e 8359 1aaf 9847 668c 2471 3a63 78c1  Q..Y...Gf.$q:cx.
-00000940: 6948 9404 7bcf 7841 6629 f3f2 b5d9 134e  iH..{.xAf).....N
-00000950: 893b 8f03 9f30 904e 677b 05ea 7212 2650  .;...0.Ng{..r.&P
-00000960: 56b0 bac7 737c 5c54 ff83 e9d8 13e9 5321  V...s|\T......S!
-00000970: 7f9b 1837 df0f 7309 a132 2367 f31d 6712  ...7..s..2#g..g.
-00000980: 7cef f706 70a2 63fc 02e7 0b2c f2b7 e5df  |...p.c....,....
-00000990: 8703 4415 37f2 9881 dc6f 4ec5 eed6 6a0d  ..D.7....oN...j.
-000009a0: 5db1 cc8a a554 4dab a134 eb95 a662 a16e  ]....TM..4...b.n
-000009b0: b551 6dd4 5ba8 657f 8760 58dd f062 bce2  .Qm.[.e..`X..b..
-000009c0: cb2d 7584 eab6 5c05 9e1c 6ddd e075 be83  .-u...\...m..u..
-000009d0: 3463 45fd 7737 be69 db8f 229e 0743 bef7  4cE.w7.i.."..C..
-000009e0: 5d04 2c9a e403 25af e93b c9c4 545a 3fd2  ].,...%..;..TZ?.
-000009f0: c88f 5fdb b282 3468 b26f c5e9 6bb6 f948  .._...4h.o..k..H
-00000a00: 7dbe 0496 56f4 1a14 e366 ed8a d0c5 123c  }...V....f.....<
-00000a10: 467a 552c 4231 09cf da72 c1a3 dec6 2307  FzU,B1...r....#.
-00000a20: 3e8a 180a 1ea9 7b2e 65ed 185c cb9e 5294  >.....{.e..\..R.
-00000a30: 9590 bd4e 0874 7dd1 a845 8ac1 0833 8405  ...N.t}..E...3..
-00000a40: d6f7 9188 685f 76cc a1bd ef09 431a 77c2  ....h_v.....C.w.
-00000a50: faa1 f01d 6638 dc97 86b8 77d2 958c 1db9  ....f8....w.....
-00000a60: 3f64 9d95 5830 2273 c2e0 4622 e0e3 d1da  ?d..X0"s..F"....
-00000a70: 3bb8 9a81 3f02 4135 d388 f8a2 3980 8abd  ;...?.A5....9...
-00000a80: d936 5877 1d44 e185 eb50 51d3 3dcc b1a8  .6Xw.D...PQ.=...
-00000a90: 0ad1 333c 1c8c f314 00e9 96d4 f789 b822  ..3<..........."
-00000aa0: e58e c8cf a7b3 ee99 6e9c dd9f e997 ea9e  ........n.......
-00000ab0: d28f 2c74 0743 ebda 1df7 ffb4 e5ce 2603  ..,t.C........&.
-00000ac0: 1958 2b05 5a57 d3db 6bd7 1a0e f671 9572  .X+.ZW..k....q.r
-00000ad0: d870 3cd9 4720 540a e94d 47e6 a43f bc2d  .p<.G T..MG..?.-
-00000ae0: c0ca 23b3 1fcc 816b 4e27 c302 aedc 43fb  ..#....kN'....C.
-00000af0: eb1d e462 e838 637b f2f9 2ff4 f726 a1e6  ...b.8c{../..&..
-00000b00: 193a 97ae 6cb3 678f b26c 9d4b dab9 74db  .:..l.g..l.K..t.
-00000b10: 7547 c3c7 f1b9 847e 2f8d c231 adc9 61ba  uG.....~/..1..a.
-00000b20: aaa5 a82b 7330 988e 0b11 d4ca 41ef 6e16  ...+s0......A.n.
-00000b30: 90a5 c0c1 e0e6 d0c5 726b 9004 115b d1c9  ........rk...[..
-00000b40: 56a9 2d80 81b9 22aa 710a ea7e 6a8f 051d  V.-...".q..~j...
-00000b50: 8ad0 e629 5071 5805 9a97 93ef de1d 5ecb  ...)PqX.......^.
-00000b60: 9ddf 46b6 f3a9 d442 eed9 610e 0fb9 ba5f  ..F....B..a...._
-00000b70: 9350 f650 cb1e dcec e291 5d1a 2da4 e92d  .P.P......].-..-
-00000b80: d132 a063 0c52 9e3d e152 a5d0 45bb b566  .2.c.R.=.R..E..f
-00000b90: 57ab b474 a5ea 2047 a9a2 96a6 74bb f5aa  W..t.. G....t...
-00000ba0: 52eb 3995 5a03 f52c bbe6 886b 44bc f51a  R.9.Z..,...kD...
-00000bb0: 6ba1 71fe 832f 334d 3543 13cc 5770 fb8a  k.q../3M5C..Wp..
-00000bc0: 3b3e 9b1b 6274 b6ab bbc5 f966 61db b40a  ;>..bt.....fa...
-00000bd0: b7ae 31ea 8950 b6e8 ff12 1cc3 5b7d 404e  ..1..P......[}@N
-00000be0: 1476 1e4e 14b4 6e6f 2637 27ca 0eec 89fb  .v.N..no&7'.....
-00000bf0: e89c 2a6c de74 7be6 e9f2 e668 64fe 31b1  ..*l.t{....hd.1.
-00000c00: bfe6 26d4 0f13 aac2 99c3 ab47 7ef2 6afe  ..&........G~.j.
-00000c10: 43a6 f32f 0000 00ff ff03 0050 4b03 0414  C../.......PK...
-00000c20: 0006 0008 0000 0021 0032 8573 9f3a 0100  .......!.2.s.:..
-00000c30: 007b 0500 001a 0008 0178 6c2f 5f72 656c  .{.......xl/_rel
-00000c40: 732f 776f 726b 626f 6f6b 2e78 6d6c 2e72  s/workbook.xml.r
-00000c50: 656c 7320 a204 0128 a000 0100 0000 0000  els ...(........
+00000640: 0000 0000 0000 0000 ac92 4d4f c330 0c86  ..........MO.0..
+00000650: ef48 fc87 c8f7 d5dd 9010 424b 7741 48bb  .H........BKwAH.
+00000660: 2154 7e80 49dc 0fb5 8da3 241b ddbf 271c  !T~.I.....$...'.
+00000670: 1054 1a83 0347 7fbd 7efc cadb dd3c 8dea  .T...G..~....<..
+00000680: c821 f6e2 34ac 8b12 143b 23b6 77ad 8697  .!..4....;#.w...
+00000690: fa71 7507 2a26 7296 4671 ace1 c411 76d5  .qu.*&r.Fq....v.
+000006a0: f5d5 f699 474a 7928 76bd 8f2a abb8 a8a1  ....GJy(v..*....
+000006b0: 4bc9 df23 46d3 f144 b110 cf2e 571a 0913  K..#F..D....W...
+000006c0: a51c 8616 3d99 815a c64d 59de 62f8 ae01  ....=..Z.MY.b...
+000006d0: d542 53ed ad86 b0b7 37a0 ea93 cf9b 7fd7  .BS.....7.......
+000006e0: 96a6 e90d 3f88 394c ecd2 9915 c873 6267  ....?.9L.....sbg
+000006f0: d9ae 7cc8 6c21 f5f9 1a55 5368 3969 b062  ..|.l!...USh9i.b
+00000700: 9e72 3a22 795f 646c c0f3 449b bf13 fd7c  .r:"y_dl..D....|
+00000710: 2d4e 9cc8 5222 3412 f832 cf47 c725 a0f5  -N..R"4..2.G.%..
+00000720: 7f5a b434 f1cb 9d79 c437 09c3 abc8 f0c9  .Z.4...y.7......
+00000730: 828b 1fa8 de01 0000 ffff 0300 504b 0304  ............PK..
+00000740: 1400 0600 0800 0000 2100 c832 432f 7e04  ........!..2C/~.
+00000750: 0000 b80c 0000 0f00 0000 786c 2f77 6f72  ..........xl/wor
+00000760: 6b62 6f6f 6b2e 786d 6ca4 575b 6fa3 3814  kbook.xml.W[o.8.
+00000770: 7e5f 69ff 03c3 f661 572a 0593 3b6a 3222  ~_i....aW*..;j2"
+00000780: 01d4 a869 d3e6 d2ce ae22 2117 9cc4 2ab7  ...i....."!...*.
+00000790: 314e 9b6a 34ff 7d8f 4948 211d 2dd9 99a8  1N.j4.}.IH!.-...
+000007a0: 35b1 7d2e df39 fece 31b9 fcbc 0d03 e985  5.}..9..1.......
+000007b0: b094 c651 5746 179a 2c91 c88b 7d1a adba  ...QWF..,...}...
+000007c0: f27c e628 6d59 4a39 8e7c 1cc4 11e9 ca6f  .|.(mYJ9.|.....o
+000007d0: 2495 3ff7 7eff edf2 3566 cf4f 71fc 2c81  $.?.~...5f.Oq.,.
+000007e0: 8128 edca 6bce 1343 5553 6f4d 429c 5ec4  .(..k..CUSoMB.^.
+000007f0: 0989 6067 19b3 1073 98b2 959a 268c 603f  ..`g...s....&.`?
+00000800: 5d13 c2c3 40d5 35ad a986 9846 f2ce 82c1  ]...@.5....F....
+00000810: 4eb1 112f 97d4 2356 ec6d 4212 f19d 1146  N../..#V.mB....F
+00000820: 02cc 017e baa6 499a 5b0b bd53 cc85 983d  ...~..I.[..S...=
+00000830: 6f12 c58b c304 4c3c d180 f2b7 cca8 2c85  o.....L<......,.
+00000840: 9e31 5c45 31c3 4f01 84bd 450d 69cb e0af  .1\E1.O...E.i...
+00000850: 09ff 4883 41cf 3dc1 d607 5721 f558 9cc6  ..H.A.=...W!.X..
+00000860: 4b7e 01a6 d51d e80f f123 4d45 a894 82ed  K~.......#ME....
+00000870: c71c 9c66 a9ae 32f2 42c5 191e 50b1 e64f  ...f..2.B...P..O
+00000880: a26a 1e6c 35df 8d21 ed97 ad21 a056 c615  .j.l5..!...!.V..
+00000890: 0392 f793 d61a 076c badc bb5c d280 3cec  .......l...\..<.
+000008a0: a82b e124 b9c5 a138 a940 9602 9c72 dba7  .+.$...8.@...r..
+000008b0: 9cf8 5db9 05d3 f895 9416 d826 e96f 6800  ..]........&.oh.
+000008c0: bb7a abae 3764 b577 a0f3 1d93 7cb2 c49b  .z..7d.w....|...
+000008d0: 80cf 80c8 b979 a88c 66b3 b393 0462 9801  .....y..f....b..
+000008e0: 272c c29c 0ce2 8803 0ff7 71fd 2ae7 7a97  ',........q.*.z.
+000008f0: 607b b08e 81e1 d284 7cdd 5046 a0b0 805f  `{......|.PF..._
+00000900: 102b 8cd8 33f0 537a 87f9 5ada b0a0 2b0f  .+..3.Sz..Z...+.
+00000910: 8cc5 3c85 f017 2b1a 0424 7519 f128 c7c1  ..<...+..$u..(..
+00000920: 228d 37cc 230b 4692 385d 30bc 5212 ec3d  ".7.#.F.8]0.R..=
+00000930: e315 59a4 cc13 734e 43b2 78c2 2971 9771  ..Y...sNC.x.)q.q
+00000940: e013 0692 e9a2 509c 2e27 6102 2505 ab05  ......P..'a.%...
+00000950: 8ee3 8f05 f53f 588e 3d91 64f5 10df eefb  .....?X.=.d.....
+00000960: 711e 214c 66e4 4cbe e34c 82ef 436b 04a7  q.!Lf.L..L..Ck..
+00000970: 39c5 2f70 b6c0 207f 5ffa 4338 3c54 7323  9./p.. ._.C8<Ts#
+00000980: 8f19 c8fd d6ee dbd6 c076 060a b26a 9a52  .........v...j.R
+00000990: 776c a4b4 51cb 529a 564b 37f5 46db 6937  wl..Q.R.VK7.F.i7
+000009a0: f5ef 100c 6b1a 5e8c 377c bda7 8d30 dd95  ....k.^.7|...0..
+000009b0: ebc0 910f 5b37 789b ef20 cdd8 50ff 1dc6  ....[7x.. ..P...
+000009c0: 376d ff51 c4f3 68c8 f7be 8b80 4583 7ca0  7m.Q..h.....E.|.
+000009d0: e435 7d27 9898 4adb 471a f9f1 6b57 5690  .5}'..J.G...kWV.
+000009e0: 060d f6ad 3c7d cd36 1fa9 cfd7 c0d0 9ade  ....<}.6........
+000009f0: 8042 dcad 5d11 ba5a 0362 a4d7 c522 1492  .B..]..Z.b..."..
+00000a00: 40d6 954b 88ac 1d22 073e 8a18 4a88 d402  @..K...".>..J...
+00000a10: a4ac 1503 b4ec 2945 59f9 d8db 8440 c717  ......)EY....@..
+00000a20: 4d5a a418 9c30 4378 6043 1f89 888a b253  MZ...0Cx`C.....S
+00000a30: 0ead bd20 0c69 3c08 ebc7 c277 98e1 b028  ... .i<....w...(
+00000a40: 0d71 1fa4 6b19 3b72 3c50 8034 22be a867  .q..k.;r<P.4"..g
+00000a50: 4057 98ed 31ba db20 0a2f 5c87 8a32 b430  @W..1.. ./\..2.0
+00000a60: c782 cca2 cc3d 1c4c 73e4 c095 35f5 7d22  .....=.Ls...5.}"
+00000a70: 6e35 b927 c2fa 74d6 3fd3 8db3 fb33 fd52  n5.'..t.?....3.R
+00000a80: 2d18 fd91 87fe 683c b876 a7c3 7f6c b9b7  -.....h<.v...l..
+00000a90: 039e 296b 958a 83ab f9ed b53b 188f 8a7a  ..)k.......;...z
+00000aa0: b56a b5f1 7456 d440 a852 c59a 4fcc d970  .j..tV.@.R..O..p
+00000ab0: 7c5b 52ab 8ecc 7e30 47ae 399f 8d4b 7ad5  |[R...~0G.9..Kz.
+00000ac0: 08ed 2f77 908b b1e3 4ced d99f 7f4c 6ce7  ../w....L....Ll.
+00000ad0: d3b9 7465 9b96 3dc9 d274 2e69 e7d2 6ddf  ..te..=..t.i..m.
+00000ae0: 9d8c 1fa7 e712 faab 12be 630e 66c7 79aa  ..........c.f.y.
+00000af0: 576a 5d99 a3d1 7c5a 82de a856 7a87 59d2  Wj]...|Z...Vz.Y.
+00000b00: ac54 1c8d 6e8e 2156 7b83 2488 d8ca 203b  .T..n.!V{.$... ;
+00000b10: 95be 400d dc95 b55a a768 ddcf eda9 e041  ..@....Z.h.....A
+00000b20: 59b5 7d8a aa38 ac12 bfab 5977 ef8e afe5  Y.}..8....Yw....
+00000b30: 5e76 fe95 1e72 64c7 393c 2669 b118 a1de  ^v...rd.9<&i....
+00000b40: a188 3db8 85c5 236b f21d a4e9 1dd1 1fc8  ..=...#k........
+00000b50: 968f 529e 3de1 02a4 d0f5 fa8d 765f ab75  ..R.=.......v_.u
+00000b60: 74e8 f8c8 51ea a8a3 29fd 7eb3 ae34 2ca7  t...Q...).~..4,.
+00000b70: d668 21b8 121a 8e68 fbe2 0dd5 d80a 8bcb  .h!....h........
+00000b80: 9f7c f168 ab99 36c1 7c03 b7a5 b88f b3b9  .|.h..6.|.......
+00000b90: 2146 67bf 7a58 5cee 16f6 ddaa 744b 1a13  !Fg.zX\.....tK..
+00000ba0: 4b84 b2d7 fe2f c129 bc81 07e4 4461 e7e1  K..../.)....Da..
+00000bb0: 44c1 c1ed cdec e644 d991 3d73 1f9d 5385  D......D..=s..S.
+00000bc0: cd9b be65 9e2e 6f4e 26e6 df33 fb4b ee42  ...e..oN&..3.K.B
+00000bd0: fd61 4255 3873 7855 c84f 5ecd 7f74 f4fe  .aBU8sxU.O^..t..
+00000be0: 0500 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+00000bf0: 0000 0021 00a1 890e 7a25 0100 00e1 0400  ...!....z%......
+00000c00: 001a 0008 0178 6c2f 5f72 656c 732f 776f  .....xl/_rels/wo
+00000c10: 726b 626f 6f6b 2e78 6d6c 2e72 656c 7320  rkbook.xml.rels 
+00000c20: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
+00000c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000d50: 0000 0000 0000 0000 0000 00bc 944d 4ec3  .............MN.
-00000d60: 3010 85f7 48dc 21f2 9eb8 49a1 fca8 4917  0...H.!...I...I.
-00000d70: 20a4 4ab0 81f6 0023 679a 4449 ecc8 3340   .J....#g.DI..3@
-00000d80: 737b ac00 4d2a 5566 1375 6369 9ee5 f73e  s{..M*Uf.uci...>
-00000d90: cdd8 5eae f64d 1d7c a2a5 d2e8 4444 e14c  ..^..M.|....DD.L
-00000da0: 04a8 95c9 4a9d 2762 bb79 beba 1301 31e8  ....J.'b.y....1.
-00000db0: 0c6a a331 111d 9258 a597 17cb 37ac 81dd  .j.1...X....7...
-00000dc0: 212a ca96 02e7 a229 1105 73fb 2025 a902  !*.....)..s. %..
-00000dd0: 1ba0 d0b4 a8dd cece d806 d895 3697 2da8  ............6.-.
-00000de0: 0a72 94f1 6cb6 9076 ec21 d223 cf60 9d25  .r..l..v.!.#.`.%
-00000df0: c2ae 3397 bfe9 5a97 fcbf b7d9 ed4a 854f  ..3...Z......J.O
-00000e00: 467d 34a8 f944 84a4 0291 5f91 2103 0667  F}4..D...._.!..g
-00000e10: 0c36 474e 44f3 ab84 0e56 c8d3 1cf3 2939  .6GND....V....)9
-00000e20: be8c ad7a 9681 e120 d10f e5dc 0773 3b6d  ...z... .....s;m
-00000e30: 53c0 62f6 ced6 cd9c 0620 2a46 b20f 263e  S.b...... *F..&>
-00000e40: 7367 621f 4c74 6698 c807 b398 744c dcd5  sgb.Ltf.....tL..
-00000e50: eef1 1d2e 2df5 b52f fe66 ca78 764f 1a87  ....-../.f.xvO..
-00000e60: f4be 94fd ea6d c1f5 940c b867 b41a ea97  .....m.....g....
-00000e70: 5257 03ca 5825 39ae bc64 f753 9229 a8d5  RW..X%9..d.S.)..
-00000e80: 6301 a51e b00e d2df 88e4 d197 997e 0300  c............~..
-00000e90: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00000ea0: 0021 001b 2784 8817 0600 0025 1200 0018  .!..'......%....
-00000eb0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00000ec0: 2f73 6865 6574 312e 786d 6cac 55db 8eda  /sheet1.xml.U...
-00000ed0: 3010 7daf d47f 88fc 4e82 73e3 22c2 8a4b  0.}.....N.s."..K
-00000ee0: 5157 da87 d56e 2fcf 2671 c0da 244e 6db3  QW...n/.&q..$Nm.
-00000ef0: 40ab fe7b c7ce 0576 d922 d856 02ec 3899  @..{...v.".V..8.
-00000f00: 3367 ce9c 09a3 9b5d 9e59 cf54 48c6 8b08  3g.....].Y.TH...
-00000f10: 61bb 8b2c 5ac4 3c61 c52a 425f bf2c 3a7d  a..,Z.<a.*B_.,:}
-00000f20: 6449 458a 8464 bca0 11da 5389 6ec6 1f3f  dIE..d....S.n..?
-00000f30: 8cb6 5c3c c935 a5ca 0284 4246 68ad 5439  ..\<.5....BFh.T9
-00000f40: 741c 19af 694e a4cd 4b5a c09d 948b 9c28  t...iN..KZ.....(
-00000f50: b814 2b47 9682 92c4 04e5 99e3 76bb a193  ..+G........v...
-00000f60: 1356 a00a 6128 2ec1 e069 ca62 3ae7 f126  .V..a(...i.b:..&
-00000f70: a785 aa40 04cd 8802 fe72 cd4a d9a0 e5f1  ...@.....r.J....
-00000f80: 2570 3911 4f9b b213 f3bc 0488 25cb 98da  %p9.O.......%...
-00000f90: 1b50 64e5 f1f0 7655 7041 9619 d4bd c33e  .Pd...vUpA.....>
-00000fa0: 89ad 9d80 8f0b 5faf 4963 ce4f 32e5 2c16  ......_.Ic.O2.,.
-00000fb0: 5cf2 54d9 80ec 549c 4fcb 1f38 0387 c42d  \.T...T.O..8...-
-00000fc0: d269 fd17 c160 df11 f499 e906 1ea0 dcf7  .i...`..........
-00000fd0: 51c2 418b e51e c0bc 7782 852d 9896 4b0c  Q.A.....w..-..K.
-00000fe0: 372c 89d0 af69 309d b9f3 20e8 f4bb dea0  7,...i0... .....
-00000ff0: e37f 1af4 3b83 0586 cbc9 7431 f0e6 5337  ....;.....t1..S7
-00001000: 7027 bfd1 7864 7c72 2fc6 23be 5119 2be8  p'..xd|r/.#.Q.+.
-00001010: bdb0 e426 8786 eda7 34e3 db08 8155 eb83  ...&....4....U..
-00001020: 07b6 5a2b 7de0 8c47 4e1b 9730 b088 96c5  ..Z+}..GN..0....
-00001030: 1234 8dd0 040f 1f43 fd84 79e0 1ba3 5b79  .4.....C..y...[y
-00001040: b4b7 1459 3ed2 8cc6 8a02 498c 2ced ef25  ...Y>.....I.,..%
-00001050: e74f fac1 5b38 ea02 a592 14d4 da3d 96e0  .O..[8.......=..
-00001060: 9208 8140 fbc3 56f1 f28e a66a 46b3 2c42  ...@..V....jF.,B
-00001070: 33a8 97c4 8a3d d37b 8888 d092 2bc5 73c3  3....=.{....+.s.
-00001080: d24c 9382 b354 f09f b430 7c4c 5acd 53e3  .L...T...0|LZ.S.
-00001090: 4708 a0ea 472b 8c1a 1338 c91f a692 197e  G...G+...8.....~
-000010a0: 2bac 4aa2 4934 c9ab c009 90a9 0361 abeb  +.J.I4.......a..
-000010b0: 7f95 ef05 bb17 290f 9150 51ab ad56 a4d1  ......)..PQ..V..
-000010c0: f958 c685 1975 6853 4253 b2c9 d403 df7e  .X...uhSBS.....~
-000010d0: a655 67b0 6ffb c8aa 1b79 479f 6936 e3a0  .Ug.o....yG.i6..
-000010e0: 1394 64e6 6798 ece7 54c6 30d0 a0b3 6d52  ..d.g...T.0...mR
-000010f0: c53c 83f6 c0af 9533 fd62 8279 24bb aa31  .<.....3.b.y$..1
-00001100: 2c51 eb08 01b7 2595 6aa1 5b01 77e3 8d04  ,Q....%.j.[.w...
-00001110: 89bf 57f7 8c3e 6d2c 34ca c4c2 baad eebb  ..W..>m,4.......
-00001120: be1d 867e 3774 83b3 8190 c204 02f5 3ab0  ...~7t........:.
-00001130: 6ff7 fb61 0ff7 7b10 28d5 5ebf 187a 5a98  o..a..{.(.^..zZ.
-00001140: 3617 9c9b 1058 df08 7945 f285 20ba 8a63  6....X..yE.. ..c
-00001150: a4b0 4682 f5ef c931 50bb 06b4 5783 c27a  ..F....1P...W..z
-00001160: 0614 06eb 1a50 f887 3035 c37a 06f4 b447  .....P..05.z...G
-00001170: 67cb 1fd4 a0b0 5eaa 3d6e 4da2 c7b7 7682  g.....^.=nM...v.
-00001180: 677b 9edb f5b0 6e75 ddb1 6b45 c38d 81f4  g{....nu..kE....
-00001190: e6ff c986 1b7b e94d 4317 db41 e087 c7fe  .....{.MC..A....
-000011a0: d255 5dd3 0d5d 5d35 2a07 dbfa 76af d7f3  .U]..]]5*...v...
-000011b0: 7c4f dbf6 cca0 e0c6 bd7a 5333 3a13 7ab6  |O.......zS3:.z.
-000011c0: 7fb8 f1af defc e328 e0c6 b6f8 e086 2b79  .......(......+y
-000011d0: 39e6 7df2 0700 00ff ff00 0000 ffff ac95  9.}.............
-000011e0: db72 8230 1086 5fc5 c903 1402 72d0 4166  .r.0.._.....r.Af
-000011f0: aa88 0714 4f4f c050 667a a374 84da f6ed  ....OO.Pfz.t....
-00001200: 1b48 1ab2 4ba6 f4a2 77fa e7cb ee9f dd64  .H..K...w......d
-00001210: 09aa d7a2 a8a3 acce c2e0 5e7e 8cee 3342  ..........^~..3B
-00001220: c9a8 7acb 6e15 fb35 a513 f6a7 95f2 f7aa  ..z.n..5........
-00001230: 2eaf 7179 bf66 752b 7cd2 7196 4f5f bea2  ..qy.fu+|.q.O_..
-00001240: a2ca 8b1b d3cc 279b 8441 de84 786e 62cc  ......'..A..xnb.
-00001250: 884f 0c21 cc7f 8411 032b 863d 422b 301e  .O.!.....+.=B+0.
-00001260: 6160 e482 5870 c225 1de1 d810 8938 c22c  a`..Xp.%.....8.,
-00001270: c920 6348 2c71 de98 0bd4 924e 5642 71a4  . cH,q.....NVBq.
-00001280: b216 8a27 958d c68b 0333 2562 932d 37ed  ...'.....3%b.-7.
-00001290: 84e2 4a65 2f94 ae0c a950 d423 d0ee 9406  ..Je/....P.#....
-000012a0: eb80 6c83 f50f 6d68 62b4 cd92 05f3 514d  ..l...mhb.....QM
-000012b0: e77d 0411 0b4e a88d c17d 1924 96fd 2ca8  .}...N...}.$..,.
-000012c0: 9eb1 206c a5b9 2e2c f94a 20aa 130f 226b  .. l...,.J ..."k
-000012d0: 81f8 4a14 1f22 9b41 b3db be59 179d 3819  ..J..".A...Y..8.
-000012e0: 76bb 1b76 bb1f 769b f6bd 5074 e70f 1a04  v..v..v...Pt....
-000012f0: 15f7 38d8 e493 e6cc 28c8 b98f 78a8 fc17  ..8.....(...x...
-00001300: 0dd2 951f dc6e d667 3064 7e9d 26ea a5f0  .....n.g0d~.&...
-00001310: d1f1 e7ea e204 cd94 26cb 8c78 ea4c 4163  ........&..x.LAc
-00001320: 27d2 2078 a8a8 19a8 0953 c47c 3f1d 2b39  '. x.....S.|?.+9
-00001330: 2845 1757 30a6 ca20 1f6b c1b0 0121 df2a  (E.W0.. .k...!.*
-00001340: 450f 60a3 f18a 90ad c68e 8bce 9368 1807  E.`..........h..
-00001350: 7572 a7b1 eca0 97b4 d758 7650 0752 f09e  ur.......XvP.R..
-00001360: 51ed 0e60 1115 ed08 1651 b54e eaa2 876a  Q..`.....Q.N...j
-00001370: 7006 8bc8 d045 5df4 3b43 e072 b209 f3e7  p....E].;C.r....
-00001380: cbb9 6c60 3663 a91c fb09 57ac f67b c2e3  ..l`6c....W..{..
-00001390: 1add 57f6 1b00 00ff ff00 0000 ffff 6c51  ..W...........lQ
-000013a0: 4d4f 8340 10fd 2b9b 49d3 6862 e5ab d842  MO.@..+.I.hb...B
-000013b0: 8104 4492 1e34 d15e bcae 6581 8d94 5d87  ..D..4.^..e...].
-000013c0: 415b 8dff dda5 b589 076f f3e6 e3bd 9937  A[.......o.....7
-000013d0: 111f 4815 b225 810c 4515 43e6 868f 2eb0  ..H..%..E.C.....
-000013e0: 3d86 832c 63f8 cafc ecd6 cd7d 7fb6 b4bd  =..,c......}....
-000013f0: 6036 bf0b 96b3 a070 0c4c b322 f0f2 ccf5  `6.....p.L."....
-00001400: ddf4 1bac 24da aaae 9424 55c7 db42 e18e  ....$....$U..B..
-00001410: 13c9 ae66 fddb 9135 f5c2 e722 776c db06  ...f...5..."wl..
-00001420: d359 3d0d ad60 74d0 2206 b1d7 28fa decc  .Y=..`t."...(...
-00001430: 012b f7d5 da68 dac0 344a 8592 0e31 3866  .+...h..4J...18f
-00001440: a032 7c43 cb93 f421 bf98 64de b4a5 d5b4  .2|C...!..d.....
-00001450: a6d5 2473 afd8 1f0c 7019 59e7 dec8 3ac9  ..$s....p.Y...:.
-00001460: 2426 f86f b324 d2bc 16f7 1c6b d9f5 ac15  $&.o.$.....k....
-00001470: 1519 e1eb 0530 9475 738e 49e9 63d6 07f6  .....0.us.I.c...
-00001480: a288 d4ee 8c1a c14b 8123 f280 554a 19fb  .......K.#..UJ..
-00001490: 4ec0 1831 f26e 040d 9a69 ae05 6ee4 a739  N..1.n...i..n..9
-000014a0: 3300 660e 121d f1d1 a218 b442 422e 0958  3.f........BB..X
-000014b0: 63f2 9fca 14da 5ccb 18e6 6e30 0f6e 166e  c.....\...n0.n.n
-000014c0: 6088 df05 92dc fe16 8c2b 188e 2fc1 75e9  `........+../.u.
-000014d0: 8c86 5b1f 0a5f fb46 084a 7e00 0000 ffff  ..[.._.F.J~.....
-000014e0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-000014f0: 9ed3 3f9d cb0b 0000 5c55 0000 1800 0000  ..?.....\U......
-00001500: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00001510: 6565 7432 2e78 6d6c 9c94 596f e230 10c7  eet2.xml..Yo.0..
-00001520: df57 daef 10f9 3d77 424b 44a8 38b5 95aa  .W....=wBKD.8...
-00001530: 55d5 eef1 6c9c 09b1 88e3 ac6d 0ab4 daef  U...l......m....
-00001540: bee3 70b4 8817 b612 214e 98f9 cd7f 2e06  ..p.....!N......
-00001550: 775b 513b 2fa0 3497 4d4e 422f 200e 344c  w[Q;/.4.MNB/ .4L
-00001560: 16bc 59e6 e4e7 8fb9 7b4b 1c6d 6853 d05a  ..Y.....{K.mhS.Z
-00001570: 3690 931d 6872 37fc fa65 b091 6aa5 2b00  6...hr7..e..j.+.
-00001580: e320 a1d1 39a9 8c69 33df d7ac 0241 b527  . ..9..i3....A.'
-00001590: 5b68 f097 522a 410d 3eaa a5af 5b05 b4e8  [h..R*A.>...[...
-000015a0: 9c44 ed47 41d0 f305 e50d d913 3275 0d43  .D.GA.......2u.C
-000015b0: 9625 6730 956c 2da0 317b 8882 9a1a d4af  .%g0.l-.1{......
-000015c0: 2bde ea23 4db0 6b70 82aa d5ba 7599 142d  +..#M.kp....u..-
-000015d0: 2216 bce6 66d7 4189 2358 76bf 6ca4 a28b  "...f.A.#Xv.l...
-000015e0: 1af3 de86 0965 ce56 e127 c22b 3e86 e9de  .....e.V.'.+>...
-000015f0: 5f44 129c 29a9 6569 3c24 fb7b cd97 e9f7  _D..).ei<$.{....
-00001600: fdbe 4fd9 8974 99ff 5598 30f1 15bc 70db  ..O..t..U.0...p.
-00001610: c077 54f4 3949 617a 6245 efb0 f893 b0de  .wT.9IazbE......
-00001620: 0966 cba5 b235 2f72 f216 c4e9 64dc 9bc4  .f...5/r....d...
-00001630: 6e2f 0c23 3799 8da6 ee78 3699 b9a3 b43f  n/.#7....x6....?
-00001640: 4b67 7114 05e9 f42f 190e 0a8e 1db6 5939  Kgq..../......Y9
-00001650: 0aca 9c8c c2ec 21ba 21fe 70d0 0dd0 2f0e  ......!.!.p.../.
-00001660: 1bfd e1ec bc4a 299e 19ad e1bb 9db8 1a67  .....J)........g
-00001670: 39c0 59b6 53ba 9072 65cd ef31 7a80 e096  9.Y.S..re..1z...
-00001680: 36e0 6c9f 5bec 355a 1167 7738 62c6 46b6  6.l.[.5Z.gw8b.F.
-00001690: 0f50 9a09 d408 18a3 6aca 0c7f 8147 f4c8  .P......j....G..
-000016a0: c942 1a23 c513 5f56 a6db 0983 ef4a 255f  .B.#.._V.....J%_
-000016b0: a1e9 5441 0d68 8c72 f73e 0746 8aa6 7fba  ..TA.h.r.>.F....
-000016c0: 04c6 e9b9 9995 9113 8c78 20fe 97db 5e8b  .........x ...^.
-000016d0: d57a d478 65bc b324 ce42 62b6 47a5 b155  .z.xe..$.Bb.G..U
-000016e0: ea9f eafc f17c acf9 bcdb eb47 e514 50d2  .....|.....G..P.
-000016f0: 756d 9ee4 e61b d8d2 6049 132f c17e db85  um......`I./.~..
-00001700: c98a dd14 34c3 4dc5 d27b 1d96 c91a 19f8  ....4.M..{......
-00001710: ed08 6eff 7170 d1e8 b6bb 6f78 61aa 9c44  ..n.qp....oxa..D
-00001720: a997 a649 eff6 c696 ceec ecf2 4578 646b  ...I........Exdk
-00001730: 8dd5 ffbd b709 adc0 1303 9577 0cbc 1f18  ...........w....
-00001740: 61e4 c571 14c4 a1f5 5c80 36f3 43af 2f29  a..q....\.6.C./)
-00001750: 7e27 e81f 0000 00ff ff00 0000 ffff cc5c  ~'.............\
-00001760: 6d6f db36 10fe 2baa 1a14 b1e7 d596 9dc4  mo.6..+.........
-00001770: 719b 64b0 f852 a771 ec36 8ebb 61c3 1018  q.d..R.q.6..a...
-00001780: 99b3 0d68 b3c2 09fa f2ef 77a4 684b a249  ...h......w.hK.I
-00001790: e9a8 d076 bff4 85b9 239f e744 3d3c f2a8  ...v....#..D=<..
-000017a0: 9c3c fc33 9f3f d2d9 e3ec ec64 f1df d760  .<.3.?.....d...`
-000017b0: 711a 4661 f0f0 7976 ff00 ff7a 15b5 c3e0  q.Fa..yv...z....
-000017c0: 5b74 30bb 7df5 d777 3a7f b89d df3f 9e86  [t0.}..w:....?..
-000017d0: ad97 9df0 ece4 56d8 f685 f169 d86e 41c3  ......V....i.nA.
-000017e0: 5d70 3b13 de67 a3f8 e6fd 944d aecf c7a3  ]p;..g.....M....
-000017f0: c949 f3ee ece4 cb59 74d2 fc72 76d2 bc55  .I.....Yt..rv..U
-00001800: 6e71 e276 1c06 d0dd 03f8 7e39 3b3a ca9b  nq.v......~9;:..
-00001810: 90a5 4953 f950 3554 142e 5bd8 5a0b 5f6b  ..IS.P5T..[.Z._k
-00001820: 799b b4c0 9fab 918e 0ff3 235d 184c 3430  y.........#].L40
-00001830: 4365 2278 af68 4ea6 97fb 63ce 27ec 7a9f  Ce"x.hN...c.'.z.
-00001840: fdf6 8e35 8256 2320 e3c9 75ad a648 b756  ...5.V# ..u..H.V
-00001850: e334 21b4 abf8 4248 f1f1 15c6 10df b616  .4!...BH........
-00001860: 5fde 27d7 b6d8 2a17 15dc c745 d6f5 9cef  _.'...*....E....
-00001870: 93f1 707a 39da ef47 b517 7f3f be86 6735  ..pz9..G...?..g5
-00001880: 1c5e 4e1a 4118 3682 259b 6f9f e7cf f6e2  .^N.A.6.%.o.....
-00001890: bda8 110c 589f b2ab 9bc9 f9ef eca7 d4f1  ....X...........
-000018a0: 67f8 0978 dd40 cb8a 2c4c 98af f3c5 c31f  g..x.@..,L......
-000018b0: fffe f9f2 e3c7 4f37 c97f 5fde cf3e cdb5  ......O7.._..>..
-000018c0: e78a 8317 5785 078e 0678 3065 5693 8fe2  ....W....x0eV...
-000018d0: 1090 aa08 c0b1 0401 c321 a055 1180 6309  .........!.U..c.
-000018e0: 028e 43c0 aa22 00c7 1204 6f8d 08e0 259d  ..C.."....o...%.
-000018f0: 2d16 b3ef 6130 4bc4 2458 ccef 4e43 61ac  -...a0K.$X..NCa.
-00001900: c425 9dc1 e705 e0e4 fba8 262c d865 b034  .%........&,.e.4
-00001910: 0298 bcd1 72da 66e7 c545 1e91 54a5 e36e  ....r.f..E..T..n
-00001920: 7ef6 0e13 9b0e a89c 5d08 5a0d 3abd ea0b  ~.......].Z.:...
-00001930: f9ab d59a c747 072d 1002 a982 1641 e8b8  .....G.-.....A..
-00001940: 0882 3006 4180 bf52 e9d4 40c6 894d 6232  ..0.A..R..@..Mb2
-00001950: 87c8 7d92 b20c 802d e115 0e2a bcfd 0fec  ..}....-...*....
-00001960: aaff 8641 940b c560 f5fe 3702 5090 abf1  ...A...`..7.P...
-00001970: af93 5a23 88f7 da25 1ad2 0896 9149 fd96  ..Z#...%.....I..
-00001980: 6af9 9c9e 7f68 b69e 696a e14a 85f8 a142  j....h..ij.J...B
-00001990: fc53 a1ae 5484 8387 a742 fd53 61ae 5484  .S..T....B.Sa.T.
-000019a0: 8307 2acc 3f15 ee4a 4538 78a0 c2fd 5319  ..*.?..JE8x...S.
-000019b0: 2869 38c8 4843 944a 432e 0701 1b7c 0e22  (i8.HC.JC....|."
-000019c0: 8c75 c939 d612 bac4 2619 1a25 3960 ba25  .u.9....&..%9`.%
-000019d0: c911 3919 566e 5c69 103f 3430 72e3 4083  ..9.Vn\i.?40r.@.
-000019e0: bad2 100e 5b92 1a07 1acc 9586 70d8 92cc  ....[.......p...
-000019f0: 38d0 e0ae 3484 c396 24c6 81c6 40c9 c081  8...4...$...@...
-00001a00: d87f e5c4 e4d0 454c 84b1 2626 912e 26ca  ......EL..&&..&.
-00001a10: 46ea d85c 665a b6c4 052c 55a4 c878 3aba  F..\fZ...,U..x:.
-00001a20: 4ed3 16b5 3d91 9bb2 b793 f1e8 667c 0119  N...=.......f|..
-00001a30: caf5 d594 d59a 86fd e9f3 51ff 92fd a2e5  ..........Q.....
-00001a40: 1e68 1864 9330 281a 86b0 dc58 3418 1a86  .h.d.0(....X4...
-00001a50: b0dc 180c 8e86 212c 3706 63a0 60e4 d6da  ......!,7.c.`...
-00001a60: 9e79 bf7f e4f2 7a08 6378 3da0 fb55 7adf  .y....z.cx=..Uz.
-00001a70: 4eb7 0df2 cc25 4e6c 1293 e4f5 503c e3c3  N....%Nl....P<..
-00001a80: 3a76 6e5b fb20 e83e a8b5 0f8a ee83 59fb  :vn[. .>......Y.
-00001a90: 60e8 3eb8 b50f 8eee 63a0 e2be 2e6e 5d97  `.>.....c....n].
-00001aa0: a727 8c35 71d3 1f9e 3241 681b 5896 cfdf  .'.5q...2Ah.X...
-00001ab0: f759 618b f7e0 dc4a ee34 9f5f 31ae 6fa5  .Ya....J.4._1.o.
-00001ac0: d023 13f7 9149 d1c8 143d b2b0 74e4 4c8b  .#...I...=..t.L.
-00001ad0: 4666 e891 85a5 e3c8 ac68 648e 1e59 583a  Ff.......hd..YX:
-00001ae0: 8ecc 8b46 1ea8 91b3 d2d4 4ecf 5f73 2b37  ...F......N._s+7
-00001af0: 9c11 e2b7 01c2 5893 26fd 5837 3131 2953  ......X.&.X711)S
-00001b00: b71e 17cd 4dab 23e9 d649 8123 b53a d26e  ....M.#..I.#.:.n
-00001b10: 9d16 3832 ab23 ebd6 5981 23b7 3af2 6e9d  ..82.#..Y.#.:.n.
-00001b20: 1738 0e54 fcd6 25a6 e7f2 1484 b126 31ed  .8.T..%......&1.
-00001b30: b6b6 1953 3608 8d01 cbfc dc9b 2ccf 7db2  ...S6.......,.}.
-00001b40: 0954 2232 2279 6aa8 53a1 ec4f c960 3aba  .T"2"yj.S..O.`:.
-00001b50: 9848 1d4a f2ab 780f 123a ab0c a1c1 918d  .H.J..x..:......
-00001b60: 8023 45e0 281a 9cb0 f41f 395a 048e a1c1  .#E.(.....9Z....
-00001b70: 094b ffe0 5811 388e 0627 2cfd 83e3 45e0  .K..X.8..',...E.
-00001b80: 060a 5c4e 123b e66c 2d6a b9bc 8dd2 5acf  ..\N.;.l-j....Z.
-00001b90: d70e f462 97e8 f234 34c9 62af 1e17 bd2b  ...b...44.b....+
-00001ba0: aa7b 8327 e9d5 4981 27b5 7bd2 5e9d 1678  .{.'..I.'.{.^..x
-00001bb0: 32bb 27eb d559 8127 b77b f25e 9d17 780e  2.'..Y.'.{.^..x.
-00001bc0: 9661 cc3d a0b4 4c97 5bb3 22b7 faa4 aa08  .a.=..L.[.".....
-00001bd0: 66cf cbdb 5a75 2f96 5dc2 5344 08a6 302d  f...Zu/.].SD..0-
-00001be0: 99bd ad46 2629 5b1d 882f 15b3 d5c8 e8a5  ...F&)[../......
-00001bf0: dc90 1a4c 208b a763 22ce d443 51a4 6b85  ...L ..c"..CQ.k.
-00001c00: b526 94e3 9665 0453 7287 a740 7646 8114  .&...e.Sr..@vF..
-00001c10: 52a0 780a d274 274f 8116 5260 780a d274  R.x..t'O..R`x..t
-00001c20: 2714 5821 058e a720 4d77 4281 1752 182c  '.X!... MwB..R.,
-00001c30: 29e4 d4c4 7210 2e2e 3838 dc76 5025 c29c  )...r...88.vP%..
-00001c40: 9ae8 a757 b24b a49a a475 4d75 7eb5 967f  ...W.K...uMu~...
-00001c50: f953 939b fe88 debc 83e2 9e93 ae28 c6e5  .S...........(..
-00001c60: d248 04ef ad4d 0733 9932 8541 93a1 3f00  .H...M.3.2.A..?.
-00001c70: 9932 ad41 9361 3f00 9932 d541 93e1 3f00  .2.A.a?..2.A..?.
-00001c80: 9932 fd51 6472 fa63 391c 8c44 d10e 7fdb  .2.Qdr.c9..D....
-00001c90: 4a95 f8b2 fad3 d14f 9864 9748 fd49 8b99  J......O.d.H.I..
-00001ca0: 1bd4 9f61 7ff4 46a4 3277 0b44 1ea3 1862  ...a..F.2w.D...b
-00001cb0: f466 fbe0 cbf4 050d 9e8a 87b4 79b1 cc45  .f..........y..E
-00001cc0: be4c 4fd0 e0d9 0ec0 97e9 071a 3cdf 01f8  .LO.........<...
-00001cd0: 32bd 3014 ee3b 9613 bb48 54e1 f07a a16a  2.0..;...HT..z.j
-00001ce0: 7639 bdd0 4f8b 6497 48bd 482b 935b d08b  v9..O.d.H.H+.[..
-00001cf0: f93d 422f 1443 8c5e 6c1f 7c99 5ea0 c153  .=B/.C.^l.|.^..S
-00001d00: f190 b6a7 1732 f265 7a81 06cf 7600 be4c  .....2.ez...v..L
-00001d10: 2fd0 e0f9 0ec0 97e9 c5aa 129f 1609 3bb6  /.............;.
-00001d20: e32c 51a8 c4eb 852a 6b76 5677 ace3 2869  .,Q....*kvVw..(i
-00001d30: 3a5c b510 d522 cfb1 6541 92ae b5b0 b516  :\..."..eA......
-00001d40: bed6 3250 2ded f503 f1c8 a964 2aad f5fb  ..2P-......d*...
-00001d50: 4969 ba95 d44c 9551 9646 52f2 cbd2 d05b  Ii...L.Q.FR....[
-00001d60: 98f2 4a6d 78b6 257f 2c95 2d14 4247 c5b7  ..Jmx.%.,.-.BG..
-00001d70: e60d 85c2 23ed 5a7a 1c25 469d dcdd 7ab8  ....#.Zz.%F...z.
-00001d80: 74be b1bb 9983 fe70 3885 abe0 cb1b 9deb  t......p8.......
-00001d90: f7d8 652c 8957 6098 ab4f 4860 d42b 30cc  ..e,.W`..OH`.+0.
-00001da0: bd49 2430 e615 18e6 1624 1218 f70a 0c73  .I$0.....$.....s
-00001db0: a7b1 1c58 fead ca56 284b df2a 5561 cbaa  ...X...V(K.*Ua..
-00001dc0: 976a ea65 ef6b c39b 65ba 03a4 eda3 4864  .j.e.k..e.....Hd
-00001dd0: f285 c98f f0a5 465f 989f 085f 66f4 8529  ......F_..._f..)
-00001de0: 84f0 e546 5f78 cac5 bef9 9067 cb91 a521  ...F_x.....g...!
-00001df0: 3794 238f d712 ccc4 282f 647a fec8 8c1f  7.#.....(/dz....
-00001e00: 9d54 be67 aecf 33b8 0866 9533 cff0 aa28  .T.g..3..f.3...(
-00001e10: 9a1d 1e8d 3cc3 aba2 6b76 78cc 37bc 2aea  ....<...kvx.7.*.
-00001e20: 6687 c77d c3ab a271 4678 f94f c2b2 45c7  f..}...qFx.O..E.
-00001e30: b277 0e3e b653 5700 961f c2c5 cb26 4de6  .w.>.SW......&M.
-00001e40: 7a18 9933 fa92 08e3 4b8d be30 6331 3267  z..3....K..0c12g
-00001e50: f485 e984 9139 a32f 3c6b 0799 6b67 cb88  .....9./<k..kg..
-00001e60: a521 3754 11bb fab9 9bec 31dd 4723 3ebb  .!7T......1.G#>.
-00001e70: 111e 6a53 b7e9 ef6e d887 fef0 a63f bd1e  ..jS...n.....?..
-00001e80: 636f c23b b321 9ed8 60e4 d395 0d75 6623  co.;.!..`....uf#
-00001e90: 3d3c 3c1b 8cda bab2 61ce 6ca4 8707 3618  =<<.....a.l...6.
-00001ea0: 7176 65c3 9dd9 480f 0f6c 305a eec0 26af  qve...H..l0Z..&.
-00001eb0: e8d9 ba62 a9bc acca 8ae2 4be8 355d 497e  ...b......K.5]I~
-00001ec0: 2aae 3397 7ec8 071f 0adb 8e89 3c27 5886  *.3.~.......<'X.
-00001ed0: c014 e458 0257 7205 a694 03f1 c3a1 a28c  ...X.Wr.........
-00001ee0: 1424 620e 1ca8 1f0e 15c5 a320 5b73 e0c0  .$b........ [s..
-00001ef0: fc70 a828 1905 299d 0307 ee87 4345 a140  .p.(..).....CE.@
-00001f00: e47d d9ea 5fa9 4aac 8a7f 69de a79a f279  .}.._.J...i....y
-00001f10: 5fbb 8dca fb4c bef0 f261 b6b7 e2f3 6371  _....L...a....cq
-00001f20: 0b35 372e 4c7a 54de 67f2 85c9 86ca fb4c  .57.LzT.g......L
-00001f30: bef0 905d f2be 6c01 a534 e4a6 fa89 7ebd  ...]..l..4....~.
-00001f40: 0f0e 30b1 da16 0b5b cb31 fe36 f459 dd26  ..0....[.1.6.Y.&
-00001f50: 6b04 c5bf eaa1 1118 d53d 7cf1 f1f1 7514  k........=|...u.
-00001f60: daf6 d10e 7120 7ee2 5059 e337 1907 ea10  ....q ~.PY.7....
-00001f70: 0769 fbf4 f950 799d d864 1c98 431c a4ed  .i...Py..d..C...
-00001f80: d3e3 5079 add9 641c b843 1ca4 edd3 e350  ..Py..d..C.....P
-00001f90: 79bd da50 1cf2 9971 b622 552a c0eb 0529  y..P...q."U*...)
-00001fa0: f16d dcda da03 c28a 5af3 4cbe 2046 a835  .m......Z.L. F.5
-00001fb0: cfe4 0b2f 306a cd33 f9c2 a447 ad79 265f  .../0j.3...G.y&_
-00001fc0: 9828 2e6b 5eb6 9e56 1a72 f529 9cf8 5d47  .(.k^..V.r.)..]G
-00001fd0: ebbf b8a9 9dfc 14b7 1901 db1d 2e76 9175  .............v.u
-00001fe0: a1c2 7320 82ef d339 545e a86c 1ca8 c373  ..s ...9T^.l...s
-00001ff0: 90b6 3b5c 646c 1c98 0307 69bb c305 c2c6  ..;\dl....i.....
-00002000: 813b 7090 b63b 1477 0387 bc30 bb54 b0db  .;p..;.w...0.T..
-00002010: ab0a 76ba 1951 4dda 66e4 0825 cc26 5f78  ..v..QM.f..%.&_x
-00002020: f950 c26c f285 498f 1266 932f 4c36 9430  .P.l..I..f./L6.0
-00002030: 9b7c e121 6384 b999 feda bdff 0100 00ff  .|.!c...........
-00002040: ff00 0000 ffff 448c 410e 8230 1045 afd2  ......D.A..0.E..
-00002050: cc01 4411 2535 9495 1b17 ae38 410d 433b  ..D.%5.....8A.C;
-00002060: 513b cd30 8684 d30b 26c4 dd7f ef27 afc9  Q;.0....&....'..
-00002070: 3ee0 dd4b a034 9a17 0eea 60bf abc1 0885  >..K.4....`.....
-00002080: b86d e5fc b327 300f 56e5 f746 117d 8fb2  .m...'0.V..F.}..
-00002090: d211 ccc0 ac1b 146d b376 3bd4 4f36 d967  .......m.v;.O6.g
-000020a0: 948e 6674 60c1 b010 26f5 4a9c 1c64 1615  ..ft`...&.J..d..
-000020b0: 4f0a 262e 7ee6 e578 5d33 39a8 4a5b d973  O.&.~..x]39.J[.s
-000020c0: 5dda 252c 17ea 1dc8 ad3f c0d2 edc5 4f94  ].%,.....?....O.
-000020d0: c2df 96ab 2d26 96e7 1811 b5fd 0200 00ff  ....-&..........
-000020e0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-000020f0: 0087 7b5f d3f5 0400 00ca 1000 0018 0000  ..{_............
-00002100: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00002110: 6865 6574 332e 786d 6c9c 934d 6be3 3010  heet3.xml..Mk.0.
-00002120: 86ef 0bfb 1f84 eeb6 fcdd c4c4 2929 aed9  ............))..
-00002130: c21e 9665 bb7b 56e4 712c 6249 4692 9b84  ...e.{V.q,bIF...
-00002140: d2ff be92 43d3 422e a160 d992 357a e61d  ....C.B..`..5z..
-00002150: cfeb d5fd 510c e805 b4e1 4a56 380e 238c  ....Q.....JV8.#.
-00002160: 4032 d572 b9ab f0f3 9f26 5860 642c 952d  @2.r.....&X`d,.-
-00002170: 1d94 840a 9fc0 e0fb f5f7 6fab 83d2 7bd3  ..........o...{.
-00002180: 0358 e408 d254 b8b7 762c 0931 ac07 414d  .X...T..v,.1..AM
-00002190: a846 906e a753 5a50 eb96 7a47 cca8 81b6  .F.n.SZP..zG....
-000021a0: f321 3190 248a 0a22 2897 f84c 28f5 2d0c  .!1.$.."(..L(.-.
-000021b0: d575 9c41 add8 2440 da33 44c3 40ad d36f  .u.A..$@.3D.@..o
-000021c0: 7a3e 9a77 9a60 b7e0 04d5 fb69 0c98 12a3  z>.w.`.....i....
-000021d0: 436c f9c0 ed69 8662 2458 f9b4 934a d3ed  Cl...i.b$X...J..
-000021e0: e0ea 3ec6 1965 e8a8 dd95 b891 bea7 99df  ..>..e..........
-000021f0: 5f65 129c 6965 5467 4347 2667 cdd7 e52f  _e..ieTgCG&g.../
-00002200: c992 5076 215d d77f 1326 ce88 8617 ee1b  ..Pv!]...&......
-00002210: f881 4abe 2629 ce2f ace4 0396 7e11 565c  ..J.&)./....~.V\
-00002220: 60fe 73e9 72e2 6d85 5ff3 6cf1 b868 d226  `.s.r.m._.l..h.&
-00002230: 4892 a208 b24d 9e05 0f77 4d14 a40f 7516  H....M...wM...u.
-00002240: 178f 9bba c9eb 37bc 5eb5 dc75 d857 8534  ......7.^..u.W.4
-00002250: 7415 dec4 e5cf 24c6 64bd 9a0d f497 c3c1  t.....$.d.......
-00002260: 7c9a 23ef c7ad 527b bff1 e4f2 443e 945c  |.#...R{....D>.\
-00002270: c536 b31f 7f69 d442 47a7 c1fe 5687 1fc0  .6...i.BG...V...
-00002280: 77bd 75e6 cfc2 cce9 f48d 2edb 530d 8639  w.u.........S..9
-00002290: 8739 5098 7a14 5383 cbe7 ee48 70ff a738  .9P.z.S....Hp..8
-000022a0: 83d0 e3fc 3cf0 d6f6 154e a230 8e96 e95d  ....<....N.0...]
-000022b0: 8ed1 168c 6db8 4762 c426 6395 f877 8e99  ....m.Gb.&c..w..
-000022c0: f593 19f5 1f00 00ff ff00 0000 ffff 9c57  ...............W
-000022d0: 6b6f a240 14fd 2bb3 6cd3 c02e 591c c547  ko.@..+.l...Y..G
-000022e0: 5b25 01b4 d115 215b 31db ec97 8645 6c93  [%....![1....El.
-000022f0: 6d6b 83d4 d67f bf97 c132 0f6d 61ea 2799  mk.......2.ma.'.
-00002300: b9dc 33e7 de33 e76a 7f73 9724 d930 ca22  ..3..3.j.s.$.0."
-00002310: ab9f ae5f 503a 50b0 8236 4fd1 e306 be9d  ..._P:P..6O.....
-00002320: e3a6 825e b119 c5e7 cbdd 30d9 c4c9 6336  ...^......0...c6
-00002330: 501a 3f5a 8ad5 8ff3 581b 8261 6503 cf5b  P.?Z....X..ae..[
-00002340: abd5 ee1b 5bab 6fc4 fb4d 0793 e526 bf3a  ....[.o..M...&.:
-00002350: e45e e9f0 9b93 1c7c a034 3b45 da2c 850c  .^.....|.4;E.,..
-00002360: 2b4b 71d7 0f4f cf59 b244 7172 7fbf 4177  +Kq..O.Y.Dqr..Aw
-00002370: d136 4111 dac1 031c f96f 14ff bb4d d7cf  .6A......o...M..
-00002380: 8f4b a56f acf2 83d4 0ce7 a17f 96d0 c6fe  .K.o............
-00002390: fcd3 8315 8f5d 31a0 5e65 d1a0 4ef5 8b06  .....]1.^e..N...
-000023a0: c1b4 685d a168 4d52 b486 5034 ee95 5eb9  ..h].hMR..P4..^.
-000023b0: c99d a125 7306 082e cfd0 c5c2 19f2 fe6e  ...%s..........n
-000023c0: 2dba cac1 9832 3010 4c61 0425 38a6 a00f  -....20.La.%8...
-000023d0: 0ea6 2d03 03c1 14a6 25b0 6913 185a 34a2  ..-.....%.i..Z4.
-000023e0: dc21 fb4a ebec 7845 4186 f5bb bad7 2c01  .!.J..xEA.....,.
-000023f0: 3385 fe39 9d8f a876 6560 20b8 a46a 8a8d  3..9...ve` ..j..
-00002400: eb16 17f1 389b 9e0c 0c04 5318 b171 bd82  ....8.....S..q..
-00002410: e471 9833 1918 08a6 3062 e3ce 080c b508  .q.3....0b......
-00002420: 4e1f b821 e553 104d 814c d1a8 1a82 4478  N..!.S.M.L....Dx
-00002430: 2439 4764 fdcd 3cb0 c4c2 13df d15b 6eb7  $9Gd..<......[n.
-00002440: 12de cb9a 8229 38a9 03b9 c825 a64a e449  .....)8....%.J.I
-00002450: 49b9 0566 edc2 142d 0b76 0914 9509 0f25  I..f...-.v.....%
-00002460: e518 98b5 0c53 b8b5 0eec 1228 2a15 1e4a  .....S.....(*..J
-00002470: ca35 30eb 013d f12e c12e 81a2 2de4 a1d8  .50..=......-...
-00002480: 5b5b 3926 b95b 4bbb 4fac c8c1 79aa 62ea  [[9&.[K.O...y.b.
-00002490: c50f f900 86a1 97ab 354a d368 a7a0 288e  ........5J.h..(.
-000024a0: c854 4e93 d540 21c1 c582 e506 0b3f b4d5  .TN..@!......?..
-000024b0: e0f2 723e 0ad5 d1eb 53f2 e5c4 39c1 3a1a  ..r>....S...9.:.
-000024c0: 8fec e1e8 ea66 3ef9 33d2 91e7 cd6e dcc0  .....f>.3....n..
-000024d0: d391 e305 ee74 bf88 356d 3f2c df71 79cc  .....t..5m?,.qy.
-000024e0: ba45 253d d62d daa2 f791 54b5 e941 aa0a  .E%=.-....T..A..
-000024f0: 7a2c bb5f 8bd1 3c9c 047e c110 37c8 4747  z,._..<..~..7.GG
-00002500: d5f4 5897 aaa4 c7ba 54fb 4027 79aa daf4  ..X.....T.@'y...
-00002510: 2058 82de a5ed 86b2 d49a ac31 5651 cb83   X.........1VQ..
-00002520: e9e4 147d 91a4 2a7f 8e25 70f4 4a79 e6af  ...}..*..%p.Jy..
-00002530: ec09 ceec d01d abe1 d502 44e8 07a1 3a99  ..........D...:.
-00002540: 3b9e ed4f 0ff5 ca34 f43b d6df 6fa9 a6a3  ;..O...4.;..o...
-00002550: c69b 6cbf fa86 7d7c fe34 59bb aee4 cfba  ..l...}|.4Y.....
-00002560: 7557 746b 92aa 6e6b f3e0 92f9 b53a b3af  uWtk..nk.....:..
-00002570: d50f a9ea ee78 e14f 4977 0bdd ea58 3bbd  .....x.OIw...X;.
-00002580: cf2e 4e6f b30b 45d1 d037 a45e 05bf a553  ..No..E..7.^...S
-00002590: 681a 94a9 1abc 54d6 a7b1 0f33 d484 7e33  h.....T....3..~3
-000025a0: a44f 231f 2400 e037 5d88 83c1 a07f 70fe  .O#.$..7].....p.
-000025b0: 0300 00ff ff00 0000 ffff b229 484c 4ff5  ...........)HLO.
-000025c0: 4d2c 4acf cc2b 56c8 494d 2bb1 5532 d033  M,J..+V.IM+.U2.3
-000025d0: 5752 28ca 4ccf 80b1 4bf2 0bc0 a2a6 4a0a  WR(.L...K.....J.
-000025e0: 49f9 2525 f9b9 305e 466a 624a 6a11 8867  I.%%..0^FjbJj..g
-000025f0: aca4 9096 9f5f 02e3 e8db d9e8 97e7 1765  ....._.........e
-00002600: 1767 a4a6 96d8 0100 0000 ffff 0300 504b  .g............PK
-00002610: 0304 1400 0600 0800 0000 2100 b145 0dec  ..........!..E..
-00002620: 5c07 0000 0221 0000 1300 0000 786c 2f74  \....!......xl/t
-00002630: 6865 6d65 2f74 6865 6d65 312e 786d 6cec  heme/theme1.xml.
-00002640: 594b 8f1b 3712 be07 c87f 20fa 2eeb d5ad  YK..7..... .....
-00002650: c7c0 b2a1 a727 f68c 6d78 642f 72e4 4894  .....'..mxd/r.H.
-00002660: 9a1e 7653 20a9 190b 8181 c039 e512 2040  ..vS ......9.. @
-00002670: 76b1 9705 f6b6 8720 4880 0458 2397 fc18  v...... H..X#...
-00002680: 0336 b2d9 1fb1 4576 4b4d 8ea8 786c 8f17  .6....EvKM..xl..
-00002690: 4e30 33c0 8c9a faaa 58ac 2a7e ac2e 5ebf  N03.....X.*~..^.
-000026a0: f924 61e8 9408 4979 da09 aad7 2a01 22e9  .$a...Iy....*.".
-000026b0: 844f 693a ef04 0fc7 a352 2b40 52e1 748a  .Oi:.....R+@R.t.
-000026c0: 194f 4927 5811 19dc bcf1 f147 d7f1 9e8a  .OI'X......G....
-000026d0: 4942 10c8 a772 0f77 8258 a9c5 5eb9 2c27  IB...r.w.X..^.,'
-000026e0: 308c e535 be20 297c 37e3 22c1 0a1e c5bc  0..5. )|7.".....
-000026f0: 3c15 f80c f426 ac5c ab54 1ae5 04d3 3440  <....&.\.T....4@
-00002700: 294e 40ed bdd9 8c4e 08aa 55aa 7554 827f  )N@....N..U.uT..
-00002710: b51a 1a6b f5c1 8df5 4443 068f a992 7a60  ...k....DC....z`
-00002720: c2c4 919e 86ec 9436 72d3 93aa 46cb 95ec  .......6r...F...
-00002730: 3381 4e31 eb04 30ff 949f 8dc9 1315 2086  3.N1..0....... .
-00002740: a582 2f3a 41c5 fc04 e51b d7cb 782f 1762  ../:A.......x/.b
-00002750: 6a87 ac25 3732 3fb9 5c2e 303d a999 39c5  j..%72?.\.0=..9.
-00002760: fc78 3369 1846 61a3 bbd1 6f00 4c6d e386  .x3i.Fa...o.Lm..
-00002770: cd61 63d8 d8e8 3300 3c99 c0aa 335b 5c9d  .ac...3.<...3[\.
-00002780: cd5a 3fcc b116 28fb e8d1 3d68 0eea 5507  .Z?...(...=h..U.
-00002790: 6fe9 af6f d9dc 8df4 af83 37a0 4c7f b885  o..o......7.L...
-000027a0: 1f8d fae0 4507 6f40 193e dac2 47bd 766f  ....E.o@.>..G.vo
-000027b0: e0ea 37a0 0cdf d8c2 372b dd41 d874 f41b  ..7.....7+.A.t..
-000027c0: 50cc 687a b285 ae44 8d7a 7fbd da0d 64c6  P.hz...D.z....d.
-000027d0: d9be 17de 8ec2 51b3 962b 2f50 900d 9b4c  ......Q..+/P...L
-000027e0: d353 cc78 aa2e 9277 097e ccc5 08c0 5a88  .S.x...w.~....Z.
-000027f0: 6145 53a4 560b 32c3 13c8 f43e 66f4 5850  aES.V.2....>f.XP
-00002800: 7440 e731 24e1 02a7 5cc2 70a5 5619 55ea  t@.1$...\.p.V.U.
-00002810: f057 ff86 e693 892e de23 d892 d636 8255  .W.......#...6.U
-00002820: 726b 48db 86e4 44d0 85ea 04b7 416b 6041  rkH...D.....Ak`A
-00002830: 5e3e 7ffe e2d9 4f2f 9efd fbc5 175f bc78  ^>....O/....._.x
-00002840: f67d 3eb7 51e5 c8ed e374 6ecb fdf6 afaf  .}>.Q....tn.....
-00002850: fffb 8fcf d17f 7efc e76f dffc 359b fa3c  ......~..o..5..<
-00002860: 5eda f857 df7d f9ea e75f 7e4f 3dac b870  ^..W.}..._~O=..p
-00002870: c5cb bffd f0ea a71f 5efe fdab 5fbf fdc6  ........^..._...
-00002880: a3bd 2bf0 b10d 1fd3 8448 7497 9ca1 073c  ..+......Ht....<
-00002890: 8105 7aec 27c7 e2cd 24c6 31a6 8e04 8e41  ..z.'...$.1....A
-000028a0: b747 f550 c50e f0ee 0a33 1fae 475c 173e  .G.P.....3..G\.>
-000028b0: 12c0 383e e0ad e563 c7d6 a358 2c15 f5cc  ..8>...c...X,...
-000028c0: 7c27 4e1c e021 e7ac c785 d701 77f4 5c96  |'N..!......w.\.
-000028d0: 87c7 cb74 ee9f 5c2c 6ddc 038c 4f7d 73f7  ...t..\,m...O}s.
-000028e0: 71ea 0478 b85c 00ed 529f ca7e 4c1c 33ef  q..x.\..R..~L.3.
-000028f0: 339c 2a3c 2729 5148 7fc7 4f08 f1ac ee53  3.*<')QH..O....S
-00002900: 4a1d bf1e d289 e092 cf14 fa94 a21e a65e  J..............^
-00002910: 978c e9b1 9348 85d0 3e4d 202e 2b9f 8110  .....H..>M .+...
-00002920: 6ac7 3787 8f50 8f33 dfaa 07e4 d445 c2b6  j.7..P.3.....E..
-00002930: c0cc 63fc 9830 c78d b7f0 52e1 c4a7 728c  ..c..0....R...r.
-00002940: 1366 3bfc 00ab d867 e4d1 4a4c 6cdc 502a  .f;....g..JLl.P*
-00002950: 88f4 9c30 8e86 5322 a54f e69e 80f5 5a41  ...0..S".O....ZA
-00002960: bf03 0ce3 0ffb 215b 252e 5228 7ae2 d379  ......![%.R(z..y
-00002970: 8039 b791 037e d28f 71b2 f0da 4cd3 d8c6  .9...~..q...L...
-00002980: 7e22 4f20 4531 bacf 950f 7ec8 dd1d a29f  ~"O E1....~.....
-00002990: 210e 38dd 19ee 4794 38e1 7e3d 113c 0472  !.8...G.8.~=.<.r
-000029a0: b54d 2a12 447f b314 9e58 de22 dcdd 8f2b  .M*.D....X."...+
-000029b0: 36c3 c4c7 325d 9138 ecda 15d4 9b1d bde5  6...2].8........
-000029c0: dc49 ed03 4218 3ec3 5342 d0c3 4f3c 16f4  .I..B.>.SB..O<..
-000029d0: f8c2 f179 61f4 ed18 5865 9ff8 12eb 3676  ...ya...Xe....6v
-000029e0: 7355 3fa7 4412 646a 9c6d 8a3c a0d2 49d9  sU?.D.dj.m.<..I.
-000029f0: 2332 e73b ec39 5c9d 239e 154e 132c 7669  #2.;.9\.#..N.,vi
-00002a00: be0b 5177 5217 4e39 2f95 de63 9313 1b78  ..QwR.N9/..c...x
-00002a10: 9742 8908 f9e2 75ca 3d09 3aac e41e eed2  .B....u.=.:.....
-00002a20: 7a3f c6ce d9a5 9fa5 3f5f 57c2 89df 45f6  z?......?_W...E.
-00002a30: 18ec cbc7 6fba 2f41 86bc b10c 10fb 857d  ....o./A.......}
-00002a40: 33c6 cc99 a048 9831 8602 c347 b720 e284  3....H.1...G. ..
-00002a50: bf10 d1e7 aa11 5b7a e566 eea6 2dc2 0045  ......[z.f..-..E
-00002a60: 9253 ef24 347d 6df1 73ae ec89 fe3f 658f  .S.$4}m.s....?e.
-00002a70: bf80 b984 82c7 aff8 5d4a 9d5d 94b2 7fae  ........]J.]....
-00002a80: c0d9 85fb 0396 3503 bc4c ef13 3849 b639  ......5..L..8I.9
-00002a90: ebaa aab9 aa6a 823f 7d55 b36b 2f5f d532  .....j.?}U.k/_.2
-00002aa0: 57b5 cc55 2de3 7bfb 7a2f b54c 51be 4065  W..U-.{.z/.LQ.@e
-00002ab0: 5374 7c4c ff27 b950 fb67 4619 3b52 2b46  St|L.'.P.gF.;R+F
-00002ac0: 0ea4 e900 4978 bb99 8e60 d0b4 a94c df72  ....Ix...`...L.r
-00002ad0: d31a 5cc4 f031 6f3c 39b8 b9c0 4606 09ae  ..\..1o<9...F...
-00002ae0: fe42 557c 14e3 05b4 89aa a6b1 3997 b9ea  .BU|........9...
-00002af0: b944 0b2e a17b 6486 4deb 959c d36d 7a50  .D...{d.M....mzP
-00002b00: cbe4 904f b30e 68b5 aabb 9d99 3b25 56c5  ...O..h.....;%V.
-00002b10: 7825 da8c 43c7 4a65 e846 b3e8 ea6d d49b  x%..C.Je.F...m..
-00002b20: 3ee9 dc74 62d7 0668 d937 31c2 9acc 35a2  >..tb..h.71...5.
-00002b30: ee31 a2b9 1e84 88fc 9e11 6665 9762 45db  .1........fe.bE.
-00002b40: 6345 4bab 5f87 6a1d c58d 2bc0 b44d 54e0  cEK._.j...+..MT.
-00002b50: f51b c14b 7b27 88c2 acb3 0c8d 3928 d5a7  ...K{'......9(..
-00002b60: 3a4e 5993 791d 5d1d 9c4b 8df4 2e67 323b  :NY.y.]..K...g2;
-00002b70: 03a0 dc5e 6740 11e9 b6b6 75e7 f2f4 eab2  ...^g@....u.....
-00002b80: 54bb 40a4 1d23 ac74 738d b0d2 3086 97e2  T.@..#.ts...0...
-00002b90: 3c3b ed56 fc65 c6ba 5d84 d431 4fbb 62bd  <;.V.e..]..1O.b.
-00002ba0: 1b0a 339a adf7 116b 4d28 e7b8 81a5 3653  ..3....kM(....6S
-00002bb0: b014 9d75 8246 3d82 5b98 095e 7482 1974  ...u.F=.[..^t..t
-00002bc0: 8fe1 63b2 80dc 91fa 0d0c b339 5cd3 4c94  ..c........9\.L.
-00002bd0: c836 fcdb 30cb 4248 35c0 32ce 1c6e 4827  .6..0.BH5.2..nH'
-00002be0: 6383 842a 2210 a349 27d0 cbdf 6403 4b0d  c..*"..I'...d.K.
-00002bf0: 8718 dbaa 3520 840f d6b8 36d0 ca87 661c  ....5 ....6...f.
-00002c00: 04dd 0d32 99cd c844 d961 b746 b4a7 b347  ...2...D.a.F...G
-00002c10: 60f8 8c2b bcdf 1af1 b707 6b49 be84 701f  `..+......kI..p.
-00002c20: c5d3 3374 cc96 e201 8614 8b9a 55ed c029  ..3t........U..)
-00002c30: 9570 8950 cdbc 39a5 7043 b621 b222 ffce  .p.P..9.pC.!."..
-00002c40: 1d4c 39ed da57 5426 87b2 71cc 1631 ce4f  .L9..WT&..q..1.O
-00002c50: 149b cc33 b821 d18d 39e6 69e3 03eb 295f  ...3.!..9.i...)_
-00002c60: 3338 74db 85c7 737d c0be f3a9 fbfa a35a  38t...s}.......Z
-00002c70: 7bce 22cd e2cc 7458 459f 9a7e 327d 7f87  {."...tXE..~2}..
-00002c80: bc65 5571 883a 5665 d46d deaf 65c1 75ed  .eUq.:Ve.m..e.u.
-00002c90: 35d7 41a2 7a4f 89d7 9cba 1738 102c d38a  5.A.zO.....8.,..
-00002ca0: c91c d3b4 c5db 34ac 393b 1f75 4dbb c482  ......4.9;.uM...
-00002cb0: c0f2 4463 87df 3667 84d7 136f 7bf2 83dc  ..Dc..6g...o{...
-00002cc0: f9ac d507 c4ba c634 896f aed8 ed9b 6f7e  .......4.o....o~
-00002cd0: fc18 c863 0077 894b a6a4 0925 dc65 0b0c  ...c.w.K...%.e..
-00002ce0: 455f 7633 99d1 066c 9127 2aaf 11e1 135a  E_v3...l.'*....Z
-00002cf0: 0ada 093e ab44 ddb0 5f8b faa5 4a2b 1a96  ...>.D.._...J+..
-00002d00: c27a 5829 b5a2 6ebd d48d a27a 7518 552b  .zX)..n....zu.U+
-00002d10: 835e ed29 1c2c 2a4e aa51 76bd 3f82 eb0c  .^.).,*N.Qv.?...
-00002d20: b6ca 2ff9 cdf8 d645 7fb2 beb1 b936 e149  ../....E.....6.I
-00002d30: 999b 8bfc b231 dc5c f457 6b17 bbe8 4714  .....1.\.Wk...G.
-00002d40: 08e8 b346 6dd4 aeb7 7b8d 52bb de1d 95c2  ...Fm...{.R.....
-00002d50: 41af 556a f71b bdd2 a0d1 6f0e 4683 7ed4  A.Uj......o.F.~.
-00002d60: 6a8f 9e06 e8d4 80c3 6ebd 1f36 86ad 52a3  j.......n..6..R.
-00002d70: daef 97c2 4645 2fa5 d52e 35c3 5aad 1b36  ....FE/...5.Z..6
-00002d80: bbad 61d8 7d9a 9734 e085 8c4a 72bf 80ab  ..a.}..4...Jr...
-00002d90: 8d8d 37fe 0700 00ff ff03 0050 4b03 0414  ..7........PK...
-00002da0: 0006 0008 0000 0021 0078 b91e 89d4 0500  .......!.x......
-00002db0: 006e 1a00 000d 0000 0078 6c2f 7374 796c  .n.......xl/styl
-00002dc0: 6573 2e78 6d6c cc19 db6e db36 f47d c0fe  es.xml...n.6.}..
-00002dd0: 4150 8a3d 0c53 2439 9662 bb96 b3c4 b180  AP.=.S$9.b......
-00002de0: 026d 1120 1930 6019 0259 a26c a292 e852  .m. .0`..Y.l...R
-00002df0: 546a 77d8 cbbe 675f b52f d921 29d9 942f  Tjw...g_./.!)../
-00002e00: b19c 7859 fd60 8914 cf85 e71c 9e1b fb17  ..xY.`..........
-00002e10: f334 d11e 11cd 31c9 3cdd 3eb5 740d 6521  .4....1.<.>.t.e!
-00002e20: 8970 36f1 f45f ee7c a3a3 6b39 0bb2 2848  .p6.._.|..k9..(H
-00002e30: 4886 3c7d 8172 fd62 f0fd 77fd 9c2d 1274  H.<}.r.b..w..-.t
-00002e40: 3b45 8869 8022 cb3d 7dca d8ac 679a 7938  ;E.i.".=}...g.y8
-00002e50: 4569 909f 9219 cae0 4b4c 681a 3018 d289  Ei......KLh.0...
-00002e60: 99cf 280a a29c 03a5 89d9 b22c d74c 039c  ..(........,.L..
-00002e70: e912 432f 0d9b 2049 03fa a998 1921 4967  ..C/.. I.....!Ig
-00002e80: 01c3 639c 60b6 10b8 742d 0d7b ef26 19a1  ..c.`...t-.{.&..
-00002e90: c138 0156 e776 3b08 b5b9 edd2 9636 a715  .8.V.v;......6..
-00002ea0: 1131 bb41 27c5 2125 3989 d929 e035 491c  .1.A'.!%9..).5I.
-00002eb0: e310 6db2 db35 bb66 10ae 3001 e6e7 61b2  ..m..5.f..0...a.
-00002ec0: 1dd3 6ad5 f63e a7cf c4d4 3629 7ac4 5c7d  ..j..>....6)z.\}
-00002ed0: faa0 9f15 a99f b25c 0b49 9131 4fef 2ea7  .......\.I.1O...
-00002ee0: 34f9 e55d e4e9 edb6 ae49 a50c 4904 627a  4..].....I..I.bz
-00002ef0: 307e d44e 7e3a 39b1 4e2d eb5e fbe1 7341  0~.N~:9.N-.^..sA
-00002f00: d8db 7ffe fa5b be3c 186f eff7 7ce7 f072  .....[.<.o..|..r
-00002f10: b121 1f17 17db d03c 183f 3f18 ba59 f1a8  .!.....<.??..Y..
-00002f20: 3064 bb6b 1c49 341f c7da e702 e50c 7696  0d.k.I4.......v.
-00002f30: f74a 0ad6 0e04 4e7d 4bb0 1589 43cb e573  .J....N}K...C..s
-00002f40: 0798 bb01 6655 806f 9e04 3caf 03de bfa9  ....fU.o..<.....
-00002f50: 04b8 8b41 3845 aacc b9ac 2581 a719 ecd6  ...A8E....%.....
-00002f60: c1a2 c84c 5373 01bf 7b6d 3aed a569 2fcf  ...LSs..{m:..i/.
-00002f70: b76f ed1c ceb1 4a70 29d2 3808 d93e 719e  .o....Jp).8..>q.
-00002f80: db75 e0df de18 7edb b27e 2f29 de6b 971f  .u....~..~/).k..
-00002f90: cc9b 0f9c b059 1adc a01f 936c 6577 a00e  .....Y.....lew..
-00002fa0: 71cc 7a9f 32f2 25f3 f927 f02d 608c 7cd5  q.z.2.%..'.-`.|.
-00002fb0: a09f 7fd5 1e83 0466 6c8e 2324 09a1 1a03  .......fl.#$....
-00002fc0: a701 c628 66b2 2045 72c5 3048 f098 62be  ...(f. Er.0H..b.
-00002fd0: 2c0e 529c 2ce4 748b 4f08 3f53 ae4b 319c  ,.R.,.t.O.?S.K1.
-00002fe0: 7ac1 90a4 20ff c77c d52b d17a cd3d e157  z... ..|.+.z.=.W
-00002ff0: dcd7 ebd0 3285 f980 9271 922c bdd7 1937  ....2....q.,...7
-00003000: 1898 18f4 c1d1 3344 331f 065a f97e b798  ......3D3..Z.~..
-00003010: 81b9 6410 93a4 dac5 ba3d ab27 3458 d82d  ..d......=.'4X.-
-00003020: a739 404e 121c 712e 2643 61a4 7432 f674  .9@N..q.&Ca.t2.t
-00003030: 5ffc 2c71 d2c7 e507 9c45 688e c0b9 822b  _.,q.....Eh....+
-00003040: e3c7 4261 1846 922d f1c8 07fd 31a1 11c4  ..Ba.F.-....1...
-00003050: dbca 47b7 00bf 9c1a f413 1433 00a7 7832  ..G........3..x2
-00003060: e54f 4666 f03f 268c 414c 1af4 231c 4c48  .OFf.?&.AL..#.LH
-00003070: 1624 9c40 05a1 4242 9c86 90ec e96c 0a21  .$.@..BB.....l.!
-00003080: b53a 57eb 9c71 1207 5128 4901 e321 4a92  .:W..q..Q(I..!J.
-00003090: 5b4e e2d7 b8a6 a379 ac38 73e1 7732 c603  [N.....y.8s.w2..
-000030a0: 0d7f 05b5 94af 9253 3980 1dd4 8084 9b93  .......S9.......
-000030b0: 40ad c640 328e ed83 d282 d92c 5970 1724  @..@2......,Yp.$
-000030c0: 1892 23e0 6a35 ba12 fa58 8d2f 133c c952  ..#.j5...X./.<.R
-000030d0: a402 dc50 c250 c823 115f c6e5 afca 424a  ...P.P.#._....BJ
-000030e0: 4615 0ad7 e9e1 52d1 e6f1 76f1 2832 e59e  F.....R...v.(2..
-000030f0: 79bb 4c97 d0ea 8e85 3b3d 5cd4 25ae 4d68  y.L.....;=\.%.Mh
-00003100: db15 9176 afd0 e54e 8059 21ef 8f45 3a46  ...v...N.Y!..E:F
-00003110: d417 8960 e9e2 6b3c d9ae 08c4 47c6 aa48  ...`..k<....G..H
-00003120: 6db7 512d 77da 8cd3 069a 804d 577a ac6b  m.Q-w......MWz.k
-00003130: 428e 2a6b db94 6d83 93b3 81bb 11b6 836d  B.*k..m........m
-00003140: 4672 aa9c 031e ba21 12cb 63a1 4d09 c55f  Fr.....!..c.M.._
-00003150: e140 f110 1ec2 3941 7408 239c 15a4 10d9  .@....9At.#.....
-00003160: 8839 8f77 9bff 2e66 1a8b ede8 ccd9 ae48  .9.w...f.......H
-00003170: cef6 f9ac 35ad eeb7 69c5 a9ed f684 0763  ....5...i......c
-00003180: 1599 a7e4 b5b1 5ed7 79dd 6697 47d4 b6ed  ......^.y.f.G...
-00003190: 1e9f c9f5 8851 a371 44f1 2aa6 f0ed 8af7  .....Q.qD.*.....
-000031a0: f84c 6e8a 57b1 de6f 5710 c767 725d 108a  .Ln.W..oW..gr]..
-000031b0: 533e 7b69 e82d ebdc ffeb f08a ac52 242f  S>{i.-.......R$/
-000031c0: 4ff9 e7c6 67e9 980e 4356 abdf b660 fecb  O...g...CV...`..
-000031d0: 28da 4c35 bc4b f2a2 dcaf 516e be16 911a  (.L5.K....Qn....
-000031e0: a9f9 60d3 8284 4cad 07d6 3326 919f 6fcb  ..`...L...3&..o.
-000031f0: 3e95 c0b2 d750 81c6 d6ec f3e9 fcf8 25b9  >....P........%.
-00003200: f6c1 a989 ce3b af0c 873c 9382 626f fbe1  .....;...<..bo..
-00003210: 549c dc5e 0ba8 326e 59ef 6c91 206f ec1c  T..^..2nY.l. o..
-00003220: 3b7b 97ed a2a3 9ede aac4 82a2 4aa9 3b6b  ;{..........J.;k
-00003230: 55e7 b202 d378 bbc8 d387 05a5 d0b9 5e54  U....x........^T
-00003240: e937 37b1 0227 9097 8aa6 a7e8 3455 056c  .77..'......4U.l
-00003250: 09f2 9157 2489 92af 2b00 a2cc 5ba7 7183  ...W$...+...[.q.
-00003260: 284f 782b 0890 b602 21fb 0a4b 1060 3c9a  (Ox+....!..K.`<.
-00003270: af0a 659e 42c3 7855 eb83 beb7 16ec 41c1  ..e.B.xU......A.
-00003280: 4859 2499 b066 d0af 4c04 64b2 cabc d51e  HY$..f..L.d.....
-00003290: 8029 f0f2 7fa0 c978 ef5b 54e9 4b69 8149  .).....x.[T.Ki.I
-000032a0: 4728 0e8a 84dd 2d3f 7afa eafd 038a 7091  G(....-?z.....p.
-000032b0: 82bc ca55 37f8 9130 81c2 d357 efef 7953  ...U7..0...W..yS
-000032c0: c276 971d 3ba0 95d2 42f4 45b8 8e6a fd91  .v..;...B.E..j..
-000032d0: f361 47f6 47ea d35d df19 5dae 5a7e 6537  .aG.G..]..].Z~e7
-000032e0: a5dd ea38 be68 9bd4 57fb e7d6 1624 a3d1  ...8.h..W....$..
-000032f0: e87a d411 2745 216f 0a50 e003 cdd9 fb1c  .z..'E!o.P......
-00003300: 1a1c f0d4 0a8a 3dfd 8fd1 d579 f77a e4b7  ......=....y.z..
-00003310: 8c8e 75d5 31da 67c8 31ba ced5 b5e1 b487  ..u.1.g.1.......
-00003320: 57d7 d77e d76a 59c3 3f95 cb81 175c 0d88  W..~.jY.?....\..
-00003330: bb0c 287d ec76 2f4f e002 8196 7a28 e57a  ..(}.v/O....z(.z
-00003340: bb9a f374 6520 252b b604 6cab bc77 5bae  ...te %+..l..w[.
-00003350: 75e9 d896 e19f 59b6 d176 838e d171 cf1c  u.....Y..v...q..
-00003360: c377 ecd6 b5db be1a 39be a3f0 ee3c f30a  .w......9....<..
-00003370: c132 6d5b 5e46 70e6 9d1e c329 4a70 5699  .2m[^Fp....)JpV.
-00003380: 5165 3cea 2cd8 0f0c 9fd8 8459 69c2 5c5d  Qe<.,......Yi.\]
-00003390: 140d fe05 0000 ffff 0300 504b 0304 1400  ..........PK....
-000033a0: 0600 0800 0000 2100 fa1f ae0b c103 0000  ......!.........
-000033b0: ba0c 0000 1400 0000 786c 2f73 6861 7265  ........xl/share
-000033c0: 6453 7472 696e 6773 2e78 6d6c ac57 db6e  dStrings.xml.W.n
-000033d0: db46 107d 2fd0 7f58 b041 91a0 8d68 f721  .F.}/..X.A...h.!
-000033e0: 701d 4906 43c9 516a 5a74 74a9 8b1a 06b1  p.I.C.QjZtt.....
-000033f0: 2647 2211 7257 e12e adf8 affa 0dfd b2ce  &G".rW..........
-00003400: 9296 6aec ac1a 17c8 23e7 7e39 33b3 ec9f  ..j.....#.~93...
-00003410: 7da9 4a76 0fb5 2aa4 1878 c7bd 238f 8148  }.Jv..*..x..#..H
-00003420: 6556 88f5 c05b 2ece 5f9f 784c 692e 325e  eV...[.._.xLi.2^
-00003430: 4a01 03ef 0194 7736 fcfe bbbe 529a a1ae  J.....w6....R...
-00003440: 5003 2fd7 7a73 eafb 2acd a1e2 aa27 3720  P./.zs..*....'7 
-00003450: 90b3 9275 c535 7ed6 6b5f 6d6a e099 ca01  ...u.5~.k_mj....
-00003460: 7455 fabf 1c1d bdf1 2b5e 088f a5b2 117a  tU......+^.....z
-00003470: e0fd fac6 638d 283e 3710 7684 9313 6fd8  ....c.(>7.v...o.
-00003480: 57c5 b0af 871f 1b50 1aa3 63f2 133b ebfb  W......P..c..;..
-00003490: 7ad8 f70d a363 4eef 182a b57c 8502 367b  z....cN..*.|..6{
-000034a0: a7ab 6cc6 02be 689b 76ce 534d 042f 6506  ..l...h.v.SM./e.
-000034b0: a52d 194a 45b4 474d cd4d 98b6 ec88 6bb0  .-.JE.GM.M....k.
-000034c0: 69bb 907b da11 c6ca 84d1 2bcb 2ae1 426d  i..{......+.*.Bm
-000034d0: a1ee ad9a b24c 04af 8819 2299 3ae2 2242  .....L....".:."B
-000034e0: d981 40c7 f79c 241a 345a dac1 4f9a 8a93  ..@...$.4Z..O...
-000034f0: 2c89 175d 54d8 165e 6d5c b563 8827 b68b  ,..]T..^m\.c.'..
-00003500: 83f1 cda6 7c60 5a32 5e96 c831 3993 3684  ....|`Z2^..19.6.
-00003510: b2ae 21d5 ecb7 793c 6535 e8a6 1690 d9a6  ..!...y<e5......
-00003520: aff3 22cd 7716 105a 95b1 bb2d 74ce 740e  ..".w..Z...-t.t.
-00003530: a8d5 961d b2ce 4807 4f17 a0d2 e7f8 0a2a  ......H.O......*
-00003540: 29d6 6857 2a78 f484 13f3 33db e620 5826  ).hW*x....3.. X&
-00003550: 41b5 2ea3 e892 6500 55f7 b5eb ba49 f50e  A.....e.U....I..
-00003560: b54a e035 0e9b 6cd6 3905 f61e f5c1 74c4  .J.5..l.9.....t.
-00003570: c2bc 119f 0cbe a9dc 378e c334 c614 2bed  ........7..4..+.
-00003580: 3c62 a4a9 141a 47b5 a562 cd33 ac5f c635  <b....G..b.3._.5
-00003590: ffcf 516c fbfb 6882 0ee5 2207 2c1a afa1  ..Ql..h...".,...
-000035a0: b589 a82b b27d d35e 163d e8ed 47da 646c  ...+.}.^.=..G.dl
-000035b0: f2df 9b7a 45a6 4ba6 8a29 d9d4 2999 8e03  ...zE.K..)..)...
-000035c0: 95c9 e596 2180 1f58 5ae8 2e82 4e9d bdcc  ....!..XZ...N...
-000035d0: 64ca a428 1f5e d1dc 46c6 cd4f 6cc3 d7f0  d..(.^..F..Ol...
-000035e0: 2dbd 7516 1dfe 222e d60d 3a3b 65ab da4e  -.u..."...:;e..N
-000035f0: f96b 7999 c262 bfce 6bdc e30e 60fd 6b1a  .ky..b..k...`.k.
-00003600: c814 3fd3 f458 accb 4239 6cdf 1ebd 65c7  ..?..X..B9l...e.
-00003610: 3764 618c 83d1 7896 cc3f fc39 b659 3f96  7da...x..?.9.Y?.
-00003620: faed 6bd6 0102 8180 9bbc c505 62ce dc1c  ..k.........b...
-00003630: ba8d 3f2e c7f3 c587 789a 8471 f44c 5b72  ..?.....x..q.L[r
-00003640: b552 a0b1 8eb2 622f 8217 c7ff 4fcd 6c8f  .R....b/....O.l.
-00003650: 47f0 9b61 be2b 654a 8f4c 125f 902d 3759  G..a.+eJ.L._.-7Y
-00003660: 4e2f e60e 4614 4cdf dbc2 d377 c928 0ee7  N/..F.L....w.(..
-00003670: 07c8 094e 4072 15bc 1f13 8130 9e2f c840  ...N@r.....0./.@
-00003680: 2c67 81a9 904d 1fff 1e44 49b0 5cc4 4ec6  ,g...M...DI.\.N.
-00003690: 6479 1910 150c 0b73 7685 b56b 838b 771e  dy.....sv..k..w.
-000036a0: 840b 42ef 06f8 a6b8 755e bc76 bdd9 71b5  ..B.....u^.v..q.
-000036b0: 17e5 9046 e0be 128f c7e3 90d6 13f6 93f3  ...F............
-000036c0: ea3a 9a6e c943 97d3 2d7d f002 3e11 0704  .:.n.C..-}..>...
-000036d0: 7d8f 3b8e ac2d 93bb 8eae 2de4 7a4d 6007  }.;..-....-.zM`.
-000036e0: edca bac3 753d 3026 7891 1b72 8b83 e9fc  ....u=0&x..r....
-000036f0: 7a3c b37b 6c1e 83a7 6ac3 537c 24e2 6b4f  z<.{l...j.S|$.kO
-00003700: 417d 0fde 9005 f8b6 345b f340 edbe a2e5  A}......4[.@....
-00003710: ea8d 0131 3370 5e3a 81be 73a8 f08c 939b  ...13p^:..s.....
-00003720: 109a b174 2d0f 835a 171d cbe7 22bf 8be2  ...t-..Z...."...
-00003730: f0c2 b9d1 7068 66f1 3519 00bb 5515 687e  ....phf.5...U.h~
-00003740: e3e5 6d7d bd5b bb43 57f8 d6b1 6933 4a72  ..m}.[.CW...i3Jr
-00003750: 1bc5 e2a7 8579 ce53 bb6e 0594 c738 a8f4  .....y.S.n...8..
-00003760: 2488 a225 1df1 bbfd b1de fa92 7529 90d5  $..%........u)..
-00003770: f5f7 5f36 e907 b278 feb8 22f7 c0d5 6f8a  .._6...x.."...o.
-00003780: 1c1f ff3d 86ff 0000 00ff ff03 0050 4b03  ...=.........PK.
-00003790: 0414 0006 0008 0000 0021 00ac d4f4 abdb  .........!......
-000037a0: 0200 003b 0d00 0018 0000 0078 6c2f 6472  ...;.......xl/dr
-000037b0: 6177 696e 6773 2f64 7261 7769 6e67 312e  awings/drawing1.
-000037c0: 786d 6cec 575d 4fa4 3014 7ddf 64ff 03e9  xml.W]O.0.}.d...
-000037d0: 7b85 9652 3e32 8c19 be36 261b d787 dd1f  {..R>2...6&.....
-000037e0: d074 c021 0b74 5250 c718 fffb 9602 3aea  .t.!.tRP......:.
-000037f0: 90a8 d1ac 26be cc5c 6eb9 e7b6 f7dc 9e96  ....&..\n.......
-00003800: c5f1 aeae 8ccb 5cb6 a568 4280 8e2c 60e4  ......\..hB..,`.
-00003810: 0d17 ebb2 390f c19f df19 f480 d176 ac59  ....9........v.Y
-00003820: b34a 3479 08ae f316 1c2f bf7f 5bec d632  .J4y...../..[..2
-00003830: b86a 1369 2880 a60d d463 0836 5db7 0d4c  .j.i(....c.6]..L
-00003840: b3e5 9bbc 66ed 91d8 e68d 1a2d 84ac 59a7  ....f......-..Y.
-00003850: 1ee5 b9b9 96ec 4a41 d795 892d 8b9a ed56  ......JA...-...V
-00003860: e66c dd6e f2bc 4b86 1130 e2b1 57a0 d5ac  .l.n..K..0..W...
-00003870: 6cc0 52cf acbb 1271 5e55 ab86 6f84 1c5c  l.R....q^U..o..\
-00003880: 8514 f560 7151 2dd1 c2ec 57d0 9b3a 4019  ...`qQ-...W..:@.
-00003890: bf8a 6289 10b1 2d7a 37d6 bbf4 b014 574b  ..b...-z7.....WK
-000038a0: ec0f fede 9e9c 8f63 d498 8ed1 e0f7 193b  .......c.......;
-000038b0: b197 f91e fe41 6adb 4396 7538 3321 2fcc  .....Aj.C.u83!/.
-000038c0: 3ce5 3b97 6cbb 2979 2659 9d1b 35e3 5284  <.;.l.)y&Y..5.R.
-000038d0: 60ac 5073 f963 6ff0 6c2c 123f bd3c 9346  `.Ps.co.l,.?.<.F
-000038e0: b90e 0106 46a3 a242 106f 98ec 0ca4 c258  ....F..B.o.....X
-000038f0: 90ef ba9f 6d37 5ac6 852c 4370 9365 3872  ....m7Z..,Cp.e8r
-00003900: d28c c04c 5990 5811 8151 4a7c 9861 db4b  ...LY.X..QJ|.a.K
-00003910: b19b c5d8 a6b7 7d34 a201 5774 77aa d34e  ......}4..Wtw..N
-00003920: d613 cd88 3e21 ba2e d53c 5b51 7447 5cd4  ....>!...<[QtG\.
-00003930: a628 8a92 e753 e3a8 b641 c4d4 44eb 59de  .(...S...A..D.Y.
-00003940: 24d8 b1e2 14ad 20a5 4904 49bc f2a1 6ffb  $..... .I.I...o.
-00003950: 1e74 ad84 44c4 8d29 75d2 5b60 2e17 a69e  .t..D..)u.[`....
-00003960: fdf4 af57 3174 40bf e291 88d3 2735 61c1  ...W1t@.....'5a.
-00003970: 7e09 7f0a feb7 edb1 74eb 3c7d 5bfb 0f17  ~.......t.<}[...
-00003980: 7657 48d5 7d2c 50cb 3176 2150 dbec baff  vWH.},P.1v!P....
-00003990: 5560 7a5e 061f 9c7c f26a a829 689c 43ff  U`z^...|.j.)h.C.
-000039a0: ee68 26ac 6343 fd5f bce7 78cf a7e2 8307  .h&.cC._..x.....
-000039b0: da1a 89e0 afd8 6f03 d208 f0ac ed3f 9099  ......o......?..
-000039c0: 087e 51e7 4d37 6880 cc2b dd13 eda6 dcb6  .~Q.M7h..+......
-000039d0: c090 41df 7df2 648d 46d6 f656 acd9 bb2b  ..A.}.d.F..V...+
-000039e0: 862e d13e 3d23 8b55 a9b0 fb02 4d4c 1d10  ...>=#.U....ML..
-000039f0: 83f7 d007 e21c dea5 187b 74dc f3cf 9007  .........{t.....
-00003a00: 6f46 983c ec79 33c2 4447 d978 2c4c 7389  oF.<.y3.DG.x,Ls.
-00003a10: df40 1dc8 4375 b03f a83a b8ae 5221 375e  .@..Cu.?.:..R!7^
-00003a20: 4197 ba08 9234 cba0 8f13 0a57 18a7 3659  A....4.....W..6Y
-00003a30: 597e 1ab9 5fea b07f 227f 1675 c0ff 551d  Y~.._..."..u..U.
-00003a40: 668e 70c7 a32e 9939 c3d1 cc19 ee23 3285  f.p....9.....#2.
-00003a50: 3ce7 f230 a23c beb7 600f f973 99e7 ee2d  <..0.<..`..s...-
-00003a60: 7399 df40 1e9c 87f2 403e a83c 1017 fbb1  s..@....@>.<....
-00003a70: ed10 483d 4b5d 5d92 c882 9e13 ad20 7208  ..H=K]]...... r.
-00003a80: 45a9 eb7a 56ec 7dc9 c367 9407 fbbd e441  E..zV.}..g.....A
-00003a90: 5f3a faef 9ee5 3f00 0000 ffff 0300 504b  _:....?.......PK
-00003aa0: 0304 1400 0600 0800 0000 2100 becf 157f  ..........!.....
-00003ab0: d708 0000 843f 0000 1400 0000 786c 2f63  .....?......xl/c
-00003ac0: 6861 7274 732f 6368 6172 7431 2e78 6d6c  harts/chart1.xml
-00003ad0: ec5b fb8f dbb8 11fe bd40 ff07 55d8 035a  .[.......@..U..Z
-00003ae0: 5cb5 b66c c92f c41b d8b2 7548 bb79 349b  \..l./....uH.y4.
-00003af0: bb02 2d8a 8296 68af ba14 a990 d43e 72b8  ..-...h......>r.
-00003b00: ffbd c387 2cd9 6b67 37b9 dc5d b355 1078  ....,.kg7..].U.x
-00003b10: 253e 46e4 cc70 f889 fae6 d9f3 db9c 38d7  %>F..p........8.
-00003b20: 988b 8cd1 a9eb 9f76 5d07 d384 a519 dd4c  .......v]......L
-00003b30: ddef dfc5 dec8 7584 4434 4584 513c 75ef  ......u.D4E.Q<u.
-00003b40: b070 9f9f fdfe 77cf 9249 7289 b8bc 2850  .p....w..Ir...(P
-00003b50: 821d 1042 c524 99ba 9752 1693 4e47 2497  ...B.$...R..NG$.
-00003b60: 3847 e294 1598 42dd 9af1 1c49 b8e5 9b4e  8G....B....I...N
-00003b70: cad1 0d08 cf49 a7d7 ed0e 3a5a 886b 05a0  .....I....:Z.k..
-00003b80: cf10 90a3 8c56 fdf9 63fa b3f5 3a4b f082  .....V..c...:K..
-00003b90: 2565 8ea9 34a3 e098 2009 1a10 9759 212a  %e..4... ....Y!*
-00003ba0: 6989 3fe0 bd7b 12f3 2ce1 4cb0 b53c 4d58  i.?..{..,.L..<MX
-00003bb0: de31 c2aa 4981 303f ec6c 6775 064a 4a91  .1..I.0?.lgu.JJ.
-00003bc0: c4fe b81b 38d7 884c ddae db51 8504 d18d  ....8..L...Q....
-00003bd0: 29c0 d4fb fec2 1472 56d2 14a7 11e3 14cc  )......rV.......
-00003be0: d168 9f27 9319 9198 5310 1531 2a61 d456  .h.'....S..1*a.V
-00003bf0: 5ff9 a334 9e23 7e55 161e 0cb7 8049 ae32  _..4.#~U.....I.2
-00003c00: 92c9 3b3d 6df7 ec19 c88e 2e19 e8c3 798b  ..;=m.........y.
-00003c10: df97 19c7 62ea 267e 50ab 20f8 5405 7487  ....b.&~P. .T.t.
-00003c20: 9d51 a767 ed0a 93f5 8389 9077 049b 09f9  .Q.g.......w....
-00003c30: dd9e 9a6d 67fb 5c3d 8418 11b2 42c9 95d2  ...mg.\=....B...
-00003c40: 4da3 f1b6 695d af3a ee2b 43f5 d26e a42e  M...i].:.+C..n..
-00003c50: 5029 d9bb 4c12 bcc0 044b 9cee e8bd 204c  P)..L....K.... L
-00003c60: ce38 46c6 0677 ac94 da1c 2bc4 23e5 cbaa  .8F..w....+.#...
-00003c70: 18ae 1719 37bd 1246 8c69 3660 9b02 9cd6  ....7..F.i6`....
-00003c80: 1693 5280 3970 6a2a af11 bf8b 1861 3b36  ..R.9pj*.....a;6
-00003c90: 8379 60ae e465 e9ed ce10 184f b115 6f9d  .y`..e.....O..o.
-00003ca0: 41de 9a69 f3b7 78ad aed6 6717 1216 cb1f  A..i..x...g.....
-00003cb0: 4ee6 27bd 671d 75af b5c2 2304 8b4a 5d17  N.'.g.u...#..J].
-00003cc0: 3202 5791 56a1 6610 8574 e049 cac1 548b  2.W.V.f..t.I..T.
-00003cd0: eb33 44c5 0d78 d13f b37f 9d12 92ff dbdc  .3D..x.?........
-00003ce0: 9e52 9463 25f2 1a2c a0e4 e83f 4256 a2a1  .R.c%..,...?BV..
-00003cf0: 0c6e f430 e0d2 8eab 7803 f340 13c1 4896  .n.0....x..@..H.
-00003d00: c619 21fa 462d 6f1c 113b 1179 eb6b a3ee  ..!.F-o..;.y.k..
-00003d10: b522 54b5 a54c f502 3da3 49c1 855c 2071  ."T..L..=.I..\ q
-00003d20: 6946 ae25 da7e aaa9 7aba 7e18 288d 4244  iF.%.~..z.~.(.BD
-00003d30: 922f d6af f006 3cf6 dafa 8ed5 577a be22  ./....<.....Wz."
-00003d40: 42eb c40e adf1 84cf 7fa4 bc35 f35c b1f4  B..........5.\..
-00003d50: ee0d 7738 934a 998e 2892 3883 619f 2321  ..w8.J..(.8.a.#!
-00003d60: df20 0e01 ca77 55b8 94af e167 4dd8 cdd4  . ...wU....gM...
-00003d70: c584 40d0 c820 6ca8 7258 2e8c 7f70 9d1b  ..@.. l.rX...p..
-00003d80: 8e8a a92b de97 8863 d721 2f28 2cac fec8  ...+...c.!/(,...
-00003d90: ef82 4ca9 6f20 2884 70c3 9b35 ab66 0da2  ..L.o (.p..5.f..
-00003da0: 0988 82e5 28b9 eb98 9b48 c2bd 0f26 064d  ....(....H...&.M
-00003db0: 1733 f0f4 3853 1edc 4113 336c 5541 84bc  .3..8S..A.3lUA..
-00003dc0: 50eb cd68 5cab ddcc 2cc5 ebb7 3033 f161  P..h\...,...03.a
-00003dd0: ea8e d530 567a 8299 99a6 e4d9 1544 77ca  ...0Vz.......Dw.
-00003de0: 2ef4 95eb 5c41 bc81 6741 8c86 9648 6092  ....\A..gA...H`.
-00003df0: a9e8 afdc eb61 5fd0 c328 f397 ccae be61  .....a_..(.....a
-00003e00: d805 317a 40a4 cc5f afd7 c601 7a55 318c  ..1z@.._....zU1.
-00003e10: 5f6f 18ca a3f4 6c76 9c4d 4566 eac8 bb02  _o....lv.MEf....
-00003e20: af61 ab99 badf e6d4 23d2 88c3 68af 0223  .a......#...h..#
-00003e30: 5391 88bd 8a44 5857 336a d08f b1fe 8369  S....DXW3j.....i
-00003e40: aa4c ab94 a302 f3d4 5d73 2f7e 6b9b 17da  .L......]s/~k...
-00003e50: 318d 7740 3407 df7b c36c 7086 f0b1 a436  1.w@4..{.lp....6
-00003e60: 0888 4b76 738e 3720 eaaf f86e 67c1 ab9a  ..Kvs.7 ...ng...
-00003e70: 1f10 ecb1 2afe eb75 027e 0e65 1192 af60  ....*..u.~.e...`
-00003e80: 39de 6b7b 81f9 c1f2 3798 272a f237 f711  9.k{....7.'*.7..
-00003e90: 2567 5eae 5604 5f64 1fee 8b3a c708 82cd  %g^.V._d...:....
-00003ea0: 3958 aeb9 9d24 137c 2bcf 858e 7670 e594  9X...$.|+...vp..
-00003eb0: 1c7c e0c7 6839 08fb c399 ef2d 0671 e405  .|..h9.....-.q..
-00003ec0: eb41 e88d 1763 df1b f67a 4114 8c83 7034  .A...c...zA...p4
-00003ed0: 9fff 546f 0be1 27ef 8bcd 2d21 d41a 383c  ..To..'...-!..8<
-00003ee0: 3c08 0330 2aad f56a 9c50 b45d f409 d203  <..0*..j.P.]....
-00003ef0: afe2 940a 8f7f b4f1 7276 12fe 797b 39ac  ........rv..y{9.
-00003f00: 2fc7 f5a5 ef4f 4e66 277e ff4f 0f07 d6c1  /....ONf'~.O....
-00003f10: e1c0 0adb 33c7 8974 fe72 f1fa 95c3 b12c  ....3..t.r.....,
-00003f20: 61b7 4e77 63aa 8aac 261a aba5 aaa2 eddf  a.Nwc...&.......
-00003f30: 4a2c 14bc 70d8 95f3 fc58 e3de 7ee3 d9ab  J,..p....X..~...
-00003f40: 8513 5d96 f44a 7cb4 5fdf f603 4423 1cc1  ..]..J|._...D#..
-00003f50: 4a70 9363 8f08 9a4d bf75 0ab4 c10f f408  Jp.c...M.u......
-00003f60: 6d8f 7358 1825 349f 386b fee8 1dc4 da0a  m.sX.%4.8k......
-00003f70: 3c56 a981 96f9 7687 ab4c 36af 4d36 3fd9  <V....v..L6.M6?.
-00003f80: 9a6c 7eb2 35d9 fc44 990c 7e1b 2603 41db  .l~.5..D..~.&.A.
-00003f90: bdd0 20cb 88a5 f8ac fb8d 36aa 869a ba60  .. .......6....`
-00003fa0: 7fab 3c62 d1ee 43d6 3bda a0b2 d8d1 0695  ..<b..C.;.......
-00003fb0: 698e 36a8 0c72 b441 a5ff bd06 b022 6a2d  i.6..r.A....."j-
-00003fc0: 989b 6adb b6da 3eb8 c6fb fd51 378a 022f  ..j...>....Q7../
-00003fd0: 5c0c 965e d01d 47de 7cd9 ef79 cb61 6fd1  \..^..G.|..y.ao.
-00003fe0: 1b0f fb61 3f8a 1a6b 7cf0 c96b 3c68 c0be  ...a?..k|..k<h..
-00003ff0: c1a4 a4d9 fb12 bfb0 9bc0 8fb0 07e8 7f5e  ...............^
-00004000: 1c2f 032f 58ce 436f d61f cdbd 71b7 b71c  ././X.Co....q...
-00004010: faf0 3f98 2d7e d251 f760 04b0 786a 1f56  ..?.-~.Q.`..xj.V
-00004020: d988 da80 55b6 e428 ac8a 1e0d ab0c 1eb2  ....U..(........
-00004030: bef6 73c0 d1fe 86a8 36be 031b e2b6 f881  ..s.....6.......
-00004040: 0db1 c555 2dae 5268 e2e9 e0aa 163e 3d74  ...U-.Rh.....>=t
-00004050: acd0 c2a7 163e dd83 4f51 0d9f a21a 3e45  .....>..OQ....>E
-00004060: 357c 8a34 7c82 df16 3eed 9d7a 7cad f0c9  5|.4|...>..z|...
-00004070: ffb2 f049 1fb1 2593 067c b225 47e1 d3e2  ...I..%..|.%G...
-00004080: 9786 4f7c b3da 9e2c 05bd 5118 07ed e152  ..O|...,..Q....R
-00004090: 7bb8 a48f 3dd4 41e3 d33d 5c6a 4150 0b82  {...=.A..=\jAP..
-000040a0: aa73 f9f6 0c49 7d0c 8177 ee87 cf90 1635  .s...I}..w.....5
-000040b0: 085a d420 6851 83a0 8506 41f0 db82 a027  .Z. hQ....A....'
-000040c0: 0282 7a5f 1604 f5cd 516f 0304 d992 a320  ..z_....Qo..... 
-000040d0: 68f9 6b82 a078 1c87 cb59 0b82 5a10 d482  h.k..x...Y..Z...
-000040e0: a0f6 439a df9e 04b5 2741 f74e 8296 3508  ..C.....'A.N..5.
-000040f0: 5ad6 2068 5983 a0a5 0641 f0db 82a0 2702  Z. hY....A....'.
-00004100: 82fa 5f16 04e9 5396 9d93 205b 7214 04c5  .._...S... [r...
-00004110: bf2a 081a 4623 f3cd 4c7d 1c6b 9291 5a9a  .*..F#..L}.k..Z.
-00004120: 514b 33d2 c0a8 fd1c d6b2 89f6 c94e 2d9b  QK3..........N-.
-00004130: a8a2 1efd 1fb0 89e2 1a04 c535 088a 6b10  ...........5..k.
-00004140: 146b 1004 bf2d 087a 2220 28f8 7920 a8e6  .k...-.z" (.y ..
-00004150: 123f 8ebf 6929 c8bf 387f b3c9 78dc a0e2  .?..i)..8...x...
-00004160: ef59 2a2d 6bba e78f ed69 15b0 8d09 2a0c  .Y*-k....i....*.
-00004170: 1fd4 eb0d 4d29 baad f856 7e10 f4bb a361  ....M)...V~....a
-00004180: 7f6c 3fe8 356a 86dd 517f 108e 424d 8883  .l?.5j..Q...BM..
-00004190: 4735 f9ef 70de 3ad3 84f4 e392 4482 800d  G5..p.:.....D...
-000041a0: bc51 9c3e c633 e0a4 ead4 0933 903c a32f  .Q.>.3.....3.<./
-000041b0: d1ad 6571 351a a69a 8dbf 435e 45b7 5b26  ..eq5.....C^E.[&
-000041c0: edca 0c1e bec9 c6b9 746a 4edf d4fd 0e43  ........tjN....C
-000041d0: 3204 2240 c4d6 c446 08ef 5738 ddf2 6873  2."@...F..W8..hs
-000041e0: f41f c6df 65c9 d54b 4871 30c2 2964 a918  ....e..KHq0.)d..
-000041f0: 6930 94e3 9512 3a35 b9bc 14f8 72ef 98e9  i0....:5....r...
-00004200: 6858 e83b cc75 421d 607a 8fc3 5ee8 3a89  hX.;.uB.`z..^.:.
-00004210: 2276 af81 950c 9779 0183 1174 0304 6db2  "v.....y...t..m.
-00004220: 01be b4e2 6a7f 0e43 da3f cc90 1e3d 8e21  ....j..C.?...=.!
-00004230: 7d84 578f 263a a5c4 10c4 f718 f687 e8ee  }.W.&:..........
-00004240: dec0 32f4 be18 edfd 3885 dd90 c1ff f7a8  ..2.....8.......
-00004250: ea83 c386 e87f 7d54 7595 a524 6636 f9c4  ......}Tu..$f6..
-00004260: df59 f2f0 5545 5556 ac70 9532 f30f ccad  .Y..UEUV.p.2....
-00004270: f7ab bb1d b23a 5991 1938 b7cd 7d01 0737  .....:Y..8..}..7
-00004280: 294c 2b02 447e 81ab 3414 f36e 06b4 54f6  )L+.D~..4..n..T.
-00004290: b224 323b bf26 b0bc 1aeb dd7c ca31 a105  .$2;.&.....|.1..
-000042a0: d0fa bd18 b337 c0c7 c598 6492 a36a 869f  .....7....d..j..
-000042b0: 1a73 6c6a 8f0e 21df f12c 5509 0e3b 6925  .slj..!..,U..;i%
-000042c0: 4f6c cd83 01ee cff5 40c4 ed7e f3db 07db  Ol......@..~....
-000042d0: cfcd 1b6a a3da d43d c491 78aa 516d 0fe2  ...j...=..x.Qm..
-000042e0: 7c24 aae9 aa39 9637 18db 48b6 3237 366c  |$...9.7..H.276l
-000042f0: d890 a4b2 e29a 3982 3aa3 4767 0bea ab7d  ......9.:.Gg...}
-00004300: c0c2 3406 dbcb f7f9 7ab2 d2da edf9 b7ca  ..4.....z.......
-00004310: 2403 3f23 5bdf 521e f743 265e 5362 3dc9  $.?#[.R..C&^Sb=.
-00004320: 6630 a499 28e6 9091 7625 6636 7f0b 5e05  f0..(...v%f6..^.
-00004330: 2c44 85d7 9585 ca83 5469 8800 b8f7 36da  ,D......Ti....6.
-00004340: 2a99 b542 b21f 4bde 5c6d 8e24 6f3e 31c4  *..B..K.\m.$o>1.
-00004350: 5bf0 8cca 0b2c 2199 70a3 f7f9 4b9d 1d17  [....,!.p...K...
-00004360: 3306 b9bc 1ad2 a874 2878 91d8 6454 e8e4  3......t(x..dT..
-00004370: c8d3 21a0 7d95 b47d 3a84 3c4d fb57 a585  ..!.}..}:.<M.W..
-00004380: ea0a d35d ddf5 5d78 6551 52cc cd56 163c  ...]..]xeQR..V.<
-00004390: ac2c 14fa 86a0 b2fb 7005 86b6 c9f3 67ff  .,......p.....g.
-000043a0: 0500 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-000043b0: 0000 0021 0041 9287 f0fd 0800 0001 3300  ...!.A........3.
-000043c0: 0014 0000 0078 6c2f 6368 6172 7473 2f63  .....xl/charts/c
-000043d0: 6861 7274 322e 786d 6cec 5b5b 6fe3 b815  hart2.xml.[[o...
-000043e0: 7e2f d0ff a00a 415f 168e ad9b 6f1d 6761  ~/....A_....o.ga
-000043f0: cbf1 62d0 cc4e 30c9 6e81 1645 414b b4a3  ..b..N0.n..EAK..
-00004400: 8622 3524 95cb 2cf6 07f5 37f4 71ff 580f  ."5$..,...7.q.X.
-00004410: 2f72 24c7 9924 8ed3 a699 e421 112f a20e  /r$..$.....!./..
-00004420: cf8d e73b 8779 f7fd 554e 9c0b cc45 c6e8  ...;.y..UN...E..
-00004430: c8f5 f63b ae83 69c2 d28c 2e47 ee4f a7b3  ...;..i....G.O..
-00004440: 56df 7584 4434 4584 513c 72af b170 bf3f  V.u.D4E.Q<r..p.?
-00004450: f8fd efde 25c3 e40c 7179 52a0 043b b008  ....%...qyR..;..
-00004460: 15c3 64e4 9e49 590c db6d 919c e11c 897d  ..d..IY..m.....}
-00004470: 5660 0a63 0bc6 7324 a1c9 97ed 94a3 4b58  V`.c..s$......KX
-00004480: 3c27 6dbf d3e9 b6f5 22ae 5d00 6db1 408e  <'m.....".].m.@.
-00004490: 325a bdcf 1ff2 3e5b 2cb2 044f 5952 e698  2Z....>[,..OYR..
-000044a0: 4a43 05c7 0449 e080 38cb 0a51 ad96 785d  JC...I..8..Q..x]
-000044b0: eedf 5a31 cf12 ce04 5bc8 fd84 e56d b358  ..Z1....[....m.X
-000044c0: b529 58cc 8bda ab5d 1d00 9352 24b1 37e8  .)X....]...R$.7.
-000044d0: 84ce 0522 23b7 e3b6 5527 4174 693a 306d  ..."#...U'Ati:0m
-000044e0: fd74 623a 392b 698a d398 710a e2a8 cdcf  .tb:9+i...q.....
-000044f0: 93e1 9848 cc29 2c15 332a 816a cbaf fc41  ...H.),.3*.j...A
-00004500: 1ccf 113f 2f8b 1690 5bc0 26e7 19c9 e4b5  ...?/...[.&.....
-00004510: deb6 7bf0 0ed6 8ecf 18f0 c3f9 843f 9719  ..{..........?..
-00004520: c762 e426 5e78 c382 f0b1 0ce8 f4da fdb6  .b.&^x..........
-00004530: 6fe5 0a9b f5c2 a190 d704 9b0d 791d 5fed  o...........y._.
-00004540: b6bd faae 2661 8608 99a3 e45c f1a6 3679  ....&a.....\..6y
-00004550: 35f5 665c bdb8 ce0c f596 5623 f520 3349  5.f\......V#. 3I
-00004560: b07e b852 bf79 969c 1dbc 43c3 394b af8f  .~.R.y....C.9K..
-00004570: b9c3 9954 4270 4491 cc32 2ee4 1112 f218  ...TBpD..2......
-00004580: 71d0 3bcf 5556 203f c2af 0561 9723 1713  q.;.UV ?...a.#..
-00004590: 02ba 9081 36a8 7ee0 02e3 5f5c e792 a362  ....6.~..._\...b
-000045a0: e48a cf25 e2d8 7510 4da0 1b38 2679 d588  ...%..u.M..8&y..
-000045b0: 25b4 3db5 4734 2442 9ea8 adeb 46a1 7a8a  %.=.G4$B....F.z.
-000045c0: 63ae fea4 78f1 09a8 115f 606a d801 7ae6  c...x...._`j..z.
-000045d0: 9aaa ccd0 2679 760e 9646 d989 7e72 9d73  ....&yv..F..~r.s
-000045e0: 903d cc04 7bd1 94eb 5973 2430 c994 4576  .=..{...Ys$0..Ev
-000045f0: 408c 6828 18c9 d259 4688 6e28 f3c3 31e1  @.h(...YF.n(..1.
-00004600: 86e9 f2ca d373 4899 7f60 a9e9 eb46 1d58  .....sH..`...F.X
-00004610: ce90 59e6 1f17 0bd3 1d54 dd6d 58b2 5a05  ..Y......T.mX.Z.
-00004620: e4b5 f601 652d d491 d705 5e80 f98f dcef  ....e-....^.....
-00004630: 72da 22d2 2c87 d1da 0046 6620 116b 0389  r.".,....Ff .k..
-00004640: d0ba 50f1 437f c672 48b3 8903 8f94 a98c  ..P.C..rH.......
-00004650: dc05 6fcd 3e99 55e4 c129 ce0b e160 e924  ..o.>.U..)...`.$
-00004660: ecb7 7f4b a740 20d7 dffe 5580 f562 45a8  ...K.@ ...U..bE.
-00004670: d4eb c002 f00c 4c6f 574a 000f 52eb 0403  ......LoWJ..R...
-00004680: 8112 74dd b048 61bf 4b99 e2a1 610b 55ac  ..t..Ha.K...a.U.
-00004690: ac75 14a0 3053 24ce cc8b 9ae1 967e 0253  .u..0S$......~.S
-000046a0: 6179 b388 fa4e a584 a894 ec54 35a6 9860  ay...N.....T5..`
-000046b0: 892d efad 1728 0893 638e 91f1 08d7 ac94  .-...(..c.......
-000046c0: da39 cc11 8f95 6755 ddf0 3ccd ac14 1346  .9....gU..<....F
-000046d0: 8ca3 5882 a728 c085 1a3a 1252 0a70 0e38  ..X..(...:.R.p.8
-000046e0: 3583 1788 5fc7 8cb0 8607 01d2 3030 2419  5..._.......00$.
-000046f0: 66e9 5563 db8c a7d8 2e6f 8932 2c12 927f  f.Uc.....o.2,...
-00004700: c20b f5c6 e2e0 4482 ebfe c3de 782f 507b  ......D.....x/P{
-00004710: d49d 301c 23d0 0e35 a190 3138 2e69 cddb  ..0.#..5..18.i..
-00004720: 1051 4807 be64 5433 195e 1c38 6360 395a  .QH..dT3.^.8c`9Z
-00004730: 6227 2db9 f6b3 6aa5 0bcd b342 894b 597d  b'-...j....B.KY}
-00004740: b5a2 69e8 afaf 2456 49e7 6b4a 8e92 041c  ..i...$VI.kJ....
-00004750: a3b6 bc5b daba a524 815f 5419 fffb c58f  ...[...$._T.....
-00004760: 7809 745f 5827 6659 951e 6b19 adf3 f4ab  x.t_X'fY..k.....
-00004770: efcc cbf9 9ce0 60ba 51f9 eeb3 61e5 38d7  ......`.Q...a.8.
-00004780: 0d71 ebad e12b 7924 f406 e0c9 2939 389f  .q...+y$....)98.
-00004790: 5fe2 20e8 77e2 386c 45d3 ee61 2bec 0ce2  _. .w.8lE..a+...
-000047a0: d6e4 30f0 5b87 3d7f ea0f 7a41 14c4 f1af  ..0.[.=...zA....
-000047b0: b5e3 f1d1 8763 583b 17ba c392 669f 4bfc  .....cX;....f.K.
-000047c0: de5a c52f e090 d48f d7ea cfc2 4e2b 0ce3  .Z./........N+..
-000047d0: 716b d20b c356 7f3a ebc7 c160 128d 67b3  qk...V.:...`..g.
-000047e0: 5fb5 c525 43a0 59eb 4db5 0b50 152b 8e75  _..%C.Y.M..P.+.u
-000047f0: a968 8db8 4792 4f92 8af6 f435 cfaa 3ce8  .h..G.O....5..<.
-00004800: 06cf baea bec7 b3be 3e81 06bb 15a8 8e0a  ........>.......
-00004810: 7627 50be 9caf 0eca d0ef 47b3 d03a f586  v'P.......G..:..
-00004820: 352a 0fbf cd61 a035 f565 da59 b45b b104  5*...a.5.e.Y.[..
-00004830: c6f5 efca fbd5 c532 1bcc a2c3 f137 2296  .......2.....7".
-00004840: de6e c5a2 b5f9 79ac 65d6 8bfb c6d3 7d03  .n....y.e.....}.
-00004850: a7d2 e089 6239 9a13 a1e1 cdee 024d 15cf  ....b9.......M..
-00004860: 1a3c f13c e886 bca7 8006 83be a770 87d4  .<.<.........p..
-00004870: 0d40 b211 3478 7d64 5e1f b91b 1169 5c52  .@..4x}d^....i\R
-00004880: 8c21 209e 652a d005 9d31 643f 1429 0d1e  .! .e*...1d?.)..
-00004890: 0794 9e0a 907a 9b01 92ff 4200 12a6 a902  .....z....B.....
-000048a0: ae0a 46ae 41a4 15ec 31da 01b1 f519 bb3c  ..F.A...1......<
-000048b0: c24b 78e3 cf78 0df5 c0c8 cf08 f23f 2a37  .Kx..x.......?*7
-000048c0: 6103 2535 3b46 f247 9437 a35d d57f 82f9  a.%5;F.G.7.]....
-000048d0: c6fe 63cc 55f0 dd0c 6a61 fe44 47bb 27d9  ..c.U...ja.DG.'.
-000048e0: 97db 4b1d 6104 d0e3 0810 6c3d d571 c771  ..K.a.....l=.q.q
-000048f0: 79d8 8d82 ded8 6b4d bbb3 b815 2eba 516b  y.....kM......Qk
-00004900: 301d 78ad 9eef 8771 3808 a3fe 6452 0b4b  0.x....q8...dR.K
-00004910: a347 87a5 f574 4564 f9b5 893c 8832 3705  .G...tEd...<.27.
-00004920: 9e95 6d27 48c7 d31b c0d3 64cf 1fee cdf6  ..m'H.....d.....
-00004930: fcad 1114 a2e2 12b2 427f cbfe be4f 48fe  ........B....OH.
-00004940: 0fd3 dca7 20a4 0743 294b 1dc8 5af9 215a  .... ..C)K..Z.!Z
-00004950: e6eb 086f b217 2822 6f60 1ecc 59c1 3c93  ...o..("o`..Y.<.
-00004960: c28b 598a 0f3a 2a49 285c bd17 9dd8 d3bd  ..Y..:*I(\......
-00004970: eb50 30da 0c05 3b4d 7a15 7e34 5851 a528  .P0...;Mz.~4XQ.(
-00004980: 1428 bc73 827f df84 e0be 09e1 e609 20d5  .(.s.......... .
-00004990: 9b9d 9a46 053f 2db3 5e2c 561a 6f79 2ad9  ...F.?-.^,V.oy*.
-000049a0: 7440 ba3a 951e e622 2cf0 7d76 17a1 d05c  t@.:...",.}v...\
-000049b0: 45da 1215 7fc9 5269 b32e e07d 8d5e a1ab  E.....Ri...}.^..
-000049c0: 0a37 0681 1ff5 bb51 77c3 40af 37e8 75bd  .7.....Qw.@.7.u.
-000049d0: aec5 8cf5 c48a 4a9d adb2 2ccd 848a c976  ......J...,....v
-000049e0: f3c7 e553 acf3 ace5 536c cf57 f229 e1d3  ...S....Sl.W.)..
-000049f0: f329 0913 72cb 5c0a a10e 6439 01f0 f422  .)..r.\...d9..."
-00004a00: d749 5456 93d3 f4de 54a2 c9b2 98c4 ec5a  .ITV....T......Z
-00004a10: 2ae2 8ef4 181a eac4 b639 f11b 89b2 64a8  *........9....d.
-00004a20: 32d3 2631 25ae f339 b307 1185 4283 15d9  2.&1%..9....B...
-00004a30: cd84 1b55 7d0b a0de 02a8 1d64 98df 02a8  ...U}......d....
-00004a40: b700 6ae7 0154 a802 a81b bf7e 7700 a5b0  ..j..T.....~w...
-00004a50: ccde b714 4289 9cb1 ea10 b727 f58b 8daa  ....B......'....
-00004a60: 26af 3faa 3207 6b13 f8dd 96d0 4d90 e575  &.?.2.k.....M..u
-00004a70: 3bbe 1774 6f47 5fde c0f7 3abd c00f 4c4c  ;..toG_...:...LL
-00004a80: 00b5 ed7a 6405 9863 ac6b 6e77 866b 2241  ...zd..c.knw.k"A
-00004a90: f0c6 52c5 fe8c 6700 2275 7dc8 1096 67f4  ..R...g."u}...g.
-00004aa0: 03ba b2a1 406d 62aa 8b69 0db4 89ae 8e99  ....@mb..i......
-00004ab0: 0592 7313 2082 edcd 72e9 dce0 9691 fb03  ..s. ...r.......
-00004ac0: 86ca 3a22 005e 5809 8015 c0e7 394e 57c0  ..:".^X.....9NW.
-00004ad0: 3747 ff64 fc34 4bce 3f40 5462 16af 2211  7G.d.4K.?@Tb..".
-00004ae0: 8854 327a f7a0 8497 205c 5d51 4041 b34f  .T2z.... \]Q@A.O
-00004af0: 9921 6363 6151 455e 83c8 af02 af05 9453  .!ccaQE^.......S
-00004b00: 2106 cb0b 2046 d025 9492 c912 0abe aaaa  !... F.%........
-00004b10: bc4d 69d7 db9c b9e8 3f2c 73b1 4518 b729  .Mi.....?,s.E..)
-00004b20: 0dd5 025d d13f 2fa9 d8fe 5f4e 21bd f01a  ...].?/..._N!...
-00004b30: fb23 2220 75e5 458c 6ded 3808 6ab8 0aae  .#" u.E.m.8.j...
-00004b40: 5ea8 b12a 8ba3 0ade 7fc5 dc2a bf6a 357c  ^..*.......*.j5|
-00004b50: 0c99 9331 e8b6 ad5c 837e 9beb 3073 0217  ...1...\.~..0s..
-00004b60: 1004 54f4 4d22 aaf2 3294 7d28 89cc 8e2e  ..T.M"..2.}(....
-00004b70: 0858 57cd dc01 1eae 1c0b bc71 dbc3 34e8  .XW........q..4.
-00004b80: dbbd 87b1 7578 ed30 7ee0 59aa 5c5e 23b9  ....ux.0~.Y.\^#.
-00004b90: 6bb0 d5ab b170 e0f7 edbd 6ef0 af90 18fa  k....p....n.....
-00004ba0: e3e7 92c9 3f39 c2fc fddf 7bda 6dab 766f  ....?9....{.m.vo
-00004bb0: 2e6d e4fe 1f5e 1bda dea5 3572 485f 7169  .m...^....5rH_qi
-00004bc0: 7a68 82e5 25c6 d68d cd4d c386 292b 7fb4  zh..%....M..)+..
-00004bd0: 21f4 590b a29e ea98 6c86 e979 421f b88d  !.Y.....l..yB...
-00004be0: 649c f3d6 914f e3cc 6886 892f f0d0 5827  d....O..h../..X'
-00004bf0: 70f7 a786 3dec 36fb cd4e e539 f71e eb39  p...=.6..N.9...9
-00004c00: 9f2e a81d de7d db5c 927c 8b05 47ee 2b8d  .....}.\.|..G.+.
-00004c10: 05d7 5c5a c371 e606 bb59 63bf df67 4298  ..\Z.q...Yc..gB.
-00004c20: d1b8 12a9 4b96 fa72 a47e 5a07 78cf 7c8d  ....K..r.~Z.x.|.
-00004c30: f3b9 abeb 3bb8 3bfc 0667 ea57 861f 7cf6  ....;.;..g.W..|.
-00004c40: 839e 9195 6e29 8dfb 3913 1f29 b1a5 717b  ....n)..9..)..q{
-00004c50: aaa6 9928 2650 593f 1763 9b57 8042 9485  ...(&PY?.c.W.B..
-00004c60: f450 2c9b aaf2 94ba 2c0e 098a 3564 52dd  .P,.....,...5dR.
-00004c70: dd7d c8a5 d5f9 f28e 0bab af2c 4350 f08c  .}.........,CP..
-00004c80: ca13 2ce1 d6f8 5223 a533 5dfe 9f41 4e10  ..,...R#.3]..AN.
-00004c90: 738d 010b b81e 0c89 9765 4685 be0d bfaf  s........eF.....
-00004ca0: ca52 ea3f 26f6 7b70 dfc4 fe55 97f7 f580  .R.?&.{p...U....
-00004cb0: 795d b502 1752 3c6a 15d3 58ad 051f 2b0b  y]...R<j..X...+.
-00004cc0: 5574 02a7 d2fc b842 8fab ff5c 39f8 0f00  Ut.....B...\9...
-00004cd0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00004ce0: 0000 2100 bc8d 4ecc 4f08 0000 152a 0000  ..!...N.O....*..
-00004cf0: 1400 0000 786c 2f63 6861 7274 732f 6368  ....xl/charts/ch
-00004d00: 6172 7433 2e78 6d6c ec5a 5b73 dbb8 157e  art3.xml.Z[s...~
-00004d10: ef4c ff03 cbf1 3e75 6491 d48d d244 de91  .L....>ud....D..
-00004d20: 296b bb53 27f1 c4d9 dd99 763a 1d08 8424  )k.S'.....v:...$
-00004d30: d420 c000 a06d 6567 fffb 1e5c 288b b292  . ...meg...\(...
-00004d40: c876 b64d 52fb 4126 7139 c4e5 7cdf b900  .v.MR.A&q9..|...
-00004d50: 2fbe bf2d 5870 4da4 a282 8fc3 f838 0a03  /..-XpM......8..
-00004d60: c2b1 c829 5f8e c39f dece 5a69 1828 8d78  ...)_.....Zi.(.x
-00004d70: 8e98 e064 1cae 890a bf3f f9f3 9f5e e011  ...d.....?...^..
-00004d80: 5e21 a92f 4b84 4900 42b8 1ae1 71b8 d2ba  ^!./K.I.B...q...
-00004d90: 1cb5 db0a af48 81d4 b128 0987 ba85 9005  .....H...(......
-00004da0: d2f0 2a97 ed5c a21b 105e b076 1245 fdb6  ..*..\...^.v.E..
-00004db0: 1512 7a01 e811 020a 4479 dd5f 1ed2 5f2c  ..z.....Dy._.._,
-00004dc0: 1614 93a9 c055 41b8 76a3 9084 210d 2ba0  .....UA.v...!.+.
-00004dd0: 56b4 54b5 341c f765 724f 6241 b114 4a2c  V.T.4..erObA..J,
-00004de0: f431 1645 db09 ab27 05c2 e25e 7b33 ab13  .1.E...'...^{3..
-00004df0: 58a4 1c69 120f a36e 708d d838 8cc2 b629  X..i...np..8...)
-00004e00: 6488 2f5d 01e1 ad9f 2e5d a114 15cf 499e  d./].....]....I.
-00004e10: 09c9 613b b6da 1778 3461 9a48 0ea2 32c1  ..a;...x4a.H..2.
-00004e20: 358c daaf 5771 d08a 1748 5e55 650b 865b  5...Wq...H^Ue..[
-00004e30: c224 e794 51bd b6d3 0e4f 5e80 ec6c 2560  .$..Q....O^..l%`
-00004e40: 3d82 37e4 5d45 2551 e310 c7dd bb25 e83e  =.7.]E%Q.....%.>
-00004e50: 7401 a241 3b6d 277e 5f61 b271 77a4 f49a  t..A;m'~_a.qw...
-00004e60: 1137 a138 4acc 6cdb 9bef da21 cc10 6373  .7.8J.l....!..cs
-00004e70: 84af ccda 6c35 de34 bdab 371d 7717 c3f4  ....l5.4..7.w...
-00004e80: b26a 641e 34d5 8cd8 875b f32b 295e 9dbc  .jd.4....[.+)^..
-00004e90: 40a3 b9c8 d717 3290 429b 4d08 5489 6754  @.....2.B.M.T.gT
-00004ea0: 2a7d 8e94 be40 12f4 2e0e 0d0a f46b f859  *}...@.......k.Y
-00004eb0: 3071 330e 0963 a00b 14b4 c194 c32a 08f9  0q3..c.......*..
-00004ec0: 3e0c 6e24 2ac7 a17a 5721 49c2 0071 0cc5  >.n$*..zW!I..q..
-00004ed0: b062 5ad6 2f99 86f7 d8cc 118d 98d2 9766  .bZ./..........f
-00004ee0: eaf6 a534 25e5 8534 ff72 b278 03a3 51ef  ...4%..4.r.x..Q.
-00004ef0: a169 3782 f1cc eda8 a8fd adc6 2107 a819  .i7.........!...
-00004f00: d849 7a05 90e3 e2d2 3e85 c115 2801 7401  .Iz.....>...(.t.
-00004f10: e0d8 29d8 e673 a408 a306 9a11 ec27 1a29  ..)..s.......'.)
-00004f20: c168 3ea3 8cd9 1783 4392 31e9 565f dfc6  .h>.....C.1.V_..
-00004f30: b60d ab8a 9722 7765 fd5e 04e2 dc78 abe2  ....."we.^...x..
-00004f40: f562 e18a 3b75 711b 44d6 5260 e376 3e60  .b..;uq.D.R`.v>`
-00004f50: 60c3 03bd 2ec9 0278 601c feb5 e02d a69d  `......x`....-..
-00004f60: 3882 762a 0872 1558 ed54 6065 95a2 5e18  8.v*.r.X.T`e..^.
-00004f70: fb19 bf54 76bd 242c 96c1 cc38 5cc8 d6ec  ...Tv.$,...8\...
-00004f80: 8d93 a24f ce00 5395 c3ad 1998 b6fd a003  ...O..S.........
-00004f90: 3cc3 6ab7 ebdd 8707 6d95 41c0 4e32 b46e  <.j.....m.A.N2.n
-00004fa0: 4051 f9ef 7061 d6cc 2d03 374b b729 0069  @Q..pa..-.7K.).i
-00004fb0: cc96 90c5 8260 7dae b451 6050 54db d3c8  .....`}..Q`PT...
-00004fc0: 769b faac 6286 e1be 4215 233c 371c 6010  v...b...B.#<7.`.
-00004fd0: b9a3 641b 4572 7b6c 14a9 a617 5469 f1d6  ..d.Er{l....Ti..
-00004fe0: bc4c 0923 9a78 3079 7e2f 99d0 1349 90e3  .L.#.x0y~/...I..
-00004ff0: fab5 a88c cae0 d11c c9cc d84c ff3c a51e  ...........L.<..
-00005000: 9658 3067 0296 6003 4a30 8e4e 4331 ab14  .X0g..`.J0.NC1..
-00005010: d03e c95d e535 92eb 4c30 d1b0 0da0 8604  .>.].5..L0......
-00005020: 341e 8f68 7edb d06b 2173 e2c5 fb41 390c  4..h~..k!s...A9.
-00005030: 00a9 bc21 0bd3 6371 72a9 c128 ffe5 6872  ...!..cqr..(..hr
-00005040: 140f 8c42 db52 a8cf 10e0 ddb4 2875 0636  ...B.R......(u.6
-00005050: 497b e676 a328 7500 9f72 6483 47d7 277f  I{.v.(u..rd.G.'.
-00005060: 03ea ae94 e97e 6d51 511a 141a 16af c5b8  .....~mQQ.......
-00005070: 17fb cd0d 106b d07d 8cab 10c6 60e8 2c93  .....k.}....`.,.
-00005080: de23 9d87 0194 72c3 e03f 2e5e 9125 90c5  .#....r..?.^.%..
-00005090: b5b7 447e 5530 b2db b167 594e 8f92 d1d1  ..D~U0...gYN....
-000050a0: ec28 79f4 d220 ae6e c092 ff93 feeb 98b1  .(y.. .n........
-000050b0: e2df eef5 98a3 821c bc5c 7e74 c073 663f  .........\~t.sf?
-000050c0: 7855 ecee dde9 519c 9a51 c6e9 6698 d06a  xU....Q..Q..f..j
-000050d0: b383 cef1 ca44 4e4e a2ef 6c0b eb89 d982  .....DNN..l.....
-000050e0: dd0d eeed dfe0 a839 58a3 154e 038c 2931  .......9X..N..)1
-000050f0: bbfe c106 c9a7 1a74 3ed5 a0bb bf01 e8d1  .......t>.......
-00005100: dd24 dd4b ad5f 7ea5 c8ad e169 333e 780a  .$.K._~....i3>x.
-00005110: 2a09 96f5 d7ac d349 a32c ebb6 7ad3 fe59  *......I.,..z..Y
-00005120: ab1b 0db3 d6e9 5927 699d 0d92 6932 1c74  ......Y'i...i2.t
-00005130: 7a9d 2cfb 6dcb f77b b0e7 d7dd 727a faa3  z.,.m..{....rz..
-00005140: 8ad3 7715 f9d1 13c3 af60 64ed 5f2b 4dfa  ..w......`d._+M.
-00005150: 49ab db39 edb7 86fd b36e 6b32 1b0e 7be9  I..9.....nk2..{.
-00005160: 3449 b36e e737 6b05 ed98 2d88 ea59 1808  4I.n.7k...-..Y..
-00005170: 3994 ef82 ddc2 038f b6c0 ee4b 3e06 f6e1  9..........K>...
-00005180: a335 fad5 1c5c 1eab d4c1 4d5b 04ab 3f16  .5...\....M[..?.
-00005190: fbce fddb 7538 9eb1 5ff3 3610 5464 19ca  ....u8.._.6.Td..
-000051a0: 22d0 b2f7 33f6 2d7a be4c ecc7 4fc3 7e7e  "...3.-z.L..O.~~
-000051b0: 3e67 ca46 482b 7173 4e96 e0b6 fc9d ec38  >g.FH+qsN......8
-000051c0: b350 f333 8278 7e2b d654 5096 21fd 0acc  .P.3.x~+.TP.!...
-000051d0: cebd f24b 22f7 965f 1069 8cef bdf6 a7d5  ...K".._.i......
-000051e0: 7cce c825 7dbf 2d0a d869 33b4 252a 7fa1  |..%}.-..i3.%*..
-000051f0: b95e b99e 493c 7436 05dd d63c d84b 87e9  .^..I<t6...<.K..
-00005200: 6010 0fef 5740 8c3c e80c 5d05 88dc f695  `...W@.<..].....
-00005210: 4c78 b371 9c9a 3e92 4b4d c887 b948 9658  Lx.q..>.KM...H.X
-00005220: 1aac e94b 3ec2 9a49 fc68 d69c 80fb 8196  ...K>..I.h......
-00005230: 2450 58c8 c34d bf1f 8b0f 4f18 0f20 264d  $PX..M....O.. &M
-00005240: d2de a017 06d8 c4a0 92e7 9f8c f79c 0fd5  ................
-00005250: f1c1 55c3 dbb2 d906 13c8 7c22 ba31 c903  ..U.......|".1..
-00005260: 6f7b d6c5 5c78 ddb2 01aa 0b83 ee1a 7cf5  o{..\x........|.
-00005270: ae54 125b 3abd dbe9 673a 05cf a310 a206  .T.[:...g:......
-00005280: b4f7 99bf 58ef 2af9 f619 d6c1 ad11 92ed  ....X.*.........
-00005290: d9a1 2dc2 1d76 8058 075d 4b02 7874 5791  ..-..v.X.]K.xtW.
-000052a0: f6ba 71b7 df4f 07de e96c 902c 4079 6253  ..q..O...l.,@ybS
-000052b0: 261f 646e 8511 f458 1a7b 2424 0563 61f3  &.dn...X.{$$.ca.
-000052c0: 306e 5c05 e52f d1ad 97bb d530 b7a1 72c3  0n\../.....0..r.
-000052d0: aaa0 db0b e173 9d73 672b 0073 b342 0777  .....s.sg+.s.B.w
-000052e0: 91cb 38fc 8140 4614 31c8 7989 0a0c d339  ..8..@F.1.y....9
-000052f0: e557 24f7 5936 3c2a d07f 847c 4bf1 d54b  .W$.Y6<*...|K..K
-00005300: a02a 27bc a627 a8a4 fcc3 951a 3a81 51dd  .*'..'......:.Q.
-00005310: 8c80 8362 bf15 6e18 7bf3 4286 8387 bda4  ...b..n.{.B.....
-00005320: a6e0 0564 bf80 8d8b 1206 a3f8 1252 806c  ...d.........R.l
-00005330: 09f9 3993 0d7c 4c26 2ede 9f89 4b0f cbc4  ..9..|L&....K...
-00005340: 1d4a e8fb d255 adbe 8f4e bea4 cce8 f091  .J...U...N......
-00005350: 89d1 6f3c 217a 70b6 0a92 e270 50a1 263e  ..o<!zp....pP.&>
-00005360: 2fd4 db76 b07c 1df1 d033 c9ac 7f10 e955  /..v.|...3.....U
-00005370: dfbc 3508 86cd d904 34db 67a5 40bb dd21  ..5.....4.g.@..!
-00005380: c69c 41b6 5891 3a3f e4b2 c810 9a8b 9715  ..A.X.:?........
-00005390: d3f4 fc9a 01b6 b6c0 0e4e dd86 56c0 41bd  .........N..V.A.
-000053a0: c72f cdf1 7d7e 7ef1 3936 4b17 3f48 9a1b  ./..}~~.96K.?H..
-000053b0: c273 fe74 c3c7 faba f10d 8b7c 7f82 7b28  .s.t.......|..{(
-000053c0: 35fa ee7f cfa6 4fce b23f d3d6 d773 8ef3  5.....O..?...s..
-000053d0: 68da 6a06 8c96 d2f6 d396 ad3a 25fa 8610  h.j........:%...
-000053e0: 4f55 73f7 e21d 910d e7ec 219f 8633 043e  OUs.......!..3.>
-000053f0: ef67 776e 3c67 3e11 8970 90e0 b8f7 f3ba  .gwn<g>..p......
-00005400: 35cf 40dc 3e58 7df6 1f9c 8b78 cf7f 6804  5.@.>X}....x..h.
-00005410: 120d 2016 cedb f73d 0ec1 e0be 00a3 19a9  .. ....=........
-00005420: 3c15 833e 11fe c704 184f 0762 c337 dba1  <..>.....O.b.7..
-00005430: 9f8f 90dc 7fc1 377b ea89 38b8 208d f34f  ......7{..8. ..O
-00005440: 9ba9 b427 a1f6 6937 defb 3f3d 947f 8e6e  ...'..i7..?=...n
-00005450: 20f3 e8ee c16c 5ff7 78c8 593c db68 96d1   ....l_.x.Y<.h..
-00005460: b79f a97a cd99 cf87 7bf0 e754 95a7 70a6  ...z....{..T..p.
-00005470: 7fa5 263e d281 04b5 b3a0 fb72 58bd fee9  ..&>.......rX...
-00005480: f02c 8ba7 ad4e da83 13c2 b89b b686 513c  .,...N........Q<
-00005490: 6b0d d269 1a45 c960 30c8 a2ed 1342 d979  k..i.E.`0....B.y
-000054a0: f019 e1a0 1d75 b68f 0965 c7dc 1043 5318  .....u...e...CS.
-000054b0: 28dc 4c79 5dda 4b68 711f e002 97cf a00e  (.Ly].Khq.......
-000054c0: ca5f a189 b293 d88a c9da be7a 6f57 0020  ._.........zoW. 
-000054d0: ccae 7182 082e 0d1c 034c cd09 82b9 e104  ..q......L......
-000054e0: d999 9dc0 acbe 9670 c8c9 fc7c f981 53f9  .......p...|..S.
-000054f0: 6f2f 3d72 c835 2e97 44f7 31e4 03dc dc52  o/=r.5..D.1....R
-00005500: 52ae 2f89 860b 544b 1b87 ae08 823b 1b33  R./...TK.....;.3
-00005510: 48b7 1269 23ec 124e 0d20 a9b5 a45c d91b  H..i#..N. ...\..
-00005520: 62c7 26f9 6f6e 111e 0fc2 00ae 99d9 ffe6  b.&.on..........
-00005530: 429b ad70 ddcd 5b27 84f4 9991 e25e 36b2  B..p..['.....^6.
-00005540: e063 55e9 b2f6 3b1f 37b1 f9e6 36e7 c9ef  .cU...;.7...6...
-00005550: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00005560: 0000 0021 00d5 2d18 319c 0400 00c2 2500  ...!..-.1.....%.
-00005570: 0014 0000 0078 6c2f 6368 6172 7473 2f73  .....xl/charts/s
-00005580: 7479 6c65 312e 786d 6cec 5a6d 6fe2 3810  tyle1.xml.Zmo.8.
-00005590: fe2b 917f 4003 f468 296a 2a75 5bad 7412  .+..@..h)j*u[.t.
-000055a0: bdad f656 bacf 2671 c0bb 8e9d b3cd 52fa  ...V..&q......R.
-000055b0: eb6f ecbc 1093 8497 2dd0 c2ed 373c 09b6  .o......-...7<..
-000055c0: e799 f133 e399 dc86 6a18 4eb1 d47f eb05  ...3....j.N.....
-000055d0: 23de 4bc2 3808 5480 a65a a743 df57 e194  #.K.8.T..Z.C.W..
-000055e0: 2458 5d24 3494 4289 585f 8422 f145 1cd3  $X]$4.B.X_.".E..
-000055f0: 90f8 91c4 73ca 277e afd3 edf9 cb59 503e  ....s.'~.....YP>
-00005600: 0dae cd22 52c2 6189 58c8 046b 7521 e4a4  ..."R.a.X..ku!..
-00005610: 9823 6130 4be7 ca4f 30e5 c8a3 5180 6052  .#a0K..O0...Q.`R
-00005620: 7477 0bdb c32f 547d a39a 113b 62fc 2b89  tw.../T}...;b.+.
-00005630: e185 9700 7590 6f45 3165 ac26 2471 4c42  ....u.oE1e.&$qLB
-00005640: 5d7f 57f0 a530 a15c 4858 040f ad9a e481  ].W..0.\HX......
-00005650: 49ef 2766 01d2 2f66 6d3c 64b3 e449 4499  I.'f../fm<d..ID.
-00005660: ecaa dfe9 d815 adf8 4b1c 67e2 cb42 ec57  ........K.g..B.W
-00005670: 66b9 bbf5 61e3 71b6 96dd 6344 e2af cfd2  f...a.q...cD....
-00005680: 53af 01ea 9a79 bc1f 4472 f80d 4a1b 2dcc  S....y..Dr..J.-.
-00005690: ebae 9e21 d664 22e4 e21e b43f 65c5 55fa  ...!.d"....?e.U.
-000056a0: 2c2d 94dc 9b07 e8a6 dfeb 232f c469 8062  ,-........#/.i.b
-000056b0: 8635 fc4c 52b0 b5e2 13e4 6136 0144 429d  .5.LR.....a6.DB.
-000056c0: 5b44 301a 7d06 cb6e 699e 6eb3 7906 2de6  [D0.}..ni.n.y.-.
-000056d0: 0163 5517 9062 c623 6307 302e cfcc 916d  .cU..b.#c.0....m
-000056e0: 1cec 5231 dd4d b3e5 6ab6 b267 e15e 12ec  ..R1.M..j..g.^..
-000056f0: 2522 82c3 8419 13f3 bf84 51e7 cb4f 2225  %"........Q..O"%
-00005700: 8d08 a86b 6523 ca49 21cb fcfd 681e 9efb  ...ke#.I!...h...
-00005710: 5dd5 4d0b 6b39 e0ac 1c8e f1a4 6b5d 7605  ].M.k9......k]v.
-00005720: 4276 0e06 6e3b 9ba5 41b3 c38c 351e e131  Bv..n;..A...5..1
-00005730: 01df 04ff 7837 46ba 6e76 f9de ce8c d4e2  ....x7F.nv......
-00005740: d691 a366 397a 309e 3bd3 c7d3 3dfa b16f  ...f9z0.;...=..o
-00005750: 36de c6cd 996e 7173 4b48 6bd8 a969 bba5  6....nqsKHk..i..
-00005760: 4ddc e051 5a70 2578 3847 6b77 4e02 a71c  M..QZp%x8GkwN...
-00005770: 8b68 01f1 460a 6de2 a4a7 d2f0 3395 4a8f  .h..F.m.....3.J.
-00005780: b0d2 cf58 4264 ee22 0f98 481b ea89 8188  ...XBd."..H.....
-00005790: 8078 194d 9137 15f2 7555 66de 8350 0e4f  .x.M.7..uUf..P.O
-000057a0: 9037 9786 bbd5 bf33 2c09 f2d8 9f1c d8ed  .7.....3,.......
-000057b0: f2aa 7f7d 853c 6d07 dd41 6f30 409e ac3e  ...}.<m..Ao0@..>
-000057c0: 1957 9f60 1ec2 5419 d17b d9e0 41c3 38b3  .W.`..T..{..A.8.
-000057d0: b14a ef67 1a88 52e7 e494 e991 3172 a307  .J.g..R.....1r..
-000057e0: 1ae1 b3a0 7c3b 7fcc 530a 6592 9d32 da63  ....|;..S.e..2.c
-000057f0: 58b1 08c2 792e 619d fbcd 29c4 2ac1 9a28  X...y.a...).*..(
-00005800: efee b71c 5d3e 6e75 9e3e d0fe f31d 971a  ....]>nu.>......
-00005810: 9840 56d7 c14a dae1 b6dc 594f e2ec c903  .@V..J....YO....
-00005820: b0f6 6e01 98d3 4d48 7a83 fe75 9191 481e  ..n...MHz..u..H.
-00005830: 65c9 e09a c39d 4ec1 6d9a c25f 6b06 e118  e.....N.m.._k...
-00005840: bd04 a984 ed09 4b48 05f7 07dc 06c0 0fea  ......KH........
-00005850: df35 746d bab7 892f 5b20 add1 9e03 6405  .5tm.../[ ....d.
-00005860: b615 2847 7801 d1c9 538b 642c 2095 0fa9  ..(Gx...S.d, ...
-00005870: 0c19 5095 a2af 2440 fdfc ca50 fee7 1f2a  ..P...$@...P...*
-00005880: 492c 7172 82ae 5bc9 a58f e0b9 2e50 06bf  I,qr..[......P..
-00005890: 6f78 7cda 77b2 8209 b84d cc81 ac4d f27f  ox|.w....M...M..
-000058a0: beb7 14d7 6691 98f3 4fb8 8178 0e75 a736  ....f...O..x.u.6
-000058b0: 69d1 2fde 38f6 9000 b65f 5636 d1d3 1e6a  i./.8...._V6...j
-000058c0: 01eb d339 cb6b 156b 4452 a4cd c1f4 90e5  ...9.k.kDR......
-000058d0: 8e35 a639 f4a1 284b 286e 725c 165c d625  .5.9..(K(nr\.\.%
-000058e0: c778 b83e f056 b184 8bb7 9047 f579 e33b  .x.>.V.....G.y.;
-000058f0: ef08 ec8e 25ab 6d6b 22c6 611d 2ce1 0221  ....%.mk".a.,..!
-00005900: 8ec8 241b 5075 e8dc 9cee 52d0 9852 2c37  ..$.Pu....R..R,7
-00005910: 3f81 ba0c 832c f609 7fff 40ea 9c68 4832  ?....,....@..hH2
-00005920: 4e52 07b4 9498 caeb 71ab 27ef 780e 9beb  NR......q.'.x...
-00005930: 3437 6f2c 4d3a 0897 784e e948 fcaf a2c7  47o,M:..xN.H....
-00005940: 8e55 b05d 48ce c592 e088 c8df 8139 40fb  .U.]H........9@.
-00005950: 08cc 6c05 4d32 213c 3a93 064f 4b39 952d  ..l.M2!<:..OK9.-
-00005960: 754c 99d0 27d7 1e30 7c53 6cdc 5aaa 185c  uL..'..0|Sl.Z..\
-00005970: 3e9e 549b a3aa 475e c452 4452 a24e bdd5  >.T...G^.RDR.N..
-00005980: b6b9 51b5 a267 36fc 4d69 fba1 b415 34f5  ..Q..g6.Mi....4.
-00005990: 39b5 acff 308d cfb1 6d25 541a d7a6 ad60  9...0...m%T....`
-000059a0: 6563 ac88 c99c f39e bc39 614b f5b5 046a  ec.......9aK...j
-000059b0: 374f f755 e42c fafe 87af 0e77 6f3a 7d50  7O.U.,.....wo:}P
-000059c0: dcf6 abdf 5463 4ba1 f7f2 88d5 34fb 6640  ....TcK.....4.f@
-000059d0: 2dd4 a3d0 7915 d9ed 375b e81c c04a f83e  -...y...7[...J.>
-000059e0: 40c7 716f df40 b484 c806 5d67 e9a9 54a9  @.qo.@....]g..T.
-000059f0: 5a1b 8665 49f1 574a 4d6f f9ae a1f1 bebb  Z..eI.WJMo......
-00005a00: 0414 3e75 9991 f30f 7aae 9a73 e85e 7f98  ..>u....z..s.^..
-00005a10: 8be7 8ea5 8a6c ef86 2296 1f5b ddfd 0700  .....l.."..[....
-00005a20: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00005a30: 0021 001c 14a7 a8fd 0000 006e 0300 0015  .!.........n....
-00005a40: 0000 0078 6c2f 6368 6172 7473 2f63 6f6c  ...xl/charts/col
-00005a50: 6f72 7331 2e78 6d6c a493 416e c230 1045  ors1.xml..An.0.E
-00005a60: af12 f900 7112 20ad 22c2 a6eb 8a05 2718  ....q. .".....'.
-00005a70: 4d6c 62c9 f620 dba5 707b 9c50 6843 2112  Mlb.. ..p{.PhC!.
-00005a80: c13b fbeb bff9 7f24 2fd1 5748 9adc 261c  .;.....$/.WH..&.
-00005a90: b548 0e46 dbf8 e06b d686 b0ab 38f7 d80a  .H.F...k....8...
-00005aa0: 033e 350a 1d79 9221 4532 9ca4 5428 78e3  .>5..y.!E2..T(x.
-00005ab0: e05b d92d 2fb2 bce0 d882 0b3d 85fd 60e0  .[.-/......=..`.
-00005ac0: 1f85 76c2 c611 929c 81e0 5372 db0b c3e8  ..v.......Sr....
-00005ad0: 48c9 4a6e 4059 9618 11da 9ae1 11b5 6089  H.Jn@Y........`.
-00005ae0: 6a6a 9667 6cb5 84aa 4f23 3eb4 4bf6 a06b  jj.gl...O#>.K..k
-00005af0: 0688 c286 9cf1 875a 31a2 cd46 b4f9 88b6  .......Z1..F....
-00005b00: 18d1 ca4e 8b2b dd83 5310 14d9 9b6b 1754  ...N.+..S....k.T
-00005b10: 7f99 4f6a ce0d ca2c 9ece c3ff 9a86 885b  ..Oj...,.......[
-00005b20: cffb c5d3 a3d6 529e 5171 7dd3 514f 8cbf  ......R.Qq}.QO..
-00005b30: 461e 8e9f 4f18 bf98 e079 bbdf 7ef6 0aea  F...O....y..~...
-00005b40: 89f6 d7c8 c3f6 8f9a 74e4 dfef b53a 0100  ........t....:..
-00005b50: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00005b60: 0021 003b 6d32 4bc1 0000 0042 0100 0023  .!.;m2K....B...#
-00005b70: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00005b80: 2f5f 7265 6c73 2f73 6865 6574 312e 786d  /_rels/sheet1.xm
-00005b90: 6c2e 7265 6c73 848f c18a c230 1445 f703  l.rels.....0.E..
-00005ba0: fe43 787b 93d6 850c 4353 3722 b855 e703  .Cx{....CS7".U..
-00005bb0: 62fa da06 db97 90f7 14fd 7bb3 1c65 c0e5  b.........{..e..
-00005bc0: e570 cfe5 369b fb3c a91b 660e 912c d4ba  .p..6..<..f..,..
-00005bd0: 0285 e463 1768 b0f0 7bda 2dbf 41b1 38ea  ...c.h..{.-.A.8.
-00005be0: dc14 092d 3c90 61d3 2ebe 9a03 4e4e 4a89  ...-<.a.....NNJ.
-00005bf0: c790 5815 0bb1 8551 24fd 18c3 7ec4 d9b1  ..X....Q$...~...
-00005c00: 8e09 a990 3ee6 d949 8979 30c9 f98b 1bd0  ....>..I.y0.....
-00005c10: acaa 6a6d f25f 07b4 2f4e b5ef 2ce4 7d57  ..jm._../N..,.}W
-00005c20: 833a 3d52 59fe ec8e 7d1f 3c6e a3bf ce48  .:=RY...}.<n...H
-00005c30: f2cf 8449 3990 603e a248 39c8 45ed f280  ...I9.`>.H9.E...
-00005c40: 6241 eb77 f69e 6b7d 0e04 a66d cccb f3f6  bA.w..k}...m....
-00005c50: 0900 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00005c60: 0000 0021 0011 98ab c9db 0000 00d0 0100  ...!............
-00005c70: 0023 0000 0078 6c2f 776f 726b 7368 6565  .#...xl/workshee
-00005c80: 7473 2f5f 7265 6c73 2f73 6865 6574 322e  ts/_rels/sheet2.
-00005c90: 786d 6c2e 7265 6c73 ac91 cd4e c330 0c80  xml.rels...N.0..
-00005ca0: ef48 bc43 e43b 49db 0342 68e9 2e68 d2ae  .H.C.;I..Bh..h..
-00005cb0: 301e 2024 6e1b d13a 51ec 017b 7bc2 6112  0. $n..:Q..{{.a.
-00005cc0: 9d26 71e1 e61f f9f3 6779 b3fd 5a66 f581  .&q.....gy..Zf..
-00005cd0: 8563 220b ad6e 4021 f914 228d 165e 0fbb  .c"..n@!.."..^..
-00005ce0: bb07 502c 8e82 9b13 a185 1332 6cfb db9b  ..P,.......2l...
-00005cf0: cd33 ce4e ea10 4f31 b3aa 1462 0b93 487e  .3.N..O1...b..H~
-00005d00: 3486 fd84 8b63 9d32 52ed 0ca9 2c4e 6a5a  4....c.2R...,NjZ
-00005d10: 4693 9d7f 7723 9aae 69ee 4df9 cd80 7ec5  F...w#..i.M...~.
-00005d20: 54fb 60a1 ec43 07ea 70ca 75f3 dfec 340c  T.`..C..p.u...4.
-00005d30: d1e3 53f2 c705 49ae ac30 a1b8 cf7a 5945  ..S...I..0...zYE
-00005d40: ba32 a258 d0fa 5ce3 73d0 eaaa 0ce6 ba4d  .2.X..\.s......M
-00005d50: fb9f 36b9 4412 2c2f 2852 a578 6575 d133  ..6.D.,/(R.xeu.3
-00005d60: 1779 a7df 22fd 489a d51f fa6f 0000 00ff  .y..".H....o....
-00005d70: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00005d80: 0081 c55e bdca 0000 0035 0200 0023 0000  ...^.....5...#..
-00005d90: 0078 6c2f 6472 6177 696e 6773 2f5f 7265  .xl/drawings/_re
-00005da0: 6c73 2f64 7261 7769 6e67 312e 786d 6c2e  ls/drawing1.xml.
-00005db0: 7265 6c73 bc91 cf0a c230 0c87 ef82 ef50  rels.....0.....P
-00005dc0: 72b7 dd26 8888 dd2e 2278 157d 80d0 657f  r..&...."x.}..e.
-00005dd0: 706b 4b53 45df de82 080a a237 4f21 09f9  pkKSE......7O!..
-00005de0: 7e1f 645d 5dc7 415c 2870 efac 865c 6620  ~.d]].A\(p...\f 
-00005df0: c81a 57f7 b6d5 703c 6c67 4b10 1cd1 d638  ..W...p<lgK....8
-00005e00: 384b 1a6e c450 95d3 c97a 4f03 c674 c45d  8K.n.P...zO..t.]
-00005e10: ef59 248a 650d 5d8c 7ea5 149b 8e46 64e9  .Y$.e.].~....Fd.
-00005e20: 3cd9 b469 5c18 31a6 36b4 caa3 3961 4baa  <..i\.1.6...9aK.
-00005e30: c8b2 850a af0c 28df 9862 576b 08bb 7a0e  ......(..bWk..z.
-00005e40: e270 f329 f937 db35 4d6f 68e3 cc79 241b  .p.).7.5Moh..y$.
-00005e50: 3f44 28d3 6188 0988 a1a5 a841 cac7 841f  ?D(.a......A....
-00005e60: 652e 932c a8cf 1ec5 ff3c 8a6f 1ef9 ff3c  e..,.....<.o...<
-00005e70: f2a7 877a 7b76 7907 0000 ffff 0300 504b  ...z{vy.......PK
-00005e80: 0304 1400 0600 0800 0000 2100 801b dc81  ..........!.....
-00005e90: d200 0000 8f01 0000 1f00 0000 786c 2f63  ............xl/c
-00005ea0: 6861 7274 732f 5f72 656c 732f 6368 6172  harts/_rels/char
-00005eb0: 7433 2e78 6d6c 2e72 656c 73ac 90c1 4ac4  t3.xml.rels...J.
-00005ec0: 3010 86ef 82ef 10e6 6ed3 ec41 4436 dd83  0.......n..AD6..
-00005ed0: 20ec 55d7 0708 e9b4 0d9b 64c2 4c10 fbf6   .U.......d.L...
-00005ee0: a617 b18b 478f 33c3 ff7d 3f73 3c7d a5a8  ....G.3..}?s<}..
-00005ef0: 3e91 2550 b660 ba1e 1466 4f63 c8b3 858f  >.%P.`...fOc....
-00005f00: cbeb c313 28a9 2e8f 2e52 460b 2b0a 9c86  ....(....RF.+...
-00005f10: fbbb e31b 4657 5b48 9650 4435 4a16 0b4b  ....FW[H.PD5J..K
-00005f20: ade5 596b f10b 2627 1d15 cced 3211 2757  ..Yk..&'....2.'W
-00005f30: dbc8 b32e ce5f dd8c fad0 f78f 9a7f 3360  ....._........3`
-00005f40: d831 d579 b4c0 e7f1 00ea b296 66be 61a7  .1.y........f.a.
-00005f50: e099 84a6 da79 4a9a a629 f88d 6acc 9eaa  .....yJ..)..j...
-00005f60: fde2 b8be 5024 7eaf 6bc4 4673 3c63 b5e0  ....P$~.k.Fs<c..
-00005f70: b79d 98ae 1504 fdb7 dbfc 87fb 462b 5b8b  ............F+[.
-00005f80: 1fab debd 71f8 0600 00ff ff03 0050 4b03  ....q........PK.
-00005f90: 0414 0006 0008 0000 0021 00a5 bb49 2774  .........!...I't
-00005fa0: 0100 004b 0300 0022 0000 0078 6c2f 6578  ...K..."...xl/ex
-00005fb0: 7465 726e 616c 4c69 6e6b 732f 6578 7465  ternalLinks/exte
-00005fc0: 726e 616c 4c69 6e6b 312e 786d 6c9c 535d  rnalLink1.xml.S]
-00005fd0: 6bc2 3014 7d1f ec3f 84bc 6bda 6e8c 596c  k.0.}..?..k.n.Yl
-00005fe0: 85a1 0361 8c81 db0f b8a6 b71a cc47 49a2  ...a.........GI.
-00005ff0: d47f bf34 ba6e 4e07 b2b7 e6e4 de73 ce3d  ...4.nN......s.=
-00006000: 371d 4f5a 25c9 0ead 1346 1734 1d26 94a0  7.OZ%....F.4.&..
-00006010: e6a6 127a 55d0 8ff7 e7c1 2325 ce83 ae40  ...zU.....#%...@
-00006020: 1a8d 05dd a3a3 93f2 f666 8cad 47ab 41be  .........f..G.A.
-00006030: 08bd 2181 44bb 82ae bd6f 72c6 1c5f a302  ..!.D....or.._..
-00006040: 3734 0dea 7053 1bab c087 a35d 31d7 5884  74..pS.....]1.X.
-00006050: caad 11bd 922c 4b92 07a6 4068 7a60 c815  .....,K...@hz`..
-00006060: bf86 4481 dd6c 9b01 37aa 012f 9642 0abf  ..D..l..7../.B..
-00006070: 8f5c 9428 9ecf 57da 5858 ca60 b64d ef49  .\.(..W.XX.`.M.I
-00006080: dbca 2cfd e20f c099 8012 dc1a 676a 3f0c  ..,.........gj?.
-00006090: 84cc d4b5 e078 ee73 c446 274e 23ed ffb8  .....x.s.F'N#...
-000060a0: b294 85f0 64c8 cd65 49f0 56f6 593e 1973  ....d..eI.V.Y>.s
-000060b0: cc32 b7d7 0471 303b 357c ab50 fb43 9c16  .2...q0;5|.P.C..
-000060c0: 6508 c568 b716 8da3 c4e6 a22a a89d 579d  e..h.......*..W.
-000060d0: 4e34 9d83 8c9b f3f8 61a5 ebc1 a533 721b  N4......a....3r.
-000060e0: b1ef 9e8c b272 cc2e 76c5 15be 82c2 c0d0  .....r..v.......
-000060f0: 7f93 1dc8 82ce da06 bbc6 5ff0 c287 4770  .........._...Gp
-00006100: 019f 85a6 0bf0 1b58 50b1 9e9d 694d c1c3  .......XP...iM..
-00006110: 02fd 51a2 3b91 5833 0fa3 263d d729 9efe  ..Q.;.X3..&=.)..
-00006120: 81c7 1963 f769 fd5d 9cbd bf88 72dd dee2  ...c.i.]....r...
-00006130: a3ef 1615 92f9 f90f 949f 0000 00ff ff03  ................
-00006140: 0050 4b03 0414 0006 0008 0000 0021 0090  .PK..........!..
-00006150: 000d b0a6 0100 00dd 0200 000f 0000 0078  ...............x
-00006160: 6c2f 6d65 7461 6461 7461 2e78 6d6c 6451  l/metadata.xmldQ
-00006170: 4b4f 1b31 10be 57e2 3f58 be6f bc21 1442  KO.1..W.?X.o.!.B
-00006180: b4bb 2802 e544 2554 28ea d5b1 c789 55bf  ..(..D%T(.....U.
-00006190: 647b 6956 55ff 7b67 bd84 0638 d9e3 197f  d{iVU.{g...8....
-000061a0: f33d 9a9b 8335 e405 62d2 deb5 743e ab29  .=...5..b...t>.)
-000061b0: 0127 bcd4 6ed7 d21f 4f9b 6a49 49ca dc49  .'..n...O.jII..I
-000061c0: 6ebc 8396 0e90 e84d 77f6 a5b1 90b9 e499  n......Mw.......
-000061d0: 1304 70a9 a5fb 9cc3 8ab1 24f6 6079 9af9  ..p.......$.`y..
-000061e0: 000e 3bca 47cb 3396 71c7 5288 c065 da03  ..;.G.3.q.R..e..
-000061f0: 646b d879 5d5f 32cb b5a3 13c2 ea20 f927  dk.y]_2...... .'
-00006200: 14ab 45f4 c9ab 3c13 de32 af94 16f0 0967  ..E...<..2.....g
-00006210: 7ec5 e4e0 38ce f218 f940 bb37 6e4f 4380  ~...8....@.7nOC.
-00006220: 4484 ef5d 466d 1f1a 04bf a0a0 9ff7 77eb  D..]Fm........w.
-00006230: 87ef 9458 ed1e fb10 7ccc 209f dffc 4096  ...X....|. ...@.
-00006240: 355a 227c 1846 0412 78ca b036 e67f f1cc  5Z"|.F..x..6....
-00006250: 4d0f a81f 9b16 e20e 11f1 9682 d179 a363  M............y.c
-00006260: 2a7b 49f4 bf6f bd79 dc6b 35d5 c200 8f9b  *{I..o.y.k5.....
-00006270: c99a 325f 1e6e bdb5 e0f2 84c5 53d2 bb31  ..2_.n......S..1
-00006280: 9171 3944 31e1 0a30 e61b 1a3f beb3 ae61  .q9D1..0...?...a
-00006290: c710 8ad0 ae51 7dee 238c 0325 99f7 024f  .....Q}.#..%...O
-000062a0: 6cd8 feea 1a38 e4fb 94cb 49fa a85b fa67  l....8....I..[.g
-000062b0: 2bb7 dba5 90a2 527c 0ed5 c5f5 2554 7cf9  +.....R|....%T|.
-000062c0: f5aa 5a88 855a d4a2 3ebf 168b bf68 2206  ..Z..Z..>....h".
-000062d0: b57a 357c 3d1a fe10 31ec 9835 5aad eea6  .z5|=...1..5Z...
-000062e0: 200a 6f85 9a0d 0f09 644b eb42 1777 22e9   .o.....dK.B.w".
-000062f0: e366 36d2 60ef 3977 cd51 6251 f081 7314  .f6.`.9w.QbQ..s.
-00006300: 6432 f0e5 8858 204e bf9c 98d2 fd03 0000  d2...X N........
-00006310: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00006320: 2100 3585 fa75 af01 0000 3c10 0000 2700  !.5..u....<...'.
-00006330: 0000 786c 2f70 7269 6e74 6572 5365 7474  ..xl/printerSett
-00006340: 696e 6773 2f70 7269 6e74 6572 5365 7474  ings/printerSett
-00006350: 696e 6773 312e 6269 6eec 57bd 4a03 4110  ings1.bin.W.J.A.
-00006360: feee 1221 f102 b148 6161 112b 1b0b 8580  ...!...Haa.+....
-00006370: 969a 68a1 a807 3142 ca88 1114 248a 492f  ..h...1B....$.I/
-00006380: 3e83 9de0 03f8 0abe 85a5 20d8 08fa 00b6  >......... .....
-00006390: 12e7 cb65 c9ba b777 2954 44d9 5926 fb33  ...e...w)TD.Y&.3
-000063a0: b333 b35f be62 ae86 7d74 702a 5a46 03bb  .3._.b..}tp*ZF..
-000063b0: 5842 050b 32ca e8e2 10e7 3896 df2e 92c5  XB..2.....8.....
-000063c0: cb06 8547 b48a 99a7 cb8c 873c ae83 4aae  ...G.......<..J.
-000063d0: 0d0f 25ef bdef cb0c 510f ab12 f5fb 85d1  ..%.....Q.......
-000063e0: fd41 0666 894b ab08 5437 d7b6 8342 649b  .A.f.K..T7...Bd.
-000063f0: 0980 0759 5295 f05e ae0e 647b c0bc 6c1a  ...YR..^..d{..l.
-00006400: a2ad 1078 3e8b ef4d 3ffa be59 fcd5 b98a  ...x>..M?..Y....
-00006410: 67fa 35fd a63f 8d2a ea08 b187 0d6c c908  g.5..?.*.....l..
-00006420: b1f3 0308 8d0f b98e 031c 0d38 d093 fffa  ...........8....
-00006430: 4446 c485 0eee 8403 8bbf 52d3 5793 4ecd  DF........R.W.N.
-00006440: fdc9 b25d d10e 0187 8043 c021 e010 8821  ...].....C.!...!
-00006450: c03e 2733 541a a3de ca06 943f f073 103a  .>'3T......?.s.:
-00006460: 0446 08e4 a533 1ff1 875c 3225 2b07 ec85  .F...3...\2%+...
-00006470: c9b1 922c 3853 6c7d 35cf 6957 bdb7 e9d7  ...,8Sl}5.iW....
-00006480: 9603 e653 fd32 ede6 5ed5 107d 2124 e719  ...S.2..^..}!$..
-00006490: 9681 2bb5 9079 6532 f2e7 dd59 ed5c 5fd2  ..+..ye2...Y.\_.
-000064a0: d6ef 7f36 cab5 98d8 de97 f466 fd9d 666c  ...6.......f..fl
-000064b0: 1353 1523 2996 8e0d 7d2e 0cd5 7371 fd22  .S.#)...}...sq."
-000064c0: 801b cfb1 be3c adf6 04a8 5231 b161 c65a  .....<....R1.a.Z
-000064d0: c6c9 84e6 a0b0 d1f9 62de 7f1d c6b4 e196  ........b.......
-000064e0: 842d 39ab 44f1 28ad ae34 aed9 7063 7c72  .-9.D.(..4..pc|r
-000064f0: 795c 4cda f55a 947f ed1f 7f5b df2f dfdc  y\L..Z.....[./..
-00006500: 7e00 0000 ffff 0300 504b 0304 1400 0600  ~.......PK......
-00006510: 0800 0000 2100 3585 fa75 af01 0000 3c10  ....!.5..u....<.
-00006520: 0000 2700 0000 786c 2f70 7269 6e74 6572  ..'...xl/printer
-00006530: 5365 7474 696e 6773 2f70 7269 6e74 6572  Settings/printer
-00006540: 5365 7474 696e 6773 322e 6269 6eec 57bd  Settings2.bin.W.
-00006550: 4a03 4110 feee 1221 f102 b148 6161 112b  J.A....!...Haa.+
-00006560: 1b0b 8580 969a 68a1 a807 3142 ca88 1114  ......h...1B....
-00006570: 248a 492f 3e83 9de0 03f8 0abe 85a5 20d8  $.I/>......... .
-00006580: 08fa 00b6 12e7 cb65 c9ba b777 2954 44d9  .......e...w)TD.
-00006590: 5926 fb33 b333 b35f be62 ae86 7d74 702a  Y&.3.3._.b..}tp*
-000065a0: 5a46 03bb 5842 050b 32ca e8e2 10e7 3896  ZF..XB..2.....8.
-000065b0: df2e 92c5 cb06 8547 b48a 99a7 cb8c 873c  .......G.......<
-000065c0: ae83 4aae 0d0f 25ef bdef cb0c 510f ab12  ..J...%.....Q...
-000065d0: f5fb 85d1 fd41 0666 894b ab08 5437 d7b6  .....A.f.K..T7..
-000065e0: 8342 649b 0980 0759 5295 f05e ae0e 647b  .Bd....YR..^..d{
-000065f0: c0bc 6c1a a2ad 1078 3e8b ef4d 3ffa be59  ..l....x>..M?..Y
-00006600: fcd5 b98a 67fa 35fd a63f 8d2a ea08 b187  ....g.5..?.*....
-00006610: 0d6c c908 b1f3 0308 8d0f b98e 031c 0d38  .l.............8
-00006620: d093 fffa 4446 c485 0eee 8403 8bbf 52d3  ....DF........R.
-00006630: 5793 4ecd fdc9 b25d d10e 0187 8043 c021  W.N....].....C.!
-00006640: e010 8821 c03e 2733 541a a3de ca06 943f  ...!.>'3T......?
-00006650: f073 103a 0446 08e4 a533 1ff1 875c 3225  .s.:.F...3...\2%
-00006660: 2b07 ec85 c9b1 922c 3853 6c7d 35cf 6957  +......,8Sl}5.iW
-00006670: bdb7 e9d7 9603 e653 fd32 ede6 5ed5 107d  .......S.2..^..}
-00006680: 2124 e719 9681 2bb5 9079 6532 f2e7 dd59  !$....+..ye2...Y
-00006690: ed5c 5fd2 d6ef 7f36 cab5 98d8 de97 f466  .\_....6.......f
-000066a0: fd9d 666c 1353 1523 2996 8e0d 7d2e 0cd5  ..fl.S.#)...}...
-000066b0: 7371 fd22 801b cfb1 be3c adf6 04a8 5231  sq.".....<....R1
-000066c0: b161 c65a c6c9 84e6 a0b0 d1f9 62de 7f1d  .a.Z........b...
-000066d0: c6b4 e196 842d 39ab 44f1 28ad ae34 aed9  .....-9.D.(..4..
-000066e0: 7063 7c72 795c 4cda f55a 947f ed1f 7f5b  pc|ry\L..Z.....[
-000066f0: df2f dfdc 7e00 0000 ffff 0300 504b 0304  ./..~.......PK..
-00006700: 1400 0600 0800 0000 2100 08f5 5e11 4603  ........!...^.F.
-00006710: 0000 5e13 0000 1000 0000 786c 2f63 616c  ..^.......xl/cal
-00006720: 6343 6861 696e 2e78 6d6c 7c58 cb6e db40  cChain.xml|X.n.@
-00006730: 0cbc 17e8 3f08 ba37 8ad4 3669 8b38 41f6  ....?..7..6i.8A.
-00006740: 05b4 e831 fd00 c151 6303 b61c 5846 d1fe  ...1...Qc...XF..
-00006750: 7d37 71b4 5c52 9cbd 1830 49cf 92b3 4372  }7q.\R...0I...Cr
-00006760: e19b bbbf fb5d f567 384e dbc3 b8aa db8b  .....].g8N......
-00006770: cbba 1ac6 f5e1 713b 3ead ea5f 0fe1 c397  ......q;>.._....
-00006780: ba9a 4efd f8d8 ef0e e3b0 aaff 0d53 7d77  ..N..........S}w
-00006790: fbfe ddcd badf aded a6df 8e55 4418 a755  ...........UD..U
-000067a0: bd39 9d9e bf35 cdb4 de0c fb7e ba38 3c0f  .9...5.....~.8<.
-000067b0: 63f4 fc3e 1cf7 fd29 7e3d 3e35 d3f3 71e8  c..>...)~=>5..q.
-000067c0: 1fa7 cd30 9cf6 bba6 bbbc bc6a f611 a0be  ...0.......j....
-000067d0: bd59 57c7 556d bab6 aeb6 ab3a 9eb8 8ba9  .YW.Um.....:....
-000067e0: d455 fff2 d92c bdf1 30b2 ffec 5e7f 741d  .U...,..0...^.t.
-000067f0: d364 e1ed d719 8cc3 909d c5df 2398 98cd  .d..........#...
-00006800: 3927 0193 ec0c c67e 66d9 f012 8473 aecc  9'.....~f....s..
-00006810: 5ea9 15d8 5852 3c79 2e4c 4071 6782 3a67  ^...XR<y.L@qg.:g
-00006820: 25c9 b067 2e00 1477 26a8 364a 213b 9fee  %..g...w&.6J!;..
-00006830: e16c 8f27 89fb 4976 7111 e754 5f74 a4dc  .l.'..Ivq..T_t..
-00006840: 6acb bdf3 2941 bf8e efb3 42e6 b81f 294e  j...)A....B...)N
-00006850: 910c 39b9 62ce 20d7 495a e14d 1399 a5d3  ..9.b. .IZ.M....
-00006860: 8b0f 6fe9 e6bf d529 7749 088c 2532 b394  ..o....)wI..%2..
-00006870: 9c2e 0157 9280 70ce 8c38 904f 4902 4e97  ...W..p..8.OI.N.
-00006880: 8003 1270 edc7 8234 a537 5da9 ce48 e01d  ...p...4.7]..H..
-00006890: 93a2 7546 4289 11e1 4c50 3a23 a1c4 8870  ..uFB...LP:#...p
-000068a0: 2628 c048 6867 4d69 2297 de19 ed5e 0ad1  &(.HhgMi"....^..
-000068b0: e814 9199 7796 4e91 2951 249c a9a9 758a  ....w.N.)Q$...u.
-000068c0: 4c89 22e1 4c50 686e b49f 0aa2 31c2 3ba3  L.".LPhn....1.;.
-000068d0: 799d 1132 3346 bcce 882f 3122 9ce9 609d  y..23F.../1"..`.
-000068e0: 115f 6244 3813 1460 c417 db48 7a69 32a6  ._bD8..`...Hzi2.
-000068f0: 22d9 6409 1de8 984e 5f15 669e 9c34 d839  ".d....N_.f..4.9
-00006900: 801c ef40 6d00 de4a 78fb b6dd c112 12de  ...@m..Jx.......
-00006910: 34cd 248c 2b8e 1eee 4c17 2041 7c31 17e9  4.$.+...L. A|1..
-00006920: 25e6 5393 0be6 79f3 a7f8 2478 1ece fb80  %.S...y...$x....
-00006930: d0d3 2a13 e8fa 2a0c 9d5e 6c48 660e 03a2  ..*...*..^lHf...
-00006940: 3b90 24d9 5987 854e 1fd7 9606 203b 36b3  ;.$.Y..N.... ;6.
-00006950: f377 12f5 bb88 d7d9 b1d4 2b22 5eaf cbb6  .w........+"^...
-00006960: 3a9b 995d 7d2e 4675 be3e 24a8 29f4 8780  :..]}.Fu.>$.)...
-00006970: 5b3c 191c 7832 f845 a407 9176 1169 21e6  [<..x2.E...v.i!.
-00006980: dcd3 3463 c0da 5f3c 585c 0bde 888b 480b  ..4c.._<X\....H.
-00006990: 22cd 22d2 c048 5d8c 464c 3eda 1d7a 8719  "."..H].FL>..z..
-000069a0: b15e 295e bf65 43b7 cff7 0350 9d47 db07  .^)^.eC....P.G..
-000069b0: a8da 837c 02c0 cfec fcd9 a737 9fd3 7bc0  ...|.......7..{.
-000069c0: 014d 6776 deab a067 0260 df03 fccc ceb3  .Mgv...g.`......
-000069d0: 07d5 3ac0 6600 f899 9df7 2410 8fde f146  ..:.f.....$....F
-000069e0: e792 cc5c 09b4 2dd9 3cf1 608b 7ab0 e61c  ...\..-.<.`.z...
-000069f0: c0c9 ec9c 33b8 8d41 fa60 0e1b 3087 4d07  ....3..A.`..0.M.
-00006a00: 3a82 ec9c 63b0 451c 507e 6617 75e9 9deb  :...c.E.P~f.u...
-00006a10: c05e b7fa dd92 59a0 8346 01ec 38c0 8e03  .^....Y..F..8...
-00006a20: ec64 7671 2e7a 50e8 f978 908f 475b 13e4  .dvq.zP..x..G[..
-00006a30: 63c1 6d59 705b 166c f1cc ceb7 2fc8 c783  c.mYp[.l..../...
-00006a40: b2f4 79e4 f53b 24b3 501a 98ed 4021 1e70  ..y..;$.P...@!.p
-00006a50: 93d9 4547 8397 805e 9305 ef0c d0cf 16cc  ..EG...^........
-00006a60: 05bb ece7 26fd 3376 fb1f 0000 ffff 0300  ....&.3v........
-00006a70: 504b 0304 1400 0600 0800 0000 2100 a329  PK..........!..)
-00006a80: 0c19 4d01 0000 6902 0000 1100 0801 646f  ..M...i.......do
-00006a90: 6350 726f 7073 2f63 6f72 652e 786d 6c20  cProps/core.xml 
-00006aa0: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
-00006ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000d20: 0000 0000 0000 00bc 94cb 6ac3 3010 45f7  ..........j.0.E.
+00000d30: 85fe 83d1 be96 edb4 6929 91b3 6829 64d1  ........i)..h)d.
+00000d40: 4d9b 7ec0 208f 1fc4 968c 66fa f0df 5798  M.~. .....f...W.
+00000d50: 6227 10d4 8dc9 4630 77d0 bd07 0d9a cdf6  b'....F0w.......
+00000d60: a76b a32f 74d4 58a3 441a 2722 42a3 6dd1  .k./t.X.D.'"B.m.
+00000d70: 984a 898f fdcb cd83 8888 c114 d05a 834a  .J...........Z.J
+00000d80: 0c48 629b 5f5f 6dde b005 f697 a86e 7a8a  .Hb.__m......nz.
+00000d90: bc8b 2125 6ae6 fe51 4ad2 3576 40b1 edd1  ..!%j..QJ.5v@...
+00000da0: f84e 695d 07ec 4b57 c91e f401 2a94 5992  .Ni]..KW....*.Y.
+00000db0: aca5 3bf6 10f9 8967 b42b 9470 bbc2 e7ef  ..;....g.+.p....
+00000dc0: 87de 27ff ef6d cbb2 d1f8 6cf5 6787 86cf  ..'..m....l.g...
+00000dd0: 4448 0dad 7eaa a131 de14 5c85 acc4 24c5  DH..~..1..\...$.
+00000de0: 9e54 c8f3 10ab 2521 bead 3b50 8dc8 33c4  .T....%!..;P..3.
+00000df0: 2491 1c3b ab10 ccfd 9230 63dc 2b32 14c0  $..;.....0c.+2..
+00000e00: 3003 757f 4a88 23bb f0a3 6421 98f4 c230  0.u.J.#...d!...0
+00000e10: 6908 66bd ec84 c061 f1ce ce7f 499a 2744  i.f....a....I.'D
+00000e20: f591 1c82 b95b 1486 87d6 6f80 e9f7 d058  .....[....o....X
+00000e30: 87e2 6f97 8c67 bf57 704e 1f4b 399e d33c  ..o..g.WpN.K9..<
+00000e40: e4c9 62ca 7f01 0000 ffff 0300 504b 0304  ..b.........PK..
+00000e50: 1400 0600 0800 0000 2100 1b27 8488 1706  ........!..'....
+00000e60: 0000 2512 0000 1800 0000 786c 2f77 6f72  ..%.......xl/wor
+00000e70: 6b73 6865 6574 732f 7368 6565 7431 2e78  ksheets/sheet1.x
+00000e80: 6d6c ac55 db8e da30 107d afd4 7f88 fc4e  ml.U...0.}.....N
+00000e90: 8273 e322 c28a 4b51 57da 87d5 6e2f cf26  .s."..KQW...n/.&
+00000ea0: 71c0 da24 4e6d b340 abfe 7bc7 ce05 76d9  q..$Nm.@..{...v.
+00000eb0: 22d8 5602 ec38 9933 67ce 9c09 a39b 5d9e  ".V..8.3g.....].
+00000ec0: 59cf 5448 c68b 0861 bb8b 2c5a c43c 61c5  Y.TH...a..,Z.<a.
+00000ed0: 2a42 5fbf 2c3a 7d64 4945 8a84 64bc a011  *B_.,:}dIE..d...
+00000ee0: da53 896e c61f 3f8c b65c 3cc9 35a5 ca02  .S.n..?..\<.5...
+00000ef0: 8442 4668 ad54 3974 1c19 af69 4ea4 cd4b  .BFh.T9t...iN..K
+00000f00: 5ac0 9d94 8b9c 28b8 142b 4796 8292 c404  Z.....(..+G.....
+00000f10: e599 e376 bba1 9313 56a0 0a61 282e c1e0  ...v....V..a(...
+00000f20: 69ca 623a e7f1 26a7 85aa 4004 cd88 02fe  i.b:..&...@.....
+00000f30: 72cd 4ad9 a0e5 f125 7039 114f 9bb2 13f3  r.J....%p9.O....
+00000f40: bc04 8825 cb98 da1b 5064 e5f1 f076 5570  ...%....Pd...vUp
+00000f50: 4196 19d4 bdc3 3e89 ad9d 808f 0b5f af49  A.....>......_.I
+00000f60: 63ce 4f32 e52c 165c f254 d980 ec54 9c4f  c.O2.,.\.T...T.O
+00000f70: cb1f 3803 87c4 2dd2 69fd 17c1 60df 11f4  ..8...-.i...`...
+00000f80: 99e9 061e a0dc f751 c241 8be5 1ec0 bc77  .......Q.A.....w
+00000f90: 8285 2d98 964b 0c37 2c89 d0af 6930 9db9  ..-..K.7,...i0..
+00000fa0: f320 e8f4 bbde a0e3 7f1a f43b 8305 86cb  . .........;....
+00000fb0: c974 31f0 e653 3770 27bf d178 647c 722f  .t1..S7p'..xd|r/
+00000fc0: c623 be51 192b e8bd b0e4 2687 86ed a734  .#.Q.+....&....4
+00000fd0: e3db 0881 55eb 8307 b65a 2b7d e08c 474e  ....U....Z+}..GN
+00000fe0: 1b97 30b0 8896 c512 348d d004 0f1f 43fd  ..0.....4.....C.
+00000ff0: 8479 e01b a35b 79b4 b714 593e d28c c68a  .y...[y...Y>....
+00001000: 0249 8c2c edef 25e7 4ffa c15b 38ea 02a5  .I.,..%.O..[8...
+00001010: 9214 d4da 3d96 e092 0881 40fb c356 f1f2  ....=.....@..V..
+00001020: 8ea6 6a46 b32c 4233 a897 c48a 3dd3 7b88  ..jF.,B3....=.{.
+00001030: 88d0 922b c573 c3d2 4c93 82b3 54f0 9fb4  ...+.s..L...T...
+00001040: 307c 4c5a cd53 e347 08a0 ea47 2b8c 1a13  0|LZ.S.G...G+...
+00001050: 38c9 1fa6 9219 7e2b ac4a a249 34c9 abc0  8.....~+.J.I4...
+00001060: 0990 a903 61ab eb7f 95ef 05bb 1729 0f91  ....a........)..
+00001070: 5051 abad 56a4 d1f9 58c6 8519 7568 5342  PQ..V...X...uhSB
+00001080: 53b2 c9d4 03df 7ea6 5567 b06f fbc8 aa1b  S.....~.Ug.o....
+00001090: 7947 9f69 36e3 a013 9464 e667 98ec e754  yG.i6....d.g...T
+000010a0: c630 d0a0 b36d 52c5 3c83 f6c0 af95 33fd  .0...mR.<.....3.
+000010b0: 6282 7924 bbaa 312c 51eb 0801 b725 956a  b.y$..1,Q....%.j
+000010c0: a15b 0177 e38d 0489 bf57 f78c 3e6d 2c34  .[.w.....W..>m,4
+000010d0: cac4 c2ba adee bbbe 1d86 7e37 7483 b381  ..........~7t...
+000010e0: 90c2 0402 f53a b06f f7fb 610f f77b 1028  .....:.o..a..{.(
+000010f0: d55e bf18 7a5a 9836 179c 9b10 58df 0879  .^..zZ.6....X..y
+00001100: 45f2 8520 ba8a 63a4 b046 82f5 efc9 3150  E.. ..c..F....1P
+00001110: bb06 b457 83c2 7a06 1406 eb1a 50f8 8730  ...W..z.....P..0
+00001120: 35c3 7a06 f4b4 4767 cb1f d4a0 b05e aa3d  5.z...Gg.....^.=
+00001130: 6e4d a2c7 b776 8267 7b9e dbf5 b06e 75dd  nM...v.g{....nu.
+00001140: b16b 45c3 8d81 f4e6 ffc9 861b 7be9 4d43  .kE.........{.MC
+00001150: 17db 41e0 87c7 fed2 555d d30d 5d5d 352a  ..A.....U]..]]5*
+00001160: 07db fa76 afd7 f37c 4fdb f6cc a0e0 c6bd  ...v...|O.......
+00001170: 7a53 333a 137a b67f b8f1 afde fce3 28e0  zS3:.z........(.
+00001180: c6b6 f8e0 862b 7939 e67d f207 0000 ffff  .....+y9.}......
+00001190: 0000 00ff ffac 95db 7282 3010 865f c5c9  ........r.0.._..
+000011a0: 0314 0272 d041 66aa 8807 144f 4fc0 5066  ...r.Af....OO.Pf
+000011b0: 7aa3 7484 daf6 ed1b 481a b24b a6f4 a277  z.t.....H..K...w
+000011c0: fae7 cbee 9fdd 6409 aad7 a2a8 a3ac cec2  ......d.........
+000011d0: e05e 7e8c ee33 42c9 a87a cb6e 15fb 35a5  .^~..3B..z.n..5.
+000011e0: 13f6 a795 f2f7 aa2e af71 79bf 6675 2b7c  .........qy.fu+|
+000011f0: d271 964f 5fbe a2a2 ca8b 1bd3 cc27 9b84  .q.O_........'..
+00001200: 41de 8478 6e62 cc88 4f0c 21cc 7f84 1103  A..xnb..O.!.....
+00001210: 2b86 3d42 2b30 1e61 60e4 8258 70c2 251d  +.=B+0.a`..Xp.%.
+00001220: e1d8 1089 38c2 2cc9 2063 482c 71de 980b  ....8.,. cH,q...
+00001230: d492 4e56 4271 a4b2 168a 2795 8dc6 8b03  ..NVBq....'.....
+00001240: 3325 6293 2d37 ed84 e24a 652f 94ae 0ca9  3%b.-7...Je/....
+00001250: 50d4 23d0 ee94 06eb 806c 83f5 0f6d 6862  P.#......l...mhb
+00001260: b4cd 9205 f351 4de7 7d04 110b 4ea8 8dc1  .....QM.}...N...
+00001270: 7d19 2496 fd2c a89e b120 6ca5 b92e 2cf9  }.$..,... l...,.
+00001280: 4a20 aa13 0f22 6b81 f84a 141f 229b 41b3  J ..."k..J..".A.
+00001290: dbbe 5917 9d38 1976 bb1b 76bb 1f76 9bf6  ..Y..8.v..v..v..
+000012a0: bd50 74e7 0f1a 0415 f738 d8e4 93e6 cc28  .Pt......8.....(
+000012b0: c8b9 8f78 a8fc 170d d295 1fdc 6ed6 6730  ...x........n.g0
+000012c0: 647e 9d26 eaa5 f0d1 f1e7 eae2 04cd 9426  d~.&...........&
+000012d0: cb8c 78ea 4c41 6327 d220 78a8 a819 a809  ..x.LAc'. x.....
+000012e0: 53c4 7c3f 1d2b 3928 4517 5730 a6ca 201f  S.|?.+9(E.W0.. .
+000012f0: 6bc1 b001 21df 2a45 0f60 a3f1 8a90 adc6  k...!.*E.`......
+00001300: 8e8b ce93 6818 0775 72a7 b1ec a097 b4d7  ....h..ur.......
+00001310: 5876 5007 52f0 9e51 ed0e 6011 15ed 0816  XvP.R..Q..`.....
+00001320: 51b5 4eea a287 6a70 068b c8d0 455d f43b  Q.N...jp....E].;
+00001330: 43e0 72b2 09f3 e7cb b96c 6036 63a9 1cfb  C.r......l`6c...
+00001340: 0957 acf6 7bc2 e31a dd57 f61b 0000 ffff  .W..{....W......
+00001350: 0000 00ff ff6c 514d 4f83 4010 fd2b 9b49  .....lQMO.@..+.I
+00001360: d368 62e5 abd8 4281 0444 921e 34d1 5ebc  .hb...B..D..4.^.
+00001370: ae65 818d 945d 8741 5b8d ffdd a5b5 8907  .e...].A[.......
+00001380: 6ff3 e6e3 bd99 3711 1f48 15b2 2581 0c45  o.....7..H..%..E
+00001390: 1543 e686 8f2e b03d 8683 2c63 f8ca fcec  .C.....=..,c....
+000013a0: d6cd 7d7f b6b4 bd60 36bf 0b96 b3a0 700c  ..}....`6.....p.
+000013b0: 4cb3 22f0 f2cc f5dd f41b ac24 daaa ae94  L."........$....
+000013c0: 2455 c7db 42e1 8e13 c9ae 66fd db91 35f5  $U..B.....f...5.
+000013d0: c2e7 2277 6cdb 06d3 593d 0dad 6074 d022  .."wl...Y=..`t."
+000013e0: 06b1 d728 fade cc01 2bf7 d5da 68da c034  ...(....+...h..4
+000013f0: 4a85 920e 3138 66a0 327c 43cb 93f4 21bf  J...18f.2|C...!.
+00001400: 9864 deb4 a5d5 b4a6 d524 73af d81f 0c70  .d.......$s....p
+00001410: 1959 e7de c83a c924 26f8 6fb3 24d2 bc16  .Y...:.$&.o.$...
+00001420: f71c 6bd9 f5ac 1515 19e1 eb05 3094 7573  ..k.........0.us
+00001430: 8e49 e963 d607 f6a2 88d4 ee8c 1ac1 4b81  .I.c..........K.
+00001440: 23f2 8055 4a19 fb4e c018 31f2 6e04 0d9a  #..UJ..N..1.n...
+00001450: 69ae 056e e4a7 3933 0066 0e12 1df1 d1a2  i..n..93.f......
+00001460: 18b4 4242 2e09 5863 f29f ca14 da5c cb18  ..BB..Xc.....\..
+00001470: e66e 300f 6e16 6e60 88df 0592 dcfe 168c  .n0.n.n`........
+00001480: 2b18 8e2f c175 e98c 865b 1f0a 5ffb 4608  +../.u...[.._.F.
+00001490: 4a7e 0000 00ff ff03 0050 4b03 0414 0006  J~.......PK.....
+000014a0: 0008 0000 0021 00d4 ad59 0d95 0b00 00ae  .....!...Y......
+000014b0: 5400 0018 0000 0078 6c2f 776f 726b 7368  T......xl/worksh
+000014c0: 6565 7473 2f73 6865 6574 322e 786d 6c9c  eets/sheet2.xml.
+000014d0: 9459 6fe2 3010 c7df 57da ef10 f93d 7742  .Yo.0...W....=wB
+000014e0: 4b44 a838 b595 aa55 d5ee f16c 9c09 b188  KD.8...U...l....
+000014f0: e3ac 6d0a b4da efbe e370 b488 17b6 1221  ..m......p.....!
+00001500: 4e98 f9cd 7f2e 0677 5b51 3b2f a034 974d  N......w[Q;/.4.M
+00001510: 4e42 2f20 0e34 4c16 bc59 e6e4 e78f b97b  NB/ .4L..Y.....{
+00001520: 4b1c 6d68 53d0 5a36 9093 1d68 7237 fcfa  K.mhS.Z6...hr7..
+00001530: 65b0 916a a52b 00e3 20a1 d139 a98c 6933  e..j.+.. ..9..i3
+00001540: dfd7 ac02 41b5 275b 68f0 9752 2a41 0d3e  ....A.'[h..R*A.>
+00001550: aaa5 af5b 05b4 e89c 44ed 4741 d0f3 05e5  ...[....D.GA....
+00001560: 0dd9 1332 750d 4396 2567 3095 6c2d a031  ...2u.C.%g0.l-.1
+00001570: 7b88 829a 1ad4 af2b deea 234d b06b 7082  {......+..#M.kp.
+00001580: aad5 ba75 9914 2d22 16bc e666 d741 8923  ...u..-"...f.A.#
+00001590: 5876 bf6c a4a2 8b1a f3de 8609 65ce 56e1  Xv.l........e.V.
+000015a0: 27c2 2b3e 86e9 de5f 4412 9c29 a965 693c  '.+>..._D..).ei<
+000015b0: 24fb 7bcd 97e9 f7fd be4f d989 7499 ff55  $.{......O..t..U
+000015c0: 9830 f115 bc70 dbc0 7754 f439 4961 7a62  .0...p..wT.9Iazb
+000015d0: 45ef b0f8 93b0 de09 66cb a5b2 352f 72f2  E.......f...5/r.
+000015e0: 16c4 e964 dc9b c46e 2f0c 2337 998d a6ee  ...d...n/.#7....
+000015f0: 7836 99b9 a3b4 3f4b 6771 1405 e9f4 2f19  x6....?Kgq..../.
+00001600: 0e0a 8e1d b659 390a ca9c 8cc2 ec21 ba21  .....Y9......!.!
+00001610: fe70 d00d d02f 0e1b fde1 ecbc 4a29 9e19  .p.../......J)..
+00001620: ade1 bb9d b81a 6739 c059 b653 ba90 7265  ......g9.Y.S..re
+00001630: cdef 317a 80e0 9636 e06c 9f5b ec35 5a11  ..1z...6.l.[.5Z.
+00001640: 6777 3862 c646 b60f 509a 09d4 0818 a36a  gw8b.F..P......j
+00001650: ca0c 7f81 47f4 c8c9 421a 23c5 135f 56a6  ....G...B.#.._V.
+00001660: db09 83ef 4a25 5fa1 e954 410d 688c 72f7  ....J%_..TA.h.r.
+00001670: 3e07 468a a67f ba04 c6e9 b999 9591 138c  >.F.............
+00001680: 7820 fe97 db5e 8bd5 7ad4 7865 bcb3 24ce  x ...^..z.xe..$.
+00001690: 4262 b647 a5b1 55ea 9fea fcf1 7cac f9bc  Bb.G..U.....|...
+000016a0: dbeb 47e5 1450 d275 6d9e e4e6 1bd8 d260  ..G..P.um......`
+000016b0: 4913 2fc1 7edb 85c9 8add 1434 c34d c5d2  I./.~......4.M..
+000016c0: 7b1d 96c9 1a19 f8ed 086e ff71 70d1 e8b6  {........n.qp...
+000016d0: bb6f 7861 aa9c 44a9 97a6 49ef f6c6 96ce  .oxa..D...I.....
+000016e0: ecec f245 7864 6b8d d5ff bdb7 09ad c013  ...Exdk.........
+000016f0: 0395 770c bc1f 1861 e4c5 7114 c4a1 f55c  ..w....a..q....\
+00001700: 8036 f343 af2f 297e 27e8 1f00 0000 ffff  .6.C./)~'.......
+00001710: 0000 00ff ffcc 5c6b 731a 3714 fd2b 9bb5  ......\ks.7..+..
+00001720: 2713 531a 58b0 8d49 6c77 583d 8213 0c8d  '.S.X..IlwX=....
+00001730: 8174 a69d 0ec3 b8b8 ed4c e266 b027 8f7f  .t.......L.f.'..
+00001740: df2b ad60 7785 7675 b516 902f 9d54 dc23  .+.`w.vu.../.T.#
+00001750: dd73 251d 3dae d6e7 0fff 2c16 8f74 fe38  .s%.=.....,..t.8
+00001760: bf3c 5ffe f735 585e 8451 183c 7c9e df3f  .<_..5X^.Q.<|..?
+00001770: c0bf 5e45 ad30 f816 1dcf 6f5f fdf5 9d2e  ..^E.0....o_....
+00001780: 1e6e 17f7 8f17 61f3 653b bc3c bf15 b63d  .n....a.e;.<...=
+00001790: 617c 11b6 9a50 7017 dcce 05fa 7218 cfde  a|...Pp.....r...
+000017a0: 4fd9 7872 351a 8ecf 1b77 97e7 5f2e a3f3  O.xr5....w.._...
+000017b0: c697 cbf3 c6ad 82c5 09ec 2c0c a0ba 07c0  ..........,.....
+000017c0: 7eb9 3c3d cd9b 9095 4943 61a8 6a2a 0a57  ~.<=....ICa.j*.W
+000017d0: 256c a384 6f94 bc4d 4ae0 bfeb 96ce 4ef2  %l..o..MJ.....N.
+000017e0: 2dbd 3398 68ce 0c94 495b 56b3 900e 1f7c  -.3.h...I[V....|
+000017f0: e80d a6ec d9ba ae06 846f 1d43 081b 3e86  .........o.C..>.
+00001800: c218 62d8 d262 c87b 6452 143f 0551 017c  ..b..b.{dR.?.Q.|
+00001810: 5c66 a157 fc05 190d a6d7 c317 bde8 e8f9  \f.W............
+00001820: df8f afa1 3f06 83eb 713d 08c3 7a30 e27c  ....?...q=..z0.|
+00001830: cc26 2fd8 b7cf 8b67 87f1 6154 0ffa ac47  .&/....g..aT...G
+00001840: d9cd 6c7c f53b fb29 05fe 0cbf 006a 0625  ..l|.;.).....j.%
+00001850: 4747 aa17 6150 7c5d 2c1f fef8 f7cf 971f  GG..aP|],.......
+00001860: 3f7e 9a25 fffb f27e fe69 a1f5 1dce bdb8  ?~.%...~.i......
+00001870: aa7b 0034 b807 c362 3dc0 28ce 0352 d503  .{.4...b=.(..R..
+00001880: 005a 3c60 380f 6855 0f00 68f1 80e3 3c60  .Z<`8.hU..h...<`
+00001890: 553d 00a0 c583 b779 0fe4 b439 3bd3 669f  U=.....y...9;.f.
+000018a0: c9a6 93b7 1924 36ed 6416 23a6 1fcc 53fc  .....$6.d.#...S.
+000018b0: f413 c630 fd92 b9ad c448 7320 4e6c 56d3  ...0.....Hs NlV.
+000018c0: 3fb8 fd24 850e 240f 5465 be5c cebf 87c1  ?..$..$.Te.\....
+000018d0: 3c51 bf60 b9b8 bb08 0540 a961 ef03 bbe9  <Q.`.....@.a....
+000018e0: bd61 302b 4ba7 de7a b6d5 0398 af37 a3df  .a0+K..z.....7..
+000018f0: c647 f520 3e6c 5966 6c3d a0d3 9b9e 90da  .G. >lYfl=......
+00001900: 14b7 9aae 07f4 ea43 a399 2a94 546c e24a  .......C..*.Tl.J
+00001910: 4500 3c50 21fe a950 572a 02e0 810a f54f  E.<P!..PW*.....O
+00001920: 85b9 5211 000f 5498 7f2a dc95 8a00 78a0  ..R...T..*....x.
+00001930: c2fd 53e9 2b69 38ce ec1e a254 1a72 2b3e  ..S.+i8....T.r+>
+00001940: d8e0 2547 18eb 92a3 e962 9cd8 244d 2f20  ..%G.....b..$M/ 
+00001950: 4256 c901 d31d 490e 198d 2758 b971 a541  BV....I...'X.q.A
+00001960: fcd0 c0c8 8d03 0dea 4a43 0076 2435 0e34  ........JC.v$5.4
+00001970: 982b 0d01 d891 cc38 d0e0 ae34 0460 4712  .+.....8...4.`G.
+00001980: e340 a3af 64e0 589c 6872 6272 e222 26c2  .@..d.X.hrbr."&.
+00001990: 5813 9348 1713 65b3 3ebe 146f 5cc0 5245  X..H..e.>..o\.RE
+000019a0: 8a8c a6c3 49ba 6d51 8781 7ad0 ac07 6fc7  ....I.mQ..z...o.
+000019b0: a3e1 6cf4 0e76 2893 9b29 3b6a 184e 7c07  ..l..v(..);j.N|.
+000019c0: c3de 35fb 453b 17a0 dd20 db74 83a2 dd10  ..5.E;... .t....
+000019d0: 965b 8b06 43bb 212c b7e6 0647 bb21 2cb7  .[..C.!,...G.!,.
+000019e0: e646 5fb9 915b 6bbb e6d3 f5a9 cbf4 10c6  .F_..[k.........
+000019f0: 303d a0fa f50d 40ab a95d 4724 3689 8938  0=....@..]G$6..8
+00001a00: 5eac af32 e293 1a76 6c17 d641 d075 d0c2  ^..2...vl..A.u..
+00001a10: 3a28 ba0e 5658 0743 d7c1 0beb e0e8 3afa  :(..VX.C......:.
+00001a20: 2aee 9be2 d671 e93d 61ac 899b de79 ca04  *....q.=a....y..
+00001a30: a16d 6069 1fbf efb3 c216 1fc2 4d90 bcc1  .m`i........M...
+00001a40: 3ab8 615c 3f4a a15b 26ee 2d93 b296 29ba  :.a\?J.[&.-...).
+00001a50: 6561 e9c8 9996 b5cc d02d 0b4b c796 5959  ea.......-.K..YY
+00001a60: cb1c ddb2 b074 6c99 97b5 dc57 2d67 a5a9  .....tl....W-g..
+00001a70: 95de 68e6 566e b891 c31f 0384 b126 4dfa  ..h.Vn.......&M.
+00001a80: 4569 6262 52a6 4e2d 2e1b 9b85 40d2 a991  EibbR.N-....@...
+00001a90: 1220 2d04 d24e 8d96 0059 2190 756a ac04  . -..N...Y!.uj..
+00001aa0: c80b 81bc 53e3 25c0 be8a dfa6 c474 5d7a  ....S.%......t]z
+00001ab0: 4118 6b12 d36a 690b 84b2 4168 0c58 e6c7  A.k..ji...Ah.X..
+00001ac0: de78 75ef 93dd 4025 2223 364f 7575 2b94  .xu...@%"#6Ouu+.
+00001ad0: fd95 f4a7 c377 63a9 43c9 fe2a 3e84 0d5d  .....wc.C..*>..]
+00001ae0: a10c a19d 235b 718e 9439 47d1 ce09 4bff  ....#[q..9G...K.
+00001af0: 91a3 65ce 31b4 73c2 d2bf 73ac cc39 8e76  ..e.1.s...s..9.v
+00001b00: 4e58 fa77 8e97 39d7 57ce e524 b16d dead  NX.w..9.W..$.m..
+00001b10: 454d 97d9 28ad f5fd dab1 9e3e 1255 5e84  EM..(......>.U^.
+00001b20: 2659 ecd6 e2b2 b9a2 aa37 2049 b746 4a90  &Y.......7 I.FJ.
+00001b30: b418 49bb 355a 8264 c548 d6ad b112 242f  ..I.5Z.d.H....$/
+00001b40: 46f2 6e8d 9720 fbab 30e6 3a28 4d7c e5d6  F.n.. ..0.:(M|..
+00001b50: acc8 2de3 a772 6cd9 fbf2 9696 2f8b 6595  ..-..rl...../.e.
+00001b60: d08b 08c1 14a6 96d1 dbac 6736 65eb 0bf1  ..........g6e...
+00001b70: 9562 36eb 19bd 9407 5283 09ec e2e9 8888  .b6.....R.......
+00001b80: 3bf5 50a4 c49a e151 0392 5fb0 952c 5455  ;.P....Q.._..,TU
+00001b90: 3c05 b237 0aa4 9402 c553 90a6 7be9 055a  <..7.....S..{..Z
+00001ba0: 4a81 e129 48d3 bd50 60a5 1438 9e82 34dd  J..)H..P`..8..4.
+00001bb0: 0b05 5e4a a1bf a290 5393 828b 70f1 64c0  ..^J....S...p.d.
+00001bc0: e1fd 804a ffe5 d444 bfbd 9255 22d5 04ea  ...J...D...U"...
+00001bd0: db59 0467 bd21 9dfd 0ac9 3d27 5d51 8ced  .Y.g.!....=']Q..
+00001be0: d248 04ef 3d93 b129 0c9a 0cfd 01c8 d8b4  .H..=..)........
+00001bf0: 064d 86fd 0064 6caa 8326 c37f 0032 36fd  .M...dl..&...26.
+00001c00: 5164 72fa 5370 3918 89a4 1dfe fd92 4af1  Qdr.Sp9.......J.
+00001c10: 65f5 a7ad df30 c92a 91fa 9326 33d5 fdf9  e....0.*...&3...
+00001c20: c6f9 cfc3 6e66 d01b be11 5b99 bb25 621f  ....nf....[..%b.
+00001c30: a318 62f4 66f7 cedb f405 ed3c 159d b47d  ..b.f......<...}
+00001c40: b1cc 45de a627 68e7 d91e 9cb7 e907 da79  ..E..'h........y
+00001c50: be07 e76d 7a61 48dc b70b 6eec 2291 85c3  ...mzaH...n."...
+00001c60: eb85 cad9 e5f4 42bf 2d92 5522 f522 cd4c  ......B.-.U".".L
+00001c70: ee40 2f16 f708 bd50 0c31 7ab1 7be7 6d7a  .@/....P.1z.{.mz
+00001c80: 8176 9e8a 4eda 9d5e c8c8 dbf4 02ed 3cdb  .v..N..^......<.
+00001c90: 83f3 36bd 403b cff7 e0bc 4d2f d699 f834  ..6.@;....M/...4
+00001ca0: 49d8 2eba ce12 894a bc5e a8b4 667b fd6a  I......J.^..f{.j
+00001cb0: 398e 92a2 9375 0951 25f2 1e5b 3ed2 a31b  9....u.Q%..[>...
+00001cc0: 256c a384 6f94 f455 496b f342 3c72 4a99  %l..o..UIk.B<rJ.
+00001cd0: 4a6b fd7d 52ba dd92 2ec6 ca28 4b23 49f9  Jk.}R......(K#I.
+00001ce0: 6569 e825 4ca1 521b 9e2d c95f 4b65 1385  ei.%L.R..-._Ke..
+00001cf0: 5051 f93b 7443 a2f0 547b e81d 4789 513b  PQ.;tC..T{..G.Q;
+00001d00: f75a 7d3c bdde dadb cc7e 6f30 98c2 c3eb  .Z}<.....~o0....
+00001d10: d58b ced5 cb4c 6d83 49bc 3a86 79fa 8474  .....Lm.I.:.y..t
+00001d20: 8c7a 750c f36e 12e9 18f3 ea18 e615 24d2  .zu..n........$.
+00001d30: 31ee d531 cc9b 46bb 63f9 5995 cd50 5a67  1..1..F.c.Y..PZg
+00001d40: 95ca b065 d54b 1575 73cf 24a2 8ee9 0dd0  ...e.K.us.$.....
+00001d50: c630 3761 61f0 23b0 3432 6161 7c22 b0cc  .07aa.#.42aa|"..
+00001d60: 8885 2184 c072 2316 7ab9 1c9b 0f79 361d  ..!..r#.z....y6.
+00001d70: 690d b921 1d79 b6b1 c14c 8cf2 42a6 ef1f  i..!.y...L..B...
+00001d80: cd9f 7854 7e67 ae8f 3378 0856 2867 9edd  ..xT~g..3x.V(g..
+00001d90: aba2 68c5 eed1 c8b3 7b55 74ad d83d e6db  ..h.....{Ut..=..
+00001da0: bd2a ea56 ec1e f7ed 5e15 8d33 ba97 ff00  .*.V....^..3....
+00001db0: 2b9b 74b4 cd39 f87c 4d3d 0158 7d5a 16af  +.t..9.|M=.X}Z..
+00001dc0: 8a34 99eb 6264 ce88 2511 064b 8d58 18b1  .4..bd..%..K.X..
+00001dd0: 1899 3362 6138 6164 ce88 85be 7690 b956  ..3ba8ad....v..V
+00001de0: 368d 680d b921 8bd8 d1ef dd64 8de9 391a  6.h..!.....d..9.
+00001df0: f106 5e20 d4a1 6edb dfdd 30f8 fe6f d69b  ..^ ..n...0..o..
+00001e00: 4e46 d897 f0ce 6c88 2736 18f9 7465 439d  NF....l.'6..teC.
+00001e10: d948 8487 bec1 a8ad 2b1b e6cc 4622 3cb0  .H......+...F"<.
+00001e20: c188 b32b 1bee cc46 223c b0c1 68b9 039b  ...+...F"<..h...
+00001e30: bca2 67f3 8a56 7959 a715 c5b7 c51b ba92  ..g..VyY........
+00001e40: fc2a 9e33 5bbf aa81 cf72 8bae 893c 6fb0  .*.3[....r...<o.
+00001e50: 0c81 29d9 6309 bf92 2730 560e c40f 878a  ..).c...'0V.....
+00001e60: 3252 b211 73e0 40fd 70a8 281e 25bb 3507  2R..s.@.p.(.%.5.
+00001e70: 0ecc 0f87 8a92 51b2 a573 e0c0 fd70 a828  ......Q..s...p.(
+00001e80: 1488 7d5f 36fb 6755 8975 f22f ddf7 a9a2  ..}_6.gU.u./....
+00001e90: fcbe afd5 42ed fb4c 5898 7c98 e3ad f8fc  ....B..LX.|.....
+00001ea0: 58bc 42cd b50b 831e b5ef 3361 61b0 a1f6  X.B.......3aa...
+00001eb0: 7d26 2c74 b2cb be2f 9b40 b186 dc94 3fd1  }&,t.../.@....?.
+00001ec0: 9ff7 c105 2656 db62 615b 708d bf0b 7d56  ....&V.ba[p...}V
+00001ed0: afc9 ea41 f91f 56a8 0746 750f 9f7f 7c7c  ...A..V..Fu...||
+00001ee0: 1d85 45e7 6887 3810 3f71 a8ac f1db 8c03  ..E.h.8.?q......
+00001ef0: 7588 83b4 7dfa 78a8 bc4e 6c33 0ecc 210e  u...}.x..Nl3..!.
+00001f00: d2f6 e971 a8bc d66c 330e dc21 0ed2 f6e9  ...q...l3..!....
+00001f10: 71a8 bc5e 6d29 0ef9 9d71 3623 6515 e0cd  q..^m)...q6#e...
+00001f20: 8494 f836 6e63 ed01 6145 ad79 262c 8811  ...6nc..aE.y&,..
+00001f30: 6acd 3361 6102 a3d6 3c13 1606 3d6a cd33  j.3aa...<...=j.3
+00001f40: 6161 a0b8 ac79 d97c 9a35 e4ea 5338 f157  aa...y.|.5..S8.W
+00001f50: 9336 ff14 522b f915 7718 01db 3d2e 7651  .6..R+..w...=.vQ
+00001f60: e142 85e7 4004 dfa7 73a8 bc50 1571 a00e  .B..@...s..P.q..
+00001f70: fd20 6df7 b8c8 1471 600e 1ca4 ed1e 1788  . m....q`.......
+00001f80: 220e dc81 83b4 dda3 b81b 38e4 85d9 2583  ".........8...%.
+00001f90: dd5a 67b0 d3c3 882a d20e 23a7 2861 3661  .Zg....*..#.(a6a
+00001fa0: 61f2 a184 d984 8541 8f12 6613 1606 1b4a  a......A..f....J
+00001fb0: 984d 58e8 648c 3037 d23f 64f7 3f00 0000  .MX.d.07.?d.?...
+00001fc0: ffff 0000 00ff ff44 8c41 0e82 3010 45af  .......D.A..0.E.
+00001fd0: d2cc 0144 1125 3594 951b 17ae 3841 0d43  ...D.%5.....8A.C
+00001fe0: 3b51 3bcd 3086 84d3 0b26 c4dd 7fef 27af  ;Q;.0....&....'.
+00001ff0: c93e e0dd 4ba0 349a 170e ea60 bfab c108  .>..K.4....`....
+00002000: 85b8 6de5 fcb3 2730 0f56 e5f7 4611 7d8f  ..m...'0.V..F.}.
+00002010: b2d2 11cc c0ac 1b14 6db3 763b d44f 36d9  ........m.v;.O6.
+00002020: 6794 8e66 7460 c1b0 1026 f54a 9c1c 6416  g..ft`...&.J..d.
+00002030: 154f 0a26 2e7e e6e5 785d 3339 a84a 5bd9  .O.&.~..x]39.J[.
+00002040: 735d da25 2c17 ea1d c8ad 3fc0 d2ed c54f  s].%,.....?....O
+00002050: 94c2 df96 ab2d 2696 e718 11b5 fd02 0000  .....-&.........
+00002060: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+00002070: 2100 877b 5fd3 f504 0000 ca10 0000 1800  !..{_...........
+00002080: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00002090: 7368 6565 7433 2e78 6d6c 9c93 4d6b e330  sheet3.xml..Mk.0
+000020a0: 1086 ef0b fb1f 84ee b6fc ddc4 c429 29ae  .............)).
+000020b0: d9c2 1e96 65bb 7b56 e471 2c62 4946 929b  ....e.{V.q,bIF..
+000020c0: 84d2 ffbe 9243 d342 2ea1 60d9 9235 7ae6  .....C.B..`..5z.
+000020d0: 1dcf ebd5 fd51 0ce8 05b4 e14a 5638 0e23  .....Q.....JV8.#
+000020e0: 8c40 32d5 72b9 abf0 f39f 2658 6064 2c95  .@2.r.....&X`d,.
+000020f0: 2d1d 9484 0a9f c0e0 fbf5 f76f ab83 d27b  -..........o...{
+00002100: d303 58e4 08d2 54b8 b776 2c09 31ac 0741  ..X...T..v,.1..A
+00002110: 4da8 4690 6ea7 535a 50eb 967a 47cc a881  M.F.n.SZP..zG...
+00002120: b6f3 2131 9024 8a0a 2228 97f8 4c28 f52d  ..!1.$.."(..L(.-
+00002130: 0cd5 759c 41ad d824 40da 3344 c340 add3  ..u.A..$@.3D.@..
+00002140: 6f7a 3e9a 779a 60b7 e004 d5fb 690c 9812  oz>.w.`.....i...
+00002150: a343 6cf9 c0ed 6986 6224 58f9 b493 4ad3  .Cl...i.b$X...J.
+00002160: ede0 ea3e c619 65e8 a8dd 95b8 91be a799  ...>..e.........
+00002170: df5f 6512 9c69 6554 6743 4726 67cd d7e5  ._e..ieTgCG&g...
+00002180: 2fc9 9250 7621 5dd7 7f13 26ce 8886 17ee  /..Pv!]...&.....
+00002190: 1bf8 814a be26 29ce 2fac e403 967e 1156  ...J.&)./....~.V
+000021a0: 5c60 fe73 e972 e26d 855f f36c f1b8 68d2  \`.s.r.m._.l..h.
+000021b0: 2648 92a2 08b2 4d9e 050f 774d 14a4 0f75  &H....M...wM...u
+000021c0: 1617 8f9b bac9 eb37 bc5e b5dc 75d8 5785  .......7.^..u.W.
+000021d0: 3474 15de c4e5 cf24 c664 bd9a 0df4 97c3  4t.....$.d......
+000021e0: c17c 9a23 efc7 ad52 7bbf f1e4 f244 3e94  .|.#...R{....D>.
+000021f0: 5cc5 36b3 1f7f 69d4 4247 a7c1 fe56 871f  \.6...i.BG...V..
+00002200: c077 bd75 e6cf c2cc e9f4 8d2e db53 0d86  .w.u.........S..
+00002210: 3987 3950 987a 1453 83cb e7ee 4870 ffa7  9.9P.z.S....Hp..
+00002220: 3883 d0e3 fc3c f0d6 f615 4ea2 308e 96e9  8....<....N.0...
+00002230: 5d8e d116 8c6d b847 62c4 2663 95f8 778e  ]....m.Gb.&c..w.
+00002240: 99f5 9319 f51f 0000 ffff 0000 00ff ff9c  ................
+00002250: 576b 6fa2 4014 fd2b b36c d3c0 2e59 1cc5  Wko.@..+.l...Y..
+00002260: 475b 2501 b4d1 1521 5b31 dbec 9786 456c  G[%....![1....El
+00002270: 936d 6b83 d4d6 7fbf 97c1 320f 6d61 ea27  .mk.......2.ma.'
+00002280: 99b9 dc33 e7de 33e7 6a7f 7397 24d9 30ca  ...3..3.j.s.$.0.
+00002290: 22ab 9fae 5f50 3a50 b082 364f d1e3 06be  "..._P:P..6O....
+000022a0: 9de3 a682 5eb1 19c5 e7cb dd30 d9c4 c963  ....^......0...c
+000022b0: 3650 1a3f 5a8a d58f f358 1b82 6165 03cf  6P.?Z....X..ae..
+000022c0: 5bab d5ee 1b5b ab6f c4fb 4d07 93e5 26bf  [....[.o..M...&.
+000022d0: 3ae4 5ee9 f09b 931c 7ca0 343b 45da 2c85  :.^.....|.4;E.,.
+000022e0: 0c2b 4b71 d70f 4fcf 59b2 4471 727f bf41  .+Kq..O.Y.Dqr..A
+000022f0: 77d1 3641 11da c103 1cf9 6f14 ffbb 4dd7  w.6A......o...M.
+00002300: cf8f 4ba5 6fac f283 d40c e7a1 7f96 d0c6  ..K.o...........
+00002310: fefc d383 158f 5d31 a05e 65d1 a04e f58b  ......]1.^e..N..
+00002320: 06c1 b468 5da1 684d 52b4 8650 34ee 955e  ...h].hMR..P4..^
+00002330: b9c9 9da1 2573 0608 2ecf d0c5 c219 f2fe  ....%s..........
+00002340: 6e2d baca c198 3230 104c 6104 2538 a6a0  n-....20.La.%8..
+00002350: 0f0e a62d 0303 c114 a625 b069 1318 5a34  ...-.....%.i..Z4
+00002360: a2dc 21fb 4aeb ec78 4541 86f5 bbba d72c  ..!.J..xEA.....,
+00002370: 0133 85fe 399d 8fa8 7665 6020 b8a4 6a8a  .3..9...ve` ..j.
+00002380: 8deb 1617 f138 9b9e 0c0c 0453 18b1 71bd  .....8.....S..q.
+00002390: 82e4 7198 3319 1808 a630 62e3 ce08 0cb5  ..q.3....0b.....
+000023a0: 084e 1fb8 21e5 5310 4d81 4cd1 a81a 8244  .N..!.S.M.L....D
+000023b0: 7824 3947 64fd cd3c b0c4 c213 dfd1 5b6e  x$9Gd..<......[n
+000023c0: b712 decb 9a82 2938 a903 b9c8 25a6 4ae4  ......)8....%.J.
+000023d0: 4949 b905 66ed c214 2d0b 7609 1495 090f  II..f...-.v.....
+000023e0: 25e5 1898 b50c 53b8 b50e ec12 282a 151e  %.....S.....(*..
+000023f0: 4aca 3530 eb01 3df1 2ec1 2e81 a22d e4a1  J.50..=......-..
+00002400: d85b 5b39 26b9 5b4b bb4f acc8 c179 aa62  .[[9&.[K.O...y.b
+00002410: eac5 0ff9 0086 a197 ab35 4ad3 68a7 a028  .........5J.h..(
+00002420: 8ec8 544e 93d5 4021 c1c5 82e5 060b 3fb4  ..TN..@!......?.
+00002430: d5e0 f272 3e0a d5d1 eb53 f2e5 c439 c13a  ...r>....S...9.:
+00002440: 1a8f ece1 e8ea 663e f933 d291 e7cd 6edc  ......f>.3....n.
+00002450: c0d3 91e3 05ee 74bf 8835 6d3f 2cdf 7179  ......t..5m?,.qy
+00002460: ccba 4525 3dd6 2dda a2f7 9154 b5e9 41aa  ..E%=.-....T..A.
+00002470: 0a7a 2cbb 5f8b d13c 9c04 7ec1 1037 c847  .z,._..<..~..7.G
+00002480: 47d5 f458 97aa a4c7 ba54 fb40 2779 aada  G..X.....T.@'y..
+00002490: f420 5882 dea5 ed86 b2d4 9aac 3156 51cb  . X.........1VQ.
+000024a0: 83e9 e414 7d91 a42a 7f8e 2570 f44a 79e6  ....}..*..%p.Jy.
+000024b0: afec 09ce ecd0 1dab e1d5 0244 e807 a13a  ...........D...:
+000024c0: 993b 9eed 4f0f f5ca 34f4 3bd6 df6f a9a6  .;..O...4.;..o..
+000024d0: a3c6 9b6c bffa 867d 7cfe 3459 bbae e4cf  ...l...}|.4Y....
+000024e0: ba75 5774 6b92 aa6e 6bf3 e092 f9b5 3ab3  .uWtk..nk.....:.
+000024f0: afd5 0fa9 eaee 78e1 4f49 770b ddea 583b  ......x.OIw...X;
+00002500: bdcf 2e4e 6fb3 0b45 d1d0 37a4 5e05 bfa5  ...No..E..7.^...
+00002510: 5368 1a94 a91a bc54 d6a7 b10f 33d4 847e  Sh.....T....3..~
+00002520: 33a4 4f23 1f24 00e0 375d 8883 c1a0 7f70  3.O#.$..7].....p
+00002530: fe03 0000 ffff 0000 00ff ffb2 2948 4c4f  ............)HLO
+00002540: f54d 2c4a cfcc 2b56 c849 4d2b b155 32d0  .M,J..+V.IM+.U2.
+00002550: 3357 5228 ca4c cf80 b14b f20b c0a2 a64a  3WR(.L...K.....J
+00002560: 0a49 f925 25f9 b930 5e46 6a62 4a6a 1188  .I.%%..0^FjbJj..
+00002570: 67ac a490 969f 5f02 e3e8 dbd9 e897 e717  g....._.........
+00002580: 6517 67a4 a696 d801 0000 00ff ff03 0050  e.g............P
+00002590: 4b03 0414 0006 0008 0000 0021 00b1 450d  K..........!..E.
+000025a0: ec5c 0700 0002 2100 0013 0000 0078 6c2f  .\....!......xl/
+000025b0: 7468 656d 652f 7468 656d 6531 2e78 6d6c  theme/theme1.xml
+000025c0: ec59 4b8f 1b37 12be 07c8 7f20 fa2e ebd5  .YK..7..... ....
+000025d0: adc7 c0b2 a1a7 27f6 8c6d 7864 2f72 e448  ......'..mxd/r.H
+000025e0: 949a 1e76 5320 a919 0b81 81c0 39e5 1220  ...vS ......9.. 
+000025f0: 4076 b197 05f6 b687 2048 8004 5823 97fc  @v...... H..X#..
+00002600: 1803 36b2 d91f b145 764b 4d8e a878 6c8f  ..6....EvKM..xl.
+00002610: 174e 3033 c08c 9afa aa58 ac2a 7eac 2e5e  .N03.....X.*~..^
+00002620: bff9 2461 e894 0849 79da 09aa d72a 0122  ..$a...Iy....*."
+00002630: e984 4f69 3aef 040f c7a3 522b 4052 e174  ..Oi:.....R+@R.t
+00002640: 8a19 4f49 2758 1119 dcbc f1f1 47d7 f19e  ..OI'X......G...
+00002650: 8a49 4210 c8a7 720f 7782 58a9 c55e b92c  .IB...r.w.X..^.,
+00002660: 2730 8ce5 35be 2029 7c37 e322 c10a 1ec5  '0..5. )|7."....
+00002670: bc3c 15f8 0cf4 26ac 5cab 541a e504 d334  .<....&.\.T....4
+00002680: 4029 4e40 edbd d98c 4e08 aa55 aa75 5482  @)N@....N..U.uT.
+00002690: 7fb5 1a1a 6bf5 c18d f544 4306 8fa9 927a  ....k....DC....z
+000026a0: 60c2 c491 9e86 ec94 3672 d393 aa46 cb95  `.......6r...F..
+000026b0: ec33 814e 31eb 0430 ff94 9f8d c913 1520  .3.N1..0....... 
+000026c0: 86a5 822f 3a41 c5fc 04e5 1bd7 cb78 2f17  .../:A.......x/.
+000026d0: 626a 87ac 2537 323f b95c 2e30 3da9 9939  bj..%72?.\.0=..9
+000026e0: c5fc 7833 6918 4661 a3bb d16f 004c 6de3  ..x3i.Fa...o.Lm.
+000026f0: 86cd 6163 d8d8 e833 003c 99c0 aa33 5b5c  ..ac...3.<...3[\
+00002700: 9dcd 5a3f ccb1 1628 fbe8 d13d 680e ea55  ..Z?...(...=h..U
+00002710: 076f e9af 6fd9 dc8d f4af 8337 a04c 7fb8  .o..o......7.L..
+00002720: 851f 8dfa e045 076f 4019 3eda c247 bd76  .....E.o@.>..G.v
+00002730: 6fe0 ea37 a00c dfd8 c237 2bdd 41d8 74f4  o..7.....7+.A.t.
+00002740: 1b50 cc68 7ab2 85ae 448d 7a7f bdda 0d64  .P.hz...D.z....d
+00002750: c6d9 be17 de8e c251 b396 2b2f 5090 0d9b  .......Q..+/P...
+00002760: 4cd3 53cc 78aa 2e92 7709 7ecc c508 c05a  L.S.x...w.~....Z
+00002770: 8861 4553 a456 0b32 c313 c8f4 3e66 f458  .aES.V.2....>f.X
+00002780: 5074 40e7 3124 e102 a75c c270 a556 1955  Pt@.1$...\.p.V.U
+00002790: eaf0 57ff 86e6 9389 2ede 23d8 92d6 3682  ..W.......#...6.
+000027a0: 5572 6b48 db86 e444 d085 ea04 b741 6b60  UrkH...D.....Ak`
+000027b0: 415e 3e7f fee2 d94f 2f9e fdfb c517 5fbc  A^>....O/....._.
+000027c0: 78f6 7d3e b751 e5c8 ede3 746e cbfd f6af  x.}>.Q....tn....
+000027d0: afff fb8f cfd1 7f7e fce7 6fdf fc35 9bfa  .......~..o..5..
+000027e0: 3c5e daf8 57df 7df9 eae7 5f7e 4f3d acb8  <^..W.}..._~O=..
+000027f0: 70c5 cbbf fdf0 eaa7 1f5e fefd ab5f bffd  p........^..._..
+00002800: c6a3 bd2b f0b1 0d1f d384 4874 979c a107  ...+......Ht....
+00002810: 3c81 057a ec27 c7e2 cd24 c631 a68e 048e  <..z.'...$.1....
+00002820: 41b7 47f5 50c5 0ef0 ee0a 331f ae47 5c17  A.G.P.....3..G\.
+00002830: 3e12 c038 3ee0 ade5 63c7 d6a3 582c 15f5  >..8>...c...X,..
+00002840: cc7c 274e 1ce0 21e7 acc7 85d7 0177 f45c  .|'N..!......w.\
+00002850: 9687 c7cb 74ee 9f5c 2c6d dc03 8c4f 7d73  ....t..\,m...O}s
+00002860: f771 ea04 78b8 5c00 ed52 9fca 7e4c 1c33  .q..x.\..R..~L.3
+00002870: ef33 9c2a 3c27 2951 487f c74f 08f1 acee  .3.*<')QH..O....
+00002880: 534a 1dbf 1ed2 89e0 92cf 14fa 94a2 1ea6  SJ..............
+00002890: 5e97 8ce9 b193 4885 d03e 4d20 2e2b 9f81  ^.....H..>M .+..
+000028a0: 106a c737 878f 508f 33df aa07 e4d4 45c2  .j.7..P.3.....E.
+000028b0: b6c0 cc63 fc98 30c7 8db7 f052 e1c4 a772  ...c..0....R...r
+000028c0: 8c13 663b fc00 abd8 67e4 d14a 4c6c dc50  ..f;....g..JLl.P
+000028d0: 2a88 f49c 308e 8653 22a5 4fe6 9e80 f55a  *...0..S".O....Z
+000028e0: 41bf 030c e30f fb21 5b25 2e52 287a e2d3  A......![%.R(z..
+000028f0: 7980 39b7 9103 7ed2 8f71 b2f0 da4c d3d8  y.9...~..q...L..
+00002900: c67e 224f 2045 31ba cf95 0f7e c8dd 1da2  .~"O E1....~....
+00002910: 9f21 0e38 dd19 ee47 9438 e17e 3d11 3c04  .!.8...G.8.~=.<.
+00002920: 72b5 4d2a 1244 7fb3 149e 58de 22dc dd8f  r.M*.D....X."...
+00002930: 2b36 c3c4 c732 5d91 38ec da15 d49b 1dbd  +6...2].8.......
+00002940: e5dc 49ed 0342 183e c353 42d0 c34f 3c16  ..I..B.>.SB..O<.
+00002950: f4f8 c2f1 7961 f4ed 1858 659f f812 eb36  ....ya...Xe....6
+00002960: 7673 553f a744 1264 6a9c 6d8a 3ca0 d249  vsU?.D.dj.m.<..I
+00002970: d923 32e7 3bec 395c 9d23 9e15 4e13 2c76  .#2.;.9\.#..N.,v
+00002980: 69be 0b51 7752 174e 392f 95de 6393 131b  i..QwR.N9/..c...
+00002990: 7897 4289 08f9 e275 ca3d 093a ace4 1eee  x.B....u.=.:....
+000029a0: d27a 3fc6 ced9 a59f a53f 5f57 c289 df45  .z?......?_W...E
+000029b0: f618 eccb c76f ba2f 4186 bcb1 0c10 fb85  .....o./A.......
+000029c0: 7d33 c6cc 99a0 4898 3186 02c3 47b7 20e2  }3....H.1...G. .
+000029d0: 84bf 10d1 e7aa 115b 7ae5 66ee a62d c200  .......[z.f..-..
+000029e0: 4592 53ef 2434 7d6d f173 aeec 89fe 3f65  E.S.$4}m.s....?e
+000029f0: 8fbf 80b9 8482 c7af f85d 4a9d 5d94 b27f  .........]J.]...
+00002a00: aec0 d985 fb03 9635 03bc 4cef 1338 49b6  .......5..L..8I.
+00002a10: 39eb aaaa b9aa 6a82 3f7d 55b3 6b2f 5fd5  9.....j.?}U.k/_.
+00002a20: 3257 b5cc 552d e37b fb7a 2fb5 4c51 be40  2W..U-.{.z/.LQ.@
+00002a30: 6553 747c 4cff 27b9 50fb 6746 193b 522b  eSt|L.'.P.gF.;R+
+00002a40: 460e a4e9 0049 78bb 998e 60d0 b4a9 4cdf  F....Ix...`...L.
+00002a50: 72d3 1a5c c4f0 316f 3c39 b8b9 c046 0609  r..\..1o<9...F..
+00002a60: aefe 4255 7c14 e305 b489 aaa6 b139 97b9  ..BU|........9..
+00002a70: eab9 440b 2ea1 7b64 864d eb95 9cd3 6d7a  ..D...{d.M....mz
+00002a80: 50cb e490 4fb3 0e68 b5aa bb9d 993b 2556  P...O..h.....;%V
+00002a90: c578 25da 8c43 c74a 65e8 46b3 e8ea 6dd4  .x%..C.Je.F...m.
+00002aa0: 9b3e e9dc 7462 d706 68d9 3731 c29a cc35  .>..tb..h.71...5
+00002ab0: a2ee 31a2 b91e 8488 fc9e 1166 6597 6245  ..1........fe.bE
+00002ac0: db63 454b ab5f 876a 1dc5 8d2b c0b4 4d54  .cEK._.j...+..MT
+00002ad0: e0f5 1bc1 4b7b 2788 c2ac b30c 8d39 28d5  ....K{'......9(.
+00002ae0: a73a 4e59 9379 1d5d 1d9c 4b8d f42e 6732  .:NY.y.]..K...g2
+00002af0: 3b03 a0dc 5e67 4011 e9b6 b675 e7f2 f4ea  ;...^g@....u....
+00002b00: b254 bb40 a41d 23ac 7473 8db0 d230 8697  .T.@..#.ts...0..
+00002b10: e23c 3bed 56fc 65c6 ba5d 84d4 314f bb62  .<;.V.e..]..1O.b
+00002b20: bd1b 0a33 9aad f711 6b4d 28e7 b881 a536  ...3....kM(....6
+00002b30: 53b0 149d 7582 463d 825b 9809 5e74 8219  S...u.F=.[..^t..
+00002b40: 748f e163 b280 dc91 fa0d 0cb3 395c d34c  t..c........9\.L
+00002b50: 94c8 36fc db30 cb42 4835 c032 ce1c 6e48  ..6..0.BH5.2..nH
+00002b60: 2763 8384 2a22 10a3 4927 d0cb df64 034b  'c..*"..I'...d.K
+00002b70: 0d87 18db aa35 2084 0fd6 b836 d0ca 8766  .....5 ....6...f
+00002b80: 1c04 dd0d 3299 cdc8 44d9 61b7 46b4 a7b3  ....2...D.a.F...
+00002b90: 4760 f88c 2bbc df1a f1b7 076b 49be 8470  G`..+......kI..p
+00002ba0: 1fc5 d333 74cc 96e2 0186 148b 9a55 edc0  ...3t........U..
+00002bb0: 2995 7089 50cd bc39 a570 43b6 21b2 22ff  ).p.P..9.pC.!.".
+00002bc0: ce1d 4c39 edda 5754 2687 b271 cc16 31ce  ..L9..WT&..q..1.
+00002bd0: 4f14 9bcc 33b8 21d1 8d39 e669 e303 eb29  O...3.!..9.i...)
+00002be0: 5f33 3874 db85 c773 7dc0 bef3 a9fb faa3  _38t...s}.......
+00002bf0: 5a7b ce22 cde2 cc74 5845 9f9a 7e32 7d7f  Z{."...tXE..~2}.
+00002c00: 87bc 6555 7188 3a56 65d4 6dde af65 c175  ..eUq.:Ve.m..e.u
+00002c10: ed35 d741 a27a 4f89 d79c ba17 3810 2cd3  .5.A.zO.....8.,.
+00002c20: 8ac9 1cd3 b4c5 db34 ac39 3b1f 754d bbc4  .......4.9;.uM..
+00002c30: 82c0 f244 6387 df36 6784 d713 6f7b f283  ...Dc..6g...o{..
+00002c40: dcf9 acd5 07c4 bac6 3489 6fae d8ed 9b6f  ........4.o....o
+00002c50: 7efc 18c8 6300 7789 4ba6 a409 25dc 650b  ~...c.w.K...%.e.
+00002c60: 0c45 5f76 3399 d106 6c91 272a af11 e113  .E_v3...l.'*....
+00002c70: 5a0a da09 3eab 44dd b05f 8bfa a54a 2b1a  Z...>.D.._...J+.
+00002c80: 96c2 7a58 29b5 a26e bdd4 8da2 7a75 1855  ..zX)..n....zu.U
+00002c90: 2b83 5eed 291c 2c2a 4eaa 5176 bd3f 82eb  +.^.).,*N.Qv.?..
+00002ca0: 0cb6 ca2f f9cd f8d6 457f b2be b1b9 36e1  .../....E.....6.
+00002cb0: 4999 9b8b fcb2 31dc 5cf4 576b 17bb e847  I.....1.\.Wk...G
+00002cc0: 1408 e8b3 466d d4ae b77b 8d52 bbde 1d95  ....Fm...{.R....
+00002cd0: c241 af55 6af7 1bbd d2a0 d16f 0e46 837e  .A.Uj......o.F.~
+00002ce0: d46a 8f9e 06e8 d480 c36e bd1f 3686 ad52  .j.......n..6..R
+00002cf0: a3da ef97 c246 452f a5d5 2e35 c35a ad1b  .....FE/...5.Z..
+00002d00: 36bb ad61 d87d 9a97 34e0 858c 4a72 bf80  6..a.}..4...Jr..
+00002d10: ab8d 8d37 fe07 0000 ffff 0300 504b 0304  ...7........PK..
+00002d20: 1400 0600 0800 0000 2100 78b9 1e89 d405  ........!.x.....
+00002d30: 0000 6e1a 0000 0d00 0000 786c 2f73 7479  ..n.......xl/sty
+00002d40: 6c65 732e 786d 6ccc 19db 6edb 36f4 7dc0  les.xml...n.6.}.
+00002d50: fe41 508a 3d0c 5324 3996 62bb 96b3 c4b1  .AP.=.S$9.b.....
+00002d60: 8002 6d11 2019 3060 1902 59a2 6ca2 92e8  ..m. .0`..Y.l...
+00002d70: 5254 6a77 d8cb be67 5fb5 2fd9 2129 d994  RTjw...g_./.!)..
+00002d80: 2fb1 9c78 59fd 6089 14cf 85e7 1c9e 1bfb  /..xY.`.........
+00002d90: 17f3 34d1 1e11 cd31 c93c dd3e b574 0d65  ..4....1.<.>.t.e
+00002da0: 2189 7036 f1f4 5fee 7ca3 a36b 390b b228  !.p6.._.|..k9..(
+00002db0: 4848 863c 7d81 72fd 62f0 fd77 fd9c 2d12  HH.<}.r.b..w..-.
+00002dc0: 743b 4588 6980 22cb 3d7d cad8 ac67 9a79  t;E.i.".=}...g.y
+00002dd0: 3845 6990 9f92 19ca e04b 4c68 1a30 18d2  8Ei......KLh.0..
+00002de0: 8999 cf28 0aa2 9c03 a589 d9b2 2cd7 4c03  ...(........,.L.
+00002df0: 9ce9 1243 2f0d 9b20 4903 faa9 9819 2149  ...C/.. I.....!I
+00002e00: 6701 c363 9c60 b610 b874 2d0d 7bef 2619  g..c.`...t-.{.&.
+00002e10: a1c1 3801 56e7 763b 08b5 b9ed d296 36a7  ..8.V.v;......6.
+00002e20: 1511 31bb 4127 c521 2539 89d9 29e0 3549  ..1.A'.!%9..).5I
+00002e30: 1ce3 106d b2db 35bb 6610 ae30 01e6 e761  ...m..5.f..0...a
+00002e40: b21d d36a d5f6 3ea7 cfc4 d436 297a c45c  ...j..>....6)z.\
+00002e50: 7dfa a09f 15a9 9fb2 5c0b 4991 314f ef2e  }.......\.I.1O..
+00002e60: a734 f9e5 5de4 e9ed b6ae 49a5 0c49 0462  .4..].....I..I.b
+00002e70: 7a30 7ed4 4e7e 3a39 b14e 2deb 5efb e173  z0~.N~:9.N-.^..s
+00002e80: 41d8 db7f fefa 5bbe 3c18 6fef f77c e7f0  A.....[.<.o..|..
+00002e90: 72b1 211f 1717 dbd0 3c18 3f3f 18ba 59f1  r.!.....<.??..Y.
+00002ea0: a830 64bb 6b1c 4934 1fc7 dae7 02e5 0c76  .0d.k.I4.......v
+00002eb0: 96f7 4a0a d60e 044e 7d4b b015 8943 cbe5  ..J....N}K...C..
+00002ec0: 7307 98bb 0166 5580 6f9e 043c af03 debf  s....fU.o..<....
+00002ed0: a904 b88b 4138 45aa ccb9 ac25 81a7 19ec  ....A8E....%....
+00002ee0: d6c1 a2c8 4c53 7301 bf7b 6d3a eda5 692f  ....LSs..{m:..i/
+00002ef0: cfb7 6fed 1cce b14a 7029 d238 08d9 3e71  ..o....Jp).8..>q
+00002f00: 9edb 75e0 dfde 187e dbb2 7e2f 29de 6b97  ..u....~..~/).k.
+00002f10: 1fcc 9b0f 9cb0 591a dca0 1f93 6c65 77a0  ......Y.....lew.
+00002f20: 0e71 cc7a 9f32 f225 f3f9 27f0 2d60 8c7c  .q.z.2.%..'.-`.|
+00002f30: d5a0 9f7f d51e 8304 666c 8e23 2409 a11a  ........fl.#$...
+00002f40: 03a7 01c6 2866 b220 4572 c530 48f0 9862  ....(f. Er.0H..b
+00002f50: be2c 0e52 9c2c e474 8b4f 083f 53ae 4b31  .,.R.,.t.O.?S.K1
+00002f60: 9c7a c190 a420 ffc7 7cd5 2bd1 7acd 3de1  .z... ..|.+.z.=.
+00002f70: 57dc d7eb d032 85f9 8092 7192 2cbd d719  W....2....q.,...
+00002f80: 3718 9818 f4c1 d133 4433 1f06 5af9 7eb7  7......3D3..Z.~.
+00002f90: 9881 b964 1093 a4da c5ba 3dab 2734 58d8  ...d......=.'4X.
+00002fa0: 2da7 3940 4e12 1c71 2e26 4361 a474 32f6  -.9@N..q.&Ca.t2.
+00002fb0: 745f fc2c 71d2 c7e5 079c 4568 8ec0 b982  t_.,q.....Eh....
+00002fc0: 2be3 c742 6118 4692 2df1 c807 fd31 a111  +..Ba.F.-....1..
+00002fd0: c4db ca47 b700 bf9c 1af4 1314 3300 a778  ...G........3..x
+00002fe0: 32e5 4f46 66f0 3f26 8c41 4c1a f423 1c4c  2.OFf.?&.AL..#.L
+00002ff0: 4816 249c 4005 a142 429c 8690 ece9 6c0a  H.$.@..BB.....l.
+00003000: 21b5 3a57 eb9c 7112 0751 2849 01e3 214a  !.:W..q..Q(I..!J
+00003010: 925b 4ee2 d7b8 a6a3 79ac 3873 e177 32c6  .[N.....y.8s.w2.
+00003020: 030d 7f05 b594 af92 5339 801d d480 849b  ........S9......
+00003030: 9340 adc6 4032 8eed 83d2 82d9 2c59 7017  .@..@2......,Yp.
+00003040: 2418 9223 e06a 35ba 12fa 588d 2f13 3cc9  $..#.j5...X./.<.
+00003050: 52a4 02dc 50c2 50c8 2311 5fc6 e5af ca42  R...P.P.#._....B
+00003060: 4a46 150a d7e9 e152 d1e6 f176 f128 32e5  JF.....R...v.(2.
+00003070: 9e79 bb4c 97d0 ea8e 853b 3d5c d425 ae4d  .y.L.....;=\.%.M
+00003080: 68db 1591 76af d0e5 4e80 5921 ef8f 453a  h...v...N.Y!..E:
+00003090: 46d4 1789 60e9 e26b 3cd9 ae08 c447 c6aa  F...`..k<....G..
+000030a0: 486d b751 2d77 da8c d306 9a80 4d57 7aac  Hm.Q-w......MWz.
+000030b0: 6b42 8e2a 6bdb 946d 8393 b381 bb11 b683  kB.*k..m........
+000030c0: 6d46 72aa 9c03 1eba 2112 cb63 a14d 09c5  mFr.....!..c.M..
+000030d0: 5fe1 40f1 101e c239 4174 0823 9c15 a410  _.@....9At.#....
+000030e0: d988 398f 779b ff2e 661a 8bed e8cc d9ae  ..9.w...f.......
+000030f0: 48ce f6f9 ac35 adee b769 c5a9 edf6 8407  H....5...i......
+00003100: 6315 99a7 e4b5 b15e d779 dd66 9747 d4b6  c......^.y.f.G..
+00003110: ed1e 9fc9 f588 51a3 7144 f12a a6f0 ed8a  ......Q.qD.*....
+00003120: f7f8 4c6e 8a57 b1de 6f57 10c7 6772 5d10  ..Ln.W..oW..gr].
+00003130: 8a53 3e7b 69e8 2deb dcff ebf0 8aac 5224  .S>{i.-.......R$
+00003140: 2f4f f9e7 c667 e998 0e43 56ab dfb6 60fe  /O...g...CV...`.
+00003150: cb28 da4c 35bc 4bf2 a2dc af51 6ebe 1691  .(.L5.K....Qn...
+00003160: 1aa9 f960 d382 844c ad07 d633 2691 9f6f  ...`...L...3&..o
+00003170: cb3e 95c0 b2d7 5081 c6d6 ecf3 e9fc f825  .>....P........%
+00003180: b9f6 c1a9 89ce 3baf 0c87 3c93 8262 6ffb  ......;...<..bo.
+00003190: e154 9cdc 5e0b a832 6e59 ef6c 9120 6fec  .T..^..2nY.l. o.
+000031a0: 1c3b 7b97 eda2 a39e deaa c482 a24a a93b  .;{..........J.;
+000031b0: 6b55 e7b2 02d3 78bb c8d3 8705 a5d0 b95e  kU....x........^
+000031c0: 54e9 3737 b102 2790 978a a6a7 e834 5505  T.77..'......4U.
+000031d0: 6c09 f291 5724 8992 af2b 00a2 cc5b a771  l...W$...+...[.q
+000031e0: 8328 4f78 2b08 90b6 0221 fb0a 4b10 603c  .(Ox+....!..K.`<
+000031f0: 9aaf 0a65 9e42 c378 55eb 83be b716 ec41  ...e.B.xU......A
+00003200: c148 5924 99b0 66d0 af4c 0464 b2ca bcd5  .HY$..f..L.d....
+00003210: 1e80 29f0 f27f a0c9 78ef 5b54 e94b 6981  ..).....x.[T.Ki.
+00003220: 4947 280e 8a84 dd2d 3f7a faea fd03 8a70  IG(....-?z.....p
+00003230: 9182 bcca 5537 f891 3081 c2d3 57ef ef79  ....U7..0...W..y
+00003240: 53c2 7697 1d3b a095 d242 f445 b88e 6afd  S.v..;...B.E..j.
+00003250: 91f3 6147 f647 ead3 5ddf 195d ae5a 7e65  ..aG.G..]..].Z~e
+00003260: 37a5 ddea 38be 689b d457 fbe7 d616 24a3  7...8.h..W....$.
+00003270: d1e8 7ad4 1127 4521 6f0a 50e0 03cd d9fb  ..z..'E!o.P.....
+00003280: 1c1a 1cf0 d40a 8a3d fd8f d1d5 79f7 7ae4  .......=....y.z.
+00003290: b78c 8e75 d531 da67 c831 bace d5b5 e1b4  ...u.1.g.1......
+000032a0: 8757 d7d7 7ed7 6a59 c33f 95cb 8117 5c0d  .W..~.jY.?....\.
+000032b0: 88bb 0c28 7dec 762f 4fe0 0281 967a 28e5  ...(}.v/O....z(.
+000032c0: 7abb 9af3 7465 2025 2bb6 046c abbc 775b  z...te %+..l..w[
+000032d0: ae75 e9d8 96e1 9f59 b6d1 7683 8ed1 71cf  .u.....Y..v...q.
+000032e0: 1cc3 77ec d6b5 dbbe 1a39 bea3 f0ee 3cf3  ..w......9....<.
+000032f0: 0ac1 326d 5b5e 4670 e69d 1ec3 294a 7056  ..2m[^Fp....)JpV
+00003300: 9951 653c ea2c d80f 0c9f d884 5969 c25c  .Qe<.,......Yi.\
+00003310: 5d14 0dfe 0500 00ff ff03 0050 4b03 0414  ]..........PK...
+00003320: 0006 0008 0000 0021 00b7 5bf5 4ac5 0300  .......!..[.J...
+00003330: 00c7 0c00 0014 0000 0078 6c2f 7368 6172  .........xl/shar
+00003340: 6564 5374 7269 6e67 732e 786d 6cac 57eb  edStrings.xml.W.
+00003350: 6ed3 4814 febf d2be c3c8 a015 0888 5b7e  n.H...........[~
+00003360: 2c50 9254 c671 095b 372e b950 4455 5953  ,P.T.q.[7..PDUYS
+00003370: fb24 b66a cf04 cfb8 a16f c533 ec93 ed19  .$.j.....o.3....
+00003380: 3b09 d5cc 7829 123f 7dee 97ef 9c33 ee1f  ;...x).?}....3..
+00003390: 7f2b 0b72 0b95 c839 1b38 87bd 0387 004b  .+.r...9.8.....K
+000033a0: 789a b3d5 c059 cc4f 5ebc 7688 9094 a5b4  x....Y.O^.v.....
+000033b0: e00c 06ce 1d08 e778 f8e7 1f7d 2124 415d  .......x...}!$A]
+000033c0: 2606 4e26 e5fa c875 4592 4149 458f af81  &.N&...uE.AIE...
+000033d0: 2167 c9ab 924a fcac 56ae 5857 4053 9101  !g...J..V.XW@S..
+000033e0: c8b2 705f 1e1c fced 9634 670e 4978 cde4  ..p_.....4g.Ix..
+000033f0: c079 f3ca 2135 cbbf d6e0 b784 d76f 9c61  .y..!5.......o.a
+00003400: 5fe4 c3be 1c7e ac41 488c 8ef0 1b72 dc77  _....~.AH....r.w
+00003410: e5b0 ef2a 46cb 9c5c 1354 6af8 0205 74f6  ...*F..\.Tj...t.
+00003420: 4e57 e88c 397c 933a ed84 26d2 103c e329  NW..9|.:..&..<.)
+00003430: 14ba a4cf 85a1 3daa 2baa c2d4 6547 5482  ......=.+...eGT.
+00003440: 4edb 85dc 9396 3096 2a8c 5e51 9431 6562  N.....0.*.^Q.1eb
+00003450: 0355 6f59 1745 cc68 6998 3124 134b 5c86  .UoY.E.hi.1$.K\.
+00003460: 50da 1168 704b 8d44 bd5a 723d f871 5d52  P..hpK.D.Zr=.q]R
+00003470: 234b c38b cc4b 6c0b 2dd7 b6da 11c4 13d9  #K...Kl.-.......
+00003480: c541 e87a 5ddc 11c9 092d 0ae4 a89c 8d36  .A.z]....-.....6
+00003490: f8bc aa20 91e4 9f59 3421 15c8 ba62 90ea  ... ...Y4!...b..
+000034a0: a62f b23c c976 1610 5aa5 b2bb c965 4664  ./.<.v..Z....eFd
+000034b0: 06a8 d594 1dd2 d648 0b4f 1ba0 9287 f8f2  .......H.O......
+000034c0: 4ace 5668 970b d87a c289 794e 3619 3092  J.Vh...z..yN6.0.
+000034d0: 7210 8dcb 303c 2329 40d9 7eed baae 52bd  r...0<#)@.~...R.
+000034e0: 46ad 0268 85c3 c6eb 5566 027b 8f7a 6f32  F..h....Uf.{.zo2
+000034f0: 227e 56b3 1b85 6f53 ee37 c7a1 1aa3 8a95  "~V...oS.7......
+00003500: b41e 31d2 8433 89a3 da50 b1e6 29d6 2fa5  ..1..3...P..)./.
+00003510: 92fe ef28 36fd dd9a 3087 729e 0116 8d56  ...(6...0.r....V
+00003520: d0d8 44d4 e5e9 be69 4ff2 1ef4 f623 ad32  ..D....iO....#.2
+00003530: 56f9 ef4d 3d35 a68b 2782 085e 5789 311d  V..M=5..'..^W.1.
+00003540: 1d95 c9f8 8620 80ef 4892 cb36 8256 9d3c  ..... ..H..6.V.<
+00003550: 4979 4238 2bee 9e9a b98d 949b 6764 4d57  IyB8+.......gdMW
+00003560: f03b bdb5 162d fe42 ca56 353a 3b22 cb4a  .;...-.B.V5:;".J
+00003570: 4ff9 6779 a9c2 62bf 4e2a dce3 1660 fd30  O.gy..b.N*...`.0
+00003580: 0dc6 143f d074 c056 452e 2cb6 af0e de92  ...?.t.VE.,.....
+00003590: c34b 6361 04de 2898 c6b3 0f5f 029d f557  .Kca..(...._...W
+000035a0: 21df be20 2d20 1008 b8c9 1b5c 20e6 d4cd  !.. - .....\ ...
+000035b0: 31b7 f1c7 4530 9b7f 8826 b11f 850f b4c5  1...E0...&......
+000035c0: 974b 0112 ebc8 4bf2 d87b 7cf8 6b6a 6a7b  .K....K..{|.kjj{
+000035d0: 6cc1 af86 f9ba e089 7964 e2e8 d4d8 72e3  l.......yd....r.
+000035e0: c5e4 7466 6184 dee4 bd2e 3c79 178f 227f  ..tfa.....<y..".
+000035f0: d641 8e71 02e2 73ef 7d60 08f8 d16c 6e0c  .A.q..s.}`...ln.
+00003600: c462 eaa9 0ae9 f4e0 9317 c6de 621e 5919  .b..........b.Y.
+00003610: e3c5 9967 a860 5898 b32d ac5d 1b6c bc13  ...g.`X..-.].l..
+00003620: cf9f 1bf4 7680 2ff3 2beb c56b d69b 1e57  ....v./.+..k...W
+00003630: 7351 ba34 3cfb 95d8 1e8f 2ead 7bec 7be7  sQ.4<.......{.{.
+00003640: d576 34ed 925d 97d3 2edd 7901 ef89 0382  .v4..]....y.....
+00003650: be47 2d47 5697 c96c 4757 17b2 bd26 b083  .G-GV..lGW...&..
+00003660: 7a65 ede1 da1e 1863 bcc8 b571 8bbd c9ec  ze.....c...q....
+00003670: 2298 ea3d 568f c123 b1a6 093e 12f1 b527  "..=V..#...>...'
+00003680: a0ba 0567 483c 7c5b aaad d951 bb9f 68d9  ...gH<|[...Q..h.
+00003690: 7aa3 404c 149c 1756 a0ef 1c0a 3ce3 c64d  z.@L...V....<..M
+000036a0: f0d5 58da 9687 42ad 8d8e e5b3 91df 8591  ..X...B.........
+000036b0: 7f6a dd68 3834 d3e8 c218 00bd 5525 487a  .j.h84......U%Hz
+000036c0: e964 4d7d 9d2b bd43 e7f8 d6d1 6953 9364  .dM}.+.C....iS.d
+000036d0: 378a c54f 72f5 9c37 edda 1550 1ee3 30a5  7..Or..7...P..0.
+000036e0: c75e 182e cc11 bfde 1feb 8dcb 499b 82b1  .^..........I...
+000036f0: bafe fdae 931e 198b e7f3 b971 0f6c fdee  ...........q.l..
+00003700: 408e bbfd 0f70 f147 64f8 1f00 0000 ffff  @....p.Gd.......
+00003710: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00003720: acd4 f4ab db02 0000 3b0d 0000 1800 0000  ........;.......
+00003730: 786c 2f64 7261 7769 6e67 732f 6472 6177  xl/drawings/draw
+00003740: 696e 6731 2e78 6d6c ec57 5d4f a430 147d  ing1.xml.W]O.0.}
+00003750: df64 ff03 e97b 8596 523e 328c 19be 3626  .d...{..R>2...6&
+00003760: 1bd7 87dd 1fd0 74c0 210b 7452 50c7 18ff  ......t.!.tRP...
+00003770: fb96 023a ea90 a8d1 ac26 becc 5c6e b9e7  ...:.....&..\n..
+00003780: b6f7 dc9e 96c5 f1ae ae8c cb5c b6a5 6842  ...........\..hB
+00003790: 808e 2c60 e40d 17eb b239 0fc1 9fdf 19f4  ..,`.....9......
+000037a0: 80d1 76ac 59b3 4a34 7908 aef3 161c 2fbf  ..v.Y.J4y...../.
+000037b0: 7f5b ecd6 32b8 6a13 6928 80a6 0dd4 6308  .[..2.j.i(....c.
+000037c0: 365d b70d 4cb3 e59b bc66 ed91 d8e6 8d1a  6]..L....f......
+000037d0: 2d84 ac59 a71e e5b9 b996 ec4a 41d7 9589  -..Y.......JA...
+000037e0: 2d8b 9aed 56e6 6cdd 6ef2 bc4b 8611 30e2  -...V.l.n..K..0.
+000037f0: b157 a0d5 ac6c c052 cfac bb12 715e 55ab  .W...l.R....q^U.
+00003800: 866f 841c 5c85 14f5 6071 512d d1c2 ec57  .o..\...`qQ-...W
+00003810: d09b 3a40 19bf 8a62 8910 b12d 7a37 d6bb  ..:@...b...-z7..
+00003820: f4b0 1457 4bec 0ffe de9e 9c8f 63d4 988e  ...WK.......c...
+00003830: d1e0 f719 3bb1 97f9 1efe 416a db43 9675  ....;.....Aj.C.u
+00003840: 3833 212f cc3c e53b 976c bb29 7926 599d  83!/.<.;.l.)y&Y.
+00003850: 1b35 e352 8460 ac50 73f9 636f f06c 2c12  .5.R.`.Ps.co.l,.
+00003860: 3fbd 3c93 46b9 0e01 0646 a3a2 4210 6f98  ?.<.F....F..B.o.
+00003870: ec0c a4c2 5890 efba 9f6d 375a c685 2c43  ....X....m7Z..,C
+00003880: 7093 6538 72d2 8cc0 4c59 9058 1181 514a  p.e8r...LY.X..QJ
+00003890: 7c98 61db 4bb1 9bc5 d8a6 b77d 34a2 0157  |.a.K......}4..W
+000038a0: 7477 aad3 4ed6 13cd 883e 21ba 2ed5 3c5b  tw..N....>!...<[
+000038b0: 5174 475c d4a6 288a 92e7 53e3 a8b6 41c4  QtG\..(...S...A.
+000038c0: d444 eb59 de24 d8b1 e214 ad20 a549 0449  .D.Y.$..... .I.I
+000038d0: bcf2 a16f fb1e 74ad 8444 c48d 2975 d25b  ...o..t..D..)u.[
+000038e0: 602e 17a6 9efd f4af 5731 7440 bfe2 9188  `.......W1t@....
+000038f0: d327 3561 c17e 097f 0afe b7ed b174 eb3c  .'5a.~.......t.<
+00003900: 7d5b fb0f 1776 5748 d57d 2c50 cb31 7621  }[...vWH.},P.1v!
+00003910: 50db ecba ff55 607a 5e06 1f9c 7cf2 6aa8  P....U`z^...|.j.
+00003920: 2968 9c43 ffee 6826 ac63 43fd 5fbc e778  )h.C..h&.cC._..x
+00003930: cfa7 e283 07da 1a89 e0af d86f 03d2 08f0  ...........o....
+00003940: aced 3f90 9908 7e51 e74d 3768 80cc 2bdd  ..?...~Q.M7h..+.
+00003950: 13ed a6dc b6c0 9041 df7d f264 8d46 d6f6  .......A.}.d.F..
+00003960: 56ac d9bb 2b86 2ed1 3e3d 238b 55a9 b0fb  V...+...>=#.U...
+00003970: 024d 4c1d 1083 f7d0 07e2 1cde a518 7b74  .ML...........{t
+00003980: dcf3 cf90 076f 4698 3cec 7933 c244 47d9  .....oF.<.y3.DG.
+00003990: 782c 4c73 89df 401d c843 75b0 3fa8 3ab8  x,Ls..@..Cu.?.:.
+000039a0: ae52 2137 5e41 97ba 0892 34cb a08f 130a  .R!7^A....4.....
+000039b0: 5718 a736 5959 7e1a b95f eab0 7f22 7f16  W..6YY~.._..."..
+000039c0: 75c0 ff55 1d66 8e70 c7a3 2e99 39c3 d1cc  u..U.f.p....9...
+000039d0: 19ee 2332 853c e7f2 30a2 3cbe b760 0ff9  ..#2.<..0.<..`..
+000039e0: 7399 e7ee 2d73 99df 401e 9c87 f240 3ea8  s...-s..@....@>.
+000039f0: 3c10 17fb b1ed 1048 3d4b 5d5d 92c8 829e  <......H=K]]....
+00003a00: 13ad 2072 0845 a9eb 7a56 ec7d c9c3 6794  .. r.E..zV.}..g.
+00003a10: 07fb bde4 415f 3afa ef9e e53f 0000 00ff  ....A_:....?....
+00003a20: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00003a30: 00be cf15 7fd7 0800 0084 3f00 0014 0000  ..........?.....
+00003a40: 0078 6c2f 6368 6172 7473 2f63 6861 7274  .xl/charts/chart
+00003a50: 312e 786d 6cec 5bfb 8fdb b811 febd 40ff  1.xml.[.......@.
+00003a60: 0755 d803 5a5c b5b6 6cc9 2fc4 1bd8 b275  .U..Z\..l./....u
+00003a70: 48bb 7934 9bbb 022d 8a82 9668 afba 14a9  H.y4...-...h....
+00003a80: 90d4 3e72 b8ff bdc3 872c d96b 6737 b9dc  ..>r.....,.kg7..
+00003a90: 5db3 5510 7825 3e46 e4cc 70f8 89fa e6d9  ].U.x%>F..p.....
+00003aa0: f3db 9c38 d798 8b8c d1a9 eb9f 765d 07d3  ...8........v]..
+00003ab0: 84a5 19dd 4cdd efdf c5de c875 8444 3445  ....L......u.D4E
+00003ac0: 8451 3c75 efb0 709f 9ffd fe77 cf92 4972  .Q<u..p....w..Ir
+00003ad0: 89b8 bc28 5082 1d10 42c5 2499 ba97 5216  ...(P...B.$...R.
+00003ae0: 934e 4724 9738 47e2 9415 9842 dd9a f11c  .NG$.8G....B....
+00003af0: 49b8 e59b 4eca d10d 08cf 49a7 d7ed 0e3a  I...N.....I....:
+00003b00: 5a88 6b05 a0cf 1090 a38c 56fd f963 fab3  Z.k.......V..c..
+00003b10: f53a 4bf0 8225 658e a934 a3e0 9820 091a  .:K..%e..4... ..
+00003b20: 1097 5921 2a69 893f e0bd 7b12 f32c e14c  ..Y!*i.?..{..,.L
+00003b30: b0b5 3c4d 58de 31c2 aa49 8130 3fec 6c67  ..<MX.1..I.0?.lg
+00003b40: 7506 4a4a 91c4 feb8 1b38 d788 4cdd aedb  u.JJ.....8..L...
+00003b50: 5185 04d1 8d29 c0d4 fbfe c214 7256 d214  Q....)......rV..
+00003b60: a711 e314 ccd1 689f 2793 1991 9853 1015  ......h.'....S..
+00003b70: 312a 61d4 565f f9a3 349e 237e 5516 1e0c  1*a.V_..4.#~U...
+00003b80: b780 49ae 3292 c93b 3d6d f7ec 19c8 8e2e  ..I.2..;=m......
+00003b90: 19e8 c379 8bdf 9719 c762 ea26 7e50 ab20  ...y.....b.&~P. 
+00003ba0: f854 0574 879d 51a7 67ed 0a93 f583 8990  .T.t..Q.g.......
+00003bb0: 7704 9b09 f9dd 9e9a 6d67 fb5c 3d84 1811  w.......mg.\=...
+00003bc0: b242 c995 d24d a3f1 b669 5daf 3aee 2b43  .B...M...i].:.+C
+00003bd0: f5d2 6ea4 2e50 29d9 bb4c 12bc c004 4b9c  ..n..P)..L....K.
+00003be0: eee8 bd20 4cce 3846 c606 77ac 94da 1c2b  ... L.8F..w....+
+00003bf0: c423 e5cb aa18 ae17 1937 bd12 468c 6936  .#.......7..F.i6
+00003c00: 609b 029c d616 9352 8039 706a 2aaf 11bf  `......R.9pj*...
+00003c10: 8b18 613b 3683 7960 aee4 65e9 edce 1018  ..a;6.y`..e.....
+00003c20: 4fb1 156f 9d41 de9a 69f3 b778 adae d667  O..o.A..i..x...g
+00003c30: 1712 16cb 1f4e e627 bd67 1d75 afb5 c223  .....N.'.g.u...#
+00003c40: 048b 4a5d 1732 0257 9156 a166 1085 74e0  ..J].2.W.V.f..t.
+00003c50: 49ca c154 8beb 3344 c50d 78d1 3fb3 7f9d  I..T..3D..x.?...
+00003c60: 1292 ffdb dc9e 5294 6325 f21a 2ca0 e4e8  ......R.c%..,...
+00003c70: 3f42 56a2 a10c 6ef4 30e0 d28e ab78 03f3  ?BV...n.0....x..
+00003c80: 4013 c148 96c6 1921 fa46 2d6f 1c11 3b11  @..H...!.F-o..;.
+00003c90: 79eb 6ba3 eeb5 2254 b5a5 4cf5 023d a349  y.k..."T..L..=.I
+00003ca0: c185 5c20 7169 46ae 25da 7eaa a97a ba7e  ..\ qiF.%.~..z.~
+00003cb0: 1828 8d42 4492 2fd6 aff0 063c f6da fa8e  .(.BD./....<....
+00003cc0: d557 7abe 2242 ebc4 0ead f184 cf7f a4bc  .Wz."B..........
+00003cd0: 35f3 5cb1 f4ee 0d77 3893 4a99 8e28 9238  5.\....w8.J..(.8
+00003ce0: 8361 9f23 21df 200e 01ca 7755 b894 afe1  .a.#!. ...wU....
+00003cf0: 674d d8cd d4c5 8440 d0c8 206c a872 582e  gM.....@.. l.rX.
+00003d00: 8c7f 709d 1b8e 8aa9 2bde 9788 63d7 212f  ..p.....+...c.!/
+00003d10: 282c acfe c8ef 824c a96f 2028 8470 c39b  (,.....L.o (.p..
+00003d20: 35ab 660d a209 8882 e528 b9eb 989b 48c2  5.f......(....H.
+00003d30: bd0f 2606 4d17 33f0 f438 531e dc41 1333  ..&.M.3..8S..A.3
+00003d40: 6c55 4184 bc50 ebcd 685c abdd cc2c c5eb  lUA..P..h\...,..
+00003d50: b730 33f1 61ea 8ed5 3056 7a82 9999 a6e4  .03.a...0Vz.....
+00003d60: d915 4477 ca2e f495 eb5c 41bc 8167 418c  ..Dw.....\A..gA.
+00003d70: 8696 4860 92a9 e8af dceb 615f d0c3 28f3  ..H`......a_..(.
+00003d80: 97cc aebe 61d8 0531 7a40 a4cc 5faf d7c6  ....a..1z@.._...
+00003d90: 017a 5531 8c5f 6f18 caa3 f46c 769c 4d45  .zU1._o....lv.ME
+00003da0: 66ea c8bb 02af 61ab 99ba dfe6 d423 d288  f.....a......#..
+00003db0: c368 af02 2353 9188 bd8a 4458 5733 6ad0  .h..#S....DXW3j.
+00003dc0: 8fb1 fe83 69aa 4cab 94a3 02f3 d45d 732f  ....i.L......]s/
+00003dd0: 7e6b 9b17 da31 8d77 4034 07df 7bc3 6c70  ~k...1.w@4..{.lp
+00003de0: 86f0 b1a4 3608 884b 7673 8e37 20ea aff8  ....6..Kvs.7 ...
+00003df0: 6e67 c1ab 9a1f 10ec b12a feeb 7502 7e0e  ng.......*..u.~.
+00003e00: 6511 92af 6039 de6b 7b81 f9c1 f237 9827  e...`9.k{....7.'
+00003e10: 2af2 37f7 1125 675e ae56 045f 641f ee8b  *.7..%g^.V._d...
+00003e20: 3ac7 0882 cd39 58ae b99d 2413 7c2b cf85  :....9X...$.|+..
+00003e30: 8e76 70e5 941c 7ce0 c768 3908 fbc3 99ef  .vp...|..h9.....
+00003e40: 2d06 71e4 05eb 41e8 8d17 63df 1bf6 7a41  -.q...A...c...zA
+00003e50: 148c 8370 349f ff54 6f0b e127 ef8b cd2d  ...p4..To..'...-
+00003e60: 21d4 1a38 3c3c 0803 302a adf5 6a9c 50b4  !..8<<..0*..j.P.
+00003e70: 5df4 09d2 03af e294 0a8f 7fb4 f172 7612  ]............rv.
+00003e80: fe79 7b39 ac2f c7f5 a5ef 4f4e 6627 7eff  .y{9./....ONf'~.
+00003e90: 4f0f 07d6 c1e1 c00a db33 c789 74fe 72f1  O........3..t.r.
+00003ea0: fa95 c3b1 2c61 b74e 7763 aa8a ac26 1aab  ....,a.Nwc...&..
+00003eb0: a5aa a2ed df4a 2c14 bc70 d895 f3fc 58e3  .....J,..p....X.
+00003ec0: de7e e3d9 ab85 135d 96f4 4a7c b45f dff6  .~.....]..J|._..
+00003ed0: 0344 231c c14a 7093 638f 089a 4dbf 750a  .D#..Jp.c...M.u.
+00003ee0: b4c1 0ff4 086d 8f73 5818 2534 9f38 6bfe  .....m.sX.%4.8k.
+00003ef0: e81d c4da 0a3c 56a9 8196 f976 87ab 4c36  .....<V....v..L6
+00003f00: af4d 363f d99a 6c7e b235 d9fc 4499 0c7e  .M6?..l~.5..D..~
+00003f10: 1b26 0341 dbbd d020 cb88 a5f8 acfb 8d36  .&.A... .......6
+00003f20: aa86 9aba 607f ab3c 62d1 ee43 d63b daa0  ....`..<b..C.;..
+00003f30: b2d8 d106 9569 8e36 a80c 72b4 41a5 ffbd  .....i.6..r.A...
+00003f40: 06b0 226a 2d98 9b6a dbb6 da3e b8c6 fbfd  .."j-..j...>....
+00003f50: 5137 8a02 2f5c 0c96 5ed0 1d47 de7c d9ef  Q7../\..^..G.|..
+00003f60: 79cb 616f d11b 0ffb 613f 8a1a 6b7c f0c9  y.ao....a?..k|..
+00003f70: 6b3c 68c0 bec1 a4a4 d9fb 12bf b09b c08f  k<h.............
+00003f80: b007 e87f 5e1c 2f03 2f58 ce43 6fd6 1fcd  ....^././X.Co...
+00003f90: bd71 b7b7 1cfa f03f 982d 7ed2 51f7 6004  .q.....?.-~.Q.`.
+00003fa0: b078 6a1f 56d9 88da 8055 b6e4 28ac 8a1e  .xj.V....U..(...
+00003fb0: 0dab 0c1e b2be f673 c0d1 fe86 a836 be03  .......s.....6..
+00003fc0: 1be2 b6f8 810d b1c5 552d ae52 68e2 e9e0  ........U-.Rh...
+00003fd0: aa16 3e3d 74ac d0c2 a716 3edd 834f 510d  ..>=t.....>..OQ.
+00003fe0: 9fa2 1a3e 4535 7c8a 347c 82df 163e ed9d  ...>E5|.4|...>..
+00003ff0: 7a7c adf0 c9ff b2f0 491f b125 9306 7cb2  z|......I..%..|.
+00004000: 2547 e1d3 e297 864f 7cb3 da9e 2c05 bd51  %G.....O|...,..Q
+00004010: 1807 ede1 527b b8a4 8f3d d441 e3d3 3d5c  ....R{...=.A..=\
+00004020: 6a41 500b 82aa 73f9 f60c 497d 0c81 77ee  jAP...s...I}..w.
+00004030: 87cf 9016 3508 5ad4 2068 5183 a085 0641  ....5.Z. hQ....A
+00004040: f0db 82a0 2702 827a 5f16 04f5 cd51 6f03  ....'..z_....Qo.
+00004050: 04d9 92a3 2068 f96b 82a0 781c 87cb 590b  .... h.k..x...Y.
+00004060: 825a 10d4 82a0 f643 9adf 9e04 b527 41f7  .Z.....C.....'A.
+00004070: 4e82 9635 085a d620 6859 83a0 a506 41f0  N..5.Z. hY....A.
+00004080: db82 a027 0282 fa5f 1604 e953 969d 9320  ...'..._...S... 
+00004090: 5b72 1404 c5bf 2a08 1a46 23f3 cd4c 7d1c  [r....*..F#..L}.
+000040a0: 6b92 915a 9a51 4b33 d2c0 a8fd 1cd6 b289  k..Z.QK3........
+000040b0: f6c9 4e2d 9ba8 a21e fd1f b089 e21a 04c5  ..N-............
+000040c0: 3508 8a6b 1014 6b10 04bf 2d08 7a22 2028  5..k..k...-.z" (
+000040d0: f879 20a8 e612 3f8e bf69 29c8 bf38 7fb3  .y ...?..i)..8..
+000040e0: c978 dca0 e2ef 592a 2d6b bae7 8fed 6915  .x....Y*-k....i.
+000040f0: b08d 092a 0c1f d4eb 0d4d 29ba adf8 567e  ...*.....M)...V~
+00004100: 10f4 bba3 617f 6c3f e835 6a86 dd51 7f10  ....a.l?.5j..Q..
+00004110: 8e42 4d88 8347 35f9 ef70 de3a d384 f4e3  .BM..G5..p.:....
+00004120: 9244 8280 0dbc 519c 3ec6 33e0 a4ea d409  .D....Q.>.3.....
+00004130: 3390 3ca3 2fd1 ad65 7135 1aa6 9a8d bf43  3.<./..eq5.....C
+00004140: 5e45 b75b 26ed ca0c 1ebe c9c6 b974 6a4e  ^E.[&........tjN
+00004150: dfd4 fd0e 4332 0422 40c4 d6c4 4608 ef57  ....C2."@...F..W
+00004160: 38dd f268 73f4 1fc6 df65 c9d5 4b48 7130  8..hs....e..KHq0
+00004170: c229 64a9 1869 3094 e395 123a 35b9 bc14  .)d..i0....:5...
+00004180: f872 ef98 e968 58e8 3bcc 7542 1d60 7a8f  .r...hX.;.uB.`z.
+00004190: c35e e83a 8922 76af 8195 0c97 7901 8311  .^.:."v.....y...
+000041a0: 7403 046d b201 beb4 e26a 7f0e 43da 3fcc  t..m.....j..C.?.
+000041b0: 901e 3d8e 217d 8457 8f26 3aa5 c410 c4f7  ..=.!}.W.&:.....
+000041c0: 18f6 87e8 eede c032 f4be 18ed fd38 85dd  .......2.....8..
+000041d0: 90c1 fff7 a8ea 83c3 86e8 7f7d 5475 95a5  ...........}Tu..
+000041e0: 2466 36f9 c4df 59f2 f055 4555 56ac 7095  $f6...Y..UEUV.p.
+000041f0: 32f3 0fcc adf7 abbb 1db2 3a59 9119 38b7  2.........:Y..8.
+00004200: cd7d 0107 3729 4c2b 0244 7e81 ab34 14f3  .}..7)L+.D~..4..
+00004210: 6e06 b454 f6b2 2432 3bbf 26b0 bc1a ebdd  n..T..$2;.&.....
+00004220: 7cca 31a1 05d0 fabd 18b3 37c0 c7c5 9864  |.1.......7....d
+00004230: 92a3 6a86 9f1a 736c 6a8f 0e21 dff1 2c55  ..j...slj..!..,U
+00004240: 090e 3b69 254f 6ccd 8301 eecf f540 c4ed  ..;i%Ol......@..
+00004250: 7ef3 db07 dbcf cd1b 6aa3 dad4 3dc4 9178  ~.......j...=..x
+00004260: aa51 6d0f e27c 24aa e9aa 3996 3718 db48  .Qm..|$...9.7..H
+00004270: b632 3736 6cd8 90a4 b2e2 9a39 823a a347  .276l......9.:.G
+00004280: 670b eaab 7dc0 c234 06db cbf7 f97a b2d2  g...}..4.....z..
+00004290: daed f9b7 ca24 033f 235b df52 1ef7 4326  .....$.?#[.R..C&
+000042a0: 5e53 623d c966 30a4 9928 e690 9176 2566  ^Sb=.f0..(...v%f
+000042b0: 367f 0b5e 052c 4485 d795 85ca 8354 6988  6..^.,D......Ti.
+000042c0: 00b8 f736 da2a 99b5 42b2 1f4b de5c 6d8e  ...6.*..B..K.\m.
+000042d0: 246f 3e31 c45b f08c ca0b 2c21 9970 a3f7  $o>1.[....,!.p..
+000042e0: f94b 9d1d 1733 06b9 bc1a d2a8 7428 7891  .K...3......t(x.
+000042f0: d864 54e8 e4c8 d321 a07d 95b4 7d3a 843c  .dT....!.}..}:.<
+00004300: 4dfb 57a5 85ea 0ad3 5ddd f55d 7865 5152  M.W.....]..]xeQR
+00004310: cccd 5616 3cac 2c14 fa86 a0b2 fb70 0586  ..V.<.,......p..
+00004320: b6c9 f367 ff05 0000 ffff 0300 504b 0304  ...g........PK..
+00004330: 1400 0600 0800 0000 2100 4192 87f0 fd08  ........!.A.....
+00004340: 0000 0133 0000 1400 0000 786c 2f63 6861  ...3......xl/cha
+00004350: 7274 732f 6368 6172 7432 2e78 6d6c ec5b  rts/chart2.xml.[
+00004360: 5b6f e3b8 157e 2fd0 ffa0 0a41 5f16 8ead  [o...~/....A_...
+00004370: 9b6f 1d67 61cb f162 d0cc 4e30 c96e 8116  .o.ga..b..N0.n..
+00004380: 4541 4bb4 a386 2235 2495 cb2c f607 f537  EAK..."5$..,...7
+00004390: f471 ff58 0f2f 7224 c799 248e d3a6 99e4  .q.X./r$..$.....
+000043a0: 2111 2fa2 0ecf 8de7 3b87 79f7 fd55 4e9c  !./.....;.y..UN.
+000043b0: 0bcc 45c6 e8c8 f5f6 3bae 8369 c2d2 8c2e  ..E.....;..i....
+000043c0: 47ee 4fa7 b356 df75 8444 3445 8451 3c72  G.O..V.u.D4E.Q<r
+000043d0: afb1 70bf 3ff8 fdef de25 c3e4 0c71 7952  ..p.?....%...qyR
+000043e0: a004 3bb0 0815 c364 e49e 4959 0cdb 6d91  ..;....d..IY..m.
+000043f0: 9ce1 1c89 7d56 600a 630b c673 24a1 c997  ....}V`.c..s$...
+00004400: ed94 a34b 583c 276d bfd3 e9b6 f522 ae5d  ...KX<'m.....".]
+00004410: 006d b140 8e32 5abd cf1f f23e 5b2c b204  .m.@.2Z....>[,..
+00004420: 4f59 52e6 984a 4305 c704 49e0 8038 cb0a  OYR..JC...I..8..
+00004430: 51ad 9678 5dee df5a 31cf 12ce 045b c8fd  Q..x]..Z1....[..
+00004440: 84e5 6db3 58b5 2958 cc8b daab 5d1d 0093  ..m.X.)X....]...
+00004450: 5224 b137 e884 ce05 2223 b7e3 b655 2741  R$.7...."#...U'A
+00004460: 7469 3a30 6dfd 7462 3a39 2b69 8ad3 9871  ti:0m.tb:9+i...q
+00004470: 0ae2 a8cd cf93 e198 48cc 292c 1533 2a81  ........H.),.3*.
+00004480: 6acb affc 411c cf11 3f2f 8b16 905b c026  j...A...?/...[.&
+00004490: e719 c9e4 b5de b67b f00e d68e cf18 f0c3  .......{........
+000044a0: f984 3f97 19c7 62e4 265e 78c3 82f0 b10c  ..?...b.&^x.....
+000044b0: e8f4 dafd b66f e50a 9bf5 c2a1 90d7 049b  .....o..........
+000044c0: 0d79 1d5f edb6 bdfa ae26 6186 0899 a3e4  .y._.....&a.....
+000044d0: 5cf1 a636 7935 f566 5cbd b8ce 0cf5 9656  \..6y5.f\......V
+000044e0: 23f5 2033 49b0 7eb8 52bf 7996 9c1d bc43  #. 3I.~.R.y....C
+000044f0: c339 4baf 8fb9 c399 5442 7044 91cc 322e  .9K.....TBpD..2.
+00004500: e411 12f2 1871 d03b cf55 5620 3fc2 af05  .....q.;.UV ?...
+00004510: 6197 2317 1302 ba90 8136 a87e e002 e35f  a.#......6.~..._
+00004520: 5ce7 92a3 62e4 8acf 25e2 d875 104d a01b  \...b...%..u.M..
+00004530: 3826 79d5 8825 b43d b547 3424 429e a8ad  8&y..%.=.G4$B...
+00004540: eb46 a17a 8a63 aefe a478 f109 a811 5f60  .F.z.c...x...._`
+00004550: 6ad8 017a e69a aacc d026 7976 0e96 46d9  j..z.....&yv..F.
+00004560: 897e 729d 7390 3dcc 047b d194 eb59 7324  .~r.s.=..{...Ys$
+00004570: 30c9 9445 7640 8c68 2818 c9d2 5946 886e  0..Ev@.h(...YF.n
+00004580: 28f3 c331 e186 e9f2 cad3 7348 997f 60a9  (..1......sH..`.
+00004590: e9eb 461d 58ce 9059 e61f 170b d31d 54dd  ..F.X..Y......T.
+000045a0: 6d58 b25a 05e4 b5f6 0165 2dd4 91d7 055e  mX.Z.....e-....^
+000045b0: 80f9 8fdc ef72 da22 d22c 87d1 da00 4666  .....r.".,....Ff
+000045c0: 2011 6b03 89d0 ba50 f143 7fc6 7248 b389   .k....P.C..rH..
+000045d0: 038f 94a9 8cdc 056f cd3e 9955 e4c1 29ce  .......o.>.U..).
+000045e0: 0be1 60e9 24ec b77f 4ba7 4020 d7df fe55  ..`.$...K.@ ...U
+000045f0: 80f5 6245 a8d4 ebc0 02f0 0c4c 6f57 4a00  ..bE.......LoWJ.
+00004600: 0f52 eb04 0381 1274 ddb0 4861 bf4b 99e2  .R.....t..Ha.K..
+00004610: a161 0b55 acac 7514 a030 5324 cecc 8b9a  .a.U..u..0S$....
+00004620: e196 7e02 5361 79b3 88fa 4ea5 84a8 94ec  ..~.Say...N.....
+00004630: 5435 a698 6089 2def ad17 2808 9363 8e91  T5..`.-...(..c..
+00004640: f108 d7ac 94da 39cc 118f 9567 55dd f03c  ......9....gU..<
+00004650: cdac 1413 468c a358 82a7 28c0 851a 3a12  ....F..X..(...:.
+00004660: 520a 700e 3835 8317 885f c78c b086 0701  R.p.85..._......
+00004670: d230 3024 1966 e955 63db 8ca7 d82e 6f89  .00$.f.Uc.....o.
+00004680: 322c 1292 7fc2 0bf5 c6e2 e044 82eb fec3  2,.........D....
+00004690: de78 2f50 7bd4 9d30 1c23 d00e 35a1 9031  .x/P{..0.#..5..1
+000046a0: 382e 69cd db10 5148 07be 6454 3319 5e1c  8.i...QH..dT3.^.
+000046b0: 3863 6039 5a62 272d b9f6 b36a a50b cdb3  8c`9Zb'-...j....
+000046c0: 4289 4b59 7db5 a269 e8af af24 5649 e76b  B.KY}..i...$VI.k
+000046d0: 4a8e 9204 1ca3 b6bc 5bda baa5 2481 5f54  J.......[...$._T
+000046e0: 19ff fbc5 8f78 0974 5f58 2766 5995 1e6b  .....x.t_X'fY..k
+000046f0: 19ad f3f4 abef cccb f99c e060 ba51 f9ee  ...........`.Q..
+00004700: b361 e538 d70d 71eb ade1 2b79 24f4 06e0  .a.8..q...+y$...
+00004710: c929 3938 9f5f e220 e877 e238 6c45 d3ee  .)98._. .w.8lE..
+00004720: 612b ec0c e2d6 e430 f05b 873d 7fea 0f7a  a+.....0.[.=...z
+00004730: 4114 c4f1 afb5 e3f1 d187 6358 3b17 bac3  A.........cX;...
+00004740: 9266 9f4b fcde 5ac5 2fe0 90d4 8fd7 eacf  .f.K..Z./.......
+00004750: c24e 2b0c e371 6bd2 0bc3 567f 3aeb c7c1  .N+..qk...V.:...
+00004760: 6012 8d67 b35f b5c5 2543 a059 eb4d b50b  `..g._..%C.Y.M..
+00004770: 5015 2b8e 75a9 688d b847 924f 928a f6f4  P.+.u.h..G.O....
+00004780: 35cf aa3c e806 cfba eabe c7b3 be3e 8106  5..<.........>..
+00004790: bb15 a88e 0a76 2750 be9c af0e cad0 ef47  .....v'P.......G
+000047a0: b3d0 3af5 8635 2a0f bfcd 61a0 35f5 65da  ..:..5*...a.5.e.
+000047b0: 59b4 5bb1 04c6 f5ef cafb d5c5 321b cca2  Y.[.........2...
+000047c0: c3f1 3722 96de 6ec5 a2b5 f979 ac65 d68b  ..7"..n....y.e..
+000047d0: fbc6 d37d 03a7 d2e0 8962 399a 13a1 e1cd  ...}.....b9.....
+000047e0: ee02 4d15 cf1a 3cf1 3ce8 86bc a780 0683  ..M...<.<.......
+000047f0: bea7 7087 d40d 40b2 1134 787d 645e 1fb9  ..p...@..4x}d^..
+00004800: 1b11 695c 528c 2120 9e65 2ad0 059d 3164  ..i\R.! .e*...1d
+00004810: 3f14 290d 1e07 949e 0a90 7a9b 0192 ff42  ?.).......z....B
+00004820: 0012 a6a9 02ae 0a46 ae41 a415 ec31 da01  .......F.A...1..
+00004830: b1f5 19bb 3cc2 4b78 e3cf 780d f5c0 c8cf  ....<.Kx..x.....
+00004840: 08f2 3f2a 3761 0325 353b 46f2 4794 37a3  ..?*7a.%5;F.G.7.
+00004850: 5dd5 7f82 f9c6 fe63 cc55 f0dd 0c6a 61fe  ]......c.U...ja.
+00004860: 4447 bb27 d997 db4b 1d61 04d0 e308 106c  DG.'...K.a.....l
+00004870: 3dd5 71c7 7179 d88d 82de d86b 4dbb b3b8  =.q.qy.....kM...
+00004880: 152e ba51 6b30 1d78 ad9e ef87 7138 08a3  ...Qk0.x....q8..
+00004890: fe64 520b 4ba3 4787 a5f5 7445 64f9 b589  .dR.K.G...tEd...
+000048a0: 3c88 3237 059e 956d 2748 c7d3 1bc0 d364  <.27...m'H.....d
+000048b0: cf1f eecd f6fc ad11 14a2 e212 b242 7fcb  .............B..
+000048c0: febe 4f48 fe0f d3dc a720 a407 4329 4b1d  ..OH..... ..C)K.
+000048d0: c85a f921 5ae6 eb08 6fb2 1728 226f 601e  .Z.!Z...o..("o`.
+000048e0: cc59 c13c 93c2 8b59 8a0f 3a2a 4928 5cbd  .Y.<...Y..:*I(\.
+000048f0: 179d d8d3 bdeb 5030 da0c 053b 4d7a 157e  ......P0...;Mz.~
+00004900: 3458 51a5 2814 28bc 7382 7fdf 84e0 be09  4XQ.(.(.s.......
+00004910: e1e6 0920 d59b 9d9a 4605 3f2d b35e 2c56  ... ....F.?-.^,V
+00004920: 1a6f 792a d974 40ba 3a95 1ee6 222c f07d  .oy*.t@.:...",.}
+00004930: 7617 a1d0 5c45 da12 157f c952 69b3 2ee0  v...\E.....Ri...
+00004940: 7d8d 5ea1 ab0a 3706 811f f5bb 5177 c340  }.^...7.....Qw.@
+00004950: af37 e875 bdae c58c f5c4 8a4a 9dad b22c  .7.u.......J...,
+00004960: cd84 8ac9 76f3 c7e5 53ac f3ac e553 6ccf  ....v...S....Sl.
+00004970: 57f2 29e1 d3f3 2909 1372 cb5c 0aa1 0e64  W.)...)..r.\...d
+00004980: 3901 f0f4 22d7 4954 5693 d3f4 de54 a2c9  9...".ITV....T..
+00004990: b298 c4ec 5a2a e28e f418 1aea c4b6 39f1  ....Z*........9.
+000049a0: 1b89 b264 a832 d326 3125 aef3 39b3 0711  ...d.2.&1%..9...
+000049b0: 8542 8315 d9cd 841b 557d 0ba0 de02 a81d  .B......U}......
+000049c0: 6498 df02 a8b7 006a e701 54a8 02a8 1bbf  d......j..T.....
+000049d0: 7e77 00a5 b0cc deb7 1442 899c b1ea 10b7  ~w.......B......
+000049e0: 27f5 8b8d aa26 af3f aa32 076b 13f8 dd96  '....&.?.2.k....
+000049f0: d04d 90e5 753b be17 746f 475f dec0 f73a  .M..u;..toG_...:
+00004a00: bdc0 0f4c 4c00 b5ed 7a64 0598 63ac 6b6e  ...LL...zd..c.kn
+00004a10: 7786 6b22 41f0 c652 c5fe 8c67 0022 757d  w.k"A..R...g."u}
+00004a20: c810 9667 f403 bab2 a140 6d62 aa8b 690d  ...g.....@mb..i.
+00004a30: b489 ae8e 9905 9273 1320 82ed cd72 e9dc  .......s. ...r..
+00004a40: e096 91fb 0386 ca3a 2200 5e58 0980 15c0  .......:".^X....
+00004a50: e739 4e57 c037 47ff 64fc 344b ce3f 4054  .9NW.7G.d.4K.?@T
+00004a60: 6216 af22 1188 5432 7af7 a084 9720 5c5d  b.."..T2z.... \]
+00004a70: 5140 41b3 4f99 2163 6361 5145 5e83 c8af  Q@A.O.!ccaQE^...
+00004a80: 02af 0594 5321 06cb 0b20 46d0 2594 92c9  ....S!... F.%...
+00004a90: 120a beaa aabc 4d69 d7db 9cb9 e83f 2c73  ......Mi.....?,s
+00004aa0: b145 18b7 290d d502 5dd1 3f2f a9d8 fe5f  .E..)...].?/..._
+00004ab0: 4e21 bdf0 1afb 2322 2075 e545 8c6d ed38  N!....#" u.E.m.8
+00004ac0: 086a b80a ae5e a8b1 2a8b a30a de7f c5dc  .j...^..*.......
+00004ad0: 2abf 6a35 7c0c 9993 31e8 b6ad 5c83 7e9b  *.j5|...1...\.~.
+00004ae0: eb30 7302 1710 0454 f44d 22aa f232 947d  .0s....T.M"..2.}
+00004af0: 2889 cc8e 2e08 5857 cddc 011e ae1c 0bbc  (.....XW........
+00004b00: 71db c334 e8db bd87 b175 78ed 307e e059  q..4.....ux.0~.Y
+00004b10: aa5c 5e23 b96b b0d5 abb1 70e0 f7ed bd6e  .\^#.k....p....n
+00004b20: f0af 9018 fae3 e792 c93f 39c2 fcfd df7b  .........?9....{
+00004b30: da6d ab76 6f2e 6de4 fe1f 5e1b dade a535  .m.vo.m...^....5
+00004b40: 7248 5f71 697a 6882 e525 c6d6 8dcd 4dc3  rH_qizh..%....M.
+00004b50: 8629 2b7f b421 f459 0ba2 9eea 986c 86e9  .)+..!.Y.....l..
+00004b60: 7942 1fb8 8d64 9cf3 d691 4fe3 cc68 8689  yB...d....O..h..
+00004b70: 2ff0 d058 2770 f7a7 863d ec36 fbcd 4ee5  /..X'p...=.6..N.
+00004b80: 39f7 1eeb 399f 2ea8 1dde 7ddb 5c92 7c8b  9...9.....}.\.|.
+00004b90: 0547 ee2b 8d05 d75c 5ac3 71e6 06bb 5963  .G.+...\Z.q...Yc
+00004ba0: bfdf 6742 98d1 b812 a94b 96fa 72a4 7e5a  ..gB.....K..r.~Z
+00004bb0: 0778 cf7c 8df3 b9ab eb3b b83b fc06 67ea  .x.|.....;.;..g.
+00004bc0: 5786 1f7c f683 9e91 956e 298d fb39 131f  W..|.....n)..9..
+00004bd0: 29b1 a571 7baa a699 2826 5059 3f17 639b  )..q{...(&PY?.c.
+00004be0: 5780 4294 85f4 502c 9baa f294 ba2c 0e09  W.B...P,.....,..
+00004bf0: 8a35 6452 dddd 7dc8 a5d5 f9f2 8e0b abaf  .5dR..}.........
+00004c00: 2c43 50f0 8cca 132c e1d6 f852 23a5 335d  ,CP....,...R#.3]
+00004c10: fe9f 414e 1073 8d01 0bb8 1e0c 8997 6546  ..AN.s........eF
+00004c20: 85be 0dbf afca 52ea 3f26 f67b 70df c4fe  ......R.?&.{p...
+00004c30: 5597 f7f5 8079 5db5 0217 523c 6a15 d358  U....y]...R<j..X
+00004c40: ad05 1f2b 0b55 7402 a7d2 fcb8 428f abff  ...+.Ut.....B...
+00004c50: 5c39 f80f 0000 00ff ff03 0050 4b03 0414  \9.........PK...
+00004c60: 0006 0008 0000 0021 00bc 8d4e cc4f 0800  .......!...N.O..
+00004c70: 0015 2a00 0014 0000 0078 6c2f 6368 6172  ..*......xl/char
+00004c80: 7473 2f63 6861 7274 332e 786d 6cec 5a5b  ts/chart3.xml.Z[
+00004c90: 73db b815 7eef 4cff 03cb f13e 7564 91d4  s...~.L....>ud..
+00004ca0: 8dd2 44de 9129 6bbb 5327 f1c4 d9dd 9976  ..D..)k.S'.....v
+00004cb0: 3a1d 0884 24d4 20c0 00a0 6d65 67ff fb1e  :...$. ...meg...
+00004cc0: 5c28 8bb2 92c8 76b6 4d52 fb41 2671 39c4  \(....v.MR.A&q9.
+00004cd0: e57c dfb9 002f bebf 2d58 704d a4a2 828f  .|.../..-XpM....
+00004ce0: c3f8 380a 03c2 b1c8 295f 8ec3 9fde ce5a  ..8.....)_.....Z
+00004cf0: 6918 288d 788e 98e0 641c ae89 0abf 3ff9  i.(.x...d.....?.
+00004d00: f39f 5ee0 115e 21a9 2f4b 8449 0042 b81a  ..^..^!./K.I.B..
+00004d10: e171 b8d2 ba1c b5db 0aaf 4881 d4b1 2809  .q........H...(.
+00004d20: 87ba 8590 05d2 f02a 97ed 5ca2 1b10 5eb0  .......*..\...^.
+00004d30: 7612 45fd b615 127a 01e8 1102 0a44 79dd  v.E....z.....Dy.
+00004d40: 5f1e d25f 2c16 1493 a9c0 5541 b876 a390  _.._,.....UA.v..
+00004d50: 8421 0d2b a056 b454 b534 1cf7 6572 4f62  .!.+.V.T.4..erOb
+00004d60: 41b1 144a 2cf4 3116 45db 09ab 2705 c2e2  A..J,.1.E...'...
+00004d70: 5e7b 33ab 1358 a41c 6912 0fa3 6e70 8dd8  ^{3..X..i...np..
+00004d80: 388c c2b6 2964 882f 5d01 e1ad 9f2e 5da1  8...)d./].....].
+00004d90: 1415 cf49 9e09 c961 3bb6 da17 7834 619a  ...I...a;...x4a.
+00004da0: 480e a232 c135 8cda af57 71d0 8a17 485e  H..2.5...Wq...H^
+00004db0: 5565 0b86 5bc2 24e7 9451 bdb6 d30e 4f5e  Ue..[.$..Q....O^
+00004dc0: 80ec 6c25 603d 8237 e45d 4525 51e3 10c7  ..l%`=.7.]E%Q...
+00004dd0: ddbb 25e8 3e74 01a2 413b 6d27 7e5f 61b2  ..%.>t..A;m'~_a.
+00004de0: 7177 a4f4 9a11 37a1 384a cc6c db9b efda  qw....7.8J.l....
+00004df0: 21cc 1063 7384 afcc da6c 35de 34bd ab37  !..cs....l5.4..7
+00004e00: 1d77 17c3 f4b2 6a64 1e34 d58c d887 5bf3  .w....jd.4....[.
+00004e10: 2b29 5e9d bc40 a3b9 c8d7 1732 9042 9b4d  +)^..@.....2.B.M
+00004e20: 0854 8967 542a 7d8e 94be 4012 f42e 0e0d  .T.gT*}...@.....
+00004e30: 0af4 6bf8 5930 7133 0e09 63a0 0b14 b4c1  ..k.Y0q3..c.....
+00004e40: 94c3 2a08 f93e 0c6e 242a c7a1 7a57 2149  ..*..>.n$*..zW!I
+00004e50: c200 710c c5b0 625a d62f 9986 f7d8 cc11  ..q...bZ./......
+00004e60: 8d98 d297 66ea f6a5 3425 e585 34ff 72b2  ....f...4%..4.r.
+00004e70: 7803 a351 efa1 6937 82f1 cced a8a8 fdad  x..Q..i7........
+00004e80: c621 07a8 19d8 497a 0590 e3e2 d23e 85c1  .!....Iz.....>..
+00004e90: 1528 0174 01e0 d829 d8e6 73a4 08a3 069a  .(.t...)..s.....
+00004ea0: 11ec 271a 29c1 683e a38c d917 8343 9231  ..'.).h>.....C.1
+00004eb0: e956 5fdf c6b6 0dab 8a97 2277 65fd 5e04  .V_......."we.^.
+00004ec0: e2dc 78ab e2f5 62e1 8a3b 7571 1b44 d652  ..x...b..;uq.D.R
+00004ed0: 60e3 763e 6060 c303 bd2e c902 7860 1cfe  `.v>``......x`..
+00004ee0: b5e0 2da6 9d38 8276 2a08 7215 58ed 5460  ..-..8.v*.r.X.T`
+00004ef0: 6595 a25e 18fb 19bf 5476 bd24 2c96 c1cc  e..^....Tv.$,...
+00004f00: 385c c8d6 ec8d 93a2 4fce 0053 95c3 ad19  8\......O..S....
+00004f10: 98b6 fda0 033c c36a b7eb dd87 076d 9541  .....<.j.....m.A
+00004f20: c04e 32b4 6e40 51f9 ef70 61d6 cc2d 0337  .N2.n@Q..pa..-.7
+00004f30: 4bb7 2900 69cc 9690 c582 607d aeb4 5160  K.).i.....`}..Q`
+00004f40: 5054 dbd3 c876 9bfa ac62 86e1 be42 1523  PT...v...b...B.#
+00004f50: 3c37 1c60 10b9 a364 1b45 727b 6c14 a9a6  <7.`...d.Er{l...
+00004f60: 1754 69f1 d6bc 4c09 239a 7830 797e 2f99  .Ti...L.#.x0y~/.
+00004f70: d013 4990 e3fa b5a8 8cca e0d1 1cc9 ccd8  ..I.............
+00004f80: 4cff 3ca5 1e96 5830 6702 9660 034a 308e  L.<...X0g..`.J0.
+00004f90: 4e43 31ab 14d0 3ec9 5de5 3592 eb4c 30d1  NC1...>.].5..L0.
+00004fa0: b00d a086 0434 1e8f 687e dbd0 6b21 73e2  .....4..h~..k!s.
+00004fb0: c5fb 4139 0c00 a9bc 210b d363 7172 a9c1  ..A9....!..cqr..
+00004fc0: 28ff e568 7214 0f8c 42db 52a8 cf10 e0dd  (..hr...B.R.....
+00004fd0: b428 7506 3649 7be6 76a3 2875 009f 7264  .(u.6I{.v.(u..rd
+00004fe0: 8347 d727 7f03 eaae 94e9 7e6d 5151 1a14  .G.'......~mQQ..
+00004ff0: 1a16 afc5 b817 fbcd 0d10 6bd0 7d8c ab10  ..........k.}...
+00005000: c660 e82c 93de 239d 8701 9472 c3e0 3f2e  .`.,..#....r..?.
+00005010: 5e91 2590 c5b5 b744 7e55 30b2 dbb1 6759  ^.%....D~U0...gY
+00005020: 4e8f 92d1 d1ec 2879 f4d2 20ae 6ec0 92ff  N.....(y.. .n...
+00005030: 93fe eb98 b1e2 dfee f598 a382 1cbc 5c7e  ..............\~
+00005040: 74c0 7366 3f78 55ec eedd e951 9c9a 51c6  t.sf?xU....Q..Q.
+00005050: e966 98d0 6ab3 83ce f1ca 444e 4ea2 ef6c  .f..j.....DNN..l
+00005060: 0beb 89d9 82dd 0dee eddf e0a8 3958 a315  ............9X..
+00005070: 4e03 8c29 31bb fec1 06c9 a71a 743e d5a0  N..)1.......t>..
+00005080: bbbf 01e8 d1dd 24dd 4bad 5f7e a5c8 ade1  ......$.K._~....
+00005090: 6933 3e78 0a2a 0996 f5d7 acd3 49a3 2ceb  i3>x.*......I.,.
+000050a0: b67a d3fe 59ab 1b0d b3d6 e959 2769 9d0d  .z..Y......Y'i..
+000050b0: 9269 321c 747a 9d2c fb6d cbf7 7bb0 e7d7  .i2.tz.,.m..{...
+000050c0: dd72 7afa a38a d377 15f9 d113 c3af 6064  .rz....w......`d
+000050d0: ed5f 2b4d fa49 abdb 39ed b786 fdb3 6e6b  ._+M.I..9.....nk
+000050e0: 321b 0e7b e934 49b3 6ee7 376b 05ed 982d  2..{.4I.n.7k...-
+000050f0: 88ea 5918 0839 94ef 82dd c203 8fb6 c0ee  ..Y..9..........
+00005100: 4b3e 06f6 e1a3 35fa d51c 5c1e abd4 c14d  K>....5...\....M
+00005110: 5b04 ab3f 16fb cefd db75 389e b15f f336  [..?.....u8.._.6
+00005120: 1054 6419 ca22 d0b2 f733 f62d 7abe 4cec  .Td.."...3.-z.L.
+00005130: c74f c37e 7e3e 67ca 4648 2b71 734e 96e0  .O.~~>g.FH+qsN..
+00005140: b6fc 9dec 38b3 50f3 3382 787e 2bd6 5450  ....8.P.3.x~+.TP
+00005150: 9621 fd0a ccce bdf2 4b22 f796 5f10 698c  .!......K".._.i.
+00005160: efbd f6a7 d57c cec8 257d bf2d 0ad8 6933  .....|..%}.-..i3
+00005170: b425 2a7f a1b9 5eb9 9e49 3c74 3605 ddd6  .%*...^..I<t6...
+00005180: 3cd8 4b87 e960 100f ef57 408c 3ce8 0c5d  <.K..`...W@.<..]
+00005190: 0588 dcf6 954c 78b3 719c 9a3e 924b 4dc8  .....Lx.q..>.KM.
+000051a0: 87b9 4896 581a ace9 4b3e c29a 49fc 68d6  ..H.X...K>..I.h.
+000051b0: 9c80 fb81 9624 5058 c8c3 4dbf 1f8b 0f4f  .....$PX..M....O
+000051c0: 180f 2026 4dd2 dea0 1706 d8c4 a092 e79f  .. &M...........
+000051d0: 8cf7 9c0f d5f1 c155 c3db b2d9 0613 c87c  .......U.......|
+000051e0: 22ba 31c9 036f 7bd6 c55c 78dd b201 aa0b  ".1..o{..\x.....
+000051f0: 83ee 1a7c f5ae 5412 5b3a bddb e967 3a05  ...|..T.[:...g:.
+00005200: cfa3 10a2 06b4 f799 bf58 ef2a f9f6 19d6  .........X.*....
+00005210: c1ad 1192 edd9 a12d c21d 7680 5807 5d4b  .......-..v.X.]K
+00005220: 0278 7457 91f6 ba71 b7df 4f07 dee9 6c90  .xtW...q..O...l.
+00005230: 2c40 7962 5326 1f64 6e85 11f4 581a 7b24  ,@ybS&.dn...X.{$
+00005240: 2405 6361 f330 6e5c 05e5 2fd1 ad97 bbd5  $.ca.0n\../.....
+00005250: 30b7 a172 c3aa a0db 0be1 739d 7367 2b00  0..r......s.sg+.
+00005260: 73b3 4207 7791 cb38 fc81 4046 1431 c879  s.B.w..8..@F.1.y
+00005270: 890a 0cd3 39e5 5724 f759 363c 2ad0 7f84  ....9.W$.Y6<*...
+00005280: 7c4b f1d5 4ba0 2a27 bca6 27a8 a4fc c395  |K..K.*'..'.....
+00005290: 1a3a 8151 dd8c 8083 62bf 156e 187b f342  .:.Q....b..n.{.B
+000052a0: 8683 87bd a4a6 e005 64bf 808d 8b12 06a3  ........d.......
+000052b0: f812 5280 6c09 f939 930d 7c4c 262e de9f  ..R.l..9..|L&...
+000052c0: 894b 0fcb c41d 4ae8 fbd2 55ad be8f 4ebe  .K....J...U...N.
+000052d0: a4cc e8f0 9189 d16f 3c21 7a70 b60a 92e2  .......o<!zp....
+000052e0: 7050 a126 3e2f d4db 76b0 7c1d f1d0 33c9  pP.&>/..v.|...3.
+000052f0: ac7f 10e9 55df bc35 0886 cdd9 0434 db67  ....U..5.....4.g
+00005300: a540 bbdd 21c6 9c41 b658 913a 3fe4 b2c8  .@..!..A.X.:?...
+00005310: 109a 8b97 15d3 f4fc 9a01 b6b6 c00e 4edd  ..............N.
+00005320: 8656 c041 bdc7 2fcd f17d 7e7e f139 364b  .V.A../..}~~.96K
+00005330: 173f 489a 1bc2 73fe 74c3 c7fa baf1 0d8b  .?H...s.t.......
+00005340: 7c7f 827b 2835 faee 7fcf a64f ceb2 3fd3  |..{(5.....O..?.
+00005350: d6d7 738e f368 da6a 068c 96d2 f6d3 96ad  ..s..h.j........
+00005360: 3a25 fa86 104f 5573 f7e2 1d91 0de7 ec21  :%...OUs.......!
+00005370: 9f86 3304 3eef 6777 6e3c 673e 1189 7090  ..3.>.gwn<g>..p.
+00005380: e0b8 f7f3 ba35 cf40 dc3e 587d f61f 9c8b  .....5.@.>X}....
+00005390: 78cf 7f68 0412 0d20 16ce dbf7 3d0e c1e0  x..h... ....=...
+000053a0: be00 a319 a93c 1583 3e11 fec7 0418 4f07  .....<..>.....O.
+000053b0: 62c3 37db a19f 8f90 dc7f c137 7bea 8938  b.7........7{..8
+000053c0: b820 8df3 4f9b a9b4 27a1 f669 37de fb3f  . ..O...'..i7..?
+000053d0: 3d94 7f8e 6e20 f3e8 eec1 6c5f f778 c859  =...n ....l_.x.Y
+000053e0: 3cdb 6896 d1b7 9fa9 7acd 99cf 877b f0e7  <.h.....z....{..
+000053f0: 5495 a770 a67f a526 3ed2 8104 b5b3 a0fb  T..p...&>.......
+00005400: 7258 bdfe e9f0 2c8b a7ad 4eda 8313 c2b8  rX....,...N.....
+00005410: 9bb6 8651 3c6b 0dd2 691a 45c9 6030 c8a2  ...Q<k..i.E.`0..
+00005420: ed13 42d9 79f0 19e1 a01d 75b6 8f09 65c7  ..B.y.....u...e.
+00005430: dc10 4353 1828 dc4c 795d da4b 6871 1fe0  ..CS.(.Ly].Khq..
+00005440: 0297 cfa0 0eca 5fa1 89b2 93d8 8ac9 dabe  ......_.........
+00005450: 7a6f 5700 20cc ae71 8208 2e0d 1c03 4ccd  zoW. ..q......L.
+00005460: 0982 b9e1 04d9 999d c0ac be96 70c8 c9fc  ............p...
+00005470: 7cf9 8153 f96f 2f3d 72c8 352e 9744 f731  |..S.o/=r.5..D.1
+00005480: e403 dcdc 5252 ae2f 8986 0b54 4b1b 87ae  ....RR./...TK...
+00005490: 0882 3b1b 3348 b712 6923 ec12 4e0d 20a9  ..;.3H..i#..N. .
+000054a0: b5a4 5cd9 1b62 c726 f96f 6e11 1e0f c200  ..\..b.&.on.....
+000054b0: ae99 d9ff e642 9bad 70dd cd5b 2784 f499  .....B..p..['...
+000054c0: 91e2 5e36 b2e0 6355 e9b2 f63b 1f37 b1f9  ..^6..cU...;.7..
+000054d0: e636 e7c9 ef00 0000 ffff 0300 504b 0304  .6..........PK..
+000054e0: 1400 0600 0800 0000 2100 d52d 1831 9c04  ........!..-.1..
+000054f0: 0000 c225 0000 1400 0000 786c 2f63 6861  ...%......xl/cha
+00005500: 7274 732f 7374 796c 6531 2e78 6d6c ec5a  rts/style1.xml.Z
+00005510: 6d6f e238 10fe 2b91 7f40 03f4 6829 6a2a  mo.8..+..@..h)j*
+00005520: 755b ad74 12bd adf6 56ba cf26 71c0 bb8e  u[.t....V..&q...
+00005530: 9db3 cd52 faeb 6fec bc10 9384 972d d0c2  ...R..o......-..
+00005540: ed37 3c09 b6e7 99f1 33e3 99dc 866a 184e  .7<.....3....j.N
+00005550: b1d4 7feb 0523 de4b c238 0854 80a6 5aa7  .....#.K.8.T..Z.
+00005560: 43df 57e1 9424 585d 2434 9442 8958 5f84  C.W..$X]$4.B.X_.
+00005570: 22f1 451c d390 f891 c473 ca27 7eaf d3ed  ".E......s.'~...
+00005580: f9cb 5950 3e0d aecd 2252 c261 8958 c804  ..YP>..."R.a.X..
+00005590: 6b75 21e4 a498 2361 304b e7ca 4f30 e5c8  ku!...#a0K..O0..
+000055a0: a351 8060 5274 770b dbc3 2f54 7da3 9a11  .Q.`Rtw.../T}...
+000055b0: 3b62 fc2b 89e1 8597 0075 906f 4531 65ac  ;b.+.....u.oE1e.
+000055c0: 2624 714c 425d 7f57 f0a5 30a1 5c48 5804  &$qLB].W..0.\HX.
+000055d0: 0fad 9ae4 8149 ef27 6601 d22f 666d 3c64  .....I.'f../fm<d
+000055e0: b3e4 4944 99ec aadf e9d8 15ad f84b 1c67  ..ID.........K.g
+000055f0: e2cb 42ec 5766 b9bb f561 e371 b696 dd63  ..B.Wf...a.q...c
+00005600: 44e2 afcf d253 af01 ea9a 79bc 1f44 72f8  D....S....y..Dr.
+00005610: 0d4a 1b2d cceb ae9e 21d6 6422 e4e2 1eb4  .J.-....!.d"....
+00005620: 3f65 c555 fa2c 2d94 dc9b 07e8 a6df eb23  ?e.U.,-........#
+00005630: 2fc4 6980 6286 35fc 4c52 b0b5 e213 e461  /.i.b.5.LR.....a
+00005640: 3601 4442 9d5b 4430 1a7d 06cb 6e69 9e6e  6.DB.[D0.}..ni.n
+00005650: b379 062d e601 6355 1790 62c6 2363 0730  .y.-..cU..b.#c.0
+00005660: 2ecf cc91 6d1c ec52 31dd 4db3 e56a b6b2  ....m..R1.M..j..
+00005670: 67e1 5e12 ec25 2282 c384 1913 f3bf 8451  g.^..%"........Q
+00005680: e7cb 4f22 258d 08a8 6b65 23ca 4921 cbfc  ..O"%...ke#.I!..
+00005690: fd68 1e9e fb5d d54d 0b6b 39e0 ac1c 8ef1  .h...].M.k9.....
+000056a0: a46b 5d76 0542 760e 066e 3b9b a541 b3c3  .k]v.Bv..n;..A..
+000056b0: 8c35 1ee1 3101 df04 ff78 3746 ba6e 76f9  .5..1....x7F.nv.
+000056c0: dece 8cd4 e2d6 91a3 6639 7a30 9e3b d3c7  ........f9z0.;..
+000056d0: d33d fab1 6f36 dec6 cd99 6e71 734b 486b  .=..o6....nqsKHk
+000056e0: d8a9 69bb a54d dce0 515a 7025 7838 476b  ..i..M..QZp%x8Gk
+000056f0: 774e 02a7 1c8b 6801 f146 0a6d e2a4 a7d2  wN....h..F.m....
+00005700: f033 954a 8fb0 d2cf 5842 64ee 220f 9848  .3.J....XBd."..H
+00005710: 1bea 8981 8880 7819 4d91 3715 f275 5566  ......x.M.7..uUf
+00005720: de83 500e 4f90 3797 86bb d5bf 332c 09f2  ..P.O.7.....3,..
+00005730: d89f 1cd8 edf2 aa7f 7d85 3c6d 07dd 416f  ........}.<m..Ao
+00005740: 3040 9eac 3e19 579f 601e c254 19d1 7bd9  0@..>.W.`..T..{.
+00005750: e041 c338 b3b1 4aef 671a 8852 e7e4 94e9  .A.8..J.g..R....
+00005760: 9131 72a3 071a e1b3 a07c 3b7f cc53 0a65  .1r......|;..S.e
+00005770: 929d 32da 6358 b108 c279 2e61 9dfb cd29  ..2.cX...y.a...)
+00005780: c42a c19a 28ef eeb7 1c5d 3e6e 759e 3ed0  .*..(....]>nu.>.
+00005790: fef3 1d97 1a98 4056 d7c1 4ada e1b6 dc59  ......@V..J....Y
+000057a0: 4fe2 ecc9 03b0 f66e 0198 d34d 487a 83fe  O......n...MHz..
+000057b0: 7591 9148 1e65 c9e0 9ac3 9d4e c16d 9ac2  u..H.e.....N.m..
+000057c0: 5f6b 06e1 18bd 04a9 84ed 094b 4805 f707  _k.........KH...
+000057d0: dc06 c00f eadf 3574 6dba b789 2f5b 20ad  ......5tm.../[ .
+000057e0: d19e 0364 05b6 1528 4778 01d1 c953 8b64  ...d...(Gx...S.d
+000057f0: 2c20 950f a90c 1950 95a2 af24 40fd fcca  , .....P...$@...
+00005800: 50fe e71f 2a49 2c71 7282 ae5b c9a5 8fe0  P...*I,qr..[....
+00005810: b92e 5006 bf6f 787c da77 b282 09b8 4dcc  ..P..ox|.w....M.
+00005820: 81ac 4df2 7fbe b714 d766 9198 f34f b881  ..M......f...O..
+00005830: 780e 75a7 3669 d12f de38 f690 00b6 5f56  x.u.6i./.8...._V
+00005840: 36d1 d31e 6a01 ebd3 39cb 6b15 6b44 52a4  6...j...9.k.kDR.
+00005850: cdc1 f490 e58e 35a6 39f4 a128 4b28 6e72  ......5.9..(K(nr
+00005860: 5c16 5cd6 25c7 78b8 3ef0 56b1 848b b790  \.\.%.x.>.V.....
+00005870: 47f5 79e3 3bef 08ec 8e25 ab6d 6b22 c661  G.y.;....%.mk".a
+00005880: 1d2c e102 218e c824 1b50 75e8 dc9c ee52  .,..!..$.Pu....R
+00005890: d098 522c 373f 81ba 0c83 2cf6 097f ff40  ..R,7?....,....@
+000058a0: ea9c 6848 324e 5207 b494 98ca eb71 ab27  ..hH2NR......q.'
+000058b0: ef78 0e9b eb34 376f 2c4d 3a08 9778 4ee9  .x...47o,M:..xN.
+000058c0: 48fc afa2 c78e 55b0 5d48 cec5 92e0 88c8  H.....U.]H......
+000058d0: df81 3940 fb08 cc6c 054d 3221 3c3a 9306  ..9@...l.M2!<:..
+000058e0: 4f4b 3995 2d75 4c99 d027 d71e 307c 536c  OK9.-uL..'..0|Sl
+000058f0: dc5a aa18 5c3e 9e54 9ba3 aa47 5ec4 5244  .Z..\>.T...G^.RD
+00005900: 52a2 4ebd d5b6 b951 b5a2 6736 fc4d 69fb  R.N....Q..g6.Mi.
+00005910: a1b4 1534 f539 b5ac ff30 8dcf b16d 2554  ...4.9...0...m%T
+00005920: 1ad7 a6ad 6065 63ac 88c9 9cf3 9ebc 3961  ....`ec.......9a
+00005930: 4bf5 b504 6a37 4ff7 55e4 2cfa fe87 af0e  K...j7O.U.,.....
+00005940: 776f 3a7d 50dc f6ab df54 634b a1f7 f288  wo:}P....TcK....
+00005950: d534 fb66 402d d4a3 d079 15d9 ed37 5be8  .4.f@-...y...7[.
+00005960: 1cc0 4af8 3e40 c771 6fdf 40b4 84c8 065d  ..J.>@.qo.@....]
+00005970: 67e9 a954 a95a 1b86 6549 f157 4a4d 6ff9  g..T.Z..eI.WJMo.
+00005980: aea1 f1be bb04 143e 7599 91f3 0f7a ae9a  .......>u....z..
+00005990: 73e8 5e7f 988b e78e a58a 6cef 8622 961f  s.^.......l.."..
+000059a0: 5bdd fd07 0000 ffff 0300 504b 0304 1400  [.........PK....
+000059b0: 0600 0800 0000 2100 1c14 a7a8 fd00 0000  ......!.........
+000059c0: 6e03 0000 1500 0000 786c 2f63 6861 7274  n.......xl/chart
+000059d0: 732f 636f 6c6f 7273 312e 786d 6ca4 9341  s/colors1.xml..A
+000059e0: 6ec2 3010 45af 12f9 0071 1220 ad22 c2a6  n.0.E....q. ."..
+000059f0: eb8a 0527 184d 6c62 c9f6 20db a570 7b9c  ...'.Mlb.. ..p{.
+00005a00: 5068 4321 12c1 3bfb ebbf f97f 242f d157  PhC!..;.....$/.W
+00005a10: 489a dc26 1cb5 480e 46db f8e0 6bd6 86b0  H..&..H.F...k...
+00005a20: ab38 f7d8 0a03 3e35 0a1d 7992 2145 329c  .8....>5..y.!E2.
+00005a30: a454 2878 e3e0 5bd9 2d2f b2bc e0d8 820b  .T(x..[.-/......
+00005a40: 3d85 fd60 e01f 8576 c2c6 1192 9c81 e053  =..`...v.......S
+00005a50: 72db 0bc3 e848 c94a 6e40 5996 1811 da9a  r....H.Jn@Y.....
+00005a60: e111 b560 896a 6a96 676c b584 aa4f 233e  ...`.jj.gl...O#>
+00005a70: b44b f6a0 6b06 88c2 869c f187 5a31 a2cd  .K..k.......Z1..
+00005a80: 46b4 f988 b618 d1ca 4e8b 2bdd 8353 1014  F.......N.+..S..
+00005a90: d99b 6b17 547f 994f 6ace 0dca 2c9e cec3  ..k.T..Oj...,...
+00005aa0: ff9a 8688 5bcf fbc5 d3a3 d652 9e51 717d  ....[......R.Qq}
+00005ab0: d351 4f8c bf46 1e8e 9f4f 18bf 98e0 79bb  .QO..F...O....y.
+00005ac0: df7e f60a ea89 f6d7 c8c3 f68f 9a74 e4df  .~...........t..
+00005ad0: efb5 3a01 0000 ffff 0300 504b 0304 1400  ..:.......PK....
+00005ae0: 0600 0800 0000 2100 3b6d 324b c100 0000  ......!.;m2K....
+00005af0: 4201 0000 2300 0000 786c 2f77 6f72 6b73  B...#...xl/works
+00005b00: 6865 6574 732f 5f72 656c 732f 7368 6565  heets/_rels/shee
+00005b10: 7431 2e78 6d6c 2e72 656c 7384 8fc1 8ac2  t1.xml.rels.....
+00005b20: 3014 45f7 03fe 4378 7b93 d685 0c43 5337  0.E...Cx{....CS7
+00005b30: 22b8 55e7 0362 fada 06db 9790 f714 fd7b  ".U..b.........{
+00005b40: b31c 65c0 e5e5 70cf e536 9bfb 3ca9 1b66  ..e...p..6..<..f
+00005b50: 0e91 2cd4 ba02 85e4 6317 68b0 f07b da2d  ..,.....c.h..{.-
+00005b60: bf41 b138 eadc 1409 2d3c 9061 d32e be9a  .A.8....-<.a....
+00005b70: 034e 4e4a 89c7 9058 150b b185 5124 fd18  .NNJ...X....Q$..
+00005b80: c37e c4d9 b18e 09a9 903e e6d9 4989 7930  .~.......>..I.y0
+00005b90: c9f9 8b1b d0ac aa6a 6df2 5f07 b42f 4eb5  .......jm._../N.
+00005ba0: ef2c e47d 5783 3a3d 5259 feec 8e7d 1f3c  .,.}W.:=RY...}.<
+00005bb0: 6ea3 bfce 48f2 cf84 4939 9060 3ea2 4839  n...H...I9.`>.H9
+00005bc0: c845 edf2 8062 41eb 77f6 9e6b 7d0e 04a6  .E...bA.w..k}...
+00005bd0: 6dcc cbf3 f609 0000 ffff 0300 504b 0304  m...........PK..
+00005be0: 1400 0600 0800 0000 2100 1198 abc9 db00  ........!.......
+00005bf0: 0000 d001 0000 2300 0000 786c 2f77 6f72  ......#...xl/wor
+00005c00: 6b73 6865 6574 732f 5f72 656c 732f 7368  ksheets/_rels/sh
+00005c10: 6565 7432 2e78 6d6c 2e72 656c 73ac 91cd  eet2.xml.rels...
+00005c20: 4ec3 300c 80ef 48bc 43e4 3b49 db03 4268  N.0...H.C.;I..Bh
+00005c30: e92e 68d2 ae30 1e20 246e 1bd1 3a51 ec01  ..h..0. $n..:Q..
+00005c40: 7b7b c261 129d 2671 e1e6 1ff9 f367 79b3  {{.a..&q.....gy.
+00005c50: fd5a 66f5 8185 6322 0bad 6e40 21f9 1422  .Zf...c"..n@!.."
+00005c60: 8d16 5e0f bbbb 0750 2c8e 829b 13a1 8513  ..^....P,.......
+00005c70: 326c fbdb 9bcd 33ce 4eea 104f 31b3 aa14  2l....3.N..O1...
+00005c80: 620b 9348 7e34 86fd 848b 639d 3252 ed0c  b..H~4....c.2R..
+00005c90: a92c 4e6a 5a46 939d 7f77 239a ae69 ee4d  .,NjZF...w#..i.M
+00005ca0: f9cd 807e c554 fb60 a1ec 4307 ea70 ca75  ...~.T.`..C..p.u
+00005cb0: f3df ec34 0cd1 e353 f2c7 0549 aeac 30a1  ...4...S...I..0.
+00005cc0: b8cf 7a59 45ba 32a2 58d0 fa5c e373 d0ea  ..zYE.2.X..\.s..
+00005cd0: aa0c e6ba 4dfb 9f36 b944 122c 2f28 52a5  ....M..6.D.,/(R.
+00005ce0: 7865 75d1 3317 79a7 df22 fd48 9ad5 1ffa  xeu.3.y..".H....
+00005cf0: 6f00 0000 ffff 0300 504b 0304 1400 0600  o.......PK......
+00005d00: 0800 0000 2100 81c5 5ebd ca00 0000 3502  ....!...^.....5.
+00005d10: 0000 2300 0000 786c 2f64 7261 7769 6e67  ..#...xl/drawing
+00005d20: 732f 5f72 656c 732f 6472 6177 696e 6731  s/_rels/drawing1
+00005d30: 2e78 6d6c 2e72 656c 73bc 91cf 0ac2 300c  .xml.rels.....0.
+00005d40: 87ef 82ef 5072 b7dd 2688 88dd 2e22 7815  ....Pr..&...."x.
+00005d50: 7d80 d065 7f70 6b4b 5345 dfde 8208 0aa2  }..e.pkKSE......
+00005d60: 374f 2109 f97e 1f64 5d5d c741 5c28 70ef  7O!..~.d]].A\(p.
+00005d70: ac86 5c66 20c8 1a57 f7b6 d570 3c6c 674b  ..\f ..W...p<lgK
+00005d80: 101c d1d6 3838 4b1a 6ec4 5095 d3c9 7a4f  ....88K.n.P...zO
+00005d90: 03c6 74c4 5def 5924 8a65 0d5d 8c7e a514  ..t.].Y$.e.].~..
+00005da0: 9b8e 4664 e93c d9b4 695c 1831 a636 b4ca  ..Fd.<..i\.1.6..
+00005db0: a339 614b aac8 b285 0aaf 0c28 df98 6257  .9aK.......(..bW
+00005dc0: 6b08 bb7a 0ee2 70f3 29f9 37db 354d 6f68  k..z..p.).7.5Moh
+00005dd0: e3cc 7924 1b3f 4428 d361 8809 88a1 a5a8  ..y$.?D(.a......
+00005de0: 41ca c784 1f65 2e93 2ca8 cf1e c5ff 3c8a  A....e..,.....<.
+00005df0: 6f1e f9ff 3cf2 a787 7a7b 7679 0700 00ff  o...<...z{vy....
+00005e00: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00005e10: 0080 1bdc 81d2 0000 008f 0100 001f 0000  ................
+00005e20: 0078 6c2f 6368 6172 7473 2f5f 7265 6c73  .xl/charts/_rels
+00005e30: 2f63 6861 7274 332e 786d 6c2e 7265 6c73  /chart3.xml.rels
+00005e40: ac90 c14a c430 1086 ef82 ef10 e66e d3ec  ...J.0.......n..
+00005e50: 4144 36dd 8320 ec55 d707 08e9 b40d 9b64  AD6.. .U.......d
+00005e60: c24c 10fb f6a6 17b1 8b47 8f33 c3ff 7d3f  .L.......G.3..}?
+00005e70: 733c 7da5 a83e 9125 50b6 60ba 1e14 664f  s<}..>.%P.`...fO
+00005e80: 63c8 b385 8fcb ebc3 1328 a92e 8f2e 5246  c........(....RF
+00005e90: 0b2b 0a9c 86fb bbe3 1b46 575b 4896 5044  .+.......FW[H.PD
+00005ea0: 354a 160b 4bad e559 6bf1 0b26 271d 15cc  5J..K..Yk..&'...
+00005eb0: ed32 1127 57db c8b3 2ece 5fdd 8cfa d0f7  .2.'W....._.....
+00005ec0: 8f9a 7f33 60d8 31d5 79b4 c0e7 f100 eab2  ...3`.1.y.......
+00005ed0: 9666 be61 a7e0 9984 a6da 794a 9aa6 29f8  .f.a......yJ..).
+00005ee0: 8d6a cc9e aafd e2b8 be50 247e af6b c446  .j.......P$~.k.F
+00005ef0: 733c 63b5 e0b7 9d98 ae15 04fd b7db fc87  s<c.............
+00005f00: fb46 2b5b 8b1f abde bd71 f806 0000 ffff  .F+[.....q......
+00005f10: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00005f20: 9000 0db0 a601 0000 dd02 0000 0f00 0000  ................
+00005f30: 786c 2f6d 6574 6164 6174 612e 786d 6c64  xl/metadata.xmld
+00005f40: 514b 4f1b 3110 be57 e23f 58be 6fbc 2114  QKO.1..W.?X.o.!.
+00005f50: 42b4 bb28 02e5 4425 5428 ead5 b1c7 8955  B..(..D%T(.....U
+00005f60: bf64 7b69 5655 ff7b 67bd 8406 38d9 e319  .d{iVU.{g...8...
+00005f70: 7ff3 3d9a 9b83 35e4 0562 d2de b574 3eab  ..=...5..b...t>.
+00005f80: 2901 27bc d46e d7d2 1f4f 9b6a 4949 cadc  ).'..n...O.jII..
+00005f90: 496e bc83 960e 90e8 4d77 f6a5 b190 b9e4  In......Mw......
+00005fa0: 9913 0470 a9a5 fb9c c38a b124 f660 799a  ...p.......$.`y.
+00005fb0: f900 0e3b ca47 cb33 9671 c752 88c0 65da  ...;.G.3.q.R..e.
+00005fc0: 0364 6bd8 795d 5f32 cbb5 a313 c2ea 20f9  .dk.y]_2...... .
+00005fd0: 2714 ab45 f4c9 ab3c 13de 32af 9416 f009  '..E...<..2.....
+00005fe0: 677e c5e4 e038 cef2 18f9 40bb 376e 4f43  g~...8....@.7nOC
+00005ff0: 8044 84ef 5d46 6d1f 1a04 bfa0 a09f f777  .D..]Fm........w
+00006000: eb87 ef94 58ed 1efb 107c cc20 9fdf fc40  ....X....|. ...@
+00006010: 9635 5a22 7c18 4604 1278 cab0 36e6 7ff1  .5Z"|.F..x..6...
+00006020: cc4d 0fa8 1f9b 16e2 0e11 f196 82d1 79a3  .M............y.
+00006030: 632a 7b49 f4bf 6fbd 79dc 6b35 d5c2 008f  c*{I..o.y.k5....
+00006040: 9bc9 9a32 5f1e 6ebd b5e0 f284 c553 d2bb  ...2_.n......S..
+00006050: 3191 7139 4431 e10a 30e6 1b1a 3fbe b3ae  1.q9D1..0...?...
+00006060: 61c7 108a d0ae 517d ee23 8c03 2599 f702  a.....Q}.#..%...
+00006070: 4f6c d8fe ea1a 38e4 fb94 cb49 faa8 5bfa  Ol....8....I..[.
+00006080: 672b b7db a590 a252 7c0e d5c5 f525 547c  g+.....R|....%T|
+00006090: f9f5 aa5a 8885 5ad4 a23e bf16 8bbf 6822  ...Z..Z..>....h"
+000060a0: 06b5 7a35 7c3d 1afe 1031 ec98 355a adee  ..z5|=...1..5Z..
+000060b0: a620 0a6f 859a 0d0f 0964 4beb 4217 7722  . .o.....dK.B.w"
+000060c0: e9e3 6636 d260 ef39 77cd 5162 51f0 8173  ..f6.`.9w.QbQ..s
+000060d0: 1464 32f0 e588 5820 4ebf 9c98 d2fd 0300  .d2...X N.......
+000060e0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+000060f0: 0021 0035 85fa 75af 0100 003c 1000 0027  .!.5..u....<...'
+00006100: 0000 0078 6c2f 7072 696e 7465 7253 6574  ...xl/printerSet
+00006110: 7469 6e67 732f 7072 696e 7465 7253 6574  tings/printerSet
+00006120: 7469 6e67 7331 2e62 696e ec57 bd4a 0341  tings1.bin.W.J.A
+00006130: 10fe ee12 21f1 02b1 4861 6111 2b1b 0b85  ....!...Haa.+...
+00006140: 8096 9a68 a1a8 0731 42ca 8811 1424 8a49  ...h...1B....$.I
+00006150: 2f3e 839d e003 f80a be85 a520 d808 fa00  />......... ....
+00006160: b612 e7cb 65c9 bab7 7729 5444 d959 26fb  ....e...w)TD.Y&.
+00006170: 33b3 33b3 5fbe 62ae 867d 7470 2a5a 4603  3.3._.b..}tp*ZF.
+00006180: bb58 4205 0b32 cae8 e210 e738 96df 2e92  .XB..2.....8....
+00006190: c5cb 0685 47b4 8a99 a7cb 8c87 3cae 834a  ....G.......<..J
+000061a0: ae0d 0f25 efbd efcb 0c51 0fab 12f5 fb85  ...%.....Q......
+000061b0: d1fd 4106 6689 4bab 0854 37d7 b683 4264  ..A.f.K..T7...Bd
+000061c0: 9b09 8007 5952 95f0 5eae 0e64 7bc0 bc6c  ....YR..^..d{..l
+000061d0: 1aa2 ad10 783e 8bef 4d3f fabe 59fc d5b9  ....x>..M?..Y...
+000061e0: 8a67 fa35 fda6 3f8d 2aea 08b1 870d 6cc9  .g.5..?.*.....l.
+000061f0: 08b1 f303 088d 0fb9 8e03 1c0d 38d0 93ff  ............8...
+00006200: fa44 46c4 850e ee84 038b bf52 d357 934e  .DF........R.W.N
+00006210: cdfd c9b2 5dd1 0e01 8780 43c0 21e0 1088  ....].....C.!...
+00006220: 21c0 3e27 3354 1aa3 deca 0694 3ff0 7310  !.>'3T......?.s.
+00006230: 3a04 4608 e4a5 331f f187 5c32 252b 07ec  :.F...3...\2%+..
+00006240: 85c9 b192 2c38 536c 7d35 cf69 57bd b7e9  ....,8Sl}5.iW...
+00006250: d796 03e6 53fd 32ed e65e d510 7d21 24e7  ....S.2..^..}!$.
+00006260: 1996 812b b590 7965 32f2 e7dd 59ed 5c5f  ...+..ye2...Y.\_
+00006270: d2d6 ef7f 36ca b598 d8de 97f4 66fd 9d66  ....6.......f..f
+00006280: 6c13 5315 2329 968e 0d7d 2e0c d573 71fd  l.S.#)...}...sq.
+00006290: 2280 1bcf b1be 3cad f604 a852 31b1 61c6  ".....<....R1.a.
+000062a0: 5ac6 c984 e6a0 b0d1 f962 de7f 1dc6 b4e1  Z........b......
+000062b0: 9684 2d39 ab44 f128 adae 34ae d970 637c  ..-9.D.(..4..pc|
+000062c0: 7279 5c4c daf5 5a94 7fed 1f7f 5bdf 2fdf  ry\L..Z.....[./.
+000062d0: dc7e 0000 00ff ff03 0050 4b03 0414 0006  .~.......PK.....
+000062e0: 0008 0000 0021 0035 85fa 75af 0100 003c  .....!.5..u....<
+000062f0: 1000 0027 0000 0078 6c2f 7072 696e 7465  ...'...xl/printe
+00006300: 7253 6574 7469 6e67 732f 7072 696e 7465  rSettings/printe
+00006310: 7253 6574 7469 6e67 7332 2e62 696e ec57  rSettings2.bin.W
+00006320: bd4a 0341 10fe ee12 21f1 02b1 4861 6111  .J.A....!...Haa.
+00006330: 2b1b 0b85 8096 9a68 a1a8 0731 42ca 8811  +......h...1B...
+00006340: 1424 8a49 2f3e 839d e003 f80a be85 a520  .$.I/>......... 
+00006350: d808 fa00 b612 e7cb 65c9 bab7 7729 5444  ........e...w)TD
+00006360: d959 26fb 33b3 33b3 5fbe 62ae 867d 7470  .Y&.3.3._.b..}tp
+00006370: 2a5a 4603 bb58 4205 0b32 cae8 e210 e738  *ZF..XB..2.....8
+00006380: 96df 2e92 c5cb 0685 47b4 8a99 a7cb 8c87  ........G.......
+00006390: 3cae 834a ae0d 0f25 efbd efcb 0c51 0fab  <..J...%.....Q..
+000063a0: 12f5 fb85 d1fd 4106 6689 4bab 0854 37d7  ......A.f.K..T7.
+000063b0: b683 4264 9b09 8007 5952 95f0 5eae 0e64  ..Bd....YR..^..d
+000063c0: 7bc0 bc6c 1aa2 ad10 783e 8bef 4d3f fabe  {..l....x>..M?..
+000063d0: 59fc d5b9 8a67 fa35 fda6 3f8d 2aea 08b1  Y....g.5..?.*...
+000063e0: 870d 6cc9 08b1 f303 088d 0fb9 8e03 1c0d  ..l.............
+000063f0: 38d0 93ff fa44 46c4 850e ee84 038b bf52  8....DF........R
+00006400: d357 934e cdfd c9b2 5dd1 0e01 8780 43c0  .W.N....].....C.
+00006410: 21e0 1088 21c0 3e27 3354 1aa3 deca 0694  !...!.>'3T......
+00006420: 3ff0 7310 3a04 4608 e4a5 331f f187 5c32  ?.s.:.F...3...\2
+00006430: 252b 07ec 85c9 b192 2c38 536c 7d35 cf69  %+......,8Sl}5.i
+00006440: 57bd b7e9 d796 03e6 53fd 32ed e65e d510  W.......S.2..^..
+00006450: 7d21 24e7 1996 812b b590 7965 32f2 e7dd  }!$....+..ye2...
+00006460: 59ed 5c5f d2d6 ef7f 36ca b598 d8de 97f4  Y.\_....6.......
+00006470: 66fd 9d66 6c13 5315 2329 968e 0d7d 2e0c  f..fl.S.#)...}..
+00006480: d573 71fd 2280 1bcf b1be 3cad f604 a852  .sq.".....<....R
+00006490: 31b1 61c6 5ac6 c984 e6a0 b0d1 f962 de7f  1.a.Z........b..
+000064a0: 1dc6 b4e1 9684 2d39 ab44 f128 adae 34ae  ......-9.D.(..4.
+000064b0: d970 637c 7279 5c4c daf5 5a94 7fed 1f7f  .pc|ry\L..Z.....
+000064c0: 5bdf 2fdf dc7e 0000 00ff ff03 0050 4b03  [./..~.......PK.
+000064d0: 0414 0006 0008 0000 0021 00d1 f804 9032  .........!.....2
+000064e0: 0300 0008 1300 0010 0000 0078 6c2f 6361  ...........xl/ca
+000064f0: 6c63 4368 6169 6e2e 786d 6c7c 58cb 6edb  lcChain.xml|X.n.
+00006500: 400c bc17 e83f 08ba 378a d436 498b 3841  @....?..7..6I.8A
+00006510: f605 f4de 7e80 60ab b101 5b0e 2ca3 68ff  ....~.`...[.,.h.
+00006520: be9b 38e2 2e29 ce5e 0c98 a487 e4f0 b5f0  ..8..).^........
+00006530: fde3 dfc3 befa 339c a6dd 715c d5ed d575  ......3...q\...u
+00006540: 5d0d e3fa b8d9 8dcf abfa d7cf f0e9 aeae  ]...............
+00006550: a673 3f6e fafd 711c 56f5 bf61 aa1f 1f3e  .s?n..q.V..a...>
+00006560: 7eb8 5ff7 fbb5 ddf6 bbb1 8a08 e3b4 aab7  ~._.............
+00006570: e7f3 cbf7 a699 d6db e1d0 4f57 c797 618c  ..........OW..a.
+00006580: 9adf c7d3 a13f c7af a7e7 667a 390d fd66  .....?....fz9..f
+00006590: da0e c3f9 b06f baeb eb9b e610 01ea 87fb  .....o..........
+000065a0: 7575 5ad5 a66b eb6a b7aa a3c7 7d0c a5ae  uuZ..k.j....}...
+000065b0: fad7 cf66 a98d ce32 79fb 6dfe 15b7 4f72  ...f...2y.m...Or
+000065c0: 66ff d4bd 99df c6b4 384c 747b 712e 6048  f.......8Lt{q.`H
+000065d0: ceec ed57 06c3 6315 ca39 057b a3ba b631  ...W..c..9.{...1
+000065e0: 96e8 798e 4840 7125 415d a292 59d8 0b17  ..y.H@q%A]..Y...
+000065f0: 008a 2b09 aa8d 35cf fc27 c22f f2e8 4914  ..+...5..'./..I.
+00006600: 82e4 82c1 4ba8 af0d a394 afe5 dad9 4bd0  ....K.........K.
+00006610: cbf1 636e 05b2 7b2f 6744 796b 8ef4 7b3d  ..cn..{/gDyk..{=
+00006620: faf0 eeef 961a 28b4 3a67 8e2a c9d2 4c62  ......(.:g.*..Lb
+00006630: 96a5 d36b e84a 3514 ca39 7407 e229 d5d0  ...k.J5..9t..)..
+00006640: e935 74a0 86ae fd5c e82d a925 4e75 4602  .5t....\.-.%NuF.
+00006650: 6f79 b2d6 1909 2546 8492 a074 4642 8911  oy....%F...tFB..
+00006660: a14c fd82 fae2 d259 fa88 8496 6b67 b4a7  .L.....Y....kg..
+00006670: 594c c3a1 5364 748a 8c4e 9129 5124 94e4  YL..Sdt..N.)Q$..
+00006680: 58a7 c894 2812 4a82 4283 df7e 2934 8d11  X...(.J.B..~)4..
+00006690: da19 cdeb 8c24 311b 23af 33e2 4b8c 0825  .....$1.#.3.K..%
+000066a0: 39d6 19f1 2546 8492 a000 23be 3846 529b  9...%F....#.8FR.
+000066b0: 5613 25c9 364b e8c0 c474 faae 37f3 8aa4  V.%.6K...t..7...
+000066c0: c209 00b9 9f41 b701 782b e1ed fb1d 0657  .....A..x+.....W
+000066d0: 4468 699b 4918 575c 3d5c 4905 9020 be18  Dhi.I.W\=\I.. ..
+000066e0: 8bd4 26e6 698c 05f3 fa78 076a 786e cee7  ..&.i....x.jxn..
+000066f0: 20a1 d3cd 12e8 fa2d 0b9d 9e6c 2031 8701   ......-...l 1..
+00006700: d61d 0832 c9d9 8485 4edf 4536 ad38 e636  ...2....N.E6.8.6
+00006710: 93f3 874e 9a77 61af b363 d3ac 087b 3d2f  ...N.wa..c...{=/
+00006720: dbea 6c66 72f5 bd27 1f02 a6d3 17be a387  ..lfr..'........
+00006730: 43ea 54dd d22f 2c3d c0b4 0b4b 0b2c fde2  C.T../,=...K.,..
+00006740: 19e2 d133 6461 e980 a55d 585a 6069 1696  ...3da...]XZ`i..
+00006750: 065a eacd 68c4 e64b b743 9f30 030e a801  .Z..h..K.C.0....
+00006760: 55ce e4fc 3e80 aef3 e8fa 80ae f620 9e00  U...>........ ..
+00006770: f033 397f f6e9 c3e7 f419 7020 db4c ce67  .39.......p .L.g
+00006780: 15cc 4c00 ec7b 809f c979 f420 5b07 d80c  ..L..{...y. [...
+00006790: 003f 93f3 9904 cda3 4fbc d1b9 4c62 de09  .?......O...Lb..
+000067a0: e9d8 b17d e2c1 15f5 e0cc 3980 93c9 3967  ...}......9...9g
+000067b0: f01a 83f0 c11e 3660 0f9b 4edf 7b99 9c73  ......6`..N.{..s
+000067c0: 0cae 8803 9d9f c945 5efa e43a 70d7 ad5e  .......E^..:p..^
+000067d0: db24 16e8 6050 003b 0eb0 e300 3b99 5cf8  .$..`P.;....;.\.
+000067e0: 450f 0a3d 1e0f e2f1 e86a 8278 6c92 f3ab  E..=.....j.xl...
+000067f0: 09aa 65c1 15cf e402 47bf e21e a4a5 ef23  ..e.....G......#
+00006800: afd7 3089 45a7 81dd 0e3a c403 6e32 b998  ..0.E....:..n2..
+00006810: 68f0 12d0 73b2 e09d 01e6 d982 bd60 97f3  h...s........`..
+00006820: dcd0 7f58 0fff 0100 00ff ff03 0050 4b03  ...X.........PK.
+00006830: 0414 0006 0008 0000 0021 0029 11c7 524c  .........!.)..RL
+00006840: 0100 0069 0200 0011 0008 0164 6f63 5072  ...i.......docPr
+00006850: 6f70 732f 636f 7265 2e78 6d6c 20a2 0401  ops/core.xml ...
+00006860: 28a0 0001 0000 0000 0000 0000 0000 0000  (...............
+00006870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000068a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000068b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000068c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000068d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000068e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000068f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006960: 0000 0000 7c92 5f4b c330 14c5 df05 bf43  ....|._K.0.....C
+00006970: c97b 9b76 eba6 2b6d 072a f3c5 8160 45f1  .{.v..+m.*...`E.
+00006980: 2d24 775b b0f9 4312 edfa ed4d bbad 5627  -$w[..C....M..V'
+00006990: 3e26 e7dc 5fce b924 5fee 451d 7c82 b15c  >&.._..$_.E.|..\
+000069a0: c902 2551 8c02 9054 312e b705 7aae 56e1  ..%Q...T1...z.V.
+000069b0: 350a ac23 9291 5a49 2850 0b16 2dcb cb8b  5..#..ZI(P..-...
+000069c0: 9cea 8c2a 038f 4669 308e 830d 3c49 da8c  ...*..Fi0...<I..
+000069d0: ea02 ed9c d319 c696 ee40 101b 7987 f4e2  .........@..y...
+000069e0: 4619 419c 3f9a 2dd6 84be 932d e049 1ccf  F.A.?.-....-.I..
+000069f0: b100 4718 7104 77c0 500f 4474 4432 3a20  ..G.q.w.P.DtD2: 
+00006a00: f587 a97b 00a3 186a 1020 9dc5 4994 e06f  ...{...j. ..I..o
+00006a10: af03 23ec 9f03 bd32 720a ee5a ed3b 1de3  ..#....2r..Z.;..
+00006a20: 8ed9 8c1e c4c1 bdb7 7c30 364d 1335 d33e  ........|06M.5.>
+00006a30: 86cf 9fe0 d7f5 c353 5f35 e4b2 db15 0554  .......S_5.....T
+00006a40: e68c 66d4 0071 ca94 f7bc aefd 7ed6 aab5  ..f..q......~...
+00006a50: 90e3 91d0 2db1 26d6 adfd be37 1cd8 4dfb  ....-.&....7..M.
+00006a60: cb7b ae7b 6e5f e300 0716 f860 d9a1 c649  .{.{n_.....`...I
+00006a70: 7999 dede 552b 544e e2c9 348c 1761 7c55  y...U+TN..4..a|U
+00006a80: 258b 2c9d 6569 fad6 3dff 63be 0b7a b810  %.,.ei..=.c..z..
+00006a90: c710 ff13 d330 9e85 f1bc 4a3a 5c96 cc46  .....0....J:\..F
+00006aa0: c413 a0cc f1d9 e728 bf00 0000 ffff 0300  .......(........
+00006ab0: 504b 0304 1400 0600 0800 0000 2100 380c  PK..........!.8.
+00006ac0: a0e5 0902 0000 3205 0000 1000 0801 646f  ......2.......do
+00006ad0: 6350 726f 7073 2f61 7070 2e78 6d6c 20a2  cProps/app.xml .
+00006ae0: 0401 28a0 0001 0000 0000 0000 0000 0000  ..(.............
 00006af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006ba0: 0000 0000 0000 007c 925f 4f83 3014 c5df  .......|._O.0...
-00006bb0: 4dfc 0ea4 efd0 f247 dd1a 6089 9af9 e212  M......G..`.....
-00006bc0: 1331 1adf 9af6 6e23 4269 da2a f2ed 2db0  .1....n#Bi.*..-.
-00006bd0: 213a e363 7bce fdf5 9c9b a6ab cfba f23e  !:.c{..........>
-00006be0: 409b b291 190a 0382 3c90 bc11 a5dc 65e8  @.......<.....e.
-00006bf0: a958 fb0b e419 cba4 6055 2321 431d 18b4  .X......`U#!C...
-00006c00: cacf cf52 ae28 6f34 3ce8 4681 b625 18cf  ...R.(o4<.F..%..
-00006c10: 91a4 a15c 6568 6fad a218 1bbe 879a 99c0  ...\eho.........
-00006c20: 39a4 13b7 8dae 9975 47bd c38a f137 b603  9......uG....7..
-00006c30: 1c11 7289 6bb0 4c30 cb70 0ff4 d544 4407  ..r.k.L0.p...DD.
-00006c40: a4e0 1352 bdeb 6a00 088e a182 1aa4 3538  ...R..j.......58
-00006c50: 0c42 fced b5a0 6bf3 e7c0 a0cc 9c75 693b  .B....k......ui;
-00006c60: e53a 1de2 ced9 828f e2e4 fe34 e564 6cdb  .:.........4.dl.
-00006c70: 3668 e321 86cb 1fe2 97cd fde3 50d5 2f65  6h.!........P./e
-00006c80: bf2b 0e28 4f05 a75c 03b3 8dce efca aa72  .+.(O..\.......r
-00006c90: fbd9 349d 8114 cf84 7e89 1533 76e3 f6bd  ..4.....~..3v...
-00006ca0: 2d41 5c77 bfbc a7ba e30e 3546 3808 cf05  -A\w......5F8...
-00006cb0: a363 8da3 f21c dfdc 166b 9447 248a 7db2  .c.......k.G$.}.
-00006cc0: f4c9 5511 2e69 7241 93e4 b57f fec7 7c1f  ..U..irA......|.
-00006cd0: 74bc a80f 21fe 2726 3e89 fd88 14e1 8246  t...!.'&>......F
-00006ce0: 84c6 8b19 f108 c853 7cf2 39f2 2f00 0000  .......S|.9./...
-00006cf0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00006d00: 2100 380c a0e5 0902 0000 3205 0000 1000  !.8.......2.....
-00006d10: 0801 646f 6350 726f 7073 2f61 7070 2e78  ..docProps/app.x
-00006d20: 6d6c 20a2 0401 28a0 0001 0000 0000 0000  ml ...(.........
-00006d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006e20: 0000 0000 0000 0000 0000 9c54 516f 9b30  ...........TQo.0
-00006e30: 107e 9fb4 ff80 786f 206b d44d 91a1 a284  .~....xo k.M....
-00006e40: 2a55 69c8 02a4 d25e 22cf 1c89 55b0 91ed  *Ui....^"...U...
-00006e50: 46c9 7efd 4c50 12d2 3993 b6b7 f37d 77df  F.~.LP..9....}w.
-00006e60: 7d77 ba33 badf d595 b505 2129 679e 3d1c  }w.3......!)g.=.
-00006e70: b8b6 058c f082 b2b5 67e7 d9e3 cd37 db92  ........g....7..
-00006e80: 0ab3 0257 9c81 67ef 41da f7fe e74f 682e  ...W..g.A....Oh.
-00006e90: 7803 4251 9096 a660 d2b3 374a 3563 c791  x.BQ...`..7J5c..
-00006ea0: 6403 3596 030d 338d 945c d458 e9a7 583b  d.5...3..\.X..X;
-00006eb0: bc2c 2981 0927 ef35 30e5 7c71 dd3b 0776  .,)..'.50.|q.;.v
-00006ec0: 0a58 01c5 4d73 22b4 3bc6 f156 fd2f 69c1  .X..Ms".;..V./i.
-00006ed0: 49ab 4f2e b37d a305 fb28 689a 8a12 ac74  I.O..}...(h....t
-00006ee0: 97fe 0b25 824b 5e2a 2bda 11a8 90d3 0791  ...%.K^*+.......
-00006ef0: 5697 0279 1754 ed7d 1739 fd27 4a09 ae20  V..y.T.}.9.'J.. 
-00006f00: d4c4 7e89 2b09 c839 3bd0 1470 3bb4 39a6  ..~.+..9;..p;.9.
-00006f10: 42fa 68ab c65b 208a 0b4b d25f 7a6c 23db  B.h..[ ..K._zl#.
-00006f20: fa89 25b4 723c 7b8b 05c5 4c69 596d 58f7  ..%.r<{...LiYmX.
-00006f30: 38d8 5523 95f0 5fb9 7893 1b00 2591 a303  8.U#.._.x...%...
-00006f40: 3ae7 c1ec c7f6 6d3a f26f 0f01 daf8 6b60  :.....m:.o....k`
-00006f50: c735 c335 14d6 02b3 35fc 4b89 e1c8 5ca3  .5.5....5.K...\.
-00006f60: 15d9 35ab 8b5f 8e21 a3aa 0299 9473 2c94  ..5.._.!.....s,.
-00006f70: 612a c3af fdb1 1cc4 7543 e974 46bb 46cf  a*......uC.tF.F.
-00006f80: f83c 8293 952a bd51 4644 17c2 b519 7a88  .<...*.QFD....z.
-00006f90: 93f0 7995 3efd 888c 99e1 349f 3daf c224  ..y.>.....4.=..$
-00006fa0: 36a3 499a 1981 49be 08b2 a764 6604 a365  6.I...I....df..e
-00006fb0: 10af 823c 4b8c e863 1066 570b 4e83 38ce  ...<K..c.fW.N.8.
-00006fc0: 5363 de34 0a26 d1e2 7a27 71fc 7295 76f6  Sc.4.&..z'q.r.v.
-00006fd0: b06a cb9a 8935 a873 af62 dff3 286d 5bbd  .j...5.s.b..(m[.
-00006fe0: 1ab0 485e cdd8 31f3 a3ac 8bcd f9b0 2b31  ..H^..1.......+1
-00006ff0: 656f 326f 323e c10a 8ef7 76e9 44e9 060b  eo2o2>....v.D...
-00007000: 28f4 899e eef1 e440 537d 6aa2 6a49 c24d  (......@S}j.jI.M
-00007010: bbe9 c531 e64f a0fd 1d96 dd17 e80f ef06  ...1.O..........
-00007020: eead ab0f bfe7 43ce f9b3 f37f 0300 00ff  ......C.........
-00007030: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00007040: 00ef 73f2 1436 0100 00a1 0200 002d 0000  ..s..6.......-..
-00007050: 0078 6c2f 6578 7465 726e 616c 4c69 6e6b  .xl/externalLink
-00007060: 732f 5f72 656c 732f 6578 7465 726e 616c  s/_rels/external
-00007070: 4c69 6e6b 312e 786d 6c2e 7265 6c73 bc92  Link1.xml.rels..
-00007080: 4d6b 0231 1086 ef85 fe87 2577 1df5 508a  Mk.1......%w..P.
-00007090: b87a b02d 080a 6dd1 dbc2 12b2 b3bb a9d9  .z.-..m.........
-000070a0: 2464 c676 fdf7 1dfa 01b5 15bc f598 64f2  $d.v..........d.
-000070b0: cc3c 6f32 5bf4 9dcb 5e31 910d 3e57 e3e1  .<o2[...^1..>W..
-000070c0: 4865 e84d a8ac 6f72 b5db 3e0c 6e55 46ac  He.M..or..>.nUF.
-000070d0: 7da5 5df0 98ab 2392 5acc afaf 66cf e834  }.]...#.Z...f..4
-000070e0: cb25 6a6d a44c 289e 72d5 32c7 2900 9916  .%jm.L(.r.2.)...
-000070f0: 3b4d c310 d1cb 491d 52a7 5996 a981 a8cd  ;M....I.R.Y.....
-00007100: 5e37 0893 d1e8 06d2 4f86 9a9f 30b3 5595  ^7......O...0.U.
-00007110: abb4 aa26 2adb 1ea3 74be cc0e 756d 0dde  ...&*...t...um..
-00007120: 0573 e8d0 f399 1680 3d63 f2da adad df3f  .s......=c.....?
-00007130: 6a6e 85ad 5383 9cab da3a 94c9 6139 2d76  jn..S....:..a9-v
-00007140: 2471 148d 750e a94c 682c 6b57 5038 2483  $q..u..Lh,kWP8$.
-00007150: 45c2 18a8 48ba 61db e120 a6f0 8286 a978  E...H.a.. .....x
-00007160: 6b35 9755 28d7 eb4d c9ad c0a5 900a 8a09  k5.U(..M........
-00007170: 7545 2d22 978c 5d94 c064 77b3 7c1a f68e  uE-"..]..dw.|...
-00007180: faef de9b 5089 ddfd d764 0ace c730 fe9f  ....P....d...0..
-00007190: 18e0 431e 4ee5 e153 5e9e 4be4 e1b7 3cfc  ..C.N..S^.K...<.
-000071a0: 9197 4282 b3f2 7059 1e4e 3ed6 fc1d 0000  ..B...pY.N>.....
-000071b0: ffff 0300 504b 0102 2d00 1400 0600 0800  ....PK..-.......
-000071c0: 0000 2100 7fd5 effa f201 0000 640a 0000  ..!.........d...
-000071d0: 1300 0000 0000 0000 0000 0000 0000 0000  ................
-000071e0: 0000 5b43 6f6e 7465 6e74 5f54 7970 6573  ..[Content_Types
-000071f0: 5d2e 786d 6c50 4b01 022d 0014 0006 0008  ].xmlPK..-......
-00007200: 0000 0021 00b5 5530 23f4 0000 004c 0200  ...!..U0#....L..
-00007210: 000b 0000 0000 0000 0000 0000 0000 002b  ...............+
-00007220: 0400 005f 7265 6c73 2f2e 7265 6c73 504b  ..._rels/.relsPK
-00007230: 0102 2d00 1400 0600 0800 0000 2100 d865  ..-.........!..e
-00007240: bac6 9e04 0000 0c0d 0000 0f00 0000 0000  ................
-00007250: 0000 0000 0000 0000 5007 0000 786c 2f77  ........P...xl/w
-00007260: 6f72 6b62 6f6f 6b2e 786d 6c50 4b01 022d  orkbook.xmlPK..-
-00007270: 0014 0006 0008 0000 0021 0032 8573 9f3a  .........!.2.s.:
-00007280: 0100 007b 0500 001a 0000 0000 0000 0000  ...{............
-00007290: 0000 0000 001b 0c00 0078 6c2f 5f72 656c  .........xl/_rel
-000072a0: 732f 776f 726b 626f 6f6b 2e78 6d6c 2e72  s/workbook.xml.r
-000072b0: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
-000072c0: 0021 001b 2784 8817 0600 0025 1200 0018  .!..'......%....
-000072d0: 0000 0000 0000 0000 0000 0000 0095 0e00  ................
-000072e0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-000072f0: 6865 6574 312e 786d 6c50 4b01 022d 0014  heet1.xmlPK..-..
-00007300: 0006 0008 0000 0021 009e d33f 9dcb 0b00  .......!...?....
-00007310: 005c 5500 0018 0000 0000 0000 0000 0000  .\U.............
-00007320: 0000 00e2 1400 0078 6c2f 776f 726b 7368  .......xl/worksh
-00007330: 6565 7473 2f73 6865 6574 322e 786d 6c50  eets/sheet2.xmlP
-00007340: 4b01 022d 0014 0006 0008 0000 0021 0087  K..-.........!..
-00007350: 7b5f d3f5 0400 00ca 1000 0018 0000 0000  {_..............
-00007360: 0000 0000 0000 0000 00e3 2000 0078 6c2f  .......... ..xl/
-00007370: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00007380: 332e 786d 6c50 4b01 022d 0014 0006 0008  3.xmlPK..-......
-00007390: 0000 0021 00b1 450d ec5c 0700 0002 2100  ...!..E..\....!.
-000073a0: 0013 0000 0000 0000 0000 0000 0000 000e  ................
-000073b0: 2600 0078 6c2f 7468 656d 652f 7468 656d  &..xl/theme/them
-000073c0: 6531 2e78 6d6c 504b 0102 2d00 1400 0600  e1.xmlPK..-.....
-000073d0: 0800 0000 2100 78b9 1e89 d405 0000 6e1a  ....!.x.......n.
-000073e0: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
-000073f0: 9b2d 0000 786c 2f73 7479 6c65 732e 786d  .-..xl/styles.xm
-00007400: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00007410: 00fa 1fae 0bc1 0300 00ba 0c00 0014 0000  ................
-00007420: 0000 0000 0000 0000 0000 009a 3300 0078  ............3..x
-00007430: 6c2f 7368 6172 6564 5374 7269 6e67 732e  l/sharedStrings.
-00007440: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-00007450: 0021 00ac d4f4 abdb 0200 003b 0d00 0018  .!.........;....
-00007460: 0000 0000 0000 0000 0000 0000 008d 3700  ..............7.
-00007470: 0078 6c2f 6472 6177 696e 6773 2f64 7261  .xl/drawings/dra
-00007480: 7769 6e67 312e 786d 6c50 4b01 022d 0014  wing1.xmlPK..-..
-00007490: 0006 0008 0000 0021 00be cf15 7fd7 0800  .......!........
-000074a0: 0084 3f00 0014 0000 0000 0000 0000 0000  ..?.............
-000074b0: 0000 009e 3a00 0078 6c2f 6368 6172 7473  ....:..xl/charts
-000074c0: 2f63 6861 7274 312e 786d 6c50 4b01 022d  /chart1.xmlPK..-
-000074d0: 0014 0006 0008 0000 0021 0041 9287 f0fd  .........!.A....
-000074e0: 0800 0001 3300 0014 0000 0000 0000 0000  ....3...........
-000074f0: 0000 0000 00a7 4300 0078 6c2f 6368 6172  ......C..xl/char
-00007500: 7473 2f63 6861 7274 322e 786d 6c50 4b01  ts/chart2.xmlPK.
-00007510: 022d 0014 0006 0008 0000 0021 00bc 8d4e  .-.........!...N
-00007520: cc4f 0800 0015 2a00 0014 0000 0000 0000  .O....*.........
-00007530: 0000 0000 0000 00d6 4c00 0078 6c2f 6368  ........L..xl/ch
-00007540: 6172 7473 2f63 6861 7274 332e 786d 6c50  arts/chart3.xmlP
-00007550: 4b01 022d 0014 0006 0008 0000 0021 00d5  K..-.........!..
-00007560: 2d18 319c 0400 00c2 2500 0014 0000 0000  -.1.....%.......
-00007570: 0000 0000 0000 0000 0057 5500 0078 6c2f  .........WU..xl/
-00007580: 6368 6172 7473 2f73 7479 6c65 312e 786d  charts/style1.xm
-00007590: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-000075a0: 001c 14a7 a8fd 0000 006e 0300 0015 0000  .........n......
-000075b0: 0000 0000 0000 0000 0000 0025 5a00 0078  ...........%Z..x
-000075c0: 6c2f 6368 6172 7473 2f63 6f6c 6f72 7331  l/charts/colors1
-000075d0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-000075e0: 0000 2100 3b6d 324b c100 0000 4201 0000  ..!.;m2K....B...
-000075f0: 2300 0000 0000 0000 0000 0000 0000 555b  #.............U[
-00007600: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00007610: 5f72 656c 732f 7368 6565 7431 2e78 6d6c  _rels/sheet1.xml
-00007620: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
-00007630: 0000 0021 0011 98ab c9db 0000 00d0 0100  ...!............
-00007640: 0023 0000 0000 0000 0000 0000 0000 0057  .#.............W
-00007650: 5c00 0078 6c2f 776f 726b 7368 6565 7473  \..xl/worksheets
-00007660: 2f5f 7265 6c73 2f73 6865 6574 322e 786d  /_rels/sheet2.xm
-00007670: 6c2e 7265 6c73 504b 0102 2d00 1400 0600  l.relsPK..-.....
-00007680: 0800 0000 2100 81c5 5ebd ca00 0000 3502  ....!...^.....5.
-00007690: 0000 2300 0000 0000 0000 0000 0000 0000  ..#.............
-000076a0: 735d 0000 786c 2f64 7261 7769 6e67 732f  s]..xl/drawings/
-000076b0: 5f72 656c 732f 6472 6177 696e 6731 2e78  _rels/drawing1.x
-000076c0: 6d6c 2e72 656c 7350 4b01 022d 0014 0006  ml.relsPK..-....
-000076d0: 0008 0000 0021 0080 1bdc 81d2 0000 008f  .....!..........
-000076e0: 0100 001f 0000 0000 0000 0000 0000 0000  ................
-000076f0: 007e 5e00 0078 6c2f 6368 6172 7473 2f5f  .~^..xl/charts/_
-00007700: 7265 6c73 2f63 6861 7274 332e 786d 6c2e  rels/chart3.xml.
-00007710: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
-00007720: 0000 2100 a5bb 4927 7401 0000 4b03 0000  ..!...I't...K...
-00007730: 2200 0000 0000 0000 0000 0000 0000 8d5f  ".............._
-00007740: 0000 786c 2f65 7874 6572 6e61 6c4c 696e  ..xl/externalLin
-00007750: 6b73 2f65 7874 6572 6e61 6c4c 696e 6b31  ks/externalLink1
-00007760: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-00007770: 0000 2100 9000 0db0 a601 0000 dd02 0000  ..!.............
-00007780: 0f00 0000 0000 0000 0000 0000 0000 4161  ..............Aa
-00007790: 0000 786c 2f6d 6574 6164 6174 612e 786d  ..xl/metadata.xm
-000077a0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-000077b0: 0035 85fa 75af 0100 003c 1000 0027 0000  .5..u....<...'..
-000077c0: 0000 0000 0000 0000 0000 0014 6300 0078  ............c..x
-000077d0: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
-000077e0: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
-000077f0: 7331 2e62 696e 504b 0102 2d00 1400 0600  s1.binPK..-.....
-00007800: 0800 0000 2100 3585 fa75 af01 0000 3c10  ....!.5..u....<.
-00007810: 0000 2700 0000 0000 0000 0000 0000 0000  ..'.............
-00007820: 0865 0000 786c 2f70 7269 6e74 6572 5365  .e..xl/printerSe
-00007830: 7474 696e 6773 2f70 7269 6e74 6572 5365  ttings/printerSe
-00007840: 7474 696e 6773 322e 6269 6e50 4b01 022d  ttings2.binPK..-
-00007850: 0014 0006 0008 0000 0021 0008 f55e 1146  .........!...^.F
-00007860: 0300 005e 1300 0010 0000 0000 0000 0000  ...^............
-00007870: 0000 0000 00fc 6600 0078 6c2f 6361 6c63  ......f..xl/calc
-00007880: 4368 6169 6e2e 786d 6c50 4b01 022d 0014  Chain.xmlPK..-..
-00007890: 0006 0008 0000 0021 00a3 290c 194d 0100  .......!..)..M..
-000078a0: 0069 0200 0011 0000 0000 0000 0000 0000  .i..............
-000078b0: 0000 0070 6a00 0064 6f63 5072 6f70 732f  ...pj..docProps/
-000078c0: 636f 7265 2e78 6d6c 504b 0102 2d00 1400  core.xmlPK..-...
-000078d0: 0600 0800 0000 2100 380c a0e5 0902 0000  ......!.8.......
-000078e0: 3205 0000 1000 0000 0000 0000 0000 0000  2...............
-000078f0: 0000 f46c 0000 646f 6350 726f 7073 2f61  ...l..docProps/a
-00007900: 7070 2e78 6d6c 504b 0102 2d00 1400 0600  pp.xmlPK..-.....
-00007910: 0800 0000 2100 ef73 f214 3601 0000 a102  ....!..s..6.....
-00007920: 0000 2d00 0000 0000 0000 0000 0000 0000  ..-.............
-00007930: 3370 0000 786c 2f65 7874 6572 6e61 6c4c  3p..xl/externalL
-00007940: 696e 6b73 2f5f 7265 6c73 2f65 7874 6572  inks/_rels/exter
-00007950: 6e61 6c4c 696e 6b31 2e78 6d6c 2e72 656c  nalLink1.xml.rel
-00007960: 7350 4b05 0600 0000 001c 001c 00ad 0700  sPK.............
-00007970: 00b4 7100 0000 00                        ..q....
+00006ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006be0: 0000 0000 0000 9c54 516f 9b30 107e 9fb4  .......TQo.0.~..
+00006bf0: ff80 786f 206b d44d 91a1 a284 2a55 69c8  ..xo k.M....*Ui.
+00006c00: 02a4 d25e 22cf 1c89 55b0 91ed 46c9 7efd  ...^"...U...F.~.
+00006c10: 4c50 12d2 3993 b6b7 f37d 77df 7d77 ba33  LP..9....}w.}w.3
+00006c20: badf d595 b505 2129 679e 3d1c b8b6 058c  ......!)g.=.....
+00006c30: f082 b2b5 67e7 d9e3 cd37 db92 0ab3 0257  ....g....7.....W
+00006c40: 9c81 67ef 41da f7fe e74f 682e 7803 4251  ..g.A....Oh.x.BQ
+00006c50: 9096 a660 d2b3 374a 3563 c791 6403 3596  ...`..7J5c..d.5.
+00006c60: 030d 338d 945c d458 e9a7 583b bc2c 2981  ..3..\.X..X;.,).
+00006c70: 0927 ef35 30e5 7c71 dd3b 0776 0a58 01c5  .'.50.|q.;.v.X..
+00006c80: 4d73 22b4 3bc6 f156 fd2f 69c1 49ab 4f2e  Ms".;..V./i.I.O.
+00006c90: b37d a305 fb28 689a 8a12 ac74 97fe 0b25  .}...(h....t...%
+00006ca0: 824b 5e2a 2bda 11a8 90d3 0791 5697 0279  .K^*+.......V..y
+00006cb0: 1754 ed7d 1739 fd27 4a09 ae20 d4c4 7e89  .T.}.9.'J.. ..~.
+00006cc0: 2b09 c839 3bd0 1470 3bb4 39a6 42fa 68ab  +..9;..p;.9.B.h.
+00006cd0: c65b 208a 0b4b d25f 7a6c 23db fa89 25b4  .[ ..K._zl#...%.
+00006ce0: 723c 7b8b 05c5 4c69 596d 58f7 38d8 5523  r<{...LiYmX.8.U#
+00006cf0: 95f0 5fb9 7893 1b00 2591 a303 3ae7 c1ec  .._.x...%...:...
+00006d00: c7f6 6d3a f26f 0f01 daf8 6b60 c735 c335  ..m:.o....k`.5.5
+00006d10: 14d6 02b3 35fc 4b89 e1c8 5ca3 15d9 35ab  ....5.K...\...5.
+00006d20: 8b5f 8e21 a3aa 0299 9473 2c94 612a c3af  ._.!.....s,.a*..
+00006d30: fdb1 1cc4 7543 e974 46bb 46cf f83c 8293  ....uC.tF.F..<..
+00006d40: 952a bd51 4644 17c2 b519 7a88 93f0 7995  .*.QFD....z...y.
+00006d50: 3efd 888c 99e1 349f 3daf c224 36a3 499a  >.....4.=..$6.I.
+00006d60: 1981 49be 08b2 a764 6604 a365 10af 823c  ..I....df..e...<
+00006d70: 4b8c e863 1066 570b 4e83 38ce 5363 de34  K..c.fW.N.8.Sc.4
+00006d80: 0a26 d1e2 7a27 71fc 7295 76f6 b06a cb9a  .&..z'q.r.v..j..
+00006d90: 8935 a873 af62 dff3 286d 5bbd 1ab0 485e  .5.s.b..(m[...H^
+00006da0: cdd8 31f3 a3ac 8bcd f9b0 2b31 656f 326f  ..1.......+1eo2o
+00006db0: 323e c10a 8ef7 76e9 44e9 060b 28f4 899e  2>....v.D...(...
+00006dc0: eef1 e440 537d 6aa2 6a49 c24d bbe9 c531  ...@S}j.jI.M...1
+00006dd0: e64f a0fd 1d96 dd17 e80f ef06 eead ab0f  .O..............
+00006de0: bfe7 43ce f9b3 f37f 0300 00ff ff03 0050  ..C............P
+00006df0: 4b01 022d 0014 0006 0008 0000 0021 0064  K..-.........!.d
+00006e00: d11d 0fde 0100 00cf 0900 0013 0000 0000  ................
+00006e10: 0000 0000 0000 0000 0000 0000 005b 436f  .............[Co
+00006e20: 6e74 656e 745f 5479 7065 735d 2e78 6d6c  ntent_Types].xml
+00006e30: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00006e40: b555 3023 f400 0000 4c02 0000 0b00 0000  .U0#....L.......
+00006e50: 0000 0000 0000 0000 0000 1704 0000 5f72  .............._r
+00006e60: 656c 732f 2e72 656c 7350 4b01 022d 0014  els/.relsPK..-..
+00006e70: 0006 0008 0000 0021 00c8 3243 2f7e 0400  .......!..2C/~..
+00006e80: 00b8 0c00 000f 0000 0000 0000 0000 0000  ................
+00006e90: 0000 003c 0700 0078 6c2f 776f 726b 626f  ...<...xl/workbo
+00006ea0: 6f6b 2e78 6d6c 504b 0102 2d00 1400 0600  ok.xmlPK..-.....
+00006eb0: 0800 0000 2100 a189 0e7a 2501 0000 e104  ....!....z%.....
+00006ec0: 0000 1a00 0000 0000 0000 0000 0000 0000  ................
+00006ed0: e70b 0000 786c 2f5f 7265 6c73 2f77 6f72  ....xl/_rels/wor
+00006ee0: 6b62 6f6f 6b2e 786d 6c2e 7265 6c73 504b  kbook.xml.relsPK
+00006ef0: 0102 2d00 1400 0600 0800 0000 2100 1b27  ..-.........!..'
+00006f00: 8488 1706 0000 2512 0000 1800 0000 0000  ......%.........
+00006f10: 0000 0000 0000 0000 4c0e 0000 786c 2f77  ........L...xl/w
+00006f20: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+00006f30: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00006f40: 0000 2100 d4ad 590d 950b 0000 ae54 0000  ..!...Y......T..
+00006f50: 1800 0000 0000 0000 0000 0000 0000 9914  ................
+00006f60: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00006f70: 7368 6565 7432 2e78 6d6c 504b 0102 2d00  sheet2.xmlPK..-.
+00006f80: 1400 0600 0800 0000 2100 877b 5fd3 f504  ........!..{_...
+00006f90: 0000 ca10 0000 1800 0000 0000 0000 0000  ................
+00006fa0: 0000 0000 6420 0000 786c 2f77 6f72 6b73  ....d ..xl/works
+00006fb0: 6865 6574 732f 7368 6565 7433 2e78 6d6c  heets/sheet3.xml
+00006fc0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00006fd0: b145 0dec 5c07 0000 0221 0000 1300 0000  .E..\....!......
+00006fe0: 0000 0000 0000 0000 0000 8f25 0000 786c  ...........%..xl
+00006ff0: 2f74 6865 6d65 2f74 6865 6d65 312e 786d  /theme/theme1.xm
+00007000: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+00007010: 0078 b91e 89d4 0500 006e 1a00 000d 0000  .x.......n......
+00007020: 0000 0000 0000 0000 0000 001c 2d00 0078  ............-..x
+00007030: 6c2f 7374 796c 6573 2e78 6d6c 504b 0102  l/styles.xmlPK..
+00007040: 2d00 1400 0600 0800 0000 2100 b75b f54a  -.........!..[.J
+00007050: c503 0000 c70c 0000 1400 0000 0000 0000  ................
+00007060: 0000 0000 0000 1b33 0000 786c 2f73 6861  .......3..xl/sha
+00007070: 7265 6453 7472 696e 6773 2e78 6d6c 504b  redStrings.xmlPK
+00007080: 0102 2d00 1400 0600 0800 0000 2100 acd4  ..-.........!...
+00007090: f4ab db02 0000 3b0d 0000 1800 0000 0000  ......;.........
+000070a0: 0000 0000 0000 0000 1237 0000 786c 2f64  .........7..xl/d
+000070b0: 7261 7769 6e67 732f 6472 6177 696e 6731  rawings/drawing1
+000070c0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+000070d0: 0000 2100 becf 157f d708 0000 843f 0000  ..!..........?..
+000070e0: 1400 0000 0000 0000 0000 0000 0000 233a  ..............#:
+000070f0: 0000 786c 2f63 6861 7274 732f 6368 6172  ..xl/charts/char
+00007100: 7431 2e78 6d6c 504b 0102 2d00 1400 0600  t1.xmlPK..-.....
+00007110: 0800 0000 2100 4192 87f0 fd08 0000 0133  ....!.A........3
+00007120: 0000 1400 0000 0000 0000 0000 0000 0000  ................
+00007130: 2c43 0000 786c 2f63 6861 7274 732f 6368  ,C..xl/charts/ch
+00007140: 6172 7432 2e78 6d6c 504b 0102 2d00 1400  art2.xmlPK..-...
+00007150: 0600 0800 0000 2100 bc8d 4ecc 4f08 0000  ......!...N.O...
+00007160: 152a 0000 1400 0000 0000 0000 0000 0000  .*..............
+00007170: 0000 5b4c 0000 786c 2f63 6861 7274 732f  ..[L..xl/charts/
+00007180: 6368 6172 7433 2e78 6d6c 504b 0102 2d00  chart3.xmlPK..-.
+00007190: 1400 0600 0800 0000 2100 d52d 1831 9c04  ........!..-.1..
+000071a0: 0000 c225 0000 1400 0000 0000 0000 0000  ...%............
+000071b0: 0000 0000 dc54 0000 786c 2f63 6861 7274  .....T..xl/chart
+000071c0: 732f 7374 796c 6531 2e78 6d6c 504b 0102  s/style1.xmlPK..
+000071d0: 2d00 1400 0600 0800 0000 2100 1c14 a7a8  -.........!.....
+000071e0: fd00 0000 6e03 0000 1500 0000 0000 0000  ....n...........
+000071f0: 0000 0000 0000 aa59 0000 786c 2f63 6861  .......Y..xl/cha
+00007200: 7274 732f 636f 6c6f 7273 312e 786d 6c50  rts/colors1.xmlP
+00007210: 4b01 022d 0014 0006 0008 0000 0021 003b  K..-.........!.;
+00007220: 6d32 4bc1 0000 0042 0100 0023 0000 0000  m2K....B...#....
+00007230: 0000 0000 0000 0000 00da 5a00 0078 6c2f  ..........Z..xl/
+00007240: 776f 726b 7368 6565 7473 2f5f 7265 6c73  worksheets/_rels
+00007250: 2f73 6865 6574 312e 786d 6c2e 7265 6c73  /sheet1.xml.rels
+00007260: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00007270: 1198 abc9 db00 0000 d001 0000 2300 0000  ............#...
+00007280: 0000 0000 0000 0000 0000 dc5b 0000 786c  ...........[..xl
+00007290: 2f77 6f72 6b73 6865 6574 732f 5f72 656c  /worksheets/_rel
+000072a0: 732f 7368 6565 7432 2e78 6d6c 2e72 656c  s/sheet2.xml.rel
+000072b0: 7350 4b01 022d 0014 0006 0008 0000 0021  sPK..-.........!
+000072c0: 0081 c55e bdca 0000 0035 0200 0023 0000  ...^.....5...#..
+000072d0: 0000 0000 0000 0000 0000 00f8 5c00 0078  ............\..x
+000072e0: 6c2f 6472 6177 696e 6773 2f5f 7265 6c73  l/drawings/_rels
+000072f0: 2f64 7261 7769 6e67 312e 786d 6c2e 7265  /drawing1.xml.re
+00007300: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
+00007310: 2100 801b dc81 d200 0000 8f01 0000 1f00  !...............
+00007320: 0000 0000 0000 0000 0000 0000 035e 0000  .............^..
+00007330: 786c 2f63 6861 7274 732f 5f72 656c 732f  xl/charts/_rels/
+00007340: 6368 6172 7433 2e78 6d6c 2e72 656c 7350  chart3.xml.relsP
+00007350: 4b01 022d 0014 0006 0008 0000 0021 0090  K..-.........!..
+00007360: 000d b0a6 0100 00dd 0200 000f 0000 0000  ................
+00007370: 0000 0000 0000 0000 0012 5f00 0078 6c2f  .........._..xl/
+00007380: 6d65 7461 6461 7461 2e78 6d6c 504b 0102  metadata.xmlPK..
+00007390: 2d00 1400 0600 0800 0000 2100 3585 fa75  -.........!.5..u
+000073a0: af01 0000 3c10 0000 2700 0000 0000 0000  ....<...'.......
+000073b0: 0000 0000 0000 e560 0000 786c 2f70 7269  .......`..xl/pri
+000073c0: 6e74 6572 5365 7474 696e 6773 2f70 7269  nterSettings/pri
+000073d0: 6e74 6572 5365 7474 696e 6773 312e 6269  nterSettings1.bi
+000073e0: 6e50 4b01 022d 0014 0006 0008 0000 0021  nPK..-.........!
+000073f0: 0035 85fa 75af 0100 003c 1000 0027 0000  .5..u....<...'..
+00007400: 0000 0000 0000 0000 0000 00d9 6200 0078  ............b..x
+00007410: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
+00007420: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
+00007430: 7332 2e62 696e 504b 0102 2d00 1400 0600  s2.binPK..-.....
+00007440: 0800 0000 2100 d1f8 0490 3203 0000 0813  ....!.....2.....
+00007450: 0000 1000 0000 0000 0000 0000 0000 0000  ................
+00007460: cd64 0000 786c 2f63 616c 6343 6861 696e  .d..xl/calcChain
+00007470: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00007480: 0000 2100 2911 c752 4c01 0000 6902 0000  ..!.)..RL...i...
+00007490: 1100 0000 0000 0000 0000 0000 0000 2d68  ..............-h
+000074a0: 0000 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
+000074b0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+000074c0: 0021 0038 0ca0 e509 0200 0032 0500 0010  .!.8.......2....
+000074d0: 0000 0000 0000 0000 0000 0000 00b0 6a00  ..............j.
+000074e0: 0064 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
+000074f0: 6c50 4b05 0600 0000 001a 001a 0002 0700  lPK.............
+00007500: 00ef 6d00 0000 00                        ..m....
```

### Comparing `ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx` & `ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/src/ragtime/base_folder/res/spreadsheet_templates/spreadsheet_rich_template.xlsx` & `ragtime-0.0.32/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/tests/full_test.py` & `ragtime-0.0.32/tests/full_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # always start with init_project before importing ragtime.config values since they are updated
 # with init_project and import works by value and not by reference, so values imported before
 # calling init_project are not updated after the function call
 ragtime.config.init_project(name=PROJECT_NAME, init_type="delete_if_exists")
 from ragtime.config import FOLDER_ANSWERS, FOLDER_QUESTIONS, logger
 
-logger.debug(f'{PROJECT_NAME} starts')
+logger.debug(f'"{PROJECT_NAME}" starts')
 
 class MCQAnsPptr(generators.Prompter):
     def get_prompt(self, question:Question, chunks:Optional[Chunks] = None) -> Prompt:
         result:Prompt = Prompt()
         result.user = f"{question.text}"
         result.system = "Répond uniquement avec la lettre. Ne donne qu'une seule réponse."
         return result
@@ -32,8 +32,8 @@
 test_file:str = 'test_quest.json'
 shutil.copy(test_file, FOLDER_QUESTIONS)
 generators.gen_Answers(folder_in=FOLDER_QUESTIONS, folder_out=FOLDER_ANSWERS,
                         json_file=test_file,
                         prompter=MCQAnsPptr(),
                         llm_names=["gpt-3.5-turbo", "mistral/mistral-large-latest"])
 
-logger.debug(f'{PROJECT_NAME} ends')
+logger.debug(f'"{PROJECT_NAME}" ends')
```

### Comparing `ragtime-0.0.31/tests/run_tests.py` & `ragtime-0.0.32/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/tests/test_quest.json` & `ragtime-0.0.32/tests/test_quest.json`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/.gitignore` & `ragtime-0.0.32/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,19 @@
 *.mp4
 *.tiff
 *.avi
 *.flv
 *.mov
 *.wmv
 
+~*
+**/~*
 keys.py
 __pycache__
 logs.txt
 litellm_uuid.txt
 **/keys.py
 **/__pycache__
 **/logs.txt
 **/litellm_uuid.txt
 **/.vscode
-.vscode
+.vscode
```

### Comparing `ragtime-0.0.31/LICENSE` & `ragtime-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.31/README.md` & `ragtime-0.0.32/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,25 @@
 
 # Presentation
 **Ragtime** 🎹 is an LLMOps framework which allows you to automatically:
 1. evaluate a Retrieval Augmented Generation (RAG) system
 2. compare different RAGs / LLMs
 3. generate Facts to allow automatic evaluation
 
+Ragtime 🎹 allows you to evaluate **long answers** not only multiple choice questions or counting common words between an answer and a baseline. It is then required to evaluate summarizers, 
+
 In Ragtime 🎹, a *RAG* is made of, optionally, a *Retriever*, and always, one or several *Large Language Model* (*LLM*).
 - A *Retriever* takes a *question* in input and returns one or several *chunks* or *paragraphs* retrieved from a documents knowledge base
 - A *LLM* is a text to text generator taking in input a *prompt*, made of a question and optional chunks, and returning an *LLMAnswer*
 
 You can specify how *prompts* are generated and how the *LLMAnswer* has to be post-processed to return an *answer*.
 
+# Contributing
+Glad you wish to contribute! More details [here](CONTRIBUTING.md).
+
 # How does it work?
 The main idea in Ragtime 🎹 is to evaluate answers returned by a RAG based on **Facts** that you define. Indeed, it is very difficult to evaluate RAGs and/or LLMs because you cannot define a "good" answer. A LLM can return many equivalent answers expressed in different ways, making impossible a simple string comparison to determine whether an answer is right or wrong. Even though many proxies have been created, counting the number of common words like in ROUGE for instance is not very precise (see [HuggingFace's `lighteval`](https://github.com/huggingface/lighteval?tab=readme-ov-file#metrics-for-generative-tasks))
 
 In Ragtime 🎹, answers returned by a RAG or a LLM are evaluated against a set of facts. If the answer validates all the facts, then the answer is deemed correct. Conversely, if some facts are not validated, the answer is considered wrong. The number of validated facts compared to the total number of facts to validate defines a score.
 
 You can either define facts manually, or have a LLM define them for you. **The evaluation of facts against answers is done automatically with another LLM**.
 
@@ -38,18 +43,18 @@
 Almost every object in Ragtime 🎹 has a `meta` field, which is a dictionnary where you can store all the extra data you need for your specific use case.
 
 # Examples
 You can now go to [ragtime-projects](https://github.com/recitalAI/ragtime-projects) to see examples of Ragtime 🎹 in action!
 
 # Troubleshooting
 ## Setting the API keys on Windows
-API keys are stored in environment variables locally on your computer. If you are using Windows, you should first set the API keys values as:
+API keys are stored in environment variables locally on your computer. If you are using Windows, you should first set the API keys values in the shell as:
 ```shell
 setx OPENAI_API_KEY sk-....
 ```
 The list of environment variable names to set, depending on the APIs you need to access, is given in the [LiteLLM documentation](https://litellm.vercel.app/docs/providers).
 
-Once the keys are set, just call `ragtime.config.init_API_keys` with the list of environment variables to make accessible to Python, for instance `init_API_keys(['OPENAI_API_KEY'])`.
+Once the keys are set, just call `ragtime.config.init_win_env` with the list of environment variables to make accessible to Python, for instance `init_API_keys(['OPENAI_API_KEY'])`.
 
 ## Using Google LLMs
 Execute what's indicated in the [LiteLLM documentation](https://litellm.vercel.app/docs/providers/vertex#gemini-pro).
 Also make sure your project has `Vertex AI` API enabled.
```

### Comparing `ragtime-0.0.31/pyproject.toml` & `ragtime-0.0.32/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ragtime"
-version = "0.0.31"
+version = "0.0.32"
 
 authors = [
   { name="Gilles Moyse", email="gilles@recital.ai" },
 ]
 maintainers = [
   { name="reciTAL", email="ragtime@recital.ai" },
 ]
```

### Comparing `ragtime-0.0.31/PKG-INFO` & `ragtime-0.0.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragtime
-Version: 0.0.31
+Version: 0.0.32
 Summary: Ragtime 🎹 is an LLMOps framework to automatically evaluate Retrieval Augmented Generation (RAG) systems and compare different RAGs / LLMs
 Project-URL: Homepage, https://github.com/recitalAI/ragtime-package
 Project-URL: Issues, https://github.com/recitalAI/ragtime-package/issues
 Author-email: Gilles Moyse <gilles@recital.ai>
 Maintainer-email: reciTAL <ragtime@recital.ai>
 License: MIT License
         
@@ -53,20 +53,25 @@
 
 # Presentation
 **Ragtime** 🎹 is an LLMOps framework which allows you to automatically:
 1. evaluate a Retrieval Augmented Generation (RAG) system
 2. compare different RAGs / LLMs
 3. generate Facts to allow automatic evaluation
 
+Ragtime 🎹 allows you to evaluate **long answers** not only multiple choice questions or counting common words between an answer and a baseline. It is then required to evaluate summarizers, 
+
 In Ragtime 🎹, a *RAG* is made of, optionally, a *Retriever*, and always, one or several *Large Language Model* (*LLM*).
 - A *Retriever* takes a *question* in input and returns one or several *chunks* or *paragraphs* retrieved from a documents knowledge base
 - A *LLM* is a text to text generator taking in input a *prompt*, made of a question and optional chunks, and returning an *LLMAnswer*
 
 You can specify how *prompts* are generated and how the *LLMAnswer* has to be post-processed to return an *answer*.
 
+# Contributing
+Glad you wish to contribute! More details [here](CONTRIBUTING.md).
+
 # How does it work?
 The main idea in Ragtime 🎹 is to evaluate answers returned by a RAG based on **Facts** that you define. Indeed, it is very difficult to evaluate RAGs and/or LLMs because you cannot define a "good" answer. A LLM can return many equivalent answers expressed in different ways, making impossible a simple string comparison to determine whether an answer is right or wrong. Even though many proxies have been created, counting the number of common words like in ROUGE for instance is not very precise (see [HuggingFace's `lighteval`](https://github.com/huggingface/lighteval?tab=readme-ov-file#metrics-for-generative-tasks))
 
 In Ragtime 🎹, answers returned by a RAG or a LLM are evaluated against a set of facts. If the answer validates all the facts, then the answer is deemed correct. Conversely, if some facts are not validated, the answer is considered wrong. The number of validated facts compared to the total number of facts to validate defines a score.
 
 You can either define facts manually, or have a LLM define them for you. **The evaluation of facts against answers is done automatically with another LLM**.
 
@@ -89,18 +94,18 @@
 Almost every object in Ragtime 🎹 has a `meta` field, which is a dictionnary where you can store all the extra data you need for your specific use case.
 
 # Examples
 You can now go to [ragtime-projects](https://github.com/recitalAI/ragtime-projects) to see examples of Ragtime 🎹 in action!
 
 # Troubleshooting
 ## Setting the API keys on Windows
-API keys are stored in environment variables locally on your computer. If you are using Windows, you should first set the API keys values as:
+API keys are stored in environment variables locally on your computer. If you are using Windows, you should first set the API keys values in the shell as:
 ```shell
 setx OPENAI_API_KEY sk-....
 ```
 The list of environment variable names to set, depending on the APIs you need to access, is given in the [LiteLLM documentation](https://litellm.vercel.app/docs/providers).
 
-Once the keys are set, just call `ragtime.config.init_API_keys` with the list of environment variables to make accessible to Python, for instance `init_API_keys(['OPENAI_API_KEY'])`.
+Once the keys are set, just call `ragtime.config.init_win_env` with the list of environment variables to make accessible to Python, for instance `init_API_keys(['OPENAI_API_KEY'])`.
 
 ## Using Google LLMs
 Execute what's indicated in the [LiteLLM documentation](https://litellm.vercel.app/docs/providers/vertex#gemini-pro).
 Also make sure your project has `Vertex AI` API enabled.
```

