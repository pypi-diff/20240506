# Comparing `tmp/openinference_instrumentation_llama_index-1.2.2.tar.gz` & `tmp/openinference_instrumentation_llama_index-1.3.0.tar.gz`

## Comparing `openinference_instrumentation_llama_index-1.2.2.tar` & `openinference_instrumentation_llama_index-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/__init__.py
--rw-r--r--   0        0        0    31646 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/_callback.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/version.py
--rw-r--r--   0        0        0    15132 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/tests/openinference/instrumentation/llama_index/test_callback.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/LICENSE
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/README.md
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/__init__.py
+-rw-r--r--   0        0        0    31854 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/_callback.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/version.py
+-rw-r--r--   0        0        0    17892 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/tests/openinference/instrumentation/llama_index/test_callback.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/README.md
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/PKG-INFO
```

### Comparing `openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/__init__.py` & `openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/_callback.py` & `openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/_callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 from uuid import uuid4
 
+from openinference.instrumentation import get_attributes_from_context
 from openinference.semconv.trace import (
     DocumentAttributes,
     EmbeddingAttributes,
     MessageAttributes,
     OpenInferenceMimeTypeValues,
     OpenInferenceSpanKindValues,
     RerankerAttributes,
@@ -439,14 +440,15 @@
                 except Exception:
                     logger.exception(
                         f"Failed to flatten attributes. event_type={event_data.event_type}, "
                         f"attributes={attributes}",
                     )
                 else:
                     span.set_attributes(flattened_attributes)
+                span.set_attributes(dict(get_attributes_from_context()))
                 span.set_status(status=status)
                 end_time = event_data.end_time
                 span.end(end_time=end_time)
                 self._self_is_finished = True
             raise
         else:
             self._self_tokens.append(value)
@@ -468,14 +470,15 @@
             status_code=trace_api.StatusCode.ERROR,
             description="\n".join(status_descriptions),
         )
     else:
         status = trace_api.Status(status_code=trace_api.StatusCode.OK)
     span.set_status(status=status)
     try:
+        span.set_attributes(dict(get_attributes_from_context()))
         span.set_attributes(dict(_flatten(attributes)))
     except Exception:
         logger.exception(
             f"Failed to set attributes on span. event_type={event_data.event_type}, "
             f"attributes={attributes}",
         )
     span.end(end_time=event_data.end_time)
```

### Comparing `openinference_instrumentation_llama_index-1.2.2/tests/openinference/instrumentation/llama_index/test_callback.py` & `openinference_instrumentation_llama_index-1.3.0/tests/openinference/instrumentation/llama_index/test_callback.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import pytest
 from httpx import AsyncByteStream, Response, SyncByteStream
 from llama_index.core import Document, ListIndex, Settings
 from llama_index.core.base.response.schema import StreamingResponse
 from llama_index.core.callbacks import CallbackManager
 from llama_index.core.schema import TextNode
 from llama_index.llms.openai import OpenAI  # type: ignore
+from openinference.instrumentation import using_attributes
 from openinference.instrumentation.llama_index import LlamaIndexInstrumentor
 from openinference.semconv.trace import (
     DocumentAttributes,
     EmbeddingAttributes,
     MessageAttributes,
     OpenInferenceSpanKindValues,
     SpanAttributes,
@@ -66,14 +67,18 @@
     is_async: bool,
     is_stream: bool,
     status_code: int,
     respx_mock: MockRouter,
     in_memory_span_exporter: InMemorySpanExporter,
     nodes: List[Document],
     chat_completion_mock_stream: Tuple[List[bytes], List[Dict[str, Any]]],
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
 ) -> None:
     n = 10  # number of concurrent queries
     questions = {randstr() for _ in range(n)}
     answer = chat_completion_mock_stream[1][0]["content"] if is_stream else randstr()
     callback_manager = CallbackManager()
     Settings.callback_manager = callback_manager
     Settings.llm = OpenAI()
@@ -105,44 +110,75 @@
 
             async def task() -> None:
                 await asyncio.gather(
                     *(query_engine.aquery(question) for question in questions),
                     return_exceptions=True,
                 )
 
-            asyncio.run(task())
+            with using_attributes(
+                session_id=session_id,
+                user_id=user_id,
+                metadata=metadata,
+                tags=tags,
+            ):
+                asyncio.run(task())
         else:
+
+            def threaded_query(question: str) -> None:
+                # This context manager must be inside this function definition so
+                # there's a different instantiation per thread. This allows to use
+                # a different context per thread, as desired
+                with using_attributes(
+                    session_id=session_id,
+                    user_id=user_id,
+                    metadata=metadata,
+                    tags=tags,
+                ):
+                    response = query_engine.query(question)
+                    (list(cast(StreamingResponse, response).response_gen) if is_stream else None,)
+
             with ThreadPoolExecutor(max_workers=n) as executor:
                 executor.map(
-                    lambda question: (
-                        (response := query_engine.query(question)),
-                        list(cast(StreamingResponse, response).response_gen) if is_stream else None,
-                    ),
+                    threaded_query,
                     questions,
                 )
 
     spans = in_memory_span_exporter.get_finished_spans()
     traces: DefaultDict[int, Dict[str, ReadableSpan]] = defaultdict(dict)
     for span in spans:
         traces[span.context.trace_id][span.name] = span
 
     assert len(traces) == n
     for spans_by_name in traces.values():
-        question = _check_spans(spans_by_name, answer, nodes, status_code, is_stream)
+        question = _check_spans(
+            spans_by_name,
+            answer,
+            nodes,
+            status_code,
+            is_stream,
+            session_id,
+            user_id,
+            metadata,
+            tags,
+        )
         assert question in questions
         questions.remove(question)
     assert len(questions) == 0
 
 
 def _check_spans(
     spans_by_name: Dict[str, ReadableSpan],
     answer: str,
     nodes: List[Document],
     status_code: int,
     is_stream: bool,
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
 ) -> str:
     assert (query_span := spans_by_name.pop("query")) is not None
     assert query_span.parent is None
     query_attributes = dict(query_span.attributes or {})
     assert query_attributes.pop(OPENINFERENCE_SPAN_KIND, None) == CHAIN.value
     question = cast(Optional[str], query_attributes.pop(INPUT_VALUE, None))
     assert question is not None
@@ -155,14 +191,16 @@
         # `on_event_end` to set the status code.
         status_code == 400 and is_stream
     ):
         assert query_span.status.status_code == trace_api.StatusCode.ERROR
         assert query_span.status.description and query_span.status.description.startswith(
             openai.BadRequestError.__name__,
         )
+
+    _check_context_attributes(query_attributes, session_id, user_id, metadata, tags)
     assert query_attributes == {}
 
     assert (synthesize_span := spans_by_name.pop("synthesize")) is not None
     assert synthesize_span.parent is not None
     assert synthesize_span.parent.span_id == query_span.context.span_id
     assert synthesize_span.context.trace_id == query_span.context.trace_id
     synthesize_attributes = dict(synthesize_span.attributes or {})
@@ -177,14 +215,15 @@
         # `on_event_end` to set the status code.
         status_code == 400 and is_stream
     ):
         assert synthesize_span.status.status_code == trace_api.StatusCode.ERROR
         assert query_span.status.description and query_span.status.description.startswith(
             openai.BadRequestError.__name__,
         )
+    _check_context_attributes(synthesize_attributes, session_id, user_id, metadata, tags)
     assert synthesize_attributes == {}
 
     assert (retrieve_span := spans_by_name.pop("retrieve")) is not None
     assert retrieve_span.parent is not None
     assert retrieve_span.parent.span_id == query_span.context.span_id
     assert retrieve_span.context.trace_id == query_span.context.trace_id
     retrieve_attributes = dict(retrieve_span.attributes or {})
@@ -199,14 +238,15 @@
     assert retrieve_attributes.pop(
         f"{RETRIEVAL_DOCUMENTS}.0.{DOCUMENT_METADATA}", None
     ) == json.dumps(nodes[0].metadata)
     assert (
         retrieve_attributes.pop(f"{RETRIEVAL_DOCUMENTS}.1.{DOCUMENT_CONTENT}", None)
         == nodes[1].text
     )
+    _check_context_attributes(retrieve_attributes, session_id, user_id, metadata, tags)
     assert retrieve_attributes == {}
 
     if status_code == 200:
         # FIXME: LlamaIndex doesn't currently capture the LLM span when status_code == 400
         # For example, if an exception is raised by the LLM at the following location,
         # `on_event_end` never gets called.
         # https://github.com/run-llama/llama_index/blob/dcef41ee67925cccf1ee7bb2dd386bcf0564ba29/llama_index/llms/base.py#L100 # noqa E501
@@ -233,30 +273,80 @@
         assert llm_attributes.pop(OUTPUT_VALUE, None) == answer
         if not is_stream:
             # FIXME: currently we can't capture messages when streaming
             assert (
                 llm_attributes.pop(f"{LLM_OUTPUT_MESSAGES}.0.{MESSAGE_ROLE}", None) == "assistant"
             )
             assert llm_attributes.pop(f"{LLM_OUTPUT_MESSAGES}.0.{MESSAGE_CONTENT}", None) == answer
+        _check_context_attributes(llm_attributes, session_id, user_id, metadata, tags)
         assert llm_attributes == {}
 
     # FIXME: maybe chunking spans should be discarded?
     assert (chunking_span := spans_by_name.pop("chunking", None)) is not None
     assert chunking_span.parent is not None
     assert chunking_span.parent.span_id == synthesize_span.context.span_id
     assert chunking_span.context.trace_id == synthesize_span.context.trace_id
     chunking_attributes = dict(chunking_span.attributes or {})
     assert chunking_attributes.pop(OPENINFERENCE_SPAN_KIND, None) is not None
+    _check_context_attributes(chunking_attributes, session_id, user_id, metadata, tags)
     assert chunking_attributes == {}
 
     assert spans_by_name == {}
 
     return question
 
 
+def _check_context_attributes(
+    attributes: Dict[str, Any],
+    session_id: str,
+    user_id: str,
+    metadata: Dict[str, Any],
+    tags: List[str],
+) -> None:
+    assert attributes.pop(SESSION_ID, None) == session_id
+    assert attributes.pop(USER_ID, None) == user_id
+    attr_metadata = attributes.pop(METADATA, None)
+    assert attr_metadata is not None
+    assert isinstance(attr_metadata, str)  # must be json string
+    metadata_dict = json.loads(attr_metadata)
+    assert metadata_dict == metadata
+    attr_tags = attributes.pop(TAG_TAGS, None)
+    assert attr_tags is not None
+    assert len(attr_tags) == len(tags)
+    assert list(attr_tags) == tags
+
+
+@pytest.fixture()
+def session_id() -> str:
+    return "my-test-session-id"
+
+
+@pytest.fixture()
+def user_id() -> str:
+    return "my-test-user-id"
+
+
+@pytest.fixture()
+def metadata() -> Dict[str, Any]:
+    return {
+        "test-int": 1,
+        "test-str": "string",
+        "test-list": [1, 2, 3],
+        "test-dict": {
+            "key-1": "val-1",
+            "key-2": "val-2",
+        },
+    }
+
+
+@pytest.fixture()
+def tags() -> List[str]:
+    return ["tag-1", "tag-2"]
+
+
 @pytest.fixture
 def nodes() -> List[TextNode]:
     return [
         Document(text=randstr(), metadata={"category": randstr()}),  # type: ignore
         TextNode(text=randstr()),
     ]
 
@@ -370,7 +460,11 @@
 TOOL_CALL_FUNCTION_NAME = ToolCallAttributes.TOOL_CALL_FUNCTION_NAME
 LLM_PROMPT_TEMPLATE = SpanAttributes.LLM_PROMPT_TEMPLATE
 LLM_PROMPT_TEMPLATE_VARIABLES = SpanAttributes.LLM_PROMPT_TEMPLATE_VARIABLES
 
 CHAIN = OpenInferenceSpanKindValues.CHAIN
 LLM = OpenInferenceSpanKindValues.LLM
 RETRIEVER = OpenInferenceSpanKindValues.RETRIEVER
+SESSION_ID = SpanAttributes.SESSION_ID
+USER_ID = SpanAttributes.USER_ID
+METADATA = SpanAttributes.METADATA
+TAG_TAGS = SpanAttributes.TAG_TAGS
```

### Comparing `openinference_instrumentation_llama_index-1.2.2/LICENSE` & `openinference_instrumentation_llama_index-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.2.2/README.md` & `openinference_instrumentation_llama_index-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.2.2/pyproject.toml` & `openinference_instrumentation_llama_index-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "opentelemetry-api",
   "opentelemetry-instrumentation",
   "opentelemetry-semantic-conventions",
+  "openinference-instrumentation>=0.1.3",
   "openinference-semantic-conventions",
   "typing-extensions",
   "wrapt",
 ]
 
 [project.optional-dependencies]
 instruments = [
@@ -54,7 +55,36 @@
 include = [
   "/src",
   "/tests",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/openinference"]
+
+[tool.mypy]
+strict = true
+explicit_package_bases = true
+exclude = [
+  "examples",
+  "dist",
+  "sdist",
+]
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = [
+  "wrapt",
+]
+
+[tool.ruff]
+line-length = 100
+target-version = "py38"
+
+[tool.ruff.lint.per-file-ignores]
+"*.ipynb" = ["E402", "E501"]
+
+[tool.ruff.lint]
+ignore-init-module-imports = true
+select = ["E", "F", "W", "I"]
+
+[tool.ruff.lint.isort]
+force-single-line = false
```

### Comparing `openinference_instrumentation_llama_index-1.2.2/PKG-INFO` & `openinference_instrumentation_llama_index-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation-llama-index
-Version: 1.2.2
+Version: 1.3.0
 Summary: OpenInference LlamaIndex Instrumentation
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-llama-index
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.8
+Requires-Dist: openinference-instrumentation>=0.1.3
 Requires-Dist: openinference-semantic-conventions
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-semantic-conventions
 Requires-Dist: typing-extensions
 Requires-Dist: wrapt
 Provides-Extra: instruments
```

