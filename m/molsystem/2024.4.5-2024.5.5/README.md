# Comparing `tmp/molsystem-2024.4.5.tar.gz` & `tmp/molsystem-2024.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molsystem-2024.4.5.tar", last modified: Sat Apr  6 01:37:10 2024, max compression
+gzip compressed data, was "molsystem-2024.5.5.tar", last modified: Sun May  5 21:25:43 2024, max compression
```

## Comparing `molsystem-2024.4.5.tar` & `molsystem-2024.5.5.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.694393 molsystem-2024.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-06 01:36:58.000000 molsystem-2024.4.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-06 01:36:58.000000 molsystem-2024.4.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-06 01:36:58.000000 molsystem-2024.4.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-06 01:36:58.000000 molsystem-2024.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-06 01:36:58.000000 molsystem-2024.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-04-06 01:37:10.694393 molsystem-2024.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-06 01:36:58.000000 molsystem-2024.4.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.678393 molsystem-2024.4.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.678393 molsystem-2024.4.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.678393 molsystem-2024.4.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9525 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.682393 molsystem-2024.4.5/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.682393 molsystem-2024.4.5/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.682393 molsystem-2024.4.5/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.694393 molsystem-2024.4.5/molsystem/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-06 01:37:10.694393 molsystem-2024.4.5/molsystem/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/align.py
--rw-r--r--   0 runner    (1001) docker     (127)    69805 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    38056 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/bonds.py
--rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    38956 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/cif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/cms_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    36450 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/configuration_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.686393 molsystem-2024.4.5/molsystem/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/data/standard_properties.csv
--rw-r--r--   0 runner    (1001) docker     (127)    26799 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/frozencolumn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/inchi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/molfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/openbabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/pdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/pubchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/qcschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/rdkit_.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/smiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    47649 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    19509 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    36917 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/system_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/system_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    26830 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.694393 molsystem-2024.4.5/molsystem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-04-06 01:37:10.000000 molsystem-2024.4.5/molsystem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-06 01:37:10.000000 molsystem-2024.4.5/molsystem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 01:37:10.000000 molsystem-2024.4.5/molsystem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-06 01:37:10.000000 molsystem-2024.4.5/molsystem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 01:37:10.000000 molsystem-2024.4.5/molsystem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-06 01:37:10.694393 molsystem-2024.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-06 01:36:58.000000 molsystem-2024.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.690393 molsystem-2024.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.694393 molsystem-2024.4.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   269083 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/1n9v.cif
--rw-r--r--   0 runner    (1001) docker     (127)  1055288 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/aa-variants-v1.cif
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/acy.mmcif
--rw-r--r--   0 runner    (1001) docker     (127)   117392 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/aminoacids.mmcif
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/benzene.cif
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/hoh.mmcif
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/polyethylene.cif
--rw-r--r--   0 runner    (1001) docker     (127)    71597 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/spacegroup_names.json
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/trigonal.cif
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_angiotensin.py
--rw-r--r--   0 runner    (1001) docker     (127)    16521 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_bonds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_cif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_configuration_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_inchi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_molfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    18784 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_openbabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_pdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_property_timings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_pubchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_qcschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_rdkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_smiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_system_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_timings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-04-06 01:36:58.000000 molsystem-2024.4.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:25:43.198535 molsystem-2024.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-05 21:25:27.000000 molsystem-2024.5.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-05 21:25:27.000000 molsystem-2024.5.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-05 21:25:27.000000 molsystem-2024.5.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-05 21:25:27.000000 molsystem-2024.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-05 21:25:27.000000 molsystem-2024.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-05-05 21:25:43.198535 molsystem-2024.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-05 21:25:27.000000 molsystem-2024.5.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:25:43.178535 molsystem-2024.5.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:25:43.182535 molsystem-2024.5.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:25:43.182535 molsystem-2024.5.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9525 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:25:43.182535 molsystem-2024.5.5/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:25:43.182535 molsystem-2024.5.5/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:25:43.182535 molsystem-2024.5.5/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-05 21:25:27.000000 molsystem-2024.5.5/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:25:43.198535 molsystem-2024.5.5/molsystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-05 21:25:43.198535 molsystem-2024.5.5/molsystem/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69805 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38056 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/bonds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38956 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/cif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/cms_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36450 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/configuration_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:25:43.190535 molsystem-2024.5.5/molsystem/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/data/standard_properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    26799 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/frozencolumn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/inchi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/molfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/openbabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33065 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/pubchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/qcschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/rdkit_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/smiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47649 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19509 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36917 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/system_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/system_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26830 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-05-05 21:25:27.000000 molsystem-2024.5.5/molsystem/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:25:43.198535 molsystem-2024.5.5/molsystem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-05-05 21:25:43.000000 molsystem-2024.5.5/molsystem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-05 21:25:43.000000 molsystem-2024.5.5/molsystem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:25:43.000000 molsystem-2024.5.5/molsystem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-05 21:25:43.000000 molsystem-2024.5.5/molsystem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 21:25:43.000000 molsystem-2024.5.5/molsystem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-05 21:25:43.198535 molsystem-2024.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-05 21:25:27.000000 molsystem-2024.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:25:43.194535 molsystem-2024.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:25:43.198535 molsystem-2024.5.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   269083 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/data/1n9v.cif
+-rw-r--r--   0 runner    (1001) docker     (127)  1055288 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/data/aa-variants-v1.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/data/acy.mmcif
+-rw-r--r--   0 runner    (1001) docker     (127)   117392 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/data/aminoacids.mmcif
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/data/benzene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/data/hoh.mmcif
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/data/polyethylene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    71597 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/data/spacegroup_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/data/trigonal.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_angiotensin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16521 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_cif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_configuration_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_inchi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_molfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18784 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_openbabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_property_timings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_pubchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_qcschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_rdkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_system_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_timings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-05 21:25:27.000000 molsystem-2024.5.5/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-05 21:25:27.000000 molsystem-2024.5.5/versioneer.py
```

### Comparing `molsystem-2024.4.5/CONTRIBUTING.rst` & `molsystem-2024.5.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/HISTORY.rst` & `molsystem-2024.5.5/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 =======
 History
 =======
-2023.4.6 -- Added gradients
+2024.5.5 -- Bugfix: bonds in RDKit
+    * There was an indexing bug translating bonds back from RDKit to SEAMM. The famous
+      0/1 problem!
+      
+2024.4.6 -- Added gradients
     * Added gradient on atoms as a separate table alongside atoms, so they take no space
       unless actually used.
       
 2024.3.13 -- Handle uppercase X, Y, Z in strings for symmetry operators
     * the Crystallographic Open Database CIF files seems to use upper case X, Y, Z in
       explicit symmetry operators. These need to be lowercased in the code.
```

### Comparing `molsystem-2024.4.5/LICENSE` & `molsystem-2024.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/PKG-INFO` & `molsystem-2024.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molsystem
-Version: 2024.4.5
+Version: 2024.5.5
 Summary: molsystem
 Home-page: https://github.com/molssi-seamm/molsystem
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: molsystem,SEAMM
 Platform: Linux
@@ -113,15 +113,19 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
-2023.4.6 -- Added gradients
+2024.5.5 -- Bugfix: bonds in RDKit
+    * There was an indexing bug translating bonds back from RDKit to SEAMM. The famous
+      0/1 problem!
+      
+2024.4.6 -- Added gradients
     * Added gradient on atoms as a separate table alongside atoms, so they take no space
       unless actually used.
       
 2024.3.13 -- Handle uppercase X, Y, Z in strings for symmetry operators
     * the Crystallographic Open Database CIF files seems to use upper case X, Y, Z in
       explicit symmetry operators. These need to be lowercased in the code.
```

### Comparing `molsystem-2024.4.5/README.rst` & `molsystem-2024.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/Makefile` & `molsystem-2024.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/_static/SEAMM inverted.png` & `molsystem-2024.5.5/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/_static/SEAMM logo.png` & `molsystem-2024.5.5/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/_static/molssi_main_logo.png` & `molsystem-2024.5.5/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/_static/molssi_main_logo_inverted_white.png` & `molsystem-2024.5.5/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/_static/molssi_square.png` & `molsystem-2024.5.5/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/_static/nsf.png` & `molsystem-2024.5.5/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/conf.py` & `molsystem-2024.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/developer_guide/installation.rst` & `molsystem-2024.5.5/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/getting_started/index.rst` & `molsystem-2024.5.5/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/index.rst` & `molsystem-2024.5.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/make.bat` & `molsystem-2024.5.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/docs/user_guide/index.rst` & `molsystem-2024.5.5/docs/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/__init__.py` & `molsystem-2024.5.5/molsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/align.py` & `molsystem-2024.5.5/molsystem/align.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/atoms.py` & `molsystem-2024.5.5/molsystem/atoms.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/bonds.py` & `molsystem-2024.5.5/molsystem/bonds.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/cell.py` & `molsystem-2024.5.5/molsystem/cell.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/cif.py` & `molsystem-2024.5.5/molsystem/cif.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/cms_schema.py` & `molsystem-2024.5.5/molsystem/cms_schema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/column.py` & `molsystem-2024.5.5/molsystem/column.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/configuration.py` & `molsystem-2024.5.5/molsystem/configuration.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/configuration_properties.py` & `molsystem-2024.5.5/molsystem/configuration_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/data/standard_properties.csv` & `molsystem-2024.5.5/molsystem/data/standard_properties.csv`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/elements.py` & `molsystem-2024.5.5/molsystem/elements.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/frozencolumn.py` & `molsystem-2024.5.5/molsystem/frozencolumn.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/inchi.py` & `molsystem-2024.5.5/molsystem/inchi.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/molfile.py` & `molsystem-2024.5.5/molsystem/molfile.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/openbabel.py` & `molsystem-2024.5.5/molsystem/openbabel.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/pdb.py` & `molsystem-2024.5.5/molsystem/pdb.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/properties.py` & `molsystem-2024.5.5/molsystem/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
             "CREATE INDEX str_data_idx_system_property  ON str_data(system, property)"
         )
         self.db.execute(
             "CREATE INDEX str_data_idx_configuration ON str_data(configuration)"
         )
         self.db.execute("CREATE INDEX str_data_idx_system ON str_data(system)")
 
-        # Integer facts
+        # Array facts
         table = self.system_db["json_data"]
         table.add_attribute("id", coltype="int", pk=True)
         table.add_attribute("configuration", coltype="int", references="configuration")
         table.add_attribute("system", coltype="int", references="system")
         table.add_attribute("property", coltype="int", references="property")
         table.add_attribute("value", coltype="str")
```

### Comparing `molsystem-2024.4.5/molsystem/pubchem.py` & `molsystem-2024.5.5/molsystem/pubchem.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/qcschema.py` & `molsystem-2024.5.5/molsystem/qcschema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/rdkit_.py` & `molsystem-2024.5.5/molsystem/rdkit_.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 except ModuleNotFoundError:
     print(
         "Please install rdkit using conda:\n" "     conda install -c conda-forge rdkit"
     )
     raise
 
 logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
 
 # Valence
 valence = {
     1: 1,
     2: 0,
     3: 1,
     4: 2,
@@ -115,12 +116,12 @@
             Is.append(i)
             Js.append(j)
             BondOrders.append(bondorder)
             logger.debug(f"bond {i} - {j} {bondorder}")
 
         self.clear()
         ids = self.atoms.append(x=Xs, y=Ys, z=Zs, atno=atnos)
-        i = [ids[x - 1] for x in Is]
-        j = [ids[x - 1] for x in Js]
+        i = [ids[x] for x in Is]
+        j = [ids[x] for x in Js]
         self.bonds.append(i=i, j=j, bondorder=BondOrders)
 
         return self
```

### Comparing `molsystem-2024.4.5/molsystem/smiles.py` & `molsystem-2024.5.5/molsystem/smiles.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/subset.py` & `molsystem-2024.5.5/molsystem/subset.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/subsets.py` & `molsystem-2024.5.5/molsystem/subsets.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/symmetry.py` & `molsystem-2024.5.5/molsystem/symmetry.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/system.py` & `molsystem-2024.5.5/molsystem/system.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/system_db.py` & `molsystem-2024.5.5/molsystem/system_db.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/system_properties.py` & `molsystem-2024.5.5/molsystem/system_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/table.py` & `molsystem-2024.5.5/molsystem/table.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/template.py` & `molsystem-2024.5.5/molsystem/template.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/templates.py` & `molsystem-2024.5.5/molsystem/templates.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem/topology.py` & `molsystem-2024.5.5/molsystem/topology.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/molsystem.egg-info/PKG-INFO` & `molsystem-2024.5.5/molsystem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molsystem
-Version: 2024.4.5
+Version: 2024.5.5
 Summary: molsystem
 Home-page: https://github.com/molssi-seamm/molsystem
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: molsystem,SEAMM
 Platform: Linux
@@ -113,15 +113,19 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
-2023.4.6 -- Added gradients
+2024.5.5 -- Bugfix: bonds in RDKit
+    * There was an indexing bug translating bonds back from RDKit to SEAMM. The famous
+      0/1 problem!
+      
+2024.4.6 -- Added gradients
     * Added gradient on atoms as a separate table alongside atoms, so they take no space
       unless actually used.
       
 2024.3.13 -- Handle uppercase X, Y, Z in strings for symmetry operators
     * the Crystallographic Open Database CIF files seems to use upper case X, Y, Z in
       explicit symmetry operators. These need to be lowercased in the code.
```

### Comparing `molsystem-2024.4.5/molsystem.egg-info/SOURCES.txt` & `molsystem-2024.5.5/molsystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/setup.py` & `molsystem-2024.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/conftest.py` & `molsystem-2024.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/data/1n9v.cif` & `molsystem-2024.5.5/tests/data/1n9v.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/data/aa-variants-v1.cif` & `molsystem-2024.5.5/tests/data/aa-variants-v1.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/data/acy.mmcif` & `molsystem-2024.5.5/tests/data/acy.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/data/aminoacids.mmcif` & `molsystem-2024.5.5/tests/data/aminoacids.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/data/benzene.cif` & `molsystem-2024.5.5/tests/data/benzene.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/data/hoh.mmcif` & `molsystem-2024.5.5/tests/data/hoh.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/data/polyethylene.cif` & `molsystem-2024.5.5/tests/data/polyethylene.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/data/spacegroup_names.json` & `molsystem-2024.5.5/tests/data/spacegroup_names.json`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/data/trigonal.cif` & `molsystem-2024.5.5/tests/data/trigonal.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_angiotensin.py` & `molsystem-2024.5.5/tests/test_angiotensin.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_atoms.py` & `molsystem-2024.5.5/tests/test_atoms.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_bonds.py` & `molsystem-2024.5.5/tests/test_bonds.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_cell.py` & `molsystem-2024.5.5/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_cif.py` & `molsystem-2024.5.5/tests/test_cif.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_configuration_properties.py` & `molsystem-2024.5.5/tests/test_configuration_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_configurations.py` & `molsystem-2024.5.5/tests/test_configurations.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_inchi.py` & `molsystem-2024.5.5/tests/test_inchi.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_molfile.py` & `molsystem-2024.5.5/tests/test_molfile.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_openbabel.py` & `molsystem-2024.5.5/tests/test_openbabel.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_pdb.py` & `molsystem-2024.5.5/tests/test_pdb.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_properties.py` & `molsystem-2024.5.5/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_property_timings.py` & `molsystem-2024.5.5/tests/test_property_timings.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_pubchem.py` & `molsystem-2024.5.5/tests/test_pubchem.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_qcschema.py` & `molsystem-2024.5.5/tests/test_qcschema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_rdkit.py` & `molsystem-2024.5.5/tests/test_rdkit.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_smiles.py` & `molsystem-2024.5.5/tests/test_smiles.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_subsets.py` & `molsystem-2024.5.5/tests/test_subsets.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_symmetry.py` & `molsystem-2024.5.5/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_system.py` & `molsystem-2024.5.5/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_system_db.py` & `molsystem-2024.5.5/tests/test_system_db.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_table.py` & `molsystem-2024.5.5/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_templates.py` & `molsystem-2024.5.5/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_timings.py` & `molsystem-2024.5.5/tests/test_timings.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/tests/test_topology.py` & `molsystem-2024.5.5/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.4.5/versioneer.py` & `molsystem-2024.5.5/versioneer.py`

 * *Files identical despite different names*

