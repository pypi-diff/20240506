# Comparing `tmp/sniffles-2.3.2.tar.gz` & `tmp/sniffles-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffles-2.3.2.tar", last modified: Wed Apr 10 23:43:28 2024, max compression
+gzip compressed data, was "sniffles-2.3.3.tar", last modified: Mon May  6 16:49:31 2024, max compression
```

## Comparing `sniffles-2.3.2.tar` & `sniffles-2.3.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:43:28.036682 sniffles-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 23:43:24.000000 sniffles-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-10 23:43:28.036682 sniffles-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-10 23:43:24.000000 sniffles-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 23:43:24.000000 sniffles-2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-10 23:43:28.036682 sniffles-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-10 23:43:24.000000 sniffles-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:43:28.028682 sniffles-2.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:43:28.032682 sniffles-2.3.2/src/sniffles/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/consensus.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25903 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/leadprov.py
--rw-r--r--   0 runner    (1001) docker     (127)    24149 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    17736 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/snf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21307 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/sniffles
--rwxr-xr-x   0 runner    (1001) docker     (127)    24081 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/sv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:43:28.036682 sniffles-2.3.2/src/sniffles/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/utils/resmon.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18412 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/vcf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:43:28.036682 sniffles-2.3.2/src/sniffles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-10 23:43:28.000000 sniffles-2.3.2/src/sniffles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-10 23:43:28.000000 sniffles-2.3.2/src/sniffles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:43:28.000000 sniffles-2.3.2/src/sniffles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-10 23:43:28.000000 sniffles-2.3.2/src/sniffles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 23:43:28.000000 sniffles-2.3.2/src/sniffles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:49:31.946817 sniffles-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-06 16:49:28.000000 sniffles-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-06 16:49:31.946817 sniffles-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-06 16:49:28.000000 sniffles-2.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 16:49:28.000000 sniffles-2.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-06 16:49:31.950817 sniffles-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-06 16:49:28.000000 sniffles-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:49:31.942817 sniffles-2.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:49:31.946817 sniffles-2.3.3/src/sniffles/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/consensus.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25903 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/leadprov.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24327 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17736 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/snf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21325 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/sniffles
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24081 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/sv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:49:31.946817 sniffles-2.3.3/src/sniffles/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/utils/resmon.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18412 2024-05-06 16:49:28.000000 sniffles-2.3.3/src/sniffles/vcf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:49:31.946817 sniffles-2.3.3/src/sniffles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-06 16:49:31.000000 sniffles-2.3.3/src/sniffles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-06 16:49:31.000000 sniffles-2.3.3/src/sniffles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:49:31.000000 sniffles-2.3.3/src/sniffles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 16:49:31.000000 sniffles-2.3.3/src/sniffles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 16:49:31.000000 sniffles-2.3.3/src/sniffles.egg-info/top_level.txt
```

### Comparing `sniffles-2.3.2/LICENSE` & `sniffles-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.2/PKG-INFO` & `sniffles-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffles
-Version: 2.3.2
+Version: 2.3.3
 Summary: A fast structural variation caller for long-read sequencing data
 Home-page: https://github.com/fritzsedlazeck/Sniffles
 Author: Moritz Smolka, Hermann Romanek
 Author-email: moritz.g.smolka@gmail.com, sniffles@romanek.at
 License: MIT
 Project-URL: Bug Tracker, https://github.com/fritzsedlazeck/Sniffles/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sniffles-2.3.2/README.md` & `sniffles-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.2/setup.cfg` & `sniffles-2.3.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sniffles
-version = 2.3.2
+version = 2.3.3
 author = Moritz Smolka, Hermann Romanek
 author_email = moritz.g.smolka@gmail.com, sniffles@romanek.at
 description = A fast structural variation caller for long-read sequencing data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fritzsedlazeck/Sniffles
 project_urls =
```

### Comparing `sniffles-2.3.2/src/sniffles/cluster.py` & `sniffles-2.3.3/src/sniffles/cluster.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.2/src/sniffles/config.py` & `sniffles-2.3.3/src/sniffles/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import argparse
 
 from typing import Union, Optional
 
 from sniffles import util
 
 VERSION = "Sniffles2"
-BUILD = "2.3.2"
+BUILD = "2.3.3"
 SNF_VERSION = "S2_rc4"
 
 
 class ArgFormatter(argparse.ArgumentDefaultsHelpFormatter, argparse.RawDescriptionHelpFormatter):
     pass
```

### Comparing `sniffles-2.3.2/src/sniffles/consensus.py` & `sniffles-2.3.3/src/sniffles/consensus.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.2/src/sniffles/leadprov.py` & `sniffles-2.3.3/src/sniffles/leadprov.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.2/src/sniffles/parallel.py` & `sniffles-2.3.3/src/sniffles/parallel.py`

 * *Files 5% similar despite different names*

```diff
@@ -444,23 +444,24 @@
     def __str__(self):
         return 'Shutdown Request'
 
     def execute(self) -> Result:
         raise SnifflesWorker.Shutdown
 
 
-class SnifflesWorker(threading.Thread):
+class SnifflesWorker:
     """
     Handle for a worker process. Since we're forking, this class will be available in
     both the parent and the worker processes.
     """
     id: int  # sequential ID of this worker, starting with 0 for the first
     externals: list = None
     recycle: bool = False
-    _running = False
+    running = True
+    pid: int = None
 
     class Shutdown(Exception):
         """
         Indicates this worker process should shut down
         """
 
     def __init__(self, process_id: int, config: Namespace, tasks: list[Task], recycle_hint: Union[bool, Callable] = None):
@@ -470,100 +471,108 @@
         self.task = None
         self.finished_tasks = []
         self.recycle = recycle_hint
 
         self.pipe_main, self.pipe_worker = multiprocessing.Pipe()
 
         self.process = multiprocessing.Process(
-            target=self.run_worker
+            target=self.run_worker,
+            daemon=True
         )
 
         self._logger = logging.getLogger('sniffles.worker')
 
-        super().__init__(target=self.run_parent)
+    def __str__(self):
+        return f'Worker {self.id} @ process {self.pid}'
 
     def start(self) -> None:
         self._logger.info(f'Starting worker {self.id}')
-        self._running = True
+        self.running = True
         self.process.start()
-        return super().start()
 
     def maybe_recycle(self):
         """
         Recycle this worker if that has been requested
         """
         recycle = self.recycle(self.id, self.process.pid) if callable(self.recycle) else self.recycle
 
         if recycle:
             self._logger.info(f'Recycling worker {self.id}')
             # Shut down current worker process
             self.pipe_main.send(ShutdownTask())
             self.process.join(2)
             # Start new one
             self.process = multiprocessing.Process(
-                target=self.run_worker
+                target=self.run_worker,
+                daemon=True
             )
             self.process.start()
 
-    def run_parent(self):
+    def run_parent(self) -> bool:
         """
         Worker thread, running in parent process
         """
         try:
-            while self._running:
-                if self.task is None:
-                    # we are not working on something...
-                    if len(self.tasks) > 0:
-                        # ...but there is more work to be done
-                        self.maybe_recycle()
-
-                        try:
-                            self.task = self.tasks.pop(0)
-                        except IndexError:
-                            # another worker may have taken the last task
-                            self._logger.debug(f'No more tasks to do for {self.id}')
-                        else:
-                            self.pipe_main.send(self.task)
-                            self._logger.info(f'Dispatched task #{self.task.id} to worker {self.id} ({len(self.tasks)}  tasks left)')
+            if self.task is None:
+                # we are not working on something...
+                if len(self.tasks) > 0:
+                    # ...but there is more work to be done
+                    self.maybe_recycle()
+
+                    try:
+                        self.task = self.tasks.pop(0)
+                    except IndexError:
+                        # another worker may have taken the last task
+                        self._logger.debug(f'No more tasks to do for {self.id}')
                     else:
-                        # ...and no more work available, so we shut down this worker
-                        self._logger.info(f'Worker {self.id} shutting down...')
-                        self.pipe_main.send(ShutdownTask())
-                        self._running = False
+                        self.pipe_main.send(self.task)
+                        self._logger.info(f'Dispatched task #{self.task.id} to worker {self.id} ({len(self.tasks)}  tasks left)')
                 else:
-                    if self.pipe_main.poll(0.01):
-                        self._logger.debug(f'Worker {self.id} got result for task {self.task.id}...')
-                        result: Result = self.pipe_main.recv()
-
-                        if result.error:
-                            self._logger.error(f'Worker {self.id} received error: {result}')
-                        else:
-                            self._logger.info(f'Worker {self.id} got result for task #{result.task_id}')
-
-                        self.task.add_result(result)
-                        self.finished_tasks.append(self.task)
-                        self.task = None
+                    # ...and no more work available, so we shut down this worker
+                    self._logger.info(f'Worker {self.id} shutting down...')
+                    self.pipe_main.send(ShutdownTask())
+                    self.running = False
+            else:
+                if self.pipe_main.poll(0.01):
+                    self._logger.debug(f'Worker {self.id} got result for task {self.task.id}...')
+                    result: Result = self.pipe_main.recv()
+
+                    if result.error:
+                        self._logger.error(f'Worker {self.id} received error: {result}')
+                    else:
+                        self._logger.info(f'Worker {self.id} got result for task #{result.task_id}')
 
-            self.process.join(10)
+                    self.task.add_result(result)
+                    self.finished_tasks.append(self.task)
+                    self.task = None
         except:
             self._logger.exception(f'Unhandled error in worker {self.id}. This may result in an orphened worker process.')
             try:
                 self.process.kill()
             except:
                 ...
-        else:
-            self._logger.info(f'Worker {self.id} done')
+
+        return self.running
+
+    def finalize(self):
+        self.process.join(10)
+
+        if self.process.exitcode is None:
+            self._logger.warning(f'Worker {self.id} refused to shut down gracefully, killing it.')
+            self.process.kill()
+            self.process.join(2)
+        self._logger.info(f'Worker {self.id} done (code {self.process.exitcode}).')
 
     def run_worker(self):
         """
         Entry point/main loop for the worker process
         """
         self.pid = os.getpid()
 
-        while self._running:
+        while self.running:
             try:
                 self._logger.debug(f'Worker {self.id} ({self.pid}) waiting for tasks...')
 
                 task = self.pipe_worker.recv()
 
                 self._logger.debug(f'Worker {self.id} got task {task.id}')
 
@@ -573,15 +582,15 @@
 
                 if result is not None:
                     self.pipe_worker.send(result)
 
                 del task
                 gc.collect()
             except self.Shutdown:
-                self._running = False
+                self.running = False
             except Exception as e:
                 self._logger.exception(f'Error in worker process')
                 self.pipe_worker.send(ErrorResult(e))
 
 
 def execute_task(task: Task):
     logging.getLogger('sniffles.parallel').info(f'Working on {task}')
```

### Comparing `sniffles-2.3.2/src/sniffles/postprocessing.py` & `sniffles-2.3.3/src/sniffles/postprocessing.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.2/src/sniffles/result.py` & `sniffles-2.3.3/src/sniffles/result.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.2/src/sniffles/snf.py` & `sniffles-2.3.3/src/sniffles/snf.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.2/src/sniffles/sniffles` & `sniffles-2.3.3/src/sniffles/sniffles`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,15 @@
             genotype_contig_svs[svcall.contig].append(svcall)
         rkwargs['genotype_lineindex_order'] = genotype_lineindex_order
         log.info(f"Opening for reading: {config.genotype_vcf} (read {len(genotype_lineindex_svs)} SVs to be genotyped)")
 
     #
     # Open output files
     #
+    vcf_out = None
     if config.vcf is not None:
 
         vcf_output_info = []
         if config.mode == "combine":
             vcf_output_info.append("multi-sample")
         else:
             vcf_output_info.append("single-sample")
@@ -410,17 +411,14 @@
     #
     for pnum in range(config.threads):
         processes.append(parallel.SnifflesWorker(process_id=pnum, config=config, tasks=tasks_list, recycle_hint=monitor))
 
     if config.vcf is not None and config.sort:
         task_id_calls = {}
 
-    for proc in processes:
-        proc.start()
-
     log.info("")
     if config.mode == "call_sample" or config.mode == "genotype_vcf":
         if config.input_is_cram:
             # CRAM file
             log.info(f"Analyzing alignments... (progress display disabled for CRAM input)")
         else:
             log.info(f"Analyzing {total_mapped} alignments total...")
@@ -429,18 +427,25 @@
     log.info("")
 
     #
     # Distribute analysis tasks to workers and collect results
     #
     analysis_start_time = time.time()
 
+    for p in processes:
+        p.start()
+
     finished_tasks: list[parallel.Task] = []
-    for proc in processes:
-        proc.join()
-        finished_tasks.extend(proc.finished_tasks)
+
+    while any([p.run_parent() for p in processes if p.running]):
+        time.sleep(0.1)
+
+    for p in processes:
+        p.finalize()
+        finished_tasks.extend(p.finished_tasks)
 
     log.info(f"Took {time.time() - analysis_start_time:.2f}s.")
     log.info("")
 
     finished_tasks.sort(key=lambda task: task.id)
 
     for t in finished_tasks:
@@ -506,15 +511,14 @@
         })
     except (ValueError, TypeError, AttributeError, ImportError):
         logging.exception(f'Error configuring loggers.')
 
     try:
         Sniffles2_Main(processes)
     except (util.Sniffles2Exit, SystemExit) as exit_code:
-        # print(f'Sniffles exit with code {exit_code}')
         if len(processes):
             # Allow time for child process error messages to propagate
             print("Sniffles2Main: Shutting down workers")
             time.sleep(10)
         for proc in processes:
             try:
                 proc.process.terminate()
@@ -522,11 +526,11 @@
                 pass
 
         for proc in processes:
             try:
                 proc.process.join()
             except:
                 pass
-        int_exit_code = exit_code.args[0]
-        exit(int_exit_code)
+        exit(exit_code.code)
     except:
         logging.getLogger('sniffles.main').exception(f'Unhandled error while running sniffles.')
+        exit(1)
```

### Comparing `sniffles-2.3.2/src/sniffles/sv.py` & `sniffles-2.3.3/src/sniffles/sv.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.2/src/sniffles/util.py` & `sniffles-2.3.3/src/sniffles/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import statistics
 import sys
 import time
 
 
 class Sniffles2Exit(Exception):
-    pass
+    code: int = 1
 
 
 def stdev(nums):
     nums = list(nums)
     return statistics.stdev(nums) if len(nums) > 1 else 0
```

### Comparing `sniffles-2.3.2/src/sniffles/utils/resmon.py` & `sniffles-2.3.3/src/sniffles/utils/resmon.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,17 +44,18 @@
 
         self._slots = config.threads
         self._update_interval = config.dev_monitor_memory or 30.0
         self._pid = os.getpid()
 
         try:
             from psutil import Process
-        except ImportError as ex:
+        except ImportError:
             logging.getLogger('sniffles.dependencies').warning(f'Dependency psutil not available - resource monitoring is disabled.')
             self._process = None
+            self._workers = {}
         else:
             self._process = Process(self._pid)
 
             self._running = True
 
             if config.dev_monitor_memory:
                 self._filename = filename = f'memory-{config.run_id}.csv'
```

### Comparing `sniffles-2.3.2/src/sniffles/vcf.py` & `sniffles-2.3.3/src/sniffles/vcf.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.2/src/sniffles.egg-info/PKG-INFO` & `sniffles-2.3.3/src/sniffles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffles
-Version: 2.3.2
+Version: 2.3.3
 Summary: A fast structural variation caller for long-read sequencing data
 Home-page: https://github.com/fritzsedlazeck/Sniffles
 Author: Moritz Smolka, Hermann Romanek
 Author-email: moritz.g.smolka@gmail.com, sniffles@romanek.at
 License: MIT
 Project-URL: Bug Tracker, https://github.com/fritzsedlazeck/Sniffles/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sniffles-2.3.2/src/sniffles.egg-info/SOURCES.txt` & `sniffles-2.3.3/src/sniffles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

