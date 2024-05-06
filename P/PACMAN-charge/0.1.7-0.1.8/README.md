# Comparing `tmp/PACMAN-charge-0.1.7.tar.gz` & `tmp/PACMAN-charge-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMAN-charge-0.1.7.tar", last modified: Sat May  4 13:50:15 2024, max compression
+gzip compressed data, was "PACMAN-charge-0.1.8.tar", last modified: Mon May  6 03:23:30 2024, max compression
```

## Comparing `PACMAN-charge-0.1.7.tar` & `PACMAN-charge-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:50:15.836752 PACMAN-charge-0.1.7/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.7/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:50:15.713307 PACMAN-charge-0.1.7/PACMANCharge/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.7/PACMANCharge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.7/PACMANCharge/atom_init.json
--rwxrwxrwx   0 root         (0) root         (0)    26470 2024-05-04 13:49:39.000000 PACMAN-charge-0.1.7/PACMANCharge/pmcharge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:50:15.779305 PACMAN-charge-0.1.7/PACMAN_charge.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:50:15.000000 PACMAN-charge-0.1.7/PACMAN_charge.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-04 13:50:15.000000 PACMAN-charge-0.1.7/PACMAN_charge.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-04 13:50:15.000000 PACMAN-charge-0.1.7/PACMAN_charge.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-04 13:50:15.000000 PACMAN-charge-0.1.7/PACMAN_charge.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-04 13:50:15.000000 PACMAN-charge-0.1.7/PACMAN_charge.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:50:15.834739 PACMAN-charge-0.1.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2918 2024-05-01 02:30:46.000000 PACMAN-charge-0.1.7/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-04 13:50:15.837752 PACMAN-charge-0.1.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-04 13:50:08.000000 PACMAN-charge-0.1.7/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:50:15.819305 PACMAN-charge-0.1.7/test/
--rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-04 13:47:28.000000 PACMAN-charge-0.1.7/test/Cu-BTC.cif
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.7/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      151 2024-05-04 13:49:04.000000 PACMAN-charge-0.1.7/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-06 03:23:30.079009 PACMAN-charge-0.1.8/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.8/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-06 03:23:29.958009 PACMAN-charge-0.1.8/PACMANCharge/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.8/PACMANCharge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.8/PACMANCharge/atom_init.json
+-rwxrwxrwx   0 root         (0) root         (0)    25764 2024-05-06 03:22:55.000000 PACMAN-charge-0.1.8/PACMANCharge/pmcharge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-06 03:23:30.022009 PACMAN-charge-0.1.8/PACMAN_charge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3244 2024-05-06 03:23:29.000000 PACMAN-charge-0.1.8/PACMAN_charge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-06 03:23:29.000000 PACMAN-charge-0.1.8/PACMAN_charge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-06 03:23:29.000000 PACMAN-charge-0.1.8/PACMAN_charge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-06 03:23:29.000000 PACMAN-charge-0.1.8/PACMAN_charge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-06 03:23:29.000000 PACMAN-charge-0.1.8/PACMAN_charge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3244 2024-05-06 03:23:30.078009 PACMAN-charge-0.1.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2855 2024-05-06 03:23:01.000000 PACMAN-charge-0.1.8/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-06 03:23:30.080009 PACMAN-charge-0.1.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-06 03:22:58.000000 PACMAN-charge-0.1.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-06 03:23:30.063009 PACMAN-charge-0.1.8/test/
+-rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-04 13:50:41.000000 PACMAN-charge-0.1.8/test/Cu-BTC.cif
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.8/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      151 2024-05-04 13:49:04.000000 PACMAN-charge-0.1.8/test/test.py
```

### Comparing `PACMAN-charge-0.1.7/LICENSE` & `PACMAN-charge-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.7/PACMANCharge/atom_init.json` & `PACMAN-charge-0.1.8/PACMANCharge/atom_init.json`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.7/PACMANCharge/pmcharge.py` & `PACMAN-charge-0.1.8/PACMANCharge/pmcharge.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,22 +16,20 @@
 from pymatgen.io.cif import CifParser
 from pymatgen.io.ase import AseAtomsAdaptor
 from torch.utils.data import Dataset,DataLoader
 from collections import defaultdict
 
 package_directory = os.path.abspath(__file__).replace("pmcharge.py","")
 files_to_download = {
-                    'mof-cm5.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_cm5/cm5.pth',
-                    'mof-cm5.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_cm5/normalizer-cm5.pkl',
-                    'mof-bader.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_bader/bader.pth',
-                    'mof-bader.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_bader/normalizer-bader.pkl',
-                    'mof-ddec.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec/ddec.pth',
-                    'mof-ddec.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec/normalizer-ddec.pkl',
-                    'cof.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec_cof/ddec.pth',
-                    'cof.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec_cof/normalizer-ddec.pkl',
+                    'cm5.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_cm5/cm5.pth',
+                    'cm5.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_cm5/normalizer-cm5.pkl',
+                    'bader.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_bader/bader.pth',
+                    'bader.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_bader/normalizer-bader.pkl',
+                    'ddec.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec/ddec.pth',
+                    'ddec.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec/normalizer-ddec.pkl'
                     }
 
 for file_name, url in files_to_download.items():
     file_path = os.path.join(package_directory, file_name)
     if not os.path.exists(file_path):
         response = requests.get(url)
         if response.status_code == 200:
@@ -42,18 +40,15 @@
             print(f"Failed to download {file_name} from {url}")
     else:
         pass
 
 import importlib
 import sys
 source = importlib.import_module('PACMANCharge')
-sys.modules['GCNCharge'] = source
-sys.modules['source'] = source
 sys.modules['model.utils'] = source
-sys.modules['source.utils'] = source
 sys.modules['model'] = source
     
 
 periodic_table_symbols = [
     'H', 'He', 'Li', 'Be', 'B', 'C', 'N', 'O', 'F', 'Ne', 'Na', 'Mg',
     'Al', 'Si', 'P', 'S', 'Cl', 'Ar', 'K', 'Ca', 'Sc', 'Ti', 'V', 'Cr',
     'Mn', 'Fe', 'Co', 'Ni', 'Cu', 'Zn', 'Ga', 'Ge', 'As', 'Se', 'Br', 'Kr',
@@ -66,35 +61,35 @@
     'Mt', 'Ds', 'Rg', 'Cn', 'Nh', 'Fl', 'Mc', 'Lv', 'Ts', 'Og'
     ]
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 print(f"Using device: {device}")
 
-def ase_format(mof):
+def ase_format(cif_file):
     try:
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')
-            mof_temp = Structure.from_file(mof)
-            mof_temp.to(filename=mof, fmt="cif")
-            struc = read(mof)
+            stru_temp = Structure.from_file(cif_file)
+            stru_temp.to(filename=cif_file, fmt="cif")
+            struc = read(cif_file)
     except:
         try:
-            struc = read(mof)
+            struc = read(cif_file)
         except Exception as e:
             print(e)
     return struc
 
-def CIF2json(structure,mof):
+def CIF2json(structure,cif_file):
     warnings.filterwarnings("ignore", category=UserWarning)
     try:
-        structure = read(mof)
+        structure = read(cif_file)
         struct = AseAtomsAdaptor.get_structure(structure)
     except:
-        struct = CifParser(mof, occupancy_tolerance=10)
+        struct = CifParser(cif_file, occupancy_tolerance=10)
         struct.get_structures()
     _c_index, _n_index, _, n_distance = struct.get_neighbor_list(r=6, numerical_tol=0, exclude_self=True)
     _nonmax_idx = []
     for i in range(len(structure)):
         idx_i = (_c_index == i).nonzero()[0]
         idx_sorted = np.argsort(n_distance[idx_i])[: 200]
         _nonmax_idx.append(idx_i[idx_sorted])
@@ -124,25 +119,25 @@
             "numbers": numbers,
             "index1": index1.tolist(),
             "index2":index2.tolist(),
             "dij": dij.tolist(),
             "nn_num": nn_num}
     return data
 
-def pre4pre(mof):
+def pre4pre(cif_file):
     warnings.filterwarnings("ignore", category=UserWarning)
     try:
         try:
-            structure = mg.Structure.from_file(mof)
+            structure = mg.Structure.from_file(cif_file)
         except:
             try:
-                atoms = read(mof)
+                atoms = read(cif_file)
                 structure = AseAtomsAdaptor.get_structure(atoms)
             except:
-                structure = CifParser(mof, occupancy_tolerance=10)
+                structure = CifParser(cif_file, occupancy_tolerance=10)
                 structure.get_structures()
         coords = structure.frac_coords
         try:
             elements = [str(site.specie) for site in structure.sites]
         except:
             elements = [str(site.species) for site in structure.sites]
         pos = []
@@ -166,16 +161,16 @@
             groups[key].append(i)
     for key, indices in groups.items():
         avg = sum(numbers[i] for i in indices) / len(indices)
         for i in indices:
             numbers[i] = avg
     return numbers
 
-def write4cif(mof,chg,digits,atom_type,neutral,charge_type):
-    name = mof.split('.cif')[0]
+def write4cif(cif_file,chg,digits,atom_type,neutral,charge_type):
+    name = cif_file.split('.cif')[0]
     chg = chg.numpy()
     dia = int(digits)
     
     if atom_type:
         sum_chg = sum(chg)
         charges = []
         if neutral:
@@ -491,42 +486,34 @@
         N,_ = atom_fea.shape
         for conv_func in self.convs:
             nbr_fea,atom_fea,global_fea = conv_func(atom_fea,nbr_fea,nbr_fea_idx1,nbr_fea_idx2,num_nbrs,crystal_atom_idx)          
         global_fea = global_fea / atom_nums
         z = self.phi_u(global_fea)
         return z
 
-def predict(cif_file,model_name="MOF",charge_type="DDEC6",digits=6,atom_type=True,neutral=True):
-    if model_name == "COF":
-        charge_model_name = package_directory + "cof.pth"
-        nor_name = package_directory + "cof.pkl"
-    elif model_name == "MOF":
-        if charge_type == "DDEC6":
-            charge_model_name = package_directory + 'mof-ddec.pth'
-            nor_name = package_directory + 'mof-ddec.pkl'
-        elif charge_type == "Bader":
-            charge_model_name = package_directory + 'mof-bader.pth'
-            nor_name = package_directory + 'mof-bader.pkl'
-        elif charge_type == "CM5":
-            charge_model_name = package_directory + 'mof-cm5.pth'
-            nor_name = package_directory + 'mof-cm5.pkl'
-
+def predict(cif_file,charge_type="DDEC6",digits=6,atom_type=True,neutral=True):
+   
+    if charge_type == "DDEC6":
+        charge_model_name = package_directory + 'ddec.pth'
+        nor_name = package_directory + 'ddec.pkl'
+    elif charge_type == "Bader":
+        charge_model_name = package_directory + 'bader.pth'
+        nor_name = package_directory + 'bader.pkl'
+    elif charge_type == "CM5":
+        charge_model_name = package_directory + 'cm5.pth'
+        nor_name = package_directory + 'cm5.pkl'
     
-    if model_name == "COF" and charge_type != "DDEC6":
-        raise ValueError("For COF, please use DDEC6 charges.")
     try:
         with open(nor_name, 'rb') as f:
             charge_nor = pickle.load(f)
         f.close()
     except FileNotFoundError:
         print(f"Please use correct charge")
-    
 
     print(f"CIF Name: {cif_file}")
-    print(f"Model Name: {model_name}")
     print(f"Charge Type: {charge_type}")
     print(f"Digits: {digits}")
     print(f"Atom Type: {atom_type}")
     print(f"Neutral: {neutral}")
 
     try:
         struc = ase_format(cif_file)
```

### Comparing `PACMAN-charge-0.1.7/PACMAN_charge.egg-info/PKG-INFO` & `PACMAN-charge-0.1.8/PACMAN_charge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.1.7
+Version: 0.1.8
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,19 +22,18 @@
 [![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sxm13/PACMAN/LICENSE.txt) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
 
 
 # Usage
 
 ```sh      
 from PACMANCharge import pmcharge
-PACMaN.predict(cif_file="./test/Cu-BTC.cif",model_name="MOF",charge_type="DDEC6",digits=10,atom_type=True,neutral=True)
+PACMaN.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=10,atom_type=True,neutral=True)
 ```
 
-* cif_file: cif file (without partial atomic charges) **[cif path]**                                          
-* model-name (default: MOF): MOF or COF                       
+* cif_file: cif file (without partial atomic charges) **[cif path]**                                                            
 * charge-type (default: DDE6): DDEC6, Bader or CM5                                        
 * digits (default: 6): number of decimal places to print for partial atomic charges. ML models were trained on a 6-digit dataset.                                                                     
 * atom-type (default: True): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
 * neutral (default: True): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
 
 # Website & Zenodo
 PACMAN-APP[link](https://gcn-charge-predicter-mtap.streamlit.app/)
```

### Comparing `PACMAN-charge-0.1.7/PKG-INFO` & `PACMAN-charge-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.1.7
+Version: 0.1.8
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,19 +22,18 @@
 [![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sxm13/PACMAN/LICENSE.txt) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
 
 
 # Usage
 
 ```sh      
 from PACMANCharge import pmcharge
-PACMaN.predict(cif_file="./test/Cu-BTC.cif",model_name="MOF",charge_type="DDEC6",digits=10,atom_type=True,neutral=True)
+PACMaN.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=10,atom_type=True,neutral=True)
 ```
 
-* cif_file: cif file (without partial atomic charges) **[cif path]**                                          
-* model-name (default: MOF): MOF or COF                       
+* cif_file: cif file (without partial atomic charges) **[cif path]**                                                            
 * charge-type (default: DDE6): DDEC6, Bader or CM5                                        
 * digits (default: 6): number of decimal places to print for partial atomic charges. ML models were trained on a 6-digit dataset.                                                                     
 * atom-type (default: True): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
 * neutral (default: True): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
 
 # Website & Zenodo
 PACMAN-APP[link](https://gcn-charge-predicter-mtap.streamlit.app/)
```

### Comparing `PACMAN-charge-0.1.7/README.md` & `PACMAN-charge-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 [![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sxm13/PACMAN/LICENSE.txt) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
 
 
 # Usage
 
 ```sh      
 from PACMANCharge import pmcharge
-PACMaN.predict(cif_file="./test/Cu-BTC.cif",model_name="MOF",charge_type="DDEC6",digits=10,atom_type=True,neutral=True)
+PACMaN.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=10,atom_type=True,neutral=True)
 ```
 
-* cif_file: cif file (without partial atomic charges) **[cif path]**                                          
-* model-name (default: MOF): MOF or COF                       
+* cif_file: cif file (without partial atomic charges) **[cif path]**                                                            
 * charge-type (default: DDE6): DDEC6, Bader or CM5                                        
 * digits (default: 6): number of decimal places to print for partial atomic charges. ML models were trained on a 6-digit dataset.                                                                     
 * atom-type (default: True): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
 * neutral (default: True): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.                                                                            
 
 # Website & Zenodo
 PACMAN-APP[link](https://gcn-charge-predicter-mtap.streamlit.app/)
```

### Comparing `PACMAN-charge-0.1.7/setup.py` & `PACMAN-charge-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from setuptools import setup, find_packages
 
 setup(
     name="PACMAN-charge",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     description="Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)",
     author="Guobin Zhao",
     author_email="sxmzhaogb@gmai.com",
     url="https://github.com/sxm13/PACMAN",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `PACMAN-charge-0.1.7/test/Cu-BTC.cif` & `PACMAN-charge-0.1.8/test/Cu-BTC.cif`

 * *Files identical despite different names*

