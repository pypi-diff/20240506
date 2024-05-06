# Comparing `tmp/urbanopt-ditto-reader-0.6.3.tar.gz` & `tmp/urbanopt_ditto_reader-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urbanopt-ditto-reader-0.6.3.tar", last modified: Mon Dec 18 23:16:46 2023, max compression
+gzip compressed data, was "urbanopt_ditto_reader-0.6.4.tar", last modified: Mon May  6 16:41:36 2024, max compression
```

## Comparing `urbanopt-ditto-reader-0.6.3.tar` & `urbanopt_ditto_reader-0.6.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:16:46.145060 urbanopt-ditto-reader-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2023-12-18 23:16:36.000000 urbanopt-ditto-reader-0.6.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-18 23:16:36.000000 urbanopt-ditto-reader-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2023-12-18 23:16:46.145060 urbanopt-ditto-reader-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2023-12-18 23:16:36.000000 urbanopt-ditto-reader-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2023-12-18 23:16:38.000000 urbanopt-ditto-reader-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 23:16:46.145060 urbanopt-ditto-reader-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:16:46.141060 urbanopt-ditto-reader-0.6.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:16:46.141060 urbanopt-ditto-reader-0.6.3/tests/urbanopt_ditto_reader/
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-12-18 23:16:38.000000 urbanopt-ditto-reader-0.6.3/tests/urbanopt_ditto_reader/test_ditto_reader_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:16:46.141060 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 23:16:38.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2023-12-18 23:16:38.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/ditto_reader_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-18 23:16:38.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/example_config.json
--rw-r--r--   0 runner    (1001) docker     (127)   554243 2023-12-18 23:16:38.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/extended_catalog.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:16:46.145060 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 23:16:38.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36976 2023-12-18 23:16:38.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/reader/read.py
--rw-r--r--   0 runner    (1001) docker     (127)    26630 2023-12-18 23:16:38.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/urbanopt_ditto_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:16:46.145060 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2023-12-18 23:16:46.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-12-18 23:16:46.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 23:16:46.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-18 23:16:46.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-18 23:16:46.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-18 23:16:46.000000 urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:41:36.705553 urbanopt_ditto_reader-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-06 16:41:31.000000 urbanopt_ditto_reader-0.6.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-06 16:41:31.000000 urbanopt_ditto_reader-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-06 16:41:36.705553 urbanopt_ditto_reader-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-06 16:41:31.000000 urbanopt_ditto_reader-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-06 16:41:32.000000 urbanopt_ditto_reader-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:41:36.705553 urbanopt_ditto_reader-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:41:36.701553 urbanopt_ditto_reader-0.6.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:41:36.701553 urbanopt_ditto_reader-0.6.4/tests/urbanopt_ditto_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-06 16:41:32.000000 urbanopt_ditto_reader-0.6.4/tests/urbanopt_ditto_reader/test_ditto_reader_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:41:36.701553 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:41:32.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-05-06 16:41:32.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/ditto_reader_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-06 16:41:32.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/example_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)   554243 2024-05-06 16:41:32.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/extended_catalog.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:41:36.705553 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:41:32.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37280 2024-05-06 16:41:32.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/reader/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26603 2024-05-06 16:41:32.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/urbanopt_ditto_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:41:36.705553 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-06 16:41:36.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-06 16:41:36.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:41:36.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-06 16:41:36.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 16:41:36.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 16:41:36.000000 urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader.egg-info/top_level.txt
```

### Comparing `urbanopt-ditto-reader-0.6.3/LICENSE.md` & `urbanopt_ditto_reader-0.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `urbanopt-ditto-reader-0.6.3/PKG-INFO` & `urbanopt_ditto_reader-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urbanopt-ditto-reader
-Version: 0.6.3
+Version: 0.6.4
 Summary: Enhancement of URBANopt GeoJSON that can be consumed by DiTTo reader
 Author-email: Tarek Elgindy <tarek.elgindy@nrel.gov>, Nathan Moore <nathan.moore@nrel.gov>, Katherine Fleming <katherine.fleming@nrel.gov>
 Project-URL: Homepage, https://github.com/urbanopt/urbanopt-ditto-reader
 Project-URL: Bug Tracker, https://github.com/urbanopt/urbanopt-ditto-reader/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -16,19 +16,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ditto.py[opendss]~=0.2.4
-Requires-Dist: opendssdirect.py~=0.8
+Requires-Dist: opendssdirect.py~=0.8.0
 Provides-Extra: dev
 Requires-Dist: pytest~=7.4; extra == "dev"
 Requires-Dist: pre-commit~=3.3; extra == "dev"
-Requires-Dist: ruff~=0.1.6; extra == "dev"
+Requires-Dist: ruff~=0.4.0; extra == "dev"
 
 # urbanopt-ditto-reader
 Enhancement of URBANopt™ GeoJSON that can be consumed by DiTTo reader \
 More detailed documentation is available on the [URBANopt documentation page](https://docs.urbanopt.net/opendss/opendss.html)
 
 # Installation Pre-requisites
 - Python >=3.8
```

### Comparing `urbanopt-ditto-reader-0.6.3/README.md` & `urbanopt_ditto_reader-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `urbanopt-ditto-reader-0.6.3/pyproject.toml` & `urbanopt_ditto_reader-0.6.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [project]
 name = "urbanopt-ditto-reader"
 dynamic = [
     "readme",
     ]
-version = "0.6.3"
+version = "0.6.4"
 authors = [
   { name="Tarek Elgindy", email="tarek.elgindy@nrel.gov" },
   { name="Nathan Moore", email="nathan.moore@nrel.gov" },
   { name="Katherine Fleming", email="katherine.fleming@nrel.gov" },
 ]
 description = "Enhancement of URBANopt GeoJSON that can be consumed by DiTTo reader"
 requires-python = "~=3.8"
@@ -30,22 +30,22 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12"
     ]
 dependencies = [
     "ditto.py[opendss] ~= 0.2.4",
-    "opendssdirect.py ~= 0.8",
+    "opendssdirect.py ~= 0.8.0",
     ]
 
 [project.optional-dependencies]
 dev = [
     "pytest ~= 7.4",
     "pre-commit ~= 3.3",
-    "ruff ~= 0.1.6",
+    "ruff ~= 0.4.0",
 ]
 
 # https://setuptools.pypa.io/en/latest/userguide/package_discovery.html
 [tool.setuptools.packages.find]
 # Must include a MANIFEST.in file in our repo: https://setuptools.pypa.io/en/latest/userguide/datafiles.html
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html#dynamic-metadata
@@ -57,27 +57,30 @@
 "Bug Tracker" = "https://github.com/urbanopt/urbanopt-ditto-reader/issues"
 
 # https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = "tests"
 
-# https://github.com/charliermarsh/ruff
+# https://docs.astral.sh/ruff/tutorial/#configuration
 [tool.ruff]
 fix = true # automatically fix problems if possible
-select = ["RUF", "E", "F", "I", "UP", "N", "S", "BLE", "A", "C4", "T10", "ISC", "ICN", "PT",
+line-length = 120
+
+# https://docs.astral.sh/ruff/linter/#rule-selection
+[tool.ruff.lint]
+extend-select = ["RUF", "E", "F", "I", "UP", "N", "S", "BLE", "A", "C4", "T10", "ISC", "ICN", "PT",
 "Q", "SIM", "TID", "ARG", "DTZ", "PD", "PGH", "PLC", "PLE", "PLR", "PLW", "PIE", "COM"] # Enable these rules
 ignore = ["PLR0913", "PLR2004", "PLR0402", "COM812", "COM819", "SIM108", "ARG002", "ISC001"] # except for these specific errors
-line-length = 120
 
 # https://docs.astral.sh/ruff/settings/#format
 [tool.ruff.format]
 # quote-style = "double"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = ["S101", "S607", "S603"] # assert statements are allowed in tests, and paths are safe
 "update_licenses.py" = ["SIM115", "A002", "ARG001"]
 "urbanopt_ditto_reader/reader/read.py" = ["PLR0912", "PLR0915"] # ignore complexity warnings in this file
 "urbanopt_ditto_reader/urbanopt_ditto_reader.py" = ["PLR0912", "PLR0915"] # ignore complexity warnings in this file
 
 [project.scripts]
 ditto_reader_cli = "urbanopt_ditto_reader.ditto_reader_cli:cli"
```

### Comparing `urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/ditto_reader_cli.py` & `urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/ditto_reader_cli.py`

 * *Files identical despite different names*

### Comparing `urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/extended_catalog.json` & `urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/extended_catalog.json`

 * *Files identical despite different names*

### Comparing `urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/reader/read.py` & `urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/reader/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,19 @@
 BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
 OF THE POSSIBILITY OF SUCH DAMAGE.
 *****************************************************************************************
 """
+
 import json
 import os
 from datetime import datetime
+from pathlib import Path
 
 from ditto.models.base import Unicode
 from ditto.models.feeder_metadata import Feeder_metadata
 from ditto.models.line import Line
 from ditto.models.load import Load
 from ditto.models.node import Node
 from ditto.models.phase_load import PhaseLoad
@@ -506,19 +508,23 @@
                 is_center_tap = upstream_transformer.is_center_tap
                 load.nominal_voltage = upstream_transformer.windings[1].nominal_voltage
             else:
                 print(f"Warning - Load {load.name} has no transformer. Assigning as MV load", flush=True)
                 load.nominal_voltage = model["urbanopt-feeder"].nominal_voltage
 
             # load the power draw of the buildings from the energy sim results
-            load_path = os.path.join(self.load_folder, id_value, "feature_reports")
+            load_path = Path(self.load_folder) / id_value / "feature_reports"
             load_multiplier = 1000
-            if os.path.exists(load_path):  # We've found the load data
+            if load_path.is_dir():  # We've found the load data
                 if self.use_reopt:
-                    rep_csv = os.path.join(load_path, "feature_optimization.csv")
+                    rep_csv = load_path / "feature_optimization.csv"
+                    if not rep_csv.is_file():
+                        print("feature_optimization.csv not found. Please run REopt post-processing first.")
+                        # TODO: Get the test to read this text appropriately from inside the SystemExit()
+                        raise SystemExit()
                     report_mtx = self._read_csv(rep_csv)
                     header_row = report_mtx.pop(0)
                     load_col_i = header_row.index("REopt:Electricity:Load:Total(kw)")
                     load_column = [row[load_col_i] for row in report_mtx]
                 else:
                     rep_csv = os.path.join(load_path, "default_feature_report.csv")
                     report_mtx = self._read_csv(rep_csv)
```

### Comparing `urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader/urbanopt_ditto_reader.py` & `urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader/urbanopt_ditto_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -462,21 +462,21 @@
             for element, line_load_val in line_overloads.items():
                 line_df_dic[element].append([time, round(line_load_val, 5), line_load_val > 1.0])
             for element, xfrm_load_val in overloaded_xfmrs.items():
                 transformer_df_dic[element].append([time, round(xfrm_load_val, 5), xfrm_load_val > 1.0])
 
         # write the collected results into CSV files
         for element, result_values in voltage_df_dic.items():
-            res_path = os.path.join(features_path, "%s.csv" % element.replace("_", "-"))
+            res_path = Path(features_path) / f"{element.replace('_', '-')}.csv"
             self._write_csv(result_values, res_path)
         for element, result_values in line_df_dic.items():
-            res_path = os.path.join(lines_path, "%s.csv" % element.replace(":", ""))
+            res_path = Path(lines_path) / f"{element.replace(':', '')}.csv"
             self._write_csv(result_values, res_path)
         for element, result_values in transformer_df_dic.items():
-            res_path = os.path.join(trans_path, "%s.csv" % element.replace(":", ""))
+            res_path = Path(trans_path) / f"{element.replace(':', '')}.csv"
             self._write_csv(result_values, res_path)
 
     @staticmethod
     def _read_single_column_csv(csv_file_path):
         """Load a single columns CSV file into a Python matrix of strings.
 
         Args:
```

### Comparing `urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader.egg-info/PKG-INFO` & `urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urbanopt-ditto-reader
-Version: 0.6.3
+Version: 0.6.4
 Summary: Enhancement of URBANopt GeoJSON that can be consumed by DiTTo reader
 Author-email: Tarek Elgindy <tarek.elgindy@nrel.gov>, Nathan Moore <nathan.moore@nrel.gov>, Katherine Fleming <katherine.fleming@nrel.gov>
 Project-URL: Homepage, https://github.com/urbanopt/urbanopt-ditto-reader
 Project-URL: Bug Tracker, https://github.com/urbanopt/urbanopt-ditto-reader/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -16,19 +16,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ditto.py[opendss]~=0.2.4
-Requires-Dist: opendssdirect.py~=0.8
+Requires-Dist: opendssdirect.py~=0.8.0
 Provides-Extra: dev
 Requires-Dist: pytest~=7.4; extra == "dev"
 Requires-Dist: pre-commit~=3.3; extra == "dev"
-Requires-Dist: ruff~=0.1.6; extra == "dev"
+Requires-Dist: ruff~=0.4.0; extra == "dev"
 
 # urbanopt-ditto-reader
 Enhancement of URBANopt™ GeoJSON that can be consumed by DiTTo reader \
 More detailed documentation is available on the [URBANopt documentation page](https://docs.urbanopt.net/opendss/opendss.html)
 
 # Installation Pre-requisites
 - Python >=3.8
```

### Comparing `urbanopt-ditto-reader-0.6.3/urbanopt_ditto_reader.egg-info/SOURCES.txt` & `urbanopt_ditto_reader-0.6.4/urbanopt_ditto_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

