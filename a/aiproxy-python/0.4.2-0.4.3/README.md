# Comparing `tmp/aiproxy_python-0.4.2-py3-none-any.whl.zip` & `tmp/aiproxy_python-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 30353 bytes, number of entries: 16
--rw-r--r--  2.0 unx      540 b- defN 24-May-03 22:58 aiproxy/__init__.py
+Zip file size: 29749 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      540 b- defN 24-May-06 14:29 aiproxy/__init__.py
 -rw-r--r--  2.0 unx     2414 b- defN 24-May-02 07:38 aiproxy/__main__.py
 -rw-r--r--  2.0 unx     7728 b- defN 24-May-01 13:52 aiproxy/accesslog.py
 -rw-r--r--  2.0 unx     7318 b- defN 24-May-02 06:49 aiproxy/anthropic_claude.py
 -rw-r--r--  2.0 unx     1337 b- defN 23-Dec-08 14:24 aiproxy/azurequeueclient.py
+-rw-r--r--  2.0 unx    11137 b- defN 24-May-06 14:29 aiproxy/bedrock_claude.py
 -rw-r--r--  2.0 unx    13037 b- defN 24-May-03 22:49 aiproxy/chatgpt.py
--rw-r--r--  2.0 unx    16284 b- defN 23-Dec-11 15:51 aiproxy/claude2.py
--rw-r--r--  2.0 unx    11392 b- defN 24-May-02 06:49 aiproxy/gemini.py
--rw-r--r--  2.0 unx    21761 b- defN 24-May-03 22:46 aiproxy/httpx_proxy.py
+-rw-r--r--  2.0 unx    11392 b- defN 24-May-06 12:26 aiproxy/gemini.py
+-rw-r--r--  2.0 unx    21761 b- defN 24-May-06 13:41 aiproxy/httpx_proxy.py
 -rw-r--r--  2.0 unx     2165 b- defN 24-Apr-02 01:14 aiproxy/proxy.py
 -rw-r--r--  2.0 unx      731 b- defN 24-May-01 13:52 aiproxy/queueclient.py
--rw-r--r--  2.0 unx    11324 b- defN 24-May-03 22:58 aiproxy_python-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    14231 b- defN 24-May-03 22:58 aiproxy_python-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-03 22:58 aiproxy_python-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-03 22:58 aiproxy_python-0.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1276 b- defN 24-May-03 22:58 aiproxy_python-0.4.2.dist-info/RECORD
-16 files, 111638 bytes uncompressed, 28277 bytes compressed:  74.7%
+-rw-r--r--  2.0 unx    11324 b- defN 24-May-06 14:30 aiproxy_python-0.4.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14341 b- defN 24-May-06 14:30 aiproxy_python-0.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-06 14:30 aiproxy_python-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-06 14:30 aiproxy_python-0.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1283 b- defN 24-May-06 14:30 aiproxy_python-0.4.3.dist-info/RECORD
+16 files, 106608 bytes uncompressed, 27659 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -9,41 +9,41 @@
 
 Filename: aiproxy/anthropic_claude.py
 Comment: 
 
 Filename: aiproxy/azurequeueclient.py
 Comment: 
 
-Filename: aiproxy/chatgpt.py
+Filename: aiproxy/bedrock_claude.py
 Comment: 
 
-Filename: aiproxy/claude2.py
+Filename: aiproxy/chatgpt.py
 Comment: 
 
 Filename: aiproxy/gemini.py
 Comment: 
 
 Filename: aiproxy/httpx_proxy.py
 Comment: 
 
 Filename: aiproxy/proxy.py
 Comment: 
 
 Filename: aiproxy/queueclient.py
 Comment: 
 
-Filename: aiproxy_python-0.4.2.dist-info/LICENSE
+Filename: aiproxy_python-0.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: aiproxy_python-0.4.2.dist-info/METADATA
+Filename: aiproxy_python-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: aiproxy_python-0.4.2.dist-info/WHEEL
+Filename: aiproxy_python-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: aiproxy_python-0.4.2.dist-info/top_level.txt
+Filename: aiproxy_python-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: aiproxy_python-0.4.2.dist-info/RECORD
+Filename: aiproxy_python-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiproxy/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 import logging
 
 logger = logging.getLogger("aiproxy")
 logger.setLevel(logging.INFO)
 log_format = logging.Formatter("[%(levelname)s] %(asctime)s : %(message)s")
 streamHandler = logging.StreamHandler()
```

## Comparing `aiproxy/claude2.py` & `aiproxy/bedrock_claude.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,373 +2,276 @@
 from datetime import datetime
 import json
 import logging
 import re
 import time
 import traceback
 from typing import List, Union
-from uuid import uuid4
-from fastapi import FastAPI, Request
-from fastapi.responses import JSONResponse, StreamingResponse, Response
 import httpx
+from fastapi import Request
+from fastapi.responses import StreamingResponse, JSONResponse
 from botocore.auth import SigV4Auth
 from botocore.awsrequest import AWSRequest
 from botocore.credentials import Credentials
-from .proxy import ProxyBase, RequestFilterBase, ResponseFilterBase, RequestFilterException, ResponseFilterException
-from .accesslog import _AccessLogBase, RequestItemBase, ResponseItemBase, StreamChunkItemBase, ErrorItemBase
-from .queueclient import QueueClientBase
+from aiproxy.proxy import RequestFilterBase, ResponseFilterBase
+from aiproxy.httpx_proxy import HTTPXProxy, SessionInfo, SessionRequestItemBase, SessionResponseItemBase, SessionStreamChunkItemBase, SessionErrorItemBase
+from aiproxy.accesslog import _AccessLogBase
+from aiproxy.queueclient import QueueClientBase
 
 
 logger = logging.getLogger(__name__)
 
 
-class Claude2RequestItem(RequestItemBase):
+class ClaudeRequestItem(SessionRequestItemBase):
     def to_accesslog(self, accesslog_cls: _AccessLogBase) -> _AccessLogBase:
         try:
-            content = self.request_json["prompt"].split("Human:")[-1].split("Assistant:")[0].strip()
-        except:
-            logger.error(f"Error at parsing prompt text for log: {self.request_json.get('prompt')}")
+            content = self.request_json["messages"][-1]["content"]
+            if isinstance(content, list):
+                content = content[-1]
+            if isinstance(content, dict):
+                if content["type"] == "text":
+                    content = content["text"]
+                elif content["type"] == "text":
+                    content = "(image)"
+                else:
+                    content = "(other)"
+
+        except Exception:
+            logger.error(f"Error at parsing request for log: {self.request_json}")
             content = None
 
         return accesslog_cls(
             request_id=self.request_id,
             created_at=datetime.utcnow(),
             direction="request",
             content=content,
             raw_body=json.dumps(self.request_json, ensure_ascii=False),
             raw_headers=json.dumps(self.request_headers, ensure_ascii=False),
-            model="anthropic.claude-v2"
+            model=self.session.extra_info["model"]
         )
 
 
-class Claude2ResponseItem(ResponseItemBase):
+class ClaudeResponseItem(SessionResponseItemBase):
     def to_accesslog(self, accesslog_cls: _AccessLogBase) -> _AccessLogBase:
+        content = None
+        prompt_tokens = 0
+        completion_tokens = 0
+        try:
+            content = self.response_json["content"][0]["text"]
+            prompt_tokens = self.response_json["usage"]["input_tokens"] \
+                if "usage" in self.response_json else 0
+            completion_tokens = self.response_json["usage"]["output_tokens"] \
+                if "usage" in self.response_json else 0
+        except Exception:
+            logger.error(f"Error at parsing response for log: {self.response_json}")
+
         return accesslog_cls(
             request_id=self.request_id,
             created_at=datetime.utcnow(),
             direction="response",
             status_code=self.status_code,
-            content=self.response_json["completion"],
+            content=content,
             function_call=None,
             tool_calls=None,
             raw_body=json.dumps(self.response_json, ensure_ascii=False),
             raw_headers=json.dumps(self.response_headers, ensure_ascii=False),
-            model="anthropic.claude-v2",
-            prompt_tokens=self.response_headers.get("x-amzn-bedrock-input-token-count", 0),
-            completion_tokens=self.response_headers.get("x-amzn-bedrock-output-token-count", 0),
+            model=self.response_json.get("model"),
+            prompt_tokens=prompt_tokens,
+            completion_tokens=completion_tokens,
             request_time=self.duration,
             request_time_api=self.duration_api
         )
 
 
-class Claude2StreamResponseItem(StreamChunkItemBase):
-    def to_accesslog(self, chunks: list, accesslog_cls: _AccessLogBase) -> _AccessLogBase:
-        chunk_jsons = []
-        response_content = ""
+class ClaudeStreamResponseItem(SessionStreamChunkItemBase):
+    def to_accesslog(self, accesslog_cls: _AccessLogBase) -> _AccessLogBase:
+        response_text = ""
+        model = ""
         prompt_tokens = 0
         completion_tokens = 0
 
-        # Parse info from chunks
-        for chunk in chunks:
-            chunk_jsons.append(chunk.chunk_json)
-            response_content += chunk.chunk_json["completion"] or ""
-
-        # Tokens
-        if len(chunk_jsons) > 0:
-            if "amazon-bedrock-invocationMetrics" in chunk_jsons[-1]:
-                prompt_tokens = chunk_jsons[-1]["amazon-bedrock-invocationMetrics"]["inputTokenCount"]
-                completion_tokens = chunk_jsons[-1]["amazon-bedrock-invocationMetrics"]["outputTokenCount"]
-            else:
-                # On error response in stream mode
-                prompt_tokens = self.response_headers.get("x-amzn-bedrock-input-token-count", 0)
-                completion_tokens = self.response_headers.get("x-amzn-bedrock-output-token-count", 0)
+        self.response_content = str(self.session.extra_info["response_events"])
+        try:
+            for chunk in self.session.extra_info["response_events"]:
+                # Parse JSON data from bytes chunk
+                for m in re.findall(rb"event\{.*?\}", chunk):
+                    b64bytes = json.loads(m[5:].decode("utf-8"))["bytes"]
+                    chunk_json = json.loads(base64.b64decode(b64bytes).decode())
+
+                    # Get metadata of request
+                    if chunk_json["type"] == "message_start":
+                        msg = chunk_json["message"]
+                        model = msg["model"]
+                        prompt_tokens = msg["usage"]["input_tokens"]
+
+                    # Get content chunk
+                    elif chunk_json["type"] == "content_block_delta":
+                        response_text += chunk_json["delta"]["text"] or ""
+
+                    # Get metadata of response
+                    elif chunk_json["type"] == "message_delta":
+                        completion_tokens = chunk_json["usage"]["output_tokens"]
+        except Exception as ex:
+            logger.error(f"Error at to_accesslog: {ex}\n{traceback.format_exc()}")
 
         return accesslog_cls(
             request_id=self.request_id,
             created_at=datetime.utcnow(),
-            direction="error" if self.response_headers.get("x-amzn-errortype") else "response",
+            direction="response",
             status_code=self.status_code,
-            content=response_content,
+            content=response_text,
             function_call=None,
             tool_calls=None,
-            raw_body=json.dumps(chunk_jsons, ensure_ascii=False),
+            raw_body=self.response_content,
             raw_headers=json.dumps(self.response_headers, ensure_ascii=False),
-            model="anthropic.claude-v2",
+            model=model,
             prompt_tokens=prompt_tokens,
             completion_tokens=completion_tokens,
             request_time=self.duration,
             request_time_api=self.duration_api
         )
 
 
-class Claude2ErrorItem(ErrorItemBase):
+class ClaudeErrorItem(SessionErrorItemBase):
     ...
 
 
-queue_item_types = [Claude2RequestItem, Claude2ResponseItem, Claude2StreamResponseItem, Claude2ErrorItem]
+queue_item_types = [ClaudeRequestItem, ClaudeResponseItem, ClaudeStreamResponseItem, ClaudeErrorItem]
 
 
-# Reverse proxy application for Claude2 on AWS Bedrock
-class Claude2Proxy(ProxyBase):
+# Reverse proxy application for Anthropic Claude3 API
+class BedrockClaudeProxy(HTTPXProxy):
     def __init__(
         self,
         *,
         aws_access_key_id: str = None,
         aws_secret_access_key: str = None,
         region_name: str = None,
         timeout=60.0,
         request_filters: List[RequestFilterBase] = None,
         response_filters: List[ResponseFilterBase] = None,
+        request_item_class: type = ClaudeRequestItem,
+        response_item_class: type = ClaudeResponseItem,
+        stream_response_item_class: type = ClaudeStreamResponseItem,
+        error_item_class: type = ClaudeErrorItem,
         access_logger_queue: QueueClientBase
     ):
         super().__init__(
+            timeout=timeout,
             request_filters=request_filters,
             response_filters=response_filters,
+            request_item_class=request_item_class,
+            response_item_class=response_item_class,
+            stream_response_item_class=stream_response_item_class,
+            error_item_class=error_item_class,
             access_logger_queue=access_logger_queue
         )
 
-        self.aws_access_key_id = aws_access_key_id
-        self.aws_secret_access_key = aws_secret_access_key
-        self.region_name = region_name
-        self.aws_url = f"https://bedrock-runtime.{self.region_name}.amazonaws.com"
+        self.api_base_url = f"https://bedrock-runtime.{region_name}.amazonaws.com"
+        self.api_chat_resource_path = "/model/{model_and_method:path}"
+        self.api_service_id = "bedrock-claude"
 
-        # AWS credentials
         self.authorizer = SigV4Auth(
             credentials=Credentials(
-                access_key=self.aws_access_key_id,
-                secret_key=self.aws_secret_access_key
+                access_key=aws_access_key_id,
+                secret_key=aws_secret_access_key
             ),
             service_name="bedrock",
-            region_name=self.region_name
+            region_name=region_name
         )
 
-        # HTTP Client (should close on end)
-        self.http_client = httpx.AsyncClient(timeout=timeout)
+    def text_to_response_json(self, text: str) -> dict:
+        return {
+            "content": [{"type": "text", "text": text}],
+            "usage": {"input_tokens": 0, "output_tokens": 0}
+        }
 
-    async def filter_request(self, request_id: str, request_json: dict, request_headers: dict, stream: bool) -> Union[dict, JSONResponse]:
+    async def filter_request(self, session: SessionInfo) -> Union[None, JSONResponse]:
         for f in self.request_filters:
-            if completion_content := await f.filter(request_id, request_json, request_headers):
-                # Return response if filter returns JsonResponse
-                resp_for_log = {
-                    "completion": completion_content
-                }
+            if completion_content := await f.filter(session.request_id, session.request_json, session.request_headers):
+                # Make JsonResponse when filter returns content
+                session.response_json = self.text_to_response_json(completion_content)
+                json_response = JSONResponse(session.response_json)
+                self.add_response_headers(json_response, session.request_id)
+                session.response_headers = dict(json_response.headers)
+
                 # Response log
-                self.access_logger_queue.put(Claude2ResponseItem(
-                    request_id=request_id,
-                    response_json=resp_for_log,
-                    response_headers={
-                        "x-amzn-bedrock-input-token-count": 0,
-                        "x-amzn-bedrock-output-token-count": 0
-                    },
-                    status_code=400 if stream else 200
-                ))
-
-                if stream:
-                    logger.warning("Claude2Proxy doesn't support instant reply from RequestFilter. Return message as 400 bad request.")
-                    return self.return_response_with_headers(JSONResponse({"message": completion_content}, status_code=400), request_id)
-                else:
-                    return self.return_response_with_headers(JSONResponse(resp_for_log), request_id)
+                self.access_logger_queue.put(
+                    self.response_item_class.from_session(session=session)
+                )
+
+                # Return response
+                if session.stream:
+                    logger.warning("ClaudeProxy for Bedrock doesn't support instant reply from RequestFilter in stream mode. Return message as 400 bad request.")
+                    json_response.status_code = 400
 
-        return request_json
+                return json_response
 
-    async def filter_response(self, request_id: str, response_json: dict) -> dict:
-        for f in self.response_filters:
-            if immediately_return_json_resp := await f.filter(request_id, response_json):
-                return immediately_return_json_resp
+        return None
 
-        return response_json
+    async def parse_request(self, fastapi_request: Request, session: SessionInfo):
+        await super().parse_request(fastapi_request, session)
+        session.stream = "invoke-with-response-stream" in str(session.request_url)
+        session.extra_info["model"] = re.search(r"model/(.*?)/", session.request_url).group(1)
 
-    def get_aws_request_header_with_cred(self, url: str, bedrock_params: dict):
+    def get_aws_request_header_with_cred(self, url: str, request_headers: dict, bedrock_params: dict):
         ar = AWSRequest(
             method="POST",
             url=url,
-            headers={
-                "Content-Type": "application/json",
-                "X-Amzn-Bedrock-Accept": "application/json",
-            },
+            headers=request_headers,
             data=json.dumps(bedrock_params).encode()
         )
         self.authorizer.add_auth(ar)
         ar.prepare()
         return ar.headers
 
-    def return_response_with_headers(self, resp: Response, request_id: str):
-        self.add_response_headers(response=resp, request_id=request_id)
-        return resp
-
-    def add_route(self, app: FastAPI, base_url: str):
-        @app.post(base_url + "/{invoke_method}")
-        async def handle_request(request: Request, invoke_method: str):
-            request_id = str(uuid4())
+    def prepare_httpx_request_headers(self, session: SessionInfo):
+        super().prepare_httpx_request_headers(session)
 
+        # Remove headers to prevent signature error
+        if "authorization" in session.request_headers:
+            del session.request_headers["authorization"]
+        if "connection" in session.request_headers:
+            del session.request_headers["connection"]
+
+        # Add AWS Authorization header
+        session.request_headers["authorization"] = \
+            self.get_aws_request_header_with_cred(
+                self.make_url(session),
+                session.request_headers,
+                session.request_json
+            )["authorization"]
+
+    def make_url(self, session: SessionInfo):
+        return f"{self.api_base_url}/model/{session.extra_info['model']}/{('invoke-with-response-stream' if session.stream else 'invoke')}"
+
+    def make_stream_response(self, async_client: httpx.AsyncClient, stream_response: httpx.Response, session: SessionInfo):
+        async def process_stream():
+            session.extra_info["response_events"] = []
             try:
-                start_time = time.time()
-                request_json = await request.json()
-                request_headers = dict(request.headers.items())
-
-                # Log request
-                self.access_logger_queue.put(Claude2RequestItem(
-                    request_id=request_id,
-                    request_json=request_json,
-                    request_headers=request_headers
-                ))
-
-                # Filter request
-                request_json = await self.filter_request(request_id, request_json, request_headers, invoke_method == "invoke-with-response-stream")
-                if isinstance(request_json, JSONResponse):
-                    return request_json
-
-                # Call API and handling response from API
-                url = f"{self.aws_url}/model/anthropic.claude-v2/{invoke_method}"
-                aws_request_header = self.get_aws_request_header_with_cred(url, request_json)
-                start_time_api = time.time()
-
-                if invoke_method == "invoke-with-response-stream":
-                    async def process_stream(stream_response: httpx.Response, status_code: int):
-                        try:
-                            async for chunk in stream_response.aiter_raw():
-                                # Parse JSON data from bytes chunk
-                                for m in re.findall(rb"event\{.*?\}", chunk):
-                                    b64bytes = json.loads(m[5:].decode("utf-8"))["bytes"]
-                                    chunk_json = json.loads(base64.b64decode(b64bytes).decode())
-                                    self.access_logger_queue.put(Claude2StreamResponseItem(
-                                        request_id=request_id,
-                                        chunk_json=chunk_json
-                                    ))
-
-                                yield chunk
-
-                            # Add hearedes for log
-                            self.return_response_with_headers(stream_response, request_id)
-
-                        finally:
-                            # Response log
-                            now = time.time()
-                            self.access_logger_queue.put(Claude2StreamResponseItem(
-                                request_id=request_id,
-                                response_headers=dict(stream_response.headers.items()),
-                                duration=now - start_time,
-                                duration_api=now - start_time_api,
-                                request_json=request_json,
-                                status_code=status_code
-                            ))
-
-                    stream_request = httpx.Request(method="POST", url=url, headers=dict(aws_request_header), json=request_json)
-                    stream_response = await self.http_client.send(request=stream_request, stream=True)
-
-                    # DO NOT raise status error here to return error info in stream
-
-                    return self.return_response_with_headers(StreamingResponse(
-                        process_stream(stream_response, stream_response.status_code),
-                        status_code=stream_response.status_code,
-                        headers=stream_response.headers
-                    ), request_id)
-
-                else:
-                    completion_response = await self.http_client.post(url=url, headers=dict(aws_request_header), json=request_json)
-                    completion_response.raise_for_status()
-
-                    duration_api = time.time() - start_time_api
-                    response_json = completion_response.json()
-
-                    # Filter response
-                    original_response_json = response_json.copy()
-                    filtered_response_json = await self.filter_response(request_id, response_json)
-
-                    # Make JSON response
-                    if original_response_json != filtered_response_json:
-                        json_response = JSONResponse(original_response_json, completion_response.status_code, completion_response.headers)
-                    else:
-                        # Remove incorrect content-length
-                        completion_response.headers.pop("Content-Length")
-                        json_response = JSONResponse(filtered_response_json, completion_response.status_code, completion_response.headers)
-
-                    self.add_response_headers(json_response, request_id)
-
-                    # Response log
-                    self.access_logger_queue.put(Claude2ResponseItem(
-                        request_id=request_id,
-                        response_json=filtered_response_json,
-                        response_headers=dict(json_response.headers.items()),
-                        duration=time.time() - start_time,
-                        duration_api=duration_api,
-                        status_code=completion_response.status_code
-                    ))
-
-                    return json_response
-
-            # Error handlers
-            except RequestFilterException as rfex:
-                logger.error(f"Request filter error: {rfex}\n{traceback.format_exc()}")
-
-                resp_json = {"error": {"message": rfex.message, "type": "request_filter_error", "param": None, "code": None}}
-
-                # Error log
-                self.access_logger_queue.put(Claude2ErrorItem(
-                    request_id=request_id,
-                    exception=rfex,
-                    traceback_info=traceback.format_exc(),
-                    response_json=resp_json,
-                    status_code=rfex.status_code
-                ))
-
-                return self.return_response_with_headers(JSONResponse(resp_json, status_code=rfex.status_code), request_id)
-
-            except ResponseFilterException as rfex:
-                logger.error(f"Response filter error: {rfex}\n{traceback.format_exc()}")
-
-                resp_json = {"error": {"message": rfex.message, "type": "response_filter_error", "param": None, "code": None}}
-
-                # Error log
-                self.access_logger_queue.put(Claude2ErrorItem(
-                    request_id=request_id,
-                    exception=rfex,
-                    traceback_info=traceback.format_exc(),
-                    response_json=resp_json,
-                    status_code=rfex.status_code
-                ))
-
-                return self.return_response_with_headers(JSONResponse(resp_json, status_code=rfex.status_code), request_id)
-
-            except httpx.HTTPStatusError as htex:
-                logger.error(f"Error at server: {htex}\n{traceback.format_exc()}")
-
-                # Error log
+                # Yield chunked responses
+                async for b in stream_response.aiter_raw():
+                    session.extra_info["response_events"].append(b)
+                    yield b
+            
+            finally:
+                # Make response log
                 try:
-                    resp_json = htex.response.json()
-                except:
-                    try:
-                        resp_json = str(await htex.response.aread())
-                    except:
-                        logger.warning("Error")
-
-                self.access_logger_queue.put(Claude2ErrorItem(
-                    request_id=request_id,
-                    exception=htex,
-                    traceback_info=traceback.format_exc(),
-                    response_json=resp_json,
-                    status_code=htex.response.status_code
-                ))
-
-                htex.response.headers.pop("content-length")
-
-                return self.return_response_with_headers(JSONResponse(
-                    resp_json,
-                    status_code=htex.response.status_code,
-                    headers=htex.response.headers
-                ), request_id)
-
-            except Exception as ex:
-                logger.error(f"Error at server: {ex}\n{traceback.format_exc()}")
-
-                resp_json = {"error": {"message": "Proxy error", "type": "proxy_error", "param": None, "code": None}}
-
-                # Error log
-                self.access_logger_queue.put(Claude2ErrorItem(
-                    request_id=request_id,
-                    exception=ex,
-                    traceback_info=traceback.format_exc(),
-                    response_json=resp_json,
-                    status_code=502
-                ))
-
-                return self.return_response_with_headers(JSONResponse(resp_json, status_code=502), request_id)
+                    now = time.time()
+                    session.duration = now - session.start_time
+                    session.duration_api = now - session.start_time_api
+                    self.access_logger_queue.put(
+                        self.stream_response_item_class.from_session(session)
+                    )
+
+                except Exception as ex:
+                    logger.error(f"Failed in making log items: {ex}\n{traceback.format_exc()}")
+                    logger.error(f"response_content: {session.response_body}")
+                
+                finally:
+                    await async_client.aclose()
+
+        return StreamingResponse(
+            process_stream(),
+            status_code=session.status_code,
+            headers=session.response_headers
+        )
```

## Comparing `aiproxy_python-0.4.2.dist-info/LICENSE` & `aiproxy_python-0.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiproxy_python-0.4.2.dist-info/METADATA` & `aiproxy_python-0.4.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiproxy-python
-Version: 0.4.2
+Version: 0.4.3
 Summary: 🦉AIProxy is a reverse proxy for ChatGPT API that provides monitoring, logging, and filtering requests and responses.
 Home-page: https://github.com/uezo/aiproxy
 Author: uezo
 Author-email: uezo@uezo.net
 Maintainer: uezo
 Maintainer-email: uezo@uezo.net
 License: Apache v2
@@ -399,60 +399,69 @@
 connection_str = f"mssql+pyodbc:///?odbc_connect=DRIVER={ODBC Driver 18 for SQL Server};SERVER=YOUR_SERVER;PORT=1433;DATABASE=YOUR_DB;UID=YOUR_UID;PWD=YOUR_PWD"
 
 worker = AccessLogWorker(connection_str=connection_str)
 ```
 
 ### Azure OpenAI
 
-**up to version 0.3.6. We are now updating🖊️**
-
-To use Azure OpenAI, instantiate `ChatGPTProxy` with `AsyncAzureOpenAI`.
+To use Azure OpenAI, use `AzureOpenAIProxy` instead of `ChatGPTProxy`.
 
 ```python
-azure_client = openai.AsyncAzureOpenAI(
-    api_key = "YOUR_API_KEY",
-    api_version = "2023-10-01-preview",
-    azure_endpoint = "https://{DEPLOYMENT_ID}.openai.azure.com/"
-)
+from aiproxy.chatgpt import AzureOpenAIProxy
 
-proxy = ChatGPTProxy(async_client=azure_client, access_logger_queue=worker.queue_client)
+aoai_proxy = AzureOpenAIProxy(
+    api_key="YOUR_API_KEY",
+    resource_name="YOUR_RESOURCE_NAME",
+    deployment_id="YOUR_DEPLOYMENT_ID",
+    api_version="2024-02-01",   # https://learn.microsoft.com/ja-jp/azure/ai-services/openai/reference#chat-completions
+    access_logger_queue=worker.queue_client
+)
+aoai_proxy.add_route(app)
 ```
 
-### Amazon Bedrock
+Clients do not need to be aware that it is Azure OpenAI; use the same code for ChatGPT API.
+
 
-**up to version 0.3.6. We are now updating🖊️**
+### Amazon Bedrock
 
-To use Claude2 on Amazon Bedrock, instantiate `Claude2Proxy`.
+To use Claude on Amazon Bedrock, use `BedrockClaudeProxy` instead of `ClaudeProxy`.
 
 ```python
-from aiproxy.claude2 import Claude2Proxy
-claude_proxy = Claude2Proxy(
+from aiproxy.bedrock_claude import BedrockClaudeProxy
+
+bedrock_claude_proxy = BedrockClaudeProxy(
     aws_access_key_id="YOUR_AWS_ACCESS_KEY_ID",
     aws_secret_access_key="YOUR_AWS_SECRET_ACCESS_KEY",
-    region_name="your-bedrock-region",
+    region_name="YOUR_REGION",
     access_logger_queue=worker.queue_client
 )
-claude_proxy.add_route(app, "/model/anthropic.claude-v2")
+bedrock_claude_proxy.add_route(app)
 ```
 
-Client side. We test API with boto3.
+
+Client side. We test API with `AnthropicBedrock`.
 
 ```python
-import boto3
-import json
-# Make client with dummy creds
-session = boto3.Session(aws_access_key_id="dummy", aws_secret_access_key="dummy",)
-bedrock = session.client(service_name="bedrock-runtime", region_name="private", endpoint_url="http://127.0.0.1:8000")
-# Call API
-response = bedrock.invoke_model(
-    modelId="anthropic.claude-v2",
-    body=json.dumps({"prompt": "Human: うなぎとあなごの違いは？\nAssistant: ", "max_tokens_to_sample": 100})
+# Make client with `base_url`
+client = anthropic.AnthropicBedrock(
+    aws_secret_key="dummy_aws_secret_access_key",
+    aws_access_key="dummy_aws_access_key_id",
+    aws_region="dummy_region_name",
+    base_url="http://127.0.0.1:8000/bedrock-claude"
 )
-# Show response
-print(json.loads(response["body"].read()))
+
+resp = client.messages.create(
+    model="anthropic.claude-3-haiku-20240307-v1:0",
+    messages=[{"role": "user", "content": [{"type": "text", "text": "こんにちは！"}]}],
+    max_tokens=512,
+    stream=True
+)
+
+for r in resp:
+    print(r)
 ```
 
 
 ## 🛟 Support
 
 For support, questions, or contributions, please open an issue in the GitHub repository. Please contact me directly when you need an enterprise or business support😊.
```

## Comparing `aiproxy_python-0.4.2.dist-info/RECORD` & `aiproxy_python-0.4.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-aiproxy/__init__.py,sha256=2Ie1ECHoAH_8EibDC6CPO93hVnAybJvArevl4UF-HtY,540
+aiproxy/__init__.py,sha256=zS_eN67lWhu4H9gqmcthPYznepLzzjcl3z7qB261_-Y,540
 aiproxy/__main__.py,sha256=YhGpey2hGBaMaNjrB5tKITdaY2wXFOQaUvnn6m1Z09g,2414
 aiproxy/accesslog.py,sha256=YmpQpOR9vYDkTq32PqiEsIlzxb7rnIetrGd7SJR38tU,7728
 aiproxy/anthropic_claude.py,sha256=4zuX-7Bh3R3BRw6eXJXObr0cPkvjk3nRcHz0UNqm0C4,7318
 aiproxy/azurequeueclient.py,sha256=uhQNH4ZSlUcFppE2_IB7HG0Hsvf2ZqGgrrJ1D1Pheqk,1337
+aiproxy/bedrock_claude.py,sha256=R3ZXJ_WdLSGPoDzXZ3imq-1e1bhYPhcwc73-bxsaF-o,11137
 aiproxy/chatgpt.py,sha256=6DFfzCDuFslL98Srh-kyoMN7ssl2PlXwE2L3CwkLqyM,13037
-aiproxy/claude2.py,sha256=MIhInTap6BQ_8pfKsSt5gCzgRObiaviSHgVaIh35iYU,16284
 aiproxy/gemini.py,sha256=KQImlmeXdwffMfpv_UR2mDozDb9C8YZB9W2fKZ1G_T8,11392
 aiproxy/httpx_proxy.py,sha256=2ptvCeX7cam6_6WHOn2mNHo9YhlG1vIQ-S2yi8hrhI8,21761
 aiproxy/proxy.py,sha256=nUMqvcH0wQQu6OsJpQTNMmIuZ0jVpzzjmOoTMCnUPRk,2165
 aiproxy/queueclient.py,sha256=TKPYRWWmKX-3e0FnMkkiuQOKvjxI-ak8-Q6XrZIJ19Y,731
-aiproxy_python-0.4.2.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
-aiproxy_python-0.4.2.dist-info/METADATA,sha256=InF3TtEKc-EQR659cDyQs9amEucJcpQLft94jSMBHzQ,14231
-aiproxy_python-0.4.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-aiproxy_python-0.4.2.dist-info/top_level.txt,sha256=QdyikybYJCoUrciRj-u1dOhyN3X7K49bma7UAjrvnmo,8
-aiproxy_python-0.4.2.dist-info/RECORD,,
+aiproxy_python-0.4.3.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
+aiproxy_python-0.4.3.dist-info/METADATA,sha256=6dfpOSDncy3kpdxCnTxYKYPUoVyjcMPEIz-gtTESGro,14341
+aiproxy_python-0.4.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+aiproxy_python-0.4.3.dist-info/top_level.txt,sha256=QdyikybYJCoUrciRj-u1dOhyN3X7K49bma7UAjrvnmo,8
+aiproxy_python-0.4.3.dist-info/RECORD,,
```

