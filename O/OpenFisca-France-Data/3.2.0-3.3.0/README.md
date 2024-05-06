# Comparing `tmp/openfisca_france_data-3.2.0.tar.gz` & `tmp/openfisca_france_data-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfisca_france_data-3.2.0.tar", last modified: Wed Apr 24 16:18:12 2024, max compression
+gzip compressed data, was "openfisca_france_data-3.3.0.tar", last modified: Mon May  6 11:01:05 2024, max compression
```

## Comparing `openfisca_france_data-3.2.0.tar` & `openfisca_france_data-3.3.0.tar`

### file list

```diff
@@ -1,141 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.585731 openfisca_france_data-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.581731 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-24 16:18:12.000000 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-24 16:18:12.000000 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:18:12.000000 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 16:18:12.000000 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-24 16:18:12.000000 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 16:18:12.000000 openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-24 16:18:12.585731 openfisca_france_data-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.561731 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2019.json
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2020.json
--rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2021.json
--rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2022.json
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2023.json
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/ines/
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/ines/ines_2019.json
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/ines/ines_2020.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/taxipp/
--rw-r--r--   0 runner    (1001) docker     (127)    12991 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/base_survey.py
--rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    24951 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.561731 openfisca_france_data-3.2.0/openfisca_france_data/dads/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/dads/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/dads/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.569731 openfisca_france_data-3.2.0/openfisca_france_data/erfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.573731 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/run_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
--rw-r--r--   0 runner    (1001) docker     (127)    26165 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
--rw-r--r--   0 runner    (1001) docker     (127)    36615 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
--rw-r--r--   0 runner    (1001) docker     (127)    13155 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.573731 openfisca_france_data-3.2.0/openfisca_france_data/erfs/old/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/old/aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)    19168 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/old/datatable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs/scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.573731 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.573731 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15394 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    25444 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
--rw-r--r--   0 runner    (1001) docker     (127)    51170 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
--rw-r--r--   0 runner    (1001) docker     (127)    35145 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/test_case_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.561731 openfisca_france_data-3.2.0/openfisca_france_data/felin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.577731 openfisca_france_data-3.2.0/openfisca_france_data/felin/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/felin/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.577731 openfisca_france_data-3.2.0/openfisca_france_data/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/model/calage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/model/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/model/id_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/model/survey_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.577731 openfisca_france_data-3.2.0/openfisca_france_data/reforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/inversion_directe_salaires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.577731 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/allocations_familiales_imposables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/cesthra_invalidee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/de_net_a_brut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.577731 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/allocations_familiales_imposables.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/cesthra_invalidite.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/landais_piketty_saez.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plf2015.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plf2016.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfr2014.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfrss2014.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/trannoy_wasmer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2015.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2016_ayrault_muet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plfr2014.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/trannoy_wasmer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.581731 openfisca_france_data-3.2.0/openfisca_france_data/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/scripts/build_input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/smic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/surveys.py
--rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/openfisca_france_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-24 16:18:12.585731 openfisca_france_data-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.581731 openfisca_france_data-3.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.565731 openfisca_france_data-3.2.0/tests/erfs_fpr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.581731 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_af.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_al.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_impot_revenu.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_inflation.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_input_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_pivot_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_rebuild_input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_salaire_imposable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:12.581731 openfisca_france_data-3.2.0/tests/erfs_fpr/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/unit/test_get_survey_scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/erfs_fpr/unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/test_fake_survey_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/test_get_baremes_salarie.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-24 16:17:55.000000 openfisca_france_data-3.2.0/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.480200 openfisca_france_data-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    15904 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.476200 openfisca_france_data-3.3.0/OpenFisca_France_Data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-06 11:01:05.000000 openfisca_france_data-3.3.0/OpenFisca_France_Data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-06 11:01:05.000000 openfisca_france_data-3.3.0/OpenFisca_France_Data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:01:05.000000 openfisca_france_data-3.3.0/OpenFisca_France_Data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-06 11:01:05.000000 openfisca_france_data-3.3.0/OpenFisca_France_Data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-06 11:01:05.000000 openfisca_france_data-3.3.0/OpenFisca_France_Data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 11:01:05.000000 openfisca_france_data-3.3.0/OpenFisca_France_Data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-06 11:01:05.480200 openfisca_france_data-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.460200 openfisca_france_data-3.3.0/openfisca_france_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.460200 openfisca_france_data-3.3.0/openfisca_france_data/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.456200 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.460200 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2019.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2020.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2021.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2022.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2023.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.460200 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/ines/
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/ines/ines_2019.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/ines/ines_2020.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.464200 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/taxipp/
+-rw-r--r--   0 runner    (1001) docker     (127)    12991 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.464200 openfisca_france_data-3.3.0/openfisca_france_data/assets/zone_apl_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/zone_apl_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.464200 openfisca_france_data-3.3.0/openfisca_france_data/assets/zone_apl_data/zone_apl/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/base_survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22091 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24951 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.456200 openfisca_france_data-3.3.0/openfisca_france_data/dads/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.464200 openfisca_france_data-3.3.0/openfisca_france_data/dads/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/dads/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.464200 openfisca_france_data-3.3.0/openfisca_france_data/erfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.464200 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26165 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36615 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13155 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.464200 openfisca_france_data-3.3.0/openfisca_france_data/erfs/old/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/old/aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19168 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/old/datatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs/scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.468200 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.468200 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15394 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25444 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51170 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35145 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/test_case_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.468200 openfisca_france_data-3.3.0/openfisca_france_data/felin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/felin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.468200 openfisca_france_data-3.3.0/openfisca_france_data/felin/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/felin/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.468200 openfisca_france_data-3.3.0/openfisca_france_data/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/model/calage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/model/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/model/id_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/model/survey_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.468200 openfisca_france_data-3.3.0/openfisca_france_data/reforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/inversion_directe_salaires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.472200 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/allocations_familiales_imposables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/cesthra_invalidee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/de_net_a_brut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.472200 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/allocations_familiales_imposables.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/cesthra_invalidite.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/landais_piketty_saez.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plf2015.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plf2016.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfr2014.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfrss2014.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/trannoy_wasmer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2015.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2016_ayrault_muet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plfr2014.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/trannoy_wasmer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.472200 openfisca_france_data-3.3.0/openfisca_france_data/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/scripts/build_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/smic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/openfisca_france_data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-06 11:01:05.480200 openfisca_france_data-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.472200 openfisca_france_data-3.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.456200 openfisca_france_data-3.3.0/tests/erfs_fpr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.476200 openfisca_france_data-3.3.0/tests/erfs_fpr/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_af.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_al.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_impot_revenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_input_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_pivot_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_rebuild_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_salaire_imposable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:01:05.476200 openfisca_france_data-3.3.0/tests/erfs_fpr/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/unit/test_get_survey_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/erfs_fpr/unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/test_fake_survey_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/test_get_baremes_salarie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/test_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-06 11:00:48.000000 openfisca_france_data-3.3.0/tests/test_misc.py
```

### Comparing `openfisca_france_data-3.2.0/CHANGELOG.md` & `openfisca_france_data-3.3.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+### 3.3.0 [#251](https://github.com/openfisca/openfisca-france-data/pull/251)
+
+* New features
+  - Introduce testing for income "inversion" (deduce gross from net)
+* Update features
+  - Corrects the inversion functions + extends the inversion of unemployment benefit's taxation
+
 ### 3.2.0 [#255](https://github.com/openfisca/openfisca-france-data/pull/255)
 
 * New features
   - Améliore la construction des variables `contrat_de_travail` et `heures_remunerees_volumes` avec l'erfs_fpr
     - Utilisations des variables `sp00` à `sp12` qui décrivent le statut d'activité sur les douze derniers mois pour prendre en compte la part de travail connue dans l'année
 
 ### 3.1.3 [#254](https://github.com/openfisca/openfisca-france-data/pull/254)
```

### Comparing `openfisca_france_data-3.2.0/CONTRIBUTING.md` & `openfisca_france_data-3.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/LICENSE` & `openfisca_france_data-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/PKG-INFO` & `openfisca_france_data-3.3.0/OpenFisca_France_Data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 3.2.0
+Version: 3.3.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `openfisca_france_data-3.2.0/OpenFisca_France_Data.egg-info/SOURCES.txt` & `openfisca_france_data-3.3.0/OpenFisca_France_Data.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
 openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
 openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
 openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
 openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
 openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
 openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
+openfisca_france_data/felin/__init__.py
 openfisca_france_data/felin/input_data_builder/__init__.py
 openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
 openfisca_france_data/model/__init__.py
 openfisca_france_data/model/base.py
 openfisca_france_data/model/calage.py
 openfisca_france_data/model/common.py
 openfisca_france_data/model/id_variables.py
@@ -92,14 +93,15 @@
 openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/trannoy_wasmer.yaml
 openfisca_france_data/scripts/__init__.py
 openfisca_france_data/scripts/build_input_data.py
 tests/test_aggregate.py
 tests/test_calibration.py
 tests/test_fake_survey_simulation.py
 tests/test_get_baremes_salarie.py
+tests/test_inversion.py
 tests/test_misc.py
 tests/erfs_fpr/integration/test_af.py
 tests/erfs_fpr/integration/test_aggregates.py
 tests/erfs_fpr/integration/test_al.py
 tests/erfs_fpr/integration/test_create_salaire_de_base.py
 tests/erfs_fpr/integration/test_impot_revenu.py
 tests/erfs_fpr/integration/test_inflation.py
```

### Comparing `openfisca_france_data-3.2.0/PKG-INFO` & `openfisca_france_data-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 3.2.0
+Version: 3.3.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `openfisca_france_data-3.2.0/README.md` & `openfisca_france_data-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/__init__.py` & `openfisca_france_data-3.3.0/openfisca_france_data/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/aggregates.py` & `openfisca_france_data-3.3.0/openfisca_france_data/aggregates.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2019.json` & `openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2019.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2020.json` & `openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2020.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2021.json` & `openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2021.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2022.json` & `openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2022.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2023.json` & `openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_2023.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_template.json` & `openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/france_entiere/france_entiere_template.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/ines/ines_2019.json` & `openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/ines/ines_2019.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/ines/ines_2020.json` & `openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/ines/ines_2020.json`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx` & `openfisca_france_data-3.3.0/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py` & `openfisca_france_data-3.3.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/base_survey.py` & `openfisca_france_data-3.3.0/openfisca_france_data/base_survey.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/common.py` & `openfisca_france_data-3.3.0/openfisca_france_data/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     for categorie_salarie, target in target_by_categorie_salarie.items():
         baremes_collection = salarie[categorie_salarie]
         baremes_to_remove = list()
         for name, bareme in baremes_collection._children.items():
             if name not in target:
                 baremes_to_remove.append(name)
 
-        # We split since we cannot remove from dict while iterating
+        # We split since we cannot remove from dict while iterating
         for name in baremes_to_remove:
             del baremes_collection._children[name]
 
     for categorie_salarie, target in target_by_categorie_salarie.items():
         test = set(
             name for name, bareme in salarie[categorie_salarie]._children.items()
             # if isinstance(bareme, MarginalRateTaxScale)
@@ -396,37 +396,52 @@
 
 
 def create_revenus_remplacement_bruts(individus, period, tax_benefit_system):
     assert 'taux_csg_remplacement' in individus
 
     individus.chomage_imposable.fillna(0, inplace = True)
     individus.retraite_imposable.fillna(0, inplace = True)
+    individus.salaire_net.fillna(0, inplace = True)
 
     parameters = tax_benefit_system.get_parameters_at_instant(period.start)
     csg = parameters.prelevements_sociaux.contributions_sociales.csg
     csg_deductible_chomage = csg.remplacement.allocations_chomage.deductible
+    pss = parameters.prelevements_sociaux.pss.plafond_securite_sociale_annuel
+    taux_abattement_csg_chomage = parameters.prelevements_sociaux.contributions_sociales.csg.remplacement.allocations_chomage.deductible.abattement.rates[0]
+    seuil_abattement_csg_chomage = parameters.prelevements_sociaux.contributions_sociales.csg.remplacement.allocations_chomage.deductible.abattement.thresholds[1]
     taux_plein = csg_deductible_chomage.taux_plein
     taux_reduit = csg_deductible_chomage.taux_reduit
     seuil_chomage_net_exoneration = (
         (35 * 52) * smic_horaire_brut[period.start.year]
         * (
             (individus.taux_csg_remplacement == 2) / (1 - taux_reduit)
             + (individus.taux_csg_remplacement >= 3) / (1 - taux_plein)
             )
-        )
+        ) - individus.salaire_net
     exonere_csg_chomage = (
         (individus.taux_csg_remplacement < 2)
         | (individus.chomage_imposable <= seuil_chomage_net_exoneration)
         )
+    taux_csg_chomage = np.where(
+        individus.taux_csg_remplacement < 2,
+        0,
+        (individus.taux_csg_remplacement == 2) * taux_reduit
+        + (individus.taux_csg_remplacement >= 3) * taux_plein
+        )
+    threshold = seuil_abattement_csg_chomage * pss * (1 - (taux_csg_chomage * (1 - taux_abattement_csg_chomage)))
+    base_csg_chomage = np.where(
+        individus.chomage_imposable <= threshold,
+        individus.chomage_imposable * (1 - taux_abattement_csg_chomage) / (1 - (taux_csg_chomage * (1 - taux_abattement_csg_chomage))),
+        (individus.chomage_imposable - seuil_abattement_csg_chomage * taux_abattement_csg_chomage * pss) / (1 - taux_csg_chomage)
+        )
     individus['chomage_brut'] = np.where(
         exonere_csg_chomage,
         individus.chomage_imposable,
-        (individus.taux_csg_remplacement == 2) * individus.chomage_imposable / (1 - taux_reduit)
-        + (individus.taux_csg_remplacement >= 3) * individus.chomage_imposable / (1 - taux_plein)
-        )
+        individus.chomage_imposable + (base_csg_chomage * taux_csg_chomage)
+    )
     assert individus['chomage_brut'].notnull().all()
 
     csg_deductible_retraite = parameters.prelevements_sociaux.contributions_sociales.csg.remplacement.pensions_retraite_invalidite.deductible
     taux_plein = csg_deductible_retraite.taux_plein
     taux_reduit = csg_deductible_retraite.taux_reduit
     if period.start.year >= 2019:
         taux_median = csg_deductible_retraite.taux_median
```

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/comparator.py` & `openfisca_france_data-3.3.0/openfisca_france_data/comparator.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/config.py` & `openfisca_france_data-3.3.0/openfisca_france_data/config.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py` & `openfisca_france_data-3.3.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/__init__.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/__init__.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/base.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/base.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/run_all.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/run_all.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/old/aggregates.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/old/aggregates.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/old/datatable.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/old/datatable.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs/scenario.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs/scenario.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/comparison.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/comparison.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/scenario.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/scenario.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/erfs_fpr/test_case_creation.py` & `openfisca_france_data-3.3.0/openfisca_france_data/erfs_fpr/test_case_creation.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/model/base.py` & `openfisca_france_data-3.3.0/openfisca_france_data/model/base.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/model/calage.py` & `openfisca_france_data-3.3.0/openfisca_france_data/model/calage.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/model/common.py` & `openfisca_france_data-3.3.0/openfisca_france_data/model/common.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/model/id_variables.py` & `openfisca_france_data-3.3.0/openfisca_france_data/model/id_variables.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/model/survey_variables.py` & `openfisca_france_data-3.3.0/openfisca_france_data/model/survey_variables.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/reforms/inversion_directe_salaires.py` & `openfisca_france_data-3.3.0/openfisca_france_data/reforms/inversion_directe_salaires.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/allocations_familiales_imposables.py` & `openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/allocations_familiales_imposables.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/cesthra_invalidee.py` & `openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/cesthra_invalidee.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/de_net_a_brut.py` & `openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/de_net_a_brut.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/landais_piketty_saez.yaml` & `openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/landais_piketty_saez.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfr2014.yaml` & `openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfr2014.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfrss2014.yaml` & `openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/parameters/plfrss2014.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2015.py` & `openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2015.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2016_ayrault_muet.py` & `openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plf2016_ayrault_muet.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plfr2014.py` & `openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/plfr2014.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/reforms/old_openfisca_france_reforms/trannoy_wasmer.py` & `openfisca_france_data-3.3.0/openfisca_france_data/reforms/old_openfisca_france_reforms/trannoy_wasmer.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/scripts/build_input_data.py` & `openfisca_france_data-3.3.0/openfisca_france_data/scripts/build_input_data.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/smic.py` & `openfisca_france_data-3.3.0/openfisca_france_data/smic.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/surveys.py` & `openfisca_france_data-3.3.0/openfisca_france_data/surveys.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/openfisca_france_data/utils.py` & `openfisca_france_data-3.3.0/openfisca_france_data/utils.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/setup.cfg` & `openfisca_france_data-3.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/setup.py` & `openfisca_france_data-3.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name = "OpenFisca-France-Data",
-    version = "3.2.0",
+    version = "3.3.0",
     description = "OpenFisca-France-Data module to work with French survey data",
     long_description = long_description,
     long_description_content_type="text/markdown",
     author = "OpenFisca Team",
     author_email = "contact@openfisca.fr",
     url = "https://github.com/openfisca/openfisca-france-data",
     license = "http://www.fsf.org/licensing/licenses/agpl-3.0.html",
```

### Comparing `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_af.py` & `openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_af.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_aggregates.py` & `openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_al.py` & `openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_al.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py` & `openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_impot_revenu.py` & `openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_impot_revenu.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_inflation.py` & `openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_inflation.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_input_variables.py` & `openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_input_variables.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_pivot_table.py` & `openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_pivot_table.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_rebuild_input_data.py` & `openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_rebuild_input_data.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_rsa.py` & `openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_rsa.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/erfs_fpr/integration/test_salaire_imposable.py` & `openfisca_france_data-3.3.0/tests/erfs_fpr/integration/test_salaire_imposable.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/erfs_fpr/unit/test_get_survey_scenario.py` & `openfisca_france_data-3.3.0/tests/erfs_fpr/unit/test_get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/test_aggregate.py` & `openfisca_france_data-3.3.0/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/test_calibration.py` & `openfisca_france_data-3.3.0/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/test_fake_survey_simulation.py` & `openfisca_france_data-3.3.0/tests/test_fake_survey_simulation.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/test_get_baremes_salarie.py` & `openfisca_france_data-3.3.0/tests/test_get_baremes_salarie.py`

 * *Files identical despite different names*

### Comparing `openfisca_france_data-3.2.0/tests/test_misc.py` & `openfisca_france_data-3.3.0/tests/test_misc.py`

 * *Files identical despite different names*

