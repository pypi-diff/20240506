# Comparing `tmp/aioautomower-2024.4.4.tar.gz` & `tmp/aioautomower-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioautomower-2024.4.4.tar", max compression
+gzip compressed data, was "aioautomower-2024.5.0.tar", max compression
```

## Comparing `aioautomower-2024.4.4.tar` & `aioautomower-2024.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2001 2024-04-25 17:42:50.257138 aioautomower-2024.4.4/README.md
--rw-r--r--   0        0        0     8299 2024-04-25 17:43:09.336976 aioautomower-2024.4.4/pyproject.toml
--rw-r--r--   0        0        0      138 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/__init__.py
--rw-r--r--   0        0        0      108 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/_secrets.yaml
--rw-r--r--   0        0        0     7241 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/auth.py
--rw-r--r--   0        0        0     5812 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/const.py
--rw-r--r--   0        0        0     5087 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/example.py
--rw-r--r--   0        0        0      970 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/exceptions.py
--rw-r--r--   0        0        0    11236 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/model.py
--rw-r--r--   0        0        0        0 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/py.typed
--rw-r--r--   0        0        0    14281 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/session.py
--rw-r--r--   0        0        0     3659 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/utils.py
--rw-r--r--   0        0        0     2811 1970-01-01 00:00:00.000000 aioautomower-2024.4.4/PKG-INFO
+-rw-r--r--   0        0        0     2001 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/README.md
+-rw-r--r--   0        0        0     8389 2024-05-06 16:16:18.016122 aioautomower-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0      138 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/__init__.py
+-rw-r--r--   0        0        0      108 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/_secrets.yaml
+-rw-r--r--   0        0        0     7241 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/auth.py
+-rw-r--r--   0        0        0     5812 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/const.py
+-rw-r--r--   0        0        0     5123 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/example.py
+-rw-r--r--   0        0        0      970 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/exceptions.py
+-rw-r--r--   0        0        0    15474 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/model.py
+-rw-r--r--   0        0        0        0 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/py.typed
+-rw-r--r--   0        0        0    13861 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/session.py
+-rw-r--r--   0        0        0     3659 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/utils.py
+-rw-r--r--   0        0        0     2811 1970-01-01 00:00:00.000000 aioautomower-2024.5.0/PKG-INFO
```

### Comparing `aioautomower-2024.4.4/README.md` & `aioautomower-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.4/pyproject.toml` & `aioautomower-2024.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aioautomower"
 # The version is set by GH action on release
-version = "2024.4.4"
+version = "2024.5.0"
 description = "MPython module to talk to Husqvarna Automower."
 authors = ["Thomas55555"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "aioautomower", from = "src" },
 ]
@@ -25,24 +25,24 @@
 aiohttp = "^3.9.3"
 mashumaro = "^3.12"
 PyJWT = "^2.8.0"
 
 [tool.poetry.group.dev.dependencies]
 codespell = "2.2.6"
 covdefaults = "2.3.0"
-coverage = {version = "7.5.0", extras = ["toml"]}
-mypy = "1.9.0"
+coverage = {version = "7.5.1", extras = ["toml"]}
+mypy = "1.10.0"
 pre-commit = "3.7.0"
 pre-commit-hooks = "4.6.0"
 pylint = "3.1.0"
-pytest = "8.1.1"
+pytest = "8.2.0"
 pytest-asyncio = "0.23.6"
 pytest-cov = "5.0.0"
-ruff = "0.4.1"
-safety = "3.1.0"
+ruff = "0.4.3"
+safety = "3.2.0"
 yamllint = "1.35.1"
 syrupy = "4.6.1"
 aioresponses = "0.7.6"
 freezegun = "1.5.0"
 pyyaml = "6.0.1"
 types-pyyaml = "^6.0.12.20240311"
 
@@ -213,14 +213,20 @@
 ignore = ["R0902"]
 
 [tool.pylint.MASTER]
 ignore = [
   "tests",
 ]
 
+[tool.pylint."MESSAGES CONTROL"]
+disable = [
+    "too-many-instance-attributes",
+    ]
+
+
 [tool.mypy]
 # Specify the target platform details in config, so your developers are
 # free to run mypy on Windows, Linux, or macOS and get consistent
 # results.
 platform = "linux"
 python_version = "3.11"
```

### Comparing `aioautomower-2024.4.4/src/aioautomower/auth.py` & `aioautomower-2024.5.0/src/aioautomower/auth.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.4/src/aioautomower/const.py` & `aioautomower-2024.5.0/src/aioautomower/const.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.4/src/aioautomower/example.py` & `aioautomower-2024.5.0/src/aioautomower/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,24 +78,24 @@
     # Add a callback, can be done at any point in time and
     # multiple callbacks can be added.
     automower_api.register_data_callback(callback)
     automower_api.register_pong_callback(pong_callback)
     # pylint: disable=unused-variable
     for _mower_id in automower_api.data:
         await asyncio.sleep(5)
-        # await automower_api.park_until_next_schedule(_mower_id)
+        # await automower_api.commands.park_until_next_schedule(_mower_id)
         # Uncomment the line above to let all your mowers park until next schedule.
         await asyncio.sleep(5)
-        # await automower_api.park_until_further_notice(_mower_id)
+        # await automower_api.commands.park_until_further_notice(_mower_id)
         # Uncomment the line above to let all your mowers park until further notice.
         await asyncio.sleep(5)
-        # await automower_api.resume_schedule(_mower_id)
+        # await automower_api.commands.resume_schedule(_mower_id)
         # Uncomment the line above to let all your mowers resume their schedule.
         await asyncio.sleep(5)
-        # await automower_api.pause_mowing(_mower_id)
+        # await automower_api.commands.pause_mowing(_mower_id)
         # Uncomment the line above to let all your mowers pause.
     await asyncio.sleep(3000)
     # The close() will stop the websocket and the token refresh tasks
     await automower_api.close()
     api_task.cancel()
     ping_pong_task.cancel()
     await websession.close()
```

### Comparing `aioautomower-2024.4.4/src/aioautomower/exceptions.py` & `aioautomower-2024.5.0/src/aioautomower/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.4/src/aioautomower/model.py` & `aioautomower-2024.5.0/src/aioautomower/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,42 @@
 """Models for Husqvarna Automower data."""
 
-from dataclasses import dataclass, field
-from datetime import UTC, datetime
+import logging
+import operator
+from dataclasses import dataclass, field, fields
+from datetime import UTC, datetime, timedelta
 from enum import Enum, StrEnum
 from re import sub
 
 from mashumaro import DataClassDictMixin, field_options
 
 from .const import ERRORCODES
 
+logging.basicConfig(level=logging.DEBUG)
+
+WEEKDAYS = (
+    "monday",
+    "tuesday",
+    "wednesday",
+    "thursday",
+    "friday",
+    "saturday",
+    "sunday",
+)
+
+WEEKDAYS_TO_RFC5545 = {
+    "monday": "MO",
+    "tuesday": "TU",
+    "wednesday": "WE",
+    "thursday": "TH",
+    "friday": "FR",
+    "saturday": "SA",
+    "sunday": "SU",
+}
+
 
 def snake_case(string: str | None) -> str:
     """Convert an error text to snake case."""
     if string is None:
         raise TypeError
     return "_".join(
         sub(
@@ -40,15 +64,14 @@
     customer_id: str
 
 
 @dataclass
 class JWT(DataClassDictMixin):
     """The content of the JWT."""
 
-    # pylint: disable=too-many-instance-attributes
     jti: str
     iss: str
     roles: list[str]
     groups: list[str]
     scopes: list[str]
     scope: str
     client_id: str
@@ -128,15 +151,14 @@
     """Information about the calendar tasks.
 
     An Automower can have several tasks. If the mower supports
     work areas the property workAreaId is required to connect
     the task to an work area.
     """
 
-    # pylint: disable=too-many-instance-attributes
     start: int
     duration: int
     monday: bool
     tuesday: bool
     wednesday: bool
     thursday: bool
     friday: bool
@@ -144,18 +166,125 @@
     sunday: bool
     work_area_id: int | None = field(
         metadata=field_options(alias="workAreaId"), default=None
     )
 
 
 @dataclass
+class AutomowerCalendarEvent(DataClassDictMixin):
+    """Information about the calendar tasks.
+
+    An Automower can have several tasks. If the mower supports
+    work areas the property workAreaId is required to connect
+    the task to an work area.
+    """
+
+    start: datetime
+    end: datetime
+    rrule: str
+    uid: str
+    work_area_id: int | None
+
+
+def husqvarna_schedule_to_calendar(
+    task_list: list,
+) -> list[AutomowerCalendarEvent]:
+    """Convert the schedule to an sorted list of calendar events."""
+    eventlist = []
+    for task_dict in task_list:
+        calendar_dataclass = Calendar.from_dict(task_dict)
+        event = ConvertScheduleToCalendar(calendar_dataclass)
+        eventlist.append(event.make_event())
+    eventlist.sort(key=operator.attrgetter("start"))
+    return eventlist
+
+
+class ConvertScheduleToCalendar:
+    """Convert the Husqvarna task to an AutomowerCalendarEvent."""
+
+    def __init__(self, task: Calendar) -> None:
+        """Initialize the schedule to calendar converter."""
+        self.task = task
+        self.now = datetime.now().astimezone()
+        self.begin_of_current_day = self.now.replace(
+            hour=0, minute=0, second=0, microsecond=0
+        )
+        self.current_day = self.now.weekday()
+
+    def next_weekday_with_schedule(self) -> datetime:
+        """Find the next weekday with a schedule entry."""
+        for days in range(8):
+            time_to_check = self.now + timedelta(days=days)
+            time_to_check_begin_of_day = time_to_check.replace(
+                hour=0, minute=0, second=0, microsecond=0
+            )
+            day_to_check = time_to_check.weekday()
+            day_to_check_as_string = WEEKDAYS[day_to_check]
+            for task_field in fields(self.task):
+                field_name = task_field.name
+                field_value = getattr(self.task, field_name)
+                if field_value is True and field_name is day_to_check_as_string:
+                    end_task = (
+                        time_to_check_begin_of_day
+                        + timedelta(minutes=self.task.start)
+                        + timedelta(minutes=self.task.duration)
+                    )
+                    if self.begin_of_current_day == time_to_check_begin_of_day:
+                        if end_task < self.now:
+                            break
+                    return self.now + timedelta(days)
+        return self.now
+
+    def make_daylist(self) -> str:
+        """Generate a RFC5545 daylist from a task."""
+        day_list = ""
+        for task_field in fields(self.task):
+            field_name = task_field.name
+            field_value = getattr(self.task, field_name)
+            if field_value is True:
+                today_rfc = WEEKDAYS_TO_RFC5545[field_name]
+                if day_list == "":
+                    day_list = today_rfc
+                else:
+                    day_list += "," + str(today_rfc)
+        return day_list
+
+    def make_event(self) -> AutomowerCalendarEvent:
+        """Generate a AutomowerCalendarEvent from a task."""
+        daylist = self.make_daylist()
+        next_wd_with_schedule = self.next_weekday_with_schedule()
+        begin_of_day_with_schedule = next_wd_with_schedule.replace(
+            hour=0, minute=0, second=0, microsecond=0
+        ).astimezone()
+        return AutomowerCalendarEvent(
+            start=(
+                begin_of_day_with_schedule + timedelta(minutes=self.task.start)
+            ).astimezone(tz=UTC),
+            end=(
+                begin_of_day_with_schedule
+                + timedelta(minutes=self.task.start)
+                + timedelta(minutes=self.task.duration)
+            ).astimezone(tz=UTC),
+            rrule=f"FREQ=WEEKLY;BYDAY={daylist}",
+            uid=f"{self.task.start}_{self.task.duration}_{daylist}",
+            work_area_id=self.task.work_area_id,
+        )
+
+
+@dataclass
 class Tasks(DataClassDictMixin):
     """DataClass for Task values."""
 
     tasks: list[Calendar]
+    events: list[AutomowerCalendarEvent] = field(
+        metadata=field_options(
+            deserialize=husqvarna_schedule_to_calendar,
+            alias="tasks",
+        ),
+    )
 
 
 @dataclass
 class Override(DataClassDictMixin):
     """DataClass for Override values."""
 
     action: str
@@ -219,16 +348,14 @@
     longitude: float
 
 
 @dataclass
 class Statistics(DataClassDictMixin):
     """DataClass for Statistics values."""
 
-    # pylint: disable=too-many-instance-attributes
-
     cutting_blade_usage_time: int | None = field(
         metadata=field_options(alias="cuttingBladeUsageTime"), default=None
     )
     number_of_charging_cycles: int | None = field(
         metadata=field_options(alias="numberOfChargingCycles"), default=None
     )
     number_of_collisions: int | None = field(
@@ -311,15 +438,14 @@
     cutting_height: int
 
 
 @dataclass
 class MowerAttributes(DataClassDictMixin):
     """DataClass for MowerAttributes."""
 
-    # pylint: disable=too-many-instance-attributes
     system: System
     battery: Battery
     capabilities: Capabilities
     mower: Mower
     calendar: Tasks
     planner: Planner
     metadata: Metadata
```

### Comparing `aioautomower-2024.4.4/src/aioautomower/session.py` & `aioautomower-2024.5.0/src/aioautomower/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import contextlib
 import datetime
 import logging
 from dataclasses import dataclass
 from typing import Any, Literal, Mapping
 
-from aiohttp import WSMsgType
+from aiohttp import WSMessage, WSMsgType
 
 from .auth import AbstractAuth
 from .const import EVENT_TYPES, REST_POLL_CYCLE
 from .exceptions import NoDataAvailableException, TimeoutException
 from .model import HeadlightModes, MowerAttributes
 from .utils import mower_list_to_dictionary_dataclass
 
@@ -43,167 +43,26 @@
     work_area_calendar = "mowers/{mower_id}/workAreas/{work_area_id}/calendar"
     "Update the calendar for a work area on the mower."
 
     error_confirm = "mowers/{mower_id}/errors/confirm"
     "Confirm mower non-fatal error"
 
 
-class AutomowerSession:
-    """Automower API to communicate with an Automower.
-
-    The `AutomowerSession` is the primary API service for this library. It supports
-    operations like getting a status or sending commands.
-    """
-
-    # pylint: disable=too-many-instance-attributes
-    # pylint: disable=too-many-nested-blocks
-    # pylint: disable=too-many-public-methods
+class _MowerCommands:
+    """Sending commands."""
 
     def __init__(
         self,
         auth: AbstractAuth,
-        poll: bool = False,
-    ) -> None:
-        """Create a session.
+    ):
+        """Send all commands to the API.
 
         :param class auth: The AbstractAuth class from aioautomower.auth.
-        :param bool poll: Poll data with rest if True.
         """
-        self._data: Mapping[Any, Any] = {}
         self.auth = auth
-        self.pong_cbs: list = []
-        self.data_update_cbs: list = []
-        self.data: dict[str, MowerAttributes] = {}
-        self.last_ws_message: datetime.datetime
-        self.loop = asyncio.get_running_loop()
-        self.poll = poll
-        self.rest_task: asyncio.Task | None = None
-        self.token = None
-        self.token_task = None
-        self.token_update_cbs: list = []
-
-    def register_data_callback(self, callback) -> None:
-        """Register a data update callback."""
-        if callback not in self.data_update_cbs:
-            self.data_update_cbs.append(callback)
-
-    def _schedule_data_callback(self, cb) -> None:
-        """Schedule a data callback."""
-        if self.poll and self.data is None:
-            raise NoDataAvailableException
-        self.loop.call_soon_threadsafe(cb, self.data)
-
-    def _schedule_data_callbacks(self) -> None:
-        """Schedule a data callbacks."""
-        for cb in self.data_update_cbs:
-            self._schedule_data_callback(cb)
-
-    def unregister_data_callback(self, callback) -> None:
-        """Unregister a data update callback.
-
-        :param func callback: Takes one function, which should be unregistered.
-        """
-        if callback in self.data_update_cbs:
-            self.data_update_cbs.remove(callback)
-
-    def register_pong_callback(self, pong_callback) -> None:
-        """Register a pong callback.
-
-        It's not real ping/pong, but a way to check if the websocket
-        is still alive, by receiving an empty message.
-        """
-        if pong_callback not in self.pong_cbs:
-            self.pong_cbs.append(pong_callback)
-
-    def _schedule_pong_callback(self, cb) -> None:
-        """Schedule a pong callback."""
-        self.loop.call_soon_threadsafe(cb, self.last_ws_message)
-
-    def _schedule_pong_callbacks(self) -> None:
-        """Schedule pong callbacks."""
-        for cb in self.pong_cbs:
-            self._schedule_pong_callback(cb)
-
-    def unregister_pong_callback(self, pong_callback) -> None:
-        """Unregister a pong update callback.
-
-        :param func callback: Takes one function, which should be unregistered.
-        """
-        if pong_callback in self.pong_cbs:
-            self.pong_cbs.remove(pong_callback)
-
-    async def connect(self) -> None:
-        """Connect to the API.
-
-        This method handles the login. Also a REST task will be started, which
-        periodically polls the REST endpoint, when polling is set to true.
-        """
-        self._schedule_data_callbacks()
-
-        if self.poll:
-            await self.get_status()
-            self.rest_task = asyncio.create_task(self._rest_task())
-
-    async def start_listening(self) -> None:  # noqa: C901
-        """Start listening to the websocket (and receive initial state)."""
-        while not self.auth.ws.closed:
-            try:
-                msg = await self.auth.ws.receive(timeout=300)
-                if msg.type in (
-                    WSMsgType.CLOSE,
-                    WSMsgType.CLOSING,
-                    WSMsgType.CLOSED,
-                ):
-                    break
-                if msg.type == WSMsgType.TEXT:
-                    if not msg.data:
-                        self.last_ws_message = datetime.datetime.now(tz=datetime.UTC)
-                        _LOGGER.debug("last_ws_message:%s", self.last_ws_message)
-                        self._schedule_pong_callbacks()
-                    if msg.data:
-                        msg_dict = msg.json()
-                        if "type" in msg_dict:
-                            if msg_dict["type"] in EVENT_TYPES:
-                                _LOGGER.debug(
-                                    "Got %s, data: %s", msg_dict["type"], msg_dict
-                                )
-                                self._update_data(msg_dict)
-                            else:
-                                _LOGGER.warning(
-                                    "Received unknown ws type %s", msg_dict["type"]
-                                )
-                        elif "ready" in msg_dict and "connectionId" in msg_dict:
-                            _LOGGER.debug(
-                                "Websocket ready=%s (id='%s')",
-                                msg_dict["ready"],
-                                msg_dict["connectionId"],
-                            )
-                elif msg.type == WSMsgType.ERROR:
-                    continue
-            except TimeoutError as exc:
-                raise TimeoutException from exc
-
-    async def send_empty_message(self) -> None:
-        """Send an empty message every 60s."""
-        while True:
-            await asyncio.sleep(60)
-            _LOGGER.debug("ping:%s", datetime.datetime.now(tz=datetime.UTC))
-            await self.auth.ws.send_str("")
-
-    async def get_status(self) -> dict[str, MowerAttributes]:
-        """Get mower status via Rest."""
-        mower_list = await self.auth.get_json(AutomowerEndpoint.mowers)
-        for idx, _ent in enumerate(mower_list["data"]):
-            mower_list["data"][idx]["attributes"].update(
-                mower_list["data"][idx]["attributes"]["settings"]
-            )
-            del mower_list["data"][idx]["attributes"]["settings"]
-        self._data = mower_list
-        self.data = mower_list_to_dictionary_dataclass(self._data)
-        return self.data
 
     async def resume_schedule(self, mower_id: str):
         """Resume schedule.
 
         Remove any override on the Planner and let the mower
         resume to the schedule set by the Calendar.
         """
@@ -335,35 +194,183 @@
 
     async def error_confirm(self, mower_id: str):
         """Confirm non-fatal mower error."""
         body = {}  # type: dict[str, str]
         url = AutomowerEndpoint.error_confirm.format(mower_id=mower_id)
         await self.auth.post_json(url, json=body)
 
+
+class AutomowerSession:
+    """Automower API to communicate with an Automower.
+
+    The `AutomowerSession` is the primary API service for this library. It supports
+    operations like getting a status or sending commands.
+    """
+
+    def __init__(
+        self,
+        auth: AbstractAuth,
+        poll: bool = False,
+    ) -> None:
+        """Create a session.
+
+        :param class auth: The AbstractAuth class from aioautomower.auth.
+        :param bool poll: Poll data with rest if True.
+        """
+        self._data: Mapping[Any, Any] | None = {}
+        self.auth = auth
+        self.commands = _MowerCommands(self.auth)
+        self.pong_cbs: list = []
+        self.data_update_cbs: list = []
+        self.data: dict[str, MowerAttributes] = {}
+        self.last_ws_message: datetime.datetime
+        self.loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
+        self.poll = poll
+        self.rest_task: asyncio.Task | None = None
+
+    def register_data_callback(self, callback) -> None:
+        """Register a data update callback."""
+        if callback not in self.data_update_cbs:
+            self.data_update_cbs.append(callback)
+
+    def _schedule_data_callback(self, cb) -> None:
+        """Schedule a data callback."""
+        if self.poll and self.data is None:
+            raise NoDataAvailableException
+        self.loop.call_soon_threadsafe(cb, self.data)
+
+    def _schedule_data_callbacks(self) -> None:
+        """Schedule a data callbacks."""
+        for cb in self.data_update_cbs:
+            self._schedule_data_callback(cb)
+
+    def unregister_data_callback(self, callback) -> None:
+        """Unregister a data update callback.
+
+        :param func callback: Takes one function, which should be unregistered.
+        """
+        if callback in self.data_update_cbs:
+            self.data_update_cbs.remove(callback)
+
+    def register_pong_callback(self, pong_callback) -> None:
+        """Register a pong callback.
+
+        It's not real ping/pong, but a way to check if the websocket
+        is still alive, by receiving an empty message.
+        """
+        if pong_callback not in self.pong_cbs:
+            self.pong_cbs.append(pong_callback)
+
+    def _schedule_pong_callback(self, cb) -> None:
+        """Schedule a pong callback."""
+        self.loop.call_soon_threadsafe(cb, self.last_ws_message)
+
+    def _schedule_pong_callbacks(self) -> None:
+        """Schedule pong callbacks."""
+        for cb in self.pong_cbs:
+            self._schedule_pong_callback(cb)
+
+    def unregister_pong_callback(self, pong_callback) -> None:
+        """Unregister a pong update callback.
+
+        :param func callback: Takes one function, which should be unregistered.
+        """
+        if pong_callback in self.pong_cbs:
+            self.pong_cbs.remove(pong_callback)
+
+    async def connect(self) -> None:
+        """Connect to the API.
+
+        This method handles the login. Also a REST task will be started, which
+        periodically polls the REST endpoint, when polling is set to true.
+        """
+        self._schedule_data_callbacks()
+
+        if self.poll:
+            await self.get_status()
+            self.rest_task = asyncio.create_task(self._rest_task())
+
+    def handle_text_message(self, msg: WSMessage) -> None:
+        """Send an empty message every 60s."""
+        if not msg.data:
+            self.last_ws_message = datetime.datetime.now(tz=datetime.UTC)
+            _LOGGER.debug("last_ws_message:%s", self.last_ws_message)
+            self._schedule_pong_callbacks()
+        if msg.data:
+            msg_dict = msg.json()
+            if "type" in msg_dict:
+                if msg_dict["type"] in EVENT_TYPES:
+                    _LOGGER.debug("Got %s, data: %s", msg_dict["type"], msg_dict)
+                    self._update_data(msg_dict)
+                else:
+                    _LOGGER.warning("Received unknown ws type %s", msg_dict["type"])
+            elif "ready" in msg_dict and "connectionId" in msg_dict:
+                _LOGGER.debug(
+                    "Websocket ready=%s (id='%s')",
+                    msg_dict["ready"],
+                    msg_dict["connectionId"],
+                )
+
+    async def start_listening(self) -> None:
+        """Start listening to the websocket (and receive initial state)."""
+        while not self.auth.ws.closed:
+            try:
+                msg = await self.auth.ws.receive(timeout=300)
+                if msg.type in (
+                    WSMsgType.CLOSE,
+                    WSMsgType.CLOSING,
+                    WSMsgType.CLOSED,
+                ):
+                    break
+                if msg.type == WSMsgType.TEXT:
+                    self.handle_text_message(msg)
+                elif msg.type == WSMsgType.ERROR:
+                    continue
+            except TimeoutError as exc:
+                raise TimeoutException from exc
+
+    async def send_empty_message(self) -> None:
+        """Send an empty message every 60s."""
+        while True:
+            await asyncio.sleep(60)
+            _LOGGER.debug("ping:%s", datetime.datetime.now(tz=datetime.UTC))
+            await self.auth.ws.send_str("")
+
+    async def get_status(self) -> dict[str, MowerAttributes]:
+        """Get mower status via Rest."""
+        mower_list = await self.auth.get_json(AutomowerEndpoint.mowers)
+        for idx, _ent in enumerate(mower_list["data"]):
+            mower_list["data"][idx]["attributes"].update(
+                mower_list["data"][idx]["attributes"]["settings"]
+            )
+            del mower_list["data"][idx]["attributes"]["settings"]
+        self._data = mower_list
+        self.data = mower_list_to_dictionary_dataclass(self._data)
+        return self.data
+
     def _update_data(self, new_data) -> None:
+        """Update internal data, with new data from websocket.
+
+        Empty tasks are ignored, so we always know the tasks.
+        """
         if self._data is None:
             raise NoDataAvailableException
-        if self._data is not None:
-            for datum in self._data["data"]:
-                if datum["type"] == "mower" and datum["id"] == new_data["id"]:
-                    for attrib in new_data["attributes"]:
-                        try:
-                            tasks = new_data["attributes"]["calendar"]["tasks"]
-                            if len(tasks) == 0:
-                                temp_task = datum["attributes"]["calendar"]["tasks"]
-                                datum["attributes"][attrib] = new_data["attributes"][
-                                    attrib
-                                ]
-                                datum["attributes"]["calendar"]["tasks"] = temp_task
-                            if len(tasks) > 0:
-                                datum["attributes"][attrib] = new_data["attributes"][
-                                    attrib
-                                ]
-                        except KeyError:  # noqa: PERF203
-                            datum["attributes"][attrib] = new_data["attributes"][attrib]
+
+        for datum in self._data["data"]:
+            if datum["type"] == "mower" and datum["id"] == new_data["id"]:
+                new_attributes: Mapping[Any, Any] = new_data["attributes"]
+                value: Mapping[Any, Any]
+                for attrib, value in new_attributes.items():
+                    if attrib == "calendar":
+                        tasks = value.get("tasks", [])
+                        if tasks:
+                            datum["attributes"]["calendar"]["tasks"] = tasks
+                    else:
+                        datum["attributes"][attrib] = value
+
         self.data = mower_list_to_dictionary_dataclass(self._data)
         self._schedule_data_callbacks()
 
     async def _rest_task(self) -> None:
         """Poll data periodically via Rest."""
         while True:
             await self.get_status()
```

### Comparing `aioautomower-2024.4.4/src/aioautomower/utils.py` & `aioautomower-2024.5.0/src/aioautomower/utils.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.4/PKG-INFO` & `aioautomower-2024.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2024.4.4
+Version: 2024.5.0
 Summary: MPython module to talk to Husqvarna Automower.
 Home-page: https://github.com/Thomas55555/aioautomower
 License: Apache 2.0
 Author: Thomas55555
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

