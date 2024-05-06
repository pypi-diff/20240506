# Comparing `tmp/ptwrapper-2.4.2.tar.gz` & `tmp/ptwrapper-2.4.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptwrapper-2.4.2.tar", max compression
+gzip compressed data, was "ptwrapper-2.4.2a1.tar", max compression
```

## Comparing `ptwrapper-2.4.2.tar` & `ptwrapper-2.4.2a1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    13025 2024-04-25 11:07:02.311391 ptwrapper-2.4.2/LICENSE.txt
--rw-r--r--   0        0        0     7570 2024-04-25 11:07:02.311648 ptwrapper-2.4.2/README.md
--rw-r--r--   0        0        0     2431 2024-05-06 16:06:18.745323 ptwrapper-2.4.2/pyproject.toml
--rw-r--r--   0        0        0       70 2024-04-25 11:07:02.312618 ptwrapper-2.4.2/src/ptwrapper/.flake8
--rw-r--r--   0        0        0      106 2024-05-06 16:18:22.314172 ptwrapper-2.4.2/src/ptwrapper/__init__.py
--rw-r--r--   0        0        0     9309 2024-05-06 16:20:58.889264 ptwrapper-2.4.2/src/ptwrapper/cli.py
--rw-r--r--   0        0        0    40099 2024-04-25 11:10:57.567162 ptwrapper-2.4.2/src/ptwrapper/config/age/cfg_agm_jui_multibody.xml
--rw-r--r--   0        0        0      526 2024-04-25 11:07:02.313721 ptwrapper-2.4.2/src/ptwrapper/config/age/cfg_agm_jui_multibody_event_definitions.xml
--rw-r--r--   0        0        0    22766 2024-04-25 11:07:02.313906 ptwrapper-2.4.2/src/ptwrapper/config/age/cfg_agm_jui_multibody_fixed_definitions.xml
--rw-r--r--   0        0        0    10910 2024-04-25 11:07:02.314134 ptwrapper-2.4.2/src/ptwrapper/config/age/cfg_agm_jui_multibody_predefined_block.xml
--rw-r--r--   0        0        0   291598 2024-04-25 11:07:02.314674 ptwrapper-2.4.2/src/ptwrapper/config/ise/BRF_MAL_SGICD_2_1_300101_351005.brf
--rw-r--r--   0        0        0    67932 2024-04-25 11:07:02.314981 ptwrapper-2.4.2/src/ptwrapper/config/ise/RES_C50_SA_CELLS_EFFICIENCY_310101_351003.csv
--rw-r--r--   0        0        0     5204 2024-04-25 11:07:02.315184 ptwrapper-2.4.2/src/ptwrapper/config/ise/eps.cfg
--rw-r--r--   0        0        0    76839 2024-04-25 11:07:02.315439 ptwrapper-2.4.2/src/ptwrapper/config/ise/events.juice.def
--rw-r--r--   0        0        0       59 2024-04-25 11:07:02.315622 ptwrapper-2.4.2/src/ptwrapper/config/ise/phs_com_res_sa_cells_count.asc
--rw-r--r--   0        0        0     7011 2024-04-25 11:07:02.315803 ptwrapper-2.4.2/src/ptwrapper/config/ise/units.def
--rw-r--r--   0        0        0     2107 2024-04-25 11:07:02.315964 ptwrapper-2.4.2/src/ptwrapper/config/session_file.json
--rw-r--r--   0        0        0      144 2024-04-25 11:07:02.316272 ptwrapper-2.4.2/src/ptwrapper/input/TOP_events.evf
--rw-r--r--   0        0        0       75 2024-04-25 11:07:02.316495 ptwrapper-2.4.2/src/ptwrapper/input/downlink.evf
--rw-r--r--   0        0        0     1987 2024-04-25 11:07:02.316781 ptwrapper-2.4.2/src/ptwrapper/input/edf/EDF_JUI_SPC_LINK_KAB.edf
--rw-r--r--   0        0        0     1488 2024-04-25 11:07:02.316957 ptwrapper-2.4.2/src/ptwrapper/input/edf/EDF_JUI_SPC_LINK_XB.edf
--rw-r--r--   0        0        0      748 2024-04-25 11:07:02.317127 ptwrapper-2.4.2/src/ptwrapper/input/edf/TBD.edf
--rw-r--r--   0        0        0      157 2024-04-25 11:07:02.317299 ptwrapper-2.4.2/src/ptwrapper/input/edf/TOP_experiments.edf
--rw-r--r--   0        0        0      317 2024-04-25 11:07:02.317660 ptwrapper-2.4.2/src/ptwrapper/input/edf/juice__spacecraft.edf
--rw-r--r--   0        0        0      875 2024-04-25 11:07:02.317852 ptwrapper-2.4.2/src/ptwrapper/input/edf/juice__spacecraft_platform.edf
--rw-r--r--   0        0        0      357 2024-04-25 11:07:02.318021 ptwrapper-2.4.2/src/ptwrapper/input/edf/juice__spacecraft_ssmm.edf
--rw-r--r--   0        0        0   930286 2024-04-25 11:07:02.319136 ptwrapper-2.4.2/src/ptwrapper/input/itl/TBD.itl
--rw-r--r--   0        0        0      259 2024-04-25 11:07:02.319514 ptwrapper-2.4.2/src/ptwrapper/input/itl/TOP_timelines.itl
--rw-r--r--   0        0        0      970 2024-04-25 11:07:02.319706 ptwrapper-2.4.2/src/ptwrapper/input/itl/downlink.itl
--rw-r--r--   0        0        0    27700 2024-04-25 11:07:02.319959 ptwrapper-2.4.2/src/ptwrapper/input/itl/platform.itl
--rw-r--r--   0        0        0        0 2024-04-25 11:07:02.320114 ptwrapper-2.4.2/src/ptwrapper/py.typed
--rw-r--r--   0        0        0     8034 2024-04-25 11:07:02.320366 ptwrapper-2.4.2/src/ptwrapper/utils.py
--rw-r--r--   0        0        0     8804 1970-01-01 00:00:00.000000 ptwrapper-2.4.2/setup.py
--rw-r--r--   0        0        0     8871 1970-01-01 00:00:00.000000 ptwrapper-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0    13025 2024-04-25 11:07:02.311391 ptwrapper-2.4.2a1/LICENSE.txt
+-rw-r--r--   0        0        0     7570 2024-04-25 11:07:02.311648 ptwrapper-2.4.2a1/README.md
+-rw-r--r--   0        0        0     2433 2024-04-25 13:25:24.603122 ptwrapper-2.4.2a1/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-04-25 11:07:02.312618 ptwrapper-2.4.2a1/src/ptwrapper/.flake8
+-rw-r--r--   0        0        0      105 2024-04-25 11:07:02.312787 ptwrapper-2.4.2a1/src/ptwrapper/__init__.py
+-rw-r--r--   0        0        0     9266 2024-04-25 11:07:02.313001 ptwrapper-2.4.2a1/src/ptwrapper/cli.py
+-rw-r--r--   0        0        0    40099 2024-04-25 11:10:57.567162 ptwrapper-2.4.2a1/src/ptwrapper/config/age/cfg_agm_jui_multibody.xml
+-rw-r--r--   0        0        0      526 2024-04-25 11:07:02.313721 ptwrapper-2.4.2a1/src/ptwrapper/config/age/cfg_agm_jui_multibody_event_definitions.xml
+-rw-r--r--   0        0        0    22766 2024-04-25 11:07:02.313906 ptwrapper-2.4.2a1/src/ptwrapper/config/age/cfg_agm_jui_multibody_fixed_definitions.xml
+-rw-r--r--   0        0        0    10910 2024-04-25 11:07:02.314134 ptwrapper-2.4.2a1/src/ptwrapper/config/age/cfg_agm_jui_multibody_predefined_block.xml
+-rw-r--r--   0        0        0   291598 2024-04-25 11:07:02.314674 ptwrapper-2.4.2a1/src/ptwrapper/config/ise/BRF_MAL_SGICD_2_1_300101_351005.brf
+-rw-r--r--   0        0        0    67932 2024-04-25 11:07:02.314981 ptwrapper-2.4.2a1/src/ptwrapper/config/ise/RES_C50_SA_CELLS_EFFICIENCY_310101_351003.csv
+-rw-r--r--   0        0        0     5204 2024-04-25 11:07:02.315184 ptwrapper-2.4.2a1/src/ptwrapper/config/ise/eps.cfg
+-rw-r--r--   0        0        0    76839 2024-04-25 11:07:02.315439 ptwrapper-2.4.2a1/src/ptwrapper/config/ise/events.juice.def
+-rw-r--r--   0        0        0       59 2024-04-25 11:07:02.315622 ptwrapper-2.4.2a1/src/ptwrapper/config/ise/phs_com_res_sa_cells_count.asc
+-rw-r--r--   0        0        0     7011 2024-04-25 11:07:02.315803 ptwrapper-2.4.2a1/src/ptwrapper/config/ise/units.def
+-rw-r--r--   0        0        0     2107 2024-04-25 11:07:02.315964 ptwrapper-2.4.2a1/src/ptwrapper/config/session_file.json
+-rw-r--r--   0        0        0      144 2024-04-25 11:07:02.316272 ptwrapper-2.4.2a1/src/ptwrapper/input/TOP_events.evf
+-rw-r--r--   0        0        0       75 2024-04-25 11:07:02.316495 ptwrapper-2.4.2a1/src/ptwrapper/input/downlink.evf
+-rw-r--r--   0        0        0     1987 2024-04-25 11:07:02.316781 ptwrapper-2.4.2a1/src/ptwrapper/input/edf/EDF_JUI_SPC_LINK_KAB.edf
+-rw-r--r--   0        0        0     1488 2024-04-25 11:07:02.316957 ptwrapper-2.4.2a1/src/ptwrapper/input/edf/EDF_JUI_SPC_LINK_XB.edf
+-rw-r--r--   0        0        0      748 2024-04-25 11:07:02.317127 ptwrapper-2.4.2a1/src/ptwrapper/input/edf/TBD.edf
+-rw-r--r--   0        0        0      157 2024-04-25 11:07:02.317299 ptwrapper-2.4.2a1/src/ptwrapper/input/edf/TOP_experiments.edf
+-rw-r--r--   0        0        0      317 2024-04-25 11:07:02.317660 ptwrapper-2.4.2a1/src/ptwrapper/input/edf/juice__spacecraft.edf
+-rw-r--r--   0        0        0      875 2024-04-25 11:07:02.317852 ptwrapper-2.4.2a1/src/ptwrapper/input/edf/juice__spacecraft_platform.edf
+-rw-r--r--   0        0        0      357 2024-04-25 11:07:02.318021 ptwrapper-2.4.2a1/src/ptwrapper/input/edf/juice__spacecraft_ssmm.edf
+-rw-r--r--   0        0        0   930286 2024-04-25 11:07:02.319136 ptwrapper-2.4.2a1/src/ptwrapper/input/itl/TBD.itl
+-rw-r--r--   0        0        0      259 2024-04-25 11:07:02.319514 ptwrapper-2.4.2a1/src/ptwrapper/input/itl/TOP_timelines.itl
+-rw-r--r--   0        0        0      970 2024-04-25 11:07:02.319706 ptwrapper-2.4.2a1/src/ptwrapper/input/itl/downlink.itl
+-rw-r--r--   0        0        0    27700 2024-04-25 11:07:02.319959 ptwrapper-2.4.2a1/src/ptwrapper/input/itl/platform.itl
+-rw-r--r--   0        0        0        0 2024-04-25 11:07:02.320114 ptwrapper-2.4.2a1/src/ptwrapper/py.typed
+-rw-r--r--   0        0        0     8034 2024-04-25 11:07:02.320366 ptwrapper-2.4.2a1/src/ptwrapper/utils.py
+-rw-r--r--   0        0        0     8806 1970-01-01 00:00:00.000000 ptwrapper-2.4.2a1/setup.py
+-rw-r--r--   0        0        0     8873 1970-01-01 00:00:00.000000 ptwrapper-2.4.2a1/PKG-INFO
```

### Comparing `ptwrapper-2.4.2/LICENSE.txt` & `ptwrapper-2.4.2a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/README.md` & `ptwrapper-2.4.2a1/README.md`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/pyproject.toml` & `ptwrapper-2.4.2a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptwrapper"
-version = "2.4.2"
+version = "2.4.2a1"
 description = "A Pointing Tool OSVE wrapper"
 authors = [
     "Marc Costa <marc.costa@ext.esa.int>",
     "Rafael Andres <rafael.andres@ext.esa.int>"
 
 ]
 license = "European Space Agency Public License (ESA-PL) Permissive (Type 3) – v2.4"
```

### Comparing `ptwrapper-2.4.2/src/ptwrapper/cli.py` & `ptwrapper-2.4.2a1/src/ptwrapper/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,22 @@
 from argparse import ArgumentParser
 
 from .utils import create_structure
 from .utils import remove_directory_if_empty
 
 from osve import osve
 
-
 def execute(root_scenario_path, session_file_path):
     sim = osve.osve()
     execution = sim.execute(root_scenario_path, session_file_path)
     return execution
 
-
 def cli(test=False):
     """CLI Resolve a PTR and generate a SPICE CK."""
-    parser = ArgumentParser(description='Pointing Tool Wrapper (PTWrapper) simulates a PTR and generates the '
-                                        'corresponding resolved PTR, SPICE CK kernels,'
+    parser = ArgumentParser(description='Pointing Tool Wrapper (PTWrapper) simulates a PTR and generates the corresponding resolved PTR, SPICE CK kernels,'
                                         'and other attitude related files. PTWrapper uses OSVE to simulate the PTR.')
 
     # Exclusive group for session-file and the other parameters
     exclusive_group = parser.add_mutually_exclusive_group(required=False)
     exclusive_group.add_argument("-s", "--session-file", help="Path to the session file to run the simulation. "
                                  "If provided the other arguments are ignored.")
 
@@ -138,25 +135,25 @@
             sa_bc_path = os.path.join(root_scenario_path, 'output', 'juice_sa_ptr.bc')
             if os.path.exists(sa_bc_path):
                 print(f'Renaming juice_sa_ptr.bc/csv to juice_sa_{fname}.bc/csv')
                 sh.move(sa_bc_path, os.path.join(output_dir, f'juice_sa_{fname}.bc'))
                 sh.move(os.path.join(root_scenario_path, 'output', 'juice_sa_ptr.csv'),
                         os.path.join(output_dir, f'juice_sa_{fname}.csv'))
             else:
-                print('SA CSV and CK files not generated.')
+                print(f'SA CSV and CK files not generated.')
 
         if args.mga_ck:
             mga_bc_path = os.path.join(root_scenario_path, 'output', 'juice_mga_ptr.bc')
             if os.path.exists(mga_bc_path):
                 print(f'Renaming juice_mga_ptr.bc/csv to juice_mga_{fname}.bc/csv')
                 sh.move(mga_bc_path, os.path.join(output_dir, f'juice_mga_{fname}.bc'))
                 sh.move(os.path.join(root_scenario_path, 'output', 'juice_mga_ptr.csv'),
                         os.path.join(output_dir, f'juice_mga_{fname}.csv'))
             else:
-                print('MGA CSV and CK files not generated.')
+                print(f'MGA CSV and CK files not generated.')
 
         if not args.no_power:
             print(f'Renaming power.csv to {fname.lower()}_v01_power.csv')
             sh.move(os.path.join(root_scenario_path, 'output', 'power.csv'),
                     os.path.join(output_dir, f'{fname.lower()}_v01_power.csv'))
 
         print(f'Renaming ptr_resolved.ptx to {fname.lower()}_v01_resolved.ptx')
```

### Comparing `ptwrapper-2.4.2/src/ptwrapper/config/age/cfg_agm_jui_multibody.xml` & `ptwrapper-2.4.2a1/src/ptwrapper/config/age/cfg_agm_jui_multibody.xml`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/config/age/cfg_agm_jui_multibody_event_definitions.xml` & `ptwrapper-2.4.2a1/src/ptwrapper/config/age/cfg_agm_jui_multibody_event_definitions.xml`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/config/age/cfg_agm_jui_multibody_fixed_definitions.xml` & `ptwrapper-2.4.2a1/src/ptwrapper/config/age/cfg_agm_jui_multibody_fixed_definitions.xml`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/config/age/cfg_agm_jui_multibody_predefined_block.xml` & `ptwrapper-2.4.2a1/src/ptwrapper/config/age/cfg_agm_jui_multibody_predefined_block.xml`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/config/ise/BRF_MAL_SGICD_2_1_300101_351005.brf` & `ptwrapper-2.4.2a1/src/ptwrapper/config/ise/BRF_MAL_SGICD_2_1_300101_351005.brf`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/config/ise/RES_C50_SA_CELLS_EFFICIENCY_310101_351003.csv` & `ptwrapper-2.4.2a1/src/ptwrapper/config/ise/RES_C50_SA_CELLS_EFFICIENCY_310101_351003.csv`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/config/ise/eps.cfg` & `ptwrapper-2.4.2a1/src/ptwrapper/config/ise/eps.cfg`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/config/ise/events.juice.def` & `ptwrapper-2.4.2a1/src/ptwrapper/config/ise/events.juice.def`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/config/ise/units.def` & `ptwrapper-2.4.2a1/src/ptwrapper/config/ise/units.def`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/config/session_file.json` & `ptwrapper-2.4.2a1/src/ptwrapper/config/session_file.json`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/input/edf/EDF_JUI_SPC_LINK_KAB.edf` & `ptwrapper-2.4.2a1/src/ptwrapper/input/edf/EDF_JUI_SPC_LINK_KAB.edf`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/input/edf/EDF_JUI_SPC_LINK_XB.edf` & `ptwrapper-2.4.2a1/src/ptwrapper/input/edf/EDF_JUI_SPC_LINK_XB.edf`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/input/edf/TBD.edf` & `ptwrapper-2.4.2a1/src/ptwrapper/input/edf/TBD.edf`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/input/edf/juice__spacecraft_platform.edf` & `ptwrapper-2.4.2a1/src/ptwrapper/input/edf/juice__spacecraft_platform.edf`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/input/itl/TBD.itl` & `ptwrapper-2.4.2a1/src/ptwrapper/input/itl/TBD.itl`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/input/itl/downlink.itl` & `ptwrapper-2.4.2a1/src/ptwrapper/input/itl/downlink.itl`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/input/itl/platform.itl` & `ptwrapper-2.4.2a1/src/ptwrapper/input/itl/platform.itl`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/src/ptwrapper/utils.py` & `ptwrapper-2.4.2a1/src/ptwrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ptwrapper-2.4.2/setup.py` & `ptwrapper-2.4.2a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ['osve>=2.4.1']
 
 entry_points = \
 {'console_scripts': ['ptwrapper = ptwrapper.cli:cli']}
 
 setup_kwargs = {
     'name': 'ptwrapper',
-    'version': '2.4.2',
+    'version': '2.4.2a1',
     'description': 'A Pointing Tool OSVE wrapper',
     'long_description': '# Pointing Tool Wrapper\n\nA JUICE SOC [Pointing Tool](https://juicept.esac.esa.int/) wrapper (`PTwrapper`) for WINDOWS, LINUX, and MACOSX for use in a local computer.\n\nAllows to simulate a Pointing Timeline Request (PTR) and to generate the corresponding SPICE CK, resolved PTR, \navailable Power, and quaternions dump file.\n\n`PTwrapper` is based on OSVE and mainly provides a shortcut to use the required functionalities and setup limited\nto simulate PTRs. You can find more information on OSVE [here](https://juigitlab.esac.esa.int/core-system/uplink/phs/osve).\n\n\n### Documentation\n\nDocumentation is available at the [JUICE SOC Toolkit Help](https://juicesoc.esac.esa.int/panel/#/navigation/help).\n\n\n## Installation\n\n```shx\npip install ptwrapper\n```\n\n## Development and testing\n\n* Clone this repository\n* Requirements:\n  * Python 3.7+\n* Create a virtual environment and install the dependencies\n\n```shx\npip install -e .\n```\n\nRun the tests with in the `tests` directory with:\n\n```shell\npython3 -m unittest\n```\n\n\n## Using the library\n\nAfter installing the library can be used with the Python Shell or with its CLI.\n\n\n### Python Shell\n\nA basic test of the library for a PTR processing is provided. The sample creates in the working directory a structure \nfolder to invoke the execution and dumps inside the OUTPUT folder the expected products (SPICE CK, resolved PTR, \navailable Power, and quaternions CSV)\n\n```\nimport os\n\nfrom ptwrapper import execute\nfrom ptwrapper import create_structure\n\nptr_content = """<prm>\n   <body>\n      <segment>\n         <data>\n            <timeline frame="SC">\n               <block ref="OBS">\n                  <startTime>2030-10-15T03:40:00</startTime>\n                  <endTime>2030-10-15T04:15:00</endTime>\n                  <attitude ref="track">\n                     <boresight ref="SC_Zaxis"/>\n                     <target ref="Jupiter"/>\n                     <phaseAngle ref="powerOptimised">\n                        <yDir>false</yDir>\n                     </phaseAngle>\n                     </attitude>\n                     <metadata>\n                        <comment>Track Power Optimised C3.0</comment>\n                     </metadata>\n               </block>\n            </timeline>\n         </data>\n     </segment>\n   </body>\n</prm>\n"""\nmk_path = \'metakernel.tm\'\nsession_file_path = create_structure(\'.\', mk_path, ptr_content)\nexecute(os.path.dirname(session_file_path), session_file_path)\n```\n\n### Command line interface\n\nThe package has a CLI entry point:\n\n```shell\nptwrapper -h\n\nusage: ptwrapper [-h] [-s SESSION_FILE] [-m META_KERNEL] [-p PTR] [-w WORKING_DIR] [-o OUTPUT_DIR] [-t TIME_STEP] [-np] [-sa] [-mga] [-q] [-f] [-v]\n\nPointing Tool Wrapper (PTWrapper) simulates a PTR and generates the corresponding resolved PTR, SPICE CK kernels,and other attitude related files. PTWrapper uses OSVE to simulate the PTR.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -s SESSION_FILE, --session-file SESSION_FILE\n                        Path to the session file to run the simulation. If provided the other arguments are ignored.\n  -m META_KERNEL, --meta-kernel META_KERNEL\n                        Path to the meta-kernel file.\n  -p PTR, --ptr PTR     Path to the PTR/PTX file input file.\n  -w WORKING_DIR, --working-dir WORKING_DIR\n                        Path to the working directory. Default is the current directory.\n  -o OUTPUT_DIR, --output-dir OUTPUT_DIR\n                        Path to the output directory. Overwrites default output file names. Default is the structure of the built-in session file.\n  -t TIME_STEP, --time-step TIME_STEP\n                        Output CK file time step in seconds. Default is 5s.\n  -np, --no-power       Indicates not to calculate available power. Default is that the Available Power will be computed.\n  -sa, --sa-ck          Generate the Solar Arrays SPICE CK. Default is that the SA CK is not generated.\n  -mga, --mga-ck        Generate the Medium Gain Antenna SPICE CK. Default is that the MGA CK is not generated.\n  -q, --quaternions     Calculate the quaternions. Default is that the quaternions will not be computed.\n  -f, --fixed-definitions\n                        Print the AGM Fixed Definitions in use for PTR design.\n  -v, --version         OSVE, AGM, and EPS libraries version.\n```\n\nYou can either run the CLI using an OSVE configuration file (`SESSION_FILE`) or by specifying a \nnumber of inputs and assume the rest of parameters as provided by the default configuration file \nincluded in the package. \n\nIn addition, if you do not specify an output directory (`OUTPUT_DIR`), the package will replicate\nthe canonical output directory and file structure and will also generate a `SESSION_FILE` that can\nbe reused. Contrarily, if you specify an `OUTPUT_DIR` the output will be simplified and provided in\nthat directory; additionally the output files will inherit the name of the input `PTR` file.\n\n> **WARNING:** Remember that the input `META_KERNEL` needs to have an adequate \n> relative or absolute path for its `PATH_VALUES` variable value.\n\nA couple of examples are provided hereunder. First specifying the output directory:\n\n```shell\nptwrapper -m kernels/juice_mini_local.tm -p ptr_simphony.xml -o . \n\nptwrapper session execution\nAGM version:  9.3.0.p1\nOSVE version: 1.6.0\n[INFO]    <AGE>  Attitude Generation Module initialization started\n[INFO]    <AGE>  AGE module setup started\n[INFO]    <AGE>  AGE module setup successfully completed\n[INFO]    <AGE>  Attitude Generation Module initialization completed\n[INFO]    <AGE>  Loading Attitude Timeline\n[INFO]    <AGE>  Checking Attitude Timeline\n[INFO]    <AGE>  Initializing Attitude Timeline\n[INFO]    <AGE>   TOTAL ENERGY for POINTING block from 2030-10-15T03:40:00Z to 2030-10-15T04:15:00Z\n[INFO]    <AGE>   Attitude from actual PTR: 812.096753 Wh (812.096753 Wh)\n[INFO]    <AGE>   Attitude from loaded CK:  812.096096 Wh (812.096096 Wh)\n[INFO]    <PIF>  XML PTR file: "ptr_resolved.ptx" generated\n[INFO]    <PIF>  Generating CK file with the following USER DEFINED parameters:\n[INFO]    <PIF>  CK frame ID:  -28001\n[INFO]    <PIF>  CK time step: 5 s\n[INFO]    <AGE>  Writing Attitude Spice CK File: juice_sc_ptr.bc\n[INFO]    <PIF>  CK file: "juice_sc_ptr.bc" generated\n[INFO]    <AGE>  Writing Attitude Text File\n[INFO]    <PIF>  POWER CSV file: "power.csv" generated\nRenaming quaternions.csv to ptr_simphony_quaternions.csv\nRenaming power.csv to ptr_simphony_power.csv\nRenaming ptr_resolved.ptx to ptr_simphony_resolved.ptx\nRenaming juice_sc_ptr.bc to ptr_simphony.bc\nCleaning up OSVE execution files and directories\n```\n\nThis will generate the following output files.\n\n```shell\n.\n|-- ptr_simphony.bc\n|-- ptr_simphony.csv\n|-- ptr_simphony.xml\n|-- ptr_simphony_log.json\n`-- ptr_simphony_resolved.ptx\n```\n\nThe same run without specifying the `OUTPUT_DIRECTORY` yields the following directory structure:\n\n```shell\n.\n|-- config\n|   |-- age\n|   |   |-- cfg_agm_jui_jupiter.xml\n|   |   |-- cfg_agm_jui_multibody_event_definitions.xml\n|   |   |-- cfg_agm_jui_multibody_fixed_definitions.xml\n|   |   `-- cfg_agm_jui_multibody_predefined_block.xml\n|   `-- ise\n|       |-- BRF_MAL_SGICD_2_1_300101_351005.brf\n|       |-- RES_C50_SA_CELLS_EFFICIENCY_310101_351003.csv\n|       |-- eps.cfg\n|       |-- events.juice.def\n|       |-- phs_com_res_sa_cells_count.asc\n|       `-- units.def\n|-- kernel\n|   `-- juice_mini_local.tm\n|-- output\n|   |-- juice_sc_ptr.bc\n|   |-- power.csv\n|   |-- ptr_resolved.ptx\n|   |-- log.json\n|   `-- quaternions.csv\n|-- ptr\n|   `-- PTR_PT_V1.ptx\n`-- session_file.json\n```',
     'author': 'Marc Costa',
     'author_email': 'marc.costa@ext.esa.int',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://juigitlab.esac.esa.int/core-system/uplink/auxiliary-tools/ptwrapper',
```

### Comparing `ptwrapper-2.4.2/PKG-INFO` & `ptwrapper-2.4.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptwrapper
-Version: 2.4.2
+Version: 2.4.2a1
 Summary: A Pointing Tool OSVE wrapper
 Home-page: https://juigitlab.esac.esa.int/core-system/uplink/auxiliary-tools/ptwrapper
 License: European Space Agency Public License (ESA-PL) Permissive (Type 3) – v2.4
 Author: Marc Costa
 Author-email: marc.costa@ext.esa.int
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

