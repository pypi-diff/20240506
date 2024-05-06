# Comparing `tmp/easyfermi-2.0.8.tar.gz` & `tmp/easyfermi-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfermi-2.0.8.tar", last modified: Mon Feb 26 15:44:38 2024, max compression
+gzip compressed data, was "easyfermi-2.0.9.tar", last modified: Wed Feb 28 11:00:43 2024, max compression
```

## Comparing `easyfermi-2.0.8.tar` & `easyfermi-2.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2024-02-26 15:44:38.860198 easyfermi-2.0.8/
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1522 2022-01-31 12:02:33.000000 easyfermi-2.0.8/LICENSE.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)      996 2024-02-26 15:44:38.860198 easyfermi-2.0.8/PKG-INFO
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)      453 2024-02-02 10:02:39.000000 easyfermi-2.0.8/README.md
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2024-02-26 15:44:38.848198 easyfermi-2.0.8/easyfermi/
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)       63 2024-02-06 14:47:20.000000 easyfermi-2.0.8/easyfermi/__init__.py
--rw-rw-r--   0 raniere   (1000) raniere   (1000)   223455 2024-02-26 12:46:40.000000 easyfermi-2.0.8/easyfermi/easyfermi.py
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2024-02-26 15:44:38.848198 easyfermi-2.0.8/easyfermi/resources/
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2024-02-26 15:44:38.856198 easyfermi-2.0.8/easyfermi/resources/ebl/
--rw-rw-r--   0 raniere   (1000) raniere   (1000)   431576 2023-10-27 15:39:40.000000 easyfermi-2.0.8/easyfermi/resources/ebl/ebl_dominguez11.fits.gz
--rw-rw-r--   0 raniere   (1000) raniere   (1000)   274043 2023-10-27 15:40:33.000000 easyfermi-2.0.8/easyfermi/resources/ebl/ebl_franceschini.fits.gz
--rw-rw-r--   0 raniere   (1000) raniere   (1000)  2467682 2024-01-25 16:25:28.000000 easyfermi-2.0.8/easyfermi/resources/ebl/ebl_franceschini_2017.fits.gz
--rw-rw-r--   0 raniere   (1000) raniere   (1000)   643130 2024-01-25 16:25:20.000000 easyfermi-2.0.8/easyfermi/resources/ebl/ebl_saldana-lopez_2021.fits.gz
--rw-rw-r--   0 raniere   (1000) raniere   (1000)   120837 2024-01-31 21:15:35.000000 easyfermi-2.0.8/easyfermi/resources/ebl/frd_abs.fits.gz
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2024-02-26 15:44:38.856198 easyfermi-2.0.8/easyfermi/resources/images/
--rw-rw-r--   0 raniere   (1000) raniere   (1000)    31775 2024-02-02 10:07:14.000000 easyfermi-2.0.8/easyfermi/resources/images/download_logo.png
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)    40332 2022-01-15 16:04:30.000000 easyfermi-2.0.8/easyfermi/resources/images/easyFermiIcon.png
--rw-rw-r--   0 raniere   (1000) raniere   (1000)   150411 2024-02-06 14:48:42.000000 easyfermi-2.0.8/easyfermi/resources/images/easyFermiWindow.png
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)   121691 2021-11-23 14:18:26.000000 easyfermi-2.0.8/easyfermi/resources/images/fermi.png
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2024-02-26 15:44:38.848198 easyfermi-2.0.8/easyfermi.egg-info/
--rw-rw-r--   0 raniere   (1000) raniere   (1000)      996 2024-02-26 15:44:38.000000 easyfermi-2.0.8/easyfermi.egg-info/PKG-INFO
--rw-rw-r--   0 raniere   (1000) raniere   (1000)      627 2024-02-26 15:44:38.000000 easyfermi-2.0.8/easyfermi.egg-info/SOURCES.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)        1 2024-02-26 15:44:38.000000 easyfermi-2.0.8/easyfermi.egg-info/dependency_links.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)       10 2024-02-26 15:44:38.000000 easyfermi-2.0.8/easyfermi.egg-info/top_level.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)       38 2024-02-26 15:44:38.860198 easyfermi-2.0.8/setup.cfg
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1228 2024-02-26 15:44:08.000000 easyfermi-2.0.8/setup.py
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2024-02-28 11:00:43.656098 easyfermi-2.0.9/
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1522 2022-01-31 12:02:33.000000 easyfermi-2.0.9/LICENSE.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)      996 2024-02-28 11:00:43.656098 easyfermi-2.0.9/PKG-INFO
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)      453 2024-02-02 10:02:39.000000 easyfermi-2.0.9/README.md
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2024-02-28 11:00:43.644098 easyfermi-2.0.9/easyfermi/
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)       63 2024-02-06 14:47:20.000000 easyfermi-2.0.9/easyfermi/__init__.py
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)   223483 2024-02-28 10:41:10.000000 easyfermi-2.0.9/easyfermi/easyfermi.py
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2024-02-28 11:00:43.640098 easyfermi-2.0.9/easyfermi/resources/
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2024-02-28 11:00:43.652098 easyfermi-2.0.9/easyfermi/resources/ebl/
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)   431576 2023-10-27 15:39:40.000000 easyfermi-2.0.9/easyfermi/resources/ebl/ebl_dominguez11.fits.gz
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)   274043 2023-10-27 15:40:33.000000 easyfermi-2.0.9/easyfermi/resources/ebl/ebl_franceschini.fits.gz
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)  2467682 2024-01-25 16:25:28.000000 easyfermi-2.0.9/easyfermi/resources/ebl/ebl_franceschini_2017.fits.gz
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)   643130 2024-01-25 16:25:20.000000 easyfermi-2.0.9/easyfermi/resources/ebl/ebl_saldana-lopez_2021.fits.gz
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)   120837 2024-01-31 21:15:35.000000 easyfermi-2.0.9/easyfermi/resources/ebl/frd_abs.fits.gz
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2024-02-28 11:00:43.652098 easyfermi-2.0.9/easyfermi/resources/images/
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)    31775 2024-02-02 10:07:14.000000 easyfermi-2.0.9/easyfermi/resources/images/download_logo.png
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)    40332 2022-01-15 16:04:30.000000 easyfermi-2.0.9/easyfermi/resources/images/easyFermiIcon.png
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)   150411 2024-02-06 14:48:42.000000 easyfermi-2.0.9/easyfermi/resources/images/easyFermiWindow.png
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)   121691 2021-11-23 14:18:26.000000 easyfermi-2.0.9/easyfermi/resources/images/fermi.png
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2024-02-28 11:00:43.644098 easyfermi-2.0.9/easyfermi.egg-info/
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)      996 2024-02-28 11:00:43.000000 easyfermi-2.0.9/easyfermi.egg-info/PKG-INFO
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)      627 2024-02-28 11:00:43.000000 easyfermi-2.0.9/easyfermi.egg-info/SOURCES.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)        1 2024-02-28 11:00:43.000000 easyfermi-2.0.9/easyfermi.egg-info/dependency_links.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)       10 2024-02-28 11:00:43.000000 easyfermi-2.0.9/easyfermi.egg-info/top_level.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)       38 2024-02-28 11:00:43.656098 easyfermi-2.0.9/setup.cfg
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1228 2024-02-28 11:00:07.000000 easyfermi-2.0.9/setup.py
```

### Comparing `easyfermi-2.0.8/LICENSE.txt` & `easyfermi-2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyfermi-2.0.8/PKG-INFO` & `easyfermi-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfermi
-Version: 2.0.8
+Version: 2.0.9
 Summary: The easiest way to analyze Fermi-LAT data
 Author: Raniere de Menezes
 Author-email: <easyfermi@gmail.com>
 Keywords: python,fermi,GUI,graphical interface,easyfermi,gamma-rays
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyfermi-2.0.8/easyfermi/easyfermi.py` & `easyfermi-2.0.9/easyfermi/easyfermi.py`

 * *Files 0% similar despite different names*

```diff
@@ -910,15 +910,15 @@
         self.toolButton_External_ltcube.clicked.connect(self.browsefiles)
         self.toolButton_VHE.setCheckable(True)
         self.toolButton_VHE.clicked.connect(self.browsefiles)
         self.toolButton_VHE.setToolTip('Here you can select a fits table with the VHE data. This is not mandatory for the MCMC.\nCheck the GitHub of easyfermi for details on the format of this table.')
         self.toolButton_External_ltcube.setToolTip('Here you can select a txt file listing one or more ltcube files.\neasyfermi automatically saves this file as "ltcube_list.txt" once you run an analysis.')
 
         self.white_box_list_of_sources_to_delete.setToolTip("e.g.: 4FGL J1222.5+0414,4FGL J1219.7+0444,4FGL ...")
-        self.white_box_TS_cut_in_the_fit.setToolTip("If the fit does not converge:\n1) All sources with TS < TS_cut will be deleted from the RoI model or...\n2) If the TS_target < TS_cut, all sources with TS < TS_target will be deleted from the RoI model.\nDefault value is TS_cut = 16.")
+        self.white_box_TS_cut_in_the_fit.setToolTip("If the fit does not converge:\n1) All sources with TS < TS_cut will be deleted from the RoI model or...\n2) If the TS_target < TS_cut, all sources with TS < TS_target will be deleted from the RoI model.\n3) The fit is performed again.\nDefault value is TS_cut = 16.")
         self.label_TS_fit_cut.setToolTip("If the fit does not converge:\n1) All sources with TS < TS_cut will be deleted from the RoI model or...\n2) If the TS_target < TS_cut, all sources with TS < TS_target will be deleted from the RoI model.\nDefault value is TS_cut = 16.")
         
         ###### Activating/deactivating options
         self.checkBox_LC.clicked.connect(self.activate)
         self.checkBox_adaptive_binning.clicked.connect(self.activate)
         self.checkBox_SED.clicked.connect(self.activate)
         self.checkBox_extension.clicked.connect(self.activate)
@@ -1599,14 +1599,15 @@
         """
 
         if self.radioButton_Standard.isChecked():
             self.reportProgress(n=None)           
             check = 0
             Coords = self.white_box_RAandDec.text().split(',')
             Energ = self.white_box_energy.text().split(',')
+            Energ = np.asarray(Energ).astype(float)
             date = self.dateTimeEdit.text()
             date2 = self.dateTimeEdit_2.text()
             times = [str(date[6:10])+'-'+str(date[3:5])+'-'+str(date[:2])+'T'+str(date[11:19]),    str(date2[6:10])+'-'+str(date2[3:5])+'-'+str(date2[:2])+'T'+str(date2[11:19])              ]
             t = Time(times)
             t0 = t.mjd[0]
             t1 = t.mjd[1]
             
@@ -1627,20 +1628,36 @@
                     else:
                         ltcube_list = np.loadtxt(self.white_box_External_ltcube.text(),ndmin=2,dtype=str)
                         ltcube_list = ltcube_list[:,0]
                         for ltcube in ltcube_list:
                             if not os.path.exists(ltcube):
                                 check = check + 1
                                 self.large_white_box_Log.setPlainText(self.large_white_box_Log.toPlainText()+f"- The path {ltcube} does not exist. Maybe you renamed the directory containing the ltcube_list.txt file. Give it a check.\n")
-
                 
                 if (len(self.white_box_spacecraft_file.text().split(' ')) > 1) or (len(self.white_box_Diffuse_dir.text().split(' ')) > 1) or (len(self.white_box_photon_dir.text().split(' ')) > 1):
                     check = check + 1
                     self.large_white_box_Log.setPlainText(self.large_white_box_Log.toPlainText()+"- The data paths cannot contain blank spaces. Please fix this before proceeding.\n")
             
+                list_of_photon_files = glob.glob(self.white_box_photon_dir.text()+"/*.fits")
+                if len(list_of_photon_files) == 0:
+                    check = check + 1
+                    print("No photon files found in the given directory.")
+                    self.large_white_box_Log.setPlainText(self.large_white_box_Log.toPlainText()+"- No photon files found in the given directory.\n")
+                
+                max_photon_energy= 0
+                for photon_file in list_of_photon_files:
+                    max_energy_in_the_file = pyfits.open(photon_file)[1].data["ENERGY"].max()
+                    if max_energy_in_the_file > max_photon_energy:
+                        max_photon_energy = max_energy_in_the_file
+                
+                if max_photon_energy > 0 and Energ[1] > 1.1*max_photon_energy:
+                    check = check + 1
+                    self.max_energy_wanning = f"The maximum energy is set to {Energ[1]} MeV, however, the highest energy photon in the dataset has only {max_photon_energy} MeV.\n\nPlease set Emax <= {max_photon_energy} MeV before proceeding."
+
+
             try:
                 if len(Coords) == 1:
                     self.recover_coords_from_name = Simbad.query_object(Coords[0])
                     try:
                         if len(self.recover_coords_from_name) == 1:
                             pass
                     except:
@@ -1653,41 +1670,24 @@
                     if (Coords[0] <= 360) & (Coords[0] >= 0) & (Coords[1] >= -90) & (Coords[1] <= 90):
                         pass
                     else:
                         print('Problems with the coordinates.')
                         check = check + 1
                         self.large_white_box_Log.setPlainText(self.large_white_box_Log.toPlainText()+"- Invalid coordinates. Try 0 <= RA <= 360 and -90 <= Dec <= 90.\n")
 
-                Energ = np.asarray(Energ).astype(float)
                 if (Energ[0] < Energ[1]) & (Energ[0] > 20) & (Energ[1] <= 10000000):
                     pass
                 else:
                     print("Problems in the energy range.")
                     check = check + 1
                     self.large_white_box_Log.setPlainText(self.large_white_box_Log.toPlainText()+"- Invalid energy range. Try values from 20 to 10000000 MeV.\n")
                 if t1 <= t0:
                     check = check + 1
                     self.large_white_box_Log.setPlainText(self.large_white_box_Log.toPlainText()+"- Stop time must be set to a date after start time.\n")
             
-                list_of_photon_files = glob.glob(self.white_box_photon_dir.text()+"/*.fits")
-                if len(list_of_photon_files) == 0:
-                    check = check + 1
-                    print("No photon files found in the given directory.")
-                    self.large_white_box_Log.setPlainText(self.large_white_box_Log.toPlainText()+"- No photon files found in the given directory.\n")
-                
-                max_photon_energy= 0
-                for photon_file in list_of_photon_files:
-                    max_energy_in_the_file = pyfits.open(photon_file)[1].data["ENERGY"].max()
-                    if max_energy_in_the_file > max_photon_energy:
-                        max_photon_energy = max_energy_in_the_file
-                
-                if max_photon_energy > 0 and Energ[1] > 1.1*max_photon_energy:
-                    check = check + 1
-                    self.max_energy_wanning = f"The maximum energy is set to {Energ[1]} MeV, however, the highest energy photon in the dataset has only {max_photon_energy} MeV.\n\nPlease set Emax <= {max_photon_energy} MeV before proceeding."
-
                 if check == 0:
                     answer = True
                 else:
                     answer = False
                 
             except:
                 answer = False
```

### Comparing `easyfermi-2.0.8/easyfermi/resources/ebl/ebl_dominguez11.fits.gz` & `easyfermi-2.0.9/easyfermi/resources/ebl/ebl_dominguez11.fits.gz`

 * *Files identical despite different names*

### Comparing `easyfermi-2.0.8/easyfermi/resources/ebl/ebl_franceschini.fits.gz` & `easyfermi-2.0.9/easyfermi/resources/ebl/ebl_franceschini.fits.gz`

 * *Files identical despite different names*

### Comparing `easyfermi-2.0.8/easyfermi/resources/ebl/ebl_franceschini_2017.fits.gz` & `easyfermi-2.0.9/easyfermi/resources/ebl/ebl_franceschini_2017.fits.gz`

 * *Files identical despite different names*

### Comparing `easyfermi-2.0.8/easyfermi/resources/ebl/ebl_saldana-lopez_2021.fits.gz` & `easyfermi-2.0.9/easyfermi/resources/ebl/ebl_saldana-lopez_2021.fits.gz`

 * *Files identical despite different names*

### Comparing `easyfermi-2.0.8/easyfermi/resources/ebl/frd_abs.fits.gz` & `easyfermi-2.0.9/easyfermi/resources/ebl/frd_abs.fits.gz`

 * *Files identical despite different names*

### Comparing `easyfermi-2.0.8/easyfermi/resources/images/download_logo.png` & `easyfermi-2.0.9/easyfermi/resources/images/download_logo.png`

 * *Files identical despite different names*

### Comparing `easyfermi-2.0.8/easyfermi/resources/images/easyFermiIcon.png` & `easyfermi-2.0.9/easyfermi/resources/images/easyFermiIcon.png`

 * *Files identical despite different names*

### Comparing `easyfermi-2.0.8/easyfermi/resources/images/easyFermiWindow.png` & `easyfermi-2.0.9/easyfermi/resources/images/easyFermiWindow.png`

 * *Files identical despite different names*

### Comparing `easyfermi-2.0.8/easyfermi/resources/images/fermi.png` & `easyfermi-2.0.9/easyfermi/resources/images/fermi.png`

 * *Files identical despite different names*

### Comparing `easyfermi-2.0.8/easyfermi.egg-info/PKG-INFO` & `easyfermi-2.0.9/easyfermi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfermi
-Version: 2.0.8
+Version: 2.0.9
 Summary: The easiest way to analyze Fermi-LAT data
 Author: Raniere de Menezes
 Author-email: <easyfermi@gmail.com>
 Keywords: python,fermi,GUI,graphical interface,easyfermi,gamma-rays
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyfermi-2.0.8/easyfermi.egg-info/SOURCES.txt` & `easyfermi-2.0.9/easyfermi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easyfermi-2.0.8/setup.py` & `easyfermi-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '2.0.8'
+VERSION = '2.0.9'
 DESCRIPTION = 'The easiest way to analyze Fermi-LAT data'
 LONG_DESCRIPTION = 'A GUI that allows to measure the flux, create light curves, SEDs, and TS maps for Fermi-LAT data.'
 
 # Setting up
 setup(
     name="easyfermi",
     version=VERSION,
```

