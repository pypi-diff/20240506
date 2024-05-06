# Comparing `tmp/com.castsoftware.uc.oneclick-1.0.3.tar.gz` & `tmp/com_castsoftware_uc_oneclick-1.0.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.oneclick-1.0.3.tar", last modified: Fri Dec 15 15:51:01 2023, max compression
+gzip compressed data, was "com_castsoftware_uc_oneclick-1.0.4b1.tar", last modified: Mon May  6 15:56:57 2024, max compression
```

## Comparing `com.castsoftware.uc.oneclick-1.0.3.tar` & `com_castsoftware_uc_oneclick-1.0.4b1.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-12-15 15:51:01.226233 com.castsoftware.uc.oneclick-1.0.3/
--rw-rw-rw-   0        0        0      981 2023-12-15 15:51:01.210219 com.castsoftware.uc.oneclick-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-12-15 15:51:01.198568 com.castsoftware.uc.oneclick-1.0.3/com.castsoftware.uc.oneclick.egg-info/
--rw-rw-rw-   0        0        0      981 2023-12-15 15:51:00.000000 com.castsoftware.uc.oneclick-1.0.3/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      884 2023-12-15 15:51:00.000000 com.castsoftware.uc.oneclick-1.0.3/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-15 15:51:00.000000 com.castsoftware.uc.oneclick-1.0.3/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      226 2023-12-15 15:51:00.000000 com.castsoftware.uc.oneclick-1.0.3/com.castsoftware.uc.oneclick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-12-15 15:51:00.000000 com.castsoftware.uc.oneclick-1.0.3/com.castsoftware.uc.oneclick.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-15 15:51:00.976927 com.castsoftware.uc.oneclick-1.0.3/oneclick/
--rw-rw-rw-   0        0        0        2 2023-10-05 21:09:34.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-15 15:51:01.033975 com.castsoftware.uc.oneclick-1.0.3/oneclick/analysis/
--rw-rw-rw-   0        0        0        0 2023-10-05 21:09:34.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/analysis/__init__.py
--rw-rw-rw-   0        0        0     2745 2023-10-05 21:09:34.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/analysis/aip_analysis.py
--rw-rw-rw-   0        0        0     1231 2023-10-05 21:09:34.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/analysis/analysis.py
--rw-rw-rw-   0        0        0     4053 2023-12-04 17:27:52.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/analysis/highlight_analysis.py
--rw-rw-rw-   0        0        0     4706 2023-10-05 21:09:34.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/analysis/trackAnalysis.py
--rw-rw-rw-   0        0        0    26771 2023-12-15 14:17:18.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/config.py
-drwxrwxrwx   0        0        0        0 2023-12-15 15:51:01.182613 com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/
--rw-rw-rw-   0        0        0        0 2023-10-05 21:09:34.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/__init__.py
--rw-rw-rw-   0        0        0     4557 2023-10-05 21:09:34.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/cleanup.py
--rw-rw-rw-   0        0        0    10362 2023-10-05 21:09:34.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/cloc.py
--rw-rw-rw-   0        0        0     9700 2023-12-15 15:01:13.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/discoveryReport.py
--rw-rw-rw-   0        0        0     2957 2023-10-05 21:09:34.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/prep.py
--rw-rw-rw-   0        0        0     4932 2023-12-15 14:22:07.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/profiler.py
--rw-rw-rw-   0        0        0      421 2023-12-04 17:27:52.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/sourceValidation.py
--rw-rw-rw-   0        0        0     5649 2023-12-04 17:27:52.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/sqlDiscovery.py
--rw-rw-rw-   0        0        0     4803 2023-12-04 17:27:52.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/unzip.py
--rw-rw-rw-   0        0        0      305 2023-10-05 21:09:34.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/exceptions.py
--rw-rw-rw-   0        0        0    11234 2023-12-04 17:27:52.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/main.py
--rw-rw-rw-   0        0        0     2152 2023-10-05 21:09:34.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/runArg.py
--rw-rw-rw-   0        0        0     2098 2023-10-05 21:09:34.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/sendEmail.py
--rw-rw-rw-   0        0        0     6440 2023-12-14 16:41:10.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/setup.py
--rw-rw-rw-   0        0        0     2600 2023-10-19 19:41:27.000000 com.castsoftware.uc.oneclick-1.0.3/oneclick/test.py
--rw-rw-rw-   0        0        0      831 2023-12-15 15:50:35.000000 com.castsoftware.uc.oneclick-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-12-15 15:51:01.226233 com.castsoftware.uc.oneclick-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 15:56:57.189332 com_castsoftware_uc_oneclick-1.0.4b1/
+-rw-rw-rw-   0        0        0      984 2024-05-06 15:56:57.169062 com_castsoftware_uc_oneclick-1.0.4b1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 15:56:57.151024 com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/
+-rw-rw-rw-   0        0        0      984 2024-05-06 15:56:56.000000 com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      867 2024-05-06 15:56:56.000000 com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 15:56:56.000000 com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      227 2024-05-06 15:56:56.000000 com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 15:56:56.000000 com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 15:56:56.881462 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/
+-rw-rw-rw-   0        0        0        2 2024-02-13 17:42:06.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:56:56.949232 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/
+-rw-rw-rw-   0        0        0        0 2024-02-13 17:42:06.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2970 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/aip_analysis.py
+-rw-rw-rw-   0        0        0     1308 2024-02-22 13:23:04.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/analysis.py
+-rw-rw-rw-   0        0        0     4288 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/highlight_analysis.py
+-rw-rw-rw-   0        0        0     4964 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/trackAnalysis.py
+-rw-rw-rw-   0        0        0    26252 2024-04-24 21:10:55.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/config.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:56:57.131412 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/
+-rw-rw-rw-   0        0        0        0 2024-02-13 17:42:06.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/__init__.py
+-rw-rw-rw-   0        0        0     4907 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/cleanup.py
+-rw-rw-rw-   0        0        0    10901 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/cloc.py
+-rw-rw-rw-   0        0        0     9689 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/discoveryReport.py
+-rw-rw-rw-   0        0        0     3853 2024-04-24 21:29:48.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/prep.py
+-rw-rw-rw-   0        0        0     4746 2024-02-13 17:42:06.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/profiler.py
+-rw-rw-rw-   0        0        0      498 2024-02-22 13:23:04.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/sourceValidation.py
+-rw-rw-rw-   0        0        0     7069 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/sqlDiscovery.py
+-rw-rw-rw-   0        0        0     5753 2024-04-24 18:58:40.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/unzip.py
+-rw-rw-rw-   0        0        0      305 2024-02-13 17:42:07.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/exceptions.py
+-rw-rw-rw-   0        0        0    11405 2024-04-24 21:36:38.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/main.py
+-rw-rw-rw-   0        0        0     2225 2024-02-22 13:23:04.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/runArg.py
+-rw-rw-rw-   0        0        0     2098 2024-02-13 17:42:07.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/sendEmail.py
+-rw-rw-rw-   0        0        0     4251 2024-02-13 17:42:07.000000 com_castsoftware_uc_oneclick-1.0.4b1/oneclick/setup.py
+-rw-rw-rw-   0        0        0      839 2024-05-06 15:51:04.000000 com_castsoftware_uc_oneclick-1.0.4b1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 15:56:57.189332 com_castsoftware_uc_oneclick-1.0.4b1/setup.cfg
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/PKG-INFO` & `com_castsoftware_uc_oneclick-1.0.4b1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 1.0.3
+Version: 1.0.4b1
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -17,10 +17,10 @@
 Requires-Dist: pyunpack
 Requires-Dist: tqdm
 Requires-Dist: patool
 Requires-Dist: archive
 Requires-Dist: pypiwin32
 Requires-Dist: psycopg2
 Requires-Dist: openpyxl
-Requires-Dist: com.castsoftware.uc.python.common>=1.1.6
+Requires-Dist: com.castsoftware.uc.python.common>=1.1.11
 Requires-Dist: com.castsoftware.uc.action-plan
-Requires-Dist: com.castsoftware.uc.arg>=1.6.8
+Requires-Dist: com.castsoftware.uc.arg>=1.6.2
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/com.castsoftware.uc.oneclick.egg-info/PKG-INFO` & `com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 1.0.3
+Version: 1.0.4b1
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -17,10 +17,10 @@
 Requires-Dist: pyunpack
 Requires-Dist: tqdm
 Requires-Dist: patool
 Requires-Dist: archive
 Requires-Dist: pypiwin32
 Requires-Dist: psycopg2
 Requires-Dist: openpyxl
-Requires-Dist: com.castsoftware.uc.python.common>=1.1.6
+Requires-Dist: com.castsoftware.uc.python.common>=1.1.11
 Requires-Dist: com.castsoftware.uc.action-plan
-Requires-Dist: com.castsoftware.uc.arg>=1.6.8
+Requires-Dist: com.castsoftware.uc.arg>=1.6.2
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt` & `com_castsoftware_uc_oneclick-1.0.4b1/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 oneclick/__init__.py
 oneclick/config.py
 oneclick/exceptions.py
 oneclick/main.py
 oneclick/runArg.py
 oneclick/sendEmail.py
 oneclick/setup.py
-oneclick/test.py
 oneclick/analysis/__init__.py
 oneclick/analysis/aip_analysis.py
 oneclick/analysis/analysis.py
 oneclick/analysis/highlight_analysis.py
 oneclick/analysis/trackAnalysis.py
 oneclick/discovery/__init__.py
 oneclick/discovery/cleanup.py
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/analysis/aip_analysis.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/aip_analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 class AIPAnalysis(Analysis):
 
     def __init__(cls, log_level:int):
         super().__init__(cls.__class__.__name__,log_level)
         pass
     
     def run(cls, config:Config):
+        cls._log.info(f'You can use oneclick to directly run AIP or HL or both analysis using command :- oneclick run -p <project name> --start=Analysis')
         if not config.is_console_active:
             cls._log.warning('AIP Console configuration is incomplete, analysis will not run')
             return 0
 
         for appl in config.application:
 
             #has thi spplication already been run?
             aip_status = config.application[appl]['aip']
             if aip_status == '' or aip_status.startswith('Error'):
                 #add a new appication in AIP Console
-                cls._log.info(f'Running analysis for {config.project_name}\{appl}')
+                # cls._log.info(f'Running analysis for {config.project_name}\{appl}')
+                cls._log.info(f'Running AIP analysis for {appl}')
 
                 java_home = config.java_home
                 if len(java_home) > 0:
                     java_home = f'{java_home}'
 
                 node_name = ""
                 if len(config.console_node) > 0:
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/analysis/analysis.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,17 @@
         cls._pid.append(Process(process,operation,name))
         pass
 
     def check_process(cls,pid:int)->Popen:
         info = cls._pid[str(pid)]
         process = info['process']
         return process.poll()
+    
+    def get_title(cls) -> str:
+        return cls.__class__.__name__
 
 
 class Process():
     def __init__(cls,process:Popen,operation:str,name:str):
         cls._process = process
         cls._operation = operation
         cls._name = name
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/analysis/highlight_analysis.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/highlight_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 class HLAnalysis(Analysis):
 
     def __init__(cls, log_level:int):
         super().__init__(cls.__class__.__name__,log_level)
         pass
 
     def run(cls, config:Config):
+        cls._log.info(f'You can use oneclick to directly run AIP or HL or both analysis using command :- oneclick run -p <project name> --start=Analysis')
         if not config.is_hl_active:
             cls._log.warning('Highlight configuration is incomplete, analysis will not run')
             return 0
         
         rest = HLRestCall(hl_base_url=config.hl_url,hl_user=config.hl_user,hl_pswd=config.hl_password,hl_instance=config.hl_instance)
 
         try:
             process = {}
             for appl in config.application:
                 hl_status = config.application[appl]['hl']
                 if hl_status == '' or hl_status.startswith('Error'):
 
-                    cls._log.info(f'Running Highlight analysis for {config.project_name}\{appl}')
+                    # cls._log.info(f'Running Highlight analysis for {config.project_name}\{appl}')
+                    cls._log.info(f'Running Highlight analysis for {appl}')
                     app_id = rest.get_app_id(appl)
                     if app_id is None:
                         cls._log.info(f'Application {appl} not found in Highlight, Creating Application {appl}...')
                         resp_code = rest.create_an_app(config.hl_instance, appl)
                         if resp_code == 200:
                             cls._log.info(f'Application {appl} created inside Highlight.')
                             app_id = rest.get_app_id(appl)
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/analysis/trackAnalysis.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/analysis/trackAnalysis.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 class TrackAnalysis(Analysis):
     def __init__(cls, post_aip_opertion, log_level:int):
         super().__init__(cls.__class__.__name__,log_level)
         cls._post_aip = post_aip_opertion
         pass
 
     def run(cls, config:Config):
-
+        cls._log.info(f"Stopping oneclick will stop HL analysis but not AIP. You can check status of AIP Scan directly on AIP Console at {config.console_url}")
         while True:
-            cls._log.info(f'Checking {len(cls._pid)} processes ...')
+            # cls._log.info(f'Checking {len(cls._pid)} processes ...')
             for p in cls._pid:
                 just_completed=False
                 process = p.process
                 if p.status is None or p.status == "Running":
                     if process is not None and process.poll() is None:
                         #process is running
                         p.status = "Running"
@@ -44,64 +44,66 @@
                                 p.status = config.application[p.name]['hl']
                         else:
                             stdout, stderr = process.communicate()
                             for line in stdout.split('\n'):
                                 #if len(find_in_list(line,p.log))==0:
                                 p.log.append(line)
                             if process.returncode == 0:
-                                p.status = 'OK'
+                                p.status = 'Complete'
                             else:
                                 p.status = f'Error: {process.returncode}'
                                 cls._log.error(f'error running {p.name}')
                                 cls._log.error('\n'.join(p.log))
 
                             if p.operation == 'AIP':
                                 config.application[p.name]['aip'] = p.status
                             else:
                                 config.application[p.name]['hl'] = p.status
                             config._save()
                             
 
-                cls._log.info(f"{p.operation} analysis for {config.project_name}\{p.name}: {p.status}")
+                cls._log.info(f"{p.operation} analysis for Application {p.name}, {p.status}")
                 if just_completed == True:
-                    if p.status != 'OK':
+                    if p.status != 'Complete':
                         for line in p.log:
                             print(f'\t{line}')
 
-                    if p.status=='OK' and  p.operation == 'AIP':
-                        cls._log.info('Running post analsis jobs...')
+                    if p.status=='Complete' and  p.operation == 'AIP':
+                        # cls._log.info('Running post analsis jobs...')
                         for proc in cls._post_aip:
                             if proc.__class__.__name__ not in config.application[p.name] or \
-                                config.application[p.name][proc.__class__.__name__] != 'OK':
+                                config.application[p.name][proc.__class__.__name__] != 'Complete':
 
                                 cls._log.info(f'******************* {proc.__class__.__name__} *******************************')
                                 proc.run(p.name)
                                 
-                                config.application[p.name][proc.__class__.__name__]='OK'
+                                config.application[p.name][proc.__class__.__name__]='Complete'
                                 config._save()
 
 
             running = False
             for p in cls._pid:
                 if p.status=='Running':
                     running = True
                     break 
             if not running:
                 cls._log.info(f'All processing complete')
                 error = False
                 for p in cls._pid:
                     cls._log.info(f"{p.operation} for {config.project_name}\{p.name}: {p.status}")
-                    if "OK" not in p.status:
+                    if "Complete" not in p.status:
                         error = True
                 break
             sleep(60)
         return error
 
 
         #     status,output = check_process(process[appl])
         #     if status != 0:
         #         cls._log.error(f'Error analyzing {appl}')
         #         error = True
         # if error:
         #     # TODO: add more desriptive error message
         #     raise RuntimeError ("")
 
+    def get_title(cls) -> str:
+        return "TRACKING ANALYSIS"
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/config.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,51 +22,46 @@
     log = None
     log_translate = {} 
 
     def __init__(self,parser:ArgumentParser,default_args={},log_level: int=INFO):
         self.log = Logger(self.__class__.__name__,log_level)
 
         args = parser.parse_args()
-
-        if not exists(abspath(args.baseFolder)):
-            raise InvalidConfigNoBase(f'Base folder must exist: {args.baseFolder}')
+ 
+        try:
+            if not exists(abspath(args.baseFolder)):
+                raise InvalidConfigNoBase(f'Base folder must exist: {args.baseFolder}')
+        except AttributeError as ae:
+                raise InvalidConfigNoBase(f'Base folder is a required argument')
+            
 
         base_config=abspath(f'{args.baseFolder}/.oneclick/config.json')
         if not exists(base_config) and args.command == 'run':
             raise NoConfigFound('Base configuration file found, please run with the "config" option')
 
-        if args.command == 'setup':
-            if not exists(base_config):
-                self._config={}
-                self._config_file=base_config
-                self.base = args.baseFolder
-            else:
-                self._config_file = abspath(f'{args.baseFolder}/.oneclick/config.json')
-                with open(abspath(self._config_file), 'rb') as config_file:
-                    self._config = load(config_file)
-        elif args.command == 'config':
+
+        if args.command == 'config':
             if not exists(base_config):
                 self._config={}
                 self._config_file=base_config
                 self.base = args.baseFolder
             else: 
                 if args.projectName is None:
                     self._config_file = abspath(f'{args.baseFolder}/.oneclick/config.json')
                 else:
                     self._config_file = abspath(f'{args.baseFolder}/.oneclick/{args.projectName}.json')
 
                 with open(abspath(self._config_file), 'rb') as config_file:
                     self._config = load(config_file)
             try:       
-                if 'java_home' not in args or args.java_home is None:
+                if args.java_home is None:
                     self.java_home = ''
                 else:
                     self.java_home = args.java_home
 
-
                 if args.cloc_version is not None: self.cloc_version = args.cloc_version
                 if args.profiler is not None: self.profiler = args.profiler
 
                 #Dashboard
                 if args.aipURL is not None: self.aip_url = args.aipURL
                 if args.aipPassword is not None: self.aip_password = args.aipPassword
                 if args.aipUser is not None: self.aip_user = args.aipUser
@@ -140,31 +135,30 @@
                             if len(self.console_key) == 0:
                                 self.console_key=secret_input('Missing console KEY:',self.console_key)
                             if len(self.console_cli) == 0:
                                 self.console_cli=folder_input('\t"AIP Console automation tools" location',dirname(self.console_cli),"aip-console-tools-cli.jar",True)
                     else:
                         self._set_console_active=False                                
 
-                if args.end in ['Analysis','Report']:
-                    if self.is_hl_active == False:                
-                        if yes_no_input('Run Highlight analysis for all applications?'):
-                            while not self.is_hl_active:
-                                if len(self.hl_url) == 0:
-                                    self.hl_url=url_input('Missing Highlight URL',self.hl_url)
-                                if len(self.hl_user) == 0:
-                                    self.hl_user=string_input('Missing Highlight User ID',self.hl_user)
-                                if len(self.hl_password) == 0:
-                                    self.hl_password=secret_input('Missing Highlight Password',self.hl_password)
-                                if len(self.hl_instance) == 0:
-                                    self.hl_instance=string_input('Missing Highlight Instance ID',self.hl_instance)
-                                else:
-                                    self.hl_instance=self.hl_instance
+                if self.is_hl_active == False:                
+                    if yes_no_input('Run Highlight analysis for all applications?'):
+                        while not self.is_hl_active:
+                            if len(self.hl_url) == 0:
+                                self.hl_url=url_input('Missing Highlight URL',self.hl_url)
+                            if len(self.hl_user) == 0:
+                                self.hl_user=string_input('Missing Highlight User ID',self.hl_user)
+                            if len(self.hl_password) == 0:
+                                self.hl_password=secret_input('Missing Highlight Password',self.hl_password)
+                            if len(self.hl_instance) == 0:
+                                self.hl_instance=string_input('Missing Highlight Instance ID',self.hl_instance)
+                            else:
+                                self.hl_instance=self.hl_instance
 
-                self.log.info(f'Run MRI analysis: {self.is_aip_active}')
-                self.log.info(f'Run Highlight analysis: {self.is_hl_active}')
+                # self.log.info(f'Run MRI analysis: {self.is_aip_active}')
+                # self.log.info(f'Run Highlight analysis: {self.is_hl_active}')
                 self._save()
 
             except JSONDecodeError as e:
                 msg = str(e)
                 self.log.error(f'Configuration file {self._config_file} must be in a JSON format {msg}')
                 exit()
 
@@ -386,14 +380,15 @@
         if self._set_value(self.console,key,value,default):
             self._set_active(self.console,['URL','API_Key','cli'])
             self._save()
 
     @property
     def is_console_active(self)->bool:
         return self._get(self.console,'Active',False)
+
     @property
     def console(self):
         return self._get(self.rest,'AIPConsole',{})
 
     @property
     def console_url(self)->str:
         return self._get(self.console,'URL')
@@ -514,15 +509,15 @@
     def project(self):
         return self._config['project']
     @project.setter
     def project(self,value):
         if type(value) is not str:
             raise ValueError(f'Expecting a the project name, got {type(value)}')
 
-        self.log.info(f'New project: {value}')
+        self.log.info(f'Starting executin of project {value}')
         if 'project' not in self._config:
             self._config['project']={}
             self._config['project']['name']=value
             self._config['project']['application']={}
 
         elif value.lower() != self.project_name.lower():
             raise ValueError("Can't rename a project")
@@ -655,24 +650,20 @@
     #         self.setting['reset']=False
     #     else:
     #         self.setting['reset']=value
     #     self._save()
 
     @property
     def java_home(self):
-        return self._get(self.setting,'java-home')
+        return self.setting['java-home']
     @java_home.setter
     def java_home(self,value):
         if self._set_value(self.setting,'java-home',value,''):
             self._save()
 
-def set_value(value:str, default:str=''):
-    if len(value) == 0:
-        value=default
-    return value
 
 def yes_no_input(prompt:str,default_value=True) -> bool:
     while True:
         if default_value:
             default_value='Y'
         else:
             default_value='N'
@@ -738,15 +729,15 @@
             if len(default_value) == 0:
                 print('Input required, please try again')
                 continue
             else:
                 i = default_value
         return i            
 
-def url_input(prompt:str, default:str):
+def url_input(prompt:str,default:str):
     while True:
         i = input(f'{prompt} [{default}]: ')
         if len(i)>0 and uri_validator(i):
             default = i
         if uri_validator(default):
             return default
         else:
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/cleanup.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/cleanup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,25 +40,25 @@
             files_list = f.read().splitlines()
 
         exclusionFolderList= abspath(f'{dir}\\scripts\\{cls.cleanup_file_prefix}deleteFolderList.txt')
         with open(exclusionFolderList) as f:
             folder_list = f.read().splitlines()
 
         apps= config.application
-        cls._log.info(f'Running {cls.__class__.__name__} for all applications')
+        # cls._log.info(f'Running {cls.__class__.__name__} for all applications')
         found = True
         while found:
             found = False
             for app in apps:
                 log_folder=f'{output_path}\\{app}'
                 create_folder(log_folder)
                 base = f'{log_folder}\\{cls.cleanup_file_prefix}'
                 cleanup_log_file= f"{base}_deletedFiles_{file_suffix}.log"
                 cls.cleanup_log = Logger('File',level=cls._log_level,file_name=cleanup_log_file,console_output=False)
-                cls._log.info(f'Cleanup file log: {cleanup_log_file}')
+                # cls._log.info(f'Cleanup file log: {cleanup_log_file}')
 
                 app_folder = abspath(f'{config.work}\\{cls.cleanup_file_prefix}\\{config.project_name}\\{app}')
 
                 # cls._log.info(f'Reviewing {app} ({app_folder})')
                 # with open (clean_up_log_file, 'a+') as file1: 
                 #     with open (clean_up_log_folder, 'a+') as file2: 
 
@@ -76,15 +76,17 @@
                         for file in files:
                             if cls.find_with_list(file,files_list):
                                 file=join(subdir, file)
                                 remove(file)
                                 file_cnt+=1
                                 cls.cleanup_log.info(f'Folder: {file}')
 
-                cls._log.info(f'Removed {file_cnt} files and {folder_cnt} folders from {app_folder}')
+                # cls._log.info(f'Removed {file_cnt} files and {folder_cnt} folders from {app_folder}')
+                cls._log.info(f'Application {app}, removed {file_cnt} files and {folder_cnt} folders')               
+                cls._log.info(f'Cleanup log: {cleanup_log_file}\n')
         cls._log.debug('Source Code cleanup done')
 
     def find_with_list(cls,find_in:str,pattern:list):
         rslt = False
         for p in pattern:
             try:
                 cls.cleanup_log.debug(f'matching: {p} in: {find_in}')
@@ -92,14 +94,17 @@
                     rslt = True
                     break
             except re.error as ex:
                 cls._log.warning(f'{ex.msg} for pattern {ex.pattern}')
             
         return rslt
 
+    def get_title(cls) -> str:
+        return "CLEANUP FOR CAST AIP"
+
 def rmtree(top):
     for root, dirs, files in walk(top, topdown=False):
         for name in files:
             filename = join(root, name)
             chmod(filename, S_IWUSR)
             remove(filename)
         for name in dirs:
@@ -109,7 +114,10 @@
 class cleanUpHL(cleanUpAIP):
     def __init__(cls,config:Config, log_level:int):
         super().__init__(config,cls.__class__.__name__,log_level)
 
     @property
     def cleanup_file_prefix(cls):
         return "HL"
+    
+    def get_title(cls) -> str:
+        return "CLEANUP FOR CAST HIGHLIGHT"
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/cloc.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/cloc.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,15 @@
                 process[appl]=None
                 continue 
             cloc_run=True
             process[appl] = cls._run_cloc(work_folder,cloc_output,cloc_output_ignored)
 
         #has all cloc processing completed
         if cloc_run:
+            cls._log.info('=> Using CLOC')
             all_done=False
             with tqdm(total=0,desc='CLOC Running') as t:
                 while (not all_done):
                     all_done=len([x for x in process.values() if x != 'DONE' and x!='ERROR' and x!=None]) == 0
                     if all_done:
                         t.total=0
                         t.refresh() 
@@ -190,15 +191,14 @@
                 #extracting required data from content of cloc_output.txt using python regex
                 header=content.split('\n')[2]
                 header_list=findall('\w+',header.upper())
 
                 summary='\n'.join(content.split('\n')[4:-4])
                 pattern='(.{25})\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})'
                 statistics_list=findall(pattern,summary)
-                
                 with open(cloc_output_ignored, 'r') as fp:
                     lines = len(fp.readlines())
                 statistics_list.append(('Unknown Files','0','0','0',str(lines)))
                 df = DataFrame(statistics_list,columns=header_list)
 
                 #making technolgy case insensitive
                 tech_list = list(map(lambda x: x.lower().strip(), tech_list))
@@ -207,19 +207,28 @@
                 #converting column values into int from string
                 numbers=['FILES','BLANK','COMMENT','CODE']
                 total_line=['']
                 for name in numbers:
                     df[name] = df[name].astype('int')
                 tab_name = f'{appl}-{cls.phase}'
                 tab_name = (tab_name[:30] + '..') if len(tab_name) > 30 else tab_name
+                loc = df['CODE'].sum()
+                if cls.phase == 'Before':
+                    cls._log.info(f'application {appl}, total loc {loc}')
+                if cls.phase == 'After':
+                    cls._log.info(f'application {appl}')    
+                    position = content.find('\n')
+                    print(content[position+1:])
                 workbook = format_table(ClocPreCleanup.writer,df,tab_name,total_line=True)
             else:
                 cls._log.error(f'Error running CLOC for {appl} {output[appl]}')
         return True
 
+    def get_title(cls) -> str:
+        return "DISCOVERY BEFORE CLEANUP"
 
 
 class ClocPostCleanup(ClocPreCleanup):
 
     def __init__(cls, config: Config, log_level:int=INFO, name = None):
         super().__init__(config,log_level,cls.__class__.__name__)
 
@@ -243,8 +252,11 @@
         ClocPreCleanup.writer.close()
         pass
 
     def if_exist_remove(cls,name:str):
         if exists(name):
             remove(name)
 
+    def get_title(cls) -> str:
+        return "DISCOVERY AFTER CLEANUP"
+
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/discoveryReport.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/discoveryReport.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         doc_para = doc.add_paragraph(f'Please find below the completed discovery for Project {config.project_name}. Note that we used CLOC for quick discovery and completeness verification. The actual lines of code discovered by the CAST solution may differ slightly from below. ')
         doc.add_heading('Questions', 1)
         doc.add_paragraph('<Specific questions to be added manually if needed. Remove this section if no questions>')
 
         doc.add_heading('Observation by Application', 1)
 
         for appl in tqdm(config.application,desc='Discovery',leave=True, position=1):
-            cls._log.info(f'Running {cls.__class__.__name__} for {appl}')
+            # cls._log.info(f'Running {cls.__class__.__name__} for {appl}')
 
             sql_report = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-SQLReport.xlsx')
 
             doc.add_heading(f'Application {appl}:', 2)
 
             before_df = cls.cloc_report(cloc_report,f'{appl}-Before')
             if before_df.empty:
@@ -84,18 +84,14 @@
                 #sql_df = sql_df[sql_df['Total']>0]
 
                 # out of scope code base
                 langs=len(before_df)
                 total, unit = convert_LOC(int(before_df['CODE'].sum()))
                 doc.add_paragraph(f"This delivery contains {langs} discovered technolog{'ies' if langs > 1 else 'y'}/extension{'s' if langs > 1 else ''}  and a total of {total} {unit}.",style='List Bullet')
 
-                if after_df.empty:
-                    cls._log.warning(f'No applicable technologies found!')
-                    after_df = DataFrame(columns=['LANGUAGE','FILES','BLANK','COMMENT','CODE','APPLICABLE'])
-
                 bsuport = after_df[after_df['APPLICABLE']==True]
                 total = int(bsuport['CODE'].sum())
                 total, unit = convert_LOC(total)
 
                 lang_list = list(bsuport['LANGUAGE'].str.strip())
                 langs = len(lang_list)
                 if langs >1:
@@ -116,18 +112,18 @@
 
                 # in scope code base
                 # asuport = after_df[before_df['APPLICABLE']==True]
                 # total = int(asuport['CODE'].sum())
                 # total, unit = convert_LOC(total)
                 #doc.add_paragraph(f'After removing all Sample, Test and other non production related code there is ({total} {unit}) in scope for this project',style='List Bullet 2')
                 #print(sql_df)
-                create_df=sql_df[sql_df['Name'].str.startswith('Create')].copy()
+                create_df=sql_df[sql_df['Name'].str.startswith('Create')]
                 if len(create_df):
                     sql_items = []
-                    create_df.sort_values(by=['Unique'],ascending=False,inplace=True)
+                    create_df.sort_values(['Unique'],ascending=False,inplace=True)
                     for index,item in create_df.iterrows():
                         count = int(item['Unique'])             # get the unique count from dataframe
                         name = item['Name'].split(" ")[1]       # remove the word Create
                         if count == 1: name = name[:-1]         # only one item, remove make name singular
                         sql_items.append(f'{count} {name}')
                     doc.add_paragraph(f'The database contains a total of {list_to_text(sql_items)}.',style='List Bullet')
                 else:
@@ -165,16 +161,19 @@
                 make_rows_bold(t.rows[len(after_df)])
 
                 # Adding style to a table
                 t.style = 'Medium Shading 1 Accent 1'
 
         # now save the document to a location
         doc.save(discovery_report)
-        cls._log.info(f'Source Code Discovery report has been written to {discovery_report}')
+        # cls._log.info(f'Source Code Discovery report has been written to {discovery_report}')
+        cls._log.info(f'Source Code Discovery report generated at {discovery_report} (note: pls review report document before sharing)\n')
 
+    def get_title(cls) -> str:
+        return "DELIVERABLE DISCOVERY REPORT"
 
 def make_rows_bold(*rows):
     for row in rows:
         for cell in row.cells:
             for paragraph in cell.paragraphs:
                 for run in paragraph.runs:
                     run.font.bold = True
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/profiler.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/profiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from oneclick.discovery.sourceValidation import SourceValidation 
 from oneclick.config import Config
 from cast_common.logger import Logger,INFO
 from cast_common.util import run_process,track_process,check_process,format_table,create_folder
 from os import listdir,remove,rename
-from os.path import exists,abspath,isfile
+from os.path import exists,abspath,getsize
 from pandas import json_normalize,ExcelWriter
 from json import load
 from tqdm import tqdm
 
 
 
 class ProfilerPreCleanup(SourceValidation):
@@ -96,18 +96,14 @@
             if not frameworks.empty: format_table(writer,frameworks,'frameworks',total_line=True)
             writer.close()
         else: 
             cls._log.warning('No profiler results found')
         pass
 
     def run(cls,config:Config):
-        if len(config.profiler) == 0 or not isfile(config.profiler):
-            cls._log.warning('Profiler path is not set in the configuration. Profiling will not be run.')
-            return
-
         for appl in config.application:
             work_folder = abspath(f'{config.work}/AIP/{config.project_name}/{appl}')
             profiler_output=abspath(f'{config.report}/{config.project_name}/{appl}')
             
             create_folder(profiler_output)
             cls._run_profiler(app_name=appl,work_folder=work_folder,profiler_output=profiler_output)
-
+
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/sqlDiscovery.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/sqlDiscovery.py`

 * *Files 22% similar despite different names*

```diff
@@ -44,21 +44,22 @@
         pass
 
     def run(cls,config:Config):
         
         apps= config.application
 
         for app in apps:
-            cls._log.info(f'Running {cls.__class__.__name__} for {app}')
+            # cls._log.info(f'Running {cls.__class__.__name__} for {app}')
+            cls._log.info(f'application {app}')
 
             cls._data=[]
             sql_files = []
             non_sql_files = []
             app_folder = abspath(f'{config.work}\\AIP\\{config.project_name}\\{app}')
-            cls._log.info(f'Searching {app_folder}')
+            # cls._log.info(f'Searching {app_folder}')
             with tqdm(total=0) as pbar:
                 for root, dirs, files in walk(app_folder):
                     for file in files:
                         if file.endswith(".bod") or \
                         file.endswith(".fnc") or \
                         file.endswith(".prc") or \
                         file.endswith(".trg") or \
@@ -92,28 +93,50 @@
                             dups = len(detail_df.drop_duplicates(subset=[key]))
                             total=len(detail_df)
                             summary_df.loc[len(summary_df.index)] = [key,total,dups,total-dups]
                         else:
                             summary_df.loc[len(summary_df.index)] = [key,0,0,0]
                             detail[key]=None
 
+                total_tables = summary_df.loc[0]['Total']
+                total_functions = summary_df.loc[1]['Total']
+                total_procedures = summary_df.loc[2]['Total']
+                total_views = summary_df.loc[3]['Total']
+                total_triggers = summary_df.loc[4]['Total']
+                total_artifacts = total_tables + total_functions + total_procedures + total_triggers + total_views
+                print('-------------------------------------')
+                print('Artifacts                     Count')
+                print('-------------------------------------')
+                print(f'Tables                          {total_tables}')
+                print(f'Functions                       {total_functions}')
+                print(f'Procedures                      {total_procedures}')
+                print(f'Views                           {total_views}')
+                print(f'Triggers                        {total_triggers}')
+                print('-------------------------------------')
+                print(f'Total Artifacts                 {total_artifacts}')
+                print('-------------------------------------')
+
                 if not summary_df.empty:
                     summary_df=summary_df.sort_values(['Name'],ascending=False)
                     filename = abspath(f'{config.report}/{config.project_name}/{app}/{app}-SQLReport.xlsx')
                     writer = ExcelWriter(filename, engine='xlsxwriter')
                     dups_format = writer.book.add_format({'bg_color': '#FFFF00', 'font_color': '#9C0006'})
                     xls=format_table(writer,summary_df,'Summary',total_line=True)
                     xls.conditional_format(f'D2:D{len(summary_df)}', {'type':'cell','criteria':'>','value':0,'format':dups_format})
 
                     for key in tqdm(cls._pattern.keys(),desc=f'Writing {filename}'):
                         if not detail[key] is None:
                             xls = format_table(writer,detail[key],key)
                             xls.conditional_format(f'A1:B{len(detail[key])}', {'type':'formula','criteria':'=COUNTIF($B:$B,$B1)>1','format':dups_format})
 
                     writer.close()
-                    cls._log.info(f'SQL Discovery Report: {filename}')
+                    # cls._log.info(f'SQL Discovery Report: {filename}')
+                    cls._log.info(f'detailed discovery report available at {filename}\n')
             else:
-                cls._log.warning(f'No SQL found')
-        cls._log.info('SQLDiscovery complete.')
+                cls._log.warning(f'No SQL found\n')
+        # cls._log.info('SQLDiscovery complete.')
         pass
 
+    def get_title(cls) -> str:
+        return "SQL ARTIFACTS DISCOVERY"
+
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/discovery/unzip.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/discovery/unzip.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,55 +18,63 @@
 
 class Unzip(SourceValidation):
    skip = ['__MACOSX','.DS_Store']
 
    def __init__(cls, config:Config, log_level:int):
         super().__init__(config,cls.__class__.__name__,log_level)
 
-   def unzip(cls,src_fldr) -> bool:
+   def unzip(cls,src_fldr:str) -> tuple[bool,int,int]:
+      unarchived_files = 0
+      archived_files = 0
       error = False
       found = True
       while found:
          found = False
          for root, dirs, files in tqdm(walk(src_fldr), leave=False, position=1):
             try:
                if '__MACOSX' in root or '.DS_Store' in files:
                   continue
                for file in files:
                   full_name = abspath(f'{root.strip()}\\{file}')
                   dest = full_name.replace(f".{full_name.split('.')[-1]}",'')
 
                   found=False
                   if file.endswith(".gz"):
+                     archived_files += 1
                      found = True
                      with gz(full_name, 'rb') as f_in:
                         if not exists(dest):
                            with open(dest, 'wb') as f_out:
                               copyfileobj(f_in, f_out)               
 
                   elif file.endswith(".tar") or \
                        file.endswith(".gztar") or \
                        file.endswith(".bztar") or \
                        file.endswith(".tgz"):
                      with tar(full_name) as f_in:
+                        archived_files += 1
                         found = True
                         create_folder(dest)
                         f_in.extractall(dest)
 
                   elif file.endswith(".7z") or file.endswith(".zip") :
+                     archived_files += 1
                      found = True
                      full_name = abspath(f'{root.strip()}\\{file}')
                      create_folder(dest)
                      with ZipFile(full_name) as zf:
                         for member in tqdm(zf.infolist(), desc='Extracting ',position=0,leave=False):
                            zf.extract(member, dest)
                      #Archive(full_name).extractall(dest,auto_create_dir=True)
 
+                  else:
+                     unarchived_files += 1
+
                   if found:     
-                     cls.zip_log.info(f'Unpacked: {full_name}')  
+                     # cls.zip_log.info(f'Unpacked: {full_name}')  
                      remove(full_name)
             except BadZipFile:
                #not a valid zip file log it then remove from staging folder
                print('')
                cls._log.error(f'Bad zip file: {full_name}')  
                remove(full_name)
 
@@ -76,18 +84,18 @@
                cls._log.error(str(ex))
                error = True
 
       #terminate on error 
       if error: 
          raise
 
-      return found
+      return found, archived_files, unarchived_files
 
    def run(cls,config:Config):
-      cls._log.info(f'Running {cls.__class__.__name__} for all applications')
+      # cls._log.info(f'Running {cls.__class__.__name__} for all applications')
       cls._log.debug('Running unzip step')
 
       #scan delivery folder for application folders
       apps= config.application
       # for (dirpath,dirnames,filenames) in walk(work_folder):
       #    apps.extend(dirnames)
       
@@ -102,26 +110,35 @@
             dateTimeObj=datetime.now()
             file_suffix=dateTimeObj.strftime("%d-%b-%Y(%H.%M.%S.%f)")
 
             zip_log_file= abspath(f"{log_folder}/unzip_{file_suffix}.log")
             log_name = 'Unzip-files'
             cls.zip_log = Logger(log_name,level=cls._log_level,file_name=zip_log_file,console_output=True)
 
-            found = cls.unzip(abspath(f'{config.work}\\AIP\\{config.project_name}\\{app}'))
-            found = cls.unzip(abspath(f'{config.work}\\HL\\{config.project_name}\\{app}'))
+            found, archived_files, unarchived_files = cls.unzip(abspath(f'{config.work}\\AIP\\{config.project_name}\\{app}'))
+            found, archived_files, unarchived_files = cls.unzip(abspath(f'{config.work}\\HL\\{config.project_name}\\{app}'))
+
+            cls._log.info(f'application {app}, found {unarchived_files} files and {archived_files} archive files')
+            embedded_archives = archived_files - 1
+            if embedded_archives > 0:   
+               cls._log.info(f'{archived_files} files unzipped successfully. {embedded_archives} embedded archives found and unzipped successfully.\n')
+            else:
+               cls._log.info(f'{archived_files} files unzipped successfully. 0 embedded archives found.\n')
 
             Logger.loggers.remove(log_name)
 
             #          full_name = abspath(f'{root.strip()}\\{file}')
             #          dest = full_name.replace(f".{full_name.split('.')[-1]}",'')
             #          cls._log.info(f'Unzipping {full_name}')
 
             #          Archive(full_name).extractall(dest,auto_create_dir=True)
                      
             #          remove(full_name)
 
-      cls._log.info('Unzip step complete')
-                                
+      # cls._log.info('Unzip step complete')
+
+   def get_title(cls) -> str:
+      return 'DISCOVER ARCHIVES AND UNZIP\n'
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/main.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,15 +114,16 @@
     run_parser.add_argument('-d','--debug',  default=False,type=bool)
 
     return parser,config_parser
 
 #TODO: d2-Ability to install onclick with all its components via PIP (d2)
 #TODO: d1-send emails (d1-SHP)
 if __name__ == '__main__':
-
+    log_level = INFO
+    log = Logger("main")
 
     print('\nCAST One Click')
     print('Copyright (c) 2023 CAST Software Inc.\n')
     print('If you need assistance, please contact us at oneclick@castsoftware.com\n')
 
 
     parser,config_parser = command_line()
@@ -131,32 +132,29 @@
 
     config = NotImplemented
     try:
         config=Config(parser,default_args)
         #printing some inital messages to the user
 
         if args.command == 'config':
-            log_level = INFO
-            log = Logger("main")
-
             file = ''
             if args.projectName is None:
                 file='Default'
             else:
                 file = args.projectName
             log.info(f'{file} configuration file successfuly updated')
             exit ()
         elif args.command == 'run':
             file_name=abspath(f'{args.baseFolder}/ONECLICK_WORK/LOGS/{config.project_name}')
             create_folder(file_name)
             config.log_filename=abspath(f'{file_name}/general.log')
             
             log_level = INFO
             log = Logger("main",file_name=config.log_filename)
-            log.info(f'Running {args.command}')
+            # log.info(f'Running {args.command}')
             config.validate_for_run()
 
     except NoConfigFound as ex:
         log.error(config_parser.format_help())
         log.error(ex)
         exit()
 
@@ -229,45 +227,52 @@
 
         RunARG(config,log_level)
 
         #TODO continue processing after analysis is done (d2)
         #TODO generate obsolescence report (d2)
     ]
 
-    step = 1
-    for p in process:
-        if issubclass(type(p), Analysis) and args.end == 'Discovery':
-            log.info('--end Discovery selected, process stopping here')
-            break
-
-
-        log.info(f'******************* Step {step} - {p.__class__.__name__} *******************************')
-        if args.start == 'Discovery':
-            if issubclass(type(p), SourceValidation):
-                status = p.run(config)
-
-        if args.start in ['Discovery','Analysis']:
-            if issubclass(type(p), Analysis):
-                status = p.run(config)
-                if status and issubclass(type(p), TrackAnalysis):
-                    log.error('One or more analysis failed, review logs and restart')
-                    break
-                elif status > 0:
-                    break
+    try:
+        step = 1
+        for p in process:
+            if issubclass(type(p), Analysis) and args.end == 'Discovery':
+                log.info('--end Discovery selected, process stopping here')
+                break
 
 
-        if args.end == 'Analysis':
-            if issubclass(type(p), RunARG):
-                break
+            log.info(f'=> STEP {step} : {p.get_title()}')
+            if args.start == 'Discovery':
+                if issubclass(type(p), SourceValidation):
+                    status = p.run(config)
+
+            if args.start in ['Discovery','Analysis']:
+                if issubclass(type(p), Analysis):
+                    status = p.run(config)
+                    if status and issubclass(type(p), TrackAnalysis):
+                        log.error('One or more analysis failed, review logs and restart')
+                        break
+                    elif status > 0:
+                        break
+
 
-        if args.start in ['Discovery','Analysis','Report']:
-            if issubclass(type(p), RunARG):
-                status = p.run(config)
-
-        # if issubclass(type(p), ActionPlan):
-        #     for appl in config.application:
-        #         log.info(f'Working on action items for {appl}')
-        #         p.run(appl)
+            if args.end == 'Analysis':
+                if issubclass(type(p), RunARG):
+                    break
+
+            if args.start in ['Discovery','Analysis','Report']:
+                if issubclass(type(p), RunARG):
+                    status = p.run(config)
+
+            # if issubclass(type(p), ActionPlan):
+            #     for appl in config.application:
+            #         log.info(f'Working on action items for {appl}')
+            #         p.run(appl)
+
+            step += 1
+    
+    except InvalidConfiguration as ic:
+        log.error(ic)
+    except Exception as ex:
+        log.error(ex)
 
-        step += 1
 
     log.info('Complete')
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/runArg.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/runArg.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,17 @@
         arg_cfg_file = abspath(f'{config.report}/{config.project_name}/{appl_name}-config.json')
         with open(arg_cfg_file, "w") as f:
             dump(cfg,f,indent=4)
 
         GeneratePPT(ARGConfig(arg_cfg_file)).save_ppt()
         pass
 
+    def get_title(cls) -> str:
+        return cls.__class__.__name__
+
 class  RunARGAIP(RunARG):
     def __init__(cls, config:Config, log_level:int) -> None:
         super().__init__(config,log_level,cls.__class__.__name__)
 
     def run(cls,appl_name:str) -> None:
         super().run(cls._config,appl_name,'AIP')
```

### Comparing `com.castsoftware.uc.oneclick-1.0.3/oneclick/sendEmail.py` & `com_castsoftware_uc_oneclick-1.0.4b1/oneclick/sendEmail.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-1.0.3/pyproject.toml` & `com_castsoftware_uc_oneclick-1.0.4b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name='com.castsoftware.uc.oneclick'
 description="Assessment Generator"
-version='1.0.3' #prod version
+version='1.0.4-beta-1' #prod version
 dependencies = [
     'pandas','python-pptx==0.6.18','python-docx',
     'argparse_formatter','django','pyunpack','tqdm',
     'patool','archive','pypiwin32','psycopg2','openpyxl',
-    'com.castsoftware.uc.python.common>=1.1.6',
+    'com.castsoftware.uc.python.common>=1.1.11',
     'com.castsoftware.uc.action-plan',
-    'com.castsoftware.uc.arg>=1.6.8'    
+    'com.castsoftware.uc.arg>=1.6.2'    
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

