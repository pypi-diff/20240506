# Comparing `tmp/rfswarm-reporter-1.2.1.tar.gz` & `tmp/rfswarm_reporter-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfswarm-reporter-1.2.1.tar", last modified: Mon Feb 19 03:36:33 2024, max compression
+gzip compressed data, was "rfswarm_reporter-1.3.0.tar", last modified: Mon May  6 03:03:29 2024, max compression
```

## Comparing `rfswarm-reporter-1.2.1.tar` & `rfswarm_reporter-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,16 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2024-02-19 03:36:33.919990 rfswarm-reporter-1.2.1/
--rw-r--r--   0 dave       (501) staff       (20)    35149 2019-11-02 13:28:40.000000 rfswarm-reporter-1.2.1/LICENSE
--rw-r--r--   0 dave       (501) staff       (20)     3158 2024-02-19 03:36:33.919647 rfswarm-reporter-1.2.1/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)     6597 2024-02-02 01:15:20.000000 rfswarm-reporter-1.2.1/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2024-02-19 03:36:33.910826 rfswarm-reporter-1.2.1/rfswarm_reporter/
--rw-r--r--   0 dave       (501) staff       (20)       53 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/rfswarm_reporter/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)   393034 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/rfswarm_reporter/rfswarm_reporter.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2024-02-19 03:36:33.913759 rfswarm-reporter-1.2.1/rfswarm_reporter.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)     3158 2024-02-19 03:36:33.000000 rfswarm-reporter-1.2.1/rfswarm_reporter.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      583 2024-02-19 03:36:33.000000 rfswarm-reporter-1.2.1/rfswarm_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2024-02-19 03:36:33.000000 rfswarm-reporter-1.2.1/rfswarm_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       80 2024-02-19 03:36:33.000000 rfswarm-reporter-1.2.1/rfswarm_reporter.egg-info/entry_points.txt
--rw-r--r--   0 dave       (501) staff       (20)       85 2024-02-19 03:36:33.000000 rfswarm-reporter-1.2.1/rfswarm_reporter.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       24 2024-02-19 03:36:33.000000 rfswarm-reporter-1.2.1/rfswarm_reporter.egg-info/top_level.txt
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2024-02-19 03:36:33.919098 rfswarm-reporter-1.2.1/robots/
--rw-r--r--   0 dave       (501) staff       (20)      818 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/robots/PythonListener.py
--rw-r--r--   0 dave       (501) staff       (20)      466 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/robots/RFSListener.py
--rw-r--r--   0 dave       (501) staff       (20)     3689 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/robots/RFSListener2.py
--rw-r--r--   0 dave       (501) staff       (20)       32 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/robots/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/robots/myLibrary.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/robots/myLibrary1.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/robots/myLibrary2.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/robots/myLibrary3.py
--rw-r--r--   0 dave       (501) staff       (20)      200 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/robots/myvariables.py
--rw-r--r--   0 dave       (501) staff       (20)     6843 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/robots/svg5.py
--rw-r--r--   0 dave       (501) staff       (20)     1863 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/robots/with_file_not_closed.py
--rw-r--r--   0 dave       (501) staff       (20)     1504 2024-02-19 03:36:30.000000 rfswarm-reporter-1.2.1/setup-reporter.py
--rw-r--r--   0 dave       (501) staff       (20)       38 2024-02-19 03:36:33.920124 rfswarm-reporter-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:03:29.903905 rfswarm_reporter-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 03:03:06.000000 rfswarm_reporter-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-06 03:03:29.903905 rfswarm_reporter-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-06 03:03:06.000000 rfswarm_reporter-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:03:29.899905 rfswarm_reporter-1.3.0/rfswarm_reporter/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 03:03:08.000000 rfswarm_reporter-1.3.0/rfswarm_reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   396738 2024-05-06 03:03:28.000000 rfswarm_reporter-1.3.0/rfswarm_reporter/rfswarm_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:03:29.903905 rfswarm_reporter-1.3.0/rfswarm_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-06 03:03:29.000000 rfswarm_reporter-1.3.0/rfswarm_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-06 03:03:29.000000 rfswarm_reporter-1.3.0/rfswarm_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 03:03:29.000000 rfswarm_reporter-1.3.0/rfswarm_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 03:03:29.000000 rfswarm_reporter-1.3.0/rfswarm_reporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 03:03:29.000000 rfswarm_reporter-1.3.0/rfswarm_reporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 03:03:29.000000 rfswarm_reporter-1.3.0/rfswarm_reporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-06 03:03:28.000000 rfswarm_reporter-1.3.0/setup-reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 03:03:29.903905 rfswarm_reporter-1.3.0/setup.cfg
```

### Comparing `rfswarm-reporter-1.2.1/LICENSE` & `rfswarm_reporter-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rfswarm-reporter-1.2.1/PKG-INFO` & `rfswarm_reporter-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: rfswarm-reporter
-Version: 1.2.1
+Version: 1.3.0
 Summary: rfswarm reporter
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
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: configparser
+Requires-Dist: pillow>=9.1.0
+Requires-Dist: pip>=21,>=22
+Requires-Dist: matplotlib
+Requires-Dist: python-docx
+Requires-Dist: openpyxl
+Requires-Dist: tzlocal>=4.1
+Requires-Dist: lxml
 
 # rfswarm (Robot Framework Swarm)
 
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
@@ -54,9 +60,7 @@
 
 
 ## Donations
 
 If you would like to thank me for this project please consider using one of the sponsorship methods:
 - [GitHub](https://github.com/sponsors/damies13/)
 - [PayPal.me](https://paypal.me/damies13/5) (the $5 is a suggestion, feel free to change to any amount you would like)
-
-
```

### Comparing `rfswarm-reporter-1.2.1/README.md` & `rfswarm_reporter-1.3.0/README.md`

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

### Comparing `rfswarm-reporter-1.2.1/rfswarm_reporter/rfswarm_reporter.py` & `rfswarm_reporter-1.3.0/rfswarm_reporter/rfswarm_reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 #
 # 	Robot Framework Swarm
 # 		Reporter
-#    Version 1.2.1
+#    Version 1.3.0
 #
 
 import argparse
 import base64  # used for embedding images  # used for xhtml export
 import configparser
 import difflib
 import glob
@@ -33,14 +33,15 @@
 import zoneinfo  # says Requires python 3.9
 from copy import copy  # used for xlsx export
 from datetime import datetime  # , timezone
 from io import BytesIO  # used for embedding images  # used for xhtml export
 from typing import Any
 
 import matplotlib  # required for matplot graphs
+import matplotlib.font_manager as font_manager
 import openpyxl  # used for xlsx export
 import tzlocal
 from docx import Document  # used for docx export
 from docx.enum.style import WD_STYLE_TYPE  # used for docx export
 from docx.enum.text import WD_ALIGN_PARAGRAPH  # used for docx export
 from docx.oxml.shared import OxmlElement, qn  # used for docx export
 from docx.shared import Cm, Pt, RGBColor  # used for docx export
@@ -116,15 +117,15 @@
 			base.debugmsg(8, "res:", res)
 			return res
 		except Exception as e:
 			base.debugmsg(5, "Exception:", e)
 
 
 class ReporterBase():
-	version="1.2.1"
+	version = "1.3.0"
 	debuglvl = 0
 
 	save_ini = True
 	running = True
 	displaygui = True
 	gui = None
 	darkmode = False
@@ -485,14 +486,45 @@
 
 		base.debugmsg(9, "format:", format)
 		tz = zoneinfo.ZoneInfo(base.rs_setting_get_timezone())
 		ftime = datetime.fromtimestamp(itime, tz).strftime(format)
 		base.debugmsg(9, "ftime:", ftime)
 		return ftime
 
+	def report_formateddatetimetosec(self, stime):
+		base.debugmsg(5, "stime:", stime)
+		try:
+			if len(stime) == 10 and stime.isdecimal():
+				return int(stime)
+
+			if len(stime) == 13 and stime.isdecimal():
+				return int(stime) / 1000
+
+			dformat = base.rs_setting_get_dateformat()
+			dformat = dformat.replace("yyyy", "%Y")
+			dformat = dformat.replace("yy", "%y")
+			dformat = dformat.replace("mm", "%m")
+			dformat = dformat.replace("dd", "%d")
+
+			tformat = base.rs_setting_get_timeformat()
+			tformat = tformat.replace("HH", "%H")
+			tformat = tformat.replace("h", "%I")
+			tformat = tformat.replace("MM", "%M")
+			tformat = tformat.replace("SS", "%S")
+			tformat = tformat.replace("AMPM", "%p")
+
+			tz = zoneinfo.ZoneInfo(base.rs_setting_get_timezone())
+
+			datetime_object = datetime.strptime(stime, "{} {}".format(dformat, tformat)).replace(tzinfo=tz)
+			base.debugmsg(5, "datetime_object:", datetime_object, datetime_object.timestamp())
+			return int(datetime_object.timestamp())
+		except Exception as e:
+			base.debugmsg(8, "e:", e)
+			return -1
+
 	#
 	# Report Settings
 	#
 	def rs_setting_get(self, name):
 		base.debugmsg(9, "name:", name)
 		if name in base.report["Report"]:
 			return base.whitespace_get_ini_value(base.report["Report"][name])
@@ -631,14 +663,28 @@
 		else:
 			return value
 
 	def rs_setting_get_timezone_list(self):
 		# ZI = zoneinfo.ZoneInfo(base.rs_setting_get_timezone())
 		return zoneinfo.available_timezones()
 
+	def rs_setting_get_starttime(self):
+		value = self.rs_setting_get_int('starttime')
+		if value < 1:
+			return self.report_starttime()
+		else:
+			return int(value)
+
+	def rs_setting_get_endtime(self):
+		value = self.rs_setting_get_int('endtime')
+		if value < 1:
+			return self.report_endtime()
+		else:
+			return int(value)
+
 	#
 	# Report Sections
 	#
 
 	def report_get_order(self, parent):
 		if parent == "TOP":
 			base.debugmsg(7, "template order:", base.report["Report"]["Order"])
@@ -1082,14 +1128,24 @@
 					# -- 		WHERE result_name GLOB 'OC3*'
 					lwhere.append("[" + colname + "] NOT GLOB '{}'".format(inpFP))
 				# "Not Regex"
 				if FNType == "Not Regex":
 					# -- 		WHERE result_name GLOB 'OC3*'
 					lwhere.append("[" + colname + "] NOT REGEXP '{}'".format(inpFP))
 
+			# Start Time
+			starttime = base.rs_setting_get_starttime()
+			if starttime > 0:
+				lwhere.append("end_time >= {}".format(starttime))
+
+			# End Time
+			endtime = base.rs_setting_get_endtime()
+			if endtime > 0:
+				lwhere.append("end_time <= {}".format(endtime))
+
 			i = 0
 			for iwhere in lwhere:
 				if i == 0:
 					sql += "WHERE {} ".format(iwhere)
 				else:
 					sql += "AND {} ".format(iwhere)
 				i += 1
@@ -1216,14 +1272,24 @@
 					for dispcol in mnamecolumns:
 						if len(fpwhere) > 1:
 							fpwhere += "AND "
 						fpwhere += "{} NOT REGEXP '{}'".format(dispcol, inpFP)
 					fpwhere += ")"
 					wherelst.append(fpwhere)
 
+			# Start Time
+			starttime = base.rs_setting_get_starttime()
+			if starttime > 0:
+				wherelst.append("MetricTime >= {}".format(starttime))
+
+			# End Time
+			endtime = base.rs_setting_get_endtime()
+			if endtime > 0:
+				wherelst.append("MetricTime <= {}".format(endtime))
+
 			# if isnum<1:
 			# 	mcolumns.append("MetricValue")
 			# 	if sc>0:
 			# 		mcolumns.append("count(MetricTime) as 'Count'")
 			# 		if "MetricValue" in grouplst:
 			# 			grouplst.remove("MetricValue")
 			# else:
@@ -1395,14 +1461,24 @@
 					# -- 		WHERE result_name GLOB 'OC3*'
 					lwhere.append("[" + colname + "] NOT GLOB '{}'".format(inpFP))
 				# "Not Regex"
 				if FNType == "Not Regex":
 					# -- 		WHERE result_name GLOB 'OC3*'
 					lwhere.append("[" + colname + "] NOT REGEXP '{}'".format(inpFP))
 
+			# Start Time
+			starttime = base.rs_setting_get_starttime()
+			if starttime > 0:
+				lwhere.append("end_time >= {}".format(starttime))
+
+			# End Time
+			endtime = base.rs_setting_get_endtime()
+			if endtime > 0:
+				lwhere.append("end_time <= {}".format(endtime))
+
 			i = 0
 			for iwhere in lwhere:
 				if i == 0:
 					sql += "WHERE {} ".format(iwhere)
 				else:
 					sql += "AND {} ".format(iwhere)
 				i += 1
@@ -1527,14 +1603,24 @@
 			else:
 				mcolumns.append("min(CAST(MetricValue AS NUMERIC)) AS 'Minimum'")
 				mcolumns.append("round(avg(CAST(MetricValue AS NUMERIC)),3) AS 'Average'")
 				mcolumns.append("round(percentile(CAST(MetricValue AS NUMERIC), {}),3) AS '{}%ile'".format(display_percentile, display_percentile))
 				mcolumns.append("max(CAST(MetricValue AS NUMERIC)) AS 'Maximum'")
 				mcolumns.append("round(stdev(CAST(MetricValue AS NUMERIC)),3) AS 'Std. Dev.'")
 
+			# Start Time
+			starttime = base.rs_setting_get_starttime()
+			if starttime > 0:
+				wherelst.append("MetricTime >= {}".format(starttime))
+
+			# End Time
+			endtime = base.rs_setting_get_endtime()
+			if endtime > 0:
+				wherelst.append("MetricTime <= {}".format(endtime))
+
 			sql = "SELECT "
 
 			i = 0
 			for col in mcolumns:
 				if i < 1:
 					sql += "{} ".format(col)
 				else:
@@ -1644,14 +1730,24 @@
 					# -- 		WHERE result_name GLOB 'OC3*'
 					lwhere.append("[" + colname + "] NOT GLOB '{}'".format(inpFP))
 				# "Not Regex"
 				if FNType == "Not Regex":
 					# -- 		WHERE result_name GLOB 'OC3*'
 					lwhere.append("[" + colname + "] NOT REGEXP '{}'".format(inpFP))
 
+			# Start Time
+			starttime = base.rs_setting_get_starttime()
+			if starttime > 0:
+				lwhere.append("r.end_time >= {}".format(starttime))
+
+			# End Time
+			endtime = base.rs_setting_get_endtime()
+			if endtime > 0:
+				lwhere.append("r.end_time <= {}".format(endtime))
+
 			i = 0
 			for iwhere in lwhere:
 				if i == 0:
 					sql += "WHERE {} ".format(iwhere)
 				else:
 					sql += "AND {} ".format(iwhere)
 				i += 1
@@ -2157,14 +2253,24 @@
 		# sql += ", r.* "
 		sql += ", mt.SecondaryMetric 'script' "
 		sql += ", mt.MetricValue 'test_name' "
 		# sql += ", mt.* "
 		sql += "FROM Results r "
 		sql += "LEFT JOIN MetricData mt on mt.PrimaryMetric = r.script_index AND mt.MetricType = 'Scenario_Test' "
 		sql += "WHERE r.result = 'FAIL' "
+
+		# Start Time
+		starttime = base.rs_setting_get_starttime()
+		if starttime > 0:
+			sql += "AND r.end_time >= {} ".format(starttime)
+		# End Time
+		endtime = base.rs_setting_get_endtime()
+		if endtime > 0:
+			sql += "AND r.end_time <= {} ".format(endtime)
+
 		# sql += "ORDER BY r.script_index, r.sequence "
 		sql += "ORDER BY [id] ASC "
 
 		base.debugmsg(8, "sql:", sql)
 		self.rt_errors_set_sql(id, sql)
 		return sql
 
@@ -2576,14 +2682,16 @@
 	t_export: Any = {}
 
 	def __init__(self, master=None):
 		base.debugmsg(0, "Robot Framework Swarm: Reporter")
 		base.debugmsg(0, "	Version", base.version)
 		signal.signal(signal.SIGINT, self.on_closing)
 
+		font_manager._get_fontconfig_fonts.cache_clear()
+
 		base.debugmsg(9, "ArgumentParser")
 		# Check for command line args
 		parser = argparse.ArgumentParser()
 		parser.add_argument('-g', '--debug', help='Set debug level, default level is 0')
 		parser.add_argument('-v', '--version', help='Display the version and exit', action='store_true')
 		parser.add_argument('-i', '--ini', help='path to alternate ini file')
 		parser.add_argument('-n', '--nogui', help='Don\'t display the GUI', action='store_true')
@@ -3032,22 +3140,22 @@
 			#
 			# Execution Date range
 			#
 			subtitle = etree.SubElement(thiselmt, 'div')
 			subtitle.set("class", "subtitle center")
 			execdr = ""
 			if base.rs_setting_get_int("showstarttime"):
-				iST = base.report_starttime()
+				iST = base.rs_setting_get_starttime()
 				fSD = "{}".format(base.report_formatdate(iST))
 				fST = "{}".format(base.report_formattime(iST))
 
 				execdr = "{} {}".format(fSD, fST)
 
 			if base.rs_setting_get_int("showendtime"):
-				iET = base.report_endtime()
+				iET = base.rs_setting_get_endtime()
 				fED = "{}".format(base.report_formatdate(iET))
 				fET = "{}".format(base.report_formattime(iET))
 
 				if not base.rs_setting_get_int("showstarttime"):
 					execdr = "{} {}".format(fED, fET)
 				else:
 					if fSD == fED:
@@ -3909,22 +4017,22 @@
 					r.add_picture(tlogo)
 					document.add_paragraph("", style='Cover Subtitle')
 			#
 			# Execution Date range
 			#
 			execdr = ""
 			if base.rs_setting_get_int("showstarttime"):
-				iST = base.report_starttime()
+				iST = base.rs_setting_get_starttime()
 				fSD = "{}".format(base.report_formatdate(iST))
 				fST = "{}".format(base.report_formattime(iST))
 
 				execdr = "{} {}".format(fSD, fST)
 
 			if base.rs_setting_get_int("showendtime"):
-				iET = base.report_endtime()
+				iET = base.rs_setting_get_endtime()
 				fED = "{}".format(base.report_formatdate(iET))
 				fET = "{}".format(base.report_formattime(iET))
 
 				if not base.rs_setting_get_int("showstarttime"):
 					execdr = "{} {}".format(fED, fET)
 				else:
 					if fSD == fED:
@@ -4899,22 +5007,22 @@
 			#
 			# Execution Date range
 			#
 			rownum = 20
 
 			execdr = ""
 			if base.rs_setting_get_int("showstarttime"):
-				iST = base.report_starttime()
+				iST = base.rs_setting_get_starttime()
 				fSD = "{}".format(base.report_formatdate(iST))
 				fST = "{}".format(base.report_formattime(iST))
 
 				execdr = "{} {}".format(fSD, fST)
 
 			if base.rs_setting_get_int("showendtime"):
-				iET = base.report_endtime()
+				iET = base.rs_setting_get_endtime()
 				fED = "{}".format(base.report_formatdate(iET))
 				fET = "{}".format(base.report_formattime(iET))
 
 				if not base.rs_setting_get_int("showstarttime"):
 					execdr = "{} {}".format(fED, fET)
 				else:
 					if fSD == fED:
@@ -6642,39 +6750,37 @@
 
 		# 		start time
 		rownum += 1
 		self.contentdata[id]["lblST"] = ttk.Label(self.contentdata[id]["Settings"], text="Start Time:")
 		self.contentdata[id]["lblST"].grid(column=0, row=rownum, sticky="nsew")
 
 		self.contentdata[id]["strST"] = tk.StringVar()
-
-		iST = base.report_starttime()
+		iST = base.rs_setting_get_starttime()
 		fST = "{} {}".format(base.report_formatdate(iST), base.report_formattime(iST))
-
 		self.contentdata[id]["strST"].set(fST)
-		self.contentdata[id]["eST"] = ttk.Label(self.contentdata[id]["Settings"], textvariable=self.contentdata[id]["strST"])
+
+		self.contentdata[id]["eST"] = ttk.Entry(self.contentdata[id]["Settings"], textvariable=self.contentdata[id]["strST"])
 		self.contentdata[id]["eST"].grid(column=1, row=rownum, sticky="nsew")
 
 		self.contentdata[id]["intST"] = tk.IntVar()
 		self.contentdata[id]["intST"].set(base.rs_setting_get_int("showstarttime"))
 		self.contentdata[id]["chkST"] = ttk.Checkbutton(self.contentdata[id]["Settings"], variable=self.contentdata[id]["intST"], command=self.cs_report_settings_update)
 		self.contentdata[id]["chkST"].grid(column=col_disp, row=rownum, sticky="nsew")
 
 		# 		end time
 		rownum += 1
 		self.contentdata[id]["lblET"] = ttk.Label(self.contentdata[id]["Settings"], text="End Time:")
 		self.contentdata[id]["lblET"].grid(column=0, row=rownum, sticky="nsew")
 
 		self.contentdata[id]["strET"] = tk.StringVar()
-
-		iET = base.report_endtime()
+		iET = base.rs_setting_get_endtime()
 		fET = "{} {}".format(base.report_formatdate(iET), base.report_formattime(iET))
-
 		self.contentdata[id]["strET"].set(fET)
-		self.contentdata[id]["eET"] = ttk.Label(self.contentdata[id]["Settings"], textvariable=self.contentdata[id]["strET"])
+
+		self.contentdata[id]["eET"] = ttk.Entry(self.contentdata[id]["Settings"], textvariable=self.contentdata[id]["strET"])
 		self.contentdata[id]["eET"].grid(column=1, row=rownum, sticky="nsew")
 
 		self.contentdata[id]["intET"] = tk.IntVar()
 		self.contentdata[id]["intET"].set(base.rs_setting_get_int("showendtime"))
 		self.contentdata[id]["chkET"] = ttk.Checkbutton(self.contentdata[id]["Settings"], variable=self.contentdata[id]["intET"], command=self.cs_report_settings_update)
 		self.contentdata[id]["chkET"].grid(column=col_disp, row=rownum, sticky="nsew")
 
@@ -6798,17 +6904,35 @@
 
 		if "strTF" in self.contentdata[id]:
 			base.rs_setting_set("timeformat", self.contentdata[id]["strTF"].get())
 
 		if "strTZ" in self.contentdata[id]:
 			base.rs_setting_set("timezone", self.contentdata[id]["strTZ"].get())
 
+		# strST
+		if "strST" in self.contentdata[id]:
+			st = self.contentdata[id]["strST"].get()
+			base.debugmsg(8, "st:", st)
+			ist = base.report_formateddatetimetosec(st)
+			base.debugmsg(8, "ist:", ist)
+			if ist > 0:
+				base.rs_setting_set_int("starttime", ist)
+
 		if "intST" in self.contentdata[id]:
 			base.rs_setting_set_int("showstarttime", self.contentdata[id]["intST"].get())
 
+		# strET
+		if "strET" in self.contentdata[id]:
+			et = self.contentdata[id]["strET"].get()
+			base.debugmsg(8, "et:", et)
+			iet = base.report_formateddatetimetosec(et)
+			base.debugmsg(8, "iet:", iet)
+			if iet > 0:
+				base.rs_setting_set_int("endtime", iet)
+
 		if "intET" in self.contentdata[id]:
 			base.rs_setting_set_int("showendtime", self.contentdata[id]["intET"].get())
 
 		if "strFont" in self.contentdata[id]:
 			base.rs_setting_set("font", self.contentdata[id]["strFont"].get())
 
 		if "intFontSz" in self.contentdata[id]:
@@ -8687,22 +8811,22 @@
 		#  top: 3	centre: 13	bottom:	23
 		rownum = 23
 
 		execdr = ""
 		fSD = ""
 
 		if base.rs_setting_get_int("showstarttime"):
-			iST = base.report_starttime()
+			iST = base.rs_setting_get_starttime()
 			fSD = "{}".format(base.report_formatdate(iST))
 			fST = "{}".format(base.report_formattime(iST))
 
 			execdr = "{} {}".format(fSD, fST)
 
 		if base.rs_setting_get_int("showendtime"):
-			iET = base.report_endtime()
+			iET = base.rs_setting_get_endtime()
 			fED = "{}".format(base.report_formatdate(iET))
 			fET = "{}".format(base.report_formattime(iET))
 
 			if not base.rs_setting_get_int("showstarttime"):
 				execdr = "{} {}".format(fED, fET)
 			else:
 				if fSD == fED:
```

### Comparing `rfswarm-reporter-1.2.1/rfswarm_reporter.egg-info/PKG-INFO` & `rfswarm_reporter-1.3.0/rfswarm_reporter.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: rfswarm-reporter
-Version: 1.2.1
+Version: 1.3.0
 Summary: rfswarm reporter
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
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: configparser
+Requires-Dist: pillow>=9.1.0
+Requires-Dist: pip>=21,>=22
+Requires-Dist: matplotlib
+Requires-Dist: python-docx
+Requires-Dist: openpyxl
+Requires-Dist: tzlocal>=4.1
+Requires-Dist: lxml
 
 # rfswarm (Robot Framework Swarm)
 
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
@@ -54,9 +60,7 @@
 
 
 ## Donations
 
 If you would like to thank me for this project please consider using one of the sponsorship methods:
 - [GitHub](https://github.com/sponsors/damies13/)
 - [PayPal.me](https://paypal.me/damies13/5) (the $5 is a suggestion, feel free to change to any amount you would like)
-
-
```

### Comparing `rfswarm-reporter-1.2.1/setup-reporter.py` & `rfswarm_reporter-1.3.0/setup-reporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README_PyPi.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="rfswarm-reporter",
-	version="1.2.1",
+	version="1.3.0",
 	author="damies13",
 	author_email="damies13+rfswarm@gmail.com",
 	description="rfswarm reporter",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/damies13/rfswarm",
 	packages=setuptools.find_packages(exclude=["*fswarm_manag*", "*fswarm_agen*", "build/*"]),
 	# I needed a recent version of pip (pip 21.0.1 worked my previous <20 version didn't) for matplotlib
 	# 	to actually install withput error
 	# https://matplotlib.org/stable/users/installing.html
 	# zoneinfo requires python 3.9
 	# tzlocal is needed to get the local timezone in a format that zoneinfo likes
-	install_requires=['configparser', 'pillow>=9.1.0', 'pip>=21,>=22', 'matplotlib', 'python-docx', 'openpyxl', 'tzlocal>=4.1'],
+	install_requires=['configparser', 'pillow>=9.1.0', 'pip>=21,>=22', 'matplotlib', 'python-docx', 'openpyxl', 'tzlocal>=4.1', 'lxml'],
 	classifiers=[
 		"Development Status :: 5 - Production/Stable",
 		"Topic :: Software Development :: Testing",
 		"Programming Language :: Python :: 3.9",
 		"License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 		"Operating System :: OS Independent",
 	],
```

