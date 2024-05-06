# Comparing `tmp/pbs4py-1.0.4.tar.gz` & `tmp/pbs4py-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbs4py-1.0.4.tar", last modified: Wed Mar  8 02:37:27 2023, max compression
+gzip compressed data, was "pbs4py-1.0.5.tar", last modified: Mon May  6 21:01:54 2024, max compression
```

## Comparing `pbs4py-1.0.4.tar` & `pbs4py-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kejacob1   (502) staff       (20)        0 2023-03-08 02:37:27.267102 pbs4py-1.0.4/
--rw-r--r--   0 kejacob1   (502) staff       (20)    14075 2022-09-19 20:10:01.000000 pbs4py-1.0.4/LICENSE
--rw-r--r--   0 kejacob1   (502) staff       (20)     4127 2023-03-08 02:37:27.266960 pbs4py-1.0.4/PKG-INFO
--rw-r--r--   0 kejacob1   (502) staff       (20)     3895 2023-03-08 02:36:38.000000 pbs4py-1.0.4/README.md
-drwxr-xr-x   0 kejacob1   (502) staff       (20)        0 2023-03-08 02:37:27.265623 pbs4py-1.0.4/pbs4py/
--rw-r--r--   0 kejacob1   (502) staff       (20)       93 2023-03-08 02:36:38.000000 pbs4py-1.0.4/pbs4py/__init__.py
--rw-r--r--   0 kejacob1   (502) staff       (20)     3717 2023-03-08 02:36:38.000000 pbs4py-1.0.4/pbs4py/bsub.py
--rw-r--r--   0 kejacob1   (502) staff       (20)      373 2023-03-08 02:36:38.000000 pbs4py-1.0.4/pbs4py/directory_utils.py
--rw-r--r--   0 kejacob1   (502) staff       (20)     1635 2023-03-08 02:36:38.000000 pbs4py-1.0.4/pbs4py/fake_pbs.py
--rw-r--r--   0 kejacob1   (502) staff       (20)     6024 2023-03-08 02:36:38.000000 pbs4py-1.0.4/pbs4py/job.py
--rw-r--r--   0 kejacob1   (502) staff       (20)     4971 2023-03-08 02:36:38.000000 pbs4py-1.0.4/pbs4py/launcher_base.py
--rw-r--r--   0 kejacob1   (502) staff       (20)    14091 2023-03-08 02:36:38.000000 pbs4py-1.0.4/pbs4py/pbs.py
--rw-r--r--   0 kejacob1   (502) staff       (20)     6698 2023-03-08 02:36:38.000000 pbs4py-1.0.4/pbs4py/pbs_batch.py
-drwxr-xr-x   0 kejacob1   (502) staff       (20)        0 2023-03-08 02:37:27.266771 pbs4py-1.0.4/pbs4py/scripts/
--rwxr-xr-x   0 kejacob1   (502) staff       (20)      555 2023-03-08 02:36:38.000000 pbs4py-1.0.4/pbs4py/scripts/job_dir.py
--rwxr-xr-x   0 kejacob1   (502) staff       (20)     4075 2023-03-08 02:36:38.000000 pbs4py-1.0.4/pbs4py/scripts/qdel_user_jobs.py
-drwxr-xr-x   0 kejacob1   (502) staff       (20)        0 2023-03-08 02:37:27.266516 pbs4py-1.0.4/pbs4py.egg-info/
--rw-r--r--   0 kejacob1   (502) staff       (20)     4127 2023-03-08 02:37:27.000000 pbs4py-1.0.4/pbs4py.egg-info/PKG-INFO
--rw-r--r--   0 kejacob1   (502) staff       (20)      414 2023-03-08 02:37:27.000000 pbs4py-1.0.4/pbs4py.egg-info/SOURCES.txt
--rw-r--r--   0 kejacob1   (502) staff       (20)        1 2023-03-08 02:37:27.000000 pbs4py-1.0.4/pbs4py.egg-info/dependency_links.txt
--rw-r--r--   0 kejacob1   (502) staff       (20)        1 2022-07-28 13:50:12.000000 pbs4py-1.0.4/pbs4py.egg-info/not-zip-safe
--rw-r--r--   0 kejacob1   (502) staff       (20)        6 2023-03-08 02:37:27.000000 pbs4py-1.0.4/pbs4py.egg-info/requires.txt
--rw-r--r--   0 kejacob1   (502) staff       (20)        7 2023-03-08 02:37:27.000000 pbs4py-1.0.4/pbs4py.egg-info/top_level.txt
--rw-r--r--   0 kejacob1   (502) staff       (20)       38 2023-03-08 02:37:27.267142 pbs4py-1.0.4/setup.cfg
--rwxr-xr-x   0 kejacob1   (502) staff       (20)     3045 2023-03-08 02:36:38.000000 pbs4py-1.0.4/setup.py
+drwxr-xr-x   0 kejacob1   (502) staff       (20)        0 2024-05-06 21:01:54.039811 pbs4py-1.0.5/
+-rw-r--r--   0 kejacob1   (502) staff       (20)    14075 2022-09-19 20:10:01.000000 pbs4py-1.0.5/LICENSE
+-rw-r--r--   0 kejacob1   (502) staff       (20)     4127 2024-05-06 21:01:54.039682 pbs4py-1.0.5/PKG-INFO
+-rw-r--r--   0 kejacob1   (502) staff       (20)     3895 2023-03-08 15:31:52.000000 pbs4py-1.0.5/README.md
+drwxr-xr-x   0 kejacob1   (502) staff       (20)        0 2024-05-06 21:01:54.038059 pbs4py-1.0.5/pbs4py/
+-rw-r--r--   0 kejacob1   (502) staff       (20)       93 2023-03-08 15:31:52.000000 pbs4py-1.0.5/pbs4py/__init__.py
+-rw-r--r--   0 kejacob1   (502) staff       (20)     3717 2023-03-08 15:31:52.000000 pbs4py-1.0.5/pbs4py/bsub.py
+-rw-r--r--   0 kejacob1   (502) staff       (20)      373 2023-03-08 15:31:52.000000 pbs4py-1.0.5/pbs4py/directory_utils.py
+-rw-r--r--   0 kejacob1   (502) staff       (20)     1635 2023-03-08 15:31:52.000000 pbs4py-1.0.5/pbs4py/fake_pbs.py
+-rw-r--r--   0 kejacob1   (502) staff       (20)     6791 2023-06-30 11:50:10.000000 pbs4py-1.0.5/pbs4py/job.py
+-rw-r--r--   0 kejacob1   (502) staff       (20)     4971 2023-03-08 15:31:52.000000 pbs4py-1.0.5/pbs4py/launcher_base.py
+-rw-r--r--   0 kejacob1   (502) staff       (20)    14068 2023-07-25 15:24:52.000000 pbs4py-1.0.5/pbs4py/pbs.py
+-rw-r--r--   0 kejacob1   (502) staff       (20)     6698 2023-03-08 15:31:52.000000 pbs4py-1.0.5/pbs4py/pbs_batch.py
+drwxr-xr-x   0 kejacob1   (502) staff       (20)        0 2024-05-06 21:01:54.039476 pbs4py-1.0.5/pbs4py/scripts/
+-rwxr-xr-x   0 kejacob1   (502) staff       (20)      555 2023-03-08 15:31:52.000000 pbs4py-1.0.5/pbs4py/scripts/job_dir.py
+-rwxr-xr-x   0 kejacob1   (502) staff       (20)     4080 2023-07-25 15:24:52.000000 pbs4py-1.0.5/pbs4py/scripts/qdel_user_jobs.py
+drwxr-xr-x   0 kejacob1   (502) staff       (20)        0 2024-05-06 21:01:54.039156 pbs4py-1.0.5/pbs4py.egg-info/
+-rw-r--r--   0 kejacob1   (502) staff       (20)     4127 2024-05-06 21:01:53.000000 pbs4py-1.0.5/pbs4py.egg-info/PKG-INFO
+-rw-r--r--   0 kejacob1   (502) staff       (20)      414 2024-05-06 21:01:54.000000 pbs4py-1.0.5/pbs4py.egg-info/SOURCES.txt
+-rw-r--r--   0 kejacob1   (502) staff       (20)        1 2024-05-06 21:01:53.000000 pbs4py-1.0.5/pbs4py.egg-info/dependency_links.txt
+-rw-r--r--   0 kejacob1   (502) staff       (20)        1 2022-07-28 13:50:12.000000 pbs4py-1.0.5/pbs4py.egg-info/not-zip-safe
+-rw-r--r--   0 kejacob1   (502) staff       (20)        6 2024-05-06 21:01:53.000000 pbs4py-1.0.5/pbs4py.egg-info/requires.txt
+-rw-r--r--   0 kejacob1   (502) staff       (20)        7 2024-05-06 21:01:53.000000 pbs4py-1.0.5/pbs4py.egg-info/top_level.txt
+-rw-r--r--   0 kejacob1   (502) staff       (20)       38 2024-05-06 21:01:54.039853 pbs4py-1.0.5/setup.cfg
+-rwxr-xr-x   0 kejacob1   (502) staff       (20)     3034 2024-05-06 20:58:47.000000 pbs4py-1.0.5/setup.py
```

### Comparing `pbs4py-1.0.4/LICENSE` & `pbs4py-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pbs4py-1.0.4/PKG-INFO` & `pbs4py-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbs4py
-Version: 1.0.4
+Version: 1.0.5
 Summary: PBS scripting utilities
 Author: Kevin Jacobson
 Author-email: kevin.e.jacobson@nasa.gov
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pbs4py-1.0.4/README.md` & `pbs4py-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pbs4py-1.0.4/pbs4py/bsub.py` & `pbs4py-1.0.5/pbs4py/bsub.py`

 * *Files identical despite different names*

### Comparing `pbs4py-1.0.4/pbs4py/fake_pbs.py` & `pbs4py-1.0.5/pbs4py/fake_pbs.py`

 * *Files identical despite different names*

### Comparing `pbs4py-1.0.4/pbs4py/job.py` & `pbs4py-1.0.5/pbs4py/job.py`

 * *Files 17% similar despite different names*

```diff
@@ -155,14 +155,28 @@
             self.model = ''
         self.requested_number_of_nodes = int(qstat_dict['Resource_List.select'].split(':')[0])
         self.ncpus_per_node = int(
             qstat_dict['Resource_List.select'].split('ncpus=')[-1].split(':')[0])
 
         self.exit_status: int = qstat_dict.get('Exit_status')
 
+        self.walltime_requested = self._convert_walltime_to_seconds(qstat_dict['Resource_List.walltime'])
+        if self.state!='Q':
+            self.hostname = qstat_dict['exec_host'].split('/')[0]
+            self.walltime_used = qstat_dict.get('resources_used.walltime')
+            if self.walltime_used is not None:
+                self.walltime_used = self._convert_walltime_to_seconds(self.walltime_used)
+                self.walltime_remaining = self.walltime_requested - self.walltime_used
+            else:
+                self.walltime_remaining = None
+
+    def _convert_walltime_to_seconds(self, walltime: str):
+        walltime_split = walltime.split(':')
+        return 3600*int(walltime_split[0]) + 60*int(walltime_split[1]) + int(walltime_split[2])
+
     def _set_empty_attributes(self):
         self.name = ''
         self.model = ''
         self.queue = ''
         self.state = ''
         self.workdir = ''
         self.requested_number_of_nodes = 0
```

### Comparing `pbs4py-1.0.4/pbs4py/launcher_base.py` & `pbs4py-1.0.5/pbs4py/launcher_base.py`

 * *Files identical despite different names*

### Comparing `pbs4py-1.0.4/pbs4py/pbs.py` & `pbs4py-1.0.5/pbs4py/pbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,27 +272,27 @@
             The file setting the environment to source inside the PBS job
         """
         return cls(queue_name='K4-route', ncpus_per_node=40,
                    queue_node_limit=16, time=time,
                    profile_file=profile_file)
 
     @classmethod
-    def k3(cls, time: int = 72, profile_file: str = '~/.bashrc'):
+    def k3b(cls, time: int = 72, profile_file: str = '~/.bashrc'):
         """
-        Constructor for the K3 queues on LaRC's K cluster including K3-standard-512.
+        Constructor for the K3b queues on LaRC's K cluster.
 
         Parameters
         ----------
         time:
             The requested job walltime in hours
         profile_file:
             The file setting the environment to source inside the PBS job
         """
-        return cls(queue_name='K3-route', ncpus_per_node=16,
-                   queue_node_limit=40, time=time,
+        return cls(queue_name='K3b-route', ncpus_per_node=28,
+                   queue_node_limit=74, time=time,
                    profile_file=profile_file)
 
     @classmethod
     def k3a(cls, time: int = 72, profile_file: str = '~/.bashrc'):
         """
         Constructor for the K3a queue on LaRC's K cluster.
```

### Comparing `pbs4py-1.0.4/pbs4py/pbs_batch.py` & `pbs4py-1.0.5/pbs4py/pbs_batch.py`

 * *Files identical despite different names*

### Comparing `pbs4py-1.0.4/pbs4py/scripts/job_dir.py` & `pbs4py-1.0.5/pbs4py/scripts/job_dir.py`

 * *Files identical despite different names*

### Comparing `pbs4py-1.0.4/pbs4py/scripts/qdel_user_jobs.py` & `pbs4py-1.0.5/pbs4py/scripts/qdel_user_jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     # remove header from qstat command
     qstat_output = qstat_output[3:]
 
     jobs = []
     for line in qstat_output:
         if line:
             id = int(re.match('\s*[0-9]+', line)[0])
-            jobs.append(PBSJob(id))
+            jobs.append(PBSJob(str(id)))
     return jobs
 
 
 def filter_jobs_to_delete_by_id_range(user_jobs: List[PBSJob], min_id: int, max_id: int):
     return [job for job in user_jobs if (job.id >= min_id and job.id <= max_id)]
```

### Comparing `pbs4py-1.0.4/pbs4py.egg-info/PKG-INFO` & `pbs4py-1.0.5/pbs4py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbs4py
-Version: 1.0.4
+Version: 1.0.5
 Summary: PBS scripting utilities
 Author: Kevin Jacobson
 Author-email: kevin.e.jacobson@nasa.gov
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pbs4py-1.0.4/setup.py` & `pbs4py-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,33 +33,33 @@
 LIABILITIES, DEMANDS, DAMAGES, EXPENSES OR LOSSES ARISING FROM SUCH USE,
 INCLUDING ANY DAMAGES FROM PRODUCTS BASED ON, OR RESULTING FROM, RECIPIENT'S USE
 OF THE SUBJECT SOFTWARE, RECIPIENT SHALL INDEMNIFY AND HOLD HARMLESS THE UNITED
 STATES GOVERNMENT, ITS CONTRACTORS AND SUBCONTRACTORS, AS WELL AS ANY PRIOR
 RECIPIENT, TO THE EXTENT PERMITTED BY LAW.  RECIPIENT'S SOLE REMEDY FOR ANY SUCH
  MATTER SHALL BE THE IMMEDIATE, UNILATERAL TERMINATION OF THIS AGREEMENT.
 """
+
 import os
 from setuptools import setup, find_packages
 
 
 __package_name__ = "pbs4py"
-__package_version__ = "1.0.4"
+__package_version__ = "1.0.5"
 
 root = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(root, 'README.md'), encoding='utf-8') as f:
+with open(os.path.join(root, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name=__package_name__,
     version=__package_version__,
     description=("PBS scripting utilities"),
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author="Kevin Jacobson",
     author_email="kevin.e.jacobson@nasa.gov",
     zip_safe=False,
     packages=find_packages(),
-    scripts=['pbs4py/scripts/qdel_user_jobs.py',
-             'pbs4py/scripts/job_dir.py'],
-    install_requires=['numpy'],
-    python_requires='>=3.6'
+    scripts=["pbs4py/scripts/qdel_user_jobs.py", "pbs4py/scripts/job_dir.py"],
+    install_requires=["numpy"],
+    python_requires=">=3.6",
 )
```

