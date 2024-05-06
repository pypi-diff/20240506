# Comparing `tmp/mrfifo-0.6.tar.gz` & `tmp/mrfifo-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrfifo-0.6.tar", last modified: Tue Apr 30 11:45:12 2024, max compression
+gzip compressed data, was "mrfifo-0.7.tar", last modified: Mon May  6 09:36:36 2024, max compression
```

## Comparing `mrfifo-0.6.tar` & `mrfifo-0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 11:45:12.490376 mrfifo-0.6/
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      115 2024-02-20 15:34:36.000000 mrfifo-0.6/.coveragerc
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 11:45:12.170377 mrfifo-0.6/.github/
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 11:45:12.286376 mrfifo-0.6/.github/workflows/
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1362 2024-02-20 15:34:36.000000 mrfifo-0.6/.github/workflows/python-package.yml
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1084 2024-03-14 08:18:30.000000 mrfifo-0.6/.github/workflows/python-publish.yml
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     3078 2024-02-20 15:34:36.000000 mrfifo-0.6/.gitignore
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1068 2024-02-20 15:34:36.000000 mrfifo-0.6/LICENSE
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     9962 2024-04-30 11:45:12.490376 mrfifo-0.6/PKG-INFO
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     9226 2024-04-30 11:29:24.000000 mrfifo-0.6/README.md
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1015 2024-04-15 12:46:55.000000 mrfifo-0.6/ROADMAP.md
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      281 2024-02-20 15:34:36.000000 mrfifo-0.6/environment.yaml
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 11:45:12.366376 mrfifo-0.6/mrfifo/
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)    14649 2024-04-17 14:37:36.000000 mrfifo-0.6/mrfifo/__init__.py
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      106 2024-04-30 11:30:03.000000 mrfifo-0.6/mrfifo/contrib.py
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)   452785 2024-04-30 11:45:11.000000 mrfifo-0.6/mrfifo/fast_loops.c
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)    11119 2024-04-17 14:37:22.000000 mrfifo-0.6/mrfifo/fast_loops.pyx
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1823 2024-02-20 15:34:36.000000 mrfifo-0.6/mrfifo/parallel.py
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     3351 2024-03-19 09:22:55.000000 mrfifo-0.6/mrfifo/parts.py
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1475 2024-03-01 13:20:46.000000 mrfifo-0.6/mrfifo/plumbing.py
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     2410 2024-04-15 12:46:55.000000 mrfifo-0.6/mrfifo/util.py
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 11:45:12.434376 mrfifo-0.6/mrfifo.egg-info/
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     9962 2024-04-30 11:45:12.000000 mrfifo-0.6/mrfifo.egg-info/PKG-INFO
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      588 2024-04-30 11:45:12.000000 mrfifo-0.6/mrfifo.egg-info/SOURCES.txt
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)        1 2024-04-30 11:45:12.000000 mrfifo-0.6/mrfifo.egg-info/dependency_links.txt
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)        1 2024-02-20 15:34:58.000000 mrfifo-0.6/mrfifo.egg-info/not-zip-safe
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       61 2024-04-30 11:45:12.000000 mrfifo-0.6/mrfifo.egg-info/requires.txt
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)        7 2024-04-30 11:45:12.000000 mrfifo-0.6/mrfifo.egg-info/top_level.txt
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      417 2024-04-30 11:38:33.000000 mrfifo-0.6/pyproject.toml
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      901 2024-04-30 11:45:12.502376 mrfifo-0.6/setup.cfg
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      974 2024-02-20 15:34:36.000000 mrfifo-0.6/setup.py
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 11:45:12.466376 mrfifo-0.6/test_data/
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       41 2024-02-20 15:34:36.000000 mrfifo-0.6/test_data/simple.txt
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       50 2024-02-20 15:34:36.000000 mrfifo-0.6/test_data/simple.txt.gz
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     3294 2024-02-20 15:34:36.000000 mrfifo-0.6/test_data/tiny_test.bam
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 11:45:12.474376 mrfifo-0.6/tests/
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)    13948 2024-04-17 14:44:56.000000 mrfifo-0.6/tests/test_cy.py
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-05-06 09:36:36.136545 mrfifo-0.7/
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      115 2024-02-20 15:34:36.000000 mrfifo-0.7/.coveragerc
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-05-06 09:36:35.808546 mrfifo-0.7/.github/
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-05-06 09:36:35.936545 mrfifo-0.7/.github/workflows/
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1362 2024-02-20 15:34:36.000000 mrfifo-0.7/.github/workflows/python-package.yml
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1084 2024-03-14 08:18:30.000000 mrfifo-0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     3078 2024-02-20 15:34:36.000000 mrfifo-0.7/.gitignore
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1068 2024-02-20 15:34:36.000000 mrfifo-0.7/LICENSE
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     9962 2024-05-06 09:36:36.132545 mrfifo-0.7/PKG-INFO
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     9226 2024-04-30 11:29:24.000000 mrfifo-0.7/README.md
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1015 2024-04-15 12:46:55.000000 mrfifo-0.7/ROADMAP.md
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      281 2024-02-20 15:34:36.000000 mrfifo-0.7/environment.yaml
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-05-06 09:36:36.024545 mrfifo-0.7/mrfifo/
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)    11606 2024-05-06 09:08:05.000000 mrfifo-0.7/mrfifo/__init__.py
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      106 2024-05-06 09:29:29.000000 mrfifo-0.7/mrfifo/contrib.py
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)   462588 2024-05-06 09:36:28.000000 mrfifo-0.7/mrfifo/fast_loops.c
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)    11482 2024-05-06 09:05:54.000000 mrfifo-0.7/mrfifo/fast_loops.pyx
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1823 2024-02-20 15:34:36.000000 mrfifo-0.7/mrfifo/parallel.py
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     3351 2024-03-19 09:22:55.000000 mrfifo-0.7/mrfifo/parts.py
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     5571 2024-05-06 09:10:12.000000 mrfifo-0.7/mrfifo/plumbing.py
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     2410 2024-04-15 12:46:55.000000 mrfifo-0.7/mrfifo/util.py
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-05-06 09:36:36.080545 mrfifo-0.7/mrfifo.egg-info/
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     9962 2024-05-06 09:36:34.000000 mrfifo-0.7/mrfifo.egg-info/PKG-INFO
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      588 2024-05-06 09:36:34.000000 mrfifo-0.7/mrfifo.egg-info/SOURCES.txt
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)        1 2024-05-06 09:36:34.000000 mrfifo-0.7/mrfifo.egg-info/dependency_links.txt
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)        1 2024-02-20 15:34:58.000000 mrfifo-0.7/mrfifo.egg-info/not-zip-safe
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       61 2024-05-06 09:36:34.000000 mrfifo-0.7/mrfifo.egg-info/requires.txt
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)        7 2024-05-06 09:36:34.000000 mrfifo-0.7/mrfifo.egg-info/top_level.txt
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      417 2024-04-30 11:38:33.000000 mrfifo-0.7/pyproject.toml
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      901 2024-05-06 09:36:36.144545 mrfifo-0.7/setup.cfg
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      974 2024-02-20 15:34:36.000000 mrfifo-0.7/setup.py
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-05-06 09:36:36.108545 mrfifo-0.7/test_data/
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       41 2024-02-20 15:34:36.000000 mrfifo-0.7/test_data/simple.txt
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       50 2024-02-20 15:34:36.000000 mrfifo-0.7/test_data/simple.txt.gz
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     3294 2024-02-20 15:34:36.000000 mrfifo-0.7/test_data/tiny_test.bam
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-05-06 09:36:36.120545 mrfifo-0.7/tests/
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)    13949 2024-05-06 09:09:28.000000 mrfifo-0.7/tests/test_cy.py
```

### Comparing `mrfifo-0.6/.github/workflows/python-package.yml` & `mrfifo-0.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/.github/workflows/python-publish.yml` & `mrfifo-0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/.gitignore` & `mrfifo-0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/LICENSE` & `mrfifo-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/PKG-INFO` & `mrfifo-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrfifo
-Version: 0.6
+Version: 0.7
 Summary: Map-Reduce parallelism over FIFOs (named pipes)
 Home-page: https://github.com/marvin-jens/mrfifo
 Author: Marvin Jens
 Author-email: marvin.jens@charite.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/marvin-jens/mrfifo/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mrfifo-0.6/README.md` & `mrfifo-0.7/README.md`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/ROADMAP.md` & `mrfifo-0.7/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/mrfifo/__init__.py` & `mrfifo-0.7/mrfifo/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,139 +1,24 @@
 from .contrib import __version__, __license__, __author__, __email__
 
 import logging
 from functools import wraps
 from collections import defaultdict
 
-from . import parallel
 from . import plumbing
 from . import parts
 from . import util
 
+from .plumbing import FIFO, fifo_routed
+
 
 class WorkflowError(Exception):
     pass
 
 
-class FIFO:
-    def __init__(self, name, mode, n=None):
-        self.logger = logging.getLogger(f"mrfifo.FIFO.{name}")
-        self.name = name
-        self.mode = mode
-        self.n = n
-        self.file_objects = []
-
-        assert mode[0] in ["r", "w"]
-
-    def _format_name(self, context):
-        return FIFO(self.name.format(**context), self.mode, n=self.n)
-
-    def is_collection(self):
-        return self.n is not None
-
-    def is_reader(self):
-        return self.mode[0] == "r"
-
-    def get_names(self, **kw):
-        if self.is_collection():
-            return [self.name.format(n=i, **kw) for i in range(self.n)]
-        else:
-            return [
-                self.name,
-            ]
-
-    def open(self, pipe_dict, manage_fifos=True, **kw):
-        from mrfifo.plumbing import open_named_pipe
-
-        if manage_fifos:
-            self.file_objects = [
-                open_named_pipe(pipe_dict[name], mode=self.mode)
-                for name in self.get_names(**kw)
-            ]
-
-            if self.is_collection():
-                return self.file_objects
-            else:
-                return self.file_objects[0]
-        else:
-            # unmanaged, return paths to fifos instead of open files
-            paths = [pipe_dict[name] for name in self.get_names(**kw)]
-            if self.is_collection():
-                return paths
-            else:
-                return paths[0]
-
-    def close(self):
-        for f in self.file_objects:
-            self.logger.debug(f"closing {f}")
-            f.flush()
-            f.close()
-            self.logger.debug(f"done closing {f}")
-
-        self.file_objects = []
-
-    def __repr__(self):
-        return f"FIFO({self.mode} names={self.get_names()}) n={self.n}"
-
-
-# class ITER(object):
-#     def __init__(self, iterable):
-#         self.iterable = iterable
-#         self.it = iter(self.iterable)
-
-#     def get(self):
-#         return next(self.it)  # this will eventually raise StopIteration
-
-
-def fifo_routed(
-    f, pass_internals=False, fifo_name_format={}, _manage_fifos=True, **kwargs
-):
-    from functools import wraps
-
-    fifo_vars = {}
-    kw = {}
-    for k, v in kwargs.items():
-        # print(f"{k} : {v} {type(v)}")
-        if type(v) is FIFO:
-            if fifo_name_format:
-                v = v._format_name(fifo_name_format)
-            fifo_vars[k] = v
-        # elif type(v) is ITER:
-        #     # replace the ITER object with whatever is returned at the current iteration
-        #     # this may raise a StopIteration
-        #     kw[k] = v.get()
-        else:
-            kw[k] = v
-
-    @wraps(f)
-    def wrapper(
-        result_dict={}, pipe_dict={}, exc_dict={}, job_name="job", args=(), **kwds
-    ):
-        kwargs = kw.copy()
-        kwargs.update(**kwds)
-
-        for target, fifo in fifo_vars.items():
-            kwargs[target] = fifo.open(pipe_dict, manage_fifos=_manage_fifos)
-
-        with parallel.ExceptionLogging(name=job_name, exc_dict=exc_dict) as el:
-            try:
-                if pass_internals:
-                    kwargs["_job_name"] = job_name
-                    kwargs["_logger"] = el.logger
-
-                res = f(*args, **kwargs)
-                result_dict[job_name] = res
-
-            finally:
-                for fifo in fifo_vars.values():
-                    fifo.close()
-
-    return wrapper, fifo_vars
-
-
 class Job:
     def __init__(self, func, result_dict={}, exc_dict={}, pipe_dict={}, name="job"):
         self.name = name
         self.func = func
         self.result_dict = result_dict
         self.exc_dict = exc_dict
         self.pipe_dict = pipe_dict
@@ -148,31 +33,32 @@
                 pipe_dict=self.pipe_dict,
                 result_dict=self.result_dict,
                 exc_dict=self.exc_dict,
                 job_name=self.name,
             ),
         )
 
-    def start(self):  # , pipes):
+    def start(self):
         assert self.p is None
-        self.p = self.create()  # pipes)
+        self.p = self.create()
         self.p.start()
 
     def join(self):
         assert self.p is not None
         self.p.join()
 
     def __str__(self):
         return f"Job({self.name}) func={self.func.__name__}"
 
 
 class Workflow:
-    def __init__(self, name, n=4):
+    def __init__(self, name, n=4, total_pipe_buffer_MB=16):
         self.name = name
         self.n = n
+        self.total_pipe_buffer = int(total_pipe_buffer_MB * 1048576)
         self.logger = logging.getLogger(f"{self.name}.Workflow")
         self.job_count_by_pattern = defaultdict(int)
 
         self._jobs = []
         self._subs = []
 
         self._fifo_readers = defaultdict(list)
@@ -299,15 +185,17 @@
                 self._fifo_balance[name] += bal
 
         # gather all named pipes that are required
         pipe_names = self.get_pipe_list()
         self.logger.debug(f"pipe_names={pipe_names}")
         self.check()
         if not dry_run:
-            with plumbing.create_named_pipes(pipe_names) as pipes:
+            with plumbing.create_named_pipes(
+                pipe_names, total_pipe_buffer=self.total_pipe_buffer
+            ) as pipes:
                 self.pipe_dict.update(pipes)
                 # start all processes in reverse data-flow order
                 for job in reversed(self._jobs):
                     if type(job) is Workflow:
                         sub = job
                         # we have a sub-workflow!
                         for job in reversed(sub._jobs):
@@ -399,24 +287,26 @@
         *argc,
         func=parts.distributor,
         header_fifo="",
         header_detect_func=None,
         header_broadcast=False,
         job_name="{workflow}.dist{n}",
         _manage_fifos=False,
+        pass_internals=True,
         **kwargs,
     ):
 
         return self.add_job(
             *argc,
             job_name=job_name,
             func=func,
             assert_n_writer_ge=1,
             assert_n_reader_ge=1,
             _manage_fifos=_manage_fifos,
+            pass_internals=pass_internals,
             header_fifo=header_fifo,
             header_detect_func=header_detect_func,
             header_broadcast=header_broadcast,
             **kwargs,
         )
 
     def workers(self, *argc, n=4, func=None, job_name="{workflow}.worker{n}", **kwargs):
@@ -437,25 +327,27 @@
         *argc,
         func=parts.collector,
         inputs=[],
         output="/dev/stdout",
         header_fifo="",
         job_name="{workflow}.collect{n}",
         _manage_fifos=False,
+        pass_internals=True,
         **kwargs,
     ):
 
         return self.add_job(
             *argc,
             job_name=job_name,
             func=func,
             inputs=inputs,
             output=output,
             assert_n_reader_ge=1,
             _manage_fifos=_manage_fifos,
+            pass_internals=pass_internals,
             header_fifo=header_fifo,
             **kwargs,
         )
 
     def funnel(self, *argc, job_name="{workflow}.funnel{n}", **kwargs):
         # basically an alias for add_job()
         return self.add_job(*argc, job_name=job_name, **kwargs)
```

### Comparing `mrfifo-0.6/mrfifo/fast_loops.c` & `mrfifo-0.7/mrfifo/fast_loops.c`

 * *Files 2% similar despite different names*

```diff
@@ -2215,14 +2215,15 @@
 static const char __pyx_k_[] = "";
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_j[] = "j";
 static const char __pyx_k_k[] = "k";
 static const char __pyx_k_n[] = "n";
 static const char __pyx_k__2[] = "*";
 static const char __pyx_k__9[] = "?";
+static const char __pyx_k_kw[] = "kw";
 static const char __pyx_k_fin[] = "fin";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_sub[] = "sub";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_CB_Z[] = "\tCB:Z:";
 static const char __pyx_k_fout[] = "fout";
 static const char __pyx_k_line[] = "line";
@@ -2254,14 +2255,15 @@
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_chunk_size[] = "chunk_size";
 static const char __pyx_k_distribute[] = "distribute";
 static const char __pyx_k_fifo_names[] = "fifo_names";
 static const char __pyx_k_sub_buffer[] = "sub_buffer";
 static const char __pyx_k_sub_lead_c[] = "sub_lead_c";
 static const char __pyx_k_sub_lookup[] = "sub_lookup";
+static const char __pyx_k_buffer_size[] = "_buffer_size";
 static const char __pyx_k_fifo_closed[] = "fifo_closed";
 static const char __pyx_k_header_fifo[] = "header_fifo";
 static const char __pyx_k_in_buf_size[] = "in_buf_size";
 static const char __pyx_k_sub_match_c[] = "sub_match_c";
 static const char __pyx_k_can_not_find[] = "can not find ";
 static const char __pyx_k_fifo_buffers[] = "fifo_buffers";
 static const char __pyx_k_header_bytes[] = "header_bytes";
@@ -2277,17 +2279,17 @@
 static const char __pyx_k_mrfifo_fast_loops[] = "mrfifo.fast_loops";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_header_detect_func[] = "header_detect_func";
 static const char __pyx_k_distribute_by_substr[] = "distribute_by_substr";
 static const char __pyx_k_mrfifo_fast_loops_pyx[] = "mrfifo/fast_loops.pyx";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_6mrfifo_10fast_loops_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fin_name, PyObject *__pyx_v_fifo_names, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_detect_func, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_header_broadcast); /* proto */
-static PyObject *__pyx_pf_6mrfifo_10fast_loops_2distribute_by_substr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fin_name, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_sub_lookup, size_t __pyx_v_sub_size, PyObject *__pyx_v_sub_lead, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_detect_func, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_header_broadcast); /* proto */
-static PyObject *__pyx_pf_6mrfifo_10fast_loops_4collect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_fout_name, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_custom_header, int __pyx_v_n_reopen_inputs); /* proto */
+static PyObject *__pyx_pf_6mrfifo_10fast_loops_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fin_name, PyObject *__pyx_v_fifo_names, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_detect_func, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_header_broadcast, size_t __pyx_v__buffer_size, CYTHON_UNUSED PyObject *__pyx_v_kw); /* proto */
+static PyObject *__pyx_pf_6mrfifo_10fast_loops_2distribute_by_substr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fin_name, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_sub_lookup, size_t __pyx_v_sub_size, PyObject *__pyx_v_sub_lead, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_detect_func, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_header_broadcast, PyObject *__pyx_v__buffer_size, CYTHON_UNUSED PyObject *__pyx_v_kw); /* proto */
+static PyObject *__pyx_pf_6mrfifo_10fast_loops_4collect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_fout_name, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v__buffer_size, PyObject *__pyx_v_custom_header, int __pyx_v_n_reopen_inputs, CYTHON_UNUSED PyObject *__pyx_v_kw); /* proto */
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, 0, 0, 0, 0};
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
@@ -2327,14 +2329,15 @@
   PyObject *__pyx_kp_b_CB_Z;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s__2;
   PyObject *__pyx_n_s__9;
   PyObject *__pyx_kp_u_as_substring_in;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_buffer;
+  PyObject *__pyx_n_s_buffer_size;
   PyObject *__pyx_kp_u_can_not_find;
   PyObject *__pyx_n_s_chunk_size;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_collect;
   PyObject *__pyx_n_s_custom_header;
   PyObject *__pyx_n_s_distribute;
   PyObject *__pyx_n_s_distribute_by_substr;
@@ -2357,14 +2360,15 @@
   PyObject *__pyx_n_s_i;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_in_buf_size;
   PyObject *__pyx_n_s_initializing;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_n_s_j;
   PyObject *__pyx_n_s_k;
+  PyObject *__pyx_n_s_kw;
   PyObject *__pyx_n_s_lead_n;
   PyObject *__pyx_n_s_line;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_mrfifo_fast_loops;
   PyObject *__pyx_kp_s_mrfifo_fast_loops_pyx;
   PyObject *__pyx_n_s_n;
   PyObject *__pyx_n_s_n_ins;
@@ -2445,14 +2449,15 @@
   Py_CLEAR(clear_module_state->__pyx_kp_b_CB_Z);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s__2);
   Py_CLEAR(clear_module_state->__pyx_n_s__9);
   Py_CLEAR(clear_module_state->__pyx_kp_u_as_substring_in);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_buffer);
+  Py_CLEAR(clear_module_state->__pyx_n_s_buffer_size);
   Py_CLEAR(clear_module_state->__pyx_kp_u_can_not_find);
   Py_CLEAR(clear_module_state->__pyx_n_s_chunk_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_collect);
   Py_CLEAR(clear_module_state->__pyx_n_s_custom_header);
   Py_CLEAR(clear_module_state->__pyx_n_s_distribute);
   Py_CLEAR(clear_module_state->__pyx_n_s_distribute_by_substr);
@@ -2475,14 +2480,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_i);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_in_buf_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_n_s_j);
   Py_CLEAR(clear_module_state->__pyx_n_s_k);
+  Py_CLEAR(clear_module_state->__pyx_n_s_kw);
   Py_CLEAR(clear_module_state->__pyx_n_s_lead_n);
   Py_CLEAR(clear_module_state->__pyx_n_s_line);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_mrfifo_fast_loops);
   Py_CLEAR(clear_module_state->__pyx_kp_s_mrfifo_fast_loops_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_n);
   Py_CLEAR(clear_module_state->__pyx_n_s_n_ins);
@@ -2541,14 +2547,15 @@
   Py_VISIT(traverse_module_state->__pyx_kp_b_CB_Z);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s__2);
   Py_VISIT(traverse_module_state->__pyx_n_s__9);
   Py_VISIT(traverse_module_state->__pyx_kp_u_as_substring_in);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_buffer);
+  Py_VISIT(traverse_module_state->__pyx_n_s_buffer_size);
   Py_VISIT(traverse_module_state->__pyx_kp_u_can_not_find);
   Py_VISIT(traverse_module_state->__pyx_n_s_chunk_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_collect);
   Py_VISIT(traverse_module_state->__pyx_n_s_custom_header);
   Py_VISIT(traverse_module_state->__pyx_n_s_distribute);
   Py_VISIT(traverse_module_state->__pyx_n_s_distribute_by_substr);
@@ -2571,14 +2578,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_i);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_in_buf_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_n_s_j);
   Py_VISIT(traverse_module_state->__pyx_n_s_k);
+  Py_VISIT(traverse_module_state->__pyx_n_s_kw);
   Py_VISIT(traverse_module_state->__pyx_n_s_lead_n);
   Py_VISIT(traverse_module_state->__pyx_n_s_line);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_mrfifo_fast_loops);
   Py_VISIT(traverse_module_state->__pyx_kp_s_mrfifo_fast_loops_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_n);
   Py_VISIT(traverse_module_state->__pyx_n_s_n_ins);
@@ -2655,14 +2663,15 @@
 #define __pyx_kp_b_CB_Z __pyx_mstate_global->__pyx_kp_b_CB_Z
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s__2 __pyx_mstate_global->__pyx_n_s__2
 #define __pyx_n_s__9 __pyx_mstate_global->__pyx_n_s__9
 #define __pyx_kp_u_as_substring_in __pyx_mstate_global->__pyx_kp_u_as_substring_in
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_buffer __pyx_mstate_global->__pyx_n_s_buffer
+#define __pyx_n_s_buffer_size __pyx_mstate_global->__pyx_n_s_buffer_size
 #define __pyx_kp_u_can_not_find __pyx_mstate_global->__pyx_kp_u_can_not_find
 #define __pyx_n_s_chunk_size __pyx_mstate_global->__pyx_n_s_chunk_size
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_collect __pyx_mstate_global->__pyx_n_s_collect
 #define __pyx_n_s_custom_header __pyx_mstate_global->__pyx_n_s_custom_header
 #define __pyx_n_s_distribute __pyx_mstate_global->__pyx_n_s_distribute
 #define __pyx_n_s_distribute_by_substr __pyx_mstate_global->__pyx_n_s_distribute_by_substr
@@ -2685,14 +2694,15 @@
 #define __pyx_n_s_i __pyx_mstate_global->__pyx_n_s_i
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_in_buf_size __pyx_mstate_global->__pyx_n_s_in_buf_size
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_n_s_j __pyx_mstate_global->__pyx_n_s_j
 #define __pyx_n_s_k __pyx_mstate_global->__pyx_n_s_k
+#define __pyx_n_s_kw __pyx_mstate_global->__pyx_n_s_kw
 #define __pyx_n_s_lead_n __pyx_mstate_global->__pyx_n_s_lead_n
 #define __pyx_n_s_line __pyx_mstate_global->__pyx_n_s_line
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_mrfifo_fast_loops __pyx_mstate_global->__pyx_n_s_mrfifo_fast_loops
 #define __pyx_kp_s_mrfifo_fast_loops_pyx __pyx_mstate_global->__pyx_kp_s_mrfifo_fast_loops_pyx
 #define __pyx_n_s_n __pyx_mstate_global->__pyx_n_s_n
 #define __pyx_n_s_n_ins __pyx_mstate_global->__pyx_n_s_n_ins
@@ -2756,57 +2766,63 @@
   PyObject *__pyx_v_fifo_names = 0;
   int __pyx_v_chunk_size;
   size_t __pyx_v_in_buf_size;
   size_t __pyx_v_out_buf_size;
   PyObject *__pyx_v_header_detect_func = 0;
   PyObject *__pyx_v_header_fifo = 0;
   PyObject *__pyx_v_header_broadcast = 0;
+  size_t __pyx_v__buffer_size;
+  CYTHON_UNUSED PyObject *__pyx_v_kw = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[8] = {0,0,0,0,0,0,0,0};
+  PyObject* values[9] = {0,0,0,0,0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("distribute (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  __pyx_v_kw = PyDict_New(); if (unlikely(!__pyx_v_kw)) return NULL;
+  __Pyx_GOTREF(__pyx_v_kw);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fin_name,&__pyx_n_s_fifo_names,&__pyx_n_s_chunk_size,&__pyx_n_s_in_buf_size,&__pyx_n_s_out_buf_size,&__pyx_n_s_header_detect_func,&__pyx_n_s_header_fifo,&__pyx_n_s_header_broadcast,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fin_name,&__pyx_n_s_fifo_names,&__pyx_n_s_chunk_size,&__pyx_n_s_in_buf_size,&__pyx_n_s_out_buf_size,&__pyx_n_s_header_detect_func,&__pyx_n_s_header_fifo,&__pyx_n_s_header_broadcast,&__pyx_n_s_buffer_size,0};
 
     /* "mrfifo/fast_loops.pyx":12
  * def distribute(str fin_name, list fifo_names, int chunk_size=10000,
  *                size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  *                header_detect_func=None, header_fifo="",             # <<<<<<<<<<<<<<
- *                header_broadcast=False):
+ *                header_broadcast=False, size_t _buffer_size=0, **kw):
  * 
  */
     values[5] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
     values[6] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject*)__pyx_kp_u_)));
 
     /* "mrfifo/fast_loops.pyx":13
  *                size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  *                header_detect_func=None, header_fifo="",
- *                header_broadcast=False):             # <<<<<<<<<<<<<<
+ *                header_broadcast=False, size_t _buffer_size=0, **kw):             # <<<<<<<<<<<<<<
  * 
  *     if header_fifo == 0:
  */
     values[7] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_False)));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
+        case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
         case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
@@ -2835,15 +2851,15 @@
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fifo_names)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("distribute", 0, 2, 8, 1); __PYX_ERR(0, 10, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("distribute", 0, 2, 9, 1); __PYX_ERR(0, 10, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_chunk_size);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
@@ -2879,21 +2895,30 @@
         CYTHON_FALLTHROUGH;
         case  7:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_header_broadcast);
           if (value) { values[7] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
         }
+        CYTHON_FALLTHROUGH;
+        case  8:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_buffer_size);
+          if (value) { values[8] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
+        }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "distribute") < 0)) __PYX_ERR(0, 10, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kw, values + 0, kwd_pos_args, "distribute") < 0)) __PYX_ERR(0, 10, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
+        case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
         case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
@@ -2924,59 +2949,66 @@
       __pyx_v_out_buf_size = __Pyx_PyInt_As_size_t(values[4]); if (unlikely((__pyx_v_out_buf_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 11, __pyx_L3_error)
     } else {
       __pyx_v_out_buf_size = ((size_t)((size_t)0x80000));
     }
     __pyx_v_header_detect_func = values[5];
     __pyx_v_header_fifo = values[6];
     __pyx_v_header_broadcast = values[7];
+    if (values[8]) {
+      __pyx_v__buffer_size = __Pyx_PyInt_As_size_t(values[8]); if (unlikely((__pyx_v__buffer_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 13, __pyx_L3_error)
+    } else {
+      __pyx_v__buffer_size = ((size_t)((size_t)0));
+    }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("distribute", 0, 2, 8, __pyx_nargs); __PYX_ERR(0, 10, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("distribute", 0, 2, 9, __pyx_nargs); __PYX_ERR(0, 10, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
+  __Pyx_DECREF(__pyx_v_kw); __pyx_v_kw = 0;
   __Pyx_AddTraceback("mrfifo.fast_loops.distribute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fin_name), (&PyUnicode_Type), 1, "fin_name", 1))) __PYX_ERR(0, 10, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fifo_names), (&PyList_Type), 1, "fifo_names", 1))) __PYX_ERR(0, 10, __pyx_L1_error)
-  __pyx_r = __pyx_pf_6mrfifo_10fast_loops_distribute(__pyx_self, __pyx_v_fin_name, __pyx_v_fifo_names, __pyx_v_chunk_size, __pyx_v_in_buf_size, __pyx_v_out_buf_size, __pyx_v_header_detect_func, __pyx_v_header_fifo, __pyx_v_header_broadcast);
+  __pyx_r = __pyx_pf_6mrfifo_10fast_loops_distribute(__pyx_self, __pyx_v_fin_name, __pyx_v_fifo_names, __pyx_v_chunk_size, __pyx_v_in_buf_size, __pyx_v_out_buf_size, __pyx_v_header_detect_func, __pyx_v_header_fifo, __pyx_v_header_broadcast, __pyx_v__buffer_size, __pyx_v_kw);
 
   /* "mrfifo/fast_loops.pyx":10
  * from libc.string cimport strstr
  * 
  * def distribute(str fin_name, list fifo_names, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *                size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  *                header_detect_func=None, header_fifo="",
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_DECREF(__pyx_v_kw);
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6mrfifo_10fast_loops_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fin_name, PyObject *__pyx_v_fifo_names, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_detect_func, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_header_broadcast) {
+static PyObject *__pyx_pf_6mrfifo_10fast_loops_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fin_name, PyObject *__pyx_v_fifo_names, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_detect_func, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_header_broadcast, size_t __pyx_v__buffer_size, CYTHON_UNUSED PyObject *__pyx_v_kw) {
   size_t __pyx_v_i;
   size_t __pyx_v_j;
   size_t __pyx_v_n_outs;
   size_t __pyx_v_n;
   char *__pyx_v_buffer;
   Py_ssize_t __pyx_v_n_read;
   char *__pyx_v_fifo_buffers[0x80];
@@ -3001,15 +3033,15 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("distribute", 0);
   __Pyx_INCREF(__pyx_v_fifo_names);
   __Pyx_INCREF(__pyx_v_header_fifo);
 
   /* "mrfifo/fast_loops.pyx":15
- *                header_broadcast=False):
+ *                header_broadcast=False, size_t _buffer_size=0, **kw):
  * 
  *     if header_fifo == 0:             # <<<<<<<<<<<<<<
  *         # special mode: use the first fifo name for header data and the other
  *         # as round-robin outputs as usual
  */
   __pyx_t_1 = (__Pyx_PyInt_BoolEqObjC(__pyx_v_header_fifo, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 15, __pyx_L1_error)
   if (__pyx_t_1) {
@@ -3031,180 +3063,217 @@
     __pyx_t_2 = 0;
 
     /* "mrfifo/fast_loops.pyx":19
  *         # as round-robin outputs as usual
  *         header_fifo = fifo_names[0]
  *         fifo_names = fifo_names[1:]             # <<<<<<<<<<<<<<
  * 
- *     cdef size_t i = 0
+ *     if _buffer_size > 0:
  */
     if (unlikely(__pyx_v_fifo_names == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(0, 19, __pyx_L1_error)
     }
     __pyx_t_2 = __Pyx_PyList_GetSlice(__pyx_v_fifo_names, 1, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_fifo_names, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
     /* "mrfifo/fast_loops.pyx":15
- *                header_broadcast=False):
+ *                header_broadcast=False, size_t _buffer_size=0, **kw):
  * 
  *     if header_fifo == 0:             # <<<<<<<<<<<<<<
  *         # special mode: use the first fifo name for header data and the other
  *         # as round-robin outputs as usual
  */
   }
 
   /* "mrfifo/fast_loops.pyx":21
  *         fifo_names = fifo_names[1:]
  * 
+ *     if _buffer_size > 0:             # <<<<<<<<<<<<<<
+ *         in_buf_size = _buffer_size
+ *         out_buf_size = _buffer_size
+ */
+  __pyx_t_1 = (__pyx_v__buffer_size > 0);
+  if (__pyx_t_1) {
+
+    /* "mrfifo/fast_loops.pyx":22
+ * 
+ *     if _buffer_size > 0:
+ *         in_buf_size = _buffer_size             # <<<<<<<<<<<<<<
+ *         out_buf_size = _buffer_size
+ * 
+ */
+    __pyx_v_in_buf_size = __pyx_v__buffer_size;
+
+    /* "mrfifo/fast_loops.pyx":23
+ *     if _buffer_size > 0:
+ *         in_buf_size = _buffer_size
+ *         out_buf_size = _buffer_size             # <<<<<<<<<<<<<<
+ * 
+ *     cdef size_t i = 0
+ */
+    __pyx_v_out_buf_size = __pyx_v__buffer_size;
+
+    /* "mrfifo/fast_loops.pyx":21
+ *         fifo_names = fifo_names[1:]
+ * 
+ *     if _buffer_size > 0:             # <<<<<<<<<<<<<<
+ *         in_buf_size = _buffer_size
+ *         out_buf_size = _buffer_size
+ */
+  }
+
+  /* "mrfifo/fast_loops.pyx":25
+ *         out_buf_size = _buffer_size
+ * 
  *     cdef size_t i = 0             # <<<<<<<<<<<<<<
  *     cdef size_t j = 0
  *     cdef size_t n_outs = len(fifo_names)
  */
   __pyx_v_i = 0;
 
-  /* "mrfifo/fast_loops.pyx":22
+  /* "mrfifo/fast_loops.pyx":26
  * 
  *     cdef size_t i = 0
  *     cdef size_t j = 0             # <<<<<<<<<<<<<<
  *     cdef size_t n_outs = len(fifo_names)
  *     cdef size_t n = 0
  */
   __pyx_v_j = 0;
 
-  /* "mrfifo/fast_loops.pyx":23
+  /* "mrfifo/fast_loops.pyx":27
  *     cdef size_t i = 0
  *     cdef size_t j = 0
  *     cdef size_t n_outs = len(fifo_names)             # <<<<<<<<<<<<<<
  *     cdef size_t n = 0
  *     cdef str line
  */
   if (unlikely(__pyx_v_fifo_names == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 23, __pyx_L1_error)
+    __PYX_ERR(0, 27, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_fifo_names); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_fifo_names); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 27, __pyx_L1_error)
   __pyx_v_n_outs = __pyx_t_3;
 
-  /* "mrfifo/fast_loops.pyx":24
+  /* "mrfifo/fast_loops.pyx":28
  *     cdef size_t j = 0
  *     cdef size_t n_outs = len(fifo_names)
  *     cdef size_t n = 0             # <<<<<<<<<<<<<<
  *     cdef str line
  *     cdef char* buffer
  */
   __pyx_v_n = 0;
 
-  /* "mrfifo/fast_loops.pyx":27
+  /* "mrfifo/fast_loops.pyx":31
  *     cdef str line
  *     cdef char* buffer
  *     cdef ssize_t n_read = 0             # <<<<<<<<<<<<<<
  *     # support input distribution to up to 128 fifos in parallel
  *     cdef char* fifo_buffers[128]
  */
   __pyx_v_n_read = 0;
 
-  /* "mrfifo/fast_loops.pyx":30
+  /* "mrfifo/fast_loops.pyx":34
  *     # support input distribution to up to 128 fifos in parallel
  *     cdef char* fifo_buffers[128]
  *     buffer = <char*>stdlib.malloc(in_buf_size)             # <<<<<<<<<<<<<<
  * 
  *     assert n <= 128
  */
   __pyx_v_buffer = ((char *)malloc(__pyx_v_in_buf_size));
 
-  /* "mrfifo/fast_loops.pyx":32
+  /* "mrfifo/fast_loops.pyx":36
  *     buffer = <char*>stdlib.malloc(in_buf_size)
  * 
  *     assert n <= 128             # <<<<<<<<<<<<<<
  *     cdef stdio.FILE *fifos[128]
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = (__pyx_v_n <= 0x80);
     if (unlikely(!__pyx_t_1)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 32, __pyx_L1_error)
+      __PYX_ERR(0, 36, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 32, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 36, __pyx_L1_error)
   #endif
 
-  /* "mrfifo/fast_loops.pyx":35
+  /* "mrfifo/fast_loops.pyx":39
  *     cdef stdio.FILE *fifos[128]
  * 
  *     cdef char* stdin_buf = <char*>stdlib.malloc(in_buf_size)             # <<<<<<<<<<<<<<
  *     cdef stdio.FILE *fin = stdio.fopen(fin_name.encode('utf-8'), 'r')
  *     cdef stdio.FILE *fheader
  */
   __pyx_v_stdin_buf = ((char *)malloc(__pyx_v_in_buf_size));
 
-  /* "mrfifo/fast_loops.pyx":36
+  /* "mrfifo/fast_loops.pyx":40
  * 
  *     cdef char* stdin_buf = <char*>stdlib.malloc(in_buf_size)
  *     cdef stdio.FILE *fin = stdio.fopen(fin_name.encode('utf-8'), 'r')             # <<<<<<<<<<<<<<
  *     cdef stdio.FILE *fheader
  *     stdio.setvbuf(fin, stdin_buf, stdio._IOFBF, in_buf_size)
  */
   if (unlikely(__pyx_v_fin_name == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 36, __pyx_L1_error)
+    __PYX_ERR(0, 40, __pyx_L1_error)
   }
-  __pyx_t_2 = PyUnicode_AsUTF8String(__pyx_v_fin_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_2 = PyUnicode_AsUTF8String(__pyx_v_fin_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L1_error)
   __pyx_v_fin = fopen(__pyx_t_4, ((char const *)"r"));
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "mrfifo/fast_loops.pyx":38
+  /* "mrfifo/fast_loops.pyx":42
  *     cdef stdio.FILE *fin = stdio.fopen(fin_name.encode('utf-8'), 'r')
  *     cdef stdio.FILE *fheader
  *     stdio.setvbuf(fin, stdin_buf, stdio._IOFBF, in_buf_size)             # <<<<<<<<<<<<<<
  * 
  *     # set up output buffers for the main fifos
  */
   (void)(setvbuf(__pyx_v_fin, __pyx_v_stdin_buf, _IOFBF, __pyx_v_in_buf_size));
 
-  /* "mrfifo/fast_loops.pyx":41
+  /* "mrfifo/fast_loops.pyx":45
  * 
  *     # set up output buffers for the main fifos
  *     for i in range(n_outs):             # <<<<<<<<<<<<<<
  *         fifo_buffers[i] = <char*>stdlib.malloc(out_buf_size)
  *         fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'w')
  */
   __pyx_t_5 = __pyx_v_n_outs;
   __pyx_t_6 = __pyx_t_5;
   for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
     __pyx_v_i = __pyx_t_7;
 
-    /* "mrfifo/fast_loops.pyx":42
+    /* "mrfifo/fast_loops.pyx":46
  *     # set up output buffers for the main fifos
  *     for i in range(n_outs):
  *         fifo_buffers[i] = <char*>stdlib.malloc(out_buf_size)             # <<<<<<<<<<<<<<
  *         fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'w')
  *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, out_buf_size)
  */
     (__pyx_v_fifo_buffers[__pyx_v_i]) = ((char *)malloc(__pyx_v_out_buf_size));
 
-    /* "mrfifo/fast_loops.pyx":43
+    /* "mrfifo/fast_loops.pyx":47
  *     for i in range(n_outs):
  *         fifo_buffers[i] = <char*>stdlib.malloc(out_buf_size)
  *         fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'w')             # <<<<<<<<<<<<<<
  *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, out_buf_size)
  * 
  */
     if (unlikely(__pyx_v_fifo_names == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 43, __pyx_L1_error)
+      __PYX_ERR(0, 47, __pyx_L1_error)
     }
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_fifo_names, __pyx_v_i), __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 43, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_fifo_names, __pyx_v_i), __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = NULL;
     __pyx_t_10 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_9)) {
@@ -3216,60 +3285,60 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_kp_u_utf_8};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
-    __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L1_error)
     (__pyx_v_fifos[__pyx_v_i]) = fopen(__pyx_t_4, ((char const *)"w"));
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "mrfifo/fast_loops.pyx":44
+    /* "mrfifo/fast_loops.pyx":48
  *         fifo_buffers[i] = <char*>stdlib.malloc(out_buf_size)
  *         fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'w')
  *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, out_buf_size)             # <<<<<<<<<<<<<<
  * 
  *     if header_detect_func:
  */
     (void)(setvbuf((__pyx_v_fifos[__pyx_v_i]), (__pyx_v_fifo_buffers[__pyx_v_i]), _IOFBF, __pyx_v_out_buf_size));
   }
 
-  /* "mrfifo/fast_loops.pyx":46
+  /* "mrfifo/fast_loops.pyx":50
  *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, out_buf_size)
  * 
  *     if header_detect_func:             # <<<<<<<<<<<<<<
  *         # if the input stream contains some special header lines, allow to detect
  *         # these and write them to a separate header-fifo
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_detect_func); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_detect_func); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 50, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "mrfifo/fast_loops.pyx":49
+    /* "mrfifo/fast_loops.pyx":53
  *         # if the input stream contains some special header lines, allow to detect
  *         # these and write them to a separate header-fifo
  *         if header_fifo:             # <<<<<<<<<<<<<<
  *             fheader = stdio.fopen(header_fifo.encode('utf-8'), 'w')
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 49, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 53, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "mrfifo/fast_loops.pyx":50
+      /* "mrfifo/fast_loops.pyx":54
  *         # these and write them to a separate header-fifo
  *         if header_fifo:
  *             fheader = stdio.fopen(header_fifo.encode('utf-8'), 'w')             # <<<<<<<<<<<<<<
  * 
  *         while(True):
  */
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_header_fifo, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 50, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_header_fifo, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 54, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_9 = NULL;
       __pyx_t_10 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
         if (likely(__pyx_t_9)) {
@@ -3281,90 +3350,90 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_kp_u_utf_8};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
-      __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L1_error)
       __pyx_v_fheader = fopen(__pyx_t_4, ((char const *)"w"));
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "mrfifo/fast_loops.pyx":49
+      /* "mrfifo/fast_loops.pyx":53
  *         # if the input stream contains some special header lines, allow to detect
  *         # these and write them to a separate header-fifo
  *         if header_fifo:             # <<<<<<<<<<<<<<
  *             fheader = stdio.fopen(header_fifo.encode('utf-8'), 'w')
  * 
  */
     }
 
-    /* "mrfifo/fast_loops.pyx":52
+    /* "mrfifo/fast_loops.pyx":56
  *             fheader = stdio.fopen(header_fifo.encode('utf-8'), 'w')
  * 
  *         while(True):             # <<<<<<<<<<<<<<
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)
  *             if n_read <= 0:
  */
     while (1) {
 
-      /* "mrfifo/fast_loops.pyx":53
+      /* "mrfifo/fast_loops.pyx":57
  * 
  *         while(True):
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)             # <<<<<<<<<<<<<<
  *             if n_read <= 0:
  *                 break
  */
       __pyx_v_n_read = getline((&__pyx_v_buffer), (&__pyx_v_in_buf_size), __pyx_v_fin);
 
-      /* "mrfifo/fast_loops.pyx":54
+      /* "mrfifo/fast_loops.pyx":58
  *         while(True):
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)
  *             if n_read <= 0:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
       __pyx_t_1 = (__pyx_v_n_read <= 0);
       if (__pyx_t_1) {
 
-        /* "mrfifo/fast_loops.pyx":55
+        /* "mrfifo/fast_loops.pyx":59
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)
  *             if n_read <= 0:
  *                 break             # <<<<<<<<<<<<<<
  * 
  *             if header_detect_func(bytes(buffer).decode("ascii")):
  */
-        goto __pyx_L9_break;
+        goto __pyx_L10_break;
 
-        /* "mrfifo/fast_loops.pyx":54
+        /* "mrfifo/fast_loops.pyx":58
  *         while(True):
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)
  *             if n_read <= 0:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
       }
 
-      /* "mrfifo/fast_loops.pyx":57
+      /* "mrfifo/fast_loops.pyx":61
  *                 break
  * 
  *             if header_detect_func(bytes(buffer).decode("ascii")):             # <<<<<<<<<<<<<<
  *                 if header_fifo:
  *                     # print("writing to fifo header")
  */
-      __pyx_t_8 = __Pyx_PyBytes_FromString(__pyx_v_buffer); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 57, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyBytes_FromString(__pyx_v_buffer); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 61, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_9 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 57, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 61, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = __Pyx_decode_bytes(__pyx_t_9, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 57, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_decode_bytes(__pyx_t_9, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 61, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_INCREF(__pyx_v_header_detect_func);
       __pyx_t_9 = __pyx_v_header_detect_func; __pyx_t_11 = NULL;
       __pyx_t_10 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_9))) {
@@ -3379,322 +3448,322 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_11, __pyx_t_8};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
         __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 57, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 61, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_1) {
 
-        /* "mrfifo/fast_loops.pyx":58
+        /* "mrfifo/fast_loops.pyx":62
  * 
  *             if header_detect_func(bytes(buffer).decode("ascii")):
  *                 if header_fifo:             # <<<<<<<<<<<<<<
  *                     # print("writing to fifo header")
  *                     stdio.fwrite(buffer, n_read, 1, fheader)
  */
-        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 58, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 62, __pyx_L1_error)
         if (__pyx_t_1) {
 
-          /* "mrfifo/fast_loops.pyx":60
+          /* "mrfifo/fast_loops.pyx":64
  *                 if header_fifo:
  *                     # print("writing to fifo header")
  *                     stdio.fwrite(buffer, n_read, 1, fheader)             # <<<<<<<<<<<<<<
  *                 if header_broadcast:
  *                     for i in range(n_outs):
  */
           (void)(fwrite(__pyx_v_buffer, __pyx_v_n_read, 1, __pyx_v_fheader));
 
-          /* "mrfifo/fast_loops.pyx":58
+          /* "mrfifo/fast_loops.pyx":62
  * 
  *             if header_detect_func(bytes(buffer).decode("ascii")):
  *                 if header_fifo:             # <<<<<<<<<<<<<<
  *                     # print("writing to fifo header")
  *                     stdio.fwrite(buffer, n_read, 1, fheader)
  */
         }
 
-        /* "mrfifo/fast_loops.pyx":61
+        /* "mrfifo/fast_loops.pyx":65
  *                     # print("writing to fifo header")
  *                     stdio.fwrite(buffer, n_read, 1, fheader)
  *                 if header_broadcast:             # <<<<<<<<<<<<<<
  *                     for i in range(n_outs):
  *                         # print(f"writing header line to fifo {i} (n_read={n_read}) line={str(buffer)}")
  */
-        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_broadcast); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 61, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_broadcast); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 65, __pyx_L1_error)
         if (__pyx_t_1) {
 
-          /* "mrfifo/fast_loops.pyx":62
+          /* "mrfifo/fast_loops.pyx":66
  *                     stdio.fwrite(buffer, n_read, 1, fheader)
  *                 if header_broadcast:
  *                     for i in range(n_outs):             # <<<<<<<<<<<<<<
  *                         # print(f"writing header line to fifo {i} (n_read={n_read}) line={str(buffer)}")
  *                         stdio.fwrite(buffer, n_read, 1, fifos[i])
  */
           __pyx_t_5 = __pyx_v_n_outs;
           __pyx_t_6 = __pyx_t_5;
           for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
             __pyx_v_i = __pyx_t_7;
 
-            /* "mrfifo/fast_loops.pyx":64
+            /* "mrfifo/fast_loops.pyx":68
  *                     for i in range(n_outs):
  *                         # print(f"writing header line to fifo {i} (n_read={n_read}) line={str(buffer)}")
  *                         stdio.fwrite(buffer, n_read, 1, fifos[i])             # <<<<<<<<<<<<<<
  *             else:
  *                 # as soon as we see a non-header line, we break and enter the main loop
  */
             (void)(fwrite(__pyx_v_buffer, __pyx_v_n_read, 1, (__pyx_v_fifos[__pyx_v_i])));
           }
 
-          /* "mrfifo/fast_loops.pyx":61
+          /* "mrfifo/fast_loops.pyx":65
  *                     # print("writing to fifo header")
  *                     stdio.fwrite(buffer, n_read, 1, fheader)
  *                 if header_broadcast:             # <<<<<<<<<<<<<<
  *                     for i in range(n_outs):
  *                         # print(f"writing header line to fifo {i} (n_read={n_read}) line={str(buffer)}")
  */
         }
 
-        /* "mrfifo/fast_loops.pyx":57
+        /* "mrfifo/fast_loops.pyx":61
  *                 break
  * 
  *             if header_detect_func(bytes(buffer).decode("ascii")):             # <<<<<<<<<<<<<<
  *                 if header_fifo:
  *                     # print("writing to fifo header")
  */
-        goto __pyx_L11;
+        goto __pyx_L12;
       }
 
-      /* "mrfifo/fast_loops.pyx":67
+      /* "mrfifo/fast_loops.pyx":71
  *             else:
  *                 # as soon as we see a non-header line, we break and enter the main loop
  *                 break             # <<<<<<<<<<<<<<
  * 
  *         if header_fifo:
  */
       /*else*/ {
-        goto __pyx_L9_break;
+        goto __pyx_L10_break;
       }
-      __pyx_L11:;
+      __pyx_L12:;
     }
-    __pyx_L9_break:;
+    __pyx_L10_break:;
 
-    /* "mrfifo/fast_loops.pyx":69
+    /* "mrfifo/fast_loops.pyx":73
  *                 break
  * 
  *         if header_fifo:             # <<<<<<<<<<<<<<
  *             # close the header fifo
  *             stdio.fclose(fheader)
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 69, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 73, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "mrfifo/fast_loops.pyx":71
+      /* "mrfifo/fast_loops.pyx":75
  *         if header_fifo:
  *             # close the header fifo
  *             stdio.fclose(fheader)             # <<<<<<<<<<<<<<
  * 
  *     # main distribute loop
  */
       (void)(fclose(__pyx_v_fheader));
 
-      /* "mrfifo/fast_loops.pyx":69
+      /* "mrfifo/fast_loops.pyx":73
  *                 break
  * 
  *         if header_fifo:             # <<<<<<<<<<<<<<
  *             # close the header fifo
  *             stdio.fclose(fheader)
  */
     }
 
-    /* "mrfifo/fast_loops.pyx":46
+    /* "mrfifo/fast_loops.pyx":50
  *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, out_buf_size)
  * 
  *     if header_detect_func:             # <<<<<<<<<<<<<<
  *         # if the input stream contains some special header lines, allow to detect
  *         # these and write them to a separate header-fifo
  */
   }
 
-  /* "mrfifo/fast_loops.pyx":74
+  /* "mrfifo/fast_loops.pyx":78
  * 
  *     # main distribute loop
  *     while(True):             # <<<<<<<<<<<<<<
  *         if n_read == 0:
  *             # we may have already read a line in the header-detection above!
  */
   while (1) {
 
-    /* "mrfifo/fast_loops.pyx":75
+    /* "mrfifo/fast_loops.pyx":79
  *     # main distribute loop
  *     while(True):
  *         if n_read == 0:             # <<<<<<<<<<<<<<
  *             # we may have already read a line in the header-detection above!
  *             # read a new-line only if n_read has explicitly been zeroed again
  */
     __pyx_t_1 = (__pyx_v_n_read == 0);
     if (__pyx_t_1) {
 
-      /* "mrfifo/fast_loops.pyx":78
+      /* "mrfifo/fast_loops.pyx":82
  *             # we may have already read a line in the header-detection above!
  *             # read a new-line only if n_read has explicitly been zeroed again
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)             # <<<<<<<<<<<<<<
  * 
  *         if n_read <= 0:
  */
       __pyx_v_n_read = getline((&__pyx_v_buffer), (&__pyx_v_in_buf_size), __pyx_v_fin);
 
-      /* "mrfifo/fast_loops.pyx":75
+      /* "mrfifo/fast_loops.pyx":79
  *     # main distribute loop
  *     while(True):
  *         if n_read == 0:             # <<<<<<<<<<<<<<
  *             # we may have already read a line in the header-detection above!
  *             # read a new-line only if n_read has explicitly been zeroed again
  */
     }
 
-    /* "mrfifo/fast_loops.pyx":80
+    /* "mrfifo/fast_loops.pyx":84
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)
  * 
  *         if n_read <= 0:             # <<<<<<<<<<<<<<
  *             break
  * 
  */
     __pyx_t_1 = (__pyx_v_n_read <= 0);
     if (__pyx_t_1) {
 
-      /* "mrfifo/fast_loops.pyx":81
+      /* "mrfifo/fast_loops.pyx":85
  * 
  *         if n_read <= 0:
  *             break             # <<<<<<<<<<<<<<
  * 
  *         j = n // chunk_size
  */
-      goto __pyx_L18_break;
+      goto __pyx_L19_break;
 
-      /* "mrfifo/fast_loops.pyx":80
+      /* "mrfifo/fast_loops.pyx":84
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)
  * 
  *         if n_read <= 0:             # <<<<<<<<<<<<<<
  *             break
  * 
  */
     }
 
-    /* "mrfifo/fast_loops.pyx":83
+    /* "mrfifo/fast_loops.pyx":87
  *             break
  * 
  *         j = n // chunk_size             # <<<<<<<<<<<<<<
  *         stdio.fwrite(buffer, n_read, 1, fifos[j % n_outs])
  *         n += 1
  */
     __pyx_v_j = (__pyx_v_n / __pyx_v_chunk_size);
 
-    /* "mrfifo/fast_loops.pyx":84
+    /* "mrfifo/fast_loops.pyx":88
  * 
  *         j = n // chunk_size
  *         stdio.fwrite(buffer, n_read, 1, fifos[j % n_outs])             # <<<<<<<<<<<<<<
  *         n += 1
  *         n_read = 0
  */
     (void)(fwrite(__pyx_v_buffer, __pyx_v_n_read, 1, (__pyx_v_fifos[(__pyx_v_j % __pyx_v_n_outs)])));
 
-    /* "mrfifo/fast_loops.pyx":85
+    /* "mrfifo/fast_loops.pyx":89
  *         j = n // chunk_size
  *         stdio.fwrite(buffer, n_read, 1, fifos[j % n_outs])
  *         n += 1             # <<<<<<<<<<<<<<
  *         n_read = 0
  * 
  */
     __pyx_v_n = (__pyx_v_n + 1);
 
-    /* "mrfifo/fast_loops.pyx":86
+    /* "mrfifo/fast_loops.pyx":90
  *         stdio.fwrite(buffer, n_read, 1, fifos[j % n_outs])
  *         n += 1
  *         n_read = 0             # <<<<<<<<<<<<<<
  * 
  *     # close down all main fifos and free the output buffers
  */
     __pyx_v_n_read = 0;
   }
-  __pyx_L18_break:;
+  __pyx_L19_break:;
 
-  /* "mrfifo/fast_loops.pyx":89
+  /* "mrfifo/fast_loops.pyx":93
  * 
  *     # close down all main fifos and free the output buffers
  *     for i in range(n_outs):             # <<<<<<<<<<<<<<
  *         stdio.fclose(fifos[i])
  *         stdlib.free(fifo_buffers[i])
  */
   __pyx_t_5 = __pyx_v_n_outs;
   __pyx_t_6 = __pyx_t_5;
   for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
     __pyx_v_i = __pyx_t_7;
 
-    /* "mrfifo/fast_loops.pyx":90
+    /* "mrfifo/fast_loops.pyx":94
  *     # close down all main fifos and free the output buffers
  *     for i in range(n_outs):
  *         stdio.fclose(fifos[i])             # <<<<<<<<<<<<<<
  *         stdlib.free(fifo_buffers[i])
  * 
  */
     (void)(fclose((__pyx_v_fifos[__pyx_v_i])));
 
-    /* "mrfifo/fast_loops.pyx":91
+    /* "mrfifo/fast_loops.pyx":95
  *     for i in range(n_outs):
  *         stdio.fclose(fifos[i])
  *         stdlib.free(fifo_buffers[i])             # <<<<<<<<<<<<<<
  * 
  *     # close the input and free the input buffer, as well as the line buffer
  */
     free((__pyx_v_fifo_buffers[__pyx_v_i]));
   }
 
-  /* "mrfifo/fast_loops.pyx":94
+  /* "mrfifo/fast_loops.pyx":98
  * 
  *     # close the input and free the input buffer, as well as the line buffer
  *     stdio.fclose(fin)             # <<<<<<<<<<<<<<
  *     stdlib.free(stdin_buf)
  *     stdlib.free(buffer)
  */
   (void)(fclose(__pyx_v_fin));
 
-  /* "mrfifo/fast_loops.pyx":95
+  /* "mrfifo/fast_loops.pyx":99
  *     # close the input and free the input buffer, as well as the line buffer
  *     stdio.fclose(fin)
  *     stdlib.free(stdin_buf)             # <<<<<<<<<<<<<<
  *     stdlib.free(buffer)
  * 
  */
   free(__pyx_v_stdin_buf);
 
-  /* "mrfifo/fast_loops.pyx":96
+  /* "mrfifo/fast_loops.pyx":100
  *     stdio.fclose(fin)
  *     stdlib.free(stdin_buf)
  *     stdlib.free(buffer)             # <<<<<<<<<<<<<<
  * 
  *     return n # number of lines distributed (excluding header)
  */
   free(__pyx_v_buffer);
 
-  /* "mrfifo/fast_loops.pyx":98
+  /* "mrfifo/fast_loops.pyx":102
  *     stdlib.free(buffer)
  * 
  *     return n # number of lines distributed (excluding header)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "mrfifo/fast_loops.pyx":10
  * from libc.string cimport strstr
@@ -3716,15 +3785,15 @@
   __Pyx_XDECREF(__pyx_v_fifo_names);
   __Pyx_XDECREF(__pyx_v_header_fifo);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mrfifo/fast_loops.pyx":101
+/* "mrfifo/fast_loops.pyx":105
  * 
  * 
  * def distribute_by_substr(str fin_name, list fifo_names, dict sub_lookup,             # <<<<<<<<<<<<<<
  *                          size_t sub_size, bytes sub_lead=b"\tCB:Z:",
  *                          size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  */
 
@@ -3750,58 +3819,65 @@
   size_t __pyx_v_sub_size;
   PyObject *__pyx_v_sub_lead = 0;
   size_t __pyx_v_in_buf_size;
   size_t __pyx_v_out_buf_size;
   PyObject *__pyx_v_header_detect_func = 0;
   PyObject *__pyx_v_header_fifo = 0;
   PyObject *__pyx_v_header_broadcast = 0;
+  PyObject *__pyx_v__buffer_size = 0;
+  CYTHON_UNUSED PyObject *__pyx_v_kw = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[10] = {0,0,0,0,0,0,0,0,0,0};
+  PyObject* values[11] = {0,0,0,0,0,0,0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("distribute_by_substr (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  __pyx_v_kw = PyDict_New(); if (unlikely(!__pyx_v_kw)) return NULL;
+  __Pyx_GOTREF(__pyx_v_kw);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fin_name,&__pyx_n_s_fifo_names,&__pyx_n_s_sub_lookup,&__pyx_n_s_sub_size,&__pyx_n_s_sub_lead,&__pyx_n_s_in_buf_size,&__pyx_n_s_out_buf_size,&__pyx_n_s_header_detect_func,&__pyx_n_s_header_fifo,&__pyx_n_s_header_broadcast,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fin_name,&__pyx_n_s_fifo_names,&__pyx_n_s_sub_lookup,&__pyx_n_s_sub_size,&__pyx_n_s_sub_lead,&__pyx_n_s_in_buf_size,&__pyx_n_s_out_buf_size,&__pyx_n_s_header_detect_func,&__pyx_n_s_header_fifo,&__pyx_n_s_header_broadcast,&__pyx_n_s_buffer_size,0};
     values[4] = __Pyx_Arg_NewRef_FASTCALL(((PyObject*)((PyObject*)__pyx_kp_b_CB_Z)));
 
-    /* "mrfifo/fast_loops.pyx":104
+    /* "mrfifo/fast_loops.pyx":108
  *                          size_t sub_size, bytes sub_lead=b"\tCB:Z:",
  *                          size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  *                          header_detect_func=None, header_fifo="",             # <<<<<<<<<<<<<<
- *                          header_broadcast=False):
+ *                          header_broadcast=False, _buffer_size=0, **kw):
  * 
  */
     values[7] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
     values[8] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject*)__pyx_kp_u_)));
 
-    /* "mrfifo/fast_loops.pyx":105
+    /* "mrfifo/fast_loops.pyx":109
  *                          size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  *                          header_detect_func=None, header_fifo="",
- *                          header_broadcast=False):             # <<<<<<<<<<<<<<
+ *                          header_broadcast=False, _buffer_size=0, **kw):             # <<<<<<<<<<<<<<
  * 
  *     if header_fifo == 0:
  */
     values[9] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_False)));
+    values[10] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)__pyx_int_0)));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
+        case 11: values[10] = __Pyx_Arg_FASTCALL(__pyx_args, 10);
+        CYTHON_FALLTHROUGH;
         case 10: values[9] = __Pyx_Arg_FASTCALL(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
         case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
@@ -3824,95 +3900,104 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fin_name)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fifo_names)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("distribute_by_substr", 0, 4, 10, 1); __PYX_ERR(0, 101, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("distribute_by_substr", 0, 4, 11, 1); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sub_lookup)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("distribute_by_substr", 0, 4, 10, 2); __PYX_ERR(0, 101, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("distribute_by_substr", 0, 4, 11, 2); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sub_size)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("distribute_by_substr", 0, 4, 10, 3); __PYX_ERR(0, 101, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("distribute_by_substr", 0, 4, 11, 3); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sub_lead);
           if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_in_buf_size);
           if (value) { values[5] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_out_buf_size);
           if (value) { values[6] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_header_detect_func);
           if (value) { values[7] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_header_fifo);
           if (value) { values[8] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_header_broadcast);
           if (value) { values[9] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case 10:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_buffer_size);
+          if (value) { values[10] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "distribute_by_substr") < 0)) __PYX_ERR(0, 101, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kw, values + 0, kwd_pos_args, "distribute_by_substr") < 0)) __PYX_ERR(0, 105, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
+        case 11: values[10] = __Pyx_Arg_FASTCALL(__pyx_args, 10);
+        CYTHON_FALLTHROUGH;
         case 10: values[9] = __Pyx_Arg_FASTCALL(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
         case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
@@ -3928,76 +4013,79 @@
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_fin_name = ((PyObject*)values[0]);
     __pyx_v_fifo_names = ((PyObject*)values[1]);
     __pyx_v_sub_lookup = ((PyObject*)values[2]);
-    __pyx_v_sub_size = __Pyx_PyInt_As_size_t(values[3]); if (unlikely((__pyx_v_sub_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 102, __pyx_L3_error)
+    __pyx_v_sub_size = __Pyx_PyInt_As_size_t(values[3]); if (unlikely((__pyx_v_sub_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 106, __pyx_L3_error)
     __pyx_v_sub_lead = ((PyObject*)values[4]);
     if (values[5]) {
-      __pyx_v_in_buf_size = __Pyx_PyInt_As_size_t(values[5]); if (unlikely((__pyx_v_in_buf_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 103, __pyx_L3_error)
+      __pyx_v_in_buf_size = __Pyx_PyInt_As_size_t(values[5]); if (unlikely((__pyx_v_in_buf_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L3_error)
     } else {
       __pyx_v_in_buf_size = ((size_t)((size_t)0x100000));
     }
     if (values[6]) {
-      __pyx_v_out_buf_size = __Pyx_PyInt_As_size_t(values[6]); if (unlikely((__pyx_v_out_buf_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 103, __pyx_L3_error)
+      __pyx_v_out_buf_size = __Pyx_PyInt_As_size_t(values[6]); if (unlikely((__pyx_v_out_buf_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L3_error)
     } else {
       __pyx_v_out_buf_size = ((size_t)((size_t)0x80000));
     }
     __pyx_v_header_detect_func = values[7];
     __pyx_v_header_fifo = values[8];
     __pyx_v_header_broadcast = values[9];
+    __pyx_v__buffer_size = values[10];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("distribute_by_substr", 0, 4, 10, __pyx_nargs); __PYX_ERR(0, 101, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("distribute_by_substr", 0, 4, 11, __pyx_nargs); __PYX_ERR(0, 105, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
+  __Pyx_DECREF(__pyx_v_kw); __pyx_v_kw = 0;
   __Pyx_AddTraceback("mrfifo.fast_loops.distribute_by_substr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fin_name), (&PyUnicode_Type), 1, "fin_name", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fifo_names), (&PyList_Type), 1, "fifo_names", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sub_lookup), (&PyDict_Type), 1, "sub_lookup", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sub_lead), (&PyBytes_Type), 1, "sub_lead", 1))) __PYX_ERR(0, 102, __pyx_L1_error)
-  __pyx_r = __pyx_pf_6mrfifo_10fast_loops_2distribute_by_substr(__pyx_self, __pyx_v_fin_name, __pyx_v_fifo_names, __pyx_v_sub_lookup, __pyx_v_sub_size, __pyx_v_sub_lead, __pyx_v_in_buf_size, __pyx_v_out_buf_size, __pyx_v_header_detect_func, __pyx_v_header_fifo, __pyx_v_header_broadcast);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fin_name), (&PyUnicode_Type), 1, "fin_name", 1))) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fifo_names), (&PyList_Type), 1, "fifo_names", 1))) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sub_lookup), (&PyDict_Type), 1, "sub_lookup", 1))) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sub_lead), (&PyBytes_Type), 1, "sub_lead", 1))) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_r = __pyx_pf_6mrfifo_10fast_loops_2distribute_by_substr(__pyx_self, __pyx_v_fin_name, __pyx_v_fifo_names, __pyx_v_sub_lookup, __pyx_v_sub_size, __pyx_v_sub_lead, __pyx_v_in_buf_size, __pyx_v_out_buf_size, __pyx_v_header_detect_func, __pyx_v_header_fifo, __pyx_v_header_broadcast, __pyx_v__buffer_size, __pyx_v_kw);
 
-  /* "mrfifo/fast_loops.pyx":101
+  /* "mrfifo/fast_loops.pyx":105
  * 
  * 
  * def distribute_by_substr(str fin_name, list fifo_names, dict sub_lookup,             # <<<<<<<<<<<<<<
  *                          size_t sub_size, bytes sub_lead=b"\tCB:Z:",
  *                          size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_DECREF(__pyx_v_kw);
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6mrfifo_10fast_loops_2distribute_by_substr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fin_name, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_sub_lookup, size_t __pyx_v_sub_size, PyObject *__pyx_v_sub_lead, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_detect_func, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_header_broadcast) {
+static PyObject *__pyx_pf_6mrfifo_10fast_loops_2distribute_by_substr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fin_name, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_sub_lookup, size_t __pyx_v_sub_size, PyObject *__pyx_v_sub_lead, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_detect_func, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_header_broadcast, PyObject *__pyx_v__buffer_size, CYTHON_UNUSED PyObject *__pyx_v_kw) {
   size_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   size_t __pyx_v_n_outs;
   size_t __pyx_v_n;
   char *__pyx_v_buffer;
   char *__pyx_v_sub_lead_c;
   size_t __pyx_v_lead_n;
@@ -4010,18 +4098,18 @@
   char *__pyx_v_stdin_buf;
   FILE *__pyx_v_fin;
   FILE *__pyx_v_fheader;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  Py_ssize_t __pyx_t_3;
-  char *__pyx_t_4;
-  char const *__pyx_t_5;
-  size_t __pyx_t_6;
+  size_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  char *__pyx_t_5;
+  char const *__pyx_t_6;
   size_t __pyx_t_7;
   size_t __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
   Py_UCS4 __pyx_t_13;
@@ -4029,257 +4117,298 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("distribute_by_substr", 0);
   __Pyx_INCREF(__pyx_v_fifo_names);
   __Pyx_INCREF(__pyx_v_header_fifo);
 
-  /* "mrfifo/fast_loops.pyx":107
- *                          header_broadcast=False):
+  /* "mrfifo/fast_loops.pyx":111
+ *                          header_broadcast=False, _buffer_size=0, **kw):
  * 
  *     if header_fifo == 0:             # <<<<<<<<<<<<<<
  *         # special mode: use the first fifo name for header data and the other
  *         # as round-robin outputs as usual
  */
-  __pyx_t_1 = (__Pyx_PyInt_BoolEqObjC(__pyx_v_header_fifo, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyInt_BoolEqObjC(__pyx_v_header_fifo, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 111, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "mrfifo/fast_loops.pyx":110
+    /* "mrfifo/fast_loops.pyx":114
  *         # special mode: use the first fifo name for header data and the other
  *         # as round-robin outputs as usual
  *         header_fifo = fifo_names[0]             # <<<<<<<<<<<<<<
  *         fifo_names = fifo_names[1:]
  * 
  */
     if (unlikely(__pyx_v_fifo_names == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 110, __pyx_L1_error)
+      __PYX_ERR(0, 114, __pyx_L1_error)
     }
     __pyx_t_2 = PyList_GET_ITEM(__pyx_v_fifo_names, 0);
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_header_fifo, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "mrfifo/fast_loops.pyx":111
+    /* "mrfifo/fast_loops.pyx":115
  *         # as round-robin outputs as usual
  *         header_fifo = fifo_names[0]
  *         fifo_names = fifo_names[1:]             # <<<<<<<<<<<<<<
  * 
- *     cdef size_t i = 0
+ *     if _buffer_size > 0:
  */
     if (unlikely(__pyx_v_fifo_names == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 111, __pyx_L1_error)
+      __PYX_ERR(0, 115, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_PyList_GetSlice(__pyx_v_fifo_names, 1, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyList_GetSlice(__pyx_v_fifo_names, 1, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_fifo_names, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "mrfifo/fast_loops.pyx":107
- *                          header_broadcast=False):
+    /* "mrfifo/fast_loops.pyx":111
+ *                          header_broadcast=False, _buffer_size=0, **kw):
  * 
  *     if header_fifo == 0:             # <<<<<<<<<<<<<<
  *         # special mode: use the first fifo name for header data and the other
  *         # as round-robin outputs as usual
  */
   }
 
-  /* "mrfifo/fast_loops.pyx":113
+  /* "mrfifo/fast_loops.pyx":117
+ *         fifo_names = fifo_names[1:]
+ * 
+ *     if _buffer_size > 0:             # <<<<<<<<<<<<<<
+ *         in_buf_size = _buffer_size
+ *         out_buf_size = _buffer_size
+ */
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v__buffer_size, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 117, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__pyx_t_1) {
+
+    /* "mrfifo/fast_loops.pyx":118
+ * 
+ *     if _buffer_size > 0:
+ *         in_buf_size = _buffer_size             # <<<<<<<<<<<<<<
+ *         out_buf_size = _buffer_size
+ * 
+ */
+    __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_v__buffer_size); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 118, __pyx_L1_error)
+    __pyx_v_in_buf_size = __pyx_t_3;
+
+    /* "mrfifo/fast_loops.pyx":119
+ *     if _buffer_size > 0:
+ *         in_buf_size = _buffer_size
+ *         out_buf_size = _buffer_size             # <<<<<<<<<<<<<<
+ * 
+ *     cdef size_t i = 0
+ */
+    __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_v__buffer_size); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L1_error)
+    __pyx_v_out_buf_size = __pyx_t_3;
+
+    /* "mrfifo/fast_loops.pyx":117
  *         fifo_names = fifo_names[1:]
  * 
+ *     if _buffer_size > 0:             # <<<<<<<<<<<<<<
+ *         in_buf_size = _buffer_size
+ *         out_buf_size = _buffer_size
+ */
+  }
+
+  /* "mrfifo/fast_loops.pyx":121
+ *         out_buf_size = _buffer_size
+ * 
  *     cdef size_t i = 0             # <<<<<<<<<<<<<<
  *     cdef ssize_t j = 0
  * 
  */
   __pyx_v_i = 0;
 
-  /* "mrfifo/fast_loops.pyx":114
+  /* "mrfifo/fast_loops.pyx":122
  * 
  *     cdef size_t i = 0
  *     cdef ssize_t j = 0             # <<<<<<<<<<<<<<
  * 
  *     cdef size_t n_outs = len(fifo_names)
  */
   __pyx_v_j = 0;
 
-  /* "mrfifo/fast_loops.pyx":116
+  /* "mrfifo/fast_loops.pyx":124
  *     cdef ssize_t j = 0
  * 
  *     cdef size_t n_outs = len(fifo_names)             # <<<<<<<<<<<<<<
  *     cdef size_t n = 0
  *     cdef str line
  */
   if (unlikely(__pyx_v_fifo_names == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 116, __pyx_L1_error)
+    __PYX_ERR(0, 124, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_fifo_names); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 116, __pyx_L1_error)
-  __pyx_v_n_outs = __pyx_t_3;
+  __pyx_t_4 = __Pyx_PyList_GET_SIZE(__pyx_v_fifo_names); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_v_n_outs = __pyx_t_4;
 
-  /* "mrfifo/fast_loops.pyx":117
+  /* "mrfifo/fast_loops.pyx":125
  * 
  *     cdef size_t n_outs = len(fifo_names)
  *     cdef size_t n = 0             # <<<<<<<<<<<<<<
  *     cdef str line
  *     cdef char* buffer
  */
   __pyx_v_n = 0;
 
-  /* "mrfifo/fast_loops.pyx":120
+  /* "mrfifo/fast_loops.pyx":128
  *     cdef str line
  *     cdef char* buffer
  *     cdef char* sub_lead_c = sub_lead             # <<<<<<<<<<<<<<
  *     cdef size_t lead_n = len(sub_lead)
  *     cdef char* sub_buffer = <char*>stdlib.malloc(sub_size)
  */
   if (unlikely(__pyx_v_sub_lead == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 120, __pyx_L1_error)
+    __PYX_ERR(0, 128, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_PyBytes_AsWritableString(__pyx_v_sub_lead); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 120, __pyx_L1_error)
-  __pyx_v_sub_lead_c = __pyx_t_4;
+  __pyx_t_5 = __Pyx_PyBytes_AsWritableString(__pyx_v_sub_lead); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_v_sub_lead_c = __pyx_t_5;
 
-  /* "mrfifo/fast_loops.pyx":121
+  /* "mrfifo/fast_loops.pyx":129
  *     cdef char* buffer
  *     cdef char* sub_lead_c = sub_lead
  *     cdef size_t lead_n = len(sub_lead)             # <<<<<<<<<<<<<<
  *     cdef char* sub_buffer = <char*>stdlib.malloc(sub_size)
  *     cdef char* sub_match_c = NULL
  */
   if (unlikely(__pyx_v_sub_lead == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 121, __pyx_L1_error)
+    __PYX_ERR(0, 129, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_PyBytes_GET_SIZE(__pyx_v_sub_lead); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 121, __pyx_L1_error)
-  __pyx_v_lead_n = __pyx_t_3;
+  __pyx_t_4 = __Pyx_PyBytes_GET_SIZE(__pyx_v_sub_lead); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_v_lead_n = __pyx_t_4;
 
-  /* "mrfifo/fast_loops.pyx":122
+  /* "mrfifo/fast_loops.pyx":130
  *     cdef char* sub_lead_c = sub_lead
  *     cdef size_t lead_n = len(sub_lead)
  *     cdef char* sub_buffer = <char*>stdlib.malloc(sub_size)             # <<<<<<<<<<<<<<
  *     cdef char* sub_match_c = NULL
  *     cdef bytes sub
  */
   __pyx_v_sub_buffer = ((char *)malloc(__pyx_v_sub_size));
 
-  /* "mrfifo/fast_loops.pyx":123
+  /* "mrfifo/fast_loops.pyx":131
  *     cdef size_t lead_n = len(sub_lead)
  *     cdef char* sub_buffer = <char*>stdlib.malloc(sub_size)
  *     cdef char* sub_match_c = NULL             # <<<<<<<<<<<<<<
  *     cdef bytes sub
  *     cdef ssize_t n_read = 0
  */
   __pyx_v_sub_match_c = NULL;
 
-  /* "mrfifo/fast_loops.pyx":125
+  /* "mrfifo/fast_loops.pyx":133
  *     cdef char* sub_match_c = NULL
  *     cdef bytes sub
  *     cdef ssize_t n_read = 0             # <<<<<<<<<<<<<<
  *     # support input distribution to up to 128 fifos in parallel
  *     cdef char* fifo_buffers[128]
  */
   __pyx_v_n_read = 0;
 
-  /* "mrfifo/fast_loops.pyx":128
+  /* "mrfifo/fast_loops.pyx":136
  *     # support input distribution to up to 128 fifos in parallel
  *     cdef char* fifo_buffers[128]
  *     buffer = <char*>stdlib.malloc(in_buf_size)             # <<<<<<<<<<<<<<
  * 
  *     assert n <= 128
  */
   __pyx_v_buffer = ((char *)malloc(__pyx_v_in_buf_size));
 
-  /* "mrfifo/fast_loops.pyx":130
+  /* "mrfifo/fast_loops.pyx":138
  *     buffer = <char*>stdlib.malloc(in_buf_size)
  * 
  *     assert n <= 128             # <<<<<<<<<<<<<<
  *     cdef stdio.FILE *fifos[128]
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = (__pyx_v_n <= 0x80);
     if (unlikely(!__pyx_t_1)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 130, __pyx_L1_error)
+      __PYX_ERR(0, 138, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 130, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 138, __pyx_L1_error)
   #endif
 
-  /* "mrfifo/fast_loops.pyx":133
+  /* "mrfifo/fast_loops.pyx":141
  *     cdef stdio.FILE *fifos[128]
  * 
  *     cdef char* stdin_buf = <char*>stdlib.malloc(in_buf_size)             # <<<<<<<<<<<<<<
  *     cdef stdio.FILE *fin = stdio.fopen(fin_name.encode('utf-8'), 'r')
  *     cdef stdio.FILE *fheader
  */
   __pyx_v_stdin_buf = ((char *)malloc(__pyx_v_in_buf_size));
 
-  /* "mrfifo/fast_loops.pyx":134
+  /* "mrfifo/fast_loops.pyx":142
  * 
  *     cdef char* stdin_buf = <char*>stdlib.malloc(in_buf_size)
  *     cdef stdio.FILE *fin = stdio.fopen(fin_name.encode('utf-8'), 'r')             # <<<<<<<<<<<<<<
  *     cdef stdio.FILE *fheader
  *     stdio.setvbuf(fin, stdin_buf, stdio._IOFBF, in_buf_size)
  */
   if (unlikely(__pyx_v_fin_name == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 134, __pyx_L1_error)
+    __PYX_ERR(0, 142, __pyx_L1_error)
   }
-  __pyx_t_2 = PyUnicode_AsUTF8String(__pyx_v_fin_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_2 = PyUnicode_AsUTF8String(__pyx_v_fin_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L1_error)
-  __pyx_v_fin = fopen(__pyx_t_5, ((char const *)"r"));
+  __pyx_t_6 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_v_fin = fopen(__pyx_t_6, ((char const *)"r"));
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "mrfifo/fast_loops.pyx":136
+  /* "mrfifo/fast_loops.pyx":144
  *     cdef stdio.FILE *fin = stdio.fopen(fin_name.encode('utf-8'), 'r')
  *     cdef stdio.FILE *fheader
  *     stdio.setvbuf(fin, stdin_buf, stdio._IOFBF, in_buf_size)             # <<<<<<<<<<<<<<
  * 
  *     # set up output buffers for the main fifos
  */
   (void)(setvbuf(__pyx_v_fin, __pyx_v_stdin_buf, _IOFBF, __pyx_v_in_buf_size));
 
-  /* "mrfifo/fast_loops.pyx":139
+  /* "mrfifo/fast_loops.pyx":147
  * 
  *     # set up output buffers for the main fifos
  *     for i in range(n_outs):             # <<<<<<<<<<<<<<
  *         fifo_buffers[i] = <char*>stdlib.malloc(out_buf_size)
  *         fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'w')
  */
-  __pyx_t_6 = __pyx_v_n_outs;
-  __pyx_t_7 = __pyx_t_6;
+  __pyx_t_3 = __pyx_v_n_outs;
+  __pyx_t_7 = __pyx_t_3;
   for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
     __pyx_v_i = __pyx_t_8;
 
-    /* "mrfifo/fast_loops.pyx":140
+    /* "mrfifo/fast_loops.pyx":148
  *     # set up output buffers for the main fifos
  *     for i in range(n_outs):
  *         fifo_buffers[i] = <char*>stdlib.malloc(out_buf_size)             # <<<<<<<<<<<<<<
  *         fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'w')
  *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, out_buf_size)
  */
     (__pyx_v_fifo_buffers[__pyx_v_i]) = ((char *)malloc(__pyx_v_out_buf_size));
 
-    /* "mrfifo/fast_loops.pyx":141
+    /* "mrfifo/fast_loops.pyx":149
  *     for i in range(n_outs):
  *         fifo_buffers[i] = <char*>stdlib.malloc(out_buf_size)
  *         fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'w')             # <<<<<<<<<<<<<<
  *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, out_buf_size)
  * 
  */
     if (unlikely(__pyx_v_fifo_names == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 141, __pyx_L1_error)
+      __PYX_ERR(0, 149, __pyx_L1_error)
     }
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_fifo_names, __pyx_v_i), __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 141, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_fifo_names, __pyx_v_i), __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_10 = NULL;
     __pyx_t_11 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_10)) {
@@ -4291,60 +4420,60 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_kp_u_utf_8};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 141, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
-    __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 141, __pyx_L1_error)
-    (__pyx_v_fifos[__pyx_v_i]) = fopen(__pyx_t_5, ((char const *)"w"));
+    __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 149, __pyx_L1_error)
+    (__pyx_v_fifos[__pyx_v_i]) = fopen(__pyx_t_6, ((char const *)"w"));
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "mrfifo/fast_loops.pyx":142
+    /* "mrfifo/fast_loops.pyx":150
  *         fifo_buffers[i] = <char*>stdlib.malloc(out_buf_size)
  *         fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'w')
  *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, out_buf_size)             # <<<<<<<<<<<<<<
  * 
  *     if header_detect_func:
  */
     (void)(setvbuf((__pyx_v_fifos[__pyx_v_i]), (__pyx_v_fifo_buffers[__pyx_v_i]), _IOFBF, __pyx_v_out_buf_size));
   }
 
-  /* "mrfifo/fast_loops.pyx":144
+  /* "mrfifo/fast_loops.pyx":152
  *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, out_buf_size)
  * 
  *     if header_detect_func:             # <<<<<<<<<<<<<<
  *         # if the input stream contains some special header lines, allow to detect these and write them to a separate header-fifo
  *         if header_fifo:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_detect_func); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_detect_func); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 152, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "mrfifo/fast_loops.pyx":146
+    /* "mrfifo/fast_loops.pyx":154
  *     if header_detect_func:
  *         # if the input stream contains some special header lines, allow to detect these and write them to a separate header-fifo
  *         if header_fifo:             # <<<<<<<<<<<<<<
  *             fheader = stdio.fopen(header_fifo.encode('utf-8'), 'w')
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 154, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "mrfifo/fast_loops.pyx":147
+      /* "mrfifo/fast_loops.pyx":155
  *         # if the input stream contains some special header lines, allow to detect these and write them to a separate header-fifo
  *         if header_fifo:
  *             fheader = stdio.fopen(header_fifo.encode('utf-8'), 'w')             # <<<<<<<<<<<<<<
  * 
  *         while(True):
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_header_fifo, __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 147, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_header_fifo, __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 155, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_10 = NULL;
       __pyx_t_11 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_10)) {
@@ -4356,90 +4485,90 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_kp_u_utf_8};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 147, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
-      __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 147, __pyx_L1_error)
-      __pyx_v_fheader = fopen(__pyx_t_5, ((char const *)"w"));
+      __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 155, __pyx_L1_error)
+      __pyx_v_fheader = fopen(__pyx_t_6, ((char const *)"w"));
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "mrfifo/fast_loops.pyx":146
+      /* "mrfifo/fast_loops.pyx":154
  *     if header_detect_func:
  *         # if the input stream contains some special header lines, allow to detect these and write them to a separate header-fifo
  *         if header_fifo:             # <<<<<<<<<<<<<<
  *             fheader = stdio.fopen(header_fifo.encode('utf-8'), 'w')
  * 
  */
     }
 
-    /* "mrfifo/fast_loops.pyx":149
+    /* "mrfifo/fast_loops.pyx":157
  *             fheader = stdio.fopen(header_fifo.encode('utf-8'), 'w')
  * 
  *         while(True):             # <<<<<<<<<<<<<<
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)
  *             if n_read <= 0:
  */
     while (1) {
 
-      /* "mrfifo/fast_loops.pyx":150
+      /* "mrfifo/fast_loops.pyx":158
  * 
  *         while(True):
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)             # <<<<<<<<<<<<<<
  *             if n_read <= 0:
  *                 break
  */
       __pyx_v_n_read = getline((&__pyx_v_buffer), (&__pyx_v_in_buf_size), __pyx_v_fin);
 
-      /* "mrfifo/fast_loops.pyx":151
+      /* "mrfifo/fast_loops.pyx":159
  *         while(True):
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)
  *             if n_read <= 0:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
       __pyx_t_1 = (__pyx_v_n_read <= 0);
       if (__pyx_t_1) {
 
-        /* "mrfifo/fast_loops.pyx":152
+        /* "mrfifo/fast_loops.pyx":160
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)
  *             if n_read <= 0:
  *                 break             # <<<<<<<<<<<<<<
  * 
  *             if header_detect_func(bytes(buffer).decode("ascii")):
  */
-        goto __pyx_L9_break;
+        goto __pyx_L10_break;
 
-        /* "mrfifo/fast_loops.pyx":151
+        /* "mrfifo/fast_loops.pyx":159
  *         while(True):
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)
  *             if n_read <= 0:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
       }
 
-      /* "mrfifo/fast_loops.pyx":154
+      /* "mrfifo/fast_loops.pyx":162
  *                 break
  * 
  *             if header_detect_func(bytes(buffer).decode("ascii")):             # <<<<<<<<<<<<<<
  *                 if header_fifo:
  *                     stdio.fwrite(buffer, n_read, 1, fheader)
  */
-      __pyx_t_9 = __Pyx_PyBytes_FromString(__pyx_v_buffer); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 154, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyBytes_FromString(__pyx_v_buffer); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 154, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __pyx_t_9 = __Pyx_decode_bytes(__pyx_t_10, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 154, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_decode_bytes(__pyx_t_10, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_INCREF(__pyx_v_header_detect_func);
       __pyx_t_10 = __pyx_v_header_detect_func; __pyx_t_12 = NULL;
       __pyx_t_11 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_10))) {
@@ -4454,441 +4583,441 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_9};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 154, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_1) {
 
-        /* "mrfifo/fast_loops.pyx":155
+        /* "mrfifo/fast_loops.pyx":163
  * 
  *             if header_detect_func(bytes(buffer).decode("ascii")):
  *                 if header_fifo:             # <<<<<<<<<<<<<<
  *                     stdio.fwrite(buffer, n_read, 1, fheader)
  *                 if header_broadcast:
  */
-        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 155, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 163, __pyx_L1_error)
         if (__pyx_t_1) {
 
-          /* "mrfifo/fast_loops.pyx":156
+          /* "mrfifo/fast_loops.pyx":164
  *             if header_detect_func(bytes(buffer).decode("ascii")):
  *                 if header_fifo:
  *                     stdio.fwrite(buffer, n_read, 1, fheader)             # <<<<<<<<<<<<<<
  *                 if header_broadcast:
  *                     for i in range(n_outs):
  */
           (void)(fwrite(__pyx_v_buffer, __pyx_v_n_read, 1, __pyx_v_fheader));
 
-          /* "mrfifo/fast_loops.pyx":155
+          /* "mrfifo/fast_loops.pyx":163
  * 
  *             if header_detect_func(bytes(buffer).decode("ascii")):
  *                 if header_fifo:             # <<<<<<<<<<<<<<
  *                     stdio.fwrite(buffer, n_read, 1, fheader)
  *                 if header_broadcast:
  */
         }
 
-        /* "mrfifo/fast_loops.pyx":157
+        /* "mrfifo/fast_loops.pyx":165
  *                 if header_fifo:
  *                     stdio.fwrite(buffer, n_read, 1, fheader)
  *                 if header_broadcast:             # <<<<<<<<<<<<<<
  *                     for i in range(n_outs):
  *                         # print(f"writing header line to fifo {i} (n_read={n_read}) line={str(buffer)}")
  */
-        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_broadcast); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 157, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_broadcast); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 165, __pyx_L1_error)
         if (__pyx_t_1) {
 
-          /* "mrfifo/fast_loops.pyx":158
+          /* "mrfifo/fast_loops.pyx":166
  *                     stdio.fwrite(buffer, n_read, 1, fheader)
  *                 if header_broadcast:
  *                     for i in range(n_outs):             # <<<<<<<<<<<<<<
  *                         # print(f"writing header line to fifo {i} (n_read={n_read}) line={str(buffer)}")
  *                         stdio.fwrite(buffer, n_read, 1, fifos[i])
  */
-          __pyx_t_6 = __pyx_v_n_outs;
-          __pyx_t_7 = __pyx_t_6;
+          __pyx_t_3 = __pyx_v_n_outs;
+          __pyx_t_7 = __pyx_t_3;
           for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
             __pyx_v_i = __pyx_t_8;
 
-            /* "mrfifo/fast_loops.pyx":160
+            /* "mrfifo/fast_loops.pyx":168
  *                     for i in range(n_outs):
  *                         # print(f"writing header line to fifo {i} (n_read={n_read}) line={str(buffer)}")
  *                         stdio.fwrite(buffer, n_read, 1, fifos[i])             # <<<<<<<<<<<<<<
  *             else:
  *                 # as soon as we see a non-header line, we break and enter the main loop
  */
             (void)(fwrite(__pyx_v_buffer, __pyx_v_n_read, 1, (__pyx_v_fifos[__pyx_v_i])));
           }
 
-          /* "mrfifo/fast_loops.pyx":157
+          /* "mrfifo/fast_loops.pyx":165
  *                 if header_fifo:
  *                     stdio.fwrite(buffer, n_read, 1, fheader)
  *                 if header_broadcast:             # <<<<<<<<<<<<<<
  *                     for i in range(n_outs):
  *                         # print(f"writing header line to fifo {i} (n_read={n_read}) line={str(buffer)}")
  */
         }
 
-        /* "mrfifo/fast_loops.pyx":154
+        /* "mrfifo/fast_loops.pyx":162
  *                 break
  * 
  *             if header_detect_func(bytes(buffer).decode("ascii")):             # <<<<<<<<<<<<<<
  *                 if header_fifo:
  *                     stdio.fwrite(buffer, n_read, 1, fheader)
  */
-        goto __pyx_L11;
+        goto __pyx_L12;
       }
 
-      /* "mrfifo/fast_loops.pyx":163
+      /* "mrfifo/fast_loops.pyx":171
  *             else:
  *                 # as soon as we see a non-header line, we break and enter the main loop
  *                 break             # <<<<<<<<<<<<<<
  * 
  *         if header_fifo:
  */
       /*else*/ {
-        goto __pyx_L9_break;
+        goto __pyx_L10_break;
       }
-      __pyx_L11:;
+      __pyx_L12:;
     }
-    __pyx_L9_break:;
+    __pyx_L10_break:;
 
-    /* "mrfifo/fast_loops.pyx":165
+    /* "mrfifo/fast_loops.pyx":173
  *                 break
  * 
  *         if header_fifo:             # <<<<<<<<<<<<<<
  *             # close the header fifo
  *             stdio.fclose(fheader)
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 173, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "mrfifo/fast_loops.pyx":167
+      /* "mrfifo/fast_loops.pyx":175
  *         if header_fifo:
  *             # close the header fifo
  *             stdio.fclose(fheader)             # <<<<<<<<<<<<<<
  * 
  *     # main distribute loop
  */
       (void)(fclose(__pyx_v_fheader));
 
-      /* "mrfifo/fast_loops.pyx":165
+      /* "mrfifo/fast_loops.pyx":173
  *                 break
  * 
  *         if header_fifo:             # <<<<<<<<<<<<<<
  *             # close the header fifo
  *             stdio.fclose(fheader)
  */
     }
 
-    /* "mrfifo/fast_loops.pyx":144
+    /* "mrfifo/fast_loops.pyx":152
  *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, out_buf_size)
  * 
  *     if header_detect_func:             # <<<<<<<<<<<<<<
  *         # if the input stream contains some special header lines, allow to detect these and write them to a separate header-fifo
  *         if header_fifo:
  */
   }
 
-  /* "mrfifo/fast_loops.pyx":170
+  /* "mrfifo/fast_loops.pyx":178
  * 
  *     # main distribute loop
  *     while(True):             # <<<<<<<<<<<<<<
  *         if n_read == 0:
  *             # we may have already read a line in the header-detection above!
  */
   while (1) {
 
-    /* "mrfifo/fast_loops.pyx":171
+    /* "mrfifo/fast_loops.pyx":179
  *     # main distribute loop
  *     while(True):
  *         if n_read == 0:             # <<<<<<<<<<<<<<
  *             # we may have already read a line in the header-detection above!
  *             # read a new-line only if n_read has explicitly been zeroed again
  */
     __pyx_t_1 = (__pyx_v_n_read == 0);
     if (__pyx_t_1) {
 
-      /* "mrfifo/fast_loops.pyx":174
+      /* "mrfifo/fast_loops.pyx":182
  *             # we may have already read a line in the header-detection above!
  *             # read a new-line only if n_read has explicitly been zeroed again
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)             # <<<<<<<<<<<<<<
  * 
  *         if n_read <= 0:
  */
       __pyx_v_n_read = getline((&__pyx_v_buffer), (&__pyx_v_in_buf_size), __pyx_v_fin);
 
-      /* "mrfifo/fast_loops.pyx":171
+      /* "mrfifo/fast_loops.pyx":179
  *     # main distribute loop
  *     while(True):
  *         if n_read == 0:             # <<<<<<<<<<<<<<
  *             # we may have already read a line in the header-detection above!
  *             # read a new-line only if n_read has explicitly been zeroed again
  */
     }
 
-    /* "mrfifo/fast_loops.pyx":176
+    /* "mrfifo/fast_loops.pyx":184
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)
  * 
  *         if n_read <= 0:             # <<<<<<<<<<<<<<
  *             break
  * 
  */
     __pyx_t_1 = (__pyx_v_n_read <= 0);
     if (__pyx_t_1) {
 
-      /* "mrfifo/fast_loops.pyx":177
+      /* "mrfifo/fast_loops.pyx":185
  * 
  *         if n_read <= 0:
  *             break             # <<<<<<<<<<<<<<
  * 
  *         # extract the \tCB:Z:<cell barcode> value.
  */
-      goto __pyx_L18_break;
+      goto __pyx_L19_break;
 
-      /* "mrfifo/fast_loops.pyx":176
+      /* "mrfifo/fast_loops.pyx":184
  *             n_read = stdio.getline(&buffer, &in_buf_size, fin)
  * 
  *         if n_read <= 0:             # <<<<<<<<<<<<<<
  *             break
  * 
  */
     }
 
-    /* "mrfifo/fast_loops.pyx":183
+    /* "mrfifo/fast_loops.pyx":191
  *         # and extract sub_n characters downstream of that
  * 
  *         sub_match_c = strstr(buffer, sub_lead_c)             # <<<<<<<<<<<<<<
  *         if sub_match_c is NULL:
  *             raise ValueError(f"can not find {sub_lead} as substring in {str(buffer)}")
  */
     __pyx_v_sub_match_c = strstr(__pyx_v_buffer, __pyx_v_sub_lead_c);
 
-    /* "mrfifo/fast_loops.pyx":184
+    /* "mrfifo/fast_loops.pyx":192
  * 
  *         sub_match_c = strstr(buffer, sub_lead_c)
  *         if sub_match_c is NULL:             # <<<<<<<<<<<<<<
  *             raise ValueError(f"can not find {sub_lead} as substring in {str(buffer)}")
  * 
  */
     __pyx_t_1 = (__pyx_v_sub_match_c == NULL);
     if (unlikely(__pyx_t_1)) {
 
-      /* "mrfifo/fast_loops.pyx":185
+      /* "mrfifo/fast_loops.pyx":193
  *         sub_match_c = strstr(buffer, sub_lead_c)
  *         if sub_match_c is NULL:
  *             raise ValueError(f"can not find {sub_lead} as substring in {str(buffer)}")             # <<<<<<<<<<<<<<
  * 
  *         sub = (sub_match_c + lead_n)[:sub_size]
  */
-      __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = 0;
+      __pyx_t_4 = 0;
       __pyx_t_13 = 127;
       __Pyx_INCREF(__pyx_kp_u_can_not_find);
-      __pyx_t_3 += 13;
+      __pyx_t_4 += 13;
       __Pyx_GIVEREF(__pyx_kp_u_can_not_find);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u_can_not_find);
-      __pyx_t_10 = __Pyx_PyObject_FormatSimple(__pyx_v_sub_lead, __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 185, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_FormatSimple(__pyx_v_sub_lead, __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 193, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_13 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) > __pyx_t_13) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) : __pyx_t_13;
-      __pyx_t_3 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_10);
+      __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_10);
       __Pyx_GIVEREF(__pyx_t_10);
       PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_10);
       __pyx_t_10 = 0;
       __Pyx_INCREF(__pyx_kp_u_as_substring_in);
-      __pyx_t_3 += 17;
+      __pyx_t_4 += 17;
       __Pyx_GIVEREF(__pyx_kp_u_as_substring_in);
       PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u_as_substring_in);
-      __pyx_t_10 = __Pyx_PyBytes_FromString(__pyx_v_buffer); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 185, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyBytes_FromString(__pyx_v_buffer); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 193, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_9 = __Pyx_PyObject_Str(__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 185, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_Str(__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 193, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_13 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) > __pyx_t_13) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) : __pyx_t_13;
-      __pyx_t_3 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_9);
+      __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_9);
       __Pyx_GIVEREF(__pyx_t_9);
       PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_9);
       __pyx_t_9 = 0;
-      __pyx_t_9 = __Pyx_PyUnicode_Join(__pyx_t_2, 4, __pyx_t_3, __pyx_t_13); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 185, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyUnicode_Join(__pyx_t_2, 4, __pyx_t_4, __pyx_t_13); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 193, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 185, __pyx_L1_error)
+      __PYX_ERR(0, 193, __pyx_L1_error)
 
-      /* "mrfifo/fast_loops.pyx":184
+      /* "mrfifo/fast_loops.pyx":192
  * 
  *         sub_match_c = strstr(buffer, sub_lead_c)
  *         if sub_match_c is NULL:             # <<<<<<<<<<<<<<
  *             raise ValueError(f"can not find {sub_lead} as substring in {str(buffer)}")
  * 
  */
     }
 
-    /* "mrfifo/fast_loops.pyx":187
+    /* "mrfifo/fast_loops.pyx":195
  *             raise ValueError(f"can not find {sub_lead} as substring in {str(buffer)}")
  * 
  *         sub = (sub_match_c + lead_n)[:sub_size]             # <<<<<<<<<<<<<<
  *         # print(f"found sub {sub}")
  * 
  */
-    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize((__pyx_v_sub_match_c + __pyx_v_lead_n) + 0, __pyx_v_sub_size - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize((__pyx_v_sub_match_c + __pyx_v_lead_n) + 0, __pyx_v_sub_size - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_sub, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "mrfifo/fast_loops.pyx":190
+    /* "mrfifo/fast_loops.pyx":198
  *         # print(f"found sub {sub}")
  * 
  *         j = sub_lookup.get(sub, -1)             # <<<<<<<<<<<<<<
  *         if j >= 0:
  *             stdio.fwrite(buffer, n_read, 1, fifos[j % n_outs])
  */
     if (unlikely(__pyx_v_sub_lookup == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "get");
-      __PYX_ERR(0, 190, __pyx_L1_error)
+      __PYX_ERR(0, 198, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_PyDict_GetItemDefault(__pyx_v_sub_lookup, __pyx_v_sub, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_GetItemDefault(__pyx_v_sub_lookup, __pyx_v_sub, __pyx_int_neg_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_14 = PyInt_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_14 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_14 = PyInt_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_14 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 198, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_j = __pyx_t_14;
 
-    /* "mrfifo/fast_loops.pyx":191
+    /* "mrfifo/fast_loops.pyx":199
  * 
  *         j = sub_lookup.get(sub, -1)
  *         if j >= 0:             # <<<<<<<<<<<<<<
  *             stdio.fwrite(buffer, n_read, 1, fifos[j % n_outs])
  * 
  */
     __pyx_t_1 = (__pyx_v_j >= 0);
     if (__pyx_t_1) {
 
-      /* "mrfifo/fast_loops.pyx":192
+      /* "mrfifo/fast_loops.pyx":200
  *         j = sub_lookup.get(sub, -1)
  *         if j >= 0:
  *             stdio.fwrite(buffer, n_read, 1, fifos[j % n_outs])             # <<<<<<<<<<<<<<
  * 
  *         n += 1
  */
       (void)(fwrite(__pyx_v_buffer, __pyx_v_n_read, 1, (__pyx_v_fifos[(__pyx_v_j % __pyx_v_n_outs)])));
 
-      /* "mrfifo/fast_loops.pyx":191
+      /* "mrfifo/fast_loops.pyx":199
  * 
  *         j = sub_lookup.get(sub, -1)
  *         if j >= 0:             # <<<<<<<<<<<<<<
  *             stdio.fwrite(buffer, n_read, 1, fifos[j % n_outs])
  * 
  */
     }
 
-    /* "mrfifo/fast_loops.pyx":194
+    /* "mrfifo/fast_loops.pyx":202
  *             stdio.fwrite(buffer, n_read, 1, fifos[j % n_outs])
  * 
  *         n += 1             # <<<<<<<<<<<<<<
  *         n_read = 0
  * 
  */
     __pyx_v_n = (__pyx_v_n + 1);
 
-    /* "mrfifo/fast_loops.pyx":195
+    /* "mrfifo/fast_loops.pyx":203
  * 
  *         n += 1
  *         n_read = 0             # <<<<<<<<<<<<<<
  * 
  *     # close down all main fifos and free the output buffers
  */
     __pyx_v_n_read = 0;
   }
-  __pyx_L18_break:;
+  __pyx_L19_break:;
 
-  /* "mrfifo/fast_loops.pyx":198
+  /* "mrfifo/fast_loops.pyx":206
  * 
  *     # close down all main fifos and free the output buffers
  *     for i in range(n_outs):             # <<<<<<<<<<<<<<
  *         stdio.fclose(fifos[i])
  *         stdlib.free(fifo_buffers[i])
  */
-  __pyx_t_6 = __pyx_v_n_outs;
-  __pyx_t_7 = __pyx_t_6;
+  __pyx_t_3 = __pyx_v_n_outs;
+  __pyx_t_7 = __pyx_t_3;
   for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
     __pyx_v_i = __pyx_t_8;
 
-    /* "mrfifo/fast_loops.pyx":199
+    /* "mrfifo/fast_loops.pyx":207
  *     # close down all main fifos and free the output buffers
  *     for i in range(n_outs):
  *         stdio.fclose(fifos[i])             # <<<<<<<<<<<<<<
  *         stdlib.free(fifo_buffers[i])
  * 
  */
     (void)(fclose((__pyx_v_fifos[__pyx_v_i])));
 
-    /* "mrfifo/fast_loops.pyx":200
+    /* "mrfifo/fast_loops.pyx":208
  *     for i in range(n_outs):
  *         stdio.fclose(fifos[i])
  *         stdlib.free(fifo_buffers[i])             # <<<<<<<<<<<<<<
  * 
  *     # close the input and free the input buffer, as well as the line buffer
  */
     free((__pyx_v_fifo_buffers[__pyx_v_i]));
   }
 
-  /* "mrfifo/fast_loops.pyx":203
+  /* "mrfifo/fast_loops.pyx":211
  * 
  *     # close the input and free the input buffer, as well as the line buffer
  *     stdio.fclose(fin)             # <<<<<<<<<<<<<<
  *     stdlib.free(stdin_buf)
  *     stdlib.free(buffer)
  */
   (void)(fclose(__pyx_v_fin));
 
-  /* "mrfifo/fast_loops.pyx":204
+  /* "mrfifo/fast_loops.pyx":212
  *     # close the input and free the input buffer, as well as the line buffer
  *     stdio.fclose(fin)
  *     stdlib.free(stdin_buf)             # <<<<<<<<<<<<<<
  *     stdlib.free(buffer)
  * 
  */
   free(__pyx_v_stdin_buf);
 
-  /* "mrfifo/fast_loops.pyx":205
+  /* "mrfifo/fast_loops.pyx":213
  *     stdio.fclose(fin)
  *     stdlib.free(stdin_buf)
  *     stdlib.free(buffer)             # <<<<<<<<<<<<<<
  * 
  *     return n # number of lines distributed (excluding header)
  */
   free(__pyx_v_buffer);
 
-  /* "mrfifo/fast_loops.pyx":207
+  /* "mrfifo/fast_loops.pyx":215
  *     stdlib.free(buffer)
  * 
  *     return n # number of lines distributed (excluding header)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "mrfifo/fast_loops.pyx":101
+  /* "mrfifo/fast_loops.pyx":105
  * 
  * 
  * def distribute_by_substr(str fin_name, list fifo_names, dict sub_lookup,             # <<<<<<<<<<<<<<
  *                          size_t sub_size, bytes sub_lead=b"\tCB:Z:",
  *                          size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  */
 
@@ -4905,20 +5034,20 @@
   __Pyx_XDECREF(__pyx_v_fifo_names);
   __Pyx_XDECREF(__pyx_v_header_fifo);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mrfifo/fast_loops.pyx":210
+/* "mrfifo/fast_loops.pyx":218
  * 
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
+ *             header_fifo="", _buffer_size=0, custom_header=None, int n_reopen_inputs=1, **kw):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6mrfifo_10fast_loops_5collect(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
@@ -4935,50 +5064,57 @@
 ) {
   PyObject *__pyx_v_fifo_names = 0;
   PyObject *__pyx_v_fout_name = 0;
   int __pyx_v_chunk_size;
   size_t __pyx_v_in_buf_size;
   size_t __pyx_v_out_buf_size;
   PyObject *__pyx_v_header_fifo = 0;
+  PyObject *__pyx_v__buffer_size = 0;
   PyObject *__pyx_v_custom_header = 0;
   int __pyx_v_n_reopen_inputs;
+  CYTHON_UNUSED PyObject *__pyx_v_kw = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[8] = {0,0,0,0,0,0,0,0};
+  PyObject* values[9] = {0,0,0,0,0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("collect (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  __pyx_v_kw = PyDict_New(); if (unlikely(!__pyx_v_kw)) return NULL;
+  __Pyx_GOTREF(__pyx_v_kw);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fifo_names,&__pyx_n_s_fout_name,&__pyx_n_s_chunk_size,&__pyx_n_s_in_buf_size,&__pyx_n_s_out_buf_size,&__pyx_n_s_header_fifo,&__pyx_n_s_custom_header,&__pyx_n_s_n_reopen_inputs,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fifo_names,&__pyx_n_s_fout_name,&__pyx_n_s_chunk_size,&__pyx_n_s_in_buf_size,&__pyx_n_s_out_buf_size,&__pyx_n_s_header_fifo,&__pyx_n_s_buffer_size,&__pyx_n_s_custom_header,&__pyx_n_s_n_reopen_inputs,0};
     values[5] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject*)__pyx_kp_u_)));
+    values[6] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)__pyx_int_0)));
 
-    /* "mrfifo/fast_loops.pyx":212
+    /* "mrfifo/fast_loops.pyx":220
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None, int n_reopen_inputs=1):             # <<<<<<<<<<<<<<
+ *             header_fifo="", _buffer_size=0, custom_header=None, int n_reopen_inputs=1, **kw):             # <<<<<<<<<<<<<<
  * 
  *     if header_fifo == 0:
  */
-    values[6] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
+    values[7] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
+        case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
         case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
@@ -4997,75 +5133,84 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fifo_names)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fout_name)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("collect", 0, 2, 8, 1); __PYX_ERR(0, 210, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("collect", 0, 2, 9, 1); __PYX_ERR(0, 218, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_chunk_size);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_in_buf_size);
           if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_out_buf_size);
           if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_header_fifo);
           if (value) { values[5] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_custom_header);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_buffer_size);
           if (value) { values[6] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_reopen_inputs);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_custom_header);
           if (value) { values[7] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  8:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_reopen_inputs);
+          if (value) { values[8] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "collect") < 0)) __PYX_ERR(0, 210, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kw, values + 0, kwd_pos_args, "collect") < 0)) __PYX_ERR(0, 218, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
+        case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
         case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
@@ -5079,80 +5224,83 @@
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_fifo_names = ((PyObject*)values[0]);
     __pyx_v_fout_name = ((PyObject*)values[1]);
     if (values[2]) {
-      __pyx_v_chunk_size = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_chunk_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
+      __pyx_v_chunk_size = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_chunk_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
     } else {
       __pyx_v_chunk_size = ((int)((int)0x2710));
     }
     if (values[3]) {
-      __pyx_v_in_buf_size = __Pyx_PyInt_As_size_t(values[3]); if (unlikely((__pyx_v_in_buf_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 211, __pyx_L3_error)
+      __pyx_v_in_buf_size = __Pyx_PyInt_As_size_t(values[3]); if (unlikely((__pyx_v_in_buf_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 219, __pyx_L3_error)
     } else {
       __pyx_v_in_buf_size = ((size_t)((size_t)0x80000));
     }
     if (values[4]) {
-      __pyx_v_out_buf_size = __Pyx_PyInt_As_size_t(values[4]); if (unlikely((__pyx_v_out_buf_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 211, __pyx_L3_error)
+      __pyx_v_out_buf_size = __Pyx_PyInt_As_size_t(values[4]); if (unlikely((__pyx_v_out_buf_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 219, __pyx_L3_error)
     } else {
       __pyx_v_out_buf_size = ((size_t)((size_t)0x100000));
     }
     __pyx_v_header_fifo = values[5];
-    __pyx_v_custom_header = values[6];
-    if (values[7]) {
-      __pyx_v_n_reopen_inputs = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_n_reopen_inputs == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L3_error)
+    __pyx_v__buffer_size = values[6];
+    __pyx_v_custom_header = values[7];
+    if (values[8]) {
+      __pyx_v_n_reopen_inputs = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_n_reopen_inputs == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 220, __pyx_L3_error)
     } else {
       __pyx_v_n_reopen_inputs = ((int)((int)1));
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("collect", 0, 2, 8, __pyx_nargs); __PYX_ERR(0, 210, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("collect", 0, 2, 9, __pyx_nargs); __PYX_ERR(0, 218, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
+  __Pyx_DECREF(__pyx_v_kw); __pyx_v_kw = 0;
   __Pyx_AddTraceback("mrfifo.fast_loops.collect", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fifo_names), (&PyList_Type), 1, "fifo_names", 1))) __PYX_ERR(0, 210, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fout_name), (&PyUnicode_Type), 1, "fout_name", 1))) __PYX_ERR(0, 210, __pyx_L1_error)
-  __pyx_r = __pyx_pf_6mrfifo_10fast_loops_4collect(__pyx_self, __pyx_v_fifo_names, __pyx_v_fout_name, __pyx_v_chunk_size, __pyx_v_in_buf_size, __pyx_v_out_buf_size, __pyx_v_header_fifo, __pyx_v_custom_header, __pyx_v_n_reopen_inputs);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fifo_names), (&PyList_Type), 1, "fifo_names", 1))) __PYX_ERR(0, 218, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fout_name), (&PyUnicode_Type), 1, "fout_name", 1))) __PYX_ERR(0, 218, __pyx_L1_error)
+  __pyx_r = __pyx_pf_6mrfifo_10fast_loops_4collect(__pyx_self, __pyx_v_fifo_names, __pyx_v_fout_name, __pyx_v_chunk_size, __pyx_v_in_buf_size, __pyx_v_out_buf_size, __pyx_v_header_fifo, __pyx_v__buffer_size, __pyx_v_custom_header, __pyx_v_n_reopen_inputs, __pyx_v_kw);
 
-  /* "mrfifo/fast_loops.pyx":210
+  /* "mrfifo/fast_loops.pyx":218
  * 
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
+ *             header_fifo="", _buffer_size=0, custom_header=None, int n_reopen_inputs=1, **kw):
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_DECREF(__pyx_v_kw);
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6mrfifo_10fast_loops_4collect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_fout_name, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_custom_header, int __pyx_v_n_reopen_inputs) {
+static PyObject *__pyx_pf_6mrfifo_10fast_loops_4collect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_fout_name, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v__buffer_size, PyObject *__pyx_v_custom_header, int __pyx_v_n_reopen_inputs, CYTHON_UNUSED PyObject *__pyx_v_kw) {
   int __pyx_v_i;
   int __pyx_v_j;
   int __pyx_v_k;
   size_t __pyx_v_n_ins;
   size_t __pyx_v_n;
   size_t __pyx_v_n_out;
   char *__pyx_v_buffer;
@@ -5167,743 +5315,784 @@
   FILE *__pyx_v_fout;
   PyObject *__pyx_v_header_bytes = NULL;
   FILE *__pyx_v_fheader;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  Py_ssize_t __pyx_t_3;
-  char const *__pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
+  size_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  char const *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
-  char const *__pyx_t_8;
-  int __pyx_t_9;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  char const *__pyx_t_9;
   int __pyx_t_10;
-  size_t __pyx_t_11;
+  int __pyx_t_11;
   size_t __pyx_t_12;
   int __pyx_t_13;
   int __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("collect", 0);
   __Pyx_INCREF(__pyx_v_fifo_names);
   __Pyx_INCREF(__pyx_v_header_fifo);
 
-  /* "mrfifo/fast_loops.pyx":214
- *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
+  /* "mrfifo/fast_loops.pyx":222
+ *             header_fifo="", _buffer_size=0, custom_header=None, int n_reopen_inputs=1, **kw):
  * 
  *     if header_fifo == 0:             # <<<<<<<<<<<<<<
  *         # special mode: use the first fifo name for header data
  *         # and the other as round-robin inputs as usual
  */
-  __pyx_t_1 = (__Pyx_PyInt_BoolEqObjC(__pyx_v_header_fifo, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 214, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyInt_BoolEqObjC(__pyx_v_header_fifo, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 222, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "mrfifo/fast_loops.pyx":217
+    /* "mrfifo/fast_loops.pyx":225
  *         # special mode: use the first fifo name for header data
  *         # and the other as round-robin inputs as usual
  *         header_fifo = fifo_names[0]             # <<<<<<<<<<<<<<
  *         fifo_names = fifo_names[1:]
  * 
  */
     if (unlikely(__pyx_v_fifo_names == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 217, __pyx_L1_error)
+      __PYX_ERR(0, 225, __pyx_L1_error)
     }
     __pyx_t_2 = PyList_GET_ITEM(__pyx_v_fifo_names, 0);
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_header_fifo, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "mrfifo/fast_loops.pyx":218
+    /* "mrfifo/fast_loops.pyx":226
  *         # and the other as round-robin inputs as usual
  *         header_fifo = fifo_names[0]
  *         fifo_names = fifo_names[1:]             # <<<<<<<<<<<<<<
  * 
- *     cdef int i = 0
+ *     if _buffer_size > 0:
  */
     if (unlikely(__pyx_v_fifo_names == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 218, __pyx_L1_error)
+      __PYX_ERR(0, 226, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_PyList_GetSlice(__pyx_v_fifo_names, 1, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyList_GetSlice(__pyx_v_fifo_names, 1, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_fifo_names, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "mrfifo/fast_loops.pyx":214
- *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
+    /* "mrfifo/fast_loops.pyx":222
+ *             header_fifo="", _buffer_size=0, custom_header=None, int n_reopen_inputs=1, **kw):
  * 
  *     if header_fifo == 0:             # <<<<<<<<<<<<<<
  *         # special mode: use the first fifo name for header data
  *         # and the other as round-robin inputs as usual
  */
   }
 
-  /* "mrfifo/fast_loops.pyx":220
+  /* "mrfifo/fast_loops.pyx":228
  *         fifo_names = fifo_names[1:]
  * 
+ *     if _buffer_size > 0:             # <<<<<<<<<<<<<<
+ *         in_buf_size = _buffer_size
+ *         out_buf_size = _buffer_size
+ */
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v__buffer_size, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__pyx_t_1) {
+
+    /* "mrfifo/fast_loops.pyx":229
+ * 
+ *     if _buffer_size > 0:
+ *         in_buf_size = _buffer_size             # <<<<<<<<<<<<<<
+ *         out_buf_size = _buffer_size
+ * 
+ */
+    __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_v__buffer_size); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 229, __pyx_L1_error)
+    __pyx_v_in_buf_size = __pyx_t_3;
+
+    /* "mrfifo/fast_loops.pyx":230
+ *     if _buffer_size > 0:
+ *         in_buf_size = _buffer_size
+ *         out_buf_size = _buffer_size             # <<<<<<<<<<<<<<
+ * 
+ *     cdef int i = 0
+ */
+    __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_v__buffer_size); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 230, __pyx_L1_error)
+    __pyx_v_out_buf_size = __pyx_t_3;
+
+    /* "mrfifo/fast_loops.pyx":228
+ *         fifo_names = fifo_names[1:]
+ * 
+ *     if _buffer_size > 0:             # <<<<<<<<<<<<<<
+ *         in_buf_size = _buffer_size
+ *         out_buf_size = _buffer_size
+ */
+  }
+
+  /* "mrfifo/fast_loops.pyx":232
+ *         out_buf_size = _buffer_size
+ * 
  *     cdef int i = 0             # <<<<<<<<<<<<<<
  *     cdef int j = 0
  *     cdef int k = 0
  */
   __pyx_v_i = 0;
 
-  /* "mrfifo/fast_loops.pyx":221
+  /* "mrfifo/fast_loops.pyx":233
  * 
  *     cdef int i = 0
  *     cdef int j = 0             # <<<<<<<<<<<<<<
  *     cdef int k = 0
  *     cdef size_t n_ins = len(fifo_names)
  */
   __pyx_v_j = 0;
 
-  /* "mrfifo/fast_loops.pyx":222
+  /* "mrfifo/fast_loops.pyx":234
  *     cdef int i = 0
  *     cdef int j = 0
  *     cdef int k = 0             # <<<<<<<<<<<<<<
  *     cdef size_t n_ins = len(fifo_names)
  *     cdef size_t n = 0
  */
   __pyx_v_k = 0;
 
-  /* "mrfifo/fast_loops.pyx":223
+  /* "mrfifo/fast_loops.pyx":235
  *     cdef int j = 0
  *     cdef int k = 0
  *     cdef size_t n_ins = len(fifo_names)             # <<<<<<<<<<<<<<
  *     cdef size_t n = 0
  *     cdef size_t n_out = 0
  */
   if (unlikely(__pyx_v_fifo_names == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 223, __pyx_L1_error)
+    __PYX_ERR(0, 235, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_fifo_names); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 223, __pyx_L1_error)
-  __pyx_v_n_ins = __pyx_t_3;
+  __pyx_t_4 = __Pyx_PyList_GET_SIZE(__pyx_v_fifo_names); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_v_n_ins = __pyx_t_4;
 
-  /* "mrfifo/fast_loops.pyx":224
+  /* "mrfifo/fast_loops.pyx":236
  *     cdef int k = 0
  *     cdef size_t n_ins = len(fifo_names)
  *     cdef size_t n = 0             # <<<<<<<<<<<<<<
  *     cdef size_t n_out = 0
  *     cdef str line
  */
   __pyx_v_n = 0;
 
-  /* "mrfifo/fast_loops.pyx":225
+  /* "mrfifo/fast_loops.pyx":237
  *     cdef size_t n_ins = len(fifo_names)
  *     cdef size_t n = 0
  *     cdef size_t n_out = 0             # <<<<<<<<<<<<<<
  *     cdef str line
  *     cdef char* buffer
  */
   __pyx_v_n_out = 0;
 
-  /* "mrfifo/fast_loops.pyx":233
+  /* "mrfifo/fast_loops.pyx":245
  *     cdef char* fifo_buffers[128]
  * 
  *     import sys             # <<<<<<<<<<<<<<
  *     # sys.stderr.write(f"collecting from {fifo_names} into {fout_name}")
  *     assert n <= 128
  */
-  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_sys, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_sys, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_sys = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "mrfifo/fast_loops.pyx":235
+  /* "mrfifo/fast_loops.pyx":247
  *     import sys
  *     # sys.stderr.write(f"collecting from {fifo_names} into {fout_name}")
  *     assert n <= 128             # <<<<<<<<<<<<<<
  *     cdef stdio.FILE *fifos[128]
  *     cdef bint[128] fifo_closed
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = (__pyx_v_n <= 0x80);
     if (unlikely(!__pyx_t_1)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 235, __pyx_L1_error)
+      __PYX_ERR(0, 247, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 235, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 247, __pyx_L1_error)
   #endif
 
-  /* "mrfifo/fast_loops.pyx":239
+  /* "mrfifo/fast_loops.pyx":251
  *     cdef bint[128] fifo_closed
  * 
  *     cdef size_t drained_fifos = 0             # <<<<<<<<<<<<<<
  *     cdef int n_loop = 0
  * 
  */
   __pyx_v_drained_fifos = 0;
 
-  /* "mrfifo/fast_loops.pyx":240
+  /* "mrfifo/fast_loops.pyx":252
  * 
  *     cdef size_t drained_fifos = 0
  *     cdef int n_loop = 0             # <<<<<<<<<<<<<<
  * 
  *     # line buffer
  */
   __pyx_v_n_loop = 0;
 
-  /* "mrfifo/fast_loops.pyx":243
+  /* "mrfifo/fast_loops.pyx":255
  * 
  *     # line buffer
  *     buffer = <char*>stdlib.malloc(out_buf_size)             # <<<<<<<<<<<<<<
  *     # prepare output file and buffer
  *     cdef char* out_buf = <char*>stdlib.malloc(out_buf_size)
  */
   __pyx_v_buffer = ((char *)malloc(__pyx_v_out_buf_size));
 
-  /* "mrfifo/fast_loops.pyx":245
+  /* "mrfifo/fast_loops.pyx":257
  *     buffer = <char*>stdlib.malloc(out_buf_size)
  *     # prepare output file and buffer
  *     cdef char* out_buf = <char*>stdlib.malloc(out_buf_size)             # <<<<<<<<<<<<<<
  *     cdef stdio.FILE *fout = stdio.fopen(fout_name.encode('utf-8'), 'w')
  *     stdio.setvbuf(fout, out_buf, stdio._IOFBF, out_buf_size)
  */
   __pyx_v_out_buf = ((char *)malloc(__pyx_v_out_buf_size));
 
-  /* "mrfifo/fast_loops.pyx":246
+  /* "mrfifo/fast_loops.pyx":258
  *     # prepare output file and buffer
  *     cdef char* out_buf = <char*>stdlib.malloc(out_buf_size)
  *     cdef stdio.FILE *fout = stdio.fopen(fout_name.encode('utf-8'), 'w')             # <<<<<<<<<<<<<<
  *     stdio.setvbuf(fout, out_buf, stdio._IOFBF, out_buf_size)
  * 
  */
   if (unlikely(__pyx_v_fout_name == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 246, __pyx_L1_error)
+    __PYX_ERR(0, 258, __pyx_L1_error)
   }
-  __pyx_t_2 = PyUnicode_AsUTF8String(__pyx_v_fout_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_2 = PyUnicode_AsUTF8String(__pyx_v_fout_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 246, __pyx_L1_error)
-  __pyx_v_fout = fopen(__pyx_t_4, ((char const *)"w"));
+  __pyx_t_5 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_v_fout = fopen(__pyx_t_5, ((char const *)"w"));
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "mrfifo/fast_loops.pyx":247
+  /* "mrfifo/fast_loops.pyx":259
  *     cdef char* out_buf = <char*>stdlib.malloc(out_buf_size)
  *     cdef stdio.FILE *fout = stdio.fopen(fout_name.encode('utf-8'), 'w')
  *     stdio.setvbuf(fout, out_buf, stdio._IOFBF, out_buf_size)             # <<<<<<<<<<<<<<
  * 
  *     # cdef char * line_bytes
  */
   (void)(setvbuf(__pyx_v_fout, __pyx_v_out_buf, _IOFBF, __pyx_v_out_buf_size));
 
-  /* "mrfifo/fast_loops.pyx":250
+  /* "mrfifo/fast_loops.pyx":262
  * 
  *     # cdef char * line_bytes
  *     if custom_header is not None:             # <<<<<<<<<<<<<<
  *         # we have a custom header string, write this first!
  *         header_bytes = custom_header.encode('utf-8')
  */
   __pyx_t_1 = (__pyx_v_custom_header != Py_None);
   if (__pyx_t_1) {
 
-    /* "mrfifo/fast_loops.pyx":252
+    /* "mrfifo/fast_loops.pyx":264
  *     if custom_header is not None:
  *         # we have a custom header string, write this first!
  *         header_bytes = custom_header.encode('utf-8')             # <<<<<<<<<<<<<<
  *         stdio.fwrite(<const char*>header_bytes, len(header_bytes), 1, fout)
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_custom_header, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 252, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = NULL;
-    __pyx_t_7 = 0;
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_custom_header, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = NULL;
+    __pyx_t_8 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_6);
+    if (likely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
-        __pyx_t_7 = 1;
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __pyx_t_8 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_kp_u_utf_8};
-      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
-      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 252, __pyx_L1_error)
+      PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_kp_u_utf_8};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __pyx_v_header_bytes = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "mrfifo/fast_loops.pyx":253
+    /* "mrfifo/fast_loops.pyx":265
  *         # we have a custom header string, write this first!
  *         header_bytes = custom_header.encode('utf-8')
  *         stdio.fwrite(<const char*>header_bytes, len(header_bytes), 1, fout)             # <<<<<<<<<<<<<<
  * 
  *     cdef stdio.FILE *fheader
  */
-    __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_header_bytes); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 253, __pyx_L1_error)
-    __pyx_t_3 = PyObject_Length(__pyx_v_header_bytes); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 253, __pyx_L1_error)
-    (void)(fwrite(((char const *)__pyx_t_8), __pyx_t_3, 1, __pyx_v_fout));
+    __pyx_t_9 = __Pyx_PyObject_AsString(__pyx_v_header_bytes); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 265, __pyx_L1_error)
+    __pyx_t_4 = PyObject_Length(__pyx_v_header_bytes); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 265, __pyx_L1_error)
+    (void)(fwrite(((char const *)__pyx_t_9), __pyx_t_4, 1, __pyx_v_fout));
 
-    /* "mrfifo/fast_loops.pyx":250
+    /* "mrfifo/fast_loops.pyx":262
  * 
  *     # cdef char * line_bytes
  *     if custom_header is not None:             # <<<<<<<<<<<<<<
  *         # we have a custom header string, write this first!
  *         header_bytes = custom_header.encode('utf-8')
  */
   }
 
-  /* "mrfifo/fast_loops.pyx":256
+  /* "mrfifo/fast_loops.pyx":268
  * 
  *     cdef stdio.FILE *fheader
  *     if header_fifo:             # <<<<<<<<<<<<<<
  *         # we have some special, un-multiplexed header data. Read this
  *         # stuff first and write it to the output
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 268, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "mrfifo/fast_loops.pyx":259
+    /* "mrfifo/fast_loops.pyx":271
  *         # we have some special, un-multiplexed header data. Read this
  *         # stuff first and write it to the output
  *         fheader = stdio.fopen(header_fifo.encode('utf-8'), 'r')             # <<<<<<<<<<<<<<
  *         while(True):
  *             n_read = stdio.getline(&buffer, &out_buf_size, fheader)
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_header_fifo, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = NULL;
-    __pyx_t_7 = 0;
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_header_fifo, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = NULL;
+    __pyx_t_8 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_6);
+    if (likely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
-        __pyx_t_7 = 1;
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __pyx_t_8 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_kp_u_utf_8};
-      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
-      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
+      PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_kp_u_utf_8};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 259, __pyx_L1_error)
-    __pyx_v_fheader = fopen(__pyx_t_4, ((char const *)"r"));
+    __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 271, __pyx_L1_error)
+    __pyx_v_fheader = fopen(__pyx_t_5, ((char const *)"r"));
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "mrfifo/fast_loops.pyx":260
+    /* "mrfifo/fast_loops.pyx":272
  *         # stuff first and write it to the output
  *         fheader = stdio.fopen(header_fifo.encode('utf-8'), 'r')
  *         while(True):             # <<<<<<<<<<<<<<
  *             n_read = stdio.getline(&buffer, &out_buf_size, fheader)
  *             if n_read <= 0:
  */
     while (1) {
 
-      /* "mrfifo/fast_loops.pyx":261
+      /* "mrfifo/fast_loops.pyx":273
  *         fheader = stdio.fopen(header_fifo.encode('utf-8'), 'r')
  *         while(True):
  *             n_read = stdio.getline(&buffer, &out_buf_size, fheader)             # <<<<<<<<<<<<<<
  *             if n_read <= 0:
  *                 break
  */
       __pyx_v_n_read = getline((&__pyx_v_buffer), (&__pyx_v_out_buf_size), __pyx_v_fheader);
 
-      /* "mrfifo/fast_loops.pyx":262
+      /* "mrfifo/fast_loops.pyx":274
  *         while(True):
  *             n_read = stdio.getline(&buffer, &out_buf_size, fheader)
  *             if n_read <= 0:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
       __pyx_t_1 = (__pyx_v_n_read <= 0);
       if (__pyx_t_1) {
 
-        /* "mrfifo/fast_loops.pyx":263
+        /* "mrfifo/fast_loops.pyx":275
  *             n_read = stdio.getline(&buffer, &out_buf_size, fheader)
  *             if n_read <= 0:
  *                 break             # <<<<<<<<<<<<<<
  * 
  *             stdio.fwrite(buffer, n_read, 1, fout)
  */
-        goto __pyx_L7_break;
+        goto __pyx_L8_break;
 
-        /* "mrfifo/fast_loops.pyx":262
+        /* "mrfifo/fast_loops.pyx":274
  *         while(True):
  *             n_read = stdio.getline(&buffer, &out_buf_size, fheader)
  *             if n_read <= 0:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
       }
 
-      /* "mrfifo/fast_loops.pyx":265
+      /* "mrfifo/fast_loops.pyx":277
  *                 break
  * 
  *             stdio.fwrite(buffer, n_read, 1, fout)             # <<<<<<<<<<<<<<
  * 
  *         # all header data has been read! close this fifo's reading end
  */
       (void)(fwrite(__pyx_v_buffer, __pyx_v_n_read, 1, __pyx_v_fout));
     }
-    __pyx_L7_break:;
+    __pyx_L8_break:;
 
-    /* "mrfifo/fast_loops.pyx":268
+    /* "mrfifo/fast_loops.pyx":280
  * 
  *         # all header data has been read! close this fifo's reading end
  *         stdio.fclose(fheader)             # <<<<<<<<<<<<<<
  * 
  *     for n_loop in range(n_reopen_inputs):
  */
     (void)(fclose(__pyx_v_fheader));
 
-    /* "mrfifo/fast_loops.pyx":256
+    /* "mrfifo/fast_loops.pyx":268
  * 
  *     cdef stdio.FILE *fheader
  *     if header_fifo:             # <<<<<<<<<<<<<<
  *         # we have some special, un-multiplexed header data. Read this
  *         # stuff first and write it to the output
  */
   }
 
-  /* "mrfifo/fast_loops.pyx":270
+  /* "mrfifo/fast_loops.pyx":282
  *         stdio.fclose(fheader)
  * 
  *     for n_loop in range(n_reopen_inputs):             # <<<<<<<<<<<<<<
  *         #print(f"opening the input fifos for the {n_loop}th time: {fifo_names}")
  *         # now prepare input from all the demuxed fifos
  */
-  __pyx_t_7 = __pyx_v_n_reopen_inputs;
-  __pyx_t_9 = __pyx_t_7;
-  for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
-    __pyx_v_n_loop = __pyx_t_10;
+  __pyx_t_8 = __pyx_v_n_reopen_inputs;
+  __pyx_t_10 = __pyx_t_8;
+  for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
+    __pyx_v_n_loop = __pyx_t_11;
 
-    /* "mrfifo/fast_loops.pyx":273
+    /* "mrfifo/fast_loops.pyx":285
  *         #print(f"opening the input fifos for the {n_loop}th time: {fifo_names}")
  *         # now prepare input from all the demuxed fifos
  *         for i in range(n_ins):             # <<<<<<<<<<<<<<
  *             fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)
  *             fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')
  */
-    __pyx_t_11 = __pyx_v_n_ins;
-    __pyx_t_12 = __pyx_t_11;
+    __pyx_t_3 = __pyx_v_n_ins;
+    __pyx_t_12 = __pyx_t_3;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_i = __pyx_t_13;
 
-      /* "mrfifo/fast_loops.pyx":274
+      /* "mrfifo/fast_loops.pyx":286
  *         # now prepare input from all the demuxed fifos
  *         for i in range(n_ins):
  *             fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)             # <<<<<<<<<<<<<<
  *             fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')
  *             stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)
  */
       (__pyx_v_fifo_buffers[__pyx_v_i]) = ((char *)malloc(__pyx_v_in_buf_size));
 
-      /* "mrfifo/fast_loops.pyx":275
+      /* "mrfifo/fast_loops.pyx":287
  *         for i in range(n_ins):
  *             fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)
  *             fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')             # <<<<<<<<<<<<<<
  *             stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)
  * 
  */
       if (unlikely(__pyx_v_fifo_names == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 275, __pyx_L1_error)
+        __PYX_ERR(0, 287, __pyx_L1_error)
       }
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_fifo_names, __pyx_v_i), __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 275, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = NULL;
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_fifo_names, __pyx_v_i), __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 287, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = NULL;
       __pyx_t_14 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_5))) {
-        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
-        if (likely(__pyx_t_6)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-          __Pyx_INCREF(__pyx_t_6);
+      if (likely(PyMethod_Check(__pyx_t_6))) {
+        __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+        if (likely(__pyx_t_7)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+          __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_14 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_kp_u_utf_8};
-        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_14, 1+__pyx_t_14);
-        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 275, __pyx_L1_error)
+        PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_kp_u_utf_8};
+        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_14, 1+__pyx_t_14);
+        __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
-      __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 275, __pyx_L1_error)
-      (__pyx_v_fifos[__pyx_v_i]) = fopen(__pyx_t_4, ((char const *)"r"));
+      __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 287, __pyx_L1_error)
+      (__pyx_v_fifos[__pyx_v_i]) = fopen(__pyx_t_5, ((char const *)"r"));
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "mrfifo/fast_loops.pyx":276
+      /* "mrfifo/fast_loops.pyx":288
  *             fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)
  *             fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')
  *             stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)             # <<<<<<<<<<<<<<
  * 
  *         drained_fifos = 0
  */
       (void)(setvbuf((__pyx_v_fifos[__pyx_v_i]), (__pyx_v_fifo_buffers[__pyx_v_i]), _IOFBF, __pyx_v_in_buf_size));
     }
 
-    /* "mrfifo/fast_loops.pyx":278
+    /* "mrfifo/fast_loops.pyx":290
  *             stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)
  * 
  *         drained_fifos = 0             # <<<<<<<<<<<<<<
  *         for i in range(n_ins):
  *             fifo_closed[i] = False
  */
     __pyx_v_drained_fifos = 0;
 
-    /* "mrfifo/fast_loops.pyx":279
+    /* "mrfifo/fast_loops.pyx":291
  * 
  *         drained_fifos = 0
  *         for i in range(n_ins):             # <<<<<<<<<<<<<<
  *             fifo_closed[i] = False
  * 
  */
-    __pyx_t_11 = __pyx_v_n_ins;
-    __pyx_t_12 = __pyx_t_11;
+    __pyx_t_3 = __pyx_v_n_ins;
+    __pyx_t_12 = __pyx_t_3;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_i = __pyx_t_13;
 
-      /* "mrfifo/fast_loops.pyx":280
+      /* "mrfifo/fast_loops.pyx":292
  *         drained_fifos = 0
  *         for i in range(n_ins):
  *             fifo_closed[i] = False             # <<<<<<<<<<<<<<
  * 
  *         # main mutiplexing loop
  */
       (__pyx_v_fifo_closed[__pyx_v_i]) = 0;
     }
 
-    /* "mrfifo/fast_loops.pyx":283
+    /* "mrfifo/fast_loops.pyx":295
  * 
  *         # main mutiplexing loop
  *         while(drained_fifos < n_ins):             # <<<<<<<<<<<<<<
  *             j = n // chunk_size
  *             k = j % n_ins # index of fifo
  */
     while (1) {
       __pyx_t_1 = (__pyx_v_drained_fifos < __pyx_v_n_ins);
       if (!__pyx_t_1) break;
 
-      /* "mrfifo/fast_loops.pyx":284
+      /* "mrfifo/fast_loops.pyx":296
  *         # main mutiplexing loop
  *         while(drained_fifos < n_ins):
  *             j = n // chunk_size             # <<<<<<<<<<<<<<
  *             k = j % n_ins # index of fifo
  *             if not fifo_closed[k]:
  */
       __pyx_v_j = (__pyx_v_n / __pyx_v_chunk_size);
 
-      /* "mrfifo/fast_loops.pyx":285
+      /* "mrfifo/fast_loops.pyx":297
  *         while(drained_fifos < n_ins):
  *             j = n // chunk_size
  *             k = j % n_ins # index of fifo             # <<<<<<<<<<<<<<
  *             if not fifo_closed[k]:
  *                 # print(f"collection wants to read from {fifo_names[k]}. blocking")
  */
       __pyx_v_k = (__pyx_v_j % __pyx_v_n_ins);
 
-      /* "mrfifo/fast_loops.pyx":286
+      /* "mrfifo/fast_loops.pyx":298
  *             j = n // chunk_size
  *             k = j % n_ins # index of fifo
  *             if not fifo_closed[k]:             # <<<<<<<<<<<<<<
  *                 # print(f"collection wants to read from {fifo_names[k]}. blocking")
  *                 n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
  */
       __pyx_t_1 = (!(__pyx_v_fifo_closed[__pyx_v_k]));
       if (__pyx_t_1) {
 
-        /* "mrfifo/fast_loops.pyx":288
+        /* "mrfifo/fast_loops.pyx":300
  *             if not fifo_closed[k]:
  *                 # print(f"collection wants to read from {fifo_names[k]}. blocking")
  *                 n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])             # <<<<<<<<<<<<<<
  *                 if n_read <= 0:
  *                     fifo_closed[k] = True
  */
         __pyx_v_n_read = getline((&__pyx_v_buffer), (&__pyx_v_out_buf_size), (__pyx_v_fifos[__pyx_v_k]));
 
-        /* "mrfifo/fast_loops.pyx":289
+        /* "mrfifo/fast_loops.pyx":301
  *                 # print(f"collection wants to read from {fifo_names[k]}. blocking")
  *                 n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
  *                 if n_read <= 0:             # <<<<<<<<<<<<<<
  *                     fifo_closed[k] = True
  *                     drained_fifos += 1
  */
         __pyx_t_1 = (__pyx_v_n_read <= 0);
         if (__pyx_t_1) {
 
-          /* "mrfifo/fast_loops.pyx":290
+          /* "mrfifo/fast_loops.pyx":302
  *                 n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
  *                 if n_read <= 0:
  *                     fifo_closed[k] = True             # <<<<<<<<<<<<<<
  *                     drained_fifos += 1
  *                 else:
  */
           (__pyx_v_fifo_closed[__pyx_v_k]) = 1;
 
-          /* "mrfifo/fast_loops.pyx":291
+          /* "mrfifo/fast_loops.pyx":303
  *                 if n_read <= 0:
  *                     fifo_closed[k] = True
  *                     drained_fifos += 1             # <<<<<<<<<<<<<<
  *                 else:
  *                     # print(f"fifo {k} ({fifo_names[k]}). {n_read} bytes. writing to {fout_name}")
  */
           __pyx_v_drained_fifos = (__pyx_v_drained_fifos + 1);
 
-          /* "mrfifo/fast_loops.pyx":289
+          /* "mrfifo/fast_loops.pyx":301
  *                 # print(f"collection wants to read from {fifo_names[k]}. blocking")
  *                 n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
  *                 if n_read <= 0:             # <<<<<<<<<<<<<<
  *                     fifo_closed[k] = True
  *                     drained_fifos += 1
  */
-          goto __pyx_L18;
+          goto __pyx_L19;
         }
 
-        /* "mrfifo/fast_loops.pyx":294
+        /* "mrfifo/fast_loops.pyx":306
  *                 else:
  *                     # print(f"fifo {k} ({fifo_names[k]}). {n_read} bytes. writing to {fout_name}")
  *                     stdio.fwrite(buffer, n_read, 1, fout)             # <<<<<<<<<<<<<<
  *                     n_out += 1
  *             n += 1
  */
         /*else*/ {
           (void)(fwrite(__pyx_v_buffer, __pyx_v_n_read, 1, __pyx_v_fout));
 
-          /* "mrfifo/fast_loops.pyx":295
+          /* "mrfifo/fast_loops.pyx":307
  *                     # print(f"fifo {k} ({fifo_names[k]}). {n_read} bytes. writing to {fout_name}")
  *                     stdio.fwrite(buffer, n_read, 1, fout)
  *                     n_out += 1             # <<<<<<<<<<<<<<
  *             n += 1
  * 
  */
           __pyx_v_n_out = (__pyx_v_n_out + 1);
         }
-        __pyx_L18:;
+        __pyx_L19:;
 
-        /* "mrfifo/fast_loops.pyx":286
+        /* "mrfifo/fast_loops.pyx":298
  *             j = n // chunk_size
  *             k = j % n_ins # index of fifo
  *             if not fifo_closed[k]:             # <<<<<<<<<<<<<<
  *                 # print(f"collection wants to read from {fifo_names[k]}. blocking")
  *                 n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
  */
       }
 
-      /* "mrfifo/fast_loops.pyx":296
+      /* "mrfifo/fast_loops.pyx":308
  *                     stdio.fwrite(buffer, n_read, 1, fout)
  *                     n_out += 1
  *             n += 1             # <<<<<<<<<<<<<<
  * 
  *         for i in range(n_ins):
  */
       __pyx_v_n = (__pyx_v_n + 1);
     }
 
-    /* "mrfifo/fast_loops.pyx":298
+    /* "mrfifo/fast_loops.pyx":310
  *             n += 1
  * 
  *         for i in range(n_ins):             # <<<<<<<<<<<<<<
  *             stdio.fclose(fifos[i])
  *             stdlib.free(fifo_buffers[i])
  */
-    __pyx_t_11 = __pyx_v_n_ins;
-    __pyx_t_12 = __pyx_t_11;
+    __pyx_t_3 = __pyx_v_n_ins;
+    __pyx_t_12 = __pyx_t_3;
     for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
       __pyx_v_i = __pyx_t_13;
 
-      /* "mrfifo/fast_loops.pyx":299
+      /* "mrfifo/fast_loops.pyx":311
  * 
  *         for i in range(n_ins):
  *             stdio.fclose(fifos[i])             # <<<<<<<<<<<<<<
  *             stdlib.free(fifo_buffers[i])
  * 
  */
       (void)(fclose((__pyx_v_fifos[__pyx_v_i])));
 
-      /* "mrfifo/fast_loops.pyx":300
+      /* "mrfifo/fast_loops.pyx":312
  *         for i in range(n_ins):
  *             stdio.fclose(fifos[i])
  *             stdlib.free(fifo_buffers[i])             # <<<<<<<<<<<<<<
  * 
  *     # free the line buffer, close the output, and free the output buffer
  */
       free((__pyx_v_fifo_buffers[__pyx_v_i]));
     }
   }
 
-  /* "mrfifo/fast_loops.pyx":303
+  /* "mrfifo/fast_loops.pyx":315
  * 
  *     # free the line buffer, close the output, and free the output buffer
  *     stdlib.free(buffer)             # <<<<<<<<<<<<<<
  *     stdio.fclose(fout)
  *     stdlib.free(out_buf)
  */
   free(__pyx_v_buffer);
 
-  /* "mrfifo/fast_loops.pyx":304
+  /* "mrfifo/fast_loops.pyx":316
  *     # free the line buffer, close the output, and free the output buffer
  *     stdlib.free(buffer)
  *     stdio.fclose(fout)             # <<<<<<<<<<<<<<
  *     stdlib.free(out_buf)
  * 
  */
   (void)(fclose(__pyx_v_fout));
 
-  /* "mrfifo/fast_loops.pyx":305
+  /* "mrfifo/fast_loops.pyx":317
  *     stdlib.free(buffer)
  *     stdio.fclose(fout)
  *     stdlib.free(out_buf)             # <<<<<<<<<<<<<<
  * 
  *     return n_out # total number of multiplexed lines (excluding header)
  */
   free(__pyx_v_out_buf);
 
-  /* "mrfifo/fast_loops.pyx":307
+  /* "mrfifo/fast_loops.pyx":319
  *     stdlib.free(out_buf)
  * 
  *     return n_out # total number of multiplexed lines (excluding header)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_n_out); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 307, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_n_out); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "mrfifo/fast_loops.pyx":210
+  /* "mrfifo/fast_loops.pyx":218
  * 
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
+ *             header_fifo="", _buffer_size=0, custom_header=None, int n_reopen_inputs=1, **kw):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("mrfifo.fast_loops.collect", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_sys);
   __Pyx_XDECREF(__pyx_v_header_bytes);
   __Pyx_XDECREF(__pyx_v_fifo_names);
   __Pyx_XDECREF(__pyx_v_header_fifo);
@@ -6067,14 +6256,15 @@
     {&__pyx_kp_b_CB_Z, __pyx_k_CB_Z, sizeof(__pyx_k_CB_Z), 0, 0, 0, 0},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 1},
     {&__pyx_n_s__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 0, 1, 1},
     {&__pyx_kp_u_as_substring_in, __pyx_k_as_substring_in, sizeof(__pyx_k_as_substring_in), 0, 1, 0, 0},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_buffer, __pyx_k_buffer, sizeof(__pyx_k_buffer), 0, 0, 1, 1},
+    {&__pyx_n_s_buffer_size, __pyx_k_buffer_size, sizeof(__pyx_k_buffer_size), 0, 0, 1, 1},
     {&__pyx_kp_u_can_not_find, __pyx_k_can_not_find, sizeof(__pyx_k_can_not_find), 0, 1, 0, 0},
     {&__pyx_n_s_chunk_size, __pyx_k_chunk_size, sizeof(__pyx_k_chunk_size), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_collect, __pyx_k_collect, sizeof(__pyx_k_collect), 0, 0, 1, 1},
     {&__pyx_n_s_custom_header, __pyx_k_custom_header, sizeof(__pyx_k_custom_header), 0, 0, 1, 1},
     {&__pyx_n_s_distribute, __pyx_k_distribute, sizeof(__pyx_k_distribute), 0, 0, 1, 1},
     {&__pyx_n_s_distribute_by_substr, __pyx_k_distribute_by_substr, sizeof(__pyx_k_distribute_by_substr), 0, 0, 1, 1},
@@ -6097,14 +6287,15 @@
     {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_in_buf_size, __pyx_k_in_buf_size, sizeof(__pyx_k_in_buf_size), 0, 0, 1, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
     {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
+    {&__pyx_n_s_kw, __pyx_k_kw, sizeof(__pyx_k_kw), 0, 0, 1, 1},
     {&__pyx_n_s_lead_n, __pyx_k_lead_n, sizeof(__pyx_k_lead_n), 0, 0, 1, 1},
     {&__pyx_n_s_line, __pyx_k_line, sizeof(__pyx_k_line), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_mrfifo_fast_loops, __pyx_k_mrfifo_fast_loops, sizeof(__pyx_k_mrfifo_fast_loops), 0, 0, 1, 1},
     {&__pyx_kp_s_mrfifo_fast_loops_pyx, __pyx_k_mrfifo_fast_loops_pyx, sizeof(__pyx_k_mrfifo_fast_loops_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
     {&__pyx_n_s_n_ins, __pyx_k_n_ins, sizeof(__pyx_k_n_ins), 0, 0, 1, 1},
@@ -6132,17 +6323,17 @@
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 32, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 41, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 193, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -6152,42 +6343,42 @@
   /* "mrfifo/fast_loops.pyx":10
  * from libc.string cimport strstr
  * 
  * def distribute(str fin_name, list fifo_names, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *                size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  *                header_detect_func=None, header_fifo="",
  */
-  __pyx_tuple__3 = PyTuple_Pack(20, __pyx_n_s_fin_name, __pyx_n_s_fifo_names, __pyx_n_s_chunk_size, __pyx_n_s_in_buf_size, __pyx_n_s_out_buf_size, __pyx_n_s_header_detect_func, __pyx_n_s_header_fifo, __pyx_n_s_header_broadcast, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_n_outs, __pyx_n_s_n, __pyx_n_s_line, __pyx_n_s_buffer, __pyx_n_s_n_read, __pyx_n_s_fifo_buffers, __pyx_n_s_fifos, __pyx_n_s_stdin_buf, __pyx_n_s_fin, __pyx_n_s_fheader); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(22, __pyx_n_s_fin_name, __pyx_n_s_fifo_names, __pyx_n_s_chunk_size, __pyx_n_s_in_buf_size, __pyx_n_s_out_buf_size, __pyx_n_s_header_detect_func, __pyx_n_s_header_fifo, __pyx_n_s_header_broadcast, __pyx_n_s_buffer_size, __pyx_n_s_kw, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_n_outs, __pyx_n_s_n, __pyx_n_s_line, __pyx_n_s_buffer, __pyx_n_s_n_read, __pyx_n_s_fifo_buffers, __pyx_n_s_fifos, __pyx_n_s_stdin_buf, __pyx_n_s_fin, __pyx_n_s_fheader); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(8, 0, 0, 20, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_mrfifo_fast_loops_pyx, __pyx_n_s_distribute, 10, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(9, 0, 0, 22, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_mrfifo_fast_loops_pyx, __pyx_n_s_distribute, 10, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 10, __pyx_L1_error)
 
-  /* "mrfifo/fast_loops.pyx":101
+  /* "mrfifo/fast_loops.pyx":105
  * 
  * 
  * def distribute_by_substr(str fin_name, list fifo_names, dict sub_lookup,             # <<<<<<<<<<<<<<
  *                          size_t sub_size, bytes sub_lead=b"\tCB:Z:",
  *                          size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  */
-  __pyx_tuple__5 = PyTuple_Pack(27, __pyx_n_s_fin_name, __pyx_n_s_fifo_names, __pyx_n_s_sub_lookup, __pyx_n_s_sub_size, __pyx_n_s_sub_lead, __pyx_n_s_in_buf_size, __pyx_n_s_out_buf_size, __pyx_n_s_header_detect_func, __pyx_n_s_header_fifo, __pyx_n_s_header_broadcast, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_n_outs, __pyx_n_s_n, __pyx_n_s_line, __pyx_n_s_buffer, __pyx_n_s_sub_lead_c, __pyx_n_s_lead_n, __pyx_n_s_sub_buffer, __pyx_n_s_sub_match_c, __pyx_n_s_sub, __pyx_n_s_n_read, __pyx_n_s_fifo_buffers, __pyx_n_s_fifos, __pyx_n_s_stdin_buf, __pyx_n_s_fin, __pyx_n_s_fheader); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(29, __pyx_n_s_fin_name, __pyx_n_s_fifo_names, __pyx_n_s_sub_lookup, __pyx_n_s_sub_size, __pyx_n_s_sub_lead, __pyx_n_s_in_buf_size, __pyx_n_s_out_buf_size, __pyx_n_s_header_detect_func, __pyx_n_s_header_fifo, __pyx_n_s_header_broadcast, __pyx_n_s_buffer_size, __pyx_n_s_kw, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_n_outs, __pyx_n_s_n, __pyx_n_s_line, __pyx_n_s_buffer, __pyx_n_s_sub_lead_c, __pyx_n_s_lead_n, __pyx_n_s_sub_buffer, __pyx_n_s_sub_match_c, __pyx_n_s_sub, __pyx_n_s_n_read, __pyx_n_s_fifo_buffers, __pyx_n_s_fifos, __pyx_n_s_stdin_buf, __pyx_n_s_fin, __pyx_n_s_fheader); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(10, 0, 0, 27, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_mrfifo_fast_loops_pyx, __pyx_n_s_distribute_by_substr, 101, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(11, 0, 0, 29, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_mrfifo_fast_loops_pyx, __pyx_n_s_distribute_by_substr, 105, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 105, __pyx_L1_error)
 
-  /* "mrfifo/fast_loops.pyx":210
+  /* "mrfifo/fast_loops.pyx":218
  * 
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
+ *             header_fifo="", _buffer_size=0, custom_header=None, int n_reopen_inputs=1, **kw):
  */
-  __pyx_tuple__7 = PyTuple_Pack(27, __pyx_n_s_fifo_names, __pyx_n_s_fout_name, __pyx_n_s_chunk_size, __pyx_n_s_in_buf_size, __pyx_n_s_out_buf_size, __pyx_n_s_header_fifo, __pyx_n_s_custom_header, __pyx_n_s_n_reopen_inputs, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_n_ins, __pyx_n_s_n, __pyx_n_s_n_out, __pyx_n_s_line, __pyx_n_s_buffer, __pyx_n_s_n_read, __pyx_n_s_fifo_buffers, __pyx_n_s_sys, __pyx_n_s_fifos, __pyx_n_s_fifo_closed, __pyx_n_s_drained_fifos, __pyx_n_s_n_loop, __pyx_n_s_out_buf, __pyx_n_s_fout, __pyx_n_s_header_bytes, __pyx_n_s_fheader); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(29, __pyx_n_s_fifo_names, __pyx_n_s_fout_name, __pyx_n_s_chunk_size, __pyx_n_s_in_buf_size, __pyx_n_s_out_buf_size, __pyx_n_s_header_fifo, __pyx_n_s_buffer_size, __pyx_n_s_custom_header, __pyx_n_s_n_reopen_inputs, __pyx_n_s_kw, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_n_ins, __pyx_n_s_n, __pyx_n_s_n_out, __pyx_n_s_line, __pyx_n_s_buffer, __pyx_n_s_n_read, __pyx_n_s_fifo_buffers, __pyx_n_s_sys, __pyx_n_s_fifos, __pyx_n_s_fifo_closed, __pyx_n_s_drained_fifos, __pyx_n_s_n_loop, __pyx_n_s_out_buf, __pyx_n_s_fout, __pyx_n_s_header_bytes, __pyx_n_s_fheader); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 218, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(8, 0, 0, 27, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_mrfifo_fast_loops_pyx, __pyx_n_s_collect, 210, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(9, 0, 0, 29, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_mrfifo_fast_loops_pyx, __pyx_n_s_collect, 218, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 218, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -6591,176 +6782,195 @@
   __Pyx_GOTREF(__pyx_t_3);
 
   /* "mrfifo/fast_loops.pyx":11
  * 
  * def distribute(str fin_name, list fifo_names, int chunk_size=10000,
  *                size_t in_buf_size=2**20, size_t out_buf_size=2**19,             # <<<<<<<<<<<<<<
  *                header_detect_func=None, header_fifo="",
- *                header_broadcast=False):
+ *                header_broadcast=False, size_t _buffer_size=0, **kw):
  */
   __pyx_t_2 = __Pyx_PyInt_FromSize_t(((size_t)0x100000)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __Pyx_PyInt_FromSize_t(((size_t)0x80000)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
+  /* "mrfifo/fast_loops.pyx":13
+ *                size_t in_buf_size=2**20, size_t out_buf_size=2**19,
+ *                header_detect_func=None, header_fifo="",
+ *                header_broadcast=False, size_t _buffer_size=0, **kw):             # <<<<<<<<<<<<<<
+ * 
+ *     if header_fifo == 0:
+ */
+  __pyx_t_5 = __Pyx_PyInt_FromSize_t(((size_t)0)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+
   /* "mrfifo/fast_loops.pyx":10
  * from libc.string cimport strstr
  * 
  * def distribute(str fin_name, list fifo_names, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *                size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  *                header_detect_func=None, header_fifo="",
  */
-  __pyx_t_5 = PyTuple_New(6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = PyTuple_New(7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 10, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 10, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4)) __PYX_ERR(0, 10, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_4)) __PYX_ERR(0, 10, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 3, Py_None)) __PYX_ERR(0, 10, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 3, Py_None)) __PYX_ERR(0, 10, __pyx_L1_error);
   __Pyx_INCREF(((PyObject*)__pyx_kp_u_));
   __Pyx_GIVEREF(((PyObject*)__pyx_kp_u_));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 4, ((PyObject*)__pyx_kp_u_))) __PYX_ERR(0, 10, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 4, ((PyObject*)__pyx_kp_u_))) __PYX_ERR(0, 10, __pyx_L1_error);
   __Pyx_INCREF(((PyObject *)Py_False));
   __Pyx_GIVEREF(((PyObject *)Py_False));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 5, ((PyObject *)Py_False))) __PYX_ERR(0, 10, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 5, ((PyObject *)Py_False))) __PYX_ERR(0, 10, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 6, __pyx_t_5)) __PYX_ERR(0, 10, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6mrfifo_10fast_loops_1distribute, 0, __pyx_n_s_distribute, NULL, __pyx_n_s_mrfifo_fast_loops, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6mrfifo_10fast_loops_1distribute, 0, __pyx_n_s_distribute, NULL, __pyx_n_s_mrfifo_fast_loops, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_t_6);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_distribute, __pyx_t_5) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_distribute, __pyx_t_4) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "mrfifo/fast_loops.pyx":103
+  /* "mrfifo/fast_loops.pyx":107
  * def distribute_by_substr(str fin_name, list fifo_names, dict sub_lookup,
  *                          size_t sub_size, bytes sub_lead=b"\tCB:Z:",
  *                          size_t in_buf_size=2**20, size_t out_buf_size=2**19,             # <<<<<<<<<<<<<<
  *                          header_detect_func=None, header_fifo="",
- *                          header_broadcast=False):
+ *                          header_broadcast=False, _buffer_size=0, **kw):
  */
-  __pyx_t_4 = __Pyx_PyInt_FromSize_t(((size_t)0x100000)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_FromSize_t(((size_t)0x80000)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_FromSize_t(((size_t)0x100000)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = __Pyx_PyInt_FromSize_t(((size_t)0x80000)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
 
-  /* "mrfifo/fast_loops.pyx":101
+  /* "mrfifo/fast_loops.pyx":105
  * 
  * 
  * def distribute_by_substr(str fin_name, list fifo_names, dict sub_lookup,             # <<<<<<<<<<<<<<
  *                          size_t sub_size, bytes sub_lead=b"\tCB:Z:",
  *                          size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  */
-  __pyx_t_2 = PyTuple_New(6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = PyTuple_New(7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(((PyObject*)__pyx_kp_b_CB_Z));
   __Pyx_GIVEREF(((PyObject*)__pyx_kp_b_CB_Z));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject*)__pyx_kp_b_CB_Z))) __PYX_ERR(0, 101, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject*)__pyx_kp_b_CB_Z))) __PYX_ERR(0, 105, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_6);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_6)) __PYX_ERR(0, 105, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 3, Py_None)) __PYX_ERR(0, 101, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 3, Py_None)) __PYX_ERR(0, 105, __pyx_L1_error);
   __Pyx_INCREF(((PyObject*)__pyx_kp_u_));
   __Pyx_GIVEREF(((PyObject*)__pyx_kp_u_));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 4, ((PyObject*)__pyx_kp_u_))) __PYX_ERR(0, 101, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 4, ((PyObject*)__pyx_kp_u_))) __PYX_ERR(0, 105, __pyx_L1_error);
   __Pyx_INCREF(((PyObject *)Py_False));
   __Pyx_GIVEREF(((PyObject *)Py_False));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 5, ((PyObject *)Py_False))) __PYX_ERR(0, 101, __pyx_L1_error);
-  __pyx_t_4 = 0;
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 5, ((PyObject *)Py_False))) __PYX_ERR(0, 105, __pyx_L1_error);
+  __Pyx_INCREF(((PyObject *)__pyx_int_0));
+  __Pyx_GIVEREF(((PyObject *)__pyx_int_0));
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 6, ((PyObject *)__pyx_int_0))) __PYX_ERR(0, 105, __pyx_L1_error);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6mrfifo_10fast_loops_3distribute_by_substr, 0, __pyx_n_s_distribute_by_substr, NULL, __pyx_n_s_mrfifo_fast_loops, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_distribute_by_substr, __pyx_t_5) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6mrfifo_10fast_loops_3distribute_by_substr, 0, __pyx_n_s_distribute_by_substr, NULL, __pyx_n_s_mrfifo_fast_loops, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_6, __pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_distribute_by_substr, __pyx_t_6) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "mrfifo/fast_loops.pyx":210
+  /* "mrfifo/fast_loops.pyx":218
  * 
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
+ *             header_fifo="", _buffer_size=0, custom_header=None, int n_reopen_inputs=1, **kw):
  */
-  __pyx_t_5 = __Pyx_PyInt_From_int(((int)0x2710)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = __Pyx_PyInt_From_int(((int)0x2710)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
 
-  /* "mrfifo/fast_loops.pyx":211
+  /* "mrfifo/fast_loops.pyx":219
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,             # <<<<<<<<<<<<<<
- *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
+ *             header_fifo="", _buffer_size=0, custom_header=None, int n_reopen_inputs=1, **kw):
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_FromSize_t(((size_t)0x80000)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_FromSize_t(((size_t)0x100000)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_FromSize_t(((size_t)0x80000)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyInt_FromSize_t(((size_t)0x100000)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 219, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
 
-  /* "mrfifo/fast_loops.pyx":212
+  /* "mrfifo/fast_loops.pyx":220
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None, int n_reopen_inputs=1):             # <<<<<<<<<<<<<<
+ *             header_fifo="", _buffer_size=0, custom_header=None, int n_reopen_inputs=1, **kw):             # <<<<<<<<<<<<<<
  * 
  *     if header_fifo == 0:
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(((int)1)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyInt_From_int(((int)1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
 
-  /* "mrfifo/fast_loops.pyx":210
+  /* "mrfifo/fast_loops.pyx":218
  * 
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
+ *             header_fifo="", _buffer_size=0, custom_header=None, int n_reopen_inputs=1, **kw):
  */
-  __pyx_t_6 = PyTuple_New(6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5)) __PYX_ERR(0, 210, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error);
+  __pyx_t_3 = PyTuple_New(7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_6);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6)) __PYX_ERR(0, 218, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error);
   __Pyx_INCREF(((PyObject*)__pyx_kp_u_));
   __Pyx_GIVEREF(((PyObject*)__pyx_kp_u_));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 3, ((PyObject*)__pyx_kp_u_))) __PYX_ERR(0, 210, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 3, ((PyObject*)__pyx_kp_u_))) __PYX_ERR(0, 218, __pyx_L1_error);
+  __Pyx_INCREF(((PyObject *)__pyx_int_0));
+  __Pyx_GIVEREF(((PyObject *)__pyx_int_0));
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 4, ((PyObject *)__pyx_int_0))) __PYX_ERR(0, 218, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 4, Py_None)) __PYX_ERR(0, 210, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 5, __pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 5, Py_None)) __PYX_ERR(0, 218, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 6, __pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error);
+  __pyx_t_6 = 0;
+  __pyx_t_4 = 0;
   __pyx_t_5 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_4 = 0;
-  __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6mrfifo_10fast_loops_5collect, 0, __pyx_n_s_collect, NULL, __pyx_n_s_mrfifo_fast_loops, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_6);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_collect, __pyx_t_3) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6mrfifo_10fast_loops_5collect, 0, __pyx_n_s_collect, NULL, __pyx_n_s_mrfifo_fast_loops, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_collect, __pyx_t_2) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "mrfifo/fast_loops.pyx":1
  * #cython: boundscheck=False, wraparound=False, initializedcheck=False, overflowcheck=False, cdivision=True             # <<<<<<<<<<<<<<
  * ###cython: boundscheck=True, wraparound=True, initializedcheck=True, overflowcheck=True, cdivision=False
  * #!python
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
```

### Comparing `mrfifo-0.6/mrfifo/fast_loops.pyx` & `mrfifo-0.7/mrfifo/fast_loops.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 from types import *
 from libc cimport stdlib, stdio
 from libc.string cimport strstr
 
 def distribute(str fin_name, list fifo_names, int chunk_size=10000, 
                size_t in_buf_size=2**20, size_t out_buf_size=2**19, 
                header_detect_func=None, header_fifo="", 
-               header_broadcast=False):
+               header_broadcast=False, size_t _buffer_size=0, **kw):
 
     if header_fifo == 0:
         # special mode: use the first fifo name for header data and the other
         # as round-robin outputs as usual
         header_fifo = fifo_names[0]
         fifo_names = fifo_names[1:]
 
+    if _buffer_size > 0:
+        in_buf_size = _buffer_size
+        out_buf_size = _buffer_size
+
     cdef size_t i = 0
     cdef size_t j = 0
     cdef size_t n_outs = len(fifo_names)
     cdef size_t n = 0
     cdef str line
     cdef char* buffer
     cdef ssize_t n_read = 0
@@ -97,23 +101,27 @@
 
     return n # number of lines distributed (excluding header)
 
 
 def distribute_by_substr(str fin_name, list fifo_names, dict sub_lookup,
                          size_t sub_size, bytes sub_lead=b"\tCB:Z:", 
                          size_t in_buf_size=2**20, size_t out_buf_size=2**19, 
-                         header_detect_func=None, header_fifo="", 
-                         header_broadcast=False):
+                         header_detect_func=None, header_fifo="",
+                         header_broadcast=False, _buffer_size=0, **kw):
 
     if header_fifo == 0:
         # special mode: use the first fifo name for header data and the other
         # as round-robin outputs as usual
         header_fifo = fifo_names[0]
         fifo_names = fifo_names[1:]
 
+    if _buffer_size > 0:
+        in_buf_size = _buffer_size
+        out_buf_size = _buffer_size
+
     cdef size_t i = 0
     cdef ssize_t j = 0
 
     cdef size_t n_outs = len(fifo_names)
     cdef size_t n = 0
     cdef str line
     cdef char* buffer
@@ -205,22 +213,26 @@
     stdlib.free(buffer)
 
     return n # number of lines distributed (excluding header)
 
 
 def collect(list fifo_names, str fout_name, int chunk_size=10000, 
             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
-            header_fifo="", custom_header=None, int n_reopen_inputs=1):
+            header_fifo="", _buffer_size=0, custom_header=None, int n_reopen_inputs=1, **kw):
 
     if header_fifo == 0:
         # special mode: use the first fifo name for header data 
         # and the other as round-robin inputs as usual
         header_fifo = fifo_names[0]
         fifo_names = fifo_names[1:]
 
+    if _buffer_size > 0:
+        in_buf_size = _buffer_size
+        out_buf_size = _buffer_size
+
     cdef int i = 0
     cdef int j = 0
     cdef int k = 0
     cdef size_t n_ins = len(fifo_names)
     cdef size_t n = 0
     cdef size_t n_out = 0
     cdef str line
```

### Comparing `mrfifo-0.6/mrfifo/parallel.py` & `mrfifo-0.7/mrfifo/parallel.py`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/mrfifo/parts.py` & `mrfifo-0.7/mrfifo/parts.py`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/mrfifo/util.py` & `mrfifo-0.7/mrfifo/util.py`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/mrfifo.egg-info/PKG-INFO` & `mrfifo-0.7/mrfifo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrfifo
-Version: 0.6
+Version: 0.7
 Summary: Map-Reduce parallelism over FIFOs (named pipes)
 Home-page: https://github.com/marvin-jens/mrfifo
 Author: Marvin Jens
 Author-email: marvin.jens@charite.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/marvin-jens/mrfifo/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mrfifo-0.6/mrfifo.egg-info/SOURCES.txt` & `mrfifo-0.7/mrfifo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/setup.cfg` & `mrfifo-0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/setup.py` & `mrfifo-0.7/setup.py`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/test_data/tiny_test.bam` & `mrfifo-0.7/test_data/tiny_test.bam`

 * *Files identical despite different names*

### Comparing `mrfifo-0.6/tests/test_cy.py` & `mrfifo-0.7/tests/test_cy.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
     assert w.result_dict["BAM_header_fifo.worker0"] == (0, 9)
     assert w.result_dict["BAM_header_fifo.worker1"] == (0, 9)
     assert w.result_dict["BAM_header_fifo.worker2"] == (0, 8)
     assert w.result_dict["BAM_header_fifo.worker3"] == (0, 8)
     assert w.result_dict["BAM_header_fifo.funnel0"] == (5, 0)
 
 
-def test_bam_reconstruct(chunk_size=1, n=4):
+def test_bam_reconstruct(chunk_size=1, n=64):
     w = (
         mf.Workflow("BAM_reconstruct")
         .BAM_reader(input="test_data/tiny_test.bam")
         .distribute(
             input=mf.FIFO("input_sam", "rt"),
             outputs=mf.FIFO("dist{n}", "wt", n=n),
             chunk_size=chunk_size,
@@ -482,11 +482,11 @@
     # test_dist()
     # test_dist_work_collect()
     # test_dist_work_funnel()
     # test_dist_work_funnel_count()
     # test_dist_work_collect_funnel()
     # test_header_broadcast()
     # test_header_fifo()
-    # test_bam_reconstruct()
+    test_bam_reconstruct()
     # test_fancy_counter()
     # test_BAM_creation()
-    test_iterate()
+    # test_iterate()
```

