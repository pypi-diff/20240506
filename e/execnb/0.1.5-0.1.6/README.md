# Comparing `tmp/execnb-0.1.5.tar.gz` & `tmp/execnb-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "execnb-0.1.5.tar", last modified: Mon Feb 13 00:36:41 2023, max compression
+gzip compressed data, was "execnb-0.1.6.tar", last modified: Mon May  6 00:46:31 2024, max compression
```

## Comparing `execnb-0.1.5.tar` & `execnb-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jhoward   (1002) jhoward   (1002)        0 2023-02-13 00:36:41.606759 execnb-0.1.5/
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)    11357 2022-06-07 21:20:02.000000 execnb-0.1.5/LICENSE
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)      111 2022-06-07 21:20:02.000000 execnb-0.1.5/MANIFEST.in
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     3139 2023-02-13 00:36:41.606759 execnb-0.1.5/PKG-INFO
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     2489 2022-09-29 18:42:45.000000 execnb-0.1.5/README.md
-drwxrwxr-x   0 jhoward   (1002) jhoward   (1002)        0 2023-02-13 00:36:41.606759 execnb-0.1.5/execnb/
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)       22 2023-02-09 21:05:46.000000 execnb-0.1.5/execnb/__init__.py
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     4833 2023-02-09 21:05:46.000000 execnb-0.1.5/execnb/_modidx.py
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     4285 2022-09-29 18:42:45.000000 execnb-0.1.5/execnb/fastshell.py
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     3568 2023-02-09 21:05:46.000000 execnb-0.1.5/execnb/nbio.py
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     8911 2023-02-09 21:05:46.000000 execnb-0.1.5/execnb/shell.py
-drwxrwxr-x   0 jhoward   (1002) jhoward   (1002)        0 2023-02-13 00:36:41.606759 execnb-0.1.5/execnb.egg-info/
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     3139 2023-02-13 00:36:41.000000 execnb-0.1.5/execnb.egg-info/PKG-INFO
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)      350 2023-02-13 00:36:41.000000 execnb-0.1.5/execnb.egg-info/SOURCES.txt
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)        1 2023-02-13 00:36:41.000000 execnb-0.1.5/execnb.egg-info/dependency_links.txt
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)       84 2023-02-13 00:36:41.000000 execnb-0.1.5/execnb.egg-info/entry_points.txt
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)        1 2022-06-07 21:20:12.000000 execnb-0.1.5/execnb.egg-info/not-zip-safe
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)       49 2023-02-13 00:36:41.000000 execnb-0.1.5/execnb.egg-info/requires.txt
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)        7 2023-02-13 00:36:41.000000 execnb-0.1.5/execnb.egg-info/top_level.txt
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)      963 2022-09-29 18:42:45.000000 execnb-0.1.5/settings.ini
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)       38 2023-02-13 00:36:41.606759 execnb-0.1.5/setup.cfg
--rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     2517 2022-07-30 09:21:44.000000 execnb-0.1.5/setup.py
+drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2024-05-06 00:46:31.923122 execnb-0.1.6/
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)    11357 2022-06-07 21:20:02.000000 execnb-0.1.6/LICENSE
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      111 2022-06-07 21:20:02.000000 execnb-0.1.6/MANIFEST.in
+-rw-r--r--   0 jhoward   (1000) jhoward   (1000)     3247 2024-05-06 00:46:31.923122 execnb-0.1.6/PKG-INFO
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2475 2024-05-06 00:44:32.000000 execnb-0.1.6/README.md
+drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2024-05-06 00:46:31.923122 execnb-0.1.6/execnb/
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       22 2023-02-13 00:40:25.000000 execnb-0.1.6/execnb/__init__.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     5229 2024-05-06 00:44:32.000000 execnb-0.1.6/execnb/_modidx.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     4285 2022-09-29 18:42:45.000000 execnb-0.1.6/execnb/fastshell.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     3660 2024-05-06 00:44:32.000000 execnb-0.1.6/execnb/nbio.py
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     9782 2024-05-06 00:44:32.000000 execnb-0.1.6/execnb/shell.py
+drwxrwxr-x   0 jhoward   (1000) jhoward   (1000)        0 2024-05-06 00:46:31.923122 execnb-0.1.6/execnb.egg-info/
+-rw-r--r--   0 jhoward   (1000) jhoward   (1000)     3247 2024-05-06 00:46:31.000000 execnb-0.1.6/execnb.egg-info/PKG-INFO
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      350 2024-05-06 00:46:31.000000 execnb-0.1.6/execnb.egg-info/SOURCES.txt
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2024-05-06 00:46:31.000000 execnb-0.1.6/execnb.egg-info/dependency_links.txt
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       84 2024-05-06 00:46:31.000000 execnb-0.1.6/execnb.egg-info/entry_points.txt
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        1 2022-06-07 21:20:12.000000 execnb-0.1.6/execnb.egg-info/not-zip-safe
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       49 2024-05-06 00:46:31.000000 execnb-0.1.6/execnb.egg-info/requires.txt
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)        7 2024-05-06 00:46:31.000000 execnb-0.1.6/execnb.egg-info/top_level.txt
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)      953 2024-05-06 00:44:32.000000 execnb-0.1.6/settings.ini
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)       38 2024-05-06 00:46:31.923122 execnb-0.1.6/setup.cfg
+-rw-rw-r--   0 jhoward   (1000) jhoward   (1000)     2517 2022-07-30 09:21:44.000000 execnb-0.1.6/setup.py
```

### Comparing `execnb-0.1.5/LICENSE` & `execnb-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `execnb-0.1.5/PKG-INFO` & `execnb-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: execnb
-Version: 0.1.5
+Version: 0.1.6
 Summary: A description of your project
-Home-page: https://github.com/fastai/execnb/tree/master/
+Home-page: https://github.com/fastai/execnb/
 Author: Jeremy Howard
 Author-email: j@fast.ai
 License: Apache Software License 2.0
 Keywords: some keywords
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: fastcore>=1.5.5
+Requires-Dist: ipython
+Provides-Extra: dev
+Requires-Dist: matplotlib; extra == "dev"
+Requires-Dist: Pillow; extra == "dev"
+
+# execnb
 
-execnb
-================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 [![CI](https://github.com/fastai/execnb/actions/workflows/test.yaml/badge.svg)](https://github.com/fastai/execnb/actions/workflows/test.yaml)
 [![Deploy to GitHub
 Pages](https://github.com/fastai/execnb/actions/workflows/deploy.yaml/badge.svg)](https://github.com/fastai/execnb/actions/workflows/deploy.yaml)
```

### Comparing `execnb-0.1.5/README.md` & `execnb-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-execnb
-================
+# execnb
+
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 [![CI](https://github.com/fastai/execnb/actions/workflows/test.yaml/badge.svg)](https://github.com/fastai/execnb/actions/workflows/test.yaml)
 [![Deploy to GitHub
 Pages](https://github.com/fastai/execnb/actions/workflows/deploy.yaml/badge.svg)](https://github.com/fastai/execnb/actions/workflows/deploy.yaml)
```

### Comparing `execnb-0.1.5/execnb/_modidx.py` & `execnb-0.1.6/execnb/_modidx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'master',
                 'doc_baseurl': '/execnb/',
                 'doc_host': 'https://fastai.github.io',
-                'git_url': 'https://github.com/fastai/execnb/tree/master/',
+                'git_url': 'https://github.com/fastai/execnb/',
                 'lib_path': 'execnb'},
   'syms': { 'execnb.fastshell': {},
             'execnb.nbio': { 'execnb.nbio.NbCell': ('nbio.html#nbcell', 'execnb/nbio.py'),
                              'execnb.nbio.NbCell.__eq__': ('nbio.html#nbcell.__eq__', 'execnb/nbio.py'),
                              'execnb.nbio.NbCell.__hash__': ('nbio.html#nbcell.__hash__', 'execnb/nbio.py'),
                              'execnb.nbio.NbCell.__init__': ('nbio.html#nbcell.__init__', 'execnb/nbio.py'),
                              'execnb.nbio.NbCell.parsed_': ('nbio.html#nbcell.parsed_', 'execnb/nbio.py'),
@@ -42,8 +42,12 @@
                               'execnb.shell._CaptureHook.quiet': ('shell.html#_capturehook.quiet', 'execnb/shell.py'),
                               'execnb.shell._CapturePub': ('shell.html#_capturepub', 'execnb/shell.py'),
                               'execnb.shell._CapturePub.publish': ('shell.html#_capturepub.publish', 'execnb/shell.py'),
                               'execnb.shell._false': ('shell.html#_false', 'execnb/shell.py'),
                               'execnb.shell._format_mimedata': ('shell.html#_format_mimedata', 'execnb/shell.py'),
                               'execnb.shell._out_exc': ('shell.html#_out_exc', 'execnb/shell.py'),
                               'execnb.shell._out_stream': ('shell.html#_out_stream', 'execnb/shell.py'),
-                              'execnb.shell.exec_nb': ('shell.html#exec_nb', 'execnb/shell.py')}}}
+                              'execnb.shell.exec_nb': ('shell.html#exec_nb', 'execnb/shell.py'),
+                              'execnb.shell.find_output': ('shell.html#find_output', 'execnb/shell.py'),
+                              'execnb.shell.out_error': ('shell.html#out_error', 'execnb/shell.py'),
+                              'execnb.shell.out_exec': ('shell.html#out_exec', 'execnb/shell.py'),
+                              'execnb.shell.out_stream': ('shell.html#out_stream', 'execnb/shell.py')}}}
```

### Comparing `execnb-0.1.5/execnb/fastshell.py` & `execnb-0.1.6/execnb/fastshell.py`

 * *Files identical despite different names*

### Comparing `execnb-0.1.5/execnb/nbio.py` & `execnb-0.1.6/execnb/nbio.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     def set_source(self, source):
         self.source = ''.join(source)
         if '_parsed_' in self: del(self['_parsed_'])
 
     def parsed_(self):
         if self.cell_type!='code' or self.source.strip()[:1] in ['%', '!']: return
-        if '_parsed_' not in self: 
+        if '_parsed_' not in self:
             try: self._parsed_ = ast.parse(self.source).body
             # you can assign the result of ! to a variable in a notebook cell
             # which will result in a syntax error if parsed with the ast module.
             except SyntaxError: return
         return self._parsed_
 
     def __hash__(self): return hash(self.source) + hash(self.cell_type)
@@ -66,14 +66,17 @@
 # %% ../nbs/01_nbio.ipynb 28
 def mk_cell(text,  # `source` attr in cell
             cell_type='code',  # `cell_type` attr in cell
             **kwargs):  # any other attrs to add to cell
     "Create an `NbCell` containing `text`"
     assert cell_type in {'code', 'markdown', 'raw'}
     if 'metadata' not in kwargs: kwargs['metadata']={}
+    if cell_type == 'code':
+        kwargs['outputs']=[]
+        kwargs['execution_count']=0
     return NbCell(0, dict(cell_type=cell_type, source=text, directives_={}, **kwargs))
 
 # %% ../nbs/01_nbio.ipynb 31
 def nb2dict(d, k=None):
     "Convert parsed notebook to `dict`"
     if k=='source': return d.splitlines(keepends=True)
     if isinstance(d, list): return list(map(nb2dict,d))
```

### Comparing `execnb-0.1.5/execnb/shell.py` & `execnb-0.1.6/execnb/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from .fastshell import FastInteractiveShell
 from .nbio import *
 from .nbio import _dict2obj
 
 from collections.abc import Callable
 
 # %% auto 0
-__all__ = ['CaptureShell', 'exec_nb']
+__all__ = ['CaptureShell', 'find_output', 'out_exec', 'out_stream', 'out_error', 'exec_nb']
 
 # %% ../nbs/02_shell.ipynb 4
 # IPython requires a DisplayHook and DisplayPublisher
 # We override `__call__` and `publish` to save outputs instead of printing them
 class _CaptureHook(DisplayHook):
     "Called when displaying a result"
 
@@ -151,15 +151,40 @@
     self._cell_idx = cell.idx_ + 1
     outs = self.run(cell.source)
     if outs:
         cell.outputs = _dict2obj(outs)
         for o in outs:
             if 'execution_count' in o: cell['execution_count'] = o['execution_count']
 
-# %% ../nbs/02_shell.ipynb 28
+# %% ../nbs/02_shell.ipynb 27
+def find_output(outp, # Output from `run`
+                ot='execute_result' # Output_type to find
+               ):
+    "Find first output of type `ot` in `CaptureShell.run` output"
+    return first(o for o in outp if o['output_type']==ot)
+
+# %% ../nbs/02_shell.ipynb 30
+def out_exec(outp):
+    "Get data from execution result in `outp`."
+    out = find_output(outp)
+    if out: return '\n'.join(first(out['data'].values()))
+
+# %% ../nbs/02_shell.ipynb 32
+def out_stream(outp):
+    "Get text from stream in `outp`."
+    out = find_output(outp, 'stream')
+    if out: return ('\n'.join(out['text'])).strip()
+
+# %% ../nbs/02_shell.ipynb 34
+def out_error(outp):
+    "Get traceback from error in `outp`."
+    out = find_output(outp, 'error')
+    if out: return '\n'.join(out['traceback'])
+
+# %% ../nbs/02_shell.ipynb 37
 def _false(o): return False
 
 @patch
 def run_all(self:CaptureShell,
             nb, # A notebook read with `nbclient` or `read_nb`
             exc_stop:bool=False, # Stop on exceptions?
             preproc:Callable=_false, # Called before each cell is executed
@@ -171,15 +196,15 @@
     if inject_code is not None: nb.cells[inject_idx].source = inject_code
     for cell in nb.cells:
         if not preproc(cell):
             self.cell(cell)
             postproc(cell)
         if self.exc and exc_stop: raise self.exc[1] from None
 
-# %% ../nbs/02_shell.ipynb 42
+# %% ../nbs/02_shell.ipynb 51
 @patch
 def execute(self:CaptureShell,
             src:str|Path, # Notebook path to read from
             dest:str|None=None, # Notebook path to write to
             exc_stop:bool=False, # Stop on exceptions?
             preproc:Callable=_false, # Called before each cell is executed
             postproc:Callable=_false, # Called after each cell is executed
@@ -192,27 +217,27 @@
     self._fname = src
     self.set_path(Path(src).parent.resolve())
     if inject_path is not None: inject_code = Path(inject_path).read_text()
     self.run_all(nb, exc_stop=exc_stop, preproc=preproc, postproc=postproc,
                  inject_code=inject_code, inject_idx=inject_idx)
     if dest: write_nb(nb, dest)
 
-# %% ../nbs/02_shell.ipynb 46
+# %% ../nbs/02_shell.ipynb 55
 @patch
 def prettytb(self:CaptureShell, 
              fname:str|Path=None): # filename to print alongside the traceback
     "Show a pretty traceback for notebooks, optionally printing `fname`."
     fname = fname if fname else self._fname
     _fence = '='*75
     cell_intro_str = f"While Executing Cell #{self._cell_idx}:" if self._cell_idx else "While Executing:"
     cell_str = f"\n{cell_intro_str}\n{self.exc[-1]}"
     fname_str = f' in {fname}' if fname else ''
     return f"{type(self.exc[1]).__name__}{fname_str}:\n{_fence}\n{cell_str}\n"
 
-# %% ../nbs/02_shell.ipynb 65
+# %% ../nbs/02_shell.ipynb 74
 @call_parse
 def exec_nb(
     src:str, # Notebook path to read from
     dest:str='', # Notebook path to write to
     exc_stop:bool=False, # Stop on exceptions?
     inject_code:str=None, # Code to inject into a cell
     inject_path:str=None, # Path to file containing code to inject into a cell
```

### Comparing `execnb-0.1.5/execnb.egg-info/PKG-INFO` & `execnb-0.1.6/execnb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: execnb
-Version: 0.1.5
+Version: 0.1.6
 Summary: A description of your project
-Home-page: https://github.com/fastai/execnb/tree/master/
+Home-page: https://github.com/fastai/execnb/
 Author: Jeremy Howard
 Author-email: j@fast.ai
 License: Apache Software License 2.0
 Keywords: some keywords
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: fastcore>=1.5.5
+Requires-Dist: ipython
+Provides-Extra: dev
+Requires-Dist: matplotlib; extra == "dev"
+Requires-Dist: Pillow; extra == "dev"
+
+# execnb
 
-execnb
-================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 [![CI](https://github.com/fastai/execnb/actions/workflows/test.yaml/badge.svg)](https://github.com/fastai/execnb/actions/workflows/test.yaml)
 [![Deploy to GitHub
 Pages](https://github.com/fastai/execnb/actions/workflows/deploy.yaml/badge.svg)](https://github.com/fastai/execnb/actions/workflows/deploy.yaml)
```

### Comparing `execnb-0.1.5/settings.ini` & `execnb-0.1.6/settings.ini`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 description = A description of your project
 copyright = Put your copyright info here
 keywords = some keywords
 user = fastai
 author = Jeremy Howard
 author_email = j@fast.ai
 branch = master
-version = 0.1.5
+version = 0.1.6
 min_python = 3.7
 requirements = fastcore>=1.5.5 ipython
 dev_requirements = matplotlib Pillow
 console_scripts = exec_nb=execnb.shell:exec_nb
 audience = Developers
 language = English
 custom_sidebar = False
@@ -21,21 +21,21 @@
 status = 2
 nbs_path = nbs
 doc_path = _docs
 recursive = False
 tst_flags = notest
 doc_host = https://fastai.github.io
 doc_baseurl = /execnb/
-git_url = https://github.com/fastai/execnb/tree/master/
+git_url = https://github.com/%(user)s/%(repo)s/
 lib_path = execnb
 title = execnb
 black_formatting = False
 readme_nb = index.ipynb
-allowed_metadata_keys = 
-allowed_cell_metadata_keys = 
+allowed_metadata_keys =
+allowed_cell_metadata_keys =
 conda_user = fastai
 preview_port = 3000
 preview_host = localhost
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
 put_version_in_init = True
```

### Comparing `execnb-0.1.5/setup.py` & `execnb-0.1.6/setup.py`

 * *Files identical despite different names*

