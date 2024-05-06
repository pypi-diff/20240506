# Comparing `tmp/haystack_pydoc_tools-0.2.0.tar.gz` & `tmp/haystack_pydoc_tools-0.3.0.tar.gz`

## Comparing `haystack_pydoc_tools-0.2.0.tar` & `haystack_pydoc_tools-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.2.0/src/haystack_pydoc_tools/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.2.0/src/haystack_pydoc_tools/__init__.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.2.0/src/haystack_pydoc_tools/loaders.py
--rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.2.0/src/haystack_pydoc_tools/renderers.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.2.0/LICENSE
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.2.0/README.md
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.3.0/src/haystack_pydoc_tools/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.3.0/src/haystack_pydoc_tools/__init__.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.3.0/src/haystack_pydoc_tools/loaders.py
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.3.0/src/haystack_pydoc_tools/renderers.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.3.0/LICENSE
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.3.0/README.md
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 haystack_pydoc_tools-0.3.0/PKG-INFO
```

### Comparing `haystack_pydoc_tools-0.2.0/src/haystack_pydoc_tools/loaders.py` & `haystack_pydoc_tools-0.3.0/src/haystack_pydoc_tools/loaders.py`

 * *Files identical despite different names*

### Comparing `haystack_pydoc_tools-0.2.0/src/haystack_pydoc_tools/renderers.py` & `haystack_pydoc_tools-0.3.0/src/haystack_pydoc_tools/renderers.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     categories: t.Dict[str, str] = dataclasses.field(init=False)
     # This exposes a special `markdown` settings value that can be used to pass
     # parameters to the underlying `MarkdownRenderer`
     markdown: MarkdownRenderer = dataclasses.field(default_factory=MarkdownRenderer)
 
     def init(self, context: Context) -> None:
         self.markdown.init(context)
-        self.version = self._doc_version()
+        self.version = os.environ.get("PYDOC_TOOLS_HAYSTACK_DOC_VERSION", self._doc_version())
         self.categories = self._readme_categories(self.version)
 
     def _doc_version(self) -> str:
         """
         Returns the docs version.
         """
         root = Path(__file__).absolute().parent.parent.parent
```

### Comparing `haystack_pydoc_tools-0.2.0/.gitignore` & `haystack_pydoc_tools-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `haystack_pydoc_tools-0.2.0/LICENSE` & `haystack_pydoc_tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `haystack_pydoc_tools-0.2.0/README.md` & `haystack_pydoc_tools-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `haystack_pydoc_tools-0.2.0/pyproject.toml` & `haystack_pydoc_tools-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haystack_pydoc_tools-0.2.0/PKG-INFO` & `haystack_pydoc_tools-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: haystack-pydoc-tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pydoc custom tools for Haystack docs
 Project-URL: Documentation, https://github.com/unknown/haystack-pydoc-tools#readme
 Project-URL: Issues, https://github.com/unknown/haystack-pydoc-tools/issues
 Project-URL: Source, https://github.com/unknown/haystack-pydoc-tools
 Author-email: Massimiliano Pippi <mpippi@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

