# Comparing `tmp/sql_lsp-0.0.2.tar.gz` & `tmp/sql_lsp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_lsp-0.0.2.tar", max compression
+gzip compressed data, was "sql_lsp-0.0.3.tar", max compression
```

## Comparing `sql_lsp-0.0.2.tar` & `sql_lsp-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       64 2023-11-20 02:38:40.112725 sql_lsp-0.0.2/README.md
--rw-r--r--   0        0        0      574 2023-11-20 04:02:57.714695 sql_lsp-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-22 21:58:30.202861 sql_lsp-0.0.2/sql_lsp/__init__.py
--rw-r--r--   0        0        0       71 2023-11-06 03:36:46.600727 sql_lsp-0.0.2/sql_lsp/__main__.py
--rw-r--r--   0        0        0     5741 2023-11-20 00:32:32.195043 sql_lsp-0.0.2/sql_lsp/completion.py
--rw-r--r--   0        0        0      321 2023-11-17 01:18:14.054285 sql_lsp-0.0.2/sql_lsp/config.py
--rw-r--r--   0        0        0     2232 2023-11-20 00:23:48.356269 sql_lsp-0.0.2/sql_lsp/database.py
--rw-r--r--   0        0        0     6128 2023-11-20 03:59:12.580905 sql_lsp-0.0.2/sql_lsp/mysql_connector.py
--rw-r--r--   0        0        0     9355 2023-11-20 04:03:06.441380 sql_lsp-0.0.2/sql_lsp/server.py
--rw-r--r--   0        0        0     3639 2023-11-08 03:28:29.230889 sql_lsp-0.0.2/sql_lsp/utils.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 sql_lsp-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       64 2024-05-05 03:55:22.442530 sql_lsp-0.0.3/README.md
+-rw-r--r--   0        0        0      539 2024-05-06 01:58:20.524220 sql_lsp-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 03:55:22.443530 sql_lsp-0.0.3/sql_lsp/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-05 03:55:22.443530 sql_lsp-0.0.3/sql_lsp/__main__.py
+-rw-r--r--   0        0        0     6169 2024-05-05 03:55:22.443530 sql_lsp-0.0.3/sql_lsp/completion.py
+-rw-r--r--   0        0        0      321 2024-05-05 03:55:22.443530 sql_lsp-0.0.3/sql_lsp/config.py
+-rw-r--r--   0        0        0     2369 2024-05-05 03:55:22.443530 sql_lsp-0.0.3/sql_lsp/database.py
+-rw-r--r--   0        0        0     7885 2024-05-05 22:35:06.934031 sql_lsp-0.0.3/sql_lsp/mysql_connector.py
+-rw-r--r--   0        0        0     9783 2024-05-06 01:58:41.463246 sql_lsp-0.0.3/sql_lsp/server.py
+-rw-r--r--   0        0        0     3966 2024-05-05 03:55:22.443530 sql_lsp-0.0.3/sql_lsp/utils.py
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 sql_lsp-0.0.3/PKG-INFO
```

### Comparing `sql_lsp-0.0.2/pyproject.toml` & `sql_lsp-0.0.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
 [tool.poetry.scripts]
 sql-ls = "sql_lsp.__main__:main"
 
 [tool.poetry]
 name = "sql-lsp"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Chahak Mehta <chahakmehta013@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.12"
 pygls = "^1.1.1"
-mysql-connector-python = "^8.2.0"
+mysql-connector = "^8.2.0"
 sqlfluff = "^2.3.5"
 tabulate = "^0.9.0"
 
 
 [tool.poetry.group.dev.dependencies]
-python-lsp-server = {extras = ["all"], version = "^1.8.2"}
 isort = "^5.12.0"
 black = "^23.10.1"
-ruff-lsp = "^0.0.42"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.basedpyright]
+reportUnusedCallResult = false
```

### Comparing `sql_lsp-0.0.2/sql_lsp/completion.py` & `sql_lsp-0.0.3/sql_lsp/completion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import re
 from bisect import bisect_left
 from operator import attrgetter
-from typing import List, Optional
 
 from lsprotocol.types import CompletionItem, CompletionItemKind, Position
 from pygls.workspace import TextDocument
 from sqlfluff.core import FluffConfig, Lexer, Parser
 from sqlfluff.core.parser.segments.base import BaseSegment
 from sqlfluff.dialects.dialect_ansi import TableReferenceSegment
 from sqlfluff.dialects.dialect_mysql import ColumnReferenceSegment
@@ -15,120 +14,133 @@
 from .database import DBConnection
 from .utils import get_json_segment
 
 logger = logging.getLogger(__file__)
 
 
 def get_segment_at_point(
-    segments: List[BaseSegment], pos: Position
-) -> Optional[BaseSegment]:
+    segments: list[BaseSegment], pos: Position
+) -> tuple[BaseSegment | None, int]:
     # Get first segment in given line
     line_start_idx = bisect_left(
         segments, pos.line + 1, key=attrgetter("pos_marker.line_no")
     )
     if not segments:
         return None, 0
     for i in range(line_start_idx, len(segments)):
         if segments[i].pos_marker.line_no != pos.line + 1:
             break
     line_end_idx = i
-    # line_end_idx = i - 1 if i != len(segments) else len(segments)
 
     line_segments = segments[line_start_idx:line_end_idx]
-    # logger.debug(f"Looking at pos: {pos}")
-    # logger.debug(
-    #     f"Total segments: {len(segments)}, Line start: {line_start_idx}, line end: {line_end_idx}"
-    # )
-    # logger.debug(f"segments: {segments}")
-    # logger.debug(f"line_segments: {line_segments}")
     segment_idx = (
         bisect_left(
             line_segments,
             pos.character + 1,
             key=attrgetter("pos_marker.line_pos"),
         )
         - 1
         if len(line_segments) != 1
         else 0
     )
-    # logger.debug(
-    #     f"segment pos: {[(x.raw, attrgetter('pos_marker.line_pos')(x)) for x in line_segments]}"
-    # )
-    # logger.debug(f"segment_idx: {segment_idx}")
-    return line_segments[segment_idx], segment_idx
+    return line_segments[segment_idx], line_start_idx + segment_idx
 
 
 def get_last_word(document: TextDocument, pos: Position):
     line = document.lines[pos.line][: pos.character]
     last_word_regex = re.compile(r"[\w`]+$", re.IGNORECASE)
-    word_matches = last_word_regex.findall(line)
+    word_matches: list[str] = last_word_regex.findall(line)
     last_word = "*"
     if len(word_matches) != 0:
         last_word = word_matches[-1]
 
     return last_word
 
 
-def _get_alias_table_name(alias: str, parsed_query: BaseSegment) -> Optional[str]:
-    from_elements = get_json_segment(parsed_query, "from_expression_elements")
+def _get_alias_table_name(alias: str, parsed_query: BaseSegment) -> str | None:
+    from_elements = list(
+        get_json_segment(
+            parsed_query.as_record(show_raw=True), "from_expression_element"
+        )
+    )
     for element in from_elements:
-        if element.get("alias_expression", {}).get("naked_identifier", "") == alias:
-            return get_json_segment(
-                element.get("table_expression", {}), "naked_identifier"
+        guessed_alias: str = element.get("alias_expression", {}).get(
+            "naked_identifier", ""
+        )
+        logger.debug(
+            f"guessed_alias: {guessed_alias}, alias: {alias}, {guessed_alias == alias}"
+        )
+        if guessed_alias == alias:
+            return list(
+                get_json_segment(
+                    element.get("table_expression", {}), "naked_identifier"
+                )
             )[-1]
     return None
 
 
 def get_completion_candidates(
     document: TextDocument, pos: Position, dbconn: DBConnection
-):
+) -> list[CompletionItem]:
     keywords = dbconn.connector.help_cache
     last_word = get_last_word(document, pos)
+    logger.debug(f"last_word: {last_word}")
     match_regex = re.compile(last_word, re.IGNORECASE)
-    candidates = []
+    candidates: list[CompletionItem] = []
 
     text = document.source
     lexer = Lexer(config=fluff_config)
     parser = Parser(config=fluff_config)
     parsed_query = parser.parse(lexer.lex(text)[0])
     segments = parsed_query.get_raw_segments()
     current_segment, segment_id = get_segment_at_point(segments, pos)
     if not current_segment:
         return []
-    logger.info(f"Completing segment: {current_segment}")
-    logger.info(f"All segments: {segments}")
+    logger.info(f"Completing segment: {current_segment} at id: {segment_id}")
+    logger.info(f"Parent segment: {current_segment.get_parent()[0]}")
     match current_segment.get_parent()[0]:
         case ColumnReferenceSegment():
-            if segments[segment_id - 1].raw == ".":
+            logger.info("Matched column segment")
+            curr_seg = segments[segment_id].raw
+            prev_seg = segments[segment_id - 1].raw
+            if curr_seg == "." or prev_seg == ".":
                 alias = segments[segment_id - 2]
-                table_name = _get_alias_table_name(alias, parsed_query)
+                alias = (
+                    segments[segment_id - 1]
+                    if curr_seg == "."
+                    else segments[segment_id - 2]
+                )
+                table_name = _get_alias_table_name(alias.raw, parsed_query)
                 columns = dbconn.get_columns(table_name=table_name)
             else:
                 columns = dbconn.get_columns()
+                logger.info(f"Columns from db: {columns}")
             candidates.extend(
                 [
                     CompletionItem(
                         label=col.name,
                         kind=CompletionItemKind.Field,
-                        detail=col.table_name,
+                        detail=f"{col.table_name} (column)",
                         documentation=str(col),
                         sort_text="0",
                     )
                     for col in columns
                     if re.match(match_regex, col.name)
                 ]
             )
         case TableReferenceSegment():
+            logger.info("Matched table reference segment")
             tables = dbconn.get_tables()
+            logger.info(f"tables from db: {tables}")
             candidates.extend(
                 [
                     CompletionItem(
                         label=table.name,
                         kind=CompletionItemKind.Field,
-                        detail=table.type,
+                        detail="(table)",
                         documentation=table.description,
                         sort_text="1",
                     )
                     for table in tables
                     if re.match(match_regex, table.name)
                 ]
             )
```

### Comparing `sql_lsp-0.0.2/sql_lsp/database.py` & `sql_lsp-0.0.3/sql_lsp/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 import logging
-from typing import Dict, List, Optional, Tuple, ValuesView
+from collections.abc import ValuesView
 
-from .mysql_connector import ColumnInfo, MySQLConnector, TableInfo
+from .mysql_connector import (
+    ColumnInfo,
+    MySQLConnector,
+    TableInfo,
+    MysqlConnectionConfig,
+)
 
 logger = logging.getLogger(__file__)
 SUPPORTED_DBS = ["mysql", "mariadb"]
 
+ConnectionConfig = MysqlConnectionConfig
+
 
 class DBConnection:
-    def __init__(self, config: dict):
+    def __init__(self, config: ConnectionConfig):
         self._config = config
         match config["driver"]:
             case "mysql":
                 self.connector = MySQLConnector(config)
             case "mariadb":
                 self.connector = MySQLConnector(config)
             case _:
                 raise ValueError(
                     f"{config['driver']} is not supported yet."
-                    f" Supported databases - {SUPPORTED_DBS}"
+                    + f" Supported databases - {SUPPORTED_DBS}"
                 )
 
     def get_help(self, function: str) -> str | None:
         return self.connector.get_help(function)
 
-    def execute_query(self, query: str) -> Tuple[Optional[List[Dict]], Optional[str]]:
+    def execute_query(
+        self, query: str
+    ) -> tuple[list[dict[str, str]] | None, Exception | None]:
         """Execute the given query on the database.
 
         Parameters
         ----------
         query: String
             Query to execute.
 
         Returns
         -------
-        Tuple[Optional[List[Dict]], Optional[String]]
+        tuple[list[dict[str, str]] | None, Exception | None]
             A tuple of (results, error). The results are a list of dictionaries
             where the keys are the columns returned by the query.
         """
         logger.info(f"execute_query(query): {query}")
         return self.connector.execute_query(query)
 
     def get_tables(self) -> ValuesView[TableInfo]:
         """Fetch dictionary of table and their types."""
         return self.connector.get_tables()
 
-    def get_columns(self, table_name: str = None) -> ValuesView[ColumnInfo]:
+    def get_columns(self, table_name: str | None = "") -> ValuesView[ColumnInfo]:
         """Fetch list of columns.
 
         If table name is provided and valid, columns for only that table are
         returned else if it is invalid then an empty list is returned.
 
         If table name is not provided, then all columns in the database are
         returned.
@@ -61,8 +70,8 @@
 
         Returns
         -------
         ValuesView[ColumnInfo]
             A values view of ColumnInfo objects for each column present in the
         table/database.
         """
-        return self.connector.get_columns()
+        return self.connector.get_columns(table_name=table_name)
```

### Comparing `sql_lsp-0.0.2/sql_lsp/server.py` & `sql_lsp-0.0.3/sql_lsp/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import json
 import logging
-from pathlib import Path
-from typing import List, Optional
+import logging.config
+import os
 
 import sqlfluff
+
+from pathlib import Path
+from typing import override, TypedDict, ParamSpec
+
 from lsprotocol import validators
 from lsprotocol.types import (
     INITIALIZE,
     TEXT_DOCUMENT_CODE_ACTION,
     TEXT_DOCUMENT_COMPLETION,
     TEXT_DOCUMENT_DID_CHANGE,
     TEXT_DOCUMENT_DID_OPEN,
     TEXT_DOCUMENT_FORMATTING,
     TEXT_DOCUMENT_HOVER,
-    CodeAction,
     CodeActionParams,
     Command,
     CompletionList,
     CompletionParams,
     Diagnostic,
     DidChangeTextDocumentParams,
     DidOpenTextDocumentParams,
@@ -25,103 +28,119 @@
     Hover,
     HoverParams,
     InitializeParams,
     Position,
     Range,
     TextEdit,
 )
-from pygls import server
+from pygls.server import LanguageServer
 from pygls.protocol import LanguageServerProtocol, lsp_method
 from pygls.workspace import TextDocument
 
 from .completion import get_completion_candidates
 from .config import fluff_config
-from .database import DBConnection
+from .database import DBConnection, ConnectionConfig
 from .utils import current_word_range, get_text_in_range, tabulate_result
 
-logging.basicConfig(filename="sql-lsp-debug.log", filemode="w", level=logging.DEBUG)
+P = ParamSpec("P")
+
+sqlfluff_logger = logging.getLogger("sqlfluff")
+sqlfluff_logger.setLevel(logging.WARNING)
+sqlfluff_rules_logger = logging.getLogger("sqlfluff.rules.reflow")
+sqlfluff_rules_logger.setLevel(logging.WARNING)
+
+server_dir = Path(f"{os.getenv('HOME')}/.local/sql-lsp").absolute()
+if not server_dir.is_dir():
+    os.makedirs(server_dir, exist_ok=True)
+logging.basicConfig(
+    filename=server_dir.joinpath("sql-lsp-debug.log"),
+    filemode="w",
+    level=logging.DEBUG,
+    format="[%(levelname)s - %(asctime)s] %(module)s:%(funcName)s(%(lineno)d) %(message)s",
+)
 logger = logging.getLogger(__file__)
 
 
+ServerConnectionConfigs = TypedDict(
+    "ServerConnectionConfigs", {"connections": dict[str, ConnectionConfig]}
+)
+
+
 class SqlLanguageServerProtocol(LanguageServerProtocol):
+    available_connections: dict[str, ConnectionConfig] = {}
+    dbconn: DBConnection | None = None
+
     @lsp_method(INITIALIZE)
+    @override
     def lsp_initialize(self, params: InitializeParams):
-        self.server_config = json.load(
-            open(
+        try:
+            with open(
                 Path(params.root_uri.rsplit(":")[-1]).joinpath(".sql-ls/config.json"),
                 "r",
+            ) as config_file:
+                server_config: ServerConnectionConfigs = json.load(config_file)
+        except FileNotFoundError:
+            logger.error("Couldn't find .sql-ls/config.json, please create one.")
+            self.show_message("Couldn't find .sql-ls/config.json, please create one.")
+        except Exception as e:
+            raise e
+        else:
+            self.available_connections = server_config["connections"]
+            self.dbconn = DBConnection(
+                config=list(self.available_connections.values())[0]
             )
-        )
-        self.available_connections = self.server_config["connections"]
-        self.dbconn = DBConnection(config=self.available_connections[0])
         return super().lsp_initialize(params)
 
 
-class SqlLanguageServer(server.LanguageServer):
-    CMD_EXPLAIN_QUERY = "explainQuery"
-    CMD_EXECUTE_QUERY = "executeQuery"
-    CMD_SHOW_DATABASES = "showDatabases"
-    CMD_SHOW_CONNECTIONS = "showConnections"
-    CMD_SHOW_CONNECTION_ALIASES = "showConnectionAliases"
-    CMD_SWITCH_CONNECTIONS = "switchConnections"
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+sql_server = LanguageServer("sql-ls", "v0.0.3", protocol_cls=SqlLanguageServerProtocol)
 
 
-sql_server = SqlLanguageServer(
-    "sql-ls", "v0.0.2", protocol_cls=SqlLanguageServerProtocol
-)
-
-
-def _publish_diagnostics(ls: SqlLanguageServer, uri: str):
+def _publish_diagnostics(ls: LanguageServer, uri: str):
     """Publish diagnostics to LSP server."""
     document = ls.workspace.get_text_document(uri)
     lint_diagnostics = sqlfluff.lint(
         document.source, dialect="mysql", config=fluff_config
     )
-    # logger.debug("Linting diagnostics:")
-    # logger.debug(f"{lint_diagnostics}")
+    logger.debug("chahak: Linting diagnostics:")
+    logger.debug(f"{lint_diagnostics}")
     diagnostics: list[Diagnostic] = [
         Diagnostic(
             range=current_word_range(
                 document,
                 position=Position(line=x["line_no"] - 1, character=x["line_pos"] - 1),
             ),
             message=x["description"],
             code=x["code"],
-            # code_description=CodeDescription(
-            #     href=f"https://docs.sqlfluff.com/en/latest/rules.html#rule-{x['name']}"
-            # ),
         )
         for x in lint_diagnostics
     ]
     ls.publish_diagnostics(uri, diagnostics=diagnostics)
 
 
 @sql_server.feature(TEXT_DOCUMENT_COMPLETION)
-def completions(ls: SqlLanguageServer, params: CompletionParams):
+def completions(ls: LanguageServer, params: CompletionParams):
     items = []
     document = ls.workspace.get_document(params.text_document.uri)
     items = get_completion_candidates(document, params.position, ls.lsp.dbconn)
+    logger.info(f"Completion items: {items}")
     return CompletionList(is_incomplete=False, items=items)
 
 
 @sql_server.feature(TEXT_DOCUMENT_DID_OPEN)
-async def did_open(ls: SqlLanguageServer, params: DidOpenTextDocumentParams):
+async def did_open(ls: LanguageServer, params: DidOpenTextDocumentParams):
     _publish_diagnostics(ls, params.text_document.uri)
 
 
 @sql_server.feature(TEXT_DOCUMENT_DID_CHANGE)
-async def did_change(ls: SqlLanguageServer, params: DidChangeTextDocumentParams):
+async def did_change(ls: LanguageServer, params: DidChangeTextDocumentParams):
     _publish_diagnostics(ls, params.text_document.uri)
 
 
 @sql_server.feature(TEXT_DOCUMENT_FORMATTING)
-def format_document(ls: SqlLanguageServer, params: DocumentFormattingParams):
+def format_document(ls: LanguageServer, params: DocumentFormattingParams):
     uri = params.text_document.uri
     document = ls.workspace.get_text_document(uri)
     formatted_doc = sqlfluff.fix(
         document.source,
         config=fluff_config,
     )
     return [
@@ -132,144 +151,142 @@
             ),
             new_text=formatted_doc,
         )
     ]
 
 
 @sql_server.feature(TEXT_DOCUMENT_HOVER)
-async def hover(ls: SqlLanguageServer, params: HoverParams) -> Hover | None:
+async def hover(ls: LanguageServer, params: HoverParams) -> Hover | None:
     """LSP handler for textDocument/hover request."""
     document = ls.workspace.get_text_document(params.text_document.uri)
     word = document.word_at_position(params.position)
-    help_str = ls.lsp.dbconn.get_help(word)
+    help_str: str = ls.lsp.dbconn.get_help(word)
     return Hover(contents=help_str)
 
 
 @sql_server.feature(TEXT_DOCUMENT_CODE_ACTION)
-def code_action(
-    ls: SqlLanguageServer, params: CodeActionParams
-) -> Optional[List[CodeAction]]:
+def code_action(ls: LanguageServer, params: CodeActionParams) -> list[Command]:
     """Get code actions.
 
     Currently supports:
         1. Explain query
         2. Execute query
         2. Show Databases
         3. Show Connections
         4. Switch Connections
     """
     document = ls.workspace.get_text_document(params.text_document.uri)
-    commands: List[Command] = [
+    commands: list[Command] = [
         Command(
             title="Explain Query",
-            command=ls.CMD_EXPLAIN_QUERY,
+            command="explainQuery",
             arguments=[document, params],
         ),
         Command(
             title="Execute Query",
-            command=ls.CMD_EXECUTE_QUERY,
+            command="executeQuery",
             arguments=[document, params],
         ),
-        Command(title="Show Databases", command=ls.CMD_SHOW_DATABASES),
-        Command(title="Show Connections", command=ls.CMD_SHOW_CONNECTIONS),
+        Command(title="Show Databases", command="showDatabases"),
+        Command(title="Show Connections", command="showConnections"),
         Command(
             title="Switch Connections",
-            command=ls.CMD_SWITCH_CONNECTIONS,
+            command="switchConnections",
             arguments=[params],
         ),
     ]
-    logging.info(f"Trying to send: {commands}")
-    # commands = []
+    logger.info(f"Trying to send: {commands}")
     return commands
 
 
 # NOTE: While the type for `args` is a tuple of `TextDocument` and
 # `CodeActionParams`, the actual parameters that get passed into the
 # function by pygls is actually a dictionary version of the classes.
 # Hence, to access the values, we use dictionary keys instead of
 # class attributes.
-@sql_server.command(sql_server.CMD_EXECUTE_QUERY)
+@sql_server.command("executeQuery")
 def execute_query(
-    ls: SqlLanguageServer, *args: tuple[TextDocument, CodeActionParams]
+    ls: LanguageServer, *args: tuple[TextDocument, CodeActionParams]
 ) -> str:
     """Execute query."""
     if not ls.lsp.dbconn:
         raise KeyError(
-            "DB Connection not found on server. `SqlLanguageServer`"
-            " might not have been initialzied with `SqlLanguageServerProtocol`."
-            " Please check."
+            "DB Connection not found on server. `LanguageServer`"
+            + " might not have been initialzied with `LanguageServerProtocol`."
+            + " Please check."
         )
     logger.info(f"chahak: execute_query (args): {args}")
     document_args = args[0][0]
     document = ls.workspace.get_text_document(document_args["uri"])
     action_params = args[0][1]
     query = get_text_in_range(document, action_params["range"])
     logger.info(f"execute_query(query): {query}")
     rows, error = ls.lsp.dbconn.execute_query(query)
     if error is not None:
         return str(error)
     return tabulate_result(rows)
 
 
-@sql_server.command(sql_server.CMD_EXPLAIN_QUERY)
+@sql_server.command("explainQuery")
 def explain_query(
-    ls: SqlLanguageServer, *args: tuple[TextDocument, CodeActionParams]
+    ls: LanguageServer, *args: tuple[TextDocument, CodeActionParams]
 ) -> str:
     """Execute query."""
     if not ls.lsp.dbconn:
         raise KeyError(
-            "DB Connection not found on server. `SqlLanguageServer`"
-            " might not have been initialzied with `SqlLanguageServerProtocol`."
-            " Please check."
+            "DB Connection not found on server. `LanguageServer`"
+            + " might not have been initialzied with `LanguageServerProtocol`."
+            + " Please check."
         )
     logger.info(f"explain_query (args): {args}")
     document_args = args[0][0]
     document = ls.workspace.get_text_document(document_args["uri"])
     action_params = args[0][1]
     query = "explain " + get_text_in_range(document, action_params["range"])
     logger.info(f"execute_query(query): {query}")
     rows, error = ls.lsp.dbconn.execute_query(query)
     if error is not None:
         return str(error)
     return tabulate_result(rows)
 
 
-@sql_server.command(sql_server.CMD_SHOW_DATABASES)
-def show_databases(ls: SqlLanguageServer, *args) -> str:
+@sql_server.command("showDatabases")
+def show_databases(ls: LanguageServer) -> str:
     """Show Databases in the connection."""
     if not ls.lsp.dbconn:
         raise KeyError(
-            "DB Connection not found on server. `SqlLanguageServer`"
-            " might not have been initialzied with `SqlLanguageServerProtocol`."
-            " Please check."
+            "DB Connection not found on server. `LanguageServer`"
+            + " might not have been initialzied with `LanguageServerProtocol`."
+            + " Please check."
         )
     query = "show databases;"
     rows = ls.lsp.dbconn.execute_query(query)
     return tabulate_result(rows)
 
 
-@sql_server.command(sql_server.CMD_SHOW_CONNECTIONS)
-def show_connections(ls: SqlLanguageServer, *args) -> str:
-    """Show Databases in the connection."""
+@sql_server.command("showConnections")
+def show_connections(ls: LanguageServer) -> str:
+    """Show available connections."""
     return tabulate_result(
-        [{**conn, "password": "****"} for conn in ls.lsp.available_connections]
+        [
+            {"alias": alias, **conn, "password": "****"}
+            for alias, conn in ls.lsp.available_connections.items()
+        ]
     )
 
 
-@sql_server.command(sql_server.CMD_SHOW_CONNECTION_ALIASES)
-def show_connection_aliases(ls: SqlLanguageServer, *args) -> str:
+@sql_server.command("showConnectionAliases")
+def show_connection_aliases(ls: LanguageServer) -> str:
     """Show aliases for all the connections.
 
     Useful for providing a selection list to switch connections.
     """
-    return "\n".join([conn["alias"] for conn in ls.lsp.available_connections])
+    return "\n".join(list(ls.lsp.available_connections.keys()))
 
 
-@sql_server.command(sql_server.CMD_SWITCH_CONNECTIONS)
-def switch_connections(ls: SqlLanguageServer, *args: tuple[CodeActionParams]):
+@sql_server.command("switchConnections")
+def switch_connections(ls: LanguageServer, *args: tuple[CodeActionParams]):
     """Switch Databases in the connection."""
     selected_alias = args[0][0]
-    selected_config = [
-        con for con in ls.lsp.available_connections if con["alias"] == selected_alias
-    ][0]
+    selected_config = ls.lsp.available_connections[selected_alias]
     ls.lsp.dbconn = DBConnection(selected_config)
     ls.send_notification(f"Changed DB Connection to {selected_alias}")
```

### Comparing `sql_lsp-0.0.2/sql_lsp/utils.py` & `sql_lsp-0.0.3/sql_lsp/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import logging
-from typing import Any, Dict, Iterator, List, Optional, Union
+
+from collections.abc import Iterator
+from typing import Any, TypedDict
 
 from lsprotocol.types import Position, Range
 from pygls.workspace import TextDocument
+from sqlfluff.core.parser.segments.base import RecordSerialisedSegment
 from tabulate import tabulate
 
 logger = logging.getLogger(__file__)
 
 
-def current_word_range(document: TextDocument, position: Position) -> Optional[Range]:
+def current_word_range(document: TextDocument, position: Position) -> Range | None:
     """Get the range of the word under the cursor."""
     word = document.word_at_position(position)
     word_len = len(word)
     line: str = document.lines[position.line]
     start = 0
     for _ in range(1000):  # prevent infinite hanging in case we hit edge case
         begin = line.find(word, start)
@@ -24,69 +27,73 @@
                 start=Position(line=position.line, character=begin),
                 end=Position(line=position.line, character=end),
             )
         start = end
     return None
 
 
-def get_text_in_range(document: TextDocument, text_range: Union[Range, dict]) -> str:
+PositionAsDict = TypedDict("PositionAsDict", {"line": int, "character": int})
+RangeAsDict = TypedDict("RangeAsDict", {"start": PositionAsDict, "end": PositionAsDict})
+
+
+def get_text_in_range(document: TextDocument, text_range: Range | RangeAsDict) -> str:
     """Get document lines as string given a range."""
     doc_lines = document.lines
     if isinstance(text_range, Range):
         first_line_index, first_char_index = (
             text_range.start.line,
             text_range.start.character,
         )
         last_line_index, last_char_index = text_range.end.line, text_range.end.character
-    elif isinstance(text_range, dict):
+    elif isinstance(text_range, dict):  # type: ignore[reportUnnecessaryIsInstance]
         first_line_index, first_char_index = (
             text_range["start"]["line"],
             text_range["start"]["character"],
         )
         last_line_index, last_char_index = (
             text_range["end"]["line"],
             text_range["end"]["character"],
         )
     else:
         raise TypeError(
             f"`range` should either be a `Range` object or a dictionary."
-            f" found: {type(text_range)}"
+            + f" found: {type(text_range)}"
         )
 
     if first_line_index == last_line_index:
         if first_char_index == last_char_index:
             return "\n".join(doc_lines)
         return doc_lines[first_line_index][first_char_index:last_char_index]
 
     logger.debug("utils (doc_lines):")
     logger.debug(f"{doc_lines}")
-    lines = []
+    lines: list[str] = []
     for i in range(first_line_index - 1, last_line_index):
         logger.debug(f"Line: {i} of {len(doc_lines) - 1}")
         if i == first_line_index:
             lines.append(doc_lines[i][first_char_index:])
         elif i == last_line_index:
             lines.append(doc_lines[i][:last_char_index])
         elif i < len(doc_lines) - 1:
             lines.append(doc_lines[i])
     return "\n".join(lines)
 
 
-def tabulate_result(rows: List[dict]) -> str:
+def tabulate_result(rows: list[dict[str, str]]) -> str:
     """Tabulate the query results"""
     return tabulate(rows, headers="keys", showindex=True, tablefmt="psql")
 
 
 def get_json_segment(
-    parse_result: Dict[str, Any], segment_type: str
-) -> Iterator[Union[str, Dict[str, Any], List[Dict[str, Any]]]]:
+    parse_result: RecordSerialisedSegment, segment_type: str
+) -> Iterator[str | dict[str, Any] | list[dict[str, Any]]]:
     """Recursively search JSON parse result for specified segment type.
 
     Args:
-        parse_result (Dict[str, Any]): JSON parse result from `sqlfluff.fix`.
+        parse_result RecordSerialisedSegment: JSON parse result from `sqlfluff.fix`.
         segment_type (str): The segment type to search for.
 
     Yields:
         Iterator[Union[str, Dict[str, Any], List[Dict[str, Any]]]]:
         Retrieves children of specified segment type as either a string for a raw
         segment or as JSON or an array of JSON for non-raw segments.
     """
```

### Comparing `sql_lsp-0.0.2/PKG-INFO` & `sql_lsp-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: sql-lsp
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: Chahak Mehta
 Author-email: chahakmehta013@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: mysql-connector-python (>=8.2.0,<9.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: mysql-connector (>=8.2.0,<9.0.0)
 Requires-Dist: pygls (>=1.1.1,<2.0.0)
 Requires-Dist: sqlfluff (>=2.3.5,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # sql-lsp
```

