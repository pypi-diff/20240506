# Comparing `tmp/rfswarm-manager-1.2.1.tar.gz` & `tmp/rfswarm_manager-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfswarm-manager-1.2.1.tar", last modified: Mon Feb 19 03:36:32 2024, max compression
+gzip compressed data, was "rfswarm_manager-1.3.0.tar", last modified: Mon May  6 03:03:29 2024, max compression
```

## Comparing `rfswarm-manager-1.2.1.tar` & `rfswarm_manager-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,16 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2024-02-19 03:36:32.248791 rfswarm-manager-1.2.1/
--rw-r--r--   0 dave       (501) staff       (20)    35149 2019-11-02 13:28:40.000000 rfswarm-manager-1.2.1/LICENSE
--rw-r--r--   0 dave       (501) staff       (20)     3156 2024-02-19 03:36:32.248542 rfswarm-manager-1.2.1/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)     6597 2024-02-02 01:15:20.000000 rfswarm-manager-1.2.1/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2024-02-19 03:36:32.241738 rfswarm-manager-1.2.1/rfswarm_manager/
--rw-r--r--   0 dave       (501) staff       (20)       53 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/rfswarm_manager/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)   316579 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/rfswarm_manager/rfswarm.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2024-02-19 03:36:32.244489 rfswarm-manager-1.2.1/rfswarm_manager.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)     3156 2024-02-19 03:36:31.000000 rfswarm-manager-1.2.1/rfswarm_manager.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      565 2024-02-19 03:36:31.000000 rfswarm-manager-1.2.1/rfswarm_manager.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2024-02-19 03:36:31.000000 rfswarm-manager-1.2.1/rfswarm_manager.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)      111 2024-02-19 03:36:31.000000 rfswarm-manager-1.2.1/rfswarm_manager.egg-info/entry_points.txt
--rw-r--r--   0 dave       (501) staff       (20)       78 2024-02-19 03:36:31.000000 rfswarm-manager-1.2.1/rfswarm_manager.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       23 2024-02-19 03:36:31.000000 rfswarm-manager-1.2.1/rfswarm_manager.egg-info/top_level.txt
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2024-02-19 03:36:32.248109 rfswarm-manager-1.2.1/robots/
--rw-r--r--   0 dave       (501) staff       (20)      818 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/robots/PythonListener.py
--rw-r--r--   0 dave       (501) staff       (20)      466 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/robots/RFSListener.py
--rw-r--r--   0 dave       (501) staff       (20)     3689 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/robots/RFSListener2.py
--rw-r--r--   0 dave       (501) staff       (20)       32 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/robots/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/robots/myLibrary.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/robots/myLibrary1.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/robots/myLibrary2.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/robots/myLibrary3.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/robots/myvariables.py
--rw-r--r--   0 dave       (501) staff       (20)     6843 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/robots/svg5.py
--rw-r--r--   0 dave       (501) staff       (20)     1863 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/robots/with_file_not_closed.py
--rw-r--r--   0 dave       (501) staff       (20)     1419 2024-02-19 03:36:30.000000 rfswarm-manager-1.2.1/setup-manager.py
--rw-r--r--   0 dave       (501) staff       (20)       38 2024-02-19 03:36:32.248886 rfswarm-manager-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:03:29.231907 rfswarm_manager-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 03:03:06.000000 rfswarm_manager-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-06 03:03:29.231907 rfswarm_manager-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-06 03:03:06.000000 rfswarm_manager-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:03:29.231907 rfswarm_manager-1.3.0/rfswarm_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 03:03:08.000000 rfswarm_manager-1.3.0/rfswarm_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   341809 2024-05-06 03:03:28.000000 rfswarm_manager-1.3.0/rfswarm_manager/rfswarm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:03:29.231907 rfswarm_manager-1.3.0/rfswarm_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-06 03:03:29.000000 rfswarm_manager-1.3.0/rfswarm_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-06 03:03:29.000000 rfswarm_manager-1.3.0/rfswarm_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 03:03:29.000000 rfswarm_manager-1.3.0/rfswarm_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 03:03:29.000000 rfswarm_manager-1.3.0/rfswarm_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 03:03:29.000000 rfswarm_manager-1.3.0/rfswarm_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 03:03:29.000000 rfswarm_manager-1.3.0/rfswarm_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-06 03:03:28.000000 rfswarm_manager-1.3.0/setup-manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 03:03:29.231907 rfswarm_manager-1.3.0/setup.cfg
```

### Comparing `rfswarm-manager-1.2.1/LICENSE` & `rfswarm_manager-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rfswarm-manager-1.2.1/PKG-INFO` & `rfswarm_manager-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: rfswarm-manager
-Version: 1.2.1
+Version: 1.3.0
 Summary: rfswarm manager
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
-License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
 Project-URL: Source, https://github.com/damies13/rfswarm
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: configparser
+Requires-Dist: HTTPServer
+Requires-Dist: pillow>=9.1.0
+Requires-Dist: psutil
+Requires-Dist: pip>=21,>=22
+Requires-Dist: matplotlib
+Requires-Dist: requests
 
 # rfswarm (Robot Framework Swarm)
 
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
@@ -54,9 +59,7 @@
 
 
 ## Donations
 
 If you would like to thank me for this project please consider using one of the sponsorship methods:
 - [GitHub](https://github.com/sponsors/damies13/)
 - [PayPal.me](https://paypal.me/damies13/5) (the $5 is a suggestion, feel free to change to any amount you would like)
-
-
```

### Comparing `rfswarm-manager-1.2.1/README.md` & `rfswarm_manager-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 |Version|Manager|Agent|Reporter|
 |---|---|---|---|
 |[![Latest PyPI version](https://img.shields.io/pypi/v/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Manager PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Agent PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-agent.svg)](https://pypi.python.org/pypi/rfswarm-agent/) | [![Number of Reporter PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-reporter.svg)](https://pypi.python.org/pypi/rfswarm-reporter/) |
 
 | Master | Branch |
 | -- | -- |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter) |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests) |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter) |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.3.0&label=Linter) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.3.0&label=Regression%20Tests) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.3.0&label=Linter) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.3.0&label=Regression%20Tests) |
 
 <img align="right" src="Doc/Images/Icon_Information.png">
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
 > _Swarm being the collective noun for Robots, just as Flock is for Birds and Herd for Sheep, so it made sense to use swarm for a performance testing tool using Robot Framework, hence rfswarm_
```

### Comparing `rfswarm-manager-1.2.1/rfswarm_manager/rfswarm.py` & `rfswarm_manager-1.3.0/rfswarm_manager/rfswarm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 #
 # 	Robot Framework Swarm
 # 		Manager
-#    Version 1.2.1
+#    Version 1.3.0
 #
 
 # 	Helpful links
 #
 #
 
 import argparse
@@ -443,26 +443,32 @@
 	# 	log_request is here to stop BaseHTTPRequestHandler logging to the console
 	# 		https://stackoverflow.com/questions/10651052/how-to-quiet-simplehttpserver/10651257#10651257
 	def log_request(self, code='-', size='-'):
 		pass
 
 
 class RFSwarmBase:
-	version="1.2.1"
+	version = "1.3.0"
 	debuglvl = 0
 
 	config = None
 	manager_ini = None
 
 	save_ini = True
 
 	# https://github.com/damies13/rfswarm/blob/master/Doc/rfswarm_manager.md#exclude-libraries
 	# default (BuiltIn,String,OperatingSystem,perftest)
 	excludelibrariesdefault = "BuiltIn,String,OperatingSystem,perftest"
 	testrepeaterdefault = False
+	injectsleepenableddefault = False
+	injectsleepminimumdefault = 15
+	injectsleepmaximumdefault = 45
+	disableloglogdefault = False
+	disablelogreportdefault = False
+	disablelogoutputdefault = False
 
 	scriptcount = 0
 	scriptlist: Any = [{}]
 	scriptfiles: Any = {}
 	scriptgrpend: Any = {}
 	scriptdefaults: Any = {}
 
@@ -1151,18 +1157,24 @@
 				st = datetime(n.year, n.month, n.day + 1, int(tarr[0]), int(tarr[1]))
 			if len(tarr) == 3:
 				st = datetime(n.year, n.month, n.day + 1, int(tarr[0]), int(tarr[1]), int(tarr[2]))
 
 		base.debugmsg(8, "st:", st, "	", int(st.timestamp()))
 		return int(st.timestamp())
 
-	def hash_file(self, file, relpath):
+	def hash_file(self, file, argrelpath=""):
 		if not (os.path.exists(file) and os.path.isfile(file)):
 			raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), file)
 		BLOCKSIZE = 65536
+
+		# if len(argrelpath) > 0:
+		base.debugmsg(7, "file:", file, "	ScriptDir:", base.config['Plan']['ScriptDir'])
+		relpath = base.get_relative_path(base.config['Plan']['ScriptDir'], file)
+		base.debugmsg(7, "file:", file, "	relpath:", relpath)
+
 		hasher = hashlib.md5()
 		hasher.update(str(os.path.getmtime(file)).encode('utf-8'))
 		hasher.update(relpath.encode('utf-8'))
 		# with open(file, 'rb') as afile:
 		# 	buf = afile.read(BLOCKSIZE)
 		# 	while len(buf) > 0:
 		# 		hasher.update(buf)
@@ -1227,28 +1239,29 @@
 				r = requests.get(url)
 				self.debugmsg(9, "tick_counter:", r.status_code)
 			except Exception:
 				pass
 			time.sleep(aday)
 
 	def replace_rf_path_variables(self, pathin, localdir):
-		base.debugmsg(8, "pathin:", pathin)
+		base.debugmsg(6, "pathin:", pathin)
 		base.debugmsg(8, "localdir:", localdir)
 		pathout = pathin
 		base.debugmsg(8, "pathout:", pathout)
 
 		# Issue #129 Handle `${CURDIR}/`
 		if pathout.find("${CURDIR}") > -1:
 			pathmod = pathout.replace("${CURDIR}", "")
 			base.debugmsg(8, "pathmod:", pathmod)
 			# https://stackoverflow.com/questions/1945920/why-doesnt-os-path-join-work-in-this-case
 			if platform.system() == "Windows":
 				pathmod = pathmod.replace("/", os.path.sep)
 				base.debugmsg(8, "pathmod:", pathmod)
 				pathout = os.path.abspath(os.path.join(localdir, *pathmod.split(os.path.sep)))
+				pathout = pathout.replace(r'${\}', r'${/}')
 			else:
 				pathout = os.path.abspath(os.path.join(os.path.sep, *localdir.split(os.path.sep), *pathmod.split(os.path.sep)))
 			base.debugmsg(8, "pathout:", pathout)
 
 		# Built-in variables - https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#built-in-variables
 
 		# ${TEMPDIR}
@@ -1257,14 +1270,15 @@
 			pathout = pathout.replace("${TEMPDIR}", tmpdir)
 			base.debugmsg(8, "pathout:", pathout)
 
 		# ${EXECDIR}
 		# not sure how to handle this for now
 
 		# ${/}
+		base.debugmsg(8, "pathout.find:", pathout.find("${/}"))
 		if pathout.find("${/}") > -1:
 			base.debugmsg(8, "Found ${/} in", pathout)
 			if pathout.find("${/}") == 0:
 				pathlst = ["${rfpv}"] + pathout.split("${/}")
 				base.debugmsg(8, "pathlst:", pathlst)
 				pathjoin = os.path.join(*pathlst)
 				base.debugmsg(8, "pathjoin:", pathjoin)
@@ -1272,27 +1286,28 @@
 				base.debugmsg(8, "pathjoin:", pathjoin)
 			else:
 				pathlst = pathout.split("${/}")
 				base.debugmsg(8, "pathlst:", pathlst)
 				pathjoin = os.path.join(*pathlst)
 				base.debugmsg(8, "pathjoin:", pathjoin)
 
-			if os.path.isfile(pathjoin):
+			filelst = glob.glob(pathjoin)
+			if os.path.isfile(pathjoin) or len(filelst) > 1:
 				base.debugmsg(8, "pathjoin:", pathjoin)
 				pathout = pathjoin
 				base.debugmsg(8, "pathout:", pathout)
 			else:
 				base.debugmsg(8, "pathjoin:", pathjoin)
 				pathout = self.localrespath(localdir, pathjoin)
 				base.debugmsg(8, "pathout:", pathout)
 
 		# ${:}
 		# ${\n}
 		# not sure whether to handle these for now
-		base.debugmsg(8, "pathout:", pathout)
+		base.debugmsg(6, "pathout:", pathout)
 
 		return pathout
 
 	def localrespath(self, localdir, resfile):
 		base.debugmsg(5, "localdir:", localdir)
 		base.debugmsg(5, "resfile:", resfile)
 		llocaldir = re.findall(r"[^\/\\]+", localdir)
@@ -1325,19 +1340,20 @@
 		if 'basedir' in self.scriptfiles[hash]:
 			basedir = self.scriptfiles[hash]['basedir']
 		else:
 			basedir = localdir
 
 		# look for __init__. files - Issue #90
 		initfiles = os.path.abspath(os.path.join(localdir, "__init__.*"))
-		base.debugmsg(7, "initfiles", initfiles)
+		base.debugmsg(8, "initfiles", initfiles)
 		filelst = glob.glob(initfiles)
 		for file in filelst:
 			base.debugmsg(7, "file:", file)
-			relfile = os.path.relpath(file, start=basedir)
+			# relfile = os.path.relpath(file, start=basedir)
+			relfile = base.get_relative_path(base.config['Plan']['ScriptDir'], file)
 			base.debugmsg(7, "relfile:", relfile)
 			newhash = self.hash_file(file, relfile)
 			base.debugmsg(7, "newhash:", newhash)
 			if newhash not in self.scriptfiles:
 				self.scriptfiles[newhash] = {
 					'id': newhash,
 					'basedir': basedir,
@@ -1348,77 +1364,83 @@
 				filename, fileext = os.path.splitext(file)
 				# splitext leaves the . on the extention, the list below needs to have the extentions
 				# starting with a . - Issue #94
 				if fileext.lower() in ['.robot', '.resource']:
 					t = threading.Thread(target=base.find_dependancies, args=(newhash, ))
 					t.start()
 
-		base.debugmsg(7, "localdir", localdir)
+		base.debugmsg(8, "localdir", localdir)
 		filename, fileext = os.path.splitext(localpath)
 
-		base.debugmsg(7, "filename, fileext:", filename, fileext)
+		base.debugmsg(8, "filename, fileext:", filename, fileext)
 
 		# splitext leaves the . on the extention, the list below needs to have the extentions
 		# starting with a . - Issue #94
 		if (fileext.lower() in ['.robot', '.resource'] and keep_going):
 			with open(localpath, 'r', encoding="utf8") as afile:
 				for line in afile:
 					if checking and '*** ' in line:
 						checking = False
 
 					if checking:
 						base.debugmsg(9, "line", line)
 						try:
 							if line.strip()[:1] != "#":
 								linearr = line.strip().split()
-								base.debugmsg(7, "linearr", linearr)
+								base.debugmsg(8, "linearr", linearr)
 								resfile = None
 								if len(linearr) > 1 and linearr[0].upper() in ['RESOURCE', 'VARIABLES', 'LIBRARY']:
 									base.debugmsg(9, "linearr[1]", linearr[1])
 									resfile = linearr[1]
 								if not resfile and len(linearr) > 2 and (linearr[0].upper() == 'METADATA' and linearr[1].upper() == 'FILE'):
 									base.debugmsg(9, "linearr[2]", linearr[2])
 									resfile = linearr[2]
 								if not resfile and len(linearr) > 2 and (linearr[0].upper() == 'IMPORT' and linearr[1].upper() == 'LIBRARY'):
 									base.debugmsg(9, "linearr[2]", linearr[2])
 									resfile = linearr[2]
 								if resfile:
-									base.debugmsg(7, "resfile", resfile)
+									base.debugmsg(8, "resfile", resfile)
 									# here we are assuming the resfile is a relative path! should we also consider files with full local paths?
 									# Issue #129 Handle ``${CURDIR}/``
 									if resfile.find("${") > -1:
 										localrespath = base.replace_rf_path_variables(resfile, localdir)
 									else:
 										localrespath = self.localrespath(localdir, resfile)
 
-									base.debugmsg(7, "localrespath", localrespath)
+									base.debugmsg(8, "localrespath", localrespath)
+									localrespath = os.path.abspath(localrespath)
+									base.debugmsg(8, "localrespath", localrespath)
 									if os.path.isfile(localrespath):
-										relfile = os.path.relpath(localrespath, start=basedir)
-										base.debugmsg(7, "relfile", relfile)
+										# relfile = os.path.relpath(localrespath, start=basedir)
+										relfile = base.get_relative_path(base.config['Plan']['ScriptDir'], localrespath)
+										base.debugmsg(8, "relfile", relfile)
 										newhash = self.hash_file(localrespath, relfile)
-										base.debugmsg(7, "newhash", newhash)
+										base.debugmsg(8, "newhash", newhash)
 										self.scriptfiles[newhash] = {
 											'id': newhash,
 											'basedir': basedir,
 											'localpath': localrespath,
 											'relpath': relfile,
 											'type': linearr[0]
 										}
 
 										t = threading.Thread(target=base.find_dependancies, args=(newhash, ))
 										t.start()
 
 									else:
+										base.debugmsg(6, "localrespath", localrespath)
 										filelst = glob.glob(localrespath)
+										base.debugmsg(6, "filelst", filelst)
 										for file in filelst:
-											base.debugmsg(9, "file", file)
-											relpath = file.replace(localdir, "")[1:]
-											base.debugmsg(9, "relpath", relpath)
+											base.debugmsg(6, "file", file)
+											# relpath = file.replace(localdir, "")[1:]
+											relpath = base.get_relative_path(base.config['Plan']['ScriptDir'], file)
+											base.debugmsg(6, "relpath", relpath)
 											newhash = self.hash_file(file, relpath)
-											base.debugmsg(9, "newhash", newhash)
+											base.debugmsg(6, "newhash", newhash)
 											self.scriptfiles[newhash] = {
 												'id': newhash,
 												'localpath': file,
 												'relpath': relpath,
 												'type': linearr[0]
 											}
 
@@ -1426,15 +1448,15 @@
 							base.debugmsg(6, "line", line)
 							base.debugmsg(6, "Exception", e)
 							base.debugmsg(6, "linearr", linearr)
 
 					# http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#test-data-sections
 					match = re.search(r'\*+([^*\v]+)', line)
 					if match is not None:
-						base.debugmsg(6, "match.group(0)", match.group(1))
+						base.debugmsg(6, "match.group(0)", match.group(0), "match.group(1)", match.group(1))
 						if match.group(1).strip().upper() in ['SETTINGS', 'SETTING', 'TEST CASES', 'TEST CASE', 'TASKS', 'TASK', 'KEYWORDS', 'KEYWORD']:
 							checking = True
 
 	def check_files_changed(self):
 		# self.scriptfiles[hash]
 		checkhashes = list(self.scriptfiles.keys())
 		base.debugmsg(6, "checkhashes:", checkhashes)
@@ -1459,16 +1481,16 @@
 
 					t = threading.Thread(target=base.find_dependancies, args=(script_hash, ))
 					t.start()
 
 					self.remove_hash(chkhash)
 
 	def get_relative_path(self, path1, path2):
-		base.debugmsg(7, "path1:", path1)
-		base.debugmsg(7, "path2:", path2)
+		base.debugmsg(5, "path1:", path1)
+		base.debugmsg(5, "path2:", path2)
 		# commonpath = os.path.commonpath([path1, path2])
 
 		base.debugmsg(8, "os.path.isdir(path1):", os.path.isdir(path1))
 		base.debugmsg(8, "os.path.isfile(path1):", os.path.isfile(path1))
 		# if not os.path.isdir(path1):
 		if os.path.isfile(path1) or not os.path.exists(path1):
 			path1 = os.path.dirname(path1)
@@ -2184,18 +2206,20 @@
 
 		if 'Plan' not in base.config:
 			base.config['Plan'] = {}
 			base.saveini()
 
 		if 'ScriptDir' not in base.config['Plan']:
 			base.config['Plan']['ScriptDir'] = base.inisafevalue(base.dir_path)
+			base.debugmsg(5, "ScriptDir: ", base.config['Plan']['ScriptDir'])
 			base.saveini()
 		else:
 			if not os.path.isdir(base.config['Plan']['ScriptDir']):
 				base.config['Plan']['ScriptDir'] = base.inisafevalue(base.dir_path)
+				base.debugmsg(5, "ScriptDir: ", base.config['Plan']['ScriptDir'])
 				base.saveini()
 
 		if 'ScenarioDir' not in base.config['Plan']:
 			base.config['Plan']['ScenarioDir'] = base.inisafevalue(base.dir_path)
 			base.saveini()
 		else:
 			if not os.path.isdir(base.config['Plan']['ScenarioDir']):
@@ -2206,14 +2230,15 @@
 			base.config['Plan']['ScenarioFile'] = ""
 			base.saveini()
 		else:
 			# check file exists - it may have been deleted since rfswarm last ran with this ini file
 			if not os.path.exists(base.config['Plan']['ScenarioFile']):
 				base.config['Plan']['ScenarioFile'] = ""
 				base.config['Plan']['ScriptDir'] = base.inisafevalue(base.dir_path)
+				base.debugmsg(5, "ScriptDir: ", base.config['Plan']['ScriptDir'])
 				base.config['Plan']['ScenarioDir'] = base.inisafevalue(base.dir_path)
 				base.saveini()
 
 		#
 		# Run
 		#
 
@@ -2576,14 +2601,46 @@
 		else:
 			base.debugmsg(1, "File contains no scenario:", ScenarioFile)
 			return 1
 
 		if "Script Defaults" in filedata:
 			base.scriptdefaults = filedata['Script Defaults']
 
+		# Set base.config['Plan']['ScriptDir']
+		base.debugmsg(5, "scriptcount:", scriptcount)
+		filelst = []
+		for i in range(scriptcount):
+			istr = str(i + 1)
+			base.debugmsg(5, "istr:", istr)
+			if istr in filedata:
+				base.debugmsg(5, "filedata[", istr, "]:", filedata[istr])
+				if "script" in filedata[istr]:
+					base.debugmsg(5, "filedata[", istr, "][script]:", filedata[istr]["script"])
+					scriptname = filedata[istr]["script"]
+					if '\\' in scriptname:
+						scriptnamearr = scriptname.split('\\')
+						scriptname = "/".join(scriptnamearr)
+					if not os.path.isabs(scriptname):
+						# relative path, need to find absolute path
+						combined = os.path.join(base.config['Plan']['ScenarioDir'], scriptname)
+						base.debugmsg(5, "combined:", combined)
+						scriptname = os.path.abspath(combined)
+					base.debugmsg(5, "scriptname:", scriptname)
+
+					filelst.append(scriptname)
+		if len(filelst) > 0:
+			commonpath = os.path.commonpath(filelst)
+			base.debugmsg(5, "commonpath: ", commonpath)
+			base.config['Plan']['ScriptDir'] = base.inisafevalue(commonpath)
+			base.saveini()
+		else:
+			base.config['Plan']['ScriptDir'] = base.inisafevalue(base.dir_path)
+			base.debugmsg(5, "ScriptDir: ", base.config['Plan']['ScriptDir'])
+			base.saveini()
+
 		rowcount = 0
 		for i in range(scriptcount):
 			ii = i + 1
 			istr = str(ii)
 			if istr in filedata:
 				base.debugmsg(5, "filedata[", istr, "]:", filedata[istr])
 				rowcount += 1
@@ -2661,14 +2718,36 @@
 
 				if "excludelibraries" in filedata[istr]:
 					base.scriptlist[ii]["excludelibraries"] = filedata[istr]["excludelibraries"]
 
 				if "robotoptions" in filedata[istr]:
 					base.scriptlist[ii]["robotoptions"] = filedata[istr]["robotoptions"]
 
+				# testrepeater = True
+				if "testrepeater" in filedata[istr]:
+					base.scriptlist[ii]["testrepeater"] = base.str2bool(filedata[istr]["testrepeater"])
+				# injectsleepenabled = True
+				if "injectsleepenabled" in filedata[istr]:
+					base.scriptlist[ii]["injectsleepenabled"] = base.str2bool(filedata[istr]["injectsleepenabled"])
+				# injectsleepminimum = 18
+				if "injectsleepminimum" in filedata[istr] and len(filedata[istr]["injectsleepminimum"]) > 0:
+					base.scriptlist[ii]["injectsleepminimum"] = int(filedata[istr]["injectsleepminimum"])
+				# injectsleepmaximum = 33
+				if "injectsleepmaximum" in filedata[istr] and len(filedata[istr]["injectsleepmaximum"]) > 0:
+					base.scriptlist[ii]["injectsleepmaximum"] = int(filedata[istr]["injectsleepmaximum"])
+				# disableloglog
+				if "disableloglog" in filedata[istr]:
+					base.scriptlist[ii]["disableloglog"] = base.str2bool(filedata[istr]["disableloglog"])
+				# disablelogreport
+				if "disablelogreport" in filedata[istr]:
+					base.scriptlist[ii]["disablelogreport"] = base.str2bool(filedata[istr]["disablelogreport"])
+				# disablelogoutput
+				if "disablelogoutput" in filedata[istr]:
+					base.scriptlist[ii]["disablelogoutput"] = base.str2bool(filedata[istr]["disablelogoutput"])
+
 				if "filters" in filedata[istr]:
 					base.debugmsg(9, "filedata[istr][filters]:", filedata[istr]["filters"], type(filedata[istr]["filters"]))
 					filtr = filedata[istr]["filters"].replace("'", '"')
 					base.debugmsg(9, "filtr:", filtr, type(filtr))
 					filtrs = json.loads(filtr)
 					base.debugmsg(9, "filtrs:", filtrs, type(filtrs))
 					base.scriptlist[ii]["filters"] = filtrs
@@ -3000,14 +3079,59 @@
 										tr = base.testrepeaterdefault
 										if "testrepeater" in base.scriptdefaults:
 											tr = base.scriptdefaults["testrepeater"]
 										if "testrepeater" in grp:
 											tr = grp["testrepeater"]
 										base.robot_schedule["Agents"][nxtagent][grurid]["testrepeater"] = str(tr)
 
+										# injectsleepenableddefault = False
+										ise = base.injectsleepenableddefault
+										if "injectsleepenabled" in base.scriptdefaults:
+											ise = base.scriptdefaults["injectsleepenabled"]
+										if "injectsleepenabled" in grp:
+											ise = grp["injectsleepenabled"]
+										base.robot_schedule["Agents"][nxtagent][grurid]["injectsleepenabled"] = str(ise)
+										if base.str2bool(ise):
+											# injectsleepminimumdefault = 15
+											ismn = base.injectsleepminimumdefault
+											if "injectsleepminimum" in base.scriptdefaults:
+												ismn = base.scriptdefaults["injectsleepminimum"]
+											if "injectsleepminimum" in grp:
+												ismn = grp["injectsleepminimum"]
+											base.robot_schedule["Agents"][nxtagent][grurid]["injectsleepminimum"] = str(ismn)
+											# injectsleepmaximumdefault = 45
+											ismx = base.injectsleepmaximumdefault
+											if "injectsleepmaximum" in base.scriptdefaults:
+												ismx = base.scriptdefaults["injectsleepmaximum"]
+											if "injectsleepmaximum" in grp:
+												ismx = grp["injectsleepmaximum"]
+											base.robot_schedule["Agents"][nxtagent][grurid]["injectsleepmaximum"] = str(ismx)
+
+										# disableloglogdefault = False
+										dll = base.disableloglogdefault
+										if "disableloglog" in base.scriptdefaults:
+											dll = base.scriptdefaults["disableloglog"]
+										if "disableloglog" in grp:
+											dll = grp["disableloglog"]
+										base.robot_schedule["Agents"][nxtagent][grurid]["disableloglog"] = str(dll)
+										# disablelogreportdefault = False
+										dlr = base.disablelogreportdefault
+										if "disablelogreport" in base.scriptdefaults:
+											dlr = base.scriptdefaults["disablelogreport"]
+										if "disablelogreport" in grp:
+											dlr = grp["disablelogreport"]
+										base.robot_schedule["Agents"][nxtagent][grurid]["disablelogreport"] = str(dlr)
+										# disablelogoutputdefault = False
+										dlo = base.disablelogoutputdefault
+										if "disablelogoutput" in base.scriptdefaults:
+											dlo = base.scriptdefaults["disablelogoutput"]
+										if "disablelogoutput" in grp:
+											dlo = grp["disablelogoutput"]
+										base.robot_schedule["Agents"][nxtagent][grurid]["disablelogoutput"] = str(dlo)
+
 										base.Agents[nxtagent]["AssignedRobots"] += 1
 										base.debugmsg(5, "base.Agents[", nxtagent, "][AssignedRobots]:", base.Agents[nxtagent]["AssignedRobots"])
 
 										currbts += 1
 										base.debugmsg(2, "Robot:", currbts, "	Test:", grp["Test"], "	Assigned to:", nxtagent)
 
 										base.debugmsg(9, "robot_schedule", base.robot_schedule)
@@ -3085,30 +3209,29 @@
 		if args:
 			scriptfile = args[0]
 		else:
 			scriptfile = ""
 		base.debugmsg(7, "scriptfile:", scriptfile)
 		if len(scriptfile) > 0:
 			base.scriptlist[r]["Script"] = scriptfile
-			script_hash = base.hash_file(scriptfile, os.path.basename(scriptfile))
+			relpath = base.get_relative_path(base.config['Plan']['ScriptDir'], scriptfile)
+			script_hash = base.hash_file(scriptfile, relpath)
 			base.scriptlist[r]["ScriptHash"] = script_hash
 
 			if script_hash not in base.scriptfiles:
 				base.scriptfiles[script_hash] = {
 					"id": script_hash,
 					"localpath": scriptfile,
-					"relpath": os.path.basename(scriptfile),
+					"relpath": relpath,
 					"type": "script"
 				}
 
 				t = threading.Thread(target=base.find_dependancies, args=(script_hash, ))
 				t.start()
 
-			base.config['Plan']['ScriptDir'] = base.inisafevalue(os.path.dirname(scriptfile))
-			base.saveini()
 		else:
 			if "ScriptHash" in base.scriptlist[r]:
 				oldhash = base.scriptlist[r]["ScriptHash"]
 				t = threading.Thread(target=base.remove_hash, args=(oldhash, ))
 				t.start()
 
 			base.scriptlist[r]["Script"] = ''
@@ -4542,15 +4665,15 @@
 						grphWindow.axis.legend(loc='upper center', bbox_to_anchor=(0.5, -0.15), ncol=2)
 
 					grphWindow.fig.set_tight_layout(True)
 					grphWindow.fig.autofmt_xdate(bottom=0.2, rotation=30, ha='right')
 					try:
 						grphWindow.canvas.draw()
 					except Exception as e:
-						base.debugmsg(5, "canvas.draw() Exception:", e)
+						base.debugmsg(9, "canvas.draw() Exception:", e)
 
 			self.gph_save(grphWindow)
 
 			self.RefreshRecentGraphs()
 
 	def gs_refresh(self, grphWindow):
 		base.debugmsg(6, "start")
@@ -4969,14 +5092,52 @@
 
 		setingsWindow.testrepeaterdefault = base.testrepeaterdefault
 		setingsWindow.testrepeatercurrent = setingsWindow.testrepeaterdefault
 		if "testrepeater" in base.scriptdefaults:
 			setingsWindow.testrepeatercurrent = base.str2bool(base.scriptdefaults["testrepeater"])
 		base.debugmsg(5, "testrepeatercurrent:", setingsWindow.testrepeatercurrent)
 
+		# injectsleepenableddefault = False
+		setingsWindow.injectsleepenableddefault = base.injectsleepenableddefault
+		setingsWindow.injectsleepenabled = setingsWindow.injectsleepenableddefault
+		if "injectsleepenabled" in base.scriptdefaults:
+			setingsWindow.injectsleepenabled = base.scriptdefaults["injectsleepenabled"]
+		base.debugmsg(5, "injectsleepenabled:", setingsWindow.injectsleepenabled)
+		# injectsleepminimumdefault = 15
+		setingsWindow.injectsleepminimumdefault = int(base.injectsleepminimumdefault)
+		setingsWindow.injectsleepminimum = setingsWindow.injectsleepminimumdefault
+		if "injectsleepminimum" in base.scriptdefaults and len(base.scriptdefaults["injectsleepminimum"]) > 0:
+			setingsWindow.injectsleepminimum = int(base.scriptdefaults["injectsleepminimum"])
+		base.debugmsg(5, "injectsleepminimum:", setingsWindow.injectsleepminimum)
+		# injectsleepmaximumdefault = 45
+		setingsWindow.injectsleepmaximumdefault = int(base.injectsleepmaximumdefault)
+		setingsWindow.injectsleepmaximum = setingsWindow.injectsleepmaximumdefault
+		if "injectsleepmaximum" in base.scriptdefaults and len(base.scriptdefaults["injectsleepmaximum"]) > 0:
+			setingsWindow.injectsleepmaximum = int(base.scriptdefaults["injectsleepmaximum"])
+		base.debugmsg(5, "injectsleepmaximum:", setingsWindow.injectsleepmaximum)
+
+		# disableloglogdefault = False
+		setingsWindow.disableloglogdefault = base.disableloglogdefault
+		setingsWindow.disableloglog = setingsWindow.disableloglogdefault
+		if "disableloglog" in base.scriptdefaults:
+			setingsWindow.disableloglog = base.scriptdefaults["disableloglog"]
+		base.debugmsg(5, "disableloglog:", setingsWindow.disableloglog)
+		# disablelogreportdefault = False
+		setingsWindow.disablelogreportdefault = base.disablelogreportdefault
+		setingsWindow.disablelogreport = setingsWindow.disablelogreportdefault
+		if "disablelogreport" in base.scriptdefaults:
+			setingsWindow.disablelogreport = base.scriptdefaults["disablelogreport"]
+		base.debugmsg(5, "disablelogreport:", setingsWindow.disablelogreport)
+		# disablelogoutputdefault = False
+		setingsWindow.disablelogoutputdefault = base.disablelogoutputdefault
+		setingsWindow.disablelogoutput = setingsWindow.disablelogoutputdefault
+		if "disablelogoutput" in base.scriptdefaults:
+			setingsWindow.disablelogoutput = base.scriptdefaults["disablelogoutput"]
+		base.debugmsg(5, "disablelogoutput:", setingsWindow.disablelogoutput)
+
 		# # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 		# Scenario
 		#
 		fmerow = 0
 
 		setingsWindow.fmeScenario = tk.Frame(setingsWindow.fmeContent)
 		# setingsWindow.fmeScenario.config(bg="blue")
@@ -5009,14 +5170,23 @@
 		setingsWindow.fmeTestDefaults = tk.Frame(setingsWindow.fmeContent)
 		# setingsWindow.fmeScenario.config(bg="blue")
 		setingsWindow.fmeTestDefaults.config(bd=1, relief="sunken")
 		# setingsWindow.fmeScenario.config(bd=1, relief="groove")
 		setingsWindow.fmeTestDefaults.grid(column=0, row=fmerow, sticky="nsew")
 
 		setingsWindow.fmeTestDefaults.columnconfigure(1, weight=1)
+		setingsWindow.fmeTestDefaults.columnconfigure(2, weight=1)
+		setingsWindow.fmeTestDefaults.columnconfigure(3, weight=1)
+		setingsWindow.fmeTestDefaults.columnconfigure(4, weight=1)
+		setingsWindow.fmeTestDefaults.columnconfigure(5, weight=1)
+		setingsWindow.fmeTestDefaults.columnconfigure(6, weight=1)
+		setingsWindow.fmeTestDefaults.columnconfigure(7, weight=1)
+		setingsWindow.fmeTestDefaults.columnconfigure(8, weight=1)
+		setingsWindow.fmeTestDefaults.columnconfigure(9, weight=1)
+		setingsWindow.fmeTestDefaults.columnconfigure(10, weight=1)
 
 		# [Server]
 		rownum += 0
 		setingsWindow.lblTestDefaults = ttk.Label(setingsWindow.fmeTestDefaults, text="Test Defaults:")
 		setingsWindow.lblTestDefaults.grid(column=0, row=rownum, sticky="nsew")
 
 		rownum += 1
@@ -5042,14 +5212,68 @@
 		setingsWindow.lblTR.grid(column=0, row=rownum, sticky="nsew")
 
 		setingsWindow.boolTR = tk.BooleanVar()
 		setingsWindow.boolTR.set(setingsWindow.testrepeatercurrent)
 		setingsWindow.inpTR = tk.Checkbutton(setingsWindow.fmeTestDefaults, variable=setingsWindow.boolTR, onvalue=True, offvalue=False)
 		setingsWindow.inpTR.grid(column=1, row=rownum, sticky="nsew")
 
+		rownum += 1
+		setingsWindow.lblIS = ttk.Label(setingsWindow.fmeTestDefaults, text="Inject Sleep:")
+		setingsWindow.lblIS.grid(column=0, row=rownum, sticky="nsew")
+
+		setingsWindow.lblISE = ttk.Label(setingsWindow.fmeTestDefaults, text="Enabled")
+		setingsWindow.lblISE.grid(column=1, row=rownum, sticky="nsew")
+		setingsWindow.lblISMN = ttk.Label(setingsWindow.fmeTestDefaults, text="Minimum")
+		setingsWindow.lblISMN.grid(column=2, row=rownum, sticky="nsew")
+		setingsWindow.lblISMX = ttk.Label(setingsWindow.fmeTestDefaults, text="Maximum")
+		setingsWindow.lblISMX.grid(column=3, row=rownum, sticky="nsew")
+
+		rownum += 1
+		setingsWindow.boolISE = tk.BooleanVar()
+		setingsWindow.boolISE.set(setingsWindow.injectsleepenabled)
+		setingsWindow.inpISE = tk.Checkbutton(setingsWindow.fmeTestDefaults, variable=setingsWindow.boolISE, onvalue=True, offvalue=False)
+		setingsWindow.inpISE.grid(column=1, row=rownum, sticky="nsew")
+
+		setingsWindow.inpISMN = ttk.Entry(setingsWindow.fmeTestDefaults, width=5, justify=tk.RIGHT)
+		setingsWindow.inpISMN.delete(0, 'end')
+		setingsWindow.inpISMN.insert(0, setingsWindow.injectsleepminimum)
+		setingsWindow.inpISMN.grid(column=2, row=rownum, sticky="nsew")
+
+		setingsWindow.inpISMX = ttk.Entry(setingsWindow.fmeTestDefaults, width=5, justify=tk.RIGHT)
+		setingsWindow.inpISMX.delete(0, 'end')
+		setingsWindow.inpISMX.insert(0, setingsWindow.injectsleepmaximum)
+		setingsWindow.inpISMX.grid(column=3, row=rownum, sticky="nsew")
+
+		rownum += 1
+		setingsWindow.lblDL = ttk.Label(setingsWindow.fmeTestDefaults, text="Disable Robot Logs:")
+		setingsWindow.lblDL.grid(column=0, row=rownum, sticky="nsew")
+
+		setingsWindow.lblDLL = ttk.Label(setingsWindow.fmeTestDefaults, text="log.html")
+		setingsWindow.lblDLL.grid(column=1, row=rownum, sticky="nsew")
+		setingsWindow.lblDLR = ttk.Label(setingsWindow.fmeTestDefaults, text="report.html")
+		setingsWindow.lblDLR.grid(column=2, row=rownum, sticky="nsew")
+		setingsWindow.lblDLO = ttk.Label(setingsWindow.fmeTestDefaults, text="output.xml")
+		setingsWindow.lblDLO.grid(column=3, row=rownum, sticky="nsew")
+
+		rownum += 1
+		setingsWindow.boolDLL = tk.BooleanVar()
+		setingsWindow.boolDLL.set(setingsWindow.disableloglog)
+		setingsWindow.inpDLL = tk.Checkbutton(setingsWindow.fmeTestDefaults, variable=setingsWindow.boolDLL, onvalue=True, offvalue=False)
+		setingsWindow.inpDLL.grid(column=1, row=rownum, sticky="nsew")
+
+		setingsWindow.boolDLR = tk.BooleanVar()
+		setingsWindow.boolDLR.set(setingsWindow.disablelogreport)
+		setingsWindow.inpDLR = tk.Checkbutton(setingsWindow.fmeTestDefaults, variable=setingsWindow.boolDLR, onvalue=True, offvalue=False)
+		setingsWindow.inpDLR.grid(column=2, row=rownum, sticky="nsew")
+
+		setingsWindow.boolDLO = tk.BooleanVar()
+		setingsWindow.boolDLO.set(setingsWindow.disablelogoutput)
+		setingsWindow.inpDLO = tk.Checkbutton(setingsWindow.fmeTestDefaults, variable=setingsWindow.boolDLO, onvalue=True, offvalue=False)
+		setingsWindow.inpDLO.grid(column=3, row=rownum, sticky="nsew")
+
 		# # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 		# Manager
 		#
 		fmerow += 1
 
 		setingsWindow.fmeServer = tk.Frame(setingsWindow.fmeContent)
 		# setingsWindow.fmeScenario.config(bg="blue")
@@ -5212,14 +5436,88 @@
 				base.scriptdefaults["testrepeater"] = str(tr)
 				self.plan_scnro_chngd = True
 			else:
 				if "testrepeater" in base.scriptdefaults:
 					del base.scriptdefaults["testrepeater"]
 					self.plan_scnro_chngd = True
 
+			# if "injectsleepenabled" in base.scriptdefaults:
+			# 	setingsWindow.injectsleepenabled = base.scriptdefaults["injectsleepenabled"]
+			ise = setingsWindow.boolISE.get()
+			base.debugmsg(5, "ise:", ise, "default:", setingsWindow.injectsleepenableddefault)
+			if ise != setingsWindow.injectsleepenableddefault:
+				base.scriptdefaults["injectsleepenabled"] = str(ise)
+				self.plan_scnro_chngd = True
+			else:
+				if "injectsleepenabled" in base.scriptdefaults:
+					del base.scriptdefaults["injectsleepenabled"]
+					self.plan_scnro_chngd = True
+
+			ismn = setingsWindow.inpISMN.get()
+			if len(ismn) > 0:
+				ismn = int(ismn)
+			else:
+				ismn = setingsWindow.injectsleepminimumdefault
+			base.debugmsg(5, "ismn:", ismn, "default:", setingsWindow.injectsleepminimumdefault, "type:", type(ismn), type(setingsWindow.injectsleepminimumdefault))
+			if ismn != setingsWindow.injectsleepminimumdefault:
+				base.debugmsg(5, "Save ismn:", ismn)
+				base.scriptdefaults["injectsleepminimum"] = str(ismn)
+				self.plan_scnro_chngd = True
+			else:
+				base.debugmsg(5, "remove ismn?:", ismn)
+				if "injectsleepminimum" in base.scriptdefaults:
+					base.debugmsg(5, "remove ismn:", ismn)
+					del base.scriptdefaults["injectsleepminimum"]
+					self.plan_scnro_chngd = True
+
+			ismx = setingsWindow.inpISMX.get()
+			if len(ismx) > 0:
+				ismx = int(ismx)
+			else:
+				ismx = setingsWindow.injectsleepmaximumdefault
+			base.debugmsg(5, "ismx:", ismx, "default:", setingsWindow.injectsleepmaximumdefault, "type:", type(ismx), type(setingsWindow.injectsleepmaximumdefault))
+			if ismx != setingsWindow.injectsleepmaximumdefault:
+				base.scriptdefaults["injectsleepmaximum"] = str(ismx)
+				self.plan_scnro_chngd = True
+			else:
+				if "injectsleepmaximum" in base.scriptdefaults:
+					del base.scriptdefaults["injectsleepmaximum"]
+					self.plan_scnro_chngd = True
+
+			# disableloglogdefault = False
+			dll = setingsWindow.boolDLL.get()
+			base.debugmsg(5, "dll:", dll, "default:", setingsWindow.disableloglogdefault)
+			if dll != setingsWindow.disableloglogdefault:
+				base.scriptdefaults["disableloglog"] = str(dll)
+				self.plan_scnro_chngd = True
+			else:
+				if "disableloglog" in base.scriptdefaults:
+					del base.scriptdefaults["disableloglog"]
+					self.plan_scnro_chngd = True
+			# disablelogreportdefault = False
+			dlr = setingsWindow.boolDLR.get()
+			base.debugmsg(5, "dlr:", dlr, "default:", setingsWindow.disablelogreportdefault)
+			if dlr != setingsWindow.disablelogreportdefault:
+				base.scriptdefaults["disablelogreport"] = str(dlr)
+				self.plan_scnro_chngd = True
+			else:
+				if "disablelogreport" in base.scriptdefaults:
+					del base.scriptdefaults["disablelogreport"]
+					self.plan_scnro_chngd = True
+			# disablelogoutputdefault = False
+			dlo = setingsWindow.boolDLO.get()
+			base.debugmsg(5, "dlo:", dlo, "default:", setingsWindow.disablelogoutputdefault)
+			if dlo != setingsWindow.disablelogoutputdefault:
+				base.scriptdefaults["disablelogoutput"] = str(dlo)
+				self.plan_scnro_chngd = True
+			else:
+				if "disablelogoutput" in base.scriptdefaults:
+					del base.scriptdefaults["disablelogoutput"]
+					self.plan_scnro_chngd = True
+
 			# # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 			# Manager
 			#
 			srvrestart = False
 			srvip = base.config['Server']['BindIP']
 			srvport = int(base.config['Server']['BindPort'])
 
@@ -5646,15 +5944,15 @@
 				self.axis.xaxis.set_major_formatter(xformatter)
 				self.fig.autofmt_xdate(bottom=0.2, rotation=30, ha='right')
 
 				self.canvas.draw()
 
 			self.pln_graph_update = False
 
-	def addScriptRow(self):
+	def addScriptRow(self, *args):
 		base.debugmsg(6, "addScriptRow")
 		row = base.scriptcount
 
 		colour = base.line_colour(base.scriptcount)
 		base.debugmsg(5, "colour:", colour)
 
 		idx = tk.Label(self.scriptgrid, text=str(base.scriptcount))
@@ -5701,15 +5999,15 @@
 		scrf = ttk.Button(fgf, image=self.imgdata[icontext], text="...", width=1)
 		scrf.config(command=lambda: self.sr_file_validate(row))
 		scrf.grid(column=1, row=0, sticky="nsew")
 		fgf.columnconfigure(scrf, weight=0)
 
 		base.scriptlist[row]["TestVar"] = tk.StringVar(value=base.scriptlist[row]["Test"], name="row{}".format(row))
 		base.scriptlist[row]["TestVar"].trace("w", self.sr_test_validate)
-		tst = ttk.OptionMenu(self.scriptgrid, base.scriptlist[row]["TestVar"], None, "test")
+		tst = ttk.OptionMenu(self.scriptgrid, base.scriptlist[row]["TestVar"], None, "test", command=lambda: self.sr_test_validate(row))
 		tst.config(width=20)
 		tst.grid(column=self.plancoltst, row=base.scriptcount, sticky="nsew")
 
 		icontext = "Advanced"
 		self.scriptgrid.columnconfigure(self.plancoladd, weight=0)
 		new = ttk.Button(self.scriptgrid, image=self.imgdata[icontext], text="Settings", command=lambda: self.sr_row_settings(row), width=1)
 		new.grid(column=self.plancolset, row=base.scriptcount, sticky="nsew")
@@ -5939,40 +6237,65 @@
 						initialdir=base.config['Plan']['ScriptDir'],
 						title="Select Robot Framework File",
 						filetypes=(("Robot Framework", "*.robot"), ("all files", "*.*"))
 					)
 				)
 			else:
 				scriptfile = ""
-		base.debugmsg(7, "scriptfile:", scriptfile)
+		base.debugmsg(5, "scriptfile:", scriptfile)
 		if len(scriptfile) > 0:
+			relpath = base.get_relative_path(base.config['Plan']['ScriptDir'], scriptfile)
+			base.debugmsg(5, "relpath:", relpath)
+
+			if ".." in relpath:
+				base.debugmsg(5, "do update relpath:", relpath)
+				base.debugmsg(5, "ScriptDir:", base.config['Plan']['ScriptDir'])
+				if base.config['Plan']['ScriptDir'] == base.dir_path:
+					base.config['Plan']['ScriptDir'] = os.path.basename(scriptfile)
+					base.debugmsg(5, "ScriptDir:", base.config['Plan']['ScriptDir'])
+					relpath = base.get_relative_path(base.config['Plan']['ScriptDir'], scriptfile)
+					base.debugmsg(5, "relpath:", relpath)
+				if len(base.scriptlist) > 1:
+					base.debugmsg(5, "base.scriptlist:", base.scriptlist)
+					filelst = [scriptfile]
+					for i in range(len(base.scriptlist)):
+						if "Script" in base.scriptlist[i]:
+							filelst.append(base.scriptlist[i]["Script"])
+					commonpath = os.path.commonpath(filelst)
+					base.debugmsg(5, "commonpath: ", commonpath)
+					base.config['Plan']['ScriptDir'] = base.inisafevalue(commonpath)
+					relpath = base.get_relative_path(base.config['Plan']['ScriptDir'], scriptfile)
+					# base.saveini()
+					for i in range(len(base.scriptlist)):
+						if "Script" in base.scriptlist[i]:
+							self.sr_file_validate(i, base.scriptlist[i]["Script"])
+
 			fg[1].configure(state='normal')
 			fg[1].select_clear()
 			fg[1].delete(0, 'end')
-			fg[1].insert(0, os.path.basename(scriptfile))
+			fg[1].insert(0, relpath)
 			fg[1].configure(state='readonly')
 
 			base.scriptlist[r]["Script"] = scriptfile
 			base.debugmsg(8, "test: ", fg[1].get())
-			script_hash = base.hash_file(scriptfile, os.path.basename(scriptfile))
+			script_hash = base.hash_file(scriptfile, relpath)
 			base.scriptlist[r]["ScriptHash"] = script_hash
 
+			base.debugmsg(5, "script_hash:", script_hash, " in scriptfiles?:", script_hash in base.scriptfiles)
 			if script_hash not in base.scriptfiles:
 				base.scriptfiles[script_hash] = {
 					"id": script_hash,
 					"localpath": scriptfile,
-					"relpath": os.path.basename(scriptfile),
+					"relpath": relpath,
 					"type": "script"
 				}
 
 				t = threading.Thread(target=base.find_dependancies, args=(script_hash, ))
 				t.start()
 
-			base.config['Plan']['ScriptDir'] = base.inisafevalue(os.path.dirname(scriptfile))
-			base.saveini()
 			self.sr_test_genlist(r)
 		else:
 			fg[1].configure(state='normal')
 			fg[1].delete(0, 'end')
 			# fg[1].select_clear()
 			fg[1].configure(state='readonly')
 			if "ScriptHash" in base.scriptlist[r]:
@@ -6090,14 +6413,23 @@
 		# well it didn't work on macosx but it may help, i'll leave it for now
 		# stgsWindow.transient()
 		# stgsWindow.transient(parent=self.root)
 		# Now it works :)
 		stgsWindow.transient(self.root)
 
 		stgsWindow.columnconfigure(0, weight=1)
+		stgsWindow.columnconfigure(1, weight=1)
+		stgsWindow.columnconfigure(2, weight=1)
+		stgsWindow.columnconfigure(3, weight=1)
+		stgsWindow.columnconfigure(4, weight=1)
+		stgsWindow.columnconfigure(5, weight=1)
+		stgsWindow.columnconfigure(6, weight=1)
+		stgsWindow.columnconfigure(7, weight=1)
+		stgsWindow.columnconfigure(8, weight=1)
+		stgsWindow.columnconfigure(9, weight=1)
 		# stgsWindow.rowconfigure(1, weight=1)
 
 		stgsWindow.title("Settings for row {}".format(r))
 		testname = ""
 		try:
 			testname = base.scriptlist[r]["TestVar"].get()
 		except Exception:
@@ -6131,56 +6463,169 @@
 			stgsWindow.testrepeaterdefault = base.str2bool(base.scriptdefaults["testrepeater"])
 
 		stgsWindow.testrepeatercurrent = stgsWindow.testrepeaterdefault
 		if "testrepeater" in base.scriptlist[r]:
 			stgsWindow.testrepeatercurrent = base.str2bool(base.scriptlist[r]["testrepeater"])
 		base.debugmsg(5, "testrepeatercurrent:", stgsWindow.testrepeatercurrent)
 
+		stgsWindow.injectsleepenableddefault = base.injectsleepenableddefault
+		if "injectsleepenabled" in base.scriptdefaults:
+			stgsWindow.injectsleepenableddefault = base.str2bool(base.scriptdefaults["injectsleepenabled"])
+		stgsWindow.injectsleepenabled = stgsWindow.injectsleepenableddefault
+		if "injectsleepenabled" in base.scriptlist[r]:
+			stgsWindow.injectsleepenabled = base.str2bool(base.scriptlist[r]["injectsleepenabled"])
+		base.debugmsg(5, "injectsleepenabled:", stgsWindow.injectsleepenabled)
+
+		stgsWindow.injectsleepminimumdefault = base.injectsleepminimumdefault
+		if "injectsleepminimum" in base.scriptdefaults:
+			stgsWindow.injectsleepminimumdefault = int(base.scriptdefaults["injectsleepminimum"])
+		stgsWindow.injectsleepminimum = stgsWindow.injectsleepminimumdefault
+		if "injectsleepminimum" in base.scriptlist[r]:
+			stgsWindow.injectsleepminimum = int(base.scriptlist[r]["injectsleepminimum"])
+		base.debugmsg(5, "injectsleepminimum:", stgsWindow.injectsleepminimum)
+
+		stgsWindow.injectsleepmaximumdefault = base.injectsleepmaximumdefault
+		if "injectsleepmaximum" in base.scriptdefaults:
+			stgsWindow.injectsleepmaximumdefault = int(base.scriptdefaults["injectsleepmaximum"])
+		stgsWindow.injectsleepmaximum = stgsWindow.injectsleepmaximumdefault
+		if "injectsleepmaximum" in base.scriptlist[r]:
+			stgsWindow.injectsleepmaximum = int(base.scriptlist[r]["injectsleepmaximum"])
+		base.debugmsg(5, "injectsleepmaximum:", stgsWindow.injectsleepmaximum)
+
+		# disableloglogdefault = False
+		stgsWindow.disableloglogdefault = base.disableloglogdefault
+		if "disableloglog" in base.scriptdefaults:
+			stgsWindow.disableloglogdefault = base.str2bool(base.scriptdefaults["disableloglog"])
+		stgsWindow.disableloglog = stgsWindow.disableloglogdefault
+		if "disableloglog" in base.scriptlist[r]:
+			stgsWindow.disableloglog = base.str2bool(base.scriptlist[r]["disableloglog"])
+		base.debugmsg(5, "disableloglog:", stgsWindow.disableloglog)
+
+		# disablelogreportdefault = False
+		stgsWindow.disablelogreportdefault = base.disablelogreportdefault
+		if "disablelogreport" in base.scriptdefaults:
+			stgsWindow.disablelogreportdefault = base.str2bool(base.scriptdefaults["disablelogreport"])
+		stgsWindow.disablelogreport = stgsWindow.disablelogreportdefault
+		if "disablelogreport" in base.scriptlist[r]:
+			stgsWindow.disablelogreport = base.str2bool(base.scriptlist[r]["disablelogreport"])
+		base.debugmsg(5, "disablelogreport:", stgsWindow.disablelogreport)
+
+		# disablelogoutputdefault = False
+		stgsWindow.disablelogoutputdefault = base.disablelogoutputdefault
+		if "disablelogoutput" in base.scriptdefaults:
+			stgsWindow.disablelogoutputdefault = base.str2bool(base.scriptdefaults["disablelogoutput"])
+		stgsWindow.disablelogoutput = stgsWindow.disablelogoutputdefault
+		if "disablelogoutput" in base.scriptlist[r]:
+			stgsWindow.disablelogoutput = base.str2bool(base.scriptlist[r]["disablelogoutput"])
+		base.debugmsg(5, "disablelogoutput:", stgsWindow.disablelogoutput)
+
 		row = 0
-		stgsWindow.lblBLNK = ttk.Label(stgsWindow, text=" ")	 # just a blank row as a spacer before the filters
+		stgsWindow.lblBLNK = ttk.Label(stgsWindow, text=" ")	 # just a blank row as a spacer
 		stgsWindow.lblBLNK.grid(column=0, row=row, sticky="nsew")
 
 		row += 1
 		stgsWindow.lblEL = ttk.Label(stgsWindow, text="Exclude libraries:")
 		stgsWindow.lblEL.grid(column=0, row=row, sticky="nsew")
 
 		row += 1
 		stgsWindow.inpEL = ttk.Entry(stgsWindow)
 		stgsWindow.inpEL.delete(0, 'end')
 		stgsWindow.inpEL.insert(0, stgsWindow.excludelibrariescurrent)
 		stgsWindow.inpEL.grid(column=0, row=row, columnspan=10, sticky="nsew")
 
 		row += 1
-		stgsWindow.lblBLNK = ttk.Label(stgsWindow, text=" ")	 # just a blank row as a spacer before the filters
+		stgsWindow.lblBLNK = ttk.Label(stgsWindow, text=" ")	 # just a blank row as a spacer
 		stgsWindow.lblBLNK.grid(column=0, row=row, sticky="nsew")
 
 		row += 1
 		stgsWindow.lblRO = ttk.Label(stgsWindow, text="Robot Options:")
 		stgsWindow.lblRO.grid(column=0, row=row, sticky="nsew")
 
 		row += 1
 		stgsWindow.inpRO = ttk.Entry(stgsWindow)
 		stgsWindow.inpRO.delete(0, 'end')
 		stgsWindow.inpRO.insert(0, stgsWindow.robotoptionscurrent)
 		stgsWindow.inpRO.grid(column=0, row=row, columnspan=10, sticky="nsew")
 
 		row += 1
-		stgsWindow.lblBLNK = ttk.Label(stgsWindow, text=" ")	 # just a blank row as a spacer before the filters
+		stgsWindow.lblBLNK = ttk.Label(stgsWindow, text=" ")	 # just a blank row as a spacer
 		stgsWindow.lblBLNK.grid(column=0, row=row, sticky="nsew")
 
 		row += 1
 		stgsWindow.lblTR = ttk.Label(stgsWindow, text="Test Repeater:")
 		stgsWindow.lblTR.grid(column=0, row=row, sticky="nsew")
 
 		stgsWindow.boolTR = tk.BooleanVar()
 		stgsWindow.boolTR.set(stgsWindow.testrepeatercurrent)
 		stgsWindow.inpTR = tk.Checkbutton(stgsWindow, variable=stgsWindow.boolTR, onvalue=True, offvalue=False)
 		stgsWindow.inpTR.grid(column=1, row=row, sticky="nsew")
 
 		row += 1
+		stgsWindow.lblBLNK = ttk.Label(stgsWindow, text=" ")	 # just a blank row as a spacer
+		stgsWindow.lblBLNK.grid(column=0, row=row, sticky="nsew")
+
+		row += 1
+		stgsWindow.lblIS = ttk.Label(stgsWindow, text="Inject Sleep:")
+		stgsWindow.lblIS.grid(column=0, row=row, sticky="nsew")
+
+		stgsWindow.lblISE = ttk.Label(stgsWindow, text="Enabled")
+		stgsWindow.lblISE.grid(column=1, row=row, sticky="nsew")
+		stgsWindow.lblISMN = ttk.Label(stgsWindow, text="Minimum")
+		stgsWindow.lblISMN.grid(column=2, row=row, sticky="nsew")
+		stgsWindow.lblISMX = ttk.Label(stgsWindow, text="Maximum")
+		stgsWindow.lblISMX.grid(column=3, row=row, sticky="nsew")
+
+		row += 1
+		stgsWindow.boolISE = tk.BooleanVar()
+		stgsWindow.boolISE.set(stgsWindow.injectsleepenabled)
+		stgsWindow.inpISE = tk.Checkbutton(stgsWindow, variable=stgsWindow.boolISE, onvalue=True, offvalue=False)
+		stgsWindow.inpISE.grid(column=1, row=row, sticky="nsew")
+
+		stgsWindow.inpISMN = ttk.Entry(stgsWindow, width=5, justify=tk.RIGHT)
+		stgsWindow.inpISMN.delete(0, 'end')
+		stgsWindow.inpISMN.insert(0, stgsWindow.injectsleepminimum)
+		stgsWindow.inpISMN.grid(column=2, row=row, sticky="nsew")
+
+		stgsWindow.inpISMX = ttk.Entry(stgsWindow, width=5, justify=tk.RIGHT)
+		stgsWindow.inpISMX.delete(0, 'end')
+		stgsWindow.inpISMX.insert(0, stgsWindow.injectsleepmaximum)
+		stgsWindow.inpISMX.grid(column=3, row=row, sticky="nsew")
+
+		row += 1
+		stgsWindow.lblBLNK = ttk.Label(stgsWindow, text=" ")	 # just a blank row as a spacer
+		stgsWindow.lblBLNK.grid(column=0, row=row, sticky="nsew")
+
+		row += 1
+		stgsWindow.lblDL = ttk.Label(stgsWindow, text="Disable Robot Log:")
+		stgsWindow.lblDL.grid(column=0, row=row, sticky="nsew")
+
+		stgsWindow.lblDLL = ttk.Label(stgsWindow, text="log.html")
+		stgsWindow.lblDLL.grid(column=1, row=row, sticky="nsew")
+		stgsWindow.lblDLR = ttk.Label(stgsWindow, text="report.html")
+		stgsWindow.lblDLR.grid(column=2, row=row, sticky="nsew")
+		stgsWindow.lblDLO = ttk.Label(stgsWindow, text="output.xml")
+		stgsWindow.lblDLO.grid(column=3, row=row, sticky="nsew")
+
+		row += 1
+		stgsWindow.boolDLL = tk.BooleanVar()
+		stgsWindow.boolDLL.set(stgsWindow.disableloglog)
+		stgsWindow.inpDLL = tk.Checkbutton(stgsWindow, variable=stgsWindow.boolDLL, onvalue=True, offvalue=False)
+		stgsWindow.inpDLL.grid(column=1, row=row, sticky="nsew")
+
+		stgsWindow.boolDLR = tk.BooleanVar()
+		stgsWindow.boolDLR.set(stgsWindow.disablelogreport)
+		stgsWindow.inpDLR = tk.Checkbutton(stgsWindow, variable=stgsWindow.boolDLR, onvalue=True, offvalue=False)
+		stgsWindow.inpDLR.grid(column=2, row=row, sticky="nsew")
+
+		stgsWindow.boolDLO = tk.BooleanVar()
+		stgsWindow.boolDLO.set(stgsWindow.disablelogoutput)
+		stgsWindow.inpDLO = tk.Checkbutton(stgsWindow, variable=stgsWindow.boolDLO, onvalue=True, offvalue=False)
+		stgsWindow.inpDLO.grid(column=3, row=row, sticky="nsew")
+
+		row += 1
 		stgsWindow.lblBLNK = ttk.Label(stgsWindow, text=" ")	 # just a blank row as a spacer before the filters
 		stgsWindow.lblBLNK.grid(column=0, row=row, sticky="nsew")
 
 		row += 1
 		stgsWindow.lblAF = ttk.Label(stgsWindow, text="Agent Filter:")
 		stgsWindow.lblAF.grid(column=0, row=row, sticky="nsew")
 
@@ -6246,14 +6691,86 @@
 			base.scriptlist[r]["testrepeater"] = str(tr)
 			self.plan_scnro_chngd = True
 		else:
 			if "testrepeater" in base.scriptlist[r]:
 				del base.scriptlist[r]["testrepeater"]
 				self.plan_scnro_chngd = True
 
+		# Inject Sleep
+		ise = stgsWindow.boolISE.get()
+		base.debugmsg(7, "ise:", ise)
+		if ise != stgsWindow.injectsleepenableddefault:
+			base.scriptlist[r]["injectsleepenabled"] = str(ise)
+			self.plan_scnro_chngd = True
+		else:
+			if "injectsleepenabled" in base.scriptlist[r]:
+				del base.scriptlist[r]["injectsleepenabled"]
+				self.plan_scnro_chngd = True
+
+		ismn = stgsWindow.inpISMN.get()
+		if len(ismn) > 0:
+			ismn = int(ismn)
+		else:
+			ismn = stgsWindow.injectsleepminimumdefault
+		base.debugmsg(7, "ismn:", ismn)
+		if ismn != stgsWindow.injectsleepminimumdefault:
+			base.scriptlist[r]["injectsleepminimum"] = str(ismn)
+			self.plan_scnro_chngd = True
+		else:
+			if "injectsleepminimum" in base.scriptlist[r]:
+				del base.scriptlist[r]["injectsleepminimum"]
+				self.plan_scnro_chngd = True
+
+		ismx = stgsWindow.inpISMX.get()
+		if len(ismx) > 0:
+			ismx = int(ismx)
+		else:
+			ismx = stgsWindow.injectsleepmaximumdefault
+		base.debugmsg(7, "ismx:", ismx)
+		if ismx != stgsWindow.injectsleepmaximumdefault:
+			base.scriptlist[r]["injectsleepmaximum"] = str(ismx)
+			self.plan_scnro_chngd = True
+		else:
+			if "injectsleepmaximum" in base.scriptlist[r]:
+				del base.scriptlist[r]["injectsleepmaximum"]
+				self.plan_scnro_chngd = True
+
+		# disableloglogdefault = False
+		dll = stgsWindow.boolDLL.get()
+		base.debugmsg(7, "ise:", ise)
+		if dll != stgsWindow.disableloglogdefault:
+			base.scriptlist[r]["disableloglog"] = str(dll)
+			self.plan_scnro_chngd = True
+		else:
+			if "disableloglog" in base.scriptlist[r]:
+				del base.scriptlist[r]["disableloglog"]
+				self.plan_scnro_chngd = True
+
+		# disablelogreportdefault = False
+		dlr = stgsWindow.boolDLR.get()
+		base.debugmsg(7, "ise:", ise)
+		if dlr != stgsWindow.disablelogreportdefault:
+			base.scriptlist[r]["disablelogreport"] = str(dlr)
+			self.plan_scnro_chngd = True
+		else:
+			if "disablelogreport" in base.scriptlist[r]:
+				del base.scriptlist[r]["disablelogreport"]
+				self.plan_scnro_chngd = True
+
+		# disablelogoutputdefault = False
+		dlo = stgsWindow.boolDLO.get()
+		base.debugmsg(7, "ise:", ise)
+		if dlo != stgsWindow.disablelogoutputdefault:
+			base.scriptlist[r]["disablelogoutput"] = str(dlo)
+			self.plan_scnro_chngd = True
+		else:
+			if "disablelogoutput" in base.scriptlist[r]:
+				del base.scriptlist[r]["disablelogoutput"]
+				self.plan_scnro_chngd = True
+
 		base.debugmsg(7, "stgsWindow.Filters:", stgsWindow.Filters)
 		if len(stgsWindow.Filters.keys()) > 0:
 			base.scriptlist[r]["filters"] = []
 			for fil in stgsWindow.Filters.keys():
 				filtr = {}
 				filtr["rule"] = stgsWindow.Filters[fil]["FilRule"].get()
 				filtr["optn"] = stgsWindow.Filters[fil]["FilOpt"].get()
@@ -7029,14 +7546,18 @@
 			don_gh = tk.Label(ab, text="Github", fg="blue", cursor="hand2")
 			don_gh.grid(column=0, row=aboutrow, sticky="nsew")
 			don_gh.bind("<Button-1>", lambda e: self.openweblink("https://github.com/sponsors/damies13/"))
 			# PayPal.me
 			don_pp = tk.Label(ab, text="PayPal", fg="blue", cursor="hand2")
 			don_pp.grid(column=1, row=aboutrow, sticky="nsew")
 			don_pp.bind("<Button-1>", lambda e: self.openweblink("https://paypal.me/damies13/5"))
+			# sponsors
+			don_sp = tk.Label(ab, text="Sponsors", fg="blue", cursor="hand2")
+			don_sp.grid(column=2, row=aboutrow, sticky="nsew")
+			don_sp.bind("<Button-1>", lambda e: self.openweblink("https://github.com/damies13/rfswarm/blob/master/Doc/Sponsors.md"))
 
 			aboutrow += 1
 			ab.rowconfigure(aboutrow, weight=1)
 			aboutrow += 1
 			ab.rowconfigure(aboutrow, weight=1)
 
 	# # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
```

### Comparing `rfswarm-manager-1.2.1/rfswarm_manager.egg-info/PKG-INFO` & `rfswarm_manager-1.3.0/rfswarm_manager.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: rfswarm-manager
-Version: 1.2.1
+Version: 1.3.0
 Summary: rfswarm manager
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
-License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
 Project-URL: Source, https://github.com/damies13/rfswarm
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: configparser
+Requires-Dist: HTTPServer
+Requires-Dist: pillow>=9.1.0
+Requires-Dist: psutil
+Requires-Dist: pip>=21,>=22
+Requires-Dist: matplotlib
+Requires-Dist: requests
 
 # rfswarm (Robot Framework Swarm)
 
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
@@ -54,9 +59,7 @@
 
 
 ## Donations
 
 If you would like to thank me for this project please consider using one of the sponsorship methods:
 - [GitHub](https://github.com/sponsors/damies13/)
 - [PayPal.me](https://paypal.me/damies13/5) (the $5 is a suggestion, feel free to change to any amount you would like)
-
-
```

### Comparing `rfswarm-manager-1.2.1/setup-manager.py` & `rfswarm_manager-1.3.0/setup-manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_PyPi.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="rfswarm-manager",
-	version="1.2.1",
+	version="1.3.0",
 	author="damies13",
 	author_email="damies13+rfswarm@gmail.com",
 	description="rfswarm manager",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/damies13/rfswarm",
 	packages=setuptools.find_packages(exclude=["*fswarm_report*", "*fswarm_agen*", "build/*"]),
```

