# Comparing `tmp/relax_py-0.5.0.tar.gz` & `tmp/relax_py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relax_py-0.5.0.tar", max compression
+gzip compressed data, was "relax_py-0.6.0.tar", max compression
```

## Comparing `relax_py-0.5.0.tar` & `relax_py-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       54 2023-11-05 14:43:09.827813 relax_py-0.5.0/README.md
--rw-r--r--   0        0        0     1591 2024-02-17 09:10:44.732230 relax_py-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-05 14:43:09.827813 relax_py-0.5.0/relax/__init__.py
--rw-r--r--   0        0        0    11671 2024-02-17 22:12:11.882405 relax_py-0.5.0/relax/app.py
--rw-r--r--   0        0        0    16348 2024-02-17 09:22:01.240731 relax_py-0.5.0/relax/html.py
--rw-r--r--   0        0        0     3899 2024-01-26 20:13:41.089047 relax_py-0.5.0/relax/injection.py
--rw-r--r--   0        0        0      414 2024-01-26 20:09:32.123920 relax_py-0.5.0/relax/injection.pyi
--rw-r--r--   0        0        0        0 2023-11-05 14:43:09.831147 relax_py-0.5.0/relax/py.typed
--rw-r--r--   0        0        0     1279 2023-12-19 21:31:47.401817 relax_py-0.5.0/relax/test.py
--rw-r--r--   0        0        0      240 2023-12-19 21:31:54.925092 relax_py-0.5.0/relax/test.pyi
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 relax_py-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-05-06 17:44:37.940558 relax_py-0.6.0/README.md
+-rw-r--r--   0        0        0     1773 2024-05-06 17:45:00.956435 relax_py-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 15:39:40.407368 relax_py-0.6.0/relax/__init__.py
+-rw-r--r--   0        0        0    13360 2024-05-06 15:41:26.463803 relax_py-0.6.0/relax/app.py
+-rw-r--r--   0        0        0     1241 2024-05-06 15:39:40.415368 relax_py-0.6.0/relax/config.py
+-rw-r--r--   0        0        0    18508 2024-05-06 15:39:40.415368 relax_py-0.6.0/relax/html.py
+-rw-r--r--   0        0        0     5568 2024-05-06 15:39:59.271153 relax_py-0.6.0/relax/injection.py
+-rw-r--r--   0        0        0     1049 2024-05-06 15:39:45.211312 relax_py-0.6.0/relax/js/hmr_reload.js
+-rw-r--r--   0        0        0        0 2024-05-06 15:39:40.415368 relax_py-0.6.0/relax/py.typed
+-rw-r--r--   0        0        0     4365 2024-05-06 15:39:40.415368 relax_py-0.6.0/relax/server.py
+-rw-r--r--   0        0        0     1089 2024-05-06 15:39:40.415368 relax_py-0.6.0/relax/test.py
+-rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 relax_py-0.6.0/PKG-INFO
```

### Comparing `relax_py-0.5.0/relax/html.py` & `relax_py-0.6.0/relax/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import warnings
+import sys
+from pathlib import Path
 from collections.abc import Iterable
 from html import escape
-from typing import Literal, Protocol, Self, Sequence
+from typing import Literal, Protocol, Self, Sequence, TypeVar
 
 from starlette.datastructures import URL
 
 HREFTarget = Literal["_blank", "_self", "_parent", "_top"]
 
 InputType = Literal[
     "text",
@@ -25,21 +27,63 @@
 HTMXRequestType = Literal["get", "post", "put", "delete"]
 
 
 class InvalidHTMLError(Exception):
     ...
 
 
+T = TypeVar("T")
+
+
 class Element(Protocol):
     _parent: "Tag | None"
     name: str
 
     def render(self) -> str:
         ...
 
+    def set_id(self, value: str) -> Self:
+        ...
+
+    @property
+    def id(self) -> str | None:
+        ...
+
+    def classes(self, classes: list[str]) -> Self:
+        ...
+
+    def attrs(self, attrs: dict) -> Self:
+        ...
+
+    def hx_get(
+        self,
+        target: str | URL,
+        hx_encoding: Literal["multipart/form-data"] | None = None,
+        hx_target: str | Self | None = None,
+        hx_swap: Literal[
+            "innerHTML",
+            "outerHTML",
+            "beforebegin",
+            "afterbegin",
+            "beforeend",
+            "afterend",
+            "delete",
+            "none",
+        ]
+        | None = None,
+        **kwargs: str,
+    ) -> Self:
+        ...
+
+
+class Component(Element, Protocol):
+    @property
+    def id(self) -> str:
+        ...
+
 
 class SelfClosingTag(Element):
     name: str
 
     def __init__(
         self,
         *,
@@ -52,15 +96,15 @@
         self._attributes: dict = {}
         self._classes: list[str] = []
         if classes:
             self.classes(classes)
         if attrs:
             self.attrs(attrs)
         if id:
-            self.id(id)
+            self.set_id(id)
         if hyperscript:
             self.hyperscript(hyperscript)
         self._parent: Tag | None = None
 
     def render(self) -> str:
         return f"<{self.name} {self._render_attributes()} />"
 
@@ -85,22 +129,26 @@
         self._attributes["_"] = command
         return self
 
     def attrs(self, attrs: dict) -> Self:
         self._attributes.update(attrs)
         return self
 
-    def id(self, value: str) -> Self:
+    def set_id(self, value: str) -> Self:
         self._attributes["id"] = value
         return self
 
+    @property
+    def id(self) -> str | None:
+        return self._attributes["id"]
+
     def _htmx(
         self,
         request_type: HTMXRequestType,
-        target: str,
+        target: str | URL,
         hx_encoding: Literal["multipart/form-data"] | None = None,
         hx_target: str | Self | None = None,
         hx_swap: Literal[
             "innerHTML",
             "outerHTML",
             "beforebegin",
             "afterbegin",
@@ -278,15 +326,15 @@
 
 
 class Fragment(Tag):
     name = "<>"
 
     def __init__(
         self,
-        children: Sequence[Element] | None,
+        children: Sequence[Element | None] | None,
     ) -> None:
         super().__init__()
         self.insert(children)
 
     def render(self) -> str:
         return super()._render_children()
 
@@ -326,16 +374,23 @@
         self,
         *,
         type: ButtonType | None = None,
         classes: list[str] | None = None,
         attrs: dict | None = None,
         id: str | None = None,
         hyperscript: str | None = None,
+        text: str | None = None,
     ) -> None:
-        super().__init__(classes=classes, attrs=attrs, id=id, hyperscript=hyperscript)
+        super().__init__(
+            classes=classes,
+            attrs=attrs,
+            id=id,
+            hyperscript=hyperscript,
+            text=text,
+        )
         if type:
             self._attributes["type"] = type
         else:
             self._attributes["type"] = "button"
 
 
 class form(Tag):
@@ -360,31 +415,44 @@
 
 
 class a(Tag):
     name = "a"
 
     def __init__(
         self,
-        href: str,
+        href: str | URL,
         target: HREFTarget | None = None,
         classes: list[str] | None = None,
         attrs: dict | None = None,
         id: str | None = None,
         hyperscript: str | None = None,
+        text: str | None = None,
     ) -> None:
-        super().__init__(classes=classes, attrs=attrs, id=id, hyperscript=hyperscript)
+        super().__init__(
+            classes=classes,
+            attrs=attrs,
+            id=id,
+            hyperscript=hyperscript,
+            text=text,
+        )
         self._attributes["href"] = href
         if target:
             self._attributes["target"] = target
 
 
 class li(Tag):
     name = "li"
 
     def render(self) -> str:
+        if not self._parent:
+            warnings.warn(
+                f'"{self.name}" element should be a child of "ul" or "ol"',
+                stacklevel=2,
+            )
+
         if self._parent and self._parent.name not in ["ul", "ol"]:
             warnings.warn(
                 f'"{self.name}" element should be a child of "ul" or "ol"',
                 stacklevel=2,
             )
         return super().render()
 
@@ -395,43 +463,25 @@
 
 
 class label(Tag):
     name = "label"
 
     def __init__(
         self,
-        _for: str,
+        _for: str | None = None,
         classes: list[str] | None = None,
         attrs: dict | None = None,
         id: str | None = None,
         hyperscript: str | None = None,
     ) -> None:
         super().__init__(classes=classes, attrs=attrs, id=id, hyperscript=hyperscript)
-        self._attributes["for"] = _for
-
-    def render(self) -> str:
-        if self._parent and all(
-            sibling.name not in ["input"] for sibling in self._parent._children
-        ):
-            warnings.warn(
-                f'"{self.name}" element should have a sibling "input"',
-                stacklevel=2,
-            )
-        return super().render()
+        if _for is not None:
+            self._attributes["for"] = _for
 
 
-# TODO:
-# class
-# x-show
-# fill
-# stroke-linecap
-# stroke-linejoin
-# stroke-width
-# viewBox
-# stroke
 class svg(Tag):
     name = "svg"
 
 
 class path(Tag):
     name = "path"
 
@@ -546,14 +596,15 @@
         self._attributes["name"] = name
         self._attributes["type"] = type
         if placeholder:
             self._attributes["placeholder"] = placeholder
         if disabled is True:
             self._attributes["disabled"] = True
 
+
 class meta(SelfClosingTag):
     name = "meta"
 
     def __init__(
         self,
         *,
         charset: str | None = None,
@@ -568,16 +619,18 @@
         else:
             super().__init__(attrs={"name": name, "content": content})
 
 
 class link(SelfClosingTag):
     name = "link"
 
-    def __init__(self, *, href: str, rel: str) -> None:
+    def __init__(self, *, href: str, rel: str, type: str | None = None) -> None:
         super().__init__(attrs={"href": href, "rel": rel})
+        if type is not None:
+            self._attributes["type"] = type
 
 
 class title(Tag):
     name = "title"
 
     def __init__(self, name: str) -> None:
         super().__init__()
@@ -596,25 +649,32 @@
     name = "script"
 
     def __init__(
         self,
         js: str | None = None,
         src: str | None = None,
         attrs: dict | None = None,
+        *,
+        type: Literal["importmap", "module", "speculationrules"] | None = None,
+        defer: bool = False,
     ) -> None:
         super().__init__()
         if js is not None:
             self.text(js)
         elif src is not None:
             self._attributes["src"] = src
         else:
             msg = "<script> element must have js or src"
             raise InvalidHTMLError(msg)
         if attrs is not None:
             self._attributes.update(attrs)
+        if defer:
+            self._attributes["defer"] = "true"
+        if type is not None:
+            self._attributes["type"] = type
 
     # sorry mate can't help you escape that
     # your risk
     def _render_children(self) -> str:
         return self._text + "".join([child.render() for child in self._children])
 
 
@@ -637,7 +697,55 @@
         super().__init__(classes=classes, attrs=attrs, id=id, hyperscript=hyperscript)
         self._attributes["lang"] = lang
 
     # TODO: ensure only head | body can be inserted
 
     def render(self) -> str:
         return "<!DOCTYPE html>" + super().render()
+
+
+class aside(Tag):
+    name = "aside"
+
+class details(Tag):
+    name = "details"
+
+class summary(Tag):
+    name = "summary"
+
+class dialog(Tag):
+    name = "dialog"
+
+class h1(Tag):
+    name = "h1"
+
+
+class h2(Tag):
+    name = "h2"
+
+
+class h3(Tag):
+    name = "h3"
+
+
+class h4(Tag):
+    name = "h4"
+
+class h5(Tag):
+    name = "h5"
+
+class figure(Tag):
+    name = "figure"
+
+def hmr_script() -> list[script]:
+    file_path = sys.modules[__name__].__file__
+    if file_path is None:
+        msg = "Cannot find current file path"
+        raise RuntimeError(msg)
+    current_path = Path(file_path)
+    with (current_path.parent / "js" / "hmr_reload.js").open() as f:
+        return [
+            script(
+                js=f.read(),
+            ),
+            script(src="https://unpkg.com/idiomorph@0.3.0"),
+        ]
```

