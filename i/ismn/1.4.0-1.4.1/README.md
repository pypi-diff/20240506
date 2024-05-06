# Comparing `tmp/ismn-1.4.0.tar.gz` & `tmp/ismn-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ismn-1.4.0.tar", last modified: Wed Feb 21 10:59:03 2024, max compression
+gzip compressed data, was "ismn-1.4.1.tar", last modified: Mon May  6 15:13:34 2024, max compression
```

## Comparing `ismn-1.4.0.tar` & `ismn-1.4.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.827879 ismn-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-21 10:56:20.000000 ismn-1.4.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.791879 ismn-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.799878 ismn-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-02-21 10:56:20.000000 ismn-1.4.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-21 10:56:20.000000 ismn-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-21 10:56:20.000000 ismn-1.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-21 10:56:20.000000 ismn-1.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-02-21 10:56:20.000000 ismn-1.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-21 10:56:20.000000 ismn-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-02-21 10:59:03.827879 ismn-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-02-21 10:56:20.000000 ismn-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.799878 ismn-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.799878 ismn-1.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.803879 ismn-1.4.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    17510 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/examples/custom_meta.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1084736 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/examples/interface.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   510142 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/examples/ismn.png
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/examples/vod.csv
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-21 10:56:20.000000 ismn-1.4.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-02-21 10:56:20.000000 ismn-1.4.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-21 10:56:20.000000 ismn-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-21 10:59:03.827879 ismn-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-21 10:56:20.000000 ismn-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.791879 ismn-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.803879 ismn-1.4.0/src/ismn/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-21 10:56:20.000000 ismn-1.4.0/src/ismn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-02-21 10:56:20.000000 ismn-1.4.0/src/ismn/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    29957 2024-02-21 10:56:20.000000 ismn-1.4.0/src/ismn/citations.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-02-21 10:56:20.000000 ismn-1.4.0/src/ismn/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-02-21 10:56:20.000000 ismn-1.4.0/src/ismn/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-02-21 10:56:20.000000 ismn-1.4.0/src/ismn/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-02-21 10:56:20.000000 ismn-1.4.0/src/ismn/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-02-21 10:56:20.000000 ismn-1.4.0/src/ismn/filecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26005 2024-02-21 10:56:20.000000 ismn-1.4.0/src/ismn/filehandlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    37858 2024-02-21 10:56:20.000000 ismn-1.4.0/src/ismn/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    18942 2024-02-21 10:56:20.000000 ismn-1.4.0/src/ismn/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.823879 ismn-1.4.0/src/ismn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-02-21 10:59:03.000000 ismn-1.4.0/src/ismn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-02-21 10:59:03.000000 ismn-1.4.0/src/ismn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 10:59:03.000000 ismn-1.4.0/src/ismn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-21 10:59:03.000000 ismn-1.4.0/src/ismn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 10:58:46.000000 ismn-1.4.0/src/ismn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-21 10:59:03.000000 ismn-1.4.0/src/ismn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-21 10:59:03.000000 ismn-1.4.0/src/ismn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.807879 ismn-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.807879 ismn-1.4.0/tests/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)    98165 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/baseline/test_interface_plotting.png
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_custom_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.807879 ismn-1.4.0/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.807879 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.795879 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.811879 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/
--rw-r--r--   0 runner    (1001) docker     (127)   948144 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.811879 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/
--rw-r--r--   0 runner    (1001) docker     (127)   979186 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.795879 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.819879 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/
--rwxr-xr-x   0 runner    (1001) docker     (127)  7186150 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_sm_0.050000_0.050000_ThetaProbe-ML2X_19500101_20210131.stm
--rwxr-xr-x   0 runner    (1001) docker     (127)     2885 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_static_variables.csv
--rw-r--r--   0 runner    (1001) docker     (127)    41902 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/Metadata.xml
--rw-r--r--   0 runner    (1001) docker     (127)   481431 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.819879 ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.795879 ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.823879 ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/
--rw-r--r--   0 runner    (1001) docker     (127)   213697 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.823879 ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/
--rw-r--r--   0 runner    (1001) docker     (127)   223981 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv
--rw-r--r--   0 runner    (1001) docker     (127)    41902 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/Metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.823879 ismn-1.4.0/tests/test_data/custom_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/custom_metadata/custom_sensormeta.csv
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/custom_metadata/custom_stationmeta.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.795879 ismn-1.4.0/tests/test_data/format_ceop_sep/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.823879 ismn-1.4.0/tests/test_data/format_ceop_sep/SMOSMANIA/
--rwxr-xr-x   0 runner    (1001) docker     (127)   102268 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/format_ceop_sep/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.795879 ismn-1.4.0/tests/test_data/format_header_values/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.823879 ismn-1.4.0/tests/test_data/format_header_values/SMOSMANIA/
--rwxr-xr-x   0 runner    (1001) docker     (127)    23088 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/format_header_values/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.823879 ismn-1.4.0/tests/test_data/malformed/
--rwxr-xr-x   0 runner    (1001) docker     (127)       17 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/malformed/mal_formed_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.795879 ismn-1.4.0/tests/test_data/zip_archives/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.823879 ismn-1.4.0/tests/test_data/zip_archives/ceop/
--rw-r--r--   0 runner    (1001) docker     (127)   105176 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/zip_archives/ceop/Data_seperate_files_20170810_20180809.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.823879 ismn-1.4.0/tests/test_data/zip_archives/format_header_values/
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/zip_archives/format_header_values/Data_SMOSMANIA.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.823879 ismn-1.4.0/tests/test_data/zip_archives/header/
--rw-r--r--   0 runner    (1001) docker     (127)    52474 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/zip_archives/header/Data_seperate_files_header_20170810_20180809.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.795879 ismn-1.4.0/tests/test_data/zip_archives/multinetwork/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:59:03.823879 ismn-1.4.0/tests/test_data/zip_archives/multinetwork/header_values/
--rw-r--r--   0 runner    (1001) docker     (127)   609917 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_data/zip_archives/multinetwork/header_values/Data_header_values.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_depth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_filecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_filehandler_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_filehandler_static.py
--rw-r--r--   0 runner    (1001) docker     (127)    12685 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-02-21 10:56:20.000000 ismn-1.4.0/tests/test_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.712715 ismn-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-06 15:11:10.000000 ismn-1.4.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.680715 ismn-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.684715 ismn-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-06 15:11:10.000000 ismn-1.4.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-06 15:11:10.000000 ismn-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-06 15:11:10.000000 ismn-1.4.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 15:11:10.000000 ismn-1.4.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-06 15:11:10.000000 ismn-1.4.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-06 15:11:10.000000 ismn-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-05-06 15:13:34.712715 ismn-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12732 2024-05-06 15:11:10.000000 ismn-1.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.684715 ismn-1.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.684715 ismn-1.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.688715 ismn-1.4.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    17510 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/examples/custom_meta.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1084761 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/examples/interface.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   510142 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/examples/ismn.png
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/examples/vod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 15:11:10.000000 ismn-1.4.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-06 15:11:10.000000 ismn-1.4.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-06 15:11:10.000000 ismn-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-06 15:13:34.712715 ismn-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-06 15:11:10.000000 ismn-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.680715 ismn-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.692715 ismn-1.4.1/src/ismn/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 15:11:10.000000 ismn-1.4.1/src/ismn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11412 2024-05-06 15:11:10.000000 ismn-1.4.1/src/ismn/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29957 2024-05-06 15:11:10.000000 ismn-1.4.1/src/ismn/citations.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-05-06 15:11:10.000000 ismn-1.4.1/src/ismn/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32309 2024-05-06 15:11:10.000000 ismn-1.4.1/src/ismn/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-05-06 15:11:10.000000 ismn-1.4.1/src/ismn/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-05-06 15:11:10.000000 ismn-1.4.1/src/ismn/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17171 2024-05-06 15:11:10.000000 ismn-1.4.1/src/ismn/filecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26046 2024-05-06 15:11:10.000000 ismn-1.4.1/src/ismn/filehandlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37930 2024-05-06 15:11:10.000000 ismn-1.4.1/src/ismn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18942 2024-05-06 15:11:10.000000 ismn-1.4.1/src/ismn/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.708715 ismn-1.4.1/src/ismn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-05-06 15:13:34.000000 ismn-1.4.1/src/ismn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-06 15:13:34.000000 ismn-1.4.1/src/ismn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:13:34.000000 ismn-1.4.1/src/ismn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 15:13:34.000000 ismn-1.4.1/src/ismn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:13:17.000000 ismn-1.4.1/src/ismn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-06 15:13:34.000000 ismn-1.4.1/src/ismn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 15:13:34.000000 ismn-1.4.1/src/ismn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.692715 ismn-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.692715 ismn-1.4.1/tests/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)    98165 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/baseline/test_interface_plotting.png
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_custom_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.692715 ismn-1.4.1/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.692715 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.680715 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.696715 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/
+-rw-r--r--   0 runner    (1001) docker     (127)   948144 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.696715 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/
+-rw-r--r--   0 runner    (1001) docker     (127)   979186 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.680715 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.704715 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/
+-rwxr-xr-x   0 runner    (1001) docker     (127)  7186150 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_sm_0.050000_0.050000_ThetaProbe-ML2X_19500101_20210131.stm
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2885 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_static_variables.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    41902 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/Metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   481431 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.708715 ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.680715 ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.708715 ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/
+-rw-r--r--   0 runner    (1001) docker     (127)   213697 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.708715 ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/
+-rw-r--r--   0 runner    (1001) docker     (127)   223981 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    41902 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/Metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.708715 ismn-1.4.1/tests/test_data/custom_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/custom_metadata/custom_sensormeta.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/custom_metadata/custom_stationmeta.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.684715 ismn-1.4.1/tests/test_data/format_ceop_sep/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.708715 ismn-1.4.1/tests/test_data/format_ceop_sep/SMOSMANIA/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   102268 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/format_ceop_sep/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.684715 ismn-1.4.1/tests/test_data/format_header_values/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.708715 ismn-1.4.1/tests/test_data/format_header_values/SMOSMANIA/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23088 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/format_header_values/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.708715 ismn-1.4.1/tests/test_data/malformed/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       17 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/malformed/mal_formed_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.684715 ismn-1.4.1/tests/test_data/zip_archives/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.708715 ismn-1.4.1/tests/test_data/zip_archives/ceop/
+-rw-r--r--   0 runner    (1001) docker     (127)   105176 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/zip_archives/ceop/Data_seperate_files_20170810_20180809.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.708715 ismn-1.4.1/tests/test_data/zip_archives/format_header_values/
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/zip_archives/format_header_values/Data_SMOSMANIA.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.708715 ismn-1.4.1/tests/test_data/zip_archives/header/
+-rw-r--r--   0 runner    (1001) docker     (127)    52474 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/zip_archives/header/Data_seperate_files_header_20170810_20180809.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.684715 ismn-1.4.1/tests/test_data/zip_archives/multinetwork/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:13:34.708715 ismn-1.4.1/tests/test_data/zip_archives/multinetwork/header_values/
+-rw-r--r--   0 runner    (1001) docker     (127)   609917 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_data/zip_archives/multinetwork/header_values/Data_header_values.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_filecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_filehandler_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_filehandler_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12685 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-06 15:11:10.000000 ismn-1.4.1/tests/test_readers.py
```

### Comparing `ismn-1.4.0/.coveragerc` & `ismn-1.4.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/.github/workflows/build.yml` & `ismn-1.4.1/.github/workflows/build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,31 @@
 name: Automated Tests
 
 on:
   push:
   pull_request:
   workflow_dispatch:
   schedule:
-    - cron: '0 0 * * *' # daily
+    - cron: '0 0 * * *'  # nightly build
 
 jobs:
   build:
-    name: Build py${{ matrix.python-version }} @ ${{ matrix.os }} 🐍
+    name: py${{ matrix.python-version }} @ ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11']
-        os: ["ubuntu-latest"]
         include:
+          - os: "ubuntu-latest"
+            python-version: '3.8'  # first supported
+          - os: "ubuntu-latest"
+            python-version: '3.12'  # latest supported
           - os: "windows-latest"
-            python-version: '3.11'
+            python-version: '3.12'  # latest supported
+          - os: "macos-latest"
+            python-version: '3.12'  # latest supported
     steps:
       - uses: actions/checkout@v2
         with:
           submodules: true
           fetch-depth: 0
       - uses: conda-incubator/setup-miniconda@v2
         with:
@@ -52,15 +56,15 @@
         run: |
           mkdir -p .artifacts
           filename=env_py${{ matrix.python-version }}_${{ matrix.os }}.yml
           conda env export --no-builds | grep -v "prefix" > .artifacts/$filename
       - name: Install package and test
         shell: bash -l {0}
         run: |
-          pip install .
+          python setup.py develop
           pytest
       - name: Upload Coverage
         shell: bash -l {0}
         run: |
           pip install coveralls && coveralls --service=github
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
@@ -77,17 +81,17 @@
             python setup.py bdist_wheel --dist-dir .artifacts/dist
           else
             # build dist on linux
             python setup.py sdist --dist-dir .artifacts/dist
           fi
           ls .artifacts/dist
       - name: Upload Artifacts
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v4
         with:
-          name: Artifacts
+          name: Artifacts-py${{ matrix.python-version }}-${{ matrix.os }}
           path: .artifacts/*
   coveralls:
     name: Submit Coveralls 👚
     needs: build
     runs-on: ubuntu-latest
     container: python:3-slim
     steps:
@@ -103,15 +107,19 @@
     runs-on: ubuntu-latest
     steps:
       - name: Print environment variables
         run: |
           echo "GITHUB_REF = $GITHUB_REF"
           echo "GITHUB_REPOSITORY = $GITHUB_REPOSITORY"
       - name: Download Artifacts
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v4
+        with:
+          path: Artifacts
+          pattern: Artifacts-*
+          merge-multiple: true
       - name: Display downloaded files
         run: ls -aR
       - name: Upload to PyPI
         uses: pypa/gh-action-pypi-publish@v1.4.1
         with:
           skip_existing: true
           verbose: true
```

### Comparing `ismn-1.4.0/.gitignore` & `ismn-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/CHANGELOG.rst` & `ismn-1.4.1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 =========
 Changelog
 =========
 
 Unreleased changes in master branch
 ===================================
 
+-
+
+Version 1.4.1
+=============
+
+- Fixed a bug where some ISMN files could not be parsed correctly due to empty spaces in the sensor name (`Issue #81 <https://github.com/TUW-GEO/ismn/issues/81>`_)
+- Parallel metadata collection now uses the repurpose package wrapper around joblib
+- Logging was improved for metadata collection
 
 Version 1.4.0
 =============
 
 - Added `ismn collect_metadata` and `ismn export_geojson` CLI programs.
 - Added method to NetworkCollection to export metadata as (geo)json.
 - Added more options when plotting the station overview map.
```

### Comparing `ismn-1.4.0/LICENSE.txt` & `ismn-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/docs/Makefile` & `ismn-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/docs/conf.py` & `ismn-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/docs/examples/custom_meta.ipynb` & `ismn-1.4.1/docs/examples/custom_meta.ipynb`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/docs/examples/interface.ipynb` & `ismn-1.4.1/docs/examples/interface.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999801912568306%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'Data for your study area can be selected and downloaded "*

 * *            "for free from <http://ismn.earth> after registration.')], delete: [2]}}, 1: "*

 * *            '{\'source\': {insert: [(4, "ISMN files are downloaded as a compressed `.zip` file '*

 * *            'after selecting the data from the website. You can extract it (with any zip software) '*

 * *            "locally into one (root) folder (in this case 'Data_separate_files'). The archive will "*

 * *            'be organ […]*

```diff
@@ -2,26 +2,26 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Reading ISMN data (`ismn.interface.ISMN_Interface`)\n",
                 "This example shows the basic functionality to read data downloaded from the International Soil Moisture Network (ISMN).\n",
-                "The data can be selected and downloaded for free from <http://ismn.earth> after registration."
+                "Data for your study area can be selected and downloaded for free from <http://ismn.earth> after registration."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For this tutorial, data (all available variables) for ISMN networks 'REMEDHUS', 'SMOSMANIA', 'FMI', 'WEGENERNET', 'GTK', 'VAS' and 'RSMN' between 2009-08-04 and 2020-12-12 was downloaded from the ISMN website. Note that - depending on when you download the data  - available stations and measurement values can vary slightly from those shown in this example.\n",
                 "\n",
                 "<img src=\"ismn.png\" style=\"height: 450px;\"/>\n",
                 "\n",
-                "ISMN files are downloaded as a compressed `.zip` file after selecting the data from the website. You can extract it (with any zip software) locally into one (root) folder (in this case 'Data_separate_files'). The will be organised like this:\n",
+                "ISMN files are downloaded as a compressed `.zip` file after selecting the data from the website. You can extract it (with any zip software) locally into one (root) folder (in this case 'Data_separate_files'). The archive will be organised like this:\n",
                 "```shell\n",
                 "Data_separate_files/\n",
                 "\u251c\u2500\u2500 network/\n",
                 "\u2502   \u251c\u2500\u2500 station/\n",
                 "\u2502   \u2502   \u251c\u2500\u2500 sensor.stm\n",
                 "\u2502   \u2502   \u251c\u2500\u2500 sensor.stm\n",
                 "\u2502   \u2502   \u251c\u2500\u2500 ...\n",
```

### Comparing `ismn-1.4.0/docs/examples/ismn.png` & `ismn-1.4.1/docs/examples/ismn.png`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/setup.cfg` & `ismn-1.4.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = ismn
 description = Readers for the data from the International Soil Moisture Database
 author = TU Wien
-author-email = ismn@geo.tuwien.ac.at
+author_email = ismn@geo.tuwien.ac.at
 license = mit
-long-description = file: README.rst
-long-description-content-type = text/x-rst; charset=UTF-8
+long_description = file: README.rst
+long_description_content_type = text/x-rst; charset=UTF-8
 url = http://ismn.geo.tuwien.ac.at
-project-urls = 
+project_urls = 
 	Documentation = https://ismn.readthedocs.io/en/latest/
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
@@ -25,14 +25,15 @@
 	pygeogrids>=0.3.2
 	numpy
 	pandas
 	click
 	configparser
 	more_itertools
 	tqdm
+	repurpose>=0.11
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `ismn-1.4.0/setup.py` & `ismn-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/src/ismn/__init__.py` & `ismn-1.4.1/src/ismn/__init__.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/src/ismn/base.py` & `ismn-1.4.1/src/ismn/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
             raise IOError("Zip archive expected, use @dir functions instead.")
         return func(cls, *args, **kwargs)
 
     return wrapper
 
 
 def dir(func):
-
     def wrapper(cls, *args, **kwargs):
         if cls.zip:
             raise IOError(
                 "Unzipped archive expected, use @zip functions instead.")
         return func(cls, *args, **kwargs)
 
     return wrapper
```

### Comparing `ismn-1.4.0/src/ismn/citations.txt` & `ismn-1.4.1/src/ismn/citations.txt`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/src/ismn/cli.py` & `ismn-1.4.1/src/ismn/cli.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/src/ismn/components.py` & `ismn-1.4.1/src/ismn/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,36 +16,28 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import os.path
-
+import sys
 from pygeogrids import BasicGrid
 from typing import Union
 
 import numpy as np
 import warnings
-import logging
 from collections import OrderedDict
+import pandas as pd
 
 from ismn.meta import MetaData, Depth
-from ismn.const import deprecated, CITATIONS
+from ismn.const import deprecated, CITATIONS, ismnlog
 
 import json
 
-logger = logging.getLogger(__name__)
-
-ch = logging.StreamHandler()
-ch.setLevel(logging.INFO)
-formatter = logging.Formatter("%(levelname)s - %(asctime)s: %(message)s")
-ch.setFormatter(formatter)
-logger.addHandler(ch)
-
 
 class IsmnComponent:
     pass
 
 
 class Sensor(IsmnComponent):
     """
@@ -117,27 +109,73 @@
         return MetaData(
         ) if self.filehandler is None else self.filehandler.metadata
 
     @property
     def data(self):
         return self.read_data()
 
+    def get_coverage(self, only_good=True, start=None, end=None,
+                     freq='1h'):
+        """
+        Estimate the temporal coverage of this sensor, i.e. the percentage
+        of valid observations in the sensor time series.
+
+        Returns
+        -------
+        only_good: bool, optional (default: True)
+            Only consider values where the ISMN quality flag is 'G'
+            as valid observations
+        start: str or datetime, optional (default: None)
+            Beginning of the period in which measurements are expected.
+            If None, the start of the time series is used.
+        end: str or datetime, optional (default: None)
+            End of the period in which measurements are expected.
+            If None, the start of the time series is used.
+        freq: str, optional (default: '1h')
+            Frequency at which the sensor is expected to take measurements.
+            Most sensors in ISMN provide hourly measurements (default).
+            If a different frequency is used, it must be on that
+            :func:`pd.date_range` can interpret.
+
+        Returns
+        -------
+        perc_coverage : float
+            Data coverage of the sensor at the chosen expected measurement
+            frequency within the chosen period. 0=No data, 100=no data gaps
+        """
+        data = self.read_data()
+        if start is None:
+            start = pd.Timestamp(data.index.values[0]).to_pydatetime()
+        else:
+            start = pd.to_datetime(start)
+        if end is None:
+            end = pd.Timestamp(data.index.values[-1]).to_pydatetime()
+        else:
+            end = pd.to_datetime(end)
+
+        if only_good:
+            data = data[data[f"{self.variable}_flag"] == 'G'].loc[:, self.variable]
+
+        cov = (len(data.values) / len(pd.date_range(start, end, freq=freq))) * 100
+
+        return cov
+
     def read_data(self):
         """
         Load data from filehandler for this Sensor by calling
         :func:`ismn.filehandlers.DataFile.read_data`.
 
         Returns
         -------
         data : pandas.DataFrame
             Insitu time series for this sensor, loaded from file or memory
             (if it was loaded and kept before).
         """
         if self.filehandler is None:
-            logging.warning(f"No filehandler found for sensor {self.name}")
+            ismnlog.warning(f"No filehandler found for sensor {self.name}")
         else:
             if self._data is None:
                 data = self.filehandler.read_data()
 
                 if self.keep_loaded_data:
                     self._data = data
 
@@ -409,29 +447,29 @@
                 variable,
                 depth,
                 name,
                 filehandler,
                 keep_loaded_data,
             )
         else:
-            logger.warning(f"Sensor already exists: {name}")
+            ismnlog.warning(f"Sensor already exists: {name}")
 
     def remove_sensor(self, name):
         """
         Remove sensor from station.
 
         Parameters
         ----------
         name : str
             Sensor name.
         """
         if name in self.sensors:
             del self.sensors[name]
         else:
-            logger.warning(f"Sensor not found: {name}")
+            ismnlog.warning(f"Sensor not found: {name}")
 
     def iter_sensors(self, **filter_kwargs):
         """
         Iterates over all sensors in this station and yields those that
         comply with the passed filter settings (or all).
 
         Parameters
@@ -560,29 +598,29 @@
             Latitude coordinate.
         elev : float
             Elevation.
         """
         if name not in self.stations:
             self.stations[name] = Station(name, lon, lat, elev)
         else:
-            logger.warning(f"Station already exists: {name}")
+            ismnlog.warning(f"Station already exists: {name}")
 
     def remove_station(self, name):
         """
         Remove Station from Network.
 
         Parameters
         ----------
         name : str
             Station name.
         """
         if name in self.stations:
             del self.stations[name]
         else:
-            logger.warning(f"Station not found {name}")
+            ismnlog.warning(f"Station not found {name}")
 
     def iter_stations(self, **filter_kwargs):
         """
         Get all stations having at least one sensor observing
         a specific variable and/or sensing depth.
 
         Parameters
```

### Comparing `ismn-1.4.0/src/ismn/const.py` & `ismn-1.4.1/src/ismn/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,21 +16,29 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import numpy as np
+import sys
 from collections import OrderedDict
 import functools
 import warnings
 import os
 import pandas as pd
+import logging
+import numpy as np
 
+ismnlog = logging.getLogger('ismn')
+ch = logging.StreamHandler()
+ch.setLevel(logging.INFO)
+formatter = logging.Formatter("%(levelname)s - %(asctime)s: %(message)s")
+ch.setFormatter(formatter)
+ismnlog.addHandler(ch)
 
 def deprecated(func):
     # mark func as deprecated (warn when used)
     @functools.wraps(func)
     def new_func(*args, **kwargs):
         warnings.simplefilter("always", DeprecationWarning)
         warnings.warn(
@@ -55,15 +63,14 @@
 class IsmnFileError(IOError):
     pass
 
 
 class DepthError(ValueError):
     pass
 
-
 # Note: At the moment citations are stored in this package, keep them updated.
 #  Once the full list of citations is provided together with the downloaded
 #  ISMN data (in the README file), citations here can be deleted (keep in mind
 #  that people might still use old data, but a new version of the package).
 CITATIONS: dict = (
     pd.read_csv(
         os.path.join(os.path.dirname(__file__), "citations.txt"),
```

### Comparing `ismn-1.4.0/src/ismn/custom.py` & `ismn-1.4.1/src/ismn/custom.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/src/ismn/filecollection.py` & `ismn-1.4.1/src/ismn/filecollection.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,75 +22,87 @@
 
 import logging
 
 import os
 from tempfile import gettempdir
 from pathlib import Path, PurePosixPath
 import numpy as np
-from tqdm import tqdm
 from typing import Union
-from multiprocessing import Pool, cpu_count
 from operator import itemgetter
 import time
-from typing import Tuple
+from typing import List, Tuple
 import pandas as pd
 from collections import OrderedDict
+from repurpose.process import parallel_process_async
+import traceback
 
 from ismn.base import IsmnRoot
 import ismn.const as const
+from ismn.const import ismnlog
 from ismn.filehandlers import DataFile, StaticMetaFile
 from ismn.meta import MetaData, MetaVar, Depth
 
 
 def _read_station_dir(
     root: Union[IsmnRoot, Path, str],
     stat_dir: Union[Path, str],
     temp_root: Path,
     custom_meta_reader: list,
-) -> Tuple[dict, list]:
+) -> Tuple[List, List]:
     """
     Parallelizable function to read metadata for files in station dir
     """
-    infos = []
+    logger = logging.getLogger('ismn_meta_collector')
 
     if not isinstance(root, IsmnRoot):
         proc_root = True
         root = IsmnRoot(root)
     else:
         proc_root = False
 
     csv = root.find_files(stat_dir, "*.csv")
 
+    erroneous_files = []
+
     try:
         if len(csv) == 0:
             raise const.IsmnFileError(
-                "Expected 1 csv file for station, found 0. "
-                "Use empty static metadata.")
+                f"Expected 1 csv file but got 0 for station {stat_dir}. "
+                "Continue with empty static metadata instead.")
         else:
             if len(csv) > 1:
-                infos.append(
-                    f"Expected 1 csv file for station, found {len(csv)}. "
+                logger.warning(
+                    f"Expected 1 csv file but got {len(csv)} for "
+                    f"station {stat_dir}. "
                     f"Use first file in dir.")
             static_meta_file = StaticMetaFile(
                 root, csv[0], load_metadata=True, temp_root=temp_root)
             station_meta = static_meta_file.metadata
     except const.IsmnFileError as e:
-        infos.append(f"Error loading static meta for station: {e}")
+        logger.warning(f"Error loading static meta file: {stat_dir}/{csv[0]}. "
+                       f"We will use the placeholder metadata here. "
+                       f"Error traceback: {traceback.format_exc()}")
         station_meta = MetaData(
-            [MetaVar(k, v) for k, v in const.CSV_META_TEMPLATE.items()])
+            [MetaVar(k, v) for k, v in const.CSV_META_TEMPLATE.items()]
+        )
+        erroneous_files.append(os.path.join(str(root), str(csv[0])))
 
     data_files = root.find_files(stat_dir, "*.stm")
 
     filelist = []
 
     for file_path in data_files:
         try:
             f = DataFile(root, file_path, temp_root=temp_root)
         except Exception as e:
-            infos.append(f"Error loading ismn file: {e}")
+            logger.error(f"Error loading ismn file {file_path}. "
+                         f"We will skip this file, it might be malformed. "
+                         f"Error traceback: {traceback.format_exc()}")
+            erroneous_files.append(file_path)
+
             continue
 
         f.metadata.merge(station_meta, inplace=True, exclude_empty=False)
 
         f.metadata = f.metadata.best_meta_for_depth(
             Depth(
                 f.metadata["instrument"].depth.start,
@@ -107,20 +119,20 @@
                     f.metadata.merge(cmeta, inplace=True)
 
         network = f.metadata["network"].val
         station = f.metadata["station"].val
 
         filelist.append((network, station, f))
 
-        infos.append(f"Processed file {file_path}")
+        logger.info(f"Processed file {file_path}")
 
     if proc_root:
         root.close()
 
-    return filelist, infos
+    return filelist, erroneous_files
 
 
 def _load_metadata_df(meta_csv_file: Union[str, Path]) -> pd.DataFrame:
     """
     Load metadata data frame from csv file
     """
 
@@ -221,102 +233,90 @@
         if isinstance(data_root, IsmnRoot):
             root = data_root
         else:
             root = IsmnRoot(data_root)
 
         os.makedirs(temp_root, exist_ok=True)
 
-        if log_path is not None:
-            log_file = os.path.join(log_path, f"{root.name}.log")
-        else:
-            log_file = None
-
-        if log_file:
-            os.makedirs(os.path.dirname(log_file), exist_ok=True)
-            logging.basicConfig(
-                filename=log_file,
-                level=logging.INFO,
-                format="%(levelname)s %(asctime)s %(message)s",
-                datefmt="%Y-%m-%d %H:%M:%S",
-            )
+        log_filename = f"{root.name}.log"
 
-        n_proc = 1 if not parallel else cpu_count()
+        n_proc = 1 if not parallel else os.cpu_count()
 
-        logging.info(f"Collecting metadata with {n_proc} processes.")
+        ismnlog.info(f"Collecting metadata with {n_proc} processes.")
 
         if not parallel:
             hint = 'Hint: Use `parallel=True` to speed up metadata ' \
                    'generation for large datasets'
         else:
             hint = ''
 
         print(
-            f"Processing metadata for all ismn stations into folder "
+            f"Collecting metadata for all ismn stations in archive "
             f"{root.path}.\n"
             f"This may take a few minutes, but is only done once...\n{hint}"
         )
 
         process_stat_dirs = []
         for net_dir, stat_dirs in root.cont.items():
             process_stat_dirs += list(stat_dirs)
 
-        args = [(root.path if root.zip else root, d, temp_root,
-                 custom_meta_readers) for d in process_stat_dirs]
-
-        pbar = tqdm(total=len(args), desc="Files Processed")
-
-        fl_elements = []
+        STATIC_KWARGS = {
+            'root': root.path if root.zip else root,
+            'temp_root': temp_root,
+            'custom_meta_reader': custom_meta_readers,
+        }
+
+        ITER_KWARGS = {
+            'stat_dir': process_stat_dirs
+        }
+
+        res = parallel_process_async(
+            _read_station_dir, ITER_KWARGS=ITER_KWARGS,
+            STATIC_KWARGS=STATIC_KWARGS,
+            n_proc=n_proc, show_progress_bars=True,
+            ignore_errors=True, log_path=log_path,
+            log_filename=log_filename, logger_name='ismn_meta_collector',
+            loglevel='INFO', progress_bar_label="Stations Processed",
+            backend='loky', verbose=False,
+        )
 
-        def update(r):
-            net_stat_fh, infos = r
-            for i in infos:
-                logging.info(i)
-            for elements in net_stat_fh:
-                fl_elements.append(elements)
-            pbar.update()
-
-        def error(e):
-            logging.error(e)
-            pbar.update()
-
-        if n_proc == 1:
-            for arg in args:
-                try:
-                    r = _read_station_dir(*arg)
-                    update(r)
-                except Exception as e:
-                    error(e)
-        else:
-            with Pool(n_proc) as pool:
-                for arg in args:
-                    pool.apply_async(
-                        _read_station_dir,
-                        arg,
-                        callback=update,
-                        error_callback=error,
-                    )
-                pool.close()
-                pool.join()
+        elements = []
+        errors = []
+        for r in res:
+            elements += r[0]
+            if len(r[1]) > 0:
+                errors += r[1]
 
-        pbar.close()
+        elements.sort(key=itemgetter(0, 1))  # sort by net name, stat name
 
-        fl_elements.sort(key=itemgetter(0, 1))  # sort by net name, stat name
-        # to ensure alphabetical order... not sure if necessary, slow?
         filelist = OrderedDict([])
-        for net, stat, fh in fl_elements:
+        for net, stat, fh in elements:
             if net not in filelist.keys():
                 filelist[net] = []
             filelist[net].append(fh)
 
         t1 = time.time()
-        info = f"Metadata generation finished after {int(t1-t0)} Seconds."
-        if log_file is not None:
-            info += f"\nMetadata and Log stored in {os.path.dirname(log_file)}"
+        info = f"Metadata collection finished after {int(t1-t0)} Seconds."
+        if log_path is not None:
+            info += (f"\nMetadata for this archive and "
+                     f"Logfile stored in {log_path}")
+
+        if len(errors) > 0:
+            info += (f"\nNOTE: {len(errors)} potentially malformed file(s) "
+                     f"found during metadata collection. These files will be "
+                     f"ignored by the reader. "
+                     f"Affected files and errors are listed in: "
+                     f"{os.path.join(log_path, log_filename)}.")
+
+            with open(os.path.join(log_path, log_filename), mode='a') as f:
+                f.write("\n----- Summary: Erroneous Files -----\n")
+                f.writelines(errors)
+                f.write("\n-------------------------------------\n")
 
-        logging.info(info)
+        ismnlog.info(info)
         print(info)
 
         return cls(root, filelist=filelist)
 
     @classmethod
     def from_metadata_df(cls, data_root, metadata_df, temp_root=gettempdir()):
         """
@@ -396,15 +396,18 @@
         temp_root : str or Path, optional (default: gettempdir())
             Temporary folder where extracted data is copied during reading from
             zip archive.
         """
         if network is not None:
             network = np.atleast_1d(network)
 
-        print(f"Found existing ismn metadata in {meta_csv_file}.")
+        print(f"Using the existing ismn metadata in {meta_csv_file} to set "
+              f"up ISMN_Interface. \n"
+              "If there are issues with the data reader, you can remove "
+              "the metadata csv file to repeat metadata collection.")
 
         metadata_df = _load_metadata_df(meta_csv_file)
 
         if network is not None:
             metadata_df = metadata_df[np.isin(metadata_df["network"].values,
                                               network)]
 
@@ -439,15 +442,15 @@
             i += 1
 
         dfs = pd.concat(dfs, axis=0, sort=True)
         cols_end = ["file_path", "file_type"]
 
         dfs = dfs[[c for c in dfs.columns if c[0] not in cols_end] +
                   [c for c in dfs.columns if c[0] in cols_end]]
-        dfs = dfs.fillna(np.nan)
+        dfs = dfs.infer_objects(copy=False).fillna(np.nan)
 
         os.makedirs(Path(os.path.dirname(meta_csv_file)), exist_ok=True)
         dfs.to_csv(meta_csv_file)
 
     def get_filehandler(self, idx):
         """
         Get the nth filehandler in a list of all filehandlers for all networks.
```

### Comparing `ismn-1.4.0/src/ismn/filehandlers.py` & `ismn-1.4.1/src/ismn/filehandlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,28 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
+import traceback
+
 import pandas as pd
 import warnings
 import numpy as np
 from tempfile import gettempdir, TemporaryDirectory
 from pathlib import Path
 from typing import Tuple, Union
 import logging
 
-warnings.simplefilter(action="ignore", category=UserWarning)
+#warnings.simplefilter(action="ignore", category=UserWarning)
 from ismn.base import IsmnRoot
 from ismn import const
-from ismn.const import IsmnFileError
+from ismn.const import IsmnFileError, ismnlog
 from ismn.meta import MetaVar, MetaData, Depth
 
 
 class IsmnFile(object):
     """
     General base class for data and static metadata files (station csv file)
     in ismn archive.
@@ -217,16 +219,16 @@
                      new_name=None) -> np.array:
         """
         Extract a field from the loaded csv metadata
         """
         field_vars = []
 
         if fieldname in data.index:
-            froms = np.atleast_1d(data.loc[fieldname]["depth_from[m]"])
-            tos = np.atleast_1d(data.loc[fieldname]["depth_to[m]"])
+            froms = np.atleast_1d(data.loc[fieldname]["depth_from[m]"]).astype(float)
+            tos = np.atleast_1d(data.loc[fieldname]["depth_to[m]"]).astype(float)
             vals = np.atleast_1d(data.loc[fieldname]["value"])
 
             for d_from, d_to, val in zip(froms, tos, vals):
                 d = Depth(d_from, d_to)
                 name = new_name if new_name is not None else fieldname
                 try:
                     val = float(val)
@@ -240,15 +242,15 @@
     def __read_csv(csvfile: Path) -> pd.DataFrame:
         """Load static metadata data frame from csv"""
         try:
             data = pd.read_csv(csvfile, delimiter=";")
             data.set_index("quantity_name", inplace=True)
         except Exception:
             # set columns manually
-            logging.info("no header: {}".format(csvfile))
+            ismnlog.info("no header: {}".format(csvfile))
             data = pd.read_csv(csvfile, delimiter=";", header=None)
             cols = list(data.columns)
             cols[:len(const.CSV_COLS)] = const.CSV_COLS  # todo: not safe
             data.columns = cols
             data.set_index("quantity_name", inplace=True)
 
         return data
@@ -292,32 +294,32 @@
             if key in lc["quantity_source_name"].values:
                 if key != "insitu":
                     lc_dict[key] = np.int32(lc.loc[lc["quantity_source_name"]
                                                    == key]["value"].values[0])
                 else:
                     lc_dict[key] = lc.loc[lc["quantity_source_name"] ==
                                           key]["value"].values[0]
-                    logging.info(
+                    ismnlog.info(
                         f"insitu land cover classification available: {self.file_path}"
                     )
 
         # read climate classifications
         try:
             cl = data.loc[["climate classification"
                           ]][["value", "quantity_source_name"]]
             for key in cl_dict.keys():
                 if key in cl["quantity_source_name"].values:
                     cl_dict[key] = cl.loc[cl["quantity_source_name"] ==
                                           key]["value"].values[0]
                     if key == "insitu":
-                        logging.info(
+                        ismnlog.info(
                             f"insitu climate classification available: {self.file_path}"
                         )
         except KeyError:
-            logging.info(f"No climate metadata found for {self.file_path}")
+            ismnlog.info(f"No climate metadata found for {self.file_path}")
 
         metavars = [
             MetaVar("lc_2000", lc_dict["CCI_landcover_2000"]),
             MetaVar("lc_2005", lc_dict["CCI_landcover_2005"]),
             MetaVar("lc_2010", lc_dict["CCI_landcover_2010"]),
             MetaVar("lc_insitu", lc_dict["insitu"]),
             MetaVar("climate_KG", cl_dict["koeppen_geiger_2007"]),
@@ -652,34 +654,38 @@
             usecols=usecols,
             skiprows=skiprows,
             parse_dates=[[0, 1]],
             engine="c",
             **kwargs
         ):
             try:
-                return pd.read_csv(
+                df = pd.read_csv(
                     filepath_or_buffer=f,
                     skiprows=skiprows,
                     usecols=usecols,
                     names=names,
-                    parse_dates=parse_dates,
                     engine=engine,
                     **kwargs
                 )
             except pd.errors.ParserError:
-                return pd.read_csv(
+                df = pd.read_csv(
                     filepath_or_buffer=f,
                     skiprows=skiprows,
                     usecols=usecols,
                     names=names,
                     sep=r'\s+',
-                    parse_dates=parse_dates,
                     engine="c",
                     **kwargs
                 )
+            for tup in parse_dates:
+                c = [df.columns[t] for t in tup]
+                df.insert(0, '_'.join(c),
+                          pd.to_datetime(df.pop(c[0]) + ' ' + df.pop(c[1])))
+
+            return df
 
         if self.root.zip:
             with TemporaryDirectory(
                     prefix="ismn", dir=self.temp_root) as tempdir:
                 filename = self.root.extract_file(self.file_path, tempdir)
                 data = readf(filename, **kwargs)
 
@@ -725,29 +731,26 @@
             Compare the sensor depth to metadata that is available in multiple
             depth layers (e.g. static metadata variables). Find the variable
             for which the depth matches best with the sensor depth.
         """
         try:
             headr, scnd, last, fname = self.get_elements_from_file()
         except Exception as e:
-            raise IOError(f"Unknown file format found for: {self.file_path}")
+            raise IOError(f"Unknown file format found for {self.file_path}:"
+                          f"{traceback.format_exc()}")
 
         elements = dict(headr=headr, scnd=scnd, last=last, fname=fname)
 
-        if len(fname) == 5 and len(headr) == 16:
-            self.file_type = "ceop"
-            raise RuntimeError("CEOP format not supported")
-        elif len(headr) == 15 and len(fname) >= 9:
+        if (len(headr) == 15) and (len(headr) == len(scnd)):
             metadata, depth = self.get_metadata_ceop_sep(elements)
             self.file_type = "ceop_sep"
-        elif len(headr) < 14 and len(fname) >= 9:
+        else:
+            # the default / fallback format is header_values
             metadata, depth = self.get_metadata_header_values(elements)
             self.file_type = "header_values"
-        else:
-            raise IOError(f"Unknown file format found for: {self.file_path}")
 
         if best_meta_for_sensor:
             depth = metadata["instrument"].depth
             metadata = metadata.best_meta_for_depth(depth)
 
         self.metadata = metadata
         self.metadata.replace("network",
```

### Comparing `ismn-1.4.0/src/ismn/interface.py` & `ismn-1.4.1/src/ismn/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
+from repurpose.process import parallel_process_async  # keep this import
 import numpy as np
 from pathlib import Path
 from tempfile import gettempdir
 import platform
 import sys
 import pandas as pd
 from collections import OrderedDict
@@ -1016,8 +1017,8 @@
         print("KOEPPEN GEIGER Climate Classification")
         print("-------------------------------------")
         for key in self.climate.keys():
             print("{:4}: {}".format(key, self.climate[key]))
 
     def close_files(self):
         # close all open filehandlers
-        self.__file_collection.close()
+        self.__file_collection.close()
```

### Comparing `ismn-1.4.0/src/ismn/meta.py` & `ismn-1.4.1/src/ismn/meta.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/src/ismn.egg-info/SOURCES.txt` & `ismn-1.4.1/src/ismn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/baseline/test_interface_plotting.png` & `ismn-1.4.1/tests/baseline/test_interface_plotting.png`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_base.py` & `ismn-1.4.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_cli.py` & `ismn-1.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_components.py` & `ismn-1.4.1/tests/test_components.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 This module tests the ISMN components.
 """
 
 import os
 import unittest
 
 import pytest
+import numpy as np
+from datetime import datetime, timedelta
 
 from ismn.components import NetworkCollection, Network, Station, Sensor, Depth
 from pygeogrids.grids import BasicGrid
 from tempfile import TemporaryDirectory
 import json
 
 rpath = os.path.join(os.path.dirname(__file__), "test_data")
@@ -259,14 +261,22 @@
             instrument, variable, d, filehandler=DataFile(root, subpath)
         )
 
         name = "{}_{}_{:1.6f}_{:1.6f}".format(instrument, variable, d.start, d.end)
 
         assert self.sensor.name == name
 
+    def test_sensor_coverage(self):
+        cov = self.sensor.get_coverage()
+        np.testing.assert_almost_equal(cov, 56.752, decimal=3)
+        start = self.sensor.metadata['timerange_from'].val.to_pydatetime()
+        assert self.sensor.get_coverage(start=start-timedelta(days=100)) < cov
+        np.testing.assert_almost_equal(
+            self.sensor.get_coverage(freq='2H'), 113.492, decimal=3)
+
     def test_sensor_attributes(self):
         """
         Test sensor attributes.
         """
         assert self.sensor.instrument == "Cosmic-ray-Probe"
         assert self.sensor.variable == "soil_moisture"
         assert self.sensor.depth == Depth(0, 0.21)
```

### Comparing `ismn-1.4.0/tests/test_custom_meta.py` & `ismn-1.4.1/tests/test_custom_meta.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm` & `ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv` & `ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm` & `ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv` & `ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_sm_0.050000_0.050000_ThetaProbe-ML2X_19500101_20210131.stm` & `ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_sm_0.050000_0.050000_ThetaProbe-ML2X_19500101_20210131.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_static_variables.csv` & `ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/FR_Aqui/fraye/FR-Aqui_FR-Aqui_fraye_static_variables.csv`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809/Metadata.xml` & `ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809/Metadata.xml`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_20170810_20180809.zip` & `ismn-1.4.1/tests/test_data/Data_seperate_files_20170810_20180809.zip`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm` & `ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_sm_0.000000_0.190000_Cosmic-ray-Probe_20170810_20180809.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv` & `ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/ARM-1/COSMOS_COSMOS_ARM-1_static_variables.csv`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm` & `ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_sm_0.000000_0.210000_Cosmic-ray-Probe_20170810_20180809.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv` & `ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/COSMOS/Barrow-ARM/COSMOS_COSMOS_Barrow-ARM_static_variables.csv`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/Data_seperate_files_header_20170810_20180809/Metadata.xml` & `ismn-1.4.1/tests/test_data/Data_seperate_files_header_20170810_20180809/Metadata.xml`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/format_ceop_sep/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm` & `ismn-1.4.1/tests/test_data/format_ceop_sep/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/format_header_values/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm` & `ismn-1.4.1/tests/test_data/format_header_values/SMOSMANIA/SMOSMANIA_SMOSMANIA_Narbonne_sm_0.050000_0.050000_ThetaProbe-ML2X_20070101_20070131.stm`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/zip_archives/ceop/Data_seperate_files_20170810_20180809.zip` & `ismn-1.4.1/tests/test_data/zip_archives/ceop/Data_seperate_files_20170810_20180809.zip`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/zip_archives/format_header_values/Data_SMOSMANIA.zip` & `ismn-1.4.1/tests/test_data/zip_archives/format_header_values/Data_SMOSMANIA.zip`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/zip_archives/header/Data_seperate_files_header_20170810_20180809.zip` & `ismn-1.4.1/tests/test_data/zip_archives/header/Data_seperate_files_header_20170810_20180809.zip`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_data/zip_archives/multinetwork/header_values/Data_header_values.zip` & `ismn-1.4.1/tests/test_data/zip_archives/multinetwork/header_values/Data_header_values.zip`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_depth.py` & `ismn-1.4.1/tests/test_depth.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_filecollection.py` & `ismn-1.4.1/tests/test_filecollection.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_filehandler_data.py` & `ismn-1.4.1/tests/test_filehandler_data.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_filehandler_static.py` & `ismn-1.4.1/tests/test_filehandler_static.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_interface.py` & `ismn-1.4.1/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_meta.py` & `ismn-1.4.1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ismn-1.4.0/tests/test_readers.py` & `ismn-1.4.1/tests/test_readers.py`

 * *Files identical despite different names*

