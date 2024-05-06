# Comparing `tmp/timewise_sup-0.4.8.tar.gz` & `tmp/timewise_sup-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timewise_sup-0.4.8.tar", max compression
+gzip compressed data, was "timewise_sup-0.5.0.tar", max compression
```

## Comparing `timewise_sup-0.4.8.tar` & `timewise_sup-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,41 @@
--rw-r--r--   0        0        0     1542 2023-12-20 16:20:20.337730 timewise_sup-0.4.8/LICENSE
--rw-r--r--   0        0        0     1178 2023-12-20 16:30:07.434295 timewise_sup-0.4.8/README.md
--rw-r--r--   0        0        0     3229 2023-12-20 16:30:07.442295 timewise_sup-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      387 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/__init__.py
--rw-r--r--   0        0        0     8210 2023-12-20 16:20:20.373730 timewise_sup-0.4.8/timewise_sup/ampel_conf.py
--rw-r--r--   0        0        0        0 2023-12-20 16:20:20.585732 timewise_sup-0.4.8/timewise_sup/analyse_lightcurves/__init__.py
--rw-r--r--   0        0        0     1720 2023-12-20 16:20:20.373730 timewise_sup-0.4.8/timewise_sup/analyse_lightcurves/bayesian_blocks.py
--rw-r--r--   0        0        0    12959 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/analyse_lightcurves/cluster.py
--rw-r--r--   0        0        0    13084 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/analyse_lightcurves/create_job_file_yaml.py
--rw-r--r--   0        0        0     5476 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/config_loader.py
--rw-r--r--   0        0        0      740 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/environment.py
--rw-r--r--   0        0        0      704 2023-12-20 16:20:20.373730 timewise_sup-0.4.8/timewise_sup/main.py
--rw-r--r--   0        0        0        0 2023-12-20 16:20:20.585732 timewise_sup-0.4.8/timewise_sup/meta_analysis/__init__.py
--rw-r--r--   0        0        0     4550 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/meta_analysis/agn.py
--rw-r--r--   0        0        0    11550 2023-12-20 16:20:20.373730 timewise_sup-0.4.8/timewise_sup/meta_analysis/baseline_subtraction.py
--rw-r--r--   0        0        0     1232 2023-12-20 16:20:20.373730 timewise_sup-0.4.8/timewise_sup/meta_analysis/catalog_match.py
--rw-r--r--   0        0        0     8700 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/meta_analysis/diagnostics.py
--rw-r--r--   0        0        0     5226 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/meta_analysis/fluence.py
--rw-r--r--   0        0        0    10508 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/meta_analysis/flux.py
--rw-r--r--   0        0        0     3058 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/meta_analysis/integrate_time.py
--rw-r--r--   0        0        0     8045 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/meta_analysis/ir_energy.py
--rw-r--r--   0        0        0    10186 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/meta_analysis/luminosity.py
--rw-r--r--   0        0        0        0 2023-12-20 16:20:20.585732 timewise_sup-0.4.8/timewise_sup/meta_analysis/plot_tns_matches.py
--rw-r--r--   0        0        0     7901 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/meta_analysis/rejection_reason.py
--rw-r--r--   0        0        0    23539 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/mongo.py
--rw-r--r--   0        0        0     1066 2023-12-20 16:20:20.377730 timewise_sup-0.4.8/timewise_sup/plots/__init__.py
--rw-r--r--   0        0        0     2462 2023-12-20 16:20:20.377730 timewise_sup-0.4.8/timewise_sup/plots/chi2_histograms.py
--rw-r--r--   0        0        0     8698 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/plots/color_plots.py
--rw-r--r--   0        0        0     5520 2023-12-20 16:20:20.377730 timewise_sup-0.4.8/timewise_sup/plots/diagnostic_plots.py
--rw-r--r--   0        0        0     4406 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/plots/ensemble_lightcurves.py
--rw-r--r--   0        0        0     2088 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/plots/ir_energies.py
--rw-r--r--   0        0        0     5228 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/plots/plot_lightcurves.py
--rw-r--r--   0        0        0     2768 2023-12-20 16:20:20.377730 timewise_sup-0.4.8/timewise_sup/plots/rise_fade_times.py
--rw-r--r--   0        0        0     2973 2023-12-20 16:20:20.377730 timewise_sup-0.4.8/timewise_sup/plots/test_data_res.py
--rw-r--r--   0        0        0    15042 2023-12-20 16:30:46.202600 timewise_sup-0.4.8/timewise_sup/samples/__pycache__/sjoerts_flares.cpython-310.pyc
--rw-r--r--   0        0        0     2822 2023-12-20 16:20:20.377730 timewise_sup-0.4.8/timewise_sup/samples/bts.py
--rw-r--r--   0        0        0    34787 2023-12-20 16:30:07.458295 timewise_sup-0.4.8/timewise_sup/samples/sjoerts_flares.py
--rw-r--r--   0        0        0     2453 1970-01-01 00:00:00.000000 timewise_sup-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1542 2024-05-05 13:30:25.005539 timewise_sup-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1178 2024-05-05 13:38:19.974185 timewise_sup-0.5.0/README.md
+-rw-r--r--   0        0        0     3283 2024-05-05 13:38:19.978185 timewise_sup-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      387 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/__init__.py
+-rw-r--r--   0        0        0     8210 2024-05-05 13:30:25.033539 timewise_sup-0.5.0/timewise_sup/ampel_conf.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:30:25.121539 timewise_sup-0.5.0/timewise_sup/analyse_lightcurves/__init__.py
+-rw-r--r--   0        0        0     1720 2024-05-05 13:30:25.033539 timewise_sup-0.5.0/timewise_sup/analyse_lightcurves/bayesian_blocks.py
+-rw-r--r--   0        0        0    12959 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/analyse_lightcurves/cluster.py
+-rw-r--r--   0        0        0    13084 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/analyse_lightcurves/create_job_file_yaml.py
+-rw-r--r--   0        0        0     5476 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/config_loader.py
+-rw-r--r--   0        0        0      740 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/environment.py
+-rw-r--r--   0        0        0     5647 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/main.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:30:25.121539 timewise_sup-0.5.0/timewise_sup/meta_analysis/__init__.py
+-rw-r--r--   0        0        0     4550 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/meta_analysis/agn.py
+-rw-r--r--   0        0        0    13738 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/meta_analysis/baseline_subtraction.py
+-rw-r--r--   0        0        0     1232 2024-05-05 13:30:25.033539 timewise_sup-0.5.0/timewise_sup/meta_analysis/catalog_match.py
+-rw-r--r--   0        0        0    18577 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/meta_analysis/diagnostics.py
+-rw-r--r--   0        0        0     5955 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/meta_analysis/fluence.py
+-rw-r--r--   0        0        0    11903 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/meta_analysis/flux.py
+-rw-r--r--   0        0        0     3058 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/meta_analysis/integrate_time.py
+-rw-r--r--   0        0        0     9274 2024-05-05 13:38:19.994185 timewise_sup-0.5.0/timewise_sup/meta_analysis/ir_energy.py
+-rw-r--r--   0        0        0    11364 2024-05-05 13:38:19.998185 timewise_sup-0.5.0/timewise_sup/meta_analysis/luminosity.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:30:25.121539 timewise_sup-0.5.0/timewise_sup/meta_analysis/plot_tns_matches.py
+-rw-r--r--   0        0        0     7031 2024-05-05 13:38:19.998185 timewise_sup-0.5.0/timewise_sup/meta_analysis/rejection_reason.py
+-rw-r--r--   0        0        0    10926 2024-05-05 13:38:19.998185 timewise_sup-0.5.0/timewise_sup/meta_analysis/separation.py
+-rw-r--r--   0        0        0    32171 2024-05-05 13:38:19.998185 timewise_sup-0.5.0/timewise_sup/mongo.py
+-rw-r--r--   0        0        0     1066 2024-05-05 13:30:25.037539 timewise_sup-0.5.0/timewise_sup/plots/__init__.py
+-rw-r--r--   0        0        0     2462 2024-05-05 13:30:25.037539 timewise_sup-0.5.0/timewise_sup/plots/chi2_histograms.py
+-rw-r--r--   0        0        0     8698 2024-05-05 13:38:19.998185 timewise_sup-0.5.0/timewise_sup/plots/color_plots.py
+-rw-r--r--   0        0        0    17829 2024-05-05 13:38:19.998185 timewise_sup-0.5.0/timewise_sup/plots/diagnostic_plots.py
+-rw-r--r--   0        0        0     4406 2024-05-05 13:38:19.998185 timewise_sup-0.5.0/timewise_sup/plots/ensemble_lightcurves.py
+-rw-r--r--   0        0        0     2088 2024-05-05 13:38:19.998185 timewise_sup-0.5.0/timewise_sup/plots/ir_energies.py
+-rw-r--r--   0        0        0     5532 2024-05-05 13:38:19.998185 timewise_sup-0.5.0/timewise_sup/plots/plot_lightcurves.py
+-rw-r--r--   0        0        0     2768 2024-05-05 13:30:25.037539 timewise_sup-0.5.0/timewise_sup/plots/rise_fade_times.py
+-rw-r--r--   0        0        0     2973 2024-05-05 13:30:25.037539 timewise_sup-0.5.0/timewise_sup/plots/test_data_res.py
+-rw-r--r--   0        0        0     3336 2024-05-05 13:38:49.734229 timewise_sup-0.5.0/timewise_sup/samples/__pycache__/sjoerts_flares.cpython-310.pyc
+-rw-r--r--   0        0        0     2822 2024-05-05 13:30:25.037539 timewise_sup-0.5.0/timewise_sup/samples/bts.py
+-rw-r--r--   0        0        0    32086 2024-05-05 13:38:19.998185 timewise_sup-0.5.0/timewise_sup/samples/data/test_sample.json
+-rw-r--r--   0        0        0     2959 2024-05-05 13:38:19.998185 timewise_sup-0.5.0/timewise_sup/samples/sjoerts_flares.py
+-rw-r--r--   0        0        0     3775 2024-05-05 13:38:19.998185 timewise_sup-0.5.0/timewise_sup/sky_match.py
+-rw-r--r--   0        0        0     2454 1970-01-01 00:00:00.000000 timewise_sup-0.5.0/PKG-INFO
```

### Comparing `timewise_sup-0.4.8/LICENSE` & `timewise_sup-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/README.md` & `timewise_sup-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/pyproject.toml` & `timewise_sup-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # ---------------------------------------------------
 # START poetry config
 
 [tool.poetry]
 name = "timewise-sup"
-version = "0.4.8"
+version = "0.5.0"
 description = "The Timewise Subtraction Pipeline produces mid-infrared difference photometry based on measurements by the WISE satelite"
 authors = ["Jannis Necker <jannis.necker@gmail.com>", "Eleni Graikou <eleni.graikou@desy.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 documentation = "https://jannisnecker.pages.desy.de/timewise_sup/docs/"
 repository = "https://gitlab.desy.de/jannisnecker/timewise_sup"
 
 [tool.poetry.scripts]
 timewise_sup = "timewise_sup.main:main"
+timewise_sup_bump = "timewise_sup.main:bump_version"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.11"
-timewise = "0.4.9"
+timewise = "0.4.10"
 extcats = "^2.4.3"
 more-itertools = "^9.0.0"
 nltk = "^3.7"
 uncertainties = "^3.1.7"
 scikit-learn = "^1.1.2"
 corner = "^2.2.1"
 ampel-core = "0.8.4"
```

### Comparing `timewise_sup-0.4.8/timewise_sup/ampel_conf.py` & `timewise_sup-0.5.0/timewise_sup/ampel_conf.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/analyse_lightcurves/bayesian_blocks.py` & `timewise_sup-0.5.0/timewise_sup/analyse_lightcurves/bayesian_blocks.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/analyse_lightcurves/cluster.py` & `timewise_sup-0.5.0/timewise_sup/analyse_lightcurves/cluster.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/analyse_lightcurves/create_job_file_yaml.py` & `timewise_sup-0.5.0/timewise_sup/analyse_lightcurves/create_job_file_yaml.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/config_loader.py` & `timewise_sup-0.5.0/timewise_sup/config_loader.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/environment.py` & `timewise_sup-0.5.0/timewise_sup/environment.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/meta_analysis/agn.py` & `timewise_sup-0.5.0/timewise_sup/meta_analysis/agn.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/meta_analysis/baseline_subtraction.py` & `timewise_sup-0.5.0/timewise_sup/meta_analysis/baseline_subtraction.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,32 +12,35 @@
 
 import json
 import os.path
 from functools import cache
 import numpy as np
 import logging
 import tqdm
+from pathlib import Path
 
 import pandas as pd
 
 from timewise_sup.mongo import DatabaseConnector, Index, Status
 from timewise_sup.environment import load_environment
+from timewise_sup.meta_analysis.diagnostics import get_baseline_changes
 from timewise import WiseDataByVisit, WISEDataDESYCluster
 
 
 logger = logging.getLogger(__name__)
 
 
 def apply_baseline_subtraction(
         wise_data: WiseDataByVisit,
         database_name: str,
         service: str = "tap",
         load_from_bigdata_dir: bool = True,
         status: Status | None = None,
-        index: Index | None = None
+        index: Index | None = None,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Apply baseline subtraction to the lightcurves. The baseline values are read from the database and subtracted from
     the lightcurves. The resulting lightcurves are returned as a dictionary. The dictionary keys are the IDs of the
     lightcurves. The values are the lightcurves themselves.
 
     :param wise_data: WISEDataByVisit object
@@ -48,14 +51,16 @@
     :type service: str, optional
     :param load_from_bigdata_dir: whether to load the data from the bigdata directory, defaults to True
     :type load_from_bigdata_dir: bool, optional
     :param status: status of the lightcurves to be processed, defaults to None
     :type status: Status, optional
     :param index: IDs of the lightcurves to be processed, defaults to None
     :type index: Index, optional
+    :param correct_with_catalog_magnitudes: whether to correct the baseline with the catalog magnitudes, defaults to False
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: dictionary containing the baseline subtracted lightcurves
     :rtype: dict
     """
 
     logger.debug(f"status {status}")
     logger.debug(f"index {index}")
 
@@ -68,17 +73,34 @@
         if index is None:
             raise ValueError("You must specify either of 'index' or 'status'!")
 
     logger.info("getting baseline values")
 
     # keys are stock IDs, values are baseline values
     baselines = database_connector.get_baselines(index=index)
-    ids = np.array(list(baselines.keys()))
+    ids = baselines.index
     logger.debug(f"got baselines for {len(ids)} objects")
 
+    # check if there are dimmer magnitudes in catalogs
+    if correct_with_catalog_magnitudes:
+        logger.debug("correcting with catalog magnitudes")
+        baseline_changes = get_baseline_changes(
+            base_name=wise_data.base_name,
+            database_name=database_name,
+            wise_data=wise_data,
+            index=ids
+        )
+        for band in ["W1", "W2"]:
+            bad_baseline_mask = baseline_changes[f"{band}_diff"] < 0
+            bad_baseline_indices = bad_baseline_mask.index[bad_baseline_mask]
+            zp = wise_data.magnitude_zeropoints['F_nu'][band].to('mJy').value
+            better_baselines = 10 ** (baseline_changes.loc[bad_baseline_indices, f"{band}_catalog_mag"] / -2.5) * zp
+            baselines.loc[bad_baseline_indices, f"{band}_baseline"] = better_baselines
+            # TODO: figure out what todo with baseline unc!
+
     # find the chunk that holds the respective IDs
     chunk_numbers = np.array([wise_data._get_chunk_number(parent_sample_index=s) for s in ids])
 
     # set up empty directory for baseline corrected lightcurves
     diff_lcs = dict()
 
     # load the chunks one after the other
@@ -108,16 +130,16 @@
                 # loop over flux and flux errors
                 f_key = WiseDataByVisit.mean_key + WiseDataByVisit.flux_density_key_ext
                 ferr_key = WiseDataByVisit.flux_density_key_ext + WiseDataByVisit.rms_key
 
                 try:
                     # f is a dict with keys: index and values: flux_densities
                     f = lc_in[b + f_key]
-                    baseline = baselines[s][f"{b}_baseline"]
-                    baseline_err = baselines[s][f"{b}_baseline_sigma"]
+                    baseline = baselines.loc[s, f"{b}_baseline"]
+                    baseline_err = baselines.loc[s, f"{b}_baseline_sigma"]
 
                     if baseline is None:
                         logger.warning(f"baseline for {s} {b} is None, skipping!")
                         continue
 
                     f_diff = {k: v - baseline for k, v in f.items()}
                     f_diff_key = "_diff" + f_key
@@ -145,14 +167,15 @@
         base_name: str,
         database_name: str,
         wise_data: WiseDataByVisit,
         status: Status,
         force_new: bool = False,
         service: str = "tap",
         load_from_bigdata_dir: bool = True,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Get the baseline subtracted lightcurves from the json file buy status. If the file does not exist, call the function
     :func:`apply_baseline_subtraction` to create it. The resulting lightcurves are returned as a dictionary. The
     dictionary keys are the IDs of the lightcurves. The values are the lightcurves themselves.
 
     :param base_name: name of the base directory
@@ -165,38 +188,39 @@
     :type status: Status
     :param force_new: whether to force the creation of a new file, defaults to False
     :type force_new: bool, optional
     :param service: :class:`timewise` service that was used to download the data, defaults to "tap"
     :type service: str, optional
     :param load_from_bigdata_dir: whether to load the data from the bigdata directory, defaults to True
     :type load_from_bigdata_dir: bool, optional
+    :param correct_with_catalog_magnitudes: whether to correct the baseline with the catalog magnitudes, defaults to False
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: dictionary containing the baseline subtracted lightcurves
     :rtype: dict
     """
     logger.info(f"getting baseline subtracted lightcurves for status {status}")
-    tsup_data_dir = load_environment("TIMEWISE_SUP_DATA")
-    fn = os.path.join(tsup_data_dir, base_name, f"diff_lcs_status{status}.json")
+    tsup_data_dir = Path(load_environment("TIMEWISE_SUP_DATA"))
+    catalog_desc = "_with_catalog_magnitudes" if correct_with_catalog_magnitudes else ""
+    fn = tsup_data_dir / base_name / f"diff_lcs_status{status}{catalog_desc}.json"
 
     if (not os.path.isfile(fn)) or force_new:
         logger.info(f"No file {fn}.")
         logger.info("Making baseline subtracted lightcurves")
         diff_lcs = apply_baseline_subtraction(
             wise_data=wise_data,
             database_name=database_name,
             service=service,
             load_from_bigdata_dir=load_from_bigdata_dir,
-            status=status
+            status=status,
+            correct_with_catalog_magnitudes=correct_with_catalog_magnitudes
         )
 
-        d = os.path.dirname(fn)
-        if not os.path.isdir(d):
-            os.makedirs(d)
-
         logger.debug(f"saving under {fn}")
-        with open(fn, "w") as f:
+        fn.parent.mkdir(parents=True, exist_ok=True)
+        with fn.open("w") as f:
             json.dump(diff_lcs, f)
 
     else:
         logger.debug(f"loading {fn}")
         with open(fn, "r") as f:
             diff_lcs = json.load(f)
 
@@ -206,14 +230,15 @@
 def get_lightcurves(
         base_name: str,
         database_name: str,
         wise_data: WiseDataByVisit,
         index: Index,
         service: str = "tap",
         load_from_bigdata_dir: bool = True,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Get the baseline subtracted lightcurves from the json file by index. If the file does not exist, call the function
     :func:`get_baseline_subtracted_lightcurves` to create it. The resulting lightcurves are returned as a dictionary.
     The dictionary keys are the IDs of the lightcurves. The values are the lightcurves themselves.
 
     :param base_name: name of the base directory
@@ -224,14 +249,16 @@
     :type wise_data: WiseDataByVisit
     :param index: IDs of the lightcurves to be processed
     :type index: Index
     :param service: :class:`timewise` service that was used to download the data, defaults to "tap"
     :type service: str, optional
     :param load_from_bigdata_dir: whether to load the data from the bigdata directory, defaults to True
     :type load_from_bigdata_dir: bool, optional
+    :param correct_with_catalog_magnitudes: whether to correct the baseline with the catalog magnitudes, defaults to False
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: dictionary containing the baseline subtracted lightcurves
     :rtype: dict
     """
     indices = list(np.atleast_1d(index))
     logger.info(f"getting lightcurves {len(indices)} objects")
     status = DatabaseConnector(base_name=base_name, database_name=database_name).get_status(index=tuple(indices))
     logger.debug(f"found {len(status['status'].unique())} statuses")
@@ -240,15 +267,16 @@
         iids = status.index[status["status"] == s]
         slcs = get_baseline_subtracted_lightcurves(
             base_name=base_name,
             database_name=database_name,
             wise_data=wise_data,
             status=s,
             service=service,
-            load_from_bigdata_dir=load_from_bigdata_dir
+            load_from_bigdata_dir=load_from_bigdata_dir,
+            correct_with_catalog_magnitudes=correct_with_catalog_magnitudes
         )
 
         for i in iids:
             lcs[str(i)] = slcs[i]
 
     logger.debug(f"returning {len(lcs)} lightcurves")
     return lcs
@@ -258,14 +286,15 @@
 def get_single_lightcurve(
         base_name: str,
         database_name: str,
         wise_data: WiseDataByVisit,
         index: str,
         service: str = "tap",
         load_from_bigdata_dir: bool = True,
+        correct_with_catalog_magnitudes: bool = False
 ) -> pd.DataFrame:
     """
     Get the baseline subtracted lightcurves from the json file by index. If the file does not exist, call the function
     :func:`get_lightcurves` to create it.
 
     :param base_name: name of the base directory
     :type base_name: str
@@ -275,19 +304,22 @@
     :type wise_data: WiseDataByVisit
     :param index: ID of the lightcurve to be processed
     :type index: str
     :param service: :class:`timewise` service that was used to download the data, defaults to "tap"
     :type service: str, optional
     :param load_from_bigdata_dir: whether to load the data from the bigdata directory, defaults to True
     :type load_from_bigdata_dir: bool, optional
+    :param correct_with_catalog_magnitudes: whether to correct the baseline with the catalog magnitudes, defaults to False
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: baseline subtracted lightcurve
     :rtype: pandas.DataFrame
     """
     lcs = get_lightcurves(
         base_name=base_name,
         database_name=database_name,
         wise_data=wise_data,
         index=index,
         service=service,
-        load_from_bigdata_dir=load_from_bigdata_dir
+        load_from_bigdata_dir=load_from_bigdata_dir,
+        correct_with_catalog_magnitudes=correct_with_catalog_magnitudes
     )
     return pd.DataFrame.from_dict(lcs[str(index)])
```

### Comparing `timewise_sup-0.4.8/timewise_sup/meta_analysis/catalog_match.py` & `timewise_sup-0.5.0/timewise_sup/meta_analysis/catalog_match.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/meta_analysis/fluence.py` & `timewise_sup-0.5.0/timewise_sup/meta_analysis/fluence.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 
 def calculate_ir_fluence(
         base_name: str,
         database_name: str,
         wise_data: WISEDataBase,
         status: Status,
         service: str = "tap",
-        load_from_bigdata_dir: bool = False
+        load_from_bigdata_dir: bool = False,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Calculate the IR fluence for a given status. The IR fluence is calculated by integrating the IR flux over the
     duration of the flare.
 
     :param base_name: base name for storage directories
     :type base_name: str
@@ -46,22 +47,25 @@
     :type wise_data: WISEDataBase
     :param status: status to calculate the IR fluence for
     :type status: Status
     :param service: service to use for the TAP query, defaults to "tap", passed to :func:`get_lightcurves`
     :type service: str, optional
     :param load_from_bigdata_dir: load from the bigdata directory, defaults to False, passed to :func:`get_lightcurves`
     :type load_from_bigdata_dir: bool, optional
+    :param correct_with_catalog_magnitudes: if True, the flux is corrected with the magnitudes from the parent sample
+    :type correct_with_catalog_magnitudes: bool, optional
     :return:
     """
     database_connector = DatabaseConnector(base_name=base_name, database_name=database_name)
     ids = database_connector.get_ids(status)
     indices = np.atleast_1d(ids)
     logger.info(f"calculating fluence for {len(indices)} objects")
     lcs = get_ir_flux(base_name, database_name, wise_data, status,
-                      service=service, load_from_bigdata_dir=load_from_bigdata_dir)
+                      service=service, load_from_bigdata_dir=load_from_bigdata_dir,
+                      correct_with_catalog_magnitudes=correct_with_catalog_magnitudes)
     flare_time = get_flare_time(base_name, database_name, indices)
     fluence = dict()
 
     for k, lc in lcs.items():
         i_fluence = time_integral(
             lc=pd.DataFrame.from_dict(lc, orient="columns"),
             key=flux_key,
@@ -82,15 +86,16 @@
 def get_ir_fluence(
         base_name: str,
         database_name: str,
         wise_data: WISEDataBase,
         status: Status,
         service: str = "tap",
         load_from_bigdata_dir: bool = False,
-        force_new: bool = False
+        force_new: bool = False,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Get the IR fluence for a given status. The IR fluence is calculated by integrating :func:`get_ir_flux` if it
     has not been calculated before. The results are cached to disk.
 
     :param base_name: base name for storage directories
     :type base_name: str
@@ -102,21 +107,24 @@
     :type status: Status
     :param service: service to use for the TAP query, defaults to "tap", passed to :func:`get_lightcurves`
     :type service: str, optional
     :param load_from_bigdata_dir: load from the bigdata directory, defaults to False, passed to :func:`get_lightcurves`
     :type load_from_bigdata_dir: bool, optional
     :param force_new: calculate fluence again, even if cache exists, defaults to False
     :type force_new: bool, optional
+    :param correct_with_catalog_magnitudes: if True, the flux is corrected with the magnitudes from the parent sample
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: dictionary with the IR fluence for each index
     :rtype: dict
     """
 
     logger.info(f"getting fluxes for status {status}")
     tsup_data_dir = load_environment("TIMEWISE_SUP_DATA")
-    fn = os.path.join(tsup_data_dir, base_name, f"fluence_ir_status{status}.json")
+    catalog_desc = "_with_catalog_magnitudes" if correct_with_catalog_magnitudes else ""
+    fn = os.path.join(tsup_data_dir, base_name, f"fluence_ir_status{status}{catalog_desc}.json")
     logger.info(f"getting IR fluence for status {status}")
 
     if os.path.exists(fn) and not force_new:
         logger.info(f"loading IR fluence from {fn}")
         with open(fn, "r") as f:
             fluence = json.load(f)
 
@@ -125,14 +133,15 @@
         logger.info(f"calculating IR fluence")
         fluence = calculate_ir_fluence(
             base_name=base_name,
             database_name=database_name,
             wise_data=wise_data,
             status=status,
             service=service,
-            load_from_bigdata_dir=load_from_bigdata_dir
+            load_from_bigdata_dir=load_from_bigdata_dir,
+            correct_with_catalog_magnitudes=correct_with_catalog_magnitudes
         )
         logger.info(f"saving IR fluence to {fn}")
         with open(fn, "w") as f:
             json.dump(fluence, f)
 
     return fluence
```

### Comparing `timewise_sup-0.4.8/timewise_sup/meta_analysis/flux.py` & `timewise_sup-0.5.0/timewise_sup/meta_analysis/flux.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,16 @@
 
 def calculate_ir_flux(
         base_name: str,
         database_name: str,
         wise_data: WISEDataBase,
         index: Index,
         service: str = "tap",
-        load_from_bigdata_dir: bool = False
+        load_from_bigdata_dir: bool = False,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Calculates the IR flux for a given index. The IR flux is calculated by multiplying the flux density with the
     frequency of the given band.
 
     :param base_name: base name for storage directories
     :type base_name: str
@@ -87,22 +88,25 @@
     :type wise_data: WISEDataBase
     :param index: index of the object
     :type index: Index
     :param service: service to use for the TAP query, defaults to "tap", passed to :func:`get_lightcurves`
     :type service: str, optional
     :param load_from_bigdata_dir: load from the bigdata directory, defaults to False, passed to :func:`get_lightcurves`
     :type load_from_bigdata_dir: bool, optional
+    :param correct_with_catalog_magnitudes: if True, the flux is corrected with the magnitudes from the parent sample
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: dictionary with the index as key and the IR fluxes as value
     :rtype: dict
     """
     indices = tuple(np.atleast_1d(index).astype(int))
     logger.info(f"calculating flux for {len(indices)} objects")
 
     lcs = get_lightcurves(base_name, database_name, wise_data, indices,
-                          service=service, load_from_bigdata_dir=load_from_bigdata_dir)
+                          service=service, load_from_bigdata_dir=load_from_bigdata_dir,
+                          correct_with_catalog_magnitudes=correct_with_catalog_magnitudes)
     logger.debug(f"got {len(lcs)} lightcurves")
     lcs_with_fluxes = dict()
 
     for i, lc_dict in lcs.items():
         lc_in = pd.DataFrame.from_dict(lc_dict, orient="columns")
         lc_out = lc_in[["mean_mjd"]].copy()
 
@@ -128,15 +132,16 @@
 def get_ir_flux(
         base_name: str,
         database_name: str,
         wise_data: WISEDataBase,
         status: Status,
         force_new: bool = False,
         service: str = "tap",
-        load_from_bigdata_dir: bool = False
+        load_from_bigdata_dir: bool = False,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Get the IR flux of the flares per status. If the cache file `flux_ir_lcs_status{status}.json` exists,
     it is loaded from there. If it does not exist, it is calculated by :func:`calculate_ir_flux` and stored there.
 
     :param base_name: base name for storage directories
     :type base_name: str
@@ -148,34 +153,38 @@
     :type status: Status
     :param force_new: if True, the IR flux is calculated even if the cache file exists, defaults to False
     :type force_new: bool, optional
     :param service: service to use for the TAP query, defaults to "tap", passed to :func:`get_lightcurves`
     :type service: str, optional
     :param load_from_bigdata_dir: load from the bigdata directory, defaults to False, passed to :func:`get_lightcurves`
     :type load_from_bigdata_dir: bool, optional
+    :param correct_with_catalog_magnitudes: if True, the flux is corrected with the magnitudes from the parent sample
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: dictionary with the index as key and the IR fluxes as value
     :rtype: dict
     """
     logger.info(f"getting fluxes for status {status}")
     tsup_data_dir = load_environment("TIMEWISE_SUP_DATA")
-    fn = os.path.join(tsup_data_dir, base_name, f"flux_ir_lcs_status{status}.json")
+    catalog_desc = "_with_catalog_magnitudes" if correct_with_catalog_magnitudes else ""
+    fn = os.path.join(tsup_data_dir, base_name, f"flux_ir_lcs_status{status}{catalog_desc}.json")
 
     if (not os.path.isfile(fn)) or force_new:
         logger.debug(f"No file {fn}")
         logger.info("calculating fluxes")
 
         database_connector = DatabaseConnector(base_name=base_name, database_name=database_name)
         indices = database_connector.get_ids(status)
         lcs = calculate_ir_flux(
             base_name,
             database_name,
             wise_data,
             indices,
             service=service,
-            load_from_bigdata_dir=load_from_bigdata_dir
+            load_from_bigdata_dir=load_from_bigdata_dir,
+            correct_with_catalog_magnitudes=correct_with_catalog_magnitudes
         )
 
         logger.debug(f"writing to {fn}")
         with open(fn, "w") as f:
             json.dump(lcs, f)
 
     else:
@@ -188,15 +197,16 @@
 
 def get_ir_flux_index(
         base_name: str,
         database_name: str,
         wise_data: WISEDataBase,
         index: Index,
         service: str = "tap",
-        load_from_bigdata_dir: bool = False
+        load_from_bigdata_dir: bool = False,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Get the IR flux of the flares by index. Checks the statuses of the flares and loads the respective files
     (or creates them) with :func:`get_ir_flux`.
 
     :param base_name: base name for storage directories
     :type base_name: str
@@ -206,38 +216,42 @@
     :type wise_data: WISEDataBase
     :param index: index of the object
     :type index: Index
     :param service: service to use for the TAP query, defaults to "tap", passed to :func:`get_lightcurves`
     :type service: str, optional
     :param load_from_bigdata_dir: load from the bigdata directory, defaults to False, passed to :func:`get_lightcurves`
     :type load_from_bigdata_dir: bool, optional
+    :param correct_with_catalog_magnitudes: if True, the flux is corrected with the magnitudes from the parent sample
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: dictionary with the index as key and the IR fluxes as value
     :rtype: dict
     """
     _index = np.atleast_1d(index).astype(int)
     database_connector = DatabaseConnector(base_name=base_name, database_name=database_name)
     statuses = database_connector.get_status(list(_index))
 
     fluxes = dict()
     for status in statuses.status.unique():
         m = statuses.status == status
         status_ir_fluxes = get_ir_flux(base_name, database_name, wise_data, status,
-                                       service=service, load_from_bigdata_dir=load_from_bigdata_dir)
+                                       service=service, load_from_bigdata_dir=load_from_bigdata_dir,
+                                       correct_with_catalog_magnitudes=correct_with_catalog_magnitudes)
         fluxes.update({str(i): status_ir_fluxes[str(i)] for i in _index[m]})
 
     return fluxes
 
 
 def get_max_flux(
         base_name: str,
         database_name: str,
         wise_data: WISEDataBase,
         index: Index,
         service: str = "tap",
-        load_from_bigdata_dir: bool = False
+        load_from_bigdata_dir: bool = False,
+        correct_with_catalog_magnitudes: bool = False
 ) -> pd.DataFrame:
     """
     Get the maximum flux of the flares by index. Gets the time of the maximum flux from the database and
     returns the flux at that time.
 
     :param base_name: base name for storage directories
     :type base_name: str
@@ -247,24 +261,27 @@
     :type wise_data: WISEDataBase
     :param index: index of the object
     :type index: Index
     :param service: service to use for the TAP query, defaults to "tap", passed to :func:`get_lightcurves`
     :type service: str, optional
     :param load_from_bigdata_dir: load from the bigdata directory, defaults to False, passed to :func:`get_lightcurves`
     :type load_from_bigdata_dir: bool, optional
+    :param correct_with_catalog_magnitudes: if True, the flux is corrected with the magnitudes from the parent sample
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: dictionary with the index as key and the maximum flux as value
     :rtype: dict
     """
 
     logger.info(f"getting max flux for {len(np.atleast_1d(index))} objects of {base_name}")
     database_connector = DatabaseConnector(base_name=base_name, database_name=database_name)
     jd_of_max_flux = database_connector.get_peak_time_jd(index)
     mjd_of_max_flux = jd_of_max_flux + jd_offset
     fluxes = get_ir_flux_index(base_name, database_name, wise_data, index,
-                               service=service, load_from_bigdata_dir=load_from_bigdata_dir)
+                               service=service, load_from_bigdata_dir=load_from_bigdata_dir,
+                               correct_with_catalog_magnitudes=correct_with_catalog_magnitudes)
     max_fluxes = {}
     for i in tqdm(index, desc="getting max fluxes"):
         lc = pd.DataFrame(fluxes[str(i)])
         i_max_fluxes = {}
         for b in ["W1", "W2"]:
             m = (lc.mean_mjd - mjd_of_max_flux.loc[str(i), f"max_mag_jd_{b}"]).abs() < 1e-9
             i_max_fluxes[f"{b}_max_flux"] = lc[m][f"{b}_{flux_key}"].values[0]
```

### Comparing `timewise_sup-0.4.8/timewise_sup/meta_analysis/integrate_time.py` & `timewise_sup-0.5.0/timewise_sup/meta_analysis/integrate_time.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/meta_analysis/ir_energy.py` & `timewise_sup-0.5.0/timewise_sup/meta_analysis/ir_energy.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,28 +12,26 @@
 * :func:`get_ir_energy_index` calculates the IR energy for a given index
 
 """
 
 import logging
 import os
 import json
-from collections.abc import Mapping
 import numpy as np
 import pandas as pd
-from scipy import integrate
+from pathlib import Path
 from timewise.wise_data_base import WISEDataBase
 
 from timewise_sup.environment import load_environment
 from timewise_sup.mongo import DatabaseConnector, Index, Status
 from timewise_sup.meta_analysis.luminosity import (
     get_ir_luminosities,
     luminosity_key,
     luminosity_err_key,
     ref_time_key,
-    get_ref_time
 )
 from timewise_sup.meta_analysis.integrate_time import time_integral
 
 
 logger = logging.getLogger(__name__)
 
 ir_energy_key = "ir_energy_erg"
@@ -42,14 +40,15 @@
 
 def calculate_ir_energy(
         base_name: str,
         database_name: str,
         wise_data: WISEDataBase,
         status: Status,
         redshifts: pd.DataFrame | None = None,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Calculate the IR energy of the flares. This is done by integrating the luminosity over the duration of the flare.
 
     :param base_name: base name for storage directories
     :type base_name: str
     :param database_name: name of the database
@@ -58,22 +57,26 @@
     :type wise_data: WISEDataBase
     :param status: status of the flare
     :type status: Status
     :param redshifts:
         redshift of the object, defaults to getting the redshift from the AMPEL catalog crossmatch,
         needs keys `z` and `z_unc`
     :type redshifts: pandas.DataFrame | None
+    :param correct_with_catalog_magnitudes: if True, the flux is corrected with the magnitudes from the parent sample
+    :type correct_with_catalog_magnitudes: bool
     :return: dictionary with the index as key and the IR energy as value
     :rtype: dict
     """
     database_connector = DatabaseConnector(base_name=base_name, database_name=database_name)
     ids = database_connector.get_ids(status)
     indices = np.atleast_1d(ids)
     logger.info(f"calculating luminosities for {len(indices)} objects")
-    luminosity_dict = get_ir_luminosities(base_name, database_name, wise_data, status, redshifts=redshifts)
+    luminosity_dict = get_ir_luminosities(base_name, database_name, wise_data, status,
+                                          redshifts=redshifts,
+                                          correct_with_catalog_magnitudes=correct_with_catalog_magnitudes)
     excess_mjd = database_connector.get_excess_mjd(indices)
 
     engs = {}  # type: dict[str, dict[str, float] | None]
 
     for k, lum_info in luminosity_dict.items():
 
         if lum_info is None:
@@ -111,14 +114,15 @@
 def get_ir_energy_status(
         base_name: str,
         database_name: str,
         status: Status,
         redshifts: pd.DataFrame | None = None,
         wise_data: WISEDataBase | None = None,
         force_new: bool = False,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Get the IR energy of the flares per status. If the cache file `ir_eng_status{status}.json` exists, it is loaded from there.
     If it does not exist, it is calculated by :func:`calculate_ir_energy` and stored there.
 
     :param base_name: base name for storage directories
     :type base_name: str
@@ -130,34 +134,38 @@
         redshift of the object, defaults to getting the redshift from the AMPEL catalog crossmatch,
         needs keys `z` and `z_unc`
     :type redshifts: pandas.DataFrame | None
     :param wise_data: instance of WISEDataBase
     :type wise_data: WISEDataBase
     :param force_new: if True, the IR energy is calculated and stored in the cache file, even if it already exists
     :type force_new: bool
+    :param correct_with_catalog_magnitudes: if True, the flux is corrected with the magnitudes from the parent sample
+    :type correct_with_catalog_magnitudes: bool
     :return: dictionary with the index as key and the IR energy as value
     :rtype: dict
     """
     logger.info(f"getting bolometric luminosities for status {status}")
-    tsup_data_dir = load_environment("TIMEWISE_SUP_DATA")
-    fn = os.path.join(tsup_data_dir, base_name, f"ir_eng_status{status}.json")
+    tsup_data_dir = Path(load_environment("TIMEWISE_SUP_DATA"))
+    catalog_desc = "_with_catalog_magnitudes" if correct_with_catalog_magnitudes else ""
+    fn = tsup_data_dir / base_name / f"ir_eng_status{status}{catalog_desc}.json"
 
     if (not os.path.isfile(fn)) or force_new:
 
         if wise_data is None:
             raise ValueError("wise_data must be given when calculating IR energies!")
         else:
             logger.debug(f"No file {fn}.")
             logger.info("Making bolometric luminosities")
             engs = calculate_ir_energy(
                 base_name=base_name,
                 database_name=database_name,
                 wise_data=wise_data,
                 status=status,
                 redshifts=redshifts,
+                correct_with_catalog_magnitudes=correct_with_catalog_magnitudes
             )
 
         with open(fn, "w") as f:
             json.dump(engs, f)
 
     else:
         logger.debug(f"loading {fn}")
@@ -181,34 +189,46 @@
 
 def get_ir_energy_index(
         base_name: str,
         database_name: str,
         index: Index,
         wise_data: WISEDataBase,
         forcenew: bool = False,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Get the IR energy of the flares per index by getting the status and calling :func:`get_ir_energy_status`
     for each status.
 
     :param base_name:
     :type base_name: str
     :param database_name:
     :type database_name: str
     :param index: index of the lightcurve
     :type index: Index
+    :param wise_data: instance of WISEDataBase
+    :type wise_data: WISEDataBase
     :param forcenew: if True, the IR energy is calculated and stored in the cache file, even if it already exists
-    :type forcenew: bool
+    :type forcenew: bool, optional
+    :param correct_with_catalog_magnitudes: if True, the flux is corrected with the magnitudes from the parent sample
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: dictionary with the index as key and the IR energy as value
     :rtype: dict
     """
 
     statuses = DatabaseConnector(base_name=base_name, database_name=database_name).get_status(index)
 
     engs_all = dict()
 
     for status in statuses.status.unique():
-        eng = get_ir_energy_status(base_name, database_name, status, wise_data, forcenew)
+        eng = get_ir_energy_status(
+            base_name=base_name,
+            database_name=database_name,
+            status=status,
+            wise_data=wise_data,
+            force_new=forcenew,
+            correct_with_catalog_magnitudes=correct_with_catalog_magnitudes
+        )
         selected_lums = {k: v for k, v in eng.items() if k in statuses.index[statuses.status == status]}
         engs_all.update(selected_lums)
 
     return engs_all
```

### Comparing `timewise_sup-0.4.8/timewise_sup/meta_analysis/luminosity.py` & `timewise_sup-0.5.0/timewise_sup/meta_analysis/luminosity.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 * :func:`calculate_ir_luminosities` calculates the IR luminosities for a given index
 * :func:`get_ir_luminosities` calculates the IR luminosities for a given status
 """
 
 import logging
 import os
 import json
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
 from astropy import units as u
 from astropy.cosmology import Planck18
 from astropy.uncertainty import normal
 from timewise.wise_data_base import WISEDataBase
@@ -44,14 +45,16 @@
 def calculate_ir_luminosities(
         base_name: str,
         database_name: str,
         wise_data: WISEDataBase,
         index: Index,
         redshift: pd.Series,
         redshift_err: pd.Series,
+        load_from_bigdata_dir: bool = False,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Calculates the IR luminosities for a given index. The IR luminosity is calculated by multiplying the flux density
     with the area of the sphere with the radius of the luminosity distance. The luminosity distance is calculated
     using the Planck18 cosmology. The area is calculated using the formula for the surface area of a sphere.
 
     :param base_name: base name for storage directories
@@ -62,24 +65,30 @@
     :type wise_data: WISEDataBase
     :param index: index of the object
     :type index: Index
     :param redshift: redshift of the object
     :type redshift: pd.Series
     :param redshift_err: redshift error of the object
     :type redshift_err: pd.Series
+    :load_from_bigdata_dir: if True, the data is loaded from the bigdata directory
+    :type load_from_bigdata_dir: bool, optional
+    :param correct_with_catalog_magnitudes: if True, the flux is corrected with the magnitudes from the parent sample
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: dictionary with the index as key and the IR luminosities as value
     :rtype: dict
     """
     indices = tuple(np.atleast_1d(index).astype(int))
     logger.info(f"calculating luminosities for {len(indices)} objects")
 
     if len(indices) != len(redshift):
         raise ValueError("redshift and index must have the same length!")
 
-    lcs = get_ir_flux_index(base_name, database_name, wise_data, indices)
+    lcs = get_ir_flux_index(base_name, database_name, wise_data, indices,
+                            load_from_bigdata_dir=load_from_bigdata_dir,
+                            correct_with_catalog_magnitudes=correct_with_catalog_magnitudes)
     logger.debug(f"got {len(lcs)} lightcurves")
 
     ref_times = get_ref_time(base_name, database_name, indices)
     ref_times.index = ref_times.index.astype(str)
     lcs_with_luminosities = dict()
 
     # avoid SettingWithCopyWarning which falsely flags something like lc[ref_time_key] = ...
@@ -88,17 +97,15 @@
         for i, lc_dict in lcs.items():
             lc_in = pd.DataFrame.from_dict(lc_dict, orient="columns")
             lc = lc_in[["mean_mjd"]]
 
             iredshift = redshift[i]
             iredshift_err = redshift_err[i]
 
-            one_plus_z = 1 + iredshift
-            one_plus_z_err = iredshift_err if not np.isnan(iredshift_err) else 0
-            one_by_one_plus_z = 1 / one_plus_z
+            one_by_one_plus_z = 1 / (1 + iredshift)
 
             dl = Planck18.luminosity_distance(iredshift)
             area = 4 * np.pi * dl ** 2
 
             # estimate the uncertainty of the luminosity distance by sampling the redshift distribution
             # if the uncertainty of the redshift is given
             if not np.isnan(iredshift_err):
@@ -111,21 +118,18 @@
             lc[ref_time_key] = (lc["mean_mjd"] - ref_times.loc[i]) * one_by_one_plus_z
 
             for b in ["W1", "W2"]:
 
                 flux_val = u.Quantity(lc_in[f"{b}_{flux_key}"] * u.Unit("erg s-1 cm-2"))
                 flux_valerr = u.Quantity(lc_in[f"{b}_{flux_err_key}"] * u.Unit("erg s-1 cm-2"))
 
-                lum = u.Quantity(flux_val * area * one_plus_z).to("erg s-1").value
+                # see http://arxiv.org/abs/astro-ph/9905116, ch. 7, eq 24
+                lum = u.Quantity(flux_val * area).to("erg s-1").value
                 lum_err = u.Quantity(
-                    np.sqrt(
-                        (flux_valerr * area * one_plus_z) ** 2
-                        + (flux_val * area_unc * one_plus_z) ** 2
-                        + (flux_val * area * one_plus_z_err) ** 2
-                    )
+                    np.sqrt((flux_valerr * area) ** 2 + (flux_val * area_unc) ** 2)
                 ).to("erg s-1").value
 
                 lc[f"{b}_{luminosity_key}"] = lum
                 lc[f"{b}_{luminosity_err_key}"] = lum_err
 
             lum_dict = {
                 "lightcurve": lc.to_dict(),
@@ -143,14 +147,16 @@
 def get_ir_luminosities(
         base_name: str,
         database_name: str,
         wise_data: WISEDataBase,
         status: Status,
         force_new: bool = False,
         redshifts: pd.DataFrame | None = None,
+        load_from_bigdata_dir: bool = False,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     """
     Calculates the IR luminosities of the lightcurves in the database for a given status. If the cache file
     `lum_ir_lcs_status{status}.json` exists, it is loaded from there. If it does not exist, it is calculated by
     :func:`calculate_ir_luminosities` and stored there.
 
     :param base_name: base name for storage directories
@@ -163,21 +169,26 @@
     :type status: Status
     :param force_new: if True, the luminosities are calculated even if the cache file exists
     :type force_new: bool
     :param redshifts:
         redshift of the object, defaults to getting the redshift from the AMPEL catalog crossmatch,
         needs keys `z` and `z_unc`
     :type redshifts: pandas.DataFrame | None
+    :param load_from_bigdata_dir: if True, the data is loaded from the bigdata directory
+    :type load_from_bigdata_dir: bool, optional
+    :param correct_with_catalog_magnitudes: if True, the flux is corrected with the magnitudes from the parent sample
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: dictionary with the index as key and the IR luminosities as value
     :rtype: dict
     """
 
     logger.info(f"getting luminosities for status {status}")
-    tsup_data_dir = load_environment("TIMEWISE_SUP_DATA")
-    fn = os.path.join(tsup_data_dir, base_name, f"lum_ir_lcs_status{status}.json")
+    tsup_data_dir = Path(load_environment("TIMEWISE_SUP_DATA"))
+    catalog_desc = "_with_catalog_magnitudes" if correct_with_catalog_magnitudes else ""
+    fn = tsup_data_dir / base_name / f"lum_ir_lcs_status{status}{catalog_desc}.json"
 
     database_connector = DatabaseConnector(base_name=base_name, database_name=database_name)
     indices = database_connector.get_ids(status)
 
     if (not os.path.isfile(fn)) or force_new:
         logger.debug(f"No file {fn}")
         logger.info("calculating luminosities")
@@ -188,15 +199,17 @@
 
         lcs = calculate_ir_luminosities(
             base_name,
             database_name,
             wise_data,
             redshifts.index,
             redshifts["z"],
-            redshifts["z_unc"]
+            redshifts["z_unc"],
+            load_from_bigdata_dir=load_from_bigdata_dir,
+            correct_with_catalog_magnitudes=correct_with_catalog_magnitudes
         )
 
         missing_mask = ~pd.Index(indices).astype(str).isin(lcs.keys())
         if any(missing_mask):
             logger.warning(f"missing {missing_mask.sum()} lightcurves")
             missing_indices = np.array(indices)[missing_mask]
             for i in missing_indices:
@@ -224,25 +237,27 @@
 def get_ir_luminosities_index(
         base_name: str,
         database_name: str,
         wise_data: WISEDataBase,
         index: Index,
         force_new: bool = False,
         redshifts: pd.DataFrame | None = None,
+        correct_with_catalog_magnitudes: bool = False
 ) -> dict:
     logger.info(f"getting luminosities for {len(np.atleast_1d(index))} indices")
     database_connector = DatabaseConnector(base_name=base_name, database_name=database_name)
     statuses = database_connector.get_status(index)
     unique_statuses = statuses.status.unique()
     logger.debug(f"unique statuses: {unique_statuses}")
 
     lums_all = dict()
 
     for status in unique_statuses:
-        lums = get_ir_luminosities(base_name, database_name, wise_data, status, force_new, redshifts)
+        lums = get_ir_luminosities(base_name, database_name, wise_data, status, force_new, redshifts,
+                                   correct_with_catalog_magnitudes=correct_with_catalog_magnitudes)
         selected_lums = {k: v for k, v in lums.items() if k in statuses.index[statuses.status == status]}
         lums_all.update(selected_lums)
 
     logger.debug(f"got {len(lums_all)} lightcurves")
     return lums_all
```

### Comparing `timewise_sup-0.4.8/timewise_sup/meta_analysis/rejection_reason.py` & `timewise_sup-0.5.0/timewise_sup/meta_analysis/rejection_reason.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,42 +14,14 @@
 
 from timewise_sup.mongo import DatabaseConnector, Index
 
 
 logger = logging.getLogger(__name__)
 
 
-def get_rejected_ids(
-        base_name: str,
-        database_name: str,
-):
-    """
-    Get the ids of the rejected objects. The rejection reason is given in the description of the
-    ``AMPEL`` ``T2DustEchoEval`` unit output.
-
-    :param base_name: base name of the wise data
-    :type base_name: str
-    :param database_name: name of the database
-    :type database_name: str
-    :return: ids of the rejected objects
-    :rtype: list
-    """
-    logger.info(f"getting rejected ids for {base_name}")
-    rejected = (
-        "No further investigation",
-        "1_maybe_interesting",
-        "2_maybe_interesting",
-        "3", "3_maybe_interesting",
-        "4", "4_maybe_interesting"
-    )
-    database_connector = DatabaseConnector(base_name=base_name, database_name=database_name)
-    ids = database_connector.get_ids(rejected)
-    return ids
-
-
 def get_rejection_reason(
         base_name: str,
         database_name: str
 ) -> dict:
     """
     Get the number of objects per rejection reason. The rejection reason is given in the description of the
     ``AMPEL`` ``T2DustEchoEval`` unit output.
@@ -58,16 +30,16 @@
     :type base_name: str
     :param database_name: name of the database
     :type database_name: str
     :return: dictionary with the rejection reason as key and the number of objects as value
     :rtype: dict
     """
     logger.info(f"getting rejection reason for {base_name}")
-    ids = get_rejected_ids(base_name, database_name)
     database_connector = DatabaseConnector(base_name=base_name, database_name=database_name)
+    ids = database_connector.get_rejected_ids()
     desc = database_connector.get_t2_dust_echo_eval_descriptions(ids)
     desc_counts = desc.description.value_counts()  # type: pd.Series
 
     # when there is a gap in the lightcurve before a potential excess, the status will be "_maybe_interesting"
     # but can have the accepted description. We can replace it with the more meaningful "gap"
     ac_str = 'Baseline before excess region, Excess region exists, Baseline before excess region, Excess region exists'
     desc_counts.rename(index={ac_str: "gap"}, inplace=True)
@@ -125,15 +97,15 @@
     :rtype: pd.DataFrame
     """
     connector = DatabaseConnector(base_name=base_name, database_name=database_name)
     _index = pd.Index(index)
     info = pd.DataFrame(index=_index, columns=["rejection_reason"], dtype=str)
 
     # find rejected ids
-    rejected_ids = get_rejected_ids(base_name, database_name)
+    rejected_ids = connector.get_rejected_ids()
 
     # find indices that have not been run, probably because of chi2 cut
     accepted_index = pd.Index(connector.get_ids(("1", "2")))
     info.loc[_index[_index.isin(index)], "rejection_reason"] = "accepted"
 
     # find indices that have not been run, probably because of chi2 cut
     not_run_index = _index[~_index.isin(accepted_index) & ~_index.isin(rejected_ids)]
```

### Comparing `timewise_sup-0.4.8/timewise_sup/mongo.py` & `timewise_sup-0.5.0/timewise_sup/mongo.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import logging
 import os
 import json
 import pandas as pd
 import numpy as np
 from tqdm import tqdm
-from pymongo import MongoClient, collection, database
+from pymongo import MongoClient, collection, database, errors as pymongo_errors
 from collections.abc import Sequence
 from pydantic import BaseModel
 from pathlib import Path
 
 from timewise_sup.environment import load_environment
 
 
@@ -140,14 +140,19 @@
 
     @staticmethod
     def connect_to_db() -> MongoClient:
         """Return the :class:`MongoClient`"""
         mongodb_port = load_environment("TIMEWISE_SUP_MONGODB_PORT")
         logger.debug(f"connecting to MongoDB at {mongodb_port}")
         client: MongoClient = MongoClient(f"mongodb://localhost:{mongodb_port}/")
+        try:
+            # The ping command is cheap and does not require auth.
+            client.admin.command('ping')
+        except pymongo_errors.ConnectionFailure as e:
+            raise pymongo_errors.ConnectionFailure(f"Could not connect to MongoDB at {mongodb_port}!") from e
         logger.debug("connected")
         return client
 
     def get_dataframe(
             self,
             collection_name: str,
             field_name_lists: list[list[str | int]],
@@ -327,14 +332,32 @@
 
                 logger.debug(f"got {len(istocks)} ids")
 
             stocks.extend(istocks)
 
         return stocks
 
+    def get_rejected_ids(self):
+        """
+        Get the ids of the rejected objects. The rejection reason is given in the description of the
+        ``AMPEL`` ``T2DustEchoEval`` unit output.
+
+        :return: ids of the rejected objects
+        :rtype: list
+        """
+        logger.debug(f"getting rejected ids")
+        rejected = (
+            "No further investigation",
+            "1_maybe_interesting",
+            "2_maybe_interesting",
+            "3", "3_maybe_interesting",
+            "4", "4_maybe_interesting"
+        )
+        return self.get_ids(rejected)
+
     def get_excess_mjd(self, index: Index) -> pd.DataFrame:
         """
         Get the excess time for the given index
 
         :param index: The wanted index
         :type index: Index
         :return: Modified Julian Days of the excess, per filter, start, end and if flare ended
@@ -366,54 +389,88 @@
                     i_excess_mjds[f"{f}_excess_end_mjd"] = max(max_excess_mjds)
                     i_excess_mjds[f"{f}_flare_ended"] = excess_ended
 
                 excess_mjds[str(x["stock"])] = i_excess_mjds
 
         return pd.DataFrame.from_dict(excess_mjds, orient="index")
 
-    def get_baselines(self, index: Index) -> dict:
+    def _calculate_baselines(self, index: Index) -> pd.DataFrame:
         """
         Returns the baseline for the lightcurves.
 
         :param index: The index of the lightcurves
         :type index: Index
         :returns: The value of the baseline flux and the :math:`1\sigma` uncertainty per filter
         :rtype: dict
         """
-        baseline = dict()
-
         indices = as_list(index)
         logger.debug(f"reading baseline values for {len(indices)} objects")
 
+        columns = ["W1_baseline", "W1_baseline_sigma", "W2_baseline", "W2_baseline_sigma"]
+        baseline = pd.DataFrame(columns=columns, index=pd.Index(indices).astype(str))
+
         for chunked_indices in chunks(indices, int(5e5)):
 
             dust_echo_filter = {
                 "unit": "T2DustEchoEval",
                 "stock": {"$in": chunked_indices},
                 "code": 0
             }
 
             for x in self.t2collection.find(
                     dust_echo_filter,
                     {"stock": 1}
             ):
-                i_baseline = dict()
+                stock = x["stock"]
+                stock_str = str(stock)
                 for y in self.t2collection.find(
-                        {"unit": "T2BayesianBlocks", "stock": x["stock"], "code": 0},
+                        {"unit": "T2BayesianBlocks", "stock": stock, "code": 0},
                         {f"body.Wise_{b}.baseline{s}": 1 for b in ["W1", "W2"] for s in ["", "_sigma"]},
                         limit=1
                 ):
                     for b in ["W1", "W2"]:
-                        i_baseline[f"{b}_baseline"] = y["body"][-1][f"Wise_{b}"]["baseline"]
-                        i_baseline[f"{b}_baseline_sigma"] = y["body"][-1][f"Wise_{b}"]["baseline_sigma"]
-
-                baseline[str(x["stock"])] = i_baseline
+                        baseline.loc[stock_str, f"{b}_baseline"] = y["body"][-1][f"Wise_{b}"]["baseline"]
+                        baseline.loc[stock_str, f"{b}_baseline_sigma"] = y["body"][-1][f"Wise_{b}"]["baseline_sigma"]
 
         return baseline
 
+    def get_baselines(self, index: Index) -> pd.DataFrame:
+        """
+        Returns the baseline for the lightcurves. Caches result to file when first called.
+
+        :param index: The index of the lightcurves
+        :type index: Index
+        :returns: The value of the baseline flux and the :math:`1\sigma` uncertainty per filter
+        :rtype: dict
+        """
+        fn = self.cache_dir / "baselines.csv"
+
+        if not os.path.isfile(fn):
+            logger.debug(f"no file {fn}")
+            baseline = self._calculate_baselines(index)
+            logger.debug(f"saving to {fn}")
+            fn.parent.mkdir(parents=True, exist_ok=True)
+            baseline.to_csv(fn)
+
+        else:
+            logger.debug(f"loading {fn}")
+            baseline = pd.read_csv(fn, index_col=0)
+            baseline.set_index(baseline.index.astype(str), inplace=True)
+
+        indices = pd.Index(index).astype(str)
+        indices_present = indices.isin(baseline.index)
+        if np.any(~indices_present):
+            logger.debug(f"{np.sum(~indices_present)} indices not found. calculating")
+            baseline_suplement = self._calculate_baselines(indices[~indices_present].astype(int))
+            baseline = pd.concat([baseline, baseline_suplement])
+            logger.debug(f"saving {len(baseline)} baselines to {fn}")
+            baseline.to_csv(fn)
+
+        return baseline.loc[indices]
+
     def _calculate_t2_dust_echo_eval_descriptions(self, index: Index) -> pd.DataFrame:
         """
         Get the description for the lightcurves
 
         :param index: The index of the lightcurves
         :type index: Index
         :return: Description per lightcurves, separated by ", "
@@ -497,14 +554,98 @@
         stocks = list()
         for lc in self.t2collection.find(filter, cols):
             stocks.append(lc["stock"])
 
         logger.debug(f"returning {len(stocks)} stock IDs")
         return stocks
 
+    def get_strength(self, index: Index | str) -> pd.DataFrame:
+        """
+        Get the strength of the dust echo and the significance of the pre-flare variability per band
+
+        :param index: The index of the lightcurves or "all"
+        :type index: Index | str
+        :return: The strength and significance per band
+        :rtype: pandas.DataFrame
+        """
+        logger.info("getting strength")
+
+        # load previous results if exist
+        columns = [
+            "W1_strength", "W1_pre_flare_var_sig", "W1_strength_by_var",
+            "W2_strength", "W2_pre_flare_var_sig", "W2_strength_by_var",
+            "min_strength", "max_var", "min_strength_by_var"
+        ]
+
+        use_all_indices = (isinstance(index, str) and (index == "all"))
+
+        filename = self.cache_dir / "strength.json"
+        if filename.is_file():
+            logger.debug(f"loading strength from {filename}")
+            strengths = pd.read_json(filename)
+            strengths.set_index(strengths.index.astype(str), inplace=True)
+        else:
+            logger.debug(f"{filename} not found, creating empty DataFrame")
+            strengths = pd.DataFrame(columns=columns)
+
+        # set up query filter
+        mongo_filter = {
+            "unit": "T2BayesianBlocks",
+            "code": 0
+        }
+
+        # if indices are specified, check if strengths are missing
+        if not use_all_indices:
+            _index = pd.Index(index).astype(str)
+            missing_mask = ~_index.isin(strengths.index.astype(str))
+            if missing_mask.any():
+                logger.debug(f"found {missing_mask.sum()} missing strengths")
+                strengths = pd.concat([strengths, pd.DataFrame(index=_index[missing_mask], columns=columns)])
+                mongo_filter["stock"] = {"$in": as_list(_index[missing_mask].astype(int))}
+            else:
+                logger.debug(f"all strengths found")
+                return strengths.loc[_index.astype(str)]
+
+        # if no indices are specified, check which of all strengths are missing
+        else:
+            logger.debug("checking for missing strengths")
+            _all_ids = pd.Index(self.get_ids("1") + self.get_ids("2") + self.get_rejected_ids()).astype(str)
+            logger.debug(f"found {len(_all_ids)} IDs")
+            missing_ids = _all_ids[~_all_ids.isin(strengths.index.astype(str))]
+            logger.debug(f"found {len(missing_ids)} missing strengths")
+            if len(missing_ids) < 1e6:
+                logger.debug(f"only querying for {len(missing_ids)} missing strengths")
+                mongo_filter["stock"] = {"$in": as_list(missing_ids)}
+            else:
+                logger.debug("more than 1e6 missing, querying for all strengths")
+            strengths = pd.concat([strengths, pd.DataFrame(index=missing_ids, columns=columns)])
+
+        # get the strengths
+        logger.debug("getting strengths")
+        for i, x in tqdm(enumerate(self.t2collection.find(mongo_filter)), desc="getting strengths"):
+            stock = str(x["stock"])
+            for band in ["W1", "W2"]:
+                res = x["body"][-1][f"Wise_{band}"]
+                strengths.loc[stock, f"{band}_strength"] = res["strength_sjoert"]
+                strengths.loc[stock, f"{band}_pre_flare_var_sig"] = res["significance"]
+
+        if ((not use_all_indices) and missing_mask.any()) or use_all_indices:
+            strengths["min_strength"] = strengths[["W1_strength", "W2_strength"]].min(axis=1)
+            strengths["max_var"] = strengths[["W1_pre_flare_var_sig", "W2_pre_flare_var_sig"]].max(axis=1)
+            strengths["W1_strength_by_var"] = strengths["W1_strength"] / strengths["W1_pre_flare_var_sig"]
+            strengths["W2_strength_by_var"] = strengths["W2_strength"] / strengths["W2_pre_flare_var_sig"]
+            strengths["min_strength_by_var"] = strengths[["W1_strength_by_var", "W2_strength_by_var"]].min(axis=1)
+            logger.debug(f"saving {len(strengths)} strengths to {filename}")
+            strengths.to_json(filename)
+
+        if not use_all_indices:
+            strengths = strengths.loc[_index.astype(str)]
+
+        return strengths
+
     def get_t2_dust_echo_eval_values(self, index: Index, value: str) -> pd.DataFrame:
         """
         Get a value per filter and lightcurve as produced by the :class:`AMPEL` :class:`T2DustEchoEval`
 
         :param index: The index of the lightcurves
         :type index: Index
         :param value: The key of the value
@@ -549,15 +690,20 @@
         return self.get_t2_dust_echo_eval_values(index, "max_mag_jd")
 
     def get_excess_end_jd(self, index: Index) -> pd.DataFrame:
         """Get the start of the excess in Julian Days"""
         return self.get_t2_dust_echo_eval_values(index, "excess_jd")
 
     def get_dust_echo_strength(self, index: Index) -> pd.DataFrame:
-        """Get the strength of the dust echo"""
+        """
+        Get the strength of the dust echo.
+        .. note::
+            This will only work if the object is status 1 or 2. If you want the strength for any object,
+            use :meth:`get_strength` instead.
+        """
         return self.get_t2_dust_echo_eval_values(index, "strength_sjoert")
 
     def get_fade_time(self, index: Index) -> pd.DataFrame:
         """Get the fade time"""
         return self.get_t2_dust_echo_eval_values(index, "e_fade")
 
     def get_rise_time(self, index: Index) -> pd.DataFrame:
@@ -600,38 +746,74 @@
             }
 
             for i in self.t2collection.find(filter):
                 matches[i["stock"]] = i["body"][-1]
 
         return matches
 
-    def get_redshift(self, index: Index) -> pd.DataFrame:
+    def get_redshift(self, index: Index, code: int = 0) -> pd.DataFrame:
         """
         Get the redshifts as determined by the :class:`AMPEL` :class:`T2DigestRedshifts`
 
         :param index: Index of the lightcurves
         :type index: Index
+        :param code: The document code to query T2CatalogMatch results to get match names
+        :type code: int
         :return: The redshift, distance to the match and the uncertainty associated to the redshift measurement method
         :rtype: pandas.DataFrame
         """
         filter = {
             "unit": "T2DigestRedshifts",
             "stock": {"$in": as_list(index)},
         }
 
         n = self.t2collection.count_documents(filter)
         logger.debug(f"found {n} documents")
 
+        redshift_keys = {
+            "NEDz_extcats": {"spec": "z"},
+            "SDSS_spec": {"spec": "z"},
+            "GLADEv23": {"spec": "z"},
+            "LSPhotoZZou": {"photo": "photoz", "spec": "specz"},
+            "wiseScosPhotoz": {"photo": "zPhoto_Corr"},
+            "twoMPZ": {"photo": "zPhoto", "spec": "zSpec"},
+            "PS1_photoz": {"photo": "z_phot"},
+            "NEDz": {"spec": "z"},
+        }
+
         redshift = dict()
+        matches = self.get_catalog_matches(index, code)
 
         for lc in self.t2collection.find(filter):
             try:
                 if "ampel_z" in lc["body"][-1]:
+
+                    # find the redshift as calculated by AMPEL T2DigestRedshift
                     d = {k: lc["body"][-1][k] for k in ["ampel_z", "ampel_dist", "group_z_precision"]}
                     redshift[str(lc["stock"])] = d
+
+                    # find the redshifts that were used to calculate the AMPEL redshift
+                    group_zs = lc["body"][-1]["group_zs"]
+                    if all([len(g) for g in group_zs]):
+                        raise ValueError(f"no group_zs found for {lc['stock']}")
+                    for group_z in group_zs:
+                        if len(group_z) > 0:
+                            break
+
+                    # find the catalog matches that provided the redshifts
+                    redshift_catalogs = []
+                    for catalog, result in matches[int(lc["stock"])].items():
+                        if (result is not None) and (catalog in redshift_keys):
+                            redshifts = [result[k] for k in redshift_keys[catalog].values() if k in result]
+                            if any([z in redshifts for z in group_z]):
+                                redshift_catalogs.append(catalog)
+                    if len(redshift_catalogs) == 0:
+                        raise ValueError(f"no redshift catalog found for {lc['stock']}")
+                    redshift[str(lc["stock"])]["catalogs"] = ", ".join(redshift_catalogs)
+
                 else:
                     redshift[str(lc["stock"])] = {"ampel_z": np.nan, "ampel_dist": np.nan, "group_z_precision": np.nan}
             except KeyError as e:
                 raise KeyError(f"{lc}: {e}")
 
         logger.debug(f"returning {len(redshift)} results")
```

### Comparing `timewise_sup-0.4.8/timewise_sup/plots/__init__.py` & `timewise_sup-0.5.0/timewise_sup/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/plots/chi2_histograms.py` & `timewise_sup-0.5.0/timewise_sup/plots/chi2_histograms.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/plots/color_plots.py` & `timewise_sup-0.5.0/timewise_sup/plots/color_plots.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/plots/ensemble_lightcurves.py` & `timewise_sup-0.5.0/timewise_sup/plots/ensemble_lightcurves.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/plots/ir_energies.py` & `timewise_sup-0.5.0/timewise_sup/plots/ir_energies.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/plots/plot_lightcurves.py` & `timewise_sup-0.5.0/timewise_sup/plots/plot_lightcurves.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,15 +76,16 @@
 
 def plot_single_lightcurve(
         base_name: str,
         database_name: str,
         wise_data: WISEDataBase,
         index: str,
         service: str = "tap",
-        load_from_bigdata_dir: bool = False
+        load_from_bigdata_dir: bool = False,
+        correct_with_catalog_magnitudes: bool = False
 ) -> tuple[mpl.figure.Figure, mpl.axes.Axes]:
     """
     Plot a single lightcurve.
 
     :param base_name: base name of the analysis
     :type base_name: str
     :param database_name: name of the database
@@ -93,25 +94,28 @@
     :type wise_data: WISEDataBase
     :param index: index of the lightcurve
     :type index: str
     :param service: service used to download the lightcurves, default "tap", passed to :func:`get_ir_flux_index`
     :type service: str, optional
     :param load_from_bigdata_dir: load from bigdata directory, defaults to False, passed to :func:`get_ir_flux_index`
     :type load_from_bigdata_dir: bool, optional
+    :param correct_with_catalog_magnitudes: if True, the flux is corrected with the magnitudes from the parent sample
+    :type correct_with_catalog_magnitudes: bool, optional
     :return: figure and axes
     :rtype: tuple[mpl.figure.Figure, mpl.axes.Axes]
     """
 
     wise_lc = pd.DataFrame.from_dict(get_ir_flux_index(
         base_name=base_name,
         database_name=database_name,
         wise_data=wise_data,
         index=index,
         service=service,
-        load_from_bigdata_dir=load_from_bigdata_dir
+        load_from_bigdata_dir=load_from_bigdata_dir,
+        correct_with_catalog_magnitudes=correct_with_catalog_magnitudes
     )[str(index)], orient="columns")
 
     return make_lightcurve_plot(wise_lc)
 
 
 def make_lightcurve_plot(
         wise_lc: pd.DataFrame,
```

### Comparing `timewise_sup-0.4.8/timewise_sup/plots/rise_fade_times.py` & `timewise_sup-0.5.0/timewise_sup/plots/rise_fade_times.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/plots/test_data_res.py` & `timewise_sup-0.5.0/timewise_sup/plots/test_data_res.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/samples/bts.py` & `timewise_sup-0.5.0/timewise_sup/samples/bts.py`

 * *Files identical despite different names*

### Comparing `timewise_sup-0.4.8/timewise_sup/samples/sjoerts_flares.py` & `timewise_sup-0.5.0/timewise_sup/samples/data/test_sample.json`

 * *Files 22% similar despite different names*

```diff
@@ -1,2175 +1,2006 @@
-00000000: 696d 706f 7274 206c 6f67 6769 6e67 0a69  import logging.i
-00000010: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
-00000020: 7064 0a66 726f 6d20 7469 6d65 7769 7365  pd.from timewise
-00000030: 2069 6d70 6f72 7420 5061 7265 6e74 5361   import ParentSa
-00000040: 6d70 6c65 4261 7365 2c20 5749 5345 4461  mpleBase, WISEDa
-00000050: 7461 4445 5359 436c 7573 7465 720a 0a66  taDESYCluster..f
-00000060: 726f 6d20 7469 6d65 7769 7365 5f73 7570  rom timewise_sup
-00000070: 2e63 6f6e 6669 675f 6c6f 6164 6572 2069  .config_loader i
-00000080: 6d70 6f72 7420 5469 6d65 7769 7365 5355  mport TimewiseSU
-00000090: 5043 6f6e 6669 670a 6672 6f6d 2074 696d  PConfig.from tim
-000000a0: 6577 6973 655f 7375 702e 6d6f 6e67 6f20  ewise_sup.mongo 
-000000b0: 696d 706f 7274 2044 6174 6162 6173 6543  import DatabaseC
-000000c0: 6f6e 6e65 6374 6f72 2c20 496e 6465 780a  onnector, Index.
-000000d0: 0a0a 6c6f 6767 6572 203d 206c 6f67 6769  ..logger = loggi
-000000e0: 6e67 2e67 6574 4c6f 6767 6572 285f 5f6e  ng.getLogger(__n
-000000f0: 616d 655f 5f29 0a0a 736a 6f65 7274 735f  ame__)..sjoerts_
-00000100: 6261 7365 5f6e 616d 6520 3d20 2273 6a6f  base_name = "sjo
-00000110: 6572 7473 5f66 6c61 7265 7322 0a73 6a6f  erts_flares".sjo
-00000120: 6572 7473 5f64 6174 6162 6173 655f 6e61  erts_database_na
-00000130: 6d65 203d 2073 6a6f 6572 7473 5f62 6173  me = sjoerts_bas
-00000140: 655f 6e61 6d65 0a0a 0a64 6566 2067 6574  e_name...def get
-00000150: 5f74 6573 745f 666c 6172 6573 5f63 6f6e  _test_flares_con
-00000160: 6669 6728 293a 0a20 2020 2063 6f6e 6669  fig():.    confi
-00000170: 6720 3d20 5469 6d65 7769 7365 5355 5043  g = TimewiseSUPC
-00000180: 6f6e 6669 6728 0a20 2020 2020 2020 2064  onfig(.        d
-00000190: 6174 6162 6173 655f 6e61 6d65 3d73 6a6f  atabase_name=sjo
-000001a0: 6572 7473 5f64 6174 6162 6173 655f 6e61  erts_database_na
-000001b0: 6d65 2c0a 2020 2020 2020 2020 7769 7365  me,.        wise
-000001c0: 5f64 6174 613d 5465 7374 5749 5345 4461  _data=TestWISEDa
-000001d0: 7461 2829 0a20 2020 2029 0a20 2020 2072  ta().    ).    r
-000001e0: 6574 7572 6e20 636f 6e66 6967 0a0a 0a63  eturn config...c
-000001f0: 6c61 7373 2054 6573 7457 4953 4544 6174  lass TestWISEDat
-00000200: 6128 5749 5345 4461 7461 4445 5359 436c  a(WISEDataDESYCl
-00000210: 7573 7465 7229 3a0a 0a20 2020 2064 6566  uster):..    def
-00000220: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00000230: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-00000240: 2020 2073 7570 6572 2854 6573 7457 4953     super(TestWIS
-00000250: 4544 6174 612c 2073 656c 6629 2e5f 5f69  EData, self).__i
-00000260: 6e69 745f 5f28 0a20 2020 2020 2020 2020  nit__(.         
-00000270: 2020 2062 6173 655f 6e61 6d65 3d54 6573     base_name=Tes
-00000280: 7450 6172 656e 7453 616d 706c 652e 6261  tParentSample.ba
-00000290: 7365 5f6e 616d 652c 0a20 2020 2020 2020  se_name,.       
-000002a0: 2020 2020 2070 6172 656e 745f 7361 6d70       parent_samp
-000002b0: 6c65 5f63 6c61 7373 3d54 6573 7450 6172  le_class=TestPar
-000002c0: 656e 7453 616d 706c 652c 0a20 2020 2020  entSample,.     
-000002d0: 2020 2020 2020 206e 5f63 6875 6e6b 733d         n_chunks=
-000002e0: 322c 0a20 2020 2020 2020 2020 2020 206d  2,.            m
-000002f0: 696e 5f73 6570 5f61 7263 7365 633d 360a  in_sep_arcsec=6.
-00000300: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00000310: 6566 2073 7562 6d69 745f 746f 5f63 6c75  ef submit_to_clu
-00000320: 7374 6572 280a 2020 2020 2020 2020 2020  ster(.          
-00000330: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00000340: 2020 2020 6e6f 6465 5f6d 656d 6f72 792c      node_memory,
-00000350: 0a20 2020 2020 2020 2020 2020 2073 696e  .            sin
-00000360: 676c 655f 6368 756e 6b3d 4e6f 6e65 2c0a  gle_chunk=None,.
-00000370: 2020 2020 2020 2020 2020 2020 6d61 736b              mask
-00000380: 5f62 795f 706f 7369 7469 6f6e 3d46 616c  _by_position=Fal
-00000390: 7365 0a20 2020 2029 3a0a 2020 2020 2020  se.    ):.      
-000003a0: 2020 6c6f 6767 6572 2e69 6e66 6f28 2265    logger.info("e
-000003b0: 6d75 6c61 7469 6e67 2063 6c75 7374 6572  mulating cluster
-000003c0: 2077 6f72 6b22 290a 0a20 2020 2020 2020   work")..       
-000003d0: 2023 2066 726f 6d20 7469 6d65 7769 7365   # from timewise
-000003e0: 2f77 6973 655f 6269 6764 6174 615f 6465  /wise_bigdata_de
-000003f0: 7379 5f63 6c75 7374 6572 2e70 790a 2020  sy_cluster.py.  
-00000400: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00000410: 6e63 6528 7369 6e67 6c65 5f63 6875 6e6b  nce(single_chunk
-00000420: 2c20 7479 7065 284e 6f6e 6529 293a 0a20  , type(None)):. 
-00000430: 2020 2020 2020 2020 2020 205f 7374 6172             _star
-00000440: 745f 6964 203d 2031 0a20 2020 2020 2020  t_id = 1.       
-00000450: 2020 2020 205f 656e 645f 6964 203d 2069       _end_id = i
-00000460: 6e74 2873 656c 662e 6e5f 6368 756e 6b73  nt(self.n_chunks
-00000470: 2a73 656c 662e 6e5f 636c 7573 7465 725f  *self.n_cluster_
-00000480: 6a6f 6273 5f70 6572 5f63 6875 6e6b 290a  jobs_per_chunk).
-00000490: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000004a0: 2020 2020 2020 2020 2020 5f73 7461 7274            _start
-000004b0: 5f69 6420 3d20 696e 7428 7369 6e67 6c65  _id = int(single
-000004c0: 5f63 6875 6e6b 2a73 656c 662e 6e5f 636c  _chunk*self.n_cl
-000004d0: 7573 7465 725f 6a6f 6273 5f70 6572 5f63  uster_jobs_per_c
-000004e0: 6875 6e6b 2920 2b20 310a 2020 2020 2020  hunk) + 1.      
-000004f0: 2020 2020 2020 5f65 6e64 5f69 6420 3d20        _end_id = 
-00000500: 696e 7428 5f73 7461 7274 5f69 6420 2b20  int(_start_id + 
-00000510: 7365 6c66 2e6e 5f63 6c75 7374 6572 5f6a  self.n_cluster_j
-00000520: 6f62 735f 7065 725f 6368 756e 6b29 202d  obs_per_chunk) -
-00000530: 2031 0a0a 2020 2020 2020 2020 6c6f 6767   1..        logg
-00000540: 6572 2e64 6562 7567 2866 224a 6f62 7320  er.debug(f"Jobs 
-00000550: 6672 6f6d 207b 5f73 7461 7274 5f69 647d  from {_start_id}
-00000560: 2074 6f20 7b5f 656e 645f 6964 7d22 290a   to {_end_id}").
-00000570: 0a20 2020 2020 2020 2066 6f72 206a 6f62  .        for job
-00000580: 5f69 6420 696e 2072 616e 6765 285f 7374  _id in range(_st
-00000590: 6172 745f 6964 2c20 5f65 6e64 5f69 642b  art_id, _end_id+
-000005a0: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-000005b0: 6c6f 6767 6572 2e64 6562 7567 2866 224a  logger.debug(f"J
-000005c0: 6f62 207b 6a6f 625f 6964 7d22 290a 2020  ob {job_id}").  
-000005d0: 2020 2020 2020 2020 2020 6368 756e 6b5f            chunk_
-000005e0: 6e75 6d62 6572 203d 2073 656c 662e 5f67  number = self._g
-000005f0: 6574 5f63 6875 6e6b 5f6e 756d 6265 725f  et_chunk_number_
-00000600: 666f 725f 6a6f 6228 6a6f 625f 6964 290a  for_job(job_id).
-00000610: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000620: 2e5f 7375 6270 726f 6365 7373 5f73 656c  ._subprocess_sel
-00000630: 6563 745f 616e 645f 6269 6e28 7365 7276  ect_and_bin(serv
-00000640: 6963 653d 2774 6170 272c 2063 6875 6e6b  ice='tap', chunk
-00000650: 5f6e 756d 6265 723d 6368 756e 6b5f 6e75  _number=chunk_nu
-00000660: 6d62 6572 2c20 6a6f 6249 443d 6a6f 625f  mber, jobID=job_
-00000670: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
-00000680: 7365 6c66 2e63 616c 6375 6c61 7465 5f6d  self.calculate_m
-00000690: 6574 6164 6174 6128 7365 7276 6963 653d  etadata(service=
-000006a0: 2774 6170 272c 2063 6875 6e6b 5f6e 756d  'tap', chunk_num
-000006b0: 6265 723d 6368 756e 6b5f 6e75 6d62 6572  ber=chunk_number
-000006c0: 2c20 6a6f 6249 443d 6a6f 625f 6964 290a  , jobID=job_id).
-000006d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000006e0: 310a 0a20 2020 2064 6566 2077 6169 745f  1..    def wait_
-000006f0: 666f 725f 6a6f 6228 7365 6c66 2c20 6a6f  for_job(self, jo
-00000700: 625f 6964 3d4e 6f6e 6529 3a0a 2020 2020  b_id=None):.    
-00000710: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-00000720: 2263 616c 6c65 6420 6475 6d6d 7920 7761  "called dummy wa
-00000730: 6974 2066 6f72 2063 6c75 7374 6572 2229  it for cluster")
-00000740: 0a0a 0a63 6c61 7373 2054 6573 7450 6172  ...class TestPar
-00000750: 656e 7453 616d 706c 6528 5061 7265 6e74  entSample(Parent
-00000760: 5361 6d70 6c65 4261 7365 293a 0a0a 2020  SampleBase):..  
-00000770: 2020 6261 7365 5f6e 616d 6520 3d20 736a    base_name = sj
-00000780: 6f65 7274 735f 6261 7365 5f6e 616d 650a  oerts_base_name.
-00000790: 0a20 2020 2064 6566 6175 6c74 5f6b 6579  .    default_key
-000007a0: 6d61 7020 3d20 7b0a 2020 2020 2020 2020  map = {.        
-000007b0: 2272 6122 3a20 2272 6122 2c0a 2020 2020  "ra": "ra",.    
-000007c0: 2020 2020 2264 6563 223a 2022 6465 6322      "dec": "dec"
-000007d0: 2c0a 2020 2020 2020 2020 2269 6422 3a20  ,.        "id": 
-000007e0: 226e 616d 6522 0a20 2020 207d 0a0a 2020  "name".    }..  
-000007f0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00000800: 656c 6629 3a0a 2020 2020 2020 2020 6c6f  elf):.        lo
-00000810: 6767 6572 2e69 6e66 6f28 2269 6e69 7469  gger.info("initi
-00000820: 616c 6973 696e 6720 7465 7374 2050 6172  alising test Par
-00000830: 656e 7453 616d 706c 6522 290a 2020 2020  entSample").    
-00000840: 2020 2020 7375 7065 7228 5465 7374 5061      super(TestPa
-00000850: 7265 6e74 5361 6d70 6c65 2c20 7365 6c66  rentSample, self
-00000860: 292e 5f5f 696e 6974 5f5f 2862 6173 655f  ).__init__(base_
-00000870: 6e61 6d65 3d54 6573 7450 6172 656e 7453  name=TestParentS
-00000880: 616d 706c 652e 6261 7365 5f6e 616d 6529  ample.base_name)
-00000890: 0a20 2020 2020 2020 2073 656c 662e 6466  .        self.df
-000008a0: 203d 2073 656c 662e 7361 6d70 6c65 2829   = self.sample()
-000008b0: 0a0a 2020 2020 6465 6620 6765 745f 7265  ..    def get_re
-000008c0: 6473 6869 6674 7328 7365 6c66 2c20 696e  dshifts(self, in
-000008d0: 6465 783a 2049 6e64 6578 2920 2d3e 2070  dex: Index) -> p
-000008e0: 642e 4461 7461 4672 616d 653a 0a20 2020  d.DataFrame:.   
-000008f0: 2020 2020 2072 6564 7368 6966 7473 203d       redshifts =
-00000900: 2073 656c 662e 6466 2e6c 6f63 5b69 6e64   self.df.loc[ind
-00000910: 6578 2c20 5b22 7a22 5d5d 0a20 2020 2020  ex, ["z"]].     
-00000920: 2020 2072 6564 7368 6966 7473 203d 2072     redshifts = r
-00000930: 6564 7368 6966 7473 5b72 6564 7368 6966  edshifts[redshif
-00000940: 7473 2021 3d20 27e2 8093 275d 2e61 7374  ts != '...'].ast
-00000950: 7970 6528 666c 6f61 7429 0a20 2020 2020  ype(float).     
-00000960: 2020 2072 6564 7368 6966 7473 203d 2072     redshifts = r
-00000970: 6564 7368 6966 7473 5b7e 7265 6473 6869  edshifts[~redshi
-00000980: 6674 735b 227a 225d 2e69 736e 6128 295d  fts["z"].isna()]
-00000990: 0a20 2020 2020 2020 2072 6564 7368 6966  .        redshif
-000009a0: 7473 5b22 7a5f 756e 6322 5d20 3d20 7265  ts["z_unc"] = re
-000009b0: 6473 6869 6674 735b 227a 225d 202a 2030  dshifts["z"] * 0
-000009c0: 2e30 310a 2020 2020 2020 2020 7265 6473  .01.        reds
-000009d0: 6869 6674 732e 7365 745f 696e 6465 7828  hifts.set_index(
-000009e0: 7265 6473 6869 6674 732e 696e 6465 782e  redshifts.index.
-000009f0: 6173 7479 7065 2873 7472 292c 2069 6e70  astype(str), inp
-00000a00: 6c61 6365 3d54 7275 6529 0a20 2020 2020  lace=True).     
-00000a10: 2020 2072 6574 7572 6e20 7265 6473 6869     return redshi
-00000a20: 6674 730a 0a20 2020 2040 7374 6174 6963  fts..    @static
-00000a30: 6d65 7468 6f64 0a20 2020 2064 6566 2073  method.    def s
-00000a40: 616d 706c 6528 293a 0a20 2020 2020 2020  ample():.       
-00000a50: 205f 7361 6d70 6c65 203d 207b 0a20 2020   _sample = {.   
-00000a60: 2020 2020 2020 2020 2022 3022 3a7b 0a20           "0":{. 
-00000a70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000a80: 6e61 6d65 223a 2241 5432 3031 3964 7367  name":"AT2019dsg
-00000a90: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000aa0: 2020 2022 7470 6561 6b22 3a35 3836 3230     "tpeak":58620
-00000ab0: 2e32 2c0a 2020 2020 2020 2020 2020 2020  .2,.            
-00000ac0: 2020 2020 2272 6973 6574 696d 6522 3a22      "risetime":"
-00000ad0: 3332 2e31 222c 0a20 2020 2020 2020 2020  32.1",.         
-00000ae0: 2020 2020 2020 2022 6661 6465 7469 6d65         "fadetime
-00000af0: 223a 2238 312e 3922 2c0a 2020 2020 2020  ":"81.9",.      
-00000b00: 2020 2020 2020 2020 2020 2264 665f 6f76            "df_ov
-00000b10: 6572 5f72 6d73 223a 3932 2e32 2c0a 2020  er_rms":92.2,.  
-00000b20: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00000b30: 665f 7261 7722 3a22 312e 3538 205c 7530  f_raw":"1.58 \u0
-00000b40: 3062 3120 302e 3032 222c 0a20 2020 2020  0b1 0.02",.     
-00000b50: 2020 2020 2020 2020 2020 2022 7a22 3a22             "z":"
-00000b60: 302e 3035 3132 222c 0a20 2020 2020 2020  0.0512",.       
-00000b70: 2020 2020 2020 2020 2022 6d62 6822 3a22           "mbh":"
-00000b80: 362e 3734 2028 4332 3129 222c 0a20 2020  6.74 (C21)",.   
-00000b90: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
-00000ba0: 676e 7464 6522 3a30 2e30 2c0a 2020 2020  gntde":0.0,.    
-00000bb0: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
-00000bc0: 7373 223a 2254 4445 222c 0a20 2020 2020  ss":"TDE",.     
-00000bd0: 2020 2020 2020 2020 2020 2022 6466 223a             "df":
-00000be0: 312e 3538 2c0a 2020 2020 2020 2020 2020  1.58,.          
-00000bf0: 2020 2020 2020 2264 665f 6522 3a30 2e30        "df_e":0.0
-00000c00: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-00000c10: 2020 2022 7261 223a 3331 342e 3236 3233     "ra":314.2623
-00000c20: 3932 362c 0a20 2020 2020 2020 2020 2020  926,.           
-00000c30: 2020 2020 2022 6465 6322 3a31 342e 3230       "dec":14.20
-00000c40: 3434 3036 330a 2020 2020 2020 2020 2020  44063.          
-00000c50: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00000c60: 2022 3122 3a7b 0a20 2020 2020 2020 2020   "1":{.         
-00000c70: 2020 2020 2020 2022 6e61 6d65 223a 2241         "name":"A
-00000c80: 5432 3031 3966 6472 222c 0a20 2020 2020  T2019fdr",.     
-00000c90: 2020 2020 2020 2020 2020 2022 7470 6561             "tpea
-00000ca0: 6b22 3a35 3836 3732 2e35 2c0a 2020 2020  k":58672.5,.    
-00000cb0: 2020 2020 2020 2020 2020 2020 2272 6973              "ris
-00000cc0: 6574 696d 6522 3a22 3330 2e38 222c 0a20  etime":"30.8",. 
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000ce0: 6661 6465 7469 6d65 223a 2233 3336 2e36  fadetime":"336.6
-00000cf0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000d00: 2020 2022 6466 5f6f 7665 725f 726d 7322     "df_over_rms"
-00000d10: 3a33 392e 322c 0a20 2020 2020 2020 2020  :39.2,.         
-00000d20: 2020 2020 2020 2022 6466 5f72 6177 223a         "df_raw":
-00000d30: 2230 2e37 3120 5c75 3030 6231 2030 2e30  "0.71 \u00b1 0.0
-00000d40: 3722 2c0a 2020 2020 2020 2020 2020 2020  7",.            
-00000d50: 2020 2020 227a 223a 2230 2e32 3636 3622      "z":"0.2666"
-00000d60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000d70: 2020 226d 6268 223a 2237 2e31 3020 2846    "mbh":"7.10 (F
-00000d80: 3230 2922 2c0a 2020 2020 2020 2020 2020  20)",.          
-00000d90: 2020 2020 2020 2270 6167 6e74 6465 223a        "pagntde":
-00000da0: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
-00000db0: 2020 2020 2022 636c 6173 7322 3a22 5444       "class":"TD
-00000dc0: 453f 222c 0a20 2020 2020 2020 2020 2020  E?",.           
-00000dd0: 2020 2020 2022 6466 223a 302e 3731 2c0a       "df":0.71,.
-00000de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000df0: 2264 665f 6522 3a30 2e30 372c 0a20 2020  "df_e":0.07,.   
-00000e00: 2020 2020 2020 2020 2020 2020 2022 7261               "ra
-00000e10: 223a 3235 372e 3237 3835 3738 3933 352c  ":257.278578935,
-00000e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e30: 2022 6465 6322 3a32 362e 3835 3536 3934   "dec":26.855694
-00000e40: 3636 3332 0a20 2020 2020 2020 2020 2020  6632.           
-00000e50: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00000e60: 2232 223a 7b0a 2020 2020 2020 2020 2020  "2":{.          
-00000e70: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
-00000e80: 3230 3139 6161 6c63 222c 0a20 2020 2020  2019aalc",.     
-00000e90: 2020 2020 2020 2020 2020 2022 7470 6561             "tpea
-00000ea0: 6b22 3a35 3836 3538 2e32 2c0a 2020 2020  k":58658.2,.    
-00000eb0: 2020 2020 2020 2020 2020 2020 2272 6973              "ris
-00000ec0: 6574 696d 6522 3a22 3439 2e30 222c 0a20  etime":"49.0",. 
-00000ed0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000ee0: 6661 6465 7469 6d65 223a 2231 3637 2e37  fadetime":"167.7
-00000ef0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000f00: 2020 2022 6466 5f6f 7665 725f 726d 7322     "df_over_rms"
-00000f10: 3a31 352e 372c 0a20 2020 2020 2020 2020  :15.7,.         
-00000f20: 2020 2020 2020 2022 6466 5f72 6177 223a         "df_raw":
-00000f30: 2231 312e 3133 205c 7530 3062 3120 302e  "11.13 \u00b1 0.
-00000f40: 3130 222c 0a20 2020 2020 2020 2020 2020  10",.           
-00000f50: 2020 2020 2022 7a22 3a22 302e 3033 3536       "z":"0.0356
-00000f60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000f70: 2020 2022 6d62 6822 3a22 372e 3233 2028     "mbh":"7.23 (
-00000f80: 4c31 3929 222c 0a20 2020 2020 2020 2020  L19)",.         
-00000f90: 2020 2020 2020 2022 7061 676e 7464 6522         "pagntde"
-00000fa0: 3a30 2e31 3834 2c0a 2020 2020 2020 2020  :0.184,.        
-00000fb0: 2020 2020 2020 2020 2263 6c61 7373 223a          "class":
-00000fc0: 2254 4445 3f22 2c0a 2020 2020 2020 2020  "TDE?",.        
-00000fd0: 2020 2020 2020 2020 2264 6622 3a31 312e          "df":11.
-00000fe0: 3133 2c0a 2020 2020 2020 2020 2020 2020  13,.            
-00000ff0: 2020 2020 2264 665f 6522 3a30 2e31 2c0a      "df_e":0.1,.
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 2272 6122 3a32 3331 2e30 3639 3433 352c  "ra":231.069435,
-00001020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001030: 2022 6465 6322 3a34 2e38 3535 3239 330a   "dec":4.855293.
-00001040: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00001050: 2020 2020 2020 2020 2020 2022 3322 3a7b             "3":{
-00001060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001070: 2022 6e61 6d65 223a 2241 5432 3031 3864   "name":"AT2018d
-00001080: 796b 222c 0a20 2020 2020 2020 2020 2020  yk",.           
-00001090: 2020 2020 2022 7470 6561 6b22 3a35 3832       "tpeak":582
-000010a0: 3631 2e34 2c0a 2020 2020 2020 2020 2020  61.4,.          
-000010b0: 2020 2020 2020 2272 6973 6574 696d 6522        "risetime"
-000010c0: 3a22 3630 2e30 222c 0a20 2020 2020 2020  :"60.0",.       
-000010d0: 2020 2020 2020 2020 2022 6661 6465 7469           "fadeti
-000010e0: 6d65 223a 2233 3432 2e30 222c 0a20 2020  me":"342.0",.   
-000010f0: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00001100: 5f6f 7665 725f 726d 7322 3a32 332e 382c  _over_rms":23.8,
-00001110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001120: 2022 6466 5f72 6177 223a 2231 2e34 3120   "df_raw":"1.41 
-00001130: 5c75 3030 6231 2030 2e30 3322 2c0a 2020  \u00b1 0.03",.  
-00001140: 2020 2020 2020 2020 2020 2020 2020 227a                "z
-00001150: 223a 2230 2e30 3336 3722 2c0a 2020 2020  ":"0.0367",.    
-00001160: 2020 2020 2020 2020 2020 2020 226d 6268              "mbh
-00001170: 223a 2235 2e35 3020 2846 3139 2922 2c0a  ":"5.50 (F19)",.
-00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001190: 2270 6167 6e74 6465 223a 302e 3030 352c  "pagntde":0.005,
-000011a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011b0: 2022 636c 6173 7322 3a22 5444 453f 222c   "class":"TDE?",
-000011c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011d0: 2022 6466 223a 312e 3431 2c0a 2020 2020   "df":1.41,.    
-000011e0: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-000011f0: 6522 3a30 2e30 332c 0a20 2020 2020 2020  e":0.03,.       
-00001200: 2020 2020 2020 2020 2022 7261 223a 3233           "ra":23
-00001210: 332e 3238 3333 3935 352c 0a20 2020 2020  3.2833955,.     
-00001220: 2020 2020 2020 2020 2020 2022 6465 6322             "dec"
-00001230: 3a34 342e 3533 3536 3132 320a 2020 2020  :44.5356122.    
-00001240: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00001250: 2020 2020 2020 2022 3422 3a7b 0a20 2020         "4":{.   
-00001260: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-00001270: 6d65 223a 2241 5432 3031 3961 616d 6522  me":"AT2019aame"
-00001280: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001290: 2020 2274 7065 616b 223a 3538 3336 332e    "tpeak":58363.
-000012a0: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-000012b0: 2020 2022 7269 7365 7469 6d65 223a 225c     "risetime":"\
-000012c0: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
-000012d0: 2020 2020 2020 2020 2266 6164 6574 696d          "fadetim
-000012e0: 6522 3a22 3133 382e 3022 2c0a 2020 2020  e":"138.0",.    
-000012f0: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-00001300: 6f76 6572 5f72 6d73 223a 3132 2e33 2c0a  over_rms":12.3,.
-00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001320: 2264 665f 7261 7722 3a22 302e 3138 205c  "df_raw":"0.18 \
-00001330: 7530 3062 3120 302e 3031 222c 0a20 2020  u00b1 0.01",.   
-00001340: 2020 2020 2020 2020 2020 2020 2022 7a22               "z"
-00001350: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-00001360: 2020 2020 2020 2020 2020 2022 6d62 6822             "mbh"
-00001370: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-00001380: 2020 2020 2020 2020 2020 2022 7061 676e             "pagn
-00001390: 7464 6522 3a30 2e35 3537 2c0a 2020 2020  tde":0.557,.    
-000013a0: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
-000013b0: 7373 223a 225c 7532 3031 3322 2c0a 2020  ss":"\u2013",.  
-000013c0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-000013d0: 6622 3a30 2e31 382c 0a20 2020 2020 2020  f":0.18,.       
-000013e0: 2020 2020 2020 2020 2022 6466 5f65 223a           "df_e":
-000013f0: 302e 3031 2c0a 2020 2020 2020 2020 2020  0.01,.          
-00001400: 2020 2020 2020 2272 6122 3a32 3135 2e30        "ra":215.0
-00001410: 3531 3831 3835 3238 362c 0a20 2020 2020  518185286,.     
-00001420: 2020 2020 2020 2020 2020 2022 6465 6322             "dec"
-00001430: 3a33 312e 3839 3431 3832 3635 0a20 2020  :31.89418265.   
-00001440: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00001450: 2020 2020 2020 2020 2235 223a 7b0a 2020          "5":{.  
-00001460: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00001470: 616d 6522 3a22 4154 3230 3138 6c7a 7322  ame":"AT2018lzs"
-00001480: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001490: 2020 2274 7065 616b 223a 3538 3337 382e    "tpeak":58378.
-000014a0: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-000014b0: 2020 2022 7269 7365 7469 6d65 223a 2231     "risetime":"1
-000014c0: 3334 2e30 222c 0a20 2020 2020 2020 2020  34.0",.         
-000014d0: 2020 2020 2020 2022 6661 6465 7469 6d65         "fadetime
-000014e0: 223a 2231 352e 3522 2c0a 2020 2020 2020  ":"15.5",.      
-000014f0: 2020 2020 2020 2020 2020 2264 665f 6f76            "df_ov
-00001500: 6572 5f72 6d73 223a 332e 332c 0a20 2020  er_rms":3.3,.   
-00001510: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00001520: 5f72 6177 223a 2230 2e30 3320 5c75 3030  _raw":"0.03 \u00
-00001530: 6231 2030 2e30 3122 2c0a 2020 2020 2020  b1 0.01",.      
-00001540: 2020 2020 2020 2020 2020 227a 223a 225c            "z":"\
-00001550: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
-00001560: 2020 2020 2020 2020 226d 6268 223a 225c          "mbh":"\
-00001570: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
-00001580: 2020 2020 2020 2020 2270 6167 6e74 6465          "pagntde
-00001590: 223a 342e 3134 342c 0a20 2020 2020 2020  ":4.144,.       
-000015a0: 2020 2020 2020 2020 2022 636c 6173 7322           "class"
-000015b0: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-000015c0: 2020 2020 2020 2020 2020 2022 6466 223a             "df":
-000015d0: 302e 3033 2c0a 2020 2020 2020 2020 2020  0.03,.          
-000015e0: 2020 2020 2020 2264 665f 6522 3a30 2e30        "df_e":0.0
-000015f0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00001600: 2020 2022 7261 223a 3236 382e 3233 3332     "ra":268.2332
-00001610: 3238 3538 3839 2c0a 2020 2020 2020 2020  285889,.        
-00001620: 2020 2020 2020 2020 2264 6563 223a 3538          "dec":58
-00001630: 2e36 3336 3434 3238 3531 310a 2020 2020  .6364428511.    
-00001640: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00001650: 2020 2020 2020 2022 3622 3a7b 0a20 2020         "6":{.   
-00001660: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-00001670: 6d65 223a 2241 5432 3032 3161 6574 7a22  me":"AT2021aetz"
-00001680: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001690: 2020 2274 7065 616b 223a 3538 3339 302e    "tpeak":58390.
-000016a0: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
-000016b0: 2020 2022 7269 7365 7469 6d65 223a 2238     "risetime":"8
-000016c0: 2e36 222c 0a20 2020 2020 2020 2020 2020  .6",.           
-000016d0: 2020 2020 2022 6661 6465 7469 6d65 223a       "fadetime":
-000016e0: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
-000016f0: 2020 2020 2020 2020 2020 2264 665f 6f76            "df_ov
-00001700: 6572 5f72 6d73 223a 3437 2e35 2c0a 2020  er_rms":47.5,.  
-00001710: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00001720: 665f 7261 7722 3a22 302e 3831 205c 7530  f_raw":"0.81 \u0
-00001730: 3062 3120 302e 3031 222c 0a20 2020 2020  0b1 0.01",.     
-00001740: 2020 2020 2020 2020 2020 2022 7a22 3a22             "z":"
-00001750: 302e 3038 3739 222c 0a20 2020 2020 2020  0.0879",.       
-00001760: 2020 2020 2020 2020 2022 6d62 6822 3a22           "mbh":"
-00001770: 362e 3231 2028 5431 3329 222c 0a20 2020  6.21 (T13)",.   
-00001780: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
-00001790: 676e 7464 6522 3a30 2e30 2c0a 2020 2020  gntde":0.0,.    
-000017a0: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
-000017b0: 7373 223a 2254 4445 3f22 2c0a 2020 2020  ss":"TDE?",.    
-000017c0: 2020 2020 2020 2020 2020 2020 2264 6622              "df"
-000017d0: 3a30 2e38 312c 0a20 2020 2020 2020 2020  :0.81,.         
-000017e0: 2020 2020 2020 2022 6466 5f65 223a 302e         "df_e":0.
-000017f0: 3031 2c0a 2020 2020 2020 2020 2020 2020  01,.            
-00001800: 2020 2020 2272 6122 3a33 3237 2e37 3332      "ra":327.732
-00001810: 3234 3036 3433 332c 0a20 2020 2020 2020  2406433,.       
-00001820: 2020 2020 2020 2020 2022 6465 6322 3a2d           "dec":-
-00001830: 312e 3131 3530 3632 3937 3333 0a20 2020  1.1150629733.   
-00001840: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00001850: 2020 2020 2020 2020 2237 223a 7b0a 2020          "7":{.  
-00001860: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00001870: 616d 6522 3a22 4154 3230 3138 6967 6522  ame":"AT2018ige"
-00001880: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001890: 2020 2274 7065 616b 223a 3538 3433 322e    "tpeak":58432.
-000018a0: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-000018b0: 2020 2022 7269 7365 7469 6d65 223a 225c     "risetime":"\
-000018c0: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
-000018d0: 2020 2020 2020 2020 2266 6164 6574 696d          "fadetim
-000018e0: 6522 3a22 3637 2e39 222c 0a20 2020 2020  e":"67.9",.     
-000018f0: 2020 2020 2020 2020 2020 2022 6466 5f6f             "df_o
-00001900: 7665 725f 726d 7322 3a36 352e 382c 0a20  ver_rms":65.8,. 
-00001910: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001920: 6466 5f72 6177 223a 2230 2e33 3120 5c75  df_raw":"0.31 \u
-00001930: 3030 6231 2030 2e30 3122 2c0a 2020 2020  00b1 0.01",.    
-00001940: 2020 2020 2020 2020 2020 2020 227a 223a              "z":
-00001950: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
-00001960: 2020 2020 2020 2020 2020 226d 6268 223a            "mbh":
-00001970: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
-00001980: 2020 2020 2020 2020 2020 2270 6167 6e74            "pagnt
-00001990: 6465 223a 302e 302c 0a20 2020 2020 2020  de":0.0,.       
-000019a0: 2020 2020 2020 2020 2022 636c 6173 7322           "class"
-000019b0: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-000019c0: 2020 2020 2020 2020 2020 2022 6466 223a             "df":
-000019d0: 302e 3331 2c0a 2020 2020 2020 2020 2020  0.31,.          
-000019e0: 2020 2020 2020 2264 665f 6522 3a30 2e30        "df_e":0.0
-000019f0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00001a00: 2020 2022 7261 223a 3131 382e 3633 3830     "ra":118.6380
-00001a10: 3530 372c 0a20 2020 2020 2020 2020 2020  507,.           
-00001a20: 2020 2020 2022 6465 6322 3a39 2e34 3934       "dec":9.494
-00001a30: 3132 3539 0a20 2020 2020 2020 2020 2020  1259.           
-00001a40: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00001a50: 2238 223a 7b0a 2020 2020 2020 2020 2020  "8":{.          
-00001a60: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
-00001a70: 3230 3231 6165 7564 222c 0a20 2020 2020  2021aeud",.     
-00001a80: 2020 2020 2020 2020 2020 2022 7470 6561             "tpea
-00001a90: 6b22 3a35 3834 3438 2e33 2c0a 2020 2020  k":58448.3,.    
-00001aa0: 2020 2020 2020 2020 2020 2020 2272 6973              "ris
-00001ab0: 6574 696d 6522 3a22 3133 372e 3622 2c0a  etime":"137.6",.
-00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ad0: 2266 6164 6574 696d 6522 3a22 3238 322e  "fadetime":"282.
-00001ae0: 3722 2c0a 2020 2020 2020 2020 2020 2020  7",.            
-00001af0: 2020 2020 2264 665f 6f76 6572 5f72 6d73      "df_over_rms
-00001b00: 223a 362e 322c 0a20 2020 2020 2020 2020  ":6.2,.         
-00001b10: 2020 2020 2020 2022 6466 5f72 6177 223a         "df_raw":
-00001b20: 2230 2e31 3520 5c75 3030 6231 2030 2e30  "0.15 \u00b1 0.0
-00001b30: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-00001b40: 2020 2020 227a 223a 225c 7532 3031 3322      "z":"\u2013"
-00001b50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001b60: 2020 226d 6268 223a 225c 7532 3031 3322    "mbh":"\u2013"
-00001b70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001b80: 2020 2270 6167 6e74 6465 223a 342e 3238    "pagntde":4.28
-00001b90: 382c 0a20 2020 2020 2020 2020 2020 2020  8,.             
-00001ba0: 2020 2022 636c 6173 7322 3a22 5c75 3230     "class":"\u20
-00001bb0: 3133 222c 0a20 2020 2020 2020 2020 2020  13",.           
-00001bc0: 2020 2020 2022 6466 223a 302e 3135 2c0a       "df":0.15,.
-00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001be0: 2264 665f 6522 3a30 2e30 312c 0a20 2020  "df_e":0.01,.   
-00001bf0: 2020 2020 2020 2020 2020 2020 2022 7261               "ra
-00001c00: 223a 3130 352e 3233 3337 3930 3530 3737  ":105.2337905077
-00001c10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001c20: 2020 2264 6563 223a 3336 2e39 3830 3935    "dec":36.98095
-00001c30: 3534 3734 320a 2020 2020 2020 2020 2020  54742.          
-00001c40: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00001c50: 2022 3922 3a7b 0a20 2020 2020 2020 2020   "9":{.         
-00001c60: 2020 2020 2020 2022 6e61 6d65 223a 2241         "name":"A
-00001c70: 5432 3031 3869 716c 222c 0a20 2020 2020  T2018iql",.     
-00001c80: 2020 2020 2020 2020 2020 2022 7470 6561             "tpea
-00001c90: 6b22 3a35 3834 3439 2e34 2c0a 2020 2020  k":58449.4,.    
-00001ca0: 2020 2020 2020 2020 2020 2020 2272 6973              "ris
-00001cb0: 6574 696d 6522 3a22 3137 2e39 222c 0a20  etime":"17.9",. 
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001cd0: 6661 6465 7469 6d65 223a 2234 312e 3022  fadetime":"41.0"
-00001ce0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001cf0: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
-00001d00: 3330 2e31 2c0a 2020 2020 2020 2020 2020  30.1,.          
-00001d10: 2020 2020 2020 2264 665f 7261 7722 3a22        "df_raw":"
-00001d20: 302e 3438 205c 7530 3062 3120 302e 3031  0.48 \u00b1 0.01
-00001d30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001d40: 2020 2022 7a22 3a22 5c75 3230 3133 222c     "z":"\u2013",
-00001d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001d60: 2022 6d62 6822 3a22 5c75 3230 3133 222c   "mbh":"\u2013",
-00001d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001d80: 2022 7061 676e 7464 6522 3a30 2e30 2c0a   "pagntde":0.0,.
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001da0: 2263 6c61 7373 223a 225c 7532 3031 3322  "class":"\u2013"
-00001db0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001dc0: 2020 2264 6622 3a30 2e34 382c 0a20 2020    "df":0.48,.   
-00001dd0: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00001de0: 5f65 223a 302e 3031 2c0a 2020 2020 2020  _e":0.01,.      
-00001df0: 2020 2020 2020 2020 2020 2272 6122 3a37            "ra":7
-00001e00: 342e 3537 3936 3637 2c0a 2020 2020 2020  4.579667,.      
-00001e10: 2020 2020 2020 2020 2020 2264 6563 223a            "dec":
-00001e20: 2d37 2e37 3637 3936 310a 2020 2020 2020  -7.767961.      
-00001e30: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00001e40: 2020 2020 2022 3130 223a 7b0a 2020 2020       "10":{.    
-00001e50: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
-00001e60: 6522 3a22 4154 3230 3138 6a75 7422 2c0a  e":"AT2018jut",.
-00001e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e80: 2274 7065 616b 223a 3538 3434 392e 362c  "tpeak":58449.6,
-00001e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ea0: 2022 7269 7365 7469 6d65 223a 225c 7532   "risetime":"\u2
-00001eb0: 3031 3322 2c0a 2020 2020 2020 2020 2020  013",.          
-00001ec0: 2020 2020 2020 2266 6164 6574 696d 6522        "fadetime"
-00001ed0: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-00001ee0: 2020 2020 2020 2020 2020 2022 6466 5f6f             "df_o
-00001ef0: 7665 725f 726d 7322 3a35 2e30 2c0a 2020  ver_rms":5.0,.  
-00001f00: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00001f10: 665f 7261 7722 3a22 302e 3132 205c 7530  f_raw":"0.12 \u0
-00001f20: 3062 3120 302e 3031 222c 0a20 2020 2020  0b1 0.01",.     
-00001f30: 2020 2020 2020 2020 2020 2022 7a22 3a22             "z":"
-00001f40: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
-00001f50: 2020 2020 2020 2020 2022 6d62 6822 3a22           "mbh":"
-00001f60: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
-00001f70: 2020 2020 2020 2020 2022 7061 676e 7464           "pagntd
-00001f80: 6522 3a35 2e37 3832 2c0a 2020 2020 2020  e":5.782,.      
-00001f90: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
-00001fa0: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
-00001fb0: 2020 2020 2020 2020 2020 2020 2264 6622              "df"
-00001fc0: 3a30 2e31 322c 0a20 2020 2020 2020 2020  :0.12,.         
-00001fd0: 2020 2020 2020 2022 6466 5f65 223a 302e         "df_e":0.
-00001fe0: 3031 2c0a 2020 2020 2020 2020 2020 2020  01,.            
-00001ff0: 2020 2020 2272 6122 3a32 3038 2e35 3334      "ra":208.534
-00002000: 3632 352c 0a20 2020 2020 2020 2020 2020  625,.           
-00002010: 2020 2020 2022 6465 6322 3a31 332e 3033       "dec":13.03
-00002020: 3232 350a 2020 2020 2020 2020 2020 2020  225.            
-00002030: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-00002040: 3131 223a 7b0a 2020 2020 2020 2020 2020  11":{.          
-00002050: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
-00002060: 3230 3231 6165 7565 222c 0a20 2020 2020  2021aeue",.     
-00002070: 2020 2020 2020 2020 2020 2022 7470 6561             "tpea
-00002080: 6b22 3a35 3834 3735 2e31 2c0a 2020 2020  k":58475.1,.    
-00002090: 2020 2020 2020 2020 2020 2020 2272 6973              "ris
-000020a0: 6574 696d 6522 3a22 3438 2e35 222c 0a20  etime":"48.5",. 
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000020c0: 6661 6465 7469 6d65 223a 2234 382e 3822  fadetime":"48.8"
-000020d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000020e0: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
-000020f0: 342e 392c 0a20 2020 2020 2020 2020 2020  4.9,.           
-00002100: 2020 2020 2022 6466 5f72 6177 223a 2230       "df_raw":"0
-00002110: 2e31 3120 5c75 3030 6231 2030 2e30 3122  .11 \u00b1 0.01"
-00002120: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002130: 2020 227a 223a 225c 7532 3031 3322 2c0a    "z":"\u2013",.
-00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002150: 226d 6268 223a 225c 7532 3031 3322 2c0a  "mbh":"\u2013",.
-00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002170: 2270 6167 6e74 6465 223a 352e 3838 312c  "pagntde":5.881,
-00002180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002190: 2022 636c 6173 7322 3a22 5c75 3230 3133   "class":"\u2013
-000021a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000021b0: 2020 2022 6466 223a 302e 3131 2c0a 2020     "df":0.11,.  
-000021c0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-000021d0: 665f 6522 3a30 2e30 312c 0a20 2020 2020  f_e":0.01,.     
-000021e0: 2020 2020 2020 2020 2020 2022 7261 223a             "ra":
-000021f0: 3335 2e37 3933 3230 3632 3132 392c 0a20  35.7932062129,. 
-00002200: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002210: 6465 6322 3a2d 392e 3534 3030 3935 3438  dec":-9.54009548
-00002220: 3739 0a20 2020 2020 2020 2020 2020 207d  79.            }
-00002230: 2c0a 2020 2020 2020 2020 2020 2020 2231  ,.            "1
-00002240: 3222 3a7b 0a20 2020 2020 2020 2020 2020  2":{.           
-00002250: 2020 2020 2022 6e61 6d65 223a 2241 5432       "name":"AT2
-00002260: 3031 3961 616d 6622 2c0a 2020 2020 2020  019aamf",.      
-00002270: 2020 2020 2020 2020 2020 2274 7065 616b            "tpeak
-00002280: 223a 3538 3530 362e 342c 0a20 2020 2020  ":58506.4,.     
-00002290: 2020 2020 2020 2020 2020 2022 7269 7365             "rise
-000022a0: 7469 6d65 223a 2238 302e 3022 2c0a 2020  time":"80.0",.  
-000022b0: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-000022c0: 6164 6574 696d 6522 3a22 3134 312e 3222  adetime":"141.2"
-000022d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000022e0: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
-000022f0: 362e 362c 0a20 2020 2020 2020 2020 2020  6.6,.           
-00002300: 2020 2020 2022 6466 5f72 6177 223a 2230       "df_raw":"0
-00002310: 2e31 3920 5c75 3030 6231 2030 2e30 3122  .19 \u00b1 0.01"
-00002320: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002330: 2020 227a 223a 225c 7532 3031 3322 2c0a    "z":"\u2013",.
-00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002350: 226d 6268 223a 225c 7532 3031 3322 2c0a  "mbh":"\u2013",.
-00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002370: 2270 6167 6e74 6465 223a 332e 3734 342c  "pagntde":3.744,
-00002380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002390: 2022 636c 6173 7322 3a22 5c75 3230 3133   "class":"\u2013
-000023a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000023b0: 2020 2022 6466 223a 302e 3139 2c0a 2020     "df":0.19,.  
-000023c0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-000023d0: 665f 6522 3a30 2e30 312c 0a20 2020 2020  f_e":0.01,.     
-000023e0: 2020 2020 2020 2020 2020 2022 7261 223a             "ra":
-000023f0: 3133 342e 3235 3631 3439 3137 3833 2c0a  134.2561491783,.
-00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002410: 2264 6563 223a 3333 2e39 3134 3938 3837  "dec":33.9149887
-00002420: 3034 380a 2020 2020 2020 2020 2020 2020  048.            
-00002430: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-00002440: 3133 223a 7b0a 2020 2020 2020 2020 2020  13":{.          
-00002450: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
-00002460: 3230 3138 6b6f 7822 2c0a 2020 2020 2020  2018kox",.      
-00002470: 2020 2020 2020 2020 2020 2274 7065 616b            "tpeak
-00002480: 223a 3538 3531 302e 322c 0a20 2020 2020  ":58510.2,.     
-00002490: 2020 2020 2020 2020 2020 2022 7269 7365             "rise
-000024a0: 7469 6d65 223a 2232 362e 3922 2c0a 2020  time":"26.9",.  
-000024b0: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-000024c0: 6164 6574 696d 6522 3a22 3136 372e 3622  adetime":"167.6"
-000024d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000024e0: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
-000024f0: 352e 362c 0a20 2020 2020 2020 2020 2020  5.6,.           
-00002500: 2020 2020 2022 6466 5f72 6177 223a 2230       "df_raw":"0
-00002510: 2e33 3320 5c75 3030 6231 2030 2e30 3122  .33 \u00b1 0.01"
-00002520: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002530: 2020 227a 223a 2230 2e30 3936 222c 0a20    "z":"0.096",. 
-00002540: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002550: 6d62 6822 3a22 5c75 3230 3133 222c 0a20  mbh":"\u2013",. 
-00002560: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002570: 7061 676e 7464 6522 3a35 2e30 3436 2c0a  pagntde":5.046,.
-00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002590: 2263 6c61 7373 223a 225c 7532 3031 3322  "class":"\u2013"
-000025a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000025b0: 2020 2264 6622 3a30 2e33 332c 0a20 2020    "df":0.33,.   
-000025c0: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-000025d0: 5f65 223a 302e 3031 2c0a 2020 2020 2020  _e":0.01,.      
-000025e0: 2020 2020 2020 2020 2020 2272 6122 3a37            "ra":7
-000025f0: 302e 3739 3333 3735 2c0a 2020 2020 2020  0.793375,.      
-00002600: 2020 2020 2020 2020 2020 2264 6563 223a            "dec":
-00002610: 2d34 2e33 3033 3038 310a 2020 2020 2020  -4.303081.      
-00002620: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00002630: 2020 2020 2022 3134 223a 7b0a 2020 2020       "14":{.    
-00002640: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
-00002650: 6522 3a22 4154 3230 3138 6c68 7622 2c0a  e":"AT2018lhv",.
-00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002670: 2274 7065 616b 223a 3538 3531 332e 352c  "tpeak":58513.5,
-00002680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002690: 2022 7269 7365 7469 6d65 223a 2231 372e   "risetime":"17.
-000026a0: 3522 2c0a 2020 2020 2020 2020 2020 2020  5",.            
-000026b0: 2020 2020 2266 6164 6574 696d 6522 3a22      "fadetime":"
-000026c0: 3131 362e 3122 2c0a 2020 2020 2020 2020  116.1",.        
-000026d0: 2020 2020 2020 2020 2264 665f 6f76 6572          "df_over
-000026e0: 5f72 6d73 223a 3332 2e33 2c0a 2020 2020  _rms":32.3,.    
-000026f0: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-00002700: 7261 7722 3a22 302e 3335 205c 7530 3062  raw":"0.35 \u00b
-00002710: 3120 302e 3031 222c 0a20 2020 2020 2020  1 0.01",.       
-00002720: 2020 2020 2020 2020 2022 7a22 3a22 5c75           "z":"\u
-00002730: 3230 3133 222c 0a20 2020 2020 2020 2020  2013",.         
-00002740: 2020 2020 2020 2022 6d62 6822 3a22 5c75         "mbh":"\u
-00002750: 3230 3133 222c 0a20 2020 2020 2020 2020  2013",.         
-00002760: 2020 2020 2020 2022 7061 676e 7464 6522         "pagntde"
-00002770: 3a30 2e30 2c0a 2020 2020 2020 2020 2020  :0.0,.          
-00002780: 2020 2020 2020 2263 6c61 7373 223a 225c        "class":"\
-00002790: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
-000027a0: 2020 2020 2020 2020 2264 6622 3a30 2e33          "df":0.3
-000027b0: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-000027c0: 2020 2022 6466 5f65 223a 302e 3031 2c0a     "df_e":0.01,.
-000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027e0: 2272 6122 3a31 3936 2e33 3533 3830 3031  "ra":196.3538001
-000027f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002800: 2020 2264 6563 223a 3231 2e39 3534 3436    "dec":21.95446
-00002810: 3237 0a20 2020 2020 2020 2020 2020 207d  27.            }
-00002820: 2c0a 2020 2020 2020 2020 2020 2020 2231  ,.            "1
-00002830: 3522 3a7b 0a20 2020 2020 2020 2020 2020  5":{.           
-00002840: 2020 2020 2022 6e61 6d65 223a 2241 5432       "name":"AT2
-00002850: 3031 3961 7664 222c 0a20 2020 2020 2020  019avd",.       
-00002860: 2020 2020 2020 2020 2022 7470 6561 6b22           "tpeak"
-00002870: 3a35 3835 3334 2e33 2c0a 2020 2020 2020  :58534.3,.      
-00002880: 2020 2020 2020 2020 2020 2272 6973 6574            "riset
-00002890: 696d 6522 3a22 3134 2e39 222c 0a20 2020  ime":"14.9",.   
-000028a0: 2020 2020 2020 2020 2020 2020 2022 6661               "fa
-000028b0: 6465 7469 6d65 223a 2235 322e 3922 2c0a  detime":"52.9",.
-000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028d0: 2264 665f 6f76 6572 5f72 6d73 223a 3637  "df_over_rms":67
-000028e0: 2e35 2c0a 2020 2020 2020 2020 2020 2020  .5,.            
-000028f0: 2020 2020 2264 665f 7261 7722 3a22 312e      "df_raw":"1.
-00002900: 3837 205c 7530 3062 3120 302e 3035 222c  87 \u00b1 0.05",
-00002910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002920: 2022 7a22 3a22 302e 3032 3936 222c 0a20   "z":"0.0296",. 
-00002930: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002940: 6d62 6822 3a22 362e 3130 2028 4632 3029  mbh":"6.10 (F20)
-00002950: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002960: 2020 2022 7061 676e 7464 6522 3a30 2e30     "pagntde":0.0
-00002970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002980: 2020 2263 6c61 7373 223a 2254 4445 3f22    "class":"TDE?"
-00002990: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000029a0: 2020 2264 6622 3a31 2e38 372c 0a20 2020    "df":1.87,.   
-000029b0: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-000029c0: 5f65 223a 302e 3035 2c0a 2020 2020 2020  _e":0.05,.      
-000029d0: 2020 2020 2020 2020 2020 2272 6122 3a31            "ra":1
-000029e0: 3235 2e39 3033 3139 3735 2c0a 2020 2020  25.9031975,.    
-000029f0: 2020 2020 2020 2020 2020 2020 2264 6563              "dec
-00002a00: 223a 342e 3338 3430 3136 360a 2020 2020  ":4.3840166.    
-00002a10: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00002a20: 2020 2020 2020 2022 3136 223a 7b0a 2020         "16":{.  
-00002a30: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00002a40: 616d 6522 3a22 4154 3230 3136 6569 7822  ame":"AT2016eix"
-00002a50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002a60: 2020 2274 7065 616b 223a 3538 3533 392e    "tpeak":58539.
-00002a70: 342c 0a20 2020 2020 2020 2020 2020 2020  4,.             
-00002a80: 2020 2022 7269 7365 7469 6d65 223a 2231     "risetime":"1
-00002a90: 3034 2e32 222c 0a20 2020 2020 2020 2020  04.2",.         
-00002aa0: 2020 2020 2020 2022 6661 6465 7469 6d65         "fadetime
-00002ab0: 223a 2234 332e 3122 2c0a 2020 2020 2020  ":"43.1",.      
-00002ac0: 2020 2020 2020 2020 2020 2264 665f 6f76            "df_ov
-00002ad0: 6572 5f72 6d73 223a 362e 392c 0a20 2020  er_rms":6.9,.   
-00002ae0: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00002af0: 5f72 6177 223a 2230 2e31 3620 5c75 3030  _raw":"0.16 \u00
-00002b00: 6231 2030 2e30 3122 2c0a 2020 2020 2020  b1 0.01",.      
-00002b10: 2020 2020 2020 2020 2020 227a 223a 225c            "z":"\
-00002b20: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
-00002b30: 2020 2020 2020 2020 226d 6268 223a 225c          "mbh":"\
-00002b40: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
-00002b50: 2020 2020 2020 2020 2270 6167 6e74 6465          "pagntde
-00002b60: 223a 332e 3237 372c 0a20 2020 2020 2020  ":3.277,.       
-00002b70: 2020 2020 2020 2020 2022 636c 6173 7322           "class"
-00002b80: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-00002b90: 2020 2020 2020 2020 2020 2022 6466 223a             "df":
-00002ba0: 302e 3136 2c0a 2020 2020 2020 2020 2020  0.16,.          
-00002bb0: 2020 2020 2020 2264 665f 6522 3a30 2e30        "df_e":0.0
-00002bc0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00002bd0: 2020 2022 7261 223a 3234 342e 3731 3634     "ra":244.7164
-00002be0: 3338 3939 3137 2c0a 2020 2020 2020 2020  389917,.        
-00002bf0: 2020 2020 2020 2020 2264 6563 223a 3633          "dec":63
-00002c00: 2e31 3733 3337 3339 3735 0a20 2020 2020  .173373975.     
-00002c10: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00002c20: 2020 2020 2020 2231 3722 3a7b 0a20 2020        "17":{.   
-00002c30: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-00002c40: 6d65 223a 2241 5432 3031 3961 616d 6722  me":"AT2019aamg"
-00002c50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002c60: 2020 2274 7065 616b 223a 3538 3534 302e    "tpeak":58540.
-00002c70: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-00002c80: 2020 2022 7269 7365 7469 6d65 223a 225c     "risetime":"\
-00002c90: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
-00002ca0: 2020 2020 2020 2020 2266 6164 6574 696d          "fadetim
-00002cb0: 6522 3a22 3933 2e37 222c 0a20 2020 2020  e":"93.7",.     
-00002cc0: 2020 2020 2020 2020 2020 2022 6466 5f6f             "df_o
-00002cd0: 7665 725f 726d 7322 3a38 2e33 2c0a 2020  ver_rms":8.3,.  
-00002ce0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00002cf0: 665f 7261 7722 3a22 302e 3134 205c 7530  f_raw":"0.14 \u0
-00002d00: 3062 3120 302e 3030 222c 0a20 2020 2020  0b1 0.00",.     
-00002d10: 2020 2020 2020 2020 2020 2022 7a22 3a22             "z":"
-00002d20: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
-00002d30: 2020 2020 2020 2020 2022 6d62 6822 3a22           "mbh":"
-00002d40: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
-00002d50: 2020 2020 2020 2020 2022 7061 676e 7464           "pagntd
-00002d60: 6522 3a31 2e39 3435 2c0a 2020 2020 2020  e":1.945,.      
-00002d70: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
-00002d80: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
-00002d90: 2020 2020 2020 2020 2020 2020 2264 6622              "df"
-00002da0: 3a30 2e31 342c 0a20 2020 2020 2020 2020  :0.14,.         
-00002db0: 2020 2020 2020 2022 6466 5f65 223a 302e         "df_e":0.
-00002dc0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00002dd0: 2020 2022 7261 223a 3237 322e 3035 3430     "ra":272.0540
-00002de0: 3032 3731 3435 2c0a 2020 2020 2020 2020  027145,.        
-00002df0: 2020 2020 2020 2020 2264 6563 223a 3530          "dec":50
-00002e00: 2e37 3836 3733 3237 3631 380a 2020 2020  .7867327618.    
-00002e10: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00002e20: 2020 2020 2020 2022 3138 223a 7b0a 2020         "18":{.  
-00002e30: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00002e40: 616d 6522 3a22 4154 3230 3138 6c63 7022  ame":"AT2018lcp"
-00002e50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002e60: 2020 2274 7065 616b 223a 3538 3534 372e    "tpeak":58547.
-00002e70: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-00002e80: 2020 2022 7269 7365 7469 6d65 223a 2239     "risetime":"9
-00002e90: 352e 3722 2c0a 2020 2020 2020 2020 2020  5.7",.          
-00002ea0: 2020 2020 2020 2266 6164 6574 696d 6522        "fadetime"
-00002eb0: 3a22 3239 372e 3422 2c0a 2020 2020 2020  :"297.4",.      
-00002ec0: 2020 2020 2020 2020 2020 2264 665f 6f76            "df_ov
-00002ed0: 6572 5f72 6d73 223a 3132 2e37 2c0a 2020  er_rms":12.7,.  
-00002ee0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00002ef0: 665f 7261 7722 3a22 302e 3136 205c 7530  f_raw":"0.16 \u0
-00002f00: 3062 3120 302e 3031 222c 0a20 2020 2020  0b1 0.01",.     
-00002f10: 2020 2020 2020 2020 2020 2022 7a22 3a22             "z":"
-00002f20: 302e 3036 222c 0a20 2020 2020 2020 2020  0.06",.         
-00002f30: 2020 2020 2020 2022 6d62 6822 3a22 5c75         "mbh":"\u
-00002f40: 3230 3133 222c 0a20 2020 2020 2020 2020  2013",.         
-00002f50: 2020 2020 2020 2022 7061 676e 7464 6522         "pagntde"
-00002f60: 3a30 2e34 3935 2c0a 2020 2020 2020 2020  :0.495,.        
-00002f70: 2020 2020 2020 2020 2263 6c61 7373 223a          "class":
-00002f80: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
-00002f90: 2020 2020 2020 2020 2020 2264 6622 3a30            "df":0
-00002fa0: 2e31 362c 0a20 2020 2020 2020 2020 2020  .16,.           
-00002fb0: 2020 2020 2022 6466 5f65 223a 302e 3031       "df_e":0.01
-00002fc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002fd0: 2020 2272 6122 3a31 3137 2e37 3038 3431    "ra":117.70841
-00002fe0: 3632 2c0a 2020 2020 2020 2020 2020 2020  62,.            
-00002ff0: 2020 2020 2264 6563 223a 312e 3335 3833      "dec":1.3583
-00003000: 3530 310a 2020 2020 2020 2020 2020 2020  501.            
-00003010: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-00003020: 3139 223a 7b0a 2020 2020 2020 2020 2020  19":{.          
-00003030: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
-00003040: 3230 3231 6165 7566 222c 0a20 2020 2020  2021aeuf",.     
-00003050: 2020 2020 2020 2020 2020 2022 7470 6561             "tpea
-00003060: 6b22 3a35 3835 3536 2e34 2c0a 2020 2020  k":58556.4,.    
-00003070: 2020 2020 2020 2020 2020 2020 2272 6973              "ris
-00003080: 6574 696d 6522 3a22 3137 2e30 222c 0a20  etime":"17.0",. 
-00003090: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000030a0: 6661 6465 7469 6d65 223a 2231 3337 2e35  fadetime":"137.5
-000030b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000030c0: 2020 2022 6466 5f6f 7665 725f 726d 7322     "df_over_rms"
-000030d0: 3a31 352e 362c 0a20 2020 2020 2020 2020  :15.6,.         
-000030e0: 2020 2020 2020 2022 6466 5f72 6177 223a         "df_raw":
-000030f0: 2230 2e31 3820 5c75 3030 6231 2030 2e30  "0.18 \u00b1 0.0
-00003100: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-00003110: 2020 2020 227a 223a 225c 7532 3031 3322      "z":"\u2013"
-00003120: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003130: 2020 226d 6268 223a 225c 7532 3031 3322    "mbh":"\u2013"
-00003140: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003150: 2020 2270 6167 6e74 6465 223a 302e 3139    "pagntde":0.19
-00003160: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-00003170: 2020 2022 636c 6173 7322 3a22 5c75 3230     "class":"\u20
-00003180: 3133 222c 0a20 2020 2020 2020 2020 2020  13",.           
-00003190: 2020 2020 2022 6466 223a 302e 3138 2c0a       "df":0.18,.
-000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031b0: 2264 665f 6522 3a30 2e30 312c 0a20 2020  "df_e":0.01,.   
-000031c0: 2020 2020 2020 2020 2020 2020 2022 7261               "ra
-000031d0: 223a 3139 312e 3032 3834 3531 3335 3531  ":191.0284513551
-000031e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000031f0: 2020 2264 6563 223a 3437 2e34 3435 3133    "dec":47.44513
-00003200: 3530 3533 360a 2020 2020 2020 2020 2020  50536.          
-00003210: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00003220: 2022 3230 223a 7b0a 2020 2020 2020 2020   "20":{.        
-00003230: 2020 2020 2020 2020 226e 616d 6522 3a22          "name":"
-00003240: 4154 3230 3230 6165 7a79 222c 0a20 2020  AT2020aezy",.   
-00003250: 2020 2020 2020 2020 2020 2020 2022 7470               "tp
-00003260: 6561 6b22 3a35 3835 3538 2e34 2c0a 2020  eak":58558.4,.  
-00003270: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00003280: 6973 6574 696d 6522 3a22 3832 2e35 222c  isetime":"82.5",
-00003290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000032a0: 2022 6661 6465 7469 6d65 223a 2233 3539   "fadetime":"359
-000032b0: 2e38 222c 0a20 2020 2020 2020 2020 2020  .8",.           
-000032c0: 2020 2020 2022 6466 5f6f 7665 725f 726d       "df_over_rm
-000032d0: 7322 3a34 2e38 2c0a 2020 2020 2020 2020  s":4.8,.        
-000032e0: 2020 2020 2020 2020 2264 665f 7261 7722          "df_raw"
-000032f0: 3a22 302e 3036 205c 7530 3062 3120 302e  :"0.06 \u00b1 0.
-00003300: 3031 222c 0a20 2020 2020 2020 2020 2020  01",.           
-00003310: 2020 2020 2022 7a22 3a22 5c75 3230 3133       "z":"\u2013
-00003320: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00003330: 2020 2022 6d62 6822 3a22 5c75 3230 3133     "mbh":"\u2013
-00003340: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00003350: 2020 2022 7061 676e 7464 6522 3a35 2e39     "pagntde":5.9
-00003360: 3239 2c0a 2020 2020 2020 2020 2020 2020  29,.            
-00003370: 2020 2020 2263 6c61 7373 223a 225c 7532      "class":"\u2
-00003380: 3031 3322 2c0a 2020 2020 2020 2020 2020  013",.          
-00003390: 2020 2020 2020 2264 6622 3a30 2e30 362c        "df":0.06,
-000033a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000033b0: 2022 6466 5f65 223a 302e 3031 2c0a 2020   "df_e":0.01,.  
-000033c0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-000033d0: 6122 3a32 3133 2e33 3334 3633 3732 3533  a":213.334637253
-000033e0: 362c 0a20 2020 2020 2020 2020 2020 2020  6,.             
-000033f0: 2020 2022 6465 6322 3a34 342e 3331 3638     "dec":44.3168
-00003400: 3034 3235 390a 2020 2020 2020 2020 2020  04259.          
-00003410: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00003420: 2022 3231 223a 7b0a 2020 2020 2020 2020   "21":{.        
-00003430: 2020 2020 2020 2020 226e 616d 6522 3a22          "name":"
-00003440: 4154 3230 3139 636c 6522 2c0a 2020 2020  AT2019cle",.    
-00003450: 2020 2020 2020 2020 2020 2020 2274 7065              "tpe
-00003460: 616b 223a 3538 3536 382e 342c 0a20 2020  ak":58568.4,.   
-00003470: 2020 2020 2020 2020 2020 2020 2022 7269               "ri
-00003480: 7365 7469 6d65 223a 2239 2e32 222c 0a20  setime":"9.2",. 
-00003490: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000034a0: 6661 6465 7469 6d65 223a 2235 342e 3822  fadetime":"54.8"
-000034b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000034c0: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
-000034d0: 3139 2e34 2c0a 2020 2020 2020 2020 2020  19.4,.          
-000034e0: 2020 2020 2020 2264 665f 7261 7722 3a22        "df_raw":"
-000034f0: 302e 3235 205c 7530 3062 3120 302e 3031  0.25 \u00b1 0.01
-00003500: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00003510: 2020 2022 7a22 3a22 5c75 3230 3133 222c     "z":"\u2013",
-00003520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003530: 2022 6d62 6822 3a22 5c75 3230 3133 222c   "mbh":"\u2013",
-00003540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003550: 2022 7061 676e 7464 6522 3a30 2e30 3431   "pagntde":0.041
-00003560: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003570: 2020 2263 6c61 7373 223a 225c 7532 3031    "class":"\u201
-00003580: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
-00003590: 2020 2020 2264 6622 3a30 2e32 352c 0a20      "df":0.25,. 
-000035a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000035b0: 6466 5f65 223a 302e 3031 2c0a 2020 2020  df_e":0.01,.    
-000035c0: 2020 2020 2020 2020 2020 2020 2272 6122              "ra"
-000035d0: 3a32 3637 2e37 3534 3633 3732 2c0a 2020  :267.7546372,.  
-000035e0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-000035f0: 6563 223a 3134 2e39 3138 3339 3731 0a20  ec":14.9183971. 
-00003600: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00003610: 2020 2020 2020 2020 2020 2232 3222 3a7b            "22":{
-00003620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003630: 2022 6e61 6d65 223a 2241 5432 3031 3961   "name":"AT2019a
-00003640: 616d 6822 2c0a 2020 2020 2020 2020 2020  amh",.          
-00003650: 2020 2020 2020 2274 7065 616b 223a 3538        "tpeak":58
-00003660: 3538 322e 352c 0a20 2020 2020 2020 2020  582.5,.         
-00003670: 2020 2020 2020 2022 7269 7365 7469 6d65         "risetime
-00003680: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
-00003690: 2020 2020 2020 2020 2020 2020 2266 6164              "fad
-000036a0: 6574 696d 6522 3a22 3135 342e 3522 2c0a  etime":"154.5",.
-000036b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036c0: 2264 665f 6f76 6572 5f72 6d73 223a 372e  "df_over_rms":7.
-000036d0: 372c 0a20 2020 2020 2020 2020 2020 2020  7,.             
-000036e0: 2020 2022 6466 5f72 6177 223a 2230 2e34     "df_raw":"0.4
-000036f0: 3020 5c75 3030 6231 2030 2e30 3122 2c0a  0 \u00b1 0.01",.
-00003700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003710: 227a 223a 225c 7532 3031 3322 2c0a 2020  "z":"\u2013",.  
-00003720: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-00003730: 6268 223a 225c 7532 3031 3322 2c0a 2020  bh":"\u2013",.  
-00003740: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00003750: 6167 6e74 6465 223a 322e 3435 392c 0a20  agntde":2.459,. 
-00003760: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003770: 636c 6173 7322 3a22 5c75 3230 3133 222c  class":"\u2013",
-00003780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003790: 2022 6466 223a 302e 342c 0a20 2020 2020   "df":0.4,.     
-000037a0: 2020 2020 2020 2020 2020 2022 6466 5f65             "df_e
-000037b0: 223a 302e 3031 2c0a 2020 2020 2020 2020  ":0.01,.        
-000037c0: 2020 2020 2020 2020 2272 6122 3a33 3333          "ra":333
-000037d0: 2e32 3639 3233 3337 3137 342c 0a20 2020  .2692337174,.   
-000037e0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-000037f0: 6322 3a32 332e 3536 3230 3231 3636 330a  c":23.562021663.
-00003800: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00003810: 2020 2020 2020 2020 2020 2022 3233 223a             "23":
-00003820: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00003830: 2020 226e 616d 6522 3a22 4154 3230 3139    "name":"AT2019
-00003840: 646c 6c22 2c0a 2020 2020 2020 2020 2020  dll",.          
-00003850: 2020 2020 2020 2274 7065 616b 223a 3538        "tpeak":58
-00003860: 3630 352e 322c 0a20 2020 2020 2020 2020  605.2,.         
-00003870: 2020 2020 2020 2022 7269 7365 7469 6d65         "risetime
-00003880: 223a 2232 392e 3622 2c0a 2020 2020 2020  ":"29.6",.      
-00003890: 2020 2020 2020 2020 2020 2266 6164 6574            "fadet
-000038a0: 696d 6522 3a22 5c75 3230 3133 222c 0a20  ime":"\u2013",. 
-000038b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000038c0: 6466 5f6f 7665 725f 726d 7322 3a36 2e38  df_over_rms":6.8
-000038d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000038e0: 2020 2264 665f 7261 7722 3a22 302e 3236    "df_raw":"0.26
-000038f0: 205c 7530 3062 3120 302e 3031 222c 0a20   \u00b1 0.01",. 
-00003900: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003910: 7a22 3a22 302e 3130 3122 2c0a 2020 2020  z":"0.101",.    
-00003920: 2020 2020 2020 2020 2020 2020 226d 6268              "mbh
-00003930: 223a 2237 2e34 3820 2854 3133 2922 2c0a  ":"7.48 (T13)",.
-00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003950: 2270 6167 6e74 6465 223a 332e 3436 312c  "pagntde":3.461,
-00003960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003970: 2022 636c 6173 7322 3a22 5444 453f 222c   "class":"TDE?",
-00003980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003990: 2022 6466 223a 302e 3236 2c0a 2020 2020   "df":0.26,.    
-000039a0: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-000039b0: 6522 3a30 2e30 312c 0a20 2020 2020 2020  e":0.01,.       
-000039c0: 2020 2020 2020 2020 2022 7261 223a 3137           "ra":17
-000039d0: 352e 3334 3739 3236 2c0a 2020 2020 2020  5.347926,.      
-000039e0: 2020 2020 2020 2020 2020 2264 6563 223a            "dec":
-000039f0: 3231 2e39 3336 3835 3832 0a20 2020 2020  21.9368582.     
-00003a00: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00003a10: 2020 2020 2020 2232 3422 3a7b 0a20 2020        "24":{.   
-00003a20: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-00003a30: 6d65 223a 2241 5432 3031 3967 7572 222c  me":"AT2019gur",
-00003a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003a50: 2022 7470 6561 6b22 3a35 3836 3037 2e35   "tpeak":58607.5
-00003a60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003a70: 2020 2272 6973 6574 696d 6522 3a22 5c75    "risetime":"\u
-00003a80: 3230 3133 222c 0a20 2020 2020 2020 2020  2013",.         
-00003a90: 2020 2020 2020 2022 6661 6465 7469 6d65         "fadetime
-00003aa0: 223a 2232 3334 2e35 222c 0a20 2020 2020  ":"234.5",.     
-00003ab0: 2020 2020 2020 2020 2020 2022 6466 5f6f             "df_o
-00003ac0: 7665 725f 726d 7322 3a33 382e 362c 0a20  ver_rms":38.6,. 
-00003ad0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003ae0: 6466 5f72 6177 223a 2230 2e33 3420 5c75  df_raw":"0.34 \u
-00003af0: 3030 6231 2030 2e30 3122 2c0a 2020 2020  00b1 0.01",.    
-00003b00: 2020 2020 2020 2020 2020 2020 227a 223a              "z":
-00003b10: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
-00003b20: 2020 2020 2020 2020 2020 226d 6268 223a            "mbh":
-00003b30: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
-00003b40: 2020 2020 2020 2020 2020 2270 6167 6e74            "pagnt
-00003b50: 6465 223a 302e 302c 0a20 2020 2020 2020  de":0.0,.       
-00003b60: 2020 2020 2020 2020 2022 636c 6173 7322           "class"
-00003b70: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-00003b80: 2020 2020 2020 2020 2020 2022 6466 223a             "df":
-00003b90: 302e 3334 2c0a 2020 2020 2020 2020 2020  0.34,.          
-00003ba0: 2020 2020 2020 2264 665f 6522 3a30 2e30        "df_e":0.0
-00003bb0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00003bc0: 2020 2022 7261 223a 3334 332e 3730 3332     "ra":343.7032
-00003bd0: 3635 322c 0a20 2020 2020 2020 2020 2020  652,.           
-00003be0: 2020 2020 2022 6465 6322 3a37 372e 3335       "dec":77.35
-00003bf0: 3239 3637 340a 2020 2020 2020 2020 2020  29674.          
-00003c00: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00003c10: 2022 3235 223a 7b0a 2020 2020 2020 2020   "25":{.        
-00003c20: 2020 2020 2020 2020 226e 616d 6522 3a22          "name":"
-00003c30: 4154 3230 3138 6c6f 6622 2c0a 2020 2020  AT2018lof",.    
-00003c40: 2020 2020 2020 2020 2020 2020 2274 7065              "tpe
-00003c50: 616b 223a 3538 3630 382e 322c 0a20 2020  ak":58608.2,.   
-00003c60: 2020 2020 2020 2020 2020 2020 2022 7269               "ri
-00003c70: 7365 7469 6d65 223a 2237 302e 3922 2c0a  setime":"70.9",.
-00003c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c90: 2266 6164 6574 696d 6522 3a22 3337 302e  "fadetime":"370.
-00003ca0: 3422 2c0a 2020 2020 2020 2020 2020 2020  4",.            
-00003cb0: 2020 2020 2264 665f 6f76 6572 5f72 6d73      "df_over_rms
-00003cc0: 223a 342e 312c 0a20 2020 2020 2020 2020  ":4.1,.         
-00003cd0: 2020 2020 2020 2022 6466 5f72 6177 223a         "df_raw":
-00003ce0: 2230 2e31 3520 5c75 3030 6231 2030 2e30  "0.15 \u00b1 0.0
-00003cf0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-00003d00: 2020 2020 227a 223a 2230 2e33 3032 222c      "z":"0.302",
-00003d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003d20: 2022 6d62 6822 3a22 382e 3938 2028 4c31   "mbh":"8.98 (L1
-00003d30: 3929 222c 0a20 2020 2020 2020 2020 2020  9)",.           
-00003d40: 2020 2020 2022 7061 676e 7464 6522 3a35       "pagntde":5
-00003d50: 2e39 3734 2c0a 2020 2020 2020 2020 2020  .974,.          
-00003d60: 2020 2020 2020 2263 6c61 7373 223a 2241        "class":"A
-00003d70: 474e 222c 0a20 2020 2020 2020 2020 2020  GN",.           
-00003d80: 2020 2020 2022 6466 223a 302e 3135 2c0a       "df":0.15,.
-00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003da0: 2264 665f 6522 3a30 2e30 312c 0a20 2020  "df_e":0.01,.   
-00003db0: 2020 2020 2020 2020 2020 2020 2022 7261               "ra
-00003dc0: 223a 3133 352e 3235 3337 3133 312c 0a20  ":135.2537131,. 
-00003dd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003de0: 6465 6322 3a33 352e 3633 3535 3339 310a  dec":35.6355391.
-00003df0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00003e00: 2020 2020 2020 2020 2020 2022 3236 223a             "26":
-00003e10: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00003e20: 2020 226e 616d 6522 3a22 4154 3230 3139    "name":"AT2019
-00003e30: 6471 7622 2c0a 2020 2020 2020 2020 2020  dqv",.          
-00003e40: 2020 2020 2020 2274 7065 616b 223a 3538        "tpeak":58
-00003e50: 3632 382e 322c 0a20 2020 2020 2020 2020  628.2,.         
-00003e60: 2020 2020 2020 2022 7269 7365 7469 6d65         "risetime
-00003e70: 223a 2236 372e 3022 2c0a 2020 2020 2020  ":"67.0",.      
-00003e80: 2020 2020 2020 2020 2020 2266 6164 6574            "fadet
-00003e90: 696d 6522 3a22 3437 352e 3022 2c0a 2020  ime":"475.0",.  
-00003ea0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00003eb0: 665f 6f76 6572 5f72 6d73 223a 3430 2e34  f_over_rms":40.4
-00003ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003ed0: 2020 2264 665f 7261 7722 3a22 312e 3737    "df_raw":"1.77
-00003ee0: 205c 7530 3062 3120 302e 3032 222c 0a20   \u00b1 0.02",. 
-00003ef0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003f00: 7a22 3a22 302e 3038 3136 222c 0a20 2020  z":"0.0816",.   
-00003f10: 2020 2020 2020 2020 2020 2020 2022 6d62               "mb
-00003f20: 6822 3a22 362e 3637 2028 4c31 3929 222c  h":"6.67 (L19)",
-00003f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003f40: 2022 7061 676e 7464 6522 3a30 2e30 2c0a   "pagntde":0.0,.
-00003f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f60: 2263 6c61 7373 223a 2254 4445 3f22 2c0a  "class":"TDE?",.
-00003f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f80: 2264 6622 3a31 2e37 372c 0a20 2020 2020  "df":1.77,.     
-00003f90: 2020 2020 2020 2020 2020 2022 6466 5f65             "df_e
-00003fa0: 223a 302e 3032 2c0a 2020 2020 2020 2020  ":0.02,.        
-00003fb0: 2020 2020 2020 2020 2272 6122 3a31 3630          "ra":160
-00003fc0: 2e38 3735 3235 2c0a 2020 2020 2020 2020  .87525,.        
-00003fd0: 2020 2020 2020 2020 2264 6563 223a 3531          "dec":51
-00003fe0: 2e33 3538 3035 0a20 2020 2020 2020 2020  .35805.         
-00003ff0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00004000: 2020 2232 3722 3a7b 0a20 2020 2020 2020    "27":{.       
-00004010: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-00004020: 2241 5432 3031 3963 7971 222c 0a20 2020  "AT2019cyq",.   
-00004030: 2020 2020 2020 2020 2020 2020 2022 7470               "tp
-00004040: 6561 6b22 3a35 3836 3337 2e32 2c0a 2020  eak":58637.2,.  
-00004050: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00004060: 6973 6574 696d 6522 3a22 3439 2e35 222c  isetime":"49.5",
-00004070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004080: 2022 6661 6465 7469 6d65 223a 2239 352e   "fadetime":"95.
-00004090: 3022 2c0a 2020 2020 2020 2020 2020 2020  0",.            
-000040a0: 2020 2020 2264 665f 6f76 6572 5f72 6d73      "df_over_rms
-000040b0: 223a 3331 2e38 2c0a 2020 2020 2020 2020  ":31.8,.        
-000040c0: 2020 2020 2020 2020 2264 665f 7261 7722          "df_raw"
-000040d0: 3a22 302e 3534 205c 7530 3062 3120 302e  :"0.54 \u00b1 0.
-000040e0: 3031 222c 0a20 2020 2020 2020 2020 2020  01",.           
-000040f0: 2020 2020 2022 7a22 3a22 302e 3236 3222       "z":"0.262"
-00004100: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004110: 2020 226d 6268 223a 2237 2e35 3620 284c    "mbh":"7.56 (L
-00004120: 3139 2922 2c0a 2020 2020 2020 2020 2020  19)",.          
-00004130: 2020 2020 2020 2270 6167 6e74 6465 223a        "pagntde":
-00004140: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
-00004150: 2020 2020 2022 636c 6173 7322 3a22 5444       "class":"TD
-00004160: 453f 222c 0a20 2020 2020 2020 2020 2020  E?",.           
-00004170: 2020 2020 2022 6466 223a 302e 3534 2c0a       "df":0.54,.
-00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004190: 2264 665f 6522 3a30 2e30 312c 0a20 2020  "df_e":0.01,.   
-000041a0: 2020 2020 2020 2020 2020 2020 2022 7261               "ra
-000041b0: 223a 3134 392e 3032 3532 352c 0a20 2020  ":149.02525,.   
-000041c0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-000041d0: 6322 3a31 392e 3534 3930 3339 0a20 2020  c":19.549039.   
-000041e0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-000041f0: 2020 2020 2020 2020 2232 3822 3a7b 0a20          "28":{. 
-00004200: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004210: 6e61 6d65 223a 2241 5432 3032 3161 6575  name":"AT2021aeu
-00004220: 6722 2c0a 2020 2020 2020 2020 2020 2020  g",.            
-00004230: 2020 2020 2274 7065 616b 223a 3538 3634      "tpeak":5864
-00004240: 312e 322c 0a20 2020 2020 2020 2020 2020  1.2,.           
-00004250: 2020 2020 2022 7269 7365 7469 6d65 223a       "risetime":
-00004260: 2234 382e 3622 2c0a 2020 2020 2020 2020  "48.6",.        
-00004270: 2020 2020 2020 2020 2266 6164 6574 696d          "fadetim
-00004280: 6522 3a22 3638 2e38 222c 0a20 2020 2020  e":"68.8",.     
-00004290: 2020 2020 2020 2020 2020 2022 6466 5f6f             "df_o
-000042a0: 7665 725f 726d 7322 3a34 2e36 2c0a 2020  ver_rms":4.6,.  
-000042b0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-000042c0: 665f 7261 7722 3a22 302e 3131 205c 7530  f_raw":"0.11 \u0
-000042d0: 3062 3120 302e 3031 222c 0a20 2020 2020  0b1 0.01",.     
-000042e0: 2020 2020 2020 2020 2020 2022 7a22 3a22             "z":"
-000042f0: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
-00004300: 2020 2020 2020 2020 2022 6d62 6822 3a22           "mbh":"
-00004310: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
-00004320: 2020 2020 2020 2020 2022 7061 676e 7464           "pagntd
-00004330: 6522 3a36 2e30 372c 0a20 2020 2020 2020  e":6.07,.       
-00004340: 2020 2020 2020 2020 2022 636c 6173 7322           "class"
-00004350: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-00004360: 2020 2020 2020 2020 2020 2022 6466 223a             "df":
-00004370: 302e 3131 2c0a 2020 2020 2020 2020 2020  0.11,.          
-00004380: 2020 2020 2020 2264 665f 6522 3a30 2e30        "df_e":0.0
-00004390: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-000043a0: 2020 2022 7261 223a 3233 372e 3536 3639     "ra":237.5669
-000043b0: 3932 3434 3439 2c0a 2020 2020 2020 2020  924449,.        
-000043c0: 2020 2020 2020 2020 2264 6563 223a 3339          "dec":39
-000043d0: 2e32 3336 3431 3439 3933 340a 2020 2020  .2364149934.    
-000043e0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000043f0: 2020 2020 2020 2022 3239 223a 7b0a 2020         "29":{.  
-00004400: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00004410: 616d 6522 3a22 4154 3230 3139 6968 7622  ame":"AT2019ihv"
-00004420: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004430: 2020 2274 7065 616b 223a 3538 3634 362e    "tpeak":58646.
-00004440: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-00004450: 2020 2022 7269 7365 7469 6d65 223a 225c     "risetime":"\
-00004460: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
-00004470: 2020 2020 2020 2020 2266 6164 6574 696d          "fadetim
-00004480: 6522 3a22 3139 2e33 222c 0a20 2020 2020  e":"19.3",.     
-00004490: 2020 2020 2020 2020 2020 2022 6466 5f6f             "df_o
-000044a0: 7665 725f 726d 7322 3a38 2e37 2c0a 2020  ver_rms":8.7,.  
-000044b0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-000044c0: 665f 7261 7722 3a22 302e 3239 205c 7530  f_raw":"0.29 \u0
-000044d0: 3062 3120 302e 3031 222c 0a20 2020 2020  0b1 0.01",.     
-000044e0: 2020 2020 2020 2020 2020 2022 7a22 3a22             "z":"
-000044f0: 302e 3136 3032 222c 0a20 2020 2020 2020  0.1602",.       
-00004500: 2020 2020 2020 2020 2022 6d62 6822 3a22           "mbh":"
-00004510: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
-00004520: 2020 2020 2020 2020 2022 7061 676e 7464           "pagntd
-00004530: 6522 3a31 2e36 3837 2c0a 2020 2020 2020  e":1.687,.      
-00004540: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
-00004550: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
-00004560: 2020 2020 2020 2020 2020 2020 2264 6622              "df"
-00004570: 3a30 2e32 392c 0a20 2020 2020 2020 2020  :0.29,.         
-00004580: 2020 2020 2020 2022 6466 5f65 223a 302e         "df_e":0.
-00004590: 3031 2c0a 2020 2020 2020 2020 2020 2020  01,.            
-000045a0: 2020 2020 2272 6122 3a31 362e 3934 3936      "ra":16.9496
-000045b0: 3732 352c 0a20 2020 2020 2020 2020 2020  725,.           
-000045c0: 2020 2020 2022 6465 6322 3a32 342e 3438       "dec":24.48
-000045d0: 3030 3838 0a20 2020 2020 2020 2020 2020  0088.           
-000045e0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-000045f0: 2233 3022 3a7b 0a20 2020 2020 2020 2020  "30":{.         
-00004600: 2020 2020 2020 2022 6e61 6d65 223a 2241         "name":"A
-00004610: 5432 3031 3964 7a68 222c 0a20 2020 2020  T2019dzh",.     
-00004620: 2020 2020 2020 2020 2020 2022 7470 6561             "tpea
-00004630: 6b22 3a35 3836 3531 2e32 2c0a 2020 2020  k":58651.2,.    
-00004640: 2020 2020 2020 2020 2020 2020 2272 6973              "ris
-00004650: 6574 696d 6522 3a22 3531 2e34 222c 0a20  etime":"51.4",. 
-00004660: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004670: 6661 6465 7469 6d65 223a 2233 3438 2e39  fadetime":"348.9
-00004680: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00004690: 2020 2022 6466 5f6f 7665 725f 726d 7322     "df_over_rms"
-000046a0: 3a36 2e34 2c0a 2020 2020 2020 2020 2020  :6.4,.          
-000046b0: 2020 2020 2020 2264 665f 7261 7722 3a22        "df_raw":"
-000046c0: 302e 3135 205c 7530 3062 3120 302e 3031  0.15 \u00b1 0.01
-000046d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000046e0: 2020 2022 7a22 3a22 302e 3331 3422 2c0a     "z":"0.314",.
-000046f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004700: 226d 6268 223a 225c 7532 3031 3322 2c0a  "mbh":"\u2013",.
-00004710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004720: 2270 6167 6e74 6465 223a 342e 3030 372c  "pagntde":4.007,
-00004730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004740: 2022 636c 6173 7322 3a22 5c75 3230 3133   "class":"\u2013
-00004750: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00004760: 2020 2022 6466 223a 302e 3135 2c0a 2020     "df":0.15,.  
-00004770: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00004780: 665f 6522 3a30 2e30 312c 0a20 2020 2020  f_e":0.01,.     
-00004790: 2020 2020 2020 2020 2020 2022 7261 223a             "ra":
-000047a0: 3138 372e 3832 3532 372c 0a20 2020 2020  187.82527,.     
-000047b0: 2020 2020 2020 2020 2020 2022 6465 6322             "dec"
-000047c0: 3a32 332e 3730 3731 3436 3636 3637 0a20  :23.7071466667. 
-000047d0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-000047e0: 2020 2020 2020 2020 2020 2233 3122 3a7b            "31":{
-000047f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004800: 2022 6e61 6d65 223a 2241 5432 3031 396b   "name":"AT2019k
-00004810: 7175 222c 0a20 2020 2020 2020 2020 2020  qu",.           
-00004820: 2020 2020 2022 7470 6561 6b22 3a35 3836       "tpeak":586
-00004830: 3532 2e32 2c0a 2020 2020 2020 2020 2020  52.2,.          
-00004840: 2020 2020 2020 2272 6973 6574 696d 6522        "risetime"
-00004850: 3a22 3935 2e36 222c 0a20 2020 2020 2020  :"95.6",.       
-00004860: 2020 2020 2020 2020 2022 6661 6465 7469           "fadeti
-00004870: 6d65 223a 2233 3135 2e36 222c 0a20 2020  me":"315.6",.   
-00004880: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00004890: 5f6f 7665 725f 726d 7322 3a36 2e31 2c0a  _over_rms":6.1,.
-000048a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048b0: 2264 665f 7261 7722 3a22 302e 3237 205c  "df_raw":"0.27 \
-000048c0: 7530 3062 3120 302e 3031 222c 0a20 2020  u00b1 0.01",.   
-000048d0: 2020 2020 2020 2020 2020 2020 2022 7a22               "z"
-000048e0: 3a22 302e 3137 3422 2c0a 2020 2020 2020  :"0.174",.      
-000048f0: 2020 2020 2020 2020 2020 226d 6268 223a            "mbh":
-00004900: 2237 2e35 3320 284c 3139 2922 2c0a 2020  "7.53 (L19)",.  
-00004910: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00004920: 6167 6e74 6465 223a 342e 3334 382c 0a20  agntde":4.348,. 
-00004930: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004940: 636c 6173 7322 3a22 5444 453f 222c 0a20  class":"TDE?",. 
-00004950: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004960: 6466 223a 302e 3237 2c0a 2020 2020 2020  df":0.27,.      
-00004970: 2020 2020 2020 2020 2020 2264 665f 6522            "df_e"
-00004980: 3a30 2e30 312c 0a20 2020 2020 2020 2020  :0.01,.         
-00004990: 2020 2020 2020 2022 7261 223a 3234 382e         "ra":248.
-000049a0: 3036 3138 3735 2c0a 2020 2020 2020 2020  061875,.        
-000049b0: 2020 2020 2020 2020 2264 6563 223a 3333          "dec":33
-000049c0: 2e35 3730 3231 310a 2020 2020 2020 2020  .570211.        
-000049d0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-000049e0: 2020 2022 3332 223a 7b0a 2020 2020 2020     "32":{.      
-000049f0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-00004a00: 3a22 4154 3230 3139 6862 6822 2c0a 2020  :"AT2019hbh",.  
-00004a10: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00004a20: 7065 616b 223a 3538 3635 322e 332c 0a20  peak":58652.3,. 
-00004a30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004a40: 7269 7365 7469 6d65 223a 2231 392e 3822  risetime":"19.8"
-00004a50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004a60: 2020 2266 6164 6574 696d 6522 3a22 3130    "fadetime":"10
-00004a70: 362e 3722 2c0a 2020 2020 2020 2020 2020  6.7",.          
-00004a80: 2020 2020 2020 2264 665f 6f76 6572 5f72        "df_over_r
-00004a90: 6d73 223a 382e 342c 0a20 2020 2020 2020  ms":8.4,.       
-00004aa0: 2020 2020 2020 2020 2022 6466 5f72 6177           "df_raw
-00004ab0: 223a 2230 2e37 3520 5c75 3030 6231 2030  ":"0.75 \u00b1 0
-00004ac0: 2e30 3122 2c0a 2020 2020 2020 2020 2020  .01",.          
-00004ad0: 2020 2020 2020 227a 223a 225c 7532 3031        "z":"\u201
-00004ae0: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
-00004af0: 2020 2020 226d 6268 223a 225c 7532 3031      "mbh":"\u201
-00004b00: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
-00004b10: 2020 2020 2270 6167 6e74 6465 223a 312e      "pagntde":1.
-00004b20: 3838 2c0a 2020 2020 2020 2020 2020 2020  88,.            
-00004b30: 2020 2020 2263 6c61 7373 223a 225c 7532      "class":"\u2
-00004b40: 3031 3322 2c0a 2020 2020 2020 2020 2020  013",.          
-00004b50: 2020 2020 2020 2264 6622 3a30 2e37 352c        "df":0.75,
-00004b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b70: 2022 6466 5f65 223a 302e 3031 2c0a 2020   "df_e":0.01,.  
-00004b80: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00004b90: 6122 3a32 3738 2e33 3330 3930 3338 2c0a  a":278.3309038,.
-00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bb0: 2264 6563 223a 3334 2e36 3834 3232 3235  "dec":34.6842225
-00004bc0: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-00004bd0: 2020 2020 2020 2020 2020 2020 2233 3322              "33"
-00004be0: 3a7b 0a20 2020 2020 2020 2020 2020 2020  :{.             
-00004bf0: 2020 2022 6e61 6d65 223a 2241 5432 3032     "name":"AT202
-00004c00: 3061 657a 7a22 2c0a 2020 2020 2020 2020  0aezz",.        
-00004c10: 2020 2020 2020 2020 2274 7065 616b 223a          "tpeak":
-00004c20: 3538 3637 372e 332c 0a20 2020 2020 2020  58677.3,.       
-00004c30: 2020 2020 2020 2020 2022 7269 7365 7469           "riseti
-00004c40: 6d65 223a 2239 392e 3822 2c0a 2020 2020  me":"99.8",.    
-00004c50: 2020 2020 2020 2020 2020 2020 2266 6164              "fad
-00004c60: 6574 696d 6522 3a22 3238 302e 3622 2c0a  etime":"280.6",.
-00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c80: 2264 665f 6f76 6572 5f72 6d73 223a 352e  "df_over_rms":5.
-00004c90: 382c 0a20 2020 2020 2020 2020 2020 2020  8,.             
-00004ca0: 2020 2022 6466 5f72 6177 223a 2230 2e31     "df_raw":"0.1
-00004cb0: 3820 5c75 3030 6231 2030 2e30 3122 2c0a  8 \u00b1 0.01",.
-00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cd0: 227a 223a 225c 7532 3031 3322 2c0a 2020  "z":"\u2013",.  
-00004ce0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-00004cf0: 6268 223a 225c 7532 3031 3322 2c0a 2020  bh":"\u2013",.  
-00004d00: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00004d10: 6167 6e74 6465 223a 342e 3737 312c 0a20  agntde":4.771,. 
-00004d20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004d30: 636c 6173 7322 3a22 5c75 3230 3133 222c  class":"\u2013",
-00004d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d50: 2022 6466 223a 302e 3138 2c0a 2020 2020   "df":0.18,.    
-00004d60: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-00004d70: 6522 3a30 2e30 312c 0a20 2020 2020 2020  e":0.01,.       
-00004d80: 2020 2020 2020 2020 2022 7261 223a 3236           "ra":26
-00004d90: 372e 3036 3531 3933 3334 3739 2c0a 2020  7.0651933479,.  
-00004da0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00004db0: 6563 223a 3535 2e32 3336 3937 3530 3639  ec":55.236975069
-00004dc0: 310a 2020 2020 2020 2020 2020 2020 7d2c  1.            },
-00004dd0: 0a20 2020 2020 2020 2020 2020 2022 3334  .            "34
-00004de0: 223a 7b0a 2020 2020 2020 2020 2020 2020  ":{.            
-00004df0: 2020 2020 226e 616d 6522 3a22 4154 3230      "name":"AT20
-00004e00: 3230 6166 6161 222c 0a20 2020 2020 2020  20afaa",.       
-00004e10: 2020 2020 2020 2020 2022 7470 6561 6b22           "tpeak"
-00004e20: 3a35 3836 3738 2e32 2c0a 2020 2020 2020  :58678.2,.      
-00004e30: 2020 2020 2020 2020 2020 2272 6973 6574            "riset
-00004e40: 696d 6522 3a22 3833 2e38 222c 0a20 2020  ime":"83.8",.   
-00004e50: 2020 2020 2020 2020 2020 2020 2022 6661               "fa
-00004e60: 6465 7469 6d65 223a 2233 3330 2e33 222c  detime":"330.3",
-00004e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e80: 2022 6466 5f6f 7665 725f 726d 7322 3a37   "df_over_rms":7
-00004e90: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
-00004ea0: 2020 2020 2264 665f 7261 7722 3a22 302e      "df_raw":"0.
-00004eb0: 3133 205c 7530 3062 3120 302e 3032 222c  13 \u00b1 0.02",
-00004ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004ed0: 2022 7a22 3a22 5c75 3230 3133 222c 0a20   "z":"\u2013",. 
-00004ee0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004ef0: 6d62 6822 3a22 5c75 3230 3133 222c 0a20  mbh":"\u2013",. 
-00004f00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004f10: 7061 676e 7464 6522 3a33 2e31 3837 2c0a  pagntde":3.187,.
-00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f30: 2263 6c61 7373 223a 225c 7532 3031 3322  "class":"\u2013"
-00004f40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004f50: 2020 2264 6622 3a30 2e31 332c 0a20 2020    "df":0.13,.   
-00004f60: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00004f70: 5f65 223a 302e 3032 2c0a 2020 2020 2020  _e":0.02,.      
-00004f80: 2020 2020 2020 2020 2020 2272 6122 3a32            "ra":2
-00004f90: 3039 2e36 3730 3339 3932 3239 312c 0a20  09.6703992291,. 
-00004fa0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004fb0: 6465 6322 3a32 342e 3731 3139 3438 3836  dec":24.71194886
-00004fc0: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-00004fd0: 2020 2020 2020 2020 2020 2020 2233 3522              "35"
-00004fe0: 3a7b 0a20 2020 2020 2020 2020 2020 2020  :{.             
-00004ff0: 2020 2022 6e61 6d65 223a 2241 5432 3031     "name":"AT201
-00005000: 3969 646d 222c 0a20 2020 2020 2020 2020  9idm",.         
-00005010: 2020 2020 2020 2022 7470 6561 6b22 3a35         "tpeak":5
-00005020: 3836 3832 2e32 2c0a 2020 2020 2020 2020  8682.2,.        
-00005030: 2020 2020 2020 2020 2272 6973 6574 696d          "risetim
-00005040: 6522 3a22 3531 2e37 222c 0a20 2020 2020  e":"51.7",.     
-00005050: 2020 2020 2020 2020 2020 2022 6661 6465             "fade
-00005060: 7469 6d65 223a 225c 7532 3031 3322 2c0a  time":"\u2013",.
-00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005080: 2264 665f 6f76 6572 5f72 6d73 223a 3235  "df_over_rms":25
-00005090: 2e32 2c0a 2020 2020 2020 2020 2020 2020  .2,.            
-000050a0: 2020 2020 2264 665f 7261 7722 3a22 302e      "df_raw":"0.
-000050b0: 3431 205c 7530 3062 3120 302e 3032 222c  41 \u00b1 0.02",
-000050c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000050d0: 2022 7a22 3a22 302e 3035 3434 222c 0a20   "z":"0.0544",. 
-000050e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000050f0: 6d62 6822 3a22 362e 3634 2028 5431 3329  mbh":"6.64 (T13)
-00005100: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00005110: 2020 2022 7061 676e 7464 6522 3a30 2e30     "pagntde":0.0
-00005120: 3032 2c0a 2020 2020 2020 2020 2020 2020  02,.            
-00005130: 2020 2020 2263 6c61 7373 223a 2254 4445      "class":"TDE
-00005140: 3f22 2c0a 2020 2020 2020 2020 2020 2020  ?",.            
-00005150: 2020 2020 2264 6622 3a30 2e34 312c 0a20      "df":0.41,. 
-00005160: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005170: 6466 5f65 223a 302e 3032 2c0a 2020 2020  df_e":0.02,.    
-00005180: 2020 2020 2020 2020 2020 2020 2272 6122              "ra"
-00005190: 3a32 3038 2e31 3935 3235 2c0a 2020 2020  :208.19525,.    
-000051a0: 2020 2020 2020 2020 2020 2020 2264 6563              "dec
-000051b0: 223a 3230 2e34 3132 3138 310a 2020 2020  ":20.412181.    
-000051c0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000051d0: 2020 2020 2020 2022 3336 223a 7b0a 2020         "36":{.  
-000051e0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-000051f0: 616d 6522 3a22 4154 3230 3139 6968 7522  ame":"AT2019ihu"
-00005200: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005210: 2020 2274 7065 616b 223a 3538 3730 392e    "tpeak":58709.
-00005220: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-00005230: 2020 2022 7269 7365 7469 6d65 223a 2237     "risetime":"7
-00005240: 392e 3722 2c0a 2020 2020 2020 2020 2020  9.7",.          
-00005250: 2020 2020 2020 2266 6164 6574 696d 6522        "fadetime"
-00005260: 3a22 3131 302e 3922 2c0a 2020 2020 2020  :"110.9",.      
-00005270: 2020 2020 2020 2020 2020 2264 665f 6f76            "df_ov
-00005280: 6572 5f72 6d73 223a 362e 322c 0a20 2020  er_rms":6.2,.   
-00005290: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-000052a0: 5f72 6177 223a 2230 2e32 3520 5c75 3030  _raw":"0.25 \u00
-000052b0: 6231 2030 2e30 3222 2c0a 2020 2020 2020  b1 0.02",.      
-000052c0: 2020 2020 2020 2020 2020 227a 223a 2230            "z":"0
-000052d0: 2e32 3722 2c0a 2020 2020 2020 2020 2020  .27",.          
-000052e0: 2020 2020 2020 226d 6268 223a 2238 2e39        "mbh":"8.9
-000052f0: 3020 284c 3139 2922 2c0a 2020 2020 2020  0 (L19)",.      
-00005300: 2020 2020 2020 2020 2020 2270 6167 6e74            "pagnt
-00005310: 6465 223a 342e 3139 322c 0a20 2020 2020  de":4.192,.     
-00005320: 2020 2020 2020 2020 2020 2022 636c 6173             "clas
-00005330: 7322 3a22 4147 4e22 2c0a 2020 2020 2020  s":"AGN",.      
-00005340: 2020 2020 2020 2020 2020 2264 6622 3a30            "df":0
-00005350: 2e32 352c 0a20 2020 2020 2020 2020 2020  .25,.           
-00005360: 2020 2020 2022 6466 5f65 223a 302e 3032       "df_e":0.02
-00005370: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005380: 2020 2272 6122 3a33 3538 2e37 3337 3932    "ra":358.73792
-00005390: 3237 2c0a 2020 2020 2020 2020 2020 2020  27,.            
-000053a0: 2020 2020 2264 6563 223a 302e 3730 3535      "dec":0.7055
-000053b0: 3432 350a 2020 2020 2020 2020 2020 2020  425.            
-000053c0: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-000053d0: 3337 223a 7b0a 2020 2020 2020 2020 2020  37":{.          
-000053e0: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
-000053f0: 3230 3139 6d65 6822 2c0a 2020 2020 2020  2019meh",.      
-00005400: 2020 2020 2020 2020 2020 2274 7065 616b            "tpeak
-00005410: 223a 3538 3731 332e 312c 0a20 2020 2020  ":58713.1,.     
-00005420: 2020 2020 2020 2020 2020 2022 7269 7365             "rise
-00005430: 7469 6d65 223a 2232 332e 3222 2c0a 2020  time":"23.2",.  
-00005440: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-00005450: 6164 6574 696d 6522 3a22 3132 372e 3922  adetime":"127.9"
-00005460: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005470: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
-00005480: 3239 2e37 2c0a 2020 2020 2020 2020 2020  29.7,.          
-00005490: 2020 2020 2020 2264 665f 7261 7722 3a22        "df_raw":"
-000054a0: 312e 3939 205c 7530 3062 3120 302e 3034  1.99 \u00b1 0.04
-000054b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000054c0: 2020 2022 7a22 3a22 302e 3039 3335 222c     "z":"0.0935",
-000054d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000054e0: 2022 6d62 6822 3a22 372e 3036 2028 5632   "mbh":"7.06 (V2
-000054f0: 3129 222c 0a20 2020 2020 2020 2020 2020  1)",.           
-00005500: 2020 2020 2022 7061 676e 7464 6522 3a30       "pagntde":0
-00005510: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
-00005520: 2020 2020 2263 6c61 7373 223a 2254 4445      "class":"TDE
-00005530: 3f22 2c0a 2020 2020 2020 2020 2020 2020  ?",.            
-00005540: 2020 2020 2264 6622 3a31 2e39 392c 0a20      "df":1.99,. 
-00005550: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005560: 6466 5f65 223a 302e 3034 2c0a 2020 2020  df_e":0.04,.    
-00005570: 2020 2020 2020 2020 2020 2020 2272 6122              "ra"
-00005580: 3a33 3231 2e38 3232 3730 382c 0a20 2020  :321.822708,.   
-00005590: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-000055a0: 6322 3a36 342e 3431 3634 3339 0a20 2020  c":64.416439.   
-000055b0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-000055c0: 2020 2020 2020 2020 2233 3822 3a7b 0a20          "38":{. 
-000055d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000055e0: 6e61 6d65 223a 2241 5432 3032 3061 6661  name":"AT2020afa
-000055f0: 6222 2c0a 2020 2020 2020 2020 2020 2020  b",.            
-00005600: 2020 2020 2274 7065 616b 223a 3538 3731      "tpeak":5871
-00005610: 372e 322c 0a20 2020 2020 2020 2020 2020  7.2,.           
-00005620: 2020 2020 2022 7269 7365 7469 6d65 223a       "risetime":
-00005630: 2234 372e 3522 2c0a 2020 2020 2020 2020  "47.5",.        
-00005640: 2020 2020 2020 2020 2266 6164 6574 696d          "fadetim
-00005650: 6522 3a22 3132 372e 3222 2c0a 2020 2020  e":"127.2",.    
-00005660: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-00005670: 6f76 6572 5f72 6d73 223a 352e 302c 0a20  over_rms":5.0,. 
-00005680: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005690: 6466 5f72 6177 223a 2230 2e32 3220 5c75  df_raw":"0.22 \u
-000056a0: 3030 6231 2030 2e30 3122 2c0a 2020 2020  00b1 0.01",.    
-000056b0: 2020 2020 2020 2020 2020 2020 227a 223a              "z":
-000056c0: 2230 2e32 3837 3522 2c0a 2020 2020 2020  "0.2875",.      
-000056d0: 2020 2020 2020 2020 2020 226d 6268 223a            "mbh":
-000056e0: 2236 2e34 3920 2856 3231 2922 2c0a 2020  "6.49 (V21)",.  
-000056f0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00005700: 6167 6e74 6465 223a 352e 3738 392c 0a20  agntde":5.789,. 
-00005710: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005720: 636c 6173 7322 3a22 5444 453f 222c 0a20  class":"TDE?",. 
-00005730: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005740: 6466 223a 302e 3232 2c0a 2020 2020 2020  df":0.22,.      
-00005750: 2020 2020 2020 2020 2020 2264 665f 6522            "df_e"
-00005760: 3a30 2e30 312c 0a20 2020 2020 2020 2020  :0.01,.         
-00005770: 2020 2020 2020 2022 7261 223a 3433 2e33         "ra":43.3
-00005780: 3334 3037 3832 3830 372c 0a20 2020 2020  340782807,.     
-00005790: 2020 2020 2020 2020 2020 2022 6465 6322             "dec"
-000057a0: 3a34 342e 3330 3135 3136 3134 3232 0a20  :44.3015161422. 
-000057b0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-000057c0: 2020 2020 2020 2020 2020 2233 3922 3a7b            "39":{
-000057d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000057e0: 2022 6e61 6d65 223a 2241 5432 3031 3961   "name":"AT2019a
-000057f0: 616d 6922 2c0a 2020 2020 2020 2020 2020  ami",.          
-00005800: 2020 2020 2020 2274 7065 616b 223a 3538        "tpeak":58
-00005810: 3731 372e 342c 0a20 2020 2020 2020 2020  717.4,.         
-00005820: 2020 2020 2020 2022 7269 7365 7469 6d65         "risetime
-00005830: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
-00005840: 2020 2020 2020 2020 2020 2020 2266 6164              "fad
-00005850: 6574 696d 6522 3a22 3135 322e 3022 2c0a  etime":"152.0",.
-00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005870: 2264 665f 6f76 6572 5f72 6d73 223a 3331  "df_over_rms":31
-00005880: 2e38 2c0a 2020 2020 2020 2020 2020 2020  .8,.            
-00005890: 2020 2020 2264 665f 7261 7722 3a22 302e      "df_raw":"0.
-000058a0: 3431 205c 7530 3062 3120 302e 3031 222c  41 \u00b1 0.01",
-000058b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000058c0: 2022 7a22 3a22 5c75 3230 3133 222c 0a20   "z":"\u2013",. 
-000058d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000058e0: 6d62 6822 3a22 5c75 3230 3133 222c 0a20  mbh":"\u2013",. 
-000058f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005900: 7061 676e 7464 6522 3a30 2e30 2c0a 2020  pagntde":0.0,.  
-00005910: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-00005920: 6c61 7373 223a 225c 7532 3031 3322 2c0a  lass":"\u2013",.
-00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005940: 2264 6622 3a30 2e34 312c 0a20 2020 2020  "df":0.41,.     
-00005950: 2020 2020 2020 2020 2020 2022 6466 5f65             "df_e
-00005960: 223a 302e 3031 2c0a 2020 2020 2020 2020  ":0.01,.        
-00005970: 2020 2020 2020 2020 2272 6122 3a38 2e39          "ra":8.9
-00005980: 3331 3130 3831 3738 382c 0a20 2020 2020  311081788,.     
-00005990: 2020 2020 2020 2020 2020 2022 6465 6322             "dec"
-000059a0: 3a34 372e 3235 3932 3534 3638 3438 0a20  :47.2592546848. 
-000059b0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-000059c0: 2020 2020 2020 2020 2020 2234 3022 3a7b            "40":{
-000059d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000059e0: 2022 6e61 6d65 223a 2241 5432 3031 396e   "name":"AT2019n
-000059f0: 6e61 222c 0a20 2020 2020 2020 2020 2020  na",.           
-00005a00: 2020 2020 2022 7470 6561 6b22 3a35 3837       "tpeak":587
-00005a10: 3137 2e34 2c0a 2020 2020 2020 2020 2020  17.4,.          
-00005a20: 2020 2020 2020 2272 6973 6574 696d 6522        "risetime"
-00005a30: 3a22 3334 2e34 222c 0a20 2020 2020 2020  :"34.4",.       
-00005a40: 2020 2020 2020 2020 2022 6661 6465 7469           "fadeti
-00005a50: 6d65 223a 2238 372e 3122 2c0a 2020 2020  me":"87.1",.    
-00005a60: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-00005a70: 6f76 6572 5f72 6d73 223a 3237 2e30 2c0a  over_rms":27.0,.
-00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a90: 2264 665f 7261 7722 3a22 302e 3336 205c  "df_raw":"0.36 \
-00005aa0: 7530 3062 3120 302e 3031 222c 0a20 2020  u00b1 0.01",.   
-00005ab0: 2020 2020 2020 2020 2020 2020 2022 7a22               "z"
-00005ac0: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-00005ad0: 2020 2020 2020 2020 2020 2022 6d62 6822             "mbh"
-00005ae0: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-00005af0: 2020 2020 2020 2020 2020 2022 7061 676e             "pagn
-00005b00: 7464 6522 3a30 2e30 3031 2c0a 2020 2020  tde":0.001,.    
-00005b10: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
-00005b20: 7373 223a 225c 7532 3031 3322 2c0a 2020  ss":"\u2013",.  
-00005b30: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00005b40: 6622 3a30 2e33 362c 0a20 2020 2020 2020  f":0.36,.       
-00005b50: 2020 2020 2020 2020 2022 6466 5f65 223a           "df_e":
-00005b60: 302e 3031 2c0a 2020 2020 2020 2020 2020  0.01,.          
-00005b70: 2020 2020 2020 2272 6122 3a33 3537 2e31        "ra":357.1
-00005b80: 3630 3238 3638 3636 372c 0a20 2020 2020  602868667,.     
-00005b90: 2020 2020 2020 2020 2020 2022 6465 6322             "dec"
-00005ba0: 3a31 392e 3236 3238 3031 3838 3333 0a20  :19.2628018833. 
-00005bb0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00005bc0: 2020 2020 2020 2020 2020 2234 3122 3a7b            "41":{
-00005bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005be0: 2022 6e61 6d65 223a 2241 5432 3031 396e   "name":"AT2019n
-00005bf0: 6e69 222c 0a20 2020 2020 2020 2020 2020  ni",.           
-00005c00: 2020 2020 2022 7470 6561 6b22 3a35 3837       "tpeak":587
-00005c10: 3332 2e32 2c0a 2020 2020 2020 2020 2020  32.2,.          
-00005c20: 2020 2020 2020 2272 6973 6574 696d 6522        "risetime"
-00005c30: 3a22 3239 2e31 222c 0a20 2020 2020 2020  :"29.1",.       
-00005c40: 2020 2020 2020 2020 2022 6661 6465 7469           "fadeti
-00005c50: 6d65 223a 2231 3039 2e35 222c 0a20 2020  me":"109.5",.   
-00005c60: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00005c70: 5f6f 7665 725f 726d 7322 3a34 2e39 2c0a  _over_rms":4.9,.
-00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c90: 2264 665f 7261 7722 3a22 302e 3336 205c  "df_raw":"0.36 \
-00005ca0: 7530 3062 3120 302e 3031 222c 0a20 2020  u00b1 0.01",.   
-00005cb0: 2020 2020 2020 2020 2020 2020 2022 7a22               "z"
-00005cc0: 3a22 302e 3133 3722 2c0a 2020 2020 2020  :"0.137",.      
-00005cd0: 2020 2020 2020 2020 2020 226d 6268 223a            "mbh":
-00005ce0: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
-00005cf0: 2020 2020 2020 2020 2020 2270 6167 6e74            "pagnt
-00005d00: 6465 223a 352e 3833 342c 0a20 2020 2020  de":5.834,.     
-00005d10: 2020 2020 2020 2020 2020 2022 636c 6173             "clas
-00005d20: 7322 3a22 5c75 3230 3133 222c 0a20 2020  s":"\u2013",.   
-00005d30: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00005d40: 223a 302e 3336 2c0a 2020 2020 2020 2020  ":0.36,.        
-00005d50: 2020 2020 2020 2020 2264 665f 6522 3a30          "df_e":0
-00005d60: 2e30 312c 0a20 2020 2020 2020 2020 2020  .01,.           
-00005d70: 2020 2020 2022 7261 223a 3332 382e 3332       "ra":328.32
-00005d80: 3731 3932 3038 3735 2c0a 2020 2020 2020  71920875,.      
-00005d90: 2020 2020 2020 2020 2020 2264 6563 223a            "dec":
-00005da0: 2d31 392e 3232 3733 3232 3235 0a20 2020  -19.22732225.   
-00005db0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00005dc0: 2020 2020 2020 2020 2234 3222 3a7b 0a20          "42":{. 
-00005dd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005de0: 6e61 6d65 223a 2241 5432 3032 3161 6575  name":"AT2021aeu
-00005df0: 6b22 2c0a 2020 2020 2020 2020 2020 2020  k",.            
-00005e00: 2020 2020 2274 7065 616b 223a 3538 3733      "tpeak":5873
-00005e10: 332e 312c 0a20 2020 2020 2020 2020 2020  3.1,.           
-00005e20: 2020 2020 2022 7269 7365 7469 6d65 223a       "risetime":
-00005e30: 2234 332e 3422 2c0a 2020 2020 2020 2020  "43.4",.        
-00005e40: 2020 2020 2020 2020 2266 6164 6574 696d          "fadetim
-00005e50: 6522 3a22 3233 382e 3122 2c0a 2020 2020  e":"238.1",.    
-00005e60: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-00005e70: 6f76 6572 5f72 6d73 223a 372e 332c 0a20  over_rms":7.3,. 
-00005e80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005e90: 6466 5f72 6177 223a 2230 2e33 3320 5c75  df_raw":"0.33 \u
-00005ea0: 3030 6231 2030 2e30 3122 2c0a 2020 2020  00b1 0.01",.    
-00005eb0: 2020 2020 2020 2020 2020 2020 227a 223a              "z":
-00005ec0: 2230 2e32 3335 222c 0a20 2020 2020 2020  "0.235",.       
-00005ed0: 2020 2020 2020 2020 2022 6d62 6822 3a22           "mbh":"
-00005ee0: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
-00005ef0: 2020 2020 2020 2020 2022 7061 676e 7464           "pagntd
-00005f00: 6522 3a32 2e38 3237 2c0a 2020 2020 2020  e":2.827,.      
-00005f10: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
-00005f20: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
-00005f30: 2020 2020 2020 2020 2020 2020 2264 6622              "df"
-00005f40: 3a30 2e33 332c 0a20 2020 2020 2020 2020  :0.33,.         
-00005f50: 2020 2020 2020 2022 6466 5f65 223a 302e         "df_e":0.
-00005f60: 3031 2c0a 2020 2020 2020 2020 2020 2020  01,.            
-00005f70: 2020 2020 2272 6122 3a32 3433 2e32 3439      "ra":243.249
-00005f80: 3334 3332 3536 372c 0a20 2020 2020 2020  3432567,.       
-00005f90: 2020 2020 2020 2020 2022 6465 6322 3a34           "dec":4
-00005fa0: 322e 3332 3738 3436 3630 3636 0a20 2020  2.3278466066.   
-00005fb0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00005fc0: 2020 2020 2020 2020 2234 3322 3a7b 0a20          "43":{. 
-00005fd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005fe0: 6e61 6d65 223a 2241 5432 3031 3968 6479  name":"AT2019hdy
-00005ff0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00006000: 2020 2022 7470 6561 6b22 3a35 3837 3439     "tpeak":58749
-00006010: 2e35 2c0a 2020 2020 2020 2020 2020 2020  .5,.            
-00006020: 2020 2020 2272 6973 6574 696d 6522 3a22      "risetime":"
-00006030: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
-00006040: 2020 2020 2020 2020 2022 6661 6465 7469           "fadeti
-00006050: 6d65 223a 2238 372e 3922 2c0a 2020 2020  me":"87.9",.    
-00006060: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-00006070: 6f76 6572 5f72 6d73 223a 342e 302c 0a20  over_rms":4.0,. 
-00006080: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006090: 6466 5f72 6177 223a 2230 2e32 3020 5c75  df_raw":"0.20 \u
-000060a0: 3030 6231 2030 2e30 3122 2c0a 2020 2020  00b1 0.01",.    
-000060b0: 2020 2020 2020 2020 2020 2020 227a 223a              "z":
-000060c0: 2230 2e34 3432 222c 0a20 2020 2020 2020  "0.442",.       
-000060d0: 2020 2020 2020 2020 2022 6d62 6822 3a22           "mbh":"
-000060e0: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
-000060f0: 2020 2020 2020 2020 2022 7061 676e 7464           "pagntd
-00006100: 6522 3a35 2e38 3633 2c0a 2020 2020 2020  e":5.863,.      
-00006110: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
-00006120: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
-00006130: 2020 2020 2020 2020 2020 2020 2264 6622              "df"
-00006140: 3a30 2e32 2c0a 2020 2020 2020 2020 2020  :0.2,.          
-00006150: 2020 2020 2020 2264 665f 6522 3a30 2e30        "df_e":0.0
-00006160: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00006170: 2020 2022 7261 223a 3134 322e 3436 3137     "ra":142.4617
-00006180: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-00006190: 2020 2022 6465 6322 3a31 392e 3439 3330     "dec":19.4930
-000061a0: 3131 0a20 2020 2020 2020 2020 2020 207d  11.            }
-000061b0: 2c0a 2020 2020 2020 2020 2020 2020 2234  ,.            "4
-000061c0: 3422 3a7b 0a20 2020 2020 2020 2020 2020  4":{.           
-000061d0: 2020 2020 2022 6e61 6d65 223a 2241 5432       "name":"AT2
-000061e0: 3031 3970 6576 222c 0a20 2020 2020 2020  019pev",.       
-000061f0: 2020 2020 2020 2020 2022 7470 6561 6b22           "tpeak"
-00006200: 3a35 3837 3530 2e31 2c0a 2020 2020 2020  :58750.1,.      
-00006210: 2020 2020 2020 2020 2020 2272 6973 6574            "riset
-00006220: 696d 6522 3a22 3133 2e31 222c 0a20 2020  ime":"13.1",.   
-00006230: 2020 2020 2020 2020 2020 2020 2022 6661               "fa
-00006240: 6465 7469 6d65 223a 2235 342e 3722 2c0a  detime":"54.7",.
-00006250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006260: 2264 665f 6f76 6572 5f72 6d73 223a 372e  "df_over_rms":7.
-00006270: 342c 0a20 2020 2020 2020 2020 2020 2020  4,.             
-00006280: 2020 2022 6466 5f72 6177 223a 2230 2e31     "df_raw":"0.1
-00006290: 3920 5c75 3030 6231 2030 2e30 3122 2c0a  9 \u00b1 0.01",.
-000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062b0: 227a 223a 2230 2e30 3937 222c 0a20 2020  "z":"0.097",.   
-000062c0: 2020 2020 2020 2020 2020 2020 2022 6d62               "mb
-000062d0: 6822 3a22 362e 3430 2028 4632 3029 222c  h":"6.40 (F20)",
-000062e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000062f0: 2022 7061 676e 7464 6522 3a32 2e37 3239   "pagntde":2.729
-00006300: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006310: 2020 2263 6c61 7373 223a 2254 4445 3f22    "class":"TDE?"
-00006320: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006330: 2020 2264 6622 3a30 2e31 392c 0a20 2020    "df":0.19,.   
-00006340: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00006350: 5f65 223a 302e 3031 2c0a 2020 2020 2020  _e":0.01,.      
-00006360: 2020 2020 2020 2020 2020 2272 6122 3a36            "ra":6
-00006370: 372e 3334 3436 3637 2c0a 2020 2020 2020  7.344667,.      
-00006380: 2020 2020 2020 2020 2020 2264 6563 223a            "dec":
-00006390: 302e 3631 3837 350a 2020 2020 2020 2020  0.61875.        
-000063a0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-000063b0: 2020 2022 3435 223a 7b0a 2020 2020 2020     "45":{.      
-000063c0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-000063d0: 3a22 4154 3230 3133 6b70 222c 0a20 2020  :"AT2013kp",.   
-000063e0: 2020 2020 2020 2020 2020 2020 2022 7470               "tp
-000063f0: 6561 6b22 3a35 3837 3533 2e31 2c0a 2020  eak":58753.1,.  
-00006400: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00006410: 6973 6574 696d 6522 3a22 3131 2e39 222c  isetime":"11.9",
-00006420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006430: 2022 6661 6465 7469 6d65 223a 2233 342e   "fadetime":"34.
-00006440: 3722 2c0a 2020 2020 2020 2020 2020 2020  7",.            
-00006450: 2020 2020 2264 665f 6f76 6572 5f72 6d73      "df_over_rms
-00006460: 223a 3434 2e34 2c0a 2020 2020 2020 2020  ":44.4,.        
-00006470: 2020 2020 2020 2020 2264 665f 7261 7722          "df_raw"
-00006480: 3a22 322e 3134 205c 7530 3062 3120 302e  :"2.14 \u00b1 0.
-00006490: 3034 222c 0a20 2020 2020 2020 2020 2020  04",.           
-000064a0: 2020 2020 2022 7a22 3a22 302e 3031 3439       "z":"0.0149
-000064b0: 3922 2c0a 2020 2020 2020 2020 2020 2020  9",.            
-000064c0: 2020 2020 226d 6268 223a 2236 2e31 3920      "mbh":"6.19 
-000064d0: 284e 3230 2922 2c0a 2020 2020 2020 2020  (N20)",.        
-000064e0: 2020 2020 2020 2020 2270 6167 6e74 6465          "pagntde
-000064f0: 223a 302e 302c 0a20 2020 2020 2020 2020  ":0.0,.         
-00006500: 2020 2020 2020 2022 636c 6173 7322 3a22         "class":"
-00006510: 5444 4522 2c0a 2020 2020 2020 2020 2020  TDE",.          
-00006520: 2020 2020 2020 2264 6622 3a32 2e31 342c        "df":2.14,
-00006530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006540: 2022 6466 5f65 223a 302e 3034 2c0a 2020   "df_e":0.04,.  
-00006550: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00006560: 6122 3a37 312e 3635 3738 3136 3630 342c  a":71.657816604,
-00006570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006580: 2022 6465 6322 3a2d 3130 2e32 3236 3331   "dec":-10.22631
-00006590: 3936 3238 320a 2020 2020 2020 2020 2020  96282.          
-000065a0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-000065b0: 2022 3436 223a 7b0a 2020 2020 2020 2020   "46":{.        
-000065c0: 2020 2020 2020 2020 226e 616d 6522 3a22          "name":"
-000065d0: 4154 3230 3139 6272 7322 2c0a 2020 2020  AT2019brs",.    
-000065e0: 2020 2020 2020 2020 2020 2020 2274 7065              "tpe
-000065f0: 616b 223a 3538 3735 382e 312c 0a20 2020  ak":58758.1,.   
-00006600: 2020 2020 2020 2020 2020 2020 2022 7269               "ri
-00006610: 7365 7469 6d65 223a 2231 3130 2e39 222c  setime":"110.9",
-00006620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006630: 2022 6661 6465 7469 6d65 223a 2234 3833   "fadetime":"483
-00006640: 2e32 222c 0a20 2020 2020 2020 2020 2020  .2",.           
-00006650: 2020 2020 2022 6466 5f6f 7665 725f 726d       "df_over_rm
-00006660: 7322 3a39 2e36 2c0a 2020 2020 2020 2020  s":9.6,.        
-00006670: 2020 2020 2020 2020 2264 665f 7261 7722          "df_raw"
-00006680: 3a22 302e 3738 205c 7530 3062 3120 302e  :"0.78 \u00b1 0.
-00006690: 3031 222c 0a20 2020 2020 2020 2020 2020  01",.           
-000066a0: 2020 2020 2022 7a22 3a22 302e 3337 3336       "z":"0.3736
-000066b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000066c0: 2020 2022 6d62 6822 3a22 372e 3230 2028     "mbh":"7.20 (
-000066d0: 4632 3029 222c 0a20 2020 2020 2020 2020  F20)",.         
-000066e0: 2020 2020 2020 2022 7061 676e 7464 6522         "pagntde"
-000066f0: 3a31 2e32 3237 2c0a 2020 2020 2020 2020  :1.227,.        
-00006700: 2020 2020 2020 2020 2263 6c61 7373 223a          "class":
-00006710: 2254 4445 3f22 2c0a 2020 2020 2020 2020  "TDE?",.        
-00006720: 2020 2020 2020 2020 2264 6622 3a30 2e37          "df":0.7
-00006730: 382c 0a20 2020 2020 2020 2020 2020 2020  8,.             
-00006740: 2020 2022 6466 5f65 223a 302e 3031 2c0a     "df_e":0.01,.
-00006750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006760: 2272 6122 3a32 3136 2e39 3433 3333 332c  "ra":216.943333,
-00006770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006780: 2022 6465 6322 3a32 392e 3531 3036 3331   "dec":29.510631
-00006790: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-000067a0: 2020 2020 2020 2020 2020 2020 2234 3722              "47"
-000067b0: 3a7b 0a20 2020 2020 2020 2020 2020 2020  :{.             
-000067c0: 2020 2022 6e61 6d65 223a 2241 5432 3032     "name":"AT202
-000067d0: 3061 6661 6322 2c0a 2020 2020 2020 2020  0afac",.        
-000067e0: 2020 2020 2020 2020 2274 7065 616b 223a          "tpeak":
-000067f0: 3538 3735 382e 332c 0a20 2020 2020 2020  58758.3,.       
-00006800: 2020 2020 2020 2020 2022 7269 7365 7469           "riseti
-00006810: 6d65 223a 2236 382e 3022 2c0a 2020 2020  me":"68.0",.    
-00006820: 2020 2020 2020 2020 2020 2020 2266 6164              "fad
-00006830: 6574 696d 6522 3a22 3935 2e30 222c 0a20  etime":"95.0",. 
-00006840: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006850: 6466 5f6f 7665 725f 726d 7322 3a31 302e  df_over_rms":10.
-00006860: 382c 0a20 2020 2020 2020 2020 2020 2020  8,.             
-00006870: 2020 2022 6466 5f72 6177 223a 2230 2e31     "df_raw":"0.1
-00006880: 3620 5c75 3030 6231 2030 2e30 3122 2c0a  6 \u00b1 0.01",.
-00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068a0: 227a 223a 225c 7532 3031 3322 2c0a 2020  "z":"\u2013",.  
-000068b0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-000068c0: 6268 223a 225c 7532 3031 3322 2c0a 2020  bh":"\u2013",.  
-000068d0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-000068e0: 6167 6e74 6465 223a 302e 3836 352c 0a20  agntde":0.865,. 
-000068f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006900: 636c 6173 7322 3a22 5c75 3230 3133 222c  class":"\u2013",
-00006910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006920: 2022 6466 223a 302e 3136 2c0a 2020 2020   "df":0.16,.    
-00006930: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-00006940: 6522 3a30 2e30 312c 0a20 2020 2020 2020  e":0.01,.       
-00006950: 2020 2020 2020 2020 2022 7261 223a 3236           "ra":26
-00006960: 382e 3431 3733 3934 3134 3131 2c0a 2020  8.4173941411,.  
-00006970: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00006980: 6563 223a 3535 2e38 3537 3533 3535 3038  ec":55.857535508
-00006990: 390a 2020 2020 2020 2020 2020 2020 7d2c  9.            },
-000069a0: 0a20 2020 2020 2020 2020 2020 2022 3438  .            "48
-000069b0: 223a 7b0a 2020 2020 2020 2020 2020 2020  ":{.            
-000069c0: 2020 2020 226e 616d 6522 3a22 4154 3230      "name":"AT20
-000069d0: 3139 7772 6422 2c0a 2020 2020 2020 2020  19wrd",.        
-000069e0: 2020 2020 2020 2020 2274 7065 616b 223a          "tpeak":
-000069f0: 3538 3736 342e 332c 0a20 2020 2020 2020  58764.3,.       
-00006a00: 2020 2020 2020 2020 2022 7269 7365 7469           "riseti
-00006a10: 6d65 223a 2238 322e 3622 2c0a 2020 2020  me":"82.6",.    
-00006a20: 2020 2020 2020 2020 2020 2020 2266 6164              "fad
-00006a30: 6574 696d 6522 3a22 5c75 3230 3133 222c  etime":"\u2013",
-00006a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006a50: 2022 6466 5f6f 7665 725f 726d 7322 3a37   "df_over_rms":7
-00006a60: 2e36 2c0a 2020 2020 2020 2020 2020 2020  .6,.            
-00006a70: 2020 2020 2264 665f 7261 7722 3a22 302e      "df_raw":"0.
-00006a80: 3135 205c 7530 3062 3120 302e 3031 222c  15 \u00b1 0.01",
-00006a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006aa0: 2022 7a22 3a22 5c75 3230 3133 222c 0a20   "z":"\u2013",. 
-00006ab0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006ac0: 6d62 6822 3a22 5c75 3230 3133 222c 0a20  mbh":"\u2013",. 
-00006ad0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006ae0: 7061 676e 7464 6522 3a32 2e35 3632 2c0a  pagntde":2.562,.
-00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b00: 2263 6c61 7373 223a 225c 7532 3031 3322  "class":"\u2013"
-00006b10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006b20: 2020 2264 6622 3a30 2e31 352c 0a20 2020    "df":0.15,.   
-00006b30: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00006b40: 5f65 223a 302e 3031 2c0a 2020 2020 2020  _e":0.01,.      
-00006b50: 2020 2020 2020 2020 2020 2272 6122 3a33            "ra":3
-00006b60: 3535 2e39 3831 3435 382c 0a20 2020 2020  55.981458,.     
-00006b70: 2020 2020 2020 2020 2020 2022 6465 6322             "dec"
-00006b80: 3a33 312e 3337 3731 350a 2020 2020 2020  :31.37715.      
-00006b90: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00006ba0: 2020 2020 2022 3439 223a 7b0a 2020 2020       "49":{.    
-00006bb0: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
-00006bc0: 6522 3a22 4154 3230 3231 6165 7568 222c  e":"AT2021aeuh",
-00006bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006be0: 2022 7470 6561 6b22 3a35 3837 3839 2e35   "tpeak":58789.5
-00006bf0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006c00: 2020 2272 6973 6574 696d 6522 3a22 5c75    "risetime":"\u
-00006c10: 3230 3133 222c 0a20 2020 2020 2020 2020  2013",.         
-00006c20: 2020 2020 2020 2022 6661 6465 7469 6d65         "fadetime
-00006c30: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
-00006c40: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-00006c50: 6f76 6572 5f72 6d73 223a 332e 392c 0a20  over_rms":3.9,. 
-00006c60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006c70: 6466 5f72 6177 223a 2230 2e32 3820 5c75  df_raw":"0.28 \u
-00006c80: 3030 6231 2030 2e30 3122 2c0a 2020 2020  00b1 0.01",.    
-00006c90: 2020 2020 2020 2020 2020 2020 227a 223a              "z":
-00006ca0: 2230 2e30 3833 3422 2c0a 2020 2020 2020  "0.0834",.      
-00006cb0: 2020 2020 2020 2020 2020 226d 6268 223a            "mbh":
-00006cc0: 2237 2e33 3920 284c 3139 2922 2c0a 2020  "7.39 (L19)",.  
-00006cd0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00006ce0: 6167 6e74 6465 223a 352e 3732 362c 0a20  agntde":5.726,. 
-00006cf0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006d00: 636c 6173 7322 3a22 5444 453f 222c 0a20  class":"TDE?",. 
-00006d10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006d20: 6466 223a 302e 3238 2c0a 2020 2020 2020  df":0.28,.      
-00006d30: 2020 2020 2020 2020 2020 2264 665f 6522            "df_e"
-00006d40: 3a30 2e30 312c 0a20 2020 2020 2020 2020  :0.01,.         
-00006d50: 2020 2020 2020 2022 7261 223a 3138 312e         "ra":181.
-00006d60: 3039 3232 3335 3033 3634 2c0a 2020 2020  0922350364,.    
-00006d70: 2020 2020 2020 2020 2020 2020 2264 6563              "dec
-00006d80: 223a 2d31 2e33 3637 3538 3038 3831 380a  ":-1.3675808818.
-00006d90: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00006da0: 2020 2020 2020 2020 2020 2022 3530 223a             "50":
-00006db0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00006dc0: 2020 226e 616d 6522 3a22 4154 3230 3139    "name":"AT2019
-00006dd0: 6d73 7122 2c0a 2020 2020 2020 2020 2020  msq",.          
-00006de0: 2020 2020 2020 2274 7065 616b 223a 3538        "tpeak":58
-00006df0: 3739 312e 322c 0a20 2020 2020 2020 2020  791.2,.         
-00006e00: 2020 2020 2020 2022 7269 7365 7469 6d65         "risetime
-00006e10: 223a 2231 3337 2e39 222c 0a20 2020 2020  ":"137.9",.     
-00006e20: 2020 2020 2020 2020 2020 2022 6661 6465             "fade
-00006e30: 7469 6d65 223a 225c 7532 3031 3322 2c0a  time":"\u2013",.
-00006e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e50: 2264 665f 6f76 6572 5f72 6d73 223a 362e  "df_over_rms":6.
-00006e60: 342c 0a20 2020 2020 2020 2020 2020 2020  4,.             
-00006e70: 2020 2022 6466 5f72 6177 223a 2230 2e31     "df_raw":"0.1
-00006e80: 3620 5c75 3030 6231 2030 2e30 3122 2c0a  6 \u00b1 0.01",.
-00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ea0: 227a 223a 225c 7532 3031 3322 2c0a 2020  "z":"\u2013",.  
-00006eb0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-00006ec0: 6268 223a 225c 7532 3031 3322 2c0a 2020  bh":"\u2013",.  
-00006ed0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00006ee0: 6167 6e74 6465 223a 332e 3933 332c 0a20  agntde":3.933,. 
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006f00: 636c 6173 7322 3a22 5c75 3230 3133 222c  class":"\u2013",
-00006f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006f20: 2022 6466 223a 302e 3136 2c0a 2020 2020   "df":0.16,.    
-00006f30: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-00006f40: 6522 3a30 2e30 312c 0a20 2020 2020 2020  e":0.01,.       
-00006f50: 2020 2020 2020 2020 2022 7261 223a 342e           "ra":4.
-00006f60: 3138 342c 0a20 2020 2020 2020 2020 2020  184,.           
-00006f70: 2020 2020 2022 6465 6322 3a36 2e33 3830       "dec":6.380
-00006f80: 3038 390a 2020 2020 2020 2020 2020 2020  089.            
-00006f90: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-00006fa0: 3531 223a 7b0a 2020 2020 2020 2020 2020  51":{.          
-00006fb0: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
-00006fc0: 3230 3139 7170 7422 2c0a 2020 2020 2020  2019qpt",.      
-00006fd0: 2020 2020 2020 2020 2020 2274 7065 616b            "tpeak
-00006fe0: 223a 3538 3739 382e 332c 0a20 2020 2020  ":58798.3,.     
-00006ff0: 2020 2020 2020 2020 2020 2022 7269 7365             "rise
-00007000: 7469 6d65 223a 2234 342e 3522 2c0a 2020  time":"44.5",.  
-00007010: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-00007020: 6164 6574 696d 6522 3a22 3133 352e 3122  adetime":"135.1"
-00007030: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007040: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
-00007050: 3133 2e38 2c0a 2020 2020 2020 2020 2020  13.8,.          
-00007060: 2020 2020 2020 2264 665f 7261 7722 3a22        "df_raw":"
-00007070: 302e 3234 205c 7530 3062 3120 302e 3031  0.24 \u00b1 0.01
-00007080: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00007090: 2020 2022 7a22 3a22 302e 3234 3222 2c0a     "z":"0.242",.
-000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 226d 6268 223a 2236 2e39 3720 284c 3139  "mbh":"6.97 (L19
-000070c0: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
-000070d0: 2020 2020 2270 6167 6e74 6465 223a 302e      "pagntde":0.
-000070e0: 3335 352c 0a20 2020 2020 2020 2020 2020  355,.           
-000070f0: 2020 2020 2022 636c 6173 7322 3a22 5444       "class":"TD
-00007100: 453f 222c 0a20 2020 2020 2020 2020 2020  E?",.           
-00007110: 2020 2020 2022 6466 223a 302e 3234 2c0a       "df":0.24,.
-00007120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007130: 2264 665f 6522 3a30 2e30 312c 0a20 2020  "df_e":0.01,.   
-00007140: 2020 2020 2020 2020 2020 2020 2022 7261               "ra
-00007150: 223a 3132 302e 3335 3733 3735 2c0a 2020  ":120.357375,.  
-00007160: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00007170: 6563 223a 3234 2e39 3239 3433 390a 2020  ec":24.929439.  
-00007180: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00007190: 2020 2020 2020 2020 2022 3532 223a 7b0a           "52":{.
-000071a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071b0: 226e 616d 6522 3a22 4154 3230 3230 6166  "name":"AT2020af
-000071c0: 6164 222c 0a20 2020 2020 2020 2020 2020  ad",.           
-000071d0: 2020 2020 2022 7470 6561 6b22 3a35 3838       "tpeak":588
-000071e0: 3032 2e32 2c0a 2020 2020 2020 2020 2020  02.2,.          
-000071f0: 2020 2020 2020 2272 6973 6574 696d 6522        "risetime"
-00007200: 3a22 3737 2e31 222c 0a20 2020 2020 2020  :"77.1",.       
-00007210: 2020 2020 2020 2020 2022 6661 6465 7469           "fadeti
-00007220: 6d65 223a 2231 3235 2e35 222c 0a20 2020  me":"125.5",.   
-00007230: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00007240: 5f6f 7665 725f 726d 7322 3a33 2e37 2c0a  _over_rms":3.7,.
-00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007260: 2264 665f 7261 7722 3a22 302e 3038 205c  "df_raw":"0.08 \
-00007270: 7530 3062 3120 302e 3031 222c 0a20 2020  u00b1 0.01",.   
-00007280: 2020 2020 2020 2020 2020 2020 2022 7a22               "z"
-00007290: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-000072a0: 2020 2020 2020 2020 2020 2022 6d62 6822             "mbh"
-000072b0: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-000072c0: 2020 2020 2020 2020 2020 2022 7061 676e             "pagn
-000072d0: 7464 6522 3a35 2e32 3137 2c0a 2020 2020  tde":5.217,.    
-000072e0: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
-000072f0: 7373 223a 225c 7532 3031 3322 2c0a 2020  ss":"\u2013",.  
-00007300: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00007310: 6622 3a30 2e30 382c 0a20 2020 2020 2020  f":0.08,.       
-00007320: 2020 2020 2020 2020 2022 6466 5f65 223a           "df_e":
-00007330: 302e 3031 2c0a 2020 2020 2020 2020 2020  0.01,.          
-00007340: 2020 2020 2020 2272 6122 3a31 3033 2e38        "ra":103.8
-00007350: 3235 3330 3730 3831 372c 0a20 2020 2020  253070817,.     
-00007360: 2020 2020 2020 2020 2020 2022 6465 6322             "dec"
-00007370: 3a35 382e 3938 3436 3933 3438 3137 0a20  :58.9846934817. 
-00007380: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00007390: 2020 2020 2020 2020 2020 2235 3322 3a7b            "53":{
-000073a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000073b0: 2022 6e61 6d65 223a 2241 5432 3031 396d   "name":"AT2019m
-000073c0: 7373 222c 0a20 2020 2020 2020 2020 2020  ss",.           
-000073d0: 2020 2020 2022 7470 6561 6b22 3a35 3838       "tpeak":588
-000073e0: 3131 2e36 2c0a 2020 2020 2020 2020 2020  11.6,.          
-000073f0: 2020 2020 2020 2272 6973 6574 696d 6522        "risetime"
-00007400: 3a22 3335 2e32 222c 0a20 2020 2020 2020  :"35.2",.       
-00007410: 2020 2020 2020 2020 2022 6661 6465 7469           "fadeti
-00007420: 6d65 223a 2232 3039 2e37 222c 0a20 2020  me":"209.7",.   
-00007430: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00007440: 5f6f 7665 725f 726d 7322 3a32 302e 382c  _over_rms":20.8,
-00007450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007460: 2022 6466 5f72 6177 223a 2230 2e33 3820   "df_raw":"0.38 
-00007470: 5c75 3030 6231 2030 2e30 3122 2c0a 2020  \u00b1 0.01",.  
-00007480: 2020 2020 2020 2020 2020 2020 2020 227a                "z
-00007490: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
-000074a0: 2020 2020 2020 2020 2020 2020 226d 6268              "mbh
-000074b0: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
-000074c0: 2020 2020 2020 2020 2020 2020 2270 6167              "pag
-000074d0: 6e74 6465 223a 302e 3032 312c 0a20 2020  ntde":0.021,.   
-000074e0: 2020 2020 2020 2020 2020 2020 2022 636c               "cl
-000074f0: 6173 7322 3a22 5c75 3230 3133 222c 0a20  ass":"\u2013",. 
-00007500: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007510: 6466 223a 302e 3338 2c0a 2020 2020 2020  df":0.38,.      
-00007520: 2020 2020 2020 2020 2020 2264 665f 6522            "df_e"
-00007530: 3a30 2e30 312c 0a20 2020 2020 2020 2020  :0.01,.         
-00007540: 2020 2020 2020 2022 7261 223a 3230 372e         "ra":207.
-00007550: 3130 3234 3137 2c0a 2020 2020 2020 2020  102417,.        
-00007560: 2020 2020 2020 2020 2264 6563 223a 382e          "dec":8.
-00007570: 3532 3837 0a20 2020 2020 2020 2020 2020  5287.           
-00007580: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00007590: 2235 3422 3a7b 0a20 2020 2020 2020 2020  "54":{.         
-000075a0: 2020 2020 2020 2022 6e61 6d65 223a 2241         "name":"A
-000075b0: 5432 3031 3974 6868 222c 0a20 2020 2020  T2019thh",.     
-000075c0: 2020 2020 2020 2020 2020 2022 7470 6561             "tpea
-000075d0: 6b22 3a35 3838 3531 2e31 2c0a 2020 2020  k":58851.1,.    
-000075e0: 2020 2020 2020 2020 2020 2020 2272 6973              "ris
-000075f0: 6574 696d 6522 3a22 3130 342e 3722 2c0a  etime":"104.7",.
-00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007610: 2266 6164 6574 696d 6522 3a22 3433 332e  "fadetime":"433.
-00007620: 3822 2c0a 2020 2020 2020 2020 2020 2020  8",.            
-00007630: 2020 2020 2264 665f 6f76 6572 5f72 6d73      "df_over_rms
-00007640: 223a 3732 2e32 2c0a 2020 2020 2020 2020  ":72.2,.        
-00007650: 2020 2020 2020 2020 2264 665f 7261 7722          "df_raw"
-00007660: 3a22 312e 3735 205c 7530 3062 3120 302e  :"1.75 \u00b1 0.
-00007670: 3032 222c 0a20 2020 2020 2020 2020 2020  02",.           
-00007680: 2020 2020 2022 7a22 3a22 302e 3035 3036       "z":"0.0506
-00007690: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000076a0: 2020 2022 6d62 6822 3a22 5c75 3230 3133     "mbh":"\u2013
-000076b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000076c0: 2020 2022 7061 676e 7464 6522 3a30 2e30     "pagntde":0.0
-000076d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000076e0: 2020 2263 6c61 7373 223a 225c 7532 3031    "class":"\u201
-000076f0: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
-00007700: 2020 2020 2264 6622 3a31 2e37 352c 0a20      "df":1.75,. 
-00007710: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007720: 6466 5f65 223a 302e 3032 2c0a 2020 2020  df_e":0.02,.    
-00007730: 2020 2020 2020 2020 2020 2020 2272 6122              "ra"
-00007740: 3a33 3336 2e39 3933 3534 322c 0a20 2020  :336.993542,.   
-00007750: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00007760: 6322 3a31 382e 3332 3230 3639 0a20 2020  c":18.322069.   
-00007770: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00007780: 2020 2020 2020 2020 2235 3522 3a7b 0a20          "55":{. 
-00007790: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000077a0: 6e61 6d65 223a 2241 5432 3032 3161 6575  name":"AT2021aeu
-000077b0: 6922 2c0a 2020 2020 2020 2020 2020 2020  i",.            
-000077c0: 2020 2020 2274 7065 616b 223a 3538 3836      "tpeak":5886
-000077d0: 302e 332c 0a20 2020 2020 2020 2020 2020  0.3,.           
-000077e0: 2020 2020 2022 7269 7365 7469 6d65 223a       "risetime":
-000077f0: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
-00007800: 2020 2020 2020 2020 2020 2266 6164 6574            "fadet
-00007810: 696d 6522 3a22 3630 2e30 222c 0a20 2020  ime":"60.0",.   
-00007820: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00007830: 5f6f 7665 725f 726d 7322 3a36 2e32 2c0a  _over_rms":6.2,.
-00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007850: 2264 665f 7261 7722 3a22 302e 3439 205c  "df_raw":"0.49 \
-00007860: 7530 3062 3120 302e 3032 222c 0a20 2020  u00b1 0.02",.   
-00007870: 2020 2020 2020 2020 2020 2020 2022 7a22               "z"
-00007880: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-00007890: 2020 2020 2020 2020 2020 2022 6d62 6822             "mbh"
-000078a0: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
-000078b0: 2020 2020 2020 2020 2020 2022 7061 676e             "pagn
-000078c0: 7464 6522 3a34 2e32 352c 0a20 2020 2020  tde":4.25,.     
-000078d0: 2020 2020 2020 2020 2020 2022 636c 6173             "clas
-000078e0: 7322 3a22 5c75 3230 3133 222c 0a20 2020  s":"\u2013",.   
-000078f0: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00007900: 223a 302e 3439 2c0a 2020 2020 2020 2020  ":0.49,.        
-00007910: 2020 2020 2020 2020 2264 665f 6522 3a30          "df_e":0
-00007920: 2e30 322c 0a20 2020 2020 2020 2020 2020  .02,.           
-00007930: 2020 2020 2022 7261 223a 3132 302e 3038       "ra":120.08
-00007940: 3332 3130 3537 3635 2c0a 2020 2020 2020  32105765,.      
-00007950: 2020 2020 2020 2020 2020 2264 6563 223a            "dec":
-00007960: 3735 2e38 3233 3038 3134 3335 330a 2020  75.8230814353.  
-00007970: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00007980: 2020 2020 2020 2020 2022 3536 223a 7b0a           "56":{.
-00007990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079a0: 226e 616d 6522 3a22 4154 3230 3230 6166  "name":"AT2020af
-000079b0: 6165 222c 0a20 2020 2020 2020 2020 2020  ae",.           
-000079c0: 2020 2020 2022 7470 6561 6b22 3a35 3838       "tpeak":588
-000079d0: 3637 2e32 2c0a 2020 2020 2020 2020 2020  67.2,.          
-000079e0: 2020 2020 2020 2272 6973 6574 696d 6522        "risetime"
-000079f0: 3a22 3330 2e32 222c 0a20 2020 2020 2020  :"30.2",.       
-00007a00: 2020 2020 2020 2020 2022 6661 6465 7469           "fadeti
-00007a10: 6d65 223a 2234 322e 3022 2c0a 2020 2020  me":"42.0",.    
-00007a20: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-00007a30: 6f76 6572 5f72 6d73 223a 352e 322c 0a20  over_rms":5.2,. 
-00007a40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007a50: 6466 5f72 6177 223a 2230 2e33 3520 5c75  df_raw":"0.35 \u
-00007a60: 3030 6231 2030 2e30 3222 2c0a 2020 2020  00b1 0.02",.    
-00007a70: 2020 2020 2020 2020 2020 2020 227a 223a              "z":
-00007a80: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
-00007a90: 2020 2020 2020 2020 2020 226d 6268 223a            "mbh":
-00007aa0: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
-00007ab0: 2020 2020 2020 2020 2020 2270 6167 6e74            "pagnt
-00007ac0: 6465 223a 352e 3538 352c 0a20 2020 2020  de":5.585,.     
-00007ad0: 2020 2020 2020 2020 2020 2022 636c 6173             "clas
-00007ae0: 7322 3a22 5c75 3230 3133 222c 0a20 2020  s":"\u2013",.   
-00007af0: 2020 2020 2020 2020 2020 2020 2022 6466               "df
-00007b00: 223a 302e 3335 2c0a 2020 2020 2020 2020  ":0.35,.        
-00007b10: 2020 2020 2020 2020 2264 665f 6522 3a30          "df_e":0
-00007b20: 2e30 322c 0a20 2020 2020 2020 2020 2020  .02,.           
-00007b30: 2020 2020 2022 7261 223a 3736 2e32 3333       "ra":76.233
-00007b40: 3038 3736 3839 372c 0a20 2020 2020 2020  0876897,.       
-00007b50: 2020 2020 2020 2020 2022 6465 6322 3a39           "dec":9
-00007b60: 2e31 3534 3138 3030 3331 0a20 2020 2020  .154180031.     
-00007b70: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00007b80: 2020 2020 2020 2235 3722 3a7b 0a20 2020        "57":{.   
-00007b90: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-00007ba0: 6d65 223a 2241 5432 3032 306d 7722 2c0a  me":"AT2020mw",.
-00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bc0: 2274 7065 616b 223a 3538 3836 372e 332c  "tpeak":58867.3,
-00007bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007be0: 2022 7269 7365 7469 6d65 223a 2231 322e   "risetime":"12.
-00007bf0: 3622 2c0a 2020 2020 2020 2020 2020 2020  6",.            
-00007c00: 2020 2020 2266 6164 6574 696d 6522 3a22      "fadetime":"
-00007c10: 3332 2e31 222c 0a20 2020 2020 2020 2020  32.1",.         
-00007c20: 2020 2020 2020 2022 6466 5f6f 7665 725f         "df_over_
-00007c30: 726d 7322 3a36 2e38 2c0a 2020 2020 2020  rms":6.8,.      
-00007c40: 2020 2020 2020 2020 2020 2264 665f 7261            "df_ra
-00007c50: 7722 3a22 302e 3132 205c 7530 3062 3120  w":"0.12 \u00b1 
-00007c60: 302e 3031 222c 0a20 2020 2020 2020 2020  0.01",.         
-00007c70: 2020 2020 2020 2022 7a22 3a22 5c75 3230         "z":"\u20
-00007c80: 3133 222c 0a20 2020 2020 2020 2020 2020  13",.           
-00007c90: 2020 2020 2022 6d62 6822 3a22 5c75 3230       "mbh":"\u20
-00007ca0: 3133 222c 0a20 2020 2020 2020 2020 2020  13",.           
-00007cb0: 2020 2020 2022 7061 676e 7464 6522 3a33       "pagntde":3
-00007cc0: 2e34 3134 2c0a 2020 2020 2020 2020 2020  .414,.          
-00007cd0: 2020 2020 2020 2263 6c61 7373 223a 225c        "class":"\
-00007ce0: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
-00007cf0: 2020 2020 2020 2020 2264 6622 3a30 2e31          "df":0.1
-00007d00: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-00007d10: 2020 2022 6466 5f65 223a 302e 3031 2c0a     "df_e":0.01,.
-00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d30: 2272 6122 3a31 3232 2e36 3936 3938 3236  "ra":122.6969826
-00007d40: 3436 2c0a 2020 2020 2020 2020 2020 2020  46,.            
-00007d50: 2020 2020 2264 6563 223a 3131 2e35 3231      "dec":11.521
-00007d60: 3133 3030 3337 330a 2020 2020 2020 2020  1300373.        
-00007d70: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00007d80: 2020 2022 3538 223a 7b0a 2020 2020 2020     "58":{.      
-00007d90: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-00007da0: 3a22 4154 3230 3230 6971 222c 0a20 2020  :"AT2020iq",.   
-00007db0: 2020 2020 2020 2020 2020 2020 2022 7470               "tp
-00007dc0: 6561 6b22 3a35 3838 3738 2e31 2c0a 2020  eak":58878.1,.  
-00007dd0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00007de0: 6973 6574 696d 6522 3a22 3232 2e37 222c  isetime":"22.7",
-00007df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007e00: 2022 6661 6465 7469 6d65 223a 2237 312e   "fadetime":"71.
-00007e10: 3522 2c0a 2020 2020 2020 2020 2020 2020  5",.            
-00007e20: 2020 2020 2264 665f 6f76 6572 5f72 6d73      "df_over_rms
-00007e30: 223a 3234 2e35 2c0a 2020 2020 2020 2020  ":24.5,.        
-00007e40: 2020 2020 2020 2020 2264 665f 7261 7722          "df_raw"
-00007e50: 3a22 302e 3435 205c 7530 3062 3120 302e  :"0.45 \u00b1 0.
-00007e60: 3031 222c 0a20 2020 2020 2020 2020 2020  01",.           
-00007e70: 2020 2020 2022 7a22 3a22 302e 3039 3622       "z":"0.096"
-00007e80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007e90: 2020 226d 6268 223a 2236 2e33 3720 2856    "mbh":"6.37 (V
-00007ea0: 3231 2922 2c0a 2020 2020 2020 2020 2020  21)",.          
-00007eb0: 2020 2020 2020 2270 6167 6e74 6465 223a        "pagntde":
-00007ec0: 302e 3030 332c 0a20 2020 2020 2020 2020  0.003,.         
-00007ed0: 2020 2020 2020 2022 636c 6173 7322 3a22         "class":"
-00007ee0: 5444 453f 222c 0a20 2020 2020 2020 2020  TDE?",.         
-00007ef0: 2020 2020 2020 2022 6466 223a 302e 3435         "df":0.45
-00007f00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007f10: 2020 2264 665f 6522 3a30 2e30 312c 0a20    "df_e":0.01,. 
-00007f20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007f30: 7261 223a 3433 2e38 3332 3136 372c 0a20  ra":43.832167,. 
-00007f40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007f50: 6465 6322 3a2d 3131 2e34 3133 3531 310a  dec":-11.413511.
-00007f60: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00007f70: 2020 2020 2020 2020 2020 2022 3539 223a             "59":
-00007f80: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00007f90: 2020 226e 616d 6522 3a22 4154 3230 3139    "name":"AT2019
-00007fa0: 7867 6722 2c0a 2020 2020 2020 2020 2020  xgg",.          
-00007fb0: 2020 2020 2020 2274 7065 616b 223a 3538        "tpeak":58
-00007fc0: 3839 312e 322c 0a20 2020 2020 2020 2020  891.2,.         
-00007fd0: 2020 2020 2020 2022 7269 7365 7469 6d65         "risetime
-00007fe0: 223a 2238 312e 3622 2c0a 2020 2020 2020  ":"81.6",.      
-00007ff0: 2020 2020 2020 2020 2020 2266 6164 6574            "fadet
-00008000: 696d 6522 3a22 3434 362e 3222 2c0a 2020  ime":"446.2",.  
-00008010: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00008020: 665f 6f76 6572 5f72 6d73 223a 342e 342c  f_over_rms":4.4,
-00008030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008040: 2022 6466 5f72 6177 223a 2230 2e31 3320   "df_raw":"0.13 
-00008050: 5c75 3030 6231 2030 2e30 3122 2c0a 2020  \u00b1 0.01",.  
-00008060: 2020 2020 2020 2020 2020 2020 2020 227a                "z
-00008070: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
-00008080: 2020 2020 2020 2020 2020 2020 226d 6268              "mbh
-00008090: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
-000080a0: 2020 2020 2020 2020 2020 2020 2270 6167              "pag
-000080b0: 6e74 6465 223a 362e 3039 312c 0a20 2020  ntde":6.091,.   
-000080c0: 2020 2020 2020 2020 2020 2020 2022 636c               "cl
-000080d0: 6173 7322 3a22 5c75 3230 3133 222c 0a20  ass":"\u2013",. 
-000080e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000080f0: 6466 223a 302e 3133 2c0a 2020 2020 2020  df":0.13,.      
-00008100: 2020 2020 2020 2020 2020 2264 665f 6522            "df_e"
-00008110: 3a30 2e30 312c 0a20 2020 2020 2020 2020  :0.01,.         
-00008120: 2020 2020 2020 2022 7261 223a 3136 322e         "ra":162.
-00008130: 3238 3432 3430 382c 0a20 2020 2020 2020  2842408,.       
-00008140: 2020 2020 2020 2020 2022 6465 6322 3a33           "dec":3
-00008150: 372e 3232 3131 3030 370a 2020 2020 2020  7.2211007.      
-00008160: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00008170: 2020 2020 2022 3630 223a 7b0a 2020 2020       "60":{.    
-00008180: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
-00008190: 6522 3a22 4154 3230 3230 6174 7122 2c0a  e":"AT2020atq",.
-000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081b0: 2274 7065 616b 223a 3538 3930 332e 322c  "tpeak":58903.2,
-000081c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000081d0: 2022 7269 7365 7469 6d65 223a 2233 392e   "risetime":"39.
-000081e0: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
-000081f0: 2020 2020 2266 6164 6574 696d 6522 3a22      "fadetime":"
-00008200: 3230 352e 3522 2c0a 2020 2020 2020 2020  205.5",.        
-00008210: 2020 2020 2020 2020 2264 665f 6f76 6572          "df_over
-00008220: 5f72 6d73 223a 3230 2e38 2c0a 2020 2020  _rms":20.8,.    
-00008230: 2020 2020 2020 2020 2020 2020 2264 665f              "df_
-00008240: 7261 7722 3a22 302e 3636 205c 7530 3062  raw":"0.66 \u00b
-00008250: 3120 302e 3031 222c 0a20 2020 2020 2020  1 0.01",.       
-00008260: 2020 2020 2020 2020 2022 7a22 3a22 5c75           "z":"\u
-00008270: 3230 3133 222c 0a20 2020 2020 2020 2020  2013",.         
-00008280: 2020 2020 2020 2022 6d62 6822 3a22 5c75         "mbh":"\u
-00008290: 3230 3133 222c 0a20 2020 2020 2020 2020  2013",.         
-000082a0: 2020 2020 2020 2022 7061 676e 7464 6522         "pagntde"
-000082b0: 3a30 2e30 322c 0a20 2020 2020 2020 2020  :0.02,.         
-000082c0: 2020 2020 2020 2022 636c 6173 7322 3a22         "class":"
-000082d0: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
-000082e0: 2020 2020 2020 2020 2022 6466 223a 302e           "df":0.
-000082f0: 3636 2c0a 2020 2020 2020 2020 2020 2020  66,.            
-00008300: 2020 2020 2264 665f 6522 3a30 2e30 312c      "df_e":0.01,
-00008310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008320: 2022 7261 223a 3130 322e 3332 3335 3338   "ra":102.323538
-00008330: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00008340: 2020 2022 6465 6322 3a36 322e 3531 3334     "dec":62.5134
-00008350: 3030 350a 2020 2020 2020 2020 2020 2020  005.            
-00008360: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-00008370: 3631 223a 7b0a 2020 2020 2020 2020 2020  61":{.          
-00008380: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
-00008390: 3230 3231 6165 756a 222c 0a20 2020 2020  2021aeuj",.     
-000083a0: 2020 2020 2020 2020 2020 2022 7470 6561             "tpea
-000083b0: 6b22 3a35 3839 3734 2e32 2c0a 2020 2020  k":58974.2,.    
-000083c0: 2020 2020 2020 2020 2020 2020 2272 6973              "ris
-000083d0: 6574 696d 6522 3a22 3739 2e30 222c 0a20  etime":"79.0",. 
-000083e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000083f0: 6661 6465 7469 6d65 223a 2232 3333 2e35  fadetime":"233.5
-00008400: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00008410: 2020 2022 6466 5f6f 7665 725f 726d 7322     "df_over_rms"
-00008420: 3a31 382e 312c 0a20 2020 2020 2020 2020  :18.1,.         
-00008430: 2020 2020 2020 2022 6466 5f72 6177 223a         "df_raw":
-00008440: 2230 2e32 3020 5c75 3030 6231 2030 2e30  "0.20 \u00b1 0.0
-00008450: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-00008460: 2020 2020 227a 223a 2230 2e36 3935 222c      "z":"0.695",
-00008470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008480: 2022 6d62 6822 3a22 5c75 3230 3133 222c   "mbh":"\u2013",
-00008490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000084a0: 2022 7061 676e 7464 6522 3a30 2e30 3731   "pagntde":0.071
-000084b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000084c0: 2020 2263 6c61 7373 223a 225c 7532 3031    "class":"\u201
-000084d0: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
-000084e0: 2020 2020 2264 6622 3a30 2e32 2c0a 2020      "df":0.2,.  
-000084f0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00008500: 665f 6522 3a30 2e30 312c 0a20 2020 2020  f_e":0.01,.     
-00008510: 2020 2020 2020 2020 2020 2022 7261 223a             "ra":
-00008520: 3133 372e 3130 3732 3034 3335 3331 2c0a  137.1072043531,.
-00008530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008540: 2264 6563 223a 3432 2e38 3934 3830 3139  "dec":42.8948019
-00008550: 3036 360a 2020 2020 2020 2020 2020 2020  066.            
-00008560: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-00008570: 3632 223a 7b0a 2020 2020 2020 2020 2020  62":{.          
-00008580: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
-00008590: 3230 3230 686c 6522 2c0a 2020 2020 2020  2020hle",.      
-000085a0: 2020 2020 2020 2020 2020 2274 7065 616b            "tpeak
-000085b0: 223a 3538 3937 382e 332c 0a20 2020 2020  ":58978.3,.     
-000085c0: 2020 2020 2020 2020 2020 2022 7269 7365             "rise
-000085d0: 7469 6d65 223a 2233 322e 3722 2c0a 2020  time":"32.7",.  
-000085e0: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-000085f0: 6164 6574 696d 6522 3a22 3632 2e39 222c  adetime":"62.9",
-00008600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008610: 2022 6466 5f6f 7665 725f 726d 7322 3a32   "df_over_rms":2
-00008620: 312e 302c 0a20 2020 2020 2020 2020 2020  1.0,.           
-00008630: 2020 2020 2022 6466 5f72 6177 223a 2230       "df_raw":"0
-00008640: 2e33 3320 5c75 3030 6231 2030 2e30 3122  .33 \u00b1 0.01"
-00008650: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008660: 2020 227a 223a 2230 2e31 3033 222c 0a20    "z":"0.103",. 
-00008670: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00008680: 6d62 6822 3a22 362e 3430 2028 4632 3029  mbh":"6.40 (F20)
-00008690: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000086a0: 2020 2022 7061 676e 7464 6522 3a30 2e30     "pagntde":0.0
-000086b0: 3138 2c0a 2020 2020 2020 2020 2020 2020  18,.            
-000086c0: 2020 2020 2263 6c61 7373 223a 2254 4445      "class":"TDE
-000086d0: 3f22 2c0a 2020 2020 2020 2020 2020 2020  ?",.            
-000086e0: 2020 2020 2264 6622 3a30 2e33 332c 0a20      "df":0.33,. 
-000086f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00008700: 6466 5f65 223a 302e 3031 2c0a 2020 2020  df_e":0.01,.    
-00008710: 2020 2020 2020 2020 2020 2020 2272 6122              "ra"
-00008720: 3a31 3636 2e39 3238 3632 3731 2c0a 2020  :166.9286271,.  
-00008730: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00008740: 6563 223a 3734 2e36 3333 3933 3232 350a  ec":74.63393225.
-00008750: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00008760: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00008770: 5f64 6620 3d20 7064 2e44 6174 6146 7261  _df = pd.DataFra
-00008780: 6d65 2e66 726f 6d5f 6469 6374 285f 7361  me.from_dict(_sa
-00008790: 6d70 6c65 2c20 6f72 6965 6e74 3d22 696e  mple, orient="in
-000087a0: 6465 7822 290a 2020 2020 2020 2020 5f64  dex").        _d
-000087b0: 662e 696e 6465 7820 3d20 5f64 662e 696e  f.index = _df.in
-000087c0: 6465 782e 6173 7479 7065 2869 6e74 290a  dex.astype(int).
-000087d0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-000087e0: 6466 0a                                  df.
+00000000: 7b0a 2020 2020 2230 223a 7b0a 2020 2020  {.    "0":{.    
+00000010: 2020 2020 226e 616d 6522 3a22 4154 3230      "name":"AT20
+00000020: 3139 6473 6722 2c0a 2020 2020 2020 2020  19dsg",.        
+00000030: 2274 7065 616b 223a 3538 3632 302e 322c  "tpeak":58620.2,
+00000040: 0a20 2020 2020 2020 2022 7269 7365 7469  .        "riseti
+00000050: 6d65 223a 2233 322e 3122 2c0a 2020 2020  me":"32.1",.    
+00000060: 2020 2020 2266 6164 6574 696d 6522 3a22      "fadetime":"
+00000070: 3831 2e39 222c 0a20 2020 2020 2020 2022  81.9",.        "
+00000080: 6466 5f6f 7665 725f 726d 7322 3a39 322e  df_over_rms":92.
+00000090: 322c 0a20 2020 2020 2020 2022 6466 5f72  2,.        "df_r
+000000a0: 6177 223a 2231 2e35 3820 5c75 3030 6231  aw":"1.58 \u00b1
+000000b0: 2030 2e30 3222 2c0a 2020 2020 2020 2020   0.02",.        
+000000c0: 227a 223a 2230 2e30 3531 3222 2c0a 2020  "z":"0.0512",.  
+000000d0: 2020 2020 2020 226d 6268 223a 2236 2e37        "mbh":"6.7
+000000e0: 3420 2843 3231 2922 2c0a 2020 2020 2020  4 (C21)",.      
+000000f0: 2020 2270 6167 6e74 6465 223a 302e 302c    "pagntde":0.0,
+00000100: 0a20 2020 2020 2020 2022 636c 6173 7322  .        "class"
+00000110: 3a22 5444 4522 2c0a 2020 2020 2020 2020  :"TDE",.        
+00000120: 2264 6622 3a31 2e35 382c 0a20 2020 2020  "df":1.58,.     
+00000130: 2020 2022 6466 5f65 223a 302e 3032 2c0a     "df_e":0.02,.
+00000140: 2020 2020 2020 2020 2272 6122 3a33 3134          "ra":314
+00000150: 2e32 3632 3339 3236 2c0a 2020 2020 2020  .2623926,.      
+00000160: 2020 2264 6563 223a 3134 2e32 3034 3430    "dec":14.20440
+00000170: 3633 2c0a 2020 2020 2020 2020 2241 6c6c  63,.        "All
+00000180: 5749 5345 5f69 6422 3a33 3135 3031 3133  WISE_id":3150113
+00000190: 3630 3133 3531 3036 3335 3734 2c0a 2020  601351063574,.  
+000001a0: 2020 2020 2020 2273 6570 5f74 6f5f 5749        "sep_to_WI
+000001b0: 5345 5f73 6f75 7263 6522 3a30 2e34 3136  SE_source":0.416
+000001c0: 3832 352c 0a20 2020 2020 2020 2022 7731  825,.        "w1
+000001d0: 6d70 726f 223a 3133 2e32 3732 2c0a 2020  mpro":13.272,.  
+000001e0: 2020 2020 2020 2277 326d 7072 6f22 3a31        "w2mpro":1
+000001f0: 332e 3235 320a 2020 2020 7d2c 0a20 2020  3.252.    },.   
+00000200: 2022 3122 3a7b 0a20 2020 2020 2020 2022   "1":{.        "
+00000210: 6e61 6d65 223a 2241 5432 3031 3966 6472  name":"AT2019fdr
+00000220: 222c 0a20 2020 2020 2020 2022 7470 6561  ",.        "tpea
+00000230: 6b22 3a35 3836 3732 2e35 2c0a 2020 2020  k":58672.5,.    
+00000240: 2020 2020 2272 6973 6574 696d 6522 3a22      "risetime":"
+00000250: 3330 2e38 222c 0a20 2020 2020 2020 2022  30.8",.        "
+00000260: 6661 6465 7469 6d65 223a 2233 3336 2e36  fadetime":"336.6
+00000270: 222c 0a20 2020 2020 2020 2022 6466 5f6f  ",.        "df_o
+00000280: 7665 725f 726d 7322 3a33 392e 322c 0a20  ver_rms":39.2,. 
+00000290: 2020 2020 2020 2022 6466 5f72 6177 223a         "df_raw":
+000002a0: 2230 2e37 3120 5c75 3030 6231 2030 2e30  "0.71 \u00b1 0.0
+000002b0: 3722 2c0a 2020 2020 2020 2020 227a 223a  7",.        "z":
+000002c0: 2230 2e32 3636 3622 2c0a 2020 2020 2020  "0.2666",.      
+000002d0: 2020 226d 6268 223a 2237 2e31 3020 2846    "mbh":"7.10 (F
+000002e0: 3230 2922 2c0a 2020 2020 2020 2020 2270  20)",.        "p
+000002f0: 6167 6e74 6465 223a 302e 302c 0a20 2020  agntde":0.0,.   
+00000300: 2020 2020 2022 636c 6173 7322 3a22 5444       "class":"TD
+00000310: 453f 222c 0a20 2020 2020 2020 2022 6466  E?",.        "df
+00000320: 223a 302e 3731 2c0a 2020 2020 2020 2020  ":0.71,.        
+00000330: 2264 665f 6522 3a30 2e30 372c 0a20 2020  "df_e":0.07,.   
+00000340: 2020 2020 2022 7261 223a 3235 372e 3237       "ra":257.27
+00000350: 3835 3738 3933 352c 0a20 2020 2020 2020  8578935,.       
+00000360: 2022 6465 6322 3a32 362e 3835 3536 3934   "dec":26.855694
+00000370: 3636 3332 2c0a 2020 2020 2020 2020 2241  6632,.        "A
+00000380: 6c6c 5749 5345 5f69 6422 3a22 222c 0a20  llWISE_id":"",. 
+00000390: 2020 2020 2020 2022 7365 705f 746f 5f57         "sep_to_W
+000003a0: 4953 455f 736f 7572 6365 223a 6e75 6c6c  ISE_source":null
+000003b0: 2c0a 2020 2020 2020 2020 2277 316d 7072  ,.        "w1mpr
+000003c0: 6f22 3a6e 756c 6c2c 0a20 2020 2020 2020  o":null,.       
+000003d0: 2022 7732 6d70 726f 223a 6e75 6c6c 0a20   "w2mpro":null. 
+000003e0: 2020 207d 2c0a 2020 2020 2232 223a 7b0a     },.    "2":{.
+000003f0: 2020 2020 2020 2020 226e 616d 6522 3a22          "name":"
+00000400: 4154 3230 3139 6161 6c63 222c 0a20 2020  AT2019aalc",.   
+00000410: 2020 2020 2022 7470 6561 6b22 3a35 3836       "tpeak":586
+00000420: 3538 2e32 2c0a 2020 2020 2020 2020 2272  58.2,.        "r
+00000430: 6973 6574 696d 6522 3a22 3439 2e30 222c  isetime":"49.0",
+00000440: 0a20 2020 2020 2020 2022 6661 6465 7469  .        "fadeti
+00000450: 6d65 223a 2231 3637 2e37 222c 0a20 2020  me":"167.7",.   
+00000460: 2020 2020 2022 6466 5f6f 7665 725f 726d       "df_over_rm
+00000470: 7322 3a31 352e 372c 0a20 2020 2020 2020  s":15.7,.       
+00000480: 2022 6466 5f72 6177 223a 2231 312e 3133   "df_raw":"11.13
+00000490: 205c 7530 3062 3120 302e 3130 222c 0a20   \u00b1 0.10",. 
+000004a0: 2020 2020 2020 2022 7a22 3a22 302e 3033         "z":"0.03
+000004b0: 3536 222c 0a20 2020 2020 2020 2022 6d62  56",.        "mb
+000004c0: 6822 3a22 372e 3233 2028 4c31 3929 222c  h":"7.23 (L19)",
+000004d0: 0a20 2020 2020 2020 2022 7061 676e 7464  .        "pagntd
+000004e0: 6522 3a30 2e31 3834 2c0a 2020 2020 2020  e":0.184,.      
+000004f0: 2020 2263 6c61 7373 223a 2254 4445 3f22    "class":"TDE?"
+00000500: 2c0a 2020 2020 2020 2020 2264 6622 3a31  ,.        "df":1
+00000510: 312e 3133 2c0a 2020 2020 2020 2020 2264  1.13,.        "d
+00000520: 665f 6522 3a30 2e31 2c0a 2020 2020 2020  f_e":0.1,.      
+00000530: 2020 2272 6122 3a32 3331 2e30 3639 3433    "ra":231.06943
+00000540: 352c 0a20 2020 2020 2020 2022 6465 6322  5,.        "dec"
+00000550: 3a34 2e38 3535 3239 332c 0a20 2020 2020  :4.855293,.     
+00000560: 2020 2022 416c 6c57 4953 455f 6964 223a     "AllWISE_id":
+00000570: 3233 3038 3130 3435 3031 3335 3130 3338  2308104501351038
+00000580: 3233 312c 0a20 2020 2020 2020 2022 7365  231,.        "se
+00000590: 705f 746f 5f57 4953 455f 736f 7572 6365  p_to_WISE_source
+000005a0: 223a 302e 3034 3134 3238 2c0a 2020 2020  ":0.041428,.    
+000005b0: 2020 2020 2277 316d 7072 6f22 3a31 312e      "w1mpro":11.
+000005c0: 3132 352c 0a20 2020 2020 2020 2022 7732  125,.        "w2
+000005d0: 6d70 726f 223a 3130 2e35 3133 0a20 2020  mpro":10.513.   
+000005e0: 207d 2c0a 2020 2020 2233 223a 7b0a 2020   },.    "3":{.  
+000005f0: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
+00000600: 3230 3138 6479 6b22 2c0a 2020 2020 2020  2018dyk",.      
+00000610: 2020 2274 7065 616b 223a 3538 3236 312e    "tpeak":58261.
+00000620: 342c 0a20 2020 2020 2020 2022 7269 7365  4,.        "rise
+00000630: 7469 6d65 223a 2236 302e 3022 2c0a 2020  time":"60.0",.  
+00000640: 2020 2020 2020 2266 6164 6574 696d 6522        "fadetime"
+00000650: 3a22 3334 322e 3022 2c0a 2020 2020 2020  :"342.0",.      
+00000660: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
+00000670: 3233 2e38 2c0a 2020 2020 2020 2020 2264  23.8,.        "d
+00000680: 665f 7261 7722 3a22 312e 3431 205c 7530  f_raw":"1.41 \u0
+00000690: 3062 3120 302e 3033 222c 0a20 2020 2020  0b1 0.03",.     
+000006a0: 2020 2022 7a22 3a22 302e 3033 3637 222c     "z":"0.0367",
+000006b0: 0a20 2020 2020 2020 2022 6d62 6822 3a22  .        "mbh":"
+000006c0: 352e 3530 2028 4631 3929 222c 0a20 2020  5.50 (F19)",.   
+000006d0: 2020 2020 2022 7061 676e 7464 6522 3a30       "pagntde":0
+000006e0: 2e30 3035 2c0a 2020 2020 2020 2020 2263  .005,.        "c
+000006f0: 6c61 7373 223a 2254 4445 3f22 2c0a 2020  lass":"TDE?",.  
+00000700: 2020 2020 2020 2264 6622 3a31 2e34 312c        "df":1.41,
+00000710: 0a20 2020 2020 2020 2022 6466 5f65 223a  .        "df_e":
+00000720: 302e 3033 2c0a 2020 2020 2020 2020 2272  0.03,.        "r
+00000730: 6122 3a32 3333 2e32 3833 3339 3535 2c0a  a":233.2833955,.
+00000740: 2020 2020 2020 2020 2264 6563 223a 3434          "dec":44
+00000750: 2e35 3335 3631 3232 2c0a 2020 2020 2020  .5356122,.      
+00000760: 2020 2241 6c6c 5749 5345 5f69 6422 3a32    "AllWISE_id":2
+00000770: 3333 3031 3433 3930 3133 3531 3035 3438  3301439013510548
+00000780: 3736 2c0a 2020 2020 2020 2020 2273 6570  76,.        "sep
+00000790: 5f74 6f5f 5749 5345 5f73 6f75 7263 6522  _to_WISE_source"
+000007a0: 3a30 2e32 3137 3833 2c0a 2020 2020 2020  :0.21783,.      
+000007b0: 2020 2277 316d 7072 6f22 3a31 312e 3937    "w1mpro":11.97
+000007c0: 352c 0a20 2020 2020 2020 2022 7732 6d70  5,.        "w2mp
+000007d0: 726f 223a 3131 2e39 350a 2020 2020 7d2c  ro":11.95.    },
+000007e0: 0a20 2020 2022 3422 3a7b 0a20 2020 2020  .    "4":{.     
+000007f0: 2020 2022 6e61 6d65 223a 2241 5432 3031     "name":"AT201
+00000800: 3961 616d 6522 2c0a 2020 2020 2020 2020  9aame",.        
+00000810: 2274 7065 616b 223a 3538 3336 332e 322c  "tpeak":58363.2,
+00000820: 0a20 2020 2020 2020 2022 7269 7365 7469  .        "riseti
+00000830: 6d65 223a 225c 7532 3031 3322 2c0a 2020  me":"\u2013",.  
+00000840: 2020 2020 2020 2266 6164 6574 696d 6522        "fadetime"
+00000850: 3a22 3133 382e 3022 2c0a 2020 2020 2020  :"138.0",.      
+00000860: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
+00000870: 3132 2e33 2c0a 2020 2020 2020 2020 2264  12.3,.        "d
+00000880: 665f 7261 7722 3a22 302e 3138 205c 7530  f_raw":"0.18 \u0
+00000890: 3062 3120 302e 3031 222c 0a20 2020 2020  0b1 0.01",.     
+000008a0: 2020 2022 7a22 3a22 5c75 3230 3133 222c     "z":"\u2013",
+000008b0: 0a20 2020 2020 2020 2022 6d62 6822 3a22  .        "mbh":"
+000008c0: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
+000008d0: 2022 7061 676e 7464 6522 3a30 2e35 3537   "pagntde":0.557
+000008e0: 2c0a 2020 2020 2020 2020 2263 6c61 7373  ,.        "class
+000008f0: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
+00000900: 2020 2020 2264 6622 3a30 2e31 382c 0a20      "df":0.18,. 
+00000910: 2020 2020 2020 2022 6466 5f65 223a 302e         "df_e":0.
+00000920: 3031 2c0a 2020 2020 2020 2020 2272 6122  01,.        "ra"
+00000930: 3a32 3135 2e30 3531 3831 3835 3238 362c  :215.0518185286,
+00000940: 0a20 2020 2020 2020 2022 6465 6322 3a33  .        "dec":3
+00000950: 312e 3839 3431 3832 3635 2c0a 2020 2020  1.89418265,.    
+00000960: 2020 2020 2241 6c6c 5749 5345 5f69 6422      "AllWISE_id"
+00000970: 3a32 3135 3231 3331 3830 3133 3531 3033  :215213180135103
+00000980: 3530 3935 2c0a 2020 2020 2020 2020 2273  5095,.        "s
+00000990: 6570 5f74 6f5f 5749 5345 5f73 6f75 7263  ep_to_WISE_sourc
+000009a0: 6522 3a30 2e31 3232 3339 322c 0a20 2020  e":0.122392,.   
+000009b0: 2020 2020 2022 7731 6d70 726f 223a 3136       "w1mpro":16
+000009c0: 2e31 3435 2c0a 2020 2020 2020 2020 2277  .145,.        "w
+000009d0: 326d 7072 6f22 3a31 352e 3731 380a 2020  2mpro":15.718.  
+000009e0: 2020 7d2c 0a20 2020 2022 3522 3a7b 0a20    },.    "5":{. 
+000009f0: 2020 2020 2020 2022 6e61 6d65 223a 2241         "name":"A
+00000a00: 5432 3031 386c 7a73 222c 0a20 2020 2020  T2018lzs",.     
+00000a10: 2020 2022 7470 6561 6b22 3a35 3833 3738     "tpeak":58378
+00000a20: 2e32 2c0a 2020 2020 2020 2020 2272 6973  .2,.        "ris
+00000a30: 6574 696d 6522 3a22 3133 342e 3022 2c0a  etime":"134.0",.
+00000a40: 2020 2020 2020 2020 2266 6164 6574 696d          "fadetim
+00000a50: 6522 3a22 3135 2e35 222c 0a20 2020 2020  e":"15.5",.     
+00000a60: 2020 2022 6466 5f6f 7665 725f 726d 7322     "df_over_rms"
+00000a70: 3a33 2e33 2c0a 2020 2020 2020 2020 2264  :3.3,.        "d
+00000a80: 665f 7261 7722 3a22 302e 3033 205c 7530  f_raw":"0.03 \u0
+00000a90: 3062 3120 302e 3031 222c 0a20 2020 2020  0b1 0.01",.     
+00000aa0: 2020 2022 7a22 3a22 5c75 3230 3133 222c     "z":"\u2013",
+00000ab0: 0a20 2020 2020 2020 2022 6d62 6822 3a22  .        "mbh":"
+00000ac0: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
+00000ad0: 2022 7061 676e 7464 6522 3a34 2e31 3434   "pagntde":4.144
+00000ae0: 2c0a 2020 2020 2020 2020 2263 6c61 7373  ,.        "class
+00000af0: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
+00000b00: 2020 2020 2264 6622 3a30 2e30 332c 0a20      "df":0.03,. 
+00000b10: 2020 2020 2020 2022 6466 5f65 223a 302e         "df_e":0.
+00000b20: 3031 2c0a 2020 2020 2020 2020 2272 6122  01,.        "ra"
+00000b30: 3a32 3638 2e32 3333 3232 3835 3838 392c  :268.2332285889,
+00000b40: 0a20 2020 2020 2020 2022 6465 6322 3a35  .        "dec":5
+00000b50: 382e 3633 3634 3432 3835 3131 2c0a 2020  8.6364428511,.  
+00000b60: 2020 2020 2020 2241 6c6c 5749 5345 5f69        "AllWISE_i
+00000b70: 6422 3a32 3637 3831 3539 3030 3133 3531  d":2678159001351
+00000b80: 3032 3034 3236 2c0a 2020 2020 2020 2020  020426,.        
+00000b90: 2273 6570 5f74 6f5f 5749 5345 5f73 6f75  "sep_to_WISE_sou
+00000ba0: 7263 6522 3a30 2e32 3830 3637 332c 0a20  rce":0.280673,. 
+00000bb0: 2020 2020 2020 2022 7731 6d70 726f 223a         "w1mpro":
+00000bc0: 3134 2e37 3432 2c0a 2020 2020 2020 2020  14.742,.        
+00000bd0: 2277 326d 7072 6f22 3a31 332e 3938 360a  "w2mpro":13.986.
+00000be0: 2020 2020 7d2c 0a20 2020 2022 3622 3a7b      },.    "6":{
+00000bf0: 0a20 2020 2020 2020 2022 6e61 6d65 223a  .        "name":
+00000c00: 2241 5432 3032 3161 6574 7a22 2c0a 2020  "AT2021aetz",.  
+00000c10: 2020 2020 2020 2274 7065 616b 223a 3538        "tpeak":58
+00000c20: 3339 302e 332c 0a20 2020 2020 2020 2022  390.3,.        "
+00000c30: 7269 7365 7469 6d65 223a 2238 2e36 222c  risetime":"8.6",
+00000c40: 0a20 2020 2020 2020 2022 6661 6465 7469  .        "fadeti
+00000c50: 6d65 223a 225c 7532 3031 3322 2c0a 2020  me":"\u2013",.  
+00000c60: 2020 2020 2020 2264 665f 6f76 6572 5f72        "df_over_r
+00000c70: 6d73 223a 3437 2e35 2c0a 2020 2020 2020  ms":47.5,.      
+00000c80: 2020 2264 665f 7261 7722 3a22 302e 3831    "df_raw":"0.81
+00000c90: 205c 7530 3062 3120 302e 3031 222c 0a20   \u00b1 0.01",. 
+00000ca0: 2020 2020 2020 2022 7a22 3a22 302e 3038         "z":"0.08
+00000cb0: 3739 222c 0a20 2020 2020 2020 2022 6d62  79",.        "mb
+00000cc0: 6822 3a22 362e 3231 2028 5431 3329 222c  h":"6.21 (T13)",
+00000cd0: 0a20 2020 2020 2020 2022 7061 676e 7464  .        "pagntd
+00000ce0: 6522 3a30 2e30 2c0a 2020 2020 2020 2020  e":0.0,.        
+00000cf0: 2263 6c61 7373 223a 2254 4445 3f22 2c0a  "class":"TDE?",.
+00000d00: 2020 2020 2020 2020 2264 6622 3a30 2e38          "df":0.8
+00000d10: 312c 0a20 2020 2020 2020 2022 6466 5f65  1,.        "df_e
+00000d20: 223a 302e 3031 2c0a 2020 2020 2020 2020  ":0.01,.        
+00000d30: 2272 6122 3a33 3237 2e37 3332 3234 3036  "ra":327.7322406
+00000d40: 3433 332c 0a20 2020 2020 2020 2022 6465  433,.        "de
+00000d50: 6322 3a2d 312e 3131 3530 3632 3937 3333  c":-1.1150629733
+00000d60: 2c0a 2020 2020 2020 2020 2241 6c6c 5749  ,.        "AllWI
+00000d70: 5345 5f69 6422 3a33 3238 3230 3031 3630  SE_id":328200160
+00000d80: 3133 3531 3033 3635 3731 2c0a 2020 2020  1351036571,.    
+00000d90: 2020 2020 2273 6570 5f74 6f5f 5749 5345      "sep_to_WISE
+00000da0: 5f73 6f75 7263 6522 3a30 2e30 3637 3337  _source":0.06737
+00000db0: 332c 0a20 2020 2020 2020 2022 7731 6d70  3,.        "w1mp
+00000dc0: 726f 223a 3135 2e33 3636 2c0a 2020 2020  ro":15.366,.    
+00000dd0: 2020 2020 2277 326d 7072 6f22 3a31 342e      "w2mpro":14.
+00000de0: 3639 330a 2020 2020 7d2c 0a20 2020 2022  693.    },.    "
+00000df0: 3722 3a7b 0a20 2020 2020 2020 2022 6e61  7":{.        "na
+00000e00: 6d65 223a 2241 5432 3031 3869 6765 222c  me":"AT2018ige",
+00000e10: 0a20 2020 2020 2020 2022 7470 6561 6b22  .        "tpeak"
+00000e20: 3a35 3834 3332 2e35 2c0a 2020 2020 2020  :58432.5,.      
+00000e30: 2020 2272 6973 6574 696d 6522 3a22 5c75    "risetime":"\u
+00000e40: 3230 3133 222c 0a20 2020 2020 2020 2022  2013",.        "
+00000e50: 6661 6465 7469 6d65 223a 2236 372e 3922  fadetime":"67.9"
+00000e60: 2c0a 2020 2020 2020 2020 2264 665f 6f76  ,.        "df_ov
+00000e70: 6572 5f72 6d73 223a 3635 2e38 2c0a 2020  er_rms":65.8,.  
+00000e80: 2020 2020 2020 2264 665f 7261 7722 3a22        "df_raw":"
+00000e90: 302e 3331 205c 7530 3062 3120 302e 3031  0.31 \u00b1 0.01
+00000ea0: 222c 0a20 2020 2020 2020 2022 7a22 3a22  ",.        "z":"
+00000eb0: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
+00000ec0: 2022 6d62 6822 3a22 5c75 3230 3133 222c   "mbh":"\u2013",
+00000ed0: 0a20 2020 2020 2020 2022 7061 676e 7464  .        "pagntd
+00000ee0: 6522 3a30 2e30 2c0a 2020 2020 2020 2020  e":0.0,.        
+00000ef0: 2263 6c61 7373 223a 225c 7532 3031 3322  "class":"\u2013"
+00000f00: 2c0a 2020 2020 2020 2020 2264 6622 3a30  ,.        "df":0
+00000f10: 2e33 312c 0a20 2020 2020 2020 2022 6466  .31,.        "df
+00000f20: 5f65 223a 302e 3031 2c0a 2020 2020 2020  _e":0.01,.      
+00000f30: 2020 2272 6122 3a31 3138 2e36 3338 3035    "ra":118.63805
+00000f40: 3037 2c0a 2020 2020 2020 2020 2264 6563  07,.        "dec
+00000f50: 223a 392e 3439 3431 3235 392c 0a20 2020  ":9.4941259,.   
+00000f60: 2020 2020 2022 416c 6c57 4953 455f 6964       "AllWISE_id
+00000f70: 223a 3131 3739 3130 3930 3031 3335 3130  ":11791090013510
+00000f80: 3439 3636 372c 0a20 2020 2020 2020 2022  49667,.        "
+00000f90: 7365 705f 746f 5f57 4953 455f 736f 7572  sep_to_WISE_sour
+00000fa0: 6365 223a 302e 3434 3938 3632 2c0a 2020  ce":0.449862,.  
+00000fb0: 2020 2020 2020 2277 316d 7072 6f22 3a31        "w1mpro":1
+00000fc0: 352e 3736 372c 0a20 2020 2020 2020 2022  5.767,.        "
+00000fd0: 7732 6d70 726f 223a 3135 2e35 380a 2020  w2mpro":15.58.  
+00000fe0: 2020 7d2c 0a20 2020 2022 3822 3a7b 0a20    },.    "8":{. 
+00000ff0: 2020 2020 2020 2022 6e61 6d65 223a 2241         "name":"A
+00001000: 5432 3032 3161 6575 6422 2c0a 2020 2020  T2021aeud",.    
+00001010: 2020 2020 2274 7065 616b 223a 3538 3434      "tpeak":5844
+00001020: 382e 332c 0a20 2020 2020 2020 2022 7269  8.3,.        "ri
+00001030: 7365 7469 6d65 223a 2231 3337 2e36 222c  setime":"137.6",
+00001040: 0a20 2020 2020 2020 2022 6661 6465 7469  .        "fadeti
+00001050: 6d65 223a 2232 3832 2e37 222c 0a20 2020  me":"282.7",.   
+00001060: 2020 2020 2022 6466 5f6f 7665 725f 726d       "df_over_rm
+00001070: 7322 3a36 2e32 2c0a 2020 2020 2020 2020  s":6.2,.        
+00001080: 2264 665f 7261 7722 3a22 302e 3135 205c  "df_raw":"0.15 \
+00001090: 7530 3062 3120 302e 3031 222c 0a20 2020  u00b1 0.01",.   
+000010a0: 2020 2020 2022 7a22 3a22 5c75 3230 3133       "z":"\u2013
+000010b0: 222c 0a20 2020 2020 2020 2022 6d62 6822  ",.        "mbh"
+000010c0: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
+000010d0: 2020 2022 7061 676e 7464 6522 3a34 2e32     "pagntde":4.2
+000010e0: 3838 2c0a 2020 2020 2020 2020 2263 6c61  88,.        "cla
+000010f0: 7373 223a 225c 7532 3031 3322 2c0a 2020  ss":"\u2013",.  
+00001100: 2020 2020 2020 2264 6622 3a30 2e31 352c        "df":0.15,
+00001110: 0a20 2020 2020 2020 2022 6466 5f65 223a  .        "df_e":
+00001120: 302e 3031 2c0a 2020 2020 2020 2020 2272  0.01,.        "r
+00001130: 6122 3a31 3035 2e32 3333 3739 3035 3037  a":105.233790507
+00001140: 372c 0a20 2020 2020 2020 2022 6465 6322  7,.        "dec"
+00001150: 3a33 362e 3938 3039 3535 3437 3432 2c0a  :36.9809554742,.
+00001160: 2020 2020 2020 2020 2241 6c6c 5749 5345          "AllWISE
+00001170: 5f69 6422 3a31 3034 3431 3336 3330 3133  _id":10441363013
+00001180: 3531 3034 3539 3237 2c0a 2020 2020 2020  51045927,.      
+00001190: 2020 2273 6570 5f74 6f5f 5749 5345 5f73    "sep_to_WISE_s
+000011a0: 6f75 7263 6522 3a30 2e31 3334 3638 322c  ource":0.134682,
+000011b0: 0a20 2020 2020 2020 2022 7731 6d70 726f  .        "w1mpro
+000011c0: 223a 3134 2e31 3336 2c0a 2020 2020 2020  ":14.136,.      
+000011d0: 2020 2277 326d 7072 6f22 3a31 332e 3038    "w2mpro":13.08
+000011e0: 330a 2020 2020 7d2c 0a20 2020 2022 3922  3.    },.    "9"
+000011f0: 3a7b 0a20 2020 2020 2020 2022 6e61 6d65  :{.        "name
+00001200: 223a 2241 5432 3031 3869 716c 222c 0a20  ":"AT2018iql",. 
+00001210: 2020 2020 2020 2022 7470 6561 6b22 3a35         "tpeak":5
+00001220: 3834 3439 2e34 2c0a 2020 2020 2020 2020  8449.4,.        
+00001230: 2272 6973 6574 696d 6522 3a22 3137 2e39  "risetime":"17.9
+00001240: 222c 0a20 2020 2020 2020 2022 6661 6465  ",.        "fade
+00001250: 7469 6d65 223a 2234 312e 3022 2c0a 2020  time":"41.0",.  
+00001260: 2020 2020 2020 2264 665f 6f76 6572 5f72        "df_over_r
+00001270: 6d73 223a 3330 2e31 2c0a 2020 2020 2020  ms":30.1,.      
+00001280: 2020 2264 665f 7261 7722 3a22 302e 3438    "df_raw":"0.48
+00001290: 205c 7530 3062 3120 302e 3031 222c 0a20   \u00b1 0.01",. 
+000012a0: 2020 2020 2020 2022 7a22 3a22 5c75 3230         "z":"\u20
+000012b0: 3133 222c 0a20 2020 2020 2020 2022 6d62  13",.        "mb
+000012c0: 6822 3a22 5c75 3230 3133 222c 0a20 2020  h":"\u2013",.   
+000012d0: 2020 2020 2022 7061 676e 7464 6522 3a30       "pagntde":0
+000012e0: 2e30 2c0a 2020 2020 2020 2020 2263 6c61  .0,.        "cla
+000012f0: 7373 223a 225c 7532 3031 3322 2c0a 2020  ss":"\u2013",.  
+00001300: 2020 2020 2020 2264 6622 3a30 2e34 382c        "df":0.48,
+00001310: 0a20 2020 2020 2020 2022 6466 5f65 223a  .        "df_e":
+00001320: 302e 3031 2c0a 2020 2020 2020 2020 2272  0.01,.        "r
+00001330: 6122 3a37 342e 3537 3936 3637 2c0a 2020  a":74.579667,.  
+00001340: 2020 2020 2020 2264 6563 223a 2d37 2e37        "dec":-7.7
+00001350: 3637 3936 312c 0a20 2020 2020 2020 2022  67961,.        "
+00001360: 416c 6c57 4953 455f 6964 223a 3734 3730  AllWISE_id":7470
+00001370: 3037 3630 3133 3531 3031 3336 3937 2c0a  07601351013697,.
+00001380: 2020 2020 2020 2020 2273 6570 5f74 6f5f          "sep_to_
+00001390: 5749 5345 5f73 6f75 7263 6522 3a30 2e31  WISE_source":0.1
+000013a0: 3534 3537 312c 0a20 2020 2020 2020 2022  54571,.        "
+000013b0: 7731 6d70 726f 223a 3134 2e35 3232 2c0a  w1mpro":14.522,.
+000013c0: 2020 2020 2020 2020 2277 326d 7072 6f22          "w2mpro"
+000013d0: 3a31 332e 3633 350a 2020 2020 7d2c 0a20  :13.635.    },. 
+000013e0: 2020 2022 3130 223a 7b0a 2020 2020 2020     "10":{.      
+000013f0: 2020 226e 616d 6522 3a22 4154 3230 3138    "name":"AT2018
+00001400: 6a75 7422 2c0a 2020 2020 2020 2020 2274  jut",.        "t
+00001410: 7065 616b 223a 3538 3434 392e 362c 0a20  peak":58449.6,. 
+00001420: 2020 2020 2020 2022 7269 7365 7469 6d65         "risetime
+00001430: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
+00001440: 2020 2020 2266 6164 6574 696d 6522 3a22      "fadetime":"
+00001450: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
+00001460: 2022 6466 5f6f 7665 725f 726d 7322 3a35   "df_over_rms":5
+00001470: 2e30 2c0a 2020 2020 2020 2020 2264 665f  .0,.        "df_
+00001480: 7261 7722 3a22 302e 3132 205c 7530 3062  raw":"0.12 \u00b
+00001490: 3120 302e 3031 222c 0a20 2020 2020 2020  1 0.01",.       
+000014a0: 2022 7a22 3a22 5c75 3230 3133 222c 0a20   "z":"\u2013",. 
+000014b0: 2020 2020 2020 2022 6d62 6822 3a22 5c75         "mbh":"\u
+000014c0: 3230 3133 222c 0a20 2020 2020 2020 2022  2013",.        "
+000014d0: 7061 676e 7464 6522 3a35 2e37 3832 2c0a  pagntde":5.782,.
+000014e0: 2020 2020 2020 2020 2263 6c61 7373 223a          "class":
+000014f0: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
+00001500: 2020 2264 6622 3a30 2e31 322c 0a20 2020    "df":0.12,.   
+00001510: 2020 2020 2022 6466 5f65 223a 302e 3031       "df_e":0.01
+00001520: 2c0a 2020 2020 2020 2020 2272 6122 3a32  ,.        "ra":2
+00001530: 3038 2e35 3334 3632 352c 0a20 2020 2020  08.534625,.     
+00001540: 2020 2022 6465 6322 3a31 332e 3033 3232     "dec":13.0322
+00001550: 352c 0a20 2020 2020 2020 2022 416c 6c57  5,.        "AllW
+00001560: 4953 455f 6964 223a 3230 3739 3131 3336  ISE_id":20791136
+00001570: 3031 3335 3130 3030 3033 382c 0a20 2020  01351000038,.   
+00001580: 2020 2020 2022 7365 705f 746f 5f57 4953       "sep_to_WIS
+00001590: 455f 736f 7572 6365 223a 302e 3232 3239  E_source":0.2229
+000015a0: 3631 2c0a 2020 2020 2020 2020 2277 316d  61,.        "w1m
+000015b0: 7072 6f22 3a31 342e 3738 372c 0a20 2020  pro":14.787,.   
+000015c0: 2020 2020 2022 7732 6d70 726f 223a 3134       "w2mpro":14
+000015d0: 2e30 3633 0a20 2020 207d 2c0a 2020 2020  .063.    },.    
+000015e0: 2231 3122 3a7b 0a20 2020 2020 2020 2022  "11":{.        "
+000015f0: 6e61 6d65 223a 2241 5432 3032 3161 6575  name":"AT2021aeu
+00001600: 6522 2c0a 2020 2020 2020 2020 2274 7065  e",.        "tpe
+00001610: 616b 223a 3538 3437 352e 312c 0a20 2020  ak":58475.1,.   
+00001620: 2020 2020 2022 7269 7365 7469 6d65 223a       "risetime":
+00001630: 2234 382e 3522 2c0a 2020 2020 2020 2020  "48.5",.        
+00001640: 2266 6164 6574 696d 6522 3a22 3438 2e38  "fadetime":"48.8
+00001650: 222c 0a20 2020 2020 2020 2022 6466 5f6f  ",.        "df_o
+00001660: 7665 725f 726d 7322 3a34 2e39 2c0a 2020  ver_rms":4.9,.  
+00001670: 2020 2020 2020 2264 665f 7261 7722 3a22        "df_raw":"
+00001680: 302e 3131 205c 7530 3062 3120 302e 3031  0.11 \u00b1 0.01
+00001690: 222c 0a20 2020 2020 2020 2022 7a22 3a22  ",.        "z":"
+000016a0: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
+000016b0: 2022 6d62 6822 3a22 5c75 3230 3133 222c   "mbh":"\u2013",
+000016c0: 0a20 2020 2020 2020 2022 7061 676e 7464  .        "pagntd
+000016d0: 6522 3a35 2e38 3831 2c0a 2020 2020 2020  e":5.881,.      
+000016e0: 2020 2263 6c61 7373 223a 225c 7532 3031    "class":"\u201
+000016f0: 3322 2c0a 2020 2020 2020 2020 2264 6622  3",.        "df"
+00001700: 3a30 2e31 312c 0a20 2020 2020 2020 2022  :0.11,.        "
+00001710: 6466 5f65 223a 302e 3031 2c0a 2020 2020  df_e":0.01,.    
+00001720: 2020 2020 2272 6122 3a33 352e 3739 3332      "ra":35.7932
+00001730: 3036 3231 3239 2c0a 2020 2020 2020 2020  062129,.        
+00001740: 2264 6563 223a 2d39 2e35 3430 3039 3534  "dec":-9.5400954
+00001750: 3837 392c 0a20 2020 2020 2020 2022 416c  879,.        "Al
+00001760: 6c57 4953 455f 6964 223a 3335 3230 3039  lWISE_id":352009
+00001770: 3130 3133 3531 3032 3330 3638 2c0a 2020  101351023068,.  
+00001780: 2020 2020 2020 2273 6570 5f74 6f5f 5749        "sep_to_WI
+00001790: 5345 5f73 6f75 7263 6522 3a30 2e31 3336  SE_source":0.136
+000017a0: 3238 2c0a 2020 2020 2020 2020 2277 316d  28,.        "w1m
+000017b0: 7072 6f22 3a31 342e 3131 382c 0a20 2020  pro":14.118,.   
+000017c0: 2020 2020 2022 7732 6d70 726f 223a 3133       "w2mpro":13
+000017d0: 2e34 3132 0a20 2020 207d 2c0a 2020 2020  .412.    },.    
+000017e0: 2231 3222 3a7b 0a20 2020 2020 2020 2022  "12":{.        "
+000017f0: 6e61 6d65 223a 2241 5432 3031 3961 616d  name":"AT2019aam
+00001800: 6622 2c0a 2020 2020 2020 2020 2274 7065  f",.        "tpe
+00001810: 616b 223a 3538 3530 362e 342c 0a20 2020  ak":58506.4,.   
+00001820: 2020 2020 2022 7269 7365 7469 6d65 223a       "risetime":
+00001830: 2238 302e 3022 2c0a 2020 2020 2020 2020  "80.0",.        
+00001840: 2266 6164 6574 696d 6522 3a22 3134 312e  "fadetime":"141.
+00001850: 3222 2c0a 2020 2020 2020 2020 2264 665f  2",.        "df_
+00001860: 6f76 6572 5f72 6d73 223a 362e 362c 0a20  over_rms":6.6,. 
+00001870: 2020 2020 2020 2022 6466 5f72 6177 223a         "df_raw":
+00001880: 2230 2e31 3920 5c75 3030 6231 2030 2e30  "0.19 \u00b1 0.0
+00001890: 3122 2c0a 2020 2020 2020 2020 227a 223a  1",.        "z":
+000018a0: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
+000018b0: 2020 226d 6268 223a 225c 7532 3031 3322    "mbh":"\u2013"
+000018c0: 2c0a 2020 2020 2020 2020 2270 6167 6e74  ,.        "pagnt
+000018d0: 6465 223a 332e 3734 342c 0a20 2020 2020  de":3.744,.     
+000018e0: 2020 2022 636c 6173 7322 3a22 5c75 3230     "class":"\u20
+000018f0: 3133 222c 0a20 2020 2020 2020 2022 6466  13",.        "df
+00001900: 223a 302e 3139 2c0a 2020 2020 2020 2020  ":0.19,.        
+00001910: 2264 665f 6522 3a30 2e30 312c 0a20 2020  "df_e":0.01,.   
+00001920: 2020 2020 2022 7261 223a 3133 342e 3235       "ra":134.25
+00001930: 3631 3439 3137 3833 2c0a 2020 2020 2020  61491783,.      
+00001940: 2020 2264 6563 223a 3333 2e39 3134 3938    "dec":33.91498
+00001950: 3837 3034 382c 0a20 2020 2020 2020 2022  87048,.        "
+00001960: 416c 6c57 4953 455f 6964 223a 3133 3439  AllWISE_id":1349
+00001970: 3133 3333 3031 3335 3130 3535 3237 342c  133301351055274,
+00001980: 0a20 2020 2020 2020 2022 7365 705f 746f  .        "sep_to
+00001990: 5f57 4953 455f 736f 7572 6365 223a 302e  _WISE_source":0.
+000019a0: 3236 3436 2c0a 2020 2020 2020 2020 2277  2646,.        "w
+000019b0: 316d 7072 6f22 3a31 342e 3536 392c 0a20  1mpro":14.569,. 
+000019c0: 2020 2020 2020 2022 7732 6d70 726f 223a         "w2mpro":
+000019d0: 3134 2e33 3031 0a20 2020 207d 2c0a 2020  14.301.    },.  
+000019e0: 2020 2231 3322 3a7b 0a20 2020 2020 2020    "13":{.       
+000019f0: 2022 6e61 6d65 223a 2241 5432 3031 386b   "name":"AT2018k
+00001a00: 6f78 222c 0a20 2020 2020 2020 2022 7470  ox",.        "tp
+00001a10: 6561 6b22 3a35 3835 3130 2e32 2c0a 2020  eak":58510.2,.  
+00001a20: 2020 2020 2020 2272 6973 6574 696d 6522        "risetime"
+00001a30: 3a22 3236 2e39 222c 0a20 2020 2020 2020  :"26.9",.       
+00001a40: 2022 6661 6465 7469 6d65 223a 2231 3637   "fadetime":"167
+00001a50: 2e36 222c 0a20 2020 2020 2020 2022 6466  .6",.        "df
+00001a60: 5f6f 7665 725f 726d 7322 3a35 2e36 2c0a  _over_rms":5.6,.
+00001a70: 2020 2020 2020 2020 2264 665f 7261 7722          "df_raw"
+00001a80: 3a22 302e 3333 205c 7530 3062 3120 302e  :"0.33 \u00b1 0.
+00001a90: 3031 222c 0a20 2020 2020 2020 2022 7a22  01",.        "z"
+00001aa0: 3a22 302e 3039 3622 2c0a 2020 2020 2020  :"0.096",.      
+00001ab0: 2020 226d 6268 223a 225c 7532 3031 3322    "mbh":"\u2013"
+00001ac0: 2c0a 2020 2020 2020 2020 2270 6167 6e74  ,.        "pagnt
+00001ad0: 6465 223a 352e 3034 362c 0a20 2020 2020  de":5.046,.     
+00001ae0: 2020 2022 636c 6173 7322 3a22 5c75 3230     "class":"\u20
+00001af0: 3133 222c 0a20 2020 2020 2020 2022 6466  13",.        "df
+00001b00: 223a 302e 3333 2c0a 2020 2020 2020 2020  ":0.33,.        
+00001b10: 2264 665f 6522 3a30 2e30 312c 0a20 2020  "df_e":0.01,.   
+00001b20: 2020 2020 2022 7261 223a 3730 2e37 3933       "ra":70.793
+00001b30: 3337 352c 0a20 2020 2020 2020 2022 6465  375,.        "de
+00001b40: 6322 3a2d 342e 3330 3330 3831 2c0a 2020  c":-4.303081,.  
+00001b50: 2020 2020 2020 2241 6c6c 5749 5345 5f69        "AllWISE_i
+00001b60: 6422 3a37 3133 3030 3436 3031 3335 3130  d":7130046013510
+00001b70: 3336 3136 342c 0a20 2020 2020 2020 2022  36164,.        "
+00001b80: 7365 705f 746f 5f57 4953 455f 736f 7572  sep_to_WISE_sour
+00001b90: 6365 223a 302e 3136 3936 3334 2c0a 2020  ce":0.169634,.  
+00001ba0: 2020 2020 2020 2277 316d 7072 6f22 3a31        "w1mpro":1
+00001bb0: 332e 3930 352c 0a20 2020 2020 2020 2022  3.905,.        "
+00001bc0: 7732 6d70 726f 223a 3133 2e35 3836 0a20  w2mpro":13.586. 
+00001bd0: 2020 207d 2c0a 2020 2020 2231 3422 3a7b     },.    "14":{
+00001be0: 0a20 2020 2020 2020 2022 6e61 6d65 223a  .        "name":
+00001bf0: 2241 5432 3031 386c 6876 222c 0a20 2020  "AT2018lhv",.   
+00001c00: 2020 2020 2022 7470 6561 6b22 3a35 3835       "tpeak":585
+00001c10: 3133 2e35 2c0a 2020 2020 2020 2020 2272  13.5,.        "r
+00001c20: 6973 6574 696d 6522 3a22 3137 2e35 222c  isetime":"17.5",
+00001c30: 0a20 2020 2020 2020 2022 6661 6465 7469  .        "fadeti
+00001c40: 6d65 223a 2231 3136 2e31 222c 0a20 2020  me":"116.1",.   
+00001c50: 2020 2020 2022 6466 5f6f 7665 725f 726d       "df_over_rm
+00001c60: 7322 3a33 322e 332c 0a20 2020 2020 2020  s":32.3,.       
+00001c70: 2022 6466 5f72 6177 223a 2230 2e33 3520   "df_raw":"0.35 
+00001c80: 5c75 3030 6231 2030 2e30 3122 2c0a 2020  \u00b1 0.01",.  
+00001c90: 2020 2020 2020 227a 223a 225c 7532 3031        "z":"\u201
+00001ca0: 3322 2c0a 2020 2020 2020 2020 226d 6268  3",.        "mbh
+00001cb0: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
+00001cc0: 2020 2020 2270 6167 6e74 6465 223a 302e      "pagntde":0.
+00001cd0: 302c 0a20 2020 2020 2020 2022 636c 6173  0,.        "clas
+00001ce0: 7322 3a22 5c75 3230 3133 222c 0a20 2020  s":"\u2013",.   
+00001cf0: 2020 2020 2022 6466 223a 302e 3335 2c0a       "df":0.35,.
+00001d00: 2020 2020 2020 2020 2264 665f 6522 3a30          "df_e":0
+00001d10: 2e30 312c 0a20 2020 2020 2020 2022 7261  .01,.        "ra
+00001d20: 223a 3139 362e 3335 3338 3030 312c 0a20  ":196.3538001,. 
+00001d30: 2020 2020 2020 2022 6465 6322 3a32 312e         "dec":21.
+00001d40: 3935 3434 3632 372c 0a20 2020 2020 2020  9544627,.       
+00001d50: 2022 416c 6c57 4953 455f 6964 223a 3139   "AllWISE_id":19
+00001d60: 3639 3132 3132 3031 3335 3130 3633 3031  6912120135106301
+00001d70: 352c 0a20 2020 2020 2020 2022 7365 705f  5,.        "sep_
+00001d80: 746f 5f57 4953 455f 736f 7572 6365 223a  to_WISE_source":
+00001d90: 302e 3433 3033 3237 2c0a 2020 2020 2020  0.430327,.      
+00001da0: 2020 2277 316d 7072 6f22 3a31 352e 3033    "w1mpro":15.03
+00001db0: 382c 0a20 2020 2020 2020 2022 7732 6d70  8,.        "w2mp
+00001dc0: 726f 223a 3134 2e38 3439 0a20 2020 207d  ro":14.849.    }
+00001dd0: 2c0a 2020 2020 2231 3522 3a7b 0a20 2020  ,.    "15":{.   
+00001de0: 2020 2020 2022 6e61 6d65 223a 2241 5432       "name":"AT2
+00001df0: 3031 3961 7664 222c 0a20 2020 2020 2020  019avd",.       
+00001e00: 2022 7470 6561 6b22 3a35 3835 3334 2e33   "tpeak":58534.3
+00001e10: 2c0a 2020 2020 2020 2020 2272 6973 6574  ,.        "riset
+00001e20: 696d 6522 3a22 3134 2e39 222c 0a20 2020  ime":"14.9",.   
+00001e30: 2020 2020 2022 6661 6465 7469 6d65 223a       "fadetime":
+00001e40: 2235 322e 3922 2c0a 2020 2020 2020 2020  "52.9",.        
+00001e50: 2264 665f 6f76 6572 5f72 6d73 223a 3637  "df_over_rms":67
+00001e60: 2e35 2c0a 2020 2020 2020 2020 2264 665f  .5,.        "df_
+00001e70: 7261 7722 3a22 312e 3837 205c 7530 3062  raw":"1.87 \u00b
+00001e80: 3120 302e 3035 222c 0a20 2020 2020 2020  1 0.05",.       
+00001e90: 2022 7a22 3a22 302e 3032 3936 222c 0a20   "z":"0.0296",. 
+00001ea0: 2020 2020 2020 2022 6d62 6822 3a22 362e         "mbh":"6.
+00001eb0: 3130 2028 4632 3029 222c 0a20 2020 2020  10 (F20)",.     
+00001ec0: 2020 2022 7061 676e 7464 6522 3a30 2e30     "pagntde":0.0
+00001ed0: 2c0a 2020 2020 2020 2020 2263 6c61 7373  ,.        "class
+00001ee0: 223a 2254 4445 3f22 2c0a 2020 2020 2020  ":"TDE?",.      
+00001ef0: 2020 2264 6622 3a31 2e38 372c 0a20 2020    "df":1.87,.   
+00001f00: 2020 2020 2022 6466 5f65 223a 302e 3035       "df_e":0.05
+00001f10: 2c0a 2020 2020 2020 2020 2272 6122 3a31  ,.        "ra":1
+00001f20: 3235 2e39 3033 3139 3735 2c0a 2020 2020  25.9031975,.    
+00001f30: 2020 2020 2264 6563 223a 342e 3338 3430      "dec":4.3840
+00001f40: 3136 362c 0a20 2020 2020 2020 2022 416c  166,.        "Al
+00001f50: 6c57 4953 455f 6964 223a 3132 3630 3130  lWISE_id":126010
+00001f60: 3435 3031 3335 3130 3134 3231 382c 0a20  4501351014218,. 
+00001f70: 2020 2020 2020 2022 7365 705f 746f 5f57         "sep_to_W
+00001f80: 4953 455f 736f 7572 6365 223a 302e 3035  ISE_source":0.05
+00001f90: 3831 3737 2c0a 2020 2020 2020 2020 2277  8177,.        "w
+00001fa0: 316d 7072 6f22 3a31 322e 3734 2c0a 2020  1mpro":12.74,.  
+00001fb0: 2020 2020 2020 2277 326d 7072 6f22 3a31        "w2mpro":1
+00001fc0: 322e 3637 340a 2020 2020 7d2c 0a20 2020  2.674.    },.   
+00001fd0: 2022 3136 223a 7b0a 2020 2020 2020 2020   "16":{.        
+00001fe0: 226e 616d 6522 3a22 4154 3230 3136 6569  "name":"AT2016ei
+00001ff0: 7822 2c0a 2020 2020 2020 2020 2274 7065  x",.        "tpe
+00002000: 616b 223a 3538 3533 392e 342c 0a20 2020  ak":58539.4,.   
+00002010: 2020 2020 2022 7269 7365 7469 6d65 223a       "risetime":
+00002020: 2231 3034 2e32 222c 0a20 2020 2020 2020  "104.2",.       
+00002030: 2022 6661 6465 7469 6d65 223a 2234 332e   "fadetime":"43.
+00002040: 3122 2c0a 2020 2020 2020 2020 2264 665f  1",.        "df_
+00002050: 6f76 6572 5f72 6d73 223a 362e 392c 0a20  over_rms":6.9,. 
+00002060: 2020 2020 2020 2022 6466 5f72 6177 223a         "df_raw":
+00002070: 2230 2e31 3620 5c75 3030 6231 2030 2e30  "0.16 \u00b1 0.0
+00002080: 3122 2c0a 2020 2020 2020 2020 227a 223a  1",.        "z":
+00002090: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
+000020a0: 2020 226d 6268 223a 225c 7532 3031 3322    "mbh":"\u2013"
+000020b0: 2c0a 2020 2020 2020 2020 2270 6167 6e74  ,.        "pagnt
+000020c0: 6465 223a 332e 3237 372c 0a20 2020 2020  de":3.277,.     
+000020d0: 2020 2022 636c 6173 7322 3a22 5c75 3230     "class":"\u20
+000020e0: 3133 222c 0a20 2020 2020 2020 2022 6466  13",.        "df
+000020f0: 223a 302e 3136 2c0a 2020 2020 2020 2020  ":0.16,.        
+00002100: 2264 665f 6522 3a30 2e30 312c 0a20 2020  "df_e":0.01,.   
+00002110: 2020 2020 2022 7261 223a 3234 342e 3731       "ra":244.71
+00002120: 3634 3338 3939 3137 2c0a 2020 2020 2020  64389917,.      
+00002130: 2020 2264 6563 223a 3633 2e31 3733 3337    "dec":63.17337
+00002140: 3339 3735 2c0a 2020 2020 2020 2020 2241  3975,.        "A
+00002150: 6c6c 5749 5345 5f69 6422 3a32 3434 3431  llWISE_id":24441
+00002160: 3633 3630 3133 3531 3031 3830 3435 2c0a  63601351018045,.
+00002170: 2020 2020 2020 2020 2273 6570 5f74 6f5f          "sep_to_
+00002180: 5749 5345 5f73 6f75 7263 6522 3a30 2e36  WISE_source":0.6
+00002190: 3936 3737 372c 0a20 2020 2020 2020 2022  96777,.        "
+000021a0: 7731 6d70 726f 223a 3134 2e30 3038 2c0a  w1mpro":14.008,.
+000021b0: 2020 2020 2020 2020 2277 326d 7072 6f22          "w2mpro"
+000021c0: 3a31 332e 3135 380a 2020 2020 7d2c 0a20  :13.158.    },. 
+000021d0: 2020 2022 3137 223a 7b0a 2020 2020 2020     "17":{.      
+000021e0: 2020 226e 616d 6522 3a22 4154 3230 3139    "name":"AT2019
+000021f0: 6161 6d67 222c 0a20 2020 2020 2020 2022  aamg",.        "
+00002200: 7470 6561 6b22 3a35 3835 3430 2e35 2c0a  tpeak":58540.5,.
+00002210: 2020 2020 2020 2020 2272 6973 6574 696d          "risetim
+00002220: 6522 3a22 5c75 3230 3133 222c 0a20 2020  e":"\u2013",.   
+00002230: 2020 2020 2022 6661 6465 7469 6d65 223a       "fadetime":
+00002240: 2239 332e 3722 2c0a 2020 2020 2020 2020  "93.7",.        
+00002250: 2264 665f 6f76 6572 5f72 6d73 223a 382e  "df_over_rms":8.
+00002260: 332c 0a20 2020 2020 2020 2022 6466 5f72  3,.        "df_r
+00002270: 6177 223a 2230 2e31 3420 5c75 3030 6231  aw":"0.14 \u00b1
+00002280: 2030 2e30 3022 2c0a 2020 2020 2020 2020   0.00",.        
+00002290: 227a 223a 225c 7532 3031 3322 2c0a 2020  "z":"\u2013",.  
+000022a0: 2020 2020 2020 226d 6268 223a 225c 7532        "mbh":"\u2
+000022b0: 3031 3322 2c0a 2020 2020 2020 2020 2270  013",.        "p
+000022c0: 6167 6e74 6465 223a 312e 3934 352c 0a20  agntde":1.945,. 
+000022d0: 2020 2020 2020 2022 636c 6173 7322 3a22         "class":"
+000022e0: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
+000022f0: 2022 6466 223a 302e 3134 2c0a 2020 2020   "df":0.14,.    
+00002300: 2020 2020 2264 665f 6522 3a30 2e30 2c0a      "df_e":0.0,.
+00002310: 2020 2020 2020 2020 2272 6122 3a32 3732          "ra":272
+00002320: 2e30 3534 3030 3237 3134 352c 0a20 2020  .0540027145,.   
+00002330: 2020 2020 2022 6465 6322 3a35 302e 3738       "dec":50.78
+00002340: 3637 3332 3736 3138 2c0a 2020 2020 2020  67327618,.      
+00002350: 2020 2241 6c6c 5749 5345 5f69 6422 3a32    "AllWISE_id":2
+00002360: 3731 3731 3531 3430 3133 3531 3030 3239  7171514013510029
+00002370: 3336 2c0a 2020 2020 2020 2020 2273 6570  36,.        "sep
+00002380: 5f74 6f5f 5749 5345 5f73 6f75 7263 6522  _to_WISE_source"
+00002390: 3a30 2e34 3832 3431 332c 0a20 2020 2020  :0.482413,.     
+000023a0: 2020 2022 7731 6d70 726f 223a 3135 2e32     "w1mpro":15.2
+000023b0: 3036 2c0a 2020 2020 2020 2020 2277 326d  06,.        "w2m
+000023c0: 7072 6f22 3a31 342e 3432 340a 2020 2020  pro":14.424.    
+000023d0: 7d2c 0a20 2020 2022 3138 223a 7b0a 2020  },.    "18":{.  
+000023e0: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
+000023f0: 3230 3138 6c63 7022 2c0a 2020 2020 2020  2018lcp",.      
+00002400: 2020 2274 7065 616b 223a 3538 3534 372e    "tpeak":58547.
+00002410: 322c 0a20 2020 2020 2020 2022 7269 7365  2,.        "rise
+00002420: 7469 6d65 223a 2239 352e 3722 2c0a 2020  time":"95.7",.  
+00002430: 2020 2020 2020 2266 6164 6574 696d 6522        "fadetime"
+00002440: 3a22 3239 372e 3422 2c0a 2020 2020 2020  :"297.4",.      
+00002450: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
+00002460: 3132 2e37 2c0a 2020 2020 2020 2020 2264  12.7,.        "d
+00002470: 665f 7261 7722 3a22 302e 3136 205c 7530  f_raw":"0.16 \u0
+00002480: 3062 3120 302e 3031 222c 0a20 2020 2020  0b1 0.01",.     
+00002490: 2020 2022 7a22 3a22 302e 3036 222c 0a20     "z":"0.06",. 
+000024a0: 2020 2020 2020 2022 6d62 6822 3a22 5c75         "mbh":"\u
+000024b0: 3230 3133 222c 0a20 2020 2020 2020 2022  2013",.        "
+000024c0: 7061 676e 7464 6522 3a30 2e34 3935 2c0a  pagntde":0.495,.
+000024d0: 2020 2020 2020 2020 2263 6c61 7373 223a          "class":
+000024e0: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
+000024f0: 2020 2264 6622 3a30 2e31 362c 0a20 2020    "df":0.16,.   
+00002500: 2020 2020 2022 6466 5f65 223a 302e 3031       "df_e":0.01
+00002510: 2c0a 2020 2020 2020 2020 2272 6122 3a31  ,.        "ra":1
+00002520: 3137 2e37 3038 3431 3632 2c0a 2020 2020  17.7084162,.    
+00002530: 2020 2020 2264 6563 223a 312e 3335 3833      "dec":1.3583
+00002540: 3530 312c 0a20 2020 2020 2020 2022 416c  501,.        "Al
+00002550: 6c57 4953 455f 6964 223a 3131 3739 3130  lWISE_id":117910
+00002560: 3135 3031 3335 3130 3135 3834 342c 0a20  1501351015844,. 
+00002570: 2020 2020 2020 2022 7365 705f 746f 5f57         "sep_to_W
+00002580: 4953 455f 736f 7572 6365 223a 302e 3232  ISE_source":0.22
+00002590: 3134 3135 2c0a 2020 2020 2020 2020 2277  1415,.        "w
+000025a0: 316d 7072 6f22 3a31 342e 3232 2c0a 2020  1mpro":14.22,.  
+000025b0: 2020 2020 2020 2277 326d 7072 6f22 3a31        "w2mpro":1
+000025c0: 342e 3230 320a 2020 2020 7d2c 0a20 2020  4.202.    },.   
+000025d0: 2022 3139 223a 7b0a 2020 2020 2020 2020   "19":{.        
+000025e0: 226e 616d 6522 3a22 4154 3230 3231 6165  "name":"AT2021ae
+000025f0: 7566 222c 0a20 2020 2020 2020 2022 7470  uf",.        "tp
+00002600: 6561 6b22 3a35 3835 3536 2e34 2c0a 2020  eak":58556.4,.  
+00002610: 2020 2020 2020 2272 6973 6574 696d 6522        "risetime"
+00002620: 3a22 3137 2e30 222c 0a20 2020 2020 2020  :"17.0",.       
+00002630: 2022 6661 6465 7469 6d65 223a 2231 3337   "fadetime":"137
+00002640: 2e35 222c 0a20 2020 2020 2020 2022 6466  .5",.        "df
+00002650: 5f6f 7665 725f 726d 7322 3a31 352e 362c  _over_rms":15.6,
+00002660: 0a20 2020 2020 2020 2022 6466 5f72 6177  .        "df_raw
+00002670: 223a 2230 2e31 3820 5c75 3030 6231 2030  ":"0.18 \u00b1 0
+00002680: 2e30 3122 2c0a 2020 2020 2020 2020 227a  .01",.        "z
+00002690: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
+000026a0: 2020 2020 226d 6268 223a 225c 7532 3031      "mbh":"\u201
+000026b0: 3322 2c0a 2020 2020 2020 2020 2270 6167  3",.        "pag
+000026c0: 6e74 6465 223a 302e 3139 322c 0a20 2020  ntde":0.192,.   
+000026d0: 2020 2020 2022 636c 6173 7322 3a22 5c75       "class":"\u
+000026e0: 3230 3133 222c 0a20 2020 2020 2020 2022  2013",.        "
+000026f0: 6466 223a 302e 3138 2c0a 2020 2020 2020  df":0.18,.      
+00002700: 2020 2264 665f 6522 3a30 2e30 312c 0a20    "df_e":0.01,. 
+00002710: 2020 2020 2020 2022 7261 223a 3139 312e         "ra":191.
+00002720: 3032 3834 3531 3335 3531 2c0a 2020 2020  0284513551,.    
+00002730: 2020 2020 2264 6563 223a 3437 2e34 3435      "dec":47.445
+00002740: 3133 3530 3533 362c 0a20 2020 2020 2020  1350536,.       
+00002750: 2022 416c 6c57 4953 455f 6964 223a 3139   "AllWISE_id":19
+00002760: 3230 3134 3639 3031 3335 3130 3634 3137  2014690135106417
+00002770: 312c 0a20 2020 2020 2020 2022 7365 705f  1,.        "sep_
+00002780: 746f 5f57 4953 455f 736f 7572 6365 223a  to_WISE_source":
+00002790: 302e 3039 3333 332c 0a20 2020 2020 2020  0.09333,.       
+000027a0: 2022 7731 6d70 726f 223a 3135 2e36 3836   "w1mpro":15.686
+000027b0: 2c0a 2020 2020 2020 2020 2277 326d 7072  ,.        "w2mpr
+000027c0: 6f22 3a31 352e 3039 360a 2020 2020 7d2c  o":15.096.    },
+000027d0: 0a20 2020 2022 3230 223a 7b0a 2020 2020  .    "20":{.    
+000027e0: 2020 2020 226e 616d 6522 3a22 4154 3230      "name":"AT20
+000027f0: 3230 6165 7a79 222c 0a20 2020 2020 2020  20aezy",.       
+00002800: 2022 7470 6561 6b22 3a35 3835 3538 2e34   "tpeak":58558.4
+00002810: 2c0a 2020 2020 2020 2020 2272 6973 6574  ,.        "riset
+00002820: 696d 6522 3a22 3832 2e35 222c 0a20 2020  ime":"82.5",.   
+00002830: 2020 2020 2022 6661 6465 7469 6d65 223a       "fadetime":
+00002840: 2233 3539 2e38 222c 0a20 2020 2020 2020  "359.8",.       
+00002850: 2022 6466 5f6f 7665 725f 726d 7322 3a34   "df_over_rms":4
+00002860: 2e38 2c0a 2020 2020 2020 2020 2264 665f  .8,.        "df_
+00002870: 7261 7722 3a22 302e 3036 205c 7530 3062  raw":"0.06 \u00b
+00002880: 3120 302e 3031 222c 0a20 2020 2020 2020  1 0.01",.       
+00002890: 2022 7a22 3a22 5c75 3230 3133 222c 0a20   "z":"\u2013",. 
+000028a0: 2020 2020 2020 2022 6d62 6822 3a22 5c75         "mbh":"\u
+000028b0: 3230 3133 222c 0a20 2020 2020 2020 2022  2013",.        "
+000028c0: 7061 676e 7464 6522 3a35 2e39 3239 2c0a  pagntde":5.929,.
+000028d0: 2020 2020 2020 2020 2263 6c61 7373 223a          "class":
+000028e0: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
+000028f0: 2020 2264 6622 3a30 2e30 362c 0a20 2020    "df":0.06,.   
+00002900: 2020 2020 2022 6466 5f65 223a 302e 3031       "df_e":0.01
+00002910: 2c0a 2020 2020 2020 2020 2272 6122 3a32  ,.        "ra":2
+00002920: 3133 2e33 3334 3633 3732 3533 362c 0a20  13.3346372536,. 
+00002930: 2020 2020 2020 2022 6465 6322 3a34 342e         "dec":44.
+00002940: 3331 3638 3034 3235 392c 0a20 2020 2020  316804259,.     
+00002950: 2020 2022 416c 6c57 4953 455f 6964 223a     "AllWISE_id":
+00002960: 3231 3433 3134 3339 3031 3335 3130 3430  2143143901351040
+00002970: 3138 372c 0a20 2020 2020 2020 2022 7365  187,.        "se
+00002980: 705f 746f 5f57 4953 455f 736f 7572 6365  p_to_WISE_source
+00002990: 223a 302e 3234 3033 3535 2c0a 2020 2020  ":0.240355,.    
+000029a0: 2020 2020 2277 316d 7072 6f22 3a31 352e      "w1mpro":15.
+000029b0: 3736 392c 0a20 2020 2020 2020 2022 7732  769,.        "w2
+000029c0: 6d70 726f 223a 3134 2e38 320a 2020 2020  mpro":14.82.    
+000029d0: 7d2c 0a20 2020 2022 3231 223a 7b0a 2020  },.    "21":{.  
+000029e0: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
+000029f0: 3230 3139 636c 6522 2c0a 2020 2020 2020  2019cle",.      
+00002a00: 2020 2274 7065 616b 223a 3538 3536 382e    "tpeak":58568.
+00002a10: 342c 0a20 2020 2020 2020 2022 7269 7365  4,.        "rise
+00002a20: 7469 6d65 223a 2239 2e32 222c 0a20 2020  time":"9.2",.   
+00002a30: 2020 2020 2022 6661 6465 7469 6d65 223a       "fadetime":
+00002a40: 2235 342e 3822 2c0a 2020 2020 2020 2020  "54.8",.        
+00002a50: 2264 665f 6f76 6572 5f72 6d73 223a 3139  "df_over_rms":19
+00002a60: 2e34 2c0a 2020 2020 2020 2020 2264 665f  .4,.        "df_
+00002a70: 7261 7722 3a22 302e 3235 205c 7530 3062  raw":"0.25 \u00b
+00002a80: 3120 302e 3031 222c 0a20 2020 2020 2020  1 0.01",.       
+00002a90: 2022 7a22 3a22 5c75 3230 3133 222c 0a20   "z":"\u2013",. 
+00002aa0: 2020 2020 2020 2022 6d62 6822 3a22 5c75         "mbh":"\u
+00002ab0: 3230 3133 222c 0a20 2020 2020 2020 2022  2013",.        "
+00002ac0: 7061 676e 7464 6522 3a30 2e30 3431 2c0a  pagntde":0.041,.
+00002ad0: 2020 2020 2020 2020 2263 6c61 7373 223a          "class":
+00002ae0: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
+00002af0: 2020 2264 6622 3a30 2e32 352c 0a20 2020    "df":0.25,.   
+00002b00: 2020 2020 2022 6466 5f65 223a 302e 3031       "df_e":0.01
+00002b10: 2c0a 2020 2020 2020 2020 2272 6122 3a32  ,.        "ra":2
+00002b20: 3637 2e37 3534 3633 3732 2c0a 2020 2020  67.7546372,.    
+00002b30: 2020 2020 2264 6563 223a 3134 2e39 3138      "dec":14.918
+00002b40: 3339 3731 2c0a 2020 2020 2020 2020 2241  3971,.        "A
+00002b50: 6c6c 5749 5345 5f69 6422 3a32 3637 3631  llWISE_id":26761
+00002b60: 3135 3130 3133 3531 3031 3939 3539 2c0a  15101351019959,.
+00002b70: 2020 2020 2020 2020 2273 6570 5f74 6f5f          "sep_to_
+00002b80: 5749 5345 5f73 6f75 7263 6522 3a30 2e35  WISE_source":0.5
+00002b90: 3538 3631 332c 0a20 2020 2020 2020 2022  58613,.        "
+00002ba0: 7731 6d70 726f 223a 3134 2e39 3439 2c0a  w1mpro":14.949,.
+00002bb0: 2020 2020 2020 2020 2277 326d 7072 6f22          "w2mpro"
+00002bc0: 3a31 342e 3837 310a 2020 2020 7d2c 0a20  :14.871.    },. 
+00002bd0: 2020 2022 3232 223a 7b0a 2020 2020 2020     "22":{.      
+00002be0: 2020 226e 616d 6522 3a22 4154 3230 3139    "name":"AT2019
+00002bf0: 6161 6d68 222c 0a20 2020 2020 2020 2022  aamh",.        "
+00002c00: 7470 6561 6b22 3a35 3835 3832 2e35 2c0a  tpeak":58582.5,.
+00002c10: 2020 2020 2020 2020 2272 6973 6574 696d          "risetim
+00002c20: 6522 3a22 5c75 3230 3133 222c 0a20 2020  e":"\u2013",.   
+00002c30: 2020 2020 2022 6661 6465 7469 6d65 223a       "fadetime":
+00002c40: 2231 3534 2e35 222c 0a20 2020 2020 2020  "154.5",.       
+00002c50: 2022 6466 5f6f 7665 725f 726d 7322 3a37   "df_over_rms":7
+00002c60: 2e37 2c0a 2020 2020 2020 2020 2264 665f  .7,.        "df_
+00002c70: 7261 7722 3a22 302e 3430 205c 7530 3062  raw":"0.40 \u00b
+00002c80: 3120 302e 3031 222c 0a20 2020 2020 2020  1 0.01",.       
+00002c90: 2022 7a22 3a22 5c75 3230 3133 222c 0a20   "z":"\u2013",. 
+00002ca0: 2020 2020 2020 2022 6d62 6822 3a22 5c75         "mbh":"\u
+00002cb0: 3230 3133 222c 0a20 2020 2020 2020 2022  2013",.        "
+00002cc0: 7061 676e 7464 6522 3a32 2e34 3539 2c0a  pagntde":2.459,.
+00002cd0: 2020 2020 2020 2020 2263 6c61 7373 223a          "class":
+00002ce0: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
+00002cf0: 2020 2264 6622 3a30 2e34 2c0a 2020 2020    "df":0.4,.    
+00002d00: 2020 2020 2264 665f 6522 3a30 2e30 312c      "df_e":0.01,
+00002d10: 0a20 2020 2020 2020 2022 7261 223a 3333  .        "ra":33
+00002d20: 332e 3236 3932 3333 3731 3734 2c0a 2020  3.2692337174,.  
+00002d30: 2020 2020 2020 2264 6563 223a 3233 2e35        "dec":23.5
+00002d40: 3632 3032 3136 3633 2c0a 2020 2020 2020  62021663,.      
+00002d50: 2020 2241 6c6c 5749 5345 5f69 6422 3a33    "AllWISE_id":3
+00002d60: 3333 3531 3234 3230 3133 3531 3030 3834  3351242013510084
+00002d70: 3936 2c0a 2020 2020 2020 2020 2273 6570  96,.        "sep
+00002d80: 5f74 6f5f 5749 5345 5f73 6f75 7263 6522  _to_WISE_source"
+00002d90: 3a30 2e30 3638 3238 392c 0a20 2020 2020  :0.068289,.     
+00002da0: 2020 2022 7731 6d70 726f 223a 3133 2e36     "w1mpro":13.6
+00002db0: 3732 2c0a 2020 2020 2020 2020 2277 326d  72,.        "w2m
+00002dc0: 7072 6f22 3a31 322e 3635 0a20 2020 207d  pro":12.65.    }
+00002dd0: 2c0a 2020 2020 2232 3322 3a7b 0a20 2020  ,.    "23":{.   
+00002de0: 2020 2020 2022 6e61 6d65 223a 2241 5432       "name":"AT2
+00002df0: 3031 3964 6c6c 222c 0a20 2020 2020 2020  019dll",.       
+00002e00: 2022 7470 6561 6b22 3a35 3836 3035 2e32   "tpeak":58605.2
+00002e10: 2c0a 2020 2020 2020 2020 2272 6973 6574  ,.        "riset
+00002e20: 696d 6522 3a22 3239 2e36 222c 0a20 2020  ime":"29.6",.   
+00002e30: 2020 2020 2022 6661 6465 7469 6d65 223a       "fadetime":
+00002e40: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
+00002e50: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
+00002e60: 362e 382c 0a20 2020 2020 2020 2022 6466  6.8,.        "df
+00002e70: 5f72 6177 223a 2230 2e32 3620 5c75 3030  _raw":"0.26 \u00
+00002e80: 6231 2030 2e30 3122 2c0a 2020 2020 2020  b1 0.01",.      
+00002e90: 2020 227a 223a 2230 2e31 3031 222c 0a20    "z":"0.101",. 
+00002ea0: 2020 2020 2020 2022 6d62 6822 3a22 372e         "mbh":"7.
+00002eb0: 3438 2028 5431 3329 222c 0a20 2020 2020  48 (T13)",.     
+00002ec0: 2020 2022 7061 676e 7464 6522 3a33 2e34     "pagntde":3.4
+00002ed0: 3631 2c0a 2020 2020 2020 2020 2263 6c61  61,.        "cla
+00002ee0: 7373 223a 2254 4445 3f22 2c0a 2020 2020  ss":"TDE?",.    
+00002ef0: 2020 2020 2264 6622 3a30 2e32 362c 0a20      "df":0.26,. 
+00002f00: 2020 2020 2020 2022 6466 5f65 223a 302e         "df_e":0.
+00002f10: 3031 2c0a 2020 2020 2020 2020 2272 6122  01,.        "ra"
+00002f20: 3a31 3735 2e33 3437 3932 362c 0a20 2020  :175.347926,.   
+00002f30: 2020 2020 2022 6465 6322 3a32 312e 3933       "dec":21.93
+00002f40: 3638 3538 322c 0a20 2020 2020 2020 2022  68582,.        "
+00002f50: 416c 6c57 4953 455f 6964 223a 3137 3539  AllWISE_id":1759
+00002f60: 3132 3132 3031 3335 3130 3634 3030 392c  121201351064009,
+00002f70: 0a20 2020 2020 2020 2022 7365 705f 746f  .        "sep_to
+00002f80: 5f57 4953 455f 736f 7572 6365 223a 302e  _WISE_source":0.
+00002f90: 3133 3937 3336 2c0a 2020 2020 2020 2020  139736,.        
+00002fa0: 2277 316d 7072 6f22 3a31 342e 3035 342c  "w1mpro":14.054,
+00002fb0: 0a20 2020 2020 2020 2022 7732 6d70 726f  .        "w2mpro
+00002fc0: 223a 3133 2e37 3437 0a20 2020 207d 2c0a  ":13.747.    },.
+00002fd0: 2020 2020 2232 3422 3a7b 0a20 2020 2020      "24":{.     
+00002fe0: 2020 2022 6e61 6d65 223a 2241 5432 3031     "name":"AT201
+00002ff0: 3967 7572 222c 0a20 2020 2020 2020 2022  9gur",.        "
+00003000: 7470 6561 6b22 3a35 3836 3037 2e35 2c0a  tpeak":58607.5,.
+00003010: 2020 2020 2020 2020 2272 6973 6574 696d          "risetim
+00003020: 6522 3a22 5c75 3230 3133 222c 0a20 2020  e":"\u2013",.   
+00003030: 2020 2020 2022 6661 6465 7469 6d65 223a       "fadetime":
+00003040: 2232 3334 2e35 222c 0a20 2020 2020 2020  "234.5",.       
+00003050: 2022 6466 5f6f 7665 725f 726d 7322 3a33   "df_over_rms":3
+00003060: 382e 362c 0a20 2020 2020 2020 2022 6466  8.6,.        "df
+00003070: 5f72 6177 223a 2230 2e33 3420 5c75 3030  _raw":"0.34 \u00
+00003080: 6231 2030 2e30 3122 2c0a 2020 2020 2020  b1 0.01",.      
+00003090: 2020 227a 223a 225c 7532 3031 3322 2c0a    "z":"\u2013",.
+000030a0: 2020 2020 2020 2020 226d 6268 223a 225c          "mbh":"\
+000030b0: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
+000030c0: 2270 6167 6e74 6465 223a 302e 302c 0a20  "pagntde":0.0,. 
+000030d0: 2020 2020 2020 2022 636c 6173 7322 3a22         "class":"
+000030e0: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
+000030f0: 2022 6466 223a 302e 3334 2c0a 2020 2020   "df":0.34,.    
+00003100: 2020 2020 2264 665f 6522 3a30 2e30 312c      "df_e":0.01,
+00003110: 0a20 2020 2020 2020 2022 7261 223a 3334  .        "ra":34
+00003120: 332e 3730 3332 3635 322c 0a20 2020 2020  3.7032652,.     
+00003130: 2020 2022 6465 6322 3a37 372e 3335 3239     "dec":77.3529
+00003140: 3637 342c 0a20 2020 2020 2020 2022 416c  674,.        "Al
+00003150: 6c57 4953 455f 6964 223a 3334 3037 3137  lWISE_id":340717
+00003160: 3732 3031 3335 3130 3232 3330 362c 0a20  7201351022306,. 
+00003170: 2020 2020 2020 2022 7365 705f 746f 5f57         "sep_to_W
+00003180: 4953 455f 736f 7572 6365 223a 302e 3234  ISE_source":0.24
+00003190: 3130 3039 2c0a 2020 2020 2020 2020 2277  1009,.        "w
+000031a0: 316d 7072 6f22 3a31 352e 3539 352c 0a20  1mpro":15.595,. 
+000031b0: 2020 2020 2020 2022 7732 6d70 726f 223a         "w2mpro":
+000031c0: 3134 2e38 3739 0a20 2020 207d 2c0a 2020  14.879.    },.  
+000031d0: 2020 2232 3522 3a7b 0a20 2020 2020 2020    "25":{.       
+000031e0: 2022 6e61 6d65 223a 2241 5432 3031 386c   "name":"AT2018l
+000031f0: 6f66 222c 0a20 2020 2020 2020 2022 7470  of",.        "tp
+00003200: 6561 6b22 3a35 3836 3038 2e32 2c0a 2020  eak":58608.2,.  
+00003210: 2020 2020 2020 2272 6973 6574 696d 6522        "risetime"
+00003220: 3a22 3730 2e39 222c 0a20 2020 2020 2020  :"70.9",.       
+00003230: 2022 6661 6465 7469 6d65 223a 2233 3730   "fadetime":"370
+00003240: 2e34 222c 0a20 2020 2020 2020 2022 6466  .4",.        "df
+00003250: 5f6f 7665 725f 726d 7322 3a34 2e31 2c0a  _over_rms":4.1,.
+00003260: 2020 2020 2020 2020 2264 665f 7261 7722          "df_raw"
+00003270: 3a22 302e 3135 205c 7530 3062 3120 302e  :"0.15 \u00b1 0.
+00003280: 3031 222c 0a20 2020 2020 2020 2022 7a22  01",.        "z"
+00003290: 3a22 302e 3330 3222 2c0a 2020 2020 2020  :"0.302",.      
+000032a0: 2020 226d 6268 223a 2238 2e39 3820 284c    "mbh":"8.98 (L
+000032b0: 3139 2922 2c0a 2020 2020 2020 2020 2270  19)",.        "p
+000032c0: 6167 6e74 6465 223a 352e 3937 342c 0a20  agntde":5.974,. 
+000032d0: 2020 2020 2020 2022 636c 6173 7322 3a22         "class":"
+000032e0: 4147 4e22 2c0a 2020 2020 2020 2020 2264  AGN",.        "d
+000032f0: 6622 3a30 2e31 352c 0a20 2020 2020 2020  f":0.15,.       
+00003300: 2022 6466 5f65 223a 302e 3031 2c0a 2020   "df_e":0.01,.  
+00003310: 2020 2020 2020 2272 6122 3a31 3335 2e32        "ra":135.2
+00003320: 3533 3731 3331 2c0a 2020 2020 2020 2020  537131,.        
+00003330: 2264 6563 223a 3335 2e36 3335 3533 3931  "dec":35.6355391
+00003340: 2c0a 2020 2020 2020 2020 2241 6c6c 5749  ,.        "AllWI
+00003350: 5345 5f69 6422 3a31 3336 3131 3336 3330  SE_id":136113630
+00003360: 3133 3531 3031 3030 3833 2c0a 2020 2020  1351010083,.    
+00003370: 2020 2020 2273 6570 5f74 6f5f 5749 5345      "sep_to_WISE
+00003380: 5f73 6f75 7263 6522 3a30 2e39 3131 3432  _source":0.91142
+00003390: 342c 0a20 2020 2020 2020 2022 7731 6d70  4,.        "w1mp
+000033a0: 726f 223a 3134 2e32 3737 2c0a 2020 2020  ro":14.277,.    
+000033b0: 2020 2020 2277 326d 7072 6f22 3a31 332e      "w2mpro":13.
+000033c0: 3432 330a 2020 2020 7d2c 0a20 2020 2022  423.    },.    "
+000033d0: 3236 223a 7b0a 2020 2020 2020 2020 226e  26":{.        "n
+000033e0: 616d 6522 3a22 4154 3230 3139 6471 7622  ame":"AT2019dqv"
+000033f0: 2c0a 2020 2020 2020 2020 2274 7065 616b  ,.        "tpeak
+00003400: 223a 3538 3632 382e 322c 0a20 2020 2020  ":58628.2,.     
+00003410: 2020 2022 7269 7365 7469 6d65 223a 2236     "risetime":"6
+00003420: 372e 3022 2c0a 2020 2020 2020 2020 2266  7.0",.        "f
+00003430: 6164 6574 696d 6522 3a22 3437 352e 3022  adetime":"475.0"
+00003440: 2c0a 2020 2020 2020 2020 2264 665f 6f76  ,.        "df_ov
+00003450: 6572 5f72 6d73 223a 3430 2e34 2c0a 2020  er_rms":40.4,.  
+00003460: 2020 2020 2020 2264 665f 7261 7722 3a22        "df_raw":"
+00003470: 312e 3737 205c 7530 3062 3120 302e 3032  1.77 \u00b1 0.02
+00003480: 222c 0a20 2020 2020 2020 2022 7a22 3a22  ",.        "z":"
+00003490: 302e 3038 3136 222c 0a20 2020 2020 2020  0.0816",.       
+000034a0: 2022 6d62 6822 3a22 362e 3637 2028 4c31   "mbh":"6.67 (L1
+000034b0: 3929 222c 0a20 2020 2020 2020 2022 7061  9)",.        "pa
+000034c0: 676e 7464 6522 3a30 2e30 2c0a 2020 2020  gntde":0.0,.    
+000034d0: 2020 2020 2263 6c61 7373 223a 2254 4445      "class":"TDE
+000034e0: 3f22 2c0a 2020 2020 2020 2020 2264 6622  ?",.        "df"
+000034f0: 3a31 2e37 372c 0a20 2020 2020 2020 2022  :1.77,.        "
+00003500: 6466 5f65 223a 302e 3032 2c0a 2020 2020  df_e":0.02,.    
+00003510: 2020 2020 2272 6122 3a31 3630 2e38 3735      "ra":160.875
+00003520: 3235 2c0a 2020 2020 2020 2020 2264 6563  25,.        "dec
+00003530: 223a 3531 2e33 3538 3035 2c0a 2020 2020  ":51.35805,.    
+00003540: 2020 2020 2241 6c6c 5749 5345 5f69 6422      "AllWISE_id"
+00003550: 3a31 3539 3731 3531 3430 3133 3531 3032  :159715140135102
+00003560: 3633 3836 2c0a 2020 2020 2020 2020 2273  6386,.        "s
+00003570: 6570 5f74 6f5f 5749 5345 5f73 6f75 7263  ep_to_WISE_sourc
+00003580: 6522 3a30 2e30 3338 3734 362c 0a20 2020  e":0.038746,.   
+00003590: 2020 2020 2022 7731 6d70 726f 223a 3133       "w1mpro":13
+000035a0: 2e36 332c 0a20 2020 2020 2020 2022 7732  .63,.        "w2
+000035b0: 6d70 726f 223a 3133 2e30 3132 0a20 2020  mpro":13.012.   
+000035c0: 207d 2c0a 2020 2020 2232 3722 3a7b 0a20   },.    "27":{. 
+000035d0: 2020 2020 2020 2022 6e61 6d65 223a 2241         "name":"A
+000035e0: 5432 3031 3963 7971 222c 0a20 2020 2020  T2019cyq",.     
+000035f0: 2020 2022 7470 6561 6b22 3a35 3836 3337     "tpeak":58637
+00003600: 2e32 2c0a 2020 2020 2020 2020 2272 6973  .2,.        "ris
+00003610: 6574 696d 6522 3a22 3439 2e35 222c 0a20  etime":"49.5",. 
+00003620: 2020 2020 2020 2022 6661 6465 7469 6d65         "fadetime
+00003630: 223a 2239 352e 3022 2c0a 2020 2020 2020  ":"95.0",.      
+00003640: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
+00003650: 3331 2e38 2c0a 2020 2020 2020 2020 2264  31.8,.        "d
+00003660: 665f 7261 7722 3a22 302e 3534 205c 7530  f_raw":"0.54 \u0
+00003670: 3062 3120 302e 3031 222c 0a20 2020 2020  0b1 0.01",.     
+00003680: 2020 2022 7a22 3a22 302e 3236 3222 2c0a     "z":"0.262",.
+00003690: 2020 2020 2020 2020 226d 6268 223a 2237          "mbh":"7
+000036a0: 2e35 3620 284c 3139 2922 2c0a 2020 2020  .56 (L19)",.    
+000036b0: 2020 2020 2270 6167 6e74 6465 223a 302e      "pagntde":0.
+000036c0: 302c 0a20 2020 2020 2020 2022 636c 6173  0,.        "clas
+000036d0: 7322 3a22 5444 453f 222c 0a20 2020 2020  s":"TDE?",.     
+000036e0: 2020 2022 6466 223a 302e 3534 2c0a 2020     "df":0.54,.  
+000036f0: 2020 2020 2020 2264 665f 6522 3a30 2e30        "df_e":0.0
+00003700: 312c 0a20 2020 2020 2020 2022 7261 223a  1,.        "ra":
+00003710: 3134 392e 3032 3532 352c 0a20 2020 2020  149.02525,.     
+00003720: 2020 2022 6465 6322 3a31 392e 3534 3930     "dec":19.5490
+00003730: 3339 2c0a 2020 2020 2020 2020 2241 6c6c  39,.        "All
+00003740: 5749 5345 5f69 6422 3a31 3438 3831 3139  WISE_id":1488119
+00003750: 3630 3133 3531 3032 3830 3332 2c0a 2020  601351028032,.  
+00003760: 2020 2020 2020 2273 6570 5f74 6f5f 5749        "sep_to_WI
+00003770: 5345 5f73 6f75 7263 6522 3a30 2e30 3737  SE_source":0.077
+00003780: 3331 322c 0a20 2020 2020 2020 2022 7731  312,.        "w1
+00003790: 6d70 726f 223a 3135 2e30 342c 0a20 2020  mpro":15.04,.   
+000037a0: 2020 2020 2022 7732 6d70 726f 223a 3134       "w2mpro":14
+000037b0: 2e34 3339 0a20 2020 207d 2c0a 2020 2020  .439.    },.    
+000037c0: 2232 3822 3a7b 0a20 2020 2020 2020 2022  "28":{.        "
+000037d0: 6e61 6d65 223a 2241 5432 3032 3161 6575  name":"AT2021aeu
+000037e0: 6722 2c0a 2020 2020 2020 2020 2274 7065  g",.        "tpe
+000037f0: 616b 223a 3538 3634 312e 322c 0a20 2020  ak":58641.2,.   
+00003800: 2020 2020 2022 7269 7365 7469 6d65 223a       "risetime":
+00003810: 2234 382e 3622 2c0a 2020 2020 2020 2020  "48.6",.        
+00003820: 2266 6164 6574 696d 6522 3a22 3638 2e38  "fadetime":"68.8
+00003830: 222c 0a20 2020 2020 2020 2022 6466 5f6f  ",.        "df_o
+00003840: 7665 725f 726d 7322 3a34 2e36 2c0a 2020  ver_rms":4.6,.  
+00003850: 2020 2020 2020 2264 665f 7261 7722 3a22        "df_raw":"
+00003860: 302e 3131 205c 7530 3062 3120 302e 3031  0.11 \u00b1 0.01
+00003870: 222c 0a20 2020 2020 2020 2022 7a22 3a22  ",.        "z":"
+00003880: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
+00003890: 2022 6d62 6822 3a22 5c75 3230 3133 222c   "mbh":"\u2013",
+000038a0: 0a20 2020 2020 2020 2022 7061 676e 7464  .        "pagntd
+000038b0: 6522 3a36 2e30 372c 0a20 2020 2020 2020  e":6.07,.       
+000038c0: 2022 636c 6173 7322 3a22 5c75 3230 3133   "class":"\u2013
+000038d0: 222c 0a20 2020 2020 2020 2022 6466 223a  ",.        "df":
+000038e0: 302e 3131 2c0a 2020 2020 2020 2020 2264  0.11,.        "d
+000038f0: 665f 6522 3a30 2e30 312c 0a20 2020 2020  f_e":0.01,.     
+00003900: 2020 2022 7261 223a 3233 372e 3536 3639     "ra":237.5669
+00003910: 3932 3434 3439 2c0a 2020 2020 2020 2020  924449,.        
+00003920: 2264 6563 223a 3339 2e32 3336 3431 3439  "dec":39.2364149
+00003930: 3933 342c 0a20 2020 2020 2020 2022 416c  934,.        "Al
+00003940: 6c57 4953 455f 6964 223a 3233 3830 3133  lWISE_id":238013
+00003950: 3933 3031 3335 3130 3334 3135 392c 0a20  9301351034159,. 
+00003960: 2020 2020 2020 2022 7365 705f 746f 5f57         "sep_to_W
+00003970: 4953 455f 736f 7572 6365 223a 302e 3039  ISE_source":0.09
+00003980: 3234 3334 2c0a 2020 2020 2020 2020 2277  2434,.        "w
+00003990: 316d 7072 6f22 3a31 342e 3135 332c 0a20  1mpro":14.153,. 
+000039a0: 2020 2020 2020 2022 7732 6d70 726f 223a         "w2mpro":
+000039b0: 3133 2e35 3131 0a20 2020 207d 2c0a 2020  13.511.    },.  
+000039c0: 2020 2232 3922 3a7b 0a20 2020 2020 2020    "29":{.       
+000039d0: 2022 6e61 6d65 223a 2241 5432 3031 3969   "name":"AT2019i
+000039e0: 6876 222c 0a20 2020 2020 2020 2022 7470  hv",.        "tp
+000039f0: 6561 6b22 3a35 3836 3436 2e35 2c0a 2020  eak":58646.5,.  
+00003a00: 2020 2020 2020 2272 6973 6574 696d 6522        "risetime"
+00003a10: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
+00003a20: 2020 2022 6661 6465 7469 6d65 223a 2231     "fadetime":"1
+00003a30: 392e 3322 2c0a 2020 2020 2020 2020 2264  9.3",.        "d
+00003a40: 665f 6f76 6572 5f72 6d73 223a 382e 372c  f_over_rms":8.7,
+00003a50: 0a20 2020 2020 2020 2022 6466 5f72 6177  .        "df_raw
+00003a60: 223a 2230 2e32 3920 5c75 3030 6231 2030  ":"0.29 \u00b1 0
+00003a70: 2e30 3122 2c0a 2020 2020 2020 2020 227a  .01",.        "z
+00003a80: 223a 2230 2e31 3630 3222 2c0a 2020 2020  ":"0.1602",.    
+00003a90: 2020 2020 226d 6268 223a 225c 7532 3031      "mbh":"\u201
+00003aa0: 3322 2c0a 2020 2020 2020 2020 2270 6167  3",.        "pag
+00003ab0: 6e74 6465 223a 312e 3638 372c 0a20 2020  ntde":1.687,.   
+00003ac0: 2020 2020 2022 636c 6173 7322 3a22 5c75       "class":"\u
+00003ad0: 3230 3133 222c 0a20 2020 2020 2020 2022  2013",.        "
+00003ae0: 6466 223a 302e 3239 2c0a 2020 2020 2020  df":0.29,.      
+00003af0: 2020 2264 665f 6522 3a30 2e30 312c 0a20    "df_e":0.01,. 
+00003b00: 2020 2020 2020 2022 7261 223a 3136 2e39         "ra":16.9
+00003b10: 3439 3637 3235 2c0a 2020 2020 2020 2020  496725,.        
+00003b20: 2264 6563 223a 3234 2e34 3830 3038 382c  "dec":24.480088,
+00003b30: 0a20 2020 2020 2020 2022 416c 6c57 4953  .        "AllWIS
+00003b40: 455f 6964 223a 3136 3531 3234 3230 3133  E_id":1651242013
+00003b50: 3531 3034 3637 3038 2c0a 2020 2020 2020  51046708,.      
+00003b60: 2020 2273 6570 5f74 6f5f 5749 5345 5f73    "sep_to_WISE_s
+00003b70: 6f75 7263 6522 3a30 2e34 3434 3034 362c  ource":0.444046,
+00003b80: 0a20 2020 2020 2020 2022 7731 6d70 726f  .        "w1mpro
+00003b90: 223a 3133 2e39 3131 2c0a 2020 2020 2020  ":13.911,.      
+00003ba0: 2020 2277 326d 7072 6f22 3a31 332e 3338    "w2mpro":13.38
+00003bb0: 0a20 2020 207d 2c0a 2020 2020 2233 3022  .    },.    "30"
+00003bc0: 3a7b 0a20 2020 2020 2020 2022 6e61 6d65  :{.        "name
+00003bd0: 223a 2241 5432 3031 3964 7a68 222c 0a20  ":"AT2019dzh",. 
+00003be0: 2020 2020 2020 2022 7470 6561 6b22 3a35         "tpeak":5
+00003bf0: 3836 3531 2e32 2c0a 2020 2020 2020 2020  8651.2,.        
+00003c00: 2272 6973 6574 696d 6522 3a22 3531 2e34  "risetime":"51.4
+00003c10: 222c 0a20 2020 2020 2020 2022 6661 6465  ",.        "fade
+00003c20: 7469 6d65 223a 2233 3438 2e39 222c 0a20  time":"348.9",. 
+00003c30: 2020 2020 2020 2022 6466 5f6f 7665 725f         "df_over_
+00003c40: 726d 7322 3a36 2e34 2c0a 2020 2020 2020  rms":6.4,.      
+00003c50: 2020 2264 665f 7261 7722 3a22 302e 3135    "df_raw":"0.15
+00003c60: 205c 7530 3062 3120 302e 3031 222c 0a20   \u00b1 0.01",. 
+00003c70: 2020 2020 2020 2022 7a22 3a22 302e 3331         "z":"0.31
+00003c80: 3422 2c0a 2020 2020 2020 2020 226d 6268  4",.        "mbh
+00003c90: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
+00003ca0: 2020 2020 2270 6167 6e74 6465 223a 342e      "pagntde":4.
+00003cb0: 3030 372c 0a20 2020 2020 2020 2022 636c  007,.        "cl
+00003cc0: 6173 7322 3a22 5c75 3230 3133 222c 0a20  ass":"\u2013",. 
+00003cd0: 2020 2020 2020 2022 6466 223a 302e 3135         "df":0.15
+00003ce0: 2c0a 2020 2020 2020 2020 2264 665f 6522  ,.        "df_e"
+00003cf0: 3a30 2e30 312c 0a20 2020 2020 2020 2022  :0.01,.        "
+00003d00: 7261 223a 3138 372e 3832 3532 372c 0a20  ra":187.82527,. 
+00003d10: 2020 2020 2020 2022 6465 6322 3a32 332e         "dec":23.
+00003d20: 3730 3731 3436 3636 3637 2c0a 2020 2020  7071466667,.    
+00003d30: 2020 2020 2241 6c6c 5749 5345 5f69 6422      "AllWISE_id"
+00003d40: 3a31 3838 3231 3234 3230 3133 3531 3030  :188212420135100
+00003d50: 3832 3338 2c0a 2020 2020 2020 2020 2273  8238,.        "s
+00003d60: 6570 5f74 6f5f 5749 5345 5f73 6f75 7263  ep_to_WISE_sourc
+00003d70: 6522 3a31 2e36 3836 3435 362c 0a20 2020  e":1.686456,.   
+00003d80: 2020 2020 2022 7731 6d70 726f 223a 3135       "w1mpro":15
+00003d90: 2e38 3031 2c0a 2020 2020 2020 2020 2277  .801,.        "w
+00003da0: 326d 7072 6f22 3a31 352e 3038 0a20 2020  2mpro":15.08.   
+00003db0: 207d 2c0a 2020 2020 2233 3122 3a7b 0a20   },.    "31":{. 
+00003dc0: 2020 2020 2020 2022 6e61 6d65 223a 2241         "name":"A
+00003dd0: 5432 3031 396b 7175 222c 0a20 2020 2020  T2019kqu",.     
+00003de0: 2020 2022 7470 6561 6b22 3a35 3836 3532     "tpeak":58652
+00003df0: 2e32 2c0a 2020 2020 2020 2020 2272 6973  .2,.        "ris
+00003e00: 6574 696d 6522 3a22 3935 2e36 222c 0a20  etime":"95.6",. 
+00003e10: 2020 2020 2020 2022 6661 6465 7469 6d65         "fadetime
+00003e20: 223a 2233 3135 2e36 222c 0a20 2020 2020  ":"315.6",.     
+00003e30: 2020 2022 6466 5f6f 7665 725f 726d 7322     "df_over_rms"
+00003e40: 3a36 2e31 2c0a 2020 2020 2020 2020 2264  :6.1,.        "d
+00003e50: 665f 7261 7722 3a22 302e 3237 205c 7530  f_raw":"0.27 \u0
+00003e60: 3062 3120 302e 3031 222c 0a20 2020 2020  0b1 0.01",.     
+00003e70: 2020 2022 7a22 3a22 302e 3137 3422 2c0a     "z":"0.174",.
+00003e80: 2020 2020 2020 2020 226d 6268 223a 2237          "mbh":"7
+00003e90: 2e35 3320 284c 3139 2922 2c0a 2020 2020  .53 (L19)",.    
+00003ea0: 2020 2020 2270 6167 6e74 6465 223a 342e      "pagntde":4.
+00003eb0: 3334 382c 0a20 2020 2020 2020 2022 636c  348,.        "cl
+00003ec0: 6173 7322 3a22 5444 453f 222c 0a20 2020  ass":"TDE?",.   
+00003ed0: 2020 2020 2022 6466 223a 302e 3237 2c0a       "df":0.27,.
+00003ee0: 2020 2020 2020 2020 2264 665f 6522 3a30          "df_e":0
+00003ef0: 2e30 312c 0a20 2020 2020 2020 2022 7261  .01,.        "ra
+00003f00: 223a 3234 382e 3036 3138 3735 2c0a 2020  ":248.061875,.  
+00003f10: 2020 2020 2020 2264 6563 223a 3333 2e35        "dec":33.5
+00003f20: 3730 3231 312c 0a20 2020 2020 2020 2022  70211,.        "
+00003f30: 416c 6c57 4953 455f 6964 223a 3234 3833  AllWISE_id":2483
+00003f40: 3133 3333 3031 3335 3130 3337 3232 312c  133301351037221,
+00003f50: 0a20 2020 2020 2020 2022 7365 705f 746f  .        "sep_to
+00003f60: 5f57 4953 455f 736f 7572 6365 223a 302e  _WISE_source":0.
+00003f70: 3235 3334 3933 2c0a 2020 2020 2020 2020  253493,.        
+00003f80: 2277 316d 7072 6f22 3a31 332e 3931 342c  "w1mpro":13.914,
+00003f90: 0a20 2020 2020 2020 2022 7732 6d70 726f  .        "w2mpro
+00003fa0: 223a 3133 2e32 3034 0a20 2020 207d 2c0a  ":13.204.    },.
+00003fb0: 2020 2020 2233 3222 3a7b 0a20 2020 2020      "32":{.     
+00003fc0: 2020 2022 6e61 6d65 223a 2241 5432 3031     "name":"AT201
+00003fd0: 3968 6268 222c 0a20 2020 2020 2020 2022  9hbh",.        "
+00003fe0: 7470 6561 6b22 3a35 3836 3532 2e33 2c0a  tpeak":58652.3,.
+00003ff0: 2020 2020 2020 2020 2272 6973 6574 696d          "risetim
+00004000: 6522 3a22 3139 2e38 222c 0a20 2020 2020  e":"19.8",.     
+00004010: 2020 2022 6661 6465 7469 6d65 223a 2231     "fadetime":"1
+00004020: 3036 2e37 222c 0a20 2020 2020 2020 2022  06.7",.        "
+00004030: 6466 5f6f 7665 725f 726d 7322 3a38 2e34  df_over_rms":8.4
+00004040: 2c0a 2020 2020 2020 2020 2264 665f 7261  ,.        "df_ra
+00004050: 7722 3a22 302e 3735 205c 7530 3062 3120  w":"0.75 \u00b1 
+00004060: 302e 3031 222c 0a20 2020 2020 2020 2022  0.01",.        "
+00004070: 7a22 3a22 5c75 3230 3133 222c 0a20 2020  z":"\u2013",.   
+00004080: 2020 2020 2022 6d62 6822 3a22 5c75 3230       "mbh":"\u20
+00004090: 3133 222c 0a20 2020 2020 2020 2022 7061  13",.        "pa
+000040a0: 676e 7464 6522 3a31 2e38 382c 0a20 2020  gntde":1.88,.   
+000040b0: 2020 2020 2022 636c 6173 7322 3a22 5c75       "class":"\u
+000040c0: 3230 3133 222c 0a20 2020 2020 2020 2022  2013",.        "
+000040d0: 6466 223a 302e 3735 2c0a 2020 2020 2020  df":0.75,.      
+000040e0: 2020 2264 665f 6522 3a30 2e30 312c 0a20    "df_e":0.01,. 
+000040f0: 2020 2020 2020 2022 7261 223a 3237 382e         "ra":278.
+00004100: 3333 3039 3033 382c 0a20 2020 2020 2020  3309038,.       
+00004110: 2022 6465 6322 3a33 342e 3638 3432 3232   "dec":34.684222
+00004120: 352c 0a20 2020 2020 2020 2022 416c 6c57  5,.        "AllW
+00004130: 4953 455f 6964 223a 3237 3737 3133 3438  ISE_id":27771348
+00004140: 3031 3335 3130 3330 3031 392c 0a20 2020  01351030019,.   
+00004150: 2020 2020 2022 7365 705f 746f 5f57 4953       "sep_to_WIS
+00004160: 455f 736f 7572 6365 223a 302e 3631 3539  E_source":0.6159
+00004170: 3039 2c0a 2020 2020 2020 2020 2277 316d  09,.        "w1m
+00004180: 7072 6f22 3a31 342e 3932 2c0a 2020 2020  pro":14.92,.    
+00004190: 2020 2020 2277 326d 7072 6f22 3a31 342e      "w2mpro":14.
+000041a0: 3630 340a 2020 2020 7d2c 0a20 2020 2022  604.    },.    "
+000041b0: 3333 223a 7b0a 2020 2020 2020 2020 226e  33":{.        "n
+000041c0: 616d 6522 3a22 4154 3230 3230 6165 7a7a  ame":"AT2020aezz
+000041d0: 222c 0a20 2020 2020 2020 2022 7470 6561  ",.        "tpea
+000041e0: 6b22 3a35 3836 3737 2e33 2c0a 2020 2020  k":58677.3,.    
+000041f0: 2020 2020 2272 6973 6574 696d 6522 3a22      "risetime":"
+00004200: 3939 2e38 222c 0a20 2020 2020 2020 2022  99.8",.        "
+00004210: 6661 6465 7469 6d65 223a 2232 3830 2e36  fadetime":"280.6
+00004220: 222c 0a20 2020 2020 2020 2022 6466 5f6f  ",.        "df_o
+00004230: 7665 725f 726d 7322 3a35 2e38 2c0a 2020  ver_rms":5.8,.  
+00004240: 2020 2020 2020 2264 665f 7261 7722 3a22        "df_raw":"
+00004250: 302e 3138 205c 7530 3062 3120 302e 3031  0.18 \u00b1 0.01
+00004260: 222c 0a20 2020 2020 2020 2022 7a22 3a22  ",.        "z":"
+00004270: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
+00004280: 2022 6d62 6822 3a22 5c75 3230 3133 222c   "mbh":"\u2013",
+00004290: 0a20 2020 2020 2020 2022 7061 676e 7464  .        "pagntd
+000042a0: 6522 3a34 2e37 3731 2c0a 2020 2020 2020  e":4.771,.      
+000042b0: 2020 2263 6c61 7373 223a 225c 7532 3031    "class":"\u201
+000042c0: 3322 2c0a 2020 2020 2020 2020 2264 6622  3",.        "df"
+000042d0: 3a30 2e31 382c 0a20 2020 2020 2020 2022  :0.18,.        "
+000042e0: 6466 5f65 223a 302e 3031 2c0a 2020 2020  df_e":0.01,.    
+000042f0: 2020 2020 2272 6122 3a32 3637 2e30 3635      "ra":267.065
+00004300: 3139 3333 3437 392c 0a20 2020 2020 2020  1933479,.       
+00004310: 2022 6465 6322 3a35 352e 3233 3639 3735   "dec":55.236975
+00004320: 3036 3931 2c0a 2020 2020 2020 2020 2241  0691,.        "A
+00004330: 6c6c 5749 5345 5f69 6422 3a32 3638 3031  llWISE_id":26801
+00004340: 3534 3530 3133 3531 3036 3130 3534 2c0a  54501351061054,.
+00004350: 2020 2020 2020 2020 2273 6570 5f74 6f5f          "sep_to_
+00004360: 5749 5345 5f73 6f75 7263 6522 3a30 2e31  WISE_source":0.1
+00004370: 3931 3337 392c 0a20 2020 2020 2020 2022  91379,.        "
+00004380: 7731 6d70 726f 223a 3134 2e35 3236 2c0a  w1mpro":14.526,.
+00004390: 2020 2020 2020 2020 2277 326d 7072 6f22          "w2mpro"
+000043a0: 3a31 332e 3938 380a 2020 2020 7d2c 0a20  :13.988.    },. 
+000043b0: 2020 2022 3334 223a 7b0a 2020 2020 2020     "34":{.      
+000043c0: 2020 226e 616d 6522 3a22 4154 3230 3230    "name":"AT2020
+000043d0: 6166 6161 222c 0a20 2020 2020 2020 2022  afaa",.        "
+000043e0: 7470 6561 6b22 3a35 3836 3738 2e32 2c0a  tpeak":58678.2,.
+000043f0: 2020 2020 2020 2020 2272 6973 6574 696d          "risetim
+00004400: 6522 3a22 3833 2e38 222c 0a20 2020 2020  e":"83.8",.     
+00004410: 2020 2022 6661 6465 7469 6d65 223a 2233     "fadetime":"3
+00004420: 3330 2e33 222c 0a20 2020 2020 2020 2022  30.3",.        "
+00004430: 6466 5f6f 7665 725f 726d 7322 3a37 2e30  df_over_rms":7.0
+00004440: 2c0a 2020 2020 2020 2020 2264 665f 7261  ,.        "df_ra
+00004450: 7722 3a22 302e 3133 205c 7530 3062 3120  w":"0.13 \u00b1 
+00004460: 302e 3032 222c 0a20 2020 2020 2020 2022  0.02",.        "
+00004470: 7a22 3a22 5c75 3230 3133 222c 0a20 2020  z":"\u2013",.   
+00004480: 2020 2020 2022 6d62 6822 3a22 5c75 3230       "mbh":"\u20
+00004490: 3133 222c 0a20 2020 2020 2020 2022 7061  13",.        "pa
+000044a0: 676e 7464 6522 3a33 2e31 3837 2c0a 2020  gntde":3.187,.  
+000044b0: 2020 2020 2020 2263 6c61 7373 223a 225c        "class":"\
+000044c0: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
+000044d0: 2264 6622 3a30 2e31 332c 0a20 2020 2020  "df":0.13,.     
+000044e0: 2020 2022 6466 5f65 223a 302e 3032 2c0a     "df_e":0.02,.
+000044f0: 2020 2020 2020 2020 2272 6122 3a32 3039          "ra":209
+00004500: 2e36 3730 3339 3932 3239 312c 0a20 2020  .6703992291,.   
+00004510: 2020 2020 2022 6465 6322 3a32 342e 3731       "dec":24.71
+00004520: 3139 3438 3836 2c0a 2020 2020 2020 2020  194886,.        
+00004530: 2241 6c6c 5749 5345 5f69 6422 3a32 3039  "AllWISE_id":209
+00004540: 3731 3234 3230 3133 3531 3034 3837 3435  7124201351048745
+00004550: 2c0a 2020 2020 2020 2020 2273 6570 5f74  ,.        "sep_t
+00004560: 6f5f 5749 5345 5f73 6f75 7263 6522 3a30  o_WISE_source":0
+00004570: 2e32 3337 3330 382c 0a20 2020 2020 2020  .237308,.       
+00004580: 2022 7731 6d70 726f 223a 3135 2e35 3634   "w1mpro":15.564
+00004590: 2c0a 2020 2020 2020 2020 2277 326d 7072  ,.        "w2mpr
+000045a0: 6f22 3a31 342e 3738 360a 2020 2020 7d2c  o":14.786.    },
+000045b0: 0a20 2020 2022 3335 223a 7b0a 2020 2020  .    "35":{.    
+000045c0: 2020 2020 226e 616d 6522 3a22 4154 3230      "name":"AT20
+000045d0: 3139 6964 6d22 2c0a 2020 2020 2020 2020  19idm",.        
+000045e0: 2274 7065 616b 223a 3538 3638 322e 322c  "tpeak":58682.2,
+000045f0: 0a20 2020 2020 2020 2022 7269 7365 7469  .        "riseti
+00004600: 6d65 223a 2235 312e 3722 2c0a 2020 2020  me":"51.7",.    
+00004610: 2020 2020 2266 6164 6574 696d 6522 3a22      "fadetime":"
+00004620: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
+00004630: 2022 6466 5f6f 7665 725f 726d 7322 3a32   "df_over_rms":2
+00004640: 352e 322c 0a20 2020 2020 2020 2022 6466  5.2,.        "df
+00004650: 5f72 6177 223a 2230 2e34 3120 5c75 3030  _raw":"0.41 \u00
+00004660: 6231 2030 2e30 3222 2c0a 2020 2020 2020  b1 0.02",.      
+00004670: 2020 227a 223a 2230 2e30 3534 3422 2c0a    "z":"0.0544",.
+00004680: 2020 2020 2020 2020 226d 6268 223a 2236          "mbh":"6
+00004690: 2e36 3420 2854 3133 2922 2c0a 2020 2020  .64 (T13)",.    
+000046a0: 2020 2020 2270 6167 6e74 6465 223a 302e      "pagntde":0.
+000046b0: 3030 322c 0a20 2020 2020 2020 2022 636c  002,.        "cl
+000046c0: 6173 7322 3a22 5444 453f 222c 0a20 2020  ass":"TDE?",.   
+000046d0: 2020 2020 2022 6466 223a 302e 3431 2c0a       "df":0.41,.
+000046e0: 2020 2020 2020 2020 2264 665f 6522 3a30          "df_e":0
+000046f0: 2e30 322c 0a20 2020 2020 2020 2022 7261  .02,.        "ra
+00004700: 223a 3230 382e 3139 3532 352c 0a20 2020  ":208.19525,.   
+00004710: 2020 2020 2022 6465 6322 3a32 302e 3431       "dec":20.41
+00004720: 3231 3831 2c0a 2020 2020 2020 2020 2241  2181,.        "A
+00004730: 6c6c 5749 5345 5f69 6422 3a32 3038 3031  llWISE_id":20801
+00004740: 3139 3630 3133 3531 3035 3035 3431 2c0a  19601351050541,.
+00004750: 2020 2020 2020 2020 2273 6570 5f74 6f5f          "sep_to_
+00004760: 5749 5345 5f73 6f75 7263 6522 3a30 2e32  WISE_source":0.2
+00004770: 3336 3930 352c 0a20 2020 2020 2020 2022  36905,.        "
+00004780: 7731 6d70 726f 223a 3133 2e36 3633 2c0a  w1mpro":13.663,.
+00004790: 2020 2020 2020 2020 2277 326d 7072 6f22          "w2mpro"
+000047a0: 3a31 332e 3537 380a 2020 2020 7d2c 0a20  :13.578.    },. 
+000047b0: 2020 2022 3336 223a 7b0a 2020 2020 2020     "36":{.      
+000047c0: 2020 226e 616d 6522 3a22 4154 3230 3139    "name":"AT2019
+000047d0: 6968 7522 2c0a 2020 2020 2020 2020 2274  ihu",.        "t
+000047e0: 7065 616b 223a 3538 3730 392e 352c 0a20  peak":58709.5,. 
+000047f0: 2020 2020 2020 2022 7269 7365 7469 6d65         "risetime
+00004800: 223a 2237 392e 3722 2c0a 2020 2020 2020  ":"79.7",.      
+00004810: 2020 2266 6164 6574 696d 6522 3a22 3131    "fadetime":"11
+00004820: 302e 3922 2c0a 2020 2020 2020 2020 2264  0.9",.        "d
+00004830: 665f 6f76 6572 5f72 6d73 223a 362e 322c  f_over_rms":6.2,
+00004840: 0a20 2020 2020 2020 2022 6466 5f72 6177  .        "df_raw
+00004850: 223a 2230 2e32 3520 5c75 3030 6231 2030  ":"0.25 \u00b1 0
+00004860: 2e30 3222 2c0a 2020 2020 2020 2020 227a  .02",.        "z
+00004870: 223a 2230 2e32 3722 2c0a 2020 2020 2020  ":"0.27",.      
+00004880: 2020 226d 6268 223a 2238 2e39 3020 284c    "mbh":"8.90 (L
+00004890: 3139 2922 2c0a 2020 2020 2020 2020 2270  19)",.        "p
+000048a0: 6167 6e74 6465 223a 342e 3139 322c 0a20  agntde":4.192,. 
+000048b0: 2020 2020 2020 2022 636c 6173 7322 3a22         "class":"
+000048c0: 4147 4e22 2c0a 2020 2020 2020 2020 2264  AGN",.        "d
+000048d0: 6622 3a30 2e32 352c 0a20 2020 2020 2020  f":0.25,.       
+000048e0: 2022 6466 5f65 223a 302e 3032 2c0a 2020   "df_e":0.02,.  
+000048f0: 2020 2020 2020 2272 6122 3a33 3538 2e37        "ra":358.7
+00004900: 3337 3932 3237 2c0a 2020 2020 2020 2020  379227,.        
+00004910: 2264 6563 223a 302e 3730 3535 3432 352c  "dec":0.7055425,
+00004920: 0a20 2020 2020 2020 2022 416c 6c57 4953  .        "AllWIS
+00004930: 455f 6964 223a 3335 3834 3130 3030 3031  E_id":3584100001
+00004940: 3335 3130 3533 3331 392c 0a20 2020 2020  351053319,.     
+00004950: 2020 2022 7365 705f 746f 5f57 4953 455f     "sep_to_WISE_
+00004960: 736f 7572 6365 223a 302e 3135 3832 3637  source":0.158267
+00004970: 2c0a 2020 2020 2020 2020 2277 316d 7072  ,.        "w1mpr
+00004980: 6f22 3a31 322e 3633 352c 0a20 2020 2020  o":12.635,.     
+00004990: 2020 2022 7732 6d70 726f 223a 3131 2e36     "w2mpro":11.6
+000049a0: 3335 0a20 2020 207d 2c0a 2020 2020 2233  35.    },.    "3
+000049b0: 3722 3a7b 0a20 2020 2020 2020 2022 6e61  7":{.        "na
+000049c0: 6d65 223a 2241 5432 3031 396d 6568 222c  me":"AT2019meh",
+000049d0: 0a20 2020 2020 2020 2022 7470 6561 6b22  .        "tpeak"
+000049e0: 3a35 3837 3133 2e31 2c0a 2020 2020 2020  :58713.1,.      
+000049f0: 2020 2272 6973 6574 696d 6522 3a22 3233    "risetime":"23
+00004a00: 2e32 222c 0a20 2020 2020 2020 2022 6661  .2",.        "fa
+00004a10: 6465 7469 6d65 223a 2231 3237 2e39 222c  detime":"127.9",
+00004a20: 0a20 2020 2020 2020 2022 6466 5f6f 7665  .        "df_ove
+00004a30: 725f 726d 7322 3a32 392e 372c 0a20 2020  r_rms":29.7,.   
+00004a40: 2020 2020 2022 6466 5f72 6177 223a 2231       "df_raw":"1
+00004a50: 2e39 3920 5c75 3030 6231 2030 2e30 3422  .99 \u00b1 0.04"
+00004a60: 2c0a 2020 2020 2020 2020 227a 223a 2230  ,.        "z":"0
+00004a70: 2e30 3933 3522 2c0a 2020 2020 2020 2020  .0935",.        
+00004a80: 226d 6268 223a 2237 2e30 3620 2856 3231  "mbh":"7.06 (V21
+00004a90: 2922 2c0a 2020 2020 2020 2020 2270 6167  )",.        "pag
+00004aa0: 6e74 6465 223a 302e 302c 0a20 2020 2020  ntde":0.0,.     
+00004ab0: 2020 2022 636c 6173 7322 3a22 5444 453f     "class":"TDE?
+00004ac0: 222c 0a20 2020 2020 2020 2022 6466 223a  ",.        "df":
+00004ad0: 312e 3939 2c0a 2020 2020 2020 2020 2264  1.99,.        "d
+00004ae0: 665f 6522 3a30 2e30 342c 0a20 2020 2020  f_e":0.04,.     
+00004af0: 2020 2022 7261 223a 3332 312e 3832 3237     "ra":321.8227
+00004b00: 3038 2c0a 2020 2020 2020 2020 2264 6563  08,.        "dec
+00004b10: 223a 3634 2e34 3136 3433 392c 0a20 2020  ":64.416439,.   
+00004b20: 2020 2020 2022 416c 6c57 4953 455f 6964       "AllWISE_id
+00004b30: 223a 3332 3135 3136 3531 3031 3335 3130  ":32151651013510
+00004b40: 3035 3039 382c 0a20 2020 2020 2020 2022  05098,.        "
+00004b50: 7365 705f 746f 5f57 4953 455f 736f 7572  sep_to_WISE_sour
+00004b60: 6365 223a 302e 3032 3935 3533 2c0a 2020  ce":0.029553,.  
+00004b70: 2020 2020 2020 2277 316d 7072 6f22 3a31        "w1mpro":1
+00004b80: 322e 3733 322c 0a20 2020 2020 2020 2022  2.732,.        "
+00004b90: 7732 6d70 726f 223a 3132 2e30 3736 0a20  w2mpro":12.076. 
+00004ba0: 2020 207d 2c0a 2020 2020 2233 3822 3a7b     },.    "38":{
+00004bb0: 0a20 2020 2020 2020 2022 6e61 6d65 223a  .        "name":
+00004bc0: 2241 5432 3032 3061 6661 6222 2c0a 2020  "AT2020afab",.  
+00004bd0: 2020 2020 2020 2274 7065 616b 223a 3538        "tpeak":58
+00004be0: 3731 372e 322c 0a20 2020 2020 2020 2022  717.2,.        "
+00004bf0: 7269 7365 7469 6d65 223a 2234 372e 3522  risetime":"47.5"
+00004c00: 2c0a 2020 2020 2020 2020 2266 6164 6574  ,.        "fadet
+00004c10: 696d 6522 3a22 3132 372e 3222 2c0a 2020  ime":"127.2",.  
+00004c20: 2020 2020 2020 2264 665f 6f76 6572 5f72        "df_over_r
+00004c30: 6d73 223a 352e 302c 0a20 2020 2020 2020  ms":5.0,.       
+00004c40: 2022 6466 5f72 6177 223a 2230 2e32 3220   "df_raw":"0.22 
+00004c50: 5c75 3030 6231 2030 2e30 3122 2c0a 2020  \u00b1 0.01",.  
+00004c60: 2020 2020 2020 227a 223a 2230 2e32 3837        "z":"0.287
+00004c70: 3522 2c0a 2020 2020 2020 2020 226d 6268  5",.        "mbh
+00004c80: 223a 2236 2e34 3920 2856 3231 2922 2c0a  ":"6.49 (V21)",.
+00004c90: 2020 2020 2020 2020 2270 6167 6e74 6465          "pagntde
+00004ca0: 223a 352e 3738 392c 0a20 2020 2020 2020  ":5.789,.       
+00004cb0: 2022 636c 6173 7322 3a22 5444 453f 222c   "class":"TDE?",
+00004cc0: 0a20 2020 2020 2020 2022 6466 223a 302e  .        "df":0.
+00004cd0: 3232 2c0a 2020 2020 2020 2020 2264 665f  22,.        "df_
+00004ce0: 6522 3a30 2e30 312c 0a20 2020 2020 2020  e":0.01,.       
+00004cf0: 2022 7261 223a 3433 2e33 3334 3037 3832   "ra":43.3340782
+00004d00: 3830 372c 0a20 2020 2020 2020 2022 6465  807,.        "de
+00004d10: 6322 3a34 342e 3330 3135 3136 3134 3232  c":44.3015161422
+00004d20: 2c0a 2020 2020 2020 2020 2241 6c6c 5749  ,.        "AllWI
+00004d30: 5345 5f69 6422 3a22 222c 0a20 2020 2020  SE_id":"",.     
+00004d40: 2020 2022 7365 705f 746f 5f57 4953 455f     "sep_to_WISE_
+00004d50: 736f 7572 6365 223a 6e75 6c6c 2c0a 2020  source":null,.  
+00004d60: 2020 2020 2020 2277 316d 7072 6f22 3a6e        "w1mpro":n
+00004d70: 756c 6c2c 0a20 2020 2020 2020 2022 7732  ull,.        "w2
+00004d80: 6d70 726f 223a 6e75 6c6c 0a20 2020 207d  mpro":null.    }
+00004d90: 2c0a 2020 2020 2233 3922 3a7b 0a20 2020  ,.    "39":{.   
+00004da0: 2020 2020 2022 6e61 6d65 223a 2241 5432       "name":"AT2
+00004db0: 3031 3961 616d 6922 2c0a 2020 2020 2020  019aami",.      
+00004dc0: 2020 2274 7065 616b 223a 3538 3731 372e    "tpeak":58717.
+00004dd0: 342c 0a20 2020 2020 2020 2022 7269 7365  4,.        "rise
+00004de0: 7469 6d65 223a 225c 7532 3031 3322 2c0a  time":"\u2013",.
+00004df0: 2020 2020 2020 2020 2266 6164 6574 696d          "fadetim
+00004e00: 6522 3a22 3135 322e 3022 2c0a 2020 2020  e":"152.0",.    
+00004e10: 2020 2020 2264 665f 6f76 6572 5f72 6d73      "df_over_rms
+00004e20: 223a 3331 2e38 2c0a 2020 2020 2020 2020  ":31.8,.        
+00004e30: 2264 665f 7261 7722 3a22 302e 3431 205c  "df_raw":"0.41 \
+00004e40: 7530 3062 3120 302e 3031 222c 0a20 2020  u00b1 0.01",.   
+00004e50: 2020 2020 2022 7a22 3a22 5c75 3230 3133       "z":"\u2013
+00004e60: 222c 0a20 2020 2020 2020 2022 6d62 6822  ",.        "mbh"
+00004e70: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
+00004e80: 2020 2022 7061 676e 7464 6522 3a30 2e30     "pagntde":0.0
+00004e90: 2c0a 2020 2020 2020 2020 2263 6c61 7373  ,.        "class
+00004ea0: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
+00004eb0: 2020 2020 2264 6622 3a30 2e34 312c 0a20      "df":0.41,. 
+00004ec0: 2020 2020 2020 2022 6466 5f65 223a 302e         "df_e":0.
+00004ed0: 3031 2c0a 2020 2020 2020 2020 2272 6122  01,.        "ra"
+00004ee0: 3a38 2e39 3331 3130 3831 3738 382c 0a20  :8.9311081788,. 
+00004ef0: 2020 2020 2020 2022 6465 6322 3a34 372e         "dec":47.
+00004f00: 3235 3932 3534 3638 3438 2c0a 2020 2020  2592546848,.    
+00004f10: 2020 2020 2241 6c6c 5749 5345 5f69 6422      "AllWISE_id"
+00004f20: 3a38 3731 3436 3930 3133 3531 3034 3335  :871469013510435
+00004f30: 3336 2c0a 2020 2020 2020 2020 2273 6570  36,.        "sep
+00004f40: 5f74 6f5f 5749 5345 5f73 6f75 7263 6522  _to_WISE_source"
+00004f50: 3a30 2e31 3335 3135 332c 0a20 2020 2020  :0.135153,.     
+00004f60: 2020 2022 7731 6d70 726f 223a 3135 2e31     "w1mpro":15.1
+00004f70: 3532 2c0a 2020 2020 2020 2020 2277 326d  52,.        "w2m
+00004f80: 7072 6f22 3a31 342e 3830 330a 2020 2020  pro":14.803.    
+00004f90: 7d2c 0a20 2020 2022 3430 223a 7b0a 2020  },.    "40":{.  
+00004fa0: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
+00004fb0: 3230 3139 6e6e 6122 2c0a 2020 2020 2020  2019nna",.      
+00004fc0: 2020 2274 7065 616b 223a 3538 3731 372e    "tpeak":58717.
+00004fd0: 342c 0a20 2020 2020 2020 2022 7269 7365  4,.        "rise
+00004fe0: 7469 6d65 223a 2233 342e 3422 2c0a 2020  time":"34.4",.  
+00004ff0: 2020 2020 2020 2266 6164 6574 696d 6522        "fadetime"
+00005000: 3a22 3837 2e31 222c 0a20 2020 2020 2020  :"87.1",.       
+00005010: 2022 6466 5f6f 7665 725f 726d 7322 3a32   "df_over_rms":2
+00005020: 372e 302c 0a20 2020 2020 2020 2022 6466  7.0,.        "df
+00005030: 5f72 6177 223a 2230 2e33 3620 5c75 3030  _raw":"0.36 \u00
+00005040: 6231 2030 2e30 3122 2c0a 2020 2020 2020  b1 0.01",.      
+00005050: 2020 227a 223a 225c 7532 3031 3322 2c0a    "z":"\u2013",.
+00005060: 2020 2020 2020 2020 226d 6268 223a 225c          "mbh":"\
+00005070: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
+00005080: 2270 6167 6e74 6465 223a 302e 3030 312c  "pagntde":0.001,
+00005090: 0a20 2020 2020 2020 2022 636c 6173 7322  .        "class"
+000050a0: 3a22 5c75 3230 3133 222c 0a20 2020 2020  :"\u2013",.     
+000050b0: 2020 2022 6466 223a 302e 3336 2c0a 2020     "df":0.36,.  
+000050c0: 2020 2020 2020 2264 665f 6522 3a30 2e30        "df_e":0.0
+000050d0: 312c 0a20 2020 2020 2020 2022 7261 223a  1,.        "ra":
+000050e0: 3335 372e 3136 3032 3836 3836 3637 2c0a  357.1602868667,.
+000050f0: 2020 2020 2020 2020 2264 6563 223a 3139          "dec":19
+00005100: 2e32 3632 3830 3138 3833 332c 0a20 2020  .2628018833,.   
+00005110: 2020 2020 2022 416c 6c57 4953 455f 6964       "AllWISE_id
+00005120: 223a 3335 3638 3131 3936 3031 3335 3130  ":35681196013510
+00005130: 3138 3634 322c 0a20 2020 2020 2020 2022  18642,.        "
+00005140: 7365 705f 746f 5f57 4953 455f 736f 7572  sep_to_WISE_sour
+00005150: 6365 223a 302e 3239 3438 3839 2c0a 2020  ce":0.294889,.  
+00005160: 2020 2020 2020 2277 316d 7072 6f22 3a31        "w1mpro":1
+00005170: 342e 3738 322c 0a20 2020 2020 2020 2022  4.782,.        "
+00005180: 7732 6d70 726f 223a 3134 2e32 3737 0a20  w2mpro":14.277. 
+00005190: 2020 207d 2c0a 2020 2020 2234 3122 3a7b     },.    "41":{
+000051a0: 0a20 2020 2020 2020 2022 6e61 6d65 223a  .        "name":
+000051b0: 2241 5432 3031 396e 6e69 222c 0a20 2020  "AT2019nni",.   
+000051c0: 2020 2020 2022 7470 6561 6b22 3a35 3837       "tpeak":587
+000051d0: 3332 2e32 2c0a 2020 2020 2020 2020 2272  32.2,.        "r
+000051e0: 6973 6574 696d 6522 3a22 3239 2e31 222c  isetime":"29.1",
+000051f0: 0a20 2020 2020 2020 2022 6661 6465 7469  .        "fadeti
+00005200: 6d65 223a 2231 3039 2e35 222c 0a20 2020  me":"109.5",.   
+00005210: 2020 2020 2022 6466 5f6f 7665 725f 726d       "df_over_rm
+00005220: 7322 3a34 2e39 2c0a 2020 2020 2020 2020  s":4.9,.        
+00005230: 2264 665f 7261 7722 3a22 302e 3336 205c  "df_raw":"0.36 \
+00005240: 7530 3062 3120 302e 3031 222c 0a20 2020  u00b1 0.01",.   
+00005250: 2020 2020 2022 7a22 3a22 302e 3133 3722       "z":"0.137"
+00005260: 2c0a 2020 2020 2020 2020 226d 6268 223a  ,.        "mbh":
+00005270: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
+00005280: 2020 2270 6167 6e74 6465 223a 352e 3833    "pagntde":5.83
+00005290: 342c 0a20 2020 2020 2020 2022 636c 6173  4,.        "clas
+000052a0: 7322 3a22 5c75 3230 3133 222c 0a20 2020  s":"\u2013",.   
+000052b0: 2020 2020 2022 6466 223a 302e 3336 2c0a       "df":0.36,.
+000052c0: 2020 2020 2020 2020 2264 665f 6522 3a30          "df_e":0
+000052d0: 2e30 312c 0a20 2020 2020 2020 2022 7261  .01,.        "ra
+000052e0: 223a 3332 382e 3332 3731 3932 3038 3735  ":328.3271920875
+000052f0: 2c0a 2020 2020 2020 2020 2264 6563 223a  ,.        "dec":
+00005300: 2d31 392e 3232 3733 3232 3235 2c0a 2020  -19.22732225,.  
+00005310: 2020 2020 2020 2241 6c6c 5749 5345 5f69        "AllWISE_i
+00005320: 6422 3a33 3238 3030 3139 3730 3133 3531  d":3280019701351
+00005330: 3034 3635 3136 2c0a 2020 2020 2020 2020  046516,.        
+00005340: 2273 6570 5f74 6f5f 5749 5345 5f73 6f75  "sep_to_WISE_sou
+00005350: 7263 6522 3a30 2e32 3039 3332 312c 0a20  rce":0.209321,. 
+00005360: 2020 2020 2020 2022 7731 6d70 726f 223a         "w1mpro":
+00005370: 3133 2e37 3535 2c0a 2020 2020 2020 2020  13.755,.        
+00005380: 2277 326d 7072 6f22 3a31 332e 3135 360a  "w2mpro":13.156.
+00005390: 2020 2020 7d2c 0a20 2020 2022 3432 223a      },.    "42":
+000053a0: 7b0a 2020 2020 2020 2020 226e 616d 6522  {.        "name"
+000053b0: 3a22 4154 3230 3231 6165 756b 222c 0a20  :"AT2021aeuk",. 
+000053c0: 2020 2020 2020 2022 7470 6561 6b22 3a35         "tpeak":5
+000053d0: 3837 3333 2e31 2c0a 2020 2020 2020 2020  8733.1,.        
+000053e0: 2272 6973 6574 696d 6522 3a22 3433 2e34  "risetime":"43.4
+000053f0: 222c 0a20 2020 2020 2020 2022 6661 6465  ",.        "fade
+00005400: 7469 6d65 223a 2232 3338 2e31 222c 0a20  time":"238.1",. 
+00005410: 2020 2020 2020 2022 6466 5f6f 7665 725f         "df_over_
+00005420: 726d 7322 3a37 2e33 2c0a 2020 2020 2020  rms":7.3,.      
+00005430: 2020 2264 665f 7261 7722 3a22 302e 3333    "df_raw":"0.33
+00005440: 205c 7530 3062 3120 302e 3031 222c 0a20   \u00b1 0.01",. 
+00005450: 2020 2020 2020 2022 7a22 3a22 302e 3233         "z":"0.23
+00005460: 3522 2c0a 2020 2020 2020 2020 226d 6268  5",.        "mbh
+00005470: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
+00005480: 2020 2020 2270 6167 6e74 6465 223a 322e      "pagntde":2.
+00005490: 3832 372c 0a20 2020 2020 2020 2022 636c  827,.        "cl
+000054a0: 6173 7322 3a22 5c75 3230 3133 222c 0a20  ass":"\u2013",. 
+000054b0: 2020 2020 2020 2022 6466 223a 302e 3333         "df":0.33
+000054c0: 2c0a 2020 2020 2020 2020 2264 665f 6522  ,.        "df_e"
+000054d0: 3a30 2e30 312c 0a20 2020 2020 2020 2022  :0.01,.        "
+000054e0: 7261 223a 3234 332e 3234 3933 3433 3235  ra":243.24934325
+000054f0: 3637 2c0a 2020 2020 2020 2020 2264 6563  67,.        "dec
+00005500: 223a 3432 2e33 3237 3834 3636 3036 362c  ":42.3278466066,
+00005510: 0a20 2020 2020 2020 2022 416c 6c57 4953  .        "AllWIS
+00005520: 455f 6964 223a 3234 3236 3134 3234 3031  E_id":2426142401
+00005530: 3335 3130 3238 3035 322c 0a20 2020 2020  351028052,.     
+00005540: 2020 2022 7365 705f 746f 5f57 4953 455f     "sep_to_WISE_
+00005550: 736f 7572 6365 223a 302e 3138 3137 3836  source":0.181786
+00005560: 2c0a 2020 2020 2020 2020 2277 316d 7072  ,.        "w1mpr
+00005570: 6f22 3a31 332e 3330 382c 0a20 2020 2020  o":13.308,.     
+00005580: 2020 2022 7732 6d70 726f 223a 3132 2e31     "w2mpro":12.1
+00005590: 3939 0a20 2020 207d 2c0a 2020 2020 2234  99.    },.    "4
+000055a0: 3322 3a7b 0a20 2020 2020 2020 2022 6e61  3":{.        "na
+000055b0: 6d65 223a 2241 5432 3031 3968 6479 222c  me":"AT2019hdy",
+000055c0: 0a20 2020 2020 2020 2022 7470 6561 6b22  .        "tpeak"
+000055d0: 3a35 3837 3439 2e35 2c0a 2020 2020 2020  :58749.5,.      
+000055e0: 2020 2272 6973 6574 696d 6522 3a22 5c75    "risetime":"\u
+000055f0: 3230 3133 222c 0a20 2020 2020 2020 2022  2013",.        "
+00005600: 6661 6465 7469 6d65 223a 2238 372e 3922  fadetime":"87.9"
+00005610: 2c0a 2020 2020 2020 2020 2264 665f 6f76  ,.        "df_ov
+00005620: 6572 5f72 6d73 223a 342e 302c 0a20 2020  er_rms":4.0,.   
+00005630: 2020 2020 2022 6466 5f72 6177 223a 2230       "df_raw":"0
+00005640: 2e32 3020 5c75 3030 6231 2030 2e30 3122  .20 \u00b1 0.01"
+00005650: 2c0a 2020 2020 2020 2020 227a 223a 2230  ,.        "z":"0
+00005660: 2e34 3432 222c 0a20 2020 2020 2020 2022  .442",.        "
+00005670: 6d62 6822 3a22 5c75 3230 3133 222c 0a20  mbh":"\u2013",. 
+00005680: 2020 2020 2020 2022 7061 676e 7464 6522         "pagntde"
+00005690: 3a35 2e38 3633 2c0a 2020 2020 2020 2020  :5.863,.        
+000056a0: 2263 6c61 7373 223a 225c 7532 3031 3322  "class":"\u2013"
+000056b0: 2c0a 2020 2020 2020 2020 2264 6622 3a30  ,.        "df":0
+000056c0: 2e32 2c0a 2020 2020 2020 2020 2264 665f  .2,.        "df_
+000056d0: 6522 3a30 2e30 312c 0a20 2020 2020 2020  e":0.01,.       
+000056e0: 2022 7261 223a 3134 322e 3436 3137 352c   "ra":142.46175,
+000056f0: 0a20 2020 2020 2020 2022 6465 6322 3a31  .        "dec":1
+00005700: 392e 3439 3330 3131 2c0a 2020 2020 2020  9.493011,.      
+00005710: 2020 2241 6c6c 5749 5345 5f69 6422 3a31    "AllWISE_id":1
+00005720: 3432 3431 3139 3630 3133 3531 3031 3732  4241196013510172
+00005730: 3231 2c0a 2020 2020 2020 2020 2273 6570  21,.        "sep
+00005740: 5f74 6f5f 5749 5345 5f73 6f75 7263 6522  _to_WISE_source"
+00005750: 3a30 2e31 3333 3539 332c 0a20 2020 2020  :0.133593,.     
+00005760: 2020 2022 7731 6d70 726f 223a 3133 2e36     "w1mpro":13.6
+00005770: 3932 2c0a 2020 2020 2020 2020 2277 326d  92,.        "w2m
+00005780: 7072 6f22 3a31 322e 3735 0a20 2020 207d  pro":12.75.    }
+00005790: 2c0a 2020 2020 2234 3422 3a7b 0a20 2020  ,.    "44":{.   
+000057a0: 2020 2020 2022 6e61 6d65 223a 2241 5432       "name":"AT2
+000057b0: 3031 3970 6576 222c 0a20 2020 2020 2020  019pev",.       
+000057c0: 2022 7470 6561 6b22 3a35 3837 3530 2e31   "tpeak":58750.1
+000057d0: 2c0a 2020 2020 2020 2020 2272 6973 6574  ,.        "riset
+000057e0: 696d 6522 3a22 3133 2e31 222c 0a20 2020  ime":"13.1",.   
+000057f0: 2020 2020 2022 6661 6465 7469 6d65 223a       "fadetime":
+00005800: 2235 342e 3722 2c0a 2020 2020 2020 2020  "54.7",.        
+00005810: 2264 665f 6f76 6572 5f72 6d73 223a 372e  "df_over_rms":7.
+00005820: 342c 0a20 2020 2020 2020 2022 6466 5f72  4,.        "df_r
+00005830: 6177 223a 2230 2e31 3920 5c75 3030 6231  aw":"0.19 \u00b1
+00005840: 2030 2e30 3122 2c0a 2020 2020 2020 2020   0.01",.        
+00005850: 227a 223a 2230 2e30 3937 222c 0a20 2020  "z":"0.097",.   
+00005860: 2020 2020 2022 6d62 6822 3a22 362e 3430       "mbh":"6.40
+00005870: 2028 4632 3029 222c 0a20 2020 2020 2020   (F20)",.       
+00005880: 2022 7061 676e 7464 6522 3a32 2e37 3239   "pagntde":2.729
+00005890: 2c0a 2020 2020 2020 2020 2263 6c61 7373  ,.        "class
+000058a0: 223a 2254 4445 3f22 2c0a 2020 2020 2020  ":"TDE?",.      
+000058b0: 2020 2264 6622 3a30 2e31 392c 0a20 2020    "df":0.19,.   
+000058c0: 2020 2020 2022 6466 5f65 223a 302e 3031       "df_e":0.01
+000058d0: 2c0a 2020 2020 2020 2020 2272 6122 3a36  ,.        "ra":6
+000058e0: 372e 3334 3436 3637 2c0a 2020 2020 2020  7.344667,.      
+000058f0: 2020 2264 6563 223a 302e 3631 3837 352c    "dec":0.61875,
+00005900: 0a20 2020 2020 2020 2022 416c 6c57 4953  .        "AllWIS
+00005910: 455f 6964 223a 3638 3031 3030 3030 3133  E_id":6801000013
+00005920: 3531 3035 3936 3436 2c0a 2020 2020 2020  51059646,.      
+00005930: 2020 2273 6570 5f74 6f5f 5749 5345 5f73    "sep_to_WISE_s
+00005940: 6f75 7263 6522 3a30 2e36 3539 3135 352c  ource":0.659155,
+00005950: 0a20 2020 2020 2020 2022 7731 6d70 726f  .        "w1mpro
+00005960: 223a 3133 2e37 3035 2c0a 2020 2020 2020  ":13.705,.      
+00005970: 2020 2277 326d 7072 6f22 3a31 332e 3234    "w2mpro":13.24
+00005980: 320a 2020 2020 7d2c 0a20 2020 2022 3435  2.    },.    "45
+00005990: 223a 7b0a 2020 2020 2020 2020 226e 616d  ":{.        "nam
+000059a0: 6522 3a22 4154 3230 3133 6b70 222c 0a20  e":"AT2013kp",. 
+000059b0: 2020 2020 2020 2022 7470 6561 6b22 3a35         "tpeak":5
+000059c0: 3837 3533 2e31 2c0a 2020 2020 2020 2020  8753.1,.        
+000059d0: 2272 6973 6574 696d 6522 3a22 3131 2e39  "risetime":"11.9
+000059e0: 222c 0a20 2020 2020 2020 2022 6661 6465  ",.        "fade
+000059f0: 7469 6d65 223a 2233 342e 3722 2c0a 2020  time":"34.7",.  
+00005a00: 2020 2020 2020 2264 665f 6f76 6572 5f72        "df_over_r
+00005a10: 6d73 223a 3434 2e34 2c0a 2020 2020 2020  ms":44.4,.      
+00005a20: 2020 2264 665f 7261 7722 3a22 322e 3134    "df_raw":"2.14
+00005a30: 205c 7530 3062 3120 302e 3034 222c 0a20   \u00b1 0.04",. 
+00005a40: 2020 2020 2020 2022 7a22 3a22 302e 3031         "z":"0.01
+00005a50: 3439 3922 2c0a 2020 2020 2020 2020 226d  499",.        "m
+00005a60: 6268 223a 2236 2e31 3920 284e 3230 2922  bh":"6.19 (N20)"
+00005a70: 2c0a 2020 2020 2020 2020 2270 6167 6e74  ,.        "pagnt
+00005a80: 6465 223a 302e 302c 0a20 2020 2020 2020  de":0.0,.       
+00005a90: 2022 636c 6173 7322 3a22 5444 4522 2c0a   "class":"TDE",.
+00005aa0: 2020 2020 2020 2020 2264 6622 3a32 2e31          "df":2.1
+00005ab0: 342c 0a20 2020 2020 2020 2022 6466 5f65  4,.        "df_e
+00005ac0: 223a 302e 3034 2c0a 2020 2020 2020 2020  ":0.04,.        
+00005ad0: 2272 6122 3a37 312e 3635 3738 3136 3630  "ra":71.65781660
+00005ae0: 342c 0a20 2020 2020 2020 2022 6465 6322  4,.        "dec"
+00005af0: 3a2d 3130 2e32 3236 3331 3936 3238 322c  :-10.2263196282,
+00005b00: 0a20 2020 2020 2020 2022 416c 6c57 4953  .        "AllWIS
+00005b10: 455f 6964 223a 3732 3330 3130 3730 3133  E_id":7230107013
+00005b20: 3531 3033 3632 3932 2c0a 2020 2020 2020  51036292,.      
+00005b30: 2020 2273 6570 5f74 6f5f 5749 5345 5f73    "sep_to_WISE_s
+00005b40: 6f75 7263 6522 3a30 2e32 3835 3832 322c  ource":0.285822,
+00005b50: 0a20 2020 2020 2020 2022 7731 6d70 726f  .        "w1mpro
+00005b60: 223a 3132 2e34 3831 2c0a 2020 2020 2020  ":12.481,.      
+00005b70: 2020 2277 326d 7072 6f22 3a31 322e 3532    "w2mpro":12.52
+00005b80: 310a 2020 2020 7d2c 0a20 2020 2022 3436  1.    },.    "46
+00005b90: 223a 7b0a 2020 2020 2020 2020 226e 616d  ":{.        "nam
+00005ba0: 6522 3a22 4154 3230 3139 6272 7322 2c0a  e":"AT2019brs",.
+00005bb0: 2020 2020 2020 2020 2274 7065 616b 223a          "tpeak":
+00005bc0: 3538 3735 382e 312c 0a20 2020 2020 2020  58758.1,.       
+00005bd0: 2022 7269 7365 7469 6d65 223a 2231 3130   "risetime":"110
+00005be0: 2e39 222c 0a20 2020 2020 2020 2022 6661  .9",.        "fa
+00005bf0: 6465 7469 6d65 223a 2234 3833 2e32 222c  detime":"483.2",
+00005c00: 0a20 2020 2020 2020 2022 6466 5f6f 7665  .        "df_ove
+00005c10: 725f 726d 7322 3a39 2e36 2c0a 2020 2020  r_rms":9.6,.    
+00005c20: 2020 2020 2264 665f 7261 7722 3a22 302e      "df_raw":"0.
+00005c30: 3738 205c 7530 3062 3120 302e 3031 222c  78 \u00b1 0.01",
+00005c40: 0a20 2020 2020 2020 2022 7a22 3a22 302e  .        "z":"0.
+00005c50: 3337 3336 222c 0a20 2020 2020 2020 2022  3736",.        "
+00005c60: 6d62 6822 3a22 372e 3230 2028 4632 3029  mbh":"7.20 (F20)
+00005c70: 222c 0a20 2020 2020 2020 2022 7061 676e  ",.        "pagn
+00005c80: 7464 6522 3a31 2e32 3237 2c0a 2020 2020  tde":1.227,.    
+00005c90: 2020 2020 2263 6c61 7373 223a 2254 4445      "class":"TDE
+00005ca0: 3f22 2c0a 2020 2020 2020 2020 2264 6622  ?",.        "df"
+00005cb0: 3a30 2e37 382c 0a20 2020 2020 2020 2022  :0.78,.        "
+00005cc0: 6466 5f65 223a 302e 3031 2c0a 2020 2020  df_e":0.01,.    
+00005cd0: 2020 2020 2272 6122 3a32 3136 2e39 3433      "ra":216.943
+00005ce0: 3333 332c 0a20 2020 2020 2020 2022 6465  333,.        "de
+00005cf0: 6322 3a32 392e 3531 3036 3331 2c0a 2020  c":29.510631,.  
+00005d00: 2020 2020 2020 2241 6c6c 5749 5345 5f69        "AllWISE_i
+00005d10: 6422 3a32 3137 3731 3238 3730 3133 3531  d":2177128701351
+00005d20: 3036 3431 3435 2c0a 2020 2020 2020 2020  064145,.        
+00005d30: 2273 6570 5f74 6f5f 5749 5345 5f73 6f75  "sep_to_WISE_sou
+00005d40: 7263 6522 3a30 2e31 3138 3437 322c 0a20  rce":0.118472,. 
+00005d50: 2020 2020 2020 2022 7731 6d70 726f 223a         "w1mpro":
+00005d60: 3134 2e33 3631 2c0a 2020 2020 2020 2020  14.361,.        
+00005d70: 2277 326d 7072 6f22 3a31 332e 3338 330a  "w2mpro":13.383.
+00005d80: 2020 2020 7d2c 0a20 2020 2022 3437 223a      },.    "47":
+00005d90: 7b0a 2020 2020 2020 2020 226e 616d 6522  {.        "name"
+00005da0: 3a22 4154 3230 3230 6166 6163 222c 0a20  :"AT2020afac",. 
+00005db0: 2020 2020 2020 2022 7470 6561 6b22 3a35         "tpeak":5
+00005dc0: 3837 3538 2e33 2c0a 2020 2020 2020 2020  8758.3,.        
+00005dd0: 2272 6973 6574 696d 6522 3a22 3638 2e30  "risetime":"68.0
+00005de0: 222c 0a20 2020 2020 2020 2022 6661 6465  ",.        "fade
+00005df0: 7469 6d65 223a 2239 352e 3022 2c0a 2020  time":"95.0",.  
+00005e00: 2020 2020 2020 2264 665f 6f76 6572 5f72        "df_over_r
+00005e10: 6d73 223a 3130 2e38 2c0a 2020 2020 2020  ms":10.8,.      
+00005e20: 2020 2264 665f 7261 7722 3a22 302e 3136    "df_raw":"0.16
+00005e30: 205c 7530 3062 3120 302e 3031 222c 0a20   \u00b1 0.01",. 
+00005e40: 2020 2020 2020 2022 7a22 3a22 5c75 3230         "z":"\u20
+00005e50: 3133 222c 0a20 2020 2020 2020 2022 6d62  13",.        "mb
+00005e60: 6822 3a22 5c75 3230 3133 222c 0a20 2020  h":"\u2013",.   
+00005e70: 2020 2020 2022 7061 676e 7464 6522 3a30       "pagntde":0
+00005e80: 2e38 3635 2c0a 2020 2020 2020 2020 2263  .865,.        "c
+00005e90: 6c61 7373 223a 225c 7532 3031 3322 2c0a  lass":"\u2013",.
+00005ea0: 2020 2020 2020 2020 2264 6622 3a30 2e31          "df":0.1
+00005eb0: 362c 0a20 2020 2020 2020 2022 6466 5f65  6,.        "df_e
+00005ec0: 223a 302e 3031 2c0a 2020 2020 2020 2020  ":0.01,.        
+00005ed0: 2272 6122 3a32 3638 2e34 3137 3339 3431  "ra":268.4173941
+00005ee0: 3431 312c 0a20 2020 2020 2020 2022 6465  411,.        "de
+00005ef0: 6322 3a35 352e 3835 3735 3335 3530 3839  c":55.8575355089
+00005f00: 2c0a 2020 2020 2020 2020 2241 6c6c 5749  ,.        "AllWI
+00005f10: 5345 5f69 6422 3a32 3639 3331 3536 3030  SE_id":269315600
+00005f20: 3133 3531 3031 3238 3338 2c0a 2020 2020  1351012838,.    
+00005f30: 2020 2020 2273 6570 5f74 6f5f 5749 5345      "sep_to_WISE
+00005f40: 5f73 6f75 7263 6522 3a30 2e32 3130 3836  _source":0.21086
+00005f50: 312c 0a20 2020 2020 2020 2022 7731 6d70  1,.        "w1mp
+00005f60: 726f 223a 3133 2e38 372c 0a20 2020 2020  ro":13.87,.     
+00005f70: 2020 2022 7732 6d70 726f 223a 3133 2e35     "w2mpro":13.5
+00005f80: 3635 0a20 2020 207d 2c0a 2020 2020 2234  65.    },.    "4
+00005f90: 3822 3a7b 0a20 2020 2020 2020 2022 6e61  8":{.        "na
+00005fa0: 6d65 223a 2241 5432 3031 3977 7264 222c  me":"AT2019wrd",
+00005fb0: 0a20 2020 2020 2020 2022 7470 6561 6b22  .        "tpeak"
+00005fc0: 3a35 3837 3634 2e33 2c0a 2020 2020 2020  :58764.3,.      
+00005fd0: 2020 2272 6973 6574 696d 6522 3a22 3832    "risetime":"82
+00005fe0: 2e36 222c 0a20 2020 2020 2020 2022 6661  .6",.        "fa
+00005ff0: 6465 7469 6d65 223a 225c 7532 3031 3322  detime":"\u2013"
+00006000: 2c0a 2020 2020 2020 2020 2264 665f 6f76  ,.        "df_ov
+00006010: 6572 5f72 6d73 223a 372e 362c 0a20 2020  er_rms":7.6,.   
+00006020: 2020 2020 2022 6466 5f72 6177 223a 2230       "df_raw":"0
+00006030: 2e31 3520 5c75 3030 6231 2030 2e30 3122  .15 \u00b1 0.01"
+00006040: 2c0a 2020 2020 2020 2020 227a 223a 225c  ,.        "z":"\
+00006050: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
+00006060: 226d 6268 223a 225c 7532 3031 3322 2c0a  "mbh":"\u2013",.
+00006070: 2020 2020 2020 2020 2270 6167 6e74 6465          "pagntde
+00006080: 223a 322e 3536 322c 0a20 2020 2020 2020  ":2.562,.       
+00006090: 2022 636c 6173 7322 3a22 5c75 3230 3133   "class":"\u2013
+000060a0: 222c 0a20 2020 2020 2020 2022 6466 223a  ",.        "df":
+000060b0: 302e 3135 2c0a 2020 2020 2020 2020 2264  0.15,.        "d
+000060c0: 665f 6522 3a30 2e30 312c 0a20 2020 2020  f_e":0.01,.     
+000060d0: 2020 2022 7261 223a 3335 352e 3938 3134     "ra":355.9814
+000060e0: 3538 2c0a 2020 2020 2020 2020 2264 6563  58,.        "dec
+000060f0: 223a 3331 2e33 3737 3135 2c0a 2020 2020  ":31.37715,.    
+00006100: 2020 2020 2241 6c6c 5749 5345 5f69 6422      "AllWISE_id"
+00006110: 3a33 3536 3431 3331 3830 3133 3531 3031  :356413180135101
+00006120: 3436 3537 2c0a 2020 2020 2020 2020 2273  4657,.        "s
+00006130: 6570 5f74 6f5f 5749 5345 5f73 6f75 7263  ep_to_WISE_sourc
+00006140: 6522 3a30 2e30 3937 3536 392c 0a20 2020  e":0.097569,.   
+00006150: 2020 2020 2022 7731 6d70 726f 223a 3135       "w1mpro":15
+00006160: 2e31 3539 2c0a 2020 2020 2020 2020 2277  .159,.        "w
+00006170: 326d 7072 6f22 3a31 342e 3637 370a 2020  2mpro":14.677.  
+00006180: 2020 7d2c 0a20 2020 2022 3439 223a 7b0a    },.    "49":{.
+00006190: 2020 2020 2020 2020 226e 616d 6522 3a22          "name":"
+000061a0: 4154 3230 3231 6165 7568 222c 0a20 2020  AT2021aeuh",.   
+000061b0: 2020 2020 2022 7470 6561 6b22 3a35 3837       "tpeak":587
+000061c0: 3839 2e35 2c0a 2020 2020 2020 2020 2272  89.5,.        "r
+000061d0: 6973 6574 696d 6522 3a22 5c75 3230 3133  isetime":"\u2013
+000061e0: 222c 0a20 2020 2020 2020 2022 6661 6465  ",.        "fade
+000061f0: 7469 6d65 223a 225c 7532 3031 3322 2c0a  time":"\u2013",.
+00006200: 2020 2020 2020 2020 2264 665f 6f76 6572          "df_over
+00006210: 5f72 6d73 223a 332e 392c 0a20 2020 2020  _rms":3.9,.     
+00006220: 2020 2022 6466 5f72 6177 223a 2230 2e32     "df_raw":"0.2
+00006230: 3820 5c75 3030 6231 2030 2e30 3122 2c0a  8 \u00b1 0.01",.
+00006240: 2020 2020 2020 2020 227a 223a 2230 2e30          "z":"0.0
+00006250: 3833 3422 2c0a 2020 2020 2020 2020 226d  834",.        "m
+00006260: 6268 223a 2237 2e33 3920 284c 3139 2922  bh":"7.39 (L19)"
+00006270: 2c0a 2020 2020 2020 2020 2270 6167 6e74  ,.        "pagnt
+00006280: 6465 223a 352e 3732 362c 0a20 2020 2020  de":5.726,.     
+00006290: 2020 2022 636c 6173 7322 3a22 5444 453f     "class":"TDE?
+000062a0: 222c 0a20 2020 2020 2020 2022 6466 223a  ",.        "df":
+000062b0: 302e 3238 2c0a 2020 2020 2020 2020 2264  0.28,.        "d
+000062c0: 665f 6522 3a30 2e30 312c 0a20 2020 2020  f_e":0.01,.     
+000062d0: 2020 2022 7261 223a 3138 312e 3039 3232     "ra":181.0922
+000062e0: 3335 3033 3634 2c0a 2020 2020 2020 2020  350364,.        
+000062f0: 2264 6563 223a 2d31 2e33 3637 3538 3038  "dec":-1.3675808
+00006300: 3831 382c 0a20 2020 2020 2020 2022 416c  818,.        "Al
+00006310: 6c57 4953 455f 6964 223a 3138 3135 3030  lWISE_id":181500
+00006320: 3136 3031 3335 3130 3333 3035 392c 0a20  1601351033059,. 
+00006330: 2020 2020 2020 2022 7365 705f 746f 5f57         "sep_to_W
+00006340: 4953 455f 736f 7572 6365 223a 302e 3038  ISE_source":0.08
+00006350: 3939 3137 2c0a 2020 2020 2020 2020 2277  9917,.        "w
+00006360: 316d 7072 6f22 3a31 332e 3434 382c 0a20  1mpro":13.448,. 
+00006370: 2020 2020 2020 2022 7732 6d70 726f 223a         "w2mpro":
+00006380: 3132 2e37 3136 0a20 2020 207d 2c0a 2020  12.716.    },.  
+00006390: 2020 2235 3022 3a7b 0a20 2020 2020 2020    "50":{.       
+000063a0: 2022 6e61 6d65 223a 2241 5432 3031 396d   "name":"AT2019m
+000063b0: 7371 222c 0a20 2020 2020 2020 2022 7470  sq",.        "tp
+000063c0: 6561 6b22 3a35 3837 3931 2e32 2c0a 2020  eak":58791.2,.  
+000063d0: 2020 2020 2020 2272 6973 6574 696d 6522        "risetime"
+000063e0: 3a22 3133 372e 3922 2c0a 2020 2020 2020  :"137.9",.      
+000063f0: 2020 2266 6164 6574 696d 6522 3a22 5c75    "fadetime":"\u
+00006400: 3230 3133 222c 0a20 2020 2020 2020 2022  2013",.        "
+00006410: 6466 5f6f 7665 725f 726d 7322 3a36 2e34  df_over_rms":6.4
+00006420: 2c0a 2020 2020 2020 2020 2264 665f 7261  ,.        "df_ra
+00006430: 7722 3a22 302e 3136 205c 7530 3062 3120  w":"0.16 \u00b1 
+00006440: 302e 3031 222c 0a20 2020 2020 2020 2022  0.01",.        "
+00006450: 7a22 3a22 5c75 3230 3133 222c 0a20 2020  z":"\u2013",.   
+00006460: 2020 2020 2022 6d62 6822 3a22 5c75 3230       "mbh":"\u20
+00006470: 3133 222c 0a20 2020 2020 2020 2022 7061  13",.        "pa
+00006480: 676e 7464 6522 3a33 2e39 3333 2c0a 2020  gntde":3.933,.  
+00006490: 2020 2020 2020 2263 6c61 7373 223a 225c        "class":"\
+000064a0: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
+000064b0: 2264 6622 3a30 2e31 362c 0a20 2020 2020  "df":0.16,.     
+000064c0: 2020 2022 6466 5f65 223a 302e 3031 2c0a     "df_e":0.01,.
+000064d0: 2020 2020 2020 2020 2272 6122 3a34 2e31          "ra":4.1
+000064e0: 3834 2c0a 2020 2020 2020 2020 2264 6563  84,.        "dec
+000064f0: 223a 362e 3338 3030 3839 2c0a 2020 2020  ":6.380089,.    
+00006500: 2020 2020 2241 6c6c 5749 5345 5f69 6422      "AllWISE_id"
+00006510: 3a34 3531 3036 3030 3133 3531 3034 3231  :451060013510421
+00006520: 3833 2c0a 2020 2020 2020 2020 2273 6570  83,.        "sep
+00006530: 5f74 6f5f 5749 5345 5f73 6f75 7263 6522  _to_WISE_source"
+00006540: 3a30 2e31 3039 3636 312c 0a20 2020 2020  :0.109661,.     
+00006550: 2020 2022 7731 6d70 726f 223a 3135 2e39     "w1mpro":15.9
+00006560: 3737 2c0a 2020 2020 2020 2020 2277 326d  77,.        "w2m
+00006570: 7072 6f22 3a31 352e 3339 310a 2020 2020  pro":15.391.    
+00006580: 7d2c 0a20 2020 2022 3531 223a 7b0a 2020  },.    "51":{.  
+00006590: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
+000065a0: 3230 3139 7170 7422 2c0a 2020 2020 2020  2019qpt",.      
+000065b0: 2020 2274 7065 616b 223a 3538 3739 382e    "tpeak":58798.
+000065c0: 332c 0a20 2020 2020 2020 2022 7269 7365  3,.        "rise
+000065d0: 7469 6d65 223a 2234 342e 3522 2c0a 2020  time":"44.5",.  
+000065e0: 2020 2020 2020 2266 6164 6574 696d 6522        "fadetime"
+000065f0: 3a22 3133 352e 3122 2c0a 2020 2020 2020  :"135.1",.      
+00006600: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
+00006610: 3133 2e38 2c0a 2020 2020 2020 2020 2264  13.8,.        "d
+00006620: 665f 7261 7722 3a22 302e 3234 205c 7530  f_raw":"0.24 \u0
+00006630: 3062 3120 302e 3031 222c 0a20 2020 2020  0b1 0.01",.     
+00006640: 2020 2022 7a22 3a22 302e 3234 3222 2c0a     "z":"0.242",.
+00006650: 2020 2020 2020 2020 226d 6268 223a 2236          "mbh":"6
+00006660: 2e39 3720 284c 3139 2922 2c0a 2020 2020  .97 (L19)",.    
+00006670: 2020 2020 2270 6167 6e74 6465 223a 302e      "pagntde":0.
+00006680: 3335 352c 0a20 2020 2020 2020 2022 636c  355,.        "cl
+00006690: 6173 7322 3a22 5444 453f 222c 0a20 2020  ass":"TDE?",.   
+000066a0: 2020 2020 2022 6466 223a 302e 3234 2c0a       "df":0.24,.
+000066b0: 2020 2020 2020 2020 2264 665f 6522 3a30          "df_e":0
+000066c0: 2e30 312c 0a20 2020 2020 2020 2022 7261  .01,.        "ra
+000066d0: 223a 3132 302e 3335 3733 3735 2c0a 2020  ":120.357375,.  
+000066e0: 2020 2020 2020 2264 6563 223a 3234 2e39        "dec":24.9
+000066f0: 3239 3433 392c 0a20 2020 2020 2020 2022  29439,.        "
+00006700: 416c 6c57 4953 455f 6964 223a 3132 3035  AllWISE_id":1205
+00006710: 3132 3432 3031 3335 3130 3536 3632 392c  124201351056629,
+00006720: 0a20 2020 2020 2020 2022 7365 705f 746f  .        "sep_to
+00006730: 5f57 4953 455f 736f 7572 6365 223a 302e  _WISE_source":0.
+00006740: 3038 3030 3933 2c0a 2020 2020 2020 2020  080093,.        
+00006750: 2277 316d 7072 6f22 3a31 342e 3637 342c  "w1mpro":14.674,
+00006760: 0a20 2020 2020 2020 2022 7732 6d70 726f  .        "w2mpro
+00006770: 223a 3133 2e38 3939 0a20 2020 207d 2c0a  ":13.899.    },.
+00006780: 2020 2020 2235 3222 3a7b 0a20 2020 2020      "52":{.     
+00006790: 2020 2022 6e61 6d65 223a 2241 5432 3032     "name":"AT202
+000067a0: 3061 6661 6422 2c0a 2020 2020 2020 2020  0afad",.        
+000067b0: 2274 7065 616b 223a 3538 3830 322e 322c  "tpeak":58802.2,
+000067c0: 0a20 2020 2020 2020 2022 7269 7365 7469  .        "riseti
+000067d0: 6d65 223a 2237 372e 3122 2c0a 2020 2020  me":"77.1",.    
+000067e0: 2020 2020 2266 6164 6574 696d 6522 3a22      "fadetime":"
+000067f0: 3132 352e 3522 2c0a 2020 2020 2020 2020  125.5",.        
+00006800: 2264 665f 6f76 6572 5f72 6d73 223a 332e  "df_over_rms":3.
+00006810: 372c 0a20 2020 2020 2020 2022 6466 5f72  7,.        "df_r
+00006820: 6177 223a 2230 2e30 3820 5c75 3030 6231  aw":"0.08 \u00b1
+00006830: 2030 2e30 3122 2c0a 2020 2020 2020 2020   0.01",.        
+00006840: 227a 223a 225c 7532 3031 3322 2c0a 2020  "z":"\u2013",.  
+00006850: 2020 2020 2020 226d 6268 223a 225c 7532        "mbh":"\u2
+00006860: 3031 3322 2c0a 2020 2020 2020 2020 2270  013",.        "p
+00006870: 6167 6e74 6465 223a 352e 3231 372c 0a20  agntde":5.217,. 
+00006880: 2020 2020 2020 2022 636c 6173 7322 3a22         "class":"
+00006890: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
+000068a0: 2022 6466 223a 302e 3038 2c0a 2020 2020   "df":0.08,.    
+000068b0: 2020 2020 2264 665f 6522 3a30 2e30 312c      "df_e":0.01,
+000068c0: 0a20 2020 2020 2020 2022 7261 223a 3130  .        "ra":10
+000068d0: 332e 3832 3533 3037 3038 3137 2c0a 2020  3.8253070817,.  
+000068e0: 2020 2020 2020 2264 6563 223a 3538 2e39        "dec":58.9
+000068f0: 3834 3639 3334 3831 372c 0a20 2020 2020  846934817,.     
+00006900: 2020 2022 416c 6c57 4953 455f 6964 223a     "AllWISE_id":
+00006910: 3130 3336 3135 3930 3031 3335 3130 3330  1036159001351030
+00006920: 3637 332c 0a20 2020 2020 2020 2022 7365  673,.        "se
+00006930: 705f 746f 5f57 4953 455f 736f 7572 6365  p_to_WISE_source
+00006940: 223a 302e 3138 3432 392c 0a20 2020 2020  ":0.18429,.     
+00006950: 2020 2022 7731 6d70 726f 223a 3134 2e38     "w1mpro":14.8
+00006960: 3236 2c0a 2020 2020 2020 2020 2277 326d  26,.        "w2m
+00006970: 7072 6f22 3a31 332e 3738 320a 2020 2020  pro":13.782.    
+00006980: 7d2c 0a20 2020 2022 3533 223a 7b0a 2020  },.    "53":{.  
+00006990: 2020 2020 2020 226e 616d 6522 3a22 4154        "name":"AT
+000069a0: 3230 3139 6d73 7322 2c0a 2020 2020 2020  2019mss",.      
+000069b0: 2020 2274 7065 616b 223a 3538 3831 312e    "tpeak":58811.
+000069c0: 362c 0a20 2020 2020 2020 2022 7269 7365  6,.        "rise
+000069d0: 7469 6d65 223a 2233 352e 3222 2c0a 2020  time":"35.2",.  
+000069e0: 2020 2020 2020 2266 6164 6574 696d 6522        "fadetime"
+000069f0: 3a22 3230 392e 3722 2c0a 2020 2020 2020  :"209.7",.      
+00006a00: 2020 2264 665f 6f76 6572 5f72 6d73 223a    "df_over_rms":
+00006a10: 3230 2e38 2c0a 2020 2020 2020 2020 2264  20.8,.        "d
+00006a20: 665f 7261 7722 3a22 302e 3338 205c 7530  f_raw":"0.38 \u0
+00006a30: 3062 3120 302e 3031 222c 0a20 2020 2020  0b1 0.01",.     
+00006a40: 2020 2022 7a22 3a22 5c75 3230 3133 222c     "z":"\u2013",
+00006a50: 0a20 2020 2020 2020 2022 6d62 6822 3a22  .        "mbh":"
+00006a60: 5c75 3230 3133 222c 0a20 2020 2020 2020  \u2013",.       
+00006a70: 2022 7061 676e 7464 6522 3a30 2e30 3231   "pagntde":0.021
+00006a80: 2c0a 2020 2020 2020 2020 2263 6c61 7373  ,.        "class
+00006a90: 223a 225c 7532 3031 3322 2c0a 2020 2020  ":"\u2013",.    
+00006aa0: 2020 2020 2264 6622 3a30 2e33 382c 0a20      "df":0.38,. 
+00006ab0: 2020 2020 2020 2022 6466 5f65 223a 302e         "df_e":0.
+00006ac0: 3031 2c0a 2020 2020 2020 2020 2272 6122  01,.        "ra"
+00006ad0: 3a32 3037 2e31 3032 3431 372c 0a20 2020  :207.102417,.   
+00006ae0: 2020 2020 2022 6465 6322 3a38 2e35 3238       "dec":8.528
+00006af0: 372c 0a20 2020 2020 2020 2022 416c 6c57  7,.        "AllW
+00006b00: 4953 455f 6964 223a 3230 3638 3130 3930  ISE_id":20681090
+00006b10: 3031 3335 3130 3032 3638 312c 0a20 2020  01351002681,.   
+00006b20: 2020 2020 2022 7365 705f 746f 5f57 4953       "sep_to_WIS
+00006b30: 455f 736f 7572 6365 223a 302e 3035 3038  E_source":0.0508
+00006b40: 3332 2c0a 2020 2020 2020 2020 2277 316d  32,.        "w1m
+00006b50: 7072 6f22 3a31 342e 3737 372c 0a20 2020  pro":14.777,.   
+00006b60: 2020 2020 2022 7732 6d70 726f 223a 3134       "w2mpro":14
+00006b70: 2e30 3436 0a20 2020 207d 2c0a 2020 2020  .046.    },.    
+00006b80: 2235 3422 3a7b 0a20 2020 2020 2020 2022  "54":{.        "
+00006b90: 6e61 6d65 223a 2241 5432 3031 3974 6868  name":"AT2019thh
+00006ba0: 222c 0a20 2020 2020 2020 2022 7470 6561  ",.        "tpea
+00006bb0: 6b22 3a35 3838 3531 2e31 2c0a 2020 2020  k":58851.1,.    
+00006bc0: 2020 2020 2272 6973 6574 696d 6522 3a22      "risetime":"
+00006bd0: 3130 342e 3722 2c0a 2020 2020 2020 2020  104.7",.        
+00006be0: 2266 6164 6574 696d 6522 3a22 3433 332e  "fadetime":"433.
+00006bf0: 3822 2c0a 2020 2020 2020 2020 2264 665f  8",.        "df_
+00006c00: 6f76 6572 5f72 6d73 223a 3732 2e32 2c0a  over_rms":72.2,.
+00006c10: 2020 2020 2020 2020 2264 665f 7261 7722          "df_raw"
+00006c20: 3a22 312e 3735 205c 7530 3062 3120 302e  :"1.75 \u00b1 0.
+00006c30: 3032 222c 0a20 2020 2020 2020 2022 7a22  02",.        "z"
+00006c40: 3a22 302e 3035 3036 222c 0a20 2020 2020  :"0.0506",.     
+00006c50: 2020 2022 6d62 6822 3a22 5c75 3230 3133     "mbh":"\u2013
+00006c60: 222c 0a20 2020 2020 2020 2022 7061 676e  ",.        "pagn
+00006c70: 7464 6522 3a30 2e30 2c0a 2020 2020 2020  tde":0.0,.      
+00006c80: 2020 2263 6c61 7373 223a 225c 7532 3031    "class":"\u201
+00006c90: 3322 2c0a 2020 2020 2020 2020 2264 6622  3",.        "df"
+00006ca0: 3a31 2e37 352c 0a20 2020 2020 2020 2022  :1.75,.        "
+00006cb0: 6466 5f65 223a 302e 3032 2c0a 2020 2020  df_e":0.02,.    
+00006cc0: 2020 2020 2272 6122 3a33 3336 2e39 3933      "ra":336.993
+00006cd0: 3534 322c 0a20 2020 2020 2020 2022 6465  542,.        "de
+00006ce0: 6322 3a31 382e 3332 3230 3639 2c0a 2020  c":18.322069,.  
+00006cf0: 2020 2020 2020 2241 6c6c 5749 5345 5f69        "AllWISE_i
+00006d00: 6422 3a33 3336 3231 3138 3130 3133 3531  d":3362118101351
+00006d10: 3032 3433 3536 2c0a 2020 2020 2020 2020  024356,.        
+00006d20: 2273 6570 5f74 6f5f 5749 5345 5f73 6f75  "sep_to_WISE_sou
+00006d30: 7263 6522 3a30 2e39 3031 3935 332c 0a20  rce":0.901953,. 
+00006d40: 2020 2020 2020 2022 7731 6d70 726f 223a         "w1mpro":
+00006d50: 3133 2e36 3133 2c0a 2020 2020 2020 2020  13.613,.        
+00006d60: 2277 326d 7072 6f22 3a31 332e 3436 390a  "w2mpro":13.469.
+00006d70: 2020 2020 7d2c 0a20 2020 2022 3535 223a      },.    "55":
+00006d80: 7b0a 2020 2020 2020 2020 226e 616d 6522  {.        "name"
+00006d90: 3a22 4154 3230 3231 6165 7569 222c 0a20  :"AT2021aeui",. 
+00006da0: 2020 2020 2020 2022 7470 6561 6b22 3a35         "tpeak":5
+00006db0: 3838 3630 2e33 2c0a 2020 2020 2020 2020  8860.3,.        
+00006dc0: 2272 6973 6574 696d 6522 3a22 5c75 3230  "risetime":"\u20
+00006dd0: 3133 222c 0a20 2020 2020 2020 2022 6661  13",.        "fa
+00006de0: 6465 7469 6d65 223a 2236 302e 3022 2c0a  detime":"60.0",.
+00006df0: 2020 2020 2020 2020 2264 665f 6f76 6572          "df_over
+00006e00: 5f72 6d73 223a 362e 322c 0a20 2020 2020  _rms":6.2,.     
+00006e10: 2020 2022 6466 5f72 6177 223a 2230 2e34     "df_raw":"0.4
+00006e20: 3920 5c75 3030 6231 2030 2e30 3222 2c0a  9 \u00b1 0.02",.
+00006e30: 2020 2020 2020 2020 227a 223a 225c 7532          "z":"\u2
+00006e40: 3031 3322 2c0a 2020 2020 2020 2020 226d  013",.        "m
+00006e50: 6268 223a 225c 7532 3031 3322 2c0a 2020  bh":"\u2013",.  
+00006e60: 2020 2020 2020 2270 6167 6e74 6465 223a        "pagntde":
+00006e70: 342e 3235 2c0a 2020 2020 2020 2020 2263  4.25,.        "c
+00006e80: 6c61 7373 223a 225c 7532 3031 3322 2c0a  lass":"\u2013",.
+00006e90: 2020 2020 2020 2020 2264 6622 3a30 2e34          "df":0.4
+00006ea0: 392c 0a20 2020 2020 2020 2022 6466 5f65  9,.        "df_e
+00006eb0: 223a 302e 3032 2c0a 2020 2020 2020 2020  ":0.02,.        
+00006ec0: 2272 6122 3a31 3230 2e30 3833 3231 3035  "ra":120.0832105
+00006ed0: 3736 352c 0a20 2020 2020 2020 2022 6465  765,.        "de
+00006ee0: 6322 3a37 352e 3832 3330 3831 3433 3533  c":75.8230814353
+00006ef0: 2c0a 2020 2020 2020 2020 2241 6c6c 5749  ,.        "AllWI
+00006f00: 5345 5f69 6422 3a31 3231 3931 3735 3730  SE_id":121917570
+00006f10: 3133 3531 3033 3433 3631 2c0a 2020 2020  1351034361,.    
+00006f20: 2020 2020 2273 6570 5f74 6f5f 5749 5345      "sep_to_WISE
+00006f30: 5f73 6f75 7263 6522 3a30 2e31 3135 3832  _source":0.11582
+00006f40: 372c 0a20 2020 2020 2020 2022 7731 6d70  7,.        "w1mp
+00006f50: 726f 223a 3132 2e32 3931 2c0a 2020 2020  ro":12.291,.    
+00006f60: 2020 2020 2277 326d 7072 6f22 3a31 312e      "w2mpro":11.
+00006f70: 3131 360a 2020 2020 7d2c 0a20 2020 2022  116.    },.    "
+00006f80: 3536 223a 7b0a 2020 2020 2020 2020 226e  56":{.        "n
+00006f90: 616d 6522 3a22 4154 3230 3230 6166 6165  ame":"AT2020afae
+00006fa0: 222c 0a20 2020 2020 2020 2022 7470 6561  ",.        "tpea
+00006fb0: 6b22 3a35 3838 3637 2e32 2c0a 2020 2020  k":58867.2,.    
+00006fc0: 2020 2020 2272 6973 6574 696d 6522 3a22      "risetime":"
+00006fd0: 3330 2e32 222c 0a20 2020 2020 2020 2022  30.2",.        "
+00006fe0: 6661 6465 7469 6d65 223a 2234 322e 3022  fadetime":"42.0"
+00006ff0: 2c0a 2020 2020 2020 2020 2264 665f 6f76  ,.        "df_ov
+00007000: 6572 5f72 6d73 223a 352e 322c 0a20 2020  er_rms":5.2,.   
+00007010: 2020 2020 2022 6466 5f72 6177 223a 2230       "df_raw":"0
+00007020: 2e33 3520 5c75 3030 6231 2030 2e30 3222  .35 \u00b1 0.02"
+00007030: 2c0a 2020 2020 2020 2020 227a 223a 225c  ,.        "z":"\
+00007040: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
+00007050: 226d 6268 223a 225c 7532 3031 3322 2c0a  "mbh":"\u2013",.
+00007060: 2020 2020 2020 2020 2270 6167 6e74 6465          "pagntde
+00007070: 223a 352e 3538 352c 0a20 2020 2020 2020  ":5.585,.       
+00007080: 2022 636c 6173 7322 3a22 5c75 3230 3133   "class":"\u2013
+00007090: 222c 0a20 2020 2020 2020 2022 6466 223a  ",.        "df":
+000070a0: 302e 3335 2c0a 2020 2020 2020 2020 2264  0.35,.        "d
+000070b0: 665f 6522 3a30 2e30 322c 0a20 2020 2020  f_e":0.02,.     
+000070c0: 2020 2022 7261 223a 3736 2e32 3333 3038     "ra":76.23308
+000070d0: 3736 3839 372c 0a20 2020 2020 2020 2022  76897,.        "
+000070e0: 6465 6322 3a39 2e31 3534 3138 3030 3331  dec":9.154180031
+000070f0: 2c0a 2020 2020 2020 2020 2241 6c6c 5749  ,.        "AllWI
+00007100: 5345 5f69 6422 3a37 3635 3130 3930 3031  SE_id":765109001
+00007110: 3335 3130 3332 3835 352c 0a20 2020 2020  351032855,.     
+00007120: 2020 2022 7365 705f 746f 5f57 4953 455f     "sep_to_WISE_
+00007130: 736f 7572 6365 223a 302e 3037 3439 3736  source":0.074976
+00007140: 2c0a 2020 2020 2020 2020 2277 316d 7072  ,.        "w1mpr
+00007150: 6f22 3a31 332e 3539 352c 0a20 2020 2020  o":13.595,.     
+00007160: 2020 2022 7732 6d70 726f 223a 3133 2e33     "w2mpro":13.3
+00007170: 3131 0a20 2020 207d 2c0a 2020 2020 2235  11.    },.    "5
+00007180: 3722 3a7b 0a20 2020 2020 2020 2022 6e61  7":{.        "na
+00007190: 6d65 223a 2241 5432 3032 306d 7722 2c0a  me":"AT2020mw",.
+000071a0: 2020 2020 2020 2020 2274 7065 616b 223a          "tpeak":
+000071b0: 3538 3836 372e 332c 0a20 2020 2020 2020  58867.3,.       
+000071c0: 2022 7269 7365 7469 6d65 223a 2231 322e   "risetime":"12.
+000071d0: 3622 2c0a 2020 2020 2020 2020 2266 6164  6",.        "fad
+000071e0: 6574 696d 6522 3a22 3332 2e31 222c 0a20  etime":"32.1",. 
+000071f0: 2020 2020 2020 2022 6466 5f6f 7665 725f         "df_over_
+00007200: 726d 7322 3a36 2e38 2c0a 2020 2020 2020  rms":6.8,.      
+00007210: 2020 2264 665f 7261 7722 3a22 302e 3132    "df_raw":"0.12
+00007220: 205c 7530 3062 3120 302e 3031 222c 0a20   \u00b1 0.01",. 
+00007230: 2020 2020 2020 2022 7a22 3a22 5c75 3230         "z":"\u20
+00007240: 3133 222c 0a20 2020 2020 2020 2022 6d62  13",.        "mb
+00007250: 6822 3a22 5c75 3230 3133 222c 0a20 2020  h":"\u2013",.   
+00007260: 2020 2020 2022 7061 676e 7464 6522 3a33       "pagntde":3
+00007270: 2e34 3134 2c0a 2020 2020 2020 2020 2263  .414,.        "c
+00007280: 6c61 7373 223a 225c 7532 3031 3322 2c0a  lass":"\u2013",.
+00007290: 2020 2020 2020 2020 2264 6622 3a30 2e31          "df":0.1
+000072a0: 322c 0a20 2020 2020 2020 2022 6466 5f65  2,.        "df_e
+000072b0: 223a 302e 3031 2c0a 2020 2020 2020 2020  ":0.01,.        
+000072c0: 2272 6122 3a31 3232 2e36 3936 3938 3236  "ra":122.6969826
+000072d0: 3436 2c0a 2020 2020 2020 2020 2264 6563  46,.        "dec
+000072e0: 223a 3131 2e35 3231 3133 3030 3337 332c  ":11.5211300373,
+000072f0: 0a20 2020 2020 2020 2022 416c 6c57 4953  .        "AllWIS
+00007300: 455f 6964 223a 2222 2c0a 2020 2020 2020  E_id":"",.      
+00007310: 2020 2273 6570 5f74 6f5f 5749 5345 5f73    "sep_to_WISE_s
+00007320: 6f75 7263 6522 3a6e 756c 6c2c 0a20 2020  ource":null,.   
+00007330: 2020 2020 2022 7731 6d70 726f 223a 6e75       "w1mpro":nu
+00007340: 6c6c 2c0a 2020 2020 2020 2020 2277 326d  ll,.        "w2m
+00007350: 7072 6f22 3a6e 756c 6c0a 2020 2020 7d2c  pro":null.    },
+00007360: 0a20 2020 2022 3538 223a 7b0a 2020 2020  .    "58":{.    
+00007370: 2020 2020 226e 616d 6522 3a22 4154 3230      "name":"AT20
+00007380: 3230 6971 222c 0a20 2020 2020 2020 2022  20iq",.        "
+00007390: 7470 6561 6b22 3a35 3838 3738 2e31 2c0a  tpeak":58878.1,.
+000073a0: 2020 2020 2020 2020 2272 6973 6574 696d          "risetim
+000073b0: 6522 3a22 3232 2e37 222c 0a20 2020 2020  e":"22.7",.     
+000073c0: 2020 2022 6661 6465 7469 6d65 223a 2237     "fadetime":"7
+000073d0: 312e 3522 2c0a 2020 2020 2020 2020 2264  1.5",.        "d
+000073e0: 665f 6f76 6572 5f72 6d73 223a 3234 2e35  f_over_rms":24.5
+000073f0: 2c0a 2020 2020 2020 2020 2264 665f 7261  ,.        "df_ra
+00007400: 7722 3a22 302e 3435 205c 7530 3062 3120  w":"0.45 \u00b1 
+00007410: 302e 3031 222c 0a20 2020 2020 2020 2022  0.01",.        "
+00007420: 7a22 3a22 302e 3039 3622 2c0a 2020 2020  z":"0.096",.    
+00007430: 2020 2020 226d 6268 223a 2236 2e33 3720      "mbh":"6.37 
+00007440: 2856 3231 2922 2c0a 2020 2020 2020 2020  (V21)",.        
+00007450: 2270 6167 6e74 6465 223a 302e 3030 332c  "pagntde":0.003,
+00007460: 0a20 2020 2020 2020 2022 636c 6173 7322  .        "class"
+00007470: 3a22 5444 453f 222c 0a20 2020 2020 2020  :"TDE?",.       
+00007480: 2022 6466 223a 302e 3435 2c0a 2020 2020   "df":0.45,.    
+00007490: 2020 2020 2264 665f 6522 3a30 2e30 312c      "df_e":0.01,
+000074a0: 0a20 2020 2020 2020 2022 7261 223a 3433  .        "ra":43
+000074b0: 2e38 3332 3136 372c 0a20 2020 2020 2020  .832167,.       
+000074c0: 2022 6465 6322 3a2d 3131 2e34 3133 3531   "dec":-11.41351
+000074d0: 312c 0a20 2020 2020 2020 2022 416c 6c57  1,.        "AllW
+000074e0: 4953 455f 6964 223a 3433 3230 3132 3230  ISE_id":43201220
+000074f0: 3133 3531 3035 3232 3338 2c0a 2020 2020  1351052238,.    
+00007500: 2020 2020 2273 6570 5f74 6f5f 5749 5345      "sep_to_WISE
+00007510: 5f73 6f75 7263 6522 3a30 2e31 3430 3633  _source":0.14063
+00007520: 312c 0a20 2020 2020 2020 2022 7731 6d70  1,.        "w1mp
+00007530: 726f 223a 3134 2e35 3636 2c0a 2020 2020  ro":14.566,.    
+00007540: 2020 2020 2277 326d 7072 6f22 3a31 342e      "w2mpro":14.
+00007550: 3230 340a 2020 2020 7d2c 0a20 2020 2022  204.    },.    "
+00007560: 3539 223a 7b0a 2020 2020 2020 2020 226e  59":{.        "n
+00007570: 616d 6522 3a22 4154 3230 3139 7867 6722  ame":"AT2019xgg"
+00007580: 2c0a 2020 2020 2020 2020 2274 7065 616b  ,.        "tpeak
+00007590: 223a 3538 3839 312e 322c 0a20 2020 2020  ":58891.2,.     
+000075a0: 2020 2022 7269 7365 7469 6d65 223a 2238     "risetime":"8
+000075b0: 312e 3622 2c0a 2020 2020 2020 2020 2266  1.6",.        "f
+000075c0: 6164 6574 696d 6522 3a22 3434 362e 3222  adetime":"446.2"
+000075d0: 2c0a 2020 2020 2020 2020 2264 665f 6f76  ,.        "df_ov
+000075e0: 6572 5f72 6d73 223a 342e 342c 0a20 2020  er_rms":4.4,.   
+000075f0: 2020 2020 2022 6466 5f72 6177 223a 2230       "df_raw":"0
+00007600: 2e31 3320 5c75 3030 6231 2030 2e30 3122  .13 \u00b1 0.01"
+00007610: 2c0a 2020 2020 2020 2020 227a 223a 225c  ,.        "z":"\
+00007620: 7532 3031 3322 2c0a 2020 2020 2020 2020  u2013",.        
+00007630: 226d 6268 223a 225c 7532 3031 3322 2c0a  "mbh":"\u2013",.
+00007640: 2020 2020 2020 2020 2270 6167 6e74 6465          "pagntde
+00007650: 223a 362e 3039 312c 0a20 2020 2020 2020  ":6.091,.       
+00007660: 2022 636c 6173 7322 3a22 5c75 3230 3133   "class":"\u2013
+00007670: 222c 0a20 2020 2020 2020 2022 6466 223a  ",.        "df":
+00007680: 302e 3133 2c0a 2020 2020 2020 2020 2264  0.13,.        "d
+00007690: 665f 6522 3a30 2e30 312c 0a20 2020 2020  f_e":0.01,.     
+000076a0: 2020 2022 7261 223a 3136 322e 3238 3432     "ra":162.2842
+000076b0: 3430 382c 0a20 2020 2020 2020 2022 6465  408,.        "de
+000076c0: 6322 3a33 372e 3232 3131 3030 372c 0a20  c":37.2211007,. 
+000076d0: 2020 2020 2020 2022 416c 6c57 4953 455f         "AllWISE_
+000076e0: 6964 223a 3136 3239 3133 3738 3031 3335  id":162913780135
+000076f0: 3130 3130 3539 372c 0a20 2020 2020 2020  1010597,.       
+00007700: 2022 7365 705f 746f 5f57 4953 455f 736f   "sep_to_WISE_so
+00007710: 7572 6365 223a 312e 3030 3035 3231 2c0a  urce":1.000521,.
+00007720: 2020 2020 2020 2020 2277 316d 7072 6f22          "w1mpro"
+00007730: 3a31 342e 3838 382c 0a20 2020 2020 2020  :14.888,.       
+00007740: 2022 7732 6d70 726f 223a 3134 2e31 3932   "w2mpro":14.192
+00007750: 0a20 2020 207d 2c0a 2020 2020 2236 3022  .    },.    "60"
+00007760: 3a7b 0a20 2020 2020 2020 2022 6e61 6d65  :{.        "name
+00007770: 223a 2241 5432 3032 3061 7471 222c 0a20  ":"AT2020atq",. 
+00007780: 2020 2020 2020 2022 7470 6561 6b22 3a35         "tpeak":5
+00007790: 3839 3033 2e32 2c0a 2020 2020 2020 2020  8903.2,.        
+000077a0: 2272 6973 6574 696d 6522 3a22 3339 2e33  "risetime":"39.3
+000077b0: 222c 0a20 2020 2020 2020 2022 6661 6465  ",.        "fade
+000077c0: 7469 6d65 223a 2232 3035 2e35 222c 0a20  time":"205.5",. 
+000077d0: 2020 2020 2020 2022 6466 5f6f 7665 725f         "df_over_
+000077e0: 726d 7322 3a32 302e 382c 0a20 2020 2020  rms":20.8,.     
+000077f0: 2020 2022 6466 5f72 6177 223a 2230 2e36     "df_raw":"0.6
+00007800: 3620 5c75 3030 6231 2030 2e30 3122 2c0a  6 \u00b1 0.01",.
+00007810: 2020 2020 2020 2020 227a 223a 225c 7532          "z":"\u2
+00007820: 3031 3322 2c0a 2020 2020 2020 2020 226d  013",.        "m
+00007830: 6268 223a 225c 7532 3031 3322 2c0a 2020  bh":"\u2013",.  
+00007840: 2020 2020 2020 2270 6167 6e74 6465 223a        "pagntde":
+00007850: 302e 3032 2c0a 2020 2020 2020 2020 2263  0.02,.        "c
+00007860: 6c61 7373 223a 225c 7532 3031 3322 2c0a  lass":"\u2013",.
+00007870: 2020 2020 2020 2020 2264 6622 3a30 2e36          "df":0.6
+00007880: 362c 0a20 2020 2020 2020 2022 6466 5f65  6,.        "df_e
+00007890: 223a 302e 3031 2c0a 2020 2020 2020 2020  ":0.01,.        
+000078a0: 2272 6122 3a31 3032 2e33 3233 3533 3831  "ra":102.3235381
+000078b0: 2c0a 2020 2020 2020 2020 2264 6563 223a  ,.        "dec":
+000078c0: 3632 2e35 3133 3430 3035 2c0a 2020 2020  62.5134005,.    
+000078d0: 2020 2020 2241 6c6c 5749 5345 5f69 6422      "AllWISE_id"
+000078e0: 3a31 3031 3031 3632 3030 3133 3531 3034  :101016200135104
+000078f0: 3734 3336 2c0a 2020 2020 2020 2020 2273  7436,.        "s
+00007900: 6570 5f74 6f5f 5749 5345 5f73 6f75 7263  ep_to_WISE_sourc
+00007910: 6522 3a30 2e30 3731 3832 2c0a 2020 2020  e":0.07182,.    
+00007920: 2020 2020 2277 316d 7072 6f22 3a31 352e      "w1mpro":15.
+00007930: 3537 312c 0a20 2020 2020 2020 2022 7732  571,.        "w2
+00007940: 6d70 726f 223a 3134 2e37 3839 0a20 2020  mpro":14.789.   
+00007950: 207d 2c0a 2020 2020 2236 3122 3a7b 0a20   },.    "61":{. 
+00007960: 2020 2020 2020 2022 6e61 6d65 223a 2241         "name":"A
+00007970: 5432 3032 3161 6575 6a22 2c0a 2020 2020  T2021aeuj",.    
+00007980: 2020 2020 2274 7065 616b 223a 3538 3937      "tpeak":5897
+00007990: 342e 322c 0a20 2020 2020 2020 2022 7269  4.2,.        "ri
+000079a0: 7365 7469 6d65 223a 2237 392e 3022 2c0a  setime":"79.0",.
+000079b0: 2020 2020 2020 2020 2266 6164 6574 696d          "fadetim
+000079c0: 6522 3a22 3233 332e 3522 2c0a 2020 2020  e":"233.5",.    
+000079d0: 2020 2020 2264 665f 6f76 6572 5f72 6d73      "df_over_rms
+000079e0: 223a 3138 2e31 2c0a 2020 2020 2020 2020  ":18.1,.        
+000079f0: 2264 665f 7261 7722 3a22 302e 3230 205c  "df_raw":"0.20 \
+00007a00: 7530 3062 3120 302e 3031 222c 0a20 2020  u00b1 0.01",.   
+00007a10: 2020 2020 2022 7a22 3a22 302e 3639 3522       "z":"0.695"
+00007a20: 2c0a 2020 2020 2020 2020 226d 6268 223a  ,.        "mbh":
+00007a30: 225c 7532 3031 3322 2c0a 2020 2020 2020  "\u2013",.      
+00007a40: 2020 2270 6167 6e74 6465 223a 302e 3037    "pagntde":0.07
+00007a50: 312c 0a20 2020 2020 2020 2022 636c 6173  1,.        "clas
+00007a60: 7322 3a22 5c75 3230 3133 222c 0a20 2020  s":"\u2013",.   
+00007a70: 2020 2020 2022 6466 223a 302e 322c 0a20       "df":0.2,. 
+00007a80: 2020 2020 2020 2022 6466 5f65 223a 302e         "df_e":0.
+00007a90: 3031 2c0a 2020 2020 2020 2020 2272 6122  01,.        "ra"
+00007aa0: 3a31 3337 2e31 3037 3230 3433 3533 312c  :137.1072043531,
+00007ab0: 0a20 2020 2020 2020 2022 6465 6322 3a34  .        "dec":4
+00007ac0: 322e 3839 3438 3031 3930 3636 2c0a 2020  2.8948019066,.  
+00007ad0: 2020 2020 2020 2241 6c6c 5749 5345 5f69        "AllWISE_i
+00007ae0: 6422 3a31 3337 3531 3432 3430 3133 3531  d":1375142401351
+00007af0: 3035 3934 3030 2c0a 2020 2020 2020 2020  059400,.        
+00007b00: 2273 6570 5f74 6f5f 5749 5345 5f73 6f75  "sep_to_WISE_sou
+00007b10: 7263 6522 3a30 2e31 3833 3936 332c 0a20  rce":0.183963,. 
+00007b20: 2020 2020 2020 2022 7731 6d70 726f 223a         "w1mpro":
+00007b30: 3136 2e34 3531 2c0a 2020 2020 2020 2020  16.451,.        
+00007b40: 2277 326d 7072 6f22 3a31 352e 3538 310a  "w2mpro":15.581.
+00007b50: 2020 2020 7d2c 0a20 2020 2022 3632 223a      },.    "62":
+00007b60: 7b0a 2020 2020 2020 2020 226e 616d 6522  {.        "name"
+00007b70: 3a22 4154 3230 3230 686c 6522 2c0a 2020  :"AT2020hle",.  
+00007b80: 2020 2020 2020 2274 7065 616b 223a 3538        "tpeak":58
+00007b90: 3937 382e 332c 0a20 2020 2020 2020 2022  978.3,.        "
+00007ba0: 7269 7365 7469 6d65 223a 2233 322e 3722  risetime":"32.7"
+00007bb0: 2c0a 2020 2020 2020 2020 2266 6164 6574  ,.        "fadet
+00007bc0: 696d 6522 3a22 3632 2e39 222c 0a20 2020  ime":"62.9",.   
+00007bd0: 2020 2020 2022 6466 5f6f 7665 725f 726d       "df_over_rm
+00007be0: 7322 3a32 312e 302c 0a20 2020 2020 2020  s":21.0,.       
+00007bf0: 2022 6466 5f72 6177 223a 2230 2e33 3320   "df_raw":"0.33 
+00007c00: 5c75 3030 6231 2030 2e30 3122 2c0a 2020  \u00b1 0.01",.  
+00007c10: 2020 2020 2020 227a 223a 2230 2e31 3033        "z":"0.103
+00007c20: 222c 0a20 2020 2020 2020 2022 6d62 6822  ",.        "mbh"
+00007c30: 3a22 362e 3430 2028 4632 3029 222c 0a20  :"6.40 (F20)",. 
+00007c40: 2020 2020 2020 2022 7061 676e 7464 6522         "pagntde"
+00007c50: 3a30 2e30 3138 2c0a 2020 2020 2020 2020  :0.018,.        
+00007c60: 2263 6c61 7373 223a 2254 4445 3f22 2c0a  "class":"TDE?",.
+00007c70: 2020 2020 2020 2020 2264 6622 3a30 2e33          "df":0.3
+00007c80: 332c 0a20 2020 2020 2020 2022 6466 5f65  3,.        "df_e
+00007c90: 223a 302e 3031 2c0a 2020 2020 2020 2020  ":0.01,.        
+00007ca0: 2272 6122 3a31 3636 2e39 3238 3632 3731  "ra":166.9286271
+00007cb0: 2c0a 2020 2020 2020 2020 2264 6563 223a  ,.        "dec":
+00007cc0: 3734 2e36 3333 3933 3232 352c 0a20 2020  74.63393225,.   
+00007cd0: 2020 2020 2022 416c 6c57 4953 455f 6964       "AllWISE_id
+00007ce0: 223a 3136 3934 3137 3432 3031 3335 3130  ":16941742013510
+00007cf0: 3338 3834 392c 0a20 2020 2020 2020 2022  38849,.        "
+00007d00: 7365 705f 746f 5f57 4953 455f 736f 7572  sep_to_WISE_sour
+00007d10: 6365 223a 302e 3033 3332 3638 2c0a 2020  ce":0.033268,.  
+00007d20: 2020 2020 2020 2277 316d 7072 6f22 3a31        "w1mpro":1
+00007d30: 342e 3131 312c 0a20 2020 2020 2020 2022  4.111,.        "
+00007d40: 7732 6d70 726f 223a 3133 2e37 3536 0a20  w2mpro":13.756. 
+00007d50: 2020 207d 0a7d                              }.}
```

### Comparing `timewise_sup-0.4.8/PKG-INFO` & `timewise_sup-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timewise-sup
-Version: 0.4.8
+Version: 0.5.0
 Summary: The Timewise Subtraction Pipeline produces mid-infrared difference photometry based on measurements by the WISE satelite
 Home-page: https://gitlab.desy.de/jannisnecker/timewise_sup
 License: BSD-3-Clause
 Author: Jannis Necker
 Author-email: jannis.necker@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: BSD License
@@ -17,15 +17,15 @@
 Requires-Dist: corner (>=2.2.1,<3.0.0)
 Requires-Dist: extcats (>=2.4.3,<3.0.0)
 Requires-Dist: jupyterlab (>=4.0.0,<5.0.0) ; extra == "jupyter"
 Requires-Dist: matplotlib-venn (>=0.11.9,<0.12.0)
 Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
 Requires-Dist: nltk (>=3.7,<4.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
-Requires-Dist: timewise (==0.4.9)
+Requires-Dist: timewise (==0.4.10)
 Requires-Dist: tkpdfviewer (>=0.1,<0.2)
 Requires-Dist: uncertainties (>=3.1.7,<4.0.0)
 Project-URL: Documentation, https://jannisnecker.pages.desy.de/timewise_sup/docs/
 Project-URL: Repository, https://gitlab.desy.de/jannisnecker/timewise_sup
 Description-Content-Type: text/markdown
 
 [![CI](https://gitlab.desy.de/jannis.necker/timewise_sup/badges/main/pipeline.svg)](https://gitlab.desy.de/jannis.necker/timewise_sup/-/commits/main)
```

