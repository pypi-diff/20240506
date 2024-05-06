# Comparing `tmp/metadynminer-0.8.0.tar.gz` & `tmp/metadynminer-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metadynminer-0.8.0.tar", last modified: Mon Apr 22 06:51:56 2024, max compression
+gzip compressed data, was "metadynminer-0.8.1.tar", last modified: Mon May  6 15:01:10 2024, max compression
```

## Comparing `metadynminer-0.8.0.tar` & `metadynminer-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 beranekj  (1000) beranekj  (1000)        0 2024-04-22 06:51:56.593922 metadynminer-0.8.0/
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)    35149 2023-03-22 09:01:26.000000 metadynminer-0.8.0/LICENSE
--rw-r--r--   0 beranekj  (1000) beranekj  (1000)     4010 2024-04-22 06:51:56.593922 metadynminer-0.8.0/PKG-INFO
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)     3151 2024-04-12 09:25:13.000000 metadynminer-0.8.0/README.md
-drwxrwxr-x   0 beranekj  (1000) beranekj  (1000)        0 2024-04-22 06:51:56.593922 metadynminer-0.8.0/metadynminer/
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)   172308 2024-04-16 12:09:26.000000 metadynminer-0.8.0/metadynminer/__init__.py
-drwxrwxr-x   0 beranekj  (1000) beranekj  (1000)        0 2024-04-22 06:51:56.593922 metadynminer-0.8.0/metadynminer.egg-info/
--rw-r--r--   0 beranekj  (1000) beranekj  (1000)     4010 2024-04-22 06:51:56.000000 metadynminer-0.8.0/metadynminer.egg-info/PKG-INFO
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)      331 2024-04-22 06:51:56.000000 metadynminer-0.8.0/metadynminer.egg-info/SOURCES.txt
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)        1 2024-04-22 06:51:56.000000 metadynminer-0.8.0/metadynminer.egg-info/dependency_links.txt
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)       78 2024-04-22 06:51:56.000000 metadynminer-0.8.0/metadynminer.egg-info/requires.txt
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)       13 2024-04-22 06:51:56.000000 metadynminer-0.8.0/metadynminer.egg-info/top_level.txt
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)       38 2024-04-22 06:51:56.593922 metadynminer-0.8.0/setup.cfg
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)     1166 2024-04-12 09:47:19.000000 metadynminer-0.8.0/setup.py
-drwxrwxr-x   0 beranekj  (1000) beranekj  (1000)        0 2024-04-22 06:51:56.593922 metadynminer-0.8.0/tests/
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)     3496 2024-04-12 11:06:06.000000 metadynminer-0.8.0/tests/test_fast.py
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)     1493 2024-04-12 12:25:34.000000 metadynminer-0.8.0/tests/test_fep.py
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)     9795 2024-04-12 12:35:38.000000 metadynminer-0.8.0/tests/test_minima.py
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)     3885 2024-04-12 12:39:02.000000 metadynminer-0.8.0/tests/test_orig.py
--rw-rw-r--   0 beranekj  (1000) beranekj  (1000)      901 2023-09-05 14:01:59.000000 metadynminer-0.8.0/tests/test_readhills.py
+drwxrwxr-x   0 beranekj  (1000) beranekj  (1000)        0 2024-05-06 15:01:10.984192 metadynminer-0.8.1/
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)    35149 2023-03-22 09:01:26.000000 metadynminer-0.8.1/LICENSE
+-rw-r--r--   0 beranekj  (1000) beranekj  (1000)     4010 2024-05-06 15:01:10.984192 metadynminer-0.8.1/PKG-INFO
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)     3151 2024-04-12 09:25:13.000000 metadynminer-0.8.1/README.md
+drwxrwxr-x   0 beranekj  (1000) beranekj  (1000)        0 2024-05-06 15:01:10.984192 metadynminer-0.8.1/metadynminer/
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)   174791 2024-05-02 13:22:30.000000 metadynminer-0.8.1/metadynminer/__init__.py
+drwxrwxr-x   0 beranekj  (1000) beranekj  (1000)        0 2024-05-06 15:01:10.984192 metadynminer-0.8.1/metadynminer.egg-info/
+-rw-r--r--   0 beranekj  (1000) beranekj  (1000)     4010 2024-05-06 15:01:10.000000 metadynminer-0.8.1/metadynminer.egg-info/PKG-INFO
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)      331 2024-05-06 15:01:10.000000 metadynminer-0.8.1/metadynminer.egg-info/SOURCES.txt
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)        1 2024-05-06 15:01:10.000000 metadynminer-0.8.1/metadynminer.egg-info/dependency_links.txt
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)       78 2024-05-06 15:01:10.000000 metadynminer-0.8.1/metadynminer.egg-info/requires.txt
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)       13 2024-05-06 15:01:10.000000 metadynminer-0.8.1/metadynminer.egg-info/top_level.txt
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)       38 2024-05-06 15:01:10.984192 metadynminer-0.8.1/setup.cfg
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)     1166 2024-05-06 15:00:57.000000 metadynminer-0.8.1/setup.py
+drwxrwxr-x   0 beranekj  (1000) beranekj  (1000)        0 2024-05-06 15:01:10.984192 metadynminer-0.8.1/tests/
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)     3496 2024-04-12 11:06:06.000000 metadynminer-0.8.1/tests/test_fast.py
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)     1493 2024-04-12 12:25:34.000000 metadynminer-0.8.1/tests/test_fep.py
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)     9795 2024-04-12 12:35:38.000000 metadynminer-0.8.1/tests/test_minima.py
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)     3885 2024-04-12 12:39:02.000000 metadynminer-0.8.1/tests/test_orig.py
+-rw-rw-r--   0 beranekj  (1000) beranekj  (1000)      901 2023-09-05 14:01:59.000000 metadynminer-0.8.1/tests/test_readhills.py
```

### Comparing `metadynminer-0.8.0/LICENSE` & `metadynminer-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metadynminer-0.8.0/PKG-INFO` & `metadynminer-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metadynminer
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python package for efficient analysis of HILLS files generated by Plumed metadynamics simulations. 
 Home-page: https://github.com/Jan8be/metadynminer.py
 Author: Jan Beránek
 Author-email: Jan1.Beranek@vscht.cz
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `metadynminer-0.8.0/README.md` & `metadynminer-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `metadynminer-0.8.0/metadynminer/__init__.py` & `metadynminer-0.8.1/metadynminer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ```python
 fep = metadynminer.FEProfile(minima, hillsfile)
 fep.plot()
 ```
 """
 
 name = "metadynminer"
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 __author__ = 'Jan Beránek'
 
 __pdoc__ = {}
 
 #print(f"""Welcome to Metadynminer version {__version__}. """)
 
 try:
@@ -148,15 +148,15 @@
 
 class Hills:
     """
     Object of Hills class are created for loading HILLS files, and obtaining the necessary information from them. 
 
     Hills files are loaded with command:
     ```python
-    hillsfile = metadynminer.Hills(name="HILLS", periodic=[False,False])
+    hillsfile = metadynminer.Hills(name="HILLS")
     ```
     
     optional parameters:
     
     * name (default="HILLS") = string with name of HILLS file
     
     * ignoretime (default=True) = boolean, if set to False, it will save the time in the HILLS file;
@@ -165,14 +165,34 @@
                                         
     * timestep = numeric value of the time difference between hills, in picoseconds
     
     * periodic (default=[False, False]) = list of boolean values telling which CV is periodic.
     
     * cv1per, cv2per, cv3per (defaults = [-numpy.pi, numpy.pi]) = List of two numeric values defining the periodicity of given CV. 
                                         Has to be provided for each periodic CV.
+
+    Hills attributes: 
+
+    * Hills.hills = array of values from the HILLS file
+    
+    * Hills.cvs = number of CVs
+
+    * Hills.cv1_name = name of CV 1
+
+    * Hills.cv1per = list of two boundaries of the perodicity interval for CV 1
+
+    * Hills.dt = time step between hills in ps
+
+    * Hills.sigma1 = widths of hills along the CV 1 axis
+
+    * Hills.cv1 = list of CV 1 values during simulation
+
+    * Hills.biasf = biasfactors
+
+    * and analogous attributes for other CVs
     """
     
     def __init__(self, name="HILLS", encoding="utf8", ignoretime=True, periodic=None, 
                  cv1per=[-np.pi, np.pi],cv2per=[-np.pi, np.pi],cv3per=[-np.pi, np.pi], timestep=None):
         self.read(name, encoding, ignoretime, periodic, 
                  cv1per=cv1per,cv2per=cv2per,cv3per=cv3per, timestep=timestep)
         self.hillsfilename = name
@@ -427,16 +447,16 @@
         * time_min, time_max = The time range for plot, closed interval, in the time unit specified by "tu"
 
         * title = optional, string that defines the title of the graph
         """
         tu = TU(tu)
         
         if time_min == time_max == 0:
-                print("Error: Values of start and end time are zero.")
-                return None
+            print("Error: Values of start and end time are zero.")
+            return None
         if time_min != None:
             #time_min = tu.inps(time_min)
             if tu.inps(time_min) < 0:
                 print("Warning: Start time is lower than zero, it will be set to zero instead. ")
                 time_min = 0
             if tu.inps(time_min) < int(self.hills[0,0]):
                 print(f"Warning: Start time {tu.inps(time_min)} ps is lower than the first time from HILLS file {int(self.hills[0,0])} ps, which will be used instead. ")
@@ -554,16 +574,16 @@
         if CV!=1 and CV!=2 and CV!=3:
             print(f"Error: supplied value of CV {CV} is not correct value")
             return None
             
         tu = TU(tu)
         
         if time_min == time_max == 0:
-                print("Error: Values of start and end time are zero.")
-                return None
+            print("Error: Values of start and end time are zero.")
+            return None
         if time_min != None:
             #time_min = tu.inps(time_min)
             if tu.inps(time_min) < 0:
                 print("Warning: Start time is lower than zero, it will be set to zero instead. ")
                 time_min = 0
             if tu.inps(time_min) < int(self.hills[0,0]):
                 print(f"Warning: Start time {tu.inps(time_min)} ps is lower than the first time from HILLS file {int(self.hills[0,0])} ps, which will be used instead. ")
@@ -671,23 +691,47 @@
                                         
     * cv1range, cv2range, cv3range = lists of two numbers, defining lower and upper bound of the respective CV (in the units of the CVs)
     
     * time_min, time_max = Limit points for closed interval of times from the HILLS file from which the FES will be constructed. Useful for making animations of flooding of the FES during simulation. The values here should have the same units as those in the HILLS file, especially if ignoretime = False. 
 
     * tu (default = "ps") = string, time unit for time_min and time_max parameters, if those are used. Available options: "s", "ms", "us", "ns", "ps", "fs"
 
+    * print_output (default = True), tells whether the function should print messages like progress of calculation
+
+    * subtract_min (deault = True), whether the global minimum value should be subtracted from the whole FES, so that global minimum has zero free energy and other states have higher values
+
+    Fes atributes: 
+
+    * Fes.fes = free energy surface
+    
+    * Fes.res = resolution of the FES
+
+    * Fes.original = whether FES should be calculated by plumed's original precise algorithm
+
+    * Fes.cvs = number of CVs
+
+    * Fes.hills = array with values from the HILLS file
+
+    * Fes.periodic = list of boolean values setting which CVs are periodic
+
+    * Fes.cv1min, Fes.cv1max = minimum and maximum values on the FES, respectively
+
+    * Fes.cv1_fes_range, Fes.cv2_fes_range, Fes.cv3_fes_range = FES range = maximum - minimum values on FES for given CV
+
+    * Fes.cv1_name, Fes.cv2_name, Fes.cv3_name = CV names
+    
     """
     
     __pdoc__["Fes.makefes"] = False
     __pdoc__["Fes.makefes2"] = False
     __pdoc__["Fes.set_fes"] = False
     
     def __init__(self, hills=None, resolution=256, original=False, \
                  calculate_new_fes=True, cv1range=None, cv2range=None, cv3range=None, \
-                 time_min=None, time_max=None, tu="ps"):
+                 time_min=None, time_max=None, tu="ps", print_output=True, subtract_min = True):
         self.res = resolution
         self.original = original
         self.cv1range = cv1range
         self.cv2range = cv2range
         self.cv3range = cv3range
         if hills != None:
             self.hills = hills
@@ -708,14 +752,16 @@
             if self.cvs >= 1:
                 self.cv1 = hills.get_cv1()
                 self.s1 = hills.get_sigma1()
 
                 self.cv1_name = hills.get_cv1_name()
                 self.cv1per = hills.get_cv1per()
 
+                self.fes = np.zeros((resolution))
+
                 if self.periodic[0]:
                     cv1min = self.cv1per[0]
                     cv1max = self.cv1per[1]
                     if cv1range != None:
                         print("Warning: CV1 is specified as periodic, to change it's range you must specify the periodicity to cv1per parameter when loading the HILLS file. The cv1range parameter is ignored. ")
                 else:
                     if cv1range == None:
@@ -745,14 +791,16 @@
             if self.cvs >= 2:
                 self.cv2 = hills.get_cv2()
                 self.s2 = hills.get_sigma2()
                 
                 self.cv2_name = hills.get_cv2_name()
                 self.cv2per = hills.get_cv2per()
 
+                self.fes = np.zeros((resolution, resolution))
+
                 if self.periodic[1]:
                     cv2min = self.cv2per[0]
                     cv2max = self.cv2per[1]
                     if cv2range != None:
                         print("Warning: CV2 is specified as periodic, to change it's range you must specify the periodicity to cv2per parameter when loading the HILLS file. The cv2range parameter is ignored. ")
                 else:
                     if cv2range == None:
@@ -782,14 +830,16 @@
 
             if self.cvs == 3:
                 self.cv3 = hills.get_cv3()
                 self.s3 = hills.get_sigma3()
 
                 self.cv3_name = hills.get_cv3_name()
                 self.cv3per = hills.get_cv3per()
+
+                self.fes = np.zeros((resolution, resolution, resolution))
                 
                 if self.periodic[2]:
                     cv3min = self.cv3per[0]
                     cv3max = self.cv3per[1]
                     if cv3range != None:
                         print("Warning: CV3 is specified as periodic, to change it's range you must specify the periodicity to cv3per parameter when loading the HILLS file. The cv3range is ignored. ")
                 else:
@@ -815,28 +865,28 @@
                         For this file, you need the exact algorithm, to do that, 
                         specify the argument 'original=True'.""")
                         return None
                         
             tu = TU(tu)
         
             if time_min == time_max == 0:
-                    print("Error: Values of start and end time are zero.")
-                    return None
+                print("Error: Values of start and end time are zero.")
+                return None
             if time_min != None:
-                time_min = tu.inps(time_min)
+                #time_min = tu.inps(time_min)
                 if time_min < 0:
                     print("Warning: Start time is lower than zero, it will be set to zero instead. ")
                     time_min = 0
                 if time_min < int(hills.hills[0,0]):
                     print(f"Warning: Start time {tu.inps(time_min)} is lower than the first time from HILLS file {int(hills.hills[0,0])}, which will be used instead. ")
                     time_min = int(hills.hills[0,0])
             else:
                 time_min = int(hills.hills[0,0])
             if time_max != None:
-                time_max = tu.inps(time_max)
+                #time_max = int(tu.inps(time_max))
                 if time_max < time_min:
                     print("Warning: End time is lower than start time. Values are flipped. ")
                     time_value = time_max
                     time_max = time_min
                     time_min = time_value
                 if time_max > int(hills.hills[-1,0]):
                     print(f"Warning: End time {tu.inps(time_max)} is higher than number of lines in HILLS file {int(hills.hills[-1,0])}, which will be used instead. ")
@@ -847,19 +897,21 @@
             if not self.ignoretime:
                 time_max = int(round(((time_max - hills.hills[0,0])/self.dt),0)) + 1
                 time_min = int(round(((time_min - hills.hills[0,0])/self.dt),0)) + 1
                 #print(f"Berofe fes: min {time_min}, max {time_max}")
 
             if calculate_new_fes:
                 if original:
-                    self.makefes2(resolution, time_min, time_max)
+                    self.makefes2(resolution, int(tu.inps(time_min)), int(tu.inps(time_max)), 
+                                  print_output=print_output, subtract_min = subtract_min)
                 else:
-                    self.makefes(resolution, time_min, time_max)
+                    self.makefes(resolution, int(tu.inps(time_min)), int(tu.inps(time_max)), 
+                                 print_output=print_output, subtract_min = subtract_min)
         
-    def makefes(self, resolution, time_min, time_max, print_output=True):
+    def makefes(self, resolution, time_min, time_max, print_output=True, subtract_min = True):
         """
         Function used internally for summing hills in Hills object with the fast Bias Sum Algorithm. 
         """
         #self.res = resolution
         #if self.res % 2 == 0:
         #    self.res += 1
         #print(f"min: {time_min}, max: {time_max}")
@@ -913,15 +965,16 @@
                         fes_crop_cv1_p = [0,gauss_center_to_end+cv1bin[line]-self.res-1]
                         gauss_crop_cv1_p = [gauss_res-(gauss_center_to_end+cv1bin[line]-self.res),gauss_res-1]
                         fes[fes_crop_cv1_p[0]:fes_crop_cv1_p[1]+1]\
                                     += gauss[gauss_crop_cv1_p[0]:gauss_crop_cv1_p[1]+1]\
                                     * self.heights[line]
             if print_output:
                 print("\n")
-            fes = fes-np.min(fes)
+            if subtract_min:
+                fes = fes-np.min(fes)
             self.fes = np.array(fes)
             
         elif self.cvs == 2:
             cv1bin = np.ceil((self.cv1-self.cv1min)*self.res/(self.cv1_fes_range))
             cv2bin = np.ceil((self.cv2-self.cv2min)*self.res/(self.cv2_fes_range))
                         
             cv1bin = cv1bin.astype(int)
@@ -1003,15 +1056,16 @@
                     if ((cv1bin[line] < gauss_center_to_end) or (cv1bin[line] > (self.res-gauss_center_to_end))) \
                             and ((cv2bin[line] < gauss_center_to_end) or (cv2bin[line] > (self.res-gauss_center_to_end))):
                         fes[fes_crop_cv1_p[0]:fes_crop_cv1_p[1]+1,fes_crop_cv2_p[0]:fes_crop_cv2_p[1]+1]\
                                     += gauss[gauss_crop_cv1_p[0]:gauss_crop_cv1_p[1]+1,gauss_crop_cv2_p[0]:gauss_crop_cv2_p[1]+1]\
                                     * self.heights[line]
             if print_output:
                 print("\n")
-            fes = fes-np.min(fes)
+            if subtract_min:
+                fes = fes-np.min(fes)
             self.fes = np.array(fes)
         elif self.cvs == 3:
             cv1bin = np.ceil((self.cv1-self.cv1min)*self.res/(self.cv1_fes_range))
             cv2bin = np.ceil((self.cv2-self.cv2min)*self.res/(self.cv2_fes_range))
             cv3bin = np.ceil((self.cv3-self.cv3min)*self.res/(self.cv3_fes_range))
                         
             cv1bin = cv1bin.astype(int)
@@ -1183,24 +1237,24 @@
                                     += gauss[gauss_crop_cv1_p[0]:gauss_crop_cv1_p[1]+1,\
                                              gauss_crop_cv2_p[0]:gauss_crop_cv2_p[1]+1,\
                                              gauss_crop_cv3_p[0]:gauss_crop_cv3_p[1]+1]\
                                     * self.heights[line]
             
             if print_output:
                 print("\n")
-            fes = fes-np.min(fes)
+            if subtract_min:
+                fes = fes-np.min(fes)
             self.fes = np.array(fes)
         else:
             print("Fes object doesn't have supported number of CVs.")
     
-    def makefes2(self, resolution, time_min, time_max, print_output=True):
+    def makefes2(self, resolution, time_min, time_max, print_output=True, subtract_min = True):
         """
         Function internally used to sum Hills in the same way as Plumed sum_hills. 
         """
-        
         self.res = resolution
         
         if self.cvs == 1:
             fes = np.zeros((self.res))
             progress = 1
             max_progress = self.res ** self.cvs
             
@@ -1216,15 +1270,16 @@
                 
                 dp2 = dist_cv1**2/(2*self.s1[time_min-1:time_max]**2)
                 tmp = np.zeros(time_max-time_min+1)
                 heights = self.heights[time_min-1:time_max]
                 tmp[dp2<6.25] = heights[dp2<6.25] * (np.exp(-dp2[dp2<6.25]) * 1.00193418799744762399 - 0.00193418799744762399)
                 fes[x] = -tmp.sum()
                     
-            fes = fes - np.min(fes)
+            if subtract_min:
+                fes = fes - np.min(fes)
             self.fes = np.array(fes)
             if print_output:
                 print("\n")
             
         elif self.cvs == 2:
             fes = np.zeros((self.res, self.res))
             progress = 0
@@ -1248,15 +1303,16 @@
                         
                     dp2 = dist_cv1**2/(2*self.s1[time_min-1:time_max]**2) + dist_cv2**2/(2*self.s2[time_min-1:time_max]**2)
                     tmp = np.zeros(time_max-time_min+1)
                     heights = self.heights[time_min-1:time_max]
                     tmp[dp2<6.25] = heights[dp2<6.25] * (np.exp(-dp2[dp2<6.25]) * 1.00193418799744762399 - 0.00193418799744762399)
                     fes[x,y] = -tmp.sum()
                     
-            fes = fes - np.min(fes)
+            if subtract_min:
+                fes = fes - np.min(fes)
             self.fes = np.array(fes)
             if print_output:
                 print("\n")
             
         elif self.cvs == 3:
             fes = np.zeros((self.res, self.res, self.res))
             progress = 0
@@ -1288,22 +1344,23 @@
                               dist_cv2**2/(2*self.s2[time_min-1:time_max]**2) + \
                               dist_cv3**2/(2*self.s3[time_min-1:time_max]**2)
                         tmp = np.zeros(time_max-time_min+1)
                         heights = self.heights[time_min-1:time_max]
                         tmp[dp2<6.25] = heights[dp2<6.25] * (np.exp(-dp2[dp2<6.25]) * 1.00193418799744762399 - 0.00193418799744762399)
                         fes[x,y,z] = -tmp.sum()
                         
-            fes = fes - np.min(fes)
+            if subtract_min:
+                fes = fes - np.min(fes)
             self.fes = np.array(fes)
             if print_output:
                 print("\n")
         else:
             print(f"Error: unsupported number of CVs: {self.cvs}.")
     
-    def plot(self, png_name=None, contours=True, contours_spacing=0.0, aspect = 1.0, cmap = "jet", 
+    def plot(self, png_name=None, contours=True, contours_spacing=0.0, aspect = 1.0, cmap = "RdYlBu_r", 
              energy_unit="kJ/mol", xlabel=None, ylabel=None, zlabel=None, label_size=12, clabel_size = 12,
              image_size=None, image_size_unit="in", dpi=100, vmin = 0, vmax = None, 
              opacity=0.2, levels=None, title = None, off_screen = False, 
              xlim=[None, None], ylim=[None, None]):
         """
         Function used to visualize FES, based on Matplotlib for 1D and 2D FES or PyVista for 3D FES. 
         
@@ -1319,15 +1376,15 @@
         * contours (default=True) = whether contours should be shown on 2D FES
         
         * contours_spacing (default=0.0) = when a positive number is set, it will be used as spacing for contours on 2D FES. 
                 Otherwise, if contours=True, there will be five equally spaced contour levels.
         
         * aspect (default = 1.0) = aspect ratio of the graph. Works with 1D and 2D FES. 
         
-        * cmap (default = "jet") = Matplotlib colormap used to color 2D or 3D FES
+        * cmap (default = "RdYlBu_r") = Matplotlib colormap used to color 2D or 3D FES
         
         * energy_unit (default="kJ/mol") = String, used in description of colorbar
 
         * xlim, ylim (default = [None, None] for both) = list of two values specifying the range of x and y axes respectively. 
         None means that Matplotlib will choose appropriate range, so this keyword is useful when you need to overwrite it. 
         Does not work for 3D FES at the moment. 
         
@@ -1501,15 +1558,15 @@
             if png_name != None:
                 p.save_graphic(png_name)
             
     
     def set_fes(self, fes):
         self.fes = fes
         
-    def surface_plot(self, cmap = "jet", 
+    def surface_plot(self, cmap = "RdYlBu_r", 
                      energy_unit="kJ/mol", xlabel=None, ylabel=None, zlabel=None, dpi=100, label_size=12, image_size=None, image_size_unit="in", rstride=1, cstride=1, vmin = 0, vmax = None, title=None):
         """
         Function for visualization of 2D FES as 3D surface plot. For now, it is based on Matplotlib, but there are issues with interactivity. 
         
         It can be interacted with in jupyter notebook or jupyter lab in %matplotlib widget mode. Otherwise it is just static image of the 3D surface plot. 
         
         ```python
@@ -1773,15 +1830,15 @@
                     new_fes.cv1_fes_range = self.cv1_fes_range
                     new_fes.cv2_fes_range = self.cv2_fes_range
                 return new_fes
             else:
                 print("Error: unknown energy unit")
                 return None
 
-    def flooding_animation(self, gif_name = "flooding.gif", use_vmax_from_end = True, with_minima = True, use_minima_from_end=False, cmap="jet", xlabel=None, ylabel=None, zlabel=None, label_size=12, image_size=None, image_size_unit="in", dpi=100, tu = "ps", time_min=None, time_max=None, step=1000, contours_spacing = 20, levels=None, opacity = 0.2, vmin = 0, vmax = None, energy_unit="kJ/mol", clear_temporary_folder=True, temporary_folder_name="temporary_folder", time_unit="ps", fps=5, enable_loop = True, minima_precise = False, minima_nbins=8, temp=300.0, 
+    def flooding_animation(self, gif_name = "flooding.gif", use_vmax_from_end = True, with_minima = True, use_minima_from_end=False, cmap="RdYlBu_r", xlabel=None, ylabel=None, zlabel=None, label_size=12, image_size=None, image_size_unit="in", dpi=100, tu = "ps", time_min=None, time_max=None, step=1000, contours_spacing = 20, levels=None, opacity = 0.2, vmin = 0, vmax = None, energy_unit="kJ/mol", clear_temporary_folder=True, temporary_folder_name="temporary_folder", time_unit="ps", fps=5, enable_loop = True, minima_precise = False, minima_nbins=8, temp=300.0, 
                            xlim=[None, None], ylim=[None, None]):
         """
         This method is used to make an animation that shows, how the FES was evolving during metadynamics simulation. It creates temporary folder and svaes plots of FES at different times during simulation, then it concatenates them to make a gif animation and removes the temporary files (remove can be switched off, if necessary). 
 
         Use:
         
         ```python
@@ -1831,16 +1888,16 @@
             return None
         else:
            os.makedirs(final_directory)
         flooding_fes = copy.deepcopy(self)
         step_fes = copy.deepcopy(self)
         
         if time_min == time_max == 0:
-                print("Error: Values of start and end time are zero.")
-                return None
+            print("Error: Values of start and end time are zero.")
+            return None
         if time_min != None:
             time_min = tu.inps(time_min)
             if time_min < 0:
                 print("Warning: Start time is lower than zero, it will be set to zero instead. ")
                 time_min = 0
             if time_min < int(self.hills.hills[0,0]):
                 print(f"Warning: Start time {tu.inps(time_min)} ps is lower than the first time from HILLS file {int(self.hills.hills[0,0])}, which will be used instead. ")
@@ -1938,29 +1995,29 @@
             try: 
                 os.rmdir(final_directory)
             except OSError:
                 print(f"Warning: directory{final_directory} is not empty and will not be removed. Metadynminer's temporary files inside were removed. ")
                
 
     
-    def make_gif(self, gif_name=None, cmap = "jet", energy_unit="kJ/mol",
+    def make_gif(self, gif_name=None, cmap = "RdYlBu_r", energy_unit="kJ/mol",
                  xlabel=None, ylabel=None, zlabel=None, label_size=12, image_size=[10,7], 
                   opacity=0.2, levels=None, frames=64):
         """
         Function that generates animation of 3D FES showing different isosurfaces.
         
         ```python
         fes.make_gif(gif_name="FES_animation.gif")
         ```
         
         Parameters:
         
         * gif_name (default="FES.gif") = String. Name of the gif of FES that will be saved in the current working directory.
         
-        * cmap (default = "jet") = Matplotlib colormap used to color the 3D FES
+        * cmap (default = "RdYlBu_r") = Matplotlib colormap used to color the 3D FES
         
         * xlabel, ylabel, zlabel = Strings, if provided, they will be used as labels for the graph
         
         * labelsize (default = 12) = size of text in labels
         
         * image_size (default = [10,7]) = List of the width and height of the picture
         
@@ -1999,15 +2056,15 @@
 
             # Add initial mesh
             plotter.add_mesh(
                 surface,
                 opacity=opacity,
                 clim=grid.get_data_range(),
                 show_scalar_bar=False,
-                cmap="jet"
+                cmap="RdYlBu_r"
             )
             plotter.add_mesh(grid.outline_corners(), color="k")
             text = plotter.add_text(f"{values[0]:.2f}+kJ/mol", position='lower_right', font_size=12)
             if xlabel == None and ylabel == None and zlabel == None:
                 plotter.show_grid(xtitle=f"CV1 - {self.cv1_name}", ytitle=f"CV2 - {self.cv2_name}", ztitle=f"CV3 - {self.cv3_name}")
             else:
                 plotter.show_grid(xtitle=xlabel, ytitle=ylabel, ztitle=zlabel)
@@ -2066,14 +2123,24 @@
     which makes the calculation using precise algorithm slow and impractical. 
 
     * temp (default = 300.0) = thermodynamical temperature of the simulation. Used only if precise=True. 
 
     * energy_unit (default = "kJ/mol") = energy unit of the free energy surface; must be either "kJ/mol" or "kcal/mol". Used only if precise=True. 
 
     * max_iteration (default=10000), the maximum number of iteration the algorithm will last when assigning FES points to their respective local minima
+
+    Attributes: 
+
+    Minima.fes = source free energy surface 
+
+    Minima.minima = pandas dataframe with local minima and their properties
+
+    Minima.m_fes = if you use precise=True, this attribute contains the FES, but each bin contains the index of the minima to which it belongs
+
+    * and other attributes analogous to those of Fes objects
     """
     
     def __init__(self, fes, nbins = 8, precise=True, temp=300.0, energy_unit="kJ/mol", max_iteration=10000, print_output=True):
         self.fes = fes.fes
         self.periodic = fes.periodic
         self.cvs = fes.cvs
         self.res = fes.res
@@ -2810,15 +2877,15 @@
                 self.minima = pd.DataFrame(np.array(self.minima), columns = ["Minimum", "free energy", "CV1bin", "CV2bin", "CV3bin", 
                                                                "CV1 - "+self.cv1_name, "CV2 - "+self.cv2_name,  "CV3 - "+self.cv3_name])
             elif len(self.minima.shape) == 1:
                 self.minima = pd.DataFrame([self.minima], columns = ["Minimum", "free energy", "CV1bin", "CV2bin", "CV3bin", 
                                                                "CV1 - "+self.cv1_name, "CV2 - "+self.cv2_name,  "CV3 - "+self.cv3_name])
         
 
-    def plot(self, png_name=None, contours=True, contours_spacing=0.0, aspect = 1.0, cmap = "jet", 
+    def plot(self, png_name=None, contours=True, contours_spacing=0.0, aspect = 1.0, cmap = "RdYlBu_r", 
                  energy_unit="kJ/mol", xlabel=None, ylabel=None, zlabel=None, label_size=12, clabel_size = 12, image_size=None, image_size_unit="in", dpi=100, color=None, vmin = 0, vmax = None, opacity=0.2, levels=None, show_points=True, point_size=4.0, title = None, off_screen = False, xlim=[None, None], ylim=[None, None]):
         """
         The same function as for visualizing Fes objects, but this time 
         with the positions of local minima shown as letters on the graph.
         
         ```python
         minima.plot(png_name="minima.png")
@@ -2831,15 +2898,15 @@
         * contours (default=True) = whether contours should be shown on 2D FES
         
         * contours_spacing (default=0.0) = when a positive number is set, it will be used as spacing for contours on 2D FES. 
                 Otherwise, if contours=True, there will be five equally spaced contour levels.
         
         * aspect (default = 1.0) = aspect ratio of the graph. Works with 1D and 2D FES. 
         
-        * cmap (default = "jet") = Matplotlib colormap used to color 2D or 3D FES
+        * cmap (default = "RdYlBu_r") = Matplotlib colormap used to color 2D or 3D FES
         
         * energy_unit (default="kJ/mol") = String, used in description of colorbar
 
         * xlim, ylim (default = [None, None] for both) = list of two values specifying the range of x and y axes respectively. 
         None means that Matplotlib will choose appropriate range, so this keyword is useful when you need to overwrite it. 
         
         * xlabel, ylabel, zlabel = Strings, if provided, they will be used as labels for the graphs
@@ -3070,29 +3137,29 @@
             if not off_screen:
                 p.show()
 
             if png_name != None:
                 p.save_graphic(png_name)
             
 
-    def make_gif(self, gif_name=None, cmap = "jet", energy_unit="kJ/mol", 
+    def make_gif(self, gif_name=None, cmap = "RdYlBu_r", energy_unit="kJ/mol", 
                  xlabel=None, ylabel=None, zlabel=None, label_size=12, image_size=[10,7], 
                   opacity=0.2, levels=None, show_points=True, point_size=4.0, frames=64):
         """
         Function that generates animation of 3D FES showing different isosurfaces.
         
         ```python
         fes.make_gif(gif_name="FES.gif")
         ```
         
         Parameters:
         
         * gif_name (default="minima.gif") = String. Name of the gif that will be saved in the working directory.
         
-        * cmap (default = "jet") = Matplotlib colormap used to color the 3D FES
+        * cmap (default = "RdYlBu_r") = Matplotlib colormap used to color the 3D FES
         
         * xlabel, ylabel, zlabel = Strings, if provided, they will be used as labels for the graph
         
         * labelsize (default = 12) = size of text in labels
         
         * image_size (default = [10,7]) = List of the width and height of the picture
         
@@ -3124,15 +3191,15 @@
 
             # Add initial mesh
             plotter.add_mesh(
                 surface,
                 opacity=0.3,
                 clim=grid.get_data_range(),
                 show_scalar_bar=False,
-                cmap="jet"
+                cmap="RdYlBu_r"
             )
             plotter.add_mesh(grid.outline_corners(), color="k")
             
             if xlabel == None and ylabel == None and zlabel == None:
                 plotter.show_grid(xtitle=f"CV1 - {self.cv1_name}", ytitle=f"CV2 - {self.cv2_name}", ztitle=f"CV3 - {self.cv3_name}")
             else:
                 plotter.show_grid(xtitle=xlabel, ytitle=ylabel, ztitle=zlabel)
@@ -3365,15 +3432,15 @@
                 self.feprofile = np.vstack([self.feprofile, profileline])
 
                 lasttime = time
             
         else:
             print("Fes object doesn't have supported number of CVs.")
     
-    def plot(self, png_name=None, image_size=None, image_size_unit="in", dpi=100, tu = "ps", xlabel=None, ylabel=None, label_size=12, cmap="jet", legend=True, xlim=[None, None], ylim=[None, None], title=None):
+    def plot(self, png_name=None, image_size=None, image_size_unit="in", dpi=100, tu = "ps", xlabel=None, ylabel=None, label_size=12, cmap="RdYlBu_r", legend=True, xlim=[None, None], ylim=[None, None], title=None):
         """
         Visualization function for free energy profiles. 
         
         ```python
         fep.plot(png_name="FEProfile.png")
         ```
         
@@ -3393,15 +3460,15 @@
         
         * xlabel (default="time (ps)")
         
         * ylabel (default="free energy difference (kJ/mol)") 
         
         * label_size (default=12) = size of labels
         
-        * cmap (default="jet") = matplotlib colormap used for coloring the line of the minima
+        * cmap (default="RdYlBu_r") = matplotlib colormap used for coloring the line of the minima
 
         * legend (default=True) = whether there should be a matplotlib's legend in the graph
 
         * xlim, ylim (default = [None, None] for both) = list of two values specifying the range of x and y axes respectively. 
         None means that Matplotlib will choose appropriate range, so this keyword is useful when you need to overwrite it. 
 
         * title = optional, string that defines the title of the graph
@@ -3425,15 +3492,15 @@
         elif image_size_unit != "in":
             print(f"Warning: unknown image_size_unit value: {image_size_unit}. Using inches instead. ")
         
         plt.figure(figsize=(image_size[0],image_size[1]), dpi=dpi)
         
         cmap=cm.get_cmap(cmap)
         
-        #colors = cm.jet((self.minima.iloc[:,1].to_numpy()).astype(float)/\
+        #colors = cm.RdYlBu_r((self.minima.iloc[:,1].to_numpy()).astype(float)/\
         #                (np.max(self.minima.iloc[:,1].to_numpy().astype(float))))
         colors = cmap(np.linspace(0,1,self.minima.shape[0]))
         for m in range(self.minima.shape[0]):
             plt.plot(tu.intu(self.feprofile[:,0]), self.feprofile[:,m+1], color=colors[m])
 
         if xlabel == None:
             plt.xlabel(f'time ({tu.name})', size=label_size)
```

### Comparing `metadynminer-0.8.0/metadynminer.egg-info/PKG-INFO` & `metadynminer-0.8.1/metadynminer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metadynminer
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python package for efficient analysis of HILLS files generated by Plumed metadynamics simulations. 
 Home-page: https://github.com/Jan8be/metadynminer.py
 Author: Jan Beránek
 Author-email: Jan1.Beranek@vscht.cz
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `metadynminer-0.8.0/setup.py` & `metadynminer-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 
 setup(
     name='metadynminer',
-    version='0.8.0',
+    version='0.8.1',
     description="Python package for efficient analysis of HILLS files generated by Plumed metadynamics simulations. ",
     long_description=(this_directory / "README.md").read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/Jan8be/metadynminer.py',
     author='Jan Beránek',
     author_email='Jan1.Beranek@vscht.cz',
     license='GPL-3.0',
```

### Comparing `metadynminer-0.8.0/tests/test_fast.py` & `metadynminer-0.8.1/tests/test_fast.py`

 * *Files identical despite different names*

### Comparing `metadynminer-0.8.0/tests/test_fep.py` & `metadynminer-0.8.1/tests/test_fep.py`

 * *Files identical despite different names*

### Comparing `metadynminer-0.8.0/tests/test_minima.py` & `metadynminer-0.8.1/tests/test_minima.py`

 * *Files identical despite different names*

### Comparing `metadynminer-0.8.0/tests/test_orig.py` & `metadynminer-0.8.1/tests/test_orig.py`

 * *Files identical despite different names*

### Comparing `metadynminer-0.8.0/tests/test_readhills.py` & `metadynminer-0.8.1/tests/test_readhills.py`

 * *Files identical despite different names*

