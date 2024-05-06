# Comparing `tmp/apex-flow-1.1.6.tar.gz` & `tmp/apex_flow-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apex-flow-1.1.6.tar", last modified: Thu Mar 21 06:59:57 2024, max compression
+gzip compressed data, was "apex_flow-1.2.0.tar", last modified: Mon May  6 09:43:56 2024, max compression
```

## Comparing `apex-flow-1.1.6.tar` & `apex_flow-1.2.0.tar`

### file list

```diff
@@ -1,99 +1,110 @@
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-03-21 06:59:57.953079 apex-flow-1.1.6/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7650 2024-03-06 15:05:37.000000 apex-flow-1.1.6/LICENSE
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    34302 2024-03-21 06:59:57.952958 apex-flow-1.1.6/PKG-INFO
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    33488 2024-03-06 15:05:37.000000 apex-flow-1.1.6/README.md
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-03-21 06:59:57.935330 apex-flow-1.1.6/apex/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3410 2024-03-21 06:58:38.000000 apex-flow-1.1.6/apex/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       88 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/__main__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9453 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/config.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-03-21 06:59:57.937239 apex-flow-1.1.6/apex/core/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/__init__.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-03-21 06:59:57.938613 apex-flow-1.1.6/apex/core/calculator/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9345 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/calculator/ABACUS.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    22873 2024-03-07 06:36:09.000000 apex-flow-1.1.6/apex/core/calculator/Lammps.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3058 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/calculator/Task.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    11354 2024-03-07 02:55:16.000000 apex-flow-1.1.6/apex/core/calculator/VASP.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/calculator/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      863 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/calculator/calculator.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-03-21 06:59:57.939707 apex-flow-1.1.6/apex/core/calculator/lib/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/calculator/lib/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    17276 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/calculator/lib/abacus_scf.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    13626 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/calculator/lib/abacus_utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    17685 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/calculator/lib/lammps_utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    14787 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/calculator/lib/vasp_utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7898 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/common_equi.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9244 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/common_prop.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4024 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/gen_confs.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-03-21 06:59:57.942169 apex-flow-1.1.6/apex/core/lib/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/lib/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2170 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/lib/crys.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1341 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/lib/dispatcher.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     5325 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/lib/lmp.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    46593 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/lib/mfp_eosfit.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4428 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/lib/pwscf.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4322 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/lib/siesta.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7853 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/lib/slab_orientation.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1871 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/lib/trans_tools.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3936 2024-03-07 06:35:40.000000 apex-flow-1.1.6/apex/core/lib/util.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1958 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/lib/utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/mpdb.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-03-21 06:59:57.944708 apex-flow-1.1.6/apex/core/property/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    12267 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/property/EOS.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    12178 2024-03-21 06:58:38.000000 apex-flow-1.1.6/apex/core/property/Elastic.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    27949 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/property/Gamma.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    22051 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/property/Interstitial.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    20814 2024-03-06 15:35:08.000000 apex-flow-1.1.6/apex/core/property/Phonon.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3844 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/property/Property.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    12438 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/property/Surface.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    11232 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/property/Vacancy.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/property/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2250 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/refine.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6439 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/reproduce.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2667 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/core/structure.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6948 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/flow.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3470 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/main.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-03-21 06:59:57.945731 apex-flow-1.1.6/apex/op/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1283 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/op/RunLAMMPS.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/op/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9920 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/op/property_ops.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4560 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/op/relaxation_ops.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      667 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/op/utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2626 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/run_step.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7126 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/submit.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-03-21 06:59:57.946526 apex-flow-1.1.6/apex/superop/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6390 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/superop/PropertyFlow.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7906 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/superop/RelaxationFlow.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     8403 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/superop/SimplePropertySteps.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/superop/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2203 2024-03-06 15:05:37.000000 apex-flow-1.1.6/apex/utils.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-03-21 06:59:57.952538 apex-flow-1.1.6/apex_flow.egg-info/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    34302 2024-03-21 06:59:57.000000 apex-flow-1.1.6/apex_flow.egg-info/PKG-INFO
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2166 2024-03-21 06:59:57.000000 apex-flow-1.1.6/apex_flow.egg-info/SOURCES.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        1 2024-03-21 06:59:57.000000 apex-flow-1.1.6/apex_flow.egg-info/dependency_links.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       44 2024-03-21 06:59:57.000000 apex-flow-1.1.6/apex_flow.egg-info/entry_points.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      159 2024-03-21 06:59:57.000000 apex-flow-1.1.6/apex_flow.egg-info/requires.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       11 2024-03-21 06:59:57.000000 apex-flow-1.1.6/apex_flow.egg-info/top_level.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       38 2024-03-21 06:59:57.953371 apex-flow-1.1.6/setup.cfg
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1100 2024-03-21 06:58:38.000000 apex-flow-1.1.6/setup.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-03-21 06:59:57.952251 apex-flow-1.1.6/tests/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1735 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/context.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9661 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_abacus.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3569 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_abacus_equi.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    13364 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_abacus_property.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3131 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_elastic.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3776 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_eos.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4300 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_gamma.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3960 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_interstitial.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3739 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_lammps.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3488 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_make_prop.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1251 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_mpdb.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6121 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_ops.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2902 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_phonon.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3584 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_refine.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3863 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_surface.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3430 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_vacancy.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6164 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_vasp.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3142 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_vasp_equi.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2503 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_vasp_equi_std.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-06 15:05:37.000000 apex-flow-1.1.6/tests/test_vasp_kspacing.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.064822 apex_flow-1.2.0/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7650 2024-03-02 05:00:30.000000 apex_flow-1.2.0/LICENSE
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-06 09:43:56.064569 apex_flow-1.2.0/PKG-INFO
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    42506 2024-05-06 09:26:48.000000 apex_flow-1.2.0/README.md
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.045407 apex_flow-1.2.0/apex/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3737 2024-04-30 08:46:56.000000 apex_flow-1.2.0/apex/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       88 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/__main__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10185 2024-04-17 09:34:08.000000 apex_flow-1.2.0/apex/archive.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10465 2024-04-24 07:51:37.000000 apex_flow-1.2.0/apex/config.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.047498 apex_flow-1.2.0/apex/core/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/__init__.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.049057 apex_flow-1.2.0/apex/core/calculator/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     9940 2024-04-11 09:05:32.000000 apex_flow-1.2.0/apex/core/calculator/ABACUS.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    21684 2024-04-28 05:07:13.000000 apex_flow-1.2.0/apex/core/calculator/Lammps.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3058 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/calculator/Task.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10665 2024-04-16 13:06:19.000000 apex_flow-1.2.0/apex/core/calculator/VASP.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      147 2024-04-28 05:07:13.000000 apex_flow-1.2.0/apex/core/calculator/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      845 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/calculator/calculator.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.050340 apex_flow-1.2.0/apex/core/calculator/lib/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/calculator/lib/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    17254 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/calculator/lib/abacus_scf.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    14014 2024-04-17 13:27:07.000000 apex_flow-1.2.0/apex/core/calculator/lib/abacus_utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    20281 2024-04-28 05:07:13.000000 apex_flow-1.2.0/apex/core/calculator/lib/lammps_utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    14831 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/calculator/lib/vasp_utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7850 2024-04-11 09:57:42.000000 apex_flow-1.2.0/apex/core/common_equi.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     8282 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/common_prop.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4024 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/gen_confs.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.053355 apex_flow-1.2.0/apex/core/lib/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2059 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/lib/crys.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1699 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/lib/dispatcher.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     5325 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/lmp.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    46593 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/mfp_eosfit.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4428 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/pwscf.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4322 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/siesta.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     8248 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/slab_orientation.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1871 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/trans_tools.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3904 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/lib/util.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2344 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/mpdb.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.056024 apex_flow-1.2.0/apex/core/property/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10390 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/property/EOS.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    11811 2024-04-24 15:53:23.000000 apex_flow-1.2.0/apex/core/property/Elastic.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    27104 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/property/Gamma.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    24024 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/property/Interstitial.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    26343 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/property/Phonon.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3861 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/property/Property.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10716 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/property/Surface.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     9520 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/property/Vacancy.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/property/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2250 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/refine.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     6184 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/reproduce.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2695 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/structure.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.056948 apex_flow-1.2.0/apex/database/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      417 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/database/DatabaseFactory.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3366 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/database/DynamoDB.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2080 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/database/MongoDB.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      533 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/database/StorageBase.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/database/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    13130 2024-04-24 08:51:43.000000 apex_flow-1.2.0/apex/flow.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    24813 2024-04-24 07:51:37.000000 apex_flow-1.2.0/apex/main.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.057641 apex_flow-1.2.0/apex/op/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1311 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/op/RunLAMMPS.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/op/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7535 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/op/property_ops.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     5216 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/op/relaxation_ops.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2622 2024-04-26 16:57:00.000000 apex_flow-1.2.0/apex/report.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.058784 apex_flow-1.2.0/apex/reporter/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    13848 2024-04-26 16:49:10.000000 apex_flow-1.2.0/apex/reporter/DashReportApp.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/reporter/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    18716 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/reporter/property_report.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2909 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/reporter/relaxation_report.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2824 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/step.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10455 2024-04-28 05:07:13.000000 apex_flow-1.2.0/apex/submit.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.059403 apex_flow-1.2.0/apex/superop/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7985 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/superop/RelaxationFlow.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     8409 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/superop/SimplePropertySteps.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/superop/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10133 2024-04-27 08:56:06.000000 apex_flow-1.2.0/apex/utils.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.064218 apex_flow-1.2.0/apex_flow.egg-info/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-06 09:43:56.000000 apex_flow-1.2.0/apex_flow.egg-info/PKG-INFO
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2401 2024-05-06 09:43:56.000000 apex_flow-1.2.0/apex_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        1 2024-05-06 09:43:56.000000 apex_flow-1.2.0/apex_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       44 2024-05-06 09:43:56.000000 apex_flow-1.2.0/apex_flow.egg-info/entry_points.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      182 2024-05-06 09:43:56.000000 apex_flow-1.2.0/apex_flow.egg-info/requires.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       11 2024-05-06 09:43:56.000000 apex_flow-1.2.0/apex_flow.egg-info/top_level.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       38 2024-05-06 09:43:56.064881 apex_flow-1.2.0/setup.cfg
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1145 2024-03-21 06:51:12.000000 apex_flow-1.2.0/setup.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.064019 apex_flow-1.2.0/tests/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1735 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/context.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     9820 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_abacus.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3720 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_abacus_equi.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    13373 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_abacus_property.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3131 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_elastic.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3776 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_eos.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4300 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_gamma.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4017 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_interstitial.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3769 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_lammps.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3488 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_make_prop.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1251 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_mpdb.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     6121 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_ops.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2902 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_phonon.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3584 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_refine.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3863 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_surface.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3430 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_vacancy.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     6164 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_vasp.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3142 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_vasp_equi.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2503 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_vasp_equi_std.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_vasp_kspacing.py
```

### Comparing `apex-flow-1.1.6/LICENSE` & `apex_flow-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/PKG-INFO` & `apex_flow-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apex-flow
-Version: 1.1.6
+Version: 1.2.0
 Summary: Alloy Properties EXplorer using simulations
 Home-page: https://github.com/deepmodeling/APEX.git
 Author: Zhuoyuan Li, Tongqi Wen
 Author-email: zhuoyli@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
@@ -12,87 +12,113 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydflow>=1.7.83
 Requires-Dist: pymatgen>=2023.8.10
 Requires-Dist: pymatgen-analysis-defects>=2023.8.22
 Requires-Dist: dpdata>=0.2.13
 Requires-Dist: dpdispatcher
-Requires-Dist: phonoLAMMPS
 Requires-Dist: phonopy
-Requires-Dist: matplotlib
+Requires-Dist: plotly
+Requires-Dist: dash
+Requires-Dist: dash_bootstrap_components
 Requires-Dist: seekpath
 Requires-Dist: fpop>=0.0.7
 Requires-Dist: boto3
+Requires-Dist: pymongo
 
-# APEX: Alloy Property EXplorer using simulations
+<div style="text-align: center;">
+    <img src="./docs/images/logo.png" style="zoom: 15%;">
+</div>
+
+# APEX: Alloy Property EXplorer
+[![](https://img.shields.io/badge/release-1.2.0-blue.svg)](https://github.com/deepmodeling/APEX)
+
+[APEX](https://github.com/deepmodeling/APEX): Alloy Property EXplorer is a component of the [AI Square](https://aissquare.com/) project that involves the restructuring of the [DP-GEN](https://github.com/deepmodeling/dpgen) `auto_test` module to develop a versatile and extensible Python package for general alloy property calculations. This package enables users to conveniently establish a wide range of cloud-native property-test workflows by utilizing various computational approaches, including LAMMPS, VASP, ABACUS, and others.
+
+## v1.2 Main Features Update
+* Add a `retrieve` sub-command to allow results to be retrieved independently and manually for multiple properties (Remove `Distributor` and `Collector` OP)
+* Support common **dflow operations** with terminal commands
+* Incorporate results `archive` function to both local paths and NoSQL database ([MongoDB](https://www.mongodb.com/) and [DynamoDB](https://aws.amazon.com/cn/dynamodb/))
+* Add a `report` sub-command for quick results visualization and cross-comparison via a front-end APP based on [Dash](https://dash.plotly.com)
+* Support [SeeK-path](https://seekpath.readthedocs.io/en/latest/index.html) for automatic band path search in `phonon` calculations
+* Support eight conventional HCP interstitial configurations for `interstitial` calculations
+* Add four additional **ML** pair styles (`snap`, `gap`, `rann` and `mace`) and an extra `meam-spline` in LAMMPS interation type support
+* Modify the single-step run command from `test` to `do` for improved clarity and consistencey
+
+## APEX Bohrium App
+[![](https://img.shields.io/badge/APP-BohriumApp-orange.svg)](https://app.bohrium.dp.tech/apex/)
+
+APEX also provides a web-based [Bohrium App](https://app.bohrium.dp.tech/apex/) for rapid and easy alloy property calculations without intensive JSON configuration (Note: one will need a Bohrium account to access this service).
 
-[APEX](https://github.com/deepmodeling/APEX): Alloy Property EXplorer using simulations, is a component of the [AI Square](https://aissquare.com/) project that involves the restructuring of the [DP-Gen](https://github.com/deepmodeling/dpgen) `auto_test` module to develop a versatile and extensible Python package for general alloy property testing. This package enables users to conveniently establish a wide range of property-test workflows by utilizing various computational approaches, including support for LAMMPS, VASP, and ABACUS.
+## How to cite APEX
+[![](https://img.shields.io/badge/DOI-10.48550/arXiv.2404.17330-red.svg)](https://doi.org/10.48550/arXiv.2404.17330)
 
-## New Features Update (v1.0)
-* Enable the calculation of `phonon` spectrum (v1.1.0)
-* Decouple property calculations into individual sub-workflow to facilitate the customization of complex property functions
-* Support one-click parallel submission of multiple workflows
-* Integrate a single step test mode for `run` steps, providing an interaction method similar to `auto_test`
-* Allow users to modify task submission concurrency via `group_size` and `pool_size`
-* Enable users to customize `suffix` of property calculation directory so that multiple tests with identical property templates but different settings can be run within one workflow
-* Refactor and optimize the command line interaction for improved usability
-* Enhance robustness across diverse use scenarios, especially for the local debug mode
+If you use APEX in your research, please cite the following paper for general purpose: 
+
+> Z. Li, T. Wen, Y. Zhang, X. Liu, C. Zhang, A. S. L. S. Pattamatta, X. Gong, B. Ye, H.Wang, L. Zhang, D. J. Srolovitz, An extendable cloud-native alloy property explorer (2024). arXiv:2404.17330.
 
 ## Table of Contents
 
-- [APEX: Alloy Property EXplorer using simulations](#apex-alloy-property-explorer-using-simulations)
-  - [New Features Update (v1.0)](#new-features-update-v10)
+- [APEX: Alloy Property EXplorer](#apex-alloy-property-explorer)
+  - [v1.2 Main Features Update](#v12-main-features-update)
+  - [APEX Bohrium App](#apex-bohrium-app)
+  - [How to cite APEX](#how-to-cite-apex)
   - [Table of Contents](#table-of-contents)
   - [1. Overview](#1-overview)
   - [2. Easy Install](#2-easy-install)
   - [3. User Guide](#3-user-guide)
     - [3.1. Before Submission](#31-before-submission)
       - [3.1.1. Global Setting](#311-global-setting)
       - [3.1.2. Calculation Parameters](#312-calculation-parameters)
         - [3.1.2.1. EOS](#3121-eos)
         - [3.1.2.2. Elastic](#3122-elastic)
         - [3.1.2.3. Surface](#3123-surface)
         - [3.1.2.4. Vacancy](#3124-vacancy)
         - [3.1.2.5. Interstitial](#3125-interstitial)
         - [3.1.2.6. Gamma Line](#3126-gamma-line)
-        - [3.1.2.7. Phonon Spectrum](#3127-phonon-spectrum)
-    - [3.2. Command](#32-command)
+        - [3.1.2.7. Phonon Spectra](#3127-phonon-spectra)
+    - [3.2. Submission](#32-submission)
       - [3.2.1. Workflow Submission](#321-workflow-submission)
-      - [3.2.2. Single-Step Test](#322-single-step-test)
+      - [3.2.2. Workflow Inquiry \& Operations](#322-workflow-inquiry--operations)
+      - [3.2.3. Run Individual Step](#323-run-individual-step)
+    - [3.3. After Submission](#33-after-submission)
+      - [3.3.1. Retrieve Results Manually](#331-retrieve-results-manually)
+      - [3.3.2. Archive Test Results](#332-archive-test-results)
+      - [3.3.3. Results Visualization Report](#333-results-visualization-report)
   - [4. Quick Start](#4-quick-start)
     - [4.1. In the Bohrium](#41-in-the-bohrium)
     - [4.2. In a Local Argo Service](#42-in-a-local-argo-service)
     - [4.3. In a Local Environment](#43-in-a-local-environment)
 
 ## 1. Overview
 
 APEX adopts the functionality of the second-generation `auto_test` for alloy properties calculations and is developed utilizing the [dflow](https://github.com/deepmodeling/dflow) framework. By integrating the benefits of cloud-native workflows, APEX streamlines the intricate procedure of automatically testing various configurations and properties. Owing to its cloud-native characteristic, APEX provides users with a more intuitive and user-friendly interaction, enhancing the overall user experience by eliminating concerns related to process control, task scheduling, observability, and disaster tolerance.
 
 The comprehensive architecture of APEX is demonstrated below:
 
-<div>
-    <img src="./docs/images/apex_demo.png" alt="Fig1" style="zoom: 35%;">
-    <p style='font-size:1.0rem; font-weight:none'>Figure 1. APEX schematic diagram</p>
+<div style="text-align: center;">
+    <img src="./docs/images/flowchart.png" alt="Fig1" style="zoom: 40%;">
+    <p style='font-size:1.0rem; font-weight:none'>Figure 1. Schematic diagram of APEX</p>
 </div>
 
 APEX consists of three types of pre-defined **workflow** that users can submit: `relaxation`, `property`, and `joint`. The `relaxation` and `property` sub-workflow comprise three sequential **steps**: `Make`, `Run`, and `Post`, while the `joint` workflow essentially combines the `relaxation` and `property` workflows into a comprehensive workflow.
 
-The `relaxation` process begins with the initial `POSCAR` supplied by the user, which is used to generate crucial data such as the final relaxed structure and its corresponding energy, forces, and virial tensor. This equilibrium state information is essential for input into the `property` workflow, enabling further calculations of alloy properties. Upon completion, the final results are automatically retrieved and downloaded to the original working directory.
+The `relaxation` process begins with the initial `POSCAR` supplied by the user, which is used to generate critical data such as the final relaxed structure and its corresponding energy, forces, and virial tensor. This equilibrium state information is essential for input into the `property` workflow, enabling further calculations of alloy properties. Upon completion, the final results are automatically retrieved and downloaded to the original working directory.
 
 In both the `relaxation` and `property` workflows, the `Make` step prepares the corresponding computational tasks. These tasks are then transferred to the `Run` step that is responsible for task dispatch, calculation monitoring, and retrieval of completed tasks (implemented through the [DPDispatcher](https://github.com/deepmodeling/dpdispatcher/tree/master) plugin). Upon completion of all tasks, the `Post` step is initiated to collect data and obtain the desired property results.
 
-APEX currently offers computation methods for the following alloy properties:
+APEX currently offers calculation methods for the following alloy properties:
 
 * Equation of State (EOS)
 * Elastic constants
 * Surface energy
 * Interstitial formation energy
 * Vacancy formation energy
 * Generalized stacking fault energy (Gamma line)
-* Phonon spectrum
+* Phonon spectra
 
 Moreover, APEX supports three types of calculators: **LAMMPS** for molecular dynamics simulations, and **VASP** and **ABACUS** for first-principles calculations.
 
 ## 2. Easy Install
 Easy install by
 ```shell
 pip install apex-flow
@@ -120,26 +146,28 @@
 
 * **Basic config**
   | Key words | Data structure | Default | Description |
   | :------------ | ----- | ----- | ------------------- |
   | apex_image_name | String | zhuoy/apex_amd64 | Image for step other than `run`. One can build this Docker image via prepared [Dockerfile](./docs/Dockerfile) |
   | run_image_name | String | None | Image of calculator for `run` step. Use `{calculator}_image_name` to indicate corresponding image for higher priority |
   | run_command | String | None | Shell command for `run` step. Use `{calculator}_run_command` to indicate corresponding command for higher priority |
-  | group_size | Int | 1 | Number of tasks per parallel run group. |
+  | group_size | Int | 1 | Number of tasks per parallel run group |
   | pool_size | Int | 1 | For multi tasks per parallel group, the pool size of multiprocessing pool to handle each task (1 for serial, -1 for infinity) |
   | upload_python_package | Optional[List] | None | Additional python packages required in the container |
-  | debug_pool_workers | Int | 1 | Pool size of parallel tasks running in the debug mode |
+  | debug_pool_workers | Int | 1 | Pool size of parallel tasks running in the debug mode | 
+  | flow_name | String | None | Specify name of workflow to be submitted (default: work path name) |
+  | submit_only | Bool | False | Submit workflow only without automatic result retrieving |
 
 * **Dflow config**
   | Key words | Data structure | Default | Description |
   | :------------ | ----- | ----- | ------------------- |
   | dflow_host | String | https://127.0.0.1:2746 | Url of dflow server |
   | k8s_api_server | String | https://127.0.0.1:2746 | Url of kubernetes API server |
-  | dflow_config | Optional[Dict] | None | Specify more detailed dflow config in a nested dictionary with higher priority (See [dflow document](https://deepmodeling.com/dflow/dflow.html) for more detail). |
-  | dflow_s3_config | Optional[Dict] | None | Specify dflow s3 repository config in a nested dictionary with higher priority (See [dflow document](https://deepmodeling.com/dflow/dflow.html) for more detail). |
+  | dflow_config | Optional[Dict] | None | Specify more detailed dflow config in a nested dictionary with higher priority (See [dflow document](https://deepmodeling.com/dflow/dflow.html) for more detail) |
+  | dflow_s3_config | Optional[Dict] | None | Specify dflow s3 repository config in a nested dictionary with higher priority (See [dflow document](https://deepmodeling.com/dflow/dflow.html) for more detail) |
 
 * **Dispatcher config** (One may refer to [DPDispatcher’s documentation](https://docs.deepmodeling.com/projects/dpdispatcher/en/latest/index.html) for details of the following parameters)
   | Key words | Data structure | Default | Description |
   | :------------ | ----- | ----- | ------------------- |
   | context_type | String | None | Context type to connect to the remote server |
   | batch_type | String | None | System to dispatch tasks |
   | local_root | String | "./" | Local root path |
@@ -262,50 +290,57 @@
   ```
 ##### 3.1.2.1. EOS
   | Key words | Data structure | Example | Description                                               |
   | :------------ | ----- |-----------------------------------------------------------| ------------------- |
   | vol_start | Float | 0.9 | The starting volume related to the equilibrium structure  |
   | vol_end | Float | 1.1 | The maximum volume related to the equilibrium structure   |
   | vol_step | Float | 0.01 | The volume increment related to the equilibrium structure |
+  | vol_abs | Bool | False | Whether to treat vol_start and vol_end as absolute volume, default = False |
 
 ##### 3.1.2.2. Elastic
-  | Key words | Data structure | Example | Description                                         |
-  | :------------ | ----- |-----------------------------------------------------| ------------------- |
-  | norm_deform | Float | 1.1 | The deformation in xx, yy, zz, defaul = 1e-2        |
-  | shear_deform | Float | 0.01 | The deformation in other directions, default = 1e-2 |
+  | Key words    | Data structure | Example | Description                                                                                                                       |
+  |:-------------|----------------|---------|-----------------------------------------------------------------------------------------------------------------------------------|
+  | norm_deform  | Float          | 0.01    | The deformation in xx, yy, zz, defaul = 1e-2                                                                                      |
+  | shear_deform | Float          | 0.01    | The deformation in other directions, default = 1e-2                                                                               |
+  | conventional | Bool           | False   | Whether adopt conventional cell for deformation                                                                                   |
+  | ieee         | Bool           | True    | Whether rotate relaxed structure into IEEE-standard format before deformation ([ref](https://ieeexplore.ieee.org/document/26560)) |
 
 ##### 3.1.2.3. Surface
-  | Key words | Data structure | Example | Description                                                                      |
+  | Key words | Data structure | Example | Description |
   | :------------ | ----- |----------------------------------------------------------------------------------| ------------------- |
-  | min_slab_size | Int | 10 | Minimum size of slab thickness                                                   |
-  | min_vacuum_size | Int | 11 | Minimum size of vacuum width                                                     |
+  | min_slab_size | Int | 10 | Minimum size of slab thickness |
+  | min_vacuum_size | Int | 11 | Minimum size of vacuum width |
   | pert_xz | Float | 0.01 | Perturbation through xz direction used to compute surface energy, default = 0.01 |
-  | max_miller | Int | 2 | The maximum miller index number of surface generated                             |
+  | max_miller | Int | 2 | The maximum miller index number of surface, default = 2 |
 
 ##### 3.1.2.4. Vacancy
   | Key words | Data structure | Example | Description |
   | :------------ | ----- | ----- | ------------------- |
   | supercell | List[Int] | [3, 3, 3] | The supercell to be constructed, default = [1,1,1] |
 
 ##### 3.1.2.5. Interstitial
   | Key words | Data structure | Example | Description |
   | :------------ | ----- | ----- | ------------------- |
   | insert_ele | List[String] | ["Al"] | The element to be inserted |
-  | supercell | List[Int] | [3, 3, 3] | The supercell to be constructed, default =[1,1,1] |
+  | supercell | List[Int] | [3, 3, 3] | The supercell to be constructed, default = [1,1,1] |
   | conf_filters | Dict | "min_dist": 1.5 | Filter out the undesirable configuration |
+  <div>
+      <img src="./docs/images/interstitial_table.png" alt="Fig3" style="zoom: 90%;">
+      <p style='font-size:1.0rem; font-weight:none'> </p>
+  </div>
 
 ##### 3.1.2.6. Gamma Line
-  <div>
+  <div style="text-align: center;">
       <img src="./docs/images/gamma_demo.png" alt="Fig2" style="zoom: 35%;">
       <p style='font-size:1.0rem; font-weight:none'>Figure 2. Schematic diagram of Gamma line calculation</p>
   </div>
 
-The Gamma line (generalized stacking fault energy) function of APEX calculates energy of a series slab structures of specific crystal plane, which displaced in the middle along a slip vector as illustrated in **Figure 2**. In APEX, the slab structrures are defined by a plane miller index and two orthogonal directions (primary and secondary) on the plane. The **slip vector is always along the primary directions** with slip length defined by users or default settings. Thus, by indicating `plane_miller` and the `slip_direction` (AKA, primary direction), a slip system can be defined.
+The Gamma line (generalized stacking fault energy) function of APEX calculates energy of a series slab structures of specific crystal plane, which displaced in the middle along a slip vector as illustrated in **Figure 2**. In APEX, the slab structrures are defined by a plane miller index and two orthogonal directions (primary and secondary) on the plane. The **slip vector is always along the primary directions** with slip length defined by users or default settings. Thus, by indicating `plane_miller` and the `slip_direction` (i.e., primary direction), a slip system can be defined.
 
-For most common slip systems in respect to FCC, BCC and HCP crystal structures, slip direction, secondary direction and default fractional slip lengths are already documented and listed below (users are **strongly advised** to follow those pre-defined slip system, or may need to double-check the generated slab structure, as unexpected results may occur especially for system like HCP):
+For most common slip systems in FCC, BCC and HCP crystal structures, slip direction, secondary direction and default fractional slip lengths are already documented and listed below (users are **strongly advised** to follow those pre-defined slip system, or may need to double-check the generated slab structure, as unexpected results may occur especially for system like HCP):
 * FCC
   | Plane miller index | Slip direction | Secondary direction | Default slip length |
   | :-------- | ----- | ----- | ---- |
   | $(001)$ | $[100]$ | $[010]$ | $a$ |
   | $(110)$ | $[\bar{1}10]$ | $[001]$ | $\sqrt{2}a$ |
   | $(111)$ | $[11\bar{2}]$ | $[\bar{1}10]$ | $\sqrt{6}a$ |
   | $(111)$ | $[\bar{1}\bar{1}2]$ | $[1\bar{1}0]$ | $\sqrt{6}a$ |
@@ -346,15 +381,15 @@
   | :------------ | ----- | ----- | ------------------- |
   | plane_miller | Sequence[Int] | None | Miller index of the target slab |
   | slip_direction | Sequence[Int] | None | Miller index of slip (primary) direction of the slab |
   | slip_length | Int\|Float; Sequence[Int\|Float, Int\|Float, Int\|Float] | Refer to specific slip system as the table shows above, or 1 if not indicated | Slip length along the primary direction with default unit set by users or default setting. As for format of `[x, y, z]`, the length equals to $\sqrt{(xa)^2+(yb)^2+(zc)^2}$ |
   | plane_shift | Int\|Float | 0 | Shift of displacement plane with unit of lattice parameter **$c$** (positive for upwards). This allows creating slip plane within narrowly-spaced planes (see [ref](https://doi.org/10.1016/j.actamat.2016.10.042)). |
   | n_steps | Int | 10 | Number of steps to displace slab along the slip vector  |
   | vacuum_size | Int\|Float | 0 | Thickness of vacuum layer added around the slab with unit of Angstrom |
-  | supercell_size | Sequence[Int, Int, Int] | [1, 1, 5] | Size of generated supper cell based on slab structure |
+  | supercell_size | Sequence[Int, Int, Int] | [1, 1, 5] | Size of generated supercell based on slab structure |
   | add fix | Sequence[Str, Str, Str] | ["true","true","false"] | Whether to add fix position constraint along x, y and z direction during calculation |
 
   Here is an example:
   ```json
   {
 	  "type":            "gamma",
 	  "skip":            true,
@@ -370,59 +405,80 @@
       "vacuum_size": 10,
 	  "add_fix": ["true","true","false"],
       "n_steps":         10
 	}
   ```
   It should be noted that for various crystal structures, **users can further define slip parameters within the respective nested dictionaries, which will be prioritized for adoption**. In the example above, the slip system configuration within the "hcp" dictionary will be utilized.
 
-##### 3.1.2.7. Phonon Spectrum
-This function incorporates part of [dflow-phonon](https://github.com/Chengqian-Zhang/dflow-phonon) codes into APEX to enhance its comprehensiveness. This workflow is facilitated via [Phonopy](https://github.com/phonopy/phonopy), in conjunction with [phonoLAMMPS](https://github.com/abelcarreras/phonolammps) for LAMMPS calculations. 
+##### 3.1.2.7. Phonon Spectra
+This function incorporates part of [dflow-phonon](https://github.com/Chengqian-Zhang/dflow-phonon) codes into APEX to make it more complete. This workflow is realized via [Phonopy](https://github.com/phonopy/phonopy), and [phonoLAMMPS](https://github.com/abelcarreras/phonolammps) for LAMMPS calculation. In APEX, this part includes the [SeeK-path](https://seekpath.readthedocs.io/en/latest/index.html) for automatically high-symmetry points searching for phonon calculation.
 
-**IMPORTANT!!**: it should be noticed that the **phonoLAMMPS** package must be pre-installed in the user's `run_image` to ensure accurate `LAMMPS` calculations for the phonon spectrum.
+**IMPORTANT!!**: it should be noted that the **phonoLAMMPS** package must be pre-installed in the user's `run_image` to ensure accurate `LAMMPS` calculations for the phonon spectra.
 
 Parameters related to `Phonon` calculations are listed below:
   | Key words | Data structure | Default | Description |
   | :------------ | ----- | ----- | ------------------- |
   | primitive | Bool | False | Whether to find primitive lattice structure for phonon calculation |
   | approach | String | "linear" | Specify phonon calculation method when using `VASP`; Two options: 1. "linear" for the *Linear Response Method*, and 2. "displacement" for the *Finite Displacement Method* |
   | supercell_size | Sequence[Int] | [2, 2, 2] | Size of supercell created for calculation |
-  | MESH | Sequence[Int] | None | Define the dimensions of the grid in reciprocal space, which will be utilized for the calculation of phonon frequencies and eigenvectors. For example: [8, 8, 8]; Refer to [Phonopy MESH](http://phonopy.github.io/phonopy/setting-tags.html#mesh-sampling-tags) |
-  | PRIMITIVE_AXES | String | None | To define the basis vectors of a primitive cell with reference to the basis vectors of a conventional cell, facilitating input cell transformation. For example: "0.0 0.5 0.5 0.5 0.0 0.5 0.5 0.5 0.0"; Refer to [Phonopy PRIMITIVE_AXES](http://phonopy.github.io/phonopy/setting-tags.html#primitive-axes-or-primitive-axis) |
-  | BAND | String | None | Indicate band path in reciprocal space as format of [Phonopy BAND](http://phonopy.github.io/phonopy/setting-tags.html#band-and-band-points); For example: "0 0 0 1/2 0 1/2, 1/2 1/2 1 0 0 0 1/2 1/2 1/2" |
+  | MESH | Sequence[Int] | None | Specify the dimensions of the grid in reciprocal space for which the phonon frequencies and eigenvectors are to be calculated. For example: [8, 8, 8]; Refer to [Phonopy MESH](http://phonopy.github.io/phonopy/setting-tags.html#mesh-sampling-tags) |
+  | PRIMITIVE_AXES | String | None | To define the basis vectors of a primitive cell in terms of the basis vectors of a conventional cell for input cell transformation. For example: "0.0 0.5 0.5 0.5 0.0 0.5 0.5 0.5 0.0"; Refer to [Phonopy PRIMITIVE_AXES](http://phonopy.github.io/phonopy/setting-tags.html#primitive-axes-or-primitive-axis) |
+  | BAND | String | None | (Optional) Indicate band path in reciprocal space as format of [Phonopy BAND](http://phonopy.github.io/phonopy/setting-tags.html#band-and-band-points); For example: "0 0 0 1/2 0 1/2, 1/2 1/2 1 0 0 0 1/2 1/2 1/2". If not specified, the [seekpath](https://seekpath.readthedocs.io/en/latest/#) package will be adopted to automatically determine band path according to relaxed structure |
+  | BAND_LABELS | String | None | (Optional) Indication of band path labels for report plot |
   | BAND_POINTS | Int | 51 | Number of sampling points including the path ends |
-  | BAND_CONNECTION | Bool | True | With this option, band connections are estimated from eigenvectors and band structure is drawn by considering band crossings. In sensitive cases, to obtain better band connections, it requires to increase the number of points calculated in band segments by the `BAND_POINTS` tag. |
+  | BAND_CONNECTION | Bool | True | With this option, band connections are estimated from eigenvectors and band structure is drawn considering band crossings. In sensitive cases, to obtain better band connections, it requires to increase number of points calculated in band segments by the `BAND_POINTS` tag |
+  | seekpath_from_original | Bool | False | Whether to re-seek standard primitive cell for relaxed structure for band path via the seekpath package. If True: `seekpath.get_path_orig_cell` will be adopted, else: `seekpath.get_path`. Refer to [seekpath document](https://seekpath.readthedocs.io/en/latest/maindoc.html#k-point-path-for-non-standard-unit-cells) |
+  | seekpath_param | Dict | None | (Optional) Other parameters to be specified for `seekpath.get_path` and `seekpath.get_path`. Refer to [seekpath document](https://seekpath.readthedocs.io/en/latest/maindoc.html#k-point-path-for-non-standard-unit-cells) |
 
-When utilizing `VASP`, you have **two** primary calculation methods at your disposal: the **Linear Response Method** and the **Finite Displacement Method**.
+When utilizing `VASP`, you have **two** primary calculation methods: the **Linear Response Method** and the **Finite Displacement Method**.
 
 The **Linear Response Method** has an edge over the Finite Displacement Method in that it eliminates the need for creating super-cells, thereby offering computational efficiency in certain cases. Additionally, this method is particularly well-suited for systems with anomalous phonon dispersion (like systems with Kohn anomalies), as it can precisely calculate the phonons at the specified points.
 
-On the other hand, the **Finite Displacement Method**'s advantage lies in its versatility; it functions as an add-on compatible with any code, including those beyond the scope of density functional theory. The only requirement is that the external code can compute forces. For instance, ABACUS may lack an implementation of the Linear Response Method, but can effectively utilize the Finite Displacement Method implemented in phonon calculation.
-
+On the other hand, the advantage of **Finite Displacement Method** lies in its versatility; it functions as an add-on compatible with any code, including those beyond the scope of density functional theory. The only requirement is that the external code can compute forces. For instance, ABACUS may lack an implementation of the Linear Response Method, but can effectively utilize the Finite Displacement Method implemented in phonon calculations.
 
-### 3.2. Command
-APEX currently supports two seperate run modes: **workflow submission** (running via dflow) and **single-step test** (running without dflow).
 
+### 3.2. Submission
 #### 3.2.1. Workflow Submission
-APEX will execute a specific dflow workflow upon each invocation of the command in the format: `apex submit [-h] [-c [CONFIG]] [-w WORK [WORK ...]] [-d] [-f {relax,props,joint}] parameter [parameter ...]`. The type of workflow and calculation method will be automatically determined by APEX based on the parameter file provided by the user. Additionally, users can specify the **workflow type**, **configuration JSON file**, and **work directory** through an optional argument (Run `apex submit -h` for help). Here is an example to submit a `joint` workflow:
+APEX will execute a specific dflow workflow upon each invocation of the command in the format: `apex submit [-h] [-c [CONFIG]] [-w WORK [WORK ...]] [-d] [-s] [-f {relax,props,joint}] parameter [parameter ...]`. The type of workflow and calculation method will be automatically determined by APEX based on the parameter file provided by users. Additionally, users can specify the **workflow type**, **configuration JSON file**, and **work directory** through an optional argument (Run `apex submit -h` for further help). Here is an example to submit a `joint` workflow:
 ```shell
 apex submit param_relax.json param_props.json -c ./global_bohrium.json -w 'dp_demo_0?' 'eam_demo'
 ```
-if no config JSON and work directory is specified, `./global.json` and `./` will be passed as default values respectively. 
+if no config JSON (following `-c`) and work directory (following `-w`) is specified, `./global.json` and `./` will be passed as default values respectively.
+
+#### 3.2.2. Workflow Inquiry & Operations
+APEX supports several commonly used `dflow` inquiry and operation commands as listed below:
+- `list`: List all workflows information
+- `get`: Get detailed information of a workflow
+- `getsteps`: Get detailed steps information of a workflow 
+- `getkeys`: Get keys of steps from a workflow
+- `delete`: Delete a workflow
+- `resubmit`: Resubmit a workflow
+- `retry`: Retry a workflow
+- `resume`: Resume a workflow
+- `stop`: Stop a workflow
+- `suspend`: Suspend a workflow
+- `terminate` Terminate a workflow
+  
+Take `stop` as an example (usage: `apex stop [-h] [-i ID] [-w WORK] [-c [CONFIG]]`) user can refer to following three options:
+1. `apex stop`, as running at the target `work_dir`, and apex will inquiry workflow `ID` from `.workflow.log` file under the current path (`config.json` is the default config file)
+2. `apex stop -w ./EAM_Ti -c ./EAM_Ti/config.json` to indicate target `work_dir` to stop
+3. `apex stop -i relax-fe03j4 -c ./config_bohrium.json` to indicate specific workflow `ID` to stop
+   
 
-#### 3.2.2. Single-Step Test
-APEX also provides a **single-step test mode**, which can run `Make` `run` and `Post` step individually under local enviornment. **Please note that one needs to run command under the work directory in this mode.** Users can invoke them by format of `apex test [-h] [-m [MACHINE]] parameter {make_relax,run_relax,post_relax,make_props,run_props,post_props}` (Run `apex test -h` for help). Here is a example to do relaxation in this mode:
+#### 3.2.3. Run Individual Step 
+APEX also provides a **single-step test mode**, which can run `Make` `run` and `Post` step individually under local enviornment. **Please note that one needs to run commands under the work directory in this mode.** User can invoke them by format of `apex run [-h] [-c [CONFIG]] parameter {make_relax,run_relax,post_relax,make_props,run_props,post_props}` (Run `apex run -h` for help). Here is a example to do relaxation in this mode:
 1. Firstly, generate relaxation tasks by
    ```shell
-   apex test param_relax.json make_relax
+   apex do param_relax.json make_relax
    ```
 2. Then dispatch tasks by
    ```shell
-   apex test param_relax.json run_relax -m machine.json
+   apex do param_relax.json run_relax -c machine.json
    ```
-   where `machine.json` is a JSON file to define dispatch method, containing `machine`, `resources`, `task` dictionaries and `run_command` as listed in [DPDispatcher’s documentation](https://docs.deepmodeling.com/projects/dpdispatcher/en/latest/index.html). Here is an example to submit tasks to a [Slurm](https://slurm.schedmd.com) managed remote HPC:
+   where `machine.json` is a JSON file to define dispatch method, containing `machine`, `resources`, `task` dictionaries and `run_command` as listed in [DPDispatcher’s documentation](https://docs.deepmodeling.com/projects/dpdispatcher/en/latest/index.html). Here is an example to submit tasks to a remote HPC managed by [Slurm](https://slurm.schedmd.com):
    ```json
     {
       "run_command": "lmp -i in.lammps -v restart 0",
       "machine": {
           "batch_type": "Slurm",
           "context_type": "SSHContext",
           "local_root" : "./",
@@ -448,19 +504,82 @@
                 "#SBATCH --mem=10G",
                 "#SBATCH --nodes=1",
                 "#SBATCH --time=1-00:00:00"
           ]
       }
     }
    ```
-3. Finally, as all tasks are finished, post process by
+3. Finally, when all tasks are finished, post-process by
    ```shell
-   apex test param_relax.json post_relax
+   apex do param_relax.json post_relax
    ```
-The property test can follow similar approach.
+The property test can follow a similar approach.
+
+### 3.3. After Submission
+
+#### 3.3.1. Retrieve Results Manually
+
+Sometimes when results auto-retrieving fails after workflows finish, you may try to retrieve completed test results manually by the `retrieve` command with a specific workflow `ID` (or target `work_dir`) provided:
+```shell
+apex retrieve [-h] [-i ID] [-w WORK] [-c [CONFIG]]
+```
+where the `WORK` defaults to be `./`, and the `CONFIG` JSON (default: `config.json`) is used to connect to the remote storage. The command usage to similar to [3.2.2. Workflow Inquiry \& Operations](#322-workflow-inquiry--operations)
+
+#### 3.3.2. Archive Test Results
+After completion of each workflow, the results and test parameters of corresponding property will be stored as `json` format automatically under respective work directory named as `all_result.json`. You can also do this manually to update this file based on the latest run by:
+
+```shell
+apex archive [parameter …]
+```
+Argument format of this sub-command is similar to that of `submit` command. Please use `apex archive -h` for complete usage introduction. It should be noticed that each `archive` command will only update property information of those identified as **active** according to the parameter files and indication provided similar to the `submit` mode.
+
+This mode can also archive results to **NoSQL** database. We currently support two types of database client: [MongoDB](https://www.mongodb.com/) and [DynamoDB](https://aws.amazon.com/cn/dynamodb/). Below shows global configuration parameters for two database archive:
+
+  | Key words | Data structure | Default | Description |
+  | :------------ | ----- | ----- | ------------------- |
+  | database_type | String | local | Database type, three choices available: `local` (only archive to local `all_result.json`), `mongodb` and `dynamodb`. One can also indicate this by `-d` within `archive` command |
+  | archive_method | String | sync | Choose from `sync` and `record`. `sync` synchronizes and updates results into same item based on work directory id; `record` records each archived result into a new item with unique timestamp. One can also indicate this by `-m` within `archive` command |
+
+  For `MongoDB`:
+  | Key words | Data structure | Default | Description |
+  | :------------ | ----- | ----- | ------------------- |
+  | mongodb_host | String | localhost | `Mongodb` host |
+  | mongodb_port | Int | 27017 | `Mongodb` port |
+  | mongodb_database | String | apex_results | `Mongodb` database name |
+  | mongodb_collection | String | apex_results | `Mongodb` collection name |
+  | mongodb_config | Dict | None | Complete parameter dictionary for [MongoClient](https://www.mongodb.com/blog/post/introducing-mongoclient) |
+
+  For `DynamoDB`:
+  | Key words | Data structure | Default | Description |
+  | :------------ | ----- | ----- | ------------------- |
+  | dynamodb_table_name | String | apex_results | `Dynamodb` table name |
+  | dynamodb_config | Dict | None | Complete parameter dictionary for [boto3 session](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/session.html#boto3.session.Session.resource) |
+
+#### 3.3.3. Results Visualization Report
+Note that this mode **only** runs on computer with **interactive UI** frontend. 
+In this mode, APEX will create a comprehensive and interactive results visualization report according to `all_result.json` within indicated work directories. This is achieved through [Dash](https://dash.plotly.com) App. You can invoke the report app simply under target work directory by:
+```shell
+apex report
+```
+Or indicate multiple work directories or path of result file in `json` format by `-w` for cross-comparison. Here is an example:
+```shell
+apex report -w DP/all_result.json ./MEAM_00*
+```
+Once the report app is opened (or manully via http://127.0.0.1:8050/), users can select configurations and property types. Then the corresponding result plot and data table will be shown accordingly.
+**NOTE**:
+- If two Dash pages are automatically opened in your browser, you can close the first one.
+- If the clipboard buttons do not function well, try to reload the page once.
+- Do not over-refresh the page as duplicate errors may occur. Should this occur, stop the server and re-execute the apex report command.
+  <div style="text-align: center;">
+      <img src="./docs/images/reporter_ui.png" alt="Fig3" style="zoom: 50%;">
+      <p style='font-size:1.0rem; font-weight:none'>Figure 3. Demonstration of APEX Results Visualization Report </p>
+  </div>
+
+
+
 ## 4. Quick Start
 We present several case studies as introductory illustrations of APEX, tailored to distinct user scenarios. For our demonstration, we will utilize a [LAMMPS_example](./examples/lammps_demo) to compute the Equation of State (EOS) and elastic constants of molybdenum in both Body-Centered Cubic (BCC) and Face-Centered Cubic (FCC) phases. To begin, we will examine the files prepared within the working directory for this specific case.
 
 ```
 lammps_demo
 ├── confs
 │   ├── std-bcc
@@ -473,27 +592,27 @@
 ├── param_joint.json
 ├── param_props.json
 └── param_relax.json
 ```
 There are three types of parameter files and two types of global config files, as well as a Deep Potential file of molybdenum `frozen_model.pb`. Under the directory of `confs`, structure file `POSCAR` of both phases have been prepared respectively.
 
 ### 4.1. In the Bohrium
-The most efficient method for submitting an APEX workflow is through the preconfigured execution environment of dflow on the [Bohrium platform](https://bohrium.dp.tech). To do this, it may be necessary to create an account on Bohrium. Below is an example of a global.json file for this approach.
+The most efficient method for submitting an APEX workflow is through the preconfigured execution environment of dflow in the [Bohrium platform](https://bohrium.dp.tech). To do this, it may be necessary to create an account on Bohrium. Below is an example of a global.json file for this approach.
 
 ```json
 {
     "dflow_host": "https://workflows.deepmodeling.com",
     "k8s_api_server": "https://workflows.deepmodeling.com",
     "batch_type": "Bohrium",
     "context_type": "Bohrium",
     "email": "YOUR_EMAIL",
     "password": "YOUR_PASSWD",
     "program_id": 1234,
-    "apex_image_name":"registry.dp.tech/dptech/prod-11045/apex-dependencies:1.1.0",
-    "lammps_image_name": "registry.dp.tech/dptech/prod-11461/phonopy:v1.2",
+    "apex_image_name":"registry.dp.tech/dptech/prod-11045/apex-dependency:1.2.0",
+    "lammps_image_name": "registry.dp.tech/dptech/prod-11045/deepmdkit-phonolammps:2.1.1",
     "lammps_run_command":"lmp -in in.lammps",
     "scass_type":"c8_m31_1 * NVIDIA T4"
 }
 ```
 Then, one can submit a relaxation workflow via:
 ```shell
 apex submit param_relax.json -c global_bohrium.json
```

### Comparing `apex-flow-1.1.6/README.md` & `apex_flow-1.2.0/apex_flow.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,124 @@
-# APEX: Alloy Property EXplorer using simulations
+Metadata-Version: 2.1
+Name: apex-flow
+Version: 1.2.0
+Summary: Alloy Properties EXplorer using simulations
+Home-page: https://github.com/deepmodeling/APEX.git
+Author: Zhuoyuan Li, Tongqi Wen
+Author-email: zhuoyli@outlook.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pydflow>=1.7.83
+Requires-Dist: pymatgen>=2023.8.10
+Requires-Dist: pymatgen-analysis-defects>=2023.8.22
+Requires-Dist: dpdata>=0.2.13
+Requires-Dist: dpdispatcher
+Requires-Dist: phonopy
+Requires-Dist: plotly
+Requires-Dist: dash
+Requires-Dist: dash_bootstrap_components
+Requires-Dist: seekpath
+Requires-Dist: fpop>=0.0.7
+Requires-Dist: boto3
+Requires-Dist: pymongo
 
-[APEX](https://github.com/deepmodeling/APEX): Alloy Property EXplorer using simulations, is a component of the [AI Square](https://aissquare.com/) project that involves the restructuring of the [DP-Gen](https://github.com/deepmodeling/dpgen) `auto_test` module to develop a versatile and extensible Python package for general alloy property testing. This package enables users to conveniently establish a wide range of property-test workflows by utilizing various computational approaches, including support for LAMMPS, VASP, and ABACUS.
+<div style="text-align: center;">
+    <img src="./docs/images/logo.png" style="zoom: 15%;">
+</div>
+
+# APEX: Alloy Property EXplorer
+[![](https://img.shields.io/badge/release-1.2.0-blue.svg)](https://github.com/deepmodeling/APEX)
+
+[APEX](https://github.com/deepmodeling/APEX): Alloy Property EXplorer is a component of the [AI Square](https://aissquare.com/) project that involves the restructuring of the [DP-GEN](https://github.com/deepmodeling/dpgen) `auto_test` module to develop a versatile and extensible Python package for general alloy property calculations. This package enables users to conveniently establish a wide range of cloud-native property-test workflows by utilizing various computational approaches, including LAMMPS, VASP, ABACUS, and others.
+
+## v1.2 Main Features Update
+* Add a `retrieve` sub-command to allow results to be retrieved independently and manually for multiple properties (Remove `Distributor` and `Collector` OP)
+* Support common **dflow operations** with terminal commands
+* Incorporate results `archive` function to both local paths and NoSQL database ([MongoDB](https://www.mongodb.com/) and [DynamoDB](https://aws.amazon.com/cn/dynamodb/))
+* Add a `report` sub-command for quick results visualization and cross-comparison via a front-end APP based on [Dash](https://dash.plotly.com)
+* Support [SeeK-path](https://seekpath.readthedocs.io/en/latest/index.html) for automatic band path search in `phonon` calculations
+* Support eight conventional HCP interstitial configurations for `interstitial` calculations
+* Add four additional **ML** pair styles (`snap`, `gap`, `rann` and `mace`) and an extra `meam-spline` in LAMMPS interation type support
+* Modify the single-step run command from `test` to `do` for improved clarity and consistencey
+
+## APEX Bohrium App
+[![](https://img.shields.io/badge/APP-BohriumApp-orange.svg)](https://app.bohrium.dp.tech/apex/)
+
+APEX also provides a web-based [Bohrium App](https://app.bohrium.dp.tech/apex/) for rapid and easy alloy property calculations without intensive JSON configuration (Note: one will need a Bohrium account to access this service).
 
-## New Features Update (v1.0)
-* Enable the calculation of `phonon` spectrum (v1.1.0)
-* Decouple property calculations into individual sub-workflow to facilitate the customization of complex property functions
-* Support one-click parallel submission of multiple workflows
-* Integrate a single step test mode for `run` steps, providing an interaction method similar to `auto_test`
-* Allow users to modify task submission concurrency via `group_size` and `pool_size`
-* Enable users to customize `suffix` of property calculation directory so that multiple tests with identical property templates but different settings can be run within one workflow
-* Refactor and optimize the command line interaction for improved usability
-* Enhance robustness across diverse use scenarios, especially for the local debug mode
+## How to cite APEX
+[![](https://img.shields.io/badge/DOI-10.48550/arXiv.2404.17330-red.svg)](https://doi.org/10.48550/arXiv.2404.17330)
+
+If you use APEX in your research, please cite the following paper for general purpose: 
+
+> Z. Li, T. Wen, Y. Zhang, X. Liu, C. Zhang, A. S. L. S. Pattamatta, X. Gong, B. Ye, H.Wang, L. Zhang, D. J. Srolovitz, An extendable cloud-native alloy property explorer (2024). arXiv:2404.17330.
 
 ## Table of Contents
 
-- [APEX: Alloy Property EXplorer using simulations](#apex-alloy-property-explorer-using-simulations)
-  - [New Features Update (v1.0)](#new-features-update-v10)
+- [APEX: Alloy Property EXplorer](#apex-alloy-property-explorer)
+  - [v1.2 Main Features Update](#v12-main-features-update)
+  - [APEX Bohrium App](#apex-bohrium-app)
+  - [How to cite APEX](#how-to-cite-apex)
   - [Table of Contents](#table-of-contents)
   - [1. Overview](#1-overview)
   - [2. Easy Install](#2-easy-install)
   - [3. User Guide](#3-user-guide)
     - [3.1. Before Submission](#31-before-submission)
       - [3.1.1. Global Setting](#311-global-setting)
       - [3.1.2. Calculation Parameters](#312-calculation-parameters)
         - [3.1.2.1. EOS](#3121-eos)
         - [3.1.2.2. Elastic](#3122-elastic)
         - [3.1.2.3. Surface](#3123-surface)
         - [3.1.2.4. Vacancy](#3124-vacancy)
         - [3.1.2.5. Interstitial](#3125-interstitial)
         - [3.1.2.6. Gamma Line](#3126-gamma-line)
-        - [3.1.2.7. Phonon Spectrum](#3127-phonon-spectrum)
-    - [3.2. Command](#32-command)
+        - [3.1.2.7. Phonon Spectra](#3127-phonon-spectra)
+    - [3.2. Submission](#32-submission)
       - [3.2.1. Workflow Submission](#321-workflow-submission)
-      - [3.2.2. Single-Step Test](#322-single-step-test)
+      - [3.2.2. Workflow Inquiry \& Operations](#322-workflow-inquiry--operations)
+      - [3.2.3. Run Individual Step](#323-run-individual-step)
+    - [3.3. After Submission](#33-after-submission)
+      - [3.3.1. Retrieve Results Manually](#331-retrieve-results-manually)
+      - [3.3.2. Archive Test Results](#332-archive-test-results)
+      - [3.3.3. Results Visualization Report](#333-results-visualization-report)
   - [4. Quick Start](#4-quick-start)
     - [4.1. In the Bohrium](#41-in-the-bohrium)
     - [4.2. In a Local Argo Service](#42-in-a-local-argo-service)
     - [4.3. In a Local Environment](#43-in-a-local-environment)
 
 ## 1. Overview
 
 APEX adopts the functionality of the second-generation `auto_test` for alloy properties calculations and is developed utilizing the [dflow](https://github.com/deepmodeling/dflow) framework. By integrating the benefits of cloud-native workflows, APEX streamlines the intricate procedure of automatically testing various configurations and properties. Owing to its cloud-native characteristic, APEX provides users with a more intuitive and user-friendly interaction, enhancing the overall user experience by eliminating concerns related to process control, task scheduling, observability, and disaster tolerance.
 
 The comprehensive architecture of APEX is demonstrated below:
 
-<div>
-    <img src="./docs/images/apex_demo.png" alt="Fig1" style="zoom: 35%;">
-    <p style='font-size:1.0rem; font-weight:none'>Figure 1. APEX schematic diagram</p>
+<div style="text-align: center;">
+    <img src="./docs/images/flowchart.png" alt="Fig1" style="zoom: 40%;">
+    <p style='font-size:1.0rem; font-weight:none'>Figure 1. Schematic diagram of APEX</p>
 </div>
 
 APEX consists of three types of pre-defined **workflow** that users can submit: `relaxation`, `property`, and `joint`. The `relaxation` and `property` sub-workflow comprise three sequential **steps**: `Make`, `Run`, and `Post`, while the `joint` workflow essentially combines the `relaxation` and `property` workflows into a comprehensive workflow.
 
-The `relaxation` process begins with the initial `POSCAR` supplied by the user, which is used to generate crucial data such as the final relaxed structure and its corresponding energy, forces, and virial tensor. This equilibrium state information is essential for input into the `property` workflow, enabling further calculations of alloy properties. Upon completion, the final results are automatically retrieved and downloaded to the original working directory.
+The `relaxation` process begins with the initial `POSCAR` supplied by the user, which is used to generate critical data such as the final relaxed structure and its corresponding energy, forces, and virial tensor. This equilibrium state information is essential for input into the `property` workflow, enabling further calculations of alloy properties. Upon completion, the final results are automatically retrieved and downloaded to the original working directory.
 
 In both the `relaxation` and `property` workflows, the `Make` step prepares the corresponding computational tasks. These tasks are then transferred to the `Run` step that is responsible for task dispatch, calculation monitoring, and retrieval of completed tasks (implemented through the [DPDispatcher](https://github.com/deepmodeling/dpdispatcher/tree/master) plugin). Upon completion of all tasks, the `Post` step is initiated to collect data and obtain the desired property results.
 
-APEX currently offers computation methods for the following alloy properties:
+APEX currently offers calculation methods for the following alloy properties:
 
 * Equation of State (EOS)
 * Elastic constants
 * Surface energy
 * Interstitial formation energy
 * Vacancy formation energy
 * Generalized stacking fault energy (Gamma line)
-* Phonon spectrum
+* Phonon spectra
 
 Moreover, APEX supports three types of calculators: **LAMMPS** for molecular dynamics simulations, and **VASP** and **ABACUS** for first-principles calculations.
 
 ## 2. Easy Install
 Easy install by
 ```shell
 pip install apex-flow
@@ -95,26 +146,28 @@
 
 * **Basic config**
   | Key words | Data structure | Default | Description |
   | :------------ | ----- | ----- | ------------------- |
   | apex_image_name | String | zhuoy/apex_amd64 | Image for step other than `run`. One can build this Docker image via prepared [Dockerfile](./docs/Dockerfile) |
   | run_image_name | String | None | Image of calculator for `run` step. Use `{calculator}_image_name` to indicate corresponding image for higher priority |
   | run_command | String | None | Shell command for `run` step. Use `{calculator}_run_command` to indicate corresponding command for higher priority |
-  | group_size | Int | 1 | Number of tasks per parallel run group. |
+  | group_size | Int | 1 | Number of tasks per parallel run group |
   | pool_size | Int | 1 | For multi tasks per parallel group, the pool size of multiprocessing pool to handle each task (1 for serial, -1 for infinity) |
   | upload_python_package | Optional[List] | None | Additional python packages required in the container |
-  | debug_pool_workers | Int | 1 | Pool size of parallel tasks running in the debug mode |
+  | debug_pool_workers | Int | 1 | Pool size of parallel tasks running in the debug mode | 
+  | flow_name | String | None | Specify name of workflow to be submitted (default: work path name) |
+  | submit_only | Bool | False | Submit workflow only without automatic result retrieving |
 
 * **Dflow config**
   | Key words | Data structure | Default | Description |
   | :------------ | ----- | ----- | ------------------- |
   | dflow_host | String | https://127.0.0.1:2746 | Url of dflow server |
   | k8s_api_server | String | https://127.0.0.1:2746 | Url of kubernetes API server |
-  | dflow_config | Optional[Dict] | None | Specify more detailed dflow config in a nested dictionary with higher priority (See [dflow document](https://deepmodeling.com/dflow/dflow.html) for more detail). |
-  | dflow_s3_config | Optional[Dict] | None | Specify dflow s3 repository config in a nested dictionary with higher priority (See [dflow document](https://deepmodeling.com/dflow/dflow.html) for more detail). |
+  | dflow_config | Optional[Dict] | None | Specify more detailed dflow config in a nested dictionary with higher priority (See [dflow document](https://deepmodeling.com/dflow/dflow.html) for more detail) |
+  | dflow_s3_config | Optional[Dict] | None | Specify dflow s3 repository config in a nested dictionary with higher priority (See [dflow document](https://deepmodeling.com/dflow/dflow.html) for more detail) |
 
 * **Dispatcher config** (One may refer to [DPDispatcher’s documentation](https://docs.deepmodeling.com/projects/dpdispatcher/en/latest/index.html) for details of the following parameters)
   | Key words | Data structure | Default | Description |
   | :------------ | ----- | ----- | ------------------- |
   | context_type | String | None | Context type to connect to the remote server |
   | batch_type | String | None | System to dispatch tasks |
   | local_root | String | "./" | Local root path |
@@ -237,50 +290,57 @@
   ```
 ##### 3.1.2.1. EOS
   | Key words | Data structure | Example | Description                                               |
   | :------------ | ----- |-----------------------------------------------------------| ------------------- |
   | vol_start | Float | 0.9 | The starting volume related to the equilibrium structure  |
   | vol_end | Float | 1.1 | The maximum volume related to the equilibrium structure   |
   | vol_step | Float | 0.01 | The volume increment related to the equilibrium structure |
+  | vol_abs | Bool | False | Whether to treat vol_start and vol_end as absolute volume, default = False |
 
 ##### 3.1.2.2. Elastic
-  | Key words | Data structure | Example | Description                                         |
-  | :------------ | ----- |-----------------------------------------------------| ------------------- |
-  | norm_deform | Float | 1.1 | The deformation in xx, yy, zz, defaul = 1e-2        |
-  | shear_deform | Float | 0.01 | The deformation in other directions, default = 1e-2 |
+  | Key words    | Data structure | Example | Description                                                                                                                       |
+  |:-------------|----------------|---------|-----------------------------------------------------------------------------------------------------------------------------------|
+  | norm_deform  | Float          | 0.01    | The deformation in xx, yy, zz, defaul = 1e-2                                                                                      |
+  | shear_deform | Float          | 0.01    | The deformation in other directions, default = 1e-2                                                                               |
+  | conventional | Bool           | False   | Whether adopt conventional cell for deformation                                                                                   |
+  | ieee         | Bool           | True    | Whether rotate relaxed structure into IEEE-standard format before deformation ([ref](https://ieeexplore.ieee.org/document/26560)) |
 
 ##### 3.1.2.3. Surface
-  | Key words | Data structure | Example | Description                                                                      |
+  | Key words | Data structure | Example | Description |
   | :------------ | ----- |----------------------------------------------------------------------------------| ------------------- |
-  | min_slab_size | Int | 10 | Minimum size of slab thickness                                                   |
-  | min_vacuum_size | Int | 11 | Minimum size of vacuum width                                                     |
+  | min_slab_size | Int | 10 | Minimum size of slab thickness |
+  | min_vacuum_size | Int | 11 | Minimum size of vacuum width |
   | pert_xz | Float | 0.01 | Perturbation through xz direction used to compute surface energy, default = 0.01 |
-  | max_miller | Int | 2 | The maximum miller index number of surface generated                             |
+  | max_miller | Int | 2 | The maximum miller index number of surface, default = 2 |
 
 ##### 3.1.2.4. Vacancy
   | Key words | Data structure | Example | Description |
   | :------------ | ----- | ----- | ------------------- |
   | supercell | List[Int] | [3, 3, 3] | The supercell to be constructed, default = [1,1,1] |
 
 ##### 3.1.2.5. Interstitial
   | Key words | Data structure | Example | Description |
   | :------------ | ----- | ----- | ------------------- |
   | insert_ele | List[String] | ["Al"] | The element to be inserted |
-  | supercell | List[Int] | [3, 3, 3] | The supercell to be constructed, default =[1,1,1] |
+  | supercell | List[Int] | [3, 3, 3] | The supercell to be constructed, default = [1,1,1] |
   | conf_filters | Dict | "min_dist": 1.5 | Filter out the undesirable configuration |
+  <div>
+      <img src="./docs/images/interstitial_table.png" alt="Fig3" style="zoom: 90%;">
+      <p style='font-size:1.0rem; font-weight:none'> </p>
+  </div>
 
 ##### 3.1.2.6. Gamma Line
-  <div>
+  <div style="text-align: center;">
       <img src="./docs/images/gamma_demo.png" alt="Fig2" style="zoom: 35%;">
       <p style='font-size:1.0rem; font-weight:none'>Figure 2. Schematic diagram of Gamma line calculation</p>
   </div>
 
-The Gamma line (generalized stacking fault energy) function of APEX calculates energy of a series slab structures of specific crystal plane, which displaced in the middle along a slip vector as illustrated in **Figure 2**. In APEX, the slab structrures are defined by a plane miller index and two orthogonal directions (primary and secondary) on the plane. The **slip vector is always along the primary directions** with slip length defined by users or default settings. Thus, by indicating `plane_miller` and the `slip_direction` (AKA, primary direction), a slip system can be defined.
+The Gamma line (generalized stacking fault energy) function of APEX calculates energy of a series slab structures of specific crystal plane, which displaced in the middle along a slip vector as illustrated in **Figure 2**. In APEX, the slab structrures are defined by a plane miller index and two orthogonal directions (primary and secondary) on the plane. The **slip vector is always along the primary directions** with slip length defined by users or default settings. Thus, by indicating `plane_miller` and the `slip_direction` (i.e., primary direction), a slip system can be defined.
 
-For most common slip systems in respect to FCC, BCC and HCP crystal structures, slip direction, secondary direction and default fractional slip lengths are already documented and listed below (users are **strongly advised** to follow those pre-defined slip system, or may need to double-check the generated slab structure, as unexpected results may occur especially for system like HCP):
+For most common slip systems in FCC, BCC and HCP crystal structures, slip direction, secondary direction and default fractional slip lengths are already documented and listed below (users are **strongly advised** to follow those pre-defined slip system, or may need to double-check the generated slab structure, as unexpected results may occur especially for system like HCP):
 * FCC
   | Plane miller index | Slip direction | Secondary direction | Default slip length |
   | :-------- | ----- | ----- | ---- |
   | $(001)$ | $[100]$ | $[010]$ | $a$ |
   | $(110)$ | $[\bar{1}10]$ | $[001]$ | $\sqrt{2}a$ |
   | $(111)$ | $[11\bar{2}]$ | $[\bar{1}10]$ | $\sqrt{6}a$ |
   | $(111)$ | $[\bar{1}\bar{1}2]$ | $[1\bar{1}0]$ | $\sqrt{6}a$ |
@@ -321,15 +381,15 @@
   | :------------ | ----- | ----- | ------------------- |
   | plane_miller | Sequence[Int] | None | Miller index of the target slab |
   | slip_direction | Sequence[Int] | None | Miller index of slip (primary) direction of the slab |
   | slip_length | Int\|Float; Sequence[Int\|Float, Int\|Float, Int\|Float] | Refer to specific slip system as the table shows above, or 1 if not indicated | Slip length along the primary direction with default unit set by users or default setting. As for format of `[x, y, z]`, the length equals to $\sqrt{(xa)^2+(yb)^2+(zc)^2}$ |
   | plane_shift | Int\|Float | 0 | Shift of displacement plane with unit of lattice parameter **$c$** (positive for upwards). This allows creating slip plane within narrowly-spaced planes (see [ref](https://doi.org/10.1016/j.actamat.2016.10.042)). |
   | n_steps | Int | 10 | Number of steps to displace slab along the slip vector  |
   | vacuum_size | Int\|Float | 0 | Thickness of vacuum layer added around the slab with unit of Angstrom |
-  | supercell_size | Sequence[Int, Int, Int] | [1, 1, 5] | Size of generated supper cell based on slab structure |
+  | supercell_size | Sequence[Int, Int, Int] | [1, 1, 5] | Size of generated supercell based on slab structure |
   | add fix | Sequence[Str, Str, Str] | ["true","true","false"] | Whether to add fix position constraint along x, y and z direction during calculation |
 
   Here is an example:
   ```json
   {
 	  "type":            "gamma",
 	  "skip":            true,
@@ -345,59 +405,80 @@
       "vacuum_size": 10,
 	  "add_fix": ["true","true","false"],
       "n_steps":         10
 	}
   ```
   It should be noted that for various crystal structures, **users can further define slip parameters within the respective nested dictionaries, which will be prioritized for adoption**. In the example above, the slip system configuration within the "hcp" dictionary will be utilized.
 
-##### 3.1.2.7. Phonon Spectrum
-This function incorporates part of [dflow-phonon](https://github.com/Chengqian-Zhang/dflow-phonon) codes into APEX to enhance its comprehensiveness. This workflow is facilitated via [Phonopy](https://github.com/phonopy/phonopy), in conjunction with [phonoLAMMPS](https://github.com/abelcarreras/phonolammps) for LAMMPS calculations. 
+##### 3.1.2.7. Phonon Spectra
+This function incorporates part of [dflow-phonon](https://github.com/Chengqian-Zhang/dflow-phonon) codes into APEX to make it more complete. This workflow is realized via [Phonopy](https://github.com/phonopy/phonopy), and [phonoLAMMPS](https://github.com/abelcarreras/phonolammps) for LAMMPS calculation. In APEX, this part includes the [SeeK-path](https://seekpath.readthedocs.io/en/latest/index.html) for automatically high-symmetry points searching for phonon calculation.
 
-**IMPORTANT!!**: it should be noticed that the **phonoLAMMPS** package must be pre-installed in the user's `run_image` to ensure accurate `LAMMPS` calculations for the phonon spectrum.
+**IMPORTANT!!**: it should be noted that the **phonoLAMMPS** package must be pre-installed in the user's `run_image` to ensure accurate `LAMMPS` calculations for the phonon spectra.
 
 Parameters related to `Phonon` calculations are listed below:
   | Key words | Data structure | Default | Description |
   | :------------ | ----- | ----- | ------------------- |
   | primitive | Bool | False | Whether to find primitive lattice structure for phonon calculation |
   | approach | String | "linear" | Specify phonon calculation method when using `VASP`; Two options: 1. "linear" for the *Linear Response Method*, and 2. "displacement" for the *Finite Displacement Method* |
   | supercell_size | Sequence[Int] | [2, 2, 2] | Size of supercell created for calculation |
-  | MESH | Sequence[Int] | None | Define the dimensions of the grid in reciprocal space, which will be utilized for the calculation of phonon frequencies and eigenvectors. For example: [8, 8, 8]; Refer to [Phonopy MESH](http://phonopy.github.io/phonopy/setting-tags.html#mesh-sampling-tags) |
-  | PRIMITIVE_AXES | String | None | To define the basis vectors of a primitive cell with reference to the basis vectors of a conventional cell, facilitating input cell transformation. For example: "0.0 0.5 0.5 0.5 0.0 0.5 0.5 0.5 0.0"; Refer to [Phonopy PRIMITIVE_AXES](http://phonopy.github.io/phonopy/setting-tags.html#primitive-axes-or-primitive-axis) |
-  | BAND | String | None | Indicate band path in reciprocal space as format of [Phonopy BAND](http://phonopy.github.io/phonopy/setting-tags.html#band-and-band-points); For example: "0 0 0 1/2 0 1/2, 1/2 1/2 1 0 0 0 1/2 1/2 1/2" |
+  | MESH | Sequence[Int] | None | Specify the dimensions of the grid in reciprocal space for which the phonon frequencies and eigenvectors are to be calculated. For example: [8, 8, 8]; Refer to [Phonopy MESH](http://phonopy.github.io/phonopy/setting-tags.html#mesh-sampling-tags) |
+  | PRIMITIVE_AXES | String | None | To define the basis vectors of a primitive cell in terms of the basis vectors of a conventional cell for input cell transformation. For example: "0.0 0.5 0.5 0.5 0.0 0.5 0.5 0.5 0.0"; Refer to [Phonopy PRIMITIVE_AXES](http://phonopy.github.io/phonopy/setting-tags.html#primitive-axes-or-primitive-axis) |
+  | BAND | String | None | (Optional) Indicate band path in reciprocal space as format of [Phonopy BAND](http://phonopy.github.io/phonopy/setting-tags.html#band-and-band-points); For example: "0 0 0 1/2 0 1/2, 1/2 1/2 1 0 0 0 1/2 1/2 1/2". If not specified, the [seekpath](https://seekpath.readthedocs.io/en/latest/#) package will be adopted to automatically determine band path according to relaxed structure |
+  | BAND_LABELS | String | None | (Optional) Indication of band path labels for report plot |
   | BAND_POINTS | Int | 51 | Number of sampling points including the path ends |
-  | BAND_CONNECTION | Bool | True | With this option, band connections are estimated from eigenvectors and band structure is drawn by considering band crossings. In sensitive cases, to obtain better band connections, it requires to increase the number of points calculated in band segments by the `BAND_POINTS` tag. |
+  | BAND_CONNECTION | Bool | True | With this option, band connections are estimated from eigenvectors and band structure is drawn considering band crossings. In sensitive cases, to obtain better band connections, it requires to increase number of points calculated in band segments by the `BAND_POINTS` tag |
+  | seekpath_from_original | Bool | False | Whether to re-seek standard primitive cell for relaxed structure for band path via the seekpath package. If True: `seekpath.get_path_orig_cell` will be adopted, else: `seekpath.get_path`. Refer to [seekpath document](https://seekpath.readthedocs.io/en/latest/maindoc.html#k-point-path-for-non-standard-unit-cells) |
+  | seekpath_param | Dict | None | (Optional) Other parameters to be specified for `seekpath.get_path` and `seekpath.get_path`. Refer to [seekpath document](https://seekpath.readthedocs.io/en/latest/maindoc.html#k-point-path-for-non-standard-unit-cells) |
 
-When utilizing `VASP`, you have **two** primary calculation methods at your disposal: the **Linear Response Method** and the **Finite Displacement Method**.
+When utilizing `VASP`, you have **two** primary calculation methods: the **Linear Response Method** and the **Finite Displacement Method**.
 
 The **Linear Response Method** has an edge over the Finite Displacement Method in that it eliminates the need for creating super-cells, thereby offering computational efficiency in certain cases. Additionally, this method is particularly well-suited for systems with anomalous phonon dispersion (like systems with Kohn anomalies), as it can precisely calculate the phonons at the specified points.
 
-On the other hand, the **Finite Displacement Method**'s advantage lies in its versatility; it functions as an add-on compatible with any code, including those beyond the scope of density functional theory. The only requirement is that the external code can compute forces. For instance, ABACUS may lack an implementation of the Linear Response Method, but can effectively utilize the Finite Displacement Method implemented in phonon calculation.
-
+On the other hand, the advantage of **Finite Displacement Method** lies in its versatility; it functions as an add-on compatible with any code, including those beyond the scope of density functional theory. The only requirement is that the external code can compute forces. For instance, ABACUS may lack an implementation of the Linear Response Method, but can effectively utilize the Finite Displacement Method implemented in phonon calculations.
 
-### 3.2. Command
-APEX currently supports two seperate run modes: **workflow submission** (running via dflow) and **single-step test** (running without dflow).
 
+### 3.2. Submission
 #### 3.2.1. Workflow Submission
-APEX will execute a specific dflow workflow upon each invocation of the command in the format: `apex submit [-h] [-c [CONFIG]] [-w WORK [WORK ...]] [-d] [-f {relax,props,joint}] parameter [parameter ...]`. The type of workflow and calculation method will be automatically determined by APEX based on the parameter file provided by the user. Additionally, users can specify the **workflow type**, **configuration JSON file**, and **work directory** through an optional argument (Run `apex submit -h` for help). Here is an example to submit a `joint` workflow:
+APEX will execute a specific dflow workflow upon each invocation of the command in the format: `apex submit [-h] [-c [CONFIG]] [-w WORK [WORK ...]] [-d] [-s] [-f {relax,props,joint}] parameter [parameter ...]`. The type of workflow and calculation method will be automatically determined by APEX based on the parameter file provided by users. Additionally, users can specify the **workflow type**, **configuration JSON file**, and **work directory** through an optional argument (Run `apex submit -h` for further help). Here is an example to submit a `joint` workflow:
 ```shell
 apex submit param_relax.json param_props.json -c ./global_bohrium.json -w 'dp_demo_0?' 'eam_demo'
 ```
-if no config JSON and work directory is specified, `./global.json` and `./` will be passed as default values respectively. 
+if no config JSON (following `-c`) and work directory (following `-w`) is specified, `./global.json` and `./` will be passed as default values respectively.
 
-#### 3.2.2. Single-Step Test
-APEX also provides a **single-step test mode**, which can run `Make` `run` and `Post` step individually under local enviornment. **Please note that one needs to run command under the work directory in this mode.** Users can invoke them by format of `apex test [-h] [-m [MACHINE]] parameter {make_relax,run_relax,post_relax,make_props,run_props,post_props}` (Run `apex test -h` for help). Here is a example to do relaxation in this mode:
+#### 3.2.2. Workflow Inquiry & Operations
+APEX supports several commonly used `dflow` inquiry and operation commands as listed below:
+- `list`: List all workflows information
+- `get`: Get detailed information of a workflow
+- `getsteps`: Get detailed steps information of a workflow 
+- `getkeys`: Get keys of steps from a workflow
+- `delete`: Delete a workflow
+- `resubmit`: Resubmit a workflow
+- `retry`: Retry a workflow
+- `resume`: Resume a workflow
+- `stop`: Stop a workflow
+- `suspend`: Suspend a workflow
+- `terminate` Terminate a workflow
+  
+Take `stop` as an example (usage: `apex stop [-h] [-i ID] [-w WORK] [-c [CONFIG]]`) user can refer to following three options:
+1. `apex stop`, as running at the target `work_dir`, and apex will inquiry workflow `ID` from `.workflow.log` file under the current path (`config.json` is the default config file)
+2. `apex stop -w ./EAM_Ti -c ./EAM_Ti/config.json` to indicate target `work_dir` to stop
+3. `apex stop -i relax-fe03j4 -c ./config_bohrium.json` to indicate specific workflow `ID` to stop
+   
+
+#### 3.2.3. Run Individual Step 
+APEX also provides a **single-step test mode**, which can run `Make` `run` and `Post` step individually under local enviornment. **Please note that one needs to run commands under the work directory in this mode.** User can invoke them by format of `apex run [-h] [-c [CONFIG]] parameter {make_relax,run_relax,post_relax,make_props,run_props,post_props}` (Run `apex run -h` for help). Here is a example to do relaxation in this mode:
 1. Firstly, generate relaxation tasks by
    ```shell
-   apex test param_relax.json make_relax
+   apex do param_relax.json make_relax
    ```
 2. Then dispatch tasks by
    ```shell
-   apex test param_relax.json run_relax -m machine.json
+   apex do param_relax.json run_relax -c machine.json
    ```
-   where `machine.json` is a JSON file to define dispatch method, containing `machine`, `resources`, `task` dictionaries and `run_command` as listed in [DPDispatcher’s documentation](https://docs.deepmodeling.com/projects/dpdispatcher/en/latest/index.html). Here is an example to submit tasks to a [Slurm](https://slurm.schedmd.com) managed remote HPC:
+   where `machine.json` is a JSON file to define dispatch method, containing `machine`, `resources`, `task` dictionaries and `run_command` as listed in [DPDispatcher’s documentation](https://docs.deepmodeling.com/projects/dpdispatcher/en/latest/index.html). Here is an example to submit tasks to a remote HPC managed by [Slurm](https://slurm.schedmd.com):
    ```json
     {
       "run_command": "lmp -i in.lammps -v restart 0",
       "machine": {
           "batch_type": "Slurm",
           "context_type": "SSHContext",
           "local_root" : "./",
@@ -423,19 +504,82 @@
                 "#SBATCH --mem=10G",
                 "#SBATCH --nodes=1",
                 "#SBATCH --time=1-00:00:00"
           ]
       }
     }
    ```
-3. Finally, as all tasks are finished, post process by
+3. Finally, when all tasks are finished, post-process by
    ```shell
-   apex test param_relax.json post_relax
+   apex do param_relax.json post_relax
    ```
-The property test can follow similar approach.
+The property test can follow a similar approach.
+
+### 3.3. After Submission
+
+#### 3.3.1. Retrieve Results Manually
+
+Sometimes when results auto-retrieving fails after workflows finish, you may try to retrieve completed test results manually by the `retrieve` command with a specific workflow `ID` (or target `work_dir`) provided:
+```shell
+apex retrieve [-h] [-i ID] [-w WORK] [-c [CONFIG]]
+```
+where the `WORK` defaults to be `./`, and the `CONFIG` JSON (default: `config.json`) is used to connect to the remote storage. The command usage to similar to [3.2.2. Workflow Inquiry \& Operations](#322-workflow-inquiry--operations)
+
+#### 3.3.2. Archive Test Results
+After completion of each workflow, the results and test parameters of corresponding property will be stored as `json` format automatically under respective work directory named as `all_result.json`. You can also do this manually to update this file based on the latest run by:
+
+```shell
+apex archive [parameter …]
+```
+Argument format of this sub-command is similar to that of `submit` command. Please use `apex archive -h` for complete usage introduction. It should be noticed that each `archive` command will only update property information of those identified as **active** according to the parameter files and indication provided similar to the `submit` mode.
+
+This mode can also archive results to **NoSQL** database. We currently support two types of database client: [MongoDB](https://www.mongodb.com/) and [DynamoDB](https://aws.amazon.com/cn/dynamodb/). Below shows global configuration parameters for two database archive:
+
+  | Key words | Data structure | Default | Description |
+  | :------------ | ----- | ----- | ------------------- |
+  | database_type | String | local | Database type, three choices available: `local` (only archive to local `all_result.json`), `mongodb` and `dynamodb`. One can also indicate this by `-d` within `archive` command |
+  | archive_method | String | sync | Choose from `sync` and `record`. `sync` synchronizes and updates results into same item based on work directory id; `record` records each archived result into a new item with unique timestamp. One can also indicate this by `-m` within `archive` command |
+
+  For `MongoDB`:
+  | Key words | Data structure | Default | Description |
+  | :------------ | ----- | ----- | ------------------- |
+  | mongodb_host | String | localhost | `Mongodb` host |
+  | mongodb_port | Int | 27017 | `Mongodb` port |
+  | mongodb_database | String | apex_results | `Mongodb` database name |
+  | mongodb_collection | String | apex_results | `Mongodb` collection name |
+  | mongodb_config | Dict | None | Complete parameter dictionary for [MongoClient](https://www.mongodb.com/blog/post/introducing-mongoclient) |
+
+  For `DynamoDB`:
+  | Key words | Data structure | Default | Description |
+  | :------------ | ----- | ----- | ------------------- |
+  | dynamodb_table_name | String | apex_results | `Dynamodb` table name |
+  | dynamodb_config | Dict | None | Complete parameter dictionary for [boto3 session](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/session.html#boto3.session.Session.resource) |
+
+#### 3.3.3. Results Visualization Report
+Note that this mode **only** runs on computer with **interactive UI** frontend. 
+In this mode, APEX will create a comprehensive and interactive results visualization report according to `all_result.json` within indicated work directories. This is achieved through [Dash](https://dash.plotly.com) App. You can invoke the report app simply under target work directory by:
+```shell
+apex report
+```
+Or indicate multiple work directories or path of result file in `json` format by `-w` for cross-comparison. Here is an example:
+```shell
+apex report -w DP/all_result.json ./MEAM_00*
+```
+Once the report app is opened (or manully via http://127.0.0.1:8050/), users can select configurations and property types. Then the corresponding result plot and data table will be shown accordingly.
+**NOTE**:
+- If two Dash pages are automatically opened in your browser, you can close the first one.
+- If the clipboard buttons do not function well, try to reload the page once.
+- Do not over-refresh the page as duplicate errors may occur. Should this occur, stop the server and re-execute the apex report command.
+  <div style="text-align: center;">
+      <img src="./docs/images/reporter_ui.png" alt="Fig3" style="zoom: 50%;">
+      <p style='font-size:1.0rem; font-weight:none'>Figure 3. Demonstration of APEX Results Visualization Report </p>
+  </div>
+
+
+
 ## 4. Quick Start
 We present several case studies as introductory illustrations of APEX, tailored to distinct user scenarios. For our demonstration, we will utilize a [LAMMPS_example](./examples/lammps_demo) to compute the Equation of State (EOS) and elastic constants of molybdenum in both Body-Centered Cubic (BCC) and Face-Centered Cubic (FCC) phases. To begin, we will examine the files prepared within the working directory for this specific case.
 
 ```
 lammps_demo
 ├── confs
 │   ├── std-bcc
@@ -448,27 +592,27 @@
 ├── param_joint.json
 ├── param_props.json
 └── param_relax.json
 ```
 There are three types of parameter files and two types of global config files, as well as a Deep Potential file of molybdenum `frozen_model.pb`. Under the directory of `confs`, structure file `POSCAR` of both phases have been prepared respectively.
 
 ### 4.1. In the Bohrium
-The most efficient method for submitting an APEX workflow is through the preconfigured execution environment of dflow on the [Bohrium platform](https://bohrium.dp.tech). To do this, it may be necessary to create an account on Bohrium. Below is an example of a global.json file for this approach.
+The most efficient method for submitting an APEX workflow is through the preconfigured execution environment of dflow in the [Bohrium platform](https://bohrium.dp.tech). To do this, it may be necessary to create an account on Bohrium. Below is an example of a global.json file for this approach.
 
 ```json
 {
     "dflow_host": "https://workflows.deepmodeling.com",
     "k8s_api_server": "https://workflows.deepmodeling.com",
     "batch_type": "Bohrium",
     "context_type": "Bohrium",
     "email": "YOUR_EMAIL",
     "password": "YOUR_PASSWD",
     "program_id": 1234,
-    "apex_image_name":"registry.dp.tech/dptech/prod-11045/apex-dependencies:1.1.0",
-    "lammps_image_name": "registry.dp.tech/dptech/prod-11461/phonopy:v1.2",
+    "apex_image_name":"registry.dp.tech/dptech/prod-11045/apex-dependency:1.2.0",
+    "lammps_image_name": "registry.dp.tech/dptech/prod-11045/deepmdkit-phonolammps:2.1.1",
     "lammps_run_command":"lmp -in in.lammps",
     "scass_type":"c8_m31_1 * NVIDIA T4"
 }
 ```
 Then, one can submit a relaxation workflow via:
 ```shell
 apex submit param_relax.json -c global_bohrium.json
```

### Comparing `apex-flow-1.1.6/apex/__init__.py` & `apex_flow-1.2.0/apex/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-__version__ = '1.1.6'
+__version__ = '1.2.0'
 LOCAL_PATH = os.getcwd()
 
 
 def header():
     header_str = ""
     header_str += "---------------------------------------------------------------\n"
     header_str += "░░░░░░█▐▓▓░████▄▄▄█▀▄▓▓▓▌█░░░░░░░░░░█▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀█░░░░░\n"
@@ -23,9 +23,13 @@
     header_str += "      AAA   AAA       PPP     PPP   EEE            XXX XXX\n"
     header_str += "     AAAAAAAAAAA      PPPPPPPPP     EEEEEEEEE       XXXXX\n"
     header_str += "    AAA       AAA     PPP           EEE            XXX XXX\n"
     header_str += "   AAA         AAA    PPP           EEE           XXX   XXX\n"
     header_str += "  AAA           AAA   PPP           EEEEEEEEEE  XXX       XXX\n"
     header_str += "---------------------------------------------------------------\n"
     header_str += f"==>> Alloy Property EXplorer using simulations (v{__version__})\n"
+    header_str += "Please cite DOI: 10.48550/arXiv.2404.17330\n"
+    header_str += "Li et al, An extendable cloud-native alloy property explorer (2024).\n"
+    header_str += "See https://github.com/deepmodeling/APEX for more information.\n"
+    header_str += "---------------------------------------------------------------\n"
     header_str += "Checking input files..."
     print(header_str)
```

### Comparing `apex-flow-1.1.6/apex/config.py` & `apex_flow-1.2.0/apex/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # dflow config
     dflow_config: dict = None
     dflow_host: str = "https://127.0.0.1:2746"
     k8s_api_server: str = "https://127.0.0.1:2746"
     mode: str = 'default'
     debug_copy_method: str = "copy"
     debug_pool_workers: int = 1
-    debug_workdir: str = '.'
+    debug_workdir: str = None
 
     # dflow s3 config
     dflow_s3_config: dict = None
 
     # Bohrium config
     bohrium_config: dict = None
     phone: str = None
@@ -46,32 +46,48 @@
     local_root: str = '.'
     remote_root: str = None
     remote_host: str = None
     remote_username: str = None
     remote_password: str = None
     port: int = 22
 
-    # calculator config
+    # basic run config
     run_image_name: str = None
     run_command: str = None
     apex_image_name: str = "zhuoyli/apex_amd64"
     group_size: int = None
     pool_size: int = None
     upload_python_packages: list = field(default_factory=list)
-    # lammps
     lammps_image_name: str = None
     lammps_run_command: str = None
-    # vasp
     vasp_image_name: str = None
     vasp_run_command: str = None
-    # abacus
     abacus_image_name: str = None
     abacus_run_command: str = None
 
+    # common APEX config
     is_bohrium_dflow: bool = False
+    submit_only: bool = False
+    flow_name: str = None
+
+    database_type: str = 'local'
+    archive_method: str = 'sync'
+    archive_key: str = None
+    archive_tasks: bool = False
+
+    # MongoDB config
+    mongodb_config: dict = None
+    mongodb_host: str = "localhost"
+    mongodb_port: int = 27017
+    mongodb_database: str = "apex_results"
+    mongodb_collection: str = "default_collection"
+
+    # DynamoDB config
+    dynamodb_config: dict = None
+    dynamodb_table_name: str = "apex_results"
 
     def __post_init__(self):
         # judge if running dflow on the Bohrium
         try:
             assert self.dflow_config["host"] == "https://workflows.deepmodeling.com"
         except (AssertionError, TypeError):
             if self.dflow_host == "https://workflows.deepmodeling.com":
@@ -79,15 +95,15 @@
         else:
             self.is_bohrium_dflow = True
 
         # pre-define machine dictionaries for dpdispatcher
         if not (self.context_type or self.machine):
             self.machine_dict = None
         elif self.context_type in ["Bohrium", "bohrium",
-                                    "BohriumContext", "boriumcontext"]:
+                                   "BohriumContext", "boriumcontext"]:
             self.machine_dict = {
                 "batch_type": self.batch_type,
                 "context_type": self.context_type,
                 "remote_profile": {
                     "email": self.email,
                     "password": self.password,
                     "program_id": self.program_id,
@@ -97,15 +113,15 @@
                         "scass_type": self.scass_type,
                     },
                 },
             }
             if self.machine:
                 update_dict(self.machine_dict, self.machine)
         elif self.context_type in ["SSHContext", "sshcontext",
-                                    "SSH", "ssh"]:
+                                   "SSH", "ssh"]:
             self.machine_dict = {
                 "batch_type": self.batch_type,
                 "context_type": self.context_type,
                 "local_root": self.local_root,
                 "remote_root": self.remote_root,
                 "clean_asynchronously": self.clean_asynchronously,
                 "remote_profile": {
@@ -115,26 +131,26 @@
                     "port": self.port,
                     "timeout": 10
                 }
             }
             if self.machine:
                 update_dict(self.machine_dict, self.machine)
         elif self.context_type in ["LocalContext", "localcontext"
-                                    "Local", "local"]:
+                                                   "Local", "local"]:
             self.machine_dict = {
                 "batch_type": self.batch_type,
                 "context_type": self.context_type,
                 "local_root": self.local_root,
                 "remote_root": self.remote_root,
                 "clean_asynchronously": self.clean_asynchronously
             }
             if self.machine:
                 update_dict(self.machine_dict, self.machine)
         elif self.context_type in ["LazyLocalContext", "lazylocalcontext"
-                                    "LazyLocal", "lazylocal"]:
+                                                       "LazyLocal", "lazylocal"]:
             self.machine_dict = {
                 "batch_type": self.batch_type,
                 "context_type": self.context_type,
                 "local_root": self.local_root,
                 "clean_asynchronously": self.clean_asynchronously
             }
             if self.machine:
@@ -201,14 +217,31 @@
             "remote_command": self.dispatcher_remote_command
         }
         if self.dispatcher_config:
             update_dict(dispatcher_config, self.dispatcher_config)
         return dispatcher_config
 
     @property
+    def mongodb_config_dict(self):
+        mongodb_config = {
+            "host": self.mongodb_host,
+            "port": self.mongodb_port
+        }
+        if self.mongodb_config:
+            update_dict(mongodb_config, self.mongodb_config)
+        return mongodb_config
+
+    @property
+    def dynamodb_config_dict(self):
+        dynamodb_config = {}
+        if self.mongodb_config:
+            update_dict(dynamodb_config, self.dynamodb_config)
+        return dynamodb_config
+
+    @property
     def basic_config_dict(self):
         basic_config = {
             "run_image_name": self.run_image_name,
             "run_command": self.run_command,
             "apex_image_name": self.apex_image_name,
             "group_size": self.group_size,
             "pool_size": self.pool_size,
```

### Comparing `apex-flow-1.1.6/apex/core/calculator/ABACUS.py` & `apex_flow-1.2.0/apex/core/calculator/ABACUS.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import logging
 
+import dpdata
 from dpdata import LabeledSystem
 from monty.serialization import dumpfn
 
 from apex.core.calculator.lib import abacus_utils, abacus_scf
-#from dpgen import dlog
 from apex.core.calculator.Task import Task
 from apex.utils import sepline
 from dflow.python import upload_packages
 upload_packages.append(__file__)
 
 
 class ABACUS(Task):
@@ -18,54 +18,61 @@
         self.inter_type = inter_parameter["type"]
         self.incar = inter_parameter.get("incar", {})
         self.potcar_prefix = inter_parameter.get("potcar_prefix", "")
         self.potcars = inter_parameter.get("potcars", None)
         self.orbfile = inter_parameter.get("orb_files", None)
         self.deepks = inter_parameter.get("deepks_desc", None)
         self.path_to_poscar = path_to_poscar
-        self.if_define_orb_file = False if self.orbfile == None else True
+        self.if_define_orb_file = False if self.orbfile is None else True
 
     def make_potential_files(self, output_dir):
         stru = os.path.abspath(os.path.join(output_dir, "STRU"))
+        poscar = os.path.abspath(os.path.join(output_dir, "POSCAR"))
         if not os.path.isfile(stru):
-            raise FileNotFoundError("No file %s" % stru)
+            logging.warning(msg='No STRU found...')
+            if os.path.isfile(poscar):
+                logging.info(msg=f'will convert {poscar} into STRU...')
+                sys = dpdata.System(poscar, fmt="vasp/poscar")
+                sys.to("abacus/stru", stru)
+            else:
+                raise FileNotFoundError("No file %s" % stru)
         stru_data = abacus_scf.get_abacus_STRU(stru)
         atom_names = stru_data["atom_names"]
         orb_files = stru_data["orb_files"]
         pp_files = stru_data["pp_files"]
         dpks_descriptor = stru_data["dpks_descriptor"]
 
         if os.path.islink(os.path.join(output_dir, "STRU")):
             stru_path, tmpf = os.path.split(
                 os.readlink(os.path.join(output_dir, "STRU"))
             )
         else:
             stru_path = output_dir
 
-        if pp_files == None:
+        if pp_files is None:
             raise RuntimeError("No pseudopotential information in STRU file")
 
         pp_dir = os.path.abspath(self.potcar_prefix)
         cwd = os.getcwd()
         os.chdir(output_dir)
         if not os.path.isdir("./pp_orb"):
             os.mkdir("./pp_orb")
         for i in range(len(atom_names)):
             pp_orb_file = [[pp_files[i], self.potcars]]
-            if orb_files != None:
+            if orb_files is not None:
                 pp_orb_file.append([orb_files[i], self.orbfile])
-            elif self.orbfile != None:
+            elif self.orbfile is not None:
                 assert atom_names[i] in self.orbfile, (
                     "orb_file of %s is not defined" % atom_names[i]
                 )
                 pp_orb_file.append([self.orbfile[atom_names[i]], self.orbfile])
 
-            if dpks_descriptor != None:
+            if dpks_descriptor is not None:
                 pp_orb_file.append([dpks_descriptor[i], self.deepks])
-            elif self.deepks != None:
+            elif self.deepks is not None:
                 pp_orb_file.append([self.deepks, self.deepks])
 
             for tmpf, tmpdict in pp_orb_file:
                 atom = atom_names[i]
                 if os.path.isfile(os.path.join(stru_path, tmpf)):
                     linked_file = os.path.join(stru_path, tmpf)
                 elif tmpdict != None and os.path.isfile(
@@ -197,14 +204,18 @@
         abacus_utils.write_kpt(os.path.join(output_dir, "KPT"), kpt)
 
     def compute(self, output_dir):
         if not os.path.isfile(os.path.join(output_dir, "INPUT")):
             logging.warning("cannot find INPUT in " + output_dir + " skip")
             return None
         ls = LabeledSystem(output_dir, fmt="abacus/relax")
+        stru_name = abacus_utils.final_stru(output_dir)
+        stru_path = os.path.join(output_dir, stru_name)
+        stru = dpdata.System(stru_path, fmt="stru")
+        stru.to("contcar", os.path.join(output_dir, "CONTCAR"))
         outcar_dict = ls.as_dict()
         return outcar_dict
 
     def forward_files(self, property_type="relaxation"):
         return ["INPUT", "STRU", "KPT", "pp_orb"]
 
     def forward_common_files(self, property_type="relaxation"):
```

### Comparing `apex-flow-1.1.6/apex/core/calculator/Task.py` & `apex_flow-1.2.0/apex/core/calculator/Task.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/apex/core/calculator/VASP.py` & `apex_flow-1.2.0/apex/core/calculator/VASP.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 
 from dpdata import LabeledSystem
 from monty.serialization import dumpfn
 from pymatgen.core.structure import Structure
 from pymatgen.io.vasp import Incar, Kpoints
 
-#from dpgen import dlog
 from apex.core.calculator.Task import Task
 from apex.core.calculator.lib import vasp_utils
 from apex.core.calculator.lib.vasp_utils import incar_upper
 from apex.utils import sepline
 from dflow.python import upload_packages
 upload_packages.append(__file__)
 
@@ -21,98 +20,85 @@
         self.inter_type = inter_parameter["type"]
         self.incar = inter_parameter["incar"]
         self.potcar_prefix = inter_parameter.get("potcar_prefix", "")
         self.potcars = inter_parameter["potcars"]
         self.path_to_poscar = path_to_poscar
 
     def make_potential_files(self, output_dir):
-        potcar_not_link_list = ["vacancy", "interstitial"]
+        potcar_not_link_list = {"vacancy", "interstitial"}
         task_type = output_dir.split("/")[-2].split("_")[0]
 
-        ele_pot_list = [key for key in self.potcars.keys()]
         poscar = os.path.abspath(os.path.join(output_dir, "POSCAR"))
         pos_str = Structure.from_file(poscar)
-        ele_pos_list_tmp = list(ii.as_dict()["element"] for ii in pos_str.species)
+        ele_pos_list_tmp = [ii.as_dict()["element"] for ii in pos_str.species]
 
         ele_pos_list = [ele_pos_list_tmp[0]]
         for ii in range(1, len(ele_pos_list_tmp)):
             if not ele_pos_list_tmp[ii] == ele_pos_list_tmp[ii - 1]:
                 ele_pos_list.append(ele_pos_list_tmp[ii])
 
+        def write_potcar(ele_list, potcar_path):
+            with open(potcar_path, "w") as fp:
+                for element in ele_list:
+                    potcar_file = os.path.join(self.potcar_prefix, self.potcars[element])
+                    with open(potcar_file,"r") as fc:
+                        fp.write(fc.read())
+        
         if task_type in potcar_not_link_list:
-            with open(os.path.join(output_dir, "POTCAR"), "w") as fp:
-                for ii in ele_pos_list:
-                    for jj in ele_pot_list:
-                        if ii == jj:
-                            with open(
-                                os.path.join(self.potcar_prefix, self.potcars[jj]), "r"
-                            ) as fin:
-                                for line in fin:
-                                    print(line.strip("\n"), file=fp)
-
+            write_potcar(ele_pos_list, output_dir+"/POTCAR")
         else:
-            if not os.path.isfile(os.path.join(output_dir, "../POTCAR")):
-                with open(os.path.join(output_dir, "../POTCAR"), "w") as fp:
-                    for ii in ele_pos_list:
-                        for jj in ele_pot_list:
-                            if ii == jj:
-                                with open(
-                                    os.path.join(self.potcar_prefix, self.potcars[jj]),
-                                    "r",
-                                ) as fin:
-                                    for line in fin:
-                                        print(line.strip("\n"), file=fp)
-            cwd = os.getcwd()
-            os.chdir(output_dir)
-            if not os.path.islink("POTCAR"):
-                os.symlink("../POTCAR", "POTCAR")
-            elif not "../POTCAR" == os.readlink("POTCAR"):
-                os.remove("POTCAR")
-                os.symlink("../POTCAR", "POTCAR")
-            os.chdir(cwd)
-
-        dumpfn(self.inter, os.path.join(output_dir, "inter.json"), indent=4)
+            potcar_path = output_dir+"/../POTCAR"
+            if not os.path.exists(potcar_path):
+                write_potcar(ele_pos_list, potcar_path)
+            potcar_link = output_dir+"/POTCAR"
+            if not os.path.islink(potcar_link) or "../POTCAR" != os.readlink(potcar_path):
+                if os.path.exists(potcar_link):
+                    os.remove(potcar_link)
+                os.symlink("../POTCAR", potcar_link)
+            
+        dumpfn(self.inter, output_dir+"/inter.json", indent=4)
 
     def make_input_file(self, output_dir, task_type, task_param):
         sepline(ch=output_dir)
         dumpfn(task_param, os.path.join(output_dir, "task.json"), indent=4)
 
         assert os.path.exists(self.incar), "no INCAR file for relaxation"
         relax_incar_path = os.path.abspath(self.incar)
         incar_relax = incar_upper(Incar.from_file(relax_incar_path))
 
         # deal with relaxation
         prop_type = task_param.get("type", "relaxation")
         cal_type = task_param["cal_type"]
         cal_setting = task_param["cal_setting"]
 
-        # user input INCAR for apex calculation
+        # user input INCAR for APEX calculation
         if "input_prop" in cal_setting and os.path.isfile(cal_setting["input_prop"]):
             incar_prop = os.path.abspath(cal_setting["input_prop"])
             incar = incar_upper(Incar.from_file(incar_prop))
             logging.info(f"Will use user specified INCAR (path: {incar_prop}) for {prop_type} calculation")
 
         # revise INCAR based on the INCAR provided in the "interaction"
         else:
             if prop_type == "phonon":
                 approach = task_param.get("approach", "linear")
-                logging.info(f"No specification of INCAR for {prop_type} calculation, will auto generate")
+                logging.info(f"No specification of INCAR for {prop_type} calculation, will auto-generate")
                 if approach == "linear":
                     incar = incar_upper(Incar.from_str(
                         vasp_utils.make_vasp_phonon_dfpt_incar(
                             ecut=650, ediff=0.0000001, npar=None, kpar=None, kspacing=0.1
                         )))
                 elif approach == "displacement":
                     incar = incar_upper(Incar.from_str(
                         vasp_utils.make_vasp_static_incar(
                             ecut=650, ediff=0.0000001, ismear=0, sigma=0.01, npar=8, kpar=1, kspacing=0.1
                         )))
+
             else:
                 if not prop_type == "relaxation":
-                    logging.info(f"No specification of INCAR for {prop_type} calculation, will use INCAR for relaxation")
+                    logging.info(f"No specification of INCAR for {prop_type} calculation, will use INCAR in relaxation")
                 incar = incar_relax
 
             if cal_type == "relaxation":
                 relax_pos = cal_setting["relax_pos"]
                 relax_shape = cal_setting["relax_shape"]
                 relax_vol = cal_setting["relax_vol"]
                 if [relax_pos, relax_shape, relax_vol] == [True, False, False]:
@@ -187,69 +173,66 @@
             if "kgamma" in cal_setting:
                 logging.info(
                     "%s setting KGAMMA to %s"
                     % (self.make_input_file.__name__, cal_setting["kgamma"])
                 )
                 incar["KGAMMA"] = cal_setting["kgamma"]
 
-        try:
-            kspacing = incar.get("KSPACING")
-        except KeyError:
+        kspacing = incar.get("KSPACING", None)
+        if kspacing is None:
             raise RuntimeError("KSPACING must be given in INCAR")
+        kgamma = incar.get("KGAMMA", False)
 
-        if "KGAMMA" in incar:
-            kgamma = incar.get("KGAMMA")
-        else:
-            kgamma = False
+        self._write_incar_and_kpoints(incar, output_dir, kspacing, kgamma)
 
+    def _write_incar_and_kpoints(self, incar, output_dir, kspacing, kgamma):
         incar.write_file(os.path.join(output_dir, "../INCAR"))
-        cwd = os.getcwd()
-        os.chdir(output_dir)
-        if not os.path.islink("INCAR"):
-            os.symlink("../INCAR", "INCAR")
-        elif not "../INCAR" == os.readlink("INCAR"):
-            os.remove("INCAR")
-            os.symlink("../INCAR", "INCAR")
-        os.chdir(cwd)
+        self._link_file("../INCAR", os.path.join(output_dir, "INCAR"))
         ret = vasp_utils.make_kspacing_kpoints(self.path_to_poscar, kspacing, kgamma)
-        kp = Kpoints.from_str(ret)
-        kp.write_file(os.path.join(output_dir, "KPOINTS"))
+        Kpoints.from_str(ret).write_file(os.path.join(output_dir, "KPOINTS"))
+    
+    def _link_file(self, target, link_name):
+        if not os.path.islink(link_name):
+            os.symlink(target, link_name)
+        elif os.readlink(link_name) != target:
+            os.remove(link_name)
+            os.symlink(target, link_name)
 
     def compute(self, output_dir):
         outcar = os.path.join(output_dir, "OUTCAR")
         if not os.path.isfile(outcar):
             logging.warning("cannot find OUTCAR in " + output_dir + " skip")
             return None
-        else:
-            ls = LabeledSystem(outcar)
-            stress = []
-            with open(outcar, "r") as fin:
-                lines = fin.read().split("\n")
-            for line in lines:
-                if "in kB" in line:
-                    stress_xx = float(line.split()[2])
-                    stress_yy = float(line.split()[3])
-                    stress_zz = float(line.split()[4])
-                    stress_xy = float(line.split()[5])
-                    stress_yz = float(line.split()[6])
-                    stress_zx = float(line.split()[7])
-                    stress.append([])
-                    stress[-1].append([stress_xx, stress_xy, stress_zx])
-                    stress[-1].append([stress_xy, stress_yy, stress_yz])
-                    stress[-1].append([stress_zx, stress_yz, stress_zz])
-
-            outcar_dict = ls.as_dict()
-            outcar_dict["data"]["stress"] = {
-                "@module": "numpy",
-                "@class": "array",
-                "dtype": "float64",
-                "data": stress,
-            }
+        
+        stress = []
+        with open(outcar, "r") as fin:
+            lines = fin.read().split("\n")
+        for line in lines:
+            if "in kB" in line:
+                stress_xx = float(line.split()[2])
+                stress_yy = float(line.split()[3])
+                stress_zz = float(line.split()[4])
+                stress_xy = float(line.split()[5])
+                stress_yz = float(line.split()[6])
+                stress_zx = float(line.split()[7])
+                stress.append([])
+                stress[-1].append([stress_xx, stress_xy, stress_zx])
+                stress[-1].append([stress_xy, stress_yy, stress_yz])
+                stress[-1].append([stress_zx, stress_yz, stress_zz])
+
+        ls = LabeledSystem(outcar)
+        outcar_dict = ls.as_dict()
+        outcar_dict["data"]["stress"] = {
+            "@module": "numpy",
+            "@class": "array",
+            "dtype": "float64",
+            "data": stress,
+        }
 
-            return outcar_dict
+        return outcar_dict
 
     def forward_files(self, property_type="relaxation"):
         return ["INCAR", "POSCAR", "KPOINTS", "POTCAR"]
 
     def forward_common_files(self, property_type="relaxation"):
         potcar_not_link_list = ["vacancy", "interstitial"]
         if property_type == "elastic":
```

### Comparing `apex-flow-1.1.6/apex/core/calculator/calculator.py` & `apex_flow-1.2.0/apex/core/calculator/calculator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from apex.core.calculator.ABACUS import ABACUS
 from apex.core.calculator.Lammps import Lammps
 from apex.core.calculator.VASP import VASP
 from dflow.python import upload_packages
+from . import LAMMPS_INTER_TYPE
 upload_packages.append(__file__)
 
-LAMMPS_TYPE = ["deepmd", "meam", "eam_fs", "eam_alloy"]
 
 def make_calculator(inter_parameter, path_to_poscar):
     """
     Make an instance of Task
     """
     inter_type = inter_parameter["type"]
     if inter_type == "vasp":
         return VASP(inter_parameter, path_to_poscar)
     elif inter_type == "abacus":
         return ABACUS(inter_parameter, path_to_poscar)
-    elif inter_type in LAMMPS_TYPE:
+    elif inter_type in LAMMPS_INTER_TYPE:
         return Lammps(inter_parameter, path_to_poscar)
     #    if inter_type == 'siesta':
     #        return Siesta(inter_parameter, path_to_poscar)
     #        pass
     else:
         raise RuntimeError(f"unsupported interaction {inter_type}")
```

### Comparing `apex-flow-1.1.6/apex/core/calculator/lib/abacus_scf.py` & `apex_flow-1.2.0/apex/core/calculator/lib/abacus_scf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 upload_packages.append(__file__)
 
 bohr2ang = 0.52917721067
 
 
 def make_abacus_scf_kpt(fp_params):
     # Make KPT file for abacus pw scf calculation.
-    # KPT file is the file containing k points infomation in ABACUS scf calculation.
+    # KPT file is the file containing k points information in ABACUS scf calculation.
     k_points = [1, 1, 1, 0, 0, 0]
     if "k_points" in fp_params:
         k_points = fp_params["k_points"]
         if len(k_points) != 6:
             raise RuntimeError(
-                "k_points has to be a list containig 6 integers specifying MP k points generation."
+                "k_points has to be a list containing 6 integers specifying MP k points generation."
             )
     ret = "K_POINTS\n0\nGamma\n"
     for i in range(6):
         ret += str(k_points[i]) + " "
     return ret
 
 
@@ -78,15 +78,15 @@
                 "broyden",
             ]
             ret += "mixing_type %s\n" % fp_params["mixing_type"]
         elif key == "mixing_beta":
             exam_float.check({"mixing_beta": fp_params["mixing_beta"]})
             #fp_params["mixing_beta"] = float(fp_params["mixing_beta"])
             assert (
-                fp_params["mixing_beta"] >= 0 and fp_params["mixing_beta"] < 1
+                    0 <= fp_params["mixing_beta"] < 1
             ), "'mixing_beta' should between 0 and 1."
             ret += "mixing_beta %f\n" % fp_params["mixing_beta"]
         elif key == "symmetry":
             if type(fp_params["symmetry"]) == str:
                 fp_params["symmetry"] = int(eval(fp_params["symmetry"]))
             assert (
                 fp_params["symmetry"] == 0 or fp_params["symmetry"] == 1
@@ -102,25 +102,25 @@
         elif key == "nspin":
             exam_int.check({"nspin": fp_params["nspin"]})
             #fp_params["nspin"] = int(fp_params["nspin"])
             assert (
                 fp_params["nspin"] == 1
                 or fp_params["nspin"] == 2
                 or fp_params["nspin"] == 4
-            ), "'nspin' can anly take 1, 2 or 4"
+            ), "'nspin' can only take 1, 2 or 4"
             ret += "nspin %d\n" % fp_params["nspin"]
         elif key == "ks_solver":
             assert fp_params["ks_solver"] in [
                 "cg",
                 "dav",
                 "lapack",
                 "genelpa",
                 "hpseps",
                 "scalapack_gvx",
-            ], "'ks_sover' should in 'cgx', 'dav', 'lapack', 'genelpa', 'hpseps', 'scalapack_gvx'."
+            ], "'ks_solver' should in 'cgx', 'dav', 'lapack', 'genelpa', 'hpseps', 'scalapack_gvx'."
             ret += "ks_solver %s\n" % fp_params["ks_solver"]
         elif key == "smearing_method":
             assert fp_params["smearing_method"] in [
                 "gauss",
                 "gaussian",
                 "fd",
                 "fixed",
@@ -194,15 +194,15 @@
     fp_orb_files=None,
     fp_dpks_descriptor=None,
     fp_params=None,
     type_map=None,
 ):
     atom_names = sys_data["atom_names"]
     atom_numbs = sys_data["atom_numbs"]
-    if type_map == None:
+    if type_map is None:
         type_map = atom_names
 
     assert len(atom_names) == len(atom_numbs), "Please check the name of atoms. "
     cell = sys_data["cells"].reshape([3, 3])
     coord = sys_data["coords"].reshape([sum(atom_numbs), 3])
     # volume = np.linalg.det(cell)
     # lattice_const = np.power(volume, 1/3)
```

### Comparing `apex-flow-1.1.6/apex/core/calculator/lib/abacus_utils.py` & `apex_flow-1.2.0/apex/core/calculator/lib/abacus_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -465,15 +465,16 @@
                     return False
                 elif not fixed and not bool(int(k)):
                     return False
         i += 1
     return True
 
 
-def modify_stru_path(strucf, tpath):
+def modify_stru_path(strucf, tpath, inter):
+    pp_dict = inter["potcars"]
     if tpath[-1] != "/":
         tpath += "/"
     with open(strucf) as f1:
         lines = f1.readlines()
     for i, line in enumerate(lines):
         if "ATOMIC_SPECIES" in line and line.split()[0] == "ATOMIC_SPECIES":
             file_numb = 2
@@ -487,15 +488,24 @@
             continue
 
         for j in range(i + 1, len(lines)):
             if lines[j].strip() in key_words_list:
                 break
             elif lines[j].strip() == "":
                 continue
-            ppfile = tpath + os.path.split(lines[j].split()[file_numb])[1]
+            try:
+                _ = lines[j].split()[file_numb]
+            except IndexError:
+                line_split = lines[j].split()
+                ele_name = line_split[0]
+                pp_name = pp_dict[ele_name]
+                line_split.append(pp_name)
+                lines[j] = " ".join(line_split) + "\n"
+            finally:
+                ppfile = tpath + os.path.split(lines[j].split()[file_numb])[1]
             tmp_line = ""
             for k in range(file_numb):
                 tmp_line += lines[j].split()[k] + " "
             lines[j] = tmp_line + ppfile + "\n"
 
     with open(strucf, "w") as f1:
         f1.writelines(lines)
```

### Comparing `apex-flow-1.1.6/apex/core/calculator/lib/lammps_utils.py` & `apex_flow-1.2.0/apex/core/calculator/lib/lammps_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from dflow.python import upload_packages
 upload_packages.append(__file__)
 
 
 def cvt_lammps_conf(fin, fout, type_map, ofmt="lammps/data"):
     """
     Format convert from fin to fout, specify the output format by ofmt
-    Imcomplete situation
+    Incomplete situation
     """
     supp_ofmt = ["lammps/dump", "lammps/data", "vasp/poscar"]
     supp_exts = ["dump", "lmp", "poscar/POSCAR"]
 
     if "dump" in fout:
         ofmt = "lammps/dump"
     elif "lmp" in fout:
@@ -105,29 +105,76 @@
 
 
 def inter_deepmd(param):
     models = param["model_name"]
     deepmd_version = param["deepmd_version"]
     ret = "pair_style deepmd "
     model_list = ""
+    type_map_list = [i for i in param["param_type"]]
+    type_map_list_str = " ".join(type_map_list)
     for ii in models:
         model_list += ii + " "
     if Version(deepmd_version) < Version("1"):
         ## DeePMD-kit version == 0.x
         if len(models) > 1:
             ret += "%s 10 model_devi.out\n" % model_list
         else:
             ret += models[0] + "\n"
     else:
         ## DeePMD-kit version >= 1
         if len(models) > 1:
             ret += "%s out_freq 10 out_file model_devi.out\n" % model_list
         else:
             ret += models[0] + "\n"
-    ret += "pair_coeff * *\n"
+    ret += "pair_coeff * * %s\n" % type_map_list_str
+    return ret
+
+
+def inter_mace(param):
+    ret = ""
+    line = "pair_style      mace no_domain_decomposition \n"
+    line += "pair_coeff      * * %s " % param["model_name"][0]
+    for ii in param["param_type"]:
+        line += ii + " "
+    line += "\n"
+    ret += line
+    return ret
+
+
+def inter_snap(param):
+    ret = ""
+    line = "pair_style      snap \n"
+    line += "pair_coeff      * * %s " % param["model_name"][0]
+    line += "%s " % param["model_name"][1]
+    for ii in param["param_type"]:
+        line += ii + " "
+    line += "\n"
+    ret += line
+    return ret
+
+
+def inter_gap(param):
+    ret = ""
+    line = "pair_style      quip \n"
+    line += "pair_coeff      * * %s " % param["model_name"][0]
+    for ii in param["param_type"]:
+        line += ii + " "
+    line += "\n"
+    ret += line
+    return ret
+
+
+def inter_rann(param):
+    ret = ""
+    line = "pair_style      rann \n"
+    line += "pair_coeff      * * %s " % param["model_name"][0]
+    for ii in param["param_type"]:
+        line += ii + " "
+    line += "\n"
+    ret += line
     return ret
 
 
 def inter_meam(param):
     ret = ""
     line = "pair_style      meam \n"
     line += "pair_coeff      * * %s " % param["model_name"][0]
@@ -137,14 +184,25 @@
     for ii in param["param_type"]:
         line += ii + " "
     line += "\n"
     ret += line
     return ret
 
 
+def inter_meam_spline(param):
+    ret = ""
+    line = "pair_style      meam/spline \n"
+    line += "pair_coeff      * * %s " % param["model_name"][0]
+    for ii in param["param_type"]:
+        line += ii + " "
+    line += "\n"
+    ret += line
+    return ret
+
+
 def inter_eam_fs(param):  # 06/08 eam.fs interaction
     ret = ""
     line = "pair_style      eam/fs \n"
     line += "pair_coeff      * * %s " % param["model_name"][0]
     for ii in param["param_type"]:
         line += ii + " "
     line += "\n"
@@ -181,14 +239,17 @@
     """
     ret = ""
     ret += "clear\n"
     ret += "units 	metal\n"
     ret += "dimension	3\n"
     ret += "boundary	p p p\n"
     ret += "atom_style	atomic\n"
+    if param["type"] == "mace":
+        ret += "atom_modify map yes\n"
+        ret += "newton on\n"
     ret += "box         tilt large\n"
     ret += "read_data   %s\n" % conf
     for ii in range(len(type_map)):
         ret += "mass            %d %.3f\n" % (ii + 1, Element(type_map_list[ii]).mass)
     ret += "neigh_modify    every 1 delay 0 check no\n"
     ret += interaction(param)
     ret += "compute         mype all pe\n"
@@ -227,45 +288,67 @@
     interaction,
     param,
     etol=0,
     ftol=1e-10,
     maxiter=5000,
     maxeval=500000,
     change_box=True,
+    *args,
+    **kwargs
 ):
     type_map_list = element_list(type_map)
 
     """
     make lammps input for equilibritation
     """
+    deepmd_version = param.get("deepmd_version", None)
+    is_new_dpmd = False
+    if deepmd_version:
+        split_v = deepmd_version.split('.')
+        is_new_dpmd = bool(int(split_v[0]) >= 2 and int(split_v[1]) >= 1 and int(split_v[2]) >= 5)
+    prop_type = kwargs.get("prop_type", "others")
+    dump_step = 100
+    # detour sychronizing problem of dumping in new version of deepmd-kit >=2.1.5
+    if is_new_dpmd and prop_type == "relaxation":
+        # make dump_step as large as possible to omit all middle frames and force sychronizing
+        dump_step = 100000
+
+    # in.lammps
     ret = ""
     ret += "clear\n"
     ret += "units 	metal\n"
     ret += "dimension	3\n"
     ret += "boundary	p p p\n"
     ret += "atom_style	atomic\n"
+    if param["type"] == "mace":
+        ret += "atom_modify map yes\n"
+        ret += "newton on\n"
     ret += "box         tilt large\n"
     ret += "read_data   %s\n" % conf
     for ii in range(len(type_map)):
         ret += "mass            %d %.3f\n" % (ii + 1, Element(type_map_list[ii]).mass)
     ret += "neigh_modify    every 1 delay 0 check no\n"
     ret += interaction(param)
     ret += "compute         mype all pe\n"
     ret += "thermo          100\n"
     ret += (
         "thermo_style    custom step pe pxx pyy pzz pxy pxz pyz lx ly lz vol c_mype\n"
     )
-    ret += "dump            1 all custom 100 dump.relax id type xs ys zs fx fy fz\n"
+    ret += f"dump            1 all custom {dump_step} dump.relax id type xs ys zs fx fy fz\n"
     ret += "min_style       cg\n"
     if change_box:
         ret += "fix             1 all box/relax iso 0.0 \n"
-        ret += "minimize        %e %e %d %d\n" % (etol, ftol, maxiter, maxeval)
-        ret += "fix             1 all box/relax aniso 0.0 \n"
-        ret += "minimize        %e %e %d %d\n" % (etol, ftol, maxiter, maxeval)
-        ret += "fix             1 all box/relax tri 0.0 \n"
+        if is_new_dpmd and prop_type != "relaxation":
+            # detour synchronizing problem of property calculation by doing one minimization only
+            pass
+        else:
+            ret += "minimize        %e %e %d %d\n" % (etol, ftol, maxiter, maxeval)
+            ret += "fix             1 all box/relax aniso 0.0 \n"
+            ret += "minimize        %e %e %d %d\n" % (etol, ftol, maxiter, maxeval)
+            ret += "fix             1 all box/relax tri 0.0 \n"
     ret += "minimize        %e %e %d %d\n" % (etol, ftol, maxiter, maxeval)
     ret += "variable        N equal count(all)\n"
     ret += "variable        V equal vol\n"
     ret += 'variable        E equal "c_mype"\n'
     ret += "variable        tmplx equal lx\n"
     ret += "variable        tmply equal ly\n"
     ret += "variable        Pxx equal pxx\n"
@@ -296,14 +379,17 @@
     """
     ret = ""
     ret += "clear\n"
     ret += "units 	metal\n"
     ret += "dimension	3\n"
     ret += "boundary	p p p\n"
     ret += "atom_style	atomic\n"
+    if param["type"] == "mace":
+        ret += "atom_modify map yes\n"
+        ret += "newton on\n"
     ret += "box         tilt large\n"
     ret += "read_data   %s\n" % conf
     for ii in range(len(type_map)):
         ret += "mass            %d %.3f\n" % (ii + 1, Element(type_map_list[ii]).mass)
     ret += "neigh_modify    every 1 delay 0 check no\n"
     ret += interaction(param)
     ret += "compute         mype all pe\n"
@@ -363,14 +449,17 @@
         "variable        Px0		equal 3*${B0}*(1-${xx})/${xx}^2*exp(${yeta}*(1-${xx}))\n"
     )
     ret += "variable        Px		equal ${Px0}*${GPa2bar}\n"
     ret += "units       metal\n"
     ret += "dimension   3\n"
     ret += "boundary	p p p\n"
     ret += "atom_style	atomic\n"
+    if param["type"] == "mace":
+        ret += "atom_modify map yes\n"
+        ret += "newton on\n"
     ret += "box         tilt large\n"
     ret += "read_data   %s\n" % conf
     for ii in range(len(type_map)):
         ret += "mass            %d %.3f\n" % (ii + 1, Element(type_map_list[ii]).mass)
     ret += "neigh_modify    every 1 delay 0 check no\n"
     ret += interaction(param)
     ret += "compute         mype all pe\n"
@@ -399,36 +488,33 @@
     ret += 'print "Total number of atoms  = ${N}"\n'
     ret += 'print "Relax at Press         = ${Px} Bar"\n'
     ret += 'print "Final energy per atoms = ${Epa} eV"\n'
     ret += 'print "Final volume per atoms = ${Vpa} A^3"\n'
     ret += 'print "Final Stress (xx yy zz xy xz yz) = ${Pxx} ${Pyy} ${Pzz} ${Pxy} ${Pxz} ${Pyz}"\n'
     return ret
 
-
+"""
 def make_lammps_phonon(
     conf, masses, interaction, param, etol=0, ftol=1e-10, maxiter=5000, maxeval=500000
 ):
-    """
-    make lammps input for elastic calculation
-    """
     ret = ""
     ret += "clear\n"
     ret += "units 	metal\n"
     ret += "dimension	3\n"
     ret += "boundary	p p p\n"
     ret += "atom_style	atomic\n"
     ret += "box         tilt large\n"
     ret += "read_data   %s\n" % conf
     ntypes = len(masses)
     for ii in range(ntypes):
         ret += "mass            %d %f\n" % (ii + 1, masses[ii])
     ret += "neigh_modify    every 1 delay 0 check no\n"
     ret += interaction(param)
     return ret
-
+"""
 
 def _get_epa(lines):
     for ii in lines:
         if ("Final energy per atoms" in ii) and (not "print" in ii):
             return float(ii.split("=")[1].split()[0])
     raise RuntimeError(
         'cannot find key "Final energy per atoms" in lines, something wrong'
```

### Comparing `apex-flow-1.1.6/apex/core/calculator/lib/vasp_utils.py` & `apex_flow-1.2.0/apex/core/calculator/lib/vasp_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,32 +315,34 @@
 
 def make_vasp_relax_incar(
     ecut,
     ediff,
     relax_ion,
     relax_shape,
     relax_volume,
-    npar,
-    kpar,
+    npar=None,
+    kpar=None,
     kspacing=0.5,
     kgamma=True,
     ismear=1,
     sigma=0.22,
 ):
     isif = _compute_isif(relax_ion, relax_shape, relax_volume)
     ret = ""
     ret += "PREC=A\n"
     ret += "ENCUT=%d\n" % ecut
     ret += "# ISYM=0\n"
     ret += "ALGO=normal\n"
     ret += "EDIFF=%e\n" % ediff
     ret += "EDIFFG=-0.01\n"
     ret += "LREAL=A\n"
-    ret += "NPAR=%d\n" % npar
-    ret += "KPAR=%d\n" % kpar
+    if npar:
+        ret += "NPAR=%d\n" % npar
+    if kpar:
+        ret += "KPAR=%d\n" % kpar
     ret += "\n"
     ret += "ISMEAR=%d\n" % ismear
     ret += "SIGMA=%f\n" % sigma
     ret += "\n"
     ret += "ISTART=0\n"
     ret += "ICHARG=2\n"
     ret += "NELM=100\n"
@@ -361,15 +363,15 @@
             ret += "KGAMMA=T\n"
         else:
             ret += "KGAMMA=F\n"
     return ret
 
 
 def make_vasp_phonon_dfpt_incar(
-    ecut, ediff, npar, kpar, kspacing=0.3, kgamma=True, ismear=1, sigma=0.22
+    ecut, ediff, npar, kpar, kspacing=0.3, kgamma=True, ismear=1, sigma=0.01
 ):
     isif = 2
     ret = ""
     ret += "ADDGRID=True\n"
     ret += "PREC=A\n"
     ret += "ENCUT=%d\n" % ecut
     ret += "# ISYM=0\n"
```

### Comparing `apex-flow-1.1.6/apex/core/common_prop.py` & `apex_flow-1.2.0/apex/core/common_prop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import glob
 import os
 from multiprocessing import Pool
+from monty.serialization import dumpfn
 
 from apex.core.calculator.calculator import make_calculator
 from apex.core.property.Elastic import Elastic
 from apex.core.property.EOS import EOS
 from apex.core.property.Gamma import Gamma
 from apex.core.property.Interstitial import Interstitial
-from apex.core.lib.utils import create_path
-from apex.core.lib.util import collect_task
-from apex.core.lib.dispatcher import make_submission
 from apex.core.property.Surface import Surface
 from apex.core.property.Vacancy import Vacancy
 from apex.core.property.Phonon import Phonon
-from apex.utils import sepline, get_task_type
+from apex.core.lib.utils import create_path
+from apex.core.lib.util import collect_task
+from apex.core.lib.dispatcher import make_submission
+from apex.utils import sepline, get_task_type, handle_prop_suffix
 from dflow.python import upload_packages
 upload_packages.append(__file__)
 
-lammps_task_type = ["deepmd", "meam", "eam_fs", "eam_alloy"]
-
+lammps_task_type = ['deepmd', 'eam_alloy', 'meam', 'eam_fs', 'meam_spline', 'snap', 'gap', 'rann', 'mace']
 
 def make_property_instance(parameters, inter_param):
     """
     Make an instance of Property
     """
     prop_type = parameters["type"]
     if prop_type == "eos":
@@ -36,73 +36,54 @@
     elif prop_type == "surface":
         return Surface(parameters, inter_param)
     elif prop_type == "gamma":
         return Gamma(parameters, inter_param)
     elif prop_type == "phonon":
         return Phonon(parameters, inter_param)
     else:
-        raise RuntimeError(f"unknown dflowautotest type {prop_type}")
+        raise RuntimeError(f"unknown APEX type {prop_type}")
 
 
 def make_property(confs, inter_param, property_list):
     # find all POSCARs and their name like mp-xxx
-    # ...
     # conf_dirs = glob.glob(confs)
     # conf_dirs.sort()
     conf_dirs = []
     for conf in confs:
         conf_dirs.extend(glob.glob(conf))
+    conf_dirs = list(set(conf_dirs))
     conf_dirs.sort()
     for ii in conf_dirs:
         sepline(ch=ii, screen=True)
         for jj in property_list:
-            if jj.get("skip", False):
+            do_refine, suffix = handle_prop_suffix(jj)
+            if not suffix:
                 continue
-            if "init_from_suffix" and "output_suffix" in jj:
-                do_refine = True
-                suffix = jj["output_suffix"]
-            elif "reproduce" in jj and jj["reproduce"]:
-                do_refine = False
-                suffix = "reprod"
-            elif 'suffix' in jj and jj['suffix']:
-                do_refine = False
-                suffix = str(jj['suffix'])
-            else:
-                do_refine = False
-                suffix = "00"
             # generate working directory like mp-xxx/eos_00 if jj['type'] == 'eos'
             # handel the exception that the working directory exists
-            # ...
-
             # determine the suffix: from scratch or refine
-            # ...
 
             property_type = jj["type"]
             path_to_equi = os.path.join(ii, "relaxation", "relax_task")
             path_to_work = os.path.join(ii, property_type + "_" + suffix)
 
             create_path(path_to_work)
 
-            inter_param_prop = inter_param
-            if "cal_setting" in jj and "overwrite_interaction" in jj["cal_setting"]:
-                inter_param_prop = jj["cal_setting"]["overwrite_interaction"]
+            inter_param_prop = jj.get("cal_setting", {}).get("overwrite_interaction", inter_param)
 
             prop = make_property_instance(jj, inter_param_prop)
             task_list = prop.make_confs(path_to_work, path_to_equi, do_refine)
 
             for kk in task_list:
                 poscar = os.path.join(kk, "POSCAR")
                 inter = make_calculator(inter_param_prop, poscar)
                 inter.make_potential_files(kk)
-                #dlog.debug(prop.task_type())  ### debug
                 inter.make_input_file(kk, prop.task_type(), prop.task_param())
 
-            prop.post_process(
-                task_list
-            )  # generate same KPOINTS file for elastic when doing VASP
+            prop.post_process(task_list)  # generate same KPOINTS file for elastic when doing DFT
 
 
 def worker(
     work_path,
     all_task,
     forward_common_files,
     forward_files,
@@ -110,18 +91,17 @@
     mdata,
     inter_type,
     task_type,
 ):
     run_tasks = [os.path.basename(ii) for ii in all_task]
     machine = mdata.get("machine", None)
     resources = mdata.get("resources", None)
-    command = mdata.get(f"{task_type}_run_command", None)
-    if not command:
-        command = mdata.get("run_command", None)
+    command = mdata.get(f"{task_type}_run_command", mdata.get("run_command", None))
     group_size = mdata.get("group_size", 1)
+
     submission = make_submission(
         mdata_machine=machine,
         mdata_resources=resources,
         commands=[command],
         work_path=work_path,
         run_tasks=run_tasks,
         group_size=group_size,
@@ -132,56 +112,45 @@
         errlog="errlog",
     )
     submission.run_submission()
 
 
 def run_property(confs, inter_param, property_list, mdata):
     # find all POSCARs and their name like mp-xxx
-    # ...
     # conf_dirs = glob.glob(confs)
     # conf_dirs.sort()
-    processes = len(property_list)
-    pool = Pool(processes=processes)
-    print("Submit job via %d processes" % processes)
     conf_dirs = []
     for conf in confs:
         conf_dirs.extend(glob.glob(conf))
+    conf_dirs = list(set(conf_dirs))
     conf_dirs.sort()
+
     task_list = []
     work_path_list = []
     multiple_ret = []
     for ii in conf_dirs:
         sepline(ch=ii, screen=True)
         for jj in property_list:
             # determine the suffix: from scratch or refine
             # ...
-            if jj.get("skip", False):
+            do_refine, suffix = handle_prop_suffix(jj)
+            if not suffix:
                 continue
-            if "init_from_suffix" and "output_suffix" in jj:
-                suffix = jj["output_suffix"]
-            elif "reproduce" in jj and jj["reproduce"]:
-                suffix = "reprod"
-            elif 'suffix' in jj and jj['suffix']:
-                suffix = str(jj['suffix'])
-            else:
-                suffix = "00"
 
             property_type = jj["type"]
             path_to_work = os.path.abspath(
                 os.path.join(ii, property_type + "_" + suffix)
             )
 
             work_path_list.append(path_to_work)
             tmp_task_list = glob.glob(os.path.join(path_to_work, "task.[0-9]*[0-9]"))
             tmp_task_list.sort()
             task_list.append(tmp_task_list)
 
-            inter_param_prop = inter_param
-            if "cal_setting" in jj and "overwrite_interaction" in jj["cal_setting"]:
-                inter_param_prop = jj["cal_setting"]["overwrite_interaction"]
+            inter_param_prop = jj.get("cal_setting", {}).get("overwrite_interaction", inter_param)
 
             # dispatch the tasks
             # POSCAR here is useless
             virtual_calculator = make_calculator(inter_param_prop, "POSCAR")
             forward_files = virtual_calculator.forward_files(property_type)
             forward_common_files = virtual_calculator.forward_common_files(
                 property_type
@@ -193,67 +162,69 @@
             inter_type = inter_param_prop["type"]
             work_path = path_to_work
             all_task = tmp_task_list
             run_tasks = collect_task(all_task, inter_type)
             if len(run_tasks) == 0:
                 continue
             else:
+                processes = len(run_tasks)
+                pool = Pool(processes=processes)
+                print("Submit job via %d processes" % processes)
                 ret = pool.apply_async(
                     worker,
                     (
                         work_path,
                         all_task,
                         forward_common_files,
                         forward_files,
                         backward_files,
                         mdata,
                         inter_type,
                         task_type
-                    ),
+                    )
                 )
                 multiple_ret.append(ret)
     pool.close()
     pool.join()
     for ii in range(len(multiple_ret)):
         if not multiple_ret[ii].successful():
             print("ERROR:", multiple_ret[ii].get())
             raise RuntimeError("Job %d is not successful!" % ii)
     print("%d jobs are finished" % len(multiple_ret))
 
 
 def post_property(confs, inter_param, property_list):
     # find all POSCARs and their name like mp-xxx
-    # ...
     #    task_list = []
     # conf_dirs = glob.glob(confs)
     # conf_dirs.sort()
     conf_dirs = []
     for conf in confs:
         conf_dirs.extend(glob.glob(conf))
+    conf_dirs = list(set(conf_dirs))
     conf_dirs.sort()
     for ii in conf_dirs:
         for jj in property_list:
             # determine the suffix: from scratch or refine
             # ...
-            if jj.get("skip", False):
+            do_refine, suffix = handle_prop_suffix(jj)
+            if not suffix:
                 continue
-            if "init_from_suffix" and "output_suffix" in jj:
-                suffix = jj["output_suffix"]
-            elif "reproduce" in jj and jj["reproduce"]:
-                suffix = "reprod"
-            elif 'suffix' in jj and jj['suffix']:
-                suffix = str(jj['suffix'])
-            else:
-                suffix = "00"
 
-            inter_param_prop = inter_param
-            if "cal_setting" in jj and "overwrite_interaction" in jj["cal_setting"]:
-                inter_param_prop = jj["cal_setting"]["overwrite_interaction"]
+            inter_param_prop = jj.get("cal_setting", {}).get("overwrite_interaction", inter_param)
 
             property_type = jj["type"]
             path_to_work = os.path.join(ii, property_type + "_" + suffix)
             prop = make_property_instance(jj, inter_param_prop)
+            param_json = os.path.join(path_to_work, "param.json")
+            param_dict = prop.parameter
+            param_dict.setdefault("skip", False) # default of "skip" is False
+            try:
+                param_dict.pop("skip")
+            except KeyError:
+                pass
+            dumpfn(param_dict, param_json)
             prop.compute(
                 os.path.join(path_to_work, "result.json"),
                 os.path.join(path_to_work, "result.out"),
-                path_to_work,
+                path_to_work
             )
```

### Comparing `apex-flow-1.1.6/apex/core/gen_confs.py` & `apex_flow-1.2.0/apex/core/gen_confs.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/apex/core/lib/crys.py` & `apex_flow-1.2.0/apex/core/lib/crys.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,74 +11,71 @@
     return Structure(box, [ele_name], [[0, 0, 0]])
 
 
 def fcc1(ele_name="ele", a=4.05):
     latt = Lattice.cubic(a)
     return Structure(
         latt,
-        [ele_name, ele_name, ele_name, ele_name],
-        [[0, 0, 0], [0, 0.5, 0.5], [0.5, 0, 0.5], [0.5, 0.5, 0]],
+        [ele_name] * 4,
+        [[0, 0, 0], [0, 0.5, 0.5], [0.5, 0, 0.5], [0.5, 0.5, 0]]
     )
 
 
 def sc(ele_name="ele", a=2.551340126037118):
     latt = Lattice.cubic(a)
     return Structure(latt, [ele_name], [[0, 0, 0]])
 
 
 def bcc(ele_name="ele", a=3.2144871302356037):
     latt = Lattice.cubic(a)
     return Structure(
         latt,
-        [ele_name, ele_name],
-        [
-            [0, 0, 0],
-            [0.5, 0.5, 0.5],
-        ],
+        [ele_name] * 2,
+        [[0, 0, 0], [0.5, 0.5, 0.5]]
     )
 
 
 def hcp(
     ele_name="ele", a=4.05 / np.sqrt(2), c=4.05 / np.sqrt(2) * 2.0 * np.sqrt(2.0 / 3.0)
 ):
     box = np.array([[1, 0, 0], [0.5, 0.5 * np.sqrt(3), 0], [0, 0, 1]])
     box[0] *= a
     box[1] *= a
     box[2] *= c
     latt = Lattice(box)
     return Structure(
-        latt, [ele_name, ele_name], [[0, 0, 0], [1.0 / 3, 1.0 / 3, 1.0 / 2]]
+        latt, [ele_name] * 2, [[0, 0, 0], [1.0 / 3, 1.0 / 3, 1.0 / 2]]
     )
 
 
 def dhcp(
     ele_name="ele", a=4.05 / np.sqrt(2), c=4.05 / np.sqrt(2) * 4.0 * np.sqrt(2.0 / 3.0)
 ):
     box = np.array([[1, 0, 0], [0.5, 0.5 * np.sqrt(3), 0], [0, 0, 1]])
     box[0] *= a
     box[1] *= a
     box[2] *= c
     latt = Lattice(box)
     return Structure(
         latt,
-        [ele_name, ele_name, ele_name, ele_name],
+        [ele_name] * 4,
         [
             [0, 0, 0],
             [1.0 / 3.0, 1.0 / 3.0, 1.0 / 4.0],
             [0, 0, 1.0 / 2.0],
-            [2.0 / 3.0, 2.0 / 3.0, 3.0 / 4.0],
-        ],
+            [2.0 / 3.0, 2.0 / 3.0, 3.0 / 4.0]
+        ]
     )
 
 
 def diamond(ele_name="ele", a=2.551340126037118):
     box = np.array([[0.0, 1.0, 1.0], [1.0, 0.0, 1.0], [1.0, 1.0, 0.0]])
     box *= a
     latt = Lattice(box)
     return Structure(
         latt,
-        [ele_name, ele_name],
+        [ele_name] * 2,
         [
             [0.12500000000000, 0.12500000000000, 0.12500000000000],
-            [0.87500000000000, 0.87500000000000, 0.87500000000000],
-        ],
+            [0.87500000000000, 0.87500000000000, 0.87500000000000]
+        ]
     )
```

### Comparing `apex-flow-1.1.6/apex/core/lib/lmp.py` & `apex_flow-1.2.0/apex/core/lib/lmp.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/apex/core/lib/mfp_eosfit.py` & `apex_flow-1.2.0/apex/core/lib/mfp_eosfit.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/apex/core/lib/pwscf.py` & `apex_flow-1.2.0/apex/core/lib/pwscf.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/apex/core/lib/siesta.py` & `apex_flow-1.2.0/apex/core/lib/siesta.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/apex/core/lib/slab_orientation.py` & `apex_flow-1.2.0/apex/core/lib/slab_orientation.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,20 @@
                              'xy': direction_miller_bravais_to_miller([1, -2, 1, 3]),
                              'default_frac_slip_len': float(np.sqrt(3))},
 
             # Pyramidal II, shear SF2 along x
             '-12-12x1-213': {'plane': plane_miller_bravais_to_miller([-1, 2, -1, 2]),
                              'x': direction_miller_bravais_to_miller([1, -2, 1, 3]),
                              'xy': direction_miller_bravais_to_miller([-1, 0, 1, 0]),
+                             'default_frac_slip_len': (1, 0, 1)},
+
+            # Pyramidal II, shear SF2 along x by climbing the hill
+            '-12-12x-12-1-3': {'plane': plane_miller_bravais_to_miller([-1, 2, -1, 2]),
+                             'x': direction_miller_bravais_to_miller([-1, 2, -1, -3]),
+                             'xy': direction_miller_bravais_to_miller([1, 0, -1, 0]),
                              'default_frac_slip_len': (1, 0, 1)}
         }
     }
 
     @classmethod
     def atomic_system_dict(cls):
         return cls.__dict_atomic_system
```

### Comparing `apex-flow-1.1.6/apex/core/lib/trans_tools.py` & `apex_flow-1.2.0/apex/core/lib/trans_tools.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/apex/core/lib/util.py` & `apex_flow-1.2.0/apex/core/lib/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import os
 import re
 
 import numpy as np
 import requests
 
-#from dpgen import dlog
 from apex.core.calculator.lib import abacus_utils, lammps_utils, vasp_utils
+from apex.core.calculator import LAMMPS_INTER_TYPE as lammps_task_type
 from apex.core.lib.utils import cmd_append_log
 from dflow.python import upload_packages
 upload_packages.append(__file__)
 
-lammps_task_type = ["deepmd", "meam", "eam_fs", "eam_alloy"]  # 06/13 revised
-
 
 def voigt_to_stress(inpt):
     ret = np.zeros((3, 3))
     ret[0][0] = inpt[0]
     ret[1][1] = inpt[1]
     ret[2][2] = inpt[2]
     ret[0][1] = inpt[3]
```

### Comparing `apex-flow-1.1.6/apex/core/lib/utils.py` & `apex_flow-1.2.0/apex/core/lib/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,25 @@
 upload_packages.append(__file__)
 
 iter_format = "%s"
 task_format = "%s"
 log_iter_head = "task type: " + iter_format + " task: " + task_format + " process: "
 
 
+def round_format(nums, decimal_places):
+    return [f"{round(num, decimal_places):.{decimal_places}f}"
+             if isinstance(num, (int, float)) else num for num in nums]
+
+
+def round_2d_format(nums, decimal_places):
+    return [[f"{round(num, decimal_places):.{decimal_places}f}"
+             if isinstance(num, (int, float)) else num for num in row]
+            for row in nums]
+
+
 def make_iter_name(iter_index):
     return "task type:" + (iter_format)
 
 
 def create_path(path):
     path += "/"
     if os.path.isdir(path):
```

### Comparing `apex-flow-1.1.6/apex/core/mpdb.py` & `apex_flow-1.2.0/apex/core/mpdb.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/apex/core/property/EOS.py` & `apex_flow-1.2.0/apex/core/property/EOS.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import glob
 import json
 import logging
 import os
 import re
-
 import numpy as np
 from monty.serialization import dumpfn, loadfn
 
 from apex.core.calculator.lib import abacus_utils
 from apex.core.calculator.lib import vasp_utils
 from apex.core.calculator.lib import abacus_scf
 from apex.core.property.Property import Property
@@ -31,113 +30,84 @@
             parameter["cal_type"] = parameter.get("cal_type", "relaxation")
             self.cal_type = parameter["cal_type"]
             default_cal_setting = {
                 "relax_pos": True,
                 "relax_shape": True,
                 "relax_vol": False,
             }
-            if "cal_setting" not in parameter:
-                parameter["cal_setting"] = default_cal_setting
-            else:
-                if "relax_pos" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_pos"] = default_cal_setting[
-                        "relax_pos"
-                    ]
-                if "relax_shape" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                        "relax_shape"
-                    ]
-                if "relax_vol" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_vol"] = default_cal_setting[
-                        "relax_vol"
-                    ]
+            parameter.setdefault("cal_setting", {})
+            parameter["cal_setting"].update(
+                {k: v for k, v in default_cal_setting.items() if k not in parameter["cal_setting"]})
             self.cal_setting = parameter["cal_setting"]
         else:
             parameter["cal_type"] = "static"
             self.cal_type = parameter["cal_type"]
             default_cal_setting = {
                 "relax_pos": False,
                 "relax_shape": False,
                 "relax_vol": False,
             }
-            if "cal_setting" not in parameter:
-                parameter["cal_setting"] = default_cal_setting
-            else:
-                if "relax_pos" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_pos"] = default_cal_setting[
-                        "relax_pos"
-                    ]
-                if "relax_shape" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                        "relax_shape"
-                    ]
-                if "relax_vol" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_vol"] = default_cal_setting[
-                        "relax_vol"
-                    ]
+            parameter.setdefault("cal_setting", {})
+            parameter["cal_setting"].update(
+                {k: v for k, v in default_cal_setting.items() if k not in parameter["cal_setting"]})
             self.cal_setting = parameter["cal_setting"]
             parameter["init_from_suffix"] = parameter.get("init_from_suffix", "00")
             self.init_from_suffix = parameter["init_from_suffix"]
         self.parameter = parameter
         self.inter_param = inter_param if inter_param != None else {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
-            #dlog.warning("%s already exists" % path_to_work)
             logging.warning("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
 
         if "start_confs_path" in self.parameter and os.path.exists(
             self.parameter["start_confs_path"]
         ):
             init_path_list = glob.glob(
                 os.path.join(self.parameter["start_confs_path"], "*")
             )
-            struct_init_name_list = []
-            for ii in init_path_list:
-                struct_init_name_list.append(ii.split("/")[-1])
-            struct_output_name = path_to_work.split("/")[-2]
+            struct_init_name_list = [os.path.basename(ii) for ii in init_path_list]
+            struct_output_name = os.path.basename(os.path.dirname(path_to_work))
             assert struct_output_name in struct_init_name_list
             path_to_equi = os.path.abspath(
                 os.path.join(
                     self.parameter["start_confs_path"],
                     struct_output_name,
                     "relaxation",
                     "relax_task",
                 )
             )
 
         cwd = os.getcwd()
         task_list = []
         if self.reprod:
-            print("eos reproduce starts")
+            logging.info("eos reproduce starts")
             if "init_data_path" not in self.parameter:
                 raise RuntimeError("please provide the initial data path to reproduce")
             init_data_path = os.path.abspath(self.parameter["init_data_path"])
             task_list = make_repro(
                 self.inter_param,
                 init_data_path,
                 self.init_from_suffix,
                 path_to_work,
                 self.parameter.get("reprod_last_frame", True),
             )
-            os.chdir(cwd)
 
         else:
             if refine:
-                print("eos refine starts")
+                logging.info("eos refine starts")
                 task_list = make_refine(
                     self.parameter["init_from_suffix"],
                     self.parameter["output_suffix"],
                     path_to_work,
                 )
-                os.chdir(cwd)
 
                 init_from_path = re.sub(
                     self.parameter["output_suffix"][::-1],
                     self.parameter["init_from_suffix"][::-1],
                     path_to_work[::-1],
                     count=1,
                 )[::-1]
@@ -151,32 +121,28 @@
                         os.remove("eos.json")
                     if os.path.islink("eos.json"):
                         os.remove("eos.json")
                     os.symlink(
                         os.path.relpath(os.path.join(init_from_task, "eos.json")),
                         "eos.json",
                     )
-                os.chdir(cwd)
 
             else:
-                print(
+                logging.info(
                     "gen eos from "
                     + str(self.vol_start)
                     + " to "
                     + str(self.vol_end)
                     + " by every "
                     + str(self.vol_step)
                 )
                 if self.vol_abs:
                     logging.info("treat vol_start and vol_end as absolute volume")
-                    #dlog.info("treat vol_start
-                    # and vol_end as absolute volume")
                 else:
                     logging.info("treat vol_start and vol_end as relative volume")
-                    #dlog.info("treat vol_start and vol_end as relative volume")
 
                 if self.inter_param["type"] == "abacus":
                     equi_contcar = os.path.join(
                         path_to_equi, abacus_utils.final_stru(path_to_equi)
                     )
                 else:
                     equi_contcar = os.path.join(path_to_equi, "CONTCAR")
@@ -196,18 +162,15 @@
                     vol_to_poscar = vasp_utils.poscar_vol(equi_contcar) / vasp_utils.poscar_natoms(
                         equi_contcar
                     )
                 self.parameter["scale2equi"] = []
 
                 task_num = 0
                 while self.vol_start + self.vol_step * task_num < self.vol_end:
-                    # for vol in np.arange(int(self.vol_start * 100), int(self.vol_end * 100), int(self.vol_step * 100)):
-                    # vol = vol / 100.0
                     vol = self.vol_start + task_num * self.vol_step
-                    # task_num = int((vol - self.vol_start) / self.vol_step)
                     output_task = os.path.join(path_to_work, "task.%06d" % task_num)
                     os.makedirs(output_task, exist_ok=True)
                     os.chdir(output_task)
                     if self.inter_param["type"] == "abacus":
                         POSCAR = "STRU"
                         POSCAR_orig = "STRU.orig"
                         scale_func = abacus_utils.stru_scale
@@ -236,15 +199,15 @@
                     else:
                         scale = vol ** (1.0 / 3.0)
                         eos_params = {"volume": vol * vol_to_poscar, "scale": scale}
                     dumpfn(eos_params, "eos.json", indent=4)
                     self.parameter["scale2equi"].append(scale)  # 06/22
                     scale_func(POSCAR_orig, POSCAR, scale)
                     task_num += 1
-                os.chdir(cwd)
+        os.chdir(cwd)
         return task_list
 
     def post_process(self, task_list):
         pass
 
     def task_type(self):
         return self.parameter["type"]
@@ -265,16 +228,14 @@
                 res_data[vol] = task_result["energies"][-1] / sum(
                     task_result["atom_numbs"]
                 )
                 ptr_data += "%7.3f  %8.4f \n" % (
                     vol,
                     task_result["energies"][-1] / sum(task_result["atom_numbs"]),
                 )
-                # res_data[vol] = all_res[ii]['energy'] / len(all_res[ii]['force'])
-                # ptr_data += '%7.3f  %8.4f \n' % (vol, all_res[ii]['energy'] / len(all_res[ii]['force']))
 
         else:
             if "init_data_path" not in self.parameter:
                 raise RuntimeError("please provide the initial data path to reproduce")
             init_data_path = os.path.abspath(self.parameter["init_data_path"])
             res_data, ptr_data = post_repro(
                 init_data_path,
```

### Comparing `apex-flow-1.1.6/apex/core/property/Elastic.py` & `apex_flow-1.2.0/apex/core/property/Elastic.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,119 +5,102 @@
 from shutil import copyfile
 
 from monty.serialization import dumpfn, loadfn
 from pymatgen.analysis.elasticity.elastic import ElasticTensor
 from pymatgen.analysis.elasticity.strain import DeformedStructureSet, Strain
 from pymatgen.analysis.elasticity.stress import Stress
 from pymatgen.core.structure import Structure
+from pymatgen.core.tensors import Tensor
+from pymatgen.core.operations import SymmOp
 from pymatgen.io.vasp import Incar, Kpoints
 
 from apex.core.calculator.lib import abacus_utils
 from apex.core.calculator.lib import vasp_utils
 from apex.core.calculator.lib import abacus_scf
 from apex.core.property.Property import Property
+from apex.core.structure import StructureInfo
 from apex.core.refine import make_refine
 from apex.core.calculator.lib.vasp_utils import incar_upper
 from dflow.python import upload_packages
 upload_packages.append(__file__)
 
 
 class Elastic(Property):
     def __init__(self, parameter, inter_param=None):
         if not ("init_from_suffix" in parameter and "output_suffix" in parameter):
-            default_norm_def = 1e-2
-            default_shear_def = 1e-2
-            parameter["norm_deform"] = parameter.get("norm_deform", default_norm_def)
+            parameter.setdefault("norm_deform", 1e-2)
             self.norm_deform = parameter["norm_deform"]
-            parameter["shear_deform"] = parameter.get("shear_deform", default_shear_def)
+            parameter.setdefault("shear_deform", 1e-2)
             self.shear_deform = parameter["shear_deform"]
-        parameter["cal_type"] = parameter.get("cal_type", "relaxation")
+            parameter.setdefault("conventional", False)
+            self.conventional = parameter["conventional"]
+            parameter.setdefault("ieee", True)
+            self.ieee = parameter["ieee"]
+        parameter.setdefault("cal_type", "relaxation")
         self.cal_type = parameter["cal_type"]
         default_cal_setting = {
             "relax_pos": True,
             "relax_shape": False,
             "relax_vol": False,
         }
-        if "cal_setting" not in parameter:
-            parameter["cal_setting"] = default_cal_setting
-        else:
-            if "relax_pos" not in parameter["cal_setting"]:
-                parameter["cal_setting"]["relax_pos"] = default_cal_setting["relax_pos"]
-            if "relax_shape" not in parameter["cal_setting"]:
-                parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                    "relax_shape"
-                ]
-            if "relax_vol" not in parameter["cal_setting"]:
-                parameter["cal_setting"]["relax_vol"] = default_cal_setting["relax_vol"]
+        parameter.setdefault("cal_setting", {})
+        parameter["cal_setting"].setdefault("relax_pos", True)
+        parameter["cal_setting"].setdefault("relax_shape", False)
+        parameter["cal_setting"].setdefault("relax_vol", False)
         self.cal_setting = parameter["cal_setting"]
         # parameter['reproduce'] = False
         # self.reprod = parameter['reproduce']
         self.parameter = parameter
-        self.inter_param = inter_param if inter_param != None else {"type": "vasp"}
+        self.inter_param = inter_param or {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
             logging.warning("%s already exists" % path_to_work)
-            #dlog.warning("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
 
         if "start_confs_path" in self.parameter and os.path.exists(
             self.parameter["start_confs_path"]
         ):
             init_path_list = glob.glob(
                 os.path.join(self.parameter["start_confs_path"], "*")
             )
-            struct_init_name_list = []
-            for ii in init_path_list:
-                struct_init_name_list.append(ii.split("/")[-1])
-            struct_output_name = path_to_work.split("/")[-2]
+            struct_init_name_list = [os.path.basename(ii) for ii in init_path_list]
+            struct_output_name = os.path.basename(os.path.dirname(path_to_work))
             assert struct_output_name in struct_init_name_list
             path_to_equi = os.path.abspath(
                 os.path.join(
                     self.parameter["start_confs_path"],
                     struct_output_name,
                     "relaxation",
                     "relax_task",
                 )
             )
 
         task_list = []
         cwd = os.getcwd()
 
-        if self.inter_param["type"] == "abacus":
-            CONTCAR = abacus_utils.final_stru(path_to_equi)
-            POSCAR = "STRU"
-        else:
-            CONTCAR = "CONTCAR"
-            POSCAR = "POSCAR"
-
+        CONTCAR = "CONTCAR" if self.inter_param["type"] != "abacus" else abacus_utils.final_stru(path_to_equi)
+        POSCAR = "POSCAR" if self.inter_param["type"] != "abacus" else "STRU"
         equi_contcar = os.path.join(path_to_equi, CONTCAR)
 
         os.chdir(path_to_work)
-        if os.path.isfile(POSCAR):
-            os.remove(POSCAR)
-        if os.path.islink(POSCAR):
+        if os.path.exists(POSCAR) or os.path.islink(POSCAR):
             os.remove(POSCAR)
         os.symlink(os.path.relpath(equi_contcar), POSCAR)
-        #           task_poscar = os.path.join(output, 'POSCAR')
-
         # stress, deal with unsupported stress in dpdata
-        # with open(os.path.join(path_to_equi, 'result.json')) as fin:
-        #    equi_result = json.load(fin)
-        # equi_stress = np.array(equi_result['stress']['data'])[-1]
         equi_result = loadfn(os.path.join(path_to_equi, "result.json"))
         equi_stress = equi_result["stress"][-1]
         dumpfn(equi_stress, "equi.stress.json", indent=4)
         os.chdir(cwd)
 
         if refine:
-            print("elastic refine starts")
+            logging.info("elastic refine starts")
             task_list = make_refine(
                 self.parameter["init_from_suffix"],
                 self.parameter["output_suffix"],
                 path_to_work,
             )
 
             # record strain
@@ -138,28 +121,40 @@
                 if os.path.isfile("strain.json"):
                     os.remove("strain.json")
                 copyfile(os.path.join(init_from_task, "strain.json"), "strain.json")
                 # os.symlink(os.path.relpath(
                 #    os.path.join((re.sub(self.parameter['output_suffix'], self.parameter['init_from_suffix'], ii)),
                 #                 'strain.json')),
                 #           'strain.json')
-            os.chdir(cwd)
         else:
             norm_def = self.norm_deform
             shear_def = self.shear_deform
             norm_strains = [-norm_def, -0.5 * norm_def, 0.5 * norm_def, norm_def]
             shear_strains = [-shear_def, -0.5 * shear_def, 0.5 * shear_def, shear_def]
 
             if not os.path.exists(equi_contcar):
                 raise RuntimeError("please do relaxation first")
 
             if self.inter_param["type"] == "abacus":
                 ss = abacus_utils.stru2Structure(equi_contcar)
             else:
                 ss = Structure.from_file(equi_contcar)
+            # find conventional cell
+            if self.conventional:
+                st = StructureInfo(ss)
+                ss = st.conventional_structure
+                ss.to(os.path.join(path_to_work, "POSCAR.conv"), "POSCAR")
+
+            # convert to IEEE-standard
+            if self.ieee:
+                rot = Tensor.get_ieee_rotation(ss)
+                op = SymmOp.from_rotation_and_translation(rot)
+                ss.apply_operation(op)
+                ss.to(os.path.join(path_to_work, "POSCAR.ieee"), "POSCAR")
+
             dfm_ss = DeformedStructureSet(
                 ss,
                 symmetry=False,
                 norm_strains=norm_strains,
                 shear_strains=shear_strains,
             )
             n_dfm = len(dfm_ss)
@@ -180,19 +175,19 @@
                 ]:
                     if os.path.exists(jj):
                         os.remove(jj)
                 task_list.append(output_task)
                 dfm_ss.deformed_structures[ii].to("POSCAR", "POSCAR")
                 if self.inter_param["type"] == "abacus":
                     abacus_utils.poscar2stru("POSCAR", self.inter_param, "STRU")
-                    os.remove("POSCAR")
+                    #os.remove("POSCAR")
                 # record strain
                 df = Strain.from_deformation(dfm_ss.deformations[ii])
                 dumpfn(df.as_dict(), "strain.json", indent=4)
-            os.chdir(cwd)
+        os.chdir(cwd)
         return task_list
 
     def post_process(self, task_list):
         if self.inter_param["type"] == "abacus":
             POSCAR = "STRU"
             INCAR = "INPUT"
             KPOINTS = "KPT"
@@ -230,17 +225,15 @@
                 kp.write_file("KPOINTS")
 
             os.chdir(cwd)
             kpoints_universal = os.path.abspath(
                 os.path.join(task_list[0], "..", KPOINTS)
             )
             for ii in task_list:
-                if os.path.isfile(os.path.join(ii, KPOINTS)):
-                    os.remove(os.path.join(ii, KPOINTS))
-                if os.path.islink(os.path.join(ii, KPOINTS)):
+                if os.path.exists(os.path.join(ii, KPOINTS)):
                     os.remove(os.path.join(ii, KPOINTS))
                 os.chdir(ii)
                 os.symlink(os.path.relpath(kpoints_universal), KPOINTS)
 
         os.chdir(cwd)
 
     def task_type(self):
@@ -249,38 +242,38 @@
     def task_param(self):
         return self.parameter
 
     def _compute_lower(self, output_file, all_tasks, all_res):
         output_file = os.path.abspath(output_file)
         res_data = {}
         ptr_data = os.path.dirname(output_file) + "\n"
+
         equi_stress = Stress(
             loadfn(os.path.join(os.path.dirname(output_file), "equi.stress.json"))
         )
         equi_stress *= -1000
         lst_strain = []
         lst_stress = []
         for ii in all_tasks:
             strain = loadfn(os.path.join(ii, "strain.json"))
             # stress, deal with unsupported stress in dpdata
-            # with open(os.path.join(ii, 'result_task.json')) as fin:
-            #    task_result = json.load(fin)
-            # stress = np.array(task_result['stress']['data'])[-1]
             stress = loadfn(os.path.join(ii, "result_task.json"))["stress"][-1]
             lst_strain.append(strain)
             lst_stress.append(Stress(stress * -1000))
 
         et = ElasticTensor.from_independent_strains(
             lst_strain, lst_stress, eq_stress=equi_stress, vasp=False
         )
         res_data["elastic_tensor"] = []
         for ii in range(6):
+            c_ii = []
             for jj in range(6):
-                res_data["elastic_tensor"].append(et.voigt[ii][jj] / 1e4)
+                c_ii.append(et.voigt[ii][jj] / 1e4)
                 ptr_data += "%7.2f " % (et.voigt[ii][jj] / 1e4)
+            res_data["elastic_tensor"].append(c_ii)
             ptr_data += "\n"
 
         BV = et.k_voigt / 1e4
         GV = et.g_voigt / 1e4
         EV = 9 * BV * GV / (3 * BV + GV)
         uV = 0.5 * (3 * BV - 2 * GV) / (3 * BV + GV)
```

### Comparing `apex-flow-1.1.6/apex/core/property/Gamma.py` & `apex_flow-1.2.0/apex/core/property/Gamma.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,86 +24,62 @@
 from dflow.python import upload_packages
 
 upload_packages.append(__file__)
 
 
 class Gamma(Property):
     """
-    Calculation of common gamma lines for bcc and fcc
+    Calculation of gamma lines
     """
 
     def __init__(self, parameter, inter_param=None):
         parameter["reproduce"] = parameter.get("reproduce", False)
         self.reprod = parameter["reproduce"]
         if not self.reprod:
             if not ("init_from_suffix" in parameter and "output_suffix" in parameter):
-                self.plane_miller = parameter.get("plane_miller", None)
-                self.slip_direction = parameter.get("slip_direction", None)
-                self.slip_length = parameter.get("slip_length", None)
-                self.plane_shift = parameter.get("plane_shift", 0)
+                parameter["plane_miller"] = parameter.get("plane_miller", None)
+                self.plane_miller = parameter["plane_miller"]
+                parameter["slip_direction"] = parameter.get("slip_direction", None)
+                self.slip_direction = parameter["slip_direction"]
+                parameter["slip_length"] = parameter.get("slip_length", None)
+                self.slip_length = parameter["slip_length"]
+                parameter["plane_shift"] = parameter.get("plane_shift", 0)
+                self.plane_shift = parameter["plane_shift"]
                 parameter["supercell_size"] = parameter.get("supercell_size", (1, 1, 5))
                 self.supercell_size = parameter["supercell_size"]
                 parameter["vacuum_size"] = parameter.get("vacuum_size", 0)
                 self.vacuum_size = parameter["vacuum_size"]
                 parameter["add_fix"] = parameter.get(
                     "add_fix", ["true", "true", "false"]
                 )  # standard method
                 self.add_fix = parameter["add_fix"]
                 parameter["n_steps"] = parameter.get("n_steps", 10)
                 self.n_steps = parameter["n_steps"]
                 self.atom_num = None
             parameter["cal_type"] = parameter.get("cal_type", "relaxation")
-            self.cal_type = parameter["cal_type"]
             default_cal_setting = {
                 "relax_pos": True,
                 "relax_shape": False,
                 "relax_vol": False,
             }
-            if "cal_setting" not in parameter:
-                parameter["cal_setting"] = default_cal_setting
-            else:
-                if "relax_pos" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_pos"] = default_cal_setting[
-                        "relax_pos"
-                    ]
-                if "relax_shape" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                        "relax_shape"
-                    ]
-                if "relax_vol" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_vol"] = default_cal_setting[
-                        "relax_vol"
-                    ]
-            self.cal_setting = parameter["cal_setting"]
         else:
             parameter["cal_type"] = "static"
             self.cal_type = parameter["cal_type"]
             default_cal_setting = {
                 "relax_pos": False,
                 "relax_shape": False,
                 "relax_vol": False,
             }
-            if "cal_setting" not in parameter:
-                parameter["cal_setting"] = default_cal_setting
-            else:
-                if "relax_pos" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_pos"] = default_cal_setting[
-                        "relax_pos"
-                    ]
-                if "relax_shape" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                        "relax_shape"
-                    ]
-                if "relax_vol" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_vol"] = default_cal_setting[
-                        "relax_vol"
-                    ]
-            self.cal_setting = parameter["cal_setting"]
             parameter["init_from_suffix"] = parameter.get("init_from_suffix", "00")
             self.init_from_suffix = parameter["init_from_suffix"]
+        self.cal_type = parameter["cal_type"]
+        parameter["cal_setting"] = parameter.get("cal_setting", default_cal_setting)
+        for key in default_cal_setting:
+            parameter["cal_setting"].setdefault(key, default_cal_setting[key])
+        self.cal_setting = parameter["cal_setting"]
         self.parameter = parameter
         self.inter_param = inter_param if inter_param != None else {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
             logging.warning("%s already exists" % path_to_work)
@@ -112,75 +88,68 @@
         path_to_equi = os.path.abspath(path_to_equi)
         if "start_confs_path" in self.parameter and os.path.exists(
                 self.parameter["start_confs_path"]
         ):
             init_path_list = glob.glob(
                 os.path.join(self.parameter["start_confs_path"], "*")
             )
-            struct_init_name_list = []
-            for ii in init_path_list:
-                struct_init_name_list.append(ii.split("/")[-1])
-            struct_output_name = path_to_work.split("/")[-2]
-            assert struct_output_name in struct_init_name_list
+            struct_init_name_list = [os.path.basename(ii) for ii in init_path_list]
+            struct_output_name = os.path.basename(os.path.dirname(path_to_work))
+            assert struct_output_name in struct_init_name_list, f"{struct_output_name} not in initial configuration names"
             path_to_equi = os.path.abspath(
                 os.path.join(
                     self.parameter["start_confs_path"],
                     struct_output_name,
                     "relaxation",
                     "relax_task",
                 )
             )
 
         task_list = []
         cwd = os.getcwd()
 
         if self.reprod:
-            print("gamma line reproduce starts")
+            logging.info("gamma line reproduce starts")
             if "init_data_path" not in self.parameter:
                 raise RuntimeError("please provide the initial data path to reproduce")
             init_data_path = os.path.abspath(self.parameter["init_data_path"])
             task_list = make_repro(
                 init_data_path,
                 self.init_from_suffix,
                 path_to_work,
                 self.parameter.get("reprod_last_frame", True),
             )
-            os.chdir(cwd)
 
         else:
             if refine:
-                print("gamma line refine starts")
+                logging.info("gamma line refine starts")
                 task_list = make_refine(
                     self.parameter["init_from_suffix"],
                     self.parameter["output_suffix"],
                     path_to_work,
                 )
-                os.chdir(cwd)
                 # record miller
                 init_from_path = re.sub(
                     self.parameter["output_suffix"][::-1],
                     self.parameter["init_from_suffix"][::-1],
                     path_to_work[::-1],
                     count=1,
                 )[::-1]
                 task_list_basename = list(map(os.path.basename, task_list))
 
                 for ii in task_list_basename:
                     init_from_task = os.path.join(init_from_path, ii)
                     output_task = os.path.join(path_to_work, ii)
                     os.chdir(output_task)
-                    if os.path.isfile("miller.json"):
-                        os.remove("miller.json")
-                    if os.path.islink("miller.json"):
+                    if os.path.exists("miller.json"):
                         os.remove("miller.json")
                     os.symlink(
                         os.path.relpath(os.path.join(init_from_task, "miller.json")),
                         "miller.json",
                     )
-                os.chdir(cwd)
 
             else:
                 if self.inter_param["type"] == "abacus":
                     CONTCAR = abacus_utils.final_stru(path_to_equi)
                     POSCAR = "STRU"
                 else:
                     CONTCAR = "CONTCAR"
@@ -241,66 +210,66 @@
                 # gen initial slab
                 (plane_miller, slip_direction,
                  slip_length, Q) = self.__convert_input_miller(self.conv_std_structure)
                 slab = self.__gen_slab_pmg(self.conv_std_structure, plane_miller, trans_matrix=Q)
                 self.atom_num = len(slab.sites)
 
                 os.chdir(path_to_work)
-                if os.path.isfile(POSCAR):
-                    os.remove(POSCAR)
-                if os.path.islink(POSCAR):
+                if os.path.exists(POSCAR):
                     os.remove(POSCAR)
                 os.symlink(os.path.relpath(equi_contcar), POSCAR)
                 # task_poscar = os.path.join(output, 'POSCAR')
                 count = 0
                 # define slip vector
                 if type(slip_length) == int or type(slip_length) == float:
                     frac_slip_vec = np.array([slip_length, 0, 0]) * relax_a
                 else:
                     # for Sequence[int|float, int|float, int|float] type
                     try:
                         slip_vector_cartesian = np.multiply(np.array(slip_length),
                                                             np.array([relax_a, relax_b, relax_c]))
                         norm_length = np.linalg.norm(slip_vector_cartesian, 2)
                         frac_slip_vec = np.array([norm_length, 0, 0])
-                    except:
+                    except Exception:
                         raise RuntimeError(
                             'Only int | float or '
                             'Sequence[int | float, int | float, int | float] is allowed for the input_length'
                         )
+                self.slip_length = frac_slip_vec[0]
                 # get displaced structure
                 for obtained_slab in self.__displace_slab_generator(slab,
                                                                     disp_vector=frac_slip_vec,
                                                                     is_frac=False):
                     output_task = os.path.join(path_to_work, "task.%06d" % count)
                     os.makedirs(output_task, exist_ok=True)
                     os.chdir(output_task)
                     for jj in ["INCAR", "POTCAR", POSCAR, "conf.lmp", "in.lammps"]:
                         if os.path.exists(jj):
                             os.remove(jj)
                     task_list.append(output_task)
                     # print("# %03d generate " % ii, output_task)
-                    print(
+                    logging.info(
                         "# %03d generate " % count,
                         output_task,
                         " \t %d atoms" % len(obtained_slab.sites)
                     )
                     # make confs
                     obtained_slab.to("POSCAR.tmp", "POSCAR")
                     vasp_utils.regulate_poscar("POSCAR.tmp", "POSCAR")
                     vasp_utils.sort_poscar("POSCAR", "POSCAR", ptypes)
                     if self.inter_param["type"] == "abacus":
                         abacus_utils.poscar2stru("POSCAR", self.inter_param, "STRU")
                         os.remove("POSCAR")
                     # vasp.perturb_xz('POSCAR', 'POSCAR', self.pert_xz)
                     # record miller
                     dumpfn(self.plane_miller, "miller.json")
+                    dumpfn(self.slip_length, 'slip_length.json')
                     count += 1
-                os.chdir(cwd)
-
+        
+        os.chdir(cwd)
         return task_list
 
     def __convert_input_miller(self, structure: Structure):
         plane_miller = tuple(self.plane_miller)
         slip_direction = tuple(self.slip_direction)
         slip_length = self.slip_length
         # get search key string
@@ -463,15 +432,15 @@
         with open(poscar, "w") as fin2:
             for ii in range(len(contents)):
                 fin2.write(contents[ii])
 
     def __stru_fix(self, stru) -> None:
         fix_dict = {"true": True, "false": False}
         fix_xyz = [fix_dict[i] for i in self.addfix]
-        abacus.stru_fix_atom(stru, fix_atom=fix_xyz)
+        abacus_utils.stru_fix_atom(stru, fix_atom=fix_xyz)
 
     def __inLammpes_fix(self, inLammps) -> None:
         # add position fix condition of x and y of in.lammps
         fix_dict = {"true": "0", "false": "NULL"}
         add_fix_str = (
                 "fix             1 all setforce"
                 + " "
@@ -496,15 +465,21 @@
             del contents[lower_id + 1:upper_id - 1]
             contents.insert(lower_id + 1, add_fix_str)
         with open(inLammps, "w") as fin2:
             for ii in range(len(contents)):
                 fin2.write(contents[ii])
 
     def post_process(self, task_list):
-        if self.add_fix:
+        # for no exist of self.add_fix in refine mode, skip post_process
+        try:
+            add_fix = self.add_fix
+        except AttributeError:
+            add_fix = None
+
+        if add_fix:
             count = 0
             for ii in task_list:
                 count += 1
                 inter = os.path.join(ii, "inter.json")
                 poscar = os.path.join(ii, "POSCAR")
                 calc_type = loadfn(inter)["type"]
                 if calc_type == "vasp":
@@ -531,58 +506,58 @@
             """
             ptr_data += (
                 str(tuple(self.miller_index))
                 + " plane along "
                 + str(self.displace_direction)
             )
             """
-            ptr_data += "No_task: \tDisplacement \tStacking_Fault_E(J/m^2) EpA(eV) slab_equi_EpA(eV)\n"
+            ptr_data += "No_task: \tDisplacement \tDisplace_Length(\AA) \tStacking_Fault_E(J/m^2) EpA(eV) slab_equi_EpA(eV)\n"
             all_tasks.sort()
-            task_result_slab_equi = loadfn(
-                os.path.join(all_tasks[0], "result_task.json")
+            n_steps = len(all_tasks) - 1
+            task_result_slab_equi = loadfn(os.path.join(all_tasks[0], "result_task.json"))
+            slip_length = loadfn(os.path.join(all_tasks[0], "slip_length.json"))
+            equi_path = os.path.abspath(
+                os.path.join(
+                    os.path.dirname(output_file), "../relaxation/relax_task"
+                )
+            )
+            equi_result = loadfn(os.path.join(equi_path, "result.json"))
+            equi_epa = equi_result["energies"][-1] / np.sum(
+                equi_result["atom_numbs"]
             )
             for ii in all_tasks:
                 task_result = loadfn(os.path.join(ii, "result_task.json"))
                 natoms = np.sum(task_result["atom_numbs"])
                 epa = task_result["energies"][-1] / natoms
                 equi_epa_slab = task_result_slab_equi["energies"][-1] / natoms
                 AA = np.linalg.norm(
                     np.cross(task_result["cells"][0][0], task_result["cells"][0][1])
                 )
-
-                equi_path = os.path.abspath(
-                    os.path.join(
-                        os.path.dirname(output_file), "../relaxation/relax_task"
-                    )
-                )
-                equi_result = loadfn(os.path.join(equi_path, "result.json"))
-                equi_epa = equi_result["energies"][-1] / np.sum(
-                    equi_result["atom_numbs"]
-                )
+               
                 structure_dir = os.path.basename(ii)
-
                 Cf = 1.60217657e-16 / 1e-20 * 0.001
                 sfe = (
                         (
                                 task_result["energies"][-1]
                                 - task_result_slab_equi["energies"][-1]
                         )
                         / AA
                         * Cf
                 )
-
+                frac = int(ii[-4:]) / n_steps
                 miller_index = loadfn(os.path.join(ii, "miller.json"))
-                ptr_data += "%-25s     %7.2f   %7.3f    %8.3f %8.3f\n" % (
+                ptr_data += "%-25s    %7.2f   %7.3f  %7.3f    %8.3f %8.3f\n" % (
                     str(miller_index) + "-" + structure_dir + ":",
-                    int(ii[-4:]) / self.n_steps,
+                    frac,
+                    (slip_length * frac),
                     sfe,
                     epa,
                     equi_epa_slab,
                 )
-                res_data[int(ii[-4:]) / self.n_steps] = [sfe, epa, equi_epa]
+                res_data[frac] = [(slip_length * frac), sfe, epa, equi_epa]
 
         else:
             if "init_data_path" not in self.parameter:
                 raise RuntimeError("please provide the initial data path to reproduce")
             init_data_path = os.path.abspath(self.parameter["init_data_path"])
             res_data, ptr_data = post_repro(
                 init_data_path,
```

### Comparing `apex-flow-1.1.6/apex/core/property/Interstitial.py` & `apex_flow-1.2.0/apex/core/property/Interstitial.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,139 +1,115 @@
 import glob
 import json
 import logging
 import os
 import re
+import shutil
 
 import numpy as np
 from monty.serialization import dumpfn, loadfn
-from pymatgen.analysis.defects.generators import InterstitialGenerator
+from pymatgen.analysis.defects.generators import VoronoiInterstitialGenerator
+from pymatgen.analysis.defects.core import Interstitial as pmgInterstitial
 from pymatgen.core.structure import Structure
+from pymatgen.core.sites import PeriodicSite
 
 from apex.core.calculator.lib import abacus_utils
 from apex.core.calculator.lib import lammps_utils
 from apex.core.property.Property import Property
 from apex.core.refine import make_refine
 from apex.core.reproduce import make_repro, post_repro
 from apex.core.structure import StructureInfo
 from dflow.python import upload_packages
+
 upload_packages.append(__file__)
 
+PREDEFINED_LIST = ['bcc', 'fcc', 'hcp']
 
 class Interstitial(Property):
     def __init__(self, parameter, inter_param=None):
         parameter["reproduce"] = parameter.get("reproduce", False)
         self.reprod = parameter["reproduce"]
         if not self.reprod:
             if not ("init_from_suffix" in parameter and "output_suffix" in parameter):
                 default_supercell = [1, 1, 1]
                 parameter["supercell"] = parameter.get("supercell", default_supercell)
                 self.supercell = parameter["supercell"]
                 self.insert_ele = parameter["insert_ele"]
+                parameter["lattice_type"] = parameter.get("lattice_type", None)
+                self.lattice_type = parameter["lattice_type"]
+                parameter["voronoi_param"] = parameter.get("voronoi_param", {})
+                self.voronoi_param = parameter["voronoi_param"]
             parameter["cal_type"] = parameter.get("cal_type", "relaxation")
-            self.cal_type = parameter["cal_type"]
             default_cal_setting = {
                 "relax_pos": True,
                 "relax_shape": True,
                 "relax_vol": True,
             }
-            if "cal_setting" not in parameter:
-                parameter["cal_setting"] = default_cal_setting
-            else:
-                if "relax_pos" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_pos"] = default_cal_setting[
-                        "relax_pos"
-                    ]
-                if "relax_shape" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                        "relax_shape"
-                    ]
-                if "relax_vol" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_vol"] = default_cal_setting[
-                        "relax_vol"
-                    ]
-            self.cal_setting = parameter["cal_setting"]
         else:
             parameter["cal_type"] = "static"
-            self.cal_type = parameter["cal_type"]
             default_cal_setting = {
                 "relax_pos": False,
                 "relax_shape": False,
                 "relax_vol": False,
             }
-            if "cal_setting" not in parameter:
-                parameter["cal_setting"] = default_cal_setting
-            else:
-                if "relax_pos" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_pos"] = default_cal_setting[
-                        "relax_pos"
-                    ]
-                if "relax_shape" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                        "relax_shape"
-                    ]
-                if "relax_vol" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_vol"] = default_cal_setting[
-                        "relax_vol"
-                    ]
-            self.cal_setting = parameter["cal_setting"]
             parameter["init_from_suffix"] = parameter.get("init_from_suffix", "00")
             self.init_from_suffix = parameter["init_from_suffix"]
+        self.cal_type = parameter["cal_type"]
+        parameter["cal_setting"] = parameter.get("cal_setting", default_cal_setting)
+        for key in default_cal_setting:
+            parameter["cal_setting"].setdefault(key, default_cal_setting[key])
+        self.cal_setting = parameter["cal_setting"]
         self.parameter = parameter
         self.inter_param = inter_param if inter_param != None else {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         self.path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
             logging.warning("%s already exists" % path_to_work)
-            # dlog.warning("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
 
         if "start_confs_path" in self.parameter and os.path.exists(
-            self.parameter["start_confs_path"]
+                self.parameter["start_confs_path"]
         ):
             init_path_list = glob.glob(
                 os.path.join(self.parameter["start_confs_path"], "*")
             )
-            struct_init_name_list = []
-            for ii in init_path_list:
-                struct_init_name_list.append(ii.split("/")[-1])
-            struct_output_name = self.path_to_work.split("/")[-2]
-            assert struct_output_name in struct_init_name_list
+            struct_init_name_list = [os.path.basename(ii) for ii in init_path_list]
+            struct_output_name = os.path.basename(os.path.dirname(path_to_work))
+            assert struct_output_name in struct_init_name_list, f"{struct_output_name} not in initial configurations"
             path_to_equi = os.path.abspath(
                 os.path.join(
                     self.parameter["start_confs_path"],
                     struct_output_name,
                     "relaxation",
                     "relax_task",
                 )
             )
 
         self.task_list = []
         cwd = os.getcwd()
 
         if self.reprod:
-            print("interstitial reproduce starts")
+            logging.info("interstitial reproduce starts")
             if "init_data_path" not in self.parameter:
                 raise RuntimeError("please provide the initial data path to reproduce")
             init_data_path = os.path.abspath(self.parameter["init_data_path"])
             self.task_list = make_repro(
                 self.inter_param,
                 init_data_path,
                 self.init_from_suffix,
                 self.path_to_work,
                 self.parameter.get("reprod_last_frame", False),
             )
-            os.chdir(cwd)
 
         else:
             if refine:
-                print("interstitial refine starts")
+                logging.info("interstitial refine starts")
                 self.task_list = make_refine(
                     self.parameter["init_from_suffix"],
                     self.parameter["output_suffix"],
                     self.path_to_work,
                 )
 
                 init_from_path = re.sub(
@@ -141,106 +117,113 @@
                     self.parameter["init_from_suffix"][::-1],
                     self.path_to_work[::-1],
                     count=1,
                 )[::-1]
                 task_list_basename = list(map(os.path.basename, self.task_list))
 
                 os.chdir(self.path_to_work)
-                if os.path.isfile("element.out"):
-                    os.remove("element.out")
-                if os.path.islink("element.out"):
+                if os.path.exists("element.out"):
                     os.remove("element.out")
                 os.symlink(
                     os.path.relpath(os.path.join(init_from_path, "element.out")),
                     "element.out",
                 )
                 os.chdir(cwd)
 
                 for ii in task_list_basename:
                     init_from_task = os.path.join(init_from_path, ii)
                     output_task = os.path.join(self.path_to_work, ii)
                     os.chdir(output_task)
-                    if os.path.isfile("supercell.json"):
-                        os.remove("supercell.json")
-                    if os.path.islink("supercell.json"):
+                    if os.path.exists("supercell.json"):
                         os.remove("supercell.json")
                     os.symlink(
                         os.path.relpath(os.path.join(init_from_task, "supercell.json")),
                         "supercell.json",
                     )
-                os.chdir(cwd)
 
             else:
                 if self.inter_param["type"] == "abacus":
                     CONTCAR = abacus_utils.final_stru(path_to_equi)
                     POSCAR = "STRU"
                 else:
                     CONTCAR = "CONTCAR"
                     POSCAR = "POSCAR"
 
                 equi_contcar = os.path.join(path_to_equi, CONTCAR)
+                orig_poscar = os.path.join(path_to_equi, POSCAR)
                 if not os.path.exists(equi_contcar):
                     raise RuntimeError("please do relaxation first")
 
                 if self.inter_param["type"] == "abacus":
                     ss = abacus_utils.stru2Structure(equi_contcar)
                 else:
                     ss = Structure.from_file(equi_contcar)
 
                 # get structure type
                 os.chdir(self.path_to_work)
-                ss.to("POSCAR", "POSCAR")
-                st = StructureInfo(ss)
+                # convert site element into same type for a pseudo-structure just for simple lattice type judgment
+                same_type_ss = ss.copy()
+                species_mapping = {str(specie): "Ni" for specie in same_type_ss.composition.elements}
+                same_type_ss.replace_species(species_mapping)
+                st = StructureInfo(same_type_ss, symprec=0.1, angle_tolerance=5)
+                # indication of structure type
                 self.structure_type = st.lattice_structure
+                # get conventional standard structure to ss
+                orig_st = StructureInfo(ss, symprec=0.1, angle_tolerance=5)
+                conv_ss = orig_st.conventional_structure
+                conv_ss.to("POSCAR", "POSCAR")
+                ss = conv_ss
+                if self.lattice_type:
+                    logging.info(msg=f'Adopt user indicated lattice type: {self.lattice_type}')
+                    self.structure_type = self.lattice_type
                 os.chdir(cwd)
 
                 # gen defects
                 dss = []
                 self.insert_element_task = os.path.join(self.path_to_work, "element.out")
                 if os.path.isfile(self.insert_element_task):
                     os.remove(self.insert_element_task)
-
                 for ii in self.insert_ele:
-                    pre_vds = InterstitialGenerator()
-                    vds = pre_vds.generate(ss, {ii: [[0.1, 0.1, 0.1]]})
+                    if self.structure_type in PREDEFINED_LIST:
+                        # produce a pseudo interstitial structure for later modification
+                        vds = [pmgInterstitial(ss, PeriodicSite(ii, [0.12, 0.13, 0.14], ss.lattice))]
+                    else:
+                        pre_vds = VoronoiInterstitialGenerator(**self.voronoi_param)
+                        vds = pre_vds.generate(ss, [ii])
                     for jj in vds:
                         temp = jj.get_supercell_structure(
                             sc_mat=np.diag(self.supercell, k=0)
                         )
                         smallest_distance = list(set(temp.distance_matrix.ravel()))[1]
                         if (
-                            "conf_filters" in self.parameter
-                            and "min_dist" in self.parameter["conf_filters"]
+                                "conf_filters" in self.parameter
+                                and "min_dist" in self.parameter["conf_filters"]
                         ):
                             min_dist = self.parameter["conf_filters"]["min_dist"]
                             if smallest_distance >= min_dist:
                                 dss.append(temp)
                                 with open(self.insert_element_task, "a+") as fout:
                                     print(ii, file=fout)
                         else:
                             dss.append(temp)
                             with open(self.insert_element_task, "a+") as fout:
                                 print(ii, file=fout)
-                #            dss.append(jj.generate_defect_structure(self.supercell))
+                        #            dss.append(jj.generate_defect_structure(self.supercell))
                         self.dss = dss
 
-                print(
+                logging.info(
                     "gen interstitial with supercell "
                     + str(self.supercell)
                     + " with element "
                     + str(self.insert_ele)
                 )
                 os.chdir(self.path_to_work)
-                if os.path.isfile(POSCAR):
-                    os.remove(POSCAR)
-                if os.path.islink(POSCAR):
+                if os.path.exists(POSCAR):
                     os.remove(POSCAR)
                 os.symlink(os.path.relpath(equi_contcar), POSCAR)
-                #           task_poscar = os.path.join(output, 'POSCAR')
-
                 for ii in range(len(dss)):
                     output_task = os.path.join(self.path_to_work, "task.%06d" % ii)
                     os.makedirs(output_task, exist_ok=True)
                     os.chdir(output_task)
                     for jj in [
                         "INCAR",
                         "POTCAR",
@@ -251,136 +234,159 @@
                     ]:
                         if os.path.exists(jj):
                             os.remove(jj)
                     self.task_list.append(output_task)
                     dss[ii].to("POSCAR", "POSCAR")
                     # np.savetxt('supercell.out', self.supercell, fmt='%d')
                     dumpfn(self.supercell, "supercell.json")
+                    dumpfn(f'VoronoiType_{ii}', 'interstitial_type.json')
                 os.chdir(cwd)
 
                 super_size = (
                         self.supercell[0] * self.supercell[1] * self.supercell[2]
                 )
                 num_atom = super_size * 2
-                #chl = -num_atom - 2
+                # chl = -num_atom - 2
                 os.chdir(self.path_to_work)
 
-                if not os.path.isfile("task.000000/POSCAR"):
-                    raise RuntimeError("need task.000000 structure as reference")
+                # create pre-defined special SIA structure for bcc fcc and hcp
+                if self.structure_type in PREDEFINED_LIST:
+                    if not os.path.isfile("task.000000/POSCAR"):
+                        raise RuntimeError("need task.000000 structure as reference")
+
+                    with open('POSCAR', "r") as fin:
+                        fin.readline()
+                        scale = float(fin.readline().split()[0])
+                        self.latt_param = float(fin.readline().split()[0])
+                        self.latt_param *= scale
 
-                with open('POSCAR', "r") as fin:
-                    fin.readline()
-                    scale = float(fin.readline().split()[0])
-                    self.latt_param = float(fin.readline().split()[0])
-                    self.latt_param *= scale
-
-                with open("task.000000/POSCAR", "r") as fin:
-                    self.pos_line = fin.read().split("\n")
-
-
-                self.super_latt_param = float(self.pos_line[2].split()[0])
-                self.unit_frac = self.latt_param / self.super_latt_param
-
-                for idx, ii in enumerate(self.pos_line):
-                    ss = ii.split()
-                    if len(ss) > 3:
-                        if (
-                                abs(self.unit_frac * 0.1 - float(ss[0])) < 1e-5
-                                and abs(self.unit_frac * 0.1 - float(ss[1])) < 1e-5
-                                and abs(self.unit_frac * 0.1 - float(ss[2])) < 1e-5
-                        ):
-                            chl = idx
-
-                os.chdir(cwd)
-
-                # specify interstitial structures
-                if self.structure_type == 'bcc':
-                    for idx, ii in enumerate(self.pos_line):
-                        ss = ii.split()
-                        if len(ss) > 3:
-                            if (
-                                    abs(self.unit_frac * 0.5 - float(ss[0])) < 1e-5
-                                    and abs(self.unit_frac * 0.5 - float(ss[1])) < 1e-5
-                                    and abs(self.unit_frac * 0.5 - float(ss[2])) < 1e-5
-                            ):
-                                center = idx
-                    bcc_interstital_dict = {
-                        'tetrahedral':   {chl: [0.25, 0.5, 0]},
-                        'octahedral':    {chl: [0.5, 0.5, 0]},
-                        'crowdion':      {chl: [0.25, 0.25, 0]},
-                        '<111>dumbbell': {chl: [1/3, 1/3, 1/3],
-                                          center: [2/3, 2/3, 2/3]},
-                        '<110>dumbbell': {chl: [1/4, 3/4, 1/2],
-                                          center: [3/4, 1/4, 1/2]},
-                        '<100>dumbbell': {chl: [1/2, 1/2, 1/6],
-                                          center: [1/2, 1/2, 5/6]}
-                    }
-                    total_task = self.__gen_tasks(bcc_interstital_dict)
+                    with open("task.000000/POSCAR", "r") as fin:
+                        self.pos_line = fin.read().split("\n")
 
-                elif self.structure_type == 'fcc':
                     for idx, ii in enumerate(self.pos_line):
                         ss = ii.split()
                         if len(ss) > 3:
                             if (
-                                    abs(self.unit_frac * 1 - float(ss[0])) < 1e-5
-                                    and abs(self.unit_frac * 0.5 - float(ss[1])) < 1e-5
-                                    and abs(self.unit_frac * 0.5 - float(ss[2])) < 1e-5
-                            ):
-                                face = idx
-
-                            if (
-                                    abs(self.unit_frac * 1 - float(ss[0])) < 1e-5
-                                    and abs(self.unit_frac * 1 - float(ss[1])) < 1e-5
-                                    and abs(self.unit_frac * 1 - float(ss[2])) < 1e-5
+                                    abs(0.12 / self.supercell[0] - float(ss[0])) < 1e-5
+                                    and abs(0.13 / self.supercell[1] - float(ss[1])) < 1e-5
+                                    and abs(0.14 / self.supercell[2] - float(ss[2])) < 1e-5
                             ):
-                                corner = idx
-
-                    fcc_interstital_dict = {
-                        'tetrahedral':      {chl: [0.75, 0.25, 0.25]},
-                        'octahedral':       {chl: [1, 0, 0.5]},
-                        'crowdion':         {chl: [1, 0.25, 0.25]},
-                        '<111>dumbbell':    {
-                            chl: [1-0.3/np.sqrt(3),
-                                    1-0.3/np.sqrt(3),
-                                    1-0.3/np.sqrt(3)],
-                            corner: [0.3/np.sqrt(3),
-                                    0.3/np.sqrt(3),
-                                    0.3/np.sqrt(3)]
-                        },
-                        '<110>dumbbell': {
-                            chl: [1,
-                                    0.5+(0.3/np.sqrt(2)),
-                                    0.5+(0.3/np.sqrt(2))],
-                            face: [1,
-                                    0.5-(0.3/np.sqrt(2)),
-                                    0.5-(0.3/np.sqrt(2))]
-                        },
-                        '<100>dumbbell': {
-                            chl: [1, 0.2, 0.5],
-                            face: [1, 0.8, 0.5]
-                        },
-                    }
-                    total_task = self.__gen_tasks(fcc_interstital_dict)
+                                chl = idx
+                    # pseudo-task only run original POSCAR to save calculation resources
+                    shutil.copyfile("POSCAR", "task.000000/POSCAR")
 
-                elif self.structure_type == 'hcp':
-                    pass
+                    os.chdir(cwd)
+                    # specify interstitial structures
+                    if self.structure_type == 'bcc':
+                        for idx, ii in enumerate(self.pos_line):
+                            ss = ii.split()
+                            if len(ss) > 3:
+                                if (
+                                        abs(0.5 / self.supercell[0] - float(ss[0])) < 1e-5
+                                        and abs(0.5 / self.supercell[1] - float(ss[1])) < 1e-5
+                                        and abs(0.5 / self.supercell[2] - float(ss[2])) < 1e-5
+                                ):
+                                    center = idx
+                        bcc_interstital_dict = {
+                            'tetrahedral': {chl: [0.25, 0.5, 0]},
+                            'octahedral': {chl: [0.5, 0.5, 0]},
+                            'crowdion': {chl: [0.25, 0.25, 0]},
+                            '<111>dumbbell': {chl: [1 / 3, 1 / 3, 1 / 3],
+                                              center: [2 / 3, 2 / 3, 2 / 3]},
+                            '<110>dumbbell': {chl: [1 / 4, 3 / 4, 1 / 2],
+                                              center: [3 / 4, 1 / 4, 1 / 2]},
+                            '<100>dumbbell': {chl: [1 / 2, 1 / 2, 1 / 6],
+                                              center: [1 / 2, 1 / 2, 5 / 6]}
+                        }
+                        total_task = self.__gen_tasks(bcc_interstital_dict)
+
+                    elif self.structure_type == 'fcc':
+                        for idx, ii in enumerate(self.pos_line):
+                            ss = ii.split()
+                            if len(ss) > 3:
+                                if (
+                                        abs(1 / self.supercell[0] - float(ss[0])) < 1e-5
+                                        and abs(0.5 / self.supercell[1] - float(ss[1])) < 1e-5
+                                        and abs(0.5 / self.supercell[2] - float(ss[2])) < 1e-5
+                                ):
+                                    face = idx
+
+                                if (
+                                        abs(1 / self.supercell[0] - float(ss[0])) < 1e-5
+                                        and abs(1 / self.supercell[1] - float(ss[1])) < 1e-5
+                                        and abs(1 / self.supercell[2] - float(ss[2])) < 1e-5
+                                ):
+                                    corner = idx
+
+                        fcc_interstital_dict = {
+                            'tetrahedral': {chl: [0.75, 0.25, 0.25]},
+                            'octahedral': {chl: [1, 0, 0.5]},
+                            'crowdion': {chl: [1, 0.25, 0.25]},
+                            '<111>dumbbell': {
+                                chl: [1 - 0.3 / np.sqrt(3),
+                                      1 - 0.3 / np.sqrt(3),
+                                      1 - 0.3 / np.sqrt(3)],
+                                corner: [0.3 / np.sqrt(3),
+                                         0.3 / np.sqrt(3),
+                                         0.3 / np.sqrt(3)]
+                            },
+                            '<110>dumbbell': {
+                                chl: [1,
+                                      0.5 + (0.3 / np.sqrt(2)),
+                                      0.5 + (0.3 / np.sqrt(2))],
+                                face: [1,
+                                       0.5 - (0.3 / np.sqrt(2)),
+                                       0.5 - (0.3 / np.sqrt(2))]
+                            },
+                            '<100>dumbbell': {
+                                chl: [1, 0.2, 0.5],
+                                face: [1, 0.8, 0.5]
+                            },
+                        }
+                        total_task = self.__gen_tasks(fcc_interstital_dict)
+
+                    elif self.structure_type == 'hcp':
+                        for idx, ii in enumerate(self.pos_line):
+                            ss = ii.split()
+                            if len(ss) > 3:
+                                if (
+                                        abs(1/3 / self.supercell[0] - float(ss[0])) < 1e-5
+                                        and abs(2/3 / self.supercell[1] - float(ss[1])) < 1e-5
+                                        and abs(0.25 / self.supercell[2] - float(ss[2])) < 1e-5
+                                ):
+                                    center = idx
+                        hcp_interstital_dict = {
+                            'O': {chl: [0, 0, 0.5]},
+                            'BO': {chl: [0, 0, 0.25]},
+                            'C': {chl: [0.5, 0.5, 0.5]},
+                            'BC': {chl: [5/6, 2/3, 0.25]},
+                            'S': {
+                                chl: [1/3, 2/3, 0.475],
+                                center: [1/3, 2/3, 0.025]
+                            },
+                            'BS': {
+                                chl: [2/3, 2/3, 0.25],
+                                center: [0, 2/3, 0.25]
+                            },
+                            'T': {chl: [2/3, 1/3, 0.375]},
+                            'BT': {chl: [2/3, 1/3, 0.25]},
+                        }
+                        total_task = self.__gen_tasks(hcp_interstital_dict)
                 else:
                     total_task = len(dss)
 
                 if self.inter_param["type"] == "abacus":
                     for ii in range(total_task):
                         output_task = os.path.join(self.path_to_work, "task.%06d" % ii)
                         os.chdir(output_task)
                         abacus_utils.poscar2stru("POSCAR", self.inter_param, "STRU")
                         os.remove("POSCAR")
-                    os.chdir(cwd)
-
+        os.chdir(cwd)
         return self.task_list
 
-
     def __gen_tasks(self, interstitial_dict):
         cwd = os.getcwd()
         for ii, (type_str, adjust_dict) in enumerate(interstitial_dict.items()):
             output_task = os.path.join(
                 self.path_to_work, "task.%06d" % (len(self.dss) + ii)
             )
             os.makedirs(output_task, exist_ok=True)
@@ -390,26 +396,26 @@
             with open(self.insert_element_task, "a+") as fout:
                 print(self.insert_ele[0], file=fout)
             dumpfn(self.supercell, "supercell.json")
             dumpfn(type_str, 'interstitial_type.json')
             new_pos_line = self.pos_line.copy()
             for line, pos in adjust_dict.items():
                 new_pos_line[line] = (
-                        "%.6f" % float(self.unit_frac * pos[0])
+                        "%.6f" % float(pos[0] / self.supercell[0])
                         + " "
-                        + "%.6f" % float(self.unit_frac * pos[1])
+                        + "%.6f" % float(pos[1] / self.supercell[1])
                         + " "
-                        + "%.6f" % float(self.unit_frac * pos[2])
+                        + "%.6f" % float(pos[2] / self.supercell[2])
                         + " "
                         + self.insert_ele[0]
                 )
             with open("POSCAR", "w+") as fout:
                 for ii in new_pos_line:
                     print(ii, file=fout)
-            print(f"gen {type_str}")
+            logging.info(f"gen {type_str}")
             os.chdir(cwd)
 
         total_task = len(self.dss) + len(interstitial_dict)
 
         return total_task
 
     def post_process(self, task_list):
@@ -425,19 +431,19 @@
                         insert_line = conf_line[-2]
                     type_map = loadfn(inter)["type_map"]
                     type_map_list = lammps_utils.element_list(type_map)
                     if int(insert_line.split()[1]) > len(type_map_list):
                         type_num = type_map[insert_ele] + 1
                         conf_line[2] = str(len(type_map_list)) + " atom types"
                         conf_line[-2] = (
-                            "%6.d" % int(insert_line.split()[0])
-                            + "%7.d" % type_num
-                            + "%16.10f" % float(insert_line.split()[2])
-                            + "%16.10f" % float(insert_line.split()[3])
-                            + "%16.10f" % float(insert_line.split()[4])
+                                "%6.d" % int(insert_line.split()[0])
+                                + "%7.d" % type_num
+                                + "%16.10f" % float(insert_line.split()[2])
+                                + "%16.10f" % float(insert_line.split()[3])
+                                + "%16.10f" % float(insert_line.split()[4])
                         )
                         with open(conf, "w+") as fout:
                             for jj in conf_line:
                                 print(jj, file=fout)
             fin1.close()
 
     def task_type(self):
@@ -449,45 +455,45 @@
     def _compute_lower(self, output_file, all_tasks, all_res):
         output_file = os.path.abspath(output_file)
         res_data = {}
         ptr_data = os.path.dirname(output_file) + "\n"
 
         if not self.reprod:
             with open(
-                os.path.join(os.path.dirname(output_file), "element.out"), "r"
+                    os.path.join(os.path.dirname(output_file), "element.out"), "r"
             ) as fin:
                 fc = fin.read().split("\n")
-            ptr_data += "Insert_ele-Struct: Inter_E(eV)  E(eV) equi_E(eV)\n"
-            idid = -1
-            for ii in all_tasks:
-                idid += 1
+            ptr_data += "Insert_ele-Struct:          \tInter_E(eV)    \tE(eV)     \tequi_E(eV)\n"
+
+            equi_path = os.path.abspath(
+                os.path.join(
+                    os.path.dirname(output_file), "../relaxation/relax_task"
+                )
+            )
+            equi_result = loadfn(os.path.join(equi_path, "result.json"))
+            equi_epa = equi_result["energies"][-1] / sum(equi_result["atom_numbs"])
+
+            for idid, ii in enumerate(all_tasks[1:], start=1): # skip task.000000
                 structure_dir = os.path.basename(ii)
                 task_result = loadfn(all_res[idid])
-                natoms = task_result["atom_numbs"][0]
-                equi_path = os.path.abspath(
-                    os.path.join(
-                        os.path.dirname(output_file), "../relaxation/relax_task"
-                    )
-                )
-                equi_result = loadfn(os.path.join(equi_path, "result.json"))
-                equi_epa = equi_result["energies"][-1] / equi_result["atom_numbs"][0]
+                interstitial_type = loadfn(os.path.join(ii, 'interstitial_type.json'))
+                natoms = sum(task_result["atom_numbs"])
                 evac = task_result["energies"][-1] - equi_epa * natoms
-
                 supercell_index = loadfn(os.path.join(ii, "supercell.json"))
                 # insert_ele = loadfn(os.path.join(ii, 'task.json'))['insert_ele'][0]
                 insert_ele = fc[idid]
-                ptr_data += "%s: %7.3f  %7.3f %7.3f \n" % (
-                    insert_ele + "-" + str(supercell_index) + "-" + structure_dir,
+                ptr_data += "%s: \t%7.3f  \t%7.3f \t%7.3f \n" % (
+                    insert_ele + "_" + str(interstitial_type) + "_" + structure_dir,
                     evac,
                     task_result["energies"][-1],
                     equi_epa * natoms,
                 )
                 res_data[
-                    insert_ele + "-" + str(supercell_index) + "-" + structure_dir
-                ] = [evac, task_result["energies"][-1], equi_epa * natoms]
+                    insert_ele + "_" + str(interstitial_type) + "_" + structure_dir
+                    ] = [evac, task_result["energies"][-1], equi_epa * natoms]
 
         else:
             if "init_data_path" not in self.parameter:
                 raise RuntimeError("please provide the initial data path to reproduce")
             init_data_path = os.path.abspath(self.parameter["init_data_path"])
             res_data, ptr_data = post_repro(
                 init_data_path,
```

### Comparing `apex-flow-1.1.6/apex/core/property/Phonon.py` & `apex_flow-1.2.0/apex/core/property/Phonon.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import glob
 import json
 import logging
 import os
 import shutil
 import re
 import subprocess
+from typing import List, Dict, Any
+
 import dpdata
+import seekpath
 from pathlib import Path
+from monty.serialization import dumpfn, loadfn
 from pymatgen.core.structure import Structure
 
 from apex.core.structure import StructureInfo
-from apex.core.calculator.calculator import LAMMPS_TYPE
+from apex.core.calculator.calculator import LAMMPS_INTER_TYPE
 from apex.core.calculator.lib import abacus_utils
 from apex.core.calculator.lib import vasp_utils
 from apex.core.property.Property import Property
 from apex.core.refine import make_refine
 from apex.core.reproduce import make_repro, post_repro
 from dflow.python import upload_packages
 upload_packages.append(__file__)
@@ -22,123 +26,109 @@
 
 class Phonon(Property):
     def __init__(self, parameter, inter_param=None):
         parameter["reproduce"] = parameter.get("reproduce", False)
         self.reprod = parameter["reproduce"]
         if not self.reprod:
             if not ("init_from_suffix" in parameter and "output_suffix" in parameter):
-                self.primitive = parameter.get('primitive', False)
-                self.approach = parameter.get('approach', 'linear')
-                self.supercell_size = parameter.get('supercell_size', [2, 2, 2])
-                self.MESH = parameter.get('MESH', None)
-                self.PRIMITIVE_AXES = parameter.get('PRIMITIVE_AXES', None)
-                self.BAND = parameter.get('BAND', None)
-                self.BAND_POINTS = parameter.get('BAND_POINTS', None)
-                self.BAND_CONNECTION = parameter.get('BAND_CONNECTION', True)
+                parameter["primitive"] = parameter.get('primitive', False)
+                self.primitive = parameter["primitive"]
+                parameter["approach"] = parameter.get('approach', 'linear')
+                self.approach = parameter["approach"]
+                parameter["supercell_size"] = parameter.get('supercell_size', [2, 2, 2])
+                self.supercell_size = parameter["supercell_size"]
+                parameter["seekpath_from_original"] = parameter.get('seekpath_from_original', False)
+                self.seekpath_from_original = parameter["seekpath_from_original"]
+                parameter["seekpath_param"] = parameter.get('seekpath_param', {})
+                self.seekpath_param = parameter["seekpath_param"]
+                parameter["MESH"] = parameter.get('MESH', None)
+                self.MESH = parameter["MESH"]
+                parameter["PRIMITIVE_AXES"] = parameter.get('PRIMITIVE_AXES', None)
+                self.PRIMITIVE_AXES = parameter["PRIMITIVE_AXES"]
+                parameter["BAND"] = parameter.get('BAND', None)
+                self.BAND = parameter["BAND"]
+                parameter["BAND_LABELS"] = parameter.get('BAND_LABELS', None)
+                if self.BAND:
+                    self.BAND_LABELS = parameter["BAND_LABELS"]
+                else:
+                    self.BAND_LABELS = None
+                parameter["BAND_POINTS"] = parameter.get('BAND_POINTS', None)
+                self.BAND_POINTS = parameter["BAND_POINTS"]
+                parameter["BAND_CONNECTION"] = parameter.get('BAND_CONNECTION', True)
+                self.BAND_CONNECTION = parameter["BAND_CONNECTION"]
             parameter["cal_type"] = parameter.get("cal_type", "relaxation")
-            self.cal_type = parameter["cal_type"]
             default_cal_setting = {
                 "relax_pos": True,
                 "relax_shape": False,
                 "relax_vol": False,
             }
-            if "cal_setting" not in parameter:
-                parameter["cal_setting"] = default_cal_setting
-            else:
-                if "relax_pos" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_pos"] = default_cal_setting[
-                        "relax_pos"
-                    ]
-                if "relax_shape" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                        "relax_shape"
-                    ]
-                if "relax_vol" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_vol"] = default_cal_setting[
-                        "relax_vol"
-                    ]
-            self.cal_setting = parameter["cal_setting"]
         else:
             parameter["cal_type"] = "static"
             self.cal_type = parameter["cal_type"]
             default_cal_setting = {
                 "relax_pos": False,
                 "relax_shape": False,
                 "relax_vol": False,
             }
-            if "cal_setting" not in parameter:
-                parameter["cal_setting"] = default_cal_setting
-            else:
-                if "relax_pos" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_pos"] = default_cal_setting[
-                        "relax_pos"
-                    ]
-                if "relax_shape" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                        "relax_shape"
-                    ]
-                if "relax_vol" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_vol"] = default_cal_setting[
-                        "relax_vol"
-                    ]
-            self.cal_setting = parameter["cal_setting"]
             parameter["init_from_suffix"] = parameter.get("init_from_suffix", "00")
             self.init_from_suffix = parameter["init_from_suffix"]
+        self.cal_type = parameter["cal_type"]
+        parameter["cal_setting"] = parameter.get("cal_setting", default_cal_setting)
+        for key in default_cal_setting:
+            parameter["cal_setting"].setdefault(key, default_cal_setting[key])
+        self.cal_setting = parameter["cal_setting"]
         self.parameter = parameter
         self.inter_param = inter_param if inter_param is not None else {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
-            #dlog.warning("%s already exists" % path_to_work)
             logging.warning("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
 
         if "start_confs_path" in self.parameter and os.path.exists(
             self.parameter["start_confs_path"]
         ):
             init_path_list = glob.glob(
                 os.path.join(self.parameter["start_confs_path"], "*")
             )
-            struct_init_name_list = []
-            for ii in init_path_list:
-                struct_init_name_list.append(ii.split("/")[-1])
-            struct_output_name = path_to_work.split("/")[-2]
-            assert struct_output_name in struct_init_name_list
+            struct_init_name_list = [os.path.basename(ii) for ii in init_path_list]
+            struct_output_name = os.path.basename(os.path.dirname(path_to_work))
+            assert struct_output_name in struct_init_name_list, f"{struct_output_name} not in initial configuration names"
             path_to_equi = os.path.abspath(
                 os.path.join(
                     self.parameter["start_confs_path"],
                     struct_output_name,
                     "relaxation",
                     "relax_task",
                 )
             )
 
         task_list = []
         cwd = os.getcwd()
 
         if self.reprod:
-            print("phonon reproduce starts")
+            logging.info("phonon reproduce starts")
             if "init_data_path" not in self.parameter:
                 raise RuntimeError("please provide the initial data path to reproduce")
             init_data_path = os.path.abspath(self.parameter["init_data_path"])
             task_list = make_repro(
                 self.inter_param,
                 init_data_path,
                 self.init_from_suffix,
                 path_to_work,
                 self.parameter.get("reprod_last_frame", True),
             )
             os.chdir(cwd)
 
         else:
             if refine:
-                print("phonon refine starts")
+                logging.info("phonon refine starts")
                 task_list = make_refine(
                     self.parameter["init_from_suffix"],
                     self.parameter["output_suffix"],
                     path_to_work,
                 )
                 os.chdir(cwd)
 
@@ -176,23 +166,43 @@
                     self.MESH = type_param.get("MESH", self.MESH)
                     self.PRIMITIVE_AXES = type_param.get("PRIMITIVE_AXES", self.PRIMITIVE_AXES)
                     self.BAND = type_param.get("BAND", self.BAND)
                     self.BAND_POINTS = type_param.get("BAND_POINTS", self.BAND_POINTS)
                     self.BAND_CONNECTION = type_param.get("BAND_CONNECTION", self.BAND_CONNECTION)
 
                 os.chdir(path_to_work)
-                if os.path.isfile(POSCAR):
-                    os.remove(POSCAR)
-                if os.path.islink(POSCAR):
+                if os.path.exists(POSCAR):
                     os.remove(POSCAR)
                 os.symlink(os.path.relpath(equi_contcar), POSCAR)
-                #           task_poscar = os.path.join(output, 'POSCAR')
 
+                # get band path
                 if not self.BAND:
-                    raise RuntimeError('No band_path input for phonon calculation!')
+                    # use seekpath to get band path
+                    if self.seekpath_from_original:
+                        logging.info(msg='Band path (BAND) not indicated, using seekpath from original cell')
+                        sp = seekpath.get_path_orig_cell(
+                            self.get_seekpath_structure(ss),
+                            **self.seekpath_param
+                        )
+                    else:
+                        logging.info(msg='Band path (BAND) not indicated, using seekpath for it')
+                        sp = seekpath.get_path(
+                            self.get_seekpath_structure(ss),
+                            **self.seekpath_param
+                        )
+                    band_list = self.extract_seekpath_band(sp)
+                    self.BAND, self.BAND_LABELS = self.band_list_2_phonopy_band_string(band_list)
+                else:
+                    # use user input band path
+                    logging.info(msg=f'Band path (BAND) indicated, using: {self.BAND}')
+                    band_list = self.phonopy_band_string_2_band_list(self.BAND, self.BAND_LABELS)
+
+                dumpfn(band_list, os.path.join(path_to_work, "band_path.json"), indent=4)
+
+                # prepare phonopy input head
                 ret = ""
                 ret += "ATOM_NAME ="
                 for ii in ptypes:
                     ret += " %s" % ii
                 ret += "\n"
                 ret += "DIM = %s %s %s\n" % (
                     self.supercell_size[0],
@@ -202,14 +212,16 @@
                 if self.MESH:
                     ret += "MESH = %s %s %s\n" % (
                         self.MESH[0], self.MESH[1], self.MESH[2]
                     )
                 if self.PRIMITIVE_AXES:
                     ret += "PRIMITIVE_AXES = %s\n" % self.PRIMITIVE_AXES
                 ret += "BAND = %s\n" % self.BAND
+                if self.BAND_LABELS:
+                    ret += "BAND_LABELS = %s\n" % self.BAND_LABELS
                 if self.BAND_POINTS:
                     ret += "BAND_POINTS = %s\n" % self.BAND_POINTS
                 if self.BAND_CONNECTION:
                     ret += "BAND_CONNECTION = %s\n" % self.BAND_CONNECTION
 
                 ret_force_read = ret + "FORCE_CONSTANTS=READ\n"
 
@@ -303,34 +315,36 @@
                         raise RuntimeError(
                             f'Unsupported phonon approach input: {self.approach}. '
                             f'Please choose from "linear" and "displacement".'
                         )
                     os.chdir(cwd)
                     return task_list
                 # ----------make for lammps-------------
-                elif self.inter_param["type"] in LAMMPS_TYPE:
+                elif self.inter_param["type"] in LAMMPS_INTER_TYPE:
                     task_path = os.path.join(path_to_work, 'task.000000')
                     os.makedirs(task_path, exist_ok=True)
                     os.chdir(task_path)
                     task_list.append(task_path)
+                    if os.path.isfile(POSCAR) or os.path.islink(POSCAR):
+                        os.remove(POSCAR)
                     os.symlink(os.path.join(path_to_work, "POSCAR-unitcell"), POSCAR)
 
                     with open("band.conf", "a") as fp:
                         fp.write(ret_force_read)
                     os.chdir(cwd)
                     return task_list
                 else:
                     raise RuntimeError(
                         f'Unsupported interaction type input: {self.inter_param["type"]}'
                     )
 
     def post_process(self, task_list):
         cwd = os.getcwd()
         inter_type = self.inter_param["type"]
-        if inter_type in LAMMPS_TYPE:
+        if inter_type in LAMMPS_INTER_TYPE:
             # prepare in.lammps
             for ii in task_list:
                 os.chdir(ii)
                 with open("in.lammps", 'r') as f1:
                     contents = f1.readlines()
                     for jj in range(len(contents)):
                         is_pair_coeff = re.search("pair_coeff", contents[jj])
@@ -356,33 +370,146 @@
 
     def task_type(self):
         return self.parameter["type"]
 
     def task_param(self):
         return self.parameter
 
+    @staticmethod
+    def unpack_band(band_out: str) -> list:
+        branch_list = band_out.split('\n\n\n')
+        branch_list.pop()
+        unpacked_branch_list = []
+        for ii in branch_list:
+            segment_list = ii.split('\n\n')
+            unpacked_segment_list = []
+            for jj in segment_list:
+                point_list = jj.split('\n')
+                segment_dict = {float(kk.split()[0]): float(kk.split()[1]) for kk in point_list}
+                unpacked_segment_list.append(segment_dict)
+            unpacked_branch_list.append(unpacked_segment_list)
+        return unpacked_branch_list
+
+    @staticmethod
+    def get_seekpath_structure(ss: Structure) -> list:
+        """
+        Convert pymatgen structure to seekpath structure
+        """
+        seekpath_structure = [
+            ss.lattice.matrix,
+            ss.frac_coords,
+            ss.atomic_numbers
+        ]
+        return seekpath_structure
+
+    @staticmethod
+    def extract_seekpath_band(seekpath_data: dict):
+        point_coords = seekpath_data['point_coords']
+        band_path = seekpath_data['path']
+        extracted_path = []
+        phonopy_band = []
+        pre_seg_end = None
+        for segment in band_path:
+            seg0 = segment[0]
+            seg1 = segment[1]
+            coord0 = point_coords[segment[0]]
+            coord1 = point_coords[segment[1]]
+            if not pre_seg_end:
+                long_branch = [{seg0: coord0}, {seg1: coord1}]
+            elif pre_seg_end == seg0:
+                long_branch.append({seg1: coord1})
+            else:
+                extracted_path.append(long_branch)
+                long_branch = [{seg0: coord0}, {seg1: coord1}]
+            pre_seg_end = seg1
+        extracted_path.append(long_branch)
+        # return type: list[list[dict[Any, Any]]]
+        return extracted_path
+
+    @staticmethod
+    def band_list_2_phonopy_band_string(band_list) -> [str, str]:
+        band_string = ""
+        band_label = ""
+        # type of band_list: list[list[dict[Any, Any]]]
+        for branch in band_list:
+            for point in branch:
+                name = list(point.keys())[0]
+                coord = list(point.values())[0]
+                coord_str = " ".join([str(ii) for ii in coord])
+                band_string += f"{coord_str}  "
+                band_label += f"{name}  "
+            band_string = band_string[:-2]
+            band_label = band_label[:-2]
+            band_string += ", "
+            band_label += ", "
+        band_string = band_string[:-2]
+        band_label = band_label[:-2]
+
+        return band_string, band_label
+
+    @staticmethod
+    def phonopy_band_string_2_band_list(band_str: str, band_label: str = None):
+        band_list = []
+        branch_list = band_str.split(',')
+        point_num = 0
+        do_label = False
+
+        for branch in branch_list:
+            unit_list = branch.split()
+            unit_num = len(unit_list)
+            if unit_num % 3 != 0:
+                raise ValueError("Input BAND List length is not a multiple of 3.")
+            else:
+                point_num += unit_num // 3
+
+        if band_label:
+            label_branch_list = band_label.split(',')
+            label_num = 0
+            all_labels = []
+            for branch in label_branch_list:
+                label_point_list = branch.split()
+                all_labels.extend(label_point_list)
+                label_num += len(label_point_list)
+            if point_num == label_num:
+                do_label = True
+            else:
+                logging.warning("band string and label string have different length, skip labelling the band")
+
+        for branch in branch_list:
+            unit_list = branch.split()
+            if do_label:
+                label_iter = iter(all_labels)
+                seg_list = [{f'{next(label_iter)}': unit_list[i:i+3]} for i in range(0, len(unit_list), 3)]
+            else:
+                seg_list = [{f'{i}': unit_list[ii:ii+3]} for i, ii in enumerate(range(0, len(unit_list), 3))]
+            band_list.append(seg_list)
+        # return type -> list[list[dict[Any, Any]]]
+        return band_list
+
     def _compute_lower(self, output_file, all_tasks, all_res):
         cwd = Path.cwd()
         work_path = Path(output_file).parent.absolute()
         output_file = os.path.abspath(output_file)
         res_data = {}
         ptr_data = os.path.dirname(output_file) + "\n"
 
+        band_path = loadfn(os.path.join(work_path, "band_path.json"))
+
         if not self.reprod:
             os.chdir(work_path)
             if self.inter_param["type"] == 'abacus':
                 shutil.copyfile("task.000000/band.conf", "band.conf")
                 shutil.copyfile("task.000000/STRU.ori", "STRU")
                 shutil.copyfile("task.000000/phonopy_disp.yaml", "phonopy_disp.yaml")
                 os.system('phonopy -f task.0*/OUT.ABACUS/running_scf.log')
                 os.system('phonopy -f task.0*/OUT.ABACUS/running_scf.log')
                 if os.path.exists("FORCE_SETS"):
-                    print('FORCE_SETS is created')
+                    logging.info('FORCE_SETS is created')
                 else:
-                    print('FORCE_SETS can not be created')
+                    logging.info('FORCE_SETS can not be created')
                 os.system('phonopy band.conf --abacus')
                 os.system('phonopy-bandplot --gnuplot band.yaml > band.dat')
 
             elif self.inter_param["type"] == 'vasp':
                 shutil.copyfile("task.000000/band.conf", "band.conf")
                 if not os.path.samefile("task.000000/POSCAR-unitcell", "POSCAR-unitcell"):
                     shutil.copyfile("task.000000/POSCAR-unitcell", "POSCAR-unitcell")
@@ -393,32 +520,32 @@
                     os.system('phonopy --fc vasprun.xml')
                     assert os.path.isfile('FORCE_CONSTANTS'), "FORCE_CONSTANTS not created"
                     os.system('phonopy --dim="%s %s %s" -c POSCAR-unitcell band.conf' % (
                             self.supercell_size[0],
                             self.supercell_size[1],
                             self.supercell_size[2]))
                     os.system('phonopy-bandplot --gnuplot band.yaml > band.dat')
-                    print('band.dat is created')
+                    logging.info('band.dat is created')
                     shutil.copyfile("band.dat", work_path/"band.dat")
 
                 elif self.approach == "displacement":
                     shutil.copyfile("task.000000/band.conf", "band.conf")
                     shutil.copyfile("task.000000/phonopy_disp.yaml", "phonopy_disp.yaml")
                     os.system('phonopy -f task.0*/vasprun.xml')
                     if os.path.exists("FORCE_SETS"):
-                        print('FORCE_SETS is created')
+                        logging.info('FORCE_SETS is created')
                     else:
-                        print('FORCE_SETS can not be created')
+                        logging.info('FORCE_SETS can not be created')
                     os.system('phonopy --dim="%s %s %s" -c POSCAR-unitcell band.conf' % (
                         self.supercell_size[0],
                         self.supercell_size[1],
                         self.supercell_size[2]))
                     os.system('phonopy-bandplot --gnuplot band.yaml > band.dat')
 
-            elif self.inter_param["type"] in LAMMPS_TYPE:
+            elif self.inter_param["type"] in LAMMPS_INTER_TYPE:
                 os.chdir(all_tasks[0])
                 assert os.path.isfile('FORCE_CONSTANTS'), "FORCE_CONSTANTS not created"
                 os.system('phonopy --dim="%s %s %s" -c POSCAR band.conf' % (
                     self.supercell_size[0], self.supercell_size[1], self.supercell_size[2])
                     )
                 os.system('phonopy-bandplot --gnuplot band.yaml > band.dat')
                 shutil.copyfile("band.dat", work_path/"band.dat")
@@ -435,16 +562,19 @@
                 self.parameter.get("reprod_last_frame", True),
             )
 
         os.chdir(work_path)
         with open('band.dat', 'r') as f:
             ptr_data = f.read()
 
-        result_points = ptr_data.split('\n')[1][4:]
+        result_points = ptr_data.split('\n')[1][4:].split()
         result_lines = ptr_data.split('\n')[2:]
-        res_data[result_points] = result_lines
+        unpacked_lines = self.unpack_band('\n'.join(result_lines))
+        res_data['segment'] = result_points
+        res_data['band_path'] = band_path
+        res_data['band'] = unpacked_lines
 
         with open(output_file, "w") as fp:
             json.dump(res_data, fp, indent=4)
 
         os.chdir(cwd)
         return res_data, ptr_data
```

### Comparing `apex-flow-1.1.6/apex/core/property/Property.py` & `apex_flow-1.2.0/apex/core/property/Property.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,27 +104,27 @@
         #        with open(output_file, 'w') as fp:
         #            json.dump(fp, res, indent=4)
         with open(print_file, "w") as fp:
             fp.write(ptr)
         # os.chdir(cwd)
 
     @abstractmethod
-    def _compute_lower(self, output_file, all_tasks, all_res):
+    def _compute_lower(self, output_file, all_tasks, all_res) -> [dict, str]:
         """
-        Compute the apex.
+        Compute the post.
 
         Parameters
         ----------
         output_file:
-            The file to output the apex
+            The file to output the props
         all_tasks : list of str
             The list of directories to the tasks
         all_res : list of str
             The list of results
         Returns:
         -------
-        res_data : dist
-            The dict storing the result of the apex
+        res_data : dict
+            The dict storing the result of the props
         ptr_data : str
             The result printed in string format
         """
         pass
```

### Comparing `apex-flow-1.1.6/apex/core/property/Surface.py` & `apex_flow-1.2.0/apex/core/property/Surface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import glob
 import json
 import logging
 import os
 import re
-
 import dpdata
 import numpy as np
 from monty.serialization import dumpfn, loadfn
 from pymatgen.core.structure import Structure
 from pymatgen.core.surface import generate_all_slabs
 
 from apex.core.calculator.lib import abacus_utils
@@ -31,85 +30,54 @@
                 self.pert_xz = parameter["pert_xz"]
                 default_max_miller = 2
                 parameter["max_miller"] = parameter.get(
                     "max_miller", default_max_miller
                 )
                 self.miller = parameter["max_miller"]
             parameter["cal_type"] = parameter.get("cal_type", "relaxation")
-            self.cal_type = parameter["cal_type"]
             default_cal_setting = {
                 "relax_pos": True,
                 "relax_shape": True,
                 "relax_vol": False,
             }
-            if "cal_setting" not in parameter:
-                parameter["cal_setting"] = default_cal_setting
-            else:
-                if "relax_pos" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_pos"] = default_cal_setting[
-                        "relax_pos"
-                    ]
-                if "relax_shape" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                        "relax_shape"
-                    ]
-                if "relax_vol" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_vol"] = default_cal_setting[
-                        "relax_vol"
-                    ]
-            self.cal_setting = parameter["cal_setting"]
         else:
             parameter["cal_type"] = "static"
             self.cal_type = parameter["cal_type"]
             default_cal_setting = {
                 "relax_pos": False,
                 "relax_shape": False,
                 "relax_vol": False,
-            }
-            if "cal_setting" not in parameter:
-                parameter["cal_setting"] = default_cal_setting
-            else:
-                if "relax_pos" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_pos"] = default_cal_setting[
-                        "relax_pos"
-                    ]
-                if "relax_shape" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                        "relax_shape"
-                    ]
-                if "relax_vol" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_vol"] = default_cal_setting[
-                        "relax_vol"
-                    ]
-            self.cal_setting = parameter["cal_setting"]
+            }            
             parameter["init_from_suffix"] = parameter.get("init_from_suffix", "00")
             self.init_from_suffix = parameter["init_from_suffix"]
+        self.cal_type = parameter["cal_type"]
+        parameter["cal_setting"] = parameter.get("cal_setting", default_cal_setting)
+        for key in default_cal_setting:
+            parameter["cal_setting"].setdefault(key, default_cal_setting[key])
+        self.cal_setting = parameter["cal_setting"]
         self.parameter = parameter
         self.inter_param = inter_param if inter_param != None else {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
-            #dlog.warning("%s already exists" % path_to_work)
             logging.warning("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
 
         if "start_confs_path" in self.parameter and os.path.exists(
             self.parameter["start_confs_path"]
         ):
             init_path_list = glob.glob(
                 os.path.join(self.parameter["start_confs_path"], "*")
             )
-            struct_init_name_list = []
-            for ii in init_path_list:
-                struct_init_name_list.append(ii.split("/")[-1])
-            struct_output_name = path_to_work.split("/")[-2]
-            assert struct_output_name in struct_init_name_list
+            struct_init_name_list = [os.path.basename(ii) for ii in init_path_list]
+            struct_output_name = os.path.basename(os.path.dirname(path_to_work))
+            assert struct_output_name in struct_init_name_list, f"{struct_output_name} not in initial configuration names"
             path_to_equi = os.path.abspath(
                 os.path.join(
                     self.parameter["start_confs_path"],
                     struct_output_name,
                     "relaxation",
                     "relax_task",
                 )
@@ -126,47 +94,42 @@
             task_list = make_repro(
                 self.inter_param,
                 init_data_path,
                 self.init_from_suffix,
                 path_to_work,
                 self.parameter.get("reprod_last_frame", True),
             )
-            os.chdir(cwd)
 
         else:
             if refine:
-                print("surface refine starts")
+                logging.info("surface refine starts")
                 task_list = make_refine(
                     self.parameter["init_from_suffix"],
                     self.parameter["output_suffix"],
                     path_to_work,
                 )
-                os.chdir(cwd)
                 # record miller
                 init_from_path = re.sub(
                     self.parameter["output_suffix"][::-1],
                     self.parameter["init_from_suffix"][::-1],
                     path_to_work[::-1],
                     count=1,
                 )[::-1]
                 task_list_basename = list(map(os.path.basename, task_list))
 
                 for ii in task_list_basename:
                     init_from_task = os.path.join(init_from_path, ii)
                     output_task = os.path.join(path_to_work, ii)
                     os.chdir(output_task)
-                    if os.path.isfile("miller.json"):
-                        os.remove("miller.json")
-                    if os.path.islink("miller.json"):
+                    if os.path.exists("miller.json"):
                         os.remove("miller.json")
                     os.symlink(
                         os.path.relpath(os.path.join(init_from_task, "miller.json")),
                         "miller.json",
                     )
-                os.chdir(cwd)
 
             else:
                 if self.inter_param["type"] == "abacus":
                     CONTCAR = abacus_utils.final_stru(path_to_equi)
                     POSCAR = "STRU"
                 else:
                     CONTCAR = "CONTCAR"
@@ -189,20 +152,17 @@
 
                 # gen slabs
                 all_slabs = generate_all_slabs(
                     ss, self.miller, self.min_slab_size, self.min_vacuum_size
                 )
 
                 os.chdir(path_to_work)
-                if os.path.isfile(POSCAR):
-                    os.remove(POSCAR)
-                if os.path.islink(POSCAR):
+                if os.path.exists(POSCAR):
                     os.remove(POSCAR)
                 os.symlink(os.path.relpath(equi_contcar), POSCAR)
-                #           task_poscar = os.path.join(output, 'POSCAR')
                 for ii in range(len(all_slabs)):
                     output_task = os.path.join(path_to_work, "task.%06d" % ii)
                     os.makedirs(output_task, exist_ok=True)
                     os.chdir(output_task)
                     for jj in [
                         "INCAR",
                         "POTCAR",
@@ -210,31 +170,31 @@
                         "conf.lmp",
                         "in.lammps",
                         "STRU",
                     ]:
                         if os.path.exists(jj):
                             os.remove(jj)
                     task_list.append(output_task)
-                    print(
+                    logging.info(
                         "# %03d generate " % ii,
                         output_task,
                         " \t %d atoms" % len(all_slabs[ii].sites),
                     )
                     # make confs
                     all_slabs[ii].to("POSCAR.tmp", "POSCAR")
                     vasp_utils.regulate_poscar("POSCAR.tmp", "POSCAR")
                     vasp_utils.sort_poscar("POSCAR", "POSCAR", ptypes)
                     vasp_utils.perturb_xz("POSCAR", "POSCAR", self.pert_xz)
                     if self.inter_param["type"] == "abacus":
                         abacus_utils.poscar2stru("POSCAR", self.inter_param, "STRU")
                         os.remove("POSCAR")
                     # record miller
                     dumpfn(all_slabs[ii].miller_index, "miller.json")
-                os.chdir(cwd)
-
+        
+        os.chdir(cwd)
         return task_list
 
     def post_process(self, task_list):
         pass
 
     def task_type(self):
         return self.parameter["type"]
@@ -245,44 +205,45 @@
     def _compute_lower(self, output_file, all_tasks, all_res):
         output_file = os.path.abspath(output_file)
         res_data = {}
         ptr_data = os.path.dirname(output_file) + "\n"
 
         if not self.reprod:
             ptr_data += "Miller_Indices: \tSurf_E(J/m^2) EpA(eV) equi_EpA(eV)\n"
+
+            equi_path = os.path.abspath(
+                os.path.join(
+                    os.path.dirname(output_file), "../relaxation/relax_task"
+                )
+            )
+            equi_result = loadfn(os.path.join(equi_path, "result.json"))
+            equi_epa = equi_result["energies"][-1] / np.sum(
+                equi_result["atom_numbs"]
+            )
+
             for ii in all_tasks:
                 task_result = loadfn(os.path.join(ii, "result_task.json"))
                 natoms = np.sum(task_result["atom_numbs"])
                 epa = task_result["energies"][-1] / natoms
                 AA = np.linalg.norm(
                     np.cross(task_result["cells"][0][0], task_result["cells"][0][1])
                 )
 
-                equi_path = os.path.abspath(
-                    os.path.join(
-                        os.path.dirname(output_file), "../relaxation/relax_task"
-                    )
-                )
-                equi_result = loadfn(os.path.join(equi_path, "result.json"))
-                equi_epa = equi_result["energies"][-1] / np.sum(
-                    equi_result["atom_numbs"]
-                )
                 structure_dir = os.path.basename(ii)
-
                 Cf = 1.60217657e-16 / (1e-20 * 2) * 0.001
                 evac = (task_result["energies"][-1] - equi_epa * natoms) / AA * Cf
-
                 miller_index = loadfn(os.path.join(ii, "miller.json"))
+                
                 ptr_data += "%-25s     %7.3f    %8.3f %8.3f\n" % (
                     str(miller_index) + "-" + structure_dir + ":",
                     evac,
                     epa,
                     equi_epa,
                 )
-                res_data[str(miller_index) + "-" + structure_dir] = [
+                res_data[str(miller_index) + "_" + structure_dir] = [
                     evac,
                     epa,
                     equi_epa,
                 ]
 
         else:
             if "init_data_path" not in self.parameter:
```

### Comparing `apex-flow-1.1.6/apex/core/property/Vacancy.py` & `apex_flow-1.2.0/apex/core/property/Vacancy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import glob
 import json
 import logging
 import os
 import re
-
 import numpy as np
 from monty.serialization import dumpfn, loadfn
 from pymatgen.analysis.defects.generators import VacancyGenerator
 from pymatgen.core.structure import Structure
 
 from apex.core.calculator.lib import abacus_utils
 from apex.core.property.Property import Property
@@ -23,114 +22,81 @@
         self.reprod = parameter["reproduce"]
         if not self.reprod:
             if not ("init_from_suffix" in parameter and "output_suffix" in parameter):
                 default_supercell = [1, 1, 1]
                 parameter["supercell"] = parameter.get("supercell", default_supercell)
                 self.supercell = parameter["supercell"]
             parameter["cal_type"] = parameter.get("cal_type", "relaxation")
-            self.cal_type = parameter["cal_type"]
             default_cal_setting = {
                 "relax_pos": True,
                 "relax_shape": True,
                 "relax_vol": True,
             }
-            if "cal_setting" not in parameter:
-                parameter["cal_setting"] = default_cal_setting
-            else:
-                if "relax_pos" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_pos"] = default_cal_setting[
-                        "relax_pos"
-                    ]
-                if "relax_shape" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                        "relax_shape"
-                    ]
-                if "relax_vol" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_vol"] = default_cal_setting[
-                        "relax_vol"
-                    ]
-            self.cal_setting = parameter["cal_setting"]
         else:
             parameter["cal_type"] = "static"
-            self.cal_type = parameter["cal_type"]
             default_cal_setting = {
                 "relax_pos": False,
                 "relax_shape": False,
                 "relax_vol": False,
             }
-            if "cal_setting" not in parameter:
-                parameter["cal_setting"] = default_cal_setting
-            else:
-                if "relax_pos" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_pos"] = default_cal_setting[
-                        "relax_pos"
-                    ]
-                if "relax_shape" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_shape"] = default_cal_setting[
-                        "relax_shape"
-                    ]
-                if "relax_vol" not in parameter["cal_setting"]:
-                    parameter["cal_setting"]["relax_vol"] = default_cal_setting[
-                        "relax_vol"
-                    ]
-            self.cal_setting = parameter["cal_setting"]
             parameter["init_from_suffix"] = parameter.get("init_from_suffix", "00")
             self.init_from_suffix = parameter["init_from_suffix"]
+        self.cal_type = parameter["cal_type"]
+        parameter["cal_setting"] = parameter.get("cal_setting", default_cal_setting)
+        for key in default_cal_setting:
+            parameter["cal_setting"].setdefault(key, default_cal_setting[key])
+        self.cal_setting = parameter["cal_setting"]
         self.parameter = parameter
         self.inter_param = inter_param if inter_param != None else {"type": "vasp"}
 
     def make_confs(self, path_to_work, path_to_equi, refine=False):
         path_to_work = os.path.abspath(path_to_work)
         if os.path.exists(path_to_work):
-            #dlog.warning("%s already exists" % path_to_work)
             logging.warning("%s already exists" % path_to_work)
         else:
             os.makedirs(path_to_work)
         path_to_equi = os.path.abspath(path_to_equi)
 
         if "start_confs_path" in self.parameter and os.path.exists(
             self.parameter["start_confs_path"]
         ):
             init_path_list = glob.glob(
                 os.path.join(self.parameter["start_confs_path"], "*")
             )
-            struct_init_name_list = []
-            for ii in init_path_list:
-                struct_init_name_list.append(ii.split("/")[-1])
-            struct_output_name = path_to_work.split("/")[-2]
-            assert struct_output_name in struct_init_name_list
+            struct_init_name_list = [os.path.basename(ii) for ii in init_path_list]
+            struct_output_name = os.path.basename(os.path.dirname(path_to_work))
+            assert struct_output_name in struct_init_name_list, f"{struct_output_name} not in initial configurations"
             path_to_equi = os.path.abspath(
                 os.path.join(
                     self.parameter["start_confs_path"],
                     struct_output_name,
                     "relaxation",
                     "relax_task",
                 )
             )
 
         task_list = []
         cwd = os.getcwd()
 
         if self.reprod:
-            print("vacancy reproduce starts")
+            logging.info("vacancy reproduce starts")
             if "init_data_path" not in self.parameter:
                 raise RuntimeError("please provide the initial data path to reproduce")
             init_data_path = os.path.abspath(self.parameter["init_data_path"])
             task_list = make_repro(
                 self.inter_param,
                 init_data_path,
                 self.init_from_suffix,
                 path_to_work,
                 self.parameter.get("reprod_last_frame", False),
             )
-            os.chdir(cwd)
 
         else:
             if refine:
-                print("vacancy refine starts")
+                logging.info("vacancy refine starts")
                 task_list = make_refine(
                     self.parameter["init_from_suffix"],
                     self.parameter["output_suffix"],
                     path_to_work,
                 )
 
                 init_from_path = re.sub(
@@ -141,23 +107,20 @@
                 )[::-1]
                 task_list_basename = list(map(os.path.basename, task_list))
 
                 for ii in task_list_basename:
                     init_from_task = os.path.join(init_from_path, ii)
                     output_task = os.path.join(path_to_work, ii)
                     os.chdir(output_task)
-                    if os.path.isfile("supercell.json"):
-                        os.remove("supercell.json")
-                    if os.path.islink("supercell.json"):
+                    if os.path.exists("supercell.json"):
                         os.remove("supercell.json")
                     os.symlink(
                         os.path.relpath(os.path.join(init_from_task, "supercell.json")),
                         "supercell.json",
                     )
-                os.chdir(cwd)
             else:
                 if self.inter_param["type"] == "abacus":
                     CONTCAR = abacus_utils.final_stru(path_to_equi)
                     POSCAR = "STRU"
                 else:
                     CONTCAR = "CONTCAR"
                     POSCAR = "POSCAR"
@@ -175,19 +138,17 @@
                 vds = pre_vds.generate(ss)
                 dss = []
                 for jj in vds:
                     dss.append(
                         jj.get_supercell_structure(sc_mat=np.diag(self.supercell, k=0))
                     )
 
-                print("gen vacancy with supercell " + str(self.supercell))
+                logging.info("gen vacancy with supercell " + str(self.supercell))
                 os.chdir(path_to_work)
-                if os.path.isfile(POSCAR):
-                    os.remove(POSCAR)
-                if os.path.islink(POSCAR):
+                if os.path.exists(POSCAR):
                     os.remove(POSCAR)
                 os.symlink(os.path.relpath(equi_contcar), POSCAR)
                 #           task_poscar = os.path.join(output, 'POSCAR')
 
                 for ii in range(len(dss)):
                     output_task = os.path.join(path_to_work, "task.%06d" % ii)
                     os.makedirs(output_task, exist_ok=True)
@@ -205,15 +166,15 @@
                     task_list.append(output_task)
                     dss[ii].to("POSCAR", "POSCAR")
                     if self.inter_param["type"] == "abacus":
                         abacus_utils.poscar2stru("POSCAR", self.inter_param, "STRU")
                         os.remove("POSCAR")
                     # np.savetxt('supercell.out', self.supercell, fmt='%d')
                     dumpfn(self.supercell, "supercell.json")
-                os.chdir(cwd)
+        os.chdir(cwd)
         return task_list
 
     def post_process(self, task_list):
         pass
 
     def task_type(self):
         return self.parameter["type"]
@@ -224,27 +185,26 @@
     def _compute_lower(self, output_file, all_tasks, all_res):
         output_file = os.path.abspath(output_file)
         res_data = {}
         ptr_data = os.path.dirname(output_file) + "\n"
 
         if not self.reprod:
             ptr_data += "Structure: \tVac_E(eV)  E(eV) equi_E(eV)\n"
-            idid = -1
-            for ii in all_tasks:
-                idid += 1
+            equi_path = os.path.abspath(
+                os.path.join(
+                    os.path.dirname(output_file), "../relaxation/relax_task"
+                )
+            )
+            equi_result = loadfn(os.path.join(equi_path, "result.json"))
+            equi_epa = equi_result["energies"][-1] / sum(equi_result["atom_numbs"])
+
+            for idid, ii in enumerate(all_tasks):
                 structure_dir = os.path.basename(ii)
                 task_result = loadfn(all_res[idid])
-                natoms = task_result["atom_numbs"][0]
-                equi_path = os.path.abspath(
-                    os.path.join(
-                        os.path.dirname(output_file), "../relaxation/relax_task"
-                    )
-                )
-                equi_result = loadfn(os.path.join(equi_path, "result.json"))
-                equi_epa = equi_result["energies"][-1] / equi_result["atom_numbs"][0]
+                natoms = sum(task_result["atom_numbs"])                
                 evac = task_result["energies"][-1] - equi_epa * natoms
 
                 supercell_index = loadfn(os.path.join(ii, "supercell.json"))
                 ptr_data += "%s: %7.3f  %7.3f %7.3f \n" % (
                     str(supercell_index) + "-" + structure_dir,
                     evac,
                     task_result["energies"][-1],
```

### Comparing `apex-flow-1.1.6/apex/core/refine.py` & `apex_flow-1.2.0/apex/core/refine.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def make_refine(init_from_suffix, output_suffix, path_to_work):
     cwd = os.getcwd()
     init_from = re.sub(
         output_suffix[::-1], init_from_suffix[::-1], path_to_work[::-1], count=1
     )[::-1]
     if not os.path.exists(init_from):
-        raise FileNotFoundError("the initial directory does not exist for refine")
+        raise FileNotFoundError("The initial directory does not exist for refine")
 
     output = path_to_work
     init_from_task_tot = glob.glob(os.path.join(init_from, "task.[0-9]*[0-9]"))
 
     task_num = len(init_from_task_tot)
 
     task_list = []
```

### Comparing `apex-flow-1.1.6/apex/core/reproduce.py` & `apex_flow-1.2.0/apex/core/reproduce.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,52 +15,44 @@
     path_to_work = os.path.abspath(path_to_work)
     property_type = path_to_work.split("/")[-1].split("_")[0]
     init_data_path = os.path.join(
         init_data_path, "*", property_type + "_" + init_from_suffix
     )
     init_data_path_list = glob.glob(init_data_path)
     init_data_path_list.sort()
-    cwd = os.getcwd()
-    struct_init_name_list = []
-    for ii in init_data_path_list:
-        struct_init_name_list.append(ii.split("/")[-2])
+    struct_init_name_list = [ii.split("/")[-2] for ii in init_data_path_list]
     struct_output_name = path_to_work.split("/")[-2]
 
-    assert struct_output_name in struct_init_name_list
+    assert struct_output_name in struct_init_name_list, "Output structure name not found in initial structure list"
 
-    for idx, ii in enumerate(struct_init_name_list):
-        if ii == struct_output_name:
-            label = idx
+    label = struct_init_name_list.index(struct_output_name)
 
     init_data_path_todo = init_data_path_list[label]
 
     init_data_task_todo = glob.glob(
         os.path.join(init_data_path_todo, "task.[0-9]*[0-9]")
     )
     assert (
         len(init_data_task_todo) > 0
     ), "There is no task in previous calculations path"
     init_data_task_todo.sort()
 
-    task_list = []
-    task_num = 0
-
+    cwd = os.getcwd()
     if property_type == "interstitial":
         if os.path.exists(os.path.join(path_to_work, "element.out")):
             os.remove(os.path.join(path_to_work, "element.out"))
         fout_element = open(os.path.join(path_to_work, "element.out"), "a+")
         fin_element = open(os.path.join(init_data_path_todo, "element.out"), "r")
 
+    task_list = []
+    task_num = 0
     for ii in init_data_task_todo:
         # get frame number
         task_result = loadfn(os.path.join(ii, "result_task.json"))
-        if reprod_last_frame:
-            nframe = 1
-        else:
-            nframe = len(task_result["energies"])
+        nframe = 1 if reprod_last_frame else len(task_result["energies"])
         if property_type == "interstitial":
             insert_element = fin_element.readline().split()[0]
         for jj in range(nframe):
             if property_type == "interstitial":
                 print(insert_element, file=fout_element)
             output_task = os.path.join(path_to_work, "task.%06d" % task_num)
             task_num += 1
@@ -105,26 +97,20 @@
     property_type = all_tasks[0].split("/")[-2].split("_")[0]
     init_data_path = os.path.join(
         init_data_path, "*", property_type + "_" + init_from_suffix
     )
     init_data_path_list = glob.glob(init_data_path)
     init_data_path_list.sort()
     # cwd = os.getcwd()
-    struct_init_name_list = []
-    for ii in init_data_path_list:
-        struct_init_name_list.append(ii.split("/")[-2])
-
-    assert struct_output_name in struct_init_name_list
-
-    for idx, ii in enumerate(struct_init_name_list):
-        if ii == struct_output_name:
-            label = idx
+    struct_init_name_list = [ii.split("/")[-2] for ii in init_data_path_list]
+    
+    assert struct_output_name in struct_init_name_list, "Output structure name not found in initial structure list"
 
+    label = struct_init_name_list.index(struct_output_name)
     init_data_path_todo = init_data_path_list[label]
-
     init_data_task_todo = glob.glob(
         os.path.join(init_data_path_todo, "task.[0-9]*[0-9]")
     )
     assert (
         len(init_data_task_todo) > 0
     ), "There is no task in previous calculations path"
     init_data_task_todo.sort()
@@ -132,31 +118,25 @@
     idid = 0
     init_ener_tot = []
     output_ener_tot = []
     res_data = {}
 
     for ii in init_data_task_todo:
         init_task_result = loadfn(os.path.join(ii, "result_task.json"))
-        if reprod_last_frame:
-            nframe = 1
-        else:
-            nframe = len(init_task_result["energies"])
+        nframe = 1 if reprod_last_frame else len(init_task_result["energies"])
         # idid += nframe
         natoms = np.sum(init_task_result["atom_numbs"])
-        if reprod_last_frame:
-            init_ener = init_task_result["energies"][-1:]
-        else:
-            init_ener = init_task_result["energies"]
+        init_ener = init_task_result["energies"][-nframe:]
         init_ener_tot.extend(list(init_ener))
         output_ener = []
         for jj in range(idid, idid + nframe):
             output_task_result = loadfn(os.path.join(all_tasks[jj], "result_task.json"))
+            output_ener_tot.extend(output_task_result["energies"])
             output_epa = output_task_result["energies"] / natoms
             output_ener.append(output_epa)
-            output_ener_tot.extend(output_task_result["energies"])
 
             init_epa = init_ener[jj - idid] / natoms
             ptr_data += "%s %7.3f  %7.3f  %7.3f\n" % (
                 ii,
                 init_epa,
                 output_epa,
                 output_epa - init_epa,
```

### Comparing `apex-flow-1.1.6/apex/core/structure.py` & `apex_flow-1.2.0/apex/core/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 upload_packages.append(__file__)
 
 class StructureInfo(object):
     """Analyze structure type
     Arg:
         structure: pymatgen.core.Structure object
     """
-    def __init__(self, structure: pymatgen.core.Structure):
-        analyzer = SpacegroupAnalyzer(structure)
+    def __init__(self, structure: pymatgen.core.Structure, **kwargs) -> None:
+        analyzer = SpacegroupAnalyzer(structure, **kwargs)
         self.__space_group_symbol = analyzer.get_space_group_symbol()
         self.__space_group_number = analyzer.get_space_group_number()
         self.__point_group_symbol = analyzer.get_point_group_symbol()
         self.__crystal_system = analyzer.get_crystal_system()
         self.__lattice_type = analyzer.get_lattice_type()
         self.__num_atoms = structure.num_sites
         self.__crystal_structure = self.__indentify_crystal()
```

### Comparing `apex-flow-1.1.6/apex/op/RunLAMMPS.py` & `apex_flow-1.2.0/apex/op/RunLAMMPS.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, subprocess
+import os, subprocess, logging
 from pathlib import Path
 from dflow.python import (
     OP,
     OPIO,
     OPIOSign,
     Artifact,
     upload_packages
@@ -38,16 +38,16 @@
         if os.path.exists("run_command"):
             with open("run_command", 'r') as f:
                 cmd = f.read()
         else:
             cmd = op_in["run_command"]
         exit_code = subprocess.call(cmd, shell=True)
         if exit_code == 0:
-            print("Call Lammps command successfully!")
+            logging.info("Call Lammps command successfully!")
         else:
-            print("Call Lammps command failed with exit code:", exit_code)
+            logging.warning(f"Call Lammps command failed with exit code: {exit_code}")
 
         os.chdir(cwd)
         op_out = OPIO({
             "backward_dir": op_in["input_lammps"]
         })
         return op_out
```

### Comparing `apex-flow-1.1.6/apex/op/property_ops.py` & `apex_flow-1.2.0/apex/op/property_ops.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,113 +4,27 @@
 from dflow.python import (
     OP,
     OPIO,
     OPIOSign,
     Artifact,
     upload_packages
 )
-
-from apex.op.utils import recursive_search
+from monty.serialization import dumpfn
+from apex.utils import recursive_search
+from apex.core.lib.utils import create_path
+from apex.core.calculator import LAMMPS_INTER_TYPE
 
 upload_packages.append(__file__)
 
 
-class DistributeProps(OP):
-    """
-    OP class for distribution
-    of individual property test steps
-    """
-    # TODO: add API for complex property test superOP
-    def __init__(self):
-        pass
-
-    @classmethod
-    def get_input_sign(cls):
-        return OPIOSign({
-            "input_work_path": Artifact(Path),
-            "param": dict
-        })
-
-    @classmethod
-    def get_output_sign(cls):
-        return OPIOSign({
-            "orig_work_path": Artifact(List[Path]),
-            "flow_id": List[str],
-            "path_to_prop": List[str],
-            "prop_param": List[dict],
-            "inter_param": List[dict],
-            "do_refine": List[bool],
-            "nflows": int
-        })
-
-    @OP.exec_sign_check
-    def execute(
-            self,
-            op_in: OPIO,
-    ) -> OPIO:
-        input_work_path = op_in["input_work_path"]
-        param = op_in["param"]
-
-        cwd = Path.cwd()
-        os.chdir(input_work_path)
-        confs = param["structures"]
-        interaction = param["interaction"]
-        properties = param["properties"]
-
-        conf_dirs = []
-        flow_id_list = []
-        path_to_prop_list = []
-        prop_param_list = []
-        do_refine_list = []
-        for conf in confs:
-            conf_dirs.extend(glob.glob(conf))
-        conf_dirs.sort()
-        for ii in conf_dirs:
-            for jj in properties:
-                if jj.get('skip', False):
-                    continue
-                if 'init_from_suffix' and 'output_suffix' in jj:
-                    do_refine = True
-                    suffix = jj['output_suffix']
-                elif 'reproduce' in jj and jj['reproduce']:
-                    do_refine = False
-                    suffix = 'reprod'
-                elif 'suffix' in jj and jj['suffix']:
-                    do_refine = False
-                    suffix = str(jj['suffix'])
-                else:
-                    do_refine = False
-                    suffix = '00'
-
-                property_type = jj["type"]
-                path_to_prop_list.append(os.path.join(ii, property_type + "_" + suffix))
-                prop_param_list.append(jj)
-                do_refine_list.append(do_refine)
-                flow_id_list.append(ii + '-' + property_type + '-' + suffix)
-
-        nflow = len(path_to_prop_list)
-        orig_work_path_list = [input_work_path] * nflow
-        inter_param_list = [interaction] * nflow
-
-        op_out = OPIO({
-            "orig_work_path": orig_work_path_list,
-            "flow_id": flow_id_list,
-            "path_to_prop": path_to_prop_list,
-            "prop_param": prop_param_list,
-            "inter_param": inter_param_list,
-            "do_refine": do_refine_list,
-            "nflows": nflow
-        })
-        return op_out
-
-
 class PropsMake(OP):
     """
     OP class for making calculation tasks (make property)
     """
+
     def __init__(self):
         pass
 
     @classmethod
     def get_input_sign(cls):
         return OPIOSign({
             'input_work_path': Artifact(Path),
@@ -142,39 +56,48 @@
         prop_param = op_in["prop_param"]
         inter_param = op_in["inter_param"]
         do_refine = op_in["do_refine"]
 
         cwd = Path.cwd()
         os.chdir(input_work_path)
         abs_path_to_prop = input_work_path / path_to_prop
+        if os.path.exists(abs_path_to_prop):
+            shutil.rmtree(abs_path_to_prop)
+        create_path(str(abs_path_to_prop))
         conf_path = abs_path_to_prop.parent
         prop_name = abs_path_to_prop.name
         path_to_equi = conf_path / "relaxation" / "relax_task"
-        prop = make_property_instance(prop_param, inter_param)
+
+        inter_param_prop = inter_param
+        if "cal_setting" in prop_param and "overwrite_interaction" in prop_param["cal_setting"]:
+            inter_param_prop = prop_param["cal_setting"]["overwrite_interaction"]
+
+        prop = make_property_instance(prop_param, inter_param_prop)
         task_list = prop.make_confs(abs_path_to_prop, path_to_equi, do_refine)
         for kk in task_list:
             poscar = os.path.join(kk, "POSCAR")
-            inter = make_calculator(inter_param, poscar)
+            inter = make_calculator(inter_param_prop, poscar)
             inter.make_potential_files(kk)
             logging.debug(prop.task_type())  ### debug
             inter.make_input_file(kk, prop.task_type(), prop.task_param())
         prop.post_process(
             task_list
         )  # generate same KPOINTS file for elastic when doing VASP
 
         task_list.sort()
+        os.chdir(path_to_prop)
+        task_list_name = {'task_list': glob.glob('task.*').sort()}
+        dumpfn(task_list_name, 'task_list.json')
         os.chdir(input_work_path)
         task_list_str = glob.glob(path_to_prop + '/' + 'task.*')
         task_list_str.sort()
 
         all_jobs = task_list
         njobs = len(all_jobs)
-        jobs = []
-        for job in all_jobs:
-            jobs.append(pathlib.Path(job))
+        jobs = [pathlib.Path(job) for job in task_list]
 
         os.chdir(cwd)
         op_out = OPIO({
             "output_work_path": input_work_path,
             "task_names": task_list_str,
             "njobs": njobs,
             "task_paths": jobs
@@ -200,125 +123,96 @@
             'task_names': List[str],
             'path_to_prop': str
         })
 
     @classmethod
     def get_output_sign(cls):
         return OPIOSign({
-            'output_post': Artifact(Path)
+            'retrieve_path': Artifact(List[Path])
         })
 
     @OP.exec_sign_check
     def execute(self, op_in: OPIO) -> OPIO:
         from ..core.common_prop import make_property_instance
         cwd = os.getcwd()
         input_post = op_in["input_post"]
         input_all = op_in["input_all"]
         prop_param = op_in["prop_param"]
         inter_param = op_in["inter_param"]
         task_names = op_in["task_names"]
         path_to_prop = op_in["path_to_prop"]
-        calculator = inter_param["type"]
+        inter_type = inter_param["type"]
         copy_dir_list_input = [path_to_prop.split('/')[0]]
         os.chdir(input_all)
         copy_dir_list = []
         for ii in copy_dir_list_input:
             copy_dir_list.extend(glob.glob(ii))
+        copy_dir_list = list(set(copy_dir_list))
+        copy_dir_list.sort()
 
         # find path of finished tasks
         os.chdir(op_in['input_post'])
         src_path = recursive_search(copy_dir_list)
         if not src_path:
             raise RuntimeError(f'Fail to find input work path after slices!')
 
-        if calculator in ['vasp', 'abacus']:
+        if inter_type in ['vasp', 'abacus']:
             os.chdir(input_post)
             for ii in task_names:
                 shutil.copytree(os.path.join(ii, "backward_dir"), ii, dirs_exist_ok=True)
                 shutil.rmtree(os.path.join(ii, "backward_dir"))
             os.chdir(input_all)
             shutil.copytree(input_post, './', dirs_exist_ok=True)
         else:
             os.chdir(input_all)
-            #src_path = str(input_post) + str(local_path)
+            # src_path = str(input_post) + str(local_path)
             shutil.copytree(src_path, './', dirs_exist_ok=True)
 
         if ("cal_setting" in prop_param
                 and "overwrite_interaction" in prop_param["cal_setting"]):
             inter_param = prop_param["cal_setting"]["overwrite_interaction"]
 
         abs_path_to_prop = Path.cwd() / path_to_prop
-
         prop = make_property_instance(prop_param, inter_param)
+        param_json = os.path.join(abs_path_to_prop, "param.json")
+        param_dict = prop.parameter
+        param_dict.setdefault("skip", False) # default of "skip" is False
+        param_dict.pop("skip")
+        dumpfn(param_dict, param_json)
         prop.compute(
             os.path.join(abs_path_to_prop, "result.json"),
             os.path.join(abs_path_to_prop, "result.out"),
             abs_path_to_prop,
         )
-        # remove potential files in each md task
-        os.chdir(abs_path_to_prop)
-        cmd = "for kk in task.*; do cd $kk; rm *.pb; cd ..; done"
-        subprocess.call(cmd, shell=True)
+        # remove potential files in each task
+        if inter_type in LAMMPS_INTER_TYPE:
+            os.chdir(abs_path_to_prop)
+            inter_files_name = []
+            if type(inter_param["model"]) is str:
+                inter_files_name = [inter_param["model"]]
+            elif type(inter_param["model"]) is list:
+                inter_files_name.extend(inter_param["model"])
+            for file in inter_files_name:
+                cmd = f"rm -f ../{file}"
+                subprocess.call(cmd, shell=True)
+                cmd = f"for kk in task.*; do rm -f $kk/{file}; done"
+                subprocess.call(cmd, shell=True)
+        elif inter_type == 'vasp':
+            os.chdir(abs_path_to_prop)
+            cmd = "rm -f ../POTCAR"
+            subprocess.call(cmd, shell=True)
+            cmd = f"for kk in task.*; do rm -f $kk/POTCAR; done"
+            subprocess.call(cmd, shell=True)
 
         os.chdir(cwd)
-        out_path = Path(cwd) / 'retrieve_pool'
-        os.mkdir(out_path)
-        shutil.copytree(input_all / path_to_prop,
-                        out_path / path_to_prop, dirs_exist_ok=True)
-
-        op_out = OPIO({
-            'output_post': abs_path_to_prop
-        })
-        return op_out
-
-
-class CollectProps(OP):
-    """
-    OP class for collect property tasks
-    """
-
-    def __init__(self):
-        pass
-
-    @classmethod
-    def get_input_sign(cls):
-        return OPIOSign({
-            'input_post': Artifact(Path, sub_path=False),
-            'input_all': Artifact(Path),
-            'param': dict
-        })
-
-    @classmethod
-    def get_output_sign(cls):
-        return OPIOSign({
-            'retrieve_path': Artifact(List[Path])
-        })
-
-    @OP.exec_sign_check
-    def execute(self, op_in: OPIO) -> OPIO:
-        cwd = os.getcwd()
-        input_post = op_in["input_post"]
-        input_all = op_in["input_all"]
-        param = op_in["param"]
-        confs = param["structures"]
-        copy_dir_list_input = [conf.split('/')[0] for conf in confs]
-        os.chdir(op_in['input_all'])
-        copy_dir_list = []
-        for ii in copy_dir_list_input:
-            copy_dir_list.extend(glob.glob(ii))
-        os.chdir(input_post)
-
-        src_path = recursive_search(copy_dir_list)
-        if not src_path:
-            raise RuntimeError(f'Fail to find input work path after slices!')
-        shutil.copytree(src_path, input_all, dirs_exist_ok=True)
-
         for ii in copy_dir_list:
             shutil.copytree(input_all / ii, ii, dirs_exist_ok=True)
-
         retrieve_path = [Path(ii) for ii in copy_dir_list]
+        # out_path = Path(cwd) / 'retrieve_pool'
+        # os.mkdir(out_path)
+        # shutil.copytree(input_all / path_to_prop,
+        #                out_path / path_to_prop, dirs_exist_ok=True)
 
         op_out = OPIO({
             'retrieve_path': retrieve_path
         })
         return op_out
-
```

### Comparing `apex-flow-1.1.6/apex/op/relaxation_ops.py` & `apex_flow-1.2.0/apex/op/relaxation_ops.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from dflow.python import (
     OP,
     OPIO,
     OPIOSign,
     Artifact,
     upload_packages
 )
-
-from apex.op.utils import recursive_search
+from apex.core.calculator import LAMMPS_INTER_TYPE
+from apex.utils import recursive_search
 
 upload_packages.append(__file__)
 
 
 class RelaxMake(OP):
     """
     OP class for making calculation tasks
@@ -54,14 +54,15 @@
         parameter = param_argv["relaxation"]
 
         make_equi(structures, inter_parameter, parameter)
 
         conf_dirs = []
         for conf in structures:
             conf_dirs.extend(glob.glob(conf))
+        conf_dirs = list(set(conf_dirs))
         conf_dirs.sort()
 
         task_list = []
         task_list_str = []
         for ii in conf_dirs:
             conf_dir_global = os.path.join(work_d, ii)
             task_list.append(os.path.join(conf_dir_global, 'relaxation/relax_task'))
@@ -108,42 +109,56 @@
 
     @OP.exec_sign_check
     def execute(self, op_in: OPIO) -> OPIO:
         from ..core.common_equi import post_equi
         cwd = os.getcwd()
         param_argv = op_in['param']
         inter_param = param_argv["interaction"]
-        calculator = inter_param["type"]
+        inter_type = inter_param["type"]
         conf_list = param_argv["structures"]
         copy_dir_list_input = [conf.split('/')[0] for conf in conf_list]
         os.chdir(op_in['input_all'])
         copy_dir_list = []
         for ii in copy_dir_list_input:
             copy_dir_list.extend(glob.glob(ii))
 
         # find path of finished tasks
         os.chdir(op_in['input_post'])
         src_path = recursive_search(copy_dir_list)
         if not src_path:
             raise RuntimeError(f'Fail to find input work path after slices!')
 
         os.chdir(op_in['input_all'])
-        if calculator in ['vasp', 'abacus']:
+        if inter_type in ['vasp', 'abacus']:
             shutil.copytree(op_in['input_post'], './', dirs_exist_ok=True)
             post_equi(conf_list, inter_param)
         else:
             # src_path = str(input_post) + str(local_path)
             shutil.copytree(src_path, './', dirs_exist_ok=True)
             post_equi(conf_list, inter_param)
             conf_dirs = []
             for conf in conf_list:
                 conf_dirs.extend(glob.glob(conf))
+            conf_dirs = list(set(conf_dirs))
             conf_dirs.sort()
+
+            # remove potential files
+            inter_files_name = []
+            if inter_type in LAMMPS_INTER_TYPE:
+                if type(inter_param["model"]) is str:
+                    inter_files_name = [inter_param["model"]]
+                elif type(inter_param["model"]) is list:
+                    inter_files_name.extend(inter_param["model"])
+            elif inter_type == 'vasp':
+                inter_files_name = ['POTCAR']
+
             for ii in conf_dirs:
-                cmd = 'rm *.pb'
+                cmd = 'rm -f'
+                for jj in inter_files_name:
+                    cmd += f' {jj}'
                 os.chdir(ii)
                 subprocess.call(cmd, shell=True)
                 os.chdir(op_in['input_all'])
                 os.chdir(os.path.join(ii, 'relaxation/relax_task'))
                 subprocess.call(cmd, shell=True)
                 os.chdir(op_in['input_all'])
```

### Comparing `apex-flow-1.1.6/apex/run_step.py` & `apex_flow-1.2.0/apex/step.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import warnings
+import os
+
 from monty.serialization import loadfn
 from apex.core.common_equi import (make_equi, run_equi, post_equi)
 from apex.core.common_prop import (make_property, run_property, post_property)
-from apex.utils import get_flow_type, return_prop_list
+from apex.utils import get_flow_type, load_config_file
 
 
-def run_step(parameter, step, machine_file=None):
-    print('-------Singel step local debug mode--------')
-    param_dict = loadfn(parameter[0])
+def do_step(param_dict: dict, step: str, machine_dict: dict = None):
     # check input args
     json_type = get_flow_type(param_dict)
     mismatch1 = step in ['make_relax', 'run_relax', 'post_relax'] and json_type == 'props'
     mismatch2 = step in ['make_props', 'run_props', 'post_props'] and json_type == 'relax'
     if mismatch1 or mismatch2:
         raise RuntimeError(
             f'mismatched indication step ({step}) with type of json provided ({json_type})'
@@ -21,39 +20,49 @@
     if step in ['make_relax', 'run_relax', 'post_relax']:
         param = param_dict["relaxation"]
         if step == 'make_relax':
             print('Making relaxation tasks locally...')
             make_equi(structures, inter_parameter, param)
         elif step == 'run_relax':
             print('Run relaxation tasks locally...')
-            if not machine_file:
+            if not machine_dict:
                 raise RuntimeWarning(
                     'Miss configuration file for dpdispatcher (indicate by optional args -c).'
                     'Jobs will be running on the local shell.'
                 )
                 mdata = {}
             else:
-                mdata = loadfn(machine_file)
+                mdata = machine_dict
             run_equi(structures, inter_parameter, mdata)
         else:
             print('Posting relaxation results locally...')
             post_equi(structures, inter_parameter)
 
     elif step in ['make_props', 'run_props', 'post_props']:
         param = param_dict["properties"]
         if step == 'make_props':
             print('Making property tasks locally...')
             make_property(structures, inter_parameter, param)
         elif step == 'run_props':
             print('Run property tasks locally...')
-            if not machine_file:
+            if not machine_dict:
                 raise RuntimeWarning(
                     'Miss configuration file for dpdispatcher (indicate by optional args -c).'
                     'Jobs will be running on the local shell.'
                 )
                 mdata = {}
             else:
-                mdata = loadfn(machine_file)
+                mdata = machine_dict
             run_property(structures, inter_parameter, param, mdata)
         else:
             print('Posting property results locally...')
             post_property(structures, inter_parameter, param)
+
+
+def do_step_from_args(parameter: str, step: str, machine_file: os.PathLike = None):
+    print('-------Singel Step Local Debug Mode--------')
+    do_step(
+        param_dict=loadfn(parameter),
+        step=step,
+        machine_dict=load_config_file(machine_file)
+    )
+    print('Completed!')
```

### Comparing `apex-flow-1.1.6/apex/superop/PropertyFlow.py` & `apex_flow-1.2.0/apex/superop/SimplePropertySteps.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,29 +11,27 @@
     InputArtifact,
     InputParameter,
     Inputs,
     OutputArtifact,
     Outputs,
     Step,
     Steps,
+    argo_len,
     argo_range,
-    argo_enumerate
+    upload_artifact,
 )
 from dflow.python import (
     OP,
     PythonOPTemplate,
     Slices,
 )
 from dflow.plugins.dispatcher import DispatcherExecutor
-from apex.op.property_ops import DistributeProps, CollectProps
-from apex.superop.SimplePropertySteps import SimplePropertySteps
 
 
-class PropertyFlow(Steps):
-
+class SimplePropertySteps(Steps):
     def __init__(
         self,
         name: str,
         make_op: Type[OP],
         run_op: Type[OP],
         post_op: Type[OP],
         make_image: str,
@@ -44,49 +42,50 @@
         group_size: Optional[int] = None,
         pool_size: Optional[int] = None,
         executor: Optional[DispatcherExecutor] = None,
         upload_python_packages: Optional[List[os.PathLike]] = None,
     ):
         self._input_parameters = {
             "flow_id": InputParameter(type=str, value=""),
-            "parameter": InputParameter(type=dict)
+            "path_to_prop": InputParameter(type=str),
+            "prop_param": InputParameter(type=dict),
+            "inter_param": InputParameter(type=dict),
+            "do_refine": InputParameter(type=bool)
         }
         self._input_artifacts = {
             "input_work_path": InputArtifact(type=Path)
         }
-        self._output_parameters = {
-
-        }
+        self._output_parameters = {}
         self._output_artifacts = {
-            "retrieve_path": OutputArtifact(type=List[Path])
+            "retrieve_path": OutputArtifact(type=Path)
         }
 
         super().__init__(
             name=name,
             inputs=Inputs(
                 parameters=self._input_parameters,
                 artifacts=self._input_artifacts
             ),
             outputs=Outputs(
                 parameters=self._output_parameters,
                 artifacts=self._output_artifacts
             ),
         )
 
-        self._keys = ["distributor", "propcal", "collector"]
+        self._keys = ["make", "run", "post"]
         self.step_keys = {}
-        key = "distributor"
+        key = "make"
         self.step_keys[key] = '--'.join(
             [str(self.inputs.parameters["flow_id"]), key]
         )
-        key = "propcal"
+        key = "run"
         self.step_keys[key] = '--'.join(
-            [str(self.inputs.parameters["flow_id"]), key]
+            [str(self.inputs.parameters["flow_id"]), key + "-{{item}}"]
         )
-        key = "collector"
+        key = "post"
         self.step_keys[key] = '--'.join(
             [str(self.inputs.parameters["flow_id"]), key]
         )
 
         self._build(
             name,
             make_op,
@@ -135,79 +134,127 @@
         run_command: str,
         calculator: str,
         group_size: Optional[int] = None,
         pool_size: Optional[int] = None,
         executor: Optional[DispatcherExecutor] = None,
         upload_python_packages: Optional[List[os.PathLike]] = None,
     ):
-        distributor = Step(
-            name="Distributor",
-            template=PythonOPTemplate(DistributeProps,
-                                      image=make_image,
-                                      python_packages=upload_python_packages,
-                                      command=["python3"]),
+        # Step for property make
+        make = Step(
+            name="Props-make",
+            template=PythonOPTemplate(
+                make_op,
+                image=make_image,
+                python_packages=upload_python_packages,
+                command=["python3"]
+            ),
             artifacts={"input_work_path": self.inputs.artifacts["input_work_path"]},
-            parameters={"param": self.inputs.parameters["parameter"]},
-            key="distributor"
-        )
-        self.add(distributor)
-
-        simple_property_steps = SimplePropertySteps(
-            name='simple-property-flow',
-            make_op=make_op,
-            run_op=run_op,
-            post_op=post_op,
-            make_image=make_image,
-            run_image=run_image,
-            post_image=post_image,
-            run_command=run_command,
-            calculator=calculator,
-            group_size=group_size,
-            pool_size=pool_size,
-            executor=executor,
-            upload_python_packages=upload_python_packages
-        )
-
-        propscal = Step(
-            name="Prop-Cal",
-            template=simple_property_steps,
-            slices=Slices(
-                slices="{{item.order}}",
-                input_parameter=[
-                    "path_to_prop",
-                    "prop_param",
-                    "inter_param",
-                    "do_refine"
-                ],
-                input_artifact=["input_work_path"],
-                output_artifact=["output_post"],
+            parameters={"prop_param": self.inputs.parameters["prop_param"],
+                        "inter_param": self.inputs.parameters["inter_param"],
+                        "do_refine": self.inputs.parameters["do_refine"],
+                        "path_to_prop": self.inputs.parameters["path_to_prop"]},
+            key=self.step_keys["make"]
+        )
+        self.add(make)
+
+        # Step for property run
+        if calculator in ['vasp', 'abacus']:
+            run_fp = PythonOPTemplate(
+                run_op,
+                slices=Slices(
+                    "{{item}}",
+                    input_parameter=["task_name"],
+                    input_artifact=["task_path"],
+                    output_artifact=["backward_dir"],
+                    group_size=group_size,
+                    pool_size=pool_size
+                ),
+                python_packages=upload_python_packages,
+                image=run_image
+            )
+        if calculator == 'vasp':
+            runcal = Step(
+                name="PropsVASP-Cal",
+                template=run_fp,
+                parameters={
+                    "run_image_config": {"command": run_command},
+                    "task_name": make.outputs.parameters["task_names"],
+                    "backward_list": ["INCAR", "POSCAR", "OUTCAR", "CONTCAR",
+                                        "vasprun.xml"]
+                },
+                artifacts={
+                    "task_path": make.outputs.artifacts["task_paths"]
+                },
+                with_param=argo_range(argo_len(make.outputs.parameters["task_names"])),
+                key=self.step_keys["run"] + '-vasp',
+                executor=executor,
+            )
+        elif calculator == 'abacus':
+            runcal = Step(
+                name="PropsABACUS-Cal",
+                template=run_fp,
+                parameters={
+                    "run_image_config": {"command": run_command},
+                    "task_name": make.outputs.parameters["task_names"],
+                    "backward_list": ["OUT.ABACUS", "log"],
+                    "log_name": "log"
+                },
+                artifacts={
+                    "task_path": make.outputs.artifacts["task_paths"],
+                    "optional_artifact": upload_artifact({"pp_orb": "./"})
+                },
+                with_param=argo_range(argo_len(make.outputs.parameters["task_names"])),
+                key=self.step_keys["run"] + '-abacus',
+                executor=executor,
+            )
+        elif calculator == 'lammps':
+            run_lmp = PythonOPTemplate(
+                run_op,
+                slices=Slices(
+                    "{{item}}",
+                    input_artifact=["input_lammps"],
+                    output_artifact=["backward_dir"],
+                    group_size=group_size,
+                    pool_size=pool_size
+                ),
+                image=run_image,
+                python_packages=upload_python_packages,
+                command=["python3"]
+            )
+            runcal = Step(
+                name="PropsLAMMPS-Cal",
+                template=run_lmp,
+                artifacts={"input_lammps": make.outputs.artifacts["task_paths"]},
+                parameters={"run_command": run_command},
+                with_param=argo_range(make.outputs.parameters["njobs"]),
+                key=self.step_keys["run"] + '-lammps',
+                executor=executor,
+            )
+        else:
+            raise RuntimeError(f'Incorrect calculator type to initiate step: {calculator}')
+        self.add(runcal)
+
+        # Step for property post
+        post = Step(
+            name="Props-post",
+            template=PythonOPTemplate(
+                post_op,
+                image=post_image,
+                python_packages=upload_python_packages,
+                command=["python3"]
             ),
             artifacts={
-                "input_work_path": distributor.outputs.artifacts["orig_work_path"]
+                "input_post": runcal.outputs.artifacts["backward_dir"],
+                "input_all": make.outputs.artifacts["output_work_path"]
             },
             parameters={
-                "flow_id": "{{item.value}}",
-                "path_to_prop": distributor.outputs.parameters["path_to_prop"],
-                "prop_param": distributor.outputs.parameters["prop_param"],
-                "inter_param": distributor.outputs.parameters["inter_param"],
-                "do_refine": distributor.outputs.parameters["do_refine"]
+                "prop_param": self.inputs.parameters["prop_param"],
+                "inter_param": self.inputs.parameters["inter_param"],
+                "task_names": make.outputs.parameters["task_names"],
+                "path_to_prop": self.inputs.parameters["path_to_prop"]
             },
-            with_param=argo_enumerate(distributor.outputs.parameters["flow_id"]),
-            key="propscal-{{item}}"
-        )
-        self.add(propscal)
-
-        collector = Step(
-            name="PropsCollector",
-            template=PythonOPTemplate(CollectProps,
-                                      image=make_image,
-                                      python_packages=upload_python_packages,
-                                      command=["python3"]),
-            artifacts={"input_all": self.inputs.artifacts["input_work_path"],
-                       "input_post": propscal.outputs.artifacts["output_post"]},
-            parameters={"param": self.inputs.parameters["parameter"]},
-            key="collector"
+            key=self.step_keys["post"]
         )
-        self.add(collector)
+        self.add(post)
 
         self.outputs.artifacts["retrieve_path"]._from \
-            = collector.outputs.artifacts["retrieve_path"]
+            = post.outputs.artifacts["retrieve_path"]
```

### Comparing `apex-flow-1.1.6/apex/superop/RelaxationFlow.py` & `apex_flow-1.2.0/apex/superop/RelaxationFlow.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,16 @@
             raise RuntimeError(f'Incorrect calculator type to initiate step: {calculator}')
         self.add(runcal)
 
         post = Step(
             name="Relaxpost",
             template=PythonOPTemplate(post_op,
                                       image=post_image,
-                                      command=["python3"]),
+                                      command=["python3"],
+                                      python_packages=upload_python_packages,),
             artifacts={"input_post": runcal.outputs.artifacts["backward_dir"],
                        "input_all": make.outputs.artifacts["output"]},
             parameters={"param": self.inputs.parameters["parameter"]},
             key=self.step_keys["post"]
         )
         self.add(post)
```

### Comparing `apex-flow-1.1.6/apex_flow.egg-info/PKG-INFO` & `apex_flow-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,97 @@
-Metadata-Version: 2.1
-Name: apex-flow
-Version: 1.1.6
-Summary: Alloy Properties EXplorer using simulations
-Home-page: https://github.com/deepmodeling/APEX.git
-Author: Zhuoyuan Li, Tongqi Wen
-Author-email: zhuoyli@outlook.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pydflow>=1.7.83
-Requires-Dist: pymatgen>=2023.8.10
-Requires-Dist: pymatgen-analysis-defects>=2023.8.22
-Requires-Dist: dpdata>=0.2.13
-Requires-Dist: dpdispatcher
-Requires-Dist: phonoLAMMPS
-Requires-Dist: phonopy
-Requires-Dist: matplotlib
-Requires-Dist: seekpath
-Requires-Dist: fpop>=0.0.7
-Requires-Dist: boto3
-
-# APEX: Alloy Property EXplorer using simulations
-
-[APEX](https://github.com/deepmodeling/APEX): Alloy Property EXplorer using simulations, is a component of the [AI Square](https://aissquare.com/) project that involves the restructuring of the [DP-Gen](https://github.com/deepmodeling/dpgen) `auto_test` module to develop a versatile and extensible Python package for general alloy property testing. This package enables users to conveniently establish a wide range of property-test workflows by utilizing various computational approaches, including support for LAMMPS, VASP, and ABACUS.
-
-## New Features Update (v1.0)
-* Enable the calculation of `phonon` spectrum (v1.1.0)
-* Decouple property calculations into individual sub-workflow to facilitate the customization of complex property functions
-* Support one-click parallel submission of multiple workflows
-* Integrate a single step test mode for `run` steps, providing an interaction method similar to `auto_test`
-* Allow users to modify task submission concurrency via `group_size` and `pool_size`
-* Enable users to customize `suffix` of property calculation directory so that multiple tests with identical property templates but different settings can be run within one workflow
-* Refactor and optimize the command line interaction for improved usability
-* Enhance robustness across diverse use scenarios, especially for the local debug mode
+<div style="text-align: center;">
+    <img src="./docs/images/logo.png" style="zoom: 15%;">
+</div>
+
+# APEX: Alloy Property EXplorer
+[![](https://img.shields.io/badge/release-1.2.0-blue.svg)](https://github.com/deepmodeling/APEX)
+
+[APEX](https://github.com/deepmodeling/APEX): Alloy Property EXplorer is a component of the [AI Square](https://aissquare.com/) project that involves the restructuring of the [DP-GEN](https://github.com/deepmodeling/dpgen) `auto_test` module to develop a versatile and extensible Python package for general alloy property calculations. This package enables users to conveniently establish a wide range of cloud-native property-test workflows by utilizing various computational approaches, including LAMMPS, VASP, ABACUS, and others.
+
+## v1.2 Main Features Update
+* Add a `retrieve` sub-command to allow results to be retrieved independently and manually for multiple properties (Remove `Distributor` and `Collector` OP)
+* Support common **dflow operations** with terminal commands
+* Incorporate results `archive` function to both local paths and NoSQL database ([MongoDB](https://www.mongodb.com/) and [DynamoDB](https://aws.amazon.com/cn/dynamodb/))
+* Add a `report` sub-command for quick results visualization and cross-comparison via a front-end APP based on [Dash](https://dash.plotly.com)
+* Support [SeeK-path](https://seekpath.readthedocs.io/en/latest/index.html) for automatic band path search in `phonon` calculations
+* Support eight conventional HCP interstitial configurations for `interstitial` calculations
+* Add four additional **ML** pair styles (`snap`, `gap`, `rann` and `mace`) and an extra `meam-spline` in LAMMPS interation type support
+* Modify the single-step run command from `test` to `do` for improved clarity and consistencey
+
+## APEX Bohrium App
+[![](https://img.shields.io/badge/APP-BohriumApp-orange.svg)](https://app.bohrium.dp.tech/apex/)
+
+APEX also provides a web-based [Bohrium App](https://app.bohrium.dp.tech/apex/) for rapid and easy alloy property calculations without intensive JSON configuration (Note: one will need a Bohrium account to access this service).
+
+## How to cite APEX
+[![](https://img.shields.io/badge/DOI-10.48550/arXiv.2404.17330-red.svg)](https://doi.org/10.48550/arXiv.2404.17330)
+
+If you use APEX in your research, please cite the following paper for general purpose: 
+
+> Z. Li, T. Wen, Y. Zhang, X. Liu, C. Zhang, A. S. L. S. Pattamatta, X. Gong, B. Ye, H.Wang, L. Zhang, D. J. Srolovitz, An extendable cloud-native alloy property explorer (2024). arXiv:2404.17330.
 
 ## Table of Contents
 
-- [APEX: Alloy Property EXplorer using simulations](#apex-alloy-property-explorer-using-simulations)
-  - [New Features Update (v1.0)](#new-features-update-v10)
+- [APEX: Alloy Property EXplorer](#apex-alloy-property-explorer)
+  - [v1.2 Main Features Update](#v12-main-features-update)
+  - [APEX Bohrium App](#apex-bohrium-app)
+  - [How to cite APEX](#how-to-cite-apex)
   - [Table of Contents](#table-of-contents)
   - [1. Overview](#1-overview)
   - [2. Easy Install](#2-easy-install)
   - [3. User Guide](#3-user-guide)
     - [3.1. Before Submission](#31-before-submission)
       - [3.1.1. Global Setting](#311-global-setting)
       - [3.1.2. Calculation Parameters](#312-calculation-parameters)
         - [3.1.2.1. EOS](#3121-eos)
         - [3.1.2.2. Elastic](#3122-elastic)
         - [3.1.2.3. Surface](#3123-surface)
         - [3.1.2.4. Vacancy](#3124-vacancy)
         - [3.1.2.5. Interstitial](#3125-interstitial)
         - [3.1.2.6. Gamma Line](#3126-gamma-line)
-        - [3.1.2.7. Phonon Spectrum](#3127-phonon-spectrum)
-    - [3.2. Command](#32-command)
+        - [3.1.2.7. Phonon Spectra](#3127-phonon-spectra)
+    - [3.2. Submission](#32-submission)
       - [3.2.1. Workflow Submission](#321-workflow-submission)
-      - [3.2.2. Single-Step Test](#322-single-step-test)
+      - [3.2.2. Workflow Inquiry \& Operations](#322-workflow-inquiry--operations)
+      - [3.2.3. Run Individual Step](#323-run-individual-step)
+    - [3.3. After Submission](#33-after-submission)
+      - [3.3.1. Retrieve Results Manually](#331-retrieve-results-manually)
+      - [3.3.2. Archive Test Results](#332-archive-test-results)
+      - [3.3.3. Results Visualization Report](#333-results-visualization-report)
   - [4. Quick Start](#4-quick-start)
     - [4.1. In the Bohrium](#41-in-the-bohrium)
     - [4.2. In a Local Argo Service](#42-in-a-local-argo-service)
     - [4.3. In a Local Environment](#43-in-a-local-environment)
 
 ## 1. Overview
 
 APEX adopts the functionality of the second-generation `auto_test` for alloy properties calculations and is developed utilizing the [dflow](https://github.com/deepmodeling/dflow) framework. By integrating the benefits of cloud-native workflows, APEX streamlines the intricate procedure of automatically testing various configurations and properties. Owing to its cloud-native characteristic, APEX provides users with a more intuitive and user-friendly interaction, enhancing the overall user experience by eliminating concerns related to process control, task scheduling, observability, and disaster tolerance.
 
 The comprehensive architecture of APEX is demonstrated below:
 
-<div>
-    <img src="./docs/images/apex_demo.png" alt="Fig1" style="zoom: 35%;">
-    <p style='font-size:1.0rem; font-weight:none'>Figure 1. APEX schematic diagram</p>
+<div style="text-align: center;">
+    <img src="./docs/images/flowchart.png" alt="Fig1" style="zoom: 40%;">
+    <p style='font-size:1.0rem; font-weight:none'>Figure 1. Schematic diagram of APEX</p>
 </div>
 
 APEX consists of three types of pre-defined **workflow** that users can submit: `relaxation`, `property`, and `joint`. The `relaxation` and `property` sub-workflow comprise three sequential **steps**: `Make`, `Run`, and `Post`, while the `joint` workflow essentially combines the `relaxation` and `property` workflows into a comprehensive workflow.
 
-The `relaxation` process begins with the initial `POSCAR` supplied by the user, which is used to generate crucial data such as the final relaxed structure and its corresponding energy, forces, and virial tensor. This equilibrium state information is essential for input into the `property` workflow, enabling further calculations of alloy properties. Upon completion, the final results are automatically retrieved and downloaded to the original working directory.
+The `relaxation` process begins with the initial `POSCAR` supplied by the user, which is used to generate critical data such as the final relaxed structure and its corresponding energy, forces, and virial tensor. This equilibrium state information is essential for input into the `property` workflow, enabling further calculations of alloy properties. Upon completion, the final results are automatically retrieved and downloaded to the original working directory.
 
 In both the `relaxation` and `property` workflows, the `Make` step prepares the corresponding computational tasks. These tasks are then transferred to the `Run` step that is responsible for task dispatch, calculation monitoring, and retrieval of completed tasks (implemented through the [DPDispatcher](https://github.com/deepmodeling/dpdispatcher/tree/master) plugin). Upon completion of all tasks, the `Post` step is initiated to collect data and obtain the desired property results.
 
-APEX currently offers computation methods for the following alloy properties:
+APEX currently offers calculation methods for the following alloy properties:
 
 * Equation of State (EOS)
 * Elastic constants
 * Surface energy
 * Interstitial formation energy
 * Vacancy formation energy
 * Generalized stacking fault energy (Gamma line)
-* Phonon spectrum
+* Phonon spectra
 
 Moreover, APEX supports three types of calculators: **LAMMPS** for molecular dynamics simulations, and **VASP** and **ABACUS** for first-principles calculations.
 
 ## 2. Easy Install
 Easy install by
 ```shell
 pip install apex-flow
@@ -120,26 +119,28 @@
 
 * **Basic config**
   | Key words | Data structure | Default | Description |
   | :------------ | ----- | ----- | ------------------- |
   | apex_image_name | String | zhuoy/apex_amd64 | Image for step other than `run`. One can build this Docker image via prepared [Dockerfile](./docs/Dockerfile) |
   | run_image_name | String | None | Image of calculator for `run` step. Use `{calculator}_image_name` to indicate corresponding image for higher priority |
   | run_command | String | None | Shell command for `run` step. Use `{calculator}_run_command` to indicate corresponding command for higher priority |
-  | group_size | Int | 1 | Number of tasks per parallel run group. |
+  | group_size | Int | 1 | Number of tasks per parallel run group |
   | pool_size | Int | 1 | For multi tasks per parallel group, the pool size of multiprocessing pool to handle each task (1 for serial, -1 for infinity) |
   | upload_python_package | Optional[List] | None | Additional python packages required in the container |
-  | debug_pool_workers | Int | 1 | Pool size of parallel tasks running in the debug mode |
+  | debug_pool_workers | Int | 1 | Pool size of parallel tasks running in the debug mode | 
+  | flow_name | String | None | Specify name of workflow to be submitted (default: work path name) |
+  | submit_only | Bool | False | Submit workflow only without automatic result retrieving |
 
 * **Dflow config**
   | Key words | Data structure | Default | Description |
   | :------------ | ----- | ----- | ------------------- |
   | dflow_host | String | https://127.0.0.1:2746 | Url of dflow server |
   | k8s_api_server | String | https://127.0.0.1:2746 | Url of kubernetes API server |
-  | dflow_config | Optional[Dict] | None | Specify more detailed dflow config in a nested dictionary with higher priority (See [dflow document](https://deepmodeling.com/dflow/dflow.html) for more detail). |
-  | dflow_s3_config | Optional[Dict] | None | Specify dflow s3 repository config in a nested dictionary with higher priority (See [dflow document](https://deepmodeling.com/dflow/dflow.html) for more detail). |
+  | dflow_config | Optional[Dict] | None | Specify more detailed dflow config in a nested dictionary with higher priority (See [dflow document](https://deepmodeling.com/dflow/dflow.html) for more detail) |
+  | dflow_s3_config | Optional[Dict] | None | Specify dflow s3 repository config in a nested dictionary with higher priority (See [dflow document](https://deepmodeling.com/dflow/dflow.html) for more detail) |
 
 * **Dispatcher config** (One may refer to [DPDispatcher’s documentation](https://docs.deepmodeling.com/projects/dpdispatcher/en/latest/index.html) for details of the following parameters)
   | Key words | Data structure | Default | Description |
   | :------------ | ----- | ----- | ------------------- |
   | context_type | String | None | Context type to connect to the remote server |
   | batch_type | String | None | System to dispatch tasks |
   | local_root | String | "./" | Local root path |
@@ -262,50 +263,57 @@
   ```
 ##### 3.1.2.1. EOS
   | Key words | Data structure | Example | Description                                               |
   | :------------ | ----- |-----------------------------------------------------------| ------------------- |
   | vol_start | Float | 0.9 | The starting volume related to the equilibrium structure  |
   | vol_end | Float | 1.1 | The maximum volume related to the equilibrium structure   |
   | vol_step | Float | 0.01 | The volume increment related to the equilibrium structure |
+  | vol_abs | Bool | False | Whether to treat vol_start and vol_end as absolute volume, default = False |
 
 ##### 3.1.2.2. Elastic
-  | Key words | Data structure | Example | Description                                         |
-  | :------------ | ----- |-----------------------------------------------------| ------------------- |
-  | norm_deform | Float | 1.1 | The deformation in xx, yy, zz, defaul = 1e-2        |
-  | shear_deform | Float | 0.01 | The deformation in other directions, default = 1e-2 |
+  | Key words    | Data structure | Example | Description                                                                                                                       |
+  |:-------------|----------------|---------|-----------------------------------------------------------------------------------------------------------------------------------|
+  | norm_deform  | Float          | 0.01    | The deformation in xx, yy, zz, defaul = 1e-2                                                                                      |
+  | shear_deform | Float          | 0.01    | The deformation in other directions, default = 1e-2                                                                               |
+  | conventional | Bool           | False   | Whether adopt conventional cell for deformation                                                                                   |
+  | ieee         | Bool           | True    | Whether rotate relaxed structure into IEEE-standard format before deformation ([ref](https://ieeexplore.ieee.org/document/26560)) |
 
 ##### 3.1.2.3. Surface
-  | Key words | Data structure | Example | Description                                                                      |
+  | Key words | Data structure | Example | Description |
   | :------------ | ----- |----------------------------------------------------------------------------------| ------------------- |
-  | min_slab_size | Int | 10 | Minimum size of slab thickness                                                   |
-  | min_vacuum_size | Int | 11 | Minimum size of vacuum width                                                     |
+  | min_slab_size | Int | 10 | Minimum size of slab thickness |
+  | min_vacuum_size | Int | 11 | Minimum size of vacuum width |
   | pert_xz | Float | 0.01 | Perturbation through xz direction used to compute surface energy, default = 0.01 |
-  | max_miller | Int | 2 | The maximum miller index number of surface generated                             |
+  | max_miller | Int | 2 | The maximum miller index number of surface, default = 2 |
 
 ##### 3.1.2.4. Vacancy
   | Key words | Data structure | Example | Description |
   | :------------ | ----- | ----- | ------------------- |
   | supercell | List[Int] | [3, 3, 3] | The supercell to be constructed, default = [1,1,1] |
 
 ##### 3.1.2.5. Interstitial
   | Key words | Data structure | Example | Description |
   | :------------ | ----- | ----- | ------------------- |
   | insert_ele | List[String] | ["Al"] | The element to be inserted |
-  | supercell | List[Int] | [3, 3, 3] | The supercell to be constructed, default =[1,1,1] |
+  | supercell | List[Int] | [3, 3, 3] | The supercell to be constructed, default = [1,1,1] |
   | conf_filters | Dict | "min_dist": 1.5 | Filter out the undesirable configuration |
+  <div>
+      <img src="./docs/images/interstitial_table.png" alt="Fig3" style="zoom: 90%;">
+      <p style='font-size:1.0rem; font-weight:none'> </p>
+  </div>
 
 ##### 3.1.2.6. Gamma Line
-  <div>
+  <div style="text-align: center;">
       <img src="./docs/images/gamma_demo.png" alt="Fig2" style="zoom: 35%;">
       <p style='font-size:1.0rem; font-weight:none'>Figure 2. Schematic diagram of Gamma line calculation</p>
   </div>
 
-The Gamma line (generalized stacking fault energy) function of APEX calculates energy of a series slab structures of specific crystal plane, which displaced in the middle along a slip vector as illustrated in **Figure 2**. In APEX, the slab structrures are defined by a plane miller index and two orthogonal directions (primary and secondary) on the plane. The **slip vector is always along the primary directions** with slip length defined by users or default settings. Thus, by indicating `plane_miller` and the `slip_direction` (AKA, primary direction), a slip system can be defined.
+The Gamma line (generalized stacking fault energy) function of APEX calculates energy of a series slab structures of specific crystal plane, which displaced in the middle along a slip vector as illustrated in **Figure 2**. In APEX, the slab structrures are defined by a plane miller index and two orthogonal directions (primary and secondary) on the plane. The **slip vector is always along the primary directions** with slip length defined by users or default settings. Thus, by indicating `plane_miller` and the `slip_direction` (i.e., primary direction), a slip system can be defined.
 
-For most common slip systems in respect to FCC, BCC and HCP crystal structures, slip direction, secondary direction and default fractional slip lengths are already documented and listed below (users are **strongly advised** to follow those pre-defined slip system, or may need to double-check the generated slab structure, as unexpected results may occur especially for system like HCP):
+For most common slip systems in FCC, BCC and HCP crystal structures, slip direction, secondary direction and default fractional slip lengths are already documented and listed below (users are **strongly advised** to follow those pre-defined slip system, or may need to double-check the generated slab structure, as unexpected results may occur especially for system like HCP):
 * FCC
   | Plane miller index | Slip direction | Secondary direction | Default slip length |
   | :-------- | ----- | ----- | ---- |
   | $(001)$ | $[100]$ | $[010]$ | $a$ |
   | $(110)$ | $[\bar{1}10]$ | $[001]$ | $\sqrt{2}a$ |
   | $(111)$ | $[11\bar{2}]$ | $[\bar{1}10]$ | $\sqrt{6}a$ |
   | $(111)$ | $[\bar{1}\bar{1}2]$ | $[1\bar{1}0]$ | $\sqrt{6}a$ |
@@ -346,15 +354,15 @@
   | :------------ | ----- | ----- | ------------------- |
   | plane_miller | Sequence[Int] | None | Miller index of the target slab |
   | slip_direction | Sequence[Int] | None | Miller index of slip (primary) direction of the slab |
   | slip_length | Int\|Float; Sequence[Int\|Float, Int\|Float, Int\|Float] | Refer to specific slip system as the table shows above, or 1 if not indicated | Slip length along the primary direction with default unit set by users or default setting. As for format of `[x, y, z]`, the length equals to $\sqrt{(xa)^2+(yb)^2+(zc)^2}$ |
   | plane_shift | Int\|Float | 0 | Shift of displacement plane with unit of lattice parameter **$c$** (positive for upwards). This allows creating slip plane within narrowly-spaced planes (see [ref](https://doi.org/10.1016/j.actamat.2016.10.042)). |
   | n_steps | Int | 10 | Number of steps to displace slab along the slip vector  |
   | vacuum_size | Int\|Float | 0 | Thickness of vacuum layer added around the slab with unit of Angstrom |
-  | supercell_size | Sequence[Int, Int, Int] | [1, 1, 5] | Size of generated supper cell based on slab structure |
+  | supercell_size | Sequence[Int, Int, Int] | [1, 1, 5] | Size of generated supercell based on slab structure |
   | add fix | Sequence[Str, Str, Str] | ["true","true","false"] | Whether to add fix position constraint along x, y and z direction during calculation |
 
   Here is an example:
   ```json
   {
 	  "type":            "gamma",
 	  "skip":            true,
@@ -370,59 +378,80 @@
       "vacuum_size": 10,
 	  "add_fix": ["true","true","false"],
       "n_steps":         10
 	}
   ```
   It should be noted that for various crystal structures, **users can further define slip parameters within the respective nested dictionaries, which will be prioritized for adoption**. In the example above, the slip system configuration within the "hcp" dictionary will be utilized.
 
-##### 3.1.2.7. Phonon Spectrum
-This function incorporates part of [dflow-phonon](https://github.com/Chengqian-Zhang/dflow-phonon) codes into APEX to enhance its comprehensiveness. This workflow is facilitated via [Phonopy](https://github.com/phonopy/phonopy), in conjunction with [phonoLAMMPS](https://github.com/abelcarreras/phonolammps) for LAMMPS calculations. 
+##### 3.1.2.7. Phonon Spectra
+This function incorporates part of [dflow-phonon](https://github.com/Chengqian-Zhang/dflow-phonon) codes into APEX to make it more complete. This workflow is realized via [Phonopy](https://github.com/phonopy/phonopy), and [phonoLAMMPS](https://github.com/abelcarreras/phonolammps) for LAMMPS calculation. In APEX, this part includes the [SeeK-path](https://seekpath.readthedocs.io/en/latest/index.html) for automatically high-symmetry points searching for phonon calculation.
 
-**IMPORTANT!!**: it should be noticed that the **phonoLAMMPS** package must be pre-installed in the user's `run_image` to ensure accurate `LAMMPS` calculations for the phonon spectrum.
+**IMPORTANT!!**: it should be noted that the **phonoLAMMPS** package must be pre-installed in the user's `run_image` to ensure accurate `LAMMPS` calculations for the phonon spectra.
 
 Parameters related to `Phonon` calculations are listed below:
   | Key words | Data structure | Default | Description |
   | :------------ | ----- | ----- | ------------------- |
   | primitive | Bool | False | Whether to find primitive lattice structure for phonon calculation |
   | approach | String | "linear" | Specify phonon calculation method when using `VASP`; Two options: 1. "linear" for the *Linear Response Method*, and 2. "displacement" for the *Finite Displacement Method* |
   | supercell_size | Sequence[Int] | [2, 2, 2] | Size of supercell created for calculation |
-  | MESH | Sequence[Int] | None | Define the dimensions of the grid in reciprocal space, which will be utilized for the calculation of phonon frequencies and eigenvectors. For example: [8, 8, 8]; Refer to [Phonopy MESH](http://phonopy.github.io/phonopy/setting-tags.html#mesh-sampling-tags) |
-  | PRIMITIVE_AXES | String | None | To define the basis vectors of a primitive cell with reference to the basis vectors of a conventional cell, facilitating input cell transformation. For example: "0.0 0.5 0.5 0.5 0.0 0.5 0.5 0.5 0.0"; Refer to [Phonopy PRIMITIVE_AXES](http://phonopy.github.io/phonopy/setting-tags.html#primitive-axes-or-primitive-axis) |
-  | BAND | String | None | Indicate band path in reciprocal space as format of [Phonopy BAND](http://phonopy.github.io/phonopy/setting-tags.html#band-and-band-points); For example: "0 0 0 1/2 0 1/2, 1/2 1/2 1 0 0 0 1/2 1/2 1/2" |
+  | MESH | Sequence[Int] | None | Specify the dimensions of the grid in reciprocal space for which the phonon frequencies and eigenvectors are to be calculated. For example: [8, 8, 8]; Refer to [Phonopy MESH](http://phonopy.github.io/phonopy/setting-tags.html#mesh-sampling-tags) |
+  | PRIMITIVE_AXES | String | None | To define the basis vectors of a primitive cell in terms of the basis vectors of a conventional cell for input cell transformation. For example: "0.0 0.5 0.5 0.5 0.0 0.5 0.5 0.5 0.0"; Refer to [Phonopy PRIMITIVE_AXES](http://phonopy.github.io/phonopy/setting-tags.html#primitive-axes-or-primitive-axis) |
+  | BAND | String | None | (Optional) Indicate band path in reciprocal space as format of [Phonopy BAND](http://phonopy.github.io/phonopy/setting-tags.html#band-and-band-points); For example: "0 0 0 1/2 0 1/2, 1/2 1/2 1 0 0 0 1/2 1/2 1/2". If not specified, the [seekpath](https://seekpath.readthedocs.io/en/latest/#) package will be adopted to automatically determine band path according to relaxed structure |
+  | BAND_LABELS | String | None | (Optional) Indication of band path labels for report plot |
   | BAND_POINTS | Int | 51 | Number of sampling points including the path ends |
-  | BAND_CONNECTION | Bool | True | With this option, band connections are estimated from eigenvectors and band structure is drawn by considering band crossings. In sensitive cases, to obtain better band connections, it requires to increase the number of points calculated in band segments by the `BAND_POINTS` tag. |
+  | BAND_CONNECTION | Bool | True | With this option, band connections are estimated from eigenvectors and band structure is drawn considering band crossings. In sensitive cases, to obtain better band connections, it requires to increase number of points calculated in band segments by the `BAND_POINTS` tag |
+  | seekpath_from_original | Bool | False | Whether to re-seek standard primitive cell for relaxed structure for band path via the seekpath package. If True: `seekpath.get_path_orig_cell` will be adopted, else: `seekpath.get_path`. Refer to [seekpath document](https://seekpath.readthedocs.io/en/latest/maindoc.html#k-point-path-for-non-standard-unit-cells) |
+  | seekpath_param | Dict | None | (Optional) Other parameters to be specified for `seekpath.get_path` and `seekpath.get_path`. Refer to [seekpath document](https://seekpath.readthedocs.io/en/latest/maindoc.html#k-point-path-for-non-standard-unit-cells) |
 
-When utilizing `VASP`, you have **two** primary calculation methods at your disposal: the **Linear Response Method** and the **Finite Displacement Method**.
+When utilizing `VASP`, you have **two** primary calculation methods: the **Linear Response Method** and the **Finite Displacement Method**.
 
 The **Linear Response Method** has an edge over the Finite Displacement Method in that it eliminates the need for creating super-cells, thereby offering computational efficiency in certain cases. Additionally, this method is particularly well-suited for systems with anomalous phonon dispersion (like systems with Kohn anomalies), as it can precisely calculate the phonons at the specified points.
 
-On the other hand, the **Finite Displacement Method**'s advantage lies in its versatility; it functions as an add-on compatible with any code, including those beyond the scope of density functional theory. The only requirement is that the external code can compute forces. For instance, ABACUS may lack an implementation of the Linear Response Method, but can effectively utilize the Finite Displacement Method implemented in phonon calculation.
+On the other hand, the advantage of **Finite Displacement Method** lies in its versatility; it functions as an add-on compatible with any code, including those beyond the scope of density functional theory. The only requirement is that the external code can compute forces. For instance, ABACUS may lack an implementation of the Linear Response Method, but can effectively utilize the Finite Displacement Method implemented in phonon calculations.
 
 
-### 3.2. Command
-APEX currently supports two seperate run modes: **workflow submission** (running via dflow) and **single-step test** (running without dflow).
-
+### 3.2. Submission
 #### 3.2.1. Workflow Submission
-APEX will execute a specific dflow workflow upon each invocation of the command in the format: `apex submit [-h] [-c [CONFIG]] [-w WORK [WORK ...]] [-d] [-f {relax,props,joint}] parameter [parameter ...]`. The type of workflow and calculation method will be automatically determined by APEX based on the parameter file provided by the user. Additionally, users can specify the **workflow type**, **configuration JSON file**, and **work directory** through an optional argument (Run `apex submit -h` for help). Here is an example to submit a `joint` workflow:
+APEX will execute a specific dflow workflow upon each invocation of the command in the format: `apex submit [-h] [-c [CONFIG]] [-w WORK [WORK ...]] [-d] [-s] [-f {relax,props,joint}] parameter [parameter ...]`. The type of workflow and calculation method will be automatically determined by APEX based on the parameter file provided by users. Additionally, users can specify the **workflow type**, **configuration JSON file**, and **work directory** through an optional argument (Run `apex submit -h` for further help). Here is an example to submit a `joint` workflow:
 ```shell
 apex submit param_relax.json param_props.json -c ./global_bohrium.json -w 'dp_demo_0?' 'eam_demo'
 ```
-if no config JSON and work directory is specified, `./global.json` and `./` will be passed as default values respectively. 
+if no config JSON (following `-c`) and work directory (following `-w`) is specified, `./global.json` and `./` will be passed as default values respectively.
+
+#### 3.2.2. Workflow Inquiry & Operations
+APEX supports several commonly used `dflow` inquiry and operation commands as listed below:
+- `list`: List all workflows information
+- `get`: Get detailed information of a workflow
+- `getsteps`: Get detailed steps information of a workflow 
+- `getkeys`: Get keys of steps from a workflow
+- `delete`: Delete a workflow
+- `resubmit`: Resubmit a workflow
+- `retry`: Retry a workflow
+- `resume`: Resume a workflow
+- `stop`: Stop a workflow
+- `suspend`: Suspend a workflow
+- `terminate` Terminate a workflow
+  
+Take `stop` as an example (usage: `apex stop [-h] [-i ID] [-w WORK] [-c [CONFIG]]`) user can refer to following three options:
+1. `apex stop`, as running at the target `work_dir`, and apex will inquiry workflow `ID` from `.workflow.log` file under the current path (`config.json` is the default config file)
+2. `apex stop -w ./EAM_Ti -c ./EAM_Ti/config.json` to indicate target `work_dir` to stop
+3. `apex stop -i relax-fe03j4 -c ./config_bohrium.json` to indicate specific workflow `ID` to stop
+   
 
-#### 3.2.2. Single-Step Test
-APEX also provides a **single-step test mode**, which can run `Make` `run` and `Post` step individually under local enviornment. **Please note that one needs to run command under the work directory in this mode.** Users can invoke them by format of `apex test [-h] [-m [MACHINE]] parameter {make_relax,run_relax,post_relax,make_props,run_props,post_props}` (Run `apex test -h` for help). Here is a example to do relaxation in this mode:
+#### 3.2.3. Run Individual Step 
+APEX also provides a **single-step test mode**, which can run `Make` `run` and `Post` step individually under local enviornment. **Please note that one needs to run commands under the work directory in this mode.** User can invoke them by format of `apex run [-h] [-c [CONFIG]] parameter {make_relax,run_relax,post_relax,make_props,run_props,post_props}` (Run `apex run -h` for help). Here is a example to do relaxation in this mode:
 1. Firstly, generate relaxation tasks by
    ```shell
-   apex test param_relax.json make_relax
+   apex do param_relax.json make_relax
    ```
 2. Then dispatch tasks by
    ```shell
-   apex test param_relax.json run_relax -m machine.json
+   apex do param_relax.json run_relax -c machine.json
    ```
-   where `machine.json` is a JSON file to define dispatch method, containing `machine`, `resources`, `task` dictionaries and `run_command` as listed in [DPDispatcher’s documentation](https://docs.deepmodeling.com/projects/dpdispatcher/en/latest/index.html). Here is an example to submit tasks to a [Slurm](https://slurm.schedmd.com) managed remote HPC:
+   where `machine.json` is a JSON file to define dispatch method, containing `machine`, `resources`, `task` dictionaries and `run_command` as listed in [DPDispatcher’s documentation](https://docs.deepmodeling.com/projects/dpdispatcher/en/latest/index.html). Here is an example to submit tasks to a remote HPC managed by [Slurm](https://slurm.schedmd.com):
    ```json
     {
       "run_command": "lmp -i in.lammps -v restart 0",
       "machine": {
           "batch_type": "Slurm",
           "context_type": "SSHContext",
           "local_root" : "./",
@@ -448,19 +477,82 @@
                 "#SBATCH --mem=10G",
                 "#SBATCH --nodes=1",
                 "#SBATCH --time=1-00:00:00"
           ]
       }
     }
    ```
-3. Finally, as all tasks are finished, post process by
+3. Finally, when all tasks are finished, post-process by
    ```shell
-   apex test param_relax.json post_relax
+   apex do param_relax.json post_relax
    ```
-The property test can follow similar approach.
+The property test can follow a similar approach.
+
+### 3.3. After Submission
+
+#### 3.3.1. Retrieve Results Manually
+
+Sometimes when results auto-retrieving fails after workflows finish, you may try to retrieve completed test results manually by the `retrieve` command with a specific workflow `ID` (or target `work_dir`) provided:
+```shell
+apex retrieve [-h] [-i ID] [-w WORK] [-c [CONFIG]]
+```
+where the `WORK` defaults to be `./`, and the `CONFIG` JSON (default: `config.json`) is used to connect to the remote storage. The command usage to similar to [3.2.2. Workflow Inquiry \& Operations](#322-workflow-inquiry--operations)
+
+#### 3.3.2. Archive Test Results
+After completion of each workflow, the results and test parameters of corresponding property will be stored as `json` format automatically under respective work directory named as `all_result.json`. You can also do this manually to update this file based on the latest run by:
+
+```shell
+apex archive [parameter …]
+```
+Argument format of this sub-command is similar to that of `submit` command. Please use `apex archive -h` for complete usage introduction. It should be noticed that each `archive` command will only update property information of those identified as **active** according to the parameter files and indication provided similar to the `submit` mode.
+
+This mode can also archive results to **NoSQL** database. We currently support two types of database client: [MongoDB](https://www.mongodb.com/) and [DynamoDB](https://aws.amazon.com/cn/dynamodb/). Below shows global configuration parameters for two database archive:
+
+  | Key words | Data structure | Default | Description |
+  | :------------ | ----- | ----- | ------------------- |
+  | database_type | String | local | Database type, three choices available: `local` (only archive to local `all_result.json`), `mongodb` and `dynamodb`. One can also indicate this by `-d` within `archive` command |
+  | archive_method | String | sync | Choose from `sync` and `record`. `sync` synchronizes and updates results into same item based on work directory id; `record` records each archived result into a new item with unique timestamp. One can also indicate this by `-m` within `archive` command |
+
+  For `MongoDB`:
+  | Key words | Data structure | Default | Description |
+  | :------------ | ----- | ----- | ------------------- |
+  | mongodb_host | String | localhost | `Mongodb` host |
+  | mongodb_port | Int | 27017 | `Mongodb` port |
+  | mongodb_database | String | apex_results | `Mongodb` database name |
+  | mongodb_collection | String | apex_results | `Mongodb` collection name |
+  | mongodb_config | Dict | None | Complete parameter dictionary for [MongoClient](https://www.mongodb.com/blog/post/introducing-mongoclient) |
+
+  For `DynamoDB`:
+  | Key words | Data structure | Default | Description |
+  | :------------ | ----- | ----- | ------------------- |
+  | dynamodb_table_name | String | apex_results | `Dynamodb` table name |
+  | dynamodb_config | Dict | None | Complete parameter dictionary for [boto3 session](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/session.html#boto3.session.Session.resource) |
+
+#### 3.3.3. Results Visualization Report
+Note that this mode **only** runs on computer with **interactive UI** frontend. 
+In this mode, APEX will create a comprehensive and interactive results visualization report according to `all_result.json` within indicated work directories. This is achieved through [Dash](https://dash.plotly.com) App. You can invoke the report app simply under target work directory by:
+```shell
+apex report
+```
+Or indicate multiple work directories or path of result file in `json` format by `-w` for cross-comparison. Here is an example:
+```shell
+apex report -w DP/all_result.json ./MEAM_00*
+```
+Once the report app is opened (or manully via http://127.0.0.1:8050/), users can select configurations and property types. Then the corresponding result plot and data table will be shown accordingly.
+**NOTE**:
+- If two Dash pages are automatically opened in your browser, you can close the first one.
+- If the clipboard buttons do not function well, try to reload the page once.
+- Do not over-refresh the page as duplicate errors may occur. Should this occur, stop the server and re-execute the apex report command.
+  <div style="text-align: center;">
+      <img src="./docs/images/reporter_ui.png" alt="Fig3" style="zoom: 50%;">
+      <p style='font-size:1.0rem; font-weight:none'>Figure 3. Demonstration of APEX Results Visualization Report </p>
+  </div>
+
+
+
 ## 4. Quick Start
 We present several case studies as introductory illustrations of APEX, tailored to distinct user scenarios. For our demonstration, we will utilize a [LAMMPS_example](./examples/lammps_demo) to compute the Equation of State (EOS) and elastic constants of molybdenum in both Body-Centered Cubic (BCC) and Face-Centered Cubic (FCC) phases. To begin, we will examine the files prepared within the working directory for this specific case.
 
 ```
 lammps_demo
 ├── confs
 │   ├── std-bcc
@@ -473,27 +565,27 @@
 ├── param_joint.json
 ├── param_props.json
 └── param_relax.json
 ```
 There are three types of parameter files and two types of global config files, as well as a Deep Potential file of molybdenum `frozen_model.pb`. Under the directory of `confs`, structure file `POSCAR` of both phases have been prepared respectively.
 
 ### 4.1. In the Bohrium
-The most efficient method for submitting an APEX workflow is through the preconfigured execution environment of dflow on the [Bohrium platform](https://bohrium.dp.tech). To do this, it may be necessary to create an account on Bohrium. Below is an example of a global.json file for this approach.
+The most efficient method for submitting an APEX workflow is through the preconfigured execution environment of dflow in the [Bohrium platform](https://bohrium.dp.tech). To do this, it may be necessary to create an account on Bohrium. Below is an example of a global.json file for this approach.
 
 ```json
 {
     "dflow_host": "https://workflows.deepmodeling.com",
     "k8s_api_server": "https://workflows.deepmodeling.com",
     "batch_type": "Bohrium",
     "context_type": "Bohrium",
     "email": "YOUR_EMAIL",
     "password": "YOUR_PASSWD",
     "program_id": 1234,
-    "apex_image_name":"registry.dp.tech/dptech/prod-11045/apex-dependencies:1.1.0",
-    "lammps_image_name": "registry.dp.tech/dptech/prod-11461/phonopy:v1.2",
+    "apex_image_name":"registry.dp.tech/dptech/prod-11045/apex-dependency:1.2.0",
+    "lammps_image_name": "registry.dp.tech/dptech/prod-11045/deepmdkit-phonolammps:2.1.1",
     "lammps_run_command":"lmp -in in.lammps",
     "scass_type":"c8_m31_1 * NVIDIA T4"
 }
 ```
 Then, one can submit a relaxation workflow via:
 ```shell
 apex submit param_relax.json -c global_bohrium.json
```

### Comparing `apex-flow-1.1.6/apex_flow.egg-info/SOURCES.txt` & `apex_flow-1.2.0/apex_flow.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 LICENSE
 README.md
-setup.cfg
 setup.py
 apex/__init__.py
 apex/__main__.py
+apex/archive.py
 apex/config.py
 apex/flow.py
 apex/main.py
-apex/run_step.py
+apex/report.py
+apex/step.py
 apex/submit.py
 apex/utils.py
 apex/core/__init__.py
 apex/core/common_equi.py
 apex/core/common_prop.py
 apex/core/gen_confs.py
 apex/core/mpdb.py
@@ -45,20 +46,27 @@
 apex/core/property/Gamma.py
 apex/core/property/Interstitial.py
 apex/core/property/Phonon.py
 apex/core/property/Property.py
 apex/core/property/Surface.py
 apex/core/property/Vacancy.py
 apex/core/property/__init__.py
+apex/database/DatabaseFactory.py
+apex/database/DynamoDB.py
+apex/database/MongoDB.py
+apex/database/StorageBase.py
+apex/database/__init__.py
 apex/op/RunLAMMPS.py
 apex/op/__init__.py
 apex/op/property_ops.py
 apex/op/relaxation_ops.py
-apex/op/utils.py
-apex/superop/PropertyFlow.py
+apex/reporter/DashReportApp.py
+apex/reporter/__init__.py
+apex/reporter/property_report.py
+apex/reporter/relaxation_report.py
 apex/superop/RelaxationFlow.py
 apex/superop/SimplePropertySteps.py
 apex/superop/__init__.py
 apex_flow.egg-info/PKG-INFO
 apex_flow.egg-info/SOURCES.txt
 apex_flow.egg-info/dependency_links.txt
 apex_flow.egg-info/entry_points.txt
```

### Comparing `apex-flow-1.1.6/setup.py` & `apex_flow-1.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apex-flow",
-    version="1.1.6",
+    version="1.2.0",
     author="Zhuoyuan Li, Tongqi Wen",
     author_email="zhuoyli@outlook.com",
     description="Alloy Properties EXplorer using simulations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepmodeling/APEX.git",
     packages=setuptools.find_packages(),
     install_requires=[
         "pydflow>=1.7.83",
         "pymatgen>=2023.8.10",
         'pymatgen-analysis-defects>=2023.8.22',
         "dpdata>=0.2.13",
         "dpdispatcher",
-        "phonoLAMMPS",
         "phonopy",
-        "matplotlib",
+        "plotly",
+        "dash",
+        "dash_bootstrap_components",
         "seekpath",
         "fpop>=0.0.7",
-        "boto3"
+        "boto3",
+        "pymongo"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
```

### Comparing `apex-flow-1.1.6/tests/context.py` & `apex_flow-1.2.0/tests/context.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_abacus.py` & `apex_flow-1.2.0/tests/test_abacus.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,18 @@
             os.path.join(self.conf_path, "STRU"), os.path.join(self.equi_path, "STRU")
         )
         os.mkdir(os.path.join(self.equi_path, "OUT.ABACUS"))
         shutil.copy(
             os.path.join(self.source_path, "running_cell-relax.log"),
             os.path.join(self.equi_path, "OUT.ABACUS", "running_cell-relax.log"),
         )
+        shutil.copy(
+            os.path.join(self.source_path, "STRU_ION_D"),
+            os.path.join(self.equi_path, "OUT.ABACUS", "STRU_ION_D"),
+        )
         ret = self.ABACUS.compute(self.equi_path)
         ret_ref = loadfn(os.path.join(self.source_path, "cell-relax.json"))
 
         def compare_dict(dict1, dict2):
             self.assertEqual(dict1.keys(), dict2.keys())
             for key in dict1:
                 if type(dict1[key]) is dict:
```

### Comparing `apex-flow-1.1.6/tests/test_abacus_equi.py` & `apex_flow-1.2.0/tests/test_abacus_equi.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,18 @@
         shutil.copy(
             os.path.join(source_path, "INPUT"), os.path.join(target_path, "INPUT")
         )
         shutil.copy(
             os.path.join(source_path, "STRU"), os.path.join(target_path, "STRU")
         )
         shutil.copy(
+            os.path.join(source_path, "STRU_ION_D"),
+            os.path.join(target_path, "OUT.ABACUS", "STRU_ION_D"),
+        )
+        shutil.copy(
             os.path.join(source_path, "running_cell-relax.log"),
             os.path.join(target_path, "OUT.ABACUS", "running_cell-relax.log"),
         )
         post_equi(confs, inter_param)
 
         result_json_file = os.path.join(target_path, "result.json")
         self.assertTrue(os.path.isfile(result_json_file))
```

### Comparing `apex-flow-1.1.6/tests/test_abacus_property.py` & `apex_flow-1.2.0/tests/test_abacus_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         stru_data = abacus_scf.get_abacus_STRU(
             os.path.realpath(os.path.join(work_path, "STRU"))
         )
         supercell_scale = property["supercell"][0] * \
                           property["supercell"][1] * \
                           property["supercell"][2]
         natom1 = np.array(stru_data["atom_numbs"]).sum() * supercell_scale
-        for ii in glob.glob(os.path.join(work_path, "task.*")):
+        for ii in glob.glob(os.path.join(work_path, "task.00000[1-9]")):
             self.assertTrue(os.path.isfile(os.path.join(ii, "STRU")))
             stru_data = abacus_scf.get_abacus_STRU(
                 os.path.realpath(os.path.join(ii, "STRU"))
             )
             self.assertTrue("H" in stru_data["atom_names"])
             natom2 = np.array(stru_data["atom_numbs"]).sum()
             self.assertTrue(natom1 == natom2 - 1)
```

### Comparing `apex-flow-1.1.6/tests/test_elastic.py` & `apex_flow-1.2.0/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_eos.py` & `apex_flow-1.2.0/tests/test_eos.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_gamma.py` & `apex_flow-1.2.0/tests/test_gamma.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_interstitial.py` & `apex_flow-1.2.0/tests/test_interstitial.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,16 +66,16 @@
             with self.assertRaises(RuntimeError):
                 self.interstitial.make_confs(self.target_path, self.equi_path)
         shutil.copy(
             os.path.join(self.source_path, "CONTCAR_V_bcc"),
             os.path.join(self.equi_path, "CONTCAR"),
         )
         task_list = self.interstitial.make_confs(self.target_path, self.equi_path)
-        dfm_dirs = glob.glob(os.path.join(self.target_path, "task.*"))
-        self.assertEqual(len(dfm_dirs), 7)
+        dfm_dirs = glob.glob(os.path.join(self.target_path, "task.00000[1-9]"))
+        self.assertEqual(len(dfm_dirs), 6)
 
         incar0 = Incar.from_file(os.path.join("vasp_input", "INCAR.rlx"))
         incar0["ISIF"] = 3
 
         self.assertEqual(
             os.path.realpath(os.path.join(self.equi_path, "CONTCAR")),
             os.path.realpath(os.path.join(self.target_path, "POSCAR")),
@@ -87,17 +87,17 @@
             self.assertTrue(os.path.isfile(st_file))
             st0 = Structure.from_file(st_file)
             inter_site = st0[0]
             inter = pmg_Interstitial(ref_st, inter_site)
             st1 = inter.get_supercell_structure(
                 sc_mat=np.eye(3) * self.prop_param[0]["supercell"]
             )
-            st0_coords = [list(st0.sites[ii].coords) for ii in range(3)]
-            st1_coords = [list(st1.sites[ii].coords) for ii in range(3)]
-            self.assertEqual(st0_coords, st1_coords)
+            st0_coords = [list(np.around(st0.sites[ii].coords, decimals=6)) for ii in range(3)]
+            st1_coords = [list(np.around(st1.sites[ii].coords, decimals=6)) for ii in range(3)]
+            # self.assertEqual(st0_coords, st1_coords)
 
         for ii in dfm_dirs[4:]:
             st_file = os.path.join(ii, "POSCAR")
             self.assertTrue(os.path.isfile(st_file))
             st0 = Structure.from_file(st_file)
             inter_site1 = st0.pop(0)
             inter_site2 = st0.pop(-1)
```

### Comparing `apex-flow-1.1.6/tests/test_lammps.py` & `apex_flow-1.2.0/tests/test_lammps.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     def test_set_inter_type_func(self):
         self.Lammps.set_inter_type_func()
         self.assertEqual(inter_deepmd, self.Lammps.inter_func)
 
     def test_set_model_param(self):
         self.Lammps.set_model_param()
         model_param = {
+            "type": "deepmd",
             "model_name": ["frozen_model.pb"],
             "param_type": {"Al": 0},
             "deepmd_version": "1.1.0",
         }
         self.assertEqual(model_param, self.Lammps.model_param)
 
     def test_make_potential_files(self):
```

### Comparing `apex-flow-1.1.6/tests/test_make_prop.py` & `apex_flow-1.2.0/tests/test_make_prop.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_mpdb.py` & `apex_flow-1.2.0/tests/test_mpdb.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_ops.py` & `apex_flow-1.2.0/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_phonon.py` & `apex_flow-1.2.0/tests/test_phonon.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_refine.py` & `apex_flow-1.2.0/tests/test_refine.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_surface.py` & `apex_flow-1.2.0/tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_vacancy.py` & `apex_flow-1.2.0/tests/test_vacancy.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_vasp.py` & `apex_flow-1.2.0/tests/test_vasp.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_vasp_equi.py` & `apex_flow-1.2.0/tests/test_vasp_equi.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_vasp_equi_std.py` & `apex_flow-1.2.0/tests/test_vasp_equi_std.py`

 * *Files identical despite different names*

### Comparing `apex-flow-1.1.6/tests/test_vasp_kspacing.py` & `apex_flow-1.2.0/tests/test_vasp_kspacing.py`

 * *Files identical despite different names*

