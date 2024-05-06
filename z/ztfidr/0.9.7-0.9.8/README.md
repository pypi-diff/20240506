# Comparing `tmp/ztfidr-0.9.7.tar.gz` & `tmp/ztfidr-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztfidr-0.9.7.tar", last modified: Fri Jul 28 18:15:26 2023, max compression
+gzip compressed data, was "ztfidr-0.9.8.tar", last modified: Wed Dec 20 15:35:56 2023, max compression
```

## Comparing `ztfidr-0.9.7.tar` & `ztfidr-0.9.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-28 18:15:26.761319 ztfidr-0.9.7/
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.7/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-07-28 18:15:26.761199 ztfidr-0.9.7/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.7/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-07-28 18:15:26.761358 ztfidr-0.9.7/setup.cfg
--rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-07-28 18:15:08.000000 ztfidr-0.9.7/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-28 18:15:26.760447 ztfidr-0.9.7/ztfidr/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      126 2023-07-28 18:15:13.000000 ztfidr-0.9.7/ztfidr/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     5542 2023-07-17 14:06:04.000000 ztfidr-0.9.7/ztfidr/host.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    16159 2023-07-13 12:05:49.000000 ztfidr-0.9.7/ztfidr/io.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    23052 2023-07-28 18:14:33.000000 ztfidr-0.9.7/ztfidr/lightcurve.py
--rw-r--r--   0 rigault   (2358) staff       (20)    18672 2023-05-23 08:15:23.000000 ztfidr-0.9.7/ztfidr/linefitter.py
--rw-r--r--   0 rigault   (2358) staff       (20)    25901 2023-07-13 12:46:52.000000 ztfidr-0.9.7/ztfidr/plotting.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1091 2023-06-18 10:58:06.000000 ztfidr-0.9.7/ztfidr/salt2.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    25280 2023-06-20 08:13:19.000000 ztfidr-0.9.7/ztfidr/sample.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.7/ztfidr/script.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10255 2023-05-24 11:57:29.000000 ztfidr-0.9.7/ztfidr/snid.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.7/ztfidr/spectroscopy.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.7/ztfidr/target.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    23636 2023-07-27 15:37:39.000000 ztfidr-0.9.7/ztfidr/typing.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     4225 2023-07-05 21:38:13.000000 ztfidr-0.9.7/ztfidr/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-28 18:15:26.761042 ztfidr-0.9.7/ztfidr.egg-info/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-07-28 18:15:26.000000 ztfidr-0.9.7/ztfidr.egg-info/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)      392 2023-07-28 18:15:26.000000 ztfidr-0.9.7/ztfidr.egg-info/SOURCES.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-07-28 18:15:26.000000 ztfidr-0.9.7/ztfidr.egg-info/dependency_links.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-07-28 18:15:26.000000 ztfidr-0.9.7/ztfidr.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-12-20 15:35:56.217236 ztfidr-0.9.8/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.8/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-12-20 15:35:56.217060 ztfidr-0.9.8/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.8/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-12-20 15:35:56.217290 ztfidr-0.9.8/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-12-20 15:35:47.000000 ztfidr-0.9.8/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-12-20 15:35:56.216230 ztfidr-0.9.8/ztfidr/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      126 2023-12-20 15:35:09.000000 ztfidr-0.9.8/ztfidr/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     5542 2023-07-17 14:06:04.000000 ztfidr-0.9.8/ztfidr/host.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    12891 2023-10-17 16:01:52.000000 ztfidr-0.9.8/ztfidr/io.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    23284 2023-10-20 11:24:16.000000 ztfidr-0.9.8/ztfidr/lightcurve.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    18672 2023-05-23 08:15:23.000000 ztfidr-0.9.8/ztfidr/linefitter.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    25899 2023-11-24 09:15:54.000000 ztfidr-0.9.8/ztfidr/plotting.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1090 2023-10-20 09:20:41.000000 ztfidr-0.9.8/ztfidr/salt2.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    27800 2023-11-16 17:11:16.000000 ztfidr-0.9.8/ztfidr/sample.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.8/ztfidr/script.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10255 2023-05-24 11:57:29.000000 ztfidr-0.9.8/ztfidr/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.8/ztfidr/spectroscopy.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.8/ztfidr/target.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    23636 2023-07-27 15:37:39.000000 ztfidr-0.9.8/ztfidr/typing.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     4225 2023-07-05 21:38:13.000000 ztfidr-0.9.8/ztfidr/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-12-20 15:35:56.216891 ztfidr-0.9.8/ztfidr.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-12-20 15:35:56.000000 ztfidr-0.9.8/ztfidr.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      392 2023-12-20 15:35:56.000000 ztfidr-0.9.8/ztfidr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-12-20 15:35:56.000000 ztfidr-0.9.8/ztfidr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-12-20 15:35:56.000000 ztfidr-0.9.8/ztfidr.egg-info/top_level.txt
```

### Comparing `ztfidr-0.9.7/LICENSE` & `ztfidr-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.7/README.md` & `ztfidr-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.7/setup.py` & `ztfidr-0.9.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.9.7'
+VERSION = '0.9.8'
         
 setup(name='ztfidr',
       version=VERSION,
       description='Tools for ZTF Ia *Internal*DataReleases',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/ztfdr',
```

### Comparing `ztfidr-0.9.7/ztfidr/host.py` & `ztfidr-0.9.8/ztfidr/host.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.7/ztfidr/io.py` & `ztfidr-0.9.8/ztfidr/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import os
 import warnings
 import pandas
 import numpy as np
 IDR_PATH = os.getenv("ZTFIDRPATH", "./dr2")
 
-__all__ = ["get_targets_data",
-           "get_host_data",
-           "get_localhost_data",           
-           "get_autotyping"]
+__all__ = ["get_targets_data"]
     
 # ================== #
 #                    #
 #   TOP LEVEL        #
 #                    #
 # ================== #
 def get_targets_data(saltmodel="default"):
@@ -37,31 +34,14 @@
     data_ = data_.loc[target_list["ztfname"]]
 
     # adding classification
     typing = get_target_typing()
     data_ = data_.join(typing["classification"], how="left")
     return data_, saltmodel
 
-def get_localhost_data(local_nkpc=2, which="mag"):
-    """ """
-    hostlocal = get_host_local(nkpc=2, which="mag")
-    hostcoords = get_host_coords()
-    dlr = get_host_mags().xs("global", axis=1)["host_dlr"]
-    hostcoords = hostcoords.merge(dlr, left_index=True, right_index=True)
-    return hostcoords.merge(hostlocal, left_index=True, right_index=True,
-                                how="left")
-
-def get_host_data(local_nkpc=2, which="mag"):
-    """ """
-    hostmag = get_host_mags().xs("global", axis=1)
-    hostcoords = get_host_coords()
-    return hostcoords.merge(hostmag, left_index=True, right_index=True,
-                                how="left")
-                                
-
 # ================== #
 #                    #
 #   BASICS           #
 #                    #
 # ================== #
 def get_targetlist(load=True, **kwargs):
     """ official list of target to use for dr2 """
@@ -192,32 +172,14 @@
     data = data.join(snidauto, on="ztfname")
     data = data.join(hostz, on="ztfname")
  #   data = data.join(override, on="ztfname")
     data
     
     return data
     
-def get_snidauto_redshift(load=True, **kwargs):
-    """ """
-    filepath = os.path.join(IDR_PATH,"tables",
-                                ".dataset_creation/redshifts/ztfdr2_snid_redshifts.csv")
-    if not load:
-        return filepath
-    
-    return pandas.read_csv(filepath, index_col=0, **kwargs)
-
-def get_snidauto_specfile_redshift(load=True, **kwargs):
-    """ """
-    filepath = os.path.join(IDR_PATH,"tables",
-                                ".dataset_creation/redshifts/snidauto_ianorm.csv")
-    if not load:
-        return filepath
-    
-    return pandas.read_csv(filepath, index_col=0, **kwargs)
-
 # Coordinates
 def get_coords_data(load=True, index_col=0, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH, "tables",
                             "ztfdr2_coordinates.csv")
     if not load:
         return filepath
@@ -270,79 +232,45 @@
     return f"{saltmodel} v={version}"
 
 # ================== #
 #                    #
 #   HOST             #
 #                    #
 # ================== #
-def get_host_coords(load=True, **kwargs):
+def get_globalhost_data(load=True, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH, "tables",
-                            ".dataset_creation/host_prop/host_photometry/global/archive/ztfdr2_hostcoords.csv")
+                            "ztfdr2_globalhost_prop.csv")
     if not load:
         return filepath
     
-    return pandas.read_csv(filepath, **{**dict(sep=" "),**kwargs}).set_index("ztfname")
+    return pandas.read_csv(filepath, index_col=0)
 
-def get_host_local(nkpc=2, which="mag", load=True, **kwargs):
+def get_localhost_data(load=True, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH, "tables",
-                            f".dataset_creation/host_prop/host_photometry/local/archive/ztfdr2_local{nkpc}kpc_{which}.csv")
+                            "ztfdr2_local2kpc_prop.csv")
     if not load:
         return filepath
-    if not os.path.isfile(filepath):
-        raise IOError(f"no such file {filepath}")
+    
+    return pandas.read_csv(filepath, index_col=0)
 
-    return pandas.read_csv(filepath, index_col=0, **kwargs)
 
-def get_host_sedfit(nkpc=2, load=True, **kwargs):
+def get_globalhost_mag():
     """ """
     filepath = os.path.join(IDR_PATH, "tables",
-                            f".dataset_creation/host_prop/host_properties/local/archive/ztfdr2_local{nkpc}kpc_sedfit.csv")
-    if not load:
-        return filepath
-    if not os.path.isfile(filepath):
-        raise IOError(f"no such file {filepath}")
-
-    return pandas.read_csv(filepath, index_col=0, **kwargs)
+                            ".dataset_creation/host_prop/host_photometry/ztfdr2_global_imcat_mag.csv")
+    return pandas.read_csv(filepath, index_col=0)
     
 
-def get_host_mags(load=True, index_col=0, raw=False, **kwargs):
+def get_localhost_mag():
     """ """
     filepath = os.path.join(IDR_PATH, "tables",
-                            ".dataset_creation/host_prop/host_photometry/global/archive/ztfdr2_hostmags.csv")
-    if not load:
-        return filepath
-
-    host_alldata = pandas.read_csv(filepath, index_col=index_col, **kwargs)
-    if raw:
-        return host_alldata
-
-    def _get_split_(which):
-        requested = f"{which}_mag"
-        if requested not in host_alldata:
-            raise ValueError(f"Unknown entry: {requested} (which={which})")
-
-        host_data = host_alldata[requested].astype(str).str.replace("nan", "np.nan").str.replace("inf", "np.nan").apply(eval)
-        host_err = host_alldata[requested+"_err"].astype(str).str.replace("nan", "np.nan").str.replace("inf", "np.nan").apply(eval)
-        flagna = host_data.isna() + host_err.isna()
-        data = pandas.DataFrame(list(host_data[~flagna]), index=host_data[~flagna].index)
-        error = pandas.DataFrame(list(host_err[~flagna]), index=host_err[~flagna].index)
-        error.columns += "_err"
-        return pandas.merge(data, error, left_index=True, right_index=True)
-
-    kpc2 = _get_split_(which="local_2kpc")
-    kpc4 = _get_split_(which="local_4kpc")
-    host_cat = _get_split_(which="host_cat")
-    hglobal = pandas.merge(host_cat,
-                          host_alldata[["z","host_dlr"]].rename({"z":"redshift"}, axis=1), 
-                          left_index=True, right_index=True,
-                               how="outer")
-    return pandas.concat([kpc2, kpc4, hglobal], axis=1,
-                          keys=["2kpc", "4kpc", "global"])
+                            ".dataset_creation/host_prop/host_photometry/ztfdr2_local2_imcat_mag.csv")
+    return pandas.read_csv(filepath, index_col=0)
     
 # ================== #
 #                    #
 #   LIGHTCURVES      #
 #                    #
 # ================== #
 def get_target_lightcurve(target, test_exist=True, load=True):
```

### Comparing `ztfidr-0.9.7/ztfidr/lightcurve.py` & `ztfidr-0.9.8/ztfidr/lightcurve.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,27 +283,36 @@
         sncosmo_lc["flux"], sncosmo_lc["flux_err"] = mag_to_flux(sncosmo_lc["mag"],
                                                                  sncosmo_lc["mag_err"],
                                                                  zp=sncosmo_lc["zp"])
         return sncosmo_lc
 
     def fit_salt(self, free_parameters=['t0', 'x0', 'x1', 'c'],
                        min_detection=5, phase_range=[-10,30], filters=["ztfr","ztfg"],
-                       as_dataframe=False, which=None,
+                       as_dataframe=False, which=None, modelprop={},
                        **kwargs):
         """ """
         import sncosmo
         from astropy import table
         from .salt2 import salt2result_to_dataframe
+
         model = self.get_saltmodel(which=which)
+        
+        if modelprop:
+            model.set( **modelprop )
+            print(dict(zip(model.param_names, model.parameters)))
+            
         sncosmo_df = self.get_sncosmotable(min_detection=min_detection, 
                                            phase_range=phase_range, 
                                            filters=filters)
+        
         fitted_data = table.Table.from_pandas(sncosmo_df)
         (result, fitted_model) = sncosmo.fit_lc(fitted_data, model,
-                                            vparam_names=free_parameters,  **kwargs)
+                                                vparam_names=free_parameters,
+                                                **kwargs)
+         
         if as_dataframe:
             return salt2result_to_dataframe(result)
         
         return (fitted_data,model), (result, fitted_model)
 
     def fit_salt_perfilter(lc, filters=["ztfg",'ztfr','ztfi'],
                            min_detection=5, free_parameters=['t0','x0', 'x1'],
```

### Comparing `ztfidr-0.9.7/ztfidr/linefitter.py` & `ztfidr-0.9.8/ztfidr/linefitter.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.7/ztfidr/plotting.py` & `ztfidr-0.9.8/ztfidr/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,18 +225,18 @@
 
 from pprint import pprint
 import numpy as np
 
 
 def show_residual(data, key="pull", ax=None, axh=None, axc=None,
                   binstat="mean", bins=np.arange(-50,50, 0.25),
-                  main_color="C0", cmap_significance="Greys_r",
+                  main_color="C0", cmap_significance="GnBu_r",
                   incl_lef=True, incl_runningpull=False,
                   pull_color=None,
-                  blw=0.1, bs=8, bec="w",
+                  blw=0.1, bs=8, ="w",
                   **kwargs):
     """ """
     from matplotlib.colors import to_rgba
     from scipy import stats
     
     if ax is None:
         fig = plt.figure(figsize=[7,3])
@@ -324,15 +324,15 @@
         axh.set_ylim(*ax.get_ylim())
         clearwhich = ["bottom","right","top","left"] # "bottom"    
         [axh.spines[which].set_visible(False) for which in clearwhich]
 
     return fig
 
 def show_lc_residuals(data, fig=None, axes=None,
-                      incl_lef=True, cmap_significance="Greys", 
+                      incl_lef=True, cmap_significance="GnBu_r", 
                       binstat="mean", key="pull",
                       bincadence=[1,1,2], # g, r, i
                       incl_runningpull=True, incl_filtername=True,
                       incl_linelabel=True, 
                       scoef_i=3, incl_hist=True,
                       phase_lines = [-20, -15, -10, -5, 0, 10, 20, 30, 40, 50],
                       propaxes={},
@@ -342,15 +342,15 @@
     # data
     data_g = data[data["filter"]=="ztfg"]
     data_r = data[data["filter"]=="ztfr"]
     data_i = data[data["filter"]=="ztfi"]
 
     
     left = propaxes.get("left", 0.1)
-    bottom, height = propaxes.get("bottom",0.1), propaxes.get("height", 0.27)
+    bottom, height = propaxes.get("bottom", 0.1), propaxes.get("height", 0.27)
     vspan, hspan = propaxes.get("vspan", 0.015),  propaxes.get("hspan", 0.001)
     width, hwidth = propaxes.get("width", 0.78),  propaxes.get("hwidth", 0.1)
     cvspan = propaxes.get("cvspan", 0.)
     print(cvspan)
     # -- Figure layout -- #
     if axes is None:
         if fig is None:
```

### Comparing `ztfidr-0.9.7/ztfidr/salt2.py` & `ztfidr-0.9.8/ztfidr/salt2.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import warnings
 from ztfquery import filters
 import numpy as np
 import pandas
 filters.load_p48_filters_to_sncosmo(basename="p48") # p48g etc.
 
 
-from .io import get_salt2params
+from .io import get_saltparams
 try:
-    SALT2PARAMS = get_salt2params()
+    SALT2PARAMS = get_saltparams()
 except:
     warnings.warn("Failed to load SALT2 parameters")
     SALT2PARAMS = None
 
 
 
 def salt2result_to_dataframe(result):
@@ -31,7 +31,8 @@
     # - Cov
     dcov = pandas.DataFrame(result["covariance"], columns=result.vparam_names, index=result.vparam_names)
     dcov.columns ="cov_"+dcov.columns
     
     # - merged
     return df.merge(dcov,  left_index=True, right_index=True, how="outer")
     
+
```

### Comparing `ztfidr-0.9.7/ztfidr/sample.py` & `ztfidr-0.9.8/ztfidr/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,85 @@
 
 import warnings
 import numpy as np
+from scipy import stats
 import pandas
 from . import io
-from astropy import time
-        
+from astropy import time, cosmology
+_COEFS = 1.57
+_COSMO = cosmology.Planck18
+# Top level method #
+
 def get_sample(**kwargs):
     """ Short to to Sample.load() """
     return Sample.load(**kwargs)
 
+
+def get_data(saltmodel="default", redshift_source=None, redshift_range=[0.015, 0.2],
+                 **kwargs):
+    """ Generic dataframe for the ZTF DR2 sample passing the cosmology cuts: 
+   
+    by default, (all could be updated through kwargs)
+    - goodcoverage=True,
+    - x1_range=[-3, 3],
+    - c_range=[-0.2, 0.3],
+    - t0_err_range=[0, 1],
+    - x1_err_range=[0, 1], 
+    - c_err_range=[0, 0.1],
+    - classification=["snia-norm", "snia", "snia-pec-91t"],
+    - data["fitprob"]>1e-4
+
+    """
+    sample = get_sample(saltmodel=saltmodel)
+    
+    prop = { **dict(goodcoverage=True,
+                    x1_range=[-3, 3],
+                    c_range=[-0.2, 0.3],
+                    t0_err_range=[0, 1],
+                    x1_err_range=[0, 1], 
+                    c_err_range=[0, 0.1],
+                    classification=["snia-norm", "snia", "snia-pec-91t"],
+                    redshift_range=redshift_range,
+                    redshift_source = redshift_source),
+              **kwargs}
+    
+    data = sample.get_data(**prop)
+    data = data[data["fitprob"]>1e-4]
+    
+    # Hubble Residuals    
+    data['mag'] = -2.5 * np.log10( data["x0"] ) + 19*_COEFS  - _COSMO.distmod(data["redshift"].values).value
+    data["mag_err"] =  +2.5/np.log(10) * data["x0_err"] / data["x0"]
+    data["cov_mag_c"] = 2.5*np.array(data['cov_x0_c'])/(np.log(10)*data['x0'])
+    data["cov_mag_x1"] = 2.5*np.array(data['cov_x0_x1'])/(np.log(10)*data['x0'])
+    
+    # Environmental data
+    localmags = io.get_localhost_mag()
+    globaldata = io.get_globalhost_data()
+    globalmags = io.get_globalhost_mag()
+    globaldata["mass_err"] = globaldata["mass_err"]/2.
+    
+    localmags["localcolor"] = localmags["PS1g"] - localmags["PS1z"]
+    localmags["localcolor_err"] = np.sqrt(localmags["PS1g_err"]**2 + localmags["PS1z_err"]**2)
+    
+    #localmags["mass"] = localmags["PS1g"] - localmags["PS1z"]
+    data = data.join(localmags[["localcolor","localcolor_err"]].loc[data.index])
+    data = data.join(globaldata[["mass","mass_err"]].loc[data.index])
+    data = data.join(globalmags[["PS1r"]].loc[data.index])
+    ## Standardisation parameters
+
+    lcolor_cut = 1
+    data["h_lowcolor"] = stats.norm.cdf(lcolor_cut, loc=data["localcolor"], scale=data["localcolor_err"])
+    data["h_lowcolor_err"] = 1e-3
+    
+    data["h_lowmass"] = stats.norm.cdf(10, loc=data["mass"], scale=data["mass_err"])
+    data["h_lowmass_err"] = 1e-3
+
+    return data.copy()
+
+
 def _get_coverage_(phase_df, prefix=None):
     """ """
     if prefix is None:
         prefix = ""
 
     n_points  = phase_df.groupby(level=0).size().to_frame(f"n_{prefix}points")
     n_bands   = ((phase_df.groupby(level=[0,1]).size()>0).groupby(level=0).sum()).to_frame(f"n_{prefix}bands")
@@ -422,15 +489,15 @@
         warnings.warn("building phase coverage takes ~30s.")
         
         import pandas
         from . import io
         phases = []
         data = self.get_data()
         
-        lcdata = io.get_lightcurve_datafile().set_index("ztfname").loc[data.index]
+        lcdata = io.get_lightcurve_datafile(contains=".csv").set_index("ztfname").loc[data.index]
         dfs = pandas.concat([pandas.read_csv(f_, delim_whitespace=True, comment='#') for f_ in lcdata["fullpath"]],
                                 keys=data.index)
         dfs["phase"] = dfs["mjd"] - data["t0"].reindex(dfs.index, level=0)
         dfs["detection"] = dfs["flux"]/dfs["flux_err"]
         phase_df = dfs.reset_index().set_index(["ztfname","filter"])[["phase","detection","flag","in_baseline"]]
         if store:
             filepath = io.get_phase_coverage(load=False)
@@ -446,15 +513,14 @@
                           ax=None, data=None, dataprop={},
                           facecolor=None, edgecolor=None, lw=2,
                           nsigma_range=3, npoints=1000,
                           density=False, normed_one=False,
                           **kwargs):
         """ """
         from matplotlib.colors import to_rgba
-        from scipy import stats
 
         # axes
         if ax is None:
             import matplotlib.pyplot as mpl
             fig = mpl.figure(figsize=[6,3])
             ax = fig.add_axes([0.1,0.2,0.8,0.7])
         else:
```

### Comparing `ztfidr-0.9.7/ztfidr/script.py` & `ztfidr-0.9.8/ztfidr/script.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.7/ztfidr/snid.py` & `ztfidr-0.9.8/ztfidr/snid.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.7/ztfidr/spectroscopy.py` & `ztfidr-0.9.8/ztfidr/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.7/ztfidr/target.py` & `ztfidr-0.9.8/ztfidr/target.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.7/ztfidr/typing.py` & `ztfidr-0.9.8/ztfidr/typing.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.7/ztfidr/utils.py` & `ztfidr-0.9.8/ztfidr/utils.py`

 * *Files identical despite different names*

