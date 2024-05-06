# Comparing `tmp/fluentogram-1.1.6.tar.gz` & `tmp/fluentogram-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluentogram-1.1.6.tar", max compression
+gzip compressed data, was "fluentogram-1.1.7.tar", max compression
```

## Comparing `fluentogram-1.1.6.tar` & `fluentogram-1.1.7.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      362 2022-04-04 18:54:18.821854 fluentogram-1.1.6/fluentogram/__init__.py
--rw-r--r--   0        0        0       99 2022-04-04 18:54:16.851408 fluentogram-1.1.6/fluentogram/cli/__init__.py
--rw-r--r--   0        0        0      904 2022-09-30 13:10:45.284667 fluentogram-1.1.6/fluentogram/cli/cli.py
--rw-r--r--   0        0        0       88 2022-04-04 18:54:18.306738 fluentogram-1.1.6/fluentogram/exceptions/__init__.py
--rw-r--r--   0        0        0      546 2022-08-29 15:07:45.341090 fluentogram-1.1.6/fluentogram/exceptions/root_locale_translator.py
--rw-r--r--   0        0        0       77 2022-04-04 18:54:17.006443 fluentogram-1.1.6/fluentogram/misc/__init__.py
--rw-r--r--   0        0        0    10783 2022-04-04 18:54:18.823854 fluentogram-1.1.6/fluentogram/misc/timezones.py
--rw-r--r--   0        0        0       55 2022-04-04 18:54:17.662591 fluentogram-1.1.6/fluentogram/src/__init__.py
--rw-r--r--   0        0        0      202 2022-04-04 18:54:16.695373 fluentogram-1.1.6/fluentogram/src/abc/__init__.py
--rw-r--r--   0        0        0      911 2022-09-30 12:38:08.196786 fluentogram-1.1.6/fluentogram/src/abc/misc.py
--rw-r--r--   0        0        0      758 2022-10-04 10:20:36.002433 fluentogram-1.1.6/fluentogram/src/abc/runner.py
--rw-r--r--   0        0        0      803 2022-04-04 18:54:18.824855 fluentogram-1.1.6/fluentogram/src/abc/transformer.py
--rw-r--r--   0        0        0      752 2022-09-30 12:49:50.365428 fluentogram-1.1.6/fluentogram/src/abc/translator.py
--rw-r--r--   0        0        0      627 2022-09-30 12:54:18.877467 fluentogram-1.1.6/fluentogram/src/abc/translator_hub.py
--rw-r--r--   0        0        0      409 2022-04-04 18:54:18.827855 fluentogram-1.1.6/fluentogram/src/impl/__init__.py
--rw-r--r--   0        0        0      690 2022-09-30 12:50:54.524500 fluentogram-1.1.6/fluentogram/src/impl/attrib_tracer.py
--rw-r--r--   0        0        0     1391 2022-10-04 10:20:58.186145 fluentogram-1.1.6/fluentogram/src/impl/runner.py
--rw-r--r--   0        0        0      120 2022-04-04 18:54:18.465774 fluentogram-1.1.6/fluentogram/src/impl/transformers/__init__.py
--rw-r--r--   0        0        0      665 2022-09-30 12:43:18.616092 fluentogram-1.1.6/fluentogram/src/impl/transformers/datetime_transformer.py
--rw-r--r--   0        0        0     1440 2022-04-04 18:54:18.829856 fluentogram-1.1.6/fluentogram/src/impl/transformers/money_transformer.py
--rw-r--r--   0        0        0      914 2022-09-30 12:54:36.237425 fluentogram-1.1.6/fluentogram/src/impl/translator.py
--rw-r--r--   0        0        0     2581 2022-09-30 12:57:49.734164 fluentogram-1.1.6/fluentogram/src/impl/translator_hub.py
--rw-r--r--   0        0        0       42 2022-08-29 15:07:45.362090 fluentogram-1.1.6/fluentogram/tests/__init__.py
--rw-r--r--   0        0        0      345 2022-08-16 05:22:59.355753 fluentogram-1.1.6/fluentogram/tests/test_generator.py
--rw-r--r--   0        0        0     1487 2022-08-29 15:07:45.370090 fluentogram-1.1.6/fluentogram/tests/test_usage.py
--rw-r--r--   0        0        0      200 2022-08-10 21:04:56.611280 fluentogram-1.1.6/fluentogram/typing_generator/__init__.py
--rw-r--r--   0        0        0     2785 2022-08-30 05:33:37.212229 fluentogram-1.1.6/fluentogram/typing_generator/parsed_ftl.py
--rw-r--r--   0        0        0     2654 2022-08-11 11:42:16.129967 fluentogram-1.1.6/fluentogram/typing_generator/renderable_items.py
--rw-r--r--   0        0        0     1711 2022-08-29 15:07:45.378090 fluentogram-1.1.6/fluentogram/typing_generator/stubs.py
--rw-r--r--   0        0        0      102 2022-08-10 19:44:19.391878 fluentogram-1.1.6/fluentogram/typing_generator/translation_dto.py
--rw-r--r--   0        0        0     1793 2022-08-10 21:05:29.828277 fluentogram-1.1.6/fluentogram/typing_generator/tree.py
--rw-r--r--   0        0        0     1102 2022-04-04 18:54:18.994893 fluentogram-1.1.6/LICENSE
--rw-r--r--   0        0        0      473 2022-10-04 10:23:48.836523 fluentogram-1.1.6/pyproject.toml
--rw-r--r--   0        0        0      996 2022-10-04 10:24:42.979302 fluentogram-1.1.6/setup.py
--rw-r--r--   0        0        0      534 2022-10-04 10:24:42.979302 fluentogram-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-06 15:18:54.403300 fluentogram-1.1.7/LICENSE
+-rw-r--r--   0        0        0      343 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/__init__.py
+-rw-r--r--   0        0        0       94 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/cli/__init__.py
+-rw-r--r--   0        0        0     2405 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/cli/cli.py
+-rw-r--r--   0        0        0       86 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/exceptions/__init__.py
+-rw-r--r--   0        0        0      528 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/exceptions/root_locale_translator.py
+-rw-r--r--   0        0        0       73 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/misc/__init__.py
+-rw-r--r--   0        0        0    10338 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/misc/timezones.py
+-rw-r--r--   0        0        0       52 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/src/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/src/abc/__init__.py
+-rw-r--r--   0        0        0      878 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/src/abc/misc.py
+-rw-r--r--   0        0        0      731 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/src/abc/runner.py
+-rw-r--r--   0        0        0      780 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/src/abc/transformer.py
+-rw-r--r--   0        0        0      727 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/src/abc/translator.py
+-rw-r--r--   0        0        0      605 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/src/abc/translator_hub.py
+-rw-r--r--   0        0        0      394 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/src/impl/__init__.py
+-rw-r--r--   0        0        0      665 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/src/impl/attrib_tracer.py
+-rw-r--r--   0        0        0     2055 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/src/impl/filter.py
+-rw-r--r--   0        0        0     1352 2024-05-06 15:18:54.403300 fluentogram-1.1.7/fluentogram/src/impl/runner.py
+-rw-r--r--   0        0        0      295 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/src/impl/stubs_translator_runner.py
+-rw-r--r--   0        0        0      117 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/src/impl/transformers/__init__.py
+-rw-r--r--   0        0        0      639 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/src/impl/transformers/datetime_transformer.py
+-rw-r--r--   0        0        0     1397 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/src/impl/transformers/money_transformer.py
+-rw-r--r--   0        0        0      886 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/src/impl/translator.py
+-rw-r--r--   0        0        0     2514 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/src/impl/translator_hub.py
+-rw-r--r--   0        0        0       40 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/tests/__init__.py
+-rw-r--r--   0        0        0     5057 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/tests/test_stub_generation.py
+-rw-r--r--   0        0        0     1441 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/tests/test_usage.py
+-rw-r--r--   0        0        0      195 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/typing_generator/__init__.py
+-rw-r--r--   0        0        0     6628 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/typing_generator/parsed_ftl.py
+-rw-r--r--   0        0        0     2686 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/typing_generator/renderable_items.py
+-rw-r--r--   0        0        0     1660 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/typing_generator/stubs.py
+-rw-r--r--   0        0        0      137 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/typing_generator/translation_dto.py
+-rw-r--r--   0        0        0     1788 2024-05-06 15:18:54.407300 fluentogram-1.1.7/fluentogram/typing_generator/tree.py
+-rw-r--r--   0        0        0      496 2024-05-06 15:18:54.407300 fluentogram-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 fluentogram-1.1.7/PKG-INFO
```

### Comparing `fluentogram-1.1.6/fluentogram/src/abc/runner.py` & `fluentogram-1.1.7/fluentogram/src/abc/runner.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# coding=utf-8
-"""
-An abstract translator runner
-"""
-from abc import ABC, abstractmethod
-
-from fluentogram.src.abc import AbstractAttribTracer
-
-
-class AbstractTranslatorRunner(AbstractAttribTracer, ABC):
-    """This is one-shot per Telegram event translator with attrib tracer access way."""
-
-    @abstractmethod
-    def get(self, key: str, **kwargs) -> str:
-        """Fastest, direct way to use translator, without sugar-like typing supported attribute access way"""
-
-    @abstractmethod
-    def _get_translation(self, key, **kwargs) -> str:
-        ...
-
-    @abstractmethod
-    def __call__(self, **kwargs) -> str:
-        ...
-
-    @abstractmethod
-    def __getattr__(self, item: str) -> 'AbstractTranslatorRunner':
-        ...
+# coding=utf-8
+"""
+An abstract translator runner
+"""
+from abc import ABC, abstractmethod
+
+from fluentogram.src.abc import AbstractAttribTracer
+
+
+class AbstractTranslatorRunner(AbstractAttribTracer, ABC):
+    """This is one-shot per Telegram event translator with attrib tracer access way."""
+
+    @abstractmethod
+    def get(self, key: str, **kwargs) -> str:
+        """Fastest, direct way to use translator, without sugar-like typing supported attribute access way"""
+
+    @abstractmethod
+    def _get_translation(self, key, **kwargs) -> str:
+        ...
+
+    @abstractmethod
+    def __call__(self, **kwargs) -> str:
+        ...
+
+    @abstractmethod
+    def __getattr__(self, item: str) -> 'AbstractTranslatorRunner':
+        ...
```

### Comparing `fluentogram-1.1.6/fluentogram/src/abc/transformer.py` & `fluentogram-1.1.7/fluentogram/src/abc/transformer.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# coding=utf-8
-"""
-An AbstractDataTransformer object, using to transform any data before being passed to translator directly.
-"""
-from abc import ABC, abstractmethod
-from typing import Any
-
-
-class AbstractDataTransformer(ABC):
-    """
-    These transformers inspired by Functions of Project Fluent by Mozilla.
-    Of course, it's a simple function, like a
-
-    def function(money: Union[int, float], **kwargs) -> str: ...
-
-    which result passes through translator, into engine itself, like a Fluent or anything else.
-    """
-
-    @abstractmethod
-    def __new__(cls, data: Any, **kwargs) -> Any:
-        """Using incoming data, create an object representation of these data for your translator via all needed
-        parameters using kwargs"""
-        raise NotImplementedError
+# coding=utf-8
+"""
+An AbstractDataTransformer object, using to transform any data before being passed to translator directly.
+"""
+from abc import ABC, abstractmethod
+from typing import Any
+
+
+class AbstractDataTransformer(ABC):
+    """
+    These transformers inspired by Functions of Project Fluent by Mozilla.
+    Of course, it's a simple function, like a
+
+    def function(money: Union[int, float], **kwargs) -> str: ...
+
+    which result passes through translator, into engine itself, like a Fluent or anything else.
+    """
+
+    @abstractmethod
+    def __new__(cls, data: Any, **kwargs) -> Any:
+        """Using incoming data, create an object representation of these data for your translator via all needed
+        parameters using kwargs"""
+        raise NotImplementedError
```

### Comparing `fluentogram-1.1.6/fluentogram/src/abc/translator.py` & `fluentogram-1.1.7/fluentogram/src/abc/translator.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# coding=utf-8
-"""
-Translator as itself
-"""
-from abc import ABC, abstractmethod
-from typing import Any
-
-
-class AbstractTranslator(ABC):
-    """A translator class, implements key-value interface for your translator mechanism."""
-
-    @abstractmethod
-    def __init__(self, locale: str, translator: Any, separator: str = "-") -> None:
-        self.locale = locale
-        self.separator = separator
-        self.translator = translator
-
-    @abstractmethod
-    def get(self, key: str, **kwargs) -> str:
-        """
-        Convert a translation key to a translated text string.
-        Use kwargs dict to pass external data to the translator.
-        Expects to be fast and furious.
-        """
-        raise NotImplementedError
+# coding=utf-8
+"""
+Translator as itself
+"""
+from abc import ABC, abstractmethod
+from typing import Any
+
+
+class AbstractTranslator(ABC):
+    """A translator class, implements key-value interface for your translator mechanism."""
+
+    @abstractmethod
+    def __init__(self, locale: str, translator: Any, separator: str = "-") -> None:
+        self.locale = locale
+        self.separator = separator
+        self.translator = translator
+
+    @abstractmethod
+    def get(self, key: str, **kwargs) -> str:
+        """
+        Convert a translation key to a translated text string.
+        Use kwargs dict to pass external data to the translator.
+        Expects to be fast and furious.
+        """
+        raise NotImplementedError
```

### Comparing `fluentogram-1.1.6/fluentogram/src/abc/translator_hub.py` & `fluentogram-1.1.7/fluentogram/src/abc/translator_hub.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# coding=utf-8
-"""
-An abstract base for the Translator Hub object
-"""
-from abc import ABC, abstractmethod
-
-from fluentogram.src.abc.runner import AbstractTranslatorRunner
-
-
-class AbstractTranslatorsHub(ABC):
-    """This class should contain a couple of translator objects, usually one object per one locale."""
-
-    @abstractmethod
-    def __init__(self):
-        raise NotImplementedError
-
-    @abstractmethod
-    def get_translator_by_locale(self, locale: str) -> AbstractTranslatorRunner:
-        """
-        Returns a Translator object by selected locale
-        """
-        raise NotImplementedError
+# coding=utf-8
+"""
+An abstract base for the Translator Hub object
+"""
+from abc import ABC, abstractmethod
+
+from fluentogram.src.abc.runner import AbstractTranslatorRunner
+
+
+class AbstractTranslatorsHub(ABC):
+    """This class should contain a couple of translator objects, usually one object per one locale."""
+
+    @abstractmethod
+    def __init__(self):
+        raise NotImplementedError
+
+    @abstractmethod
+    def get_translator_by_locale(self, locale: str) -> AbstractTranslatorRunner:
+        """
+        Returns a Translator object by selected locale
+        """
+        raise NotImplementedError
```

### Comparing `fluentogram-1.1.6/fluentogram/src/impl/attrib_tracer.py` & `fluentogram-1.1.7/fluentogram/src/impl/attrib_tracer.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# coding=utf-8
-"""
-An AttribTracer implementation
-"""
-
-from fluentogram.src.abc import AbstractAttribTracer
-
-
-class AttribTracer(AbstractAttribTracer):
-    """Attribute tracer class for obj.attrib1.attrib2 access"""
-
-    def __init__(self) -> None:
-        self.request_line = ""
-
-    def _get_request_line(self) -> str:
-        request_line = self.request_line
-        self.request_line = ""
-        return request_line
-
-    def __getattr__(self, item) -> 'AttribTracer':
-        """
-        This method exists to map the "obj.attrib1.attrib2" access to "attrib1-attrib2" key.
-        """
-        self.request_line += f"{item}{self.separator}"
-        return self
+# coding=utf-8
+"""
+An AttribTracer implementation
+"""
+
+from fluentogram.src.abc import AbstractAttribTracer
+
+
+class AttribTracer(AbstractAttribTracer):
+    """Attribute tracer class for obj.attrib1.attrib2 access"""
+
+    def __init__(self) -> None:
+        self.request_line = ""
+
+    def _get_request_line(self) -> str:
+        request_line = self.request_line
+        self.request_line = ""
+        return request_line
+
+    def __getattr__(self, item) -> 'AttribTracer':
+        """
+        This method exists to map the "obj.attrib1.attrib2" access to "attrib1-attrib2" key.
+        """
+        self.request_line += f"{item}{self.separator}"
+        return self
```

### Comparing `fluentogram-1.1.6/fluentogram/src/impl/runner.py` & `fluentogram-1.1.7/fluentogram/src/impl/runner.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# coding=utf-8
-"""
-A translator runner by itself
-"""
-from typing import Iterable
-
-from fluentogram.src.abc import AbstractTranslator
-from fluentogram.src.abc.runner import AbstractTranslatorRunner
-from fluentogram.src.impl import AttribTracer
-
-
-class TranslatorRunner(AbstractTranslatorRunner, AttribTracer):
-    """This is one-shot per Telegram event translator with attrib tracer access way."""
-
-    def __init__(self, translators: Iterable[AbstractTranslator], separator: str = "-") -> None:
-        super().__init__()
-        self.translators = translators
-        self.separator = separator
-        self.request_line = ""
-
-    def get(self, key: str, **kwargs) -> str:
-        """Fastest, direct way to use translator, without sugar-like typing supported attribute access way"""
-        return self._get_translation(key, **kwargs)
-
-    def _get_translation(self, key, **kwargs):
-        for translator in self.translators:
-            try:
-                return translator.get(key, **kwargs)
-            except KeyError:
-                continue
-
-    def __call__(self, **kwargs) -> str:
-        text = self._get_translation(self.request_line[:-1], **kwargs)
-        self.request_line = ""
-        return text
-
-    def __getattr__(self, item: str) -> 'TranslatorRunner':
-        self.request_line += f"{item}{self.separator}"
-        return self
+# coding=utf-8
+"""
+A translator runner by itself
+"""
+from typing import Iterable
+
+from fluentogram.src.abc import AbstractTranslator
+from fluentogram.src.abc.runner import AbstractTranslatorRunner
+from fluentogram.src.impl import AttribTracer
+
+
+class TranslatorRunner(AbstractTranslatorRunner, AttribTracer):
+    """This is one-shot per Telegram event translator with attrib tracer access way."""
+
+    def __init__(self, translators: Iterable[AbstractTranslator], separator: str = "-") -> None:
+        super().__init__()
+        self.translators = translators
+        self.separator = separator
+        self.request_line = ""
+
+    def get(self, key: str, **kwargs) -> str:
+        """Fastest, direct way to use translator, without sugar-like typing supported attribute access way"""
+        return self._get_translation(key, **kwargs)
+
+    def _get_translation(self, key, **kwargs):
+        for translator in self.translators:
+            try:
+                return translator.get(key, **kwargs)
+            except KeyError:
+                continue
+
+    def __call__(self, **kwargs) -> str:
+        text = self._get_translation(self.request_line[:-1], **kwargs)
+        self.request_line = ""
+        return text
+
+    def __getattr__(self, item: str) -> 'TranslatorRunner':
+        self.request_line += f"{item}{self.separator}"
+        return self
```

### Comparing `fluentogram-1.1.6/fluentogram/src/impl/transformers/datetime_transformer.py` & `fluentogram-1.1.7/fluentogram/src/impl/transformers/datetime_transformer.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# coding=utf-8
-"""
-A DateTimeTransformer itself
-"""
-from datetime import datetime
-from typing import Union
-
-from fluent_compiler.types import fluent_date, FluentDateType, FluentNone
-
-from fluentogram.src.abc import AbstractDataTransformer
-
-
-class DateTimeTransformer(AbstractDataTransformer):
-    """This transformer converts a default python datetime object to FluentDate
-    Typings refer to https://github.com/tc39/ecma402
-    """
-
-    def __new__(
-            cls,
-            date: datetime,
-            **kwargs
-    ) -> Union[FluentDateType, FluentNone]:
-        return fluent_date(
-            date,
-            **kwargs
-        )
+# coding=utf-8
+"""
+A DateTimeTransformer itself
+"""
+from datetime import datetime
+from typing import Union
+
+from fluent_compiler.types import fluent_date, FluentDateType, FluentNone
+
+from fluentogram.src.abc import AbstractDataTransformer
+
+
+class DateTimeTransformer(AbstractDataTransformer):
+    """This transformer converts a default python datetime object to FluentDate
+    Typings refer to https://github.com/tc39/ecma402
+    """
+
+    def __new__(
+            cls,
+            date: datetime,
+            **kwargs
+    ) -> Union[FluentDateType, FluentNone]:
+        return fluent_date(
+            date,
+            **kwargs
+        )
```

### Comparing `fluentogram-1.1.6/fluentogram/src/impl/transformers/money_transformer.py` & `fluentogram-1.1.7/fluentogram/src/impl/transformers/money_transformer.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# coding=utf-8
-"""
-A MoneyTransformer by itself
-"""
-from decimal import Decimal
-from typing import Literal, Union
-
-from fluent_compiler.types import fluent_number, FluentNumber, FluentNone
-
-from fluentogram.src.abc import AbstractDataTransformer
-
-
-class MoneyTransformer(AbstractDataTransformer):
-    """This transformer converts a decimal object to FluentNumber with proper metadata.
-    Typings refer to https://github.com/tc39/ecma402
-    """
-
-    def __new__(
-        cls,
-        amount: Decimal,
-        currency: str,
-        currency_display: Union[
-            Literal["code"], Literal["symbol"], Literal["name"]
-        ] = "code",
-        use_grouping: bool = False,
-        minimum_significant_digits: int = None,
-        maximum_significant_digits: int = None,
-        minimum_fraction_digits: int = None,
-        maximum_fraction_digits: int = None,
-        **kwargs
-    ) -> Union[FluentNumber, FluentNone]:
-        return fluent_number(
-            amount,
-            style="currency",
-            currencyDisplay=currency_display,
-            currency=currency,
-            useGrouping=use_grouping,
-            minimumSignificantDigits=minimum_significant_digits,
-            maximumSignificantDigits=maximum_significant_digits,
-            minimumFractionDigits=minimum_fraction_digits,
-            maximumFractionDigits=maximum_fraction_digits,
-            **kwargs
-        )
+# coding=utf-8
+"""
+A MoneyTransformer by itself
+"""
+from decimal import Decimal
+from typing import Literal, Union
+
+from fluent_compiler.types import fluent_number, FluentNumber, FluentNone
+
+from fluentogram.src.abc import AbstractDataTransformer
+
+
+class MoneyTransformer(AbstractDataTransformer):
+    """This transformer converts a decimal object to FluentNumber with proper metadata.
+    Typings refer to https://github.com/tc39/ecma402
+    """
+
+    def __new__(
+        cls,
+        amount: Decimal,
+        currency: str,
+        currency_display: Union[
+            Literal["code"], Literal["symbol"], Literal["name"]
+        ] = "code",
+        use_grouping: bool = False,
+        minimum_significant_digits: int = None,
+        maximum_significant_digits: int = None,
+        minimum_fraction_digits: int = None,
+        maximum_fraction_digits: int = None,
+        **kwargs
+    ) -> Union[FluentNumber, FluentNone]:
+        return fluent_number(
+            amount,
+            style="currency",
+            currencyDisplay=currency_display,
+            currency=currency,
+            useGrouping=use_grouping,
+            minimumSignificantDigits=minimum_significant_digits,
+            maximumSignificantDigits=maximum_significant_digits,
+            minimumFractionDigits=minimum_fraction_digits,
+            maximumFractionDigits=maximum_fraction_digits,
+            **kwargs
+        )
```

### Comparing `fluentogram-1.1.6/fluentogram/src/impl/translator_hub.py` & `fluentogram-1.1.7/fluentogram/src/impl/translator_hub.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# coding=utf-8
-"""
-A Translator Hub, using as factory for Translator objects
-"""
-from typing import Dict, Iterable, List, Union
-
-from fluentogram.exceptions import NotImplementedRootLocaleTranslator
-from fluentogram.src.abc import AbstractTranslator, AbstractTranslatorsHub
-from fluentogram.src.impl import TranslatorRunner
-
-
-class TranslatorHub(AbstractTranslatorsHub):
-    """
-    This class implements a storage for all single-locale translators.
-    """
-
-    def __init__(
-            self,
-            locales_map: Dict[str, Union[str, Iterable[str]]],
-            translators: List[AbstractTranslator],
-            root_locale: str = "en",
-            separator: str = "-",
-    ) -> None:
-        self.locales_map = dict(
-            zip(
-                locales_map.keys(),
-                map(
-                    lambda lang: tuple([lang]) if isinstance(lang, str) else lang,
-                    locales_map.values()
-                )
-            )
-        )
-        self.translators = translators
-        self.root_locale = root_locale
-        self.separator = separator
-        self.storage: Dict[str, AbstractTranslator] = dict(
-            zip([translator.locale for translator in translators], translators)
-        )
-        if not self.storage.get(root_locale):
-            raise NotImplementedRootLocaleTranslator(self.root_locale)
-        self.translators_map: Dict[str, Iterable[AbstractTranslator]] = self._locales_map_parser(self.locales_map)
-
-    def _locales_map_parser(
-            self,
-            locales_map: Dict[str, Union[str, Iterable[str]]]
-    ) -> Dict[str, Iterable[AbstractTranslator]]:
-        return {
-            lang: tuple(
-                [self.storage.get(locale)
-                 for locale in translator_locales if locale in self.storage.keys()]
-            )
-            for lang, translator_locales in
-            locales_map.items()
-        }
-
-    def get_translator_by_locale(self, locale: str) -> TranslatorRunner:
-        """
-        Here is a little tricky moment.
-        There should be like a one-shot scheme.
-        For proper isolation, function returns TranslatorRunner new instance every time, not the same translator.
-        This trick makes "obj.attribute1.attribute2" access to be able.
-        You are able to do what you want, refer to the abstract class.
-        """
-        return TranslatorRunner(
-            translators=self.translators_map.get(locale) or self.translators_map[self.root_locale],
-            separator=self.separator
-        )
+# coding=utf-8
+"""
+A Translator Hub, using as factory for Translator objects
+"""
+from typing import Dict, Iterable, List, Union
+
+from fluentogram.exceptions import NotImplementedRootLocaleTranslator
+from fluentogram.src.abc import AbstractTranslator, AbstractTranslatorsHub
+from fluentogram.src.impl import TranslatorRunner
+
+
+class TranslatorHub(AbstractTranslatorsHub):
+    """
+    This class implements a storage for all single-locale translators.
+    """
+
+    def __init__(
+            self,
+            locales_map: Dict[str, Union[str, Iterable[str]]],
+            translators: List[AbstractTranslator],
+            root_locale: str = "en",
+            separator: str = "-",
+    ) -> None:
+        self.locales_map = dict(
+            zip(
+                locales_map.keys(),
+                map(
+                    lambda lang: tuple([lang]) if isinstance(lang, str) else lang,
+                    locales_map.values()
+                )
+            )
+        )
+        self.translators = translators
+        self.root_locale = root_locale
+        self.separator = separator
+        self.storage: Dict[str, AbstractTranslator] = dict(
+            zip([translator.locale for translator in translators], translators)
+        )
+        if not self.storage.get(root_locale):
+            raise NotImplementedRootLocaleTranslator(self.root_locale)
+        self.translators_map: Dict[str, Iterable[AbstractTranslator]] = self._locales_map_parser(self.locales_map)
+
+    def _locales_map_parser(
+            self,
+            locales_map: Dict[str, Union[str, Iterable[str]]]
+    ) -> Dict[str, Iterable[AbstractTranslator]]:
+        return {
+            lang: tuple(
+                [self.storage.get(locale)
+                 for locale in translator_locales if locale in self.storage.keys()]
+            )
+            for lang, translator_locales in
+            locales_map.items()
+        }
+
+    def get_translator_by_locale(self, locale: str) -> TranslatorRunner:
+        """
+        Here is a little tricky moment.
+        There should be like a one-shot scheme.
+        For proper isolation, function returns TranslatorRunner new instance every time, not the same translator.
+        This trick makes "obj.attribute1.attribute2" access to be able.
+        You are able to do what you want, refer to the abstract class.
+        """
+        return TranslatorRunner(
+            translators=self.translators_map.get(locale) or self.translators_map[self.root_locale],
+            separator=self.separator
+        )
```

### Comparing `fluentogram-1.1.6/fluentogram/tests/test_usage.py` & `fluentogram-1.1.7/fluentogram/tests/test_usage.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# coding=utf-8
-import unittest
-from datetime import datetime
-from decimal import Decimal
-
-from fluent_compiler.bundle import FluentBundle
-
-from fluentogram import (
-    FluentTranslator,
-    TranslatorHub,
-    TranslatorRunner,
-    MoneyTransformer,
-    DateTimeTransformer,
-)
-
-
-class BasicUsage(unittest.TestCase):
-    def test_full_usage(self):
-        example_ftl_file_content = """
-welcome = Welcome to the fluent aiogram addon!
-greet-by-name = Hello, { $user }!
-shop-success-payment = Your money, { $amount }, has been sent successfully at { $dt }.
-        """
-        t_hub = TranslatorHub(
-            {"ua": ("ua", "ru", "en"), "ru": ("ru", "en"), "en": ("en",)},
-            translators=[
-                FluentTranslator(
-                    locale="en",
-                    translator=FluentBundle.from_string(
-                        "en-US", example_ftl_file_content, use_isolating=False
-                    ),
-                )
-            ],
-            root_locale="en",
-        )
-        translator_runner: TranslatorRunner = t_hub.get_translator_by_locale("en")
-        print(
-            translator_runner.welcome(),
-            "\n",
-            translator_runner.greet.by.name(user="Alex"),
-            "\n",
-            translator_runner.shop.success.payment(
-                amount=MoneyTransformer(currency="$", amount=Decimal("500")),
-                dt=DateTimeTransformer(datetime.now()),
-            ),
-        )
+# coding=utf-8
+import unittest
+from datetime import datetime
+from decimal import Decimal
+
+from fluent_compiler.bundle import FluentBundle
+
+from fluentogram import (
+    FluentTranslator,
+    TranslatorHub,
+    TranslatorRunner,
+    MoneyTransformer,
+    DateTimeTransformer,
+)
+
+
+class BasicUsage(unittest.TestCase):
+    def test_full_usage(self):
+        example_ftl_file_content = """
+welcome = Welcome to the fluent aiogram addon!
+greet-by-name = Hello, { $user }!
+shop-success-payment = Your money, { $amount }, has been sent successfully at { $dt }.
+        """
+        t_hub = TranslatorHub(
+            {"ua": ("ua", "ru", "en"), "ru": ("ru", "en"), "en": ("en",)},
+            translators=[
+                FluentTranslator(
+                    locale="en",
+                    translator=FluentBundle.from_string(
+                        "en-US", example_ftl_file_content, use_isolating=False
+                    ),
+                )
+            ],
+            root_locale="en",
+        )
+        translator_runner: TranslatorRunner = t_hub.get_translator_by_locale("en")
+        print(
+            translator_runner.welcome(),
+            "\n",
+            translator_runner.greet.by.name(user="Alex"),
+            "\n",
+            translator_runner.shop.success.payment(
+                amount=MoneyTransformer(currency="$", amount=Decimal("500")),
+                dt=DateTimeTransformer(datetime.now()),
+            ),
+        )
```

### Comparing `fluentogram-1.1.6/fluentogram/typing_generator/stubs.py` & `fluentogram-1.1.7/fluentogram/typing_generator/stubs.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from typing import Iterator
-
-from fluentogram.typing_generator.renderable_items import (
-    Var,
-    Knot,
-    InternalMethod,
-    Method,
-    Runner,
-)
-from fluentogram.typing_generator.tree import Tree
-
-
-class Stubs:
-    def __init__(self, tree: Tree, root: str = "TranslatorRunner") -> None:
-        self.root = root
-        self.nodes = tree.elements
-        self.content: str = "from typing import Literal\n\n    "
-        for stub in self._gen_stubs():
-            self.content += stub
-
-    def _gen_stubs(self) -> Iterator[str]:
-        for path, node in self.nodes.items():
-            if node.is_leaf:
-                continue
-            if node.path:
-                knot = Knot(node.path)
-            else:
-                knot = Runner(self.root)
-            if node.children:
-                if node.value:
-                    knot.add_method(
-                        InternalMethod(node.value, args=node.translation_vars)
-                    )
-                for name, sub_node in node.children.items():
-                    if sub_node.is_leaf:
-                        if sub_node.value:
-                            knot.add_method(
-                                Method(
-                                    name, sub_node.value, args=sub_node.translation_vars
-                                )
-                            )
-                    else:
-                        knot.add_var(Var(name, sub_node.path))
-            yield knot.render()
-
-    def to_file(self, file_name: str) -> None:
-        with open(file_name, "w", encoding="utf-8") as f:
-            f.write(self.content)
-
-    def echo(self) -> str:
-        return self.content
+from typing import Iterator
+
+from fluentogram.typing_generator.renderable_items import (
+    Var,
+    Knot,
+    InternalMethod,
+    Method,
+    Runner,
+)
+from fluentogram.typing_generator.tree import Tree
+
+
+class Stubs:
+    def __init__(self, tree: Tree, root: str = "TranslatorRunner") -> None:
+        self.root = root
+        self.nodes = tree.elements
+        self.content: str = "from typing import Literal\n\n    "
+        for stub in self._gen_stubs():
+            self.content += stub
+
+    def _gen_stubs(self) -> Iterator[str]:
+        for path, node in self.nodes.items():
+            if node.is_leaf:
+                continue
+            if node.path:
+                knot = Knot(node.path)
+            else:
+                knot = Runner(self.root)
+            if node.children:
+                if node.value:
+                    knot.add_method(
+                        InternalMethod(node.value, args=node.translation_vars)
+                    )
+                for name, sub_node in node.children.items():
+                    if sub_node.is_leaf:
+                        if sub_node.value:
+                            knot.add_method(
+                                Method(
+                                    name, sub_node.value, args=sub_node.translation_vars
+                                )
+                            )
+                    else:
+                        knot.add_var(Var(name, sub_node.path))
+            yield knot.render()
+
+    def to_file(self, file_name: str) -> None:
+        with open(file_name, "w", encoding="utf-8") as f:
+            f.write(self.content)
+
+    def echo(self) -> str:
+        return self.content
```

### Comparing `fluentogram-1.1.6/fluentogram/typing_generator/tree.py` & `fluentogram-1.1.7/fluentogram/typing_generator/tree.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,59 @@
-from dataclasses import dataclass
-from typing import Optional
-
-from fluentogram.typing_generator.translation_dto import Translation
-
-
-@dataclass
-class TreeNode:
-    path: str
-    children: dict[str, "TreeNode"]
-    name: str
-    value: Optional[str] = None
-    translation_vars: Optional[list] = None
-
-    @property
-    def is_leaf(self) -> bool:
-        if not self.children:
-            return True
-        return False
-
-
-class Tree:
-    def __init__(
-            self,
-            ftl_syntax: dict[str, Translation],
-            separator: str = "-",
-            safe_separator: str = "",
-    ) -> None:
-        self.safe_separator = safe_separator
-        self.ftl_syntax = ftl_syntax
-        self.separator = separator
-        self.elements: dict[tuple[str, ...], TreeNode] = {}
-        for path, translation in ftl_syntax.items():
-            *point_path, name = path.split("-")
-            point_path.insert(0, "")
-            self._build(tuple(point_path), name, translation)
-
-    def path_to_str(self, path: tuple) -> str:
-        clean_path = map(lambda s: s[0].capitalize() + s[1:], filter(lambda x: x, path))
-        return self.safe_separator.join(clean_path)
-
-    def _build(self, path: tuple[str, ...], name: str, value=None) -> None:
-        own_class_def = TreeNode(
-            path=self.path_to_str(path + (name,)),
-            name=name,
-            value=value.text if value else "",
-            children={},
-            translation_vars=value.args if value else [],
-        )
-
-        if path:
-            if path not in self.elements:
-                self._build(path[:-1], path[-1])
-
-            self.elements[path].children[name] = own_class_def
-
-        self.elements.setdefault(path + (name,), own_class_def)
+from dataclasses import dataclass
+from typing import Optional
+
+from ordered_set import OrderedSet
+
+from fluentogram.typing_generator.translation_dto import Translation
+
+
+@dataclass
+class TreeNode:
+    path: str
+    children: dict[str, "TreeNode"]
+    name: str
+    value: Optional[str] = None
+    translation_vars: Optional[OrderedSet] = None
+
+    @property
+    def is_leaf(self) -> bool:
+        if not self.children:
+            return True
+        return False
+
+
+class Tree:
+    def __init__(
+            self,
+            ftl_syntax: dict[str, Translation],
+            separator: str = "-",
+            safe_separator: str = "",
+    ) -> None:
+        self.safe_separator = safe_separator
+        self.ftl_syntax = ftl_syntax
+        self.separator = separator
+        self.elements: dict[tuple[str, ...], TreeNode] = {}
+        for path, translation in ftl_syntax.items():
+            *point_path, name = path.split("-")
+            point_path.insert(0, "")
+            self._build(tuple(point_path), name, translation)
+
+    def path_to_str(self, path: tuple) -> str:
+        clean_path = map(lambda s: s[0].capitalize() + s[1:], filter(lambda x: x, path))
+        return self.safe_separator.join(clean_path)
+
+    def _build(self, path: tuple[str, ...], name: str, value=None) -> None:
+        own_class_def = TreeNode(
+            path=self.path_to_str(path + (name,)),
+            name=name,
+            value=value.text if value else "",
+            children={},
+            translation_vars=value.args if value else OrderedSet(),
+        )
+
+        if path:
+            if path not in self.elements:
+                self._build(path[:-1], path[-1])
+
+            self.elements[path].children[name] = own_class_def
+
+        self.elements.setdefault(path + (name,), own_class_def)
```

### Comparing `fluentogram-1.1.6/LICENSE` & `fluentogram-1.1.7/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 MIT. All rights reserved.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NON INFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 MIT. All rights reserved.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NON INFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `fluentogram-1.1.6/PKG-INFO` & `fluentogram-1.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: fluentogram
-Version: 1.1.6
+Version: 1.1.7
 Summary: A proper way to use an i18n mechanism with Aiogram3.
 Home-page: https://github.com/Arustinal/fluentogram
 License: MIT
 Author: Aleks
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fluent-compiler (>=0.3,<0.4)
+Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
+Requires-Dist: watchdog (>=2.3.0,<3.0.0)
 Project-URL: Repository, https://github.com/Arustinal/fluentogram
```

