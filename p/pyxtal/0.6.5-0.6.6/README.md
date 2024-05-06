# Comparing `tmp/pyxtal-0.6.5.tar.gz` & `tmp/pyxtal-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxtal-0.6.5.tar", last modified: Sun Apr 21 00:39:52 2024, max compression
+gzip compressed data, was "pyxtal-0.6.6.tar", last modified: Mon May  6 01:06:30 2024, max compression
```

## Comparing `pyxtal-0.6.5.tar` & `pyxtal-0.6.6.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.881802 pyxtal-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-21 00:39:37.000000 pyxtal-0.6.5/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-04-21 00:39:37.000000 pyxtal-0.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-21 00:39:52.881802 pyxtal-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-21 00:39:37.000000 pyxtal-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.845802 pyxtal-0.6.5/pyxtal/
--rw-r--r--   0 runner    (1001) docker     (127)    31243 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/XRD.py
--rw-r--r--   0 runner    (1001) docker     (127)   114634 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/block_crystal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/crystal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.865802 pyxtal-0.6.5/pyxtal/database/
--rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/HM_Full.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/atomic_scattering_params.json
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/bonds.json
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/bug.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.873802 pyxtal-0.6.5/pyxtal/database/cifs/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/0-G62.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/1-G59.cif
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/191.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/2-G71.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/3-G139.cif
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/4-G225.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/ACBNZA01.cif
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/AXOSOW01.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/BTO-Amm2.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/BTO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/FAU.cif
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Fd3.cif
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Fd3.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Fd3m.cif
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/GUMMUW.cif
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/GeF2.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/HAHCOI.cif
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/I41amd.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/I4_132.cif
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/JAPWIH.cif
--rw-r--r--   0 runner    (1001) docker     (127)   441469 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/LAGNAL.cif
--rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/LUFHAW.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/LiCs.cif
--rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/MERQIM.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/MPWO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/NaCl.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/NaSb3F10.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/NbO2.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/NiS-Cm.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/P3_112.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/P4_332.cif
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/P4nmm.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/P6_422.cif
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/PAHYON01.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/PPO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/PVO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Pm3.cif
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Pmmn.vasp
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Pn3.vasp
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/Pn3m.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/R-3.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/R-3c.cif
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/R32.cif
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/TMPPIO03.cif
--rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/WEXBOS.cif
--rw-r--r--   0 runner    (1001) docker     (127)   177150 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/YICMOP.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/anthracene.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/aspirin-c.cif
--rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/aspirin.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/benzene.cif
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/bug.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/c_bug.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/c_bug2.vasp
--rw-r--r--   0 runner    (1001) docker     (127)    17895 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/coumarin.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/dist_6_0.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/dist_6_1.cif
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/gdh.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/ht_KNbBO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/ht_cristobalite.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/ht_quartz.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/ice.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/lt_KNbBO.cif
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/lt_cristobalite.cif
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/lt_quartz.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/naphthalene.cif
--rw-r--r--   0 runner    (1001) docker     (127)   317844 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/resorcinol.cif
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/sim-0.vasp
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/sim-1.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/cifs/xxvi.cif
--rw-r--r--   0 runner    (1001) docker     (127)  1103778 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/clusters.json
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/element.py
--rw-r--r--   0 runner    (1001) docker     (127) 10480157 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/k_subgroup.json
--rw-r--r--   0 runner    (1001) docker     (127)    20717 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/layer.csv
--rw-r--r--   0 runner    (1001) docker     (127)    25842 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/layer_generators.csv
--rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/layer_symmetry.csv
--rw-r--r--   0 runner    (1001) docker     (127)   294912 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/mech.db
--rw-r--r--   0 runner    (1001) docker     (127)    90734 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/molecules.json
--rw-r--r--   0 runner    (1001) docker     (127)   130892 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/point.csv
--rw-r--r--   0 runner    (1001) docker     (127)   146327 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/point_generators.csv
--rw-r--r--   0 runner    (1001) docker     (127)   301944 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/point_symmetry.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18501 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/rod.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21935 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/rod_generators.csv
--rw-r--r--   0 runner    (1001) docker     (127)    44320 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/rod_symmetry.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/symbols.json
--rw-r--r--   0 runner    (1001) docker     (127)  1245398 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/t_subgroup.json
--rw-r--r--   0 runner    (1001) docker     (127)   259897 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/wyckoff_generators.csv
--rw-r--r--   0 runner    (1001) docker     (127)   251719 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/wyckoff_list.csv
--rw-r--r--   0 runner    (1001) docker     (127)   117892 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/wyckoff_sets.json
--rw-r--r--   0 runner    (1001) docker     (127)   627207 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/database/wyckoff_symmetry.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    18755 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    42644 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/elasticity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.877802 pyxtal-0.6.5/pyxtal/interface/
--rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/LJ.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27559 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/dftb.py
--rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/gulp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19373 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/lammpslib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/interface/vasprun.py
--rw-r--r--   0 runner    (1001) docker     (127)    23019 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    70535 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)    18102 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/molecular_crystal.py
--rw-r--r--   0 runner    (1001) docker     (127)    66288 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/msg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30343 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.877802 pyxtal-0.6.5/pyxtal/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/optimize/fire.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/optimize/fire2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/optimize/myscipy_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/plane.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.877802 pyxtal-0.6.5/pyxtal/potentials/
--rw-r--r--   0 runner    (1001) docker     (127)  1820580 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/potentials/CuAg.eam.alloy
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/potentials/LJ_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/potentials/Si.tersoff
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/potentials/SiCGe.tersoff
--rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/potentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/representation.py
--rw-r--r--   0 runner    (1001) docker     (127)    46126 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/supergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)   139385 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    46203 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/tolerance.py
--rw-r--r--   0 runner    (1001) docker     (127)    19437 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/viz.py
--rw-r--r--   0 runner    (1001) docker     (127)    45507 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/wyckoff_site.py
--rw-r--r--   0 runner    (1001) docker     (127)    21159 2024-04-21 00:39:37.000000 pyxtal-0.6.5/pyxtal/wyckoff_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.881802 pyxtal-0.6.5/pyxtal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-21 00:39:52.000000 pyxtal-0.6.5/pyxtal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-21 00:39:52.000000 pyxtal-0.6.5/pyxtal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 00:39:52.000000 pyxtal-0.6.5/pyxtal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-21 00:39:52.000000 pyxtal-0.6.5/pyxtal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 00:39:52.000000 pyxtal-0.6.5/pyxtal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:39:52.877802 pyxtal-0.6.5/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4251 2024-04-21 00:39:37.000000 pyxtal-0.6.5/scripts/pyxtal_main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-04-21 00:39:37.000000 pyxtal-0.6.5/scripts/pyxtal_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-21 00:39:52.881802 pyxtal-0.6.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1850 2024-04-21 00:39:37.000000 pyxtal-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.549897 pyxtal-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 01:06:26.000000 pyxtal-0.6.6/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-06 01:06:26.000000 pyxtal-0.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-06 01:06:30.549897 pyxtal-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-06 01:06:26.000000 pyxtal-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.513897 pyxtal-0.6.6/pyxtal/
+-rw-r--r--   0 runner    (1001) docker     (127)    31243 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/XRD.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126538 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/block_crystal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/crystal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.533897 pyxtal-0.6.6/pyxtal/database/
+-rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/HM_Full.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/atomic_scattering_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/bug.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.541897 pyxtal-0.6.6/pyxtal/database/cifs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/0-G62.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/1-G59.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/191.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/2-G71.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/3-G139.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/4-G225.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/ACBNZA01.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/AXOSOW01.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/BTO-Amm2.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/BTO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/FAU.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Fd3.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Fd3.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Fd3m.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/GUMMUW.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/GeF2.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/HAHCOI.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/I41amd.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/I4_132.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/JAPWIH.cif
+-rw-r--r--   0 runner    (1001) docker     (127)   441469 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/LAGNAL.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/LUFHAW.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/LiCs.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/MERQIM.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/MPWO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/NaCl.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/NaSb3F10.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/NbO2.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/NiS-Cm.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/P3_112.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/P4_332.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/P4nmm.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/P6_422.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/PAHYON01.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/PPO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/PVO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Pm3.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Pmmn.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Pn3.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Pn3m.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/R-3.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/R-3c.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/R32.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/TMPPIO03.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/WEXBOS.cif
+-rw-r--r--   0 runner    (1001) docker     (127)   177150 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/YICMOP.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/anthracene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/aspirin-c.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/aspirin.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/benzene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/bug.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/c_bug.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/c_bug2.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)    17895 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/coumarin.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/dist_6_0.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/dist_6_1.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/gdh.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/ht_KNbBO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/ht_cristobalite.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/ht_quartz.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/ice.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/lt_KNbBO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/lt_cristobalite.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/lt_quartz.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/naphthalene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)   317844 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/resorcinol.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/sim-0.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/sim-1.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/xxvi.cif
+-rw-r--r--   0 runner    (1001) docker     (127)  1103778 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/clusters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)  9679835 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/k_subgroup.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20717 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/layer.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    25842 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/layer_generators.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/layer_symmetry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   294912 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/mech.db
+-rw-r--r--   0 runner    (1001) docker     (127)    90734 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/molecules.json
+-rw-r--r--   0 runner    (1001) docker     (127)   130892 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/point.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   146327 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/point_generators.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   301944 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/point_symmetry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18501 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/rod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21935 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/rod_generators.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    44320 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/rod_symmetry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/symbols.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1245398 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/t_subgroup.json
+-rw-r--r--   0 runner    (1001) docker     (127)   259897 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/wyckoff_generators.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   251719 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/wyckoff_list.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   117892 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/wyckoff_sets.json
+-rw-r--r--   0 runner    (1001) docker     (127)   627207 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/wyckoff_symmetry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18755 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42644 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/elasticity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.545897 pyxtal-0.6.6/pyxtal/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/LJ.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27559 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/dftb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/gulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19373 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/lammpslib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/vasprun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23018 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71828 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18102 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/molecular_crystal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66288 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36170 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.545897 pyxtal-0.6.6/pyxtal/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/optimize/fire.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/optimize/fire2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/optimize/myscipy_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/plane.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.545897 pyxtal-0.6.6/pyxtal/potentials/
+-rw-r--r--   0 runner    (1001) docker     (127)  1820580 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/potentials/CuAg.eam.alloy
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/potentials/LJ_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/potentials/Si.tersoff
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/potentials/SiCGe.tersoff
+-rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/potentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18145 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46115 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)   144617 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48128 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/tolerance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45527 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/wyckoff_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21753 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/wyckoff_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.549897 pyxtal-0.6.6/pyxtal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-06 01:06:30.000000 pyxtal-0.6.6/pyxtal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-06 01:06:30.000000 pyxtal-0.6.6/pyxtal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 01:06:30.000000 pyxtal-0.6.6/pyxtal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 01:06:30.000000 pyxtal-0.6.6/pyxtal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 01:06:30.000000 pyxtal-0.6.6/pyxtal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.545897 pyxtal-0.6.6/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4251 2024-05-06 01:06:26.000000 pyxtal-0.6.6/scripts/pyxtal_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-05-06 01:06:26.000000 pyxtal-0.6.6/scripts/pyxtal_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 01:06:30.549897 pyxtal-0.6.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1802 2024-05-06 01:06:26.000000 pyxtal-0.6.6/setup.py
```

### Comparing `pyxtal-0.6.5/LICENSE.txt` & `pyxtal-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/PKG-INFO` & `pyxtal-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <=3.12
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: spglib>=1.10.4
 Requires-Dist: pymatgen>=2024.3.1
 Requires-Dist: pandas>=2.0.2
 Requires-Dist: networkx>=2.3
 Requires-Dist: ase>=3.18.0
```

### Comparing `pyxtal-0.6.5/README.md` & `pyxtal-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/XRD.py` & `pyxtal-0.6.6/pyxtal/XRD.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/__init__.py` & `pyxtal-0.6.6/pyxtal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -493,14 +493,27 @@
             #import pymatgen.analysis.structure_matcher as sm
             #self.dim = 3
             #self.PBC = [1, 1, 1]
             #pmg1 = self.to_pymatgen()
             #if not sm.StructureMatcher().fit(struc, pmg1):
             #    raise RuntimeError("The structure is inconsistent after conversion")
 
+    def are_valid_numIons(self):
+        """
+        Check if the numIons are correct for debugging
+        """
+
+        N = [s.wp.multiplicity for s in self.atom_sites]
+        #for s in self.atom_sites: print(s.wp.multiplicity, s.wp.get_label())
+        if sum(N) != sum(self.numIons):
+            print("Inconsistent numIons", sum(N), self.numIons)
+            return False
+        else:
+            return True
+
     def check_H_coordination(self, r=1.12):
         """
         A function to check short if H is connected to more than one atom
         Mainly used for debug, powered by pymatgen
 
         Args:
             r: the given cutoff distances
@@ -655,28 +668,29 @@
         Generate a structure with lower symmetry
 
         Args:
             perms: e.g., {"Si": "C"}
             H: space group number (int)
             eps: pertubation term (float)
             idx: list
-            group_type: `t`, `k` or `t+k`
-            max_cell: maximum cell reconstruction (float)
+            group_type (string): `t`, `k` or `t+k`
+            max_cell (float): maximum cell reconstruction
+            min_cell (float): maximum cell reconstruction
 
         Returns:
             a list of pyxtal structures with lower symmetries
         """
 
         #randomly choose a subgroup from the available list
         idx, sites, t_types, k_types = self._get_subgroup_ids(H, group_type, idx, max_cell, min_cell)
 
         valid_splitters = []
         bad_splitters = []
         for id in idx:
-            gtype = (t_types+k_types)[id]
+            gtype = (t_types + k_types)[id]
             if gtype == 'k':
                 id -= len(t_types)
             splitter = wyckoff_split(G=self.group, wp1=sites, idx=id, group_type=gtype)
 
             if not splitter.error:
                 if perms is None:
                     if splitter.valid_split:
@@ -716,14 +730,15 @@
             new_strucs = []
             for splitter in valid_splitters:
                 #print(splitter)
                 if perms is None:
                     new_struc = self._subgroup_by_splitter(splitter, eps=eps)
                 else:
                     new_struc = self._apply_substitution(splitter, perms)
+                #if not new_struc.are_valid_numIons(): print(new_struc); import sys; sys.exit()
                 new_strucs.append(new_struc)
             return new_strucs
 
     def subgroup_by_path(self, gtypes, ids, eps=0, mut_lat=False):
         """
         Generate a structure with lower symmetry (for atomic crystals only)
 
@@ -767,14 +782,22 @@
             group_type: `t` or `k`
             max_cell: maximum cell reconstruction (float)
 
         Returns:
             a pyxtal structure with lower symmetries
         """
         idx, sites, t_types, k_types = self._get_subgroup_ids(H, group_type, None, max_cell, min_cell)
+        #print("Test subgroup_once", self.group.number, idx, sites)
+
+        if idx is None or len(idx) == 0:
+            msg = "Cannot find the valid splitter id\n"
+            msg += "This is most likely due to the cell size is not sufficient for k-subgroup\n"
+            msg += "You may increase the max_cell"
+            print(msg)
+            return None
 
         # Try 100 times to see if a valid split can be found
         count = 0
         while count < 100:
             id = choice(idx)
             gtype = (t_types+k_types)[id]
             if gtype == 'k':
@@ -818,15 +841,17 @@
                         if trail_struc is not None:
                             multiple = sum(trail_struc.numIons)/sum(self.numIons)
                             max_cell = max([1, max_cell/multiple])
                             ans = trail_struc.subgroup_once(eps, H, None, group_type, max_cell)
                             if ans.group.number > 1:
                                 return ans
             count += 1
-        raise RuntimeError("Cannot find the splitter")
+
+        print("Cannot find the splitter")
+        return None
 
     def _apply_substitution(self, splitter, perms):
         """
         Apply the substitution
         """
         try:
             new_struc = self._subgroup_by_splitter(splitter)
@@ -882,15 +907,15 @@
                 dicts[key].extend(dict2[key])
 
         Hs = dicts['subgroup']
         trans = dicts['transformation']
 
         if idx is None:
             idx = []
-            if not self.molecular or self.group.number>142:
+            if not self.molecular or self.group.number > 142:
                 for i, tran in enumerate(trans):
                     if min_cell<=np.linalg.det(tran[:3,:3])<=max_cell:
                         idx.append(i)
             else:
                 # for molecular crystals, assume the cell does not change
                 for i, tran in enumerate(trans):
                     tran = np.abs(tran[:3,:3])
@@ -906,16 +931,16 @@
             for id in idx:
                 if id >= len(Hs):
                     raise ValueError("The idx exceeds the number of possible splits")
 
         if H is not None:
             idx = [id for id in idx if Hs[id] == H]
 
-        if len(idx) == 0:
-            raise RuntimeError("Cannot find the splitter")
+        #if len(idx) == 0:
+        #    raise RuntimeError("Cannot find the splitter")
 
         if self.molecular:
             struc_sites = self.mol_sites
         else:
             struc_sites = self.atom_sites
 
         sites = [site.wp.get_label() for site in struc_sites]
@@ -1004,30 +1029,30 @@
                     pos0 += eps*dis*(np.random.random()-0.5)
                     wp = Wyckoff_position.from_symops(ops2, h)
                     _site = mol_site(_mol, pos0, ori, wp, lattice)
                     _site.type = site.type
                     split_sites.append(_site)
                     id += wp.multiplicity
             new_struc.mol_sites = split_sites
-            new_struc.numMols = [int(multiples*numMol) for numMol in self.numMols]
+            new_struc.numMols = [int(round(multiples*numMol)) for numMol in self.numMols]
 
         else:
             for i, site in enumerate(self.atom_sites):
                 pos = site.position
                 for ops1, ops2 in zip(splitter.G2_orbits[i], splitter.H_orbits[i]):
                     pos0 = apply_ops(pos, ops1)[0]
                     pos0 -= np.floor(pos0)
                     dis = (np.random.sample(3) - 0.5).dot(self.lattice.matrix)
                     dis /= np.linalg.norm(dis)
                     pos0 += np.dot(eps*dis*(np.random.random()-0.5), self.lattice.inv_matrix)
                     wp = Wyckoff_position.from_symops(ops2, h)
                     split_sites.append(atom_site(wp, pos0, site.specie))
 
             new_struc.atom_sites = split_sites
-            new_struc.numIons = [int(multiples*numIon) for numIon in self.numIons]
+            new_struc.numIons = [int(round(multiples*numIon)) for numIon in self.numIons]
         new_struc.lattice = lattice
         new_struc.source = 'subgroup'
 
         return new_struc
 
     def apply_perturbation(self, d_lat=0.05, d_coor=0.05, d_rot=1):
         """
@@ -1312,22 +1337,22 @@
     def get_std_representation(self, trans):
         """
         Perform cell transformation so that the symmetry operations
         follow standard space group notation
         """
         pass
 
-    def get_1D_representation(self):
+    def get_1D_representation(self, standard=False):
         """
         Get the 1D representation class for molecular crystals
         """
         if self.molecular:
             rep = representation.from_pyxtal(self)
         else:
-            rep = representation_atom.from_pyxtal(self)
+            rep = representation_atom.from_pyxtal(self, standard=standard)
         return rep
 
     def transform(self, trans, lattice=None):
         """
         Perform cell transformation and symmetry operation
 
         Args:
@@ -1536,16 +1561,21 @@
                 elif len(wp) == 4: # tuple:
                     (key, x, y, z) = wp
                     _wp = choose_wyckoff(self.group, site=key)
                     if _wp is not False:
                         if _wp.get_dof() == 0: #fixed pos
                             pt = [0.0, 0.0, 0.0]
                         else:
-                            pt = _wp.get_all_positions([x, y, z])[0]
-                        _sites.append(atom_site(_wp, pt, sp))
+                            ans = _wp.get_all_positions([x, y, z])
+                            if ans is not None:
+                                pt = ans[0]
+                            else:
+                                pt = None
+                        if pt is not None:
+                            _sites.append(atom_site(_wp, pt, sp))
                     else:
                         raise RuntimeError("Cannot interpret site", key)
                 else: # List of atomic coordinates
                     pt, _wp, _ = wp0.merge(wp, lattice.matrix, tol=tol)
                     _sites.append(atom_site(_wp, pt, sp))
 
         self.atom_sites = _sites
@@ -2040,15 +2070,15 @@
 
         # remove close translations
         good_translations = []
         for trans in translations:
             match = False
             for trans_ref in good_translations:
                 diff = trans - trans_ref
-                diff -= np.round(diff)
+                diff -= np.rint(diff)
                 diff = np.dot(diff, self.lattice.matrix)
                 if np.linalg.norm(diff) < tol:
                     match = True
                     break
             if not match:
                 good_translations.append(trans)
         self.axis = axis
@@ -3094,7 +3124,312 @@
                 print("\n Write charmm.rtf and charmm.prm ......")
                 ase_with_ff.write_charmmfiles()
                 #ase_with_ff.write_charmmfiles_by_parmd()
 
             return ase_with_ff
         else:
             raise NotImplementedError("\nNo support for atomic crystals")
+
+    def update_from_1d_rep(self, x):
+        """
+        update the xtal from the 1d representation
+        Group: I 41/a m d:2 (141)
+        2.5019,   2.5019,   8.7534,  90.0000,  90.0000,  90.0000, tetragonal
+        Wyckoff sites:
+        C @ [ 0.0000  0.2500  0.4614], WP [8e] Site [2mm.]
+
+        the above rep is [2.5019, 8.7514, 0.4614]
+
+        Args:
+            x (float): input variable array to describe a xtal
+        """
+        N = self.lattice.dof
+        cell, pos = x[:N], x[N:]
+
+        # update cell
+        l_type = self.lattice.ltype
+        self.lattice = Lattice.from_1d_representation(cell, l_type)
+        #print("lattice dof", N, cell, l_type, self.lattice)
+
+        # update position
+        start = 0
+        for site in self.atom_sites:
+            end = start + site.wp.get_dof()
+            xyz = site.wp.get_position_from_free_xyzs(pos[start:end])
+            site.update(xyz)
+            start = end
+        #xtal.to_ase().write('init.vasp', vasp5=True, format='vasp', direct=True)
+
+    def get_1d_rep_x(self):
+        """
+        Get a simplified x representation for a crystal
+        Group: I 41/a m d:2 (141)
+        2.5019,   2.5019,   8.7534,  90.0000,  90.0000,  90.0000, tetragonal
+        Wyckoff sites:
+        C @ [ 0.0000  0.2500  0.4614], WP [8e] Site [2mm.]
+
+        The above rep is [2.5019, 8.7514, 0.4614]
+        """
+
+        rep = self.get_1D_representation(standard=True)
+        cell, xyzs = rep.x[0][1:], rep.x[1:]
+        x = cell
+        for xyz in xyzs:
+            x = np.hstack((x, xyz[2:]))
+
+        return x
+
+    def from_spg_wps_rep(self, spg, wps, x, elements=None):
+        """
+        An advanced way to build pyxtal from wyckoff position
+        and compacted 1d x representation
+
+        Args:
+            spg (int): space group number 1-230
+            wps (list): wyckoff representation (e.g., ['6a', '6a'])
+            x (array): 1d representation
+            elements (list): list of element string
+        """
+        if elements is None: elements = ['C'] * len(wps)
+        group = Group(spg)
+        sites = []
+        for i, _wp in enumerate(wps):
+            letter = _wp[-1]
+            for wp in group:
+                if wp.letter == letter:
+                    sites.append((elements[i], wp))
+                    break
+        self.from_1d_rep(x, sites)
+
+    def from_1d_rep(self, x, sites):
+        """
+        An advanced way to build pyxtal from the 1d representation
+
+        Args:
+            x: 1d representation
+            sites: list of (element, wp)
+        """
+        l_type = sites[0][1].lattice_type
+        N = sum(Lattice.get_dofs(l_type))
+        cell, pos = x[:N], x[N:]
+        lat = Lattice.from_1d_representation(cell, l_type)
+
+        species, numIons = [], []
+        total_sites = []
+
+        start = 0
+        for site in sites:
+            (specie, _wp) = site
+            end = start + _wp.get_dof()
+            xyz = pos[start:end]
+            full_xyz = _wp.get_position_from_free_xyzs(xyz)
+            [x, y, z] = full_xyz
+            start = end
+            label = _wp.get_label()
+            if specie not in species:
+                species.append(specie)
+                numIons.append(_wp.multiplicity)
+                total_sites.append([(label, x, y, z)])
+            else:
+                idx = species.index(specie)
+                numIons[idx] += _wp.multiplicity
+                total_sites[idx].append((label, x, y, z))
+        #print(species, numIons,  total_sites)
+
+        spg = sites[0][1].number
+        try:
+            self.build(spg, species, numIons, lat, total_sites)
+        except:
+            print("input x", x)
+            print("input build", spg, numIons, lat, total_sites)
+            raise ValueError('Problem in build')
+
+
+    def check_validity(self, criteria, verbose=False):
+        """
+        Check if the xtal is valid for a given list of criteria.
+        Currently support the following keywords
+        - MIN_Density (float)
+        - CN: coordination number (int)
+        - Dimension: (int)
+
+        Args:
+            criteria (dict): keywords and the threshhold values
+            verbose (bool): whether or not print out details
+
+        Return:
+            bool value regarding the validity
+        """
+
+        if len(criteria.keys()) == 0:
+            return True
+
+        if 'exclude_ii' not in criteria:
+            criteria['exclude_ii'] = False
+
+
+        if 'MIN_Density' in criteria:
+            den1 = self.get_density()
+            den2 = criteria['MIN_Density']
+            if den1 < den2:
+                if verbose:
+                    msg = "===Invalid in MIN_density {:.2f}=>{:.2f}".format(den1, den2)
+                    print(msg)
+                return False
+
+        if 'CN' in criteria:
+            if criteria['exclude_ii']:
+                options = [True, False]
+            else:
+                options = [False]
+
+            for option in options:
+                try:
+                    self.set_site_coordination(criteria['cutoff'], exclude_ii=option)
+                except:
+                    if verbose:
+                        print("=====Invalid in CN calculation")
+                    return False
+                for s in self.atom_sites:
+                    ele = s.specie
+                    cn1 = s.coordination
+                    cn2 = criteria['CN'][ele]
+                    #print(ele, cn1, option)
+                    if cn1 != cn2:
+                        if verbose:
+                            strs = "=====Invalid CN {:s} [{:d}=>{:d}]".format(ele, cn1, cn2)
+                            strs += ", exclude ii: " + str(option)
+                            print(strs)
+                        return False
+
+        if 'Dimension' in criteria:
+            try:
+                dim1 = self.get_dimensionality(criteria_cutoff)
+            except:
+                dim1 = 3
+            dim2 = criteria['Dimension'];
+            if dim1 != dim2:
+                if verbose:
+                    print("=====Invalid in Dimension {:d}=>{:d}".format(dim1, dim2))
+                return False
+
+        return True
+
+    def get_xtal_string(self, dicts=None, header=None):
+        """
+        get the xtal string
+
+        Args:
+            xtal: pyxtal instance
+            sim (float): similarity metric
+            status (bool): whether or not the structure is valid
+            energy (float): the energy value
+        """
+        spg_num, spg_symbol = self.group.number, self.group.symbol
+        density = self.get_density()
+        dof = self.get_dof()
+        N_atoms = sum(self.numIons)
+        if header is not None:
+            strs = header
+        else:
+            strs = ""
+        strs += "*{:3d} {:3d} {:4d} {:10s} {:8.2f} ".format(
+                N_atoms, dof, spg_num, spg_symbol, density)
+
+        if dicts is not None:
+            # Similarity, energy, status
+            for key in dicts:
+                value = dicts[key]
+                if type(value) == float:
+                    strs += " {:8.3f} ".format(value)
+                elif type(value) == str:
+                    strs += " {:24s} ".format(value)
+                elif type(value) == bool:
+                    strs += " {:5s} ".format(str(value))
+
+        for s in self.atom_sites:
+            strs += "{:s} ".format(s.wp.get_label())
+        return strs
+
+
+    def get_tabular_representation(self, ids=None, normalize=True, N_wp=6, max_abc=50.0, max_angle=np.pi):
+        """
+        Convert the xtal to a 1D reprsentation organized as
+        (space_group_number, a, b, c, alpha, beta, gamma, wp1, wp2, ....)
+        each wp is represented by 4 numbers (wp_id, x, y, z)
+
+        Args:
+            ids (list): index of generators for each wp
+            normalize (bool): whether or not normalize the data to (0, 1)
+            N_wp (int): number of maximum wp sites
+            max_abc (float): maximum a, b, c length (used in normalization)
+            max_angle (float): maximum angle in radian (used in normalization)
+
+        Returns:
+            a 1D vector such as (141, 3, 3, 3, pi/2, pi/2, pi/2, wp_id, x, y, z)
+        """
+
+        if ids is None:
+            ids = [0] * len(self.atom_sites)
+        else:
+            assert(len(ids) == len(self.atom_sites))
+
+        if len(ids) > N_wp:
+            raise ValueError("Cannot handle too many atom sites", len(ids), N_wp)
+
+        N_cell, N_site = 7, N_wp * 4
+
+        # If the number of wp is less then 6, assign -1
+        rep = -np.ones(N_cell + N_site) # 7 + 6 + 18 = 31
+        rep[0] = self.group.number
+        rep[1:7] = self.lattice.get_para()
+
+        if normalize:
+            rep[0] /= 230
+            rep[1:4] /= max_abc
+            rep[4:7] /= max_angle
+
+        count = N_cell
+        for id, site in zip(ids, self.atom_sites):
+            rep[count] = site.wp.index
+            if normalize: rep[count] /= len(self.group)
+            xyz = site.coords[id] # position
+            xyz -= np.floor(xyz)
+            rep[count+1:count+4] = xyz
+            count += 4
+        return rep
+
+
+    def from_tabular_representation(self, rep, max_abc=50.0, max_angle=180):
+        """
+        Reconstruc xtal from 1d tabular_representation
+        Currently assuming the elemental composition like carbon
+
+        Args:
+            rep: 1D array
+            max_abc (float): maximum a, b, c length (used in normalization)
+            max_angle (float): maximum angle in radian (used in normalization)
+
+        """
+        number = int(np.round(rep[0] * 230))
+        if 1 <= number <= 230:
+            group = Group(number)
+            [a, b, c, alpha, beta, gamma] = rep[1:7]
+            a, b, c = a * max_abc, b * max_abc, c * max_abc
+            alpha, beta, gamma = alpha*max_angle, beta*max_angle, gamma*max_angle
+            lattice = np.array([a, b, c, alpha, beta, gamma])
+            sites_info = np.reshape(rep[7:], (int((len(rep)-7)/4), 4))
+            sites = []
+            numIons = 0
+            for site_info in sites_info:
+                [id, x, y, z] = site_info
+                if min(site_info) > -0.01:
+                    wp_id = int(np.round(len(group)*id))
+                    if wp_id >= len(group): wp_id = -1
+                    wp = group[wp_id]
+                    xyz = wp.search_generator([x, y, z])#; print(wp.get_label(), xyz)
+                    if xyz is not None:
+                        xyz, wp, _ = wp.merge(xyz, np.eye(3), 1e-3)
+                        label = wp.get_label()
+                        sites.append((label, xyz[0], xyz[1], xyz[2]))#; print(x, y, z, label, xyz[0], xyz[1], xyz[2])
+                        numIons += wp.multiplicity
+            self.build(group, ['C'], [numIons], lattice, [sites])
```

### Comparing `pyxtal-0.6.5/pyxtal/block_crystal.py` & `pyxtal-0.6.6/pyxtal/block_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/constants.py` & `pyxtal-0.6.6/pyxtal/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,14 +25,19 @@
                   "spherical", "Spherical",
                   "ellipsoidal", "Ellipsoidal",
                  ]
 single_smiles = [
                  "Cl-", "F-", "Br-", "I-", "Li+", "Na+", "Cs+", "Rb+",
                  "[Cl-]", "[F-]", "[Br-]", "[I-]", "[Li+]", "[Na+]", "[Cs+]", "Rb+",
                 ]
+hex_cell = np.array([[1, -0.5, 0], [0, np.sqrt(3) / 2, 0], [0, 0, 1]])
+all_sym_directions = [(1, 0, 0), (0, 1, 0), (0, 0, 1), (1, 1, 1),
+                      (1, -1, -1), (-1, 1, -1), (-1, -1, 1), (1, -1, 0),
+                      (1, 1, 0), (0, 1, -1), (0, 1, 1), (-1, 0, 1),
+                      (1, 0, 1), (1, -2, 0), (2, -1, 0)]
 
 logo = """#############################################################
 #             ______       _    _          _                #
 #            (_____ \     \ \  / /        | |               #
 #             _____) )   _ \ \/ / |_  ____| |               #
 #            |  ____/ | | | )  (|  _)/ _  | |               #
 #            | |    | |_| |/ /\ \ |_( (_| | |___            #
```

### Comparing `pyxtal-0.6.5/pyxtal/crystal.py` & `pyxtal-0.6.6/pyxtal/crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/HM_Full.csv` & `pyxtal-0.6.6/pyxtal/database/HM_Full.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/atomic_scattering_params.json` & `pyxtal-0.6.6/pyxtal/database/atomic_scattering_params.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/bonds.json` & `pyxtal-0.6.6/pyxtal/database/bonds.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/bug.json` & `pyxtal-0.6.6/pyxtal/database/bug.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/0-G62.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/0-G62.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/1-G59.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/1-G59.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/2-G71.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/2-G71.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/3-G139.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/3-G139.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/4-G225.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/4-G225.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/ACBNZA01.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/ACBNZA01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/AXOSOW01.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/AXOSOW01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/BTO-Amm2.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/BTO-Amm2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/BTO.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/BTO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/FAU.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/FAU.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/Fd3.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/Fd3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/Fd3.vasp` & `pyxtal-0.6.6/pyxtal/database/cifs/Fd3.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/Fd3m.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/Fd3m.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/GUMMUW.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/GUMMUW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/GeF2.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/GeF2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/HAHCOI.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/HAHCOI.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/I4_132.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/I4_132.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/JAPWIH.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/JAPWIH.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/LAGNAL.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/LAGNAL.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/LUFHAW.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/LUFHAW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/LiCs.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/LiCs.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/MERQIM.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/MERQIM.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/MPWO.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/MPWO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/NaCl.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/NaCl.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/NaSb3F10.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/NaSb3F10.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/NbO2.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/NbO2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/NiS-Cm.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/NiS-Cm.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/P3_112.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/P3_112.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/P4_332.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/P4_332.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/P6_422.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/P6_422.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/PAHYON01.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/PAHYON01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/PPO.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/PPO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/PVO.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/PVO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/Pm3.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/Pm3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/R-3.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/R-3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/R-3c.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/R-3c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/R32.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/R32.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/TMPPIO03.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/TMPPIO03.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/WEXBOS.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/WEXBOS.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/YICMOP.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/YICMOP.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/anthracene.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/anthracene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/aspirin-c.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/aspirin-c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/aspirin.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/aspirin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/benzene.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/benzene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/bug.vasp` & `pyxtal-0.6.6/pyxtal/database/cifs/bug.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/c_bug.vasp` & `pyxtal-0.6.6/pyxtal/database/cifs/c_bug.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/c_bug2.vasp` & `pyxtal-0.6.6/pyxtal/database/cifs/c_bug2.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/coumarin.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/coumarin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/dist_6_0.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/dist_6_0.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/dist_6_1.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/dist_6_1.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/gdh.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/gdh.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/ht_KNbBO.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/ht_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/ht_cristobalite.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/ht_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/ht_quartz.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/ht_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/ice.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/ice.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/lt_KNbBO.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/lt_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/lt_cristobalite.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/lt_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/lt_quartz.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/lt_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/naphthalene.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/naphthalene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/resorcinol.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/resorcinol.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/cifs/xxvi.cif` & `pyxtal-0.6.6/pyxtal/database/cifs/xxvi.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/clusters.json` & `pyxtal-0.6.6/pyxtal/database/clusters.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/collection.py` & `pyxtal-0.6.6/pyxtal/database/collection.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/element.py` & `pyxtal-0.6.6/pyxtal/database/element.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/layer.csv` & `pyxtal-0.6.6/pyxtal/database/layer.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/layer_generators.csv` & `pyxtal-0.6.6/pyxtal/database/layer_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/layer_symmetry.csv` & `pyxtal-0.6.6/pyxtal/database/layer_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/mech.db` & `pyxtal-0.6.6/pyxtal/database/mech.db`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/molecules.json` & `pyxtal-0.6.6/pyxtal/database/molecules.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/point.csv` & `pyxtal-0.6.6/pyxtal/database/point.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/point_generators.csv` & `pyxtal-0.6.6/pyxtal/database/point_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/point_symmetry.csv` & `pyxtal-0.6.6/pyxtal/database/point_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/rod.csv` & `pyxtal-0.6.6/pyxtal/database/rod.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/rod_generators.csv` & `pyxtal-0.6.6/pyxtal/database/rod_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/rod_symmetry.csv` & `pyxtal-0.6.6/pyxtal/database/rod_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/symbols.json` & `pyxtal-0.6.6/pyxtal/database/symbols.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/t_subgroup.json` & `pyxtal-0.6.6/pyxtal/database/t_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/wyckoff_generators.csv` & `pyxtal-0.6.6/pyxtal/database/wyckoff_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/wyckoff_list.csv` & `pyxtal-0.6.6/pyxtal/database/wyckoff_list.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/wyckoff_sets.json` & `pyxtal-0.6.6/pyxtal/database/wyckoff_sets.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/database/wyckoff_symmetry.csv` & `pyxtal-0.6.6/pyxtal/database/wyckoff_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/descriptor.py` & `pyxtal-0.6.6/pyxtal/descriptor.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/elasticity.py` & `pyxtal-0.6.6/pyxtal/elasticity.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/interface/LJ.py` & `pyxtal-0.6.6/pyxtal/interface/LJ.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/interface/dftb.py` & `pyxtal-0.6.6/pyxtal/interface/dftb.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/interface/gulp.py` & `pyxtal-0.6.6/pyxtal/interface/gulp.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/interface/lammpslib.py` & `pyxtal-0.6.6/pyxtal/interface/lammpslib.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/interface/vasp.py` & `pyxtal-0.6.6/pyxtal/interface/vasp.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/interface/vasprun.py` & `pyxtal-0.6.6/pyxtal/interface/vasprun.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/io.py` & `pyxtal-0.6.6/pyxtal/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
                     wps.append(self.wyc)
                     ids.append(id)
                 else: #special sites
                     for id0 in tmp_ids:
                         p0 = positions[id0]
                         p1, wp, _ = self.wyc.merge(p0, new_lat, 0.1)
                         diff = p1 - p0
-                        diff -= np.round(diff)
+                        diff -= np.rint(diff)
                         if np.abs(diff).sum() < 1e-2: #sort position by mapping
                             wps.append(wp)
                             ids.append(id0) #find the right ids
                             #print("add special", wp.index, id0)
                             break
         #print("===============================================================", self.wps)
```

### Comparing `pyxtal-0.6.5/pyxtal/lattice.py` & `pyxtal-0.6.6/pyxtal/lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,16 @@
             self.dof = 1
 
     @classmethod
     def get_dofs(self, ltype):
         """
         get the number of degree of freedom
         """
+        #if ltype is None: ltype = self.ltype
+
         if ltype in ["triclinic"]:
             dofs = [3, 3]
         elif ltype in ["monoclinic"]:
             dofs = [3, 1]
         elif ltype in ['orthorhombic']:
             dofs = [3, 0]
         elif ltype in ['tetragonal', 'hexagonal', 'trigonal']:
@@ -462,23 +464,24 @@
         elif self.ltype in ['monoclinic']:
             return [a, b, c, beta]
         else:
             return [a, b, c, alpha, beta, gamma]
 
     @classmethod
     def from_1d_representation(self, v, ltype):
+        #print('test', v, type(v), len(v), v[0])
         if ltype == 'triclinic':
             a, b, c, alpha, beta, gamma = v[0], v[1], v[2], v[3], v[4], v[5]
         elif ltype == 'monoclinic':
             a, b, c, alpha, beta, gamma = v[0], v[1], v[2], 90, v[3], 90
         elif ltype == 'orthorhombic':
             a, b, c, alpha, beta, gamma = v[0], v[1], v[2], 90, 90, 90
         elif ltype == 'tetragonal':
             a, b, c, alpha, beta, gamma = v[0], v[0], v[1], 90, 90, 90
-        elif ltype == 'hexagonal':
+        elif ltype in ['trigonal', 'hexagonal']:
             a, b, c, alpha, beta, gamma = v[0], v[0], v[1], 90, 90, 120
         else:
             a, b, c, alpha, beta, gamma = v[0], v[0], v[0], 90, 90, 90
         try:
             l = Lattice.from_para(a, b, c, alpha, beta, gamma, ltype=ltype)
             return l
         except:
@@ -908,14 +911,38 @@
         try:
             paras = [self.a, self.b, self.c, self.alpha, self.beta, self.gamma]
             matrix = para2matrix(paras)
             return True
         except:
             return False
 
+    def is_valid_lattice(self, tol=1e-3):
+        if self.ltype in ['cubic', 'Cubic']:
+            if (self.a-self.b) > tol or (self.a-self.c) > tol or \
+                (self.alpha-np.pi/2) > tol or (self.beta-np.pi/2) > tol \
+                or (self.gamma-np.pi/2) > tol:
+                return False
+        if self.ltype in ['hexagonal', 'trigonal', 'Hexagonal', 'Trigonal']:
+            if (self.a-self.b) > tol or (self.alpha-np.pi/2) > tol \
+                or (self.beta-np.pi/2) > tol or (self.gamma-2/3*np.pi) > tol:
+                return False
+        elif self.ltype in ['tetragonal', 'Tetragonal']:
+            if (self.a-self.b) > tol or (self.alpha-np.pi/2) > tol \
+                or (self.beta-np.pi/2) > tol or (self.gamma-np.pi/2) > tol:
+                return False
+        elif self.ltype in ['orthorhombic', 'Orthorhombic']:
+            if (self.alpha-np.pi/2) > tol or (self.beta-np.pi/2) > tol \
+                    or (self.gamma-np.pi/2) > tol:
+                return False
+        elif self.ltype in ['monoclinic', 'Monoclinic']:
+            if (self.alpha-np.pi/2) > tol or (self.gamma-np.pi/2) > tol:
+                return False
+
+        return True
+
     def check_mismatch(self, trans, l_type, tol=1.0, a_tol=10):
         """
         check if the lattice mismatch is big after a transformation
         This is mostly used in supergroup function
         QZ: to fix ===============
 
         Args:
```

### Comparing `pyxtal-0.6.5/pyxtal/molecular_crystal.py` & `pyxtal-0.6.6/pyxtal/molecular_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/molecule.py` & `pyxtal-0.6.6/pyxtal/molecule.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/msg.py` & `pyxtal-0.6.6/pyxtal/msg.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/operations.py` & `pyxtal-0.6.6/pyxtal/operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # External Libraries
 from pymatgen.core.operations import SymmOp
 
 # PyXtal imports
 from pyxtal.msg import printx
 from pyxtal.tolerance import Tol_matrix
-from pyxtal.constants import rad, deg, pyxtal_verbosity
+from pyxtal.constants import rad, deg, hex_cell, all_sym_directions
 
 # ------------------------------
 # Define functions
 def check_distance(
     coord1,
     coord2,
     species1,
@@ -96,16 +96,16 @@
     for i, c1 in enumerate(coordinates):
         specie1 = species[i]
         for j, c2 in enumerate(coordinates):
             if j > i:
                 specie2 = species[j]
                 diff = np.array(c2) - np.array(c1)
                 d_min = distance(diff, lattice, PBC=PBC)
-                rad = Element(specie1).covalent_radius + Element(specie2).covalent_radius
-                tol = factor * 0.5 * rad
+                radius = Element(specie1).covalent_radius + Element(specie2).covalent_radius
+                tol = factor * 0.5 * radius
                 if d_min < tol:
                     return False
     return True
 
 
 def check_images(
     coords,
@@ -326,14 +326,15 @@
     Returns:
         an array of filtered coords with the same shape as coords
     """
 
     def filter_vector_euclidean(vector):
         for i, a in enumerate(PBC):
             if a:
+                # QZ: check if this is equivalent to -= np.rint()
                 vector[i] -= np.floor(vector[i])
                 if vector[i] > 0.5:
                     vector[i] = 1 - vector[i]
         return vector
 
     return np.apply_along_axis(filter_vector_euclidean, -1, coords)
 
@@ -602,15 +603,15 @@
     v1 = op1.translation_vector
     v2 = op2.translation_vector
 
     difference = v2 - v1
 
     for i, a in enumerate(PBC):
         if a:
-            difference[i] -= np.floor(difference[i])
+            difference[i] -= np.rint(difference[i])
 
     d = np.linalg.norm(difference)
 
     if abs(d) < rtol:
         return True
     else:
         return False
@@ -631,124 +632,269 @@
 
     Note: reflections are treated as rotoinversions of order 2.
 
     Args:
         SymmOp: a pymatgen.core.structure.SymmOp object to analyze
     """
 
-    # TODO: include support for off-center operations
+    # ++++: include support for off-center operations
     # TODO: include support for shear and scaling operations
     # TODO: include support for matrix-column and axis-angle initialization
     def get_order(angle, rotoinversion=False, tol=1e-2):
         # Find the order of a rotation based on its angle
         found = False
         for n in range(1, 61):
             x = (n * angle) / (2.0 * np.pi)
-            y = x - np.round(x)
+            y = x - np.rint(x)
             if abs(y) <= tol:
                 found = True
                 break
         if found:
             # Double order of odd-rotation rotoinversions
-            #if rotoinversion:
-            #    if n % 2 == 1:
-            #        return int(n * 2)
-            #    else:
-            #        return int(n)
-            #else:
-            return int(n)
+            if rotoinversion:
+                if n % 2 == 1:
+                    return int(n * 2)
+                else:
+                    return int(n)
+            else:
+                return int(n)
         if not found:
             return "irrational"
 
-    def __init__(self, op):
+    def __init__(self, op, parse_trans=False, hexagonal=False):
+
         if type(op) == deepcopy(SymmOp):
+            # The numerical tolerance associated with op
+            # The 4x4 affine matrix of the op
+            # The 3x3 rotation (or rotoinversion) matrix
+            # The determinant of self.m
             self.op = op
-            """The original SymmOp object being analyzed"""
             self.tol = op.tol
-            """The numerical tolerance associated with self.op"""
             self.affine_matrix = op.affine_matrix
-            """The 4x4 affine matrix of the op"""
             self.m = op.rotation_matrix
-            """The 3x3 rotation (or rotoinversion) matrix, which ignores the
-            translational part of self.op"""
             self.det = np.linalg.det(self.m)
-            """The determinant of self.m"""
+            self.hexagonal = hexagonal
+
         elif (type(op) == np.ndarray) or (type(op) == np.matrix):
             if op.shape == (3, 3):
                 self.op = SymmOp.from_rotation_and_translation(op, [0, 0, 0])
                 self.m = self.op.rotation_matrix
                 self.det = np.linalg.det(op)
         else:
-            printx("Error: OperationAnalyzer requires a SymmOp or 3x3 array.", priority=1)
+            raise ValueError("Error: OperationAnalyzer requires a SymmOp or 3x3 array.")
+
+        self.symbol = None
+        self.parse_trans = parse_trans # only for space group
+
         # If rotation matrix is not orthogonal
         if not is_orthogonal(self.m):
             self.type = "general"
             self.axis, self.angle, self.order, self.rotation_order = (
                 None,
                 None,
                 None,
                 None,
             )
         # If rotation matrix is orthogonal
         else:
-            # If determinant is positive
+            # If determinant is positive, rotation
             if np.linalg.det(self.m) > 0:
                 self.inverted = False
                 rotvec = Rotation.from_matrix(self.m).as_rotvec()
                 if np.sum(rotvec.dot(rotvec)) < 1e-6:
                     self.axis = None
                     self.angle = 0
                 else:
                     self.angle = np.linalg.norm(rotvec)
                     self.axis = rotvec / self.angle
+                    if self.hexagonal:
+                        #print('convert hex', self.axis, np.dot(self.axis, hex_cell))
+                        self.axis = np.dot(self.axis, hex_cell)
+                    #parse symmetry direction
+                    if self.parse_trans and not self.parse_axis():
+                        self.axis *= -1
+                        self.angle = 2*np.pi - self.angle
+                        #print('switch angle', self.angle)
+
                 if np.isclose(self.angle, 0):
+                    # Types: 'identity', 'inversion', 'rotation', or 'rotoinversion'.
+                    # order: the number of times to get to origin
+                    # rotation_order: 2, 3, 4, 6
                     self.type = "identity"
-                    """The type of operation. Is one of 'identity', 'inversion',
-                    'rotation', or 'rotoinversion'."""
                     self.order = int(1)
-                    """The order of the operation. This is the number of times
-                    the operation must be applied consecutively to return to the
-                    identity operation. If no integer number if found, we set
-                    this to 'irrational'."""
                     self.rotation_order = int(1)
-                    """The order of the rotational (non-inversional) part of the
-                    operation. Must be used in conjunction with self.order to
-                    determine the properties of the operation."""
+                    self.symbol = '1'
                 else:
                     self.type = "rotation"
                     self.order = OperationAnalyzer.get_order(self.angle)
                     self.rotation_order = self.order
-            # If determinant is negative
+                    if self.parse_trans:
+                        self.symbol = self.parse_screw_symmetry()
+
+            # If determinant is negative, rotoinversion (including reflection)
             elif np.linalg.det(self.m) < 0:
                 self.inverted = True
                 rotvec = Rotation.from_matrix(-1 * self.m).as_rotvec()
                 if np.sum(rotvec.dot(rotvec)) < 1e-6:
                     self.axis = None
                     self.angle = 0
                 else:
                     self.angle = np.linalg.norm(rotvec)
                     self.axis = rotvec / self.angle
-
+                    if self.hexagonal:
+                        #print('convert hex', self.axis, np.dot(self.axis, hex_cell))
+                        self.axis = np.dot(self.axis, hex_cell)
                 if np.isclose(self.angle, 0):
+                    self.symbol = '-1'
                     self.type = "inversion"
                     self.order = int(2)
                     self.rotation_order = int(1)
                 else:
+                    #parse symmetry direction
+                    #if self.parse_trans and not self.parse_axis():
+                    #    self.axis *= -1
+                    #    self.angle = 2*np.pi - self.angle
+                    #    print('switch angle', self.angle)
+
                     self.axis *= -1
                     self.type = "rotoinversion"
                     self.order = OperationAnalyzer.get_order(
                         self.angle, rotoinversion=True
                     )
                     self.rotation_order = OperationAnalyzer.get_order(
                         self.angle, rotoinversion=False
                     )
+                    if self.parse_trans:
+                        self.symbol = self.parse_glide_symmetry()
             elif np.linalg.det(self.m) == 0:
                 self.type = "degenerate"
                 self.axis, self.angle = None, None
 
+    def parse_screw_symmetry(self, tol=1e-2):
+        """
+        If the point group symmetry is rotation, parse the screw vector
+
+        Returns:
+            0, 2_1, 3_1, 3_2, 4_1, 4_2, 4_3, 6_1, 6_2, 6_3, 6_4, 6_5
+        """
+        # only count the translation on the given axis
+        vec = self.translation_vector.copy()
+        if np.isclose(abs(np.dot(self.axis, np.array([1, 0, 0]))), 1):
+            vec[1] = 0
+            vec[2] = 0
+        elif np.isclose(abs(np.dot(self.axis, np.array([0, 1, 0]))), 1):
+            vec[0] = 0
+            vec[2] = 0
+        elif np.isclose(abs(np.dot(self.axis, np.array([0, 0, 1]))), 1):
+            vec[0] = 0
+            vec[1] = 0
+        else:
+            vec = 0
+        # No screw symmetry for other directios for tetragonal????
+
+        if np.linalg.norm(vec) < tol:
+            return str(self.order) # 2, 3, 4, 6
+        else:
+            trans = np.sum(vec)
+            if self.order == 2:
+                return '2_1'
+            elif self.order == 3:
+                if abs(self.angle/trans - 2*np.pi) < tol:
+                    return '3_1'
+                else:
+                    return '3_2'
+            elif self.order == 4:
+                if abs(trans) < tol: #
+                    return '4_2'
+                elif abs(self.angle/trans - 2*np.pi) < tol:
+                    return '4_1'
+                elif abs(self.angle/trans - np.pi) < tol or \
+                    abs(self.angle/trans - 3*np.pi) < tol:
+                    return '4_2'
+                elif abs(self.angle/trans - 2/3*np.pi) < tol or \
+                    abs(self.angle/trans - 6*np.pi) < tol:
+                    return '4_3'
+            elif self.order == 6:
+                if abs(trans) < tol: #
+                    return '6_3'
+                elif abs(self.angle/trans - 2*np.pi) < tol:
+                    return '6_1'
+                elif abs(self.angle/trans - np.pi) < tol or\
+                    abs(self.angle/trans - 5/2*np.pi) < tol:
+                    return '6_2'
+                elif abs(self.angle/trans - 2/3*np.pi) < tol or\
+                    abs(self.angle/trans - 10/3*np.pi) < tol:
+                    return '6_3'
+                elif abs(self.angle/trans - 1/2*np.pi) < tol or\
+                    abs(self.angle/trans - 5*np.pi) < tol:
+                    return '6_4'
+                elif abs(self.angle/trans - 2/5*np.pi) < tol or\
+                    abs(self.angle/trans - 10*np.pi) < tol:
+                    return '6_5'
+
+        print("Cannot assign symbol", self.angle, trans)
+
+
+    def parse_glide_symmetry(self, tol=1e-2):
+        """
+        If the point group symmetry is rotation, parse the screw vector
+        Returns:
+            m, a, b, c, n, d
+        """
+        if self.rotation_order > 2:
+            return '-'+str(self.rotation_order)
+        elif abs(self.angle - np.pi) > tol:
+            return 'm' # just indicate
+        else:
+            vec = self.translation_vector.copy()
+            if np.isclose(abs(np.dot(self.axis, np.array([1, 0, 0]))), 1):
+                vec[0] = 0
+            elif np.isclose(abs(np.dot(self.axis, np.array([0, 1, 0]))), 1):
+                vec[1] = 0
+            elif np.isclose(abs(np.dot(self.axis, np.array([0, 0, 1]))), 1):
+                vec[2] = 0
+
+            if np.linalg.norm(vec) < tol:
+                return 'm'
+            else:
+                if np.linalg.norm(vec - np.array([1/2, 0, 0])) < tol:
+                    return 'a'
+                elif np.linalg.norm(vec - np.array([0, 1/2, 0])) < tol:
+                    return 'b'
+                elif np.linalg.norm(vec - np.array([0, 0, 1/2])) < tol:
+                    return 'c'
+                elif np.linalg.norm(vec - np.array([0, 1/2, 1/2])) < tol or\
+                    np.linalg.norm(vec - np.array([1/2, 0, 1/2])) < tol or\
+                    np.linalg.norm(vec - np.array([1/2, 1/2, 0])) < tol:
+                    return 'n'
+                elif np.linalg.norm(vec - np.array([1/2, 1/2, 1/2])) < tol:
+                    if np.isclose(abs(np.dot(self.axis, np.array([0, -0.7071, 0.7071]))), 1) or\
+                       np.isclose(abs(np.dot(self.axis, np.array([-0.7071, 0, 0.7071]))), 1):
+                        return 'n'
+                    else:
+                        return 'c'
+                else:
+                    return 'd'
+
+
+    def parse_axis(self):
+        """
+        parse if the axis follows the standard convention
+        """
+        ax = self.axis
+        ax /= np.linalg.norm(ax)
+        for direction in all_sym_directions:
+            direction /= np.linalg.norm(direction)
+            #print(direction, np.dot(direction, ax))
+            if np.isclose(np.dot(direction, ax), 1):
+                return True
+            elif np.isclose(np.dot(direction, ax), -1):
+                return False
+        raise ValueError("Cannot find the symmetry direction", ax)
+
     def __str__(self):
         """
         A custom printing string for the object. The type, order, angle, and
         axis are printed. Converts values close to 0 to 0 for readability. Also
         only prints the real part of the axis.
         """
         # Avoid printing '-0.' instead of '0.'
@@ -820,23 +966,25 @@
         Returns:
             True if op2 is conjugate to op1, and False otherwise
         """
         if type(op1) != OperationAnalyzer:
             opa1 = OperationAnalyzer(op1)
         return opa1.is_conjugate(op2)
 
+
+
 def find_ids(coords, ref, tol=1e-3):
     """
     find the refernce ids that can match
     """
     ids = []
     #print('ref', ref)
     for coord in coords:
         diffs = ref - coord
-        diffs -= np.round(diffs)
+        diffs -= np.rint(diffs)
         norms = np.linalg.norm(diffs, axis=1)
         #print(norms, diffs)
         for i, norm in enumerate(norms):
             if norm < tol and i not in ids:
                 ids.append(i)
                 break
     return ids
@@ -852,15 +1000,15 @@
         cell: cell matrix 3*3 array
 
     Returns:
         position: matched position
         id: matched id
     """
     diffs = positions - ref
-    diffs -= np.round(diffs)
+    diffs -= np.rint(diffs)
     diffs = np.dot(diffs, cell)
     dists = np.linalg.norm(diffs, axis=1)
     id = np.argmin(dists)
     return positions[id], dists[id]
```

### Comparing `pyxtal-0.6.5/pyxtal/optimize/fire.py` & `pyxtal-0.6.6/pyxtal/optimize/fire.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/optimize/fire2.py` & `pyxtal-0.6.6/pyxtal/optimize/fire2.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/optimize/myscipy_optimize.py` & `pyxtal-0.6.6/pyxtal/optimize/myscipy_optimize.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/plane.py` & `pyxtal-0.6.6/pyxtal/plane.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
                     center, lower, upper = center-1, lower-1, upper-1
                     new = False
                 elif lower - 1 >= group[1] and upper -1 <= group[2]:
                     center, lower, upper = center-1, lower-1, upper-1
                     new = False
                 else:
                     dist = center - group[0]
-                    shift = np.round(dist)
+                    shift = np.rint(dist)
                     if abs(dist-shift) < tol:
                         new = False
                         lower -= shift
                         upper -= shift
 
                 if not new:
                     # Update group
```

### Comparing `pyxtal-0.6.5/pyxtal/potentials/CuAg.eam.alloy` & `pyxtal-0.6.6/pyxtal/potentials/CuAg.eam.alloy`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/potentials/LJ_cluster.py` & `pyxtal-0.6.6/pyxtal/potentials/LJ_cluster.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/potentials/Si.tersoff` & `pyxtal-0.6.6/pyxtal/potentials/Si.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/potentials/SiCGe.tersoff` & `pyxtal-0.6.6/pyxtal/potentials/SiCGe.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/representation.py` & `pyxtal-0.6.6/pyxtal/representation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def __init__(self, x):
         self.x = x
 
     def __str__(self):
         return self.to_string()
 
     @classmethod
-    def from_pyxtal(cls, struc, standard=False):
+    def from_pyxtal(cls, struc, standard=True):
         """
         Initialize 1D rep. from the pyxtal object
 
         Args:
             struc: pyxtal object
         """
         if standard and not struc.standard_setting:
@@ -455,24 +455,24 @@
                     diff_cell = tmp2 - tmp1
                     diffs.extend(diff_cell)
                 # site difference
                 else:
                     # symmmetry variation
                     xyzs = wp.apply_ops(tmp2[:3])
                     diff_xyzs = xyzs - tmp1[:3]
-                    diff_xyzs -= np.round(diff_xyzs)
+                    diff_xyzs -= np.rint(diff_xyzs)
                     id = np.argmin(np.linalg.norm(diff_xyzs, axis=1))
                     diff_xyz = diff_xyzs[id]
                     diff_ori = tmp2[3:6] - tmp1[3:6]
                     diff_ori /= [360.0, 180.0, 360.0]
-                    diff_ori -= np.round(diff_ori)
+                    diff_ori -= np.rint(diff_ori)
                     diff_ori *= [360.0, 180.0, 360.0]
                     diff_tor = tmp2[6:] - tmp1[6:]
                     diff_tor /= 360.0
-                    diff_tor -= np.round(diff_tor)
+                    diff_tor -= np.rint(diff_tor)
                     diff_tor *= 360.0
                     diffs.extend(diff_xyz)
                     diffs.extend(diff_ori)
                     diffs.extend(diff_tor)
             return np.array(diffs)
 
 if __name__ == "__main__":
```

### Comparing `pyxtal-0.6.5/pyxtal/supergroup.py` & `pyxtal-0.6.6/pyxtal/supergroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,25 +183,25 @@
     diffs = []
     coords = []
     # loop over all nearby translations
     for shift in shifts:
         res = np.dot(rot, pos + shift) + tran.T
         tmp = sym.search_cloest_wp(G, wp1, op, res)
         diff = res - tmp
-        diff -= np.round(diff)
+        diff -= np.rint(diff)
         dist = np.linalg.norm(diff)
         diffs.append(dist)
         coords.append(tmp)
         if dist < 1e-1:
             break
     # choose the one returns minimum difference
     diffs = np.array(diffs)
     minID = np.argmin(diffs)
     tmp = coords[minID]
-    tmp -= np.round(tmp)
+    tmp -= np.rint(tmp)
     return tmp, np.min(diffs)
 
 
 def search_G2(rot, tran, pos1, pos2, cell=None):
     """
     search the best matched position in G2 basis
 
@@ -213,34 +213,34 @@
         cell: 3*3 matrix
 
     Returns:
         pos: matched position in G2
         dist: relative distance
     """
 
-    pos1 -= np.round(pos1)
+    pos1 -= np.rint(pos1)
     shifts = ALL_SHIFTS
 
     dists = []
     for shift in shifts:
         res = np.dot(rot, pos1 + shift + tran.T)
         diff = res - pos2
-        diff -= np.round(diff)
+        diff -= np.rint(diff)
         dist = np.linalg.norm(diff)
         dists.append(dist)
         if dist < 1e-1:
             break
     dists = np.array(dists)
     dist = np.min(dists)
     shift = shifts[np.argmin(dists)]
     pos = np.dot(rot, pos1 + shift + tran.T)
 
 
     diff = pos - pos2
-    diff -= np.round(diff)
+    diff -= np.rint(diff)
 
     if cell is not None:
         diff = np.dot(diff, cell)
 
     dist = np.linalg.norm(diff)
 
     return pos, dist
@@ -657,15 +657,15 @@
 
             tmp, _ = search_G1(splitter.G, rot, tran, coord_G2, wp1, op_G1)
 
             # initial guess on disp
             if translation is None:
                 coord_G2, dist1 = search_G2(inv_rot, -tran, tmp, coord_H, None)
                 diff = coord_G2 - coord_H
-                diff -= np.round(diff)
+                diff -= np.rint(diff)
                 translation = diff.copy()
                 for m in range(3):
                     if abs(diff[m])<1e-4:
                         mask.append(m)
                 dist = 0
             else:
                 coord_G2, dist = search_G2(inv_rot, -tran, tmp, coord_H+translation, self.cell)
@@ -708,25 +708,25 @@
         # since rotation does not change, search for the closest match on rotation
         # then we can get the translation vector
         for op_G22 in ops_G22:
             diff = (op_G22.rotation_matrix - op_G21.rotation_matrix).flatten()
             if np.sum(diff**2) < 1e-3:
                 trans = op_G22.translation_vector - op_G21.translation_vector
                 break
-        trans -= np.round(trans)
+        trans -= np.rint(trans)
         coords11 = apply_ops(coord1_G2, ops_H1)
         coords11 += trans
         tmp, dist = get_best_match(coords11, coord2_G2, self.cell)
 
         # needed displacement
         if run_type == 1:
             return dist/2 #np.linalg.norm(np.dot(d/2, self.cell))
         else:
             d = coord2_G2 - tmp
-            d -= np.round(d)
+            d -= np.rint(d)
             op_G11 = splitter.G1_orbits[id][0][0]
             coord2_G2 -= d/2
             coord1_G2 += d/2
             coord1_G1, _ = search_G1(splitter.G, rot, tran, tmp, wp1, op_G11)
             return coord1_G1, [coord1_G2, coord2_G2], coord_H
 
     def symmetrize_site_double_t(self, splitter, id, coord_H, translation, run_type=1):
@@ -765,15 +765,15 @@
 
         #self.print_wp(splitter, id)
         if run_type == 1:
             return dist/2
         else:
             # G1->G2->H
             d = coord2_G1 - tmp
-            d -= np.round(d)
+            d -= np.rint(d)
             coord2_G1 -= d/2
 
             coords22 = apply_ops(coord2_G1, ops_G1)
             coord1_G1, dist = get_best_match(coords22, coord1_G1, cell_G)
             #print("in G", l1, coord1_G1, l2, coord2_G1)
 
             # backward search (G->H)
@@ -882,15 +882,15 @@
         for i, wp2 in enumerate(sp.wp2_lists):
             wp1 = sp.wp1_lists[i]
             strs = ''
             for wp in wp2:
                 x, y, ele = coords_H[count], coords_G[count], elements[count]
                 label = wp.get_label() + '->' + wp1.get_label()
                 dis = y - x - translation
-                dis -= np.round(dis)
+                dis -= np.rint(dis)
                 dis_abs = np.linalg.norm(dis.dot(self.cell))
                 output = "{:2s}[{:8s}] {:8.4f}{:8.4f}{:8.4f}".format(ele, label, *x)
                 output += " -> {:8.4f}{:8.4f}{:8.4f}".format(*y)
                 output += " -> {:8.4f}{:8.4f}{:8.4f} {:8.4f}".format(*dis, dis_abs)
                 count += 1
                 disps.append(dis_abs)
                 print(output)
@@ -923,15 +923,15 @@
         # Get the list of atomic displacements
         disps = []
         count = 0
         for wp2 in sp.wp2_lists:
             for wp in wp2:
                 x, y, ele = coords_H1[count], coords_G2[count], elements[count]
                 disp = y - x - translation
-                disp -= np.round(disp)
+                disp -= np.rint(disp)
                 disps.append(disp)
                 count += 1
 
         # Create the PyXtals
         strucs = []
         disps = np.array(disps)
         disps /= (N_images-1)
```

### Comparing `pyxtal-0.6.5/pyxtal/symmetry.py` & `pyxtal-0.6.6/pyxtal/symmetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     filtered_coords_euclidean,
     distance,
     distance_matrix,
     create_matrix,
     OperationAnalyzer,
     check_images,
 )
-from pyxtal.constants import letters
+from pyxtal.constants import letters, hex_cell, all_sym_directions
 import importlib.util
 import os
 
 def rf(package_name, resource_path):
     package_path = importlib.util.find_spec(package_name).submodule_search_locations[0]
     return os.path.join(package_path, resource_path)
 # ------------------------------ Constants ---------------------------------------
@@ -53,21 +53,15 @@
 point_df = read_csv(rf("pyxtal", "database/point.csv"))
 point_symmetry_df = read_csv(rf("pyxtal", "database/point_symmetry.csv"))
 point_generators_df = read_csv(rf("pyxtal", "database/point_generators.csv"))
 symbols = loadfn(rf("pyxtal", "database/symbols.json"))
 t_subgroup = loadfn(rf("pyxtal",'database/t_subgroup.json'))
 k_subgroup = loadfn(rf("pyxtal",'database/k_subgroup.json'))
 wyc_sets = loadfn(rf("pyxtal",'database/wyckoff_sets.json'))
-hex_cell = np.array([[1, -0.5, 0], [0, np.sqrt(3) / 2, 0], [0, 0, 1]])
 hall_table = read_csv(rf("pyxtal", "database/HM_Full.csv"), sep=',')
-all_directions = [(1, 0, 0), (0, 1, 0), (0, 0, 1), (1, 1, 1),
-                  (1, -1, -1), (-1, 1, -1), (-1, -1, 1), (1, -1, 0),
-                  (1, 1, 0), (0, 1, -1), (0, 1, 1), (-1, 0, 1),
-                  (1, 0, 1), (1, 2, 0), (2, 1, 0)]
-
 #The map between spglib default space group and hall numbers
 spglib_hall_numbers = [
 1,   2,   3,   6,   9,   18,  21,  30,  39,  57,  60,  63,  72,  81,  90,
 108, 109, 112, 115, 116, 119, 122, 123, 124, 125, 128, 134, 137, 143, 149,
 155, 161, 164, 170, 173, 176, 182, 185, 191, 197, 203, 209, 212, 215, 218,
 221, 227, 228, 230, 233, 239, 245, 251, 257, 263, 266, 269, 275, 278, 284,
 290, 292, 298, 304, 310, 313, 316, 322, 334, 335, 337, 338, 341, 343, 349,
@@ -555,14 +549,42 @@
                 if True in _free:
                     has_freedom.append(True)
                 else:
                     has_freedom.append(False)
 
         return combinations, has_freedom, indices
 
+    def get_spg_symmetry_object(self):
+        """
+        Generate the symmetry table for the given space group
+        It only supports space group now!
+        """
+
+        if self.dim == 3:
+            l_type, bravis = self.lattice_type, self.symbol[0]
+            wp = self.get_wyckoff_position(0)
+
+            if 143 <= self.number <= 194:
+                ops = wp.get_euclidean_ops()
+                hexagonal = True
+            else:
+                ops = wp.ops
+
+            if bravis in ['A', 'B', 'C', 'I']:
+                ops = ops[:int(len(ops)/2)]
+            elif bravis == 'R':
+                ops = ops[:int(len(ops)/3)]
+            elif bravis == 'F':
+                ops = ops[:int(len(ops)/4)]
+
+            return site_symmetry(ops, l_type, bravis, True)
+            #ss.to_beautiful_matrix_representation()
+        else:
+            raise ValueError("Only supports space group symmetry")
+
     def get_wyckoff_position(self, index):
         """
         Returns a single Wyckoff_position object.
 
         Args:
             index: the index of the Wyckoff position within the group.
 
@@ -779,15 +801,15 @@
                 sgs = range(1,231)
             else:
                 sgs = G
 
             for sg in sgs:
                 subgroups = None
                 if group_type == 't':
-                    if sg>self.number:
+                    if sg > self.number:
                         subgroups = Group(sg, quick=True).get_max_t_subgroup()
                 else:
                     g1 = Group(sg)
                     if g1.point_group == self.point_group:
                         subgroups = Group(sg, quick=True).get_max_k_subgroup()
                 if subgroups is not None:
                     for i, sub in enumerate(subgroups['subgroup']):
@@ -1354,31 +1376,32 @@
     -x+1/2, -y, z+1/2
     -x, y+1/2, -z+1/2
     x+1/2, -y+1/2, -z
 
     """
 
     #=============================Initialization===========================
-    def from_dict(dictionary):
+    @classmethod
+    def from_dict(cls, dictionary):
         """
         Constructs a Wyckoff_position object using a dictionary.
         """
-        wp = Wyckoff_position()
+        wp = cls()
         for key in dictionary:
             setattr(wp, key, dictionary[key])
         #wp.get_site_symmetry()
         wp.set_euclidean()
         # For nonstandard setting only
         if wp.P1 is not None and not identity_ops(wp.P1):
             wp.set_generators()
             wp.set_ops()
         return wp
 
-
-    def from_group_and_letter(group, letter, dim=3, style='pyxtal', hn=None):
+    @classmethod
+    def from_group_and_letter(cls, group, letter, dim=3, style='pyxtal', hn=None):
         """
         Creates a Wyckoff_position using the space group number and index
 
         Args:
             group: the international number of the symmetry group
             letter: e.g. 4a
             dim: the periodic dimension of the crystal
@@ -1389,20 +1412,21 @@
         for c in letter:
             if c.isalpha():
                 letter = c
                 break
         ops_all = get_wyckoffs(group, dim=dim)
         index = index_from_letter(letter, ops_all, dim=dim)
         if hn is not None:
-            wp = Wyckoff_position.from_group_and_index(hn, index, dim, use_hall=True, wyckoffs=ops_all)
+            wp = cls.from_group_and_index(hn, index, dim, use_hall=True, wyckoffs=ops_all)
         else:
-            wp = Wyckoff_position.from_group_and_index(group, index, dim, style=style, wyckoffs=ops_all)
+            wp = cls.from_group_and_index(group, index, dim, style=style, wyckoffs=ops_all)
         return wp
 
-    def from_group_and_index(group, index, dim=3, use_hall=False, style='pyxtal', wyckoffs=None):
+    @classmethod
+    def from_group_and_index(cls, group, index, dim=3, use_hall=False, style='pyxtal', wyckoffs=None):
         """
         Creates a Wyckoff_position using the space group number and index
 
         Args:
             group: the international number of the symmetry group
             index: the index of the Wyckoff position within the group.
             dim: the periodic dimension of the crystal
@@ -1456,39 +1480,40 @@
                   "P1": P1,
                   "hall_number": hall_number,
                   "symbol": symbol,
                   "directions": directions,
                   "lattice_type": lattice_type,
                  }
 
-        return Wyckoff_position.from_dict(wpdict)
+        return cls.from_dict(wpdict)
 
-    def from_symops_wo_group(ops):
+    @classmethod
+    def from_symops_wo_group(cls, ops):
         """
         search Wyckoff Position by symmetry operations
         Now only supports space group symmetry
         Assuming general position only
 
         Args:
             ops: a list of symmetry operations
 
         Returns:
             `Wyckoff_position`
         """
         _, spg_num = get_symmetry_from_ops(ops)
-        wp = Wyckoff_position.from_group_and_index(spg_num, 0)
+        wp = cls.from_group_and_index(spg_num, 0)
         if isinstance(ops[0], str):
             ops = [SymmOp.from_xyz_str(op) for op in ops]
         wp.ops = ops
         match_spg, match_hm = wp.update()
         #print("match_spg", match_spg, "match_hall", match_hm)
         return wp
 
-
-    def from_symops(ops, G):
+    @classmethod
+    def from_symops(cls,ops, G):
         """
         search Wyckoff Position by symmetry operations
 
 
         Args:
             ops: a list of symmetry operations
             G: the Group object
@@ -1797,27 +1822,27 @@
     def get_site_symm_wo_translation(self):
         ops = []
         for op in self.symmetry[0]:
             op = SymmOp.from_rotation_and_translation(op.rotation_matrix, [0, 0, 0])
             ops.append(op)
         return ops
 
-    def get_site_symmetry_object(self):
-        ops = self.get_site_symm_ops()
+    def get_site_symmetry_object(self, idx=0):
+        ops = self.get_site_symm_ops(idx)
         return site_symmetry(ops, self.lattice_type, self.symbol[0])
 
-    def get_site_symmetry(self):
-        ss = self.get_site_symmetry_object()
+    def get_site_symmetry(self, idx=0):
+        ss = self.get_site_symmetry_object(idx)
         self.site_symm = ss.name #ss_string_from_ops(ops, self.number, dim=self.dim)
 
-    def get_site_symm_ops(self):
+    def get_site_symm_ops(self, idx=0):
         if self.euclidean:
-            ops = self.get_euclidean_symmetries()
+            ops = self.get_euclidean_symmetries(idx)
         else:
-            ops = self.symmetry[0]
+            ops = self.symmetry[idx]
         return ops
 
     def get_hm_number(tol=1e-5):
         if self.index == 0:
             return get_symmetry_from_ops(self.ops, tol)[0]
         else:
             print(self)
@@ -1869,27 +1894,47 @@
                     if self.ops[0].rotation_matrix[2,2] != 1:
                         return [2]
                     elif self.ops[0].rotation_matrix[1,1] != 1:
                         return [1]
                     elif self.ops[0].rotation_matrix[0,0] != 1:
                         return [0]
 
-    def get_euclidean_symmetries(self):
+    def get_euclidean_symmetries(self, idx=0):
         """
         return the symmetry operation object at the Euclidean space
 
         Returns:
             list of pymatgen SymmOp object
         """
+        if idx >= len(self.symmetry):
+            raise ValueError("Cannot pick {:d} in {:d} operations".format(idx, len(self.symmetry)))
         ops = []
-        for op in self.symmetry[0]:
+        for op in self.symmetry[idx]:
             hat = SymmOp.from_rotation_and_translation(hex_cell, [0, 0, 0])
             ops.append(hat * op * hat.inverse)
         return ops
 
+    def get_euclidean_ops(self):
+        """
+        return the symmetry operation object at the Euclidean space
+
+        Returns:
+            list of pymatgen SymmOp object
+        """
+        ops = [None] * len(self.ops)
+        for i, op in enumerate(self.ops):
+            hat = SymmOp.from_rotation_and_translation(hex_cell, [0, 0, 0])
+            op_tmp = hat * op * hat.inverse
+            ops[i] = op_tmp.from_rotation_and_translation(op_tmp.rotation_matrix,
+                                                          op.translation_vector)
+            #ops[i].translation_vector = op.translation_vector
+
+        return ops
+
+
     def get_euclidean_generator(self, cell, idx=0):
         """
         return the symmetry operation object at the Euclidean space
 
         Args:
             cell: 3*3 cell matrix
             idx: the index of wp generator
@@ -1947,18 +1992,21 @@
         >>> wp2.get_all_positions([1/2, 1/2, 1/2])
         array([[0. , 0. , 0. ],
                [0.5, 0. , 0.5],
                [0. , 0.5, 0. ],
                [0.5, 0.5, 0.5]])
         """
 
-        pos0, _, _ = self.merge(pos, np.eye(3), 0.01)
-        res = self.apply_ops(pos0)
-        res -= np.floor(res)
-        return res
+        pos0 = self.search_generator(pos)
+        if pos0 is not None:
+            res = self.apply_ops(pos0)
+            res -= np.floor(res)
+            return res
+        else:
+            return None
 
     #=============================Evaluations===========================
     def is_standard_setting(self):
         """
         Check if the symmetry operation follows the standard setting
         """
         G_ops = get_wyckoffs(self.number, dim=self.dim)
@@ -1984,15 +2032,15 @@
             ops0 = wp2.ops
 
         if len(ops0) == len(self.ops):
             count = 0
             for i, op0 in enumerate(ops0):
                 for j, op1 in enumerate(self.ops):
                     diff0 = op0.translation_vector - op1.translation_vector
-                    diff0 -= np.round(diff0)
+                    diff0 -= np.rint(diff0)
                     diff1 = op0.rotation_matrix - op1.rotation_matrix
                     if max([np.abs(diff0).sum(), np.abs(diff1).sum()]) < tol:
                         count += 1
             if count == len(ops0):
                 return True
             else:
                 return False
@@ -2071,15 +2119,15 @@
         if pt1 is None or pt2 is None:
             return False
         else:
             pt1 = np.array(pt1); pt1 -= np.floor(pt1)
             pt2 = np.array(pt2); pt2 -= np.floor(pt2)
             pts = self.apply_ops(pt1); pts -= np.floor(pts)
             diffs = pt2 - pts
-            diffs -= np.round(diffs)
+            diffs -= np.rint(diffs)
             diffs = np.dot(diffs, cell)
             dists = np.linalg.norm(diffs, axis=1)
             #print(dists)
             if len(dists[dists<tol]) > 0:
                 return True
             else:
                 return False
@@ -2161,14 +2209,15 @@
             passed_distance_check = True
             x = np.argwhere(dm < tol)
             for y in x:
                 # Ignore distance from atom to itself
                 if y[0] == 0 and y[1] == 0:
                     pass
                 else:
+                    #print(dm); print(y)
                     passed_distance_check = False
                     break
 
             # for molecular crystal, one more check
             if not check_images([coor[0]], [6], lattice, PBC=PBC, tol=tol):
                 passed_distance_check = False
 
@@ -2299,15 +2348,15 @@
             ops = get_wyckoffs(self.number, dim=self.dim)[0]
 
         match = False
         for op in ops:
             pos1 = op.operate(pos) #
             pos0 = self.ops[0].operate(pos1)
             diff = pos1 - pos0
-            diff -= np.round(diff)
+            diff -= np.rint(diff)
             diff = np.abs(diff)
             #print(self.letter, "{:24s}".format(op.as_xyz_str()), pos, pos0, pos1, diff)
             if diff.sum() < tol:
                 pos1 -= np.floor(pos1)
                 match = True
                 break
 
@@ -2333,15 +2382,15 @@
             ops = get_wyckoffs(self.number, dim=self.dim)[0]
 
         coords = []
         for op in ops:
             pos1 = op.operate(pos)
             pos0 = self.ops[0].operate(pos1)
             diff = pos1 - pos0
-            diff -= np.round(diff)
+            diff -= np.rint(diff)
             diff = np.abs(diff)
             #print(wp.letter, pos1, pos0, diff)
             if diff.sum() < tol:
                 pos1 -= np.floor(pos1)
                 coords.append(pos1)
         return coords
 
@@ -2367,15 +2416,20 @@
             PBC: A periodic boundary condition list, where 1 means periodic, 0
                 means not periodic. Ex: [1,1,1] -> full 3d periodicity, [0,0,1]
                 -> 1d periodicity along the z axis
 
         Returns:
             a transformed 3-vector (numpy array)
         """
-        op = self.ops[id]
+        # Must be different for hexcell
+        if self.euclidean:
+            op = self.get_euclidean_generator(cell, id)
+        else:
+            op = self.ops[id]
+
         rot = op.rotation_matrix
         trans = op.translation_vector
         point = np.array(point, dtype=float)
 
         def project_single(point, rot, trans):
             # move the point in the opposite direction of the translation
             point -= trans
@@ -2594,15 +2648,15 @@
     return SymmOp(m)
 
 def are_equivalent_ops(op1, op2, tol=1e-2):
     """
     check if two ops are equivalent, assuming the same ordering
     """
     diff = op1.affine_matrix - op2.affine_matrix
-    diff[:,3] -= np.round(diff[:,3])
+    diff[:,3] -= np.rint(diff[:,3])
     diff = np.abs(diff.flatten())
     if np.sum(diff) < tol:
         return True
     else:
         return False
 
 
@@ -2697,54 +2751,117 @@
     of the symmetry elements. The constituents of the oriented
     symbol are ordered according to the symmetry directions of
     the corresponding crystal lattice (primary, secondary and tertiary)
 
     Args:
         ops: a list of SymmOp objects representing the site symmetry
         lattice_type (str): e.g., 'cubic'
-        hm_symbol (str): hm_symbol for lattice 'P', 'R'
+        Bravis (str): 'P', 'R', 'A', 'B', 'C', 'F', 'I'
+        parse_trans (bool): do space group or site
 
     Returns:
         a string representing the site symmetry (e.g., `2mm`)
     """
-    def __init__(self, ops, lattice_type, hm_symbol):
+    def __init__(self, ops, lattice_type, Bravis='P', parse_trans=False):
 
         #self.G = G
-        self.opas = [OperationAnalyzer(op) for op in ops]
+        if lattice_type in ['hexagonal', 'trigonal']:
+            hexagonal = True
+        else:
+            hexagonal = False
+
+        self.parse_trans = parse_trans
+        self.opas = [OperationAnalyzer(op, parse_trans, hexagonal) for op in ops]
         self.lattice_type = lattice_type
-        self.directions = get_symmetry_directions(lattice_type, hm_symbol)
-        tables = self.to_table()
-        self.set_full_hm_symbols(tables)
-        self.set_short_symbols()
+        self.directions = get_symmetry_directions(lattice_type, Bravis)
+
+        if not parse_trans:
+            self.symbols = ['1', '-1', '2', 'm', '3', '4', '-4', '-3', '6', '-6']
+        else:
+            self.symbols = ['1', '-1', '2', '2_1', 'm', 'a', 'b', 'c', 'n', 'd',
+                   '3', '3_1', '3_2', '4', '-4', '4_1', '4_2', '4_3',
+                   '-3', '6', '6_1', '6_2', '6_3', '6_4', '6_5', '-6']
+        self.set_table()
+
+        if not parse_trans:
+            self.set_full_hm_symbols(self.table)
+            self.set_short_symbols()
+
+    def to_one_hot(self):
+        matrix = self.to_matrix_representation()
+        one_hot_matrix = np.zeros([len(matrix), 13], dtype=int)
+        for i, axis in enumerate(all_sym_directions):
+            symbol, id = self.get_highest_symmetry(matrix[i])
+            one_hot_matrix[i, id] = 1
+        return one_hot_matrix
+
+    def to_matrix_representation_spg(self):
+        """
+        To create a binary matrix to represent the symmetry elements on each axis
+        Translation is alos counted here.
+        """
+
+        matrix = np.zeros([len(all_sym_directions), len(self.symbols)], dtype=int)
+        # every direction must has identity symmetry
+        matrix[:, 0] = 1
+        self.inversion = False
+
+        for opa in self.opas:
+            if opa.type == 'inversion':
+                self.inversion = True
+
+            elif opa.type != 'identity':
+                _ax0 = opa.axis /np.linalg.norm(opa.axis)
+
+                store = False
+                for i, ax in enumerate(all_sym_directions):
+                    ax0 = ax / np.linalg.norm(ax)#; print(opa.axis, ax, np.dot(_ax0, ax0))
+                    if np.isclose(abs(np.dot(_ax0, ax0)), 1):
+                        store = True
+                        break
+
+                if store:
+                    # Pure rotation
+                    #print('add symmetry', i, ax, opa.type, opa.order)
+                    if opa.symbol in self.symbols:
+                        matrix[i, self.symbols.index(opa.symbol)] = 1
+                    else:
+                        print("To debug", opa.symbol, opa); import sys; sys.exit()
+                else:
+                    raise ValueError("Cannot parse the axis", opa.axis, all_sym_directions)
+
+            if self.inversion:
+                matrix[:, 1] = 1 # if inversion is present
+        return matrix
+
 
     def to_matrix_representation(self):
         """
-        To create a 15 * 14 binary matrix to represent the
-        symmetry elements on each axes
+        To create a 15 * 10 binary matrix to represent the
+        symmetry elements on each axis
         #[1, -1, 2, m, 3, 2/m, 4, -3, 6, 4/m, -6, 6/m]
         [1, -1, 2, m, 3, 4, -3, 6, -6]
         """
         symbols = ['1', '-1', '2', 'm', '3', '4', '-4', '-3', '6', '-6']
-        matrix = np.zeros([len(all_directions), len(symbols)], dtype=int)
+        matrix = np.zeros([len(all_sym_directions), len(symbols)], dtype=int)
         # every direction must has identity symmetry
         matrix[:, 0] = 1
         self.inversion = False
 
         for opa in self.opas:
             if opa.type == 'inversion':
                 self.inversion = True
+
             elif opa.type != 'identity':
-                for i, ax in enumerate(all_directions):
+                _ax0 = opa.axis /np.linalg.norm(opa.axis)
+
+                for i, ax in enumerate(all_sym_directions):
                     store = False
-                    if self.lattice_type in ['hexagonal', 'trigonal']:
-                        ax0 = np.dot(ax, hex_cell.T)
-                        ax0 /= np.linalg.norm(ax0)
-                    else:
-                        ax0 = ax / np.linalg.norm(ax)
-                    if np.isclose(abs(np.dot(opa.axis, ax0)), 1):
+                    ax0 = ax / np.linalg.norm(ax) #; print(opa.axis, ax, np.dot(opa.axis, ax0))
+                    if np.isclose(abs(np.dot(_ax0, ax0)), 1):
                         store = True
                         break
                 if store:
                     # Pure rotation
                     #print('add symmetry', i, ax, opa.type, opa.order)
                     if opa.type == 'rotation':
                         if opa.order == 2:
@@ -2754,61 +2871,72 @@
                         elif opa.order == 4:
                             matrix[i, 5] = 1
                         elif opa.order == 6:
                             matrix[i, 8] = 1
                         else:
                             raise RuntimeError("Unexpected rotation order", opa.order)
                     elif opa.type == 'rotoinversion':
-                        if opa.order == 2:
+                        if opa.rotation_order == 2:
                             matrix[i, 3] = 1 # -2 is m
-                        elif opa.order == 3:
-                            matrix[i, 7] = 1 # -2 is m
-                        elif opa.order == 4:
+                        elif opa.rotation_order == 3:
+                            matrix[i, 7] = 1 # -3
+                        elif opa.rotation_order == 4:
                             matrix[i, 6] = 1 # -4
-                        elif opa.order == 6:
+                        elif opa.rotation_order == 6:
                             matrix[i, 9] = 1
                         else:
                             raise RuntimeError("Unexpected rotinversion order", opa.order)
+                else:
+                    raise ValueError("Cannot parse the axis", opa.axis, all_sym_directions)
+
             if self.inversion:
                 matrix[:, 1] = 1 # if inversion is present
         return matrix
 
-    def to_table(self, skip=False):
+    def set_table(self, skip=False):
         """
         Get the complete table representation.
 
         Args:
             skip (bool): whether or not skip 1 or -1 symmetry
 
         Returns:
             sorted table with (list of symmetry elements, symbols, order)
         """
         # Complete list of symmetry for one given axis
         # symbols = ['1', '-1', '2', 'm', '3', '4', '-4', '-3', '6', '-6']
         if self.lattice_type == 'triclinic': skip = False
 
-        matrix = self.to_matrix_representation()
+        if self.parse_trans:
+            matrix = self.to_matrix_representation_spg()
+        else:
+            matrix = self.to_matrix_representation()
+
         tables = []
-        for i, axis in enumerate(all_directions):
+        for i, axis in enumerate(all_sym_directions):
             direction_id = find_axis_order(axis, self.directions)
             if direction_id is not None:
                 if skip:
                     num_symmetries = matrix[i, 2:].sum()
                 else:
                     num_symmetries = matrix[i].sum()
                 if num_symmetries > 0:
                     strs = '{:4d} ({:2d} {:2d} {:2d}): '.format(direction_id, *axis)
-                    strs += "{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}".format(*matrix[i])
-                    symbol = self.get_highest_symmetry(matrix[i])
-                    strs += "{:>6s}".format(symbol)
-                    tables.append((strs, symbol, direction_id))
+                    for sym in matrix[i]:
+                        strs +="{:4d} ".format(sym)
+                    #strs += "{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}{:4d}".format(*matrix[i])
+                    if not self.parse_trans:
+                        symbol, _ = self.get_highest_symmetry(matrix[i])
+                        strs += "{:>6s}".format(symbol)
+                        tables.append((strs, symbol, direction_id))
+                    else:
+                        tables.append((strs, direction_id))
             #else:
             #    raise ValueError('Wrong input axis', axis, 'lattice_type', self.lattice_type)
-        sorted_tables = sorted(tables, key=lambda x: x[-1])
-        return sorted_tables
+        self.table = sorted(tables, key=lambda x: x[-1])
 
     def set_full_hm_symbols(self, tables):
         """
         Set the full hm symbols for each axis
 
         Args:
             tables: sorted table with (list of symmetry elements, symbols, order)
@@ -2988,17 +3116,27 @@
     def to_beautiful_matrix_representation(self, skip=True):
         """
         A shortcut to check the representation
 
         Args:
             skip (bool): whether or not skip 1 or -1 symmetry
         """
-        print('Order    Axis       1  -1   2   m   3   4  -4  -3   6  -6   Group')
-        sorted_tables = self.to_table(skip)
-        for row in sorted_tables:
+        strs = 'Order    Axis       '
+        if self.parse_trans:
+            symbols = ['1', '-1', '2', '2_1', 'm', 'a', 'b', 'c', 'n', 'd',
+                   '3', '3_1', '3_2', '4', '-4', '4_1', '4_2', '4_3',
+                   '-3', '6', '6_1', '6_2', '6_3', '6_4', '6_5', '-6']
+        else:
+            symbols = ['1', '-1', '2', 'm', '3', '4', '-4', '-3', '6', '-6']
+
+        for symbol in symbols:
+            strs += '{:<4s} '.format(symbol)
+        print(strs)
+        if not hasattr(self, 'table'): self.set_table(skip)
+        for row in self.table:
             print(row[0])
 
     def get_highest_symmetry(self, row):
         #['1']
         #['1', '-1']
         #['1', '2']
         #['1', 'm']
@@ -3022,17 +3160,17 @@
             (np.array([1, 0, 1, 0, 0, 0, 1, 0, 0, 0], dtype=int), '-4'),
             (np.array([1, 1, 0, 0, 1, 0, 0, 1, 0, 0], dtype=int), '-3'),
             (np.array([1, 0, 1, 0, 1, 0, 0, 0, 1, 0], dtype=int), '6'),
             (np.array([1, 0, 0, 1, 1, 0, 0, 0, 0, 1], dtype=int), '-6'),
             (np.array([1, 1, 1, 1, 0, 1, 1, 0, 0, 0], dtype=int), '4/m'),
             (np.array([1, 1, 1, 1, 1, 0, 0, 1, 1, 1], dtype=int), '6/m')]
 
-        for ref_array in ref_arrays:
+        for i, ref_array in enumerate(ref_arrays):
             if np.array_equal(row, ref_array[0]):
-                return ref_array[1]
+                return ref_array[1], i
         else:
             symbols = ['1', '-1', '2', 'm', '3', '4', '-4', '-3', '6', '-6']
             strs = [symbols[i] for i, x in enumerate(row) if x == 1]
             raise ValueError("Incompatible symmetry list", strs)
 
 
 def organized_wyckoffs(group):
@@ -3294,15 +3432,15 @@
             of space group Ia-3(206). The site symmetry includes the operations
             (-z+1,x-1/2,-y+1/2) and (y+1/2,-z+1/2,-x+1). These operations are
             not listed in the general position, but correspond to the operations
             (-z,x+1/2,-y+1/2) and (y+1/2,-z+1/2,-x), respectively, just shifted
             by (+1,-1,0) and (0,0,+1), respectively.
             """
             el = SymmOp.from_rotation_and_translation(
-                op.rotation_matrix, op.translation_vector - np.round(displacement)
+                op.rotation_matrix, op.translation_vector - np.rint(displacement)
             )
             symmetry.append(el)
     return symmetry
 
 def check_wyckoff_position(points, group, tol=1e-3):
     """
     Given a list of points, returns a single index of a matching Wyckoff
@@ -3519,34 +3657,34 @@
         wp0 = G[0]
         coords = wp.search_all_generators(pos, wp0)
         if len(coords)>0:
             diffs = []
             for coord in coords:
                 tmp = op.operate(coord)
                 diff1 = tmp - pos
-                diff1 -= np.round(diff1)
+                diff1 -= np.rint(diff1)
                 dist = np.linalg.norm(diff1)
                 if dist < 1e-3:
                     return tmp
                 else:
                     diffs.append(dist)
             minID = np.argmin(diffs)
             return op.operate(coords[minID])
 
         # if not match, search for the closest solution
         else:
             # extract all possible xyzs
             all_xyz = apply_ops(pos, wp0)[1:]
             dists = all_xyz - pos
-            dists -= np.round(dists)
+            dists -= np.rint(dists)
             ds = np.linalg.norm(dists, axis=1)
             ids = np.argsort(ds)
             for id in ids:
                 d = all_xyz[id] - pos
-                d -= np.round(d)
+                d -= np.rint(d)
                 res = pos + d/2
                 if wp.search_generator(res, wp0) is not None:
                     #print(ds[id], pos, res)
                     return res
             return op.operate(pos)
 
 
@@ -3851,15 +3989,15 @@
 
     # in case of (x+1/2, y, z) as the first
     if np.linalg.norm(tran_P) > 1e-3:
         base = ops[0].translation_vector
         for i, op in enumerate(ops):
             inv = np.linalg.inv(op.affine_matrix)
             trans = inv[:3, 3] + base
-            trans -= np.round(trans)
+            trans -= np.rint(trans)
             rot_ops = ops[i].rotation_matrix
             ops[i] = SymmOp.from_rotation_and_translation(rot_ops, trans)
 
     return ops
 
 def trim_ops(ops):
     """
@@ -3955,26 +4093,36 @@
                 [(1, -1, 0), (1, 1, 0), (0, 1, -1),
                  (0, 1, 1), (-1, 0, 1), (1, 0, 1)]]
     else:
         return [[(0, 1, 0)]]
 
 
 if __name__ == "__main__":
-    print("Test of pyxtal.wp.site symmetry")
-    for i in [14, 36, 62, 99, 143, 160, 182, 191, 225, 230]:
+    print("Test pyxtal.wp.site symmetry")
+    spg_list = [14, 36, 62, 99, 143, 160, 182, 191, 225, 230]
+    for i in spg_list:
         g = Group(i)
         for wp in g:
             wp.get_site_symmetry()
             print("{:4d} {:10s} {:10s}".format(wp.number, wp.get_label(), wp.site_symm))
 
-    print("Test of pyxtal.wp.site symmetry representation")
-    for i in [14, 36, 62, 99, 143, 160, 182, 191, 225, 230]:
+    print("Test pyxtal.wp.site symmetry representation")
+    for i in spg_list:
         g = Group(i)
         for wp in g:
-            #ss = site_symmetry(wp.get_site_symm_ops(), g.lattice_type, g.symbol[0])
             if wp.index > 0:
-                ss = wp.get_site_symmetry_object()
-                print('\n{:4d} {:10s} {:10s}'.format(wp.number, wp.get_label(), ss.name), ss.hm_symbols)
-                ss.to_beautiful_matrix_representation(skip=True)
-                #print(ss.to_matrix_representation())
-                #if ss.name == '1':
-                #    print("Problem eixt")
+                for idx in range(1): #wp.multiplicity):
+                    ss = wp.get_site_symmetry_object(idx)
+                    print('\n{:4d} {:10s} {:10s}'.format(wp.number, wp.get_label(), ss.name), ss.hm_symbols)
+                    #ss.to_beautiful_matrix_representation(skip=True)
+                    #print(ss.to_matrix_representation())
+                    #print(ss.to_one_hot())
+
+    print("Test pyxtal.wp.site space group")
+    for i in spg_list:
+        g = Group(i)
+        print('\n', g.number, g.symbol)
+        ss = g.get_spg_symmetry_object()
+        ss.to_beautiful_matrix_representation()
+        #matrix = ss.to_matrix_representation_spg()
+        #print(matrix)
+        #print(sum(sum(matrix)))
```

### Comparing `pyxtal-0.6.5/pyxtal/test_all.py` & `pyxtal-0.6.6/pyxtal/test_all.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pyxtal.lattice import Lattice
 from pyxtal.molecule import pyxtal_molecule
 from pyxtal.symmetry import Group, Wyckoff_position, get_wyckoffs, Hall
 from pyxtal.XRD import Similarity
 from pyxtal.operations import get_inverse
 from pyxtal.supergroup import supergroups, supergroup
 from pyxtal.util import generate_wp_lib
-
+from pyxtal.wyckoff_site import atom_site
 
 def resource_filename(package_name, resource_path):
     package_path = importlib.util.find_spec(package_name).submodule_search_locations[0]
     return os.path.join(package_path, resource_path)
 
 cif_path = resource_filename("pyxtal", "database/cifs/")
 l01 = Lattice.from_matrix([[4.08, 0, 0], [0, 9.13, 0], [0, 0, 5.50]])
@@ -50,14 +50,23 @@
     def test_print_group_and_dof(self):
         for d in [(1, 6), (15, 4), (60, 3), (143, 2), (208, 1)]:
             (sg, dof_ref) = d
             g = Group(sg)
             dof = g.get_lattice_dof()
             self.assertTrue(dof == dof_ref)
 
+    def test_get_spg_symmetry_object(self):
+        spg_list = [14, 36, 62, 99, 143, 160, 182, 191, 225, 230]
+        ans = [32, 18, 36, 21, 16, 19, 24, 48, 62, 62]
+        for spg, num in zip(spg_list, ans):
+            g = Group(spg)
+            ss = g.get_spg_symmetry_object()
+            matrix = ss.to_matrix_representation_spg()
+            self.assertTrue(num == sum(sum(matrix)))
+
     def test_short_path(self):
         g = Group(217)
         path = g.short_path_to_general_wp(7)
         self.assertTrue(path[-1][2] == 145)
 
     def test_spg_symmetry(self):
         N_polar, N_centro, N_chiral = 0, 0, 0
@@ -571,14 +580,22 @@
         self.assertFalse(wp.are_equivalent_pts(a,e))
 
         wp = g[1]
         a = [ 0.00,  0.127,  0.254]
         b = [-0.01, -0.127, -0.250]
         self.assertTrue(wp.are_equivalent_pts(a,b))
 
+    def test_project(self):
+        pt = np.array([0.0629, 0.1258, 0.25])
+        g = Group(178)
+        wp = g[1]
+        xyz0 = wp.project(pt, np.eye(3))
+        diff = np.sum((pt - xyz0)**2)
+        self.assertTrue(diff < 1e-8)
+
     def test_euclidean(self):
 
         def check_error(spg, pt, cell):
             p0 = np.dot(pt, cell.matrix)
             for sg in spg:
                 wp = Group(sg)[0]
                 for i in range(len(wp)):
@@ -589,15 +606,15 @@
                     if wp.euclidean:
                         p2 = np.dot(op1.operate(p0), cell.inv_matrix)
                     else:
                         p2 = np.dot(op1.apply_rotation_only(p0), cell.inv_matrix)
                         p2 += op1.translation_vector
 
                     diff = p1-p2
-                    diff -= np.round(diff)
+                    diff -= np.rint(diff)
                     if np.linalg.norm(diff) > 0.02:
                         #res = '{:2d} {:28s}'.format(i, op0.as_xyz_str())
                         #res += ' {:28s}'.format(op1.as_xyz_str())
                         #res += '{:6.3f} {:6.3f} {:6.3f} -> '.format(*p1)
                         #res += '{:6.3f} {:6.3f} {:6.3f} -> '.format(*p2)
                         #res += '{:6.3f} {:6.3f} {:6.3f}'.format(*diff)
                         #print(res)
@@ -929,14 +946,29 @@
         l6 = Lattice.from_para(3.454, 3.401, 5.908, 90.00, 105.80, 90.00, ltype='monoclinic')
         l7 = Lattice.from_para(6.028, 3.419, 6.028, 90.00, 146.92, 90.00, ltype='monoclinic')
         l7, _ = l7.optimize_multi()
         trans, diff = l7.search_transformation(l6)
         l7 = l7.transform_multi(trans)
         self.assertTrue(np.abs(l7.matrix-l6.matrix).sum() < 0.25)
 
+    def test_is_valid_lattice(self):
+        l8 = Lattice.from_para(3.454, 3.401, 5.908, 90.00, 105.80, 91.00, ltype='monoclinic')
+        l9 = Lattice.from_para(3.454, 3.401, 5.908, 90.00, 105.80, 90.00, ltype='monoclinic')
+        l10 = Lattice.from_para(3.454, 3.401, 5.908, 90.00, 90.00, 90.00, ltype='cubic')
+        self.assertTrue(not l8.is_valid_lattice())
+        self.assertTrue(l9.is_valid_lattice())
+        self.assertTrue(not l10.is_valid_lattice())
+
+    def test_from_1d_representation(self):
+        lat = Lattice.from_1d_representation([5.09, 6.11], 'trigonal')
+        self.assertTrue(abs(lat.a-5.09)<1e-3)
+        self.assertTrue(abs(lat.c-6.11)<1e-3)
+        self.assertTrue(abs(lat.gamma-2/3*np.pi)<1e-3)
+
+
 class TestSymmetry(unittest.TestCase):
     def test_from_symops_wo_grou(self):
         data = [
         (["x, y, z", "-x, y+1/2, -z"], 4, 6),
         (["x, y, z", "-x+1/2, -y, z+1/2", "-x, y, z", "x+1/2, -y, z+1/2"], 31, 155),
         (["x, y, z", "-x, -y, -z", "-x+1/2, y+1/2, -z", "x+1/2, -y+1/2, z"], 14, 83),
         (["x, y, z", "-x, -y, -z", "-x+1/2, y+1/2, -z+1/2", "x+1/2, -y+1/2, z+1/2"], 14, 82),
@@ -1139,14 +1171,30 @@
         l = list(range(len(struc.atom_sites)))
         shuffle(l)
         struc.atom_sites = [struc.atom_sites[i] for i in l]
         struc.resort()
         N2 = len(struc.atom_sites)
         self.assertTrue(N1 == N2)
 
+class Test_wyckoff_site(unittest.TestCase):
+    def test_atom_site(self):
+        """
+        Test the search function
+        """
+        wp = Group(227)[-5]
+        arr = np.array([0.1, 0.1, 0.1])
+        for xyz in [[0.6501, 0.15001, 0.5999],
+                    [0.6501, 0.14999, 0.5999],
+                    [0.6499, 0.14999, 0.5999],
+                    [0.6499, 0.14999, 0.60001],
+                   ]:
+            site = atom_site(wp, xyz, search=True)
+            self.assertTrue(np.allclose(site.position, arr, rtol=1e-3))
+
+
 class Test_operations(unittest.TestCase):
     def test_inverse(self):
         coord0 = [0.35, 0.1, 0.4]
         coords = np.array([
           [0.350,  0.100,  0.400],
           [0.350,  0.100,  0.000],
           [0.350,  0.100,  0.000],
```

### Comparing `pyxtal-0.6.5/pyxtal/tolerance.py` & `pyxtal-0.6.6/pyxtal/tolerance.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/util.py` & `pyxtal-0.6.6/pyxtal/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,15 +461,15 @@
         orders.append(i)
         shifts.append(np.zeros(3))
         ref_i = refs[i]
         good = False
         for j in lefts[1:]:
             ref_j = refs[j]
             dist = ref_j - ref_i
-            shift = np.round(dist)
+            shift = np.rint(dist)
             dist -= shift
             dist = np.linalg.norm(dist.dot(atoms.cell[:]))
             if dist < tol:
                 orders.append(j)
                 shifts.append(shift)
                 good = True
                 break
@@ -591,14 +591,46 @@
                 if abs(vol1-vol2)/vol1<5e-2:
                     pmg_s2.remove_species("H")
                     if sm.StructureMatcher().fit(pmg_s1, pmg_s2):
                         #print(pmg_s2); import sys; sys.exit()
                         return False
         return True
 
+def new_struc_wo_energy(xtal, xtals):
+    """
+    check if this is a new structure
+
+    Args:
+        xtal: input structure
+        xtals: list of reference structures
+
+    Return:
+        `None` or the id of matched structure
+    """
+    import pymatgen.analysis.structure_matcher as sm
+
+    if xtal is None:
+        return False
+    else:
+        pmg_s1 = xtal.to_pymatgen()
+        pmg_s1.remove_species("H")
+        vol1 = pmg_s1.lattice.volume
+
+        for xtal2 in xtals:
+            #print(rep); print(rep2)
+            pmg_s2 = xtal2.to_pymatgen()
+            vol2 = pmg_s2.lattice.volume
+            if abs(vol1-vol2)/vol1<5e-2:
+                pmg_s2.remove_species("H")
+                if sm.StructureMatcher().fit(pmg_s1, pmg_s2):
+                    #print(pmg_s2); import sys; sys.exit()
+                    return False
+        return True
+
+
 
 if __name__ == "__main__":
     from argparse import ArgumentParser
 
     parser = ArgumentParser()
     parser.add_argument(
         "-f",
```

### Comparing `pyxtal-0.6.5/pyxtal/viz.py` & `pyxtal-0.6.6/pyxtal/viz.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/pyxtal/wyckoff_site.py` & `pyxtal-0.6.6/pyxtal/wyckoff_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,80 +26,86 @@
 from pyxtal.lattice import Lattice
 
 class atom_site:
     """
     Class for storing atomic Wyckoff positions with a single coordinate.
 
     Args:
-        wp: a `Wyckoff_position <pyxtal.symmetry.Wyckoff_position.html> object
-        coordinate: a fractional 3-vector for the generating atom's coordinate
-        specie: an Element, element name or symbol, or atomic number of the atom
-        search: to search for the optimum position for special wyckoff site
+        wp: a `WP <pyxtal.symmetry.Wyckoff_position.html> object
+        coordinate (float): a fractional (x, y, z) coordinate
+        specie (str): element name or symbol, or atomic number
+        search (bool): whether or not search generator for special WP
     """
 
     def __init__(self, wp=None, coordinate=None, specie=1, search=False):
+
         self.position = np.array(coordinate)
+        self.position -= np.floor(self.position)
         self.specie = Element(specie).short_name
         self.wp = wp
         self.coordination = None
 
         self._get_dof()
         self.PBC = self.wp.PBC
         self.multiplicity = self.wp.multiplicity
-        if search:
-            self.search_position()
+        if search: self.search_position()
+
         self.update()
 
     def __str__(self):
+
         if not hasattr(self.wp, "site_symm"): self.wp.get_site_symmetry()
         s = "{:>2s} @ [{:7.4f} {:7.4f} {:7.4f}], ".format(self.specie, *self.position)
         s += "WP [{:}] ".format(self.wp.get_label())
         if self.coordination is not None:
             s += " CN [{:2d}] ".format(self.coordination)
         s += "Site [{:}]".format(self.wp.site_symm.replace(" ",""))
 
         return s
 
     def __repr__(self):
+
         return str(self)
 
     def copy(self):
         """
         Simply copy the structure
         """
+
         return deepcopy(self)
 
     def save_dict(self):
+
         dict0 = {"position": self.position,
                  "specie": self.specie,
                  "wp": self.wp.save_dict(),
                 }
         return dict0
 
     def _get_dof(self):
         """
         get the number of dof for the given structures:
         """
+
         self.dof = self.wp.get_dof()
-        #freedom = np.trace(self.wp.ops[0].rotation_matrix) > 0
-        #self.dof = len(freedom[freedom==True])
-        #self.dof = len(freedom[freedom==True])
 
     @classmethod
     def load_dict(cls, dicts):
         """
         load the sites from a dictionary
         """
+
         position = dicts["position"]
         specie = dicts["specie"]
         if 'wp' in dicts:
             wp = Wyckoff_position.load_dict(dicts['wp'])
         else:
             hn, index = dicts['hn'], dicts['index']
             wp = Wyckoff_position.from_group_and_index(hn, index, use_hall=True)
+
         return cls(wp, position, specie)
 
     def perturbate(self, lattice, magnitude=0.1):
         """
         Random perturbation of the site
 
         Args:
@@ -108,31 +114,39 @@
         """
         dis = (np.random.sample(3) - 0.5).dot(lattice)
         dis /= np.linalg.norm(dis)
         dis *= magnitude
         pos = self.position + dis.dot(np.linalg.inv(lattice))
         self.update(pos)
 
-    def search_position(self):
+    def search_position(self, tol=1e-3):
         """
-        Sometimes, the initial posiition is not the proper generator
+        Sometimes, the initial position is not the proper generator
         Needs to find the proper generator
         """
+
+        found = False
         if self.wp.index > 0:
             wp0 = Group(self.wp.number, self.wp.dim)[0]
-            pos = self.position
-            coords = wp0.apply_ops(pos)
-            for coord in coords:
+            for coord in wp0.apply_ops(self.position):
+                coord -= np.floor(coord)
                 ans = self.wp.ops[0].operate(coord)
                 diff = coord - ans
-                diff -= np.floor(diff)
-                if np.sum(diff**2)<1e-4:
+                diff -= np.rint(diff)
+                if np.sum(diff**2) < tol:
+                    found = True
+                    #print(found, coord, coord-ans)
                     self.position = coord - np.floor(coord)
                     break
 
+        if not found:
+            print("\nInput xyz", self.position)
+            print("Target operation", self.wp.ops[0].as_xyz_str())
+            raise ValueError("Cannot generate the desried generator")
+
     def encode(self):
         """
         transform dict to 1D vector
         [specie, wp.index, free x, y, z]
         """
         xyz = self.wp.get_free_xyzs(self.position)
         #print(self.wp.ops[0].rotation_matrix, self.wp.get_frozen_axis(), self.wp.get_dof())
@@ -182,37 +196,40 @@
         )
         self.update()
 
     def update(self, pos=None, reset_wp=False):
         """
         Used to generate coords from self.position
         """
+
         if pos is None:
             pos = self.position
         if reset_wp:
             self.wp.ops = Group(self.wp.number)[self.wp.index].ops
         self.coords = self.wp.apply_ops(pos)
         self.position = self.coords[0]
 
     def get_translations(self, pos, axis):
         """
-        return the displacement towards the reference positions
+        Get the displacement towards the reference positions
 
         Args:
             pos: reference position (1*3 vector)
             lattice: 3*3 matrix
             translation:
             axis:
         """
+
         #diffs0 = pos - self.coords
         diffs0 = self.wp.apply_ops(pos) - self.position
         diffs = diffs0.copy()
-        diffs -= np.round(diffs)
+        diffs -= np.rint(diffs)
         diffs[:, axis] = 0
         translations = diffs0 - diffs
+
         return translations
 
     def get_disp(self, pos, lattice, translation):
         """
         return the displacement towards the reference positions
 
         Args:
@@ -221,35 +238,35 @@
             translation:
         """
         coords = self.wp.apply_ops(pos)
         diffs = coords - (self.position + translation)
         #coords = self.wp.apply_ops(self.position + translation)
         #diffs = pos - coords
 
-        diffs -= np.round(diffs)
+        diffs -= np.rint(diffs)
         dists = np.linalg.norm(diffs.dot(lattice), axis=1)
         id = np.argmin(dists)
 
         #print("++++", id, dists[id], id, diffs[id], translation) #; import sys; sys.exit()
         return diffs[id], dists[id]
 
     def check_with_ws2(self, ws2, lattice, tm, same_group=True):
         """
         Given two Wyckoff sites, checks the inter-atomic distances between them.
 
         Args:
-            ws2: a different Wyckoff_site object (will always return False if
+            - ws2: a different WP object (will always return False if
             two identical WS's are provided)
-            lattice: a 3x3 cell matrix
-            same_group: whether or not the two WS's are in the same structure.
+            - lattice: a 3x3 cell matrix
+            - same_group: whether or not two WS's are in the same structure.
             Default value True reduces the calculation cost
         Returns:
-            True if all distances are greater than the allowed tolerances.
-            False if any distance is smaller than the allowed tolerance
+            True or False
         """
+
         # Ensure the PBC values are valid
         if self.PBC != ws2.PBC:
             raise ValueError("PBC values do not match between Wyckoff sites")
         # Get tolerance
         tol = tm.get_tol(self.specie, ws2.specie)
         # Symmetry shortcut method: check only some atoms
         if same_group is True:
@@ -308,31 +325,33 @@
         site2.specie = eles[1]
         site1.update(site1.position + shift)
         site2.update(site2.position - shift)
         return site1, site2
 
     def to_mol_site(self, lattice, molecule, ori=[0, 0, 0], reflect=False, type_id=0):
         """
-        transform it to the mol_sites, i.e., to build a molecule on
+        Transform it to the mol_sites, i.e., to build a molecule on
         the current WP
         """
+
         dicts = {}
         dicts['smile'] = molecule.smile
         dicts['type'] = type_id
         dicts['dim'] = 3
         dicts['PBC'] = [1, 1, 1]
         dicts['hn'] = self.wp.hall_number
         dicts['index'] = self.wp.index
         dicts['lattice'] = lattice.matrix
         dicts['lattice_type'] = lattice.ltype
         dicts['center'] = self.position
         if molecule.smile not in ["Cl-"]:
             dicts['orientation'] = np.array(ori)
             dicts['rotor'] = molecule.get_torsion_angles()
             dicts['reflect'] = reflect
+
         return mol_site.from_1D_dicts(dicts)
 
 class mol_site:
     """
     Class for storing molecular Wyckoff positions and orientations within
     the molecular_crystal class. Each mol_site object represenents an
     entire Wyckoff position, not necessarily a single molecule.
@@ -344,14 +363,15 @@
         orientation: an `Orientation <pyxtal.molecule.Oreintation.html>`_ object
         wp: a `Wyckoff_position <pyxtal.symmetry.Wyckoff_position.html>`_ object
         lattice: a `Lattice <pyxtal.lattice.Lattice>`_ object
         stype: integer number to specify the type of molecule
     """
 
     def __init__(self, mol, position, orientation, wp, lattice=None, stype=0):
+
         # describe the molecule
         self.molecule = mol
         self.wp = wp
         self.position = position # fractional coordinate of molecular center
         self.orientation = orientation #pyxtal.molecule.orientation object
         if isinstance(lattice, Lattice):
             self.lattice = lattice
```

### Comparing `pyxtal-0.6.5/pyxtal/wyckoff_split.py` & `pyxtal-0.6.6/pyxtal/wyckoff_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         group_type (string): 't' or 'k'
         elements: corresponding chemical species for each wp
     """
 
     def __init__(self, G=197, idx=None, wp1=[0, 1], group_type='t', elements=None):
         self.error = False
         self.elements = elements
-        if type(G) is int:
+        if type(G) in [int, np.int64]:
             self.G = sym.Group(G)  # Group object
         else:
             self.G = G
         self.group_type = group_type
         if group_type == 't':
             self.wyc = self.G.get_max_t_subgroup()
         else:
@@ -98,34 +98,34 @@
         self.elements = [self.elements[id] for id in ids]
 
 
     def parse_wp2(self, idx):
         """
         query the wp2 and transformation matrix from the given {G, H, wp1}
         """
-        #print("trans", idx)
         #print(self.wyc['transformation'])
         #subgroup_relations.reverse()
-        trans = self.wyc['transformation'][idx]
-        subgroup_relations = self.wyc['relations'][idx]
+        trans = self.wyc['transformation'][idx]#; print("trans", trans)
+        subgroup_relations = self.wyc['relations'][idx] #; print('subgroup_relations', subgroup_relations)
         subgroup_relations = list(reversed(subgroup_relations))
 
-        self.R = np.zeros([4,4])
-        self.R[:3,:3] += trans[:3,:3]
-        self.R[3,3] = 1
+        self.R = np.zeros([4, 4])
+        self.R[:3, :3] += trans[:3, :3]
+        self.R[3, 3] = 1
         self.inv_R = np.linalg.inv(self.R)
-        inv_t = np.dot(self.inv_R[:3,:3], trans[:,3].T)
-        self.inv_R[:3,3] = -1*inv_t.T
-        self.R[:3,3] = trans[:3,3]
+        inv_t = np.dot(self.inv_R[:3, :3], trans[:,3].T)
+        self.inv_R[:3, 3] = -1*inv_t.T
+        self.R[:3, 3] = trans[:3, 3]
         self.multi = np.linalg.det(self.R[:3, :3])
 
         wp2_lists = []
         for wp1_index in self.wp1_indices:
             wp2_list = []
             for letter in subgroup_relations[wp1_index]:
+                #if letter == '4a': letter = '8c'
                 id = sym.index_from_letter(letter[-1], self.H)
                 wp2_list.append(self.H[id])
             wp2_lists.append(wp2_list)
         self.wp2_lists = wp2_lists
         self.index=self.wyc['index'][idx]
         self.cosets=self.wyc['cosets'][idx]
         #import sys; sys.exit()
@@ -295,69 +295,74 @@
                     self.valid_split = False
                     self.error = True
                     return None, None
                 return self.split_t(new_wp1, wp2_lists, quadrant=quadrant)
         return G1_orbits, G2_orbits
 
 
-    def split_k(self, wp1, wp2_lists):
+    def split_k(self, wp1, wp2_lists, tol=1e-5):
         """
         split the generators in w1 to different w2s for k-subgroup
         """
 
         wp1_generators = [np.array(wp.as_dict()['matrix']) for wp in wp1]
 
         G1_orbits = []
         G2_orbits = []
-        quadrant=deepcopy(self.inv_R[:3,3])
-        quadrant[np.abs(quadrant)<1e-5] = 0 #finds the orientation of the subgroup_basis
+        quadrant = deepcopy(self.inv_R[:3, 3])
+        quadrant[np.abs(quadrant) < tol] = 0 #finds the orientation of the subgroup_basis
+
         for i in range(3):
-            if quadrant[i]>=0:
+            if quadrant[i] >= 0:
                 quadrant[i] = 1
             else:
                 quadrant[i] = -1
 
         all_g2_orbits = []
         translations = self.translation_generator()
+
         # the translation generator provides all the possible ways to translate
         # the starting positions, then they are shifted
         for translation in translations:
             for gen in wp1_generators:#into the proper orientation
                 orbit = np.matmul(self.inv_R,gen)
-                orbit[np.abs(orbit)<1e-5] = 0
-                orbit[np.abs(orbit-1)<1e-5] = 1
-                orbit[np.abs(orbit+1)<1e-5] = -1
+                orbit[np.abs(orbit) < tol] = 0
+                orbit[np.abs(orbit-1) < tol] = 1
+                orbit[np.abs(orbit+1) < tol] = -1
                 for i in range(3):
                     if quadrant[i] == 1:
                         orbit[i][3] += translation[i]
-                        orbit[i][3] = orbit[i][3]%1
-                        if np.abs(orbit[i][3]-1) < 1e-5:
+                        orbit[i][3] = orbit[i][3] % 1
+                        if np.abs(orbit[i][3]-1) < tol:
                             orbit[i][3] = 0
                     else:
                         orbit[i][3] += (translation[i])%-1
-                        orbit[i][3] = orbit[i][3]%-1
-                        if np.abs(orbit[i][3]) < 1e-5:
+                        orbit[i][3] = orbit[i][3] % -1
+                        if np.abs(orbit[i][3]) < tol:
                             orbit[i][3] = -1
                 all_g2_orbits.append(orbit)
 
         for wp2 in wp2_lists:
 
             #final_G2=[]
             temp = np.array(deepcopy(all_g2_orbits))
-            temp[np.abs(temp) <1e-5] = 0
+            temp[np.abs(temp) < tol] = 0
             temp = temp.tolist()
 
             for j, x in enumerate(temp):
                 temp[j] = SymmOp(x)
 
             for orbit in temp:
                 try_match = np.array([np.matmul(x.as_dict()['matrix'], orbit.as_dict()['matrix']) for x in wp2])
-                try_match[np.abs(try_match) <1e-5] = 0
-                try_match[np.abs(try_match-1) <1e-5] = 1
-                try_match[np.abs(try_match+1) <1e-5] = -1
+                try_match[np.abs(try_match) < tol] = 0
+                try_match[np.abs(try_match-1) < tol] = 1
+                try_match[np.abs(try_match+1) < tol] = -1
+
+                #print('\norbit\n', orbit)
+                #print('\ntry_match\n', try_match)
 
                 for j in range(len(try_match)):
                     for k in range(3):
                         try_match[j][k][3] = try_match[j][k][3]%quadrant[k]
                         if try_match[j][k][3] == 0 and quadrant[k] == -1:
                             try_match[j][k][3]=-1
                 try_match=try_match.tolist()
@@ -381,25 +386,28 @@
         for position in G2_orbits:
             final_G1 = []
             for orbit in position:
                 final_G1.append(SymmOp(np.matmul(self.R,orbit.as_dict()['matrix'])))
             G1_orbits.append(final_G1)
 
         if len(G1_orbits) != len(wp2_lists):
-            raise ValueError('inaccurate')
+            print('wp2_lists', wp2_lists)
+            print('G1_orbits', G1_orbits)
+            print('G2_orbits', G2_orbits)
+            raise ValueError('inconsistent G1_orbits and wp2_lists')
         else:
             return G1_orbits, G2_orbits
 
     def translation_generator(self):
         """
         a function to handle the translation during lattice transformation
         """
         modulo = round(np.linalg.det(self.R[:3,:3]))
         inv_rotation = np.array(self.inv_R[:3,:3])*modulo
-        subgroup_basis_vectors = (np.round(inv_rotation.transpose()).astype(int)%modulo).tolist()
+        subgroup_basis_vectors = (np.rint(inv_rotation.transpose()).astype(int)%modulo).tolist()
 
         # remove the [0,0,0] vectors
         translations = [x for x in subgroup_basis_vectors if x!=[0,0,0]]
 
         #find the independent vectors
         if len(translations) == 0:
             independent_vectors = [[0,0,0]]
@@ -410,15 +418,15 @@
             inner_product = np.inner(translations[0],translations[1])
             difference=norm-inner_product
             if difference == 0.:
                 independent_vectors = [translations[0]]
             else:
                 independent_vectors = translations
         else:
-            norms=np.round([np.linalg.norm(translations[i])*np.linalg.norm(translations[j]) for i in range(2) for j in range(i+1,3)])
+            norms=np.rint([np.linalg.norm(translations[i])*np.linalg.norm(translations[j]) for i in range(2) for j in range(i+1,3)])
             inner_products = np.array([np.inner(translations[i],translations[j]) for i in range(2) for j in range(i+1,3)])
             differences = inner_products - norms
             independent_vectors=[translations[0]]
             if differences[0]!=0. and differences[1]==0.:
                 independent_vectors.append(translations[1])
             elif differences[0]==0. and differences[1]!=0.:
                 independent_vectors.append(translations[2])
@@ -485,17 +493,22 @@
     if len(mat2) == 0:
         return False
     else:
         for mat in mat2:
             if np.array_equal(mat[:3,:3], mat1[:3,:3]):
                 diffs = np.abs(mat[:3,3] - mat1[:3,3])
                 if PBC:
-                    diffs -= np.floor(diffs)
+                    diffs -= np.rint(diffs)
                 #print("diffs", diffs)
-                if (diffs*diffs).sum() < eps:
+                if (diffs**2).sum() < eps:
                     return True
         return False
 
 if __name__ == "__main__":
 
-    sp = wyckoff_split(G=14, idx=1, wp1=['2c', '4e'], group_type='t')
-    print(sp)
+    #sp = wyckoff_split(G=14, idx=1, wp1=['2c', '4e'], group_type='t')
+    #print(sp)
+    for idx in range(4):
+        #sp = wyckoff_split(G=210, idx=idx, wp1=['8b'], group_type='k')
+        sp = wyckoff_split(G=224, idx=idx, wp1=['24j'], group_type='k')
+        #print(sp)
+        print(sp.error)
```

### Comparing `pyxtal-0.6.5/pyxtal.egg-info/PKG-INFO` & `pyxtal-0.6.6/pyxtal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <=3.12
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: spglib>=1.10.4
 Requires-Dist: pymatgen>=2024.3.1
 Requires-Dist: pandas>=2.0.2
 Requires-Dist: networkx>=2.3
 Requires-Dist: ase>=3.18.0
```

### Comparing `pyxtal-0.6.5/pyxtal.egg-info/SOURCES.txt` & `pyxtal-0.6.6/pyxtal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/scripts/pyxtal_main.py` & `pyxtal-0.6.6/scripts/pyxtal_main.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/scripts/pyxtal_symmetry.py` & `pyxtal-0.6.6/scripts/pyxtal_symmetry.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.5/setup.py` & `pyxtal-0.6.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,10 +53,10 @@
         #'pyshtools>=4.10.3',
         #"openbabel>=3.0.0",
     ],
     extra_require={
         'visualization': ["py3Dmol>=0.8.0"],
         'descriptor': ["pyshtools>=4.10.3"],
         },
-    python_requires=">=3.7, <=3.12", #add the restriction for now issue #189
+    python_requires=">=3.7",
     license="MIT",
 )
```

