# Comparing `tmp/elia_chat-0.4.1.tar.gz` & `tmp/elia_chat-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elia_chat-0.4.1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `elia_chat-0.4.1.tar` & `elia_chat-1.0.0b1.tar`

### file list

```diff
@@ -1,24 +1,39 @@
--rw-r--r--   0        0        0     2190 2023-09-22 22:50:29.474172 elia_chat-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-04-04 16:19:27.149530 elia_chat-0.4.1/elia_chat/__init__.py
--rw-r--r--   0        0        0     2160 2023-11-14 20:20:13.145296 elia_chat-0.4.1/elia_chat/__main__.py
--rw-r--r--   0        0        0      678 2023-09-22 22:50:29.477552 elia_chat-0.4.1/elia_chat/app.py
--rw-r--r--   0        0        0     2680 2023-11-14 20:20:18.600897 elia_chat-0.4.1/elia_chat/chats_manager.py
--rw-r--r--   0        0        0        0 2023-07-28 16:46:45.256896 elia_chat-0.4.1/elia_chat/database/__init__.py
--rw-r--r--   0        0        0     2211 2023-11-14 20:20:18.601644 elia_chat-0.4.1/elia_chat/database/converters.py
--rw-r--r--   0        0        0      201 2023-07-28 16:46:45.257828 elia_chat-0.4.1/elia_chat/database/create_database.py
--rw-r--r--   0        0        0     1977 2023-06-09 20:15:04.805077 elia_chat-0.4.1/elia_chat/database/import_chatgpt.py
--rw-r--r--   0        0        0     2524 2023-11-14 20:20:18.602509 elia_chat-0.4.1/elia_chat/database/models.py
--rw-r--r--   0        0        0     5665 2023-12-18 23:55:49.577989 elia_chat-0.4.1/elia_chat/elia.scss
--rw-r--r--   0        0        0     1619 2023-11-14 20:20:18.603031 elia_chat-0.4.1/elia_chat/models.py
--rw-r--r--   0        0        0     4413 2023-11-14 20:20:18.604094 elia_chat-0.4.1/elia_chat/screens/chat_screen.py
--rw-r--r--   0        0        0     2388 2023-11-14 20:20:18.604672 elia_chat-0.4.1/elia_chat/screens/message_info_modal.py
--rw-r--r--   0        0        0      801 2023-11-14 20:20:13.150017 elia_chat-0.4.1/elia_chat/time_display.py
--rw-r--r--   0        0        0      286 2023-05-23 21:08:47.713606 elia_chat-0.4.1/elia_chat/widgets/agent_is_typing.py
--rw-r--r--   0        0        0    14391 2023-11-14 20:20:18.605873 elia_chat-0.4.1/elia_chat/widgets/chat.py
--rw-r--r--   0        0        0      877 2023-05-27 16:37:32.190885 elia_chat-0.4.1/elia_chat/widgets/chat_header.py
--rw-r--r--   0        0        0     4563 2023-07-28 16:57:25.646333 elia_chat-0.4.1/elia_chat/widgets/chat_list.py
--rw-r--r--   0        0        0     5404 2023-11-14 20:20:18.606476 elia_chat-0.4.1/elia_chat/widgets/chat_options.py
--rw-r--r--   0        0        0     1977 2023-11-14 20:20:18.607353 elia_chat-0.4.1/elia_chat/widgets/chatbox.py
--rw-r--r--   0        0        0     1446 2023-05-31 20:48:24.143848 elia_chat-0.4.1/elia_chat/widgets/token_analysis.py
--rw-r--r--   0        0        0      732 2023-12-18 23:56:05.208628 elia_chat-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 elia_chat-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/.python-version
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/requirements-dev.lock
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/requirements.lock
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/__init__.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/__main__.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/app.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/chats_manager.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/config.py
+-rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/elia.scss
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/launch_args.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/locations.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/models.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/runtime_config.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/time_display.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/database/__init__.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/database/converters.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/database/database.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/database/import_chatgpt.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/database/models.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/screens/chat_details.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/screens/chat_screen.py
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/screens/help_screen.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/screens/home_screen.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/agent_is_typing.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/app_header.py
+-rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/chat.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/chat_header.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/chat_list.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/chat_options.py
+-rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/chatbox.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/prompt_input.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/token_analysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/tests/__init__.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/.gitignore
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/README.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/PKG-INFO
```

### Comparing `elia_chat-0.4.1/elia_chat/database/import_chatgpt.py` & `elia_chat-1.0.0b1/elia_chat/database/import_chatgpt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,85 @@
 import json
 from datetime import datetime
 from pathlib import Path
 
-from sqlalchemy.orm import Session
+from rich.console import Console
+from rich.live import Live
+from rich.text import Text
 
-from elia_chat.database.models import MessageDao, ChatDao, engine
+from elia_chat.database.database import get_session
+from elia_chat.database.models import MessageDao, ChatDao
 
 
-def import_chatgpt_data(file: Path) -> None:
-    # Load the JSON data
+async def import_chatgpt_data(file: Path) -> None:
+    console = Console()
+
     with open(file, "r") as f:
         data = json.load(f)
 
-    # Create a new session
-    session = Session(engine)
+    console.print("[green]Loaded and parsed JSON.")
 
-    # Iterate over each chat in the data
-    for chat_data in data:
-        # Create a new ChatDao instance and add it to the session
-        chat = ChatDao(
-            model=None, started_at=datetime.fromtimestamp(chat_data["create_time"])
+    def output_progress(
+        imported_count: int, total_count: int, message_count: int
+    ) -> Text:
+        style = "green" if imported_count == total_count else "yellow"
+        return Text.from_markup(
+            f"Imported [b]{imported_count}[/] of [b]{total_count}[/] chats.\n"
+            f"[b]{message_count}[/] messages in total.",
+            style=style,
         )
-        session.add(chat)
-        session.commit()  # Make sure to commit so that chat.id is assigned
 
-        for message_id, message_data in chat_data["mapping"].items():
-            message_info = message_data.get("message")
-            if message_info:
-                metadata = message_info.get("metadata", {})
-                if metadata:
-                    model = metadata.get("model_slug")
-                    if model is not None:
-                        chat.model = model
-                        session.add(chat)
-                        session.commit()
-
-                message = MessageDao(
-                    chat_id=chat.id,
-                    role=message_info["author"]["role"],
-                    content=message_info["content"]["parts"][0],
-                    timestamp=datetime.fromtimestamp(message_info["create_time"]),
-                    status=message_info.get("status"),
-                    end_turn=message_info.get("end_turn"),
-                    weight=message_info.get("weight"),
-                    meta=metadata,
-                    recipient=message_info.get("recipient"),
+    message_count = 0
+    with Live(output_progress(0, len(data), message_count)) as live:
+        async with get_session() as session:
+            for chat_number, chat_data in enumerate(data, start=1):
+                chat = ChatDao(
+                    title=chat_data.get("title"),
+                    model="gpt-3.5-turbo",
+                    started_at=datetime.fromtimestamp(
+                        chat_data.get("create_time", 0) or 0
+                    ),
                 )
-                session.add(message)
-
-        session.commit()
+                session.add(chat)
+                await (
+                    session.commit()
+                )  # Make sure to commit so that chat.id is assigned
+
+                for _message_id, message_data in chat_data["mapping"].items():
+                    message_info = message_data.get("message")
+                    if message_info:
+                        metadata = message_info.get("metadata", {})
+                        model = "gpt-3.5-turbo"
+                        if metadata:
+                            model = metadata.get("model_slug")
+                            chat.model = (
+                                "gpt-4-turbo" if model == "gpt-4" else "gpt-3.5-turbo"
+                            )
+                            session.add(chat)
+                            await session.commit()
+
+                        role = message_info["author"]["role"]
+                        chat_id = chat.id
+                        message = MessageDao(
+                            chat_id=chat_id,
+                            role=role,
+                            content=str(message_info["content"].get("parts", [""])[0]),
+                            timestamp=datetime.fromtimestamp(
+                                message_info.get("create_time", 0) or 0
+                            ),
+                            model=model,
+                            meta=metadata,
+                        )
+                        session.add(message)
+                        message_count += 1
+                        live.update(
+                            output_progress(chat_number, len(data), message_count)
+                        )
 
-    # Close the session when you're done
-    session.close()
+                await session.commit()
 
 
 if __name__ == "__main__":
     path = Path("resources/conversations.json")
-    import_chatgpt_data(path)
+    import asyncio
+
+    asyncio.run(import_chatgpt_data(path))
```

### Comparing `elia_chat-0.4.1/elia_chat/models.py` & `elia_chat-1.0.0b1/elia_chat/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,75 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from datetime import datetime
-from typing import Optional
+from datetime import UTC, datetime
+from typing import TYPE_CHECKING
 
-from langchain.schema import BaseMessage
 
-from elia_chat.widgets.chat_options import GPTModel, MODEL_MAPPING, DEFAULT_MODEL
+from elia_chat.config import LaunchConfig, EliaChatModel
+
+if TYPE_CHECKING:
+    from litellm.types.completion import ChatCompletionMessageParam
+
+
+class UnknownModel(EliaChatModel):
+    pass
+
+
+def get_model_by_name(model_name: str, config: LaunchConfig) -> EliaChatModel:
+    """Given the name of a model as a string, return the EliaChatModel."""
+    try:
+        return {model.name: model for model in config.all_models}[model_name]
+    except KeyError:
+        return UnknownModel(name=model_name)
+
+
+@dataclass
+class ChatMessage:
+    message: ChatCompletionMessageParam
+    timestamp: datetime | None
+    model: str
 
 
 @dataclass
 class ChatData:
-    id: str | None
+    id: int | None  # Can be None before the chat gets assigned ID from database.
     model_name: str
     title: str | None
-    create_timestamp: float | None
-    messages: list[BaseMessage]
+    create_timestamp: datetime | None
+    messages: list[ChatMessage]
 
     @property
     def short_preview(self) -> str:
-        first_user_message = self.first_user_message
-        if first_user_message is None:
-            return "Empty chat..."
-        first_content = first_user_message.content or ""
-        return first_content[:24] + "..."
+        first_message = self.first_user_message.message
 
-    @property
-    def first_user_message(self) -> BaseMessage | None:
-        return self.messages[1] if len(self.messages) > 1 else None
+        if "content" in first_message:
+            first_message = first_message["content"]
+            # We have content, but it's not guaranteed to be a string quite yet.
+            # In the case of tool calls or image generation requests, we can
+            # have non-string types here. We're not handling/considering this atm.
+            if first_message and isinstance(first_message, str):
+                if len(first_message) > 77:
+                    return first_message[:77] + "..."
+                else:
+                    return first_message
 
-    @property
-    def non_system_messages(self) -> list[BaseMessage]:
-        return self.messages[1:]
+        return ""
 
     @property
-    def create_time(self) -> datetime:
-        return datetime.fromtimestamp(self.create_timestamp or 0).astimezone()
+    def system_prompt(self) -> ChatMessage:
+        return self.messages[0]
 
     @property
-    def update_time(self) -> datetime:
-        return datetime.fromtimestamp(
-            self.messages[-1].get("timestamp", 0) if self.messages else 0
-        )
+    def first_user_message(self) -> ChatMessage:
+        return self.messages[1]
 
-
-@dataclass
-class EliaContext:
-    """
-    Elia Context
-    """
-
-    chat_message: Optional[str] = None
-    model_name: str = DEFAULT_MODEL.name
+    @property
+    def non_system_messages(
+        self,
+    ) -> list[ChatMessage]:
+        return self.messages[1:]
 
     @property
-    def gpt_model(self) -> GPTModel:
-        gpt_model = MODEL_MAPPING.get(self.model_name)
-        if gpt_model is None:
-            raise ValueError(f"Unknown model name: {self.model_name}")
-        return gpt_model
+    def update_time(self) -> datetime:
+        message_timestamp = self.messages[-1].timestamp
+        return message_timestamp.astimezone().replace(tzinfo=UTC)
```

### Comparing `elia_chat-0.4.1/elia_chat/time_display.py` & `elia_chat-1.0.0b1/elia_chat/time_display.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from datetime import datetime, timezone
 
 
-def format_timestamp(timestamp: float) -> str:
-    """Convert a Unix timestamp into a string in human-readable format.
+def format_timestamp(dt: datetime) -> str:
+    """Convert a datetime into the local timezone and format it.
 
     Args:
-        timestamp: The Unix timestamp.
+        dt: The datetime object to format.
 
     Returns:
         The string timestamp in the format "%Y-%m-%d %H:%M:%S".
     """
-    utc_dt = datetime.fromtimestamp(timestamp, timezone.utc)
-    local_dt = utc_dt.astimezone()
+    local_dt = convert_to_local(dt)
     return local_dt.strftime("%Y-%m-%d %H:%M:%S")
 
 
 def convert_to_local(utc_dt: datetime) -> datetime:
     """Given a UTC datetime, return a datetime in the local timezone."""
     local_dt_now = datetime.now()
     local_tz = local_dt_now.astimezone().tzinfo
```

### Comparing `elia_chat-0.4.1/elia_chat/widgets/chat.py` & `elia_chat-1.0.0b1/elia_chat/widgets/chat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,395 +1,305 @@
 from __future__ import annotations
 
-import os
-import time
+import datetime
 from dataclasses import dataclass
+from typing import TYPE_CHECKING, cast
 
-from langchain.chat_models.base import BaseChatModel
-from langchain.llms.base import LLM
-from langchain.schema import (
-    AIMessage,
-    BaseMessage,
-    HumanMessage,
-    SystemMessage,
-)
-from langchain.schema.messages import BaseMessageChunk
 from textual import log, on, work, events
 from textual.app import ComposeResult
-from textual.containers import ScrollableContainer, Vertical, VerticalScroll
+from textual.binding import Binding
+from textual.containers import VerticalScroll
+from textual.css.query import NoMatches
 from textual.message import Message
 from textual.reactive import reactive
 from textual.widget import Widget
-from textual.widgets import Input
 
 from elia_chat.chats_manager import ChatsManager
-from elia_chat.models import ChatData, EliaContext
+from elia_chat.models import ChatData, ChatMessage
+from elia_chat.screens.chat_details import ChatDetails
 from elia_chat.widgets.agent_is_typing import AgentIsTyping
 from elia_chat.widgets.chat_header import ChatHeader
-from elia_chat.widgets.chat_options import (
-    DEFAULT_MODEL,
-    MODEL_MAPPING,
-    ChatOptions,
-    GPTModel,
+from elia_chat.widgets.prompt_input import PromptInput
+from elia_chat.models import (
+    EliaChatModel,
+    get_model_by_name,
 )
 from elia_chat.widgets.chatbox import Chatbox
 
 
+if TYPE_CHECKING:
+    from elia_chat.app import Elia
+    from litellm.types.completion import (
+        ChatCompletionUserMessageParam,
+        ChatCompletionAssistantMessageParam,
+    )
+
+
 class Chat(Widget):
+    BINDINGS = [
+        Binding("escape", "close", "Close", key_display="esc"),
+        Binding("shift+down", "scroll_container_down", show=False),
+        Binding("shift+up", "scroll_container_up", show=False),
+        Binding(
+            key="g",
+            action="focus_first_message",
+            description="First message",
+            key_display="g",
+            show=False,
+        ),
+        Binding(
+            key="G",
+            action="focus_latest_message",
+            description="Latest message",
+            show=False,
+        ),
+        Binding(key="f2", action="details", description="Chat info"),
+    ]
+
     allow_input_submit = reactive(True)
     """Used to lock the chat input while the agent is responding."""
 
-    def __init__(self) -> None:
+    def __init__(self, chat_data: ChatData) -> None:
         super().__init__()
-
-        self.persona_directive = os.getenv(
-            "ELIA_DIRECTIVE", "You are a helpful assistant."
-        )
-        # The thread initially only contains the system message.
-        self.chat_container: ScrollableContainer | None = None
-        self.chat_options: ChatOptions | None = None
-        self.chat_data = ChatData(
-            id=None,
-            title=None,
-            create_timestamp=None,
-            model_name=DEFAULT_MODEL.name,
-            messages=[
-                SystemMessage(
-                    content=self.persona_directive,
-                    additional_kwargs={
-                        "timestamp": time.time(),
-                        "status": None,
-                        "end_turn": None,
-                        "weight": None,
-                        "metadata": None,
-                        "recipient": "all",
-                    },
-                )
-            ],
-        )
+        self.chat_data = chat_data
+        self.elia = cast("Elia", self.app)
+        self.model = get_model_by_name(chat_data.model_name, self.elia.launch_config)
 
     @dataclass
     class AgentResponseStarted(Message):
         pass
 
     @dataclass
     class AgentResponseComplete(Message):
-        chat_id: str | None
-        message: BaseMessage
+        chat_id: int | None
+        message: ChatMessage
+        chatbox: Chatbox
 
     @dataclass
     class FirstMessageSent(Message):
         chat_data: ChatData
 
     @dataclass
-    class SavedChatLoaded(Message):
-        chat_data: ChatData
-
-    @dataclass
     class UserMessageSubmitted(Message):
-        chat_id: str
-        message: BaseMessage
+        chat_id: int
+        message: ChatMessage
+
+    def compose(self) -> ComposeResult:
+        yield ChatHeader(chat=self.chat_data, model=self.model)
+
+        with VerticalScroll(id="chat-container") as vertical_scroll:
+            vertical_scroll.can_focus = False
+
+        yield PromptInput(id="prompt")
+        yield AgentIsTyping()
+
+    async def on_mount(self, _: events.Mount) -> None:
+        """
+        When the component is mounted, we need to check if there is a new chat to start
+        """
+        await self.load_chat(self.chat_data)
+
+        # TODO - The code below shouldn't be required.
+        #  Seems like a Textual bug.
+        self.set_timer(
+            0.05,
+            callback=lambda: self.chat_container.scroll_end(animate=False, force=True),
+        )
+
+    @property
+    def chat_container(self) -> VerticalScroll:
+        return self.query_one("#chat-container", VerticalScroll)
 
     @property
     def is_empty(self) -> bool:
         """True if the conversation is empty, False otherwise."""
         return len(self.chat_data.messages) == 1  # Contains system message at first.
 
     def scroll_to_latest_message(self):
-        if self.chat_container is not None:
-            self.chat_container.refresh()
-            self.chat_container.scroll_end(animate=False)
+        container = self.chat_container
+        container.refresh()
+        container.scroll_end(animate=False, force=True)
+
+    def key_d(self):
+        print(self.chat_container.scroll_y)
+        print(self.chat_container.max_scroll_y)
 
     async def new_user_message(self, content: str) -> None:
         log.debug(f"User message submitted in chat {self.chat_data.id!r}: {content!r}")
-        user_message = HumanMessage(
-            content=content,
-            additional_kwargs={
-                "timestamp": time.time(),
-                "status": None,
-                "end_turn": None,
-                "weight": None,
-                "metadata": None,
-                "recipient": None,
-            },
-        )
-        # If the thread was empty, and now it's not, remove the ConversationOptions.
-        is_first_message = self.is_empty
-        if is_first_message:
-            log.debug(
-                f"First user message received in "
-                f"conversation with model {self.chat_data.model_name!r}"
-            )
-            assert self.chat_options is not None
-            self.chat_options.display = False
-
-            # At this point, we should create the conversation in the database.
-            # Note that we don't need to add the message here, since `create_chat`
-            # already adds any of the messages already present in the chat.
-            self.chat_data.id = str(ChatsManager.create_chat(chat_data=self.chat_data))
-
-            # Add the first message to the thread AFTER creating the chat, since
-            # we don't want ChatsManager.create_chat to persist the message for us.
-            # The message will be persisted by us below, outwith this if block.
-
-        self.chat_data.messages.append(user_message)
-        if is_first_message:
-            self.post_message(
-                Chat.FirstMessageSent(
-                    chat_data=self.chat_data,
-                )
-            )
-
-        ChatsManager.add_message_to_chat(
-            chat_id=str(self.chat_data.id), message=user_message
+        now_utc = datetime.datetime.now(datetime.UTC)
+        user_message: ChatCompletionUserMessageParam = {
+            "content": content,
+            "role": "user",
+        }
+        user_chat_message = ChatMessage(
+            user_message, now_utc, self.chat_data.model_name
+        )
+        self.chat_data.messages.append(user_chat_message)
+        await ChatsManager.add_message_to_chat(
+            chat_id=self.chat_data.id, message=user_chat_message
         )
 
-        assert self.chat_data.id is not None
         self.post_message(
             Chat.UserMessageSubmitted(
-                chat_id=str(self.chat_data.id), message=user_message
+                chat_id=self.chat_data.id, message=user_chat_message
             )
         )
-
-        assert self.chat_data.model_name is not None
-        user_message_chatbox = Chatbox(user_message, self.chat_data.model_name)
+        user_message_chatbox = Chatbox(user_chat_message, self.chat_data.model_name)
 
         assert (
             self.chat_container is not None
         ), "Textual has mounted container at this point in the lifecycle."
 
         await self.chat_container.mount(user_message_chatbox)
         self.scroll_to_latest_message()
-        self.post_message(self.AgentResponseStarted())
         self.stream_agent_response()
 
-    async def clear_thread(self) -> None:
-        """Remove the internal thread representing the chat, and update the DOM."""
-
-        # We have to maintain the system message.
-        self.chat_data.messages = self.chat_data.messages[:1]
-
-        assert self.chat_container is not None
-
-        # Clear the part of the DOM containing the chat messages.
-        # Important that we make a copy before removing inside the loop!
-        children = list(self.chat_container.children)
-        for child in children:
-            await child.remove()
-
-    @work(exclusive=True)
+    @work
     async def stream_agent_response(self) -> None:
-        self.scroll_to_latest_message()
         log.debug(
             f"Creating streaming response with model {self.chat_data.model_name!r}"
         )
-        selected_model: GPTModel = MODEL_MAPPING[self.chat_data.model_name]
-        llm: BaseChatModel = selected_model.model
-        trimmed_messages = self.trim_messages(
-            model=llm,
-            messages=self.chat_data.messages,
-            max_tokens=selected_model.token_limit,
-            preserve_system_message=True,
-        )
-        streaming_response = llm.astream(input=trimmed_messages)
-        # TODO - ensure any metadata available in streaming response is passed through
-        message = AIMessage(
-            content="",
-            additional_kwargs={
-                "timestamp": time.time(),
-                "status": None,
-                "end_turn": None,
-                "weight": None,
-                "metadata": None,
-                "recipient": None,
-            },
+        model: EliaChatModel = get_model_by_name(
+            self.chat_data.model_name, self.elia.launch_config
         )
+
+        from litellm import ModelResponse, acompletion
+        from litellm.utils import trim_messages
+
+        raw_messages = [message.message for message in self.chat_data.messages]
+        messages: list[ChatCompletionUserMessageParam] = trim_messages(
+            raw_messages, model.name
+        )  # type: ignore
+        response = await acompletion(
+            messages=messages,
+            stream=True,
+            model=model.name,
+            temperature=model.temperature,
+            max_retries=model.max_retries,
+        )
+        ai_message: ChatCompletionAssistantMessageParam = {
+            "content": "",
+            "role": "assistant",
+        }
+        now = datetime.datetime.now(datetime.UTC)
+        message = ChatMessage(message=ai_message, model=model.name, timestamp=now)
+
         assert self.chat_data.model_name is not None
         response_chatbox = Chatbox(
             message=message,
             model_name=self.chat_data.model_name,
+            classes="response-in-progress",
         )
         assert (
             self.chat_container is not None
         ), "Textual has mounted container at this point in the lifecycle."
-        await self.chat_container.mount(response_chatbox)
-        async for token in streaming_response:
-            if isinstance(token, BaseMessageChunk):
-                token_str = token.content
-            else:
-                token_str = str(token)
-            response_chatbox.append_chunk(token_str)
-            scroll_y = self.chat_container.scroll_y
-            max_scroll_y = self.chat_container.max_scroll_y
-            if scroll_y in range(max_scroll_y - 3, max_scroll_y + 1):
-                self.chat_container.scroll_end(animate=False)
-        self.post_message(
-            self.AgentResponseComplete(
-                chat_id=self.chat_data.id,
-                message=response_chatbox.message,
+
+        try:
+            chunk_count = 0
+            async for chunk in response:
+                chunk = cast(ModelResponse, chunk)
+                response_chatbox.border_title = "Agent is responding..."
+
+                if chunk_count == 0:
+                    self.post_message(self.AgentResponseStarted())
+                    await self.chat_container.mount(response_chatbox)
+
+                chunk_content = chunk.choices[0].delta.content
+                if isinstance(chunk_content, str):
+                    response_chatbox.append_chunk(chunk_content)
+                else:
+                    break
+
+                scroll_y = self.chat_container.scroll_y
+                max_scroll_y = self.chat_container.max_scroll_y
+                if scroll_y in range(max_scroll_y - 3, max_scroll_y + 1):
+                    self.chat_container.scroll_end(animate=False)
+
+                chunk_count += 1
+        except Exception:
+            self.notify(
+                "There was a problem using this model. "
+                "Please check your configuration file.",
+                title="Error",
+                severity="error",
+                timeout=15,
+            )
+        else:
+            self.post_message(
+                self.AgentResponseComplete(
+                    chat_id=self.chat_data.id,
+                    message=response_chatbox.message,
+                    chatbox=response_chatbox,
+                )
             )
-        )
 
     @on(AgentResponseComplete)
     def agent_finished_responding(self, event: AgentResponseComplete) -> None:
         # Ensure the thread is updated with the message from the agent
         self.chat_data.messages.append(event.message)
+        event.chatbox.border_title = "Agent"
+        event.chatbox.remove_class("response-in-progress")
 
-    @on(Input.Submitted, "#chat-input")
-    async def user_chat_message_submitted(self, event: Input.Submitted) -> None:
+    @on(PromptInput.PromptSubmitted)
+    async def user_chat_message_submitted(
+        self, event: PromptInput.PromptSubmitted
+    ) -> None:
         if self.allow_input_submit is True:
-            user_message = event.value
-            event.input.value = ""
+            user_message = event.text
             await self.new_user_message(user_message)
+            event.prompt_input.clear()
 
-    async def load_chat(self, chat: ChatData) -> None:
-        assert self.chat_options is not None
-        assert self.chat_container is not None
-
-        # If the options display is visible, get rid of it.
-        self.chat_options.display = False
+    @on(PromptInput.CursorEscapingTop)
+    async def on_cursor_up_from_prompt(self) -> None:
+        self.focus_latest_message()
+
+    def get_latest_chatbox(self) -> Chatbox:
+        return self.query(Chatbox).last()
+
+    def focus_latest_message(self) -> None:
+        try:
+            self.get_latest_chatbox().focus()
+        except NoMatches:
+            pass
+
+    def action_focus_latest_message(self) -> None:
+        self.focus_latest_message()
+
+    def action_focus_first_message(self) -> None:
+        try:
+            self.query(Chatbox).first().focus()
+        except NoMatches:
+            pass
+
+    def action_scroll_container_up(self) -> None:
+        if self.chat_container:
+            self.chat_container.scroll_up()
+
+    def action_scroll_container_down(self) -> None:
+        if self.chat_container:
+            self.chat_container.scroll_down()
 
-        # Update the chat data
-        await self.clear_thread()
-        self.chat_data = chat
+    async def action_details(self) -> None:
+        await self.app.push_screen(ChatDetails(self.chat_data))
 
-        assert self.chat_data.model_name is not None
+    async def load_chat(self, chat_data: ChatData) -> None:
+        assert self.chat_container is not None
         chatboxes = [
             Chatbox(chat_message, self.chat_data.model_name)
-            for chat_message in chat.non_system_messages
+            for chat_message in self.chat_data.non_system_messages
         ]
         await self.chat_container.mount_all(chatboxes)
-        self.chat_container.scroll_end(animate=False)
-
+        self.chat_container.scroll_end(animate=False, force=True)
         chat_header = self.query_one(ChatHeader)
-        chat_header.title = chat.short_preview or "Untitled Chat"
-        chat_header.model_name = chat.model_name or "unknown model"
-        self.post_message(Chat.SavedChatLoaded(chat))  # TODO - required?
-
-    async def prepare_for_new_chat(self) -> None:
-        await self.clear_thread()
-
-        # Show the options to let the user configure the new chat.
-        assert self.chat_options is not None
-
-        chat_header = self.query_one(ChatHeader)
-        self.chat_data.id = None
-        chat_header.title = "Untitled Chat"
-        chat_header.model_name = self.chat_data.model_name or "unknown model"
-        self.chat_options.display = True
-
-        log.debug(f"Prepared for new chat. Chat data = {self.chat_data}")
-
-    def compose(self) -> ComposeResult:
-        yield ChatHeader()
-        with Vertical(id="chat-input-container"):
-            yield Input(placeholder="[I] Enter your message here...", id="chat-input")
-            yield AgentIsTyping()
-
-        with VerticalScroll() as vertical_scroll:
-            self.chat_container = vertical_scroll
-            vertical_scroll.can_focus = False
-
-        self.chat_options = ChatOptions()
-        yield self.chat_options
-
-        # TODO - check if conversation is pre-existing.
-        #  If it already exists, load it here.
-        #  If it's a new empty conversation, show the
-        #  options for a new conversation.
-
-    async def on_mount(self, _: events.Mount) -> None:
-        """
-        When the component is mounted, we need to check if there is a new chat to start
-        """
-        app_context: EliaContext = self.app.elia_context  # type: ignore[attr-defined]
-        gpt_model = app_context.gpt_model
-        self.chat_data.model_name = gpt_model.name
-        chat_input = self.query_one("#chat-input")
-        if app_context.chat_message is not None:
-            await self.prepare_for_new_chat()
-            await self.new_user_message(app_context.chat_message)
-            chat_input.focus()
-
-    @classmethod
-    def get_message_length(
-        cls,
-        messages: list[BaseMessage],
-        model: BaseChatModel | LLM,
-    ) -> tuple[list[tuple[BaseMessage, int]], int]:
-        """
-        Get the length of messages
-        """
-        if len(messages) == 0:
-            raise ValueError("No messages provided")
-        total_length = 0
-        message_lengths: list[tuple[BaseMessage, int]] = []
-        for message in messages:
-            message_length = model.get_num_tokens_from_messages(messages=[message])
-            message_lengths.append((message, message_length))
-            total_length += message_length
-        return message_lengths, total_length
-
-    @classmethod
-    def trim_messages(
-        cls,
-        model: BaseChatModel | LLM,
-        messages: list[BaseMessage],
-        max_tokens: int,
-        preserve_system_message: bool = True,
-    ) -> list[BaseMessage]:
-        """
-        Trim messages to fit within max_tokens
-
-        This method pre-calculates the length of each message, then iterates
-        through the messages in reverse order, adding them to a list until
-        the total number of tokens exceeds max_tokens. Optionally, the system
-        message can be preserved at the beginning of the chat.
-
-        Parameters
-        ----------
-        model: BaseChatModel | LLM
-            Language model
-        messages: list[BaseMessage]
-            Messages
-        max_tokens: int
-            Maximum number of tokens
-        preserve_system_message: bool
-            Whether to preserve the system message at the beginning of the chat
-
-        Returns
-        -------
-        list[BaseMessage]
-            Trimmed messages
-        """
-        message_lengths, total_length = cls.get_message_length(
-            messages=messages, model=model
+        chat_header.update_header(
+            chat=chat_data,
+            model=get_model_by_name(chat_data.model_name, self.elia.launch_config),
         )
-        if total_length <= max_tokens:
-            return messages
-        total_tokens = 0
-        trimmed_messages: list[BaseMessage] = []
-        preserved_messages: list[BaseMessage] = []
-        if preserve_system_message is True and isinstance(messages[0], SystemMessage):
-            system_message_tokens = model.get_num_tokens_from_messages(
-                messages=[messages[0]]
-            )
-            if system_message_tokens > max_tokens:
-                raise ValueError(
-                    f"System message is too long ({system_message_tokens} tokens)"
-                )
-            total_tokens += system_message_tokens
-            preserved_messages.append(messages[0])
-            message_lengths = message_lengths[1:]
-        for message, length in reversed(message_lengths):
-            total_tokens += length
-            if total_tokens > max_tokens:
-                break
-            else:
-                trimmed_messages.append(message)
-        if len(trimmed_messages) == 0:
-            msg = (
-                f"Unable to trim ({len(messages)}) messages to fit "
-                f"within max_tokens ({max_tokens})"
-            )
-            raise ValueError(msg)
-        return preserved_messages + list(reversed(trimmed_messages))
+
+        # If the last message didn't receive a response, try again.
+        messages = chat_data.messages
+        if messages and messages[-1].message["role"] == "user":
+            self.stream_agent_response()
+
+    def action_close(self) -> None:
+        self.app.clear_notifications()
+        self.app.pop_screen()
```

### Comparing `elia_chat-0.4.1/elia_chat/widgets/chat_list.py` & `elia_chat-1.0.0b1/elia_chat/widgets/chat_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,126 @@
 from __future__ import annotations
 
 import datetime
 from dataclasses import dataclass
 
 import humanize
 from rich.console import RenderResult, Console, ConsoleOptions
+from rich.markup import escape
 from rich.padding import Padding
 from rich.text import Text
-from textual import log, on
-from textual.app import ComposeResult
-from textual.containers import Horizontal, Vertical
+from textual import events, log, on
+from textual.binding import Binding
 from textual.message import Message
-from textual.reactive import reactive
-from textual.widget import Widget
-from textual.widgets import Button, OptionList, Static
+from textual.widgets import OptionList
 from textual.widgets.option_list import Option
 
 from elia_chat.chats_manager import ChatsManager
-from elia_chat.models import ChatData
+from elia_chat.config import LaunchConfig
+from elia_chat.models import ChatData, get_model_by_name
 
 
 @dataclass
 class ChatListItemRenderable:
     chat: ChatData
-    is_open: bool = False
+    config: LaunchConfig
 
     def __rich_console__(
         self, console: Console, options: ConsoleOptions
     ) -> RenderResult:
-        utc_dt = datetime.datetime.utcnow()
-        local_dt = utc_dt.astimezone()
-        delta = local_dt - self.chat.create_time
-        subtitle = humanize.naturaltime(delta)
+        now = datetime.datetime.now(datetime.UTC)
+        delta = now - self.chat.update_time
+        time_ago = humanize.naturaltime(delta)
+        time_ago_text = Text(time_ago, style="dim i")
+        model = get_model_by_name(self.chat.model_name, self.config)
+        subtitle = f"[dim]{escape(model.display_name or model.name)}"
+        if model.provider:
+            subtitle += f" [i]by[/] {escape(model.provider)}"
+        model_text = Text.from_markup(subtitle)
+        title = self.chat.title or self.chat.short_preview.replace("\n", " ")
         yield Padding(
-            Text.assemble(
-                (self.chat.short_preview, "" if not self.is_open else "b"),
-                "\n",
-                (subtitle, "dim"),
-            ),
-            pad=(0, 1),
-            style="reverse" if self.is_open else "",
+            Text.assemble(title, "\n", model_text, "\n", time_ago_text),
+            pad=(0, 0, 0, 1),
         )
 
 
 class ChatListItem(Option):
-    def __init__(self, chat: ChatData, is_open: bool = False) -> None:
+    def __init__(self, chat: ChatData, config: LaunchConfig) -> None:
         """
         Args:
             chat: The chat associated with this option.
-            is_open: True if this is the chat that's currently open.
         """
-        super().__init__(ChatListItemRenderable(chat, is_open=is_open))
+        super().__init__(ChatListItemRenderable(chat, config))
         self.chat = chat
-        self.is_open = is_open
+        self.config = config
 
 
-class ChatList(Widget):
-    COMPONENT_CLASSES = {"app-title", "app-subtitle"}
-
-    current_chat_id: reactive[str | None] = reactive(None)
+class ChatList(OptionList):
+    BINDINGS = [
+        Binding("j,down", "cursor_down", "Down", show=False),
+        Binding("k,up", "cursor_up", "Up", show=False),
+        Binding("G,end", "last", "Last", show=False),
+        Binding("l,enter", "select", "Select", show=False),
+        Binding("g,home", "first", "First", show=False),
+        Binding("pagedown", "page_down", "Page Down", show=False),
+        Binding("pageup", "page_up", "Page Up", show=False),
+    ]
 
     @dataclass
     class ChatOpened(Message):
         chat: ChatData
 
-    def compose(self) -> ComposeResult:
-        with Vertical(id="cl-header-container"):
-            yield Static(Text("elia", style=self.get_component_rich_style("app-title")))
-            yield Static(
-                Text(
-                    "ChatGPT in the terminal",
-                    style=self.get_component_rich_style("app-subtitle"),
-                )
-            )
-
-        self.options = self.load_chat_list_items()
-        option_list = OptionList(
-            *self.options,
-            id="cl-option-list",
-        )
-        yield option_list
-
-        with Horizontal(id="cl-button-container"):
-            yield Button("[Ctrl+N] New Chat", id="cl-new-chat-button")
+    async def on_mount(self) -> None:
+        await self.reload_and_refresh()
 
-    @on(OptionList.OptionSelected, "#cl-option-list")
-    def post_chat_opened(self, event: OptionList.OptionSelected) -> None:
+    @on(OptionList.OptionSelected)
+    async def post_chat_opened(self, event: OptionList.OptionSelected) -> None:
         assert isinstance(event.option, ChatListItem)
         chat = event.option.chat
-        self.current_chat_id = chat.id
-        self.reload_and_refresh()
+        await self.reload_and_refresh()
         self.post_message(ChatList.ChatOpened(chat=chat))
 
-    def on_focus(self) -> None:
-        log.debug("Sidebar focused")
-        self.query_one("#cl-option-list", OptionList).focus()
+    @on(OptionList.OptionHighlighted)
+    @on(events.Focus)
+    def show_border_subtitle(self) -> None:
+        if self.highlighted is not None:
+            self.border_subtitle = "[[white]Enter[/]] Open chat"
+        elif self.option_count > 0:
+            self.highlighted = 0
+
+    def on_blur(self) -> None:
+        self.border_subtitle = None
 
-    def reload_and_refresh(self, new_highlighted: int = -1) -> None:
+    async def reload_and_refresh(self, new_highlighted: int = -1) -> None:
         """Reload the chats and refresh the widget. Can be used to
         update the ordering/previews/titles etc contained in the list.
 
         Args:
             new_highlighted: The index to highlight after refresh.
         """
-        self.options = self.load_chat_list_items()
-        option_list = self.query_one(OptionList)
-        old_highlighted = option_list.highlighted
-        option_list.clear_options()
-        option_list.add_options(self.options)
+        self.options = await self.load_chat_list_items()
+        old_highlighted = self.highlighted
+        self.clear_options()
+        self.add_options(self.options)
+        self.border_title = f"History ({len(self.options)})"
         if new_highlighted > -1:
-            option_list.highlighted = new_highlighted
+            self.highlighted = new_highlighted
         else:
-            option_list.highlighted = old_highlighted
+            self.highlighted = old_highlighted
 
-    def load_chat_list_items(self) -> list[ChatListItem]:
-        chats = self.load_chats()
-        return [
-            ChatListItem(chat, is_open=self.current_chat_id == chat.id)
-            for chat in chats
-        ]
+    async def load_chat_list_items(self) -> list[ChatListItem]:
+        chats = await self.load_chats()
+        return [ChatListItem(chat, self.app.launch_config) for chat in chats]
 
-    def load_chats(self) -> list[ChatData]:
-        all_chats = ChatsManager.all_chats()
+    async def load_chats(self) -> list[ChatData]:
+        all_chats = await ChatsManager.all_chats()
         return all_chats
 
     def create_chat(self, chat_data: ChatData) -> None:
-        new_chat_list_item = ChatListItem(chat_data, is_open=True)
+        new_chat_list_item = ChatListItem(chat_data, self.app.launch_config)
         log.debug(f"Creating new chat {new_chat_list_item!r}")
 
         option_list = self.query_one(OptionList)
         self.options = [
             new_chat_list_item,
             *self.options,
         ]
```

### Comparing `elia_chat-0.4.1/elia_chat/widgets/token_analysis.py` & `elia_chat-1.0.0b1/elia_chat/widgets/token_analysis.py`

 * *Files identical despite different names*

