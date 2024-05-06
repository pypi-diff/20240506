# Comparing `tmp/pthugefileviewer-0.4.1.tar.gz` & `tmp/pthugefileviewer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pthugefileviewer-0.4.1.tar", last modified: Wed May  1 22:08:28 2024, max compression
+gzip compressed data, was "pthugefileviewer-0.5.0.tar", last modified: Mon May  6 21:08:07 2024, max compression
```

## Comparing `pthugefileviewer-0.4.1.tar` & `pthugefileviewer-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/pthugefileviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-01 22:08:28.000000 pthugefileviewer-0.4.1/pthugefileviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-01 22:08:28.000000 pthugefileviewer-0.4.1/pthugefileviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:08:28.000000 pthugefileviewer-0.4.1/pthugefileviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 22:08:28.000000 pthugefileviewer-0.4.1/pthugefileviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 22:08:28.000000 pthugefileviewer-0.4.1/pthugefileviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:08:28.571317 pthugefileviewer-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/src/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7986 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/src/bin/hfv-regexbuild
--rwxr-xr-x   0 runner    (1001) docker     (127)     1895 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/src/bin/hfv-view
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/src/pthugefileviewer/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/src/pthugefileviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/src/pthugefileviewer/hugefilevieweruicontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/src/pthugefileviewer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/tests/test_hfv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:08:07.665507 pthugefileviewer-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-06 21:08:07.665507 pthugefileviewer-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:08:07.665507 pthugefileviewer-0.5.0/pthugefileviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-06 21:08:07.000000 pthugefileviewer-0.5.0/pthugefileviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-06 21:08:07.000000 pthugefileviewer-0.5.0/pthugefileviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:08:07.000000 pthugefileviewer-0.5.0/pthugefileviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 21:08:07.000000 pthugefileviewer-0.5.0/pthugefileviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 21:08:07.000000 pthugefileviewer-0.5.0/pthugefileviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-06 21:08:07.665507 pthugefileviewer-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:08:07.661507 pthugefileviewer-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:08:07.665507 pthugefileviewer-0.5.0/src/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7986 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/src/bin/hfv-regexbuild
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1895 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/src/bin/hfv-view
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:08:07.665507 pthugefileviewer-0.5.0/src/pthugefileviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/src/pthugefileviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/src/pthugefileviewer/hugefilevieweruicontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/src/pthugefileviewer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:08:07.665507 pthugefileviewer-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/tests/test_hfv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-06 21:08:00.000000 pthugefileviewer-0.5.0/tests/test_hfv_regex.py
```

### Comparing `pthugefileviewer-0.4.1/LICENSE` & `pthugefileviewer-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.4.1/PKG-INFO` & `pthugefileviewer-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pthugefileviewer
-Version: 0.4.1
+Version: 0.5.0
 Summary: Huge file viewer control for prompt-toolkit
 Home-page: http://github.com/lpenz/pthugefileviewer
 Author: "Leandro Lisboa Penz"
 Author-email: "lpenz@lpenz.org"
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

### Comparing `pthugefileviewer-0.4.1/README.md` & `pthugefileviewer-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.4.1/pthugefileviewer.egg-info/PKG-INFO` & `pthugefileviewer-0.5.0/pthugefileviewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pthugefileviewer
-Version: 0.4.1
+Version: 0.5.0
 Summary: Huge file viewer control for prompt-toolkit
 Home-page: http://github.com/lpenz/pthugefileviewer
 Author: "Leandro Lisboa Penz"
 Author-email: "lpenz@lpenz.org"
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

### Comparing `pthugefileviewer-0.4.1/setup.cfg` & `pthugefileviewer-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pthugefileviewer
-version = 0.4.1
+version = 0.5.0
 description = Huge file viewer control for prompt-toolkit
 license = MIT
 license_files = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = "Leandro Lisboa Penz"
 author_email = "lpenz@lpenz.org"
```

### Comparing `pthugefileviewer-0.4.1/src/bin/hfv-regexbuild` & `pthugefileviewer-0.5.0/src/bin/hfv-regexbuild`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.4.1/src/bin/hfv-view` & `pthugefileviewer-0.5.0/src/bin/hfv-view`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.4.1/src/pthugefileviewer/hugefilevieweruicontrol.py` & `pthugefileviewer-0.5.0/src/pthugefileviewer/hugefilevieweruicontrol.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Control for the huge file widget"""
 
 import io
 import mmap
 import re
 from contextlib import contextmanager
+from enum import Enum
 from typing import TYPE_CHECKING, Generator, Iterator, List, Optional  # noqa: I101
 
 from prompt_toolkit.formatted_text import StyleAndTextTuples
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.key_binding.key_bindings import KeyBindingsBase
 from prompt_toolkit.key_binding.key_processor import KeyPressEvent
 from prompt_toolkit.layout.controls import UIContent, UIControl
@@ -89,18 +90,21 @@
         with self.tmp_offset():
             for _ in range(self._height):
                 line = self._mm.readline()
                 if not line:
                     break
                 yield line.rstrip()
 
-    def update_lines(self) -> None:
-        self._lines = [
+    def get_lines_style(self) -> List[StyleAndTextTuples]:
+        return [
             [("", line.decode("utf-8", errors="replace"))] for line in self.get_lines()
         ]
+
+    def update_lines(self) -> None:
+        self._lines = self.get_lines_style()
         if self.height > len(self._lines) and self.offset < self._offset_max:
             self.go_up(self._height - len(self._lines))
 
     def get_char(self, offset: Optional[int] = None) -> bytes:
         with self.tmp_offset():
             if offset is not None:
                 self._mm.seek(offset)
@@ -192,14 +196,17 @@
     def go_pageup(self) -> None:
         self.go_up(self.height)
 
     def go_pagedown(self) -> None:
         self.go_down(self.height)
 
 
+OffsetEvent = Enum("OffsetEvent", ["RE_START", "RE_END", "NEWLINE", "END"])
+
+
 class HugeFileViewerRegexUIControl(HugeFileViewerUIControl):
     def __init__(self, fd: io.BufferedReader):
         self.regex: Optional[re.Pattern[bytes]] = None
         self.regex_ok: Optional[re.Pattern[bytes]] = None
         HugeFileViewerUIControl.__init__(self, fd)
 
     def re_search(
@@ -222,43 +229,59 @@
         m = self.re_search(self.regex, offset)
         if m:
             self.go_line_offset(m.end())
             self.go_down(1)
         else:
             self.update_lines()
 
-    def update_lines(self) -> None:
+    def get_lines_style(self) -> List[StyleAndTextTuples]:
         contents = b"\n".join(self.get_lines())
-        m = None
+        matches = []
         if self.regex is not None:
-            m = self.regex.search(contents)
-        if m:
+            matches = list(self.regex.finditer(contents))
+        if matches:
             self.regex_ok = self.regex
-            style = "class:match"
-        elif not m and self.regex_ok is not None:
-            m = self.regex_ok.search(contents)
-            style = "class:oldmatch"
-        if not m:
-            HugeFileViewerUIControl.update_lines(self)
-            return
-        start = m.start()
-        end = m.end()
-        pre, matched, pos = contents[:start], contents[start:end], contents[end:]
-        self._lines = []
+            re_style = "class:match"
+        elif not matches and self.regex_ok is not None:
+            matches = list(self.regex_ok.finditer(contents))
+            re_style = "class:oldmatch"
+        else:
+            re_style = ""
+        offsetList = []
+        for m in matches:
+            offsetList.append((m.start(), OffsetEvent.RE_START))
+            offsetList.append((m.end(), OffsetEvent.RE_END))
+        o = 0
+        while (newline := contents.find(b"\n", o)) != -1:
+            offsetList.append((newline, OffsetEvent.NEWLINE))
+            o = newline + 1
+        offsetList.append((len(contents), OffsetEvent.END))
+        offsetList.sort(key=lambda x: x[0])
+        offsets: dict[int, set[OffsetEvent]] = {}
+        for offset, what in offsetList:
+            events = offsets.setdefault(offset, set())
+            events.add(what)
+            if OffsetEvent.RE_START in events and OffsetEvent.RE_END in events:
+                events.remove(OffsetEvent.RE_START)
+                events.remove(OffsetEvent.RE_END)
+            if not events:
+                offsets.pop(offset)
+        linestyle = []
         current: StyleAndTextTuples = []
-        lines = pre.split(b"\n")
-        for i, line in enumerate(lines):
-            current += [("", line.decode("utf-8"))]
-            if i != len(lines) - 1:
-                self._lines.append(current)
-                current = []
-        lines = matched.split(b"\n")
-        for i, line in enumerate(lines):
-            current += [(style, line.decode("utf-8"))]
-            if i != len(lines) - 1:
-                self._lines.append(current)
+        styles: set[str] = set()
+        o_curr = 0
+        for o_next, events in offsets.items():
+            if o_next > o_curr:
+                current.append(
+                    (" ".join(styles), contents[o_curr:o_next].decode("utf-8"))
+                )
+            if OffsetEvent.RE_START in events:
+                styles.add(re_style)
+                o_curr = o_next
+            if OffsetEvent.RE_END in events:
+                styles.remove(re_style)
+                o_curr = o_next
+            if OffsetEvent.NEWLINE in events or OffsetEvent.END in events:
+                linestyle.append(current)
                 current = []
-        lines = pos.split(b"\n")
-        for i, line in enumerate(lines):
-            current += [("", line.decode("utf-8"))]
-            self._lines.append(current)
-            current = []
+                o_curr = o_next + 1
+        return linestyle
```

### Comparing `pthugefileviewer-0.4.1/tests/test_hfv.py` & `pthugefileviewer-0.5.0/tests/test_hfv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""hugefilevieweruicontrol tests"""
+"""HugeFileViewerUIControl tests"""
 
 import tempfile
 import unittest
 from typing import List
 
 from pthugefileviewer.hugefilevieweruicontrol import HugeFileViewerUIControl
 
@@ -44,14 +44,20 @@
         control = self.controlLines(1, lines, self.newlines)
         self.assertEqual(get_lines(control), tobytes(lines))
 
     def test_too_high(self) -> None:
         control = self.controlNums(3, 1, self.newlines)
         self.assertEqual(get_lines(control), [b"0"])
 
+    def test_linestyle(self) -> None:
+        control = self.controlNums(3, 5, self.newlines)
+        self.assertEqual(
+            control.get_lines_style(), [[("", "0")], [("", "1")], [("", "2")]]
+        )
+
     def test_updown(self) -> None:
         control = self.controlNums(3, 5, self.newlines)
         self.assertEqual(get_lines(control), [b"0", b"1", b"2"])
         self.assertEqual(get_lines(control), [b"0", b"1", b"2"])
         control.go_down()
         self.assertEqual(get_lines(control), [b"1", b"2", b"3"])
         control.go_down()
@@ -164,15 +170,15 @@
         self.assertEqual(get_lines(control), [b"4", b"5", b"6"])
         control.go_pageup()
         self.assertEqual(get_lines(control), [b"1", b"2", b""])
         control.go_pagedown()
         self.assertEqual(get_lines(control), [b"4", b"5", b"6"])
 
 
-class TestGapNewlineAtEnd(unittest.TestCase, Base):
+class TestGapNewlineAtEnd(TestGap):
     newlines = 1
 
 
 class TestNewlineTopBottom(unittest.TestCase, Base):
     def test_updown(self) -> None:
         lines = [""] + [f"{i}" for i in range(7)]
         control = self.controlLines(3, lines, 3)
```

